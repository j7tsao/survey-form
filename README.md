<<<<<<< HEAD
# Survey Form
* freeCodeCamp "Responsive Web Design" Project - [Survey Form](https://www.freecodecamp.org/learn/responsive-web-design/responsive-web-design-projects/build-a-survey-form/)
* It meets all the project requirements
* The page could be seen [here](https://codepen.io/yuchit/full/abNLawa)
=======
<html>
<head>
<title>Watashi Ice Cream Shop Survery</title>
<meta name="viewport" 
      content="width=device-width, initial-scale=1.0" 
      charset="UTF-8">
<style>
  :root {
  font-size: 10px;
  }
  * {
    box-sizing: border-box;
  }

  #title {
    font-size: 2.5rem;
    text-align: center;
    position: relative;
    margin-top: 0;
    margin-bottom: 0.5rem;
  }

  body {
    font-family: "Arial", "Helvetica";
    font-size: 2rem;
    font-weight: bold;
    line-height: 1.2em;
  }

  body::before {
    content:"";
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    z-index: -1;
    background-image:
      linear-gradient(
        120deg,
        rgba(158, 158, 158, 0.6),
        rgba(220, 220, 220, 0.7)
      ),
      url("https://cdn.britannica.com/s:700x500/50/80550-050-5D392AC7/Scoops-kinds-ice-cream.jpg");
    background-repeat: no-repeat;
    background-size: cover;
  }

  #description {
    text-align: center;
    line-height: 1.2;
    position: relative;
    font-style: oblique;
    color: hsla(0, 100%, 30%, 0.8);
  }

  .formblock {
    width: 100%;
    margin: 3.125rem auto 0 auto;
  }

  @media (min-width: 576px) {
    .formblock {
      max-width: 540px;
    }
  }

  @media (min-width: 768px) {
    .formblock {
      max-width: 720px;
    }
  }

  form {
    left: 0%;
    top: 2rem;
    background-color: #eee;
    opacity: 0.7;
    border-radius: 5px;
    margin: 3.5rem auto 0 auto;
    padding: 2.5rem 2.625rem;
  }
  @media (min-width: 480px) {
    form {
      padding: 2.5rem;
    }
  }

  .form-cell {
    margin: 0 auto 1.25rem auto;
    padding: 0.25rem;
  }

  label {
    display: flex;
    align-items: center;
    margin-bottom: 0.5rem;
  }

  .input-radio,
  .input-checkbox {
    display: inline-block;
    margin-right: 0.65rem;
    min-height: 1.25rem;
    min-width: 1.25rem;
  }

  input,
  button,
  select,
  textarea {
    margin: 0;
    font-family: inherit;
    font-size: inherit;
    line-height: inherit;
  }

  .form-fashion{
    height: 3.5rem;
    width: 100%;
    border-radius: 5px;
    border: 0px solid gray;
  }

  .textarea-fashion {
    font-size: 1.2rem;
    width: 100%;
    min-height: 20rem;
    border-radius: 5px;
    border: 0px solid gray;
    padding: 0.65rem;
    resize: vertical;
  }

  #submit {
    color: white;
    text-align: center;
    width: 100%;
    padding: 1em;
    background: red;
    font-weight: bold;
    border: 0px solid gray;
    border-radius: 4px;
    cursor: pointer;
  }
</style>
</head>
<body>
  <div class="formblock">
    <header class="header">
      <h1 id="title">
        Watashi Ice Cream Shop Survey
      </h1>
      <p id="description">
        Thank you for the supports to Watashi Ice Cream Shop. 
        We would like to learn more about your tastes from this survey.
      </p>
    </header>
    <form id="survey-form" action="#">
      <div class="form-cell">
        <label for="name" id="name-label">Name</label>
        <input type="text" 
               id="name" 
               name="name" 
               placeholder="Enter your name" 
               class="form-fashion"
               required>
      </div>
      <div class="form-cell">
        <label for="email" id="email-label">Email</label>
        <input type="email" 
               id="email" 
               name="email" 
               placeholder="Enter your email"
               class="form-fashion"
               required>
      </div>
      <div class="form-cell">
        <label for="age" id="age-label">How old are you?</label>
        <input type="number"
               id="number"
               name="age"
               min="7"
               max="100"
               class="form-fashion"
               placeholder="Age">
      </div>
      <div class="form-cell">
        <label for="number" id="number-label">Cell/Phone</label>
        <input type="tel" 
               id="phone" 
               name="phone" 
               placeholder="Enter your cell; 123-456-7890"
               class="form-fashion"
               pattern="[0-9]{3}-[0-9]{3}-[0-9]{4}"
               required>
      </div>
      <div class="form-cell">
        <label for="male" id="male-label">
            <input type="radio"
                   id="male"
                   name="gender"
                   class="input-radio"
                   value="male">
                   Male
        </label>
        <label for="female" id="female-label">
          <input type="radio"
                 id="female"
                 name="gender"
                 class="input-radio"
                 value="female">
          Female</label>
      </div>
      <div class="form-cell">
        <label for="dropdown" id="dropdown-label">What is your favorite flavor?</label>
        <select id="dropdown" name="favorite" class="form-fashion">
            <option value="chocolate">Chocolate</option>
            <option value="vailla">Vanilla</option>
            <option value="mint">Mint</optipn>
            <option value="almond">Almond</option>
            <option value="bluberry">Blueberry</option>
            <option value="caramel apple">Caramel Apple</option>
            <option value="banana coconut">Banana Cocont</option>
            <option value="cheesecake">Cheesecake</option>
        </select>
      </div>
      <div class="form-cell">
        <p id="freqq">How often do you have ice cream? (Check all the apply)</p>
        
        <label for="freq1" id="freq1-label">
          <input type="checkbox" 
                 id="freq1" 
                 name="freq1"
                 class="input-checkbox"
                 value="half day">
          Once half a day</label>
        <label for="freq2" id="freq2-label">
          <input type="checkbox" 
                 id="freq2" 
                 name="freq2" 
                 class="input-checkbox"
                 value="everyday">
          Everyday</label>
        <label for="freq3" id="freq3-label">
          <input type="checkbox" 
                 id="freq3" 
                 name="freq3"
                 class="input-checkbox"
                 value="every week">
          Every Weeek</label>
        <label for="freq4" id="freq4-label">
          <input type="checkbox" 
                 id="freq4" 
                 name="freq4"
                 class="input-checkbox"
                 value="twice a week">
          Twice A Week</label>
    </div>
    <div class="form-cell">
        <p>Leave us a message or comment if you like:</p>
        <textarea id="message" 
                  name="message"
                  class="textarea-fashion"
                  placeholder="Write your message here...">
        </textarea>
    </div>
    <div class="form-cell">
      <button type="submit" id="submit" class="submit-button">
        Submit
      </button>
    </div>
  </form>
</div>
</body>
</html>
>>>>>>> 85a21c8a0cefc8fab4f2eb23c23c0eb18d253838
