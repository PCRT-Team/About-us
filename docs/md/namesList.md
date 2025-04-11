# 人员名单

<style>
    #bilibutton {
    height: 20px;
    width: 50px;
    background-color: rgb(50, 155, 230);
    /*按钮边框宽度*/
    border: 0px;
    /*圆角*/
    border-radius: 50px;
    font-size: 13px;
    /*手指-鼠标*/
    cursor: pointer;
    /*颜色-字*/
    color: white;
    /*添加动画*/
    transition: background-color 0.3s ease;
}
/*鼠标悬停事件*/
#bilibutton:hover {
    background-color: rgb(30, 120, 200);
}
#gitbutton {
    height: 20px;
    width: 50px;
    background-color: rgb(0, 0, 0);
    /*按钮边框宽度*/
    border: 0px;
    /*圆角*/
    border-radius: 50px;
    font-size: 13px;
    /*手指-鼠标*/
    cursor: pointer;
    /*颜色-字*/
    color: white;
    /*添加动画*/
    transition: background-color 0.3s ease;
}
/*鼠标悬停事件*/
#gitbutton:hover {
    background-color: rgb(75, 75, 75);
}
</style>


> 注：排列不分先后
<div style="display: flex; flex-wrap: wrap; gap: 10px;" id="memberList">
</div>

<script>
const pcrt_members = [
    {name: "欧一biang吔", img: "o1b.jpg", bilibili: 437161770, github: "Allenkzf"},
    {name: "HLMC", img: "hlmc.jpg", bilibili: 357681195, github: "2278535805"},
    {name: "LMZO", img: "lmz.jpg", bilibili: null, github: null},
    {name: "空吧哇", img: "kbw.jpg", bilibili: 527630410, github: "K0nGbawa"},
    {name: "Bnao", img: "bnao.jpg", bilibili: 396563011, github: null},
    {name: "qaqFei", img: "qifie.jpg", bilibili: 3537119301601486, github: "qaqFei"},
    {name: "冰猫", img: "bbc.jpg", bilibili: 1644970825, github: null},
    {name: "Bychuhan", img: "bch.jpg", bilibili: 564698247, github: null},
    {name: "️泡水⑨fumo", img: "9.jpg", bilibili: null, github: null},
    {name: "️skyhigh173", img: "skyhigh173.jpg", bilibili: null, github: null},
    {name: "️realtvop", img: "qiaozhi.jpg", bilibili: null, github: null},
    {name: "️Xx_Dark_D_xX", img: "wssr.jpg", bilibili: null, github: null},
    {name: "️小奶椰", img: "xny.jpg", bilibili: null, github: null},
];
const memberList = document.getElementById("memberList");

for (const member of pcrt_members) {
    const memberDiv = document.createElement("div");
    memberDiv.style.textAlign = "center";

    const memberImg = document.createElement("img");
    memberImg.src = `./userImg/${member.img}`;
    memberImg.alt = member.name;
    memberImg.width = 100;
    memberImg.height = 100;
    memberImg.style.borderRadius = "50%";

    const memberName = document.createElement("p");
    memberName.innerText = member.name;

    memberDiv.appendChild(memberImg);
    memberDiv.appendChild(memberName);

    if (member.bilibili) {
        const bilibiliButton = document.createElement("button");
        bilibiliButton.id = "bilibutton";
        bilibiliButton.innerText = "Bilibili";
        bilibiliButton.onclick = () => window.location.href = `https://space.bilibili.com/${member.bilibili}`;
        memberDiv.appendChild(bilibiliButton);
    }

    if (member.github) {
        const githubButton = document.createElement("button");
        githubButton.id = "gitbutton";
        githubButton.innerText = "Github";
        githubButton.onclick = () => window.location.href = `https://github.com/${member.github}`;
        memberDiv.appendChild(githubButton);
    }

    memberList.appendChild(memberDiv);
}

</script>

<!-- 
copy from zywyjsq
copy by bbc
       　  　▃▆█▇▄▖
　 　 　 ▟◤▖　　　◥█▎
   　 ◢◤　 ▐　　　 　▐▉
　 ▗◤　　　▂　▗▖　　▕█▎
　◤　▗▅▖◥▄　▀◣　　█▊
▐　▕▎◥▖◣◤　　　　◢██
█◣　◥▅█▀　　　　▐██◤
▐█▙▂　　     　◢██◤
◥██◣　　　　◢▄◤
 　　▀██▅▇▀


114514 别找了哥们，这次没泄火的渠道了。
 -->


> 待补充
