<template>
    <nav class="sidebar" :class="{active: isActive}">
    <div class="logo__content">
        <div class="logo">
            <box-icon type='logo' name='meta' animation="spin-hover" ></box-icon>
            <div class="logo__name">Navbar</div>
        </div>
        <box-icon name='menu' @click="handleClick" ></box-icon>
    </div>

    <ul class="nav__list">
        <li class="searchbox-li">
            
                <box-icon name='search' animation="burst-hover" @click="handleClickSearch"></box-icon>
                <input type="text" placeholder="Search...">
            
        </li>
        <li>
            <a href="#">
                <box-icon name='dashboard' type='solid' animation="flashing-hover" ></box-icon>
                <span class="links__name">Dashboard</span>
            </a>
            <span class="tooltip">Dashboard</span>
        </li>
        <li>
            <a href="#">
                <box-icon name='user' animation="flashing-hover" ></box-icon>
                <span class="links__name">User</span>
            </a>
            <span class="tooltip">User</span>
        </li>
        <li>
            <a href="#">
                <box-icon name='message-rounded-dots' animation="flashing-hover" ></box-icon>
                <span class="links__name">Messages</span>
            </a>
            <span class="tooltip">Messages</span>
        </li>
        <li>
            <a href="#">
                <box-icon name='pie-chart-alt-2' animation="flashing-hover" ></box-icon>
                <span class="links__name">Analytics</span>
            </a>
            <span class="tooltip">Analytics</span>
        </li>
        <li>
            <a href="#">
                <box-icon name='cart' animation="flashing-hover" ></box-icon>
                <span class="links__name">Orders</span>
            </a>
            <span class="tooltip">Orders</span>
        </li>
        <li>
            <a href="#">
                <box-icon name='cog' animation="flashing-hover" ></box-icon>
                <span class="links__name">Settings</span>
            </a>
            <span class="tooltip">Settings</span>
        </li>
    </ul>

    <div class="profile__content">
        <div class="profile">
            <div class="profile__details">
               <img src="../assets/46.jpg" alt="profile-pic">
               <div class="name__job">
                <div class="name">Marco Basten</div>
                <div class="job">Frontend Developer</div>
               </div>
            </div>
            <box-icon name='log-out' id="log__out" animation="tada-hover"></box-icon>
        </div>
    </div>
  </nav>
</template>

<script>
import 'boxicons';

export default {
    data() {
        return {
            isActive: true,
        }
    },
    methods: {
        handleClick() {
            this.isActive = !this.isActive;
        },
        handleClickSearch() {
            if(this.isActive === false)
                this.isActive = true;
        }
    }
}
</script>

<style>

</style>