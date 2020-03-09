# FreeCodecamp-Learning
Survey form code

<!DOCTYPE html>
<html>
<title>Survey form</title>
<link href="stylesheet.css" rel="stylesheet" type="text/css">
<body>

<div class="container">
  <header class="header">
    <h1 id="title" class="text-center">Booming Survey Form</h1>
    <p id="description" class="description text-center">
      Please Fill all of the information on the blank column to improve our management
    </p>
  </header>
  <form id="survey-form">
    <div class="form-group">
      <label id="name-label" for="name">Name</label>
      <input
            type="text"
            name="name"
            id="name"
            class="form-control"
            placeholder="Enter Your Name"
            required
            />
        </div>
    <div class="form-group">
      <label id="email-label" for="email">Email</label>
      <input
             type="text"
             name="email"
             id="email"
             class="form-control"
             placeholder="enter Your Email"
             required
             />
    </div>
    <label id="age-label" for"age">Age</label>
    <input
           type="text"
           name="age"
           id="age"
           min="10"
           max="20"
           class="form-control"
           placeholder="Age"
           />
    </div>
      <div class="form-group">
        <p>Choose which semester are you studying</p>
        <select id="dropdown" name="role" class="form-control" required>
          <option disabled selected value>Select Current Semester</option>
          <option value="1th semester">1th Semester Student</option>
          <option value="2th semester">2th Semester Student</option>
          <option value="3th semester">3th Semester Student</option>
          <option value="4th semester">4th Semester Student</option>
          <option value="5th semester">5th Semester Student</option>
          <option value="6th semester">6th Semester Student</option>
          <option value="7th semester">7th Semester Student</option>
          <option value="8th semester">8th Semester Student</option>
        </select>
  </div>
  
  <div class="form-group">
    <p>Would you recommend your friend to play in booming games?</p>
    <label>
      <input
         name="user-recommend"
         value="definitely"
         type="radio"
         class-"input-radio"
         checked
         >Definitely</label>
     <label>
      <input
         name="user-recommend"
         value="maybe"
         type="radio"
         class-"input-radio"
         >Maybe</label>
      <label>
      <input
         name="user-recommend"
         value="not-sure"
         type="radio"
         class-"input-radio"
         checked
         >Not Sure</label>
    
     <div class="form-group">
        <p>Choose which things you like the most about booming games</p>
        <select id="dropdown" name="mostlike" class="form-control" required>
          <option disabled selected value>Select an option</option>
          <option value="services">Services</option>
          <option value="high quality games">High Quality Games</option>
          <option value="price">Price</option>
        </select>
  </div>
    
  <div class="form-group">
    <p>
      What Would you like to see improved?
   </p>
    
   <label>
     <input
        name="prefer"
        value="services"
        type="checkbox"
        class="input-checkbox"
        />Services</label>
    
    <label>
      <input
        name="prefer"
        value="graphics-quality"
        type="checkbox"
        class="input-checkbox"
        />Graphics-quality</label>
    <label>
      <input
        name="prefer"
        value="cheaper-price"
        type="checkbox"
        class="input-checkbox"
        />Cheaper Prize</label>
     <label>
      <input
        name="prefer"
        value="additional-games"
        type="checkbox"
        class="input-checkbox"
        />Additional-games</label>
    </div>
    
    <div class="form-group">
      <p>Any Feedback or Suggestion</p>
      <textarea
        id="comments"
        class-"input-textarea"
        name="comment"
        placeholder="Enter your comment here.."
        ></textarea>
    </div>
    
    <div class="form-group">
      <button type="submit" id="submit" class="submit-button">
        Submit
      </button>
    </div>
   </form>
</div>

</body>
</html>
  
 
@import url('https://fonts.googleapis.com/css?family=Poppins:200i,400&display=swap');

:root {
  --color-white: #f3f3f3;
  --color-darkblue:  #1b1b32;
  --color-darkblue-alpha: rgba(27, 27, 50, 0.8);
  --color-green: #37af65;
}

*,
*::before,
*::after {
  box-sizing: border-box;
}

body {
  font-family: 'Poppings', sans-serif;
  font-size: 1rem;
  font-weight: 400;
  line-height: 1,4;
  color: var(--color-white);
  margin: 0;
}

body::before {
  content: '';
  position: fixed;
  top: 0;
  left: 0;
  height: 100%;
  width: 100%;
  z-index: -1;
  background: var(--color-darkblue);
  background-image: linear-gradient(115deg,
      rgba(58, 58, 158, 0.8),
      rgba(136, 136, 206, 0.7)
    ),
    url(https://cdn.freecodecamp.org/testable-projects-fcc/images/survey-form-background.jpeg);
  background-size: cover;
  background-repeat: no-repeat;
  background-position: center;
}

h1 {
  text-align: center;
  font-weight: 400;
  line-height: 1.2;
}

p {
  font-size: 1.2rem;
}

h1, 
p {
  margin-top: 0;
  margin-bottom: 0,5rem;
}

label {
  display: flex;
  text-align: center;
  font-size: 1.125rem;
  margin-bottom: 0.5rem;
}

input,
button,
select,
text-area {
  margin: 0;
  font-family: inherit;
  font-size: inherit;
  line-height: inherit;
}

button {
  border: none;
}

.container {
  width: 100%;
  margin: 2rem;
}

@media (min-width: 576px) {
  .container {
    max-width: 550px;
  }
}

@media (min-width: 770px) {
  .container {
    max-width: 720px;
  }
}

.header {
  padding: 0 0.625rem;
  margin-bottom: 2rem;
}

.description {
  font-style: italic;
  font-weight: 200;
  text-shadow: 1px 1px 1px rgba(0, 0, 0, 0.4);
}

.clue {
  margin-left: 0.25rem;
  font-size: 1rem;
  color:  #e4e4e4;
}

.text-center {
  text-align: center;
}

form {
  background: var(--color-darkblue-alpha);
  padding: 2.5rem 0.625rem;
  border-radius: 0.25rem;
}

@media (min-width: 480px) {
  form {
    padding: 2.5rem;
  }
}

.form-group {
  margin: 0 auto 1.25rem auto;
  padding: 0.25rem;
}
 
.form-control {
  display: block;
  width: 100%;
  height: 2.375rem;
  padding: 0.375rem 0.75rem;
  color: #495057;
  background-color: #fff;
  background-clip: padding-box;
  border: 1px solid #ced4da;
  border-radius: 0.25rem;
  transition: border-color 0.15s ease-in-out, box-shadow 0.15s ease-in-out;  
}

.form-control: focus {
  border-color: #80bdff;
  outline: 0;
  box-shadow: 0 0 0 0.2rem rgba(0, 123, 255, 0.25);
}

.input-radio
.input-checkbox {
  display: inline-block;
  margin-right: 0.625rem;
  min-height: 1.25rem;
  min-width: 1.25rem;
}

.input-textarea {
  min-height: 120px;
  width: 100%;
  padding: 0.625rem;
  resize: vertical;
}

.submit-button {
  display: block;
  width: 100%;
  padding: 0.75rem;
  background: var(--color-green);
  color: inherit;
  border-radius: 2px;
  cursor: pointer;
}
    
         
          
