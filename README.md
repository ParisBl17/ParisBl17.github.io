body {
  font-family:Baskerville, "Palatino Linotype", Palatino, "Century Schoolbook L", "Times New Roman", "serif";
	font-size:20px;
  background: #f4f4f9;
  color: #333;
  display: flex;
  flex-direction: column;
  min-height: 100vh;
}

header {
  background-color: #8a2be2;
	font-size:40px;
  color: white;
  padding: 1rem;
  text-align: center;
}

.container {
  display: flex;
  flex: 1;
}

.sidebar {
  width: 250px;
  background:#260438; 
  padding: 1rem;
  display: flex;
  flex-direction: column;
	
}

.sidebar button {
  background: none;
  border: none;
  color: white;
  padding: 1rem;
  margin-bottom: 0.5rem;
  cursor: pointer;
  font-size:25px;
  transition: background 0.3s;
  text-align: left;
}

.sidebar button:hover {
  background: #4b0082;
	
	
}

main {
  flex: 1;
  display: flex;
  justify-content: center;
  align-items: flex-start;
  padding: 2rem;
}

.content {
  display: none;
  max-width: 800px;
  text-align: justify;
  background: white;
  padding: 2rem;
  border-radius: 10px;
  box-shadow: 0 2px 10px rgba(0,0,0,0.1);
  line-height: 1.6;
}

.content.active {
  display: block;
}

h2 {
  text-align: center;
  color: #8a2be2; 
}

footer {
  text-align: center;
  padding: 1rem;
  background: #8a2be2; 
  color: white;
}

@media (max-width: 768px) {
  .container {
    flex-direction: column;
  }

  .sidebar {
    width: 100%;
    flex-direction: row;
    justify-content: center;
    flex-wrap: wrap;
	  
  }

  .sidebar button {
    flex: 1 1 auto;
    text-align: center;
    margin: 0.5rem;
	  
  }

  main {
    padding: 1rem;
  }

  .content {
    padding: 1rem;
  }
}
