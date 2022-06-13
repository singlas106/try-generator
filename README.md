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
