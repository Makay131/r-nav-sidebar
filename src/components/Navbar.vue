<template>
  <nav class="sidebar">
    <div class="logo__content">
        <div class="logo">
            <i class='bx bxl-meta'></i>
            <div class="logo__name">Navbar</div>
        </div>
        <i class='bx bx-menu' id="btn"></i>
    </div>

    <ul class="nav__list">
        <li>
            
                <box-icon name='search' ></box-icon>
                <input type="text" placeholder="Search...">
            
            <!--<span class="tooltip">Dashboard</span>-->
        </li>
        <li>
            <a href="#">
                <box-icon name='dashboard' type='solid' ></box-icon>
                <span class="links__name">Dashboard</span>
            </a>
            <!--<span class="tooltip">Dashboard</span>-->
        </li>
        <li>
            <a href="#">
                <box-icon name='user' ></box-icon>
                <span class="links__name">User</span>
            </a>
            <!--<span class="tooltip">User</span>-->
        </li>
        <li>
            <a href="#">
                <box-icon name='message-rounded-dots' ></box-icon>
                <span class="links__name">Messages</span>
            </a>
            <!--<span class="tooltip">Messages</span>-->
        </li>
        <li>
            <a href="#">
                <box-icon name='pie-chart-alt-2' ></box-icon>
                <span class="links__name">Analytics</span>
            </a>
            <!--<span class="tooltip">Analytics</span>-->
        </li>
        <li>
            <a href="#">
                <box-icon name='cart' ></box-icon>
                <span class="links__name">Orders</span>
            </a>
            <!--<span class="tooltip">Orders</span>-->
        </li>
        <li>
            <a href="#">
                <box-icon name='cog' ></box-icon>
                <span class="links__name">Settings</span>
            </a>
            <!--<span class="tooltip">Settings</span>-->
        </li>
    </ul>

    <div class="profile__content">
        <div class="profile">
            <div class="profile__details">
               <!-- <img src="../assets/46.jpg" alt="profile-pic"> -->
               <div class="name__job">
                <div class="name">Marco Basten</div>
                <div class="job">Frontend Developer</div>
               </div>
            </div>
            <box-icon name='log-out' id="log__out" ></box-icon>
        </div>
    </div>
  </nav>
</template>

<script>
import 'boxicons';

export default {

}
</script>

<style>

</style>