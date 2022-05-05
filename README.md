# CRM
Clone 

Final Code 
https://github.com/kubowania/monday-crm-clone 
https://github.com/kubowania/monday-crm-clone/tree/main/public
https://github.com/kubowania/monday-crm-clone/tree/main/src



https://raw.githubusercontent.com/RodrigoMvs123/CRM/main/README.md

https://github.com/RodrigoMvs123/CRM/blame/main/README.md


R:  Microsoft Original Documentation 
https://docs.microsoft.com/en-us/dotnet/api/microsoft.xrm.tooling.connector.crmserviceclient.clone?view=dataverse-sdk-latest  
https://docs.microsoft.com/en-us/power-apps/developer/data-platform/xrm-tooling/use-crmserviceclient-constructors-connect
https://docs.microsoft.com/en-us/power-apps/developer/data-platform/xrm-tooling/sample-tpl-crmserviceclient

🛑 Build a Monday CRM Clone with GET POST PUT DELETE Requests | React + NodeJS + useContext Hook 

To Build a CRM Clone with “GET”, “POST”, “PUT”, “DELETE”, Requests | React + NodeJS + useContext, Hook.

Final Code: https://github.com/kubowania/monday-crm-clone 

https://auth.cloud.datastax.com/auth/realms/CloudUsers/protocol/openid-connect/registrations?client_id=auth-proxy&response_type=code&scope=openid+profile+email&redirect_uri=https://astra.datastax.com/welcome&utm_source=youtube&utm_medium=referral&utm_campaign=ania-kubow&utm_term=frontend-devplay&utm_content=monday-crm-clone 





To Add 
New Project 
React 
Package.json
[
Script 
]

1 - // To Delete 
Index JS File 
JS File 
To Delete 
Line 01 // Logo 
Function 
Const 
To Delete 
To Delete // Header 
To Delete 
Index.Css File 


2- // Context.js
Project 
Clone 
SRC // Source Directory 
                    New / Directory 
JavaScript File 
context.js
import {createContext} from “react”
const CategoryContexts = createContext ({
categories=null,
setCategories: () => {]
})
export default CategoriesDefault
New JavaScript File 


3 - // AvatarDisplay Component 
Import blankAvatar from '../ images / blank-profile-avatar.png ' 
const AvatarDisplay = ( { ticket } ) = > {
   return (
<div> className = "avatar-container" 
<div className = "image-conteiner">
<image src = { ticket.avatar ? ticket.avatar: blankaAvatar  } alt = { ' photo of ' + ticket owner } />
</div>
</div> 
)
}
export default AvatarDisplay 
// - Image Directory 
            Components 
New 
New JavaScript File 


4 - // DeleteBlock Component 
import axios from ‘axios’
const DeleteBlock = (documentId ) = > {
const response await axios.delete(‘http://localhost:8000/tickets/${documentId}/’)
const success =  response.status == 200  
if (success) window.location.reload()
const deleteticket = async () => {
}
return ( 
<div className =”delete-block” >
<div> className”delete-icon” onClick {deleteticket}  </div>
</div>
 )
}
export default DeleteBlock 
            Components 
New 
New JavaScript File 
            Components 
New 
New JavaScript File 


5 - // Nav Component 
import logo from ‘../import/crm-logo-png’ 
import { useNavigate } from ‘react-router-dom
const = Nav () => {
const navigate = useNavigate () 
   return (
<nav>
<div classname = “logo-conteiner”>
<div calssName = “controls-conteiner”> 
<div className= “ icon ”onClick  = { () => navigate (‘/ticket’ )} >+</div>
<div className= “ icon ”onClick  = { () => navigate (‘/ticket’ )} > << </div>
<div className= ” icon ”></div>
</div>
<img src ( logo ) alt = “logo”/> 
</nav>
)
}
export default Nav.js

 
6 - // PriorityDisplay Component 
const PriorityDisplay = ( { priority } ) = > {
   return (
<div className=”priority-display”>
<div className=”star-container” >
<h3 style={{ color: priority }  }> =1 ? ‘rgb(253, 253, 150)’ : ‘ ‘ } } >☆<h3/>
<h3 style={{ color: priority }  }> =2 ? ‘rgb(253, 253, 150)’ : ‘ ‘ } } >☆<h3/>
<h3 style={{ color: priority }  }> =3 ? ‘rgb(253, 253, 150)’ : ‘ ‘ } } >☆<h3/>
<h3 style={{ color: priority }  }> =4 ? ‘rgb(253, 253, 150)’ : ‘ ‘ } } >☆<h3/>
<h3 style={{ color: priority }  }> =5 ? ‘rgb(253, 253, 150)’ : ‘ ‘ } } >☆<h3/>
</div>
</div> 
)
}
export default PriorityDisplay
Components 
New 
New JavaScript File 
            

7 - // ProgressDisplay Component 
const ProgressDisplay = ( { progress } ) = > {
   return (
<div className=”progress-display”>
<div>className=”progress-bar”</div>
<div>
style={{ witdh:progress + ‘%’ }}
className=”progressindicator”
</div>
</div> 
</div>
)
}
export default ProgressDisplay 
            Components 
New 
New JavaScript File 


8 - // StatusDisplay Component 
  const StatusDisplay  = ( { status  } ) =>  {
const getColor = ( status ) = > 
let color
switch = ( status ) {
case ‘done’:
color: ‘rgb ( 186, 255, 201 )’  
break 
case ‘working on it’:
color = color ‘ rgb ( 255, 223, 186 )’ 
break
case: ‘stuck’ : 
color = ‘ rgb ( 255, 179, 186 )’ 
break
default: 
color: ‘ rgb ( 186, 255, 255 )’ 
}
return color 
  }
return ( 
<div>className=”status-display” style= {{ backgroundcolor: getColor(status)}} 
{ status }
<div/>
)
} 
Components 
New 
New JavaScript File 


9 - // TicketCardjs. Component 
import { Link } from ‘react-from-dom’ 
import AvatarDisplay from “/.AvatarDisplay”
import StatusDisplay from “/.StatusDisplay”
import PriorityDisplay from “/.PriorityDisplay”
import ProgressDisplay from “/.ProgressDisplay” 
import DeleteBlock from “/.DeleteBlock”  
const TicketCard = ( { color, filteredTicket } ) = > {
   return (
<div className = “ticket-card”>
<link to={'/ticket/${ticket.documentId' } }
id = " link " >   
 <div> className= “ ticket color ” style= {{backgroundColor: color}}> </div>
<h3>filteredTicket.title</h3>
<AvatarDisplay ticket={ticket}/>
<StatusDisplay status:{ticket.status}/>
<PriorityDisplay priority={ticket.priority}/>
<ProgressDisplay priority=”ticket.progress”/>
 <link/>
<DeleteBlock documentId = {ticket documentId}/>
</div> 
)
}



export default TicketCard.js 
Pages 
New 
New JavaScript File 

  
10 - // Dashboard Component 
const Dashboard = ( ) {
   return (
<div>Dashboard</div> 
)
}
export default Dashboard  
Pages 
New 
New JavaScript File 

  
11 - // TicketPage Component 

import { use State, useContex, useEffect } from ‘react’
import {useNavigate, useParams} from ‘react-router ’
import axios from ‘axios’
import CategoriesContex from ‘../context’
 const TicketPage = ({editMode} ) = > {
const {fromData, setFormData = useState (
status: ‘not started’ ,
progress: 0;
category: categories[0],
timestamp: new: new Date (). toISOString () 
) }
const {categories, setCategories} = useContex (CategoriesContex) 
const navigate = useNavigate () 
let { id } = useParams ()
const handleSubmit = sync (e) = > {
e.preventDefault () 
if (editMode) {
const response = await axios.put(‘http://localhost:8000/tickets/${id}’ {
data:formData
})
const success = response.status === 200
if (success) 
navigate {‘/’}
}
}
if ( !editmode ) {
const response = await axios.post (‘https://localhost:8000/tickets’,
{  
formData
})
 const success = response.status === 200
if (success) 
navigate {‘/’}
}
}
}
const fetchData = () => async {
const response = await axios.get(‘http://localhost:8000/tickets/${id}’)
setFormData(response.data.data)
}
use effect (()) => {
if (editMode) fetchData()
}, [])
const handleChange = () = > {
const value = e.target.value
const name = e.target.name
setFormData ((prevState) = > ({
…prevState,
[name]: value
})
)
}
{ editMode && 
<> 
<input 
   type = “ range ”
   id = “progress”
   name = “progress”
   value= {formData.progress}
   min=”0”
   max=”100”
   onChange={handleChange}
/>
<label htmlFor=”progress” >Progress</label>
<label>Status</label>
<select
name=”status”
value={formData.status}
onChange={habdleChange}
>
<option selected = {formData.status === ‘done’} value=’done’>Done</option>
<option selected = {formData.status === ‘working on it’} value=’working on it’>Working on it</option>
<option selected = {formData.status === ‘stuck’} value=’stuck’>Stuck</option>
<option selected = {formData.status === ‘not started’} value=’not started’>Not Started</option>
</select> 
</>
}
<input type=”submit”/>
</section>
<section>
<label htmlFor =”owner”=Owner></label>
<input
id=”owner”
name=”owner”
type=”text”
onChange={handleChange}
required={true}
value={form.Data.owner}
/>
<label htmlFor =”avatar”=Avatar></label>
<input
id=”avatar”
name=”avatar”
type=”url”
onChange={handleChange}
required={true}
value={form.Data.avatar}
/>
<div class name=”img-preview”>
{formData.avatar && )
<img src= {form.Data.avatar} alt= “img-preview”/>
)}
</div>
</section>
</form>
</div>
</div>
)
}
console.log (formData) 
return (
<div className “ticket”>
<h1> { editMode ? ‘ Update your Ticket’ : Create a Ticket } </h1>
</div> 
<div className=”ticket-conteiner”> 
<form onSubmit={handleSubmit}>
<section> 
<label htmlFor=”title”>Title</label> 
<input
id=”title”
name=”title”
type=”text”
onChange={handleChange}
required={true}
value={form.Data.title}
/>
<label htmlFor=”description”>Description</label> 
<input
id=”description”
name=”description”
type=”text”
onChange={handleChange}
required={true}
value={form.Data.description}
/>
<label>Category</label>
<select
name=”category”
value = {formData.category I I ‘New Category’}
onChange=hendlecategory
>
categories? .map ( category, _index) => (
<option key={_index} value={category}></option>
))}
</select>
<label htmlFor=”new-category”>New Category</label> 
<input
id=”new-category”
name=”category”
type=”text”
onChange={handleChange}
value={form.Data.category}
/>
<label>Priority</label>
<label htmlFor=”priority-1”>1</label>
<div className=”multiple-input-container”>
<input
id”priority-1”
name=”priority”
type=”radio” 
onChange= {handleChange}
value={1}
checked={formData.priority ===1 }
/>
label htmlFor=”priority-1”>1</label>
<label>Priority</label>
<label htmlFor=”priority-1”>1</label>
<div className=”multiple-input-container”>
<input
id”priority-2”
name=”priority”
type=”radio” 
onChange= {handleChange}
value={2}
checked={formData.priority ===2 }
/>
<label>Priority</label>
<label htmlFor=”priority-2”>2</label>
<div className=”multiple-input-container”>
<input
id”priority-3”
name=”priority”
type=”radio” 
onChange= {handleChange}
value={1}
checked={formData.priority === }
/>
<label>Priority</label>
<label htmlFor=”priority-3”>3</label>
<div className=”multiple-input-container”>
<input
id”priority-4”
name=”priority”
type=”radio” 
onChange= {handleChange}
value={4}
checked={formData.priority ===4 }
/>
<label>Priority</label>
<label htmlFor=”priority-4”>4</label>
<div className=”multiple-input-container”>
<input
id”priority-5”
name=”priority”
type=”radio” 
onChange= {handleChange}
value={5}
checked={formData.priority ===5 }
/>
<label htmlFor=”priority-5”>5</label>
</div>
export default TicketPage 
Pages 
New 
New JavaScript File 

  
12 - // Appjs. 
Terminal 
npm i react - router - dom 
// App.js 
import { BrowserRouter, Route, Routes } from ‘ react - router - dom ’ // package.json
const Class Name = ( ) {
   return (
<div>App</div> 
)
}
export default App
//
 SoftWare Version 
 package.json
“ react - router - dom ”: “ 6.2.2 ”,  
“ react - router - dom  ”: “ 6.2.1 ”, 
Terminal 
To Change SoftWare Version 
npm i 

  
13 - //App.js
import { BrowserRouter, Route, Routes } from ‘ react - router - dom ’ // package.json
import { useState } from ‘react’
import Nav from ‘ ./ components / Nav ’
import Dashboard from ‘ ./ pages/Dashboard ’ 
import TicketPage from ‘ ./ pages/TicketPage ’
import CategoriesContext from ‘../context’
const app => ( ) {
const [categories, setCategories] = useState(null)   
const value = { categories, setCategories } 
return (
< div class Name = “ app ” > 
<CategoriesContext,Provider value = {value}>
<BrowserRouter>   
   <Nav/> 
   <Routes>
      <Route path = ‘ / ’ element = {<Dashboard>}/> 
      <Route path = ‘ / ticket ’ element = {<TicketPage>}/> 
      <Route path = ‘ / ticket / : id ’ element = {<TicketPage editMode  = {[ True ]/}>}/> 
   </Routes> 
</BrowserRouter>
</CategoriesContext,Provider>
</div> 
)
}
export default App
}


14 - // Dashboard.JS Categories 
import {useState, useEffect, useContex } from ‘react’ 
import Ticket Card from ‘ ../ components/TicketCard ’
import axios from ‘axios’ 
import CategoriesContext from ‘../context’ 
const Dashboard = ( ) 
const {tickets, setTickets } = useState ( null ) 
const { categories, setCategories } = useContex (categoriesContex) 
useEffect (async () = > {
const response = await axios.get(‘http://localhosto:8000/tickets’) 
const dataObject response.data.data
const arreysOfkeys = object.keys(dataObject)  
const arreyOfdata = object.keys(dataObject) map(key)=>dataObject[key])
const formattedArray = []
arreyOfKeys.forEach(key, index) => {
const formattedData = {... arrayOfData [index] }
formattedData ‘documentId’ = key 
formattedArray.push (formattedData) 
})  
setTickets(formattedArray) 
}, [])
useEffect (() => ) {
setCategories ([...new Set (tickets?.map ({category}) =>cayegory)])
}, [tickets] )
console.log(categories)
const tickets = [
{
category: ‘ Q1 2022 ’,
color: ‘red’,
title: ‘ NFT Safety 101 Video’  
owner: ‘ Rodrigo ’
avatar: ‘ 12HR+ YouTube Coding Bootcamp 2021! ’,
status: ‘ done  ’,
priority: ‘ 5 ’,
progress: ‘ 40 ’,
description: ‘ Make a video showcase how to work with NFTs safety, including how to know if one is not genuine ’,
timestamp: ‘ 2022 - 02 - 11T07:36:17+0000 ’
},
{
category: ‘ Q1 2022 ’,
color: ‘red’,
title: ‘ Bild and Sell AI Model’  
owner: ‘ Rodrigo ’
avatar: ‘ 12HR+ YouTube Coding Bootcamp 2021! ’,
status: ‘ working on it  ’,
priority: ‘ 2 ’,
progress: ‘ 70 ’,
description: ‘ Make a video about AI ’,
timestamp: ‘ 2022 - 02 - 13T07:36:17+0000 ’
category: ‘ Q2 2022 ’,
color: ‘blue’,
title: ‘ Biuld a bot’  
owner: ‘ Rodrigo ’
avatar: ‘ 12HR+ YouTube Coding Bootcamp 2021! ’,
status: ‘ done  ’,
priority: ‘ 3 ’,
progress: ‘ 10 ’,
description: ‘ Make a video showcase how to work with NFTs safety, including how to know if one is not genuine ’,
timestamp: ‘ 2022 - 02 - 11T07:36:17+0000 ’
}
]
const colors = [ 
‘rgb(255,179,186)’,
‘rgb(255,233,186)’,
‘rgb’(255,255,186),
‘rgb(186,255,201)’,
‘rgb(186,255,255)’,
]
const uniqueCategories = [ 
...new Set(tickects?.map(({category}) => category))) 
]
return (
<div className = “ dashboard ”>
<h1>My Projects</h1>
<div className= “ ticket-container ” >
      {tickets && uniqueCategories?.map({uniqueCategory, categoryIndex) => (
<div key={categoryIndex}>
<h3>uniqueCategory</h3>
{tickets.filter(ticket => ticket.category === uniqueCategory ) 
.map ( filteredTicket, _index) => (
 <TicketCard
id= {_index}
color={colors[categoryindex] || colors[0]}
ticket={filteredTickect}
/>
))
}
<div/>
) )
}
</div>
export default Dashboard  
// inspect 
Pages 
New 
New JavaScript File 

  
15 - // Index.css

html, body {
margin: 0;
padding: 0;
font - family: ‘ Trebuchet MS ’, Arial, sans - serif; 
} 
.app {
display: flex; 
}
# link{
text-decoration: none;
color: rgb (46, 46, 46);
}
/*----- Nav —--*/ 
nav {
height: 100vh;
background-color: rgb ( 43, 43, 63 );
color: rgb ( 255, 255, 255 ) ;
text- align: center;
display: flex;
flex-direction: column; 
justify-content: space-between;   
}
nav .logo-conteiner,
nav controls-conteiner { 
padding: 40px 25px;
display: flex;
flex-direction: column;
}
nav .logo-conteiner,
width 20px; 
}
nav .icon {
color: rgb ( 255, 255, 255 );
}
/*----- Dashboard —--*/
.dashboard {
padding: 30px;
width: 100%;
}
.dashoboard ticket-cointainer { 
height: 80vh;
overflow: scroll;
}
/*----- TicketCard —--*/
.Ticket-card {
display: flex;
width: 100%;
}
.ticket-card # {
display: flex;
width: 100%;
}
.ticket-card # > ☆ {
background-color = rgb (211,211,211);
margin: 2px;
padding 30px;
width 100%;
display: flex;
align-items: center;
}
.ticket-card .ticket-color { 
width: 15px !important ;
Padding: 10px !important; 
margin: 2px;
} 
.ticket-card .avatar-container {
display: flex;
justify-content: center;
width: 80px;
}
.ticket-card .img-container {
height: 50px;
width: 50px;
border-radius: 25px;
overflow: hidden;
.ticket-card .img-container img {
width: 100px;
}
 }
.ticket-card .status-display {
display: flex;
justify-content: center;
}
.ticket-card .priority-display {
display: flex;
justify-content: center;
}
.ticket-card .priority-display .star-container {
display: flex;
}
.ticket-card .priority-display .star-container h3 {
margin: 7px;
padding: 0px;
}
.ticket-card .progress-display {
min-width: 200px;
}
.ticket-card .progress-bar {
width: 100%;
height: 30px;
background-color: rgb(158, 158, 158 );
border-radious: 15px;
overflow: hidden;
}
.ticket-card .progress-bar .progress-indicator {
background-color: rgb( 104, 104, 175);
height: 100%;
 }
.ticket-card .delete-block {
background-color: rgb (211, 211, 211);
width: 50px;
margin: 2px;
display: flex;
justify-content: center;
align-items: center;
}
.ticket-card .delete-block.delete-icon {
width: 2opx;
height: 20px;
border-radius: 10px;
background-color: rgb (61, 61, 61);
display: flex;
justify-content: center;
align-items: center; 
color: rgb (255, 255, 255) 
}
/*—- Ticket Page —-- */
.ticket {
padding; 30px;
width:100px;
}
.ticket .ticket-container {
width: 100%;
display: flex;
justify-content: center;
}  
.ticket form {
display: flex;
}
.ticket form section {
display: flex;
flex-direction: column 
margin:10px;
width: 500px;
}
.ticket form label {
margin: 20px o o o;
}
.ticket form select 
.ticket form input {
padding 10px;
font-size: 15px;
border-radius: 10px;
border: 1.5px solid rgb 9 (218,218,218);
margin: 5px; 
}
.ticket form .multiple-input-container {
margin: 20px 20 px 0;
} 
Project
Monday-clone 
SRC 
README.md
New
JavaScript File 
server.js
Terminal: monday-clone % npm i express cors axios dotenv
monday-clone % npm i nodemon
Project
Monday-clone 
SRC 
package.json 
npm i nodemon - - save-dev 
to change line 11:
To change line 20 and 21: 
Project
Monday-clone 
SRC 
package.json 
Terminal: % npm run start: backend


16 - // server.js
const PORT = 8000
const express = require (‘express’)
const cors =  require (‘cors’)’
require (‘dotenv’). config () 
const axios = require (‘axios’)
const app = express ()
app.use(cors())
app.use (express.json () ) 
const url = process.env.URL
const token = process.env.ASTRA_TOKEN
app.get(‘/tickets’, async ( res, res ) => {
const options = {
method ‘GET’,
headers: {
accepts: ‘applications/json’,
‘X-Cassandra-Token’: token, 
}
}
try {
const response = await axios ( ‘${url}?page-size=20’, options ) 
rest.status(200).json(response.data) 
} catch ( err ) {
console.log ( err) 
res.status ( 500 ).json({message:err})
}
})
app.get(‘/tickets/:documentId’, async ( req,res ) => ) {
const id = req.params.documentId
const options = {
method: ‘GET’, 
headers:{
accepts: ‘application.json’,
‘X-Cassandra-Token: token’, 
}
}
try {
const response = await axios (‘${url}/${id}’), options 
res.status(200).json(response,data) 
} catch (err) {
console.log ( err) 
res.status ( 500 ).json({message:err})
}
})
app.post(‘/tickets’ , async ( req, res ) = > {
const formData = req.form.body.formData 
const options - {
method ‘POST’,
headers: {
accepts: ‘applications/json’,
‘X-Cassandra-Token’: token, 
‘Content-Type’: ‘application.json’,
},
data: formData
}
try {
const response = await axios ( url. option ) 
res.status(200).json(response.data)
} catch (err ) {
console.log ( err) 
res.status ( 500 ).json({message:err})
}
})
app.put(‘/tickets/:documentId’, async ( req,res ) => ) {
const id = req.params.documentId
const data = req.body.data
const options = {
method: ‘PUT’, 
headers:{
accepts: ‘application.json’,
‘X-Cassandra-Token: token’, 
},
data 
}
try {
const response = await axios (‘${url}/${id}’), options 
res.status(200).json(response,data) 
} catch (err) {
console.log ( err) 
res.status ( 500 ).json({message:err})
}
})
app.delete(‘/tickets/:documentId’, async(req, res)=>{
const id = req.params.documentId
const options ={
method: ‘DELETE’, 
headers: {
accepts: ‘applications/json’,
‘X-Cassandra-Token’ : token 
}
}
try {
const response = await axios (‘${url}/${id}’), options 
res.status(200).json(response,data) 
} catch (err) {
console.log ( err) 
res.status ( 500 ).json({message:err})
}
}
}) 
app.listen ( PORT, () = > console.log (‘server running on PORT’ + PORT ) )
to add an new task
server.js 
New
JavaScript File 


17 // dummydate.js
 //   
const tickets = [
{
category: ‘ Q1 2022 ’,
color: ‘red’,
title: ‘ NFT Safety 101 Video’  
owner: ‘ Rodrigo ’
avatar: ‘ 12HR+ YouTube Coding Bootcamp 2021! ’,
status: ‘ done  ’,
priority: ‘ 5 ’,
progress: ‘ 40 ’,
description: ‘ Make a video showcase how to work with NFTs safety, including how to know if one is not genuine ’,
timestamp: ‘ 2022 - 02 - 11T07:36:17+0000 ’
},
{
category: ‘ Q1 2022 ’,
color: ‘red’,
title: ‘ Bild and Sell AI Model’  
owner: ‘ Rodrigo ’
avatar: ‘ 12HR+ YouTube Coding Bootcamp 2021! ’,
status: ‘ working on it  ’,
priority: ‘ 2 ’,
progress: ‘ 70 ’,
description: ‘ Make a video about AI ’,
timestamp: ‘ 2022 - 02 - 13T07:36:17+0000 ’
category: ‘ Q2 2022 ’,
color: ‘blue’,
title: ‘ Biuld a bot’  
owner: ‘ Rodrigo ’
avatar: ‘ 12HR+ YouTube Coding Bootcamp 2021! ’,
status: ‘ done  ’,
priority: ‘ 3 ’,
progress: ‘ 10 ’,
description: ‘ Make a video showcase how to work with NFTs safety, including how to know if one is not genuine ’,
timestamp: ‘ 2022 - 02 - 11T07:36:17+0000 ’
}
 ]
const colors = [ 
‘rgb(255,179,186)’,
‘rgb(255,233,186)’,
‘rgb’(255,255,186),
‘rgb(186,255,201)’,
‘rgb(186,255,255)’,
]
//


18 - // .env
URL = http://…// tickets / collections 
ASTRA_TOKEN = Astra CS:...//DBToken 




