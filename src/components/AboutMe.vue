<script setup>

//import skill logos
import DotNetLogo from './icons/DotNetLogo.vue'
import CSharpLogo from './icons/CSharpLogo.vue'
import PHPLogo from './icons/PHPLogo.vue'
import LinuxLogo from './icons/LinuxLogo.vue'
import JSLogo from './icons/JavaScriptLogo.vue'
import jQueryLogo from './icons/jQueryLogo.vue'
import HTMLLogo from './icons/HTMLLogo.vue'
import CSSLogo from './icons/CSSLogo.vue'
import WordPressLogo from './icons/WordPressLogo.vue'
import BrightBulb from './icons/BrightBulb.vue'
import MagnifyingGlass from './icons/MagnifyingGlass.vue'
import Bug from './icons/Bug.vue'
import Noteboard from './icons/Noteboard.vue'
import DataBase from './icons/dbIcon.vue'
import WebDesignIcon from './icons/WebDesignIcon.vue'
</script>

<template>
    <div class="container">
        <p>
            Innovative and result-driven Software Developer with 2+ years of experience spanning software architecture, object-oriented programming, website design and database architecture. Proven track record in supporting company-wide technology projects and adopting agile & lean methodologies — assisting SDLC, gathering requirements & user stories, identifying product roadmaps & value streams, influencing full stack development, database design, code debugging, unit testing and technical documentation.
        </p>
        <ul>
            <li><span><DotNetLogo/></span><span>NET Core Framework</span></li>
            <li><span><CSharpLogo/></span><span>C Sharp</span></li>
            <li><span><PHPLogo/></span><span>PHP</span></li>
            <li><span><HTMLLogo/></span><span>HTML</span></li>
            <li><span><CSSLogo/></span><span>CSS</span></li>
            <li><span><JSLogo/></span><span>javaScript</span></li>
            <li><span><jQueryLogo/></span><span>jQuery</span></li>
            <li><span><LinuxLogo/></span><span>Linux Server Hosting</span></li>
            <li><span><WordPressLogo/></span><span>Wordpress</span></li>
            <li><span><DataBase/></span><span>Database Architecture</span></li>
            <li><span><BrightBulb/></span><span>Fast Learner</span></li>
            <li><span><MagnifyingGlass/></span><span>Detail Oriented</span></li>
            <li><span><Bug/></span><span>Code debugging</span></li>
            <li><span><WebDesignIcon/></span><span>Web Design</span></li>
            <li><span><Noteboard/></span><span>Technical Documentation</span></li>
        </ul>
    </div>
</template>

<style scoped>
    .container{
        max-width:70%;
        text-align: center;
        margin-bottom:3rem;
    }

    @media(max-width:800px) {
            .container{
                max-width:100%;
            }
    }

    svg{
        -webkit-box-shadow: 0px 0px 11px 0px rgba(255,255,255,0.75);
        -moz-box-shadow: 0px 0px 11px 0px rgba(255,255,255,0.75);
        box-shadow: 0px 0px 11px 0px rgba(255,255,255,0.75);
        background-color: rgba(255,255,255,0.75);
        padding:5px;
        border-radius:15%;
        min-width:48px;
        min-height:48px;
        color:#001f68;
    }

    ul{
        display: flex;
        flex-wrap: wrap;
        text-align: left;
    }
    li{
        list-style-type: none;
        display: flex;
        padding-top:1rem;
    }
    li span:first-child{
        width:6.5rem;
        display: inline-block;
    }
    li span:first-child svg{
        height:3rem;
        margin:0 auto;
        display: flex;
    }
    li span:last-child{
        width:18rem;
    }

    @media(max-width:800px) {

            ul{
                padding: 0;
            }

            li span:first-child{
                width:auto;
                margin-right:1.0rem;
                display: flex;
                align-items: center;
            }

            li span:last-child{
                width:60vw;
                display: flex;
                align-items: center;
            }

            li{
                padding-top:1.5rem;
            }
    }
</style>