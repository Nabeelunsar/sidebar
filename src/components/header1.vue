<template>
    <div class="navbar">
        <div class="logo">test <span>Hippo<i class="fa-solid fa-hippo"></i></span></div>
        <form action="#">
            <input type="search" class="search-data" placeholder="search">
            <button type="submit" class="fas fa-search"></button>
        </form>
    </div>
</template>
<script>
export default {
    name: 'header1'
}
</script>
<style scoped> .navbar {
     position: fixed;
     width: 100%;
     display: flex;
     align-items: center;
     justify-content: space-between;
     background-color: gray;
     padding: 12px 12px 12px 12px;
     color: white;
 }

 .logo {
     font-size: 24px;
     font-weight: bold;

 }

 .navbar form {
     display: flex;
     height: 34px;
     background: white;
     border-radius: 4px;
     border: 1px solid rgba(155 155 155 0.2);
 }

 .navbar form .search-data {
     height: 100%;
     width: 180px;
     padding: 0 10px;
     color: white;
     font-weight: 500;
     background: none;
     border: none;
     font-size: 17px;
     outline: none;
     color: gray;
 }

 .fa-hippo {
     color: orange;
 }

 .navbar form button {
     background: #ff3d00;
     border: none;
     cursor: pointer;
     font-size: 17px;
     color: white;
     border-radius: 2px;
     padding: 0 12px;
 }

 .navbar form button:hover {
     background: orange;
 }

 @media only screen and (max-width:500px) {
     .navbar form {
         display: none;
     }
 }
</style>