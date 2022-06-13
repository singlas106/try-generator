# try-generator

import React, { useEffect, useState } from 'react';
// import './App.css';

const App = () => {
  const [name, setName] = useState('');
  const [email, setEmail] = useState('');
  const [password, setPassword] = useState('');

  useEffect(() => {
    // console.log("name", name);
    // console.log("email", email);
    // console.log("password", password);
  })

  return(
    <div>
      <form className='tc bg-light-green '>
           <label>
            Name:<input type="text" name="name" onChange={(e) => setName(e.target.value)} />
           </label> <br/> 
           {/* <input type="submit" value="Submit" /> <br/>  */}
           <label> 
            Email:<input type="email" name="email" onChange={(e) => setEmail(e.target.value)} />
          </label> <br/> 
           {/* <input type="submit" value="Submit" /> <br/> */}
           <label>
            DOB:<input type="date" name="dob" />
          </label> <br/>
          <label>
            password: <input type="password" required onChange={(e) => setPassword(e.target.value)} />
          </label>
          <button onClick={() => console.log(name, email)}>submit</button>
      </form>
    </div> 
       
  )
}
export default App;

import React, { useEffect, useState } from 'react';
// import './App.css';

const App = () => {
  const [state, setState] = useState({count: 0, number: 0})

  

  return(
    <div>
      <p>u clicked {state.count} times </p>
      {/* <p>u won {number} times </p> */}
      <button onClick={() => setState({...state, count: state.count +1})}>Click me</button>
      {/* <button onClick={() => setNumber(number + 1)}>winnning streak!!</button> */}
    </div>
  )
}


export default App;
// const [count, setCount] = useState(0);
    // const [number, setNumber] = useState(0);
  

return(
    <div>
      <p>u clicked {count} times </p>
      <p>u won {number} times </p>
      <button onClick={() => setState({count +1})}>Click me</button>
      <button onClick={() => setNumber(number + 1)}>winnning streak!!</button>
    </div>
  )
}
