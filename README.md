.container{
    margin:auto;
    margin-top: 150px;
    background-color: aquamarine;
    width: 30%;
    height: 200PX;
    padding-top: 50px;
}
button{
    background:rgb(136, 39, 226);
    font-family: Georgia, 'Times New Roman', Times, serif;
    font-size: 20px;
    color: white;
    width: 80%;
    padding: 10px 50px;
    border-radius: 10px;
    margin-top: 20px;
    margin-left: 20px;
    text-align: left;
}
.icon{
    float: right;
    margin-right: 0px;
}
.link{
    color:white;
    text-decoration: none;
    padding: 8px 12px;
    border-radius: 3px;
}


import React from 'react';
import './Principal.css';
import {BrowserRouter as Router, Route, Switch} from 'react-router-dom';
import { FontAwesomeIcon } from '@fortawesome/react-fontawesome';
import {faUsers} from '@fortawesome/free-solid-svg-icons'
import EstudiantePermiso from '../permisos/EstudiantePermiso';
const principal = () => {
    return (
        
        <div className="container">
            
            <EstudiantePermiso/>
            <button onClick={EstudiantePermiso}><FontAwesomeIcon icon={faUsers} className="icon"/>
                <a href="./EstudiantePermisos.js" className="link">DOCENTES</a>
            </button>
            <button ><FontAwesomeIcon icon={faUsers} className="icon" />
                <a href="#" className="link">ESTUDIANTES</a>
            </button>
            
        </div>
       
    )
}

export default principal;
