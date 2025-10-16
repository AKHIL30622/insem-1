
import React from 'react';

function Welcome(props) {
  return <h2>Welcome, {props.name}!</h2>;
}

export default Welcome;
 
import React from 'react';
import Welcome from './Welcome';

function App () {
  const students = ['Deepak', 'Akhil', 'Priya', 'Rahul'];

  return (
    <div style={{ padding: 20 }}>
      <h1> Student Dashboard </h1> 
      {students.map((student, index) => (
        <Welcome key={index} name={student} />
      ))}
    </div>
  );
}

export default App;
