
<template>
  <!-- <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.5.0/dist/css/bootstrap.min.css" rel="stylesheet"> -->
  

  <div class="contact_main">
      <div class="wrap_div">
          <div class="header_cntct">
          <div class="txt_quick_strt"> Quick start</div>
          <div class="hedr_box1">
              <div>
                  <svg width="22" height="22" viewBox="0 0 22 22" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M11 0C4.925 0 0 4.925 0 11s4.925 11 11 11 11-4.925 11-11A11 11 0 0 0 11 0z" fill="#E0F5F1"></path><path d="M14.29 8.33a.69.69 0 0 1 0 1l-4.34 4.34a.71.71 0 0 1-1 0l-2.24-2.26a.707.707 0 1 1 1-1l1.79 1.77 3.8-3.85a.71.71 0 0 1 .99 0z" fill="#009A79"></path></svg>
              </div>
              <div class="box1_txt">Understand the Team Inbox</div>
          </div>
          <!-- -->
          <div class="btw_line"></div>
          <!--  -->
          <div class="hedr_box1">
              <div class="contct_num2">2</div>
              <div class="box1_txt">Add support channels</div>
              <div class="cnct_btn_div"><button class="cnct_btn">Connect</button></div>
          </div>
          <!--  -->
          <div class="btw_line"></div>
          <!--  -->
          <div class="hedr_box1">
              <div class="contct_num2">3</div>
              <div class="box1_txt">Provide intelligent self service</div>
          </div>
      </div>
  </div>
      
      <!--  -->
      <!-- sidebar -->
      <div class="sidebar_container">
          <div class="chat_baloon">
              <img src="/dashboard/chat-balloon.png" alt="">
          </div>
          <div class="dashbrd">
              <img src="/dashboard/dashboard.png" alt="">
          </div>
          <div class="message">
              <img src="/dashboard/message.png" alt="">
          </div>
          <router-link :to="{ name: 'users'}">
          <div class="user">
              <img src="/dashboard/user.png" alt="">
          </div>
          </router-link>
          <div class="people">
              <img src="/dashboard/people.png" alt="">
          </div>
          <div class="open_book">
              <img src="/dashboard/open-book.png" alt="">
          </div>
          <div class="chat">
              <img src="/dashboard/chat.png" alt="">
          </div>
          <div class="mega_phone">
              <img src="/dashboard/megaphone.png" alt="">
          </div>
          <div class="stats">
              <img src="/dashboard/stats.png" alt="">
          </div>
          <div class="settings">
              <img src="/dashboard/settings.png" alt="">
          </div>
          <div class="colr_menu">
              <img src="https://accounts.freshworks.com/omnibar/assets/stable/switcher.svg?v=v2.1.2-1695193281" alt="" role="presentation">
          </div>
      </div>
      <!--  -->
      <!-- secnd_navbar -->

      <div class="wrap_div2">
        <div class="scnd_thrd_wrap">
            <div class="scndry_navbar">
          <div class="inptdiv">
              <svg class="serch_img" width="16" height="16" viewBox="0 0 16 16" xmlns="http://www.w3.org/2000/svg"><g fill="none" fill-rule="evenodd"><path fill-opacity=".01" fill="#FFF" opacity=".01" d="M1 1h14v14H1z"></path><g stroke="#000"><path stroke-linecap="round" d="M9.733 9.733L14.5 14.5"></path><path d="M11.033 6.267a4.767 4.767 0 1 1-9.533 0 4.767 4.767 0 0 1 9.533 0z"></path></g></g></svg>
              <input type="text" placeholder="Search your CRM...">
          </div>
          <div class="inner_navbar">
              <div class="inner_txt">Your trial ends in 14 days
                  <svg class="warn_img"  data-toggle="tooltip" data-placement="bottom" data-html="true" data-original-title="Your current plan is <b>Freshworks CS Suite Enterprise</b>" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20"><g data-name="Layer 1"><path d="M10 20a10 10 0 1 1 10-10 10 10 0 0 1-10 10zm0-18.6a8.6 8.6 0 1 0 8.6 8.6A8.61 8.61 0 0 0 10 1.4z"></path><path d="M11.29 13.33h-.59V9.45a.7.7 0 0 0-.7-.7H8.71a.7.7 0 1 0 0 1.4h.59v3.18h-.59a.7.7 0 1 0 0 1.4h2.58a.7.7 0 0 0 0-1.4zM10 5.27a1.05 1.05 0 1 1-1 1.05 1 1 0 0 1 1-1.05z"></path></g></svg>
              </div>
             <div class="explre_btn_div"> <button class="explre_btn">Explore plans</button></div>
             <div class="explre_btn_div"> <button class="explre_btn">Request Demo</button></div>
             <div class="explre_btn_div"> <button class="explre_btn">Recommended Features</button></div>
          </div>
          <!--  -->
          <div class="navbr_divider"></div>
          <div class="plus_btn"><img src="/dashboard/plus.png" alt=""></div>
          <div class="navbr_divider"></div>
          <div class="plus_btn"><img src="/dashboard/bell.png" alt=""></div>
          <div class="navbr_divider"></div>
          <div class="name_a">A</div>
      </div>
      <!--  -->
      <!-- thrd_bar -->
      <div class="thrd_bar">
          <div class="section_one">
            <div @click="setCurrentBtn('btn0')" :class="current_btn == 'btn0' ? 'active_btn' : ''" class="new_contct_sect">
                  <div class="txt_mycontct">All Contacts</div>
                  <div class="txt_four">4</div>
                  <!-- <div class="close_icon"><img src="/dashboard/close.png" alt=""></div> -->
              </div>
              <!--  new contacts-->
              <div @click="setCurrentBtn('btn1')" :class="current_btn == 'btn1' ? 'active_btn' : ''" class="new_contct_sect">
                  <div class="txt_new_contct">Subscribed</div>
              </div>
              <!-- allcontact -->
              <div @click="setCurrentBtn('btn2')" :class="current_btn == 'btn2' ? 'active_btn' : ''" class="new_contct_sect">
                  <div class="txt_new_contct">New</div>
              </div>
              <!--  -->
              <div class="new_contct_sect">
                  <div class="txt_new_contct">+9 More...</div>
              </div>
              <!--  -->
              <div class="new_contct_sect">
                  <div class="txt_new_ctrl">Ctrl O</div>
              </div>
          </div>
          <!-- section two -->
          <div class="section_two">
              <button class="cutmiz_tble">
              <svg width="1em" height="1em" viewBox="0 0 14 14" fill="none" xmlns="http://www.w3.org/2000/svg" class="icon--container_WX8MsF4aQZ5i3RN1  svg-md undefined m-r-5"><path opacity="0.01" fill="#fff" fill-opacity="0.2" d="M0 0h14v14H0z"></path><path stroke="#333" stroke-linecap="round" stroke-linejoin="round" d="M2 7.5v6M2 .5v3"></path><circle cx="2" cy="5.5" r="1.5" stroke="#333" stroke-linecap="round" stroke-linejoin="round"></circle><path d="M7 11.5v2M7 .5v7" stroke="#333" stroke-linecap="round" stroke-linejoin="round"></path><circle cx="7" cy="9.5" r="1.5" stroke="#333" stroke-linecap="round" stroke-linejoin="round"></circle><path stroke="#333" stroke-linecap="round" stroke-linejoin="round" d="M12 7.5v6M12 .5v3"></path><circle cx="12" cy="5.5" r="1.5" stroke="#333" stroke-linecap="round" stroke-linejoin="round"></circle></svg>
              Customize table
          </button>
          <div class="imprt_btns_div">
              <button class="imprt_btn">
                  <svg width="1em" height="1em" viewBox="0 0 14 14" fill="none" xmlns="http://www.w3.org/2000/svg" class="m-r-5"><path opacity="0.01" fill="#fff" fill-opacity="0.01" d="M0 0h14v14H0z"></path><path d="M7 .5a6.5 6.5 0 1 0 0 13 6.5 6.5 0 0 0 0-13Z" stroke="#384551" stroke-linecap="round" stroke-linejoin="round"></path><path d="M4.4 7 7 9.6 9.6 7M7 4.4v5.2" stroke="#384551" stroke-linecap="round" stroke-linejoin="round"></path></svg>
                  Import Contacts
              </button>
              <select name="View Import History" id="">
                  <option value=""></option>
              </select>
          </div>
          <div class="add_cntct_btn_div">
              <button class="add_cntct_btn">
                  <svg width="1em" height="1em" viewBox="0 0 14 14" fill="none" xmlns="http://www.w3.org/2000/svg"><path opacity="0.01" fill="#fff" fill-opacity="0.01" d="M0 0h14v14H0z"></path><path d="M3.285 7h7.429M7 3.286v7.428" stroke="#fff" stroke-linecap="round"></path><rect x="0.5" y="0.5" width="13" height="13" rx="6.5" stroke="#fff" stroke-linecap="round" stroke-linejoin="round"></rect></svg>
                  Add Contact
              </button>
          </div>
          </div>
      </div>
        </div>
     
      <!-- 4bar -->

      <div class="forth_bar">
          <div class="forth_sect_one">
              <div class="tabl_btn_div">
                  <button class="tabl_btn">
                      <svg width="1em" height="1em" viewBox="0 0 14 14" fill="none" xmlns="http://www.w3.org/2000/svg" class="icon--container_WX8MsF4aQZ5i3RN1   vt__item-icon_MOzQfW1J23ifi3kW"><path fill-rule="evenodd" clip-rule="evenodd" d="M1.5 0A1.5 1.5 0 0 0 0 1.5v11A1.5 1.5 0 0 0 1.5 14h11a1.5 1.5 0 0 0 1.5-1.5v-11A1.5 1.5 0 0 0 12.5 0h-11ZM1 1.5a.5.5 0 0 1 .5-.5h2v2.5H1v-2Zm0 3v8a.5.5 0 0 0 .5.5h2V4.5H1ZM4.5 13h8a.5.5 0 0 0 .5-.5v-8H4.5V13ZM13 3.5v-2a.5.5 0 0 0-.5-.5h-8v2.5H13Z" fill="#000"></path></svg>
                      Table
                      <select name="" id=""></select>
                  </button>
              </div>
              <div>
                  <svg width="1em" height="1em" viewBox="0 0 15 14" fill="none" xmlns="http://www.w3.org/2000/svg" class="svg-md icon-style_myh0__iGZZd8UNMi"><path opacity="0.01" fill="#fff" fill-opacity="0.01" d="M1 0h14v14H1z"></path><path d="M7.95 1h6.503M7.95 5h6.503M7.95 9h6.503M7.95 13h6.503" stroke="#384551" stroke-linecap="round"></path><path d="M1.484 3.188 3.67 1 5.86 3.188M5.859 10.813 3.67 13l-2.187-2.188M3.671 12.989V1" stroke="#384551" stroke-linecap="round" stroke-linejoin="round"></path></svg>
              </div>

              <div class="tabl_btn_div">
                  <button class="tabl_btn2">
                      <svg width="1em" height="1em" viewBox="0 0 14 14" fill="none" xmlns="http://www.w3.org/2000/svg" class="icon--container_WX8MsF4aQZ5i3RN1  svg-md "><path d="M.5 10.25 7 13.5l6.5-3.25M.5 7 7 10.25 13.5 7M7 .5.5 3.75 7 7l6.5-3.25L7 .5Z" stroke="#384551" stroke-linecap="round" stroke-linejoin="round"></path></svg>
                      Bulk actions
                  </button>
              </div>

              <div class="tabl_btn_div">
                  <button class="tabl_btn2">
                      <svg width="1em" height="1em" viewBox="0 0 14 15" fill="none" xmlns="http://www.w3.org/2000/svg" class="icon--container_WX8MsF4aQZ5i3RN1  svg-md "><path opacity="0.01" fill="#fff" fill-opacity="0.01" d="M0 .5h14v14H0z"></path><path stroke="#384551" stroke-linecap="round" d="M.5 3.5h13M2.5 7.5h9M5.5 11.5h3"></path></svg>
                      1 filter applied
                  </button>
              </div>
          </div>
      </div>
      <!--  -->
      <div class="table-responsive_main">
          <table class="table1  table-hover table-bordered">
<thead>
  <tr>
    <th class="tble_name_sect" scope="col"> <input class="inptchck" type="checkbox"> Name <select name="" id="table_slct"></select></th>
    <th class="tble_txt" scope="col">Emails <select name="" id="table_slct2"></select></th>
    <th class="tble_name_sect" scope="col">Work <select name="" id="table_slct"></select></th>
    <th class="tble_txt2" scope="col">Next activity <select name="" id="table_slct2"></select></th>
    <th class="tble_txt" scope="col">Tags <select name="" id="table_slct2"></select></th>
    <th class="tble_txt" scope="col">Sales owner <select name="" id="table_slct2"></select></th>
    <th class="tble_txt" scope="col">Status <select name="" id="table_slct2"></select></th>
    <th class="tble_txt" scope="col">Accounts <select name="" id="table_slct2"></select></th>
    <th class="tble_txt" scope="col">+</th>
  </tr>
</thead>
<tbody>
  <tr v-for="(item, index) in visibleItems" :key="index" @click="showDetails(item)"    >
      <th class="name_sect " scope="row"><input class="inptchck" type="checkbox">
      <img class="tble_img v-b-modal.modal-scrollable" :src="item.image" alt=""><p class="text-primary ">{{item.name}}</p>
      </th>
    <td class="tble_txt">{{item.email}}</td>
    <td class="tble_txt">{{item.work}}</td>
    <td class="tble_txt">{{item.nextActivity }}</td>
    <td class="tble_txt">{{item.tags}}</td>
    <td class="tble_txt"><button type="button" class="badge">
      <svg width="1em" height="1em" viewBox="0 0 14 13" fill="none" xmlns="http://www.w3.org/2000/svg" class="icon--container_WX8MsF4aQZ5i3RN1  svg-md "><g stroke="#333"><path d="M2.284 9.746a.1.1 0 0 0 .096.072h9.246a.1.1 0 0 0 .096-.072l1.626-5.75a.2.2 0 0 0-.292-.227L9.584 5.765a.1.1 0 0 1-.138-.04L7.18 1.377a.2.2 0 0 0-.354 0l-2.27 4.348a.1.1 0 0 1-.139.04L.945 3.77a.2.2 0 0 0-.292.228l1.631 5.749Z"></path><path d="M2.401 12.103h9.2" stroke-linecap="round"></path></g></svg>
      {{item.SalesOwner}}</button></td>
      <td><button type="button" class="btn_won">
          <svg width="1em" height="1em" viewBox="0 0 14 12" fill="none" xmlns="http://www.w3.org/2000/svg" class="status_icon green"><path opacity="0.01" fill="#fff" fill-opacity="0.2" d="M1 0h12v12H1z"></path><path opacity="0.01" fill="#fff" fill-opacity="0.01" d="M1 0h12v12H1z"></path><path clip-rule="evenodd" d="M9.189 10.47h-7.76L4.81 6.092 1.43 1.715h7.76l3.383 4.377-3.383 4.378Z" stroke="#264966" stroke-width="0.86" stroke-linecap="round" stroke-linejoin="round"></path></svg>
          {{item.status}}</button></td>
      <td><p class="text-primary">{{item.account}}</p></td>
      <td></td>
  </tr>

</tbody>
</table>

      </div>
      <div>
        <b-pagination 
        v-model="currentPage" 
        :total-rows="totalRows" 
        :per-page="perPage"  
        @change="onPageChange" 
        size="sm" 
        align="center">
        </b-pagination>
      </div>
      <br><br>

      <b-sidebar v-model="sidebarVisible"  id="sidebar-1" right shadow >
   <div class="px-3 py-2" v-if="selectedItem">
    <div class="profl_sect">
        <img class="modal_img" :src="selectedItem.image" alt=""> 
        <h2 style="font-weight: 800px; font-size: 18px; color: black;">{{ selectedItem.name }}<br>
            <h6>{{ selectedItem.email }}</h6> 
        </h2>
        <div class="dtl_btn_top">
            <button class="tabl_btn"><svg class="svg-md mg-r-5 custom-button-svg" width="14" height="14" viewBox="0 0 14 14" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M14 0H0v14h14V0z" fill="#fff" fill-opacity=".01"></path><path d="M7.696 6.304l2.803-2.803M6.567 10.5H3.5V7.433M7.433 3.5H10.5v3.067M10.5 3.5l-7 7" stroke="#333" stroke-linecap="round" stroke-linejoin="round"></path><rect x=".5" y=".5" width="13" height="13" rx="2" stroke="#333" stroke-linecap="round" stroke-linejoin="round"></rect></svg>
                See all Details</button>
        </div>
        <div class="dtl_btn_top2">
                <button class="tabl_btn"><svg class=" custom-button-svg" width="8" height="14" viewBox="0 0 8 14" xmlns="http://www.w3.org/2000/svg"><g fill="none" fill-rule="evenodd"><path fill-opacity=".01" fill="#FFF" fill-rule="nonzero" opacity=".01" d="M-3 0h14v14H-3z"></path><path d="M7.5.5L1 7l6.5 6.5" opacity=".6" stroke="#000" stroke-linecap="round" stroke-linejoin="round"></path></g></svg></button> 
                <button class="tabl_btn"><svg class=" custom-button-svg" width="8" height="14" viewBox="0 0 8 14" xmlns="http://www.w3.org/2000/svg"><g fill="none" fill-rule="evenodd"><path fill-opacity=".01" fill="#FFF" fill-rule="nonzero" opacity=".01" d="M11 0H-3v14h14z"></path><path d="M.5.5L7 7 .5 13.5" opacity=".6" stroke="#000" stroke-linecap="round" stroke-linejoin="round"></path></g></svg></button>
            </div>
    </div>
    <div class="btn_div">
        <div class="top_btns">   
            <div class="popup_btns_div">
                <button class="tabl_btn"><svg class="svg-md valign-middle mg-r-5 custom-button-svg" width="18" height="18" viewBox="0 0 18 18" xmlns="http://www.w3.org/2000/svg"><g stroke="#000" fill="none" fill-rule="evenodd"><path d="M10.921.52H4.113c-.94 0-1.702.761-1.702 1.701v13.616c0 .94.762 1.702 1.702 1.702h10.212c.94 0 1.702-.762 1.702-1.702V5.625L10.921.52z"></path><path d="M10.921.52v4.105a1 1 0 0 0 1 1h4.106"></path><path d="M12.623 9.88H5.815M12.623 13.284H5.815M7.517 6.476H5.815" stroke-linecap="round" stroke-linejoin="round"></path></g></svg>
                <div>Note</div>
            </button>
            </div>     
           
        </div>
    <button class="tabl_btn"><svg class="svg-md valign-middle mg-r-5 custom-button-svg" width="18" height="18" viewBox="0 0 18 18" xmlns="http://www.w3.org/2000/svg"><g stroke="#000" fill="none" fill-rule="evenodd"><path d="M10.703 1.75H4.141c-.906 0-1.641.705-1.641 1.575v12.6c0 .87.735 1.575 1.64 1.575h9.844c.906 0 1.641-.705 1.641-1.575V3.75a2 2 0 0 0-2-2h-2.922z"></path><g stroke-linecap="round"><path d="M5.716.525v2.154M12.826.525v2.154M9.271.525v2.154"></path></g><path d="M5.563 10.48l2.456 2.398c.083.08.215.08.298 0L13 8.306" stroke-linecap="round"></path></g></svg>
    <div>Task</div>
    </button>
    <button class="tabl_btn"><svg class="svg-md valign-middle mg-r-5 custom-button-svg" width="18" height="18" viewBox="0 0 18 18" xmlns="http://www.w3.org/2000/svg"><g transform="translate(1)" stroke="#000" fill="none" fill-rule="evenodd" stroke-linecap="round" stroke-linejoin="round"><rect y="1.778" width="16" height="15.8" rx="2"></rect><path d="M11.556.5v3M4.444.5v3M0 8.111h16"></path></g></svg>
    <div>Meeting</div>
    </button>
    <button class="tabl_btn"><svg width="20" height="20" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg" class="svg-md valign-middle mg-r-5"><path fill-rule="evenodd" clip-rule="evenodd" d="M10.7.7A.7.7 0 0 0 10 0H.7a.7.7 0 0 0-.7.7v18.6a.7.7 0 0 0 .7.7h18.6a.7.7 0 0 0 .7-.7V6.9a.7.7 0 0 0-.7-.7h-8.6V.7zM4 12.4a.92.92 0 0 0-.92.92v5.28H1.4V1.4h7.9v17.2H7.54v-5.28a.92.92 0 0 0-.92-.92H4zm13.36 2.9a.7.7 0 0 0-.7-.7h-4a.7.7 0 1 0 0 1.4h4a.7.7 0 0 0 .7-.7zm0-4a.7.7 0 0 0-.7-.7h-4a.7.7 0 1 0 0 1.4h4a.7.7 0 0 0 .7-.7zm-9.3-2.19a.7.7 0 0 0-.7-.7h-4a.7.7 0 1 0 0 1.4h4a.7.7 0 0 0 .7-.7zm0-3.98a.7.7 0 0 0-.7-.7h-4a.7.7 0 0 0 0 1.4h4a.7.7 0 0 0 .7-.7zM4.48 13.8h1.66v4.8H4.48v-4.8zm6.22-6.2h7.9v11h-7.9v-11z"></path></svg>
    <div>Add account</div>
    </button>
    <button class="tabl_btn"><svg class="svg-md" width="4" height="14" viewBox="0 0 4 14" xmlns="http://www.w3.org/2000/svg"><g fill="none" fill-rule="evenodd"><path fill-opacity=".01" fill="#FFF" opacity=".01" d="M-5 0H9v14H-5z"></path><g transform="translate(.833 .583)" fill="#000"><circle cx="1.3" cy="1.3" r="1.3"></circle><circle cx="1.3" cy="6.5" r="1.3"></circle><circle cx="1.3" cy="11.7" r="1.3"></circle></g></g></svg></button>
    </div>
    <hr>
    <br>
    <div class="txt_lyf_cycle">
        <h3 class="overview_txt">Overview</h3>
        <button class="tabl_btn"><svg class="svg-md custom-button-svg" width="18" height="18" viewBox="0 0 18 18" xmlns="http://www.w3.org/2000/svg"><g fill="none" fill-rule="evenodd"><path fill-opacity=".01" fill="#FFF" opacity=".01" d="M0 0h18v18H0z"></path><g stroke="#000" stroke-linecap="round" stroke-linejoin="round"><path d="M14.718 11.318c-.21.477-.11 1.034.255 1.407l.047.046a1.545 1.545 0 1 1-2.187 2.187l-.047-.047a1.275 1.275 0 0 0-1.406-.255c-.467.2-.77.659-.773 1.167v.132a1.545 1.545 0 0 1-3.09 0v-.07a1.275 1.275 0 0 0-.835-1.167 1.275 1.275 0 0 0-1.407.255l-.046.047a1.545 1.545 0 1 1-2.187-2.187l.047-.047c.364-.372.465-.93.255-1.406-.2-.467-.659-.77-1.167-.773h-.132a1.545 1.545 0 1 1 0-3.09h.07a1.275 1.275 0 0 0 1.167-.835c.21-.477.11-1.034-.255-1.407L2.98 5.23a1.545 1.545 0 1 1 2.187-2.187l.047.047c.372.364.93.465 1.406.255h.062c.467-.2.77-.659.773-1.167v-.132a1.545 1.545 0 1 1 3.09 0v.07c.002.508.306.967.773 1.167.477.21 1.034.11 1.407-.255l.046-.047a1.545 1.545 0 1 1 2.187 2.187l-.047.047c-.364.372-.465.93-.255 1.406v.062c.2.467.659.77 1.167.773h.132a1.545 1.545 0 0 1 0 3.09h-.07a1.275 1.275 0 0 0-1.167.773z"></path><circle cx="9" cy="9" r="2"></circle></g></g></svg>
        <div>Customize overview</div>
        </button>
    </div>
    <br>
    <div class="txt_lyf_cycle1">
        <h6>Life Cycle stage</h6>
        <h6>Status</h6>
    </div>

    <div class="txt_lyf_cycle2">
        <h6 class="text-primary">Customer <select name="" id=""></select></h6>
        <div>
            <b-progress :max="max" class="mb-3">
      <b-progress-bar variant="success" :value="values[0]"><b class="text-dark">New</b></b-progress-bar> |
      <b-progress-bar variant="success" :value="values[1]"><b class="text-dark">Contacted</b></b-progress-bar>|
      <b-progress-bar variant="success" :value="values[2]"><b class="text-dark">Interested / U</b></b-progress-bar>|
      <b-progress-bar variant="success" :value="values[1]"><b class="text-dark">Qualified</b></b-progress-bar>|
      <b-progress-bar variant="light" :value="values[1]"><b class="text-dark">Negotiation / Lo</b></b-progress-bar>|
      <b-progress-bar variant="light" :value="values[1]"><b class="text-dark">Won / Churned</b></b-progress-bar>
    </b-progress>
        </div>
        
    </div>  
    <hr>
    <div>
        <div class="tag_icon"><svg class="tag_icon" viewBox="0 0 14 14" fill="none" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" clip-rule="evenodd" d="M13.084 8.416l-4.661 4.661a1.3 1.3 0 0 1-1.84 0L1 7.5V1h6.5l5.584 5.583a1.3 1.3 0 0 1 0 1.833z" stroke="#000" stroke-linecap="round" stroke-linejoin="round"></path><path d="M4.25 5.643a1.393 1.393 0 1 0 0-2.786 1.393 1.393 0 0 0 0 2.786z" stroke="#000"></path></svg>        Click to add Tags
</div>
    </div>
    <hr>
    <div class="more_dtls_div">
        <div>
        <h5>Location</h5>
        <h6 class="text-info">Toronto, Ontario, Canada</h6>
        </div>
        <div>
            <h5>Accounts</h5>
        <h6 class="text-info">Acme Inc (sample)</h6>
        </div>
        <div>
            <h5>Emails</h5>
        <h6 class="text-dark">lauranordasample@gmail.com</h6>
        </div>

        <div>
        <h5>Mobile</h5>
        <h6 class="text-dark">19266343001</h6>
        </div>
        <div>
            <h5>Sales owner</h5>
        <h6 class="text-dark">ajais vraj</h6>
        </div>
        <div>
            <h5>Created at</h5>
        <h6 class="text-dark">a month ago</h6>
        </div>
    </div>
    Show all <select name="" id=""></select>
    <hr>
    <div class="text_area"> 
        <input class="inpt_area" type="text" placeholder="Add a note...">
        <hr>
        <p class="inpt_text">Laura wants to buy one more license and will decide by the end of the month.</p>
        <br>
        <p class="inpt_text">ajais vraj . 13 days ago</p>
    </div>
    <!--  -->
    <div class="bottom_icons">
        <div class="icon_cover">
            <svg viewBox="0 0 14 14" xmlns="http://www.w3.org/2000/svg" width="1em" height="1em" class="icon--container_WX8MsF4aQZ5i3RN1  card-icon_d2zbHgAjG6G91rwP "><g fill="none" fill-rule="evenodd"><path fill-opacity="0.2" fill="#FFF" opacity="0.01" d="M0 0h14v14H0z"></path><g stroke="#eb8344"><path d="m8.717 2.398 4.255 7.347a2 2 0 0 1-1.73 3.002h-8.51A2 2 0 0 1 1 9.745l4.255-7.347a2 2 0 0 1 3.461 0ZM7 9.603v1.121M7 3.615v4.807"></path></g></g></svg>
        </div>
        <div>Couldn’t load this card. Try refreshing the page.</div>
    </div>
    <!--  -->
    <div class="bottom_icons2">
        <div class="icon_cover2">
            <svg width="1em" height="1em" viewBox="0 0 22 22" fill="none" xmlns="http://www.w3.org/2000/svg" class="icon--container_WX8MsF4aQZ5i3RN1  card-icon_d2zbHgAjG6G91rwP "><path opacity="0.01" fill="#fff" fill-opacity="0.2" d="M1 1h20v20H1z"></path><path opacity="0.01" fill="#A9A9EB" d="M1 1h20v20H1z"></path><rect x="1.313" y="3.465" width="19.375" height="17.222" rx="2" fill="#fff" stroke="#6E49B8" stroke-linecap="round" stroke-linejoin="round"></rect><path d="M1.313 5.465a2 2 0 0 1 2-2h15.374a2 2 0 0 1 2 2v2.844H1.313V5.465Z" fill="#B4A3D6" stroke="#6E49B8" stroke-linecap="round" stroke-linejoin="round"></path><path d="M15.306 1.313v4.305M6.694 1.313v4.305" stroke="#6E49B8" stroke-linecap="round" stroke-linejoin="round"></path></svg>        </div>
        <div>No upcoming meetings with Laura Norda. <br>
            <b class="text-info">Add meeting</b>
        </div>
    </div>
    <!--  -->
    <div class="bottom_icons2">
        <div class="icon_cover">
            <svg xmlns="http://www.w3.org/2000/svg" width="1em" height="1em" viewBox="0 0 22 15" fill="none" class="icon--container_WX8MsF4aQZ5i3RN1  card-icon_d2zbHgAjG6G91rwP "><path fill-rule="evenodd" clip-rule="evenodd" d="M1.313 2.75a2 2 0 0 1 2-2h15.374a2 2 0 0 1 2 2v8.799a2 2 0 0 1-2 2H3.313a2 2 0 0 1-2-2V2.75Z" fill="#FDDBB5" stroke="#E86F25" stroke-linecap="round" stroke-linejoin="round"></path><path fill-rule="evenodd" clip-rule="evenodd" d="M1.313 2.54a.9.9 0 0 1 1.478-.69L11 8.749l8.209-6.897a.9.9 0 0 1 1.479.689v8.867a2 2 0 0 1-2 2H3.313a2 2 0 0 1-2-2V2.54Z" fill="#fff" stroke="#E86F25" stroke-linecap="round" stroke-linejoin="round"></path></svg>        </div>
        <b class="text-dark">Laura Norda sent an email
            <p>5 Days ago</p>
        </b>
    </div>
    <!--  -->
    <div class="bottom_icons2">
        <div class="icon_cover3">
            <svg xmlns="http://www.w3.org/2000/svg" width="1em" height="1em" viewBox="0 0 21 21" fill="none" class="icon--container_WX8MsF4aQZ5i3RN1  card-icon_d2zbHgAjG6G91rwP "><circle cx="10.236" cy="10.764" r="9.236" fill="#fff" stroke="#2895A4" stroke-linecap="round" stroke-linejoin="round"></circle><circle cx="10.236" cy="10.764" fill="#ABECF5" stroke="#2895A4" stroke-linecap="round" stroke-linejoin="round" r="5.278"></circle><circle cx="10.236" cy="10.764" fill="#fff" r="1.319"></circle><path d="M10.236 10.764 18.1 2.9M18.1 1v1.9H20" stroke="#2895A4" stroke-linecap="round" stroke-linejoin="round"></path></svg>        </div>
        <p class="text-dark">Laura Norda is not part of any sales sequence.</p>
    </div>
   </div>
</b-sidebar>
      </div>
  </div>
</template>

<script>
export default {
    data() {
      return {
        values: [15, 30, 20],
        max: 100,
        current_btn: 'btn0',
        perPage: 5, 
        currentPage: 1,
        displayedItems: [],
        sidebarVisible: false,
        selectedItem: null,
        TableData:[
            
        {   name: 'Laura Norda ',
            image: '/dashboard/prof_pic_dashbrd.png',
            email: 'lauranordasample@gmail.com', 
            work: '4167348672', 
            nextActivity: '+ Add task',
            tags: '+ Click to Add',
            SalesOwner: 'ajaisvraj', 
            status: 'Won', 
            account: 'Acme Inc (sample)' 
        },
        {   name: 'Spector Calista',
            image: '/dashboard/prof_pic_dashbrd2.png',   
            email: 'spectorcalista@gmail.com', 
            work: '3684945781', 
            nextActivity: '+ Add task',
            tags: '+ Click to Add',
            SalesOwner: 'ajaisvraj', 
            status: 'Lost', 
            account: 'Techcave (sample)' 
        },
        {   name: 'Jay Patel',
            image: '/dashboard/prof_pic_dashbrd3.png',
            email: 'jaypatelsample@gmail.com', 
            work: '+ Click to Add', 
            nextActivity: '+ Add task',
            tags: '+ Click to Add',
            SalesOwner: 'ajaisvraj', 
            status: 'Won', 
            account: 'E Corp (sample)' 
        },
        {   name: 'Jane Sampleton',
            image: '/dashboard/prof_pic_dashbrd4.png',
            email: 'janesampleton@gmail.com', 
            work: '3684932360', 
            nextActivity: '+ Add task',
            tags: '+ Click to Add',
            SalesOwner: 'ajaisvraj', 
            status: 'Won', 
            account: 'Widgetz.io ' 
        },
        {   name: 'Laura Norda',
            image: '/dashboard/prof_pic_dashbrd.png',
            email: 'lauranordasample@gmail.com', 
            work: '4167348672', 
            nextActivity: '+ Add task',
            tags: '+ Click to Add',
            SalesOwner: 'ajaisvraj', 
            status: 'Won', 
            account: 'Acme Inc (sample)' 
        },
        {   name: 'Jane Sampleton',
            image: '/dashboard/prof_pic_dashbrd4.png',
            email: 'janesampleton@gmail.com', 
            work: '3684932360', 
            nextActivity: '+ Add task',
            tags: '+ Click to Add',
            SalesOwner: 'ajaisvraj', 
            status: 'Won', 
            account: 'Widgetz.io ' 
        },
        {   name: 'Jay Patel (sample)',
            image: '/dashboard/prof_pic_dashbrd3.png',
            email: 'jaypatelsample@gmail.com', 
            work: '+ Click to Add', 
            nextActivity: '+ Add task',
            tags: '+ Click to Add',
            SalesOwner: 'ajaisvraj', 
            status: 'Won', 
            account: 'E Corp (sample)' 
        },
        {   name: 'Laura Norda (sample)',
            image: '/dashboard/prof_pic_dashbrd.png',
            email: 'lauranordasample@gmail.com', 
            work: '4167348672', 
            nextActivity: '+ Add task',
            tags: '+ Click to Add',
            SalesOwner: 'ajaisvraj', 
            status: 'Won', 
            account: 'Acme Inc (sample)' 
        },
        {   name: 'Spector Calista',
            image: '/dashboard/prof_pic_dashbrd2.png',   
            email: 'spectorcalista@gmail.com', 
            work: '3684945781', 
            nextActivity: '+ Add task',
            tags: '+ Click to Add',
            SalesOwner: 'ajaisvraj', 
            status: 'Lost', 
            account: 'Techcave (sample)' 
        },
        {   name: 'Laura Norda (sample)',
            image: '/dashboard/prof_pic_dashbrd.png',
            email: 'lauranordasample@gmail.com', 
            work: '4167348672', 
            nextActivity: '+ Add task',
            tags: '+ Click to Add',
            SalesOwner: 'ajaisvraj', 
            status: 'Won', 
            account: 'Acme Inc (sample)' 
        },
        {   name: 'Laura Norda (sample)',
            image: '/dashboard/prof_pic_dashbrd.png',
            email: 'lauranordasample@gmail.com', 
            work: '4167348672', 
            nextActivity: '+ Add task',
            tags: '+ Click to Add',
            SalesOwner: 'ajaisvraj', 
            status: 'Won', 
            account: 'Acme Inc (sample)' 
        }
        ]   
      }
    },
    computed: {
    totalRows() {
    return this.TableData.length; 
    },
    visibleItems() {
      const startIndex = (this.currentPage - 1) * this.perPage;
      const endIndex = startIndex + this.perPage;
      return this.TableData.slice(startIndex, endIndex);
    },
  },
  methods: {
    toggleSidebar() {
      this.$refs.mySidebar.toggle();
    },
    setCurrentBtn(btn) {
      this.current_btn = btn;
    },
    onPageChange(newPage) {
      this.currentPage = newPage;
  },
  showDetails(item) {
    this.selectedItem = item;
    this.sidebarVisible = true;
  }

  }
};
</script>


<style>
@import './style/homestyle.css';
</style>

