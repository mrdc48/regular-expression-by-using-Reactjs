# regular-expression-by-using-Reactjs

``` JavaScript

function App (){
  let [content,setContent] = useState({ background:"blue", text:"number is must"})
   
   Hello = (e) => {
     var reg = /^[6-9]{1}[0-9]{9}$/
     if (reg.test(e.target.value)) {
       setContent({
         background: "green",
         text: "varified mobile number"
       })
     } 
     else {
       setContent({
         background: "red",
         text : "invalid mobile number"
       })
     }
   }
  return(
   <>
    <p style={{background: content.background, padding: "8px", textAlign: "center",color:"#fff"}}> {content.text}</p>
    <input style={{marginLeft: "50px", padding: "8px"}}type={"number"} placeholder={" enter number"} onKeyUp={(event) => {
      Hello (event)}}/>
   </>
    
    )
}
export default App;

```
