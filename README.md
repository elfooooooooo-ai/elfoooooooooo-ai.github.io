[Uploading elfo_yam.html…]()
# elfoooooooooo-ai.github.io<!DOCTYPE html>
<html lang="en"><head><meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1, viewport-fit=cover">
<title>NEON HARBOR · v12 NOVA UPDATE</title>
<link href="https://fonts.googleapis.com/css2?family=Rajdhani:wght@500;700&family=Vazirmatn:wght@400;700&display=swap" rel="stylesheet">
<style>
:root{--ink:#070b12;--cy:#36f1ff;--mg:#ff3d8b;--tx:#cfeaf0;--pn:rgba(7,13,24,.72)}
html,body{margin:0;height:100%;background:var(--ink);overflow:hidden;font-family:Rajdhani,'Segoe UI',system-ui,sans-serif;color:var(--tx)}
#gl{display:block;width:100%;height:100%}
.hud{position:fixed;pointer-events:none;background:var(--pn);border:1px solid rgba(54,241,255,.35);border-radius:6px;padding:6px 12px;font-size:18px}
#info{top:max(16px,env(safe-area-inset-top));right:16px;display:flex;gap:16px;align-items:center}
#clock{color:var(--cy);font-size:24px}#money{color:#9dffb0}
#mini{position:fixed;left:16px;bottom:max(16px,env(safe-area-inset-bottom));width:180px;height:180px;border:2px solid var(--cy);border-radius:50%;background:#0b1220;pointer-events:none}
#speed{right:16px;bottom:max(16px,env(safe-area-inset-bottom));width:132px;height:132px;padding:0;display:none;text-align:center}
#speed svg{position:absolute;inset:0;width:100%;height:100%}
#speed path{fill:none;stroke-width:6;stroke-linecap:round}
.bg{stroke:rgba(54,241,255,.15)}.fg{stroke:var(--cy);stroke-dasharray:226.2;stroke-dashoffset:226.2}
#speed div{position:absolute;inset:0;display:flex;flex-direction:column;justify-content:center}
#spd{font-size:40px;line-height:1}#speed small{opacity:.7}
#prompt{left:50%;bottom:22%;transform:translateX(-50%);display:none;color:var(--cy)}
#toast{left:50%;top:70px;transform:translateX(-50%);display:none;color:var(--mg)}
#fps{left:16px;top:16px;display:none;font-size:14px}
#screen{position:fixed;inset:0;display:flex;flex-direction:column;align-items:center;justify-content:center;gap:10px;background:rgba(5,8,16,.78);cursor:pointer;text-align:center}
#screen h1{margin:0;font-size:clamp(44px,9vw,92px);letter-spacing:.06em;color:var(--cy);text-shadow:0 0 28px rgba(54,241,255,.55),4px 4px 0 var(--mg)}
#sub{font-size:24px;margin:0 0 4px}#sub2{font-size:15px;margin:0 0 14px;color:#8fd8e8;opacity:.85}#build{position:fixed;left:16px;top:44px;font-size:12px;letter-spacing:.08em;color:var(--cy);opacity:.72;pointer-events:none;z-index:4;text-shadow:0 0 8px rgba(54,241,255,.53)}
.keys{display:grid;grid-template-columns:auto auto;gap:4px 22px;text-align:left;font-size:18px}.keys b{color:var(--cy)}

#shop{display:none;position:fixed;right:18px;top:80px;width:min(330px,calc(100vw - 36px));max-height:78vh;overflow:auto;background:rgba(5,12,24,.96);border:1px solid var(--cy);border-radius:10px;padding:14px;z-index:5;box-shadow:0 0 24px #36f14422}
#shop h2{margin:0 0 8px;color:var(--cy)}#shop p{margin:5px 0 12px}
.shopgrid{display:grid;grid-template-columns:1fr 1fr;gap:7px}
#shop button{background:#101f30;color:#d8faff;border:1px solid #267b8a;padding:9px;border-radius:5px;font:inherit;cursor:pointer}
#shop button:hover{border-color:var(--cy);background:#17354a}
#wanted{color:#ffce54;letter-spacing:3px;font-size:21px}
#bars{top:68px;right:16px;width:210px;display:flex;flex-direction:column;gap:5px;font-size:15px}
.bar{height:9px;background:#0007;border:1px solid #fff4}.bar i{display:block;height:100%;width:100%}
#hbi{background:#d9302c}#abi{background:#d8dde6}#wp{color:#ffdca0;letter-spacing:.08em}
#obj{left:50%;bottom:max(12px,env(safe-area-inset-bottom));transform:translateX(-50%);color:#ffd24a;font-size:20px;white-space:nowrap}
#zone{position:fixed;right:24px;bottom:170px;font-size:clamp(34px,5vw,58px);font-weight:700;font-style:italic;text-transform:uppercase;color:#f0e2b0;text-shadow:2px 2px 0 #000,0 0 14px #000a;opacity:0;pointer-events:none}
@keyframes zn{0%{opacity:0;transform:translateY(12px)}12%,72%{opacity:1;transform:none}100%{opacity:0}}
#ovl{position:fixed;left:0;right:0;top:32%;text-align:center;display:none;pointer-events:none;z-index:6}
#ovl h2{margin:0;font-size:clamp(56px,12vw,150px);letter-spacing:.04em;font-style:italic;text-transform:uppercase;text-shadow:3px 3px 0 #000,0 0 30px #000}
#ovl p{margin:0;font-size:36px;color:#fff;text-shadow:2px 2px #000}
#hit{position:fixed;inset:0;pointer-events:none;background:radial-gradient(transparent 45%,rgba(200,0,0,.7));opacity:0}
#gl.dead{filter:grayscale(1) contrast(1.15)}
#skin{display:none;position:fixed;right:18px;top:80px;width:min(330px,calc(100vw - 36px));max-height:78vh;overflow:auto;background:rgba(5,12,24,.96);border:1px solid var(--cy);border-radius:10px;padding:14px;z-index:5}
#skin h2{margin:0 0 8px;color:var(--cy)}#skin p{margin:5px 0 12px}
#skin button{background:#101f30;color:#d8faff;border:1px solid #267b8a;padding:9px;border-radius:5px;font:inherit;cursor:pointer}#skin button:hover{border-color:var(--cy);background:#17354a}
#mapv{display:none;position:fixed;inset:0;z-index:4;background:rgba(4,8,16,.94);flex-direction:column;align-items:center;justify-content:center;gap:8px}
#mapc{border:2px solid var(--cy);cursor:crosshair;max-width:100%}#mapk{color:var(--cy);font-size:18px}.mzb{background:#101f30;color:#d8faff;border:1px solid #267b8a;border-radius:5px;font:inherit;font-size:20px;width:40px;height:34px;cursor:pointer}.mzb:hover{border-color:var(--cy)}#toast{z-index:7}
#vig{position:fixed;inset:0;pointer-events:none;background:radial-gradient(ellipse at center,transparent 58%,rgba(0,0,0,.42))}
#xh{position:fixed;left:50%;top:50%;width:14px;height:14px;margin:-7px;border:2px solid #fff;border-radius:50%;opacity:.8;pointer-events:none;display:none}
#gl{touch-action:none}#alb{position:fixed;left:50%;bottom:18%;transform:translateX(-50%);display:none;z-index:7;padding:12px 26px;font:700 18px Rajdhani,sans-serif;letter-spacing:.15em;color:#001018;background:#36f1ff;border:0;border-radius:6px;cursor:pointer;box-shadow:0 0 24px #36f1ff}#lcd{position:fixed;left:0;right:0;top:20%;text-align:center;display:none;pointer-events:none;z-index:6;font:700 clamp(40px,10vw,120px) Rajdhani,sans-serif;font-style:italic;color:#fff;text-shadow:3px 3px 0 #000,0 0 30px #36f1ff}#fade{position:fixed;inset:0;background:#000;opacity:0;pointer-events:none;z-index:8;transition:opacity 1s}#gho{position:fixed;inset:0;display:none;pointer-events:none;box-shadow:inset 0 0 140px rgba(54,241,255,.38)}#gho b{position:absolute;left:50%;top:14px;transform:translateX(-50%);color:var(--cy);letter-spacing:.3em;font-size:18px;text-shadow:0 0 12px var(--cy)}
.mn{display:block;width:min(320px,80vw);margin:6px;padding:14px;font:700 24px Rajdhani,sans-serif;letter-spacing:.08em;color:var(--cy);background:#0b1626;border:1px solid var(--cy);border-radius:8px;cursor:pointer}.mn:hover{background:#16344a}
#set{display:none;position:fixed;inset:0;z-index:9;background:rgba(5,8,16,.92);align-items:center;justify-content:center}
.sb{width:min(560px,94vw);max-height:90vh;overflow:auto;background:rgba(5,12,24,.97);border:1px solid var(--cy);border-radius:10px;padding:14px;font-size:18px}
.sb h2,.sb h3{margin:6px 0;color:var(--cy)}.r{display:flex;justify-content:space-between;align-items:center;gap:10px;margin:6px 0}
.r button{background:#101f30;color:#d8faff;border:1px solid #267b8a;padding:7px 12px;border-radius:5px;font:inherit;cursor:pointer}.ch{font-size:14px;opacity:.85;margin:3px 0}.ch b{color:var(--mg)}
#mob{display:none;position:fixed;inset:0;z-index:10;pointer-events:none}
.mbt{position:absolute;transform:translate(-50%,-50%);border-radius:50%;background:#0b1626;border:2px solid var(--cy);color:var(--cy);text-align:center;font-weight:700;pointer-events:auto;touch-action:none;user-select:none}.mbt.on,.mbt.sel{background:var(--cy);color:#000}
#med{display:none;position:fixed;inset:0;z-index:9;background:rgba(5,8,16,.88);align-items:flex-end;justify-content:center}.lg{display:flex;flex-wrap:wrap;gap:2px 12px;font-size:13px;margin-top:6px}.lg b{color:var(--cy)}
#scope{display:none;position:fixed;inset:0;pointer-events:none;z-index:3;background:linear-gradient(#000,#000) center/1px 70% no-repeat,linear-gradient(#000,#000) center/70% 1px no-repeat,radial-gradient(circle at center,transparent 34%,#000 35%)}
body.nc,body.nc *{cursor:none!important}
body.fa,body.fa button,body.fa input,body.fa .mn{font-family:Vazirmatn,Tahoma,sans-serif!important}body.fa *{letter-spacing:0!important}body.fa .sb,body.fa #shop,body.fa #skin{direction:rtl;text-align:right}
</style></head><body>
<canvas id="gl"></canvas><canvas id="mini" width="200" height="200"></canvas><div id="vig"></div><div id="gho"><b>GHOST</b></div><div id="lcd"></div><button id="alb">AUTO LAND [G]</button><div id="fade"></div><div id="xh"></div>
<div id="info" class="hud"><b id="clock">09:00</b><span id="loc">Downtown</span><span id="wanted">☆☆☆☆☆</span><span id="money">$ 5,000</span></div>
<div id="build">BUILD v12 · NOVA UPDATE</div>
<div id="shop"></div>
<div id="speed" class="hud"><svg viewBox="0 0 120 120"><path class="bg" d="M26.06 93.94A48 48 0 1 1 93.94 93.94"/><path id="arc" class="fg" d="M26.06 93.94A48 48 0 1 1 93.94 93.94"/></svg><div><b id="spd">0</b><small>km/h</small></div></div>
<div id="prompt" class="hud">Press F to enter vehicle</div><div id="toast" class="hud"></div><div id="fps" class="hud"></div>
<div id="bars" class="hud"><div id="wp">FIST</div><div class="bar"><i id="abi" style="width:0"></i></div><div class="bar"><i id="hbi"></i></div><div id="jetw" style="display:none;color:#8fe8ff">JET</div><div class="bar" id="jetb" style="display:none"><i id="jbi" style="background:#36f1ff;width:100%"></i></div></div>
<div id="obj" class="hud"></div><div id="zone"></div><div id="hit"></div><div id="ovl"><h2 id="ot"></h2><p id="os"></p></div>
<div id="skin"></div><div id="mapv"><canvas id="mapc"></canvas><div id="mapk"><button class="mzb" id="mzp">＋</button> <button class="mzb" id="mzm">－</button> <button class="mzb" id="mzr">⟲</button> M / Esc: close · Click: waypoint · Wheel / pinch: zoom · Drag: pan</div></div>
<div id="screen"><h1>NEON HARBOR</h1><p id="sub">GTA_elfo · v12 NOVA UPDATE</p><p id="sub2">Nova City · Flying cars · Jetpack · Aliens · Performance boost</p><button class="mn" id="bStart">Start GTA_elfo</button><button class="mn" id="bSet">Settings</button></div>
<div id="set"></div><div id="mob"></div><div id="med"></div><div id="scope"></div>
<script src="https://cdnjs.cloudflare.com/ajax/libs/three.js/r128/three.min.js"></script>
<script>
var ENVM=[];
(()=>{'use strict';
const $=id=>document.getElementById(id);let Game;
/* ===== CONFIG ===== */
const C=Object.freeze({seed:1337,half:1250,zs:3250,step:120,roadW:16,aveW:24,aves:[3,7],cell:40,walk:4,sprint:8,jump:7,grav:-22,pr:.5,enter:4,cycle:480,start:9,
 car:{max:55,acc:34,brake:45,drag:.06,roll:1.5,steer:.6,wb:2.6,grip:7,hb:1.1,rev:15},
 npc:{n:55,parked:35,cull:340,near:160,far:330,follow:15},
 cam:{fd:6,fh:2.2,cd:9,ch:3.5,fov:70,fovMax:85,idle:2},
 moto:{max:62,acc:42,brake:50,drag:.06,roll:1.5,steer:.8,wb:1.8,grip:9,hb:1.1,rev:8},
 ped:{n:36,cull:260,spread:300,hit:1.7},mis:{reward:1500,r:7}});
/* ===== UTILS ===== */
const U={rng(a){return()=>{a|=0;a=a+0x6D2B79F5|0;let t=Math.imul(a^a>>>15,1|a);t=t+Math.imul(t^t>>>7,61|t)^t;return((t^t>>>14)>>>0)/4294967296}},
 clamp:(v,a,b)=>Math.min(b,Math.max(a,v)),lerp:(a,b,t)=>a+(b-a)*t,wrap:a=>Math.atan2(Math.sin(a),Math.cos(a)),
 lerpA:(a,b,t)=>a+U.wrap(b-a)*t,sm:(a,b,x)=>{x=U.clamp((x-a)/(b-a),0,1);return x*x*(3-2*x)}};
const WEAP={Pistol:{dmg:34,rate:.28,rng:60,pel:1,spr:.012,ammo:48,len:.34},SMG:{dmg:18,rate:.075,rng:55,pel:1,spr:.05,ammo:120,len:.5,auto:1},
 Shotgun:{dmg:16,rate:.8,rng:28,pel:7,spr:.12,ammo:24,len:.85},Rifle:{dmg:28,rate:.11,rng:90,pel:1,spr:.025,ammo:90,len:.95,auto:1},Sniper:{dmg:100,rate:1.2,rng:220,pel:1,spr:0,ammo:12,len:1.15}},GUNS=Object.keys(WEAP);
const SHOPS=[],SHOPDEF={gun:{name:'HARBOR ARMS',css:'#ff5a5a',col:0x7a2a2a},att:{name:'ATTACHMENT LAB',css:'#ffb84d',col:0x6a4a1a},car:{name:'PREMIUM MOTORS',css:'#4dffa0',col:0x1a5a3a},moto:{name:'TWO WHEELS',css:'#c77dff',col:0x4a2a6a},garage:{name:'ELFO GARAGE',css:'#ffe94d',col:0x5a5a1a},arena:{name:'CHALLENGE HALL',css:'#ff7a3d',col:0x6a2a14},air:{name:'AIRCRAFT DEALER',css:'#6ad0ff',col:0x2a6a9a},mil:{name:'MILITARY DEPOT',css:'#9bd15a',col:0x3a4a2a},space:{name:'ASTRA SPACEWORKS',css:'#b58cff',col:0x2a2a5a},skin:{name:'URBAN THREADS',css:'#4dd2ff',col:0x2a5a7a},nova:{name:'NOVA OUTFITTERS',css:'#7dffd0',col:0x1a6a5a}},
LOTS={'9,5':'arena','0,3':'mil','5,5':'gun','2,8':'gun','6,4':'att','1,6':'att','3,3':'car','8,7':'car','4,7':'moto','7,4':'moto','6,6':'garage','2,2':'garage','8,3':'garage','3,6':'skin'};
const SKINS=[{n:'Harbor Blue',sh:0x2b6cff,pn:0x222a3a,sk:0xe0b090,price:0},{n:'Tourist',sh:0xf0a030,pn:0x6fa8ff,sk:0xe0b090,price:100},{n:'Street Red',sh:0xc0392b,pn:0x1a1a1a,sk:0xc68c62,price:150},
 {n:'Neon Punk',sh:0xff3d8b,pn:0x1b1030,sk:0xe0b090,price:250},{n:'Cyber Cyan',sh:0x36f1ff,pn:0x0a2a3a,sk:0x8d5a3b,price:300},{n:'Business',sh:0x20242c,pn:0x101216,sk:0xf1cfb0,price:350},
 {n:'Tactical',sh:0x3d4a3a,pn:0x2a2f26,sk:0xc68c62,price:400},{n:'Gold Suit',sh:0xe8c547,pn:0x2a2a2a,sk:0x8d5a3b,price:500}];
const MAPLBL=[['SOUTH GATE',0,570],['GREENFIELD PARK',360,-300],['DOWNTOWN',0,-170],['WESTGATE',-420,-60],['EASTSIDE',420,200],['CENTRAL PLAZA',-60,78],['AIRPORT',0,-630],['NORTH HIGHLANDS',0,-1000],['EAST OUTSKIRTS',950,-250],['WEST OUTSKIRTS',-950,-250],['RING HIGHWAY',1150,-700]];
const SHIPS={shuttle:{n:'Orbiter S1 Shuttle',p:350000,i:0},capsule:{n:'Starlift Capsule',p:200000,i:1},cruiser:{n:'Aether X Cruiser',p:900000,i:2}};
const PADR=22,SHIPST={shuttle:{thr:22,rcs:1.3,burn:1.2,fuel:100},capsule:{thr:20,rcs:1,burn:1,fuel:100},cruiser:{thr:26,rcs:2.2,burn:1,fuel:120}};
const mtR=(m,x,z)=>{const N=m[4]||16,q=2*Math.PI/N;let f=(Math.atan2(x-m[0],z-m[1])-(m[5]||0))%q;if(f<0)f+=q;return m[2]*Math.cos(Math.PI/N)/Math.cos(f-Math.PI/N)},
mtIn=(m,x,z,y)=>y<m[3]&&Math.hypot(x-m[0],z-m[1])<mtR(m,x,z)*(1-Math.max(0,y)/m[3]);
const POI=[],EMPTY=[],CIRC=[-1.3,0,1.3],NOKEY={};
const MAG={Pistol:12,SMG:30,Shotgun:6,Rifle:30,Sniper:5},RL={Pistol:1.2,SMG:1.5,Shotgun:2.1,Rifle:1.8,Sniper:2.3},
ATT=[['sil','Suppressor',400],['stock','Stock',300],['long','Long barrel',500],['short','Short barrel',350],['scp','Scope (aim: RMB / Z)',600],['mag','Extended magazine',450]];
/* d=[length,width,roof,hood,deck,windshieldBase,roofFront,roofRear,deckStart] */
const CARMODELS={Sedan:{n:'Classic Sedan',p:2500,c:0x2c7be5,mx:1,ac:1,d:[4.4,1.8,1.35,.85,.95,.6,-.2,-.7,-1.5]},
 Muscle:{n:'Ford Mustang GT',p:4500,c:0x1f3d9c,mx:1.15,ac:1.2,d:[4.8,1.95,1.3,.95,1,.5,-.3,-1.2,-1.9]},
 SUV:{n:'Range SUV',p:4000,c:0x222222,mx:1,ac:1,d:[4.8,2,1.85,1.2,1.65,1.1,.3,-2.1,-2.2]},
 Porsche:{n:'Porsche 911',p:8000,c:0xc9ccd4,mx:1.25,ac:1.3,d:[4.5,1.85,1.3,.85,1,.65,-.2,-1.1,-1.8]},
 Pickup:{n:'Ford F-150 Pickup',p:5000,c:0xb8402a,mx:1,ac:1.05,d:[5.4,2,1.9,1.25,1.15,1.2,.5,-.5,-.55]},
 Van:{n:'Mercedes Sprinter Van',p:4200,c:0xe8e8e8,mx:.95,ac:.95,d:[5.2,2,2.2,1.3,2.1,1.7,1.3,-2.5,-2.55]},
 Taxi:{n:'City Taxi',p:2600,c:0xf2c200,mx:1,ac:1,d:[4.4,1.8,1.35,.85,.95,.6,-.2,-.7,-1.5]},
 BMW:{n:'BMW M3',p:6500,c:0xf0f0f4,mx:1.2,ac:1.25,d:[4.7,1.9,1.38,.9,1,.7,-.3,-1.2,-1.7]},
 GWagon:{n:'Mercedes G63',p:12000,c:0x111111,mx:1.1,ac:1.1,d:[4.7,2,1.95,1.2,1.75,.9,.2,-2.1,-2.2]},
 Corvette:{n:'Chevrolet Corvette',p:9000,c:0xc83a12,mx:1.3,ac:1.35,sp:1,d:[4.6,1.95,1.18,.75,.92,.7,-.1,-.95,-1.65]},
 McLaren:{n:'McLaren P1',p:22000,c:0xff6a00,mx:1.45,ac:1.55,sp:1,d:[4.6,2,1.12,.66,.88,.9,-.1,-1.1,-1.75]},
 Bugatti:{n:'Bugatti Chiron',p:30000,c:0x123a9a,mx:1.6,ac:1.6,sp:1,d:[4.7,2,1.2,.8,.98,.75,-.2,-1,-1.7]},
 Ferrari:{n:'Ferrari 488',p:14000,c:0xd10000,mx:1.32,ac:1.4,sp:1,d:[4.5,1.95,1.2,.78,.95,.75,-.1,-.9,-1.6]},
 Police2:{n:'Muscle Racer',p:7000,c:0x6a1fb0,mx:1.3,ac:1.35,sp:1,d:[4.8,1.95,1.25,.9,1,.55,-.3,-1.2,-1.9]},Hatch:{n:'City Hatchback',p:1800,c:0x22aa66,mx:.95,ac:1,d:[3.9,1.7,1.4,.8,.9,.55,-.1,-.5,-1.3]},Limo:{n:'Stretch Limo',p:9500,c:0x0a0a0a,mx:1,ac:.9,d:[6.4,2,1.4,.9,1,.6,-.3,-2.4,-2.9]},Revuelto:{n:'Lamborghini Revuelto',p:260000,c:0x121216,lx(L,w,H,hh,dh,B,C){const W=[1,1,1],R=[1,.05,.05],O=[1,.5,.05],o=[];for(const s of[1,-1])o.push(B(.85,.05,.07,s*.62,hh-.28,L/2+.05,W,0,0,-s*.28),B(.45,.05,.07,s*.3,hh-.46,L/2+.05,W,0,0,s*.75),B(.3,.04,.07,s*.78,hh-.4,L/2+.05,O));o.push(B(w-.45,.07,.07,0,dh-.08,-L/2-.05,R),B(.5,.1,.07,.55,dh-.22,-L/2-.05,R),B(.5,.1,.07,-.55,dh-.22,-L/2-.05,R));return o},mx:1.55,ac:1.6,sp:1,d:[4.95,2.03,1.14,.7,.82,.45,-.2,-1.15,-1.8],ex(P,bx,K,ch,L,w,H,hh,dh,gc,z1){P.push(bx(w*.5,.03,1.1,0,hh+.01,L/2-1.3,[.1,.1,.12]),bx(.5,.04,.9,.5,dh+.02,-L/2+.8,[.1,.1,.12]),bx(.5,.04,.9,-.5,dh+.02,-L/2+.8,[.1,.1,.12]),bx(w-.2,.08,.5,0,gc+.05,-L/2+.1,K))}},
RevueltoSV:{n:'Lamborghini Revuelto SV',p:340000,c:0xc4161c,lx(L,w,H,hh,dh,B,C){const W=[1,1,1],R=[1,.05,.05],O=[1,.5,.05],o=[];for(const s of[1,-1])o.push(B(.85,.05,.07,s*.62,hh-.28,L/2+.05,W,0,0,-s*.28),B(.45,.05,.07,s*.3,hh-.46,L/2+.05,W,0,0,s*.75),B(.3,.04,.07,s*.78,hh-.4,L/2+.05,O));o.push(B(w-.45,.07,.07,0,dh-.08,-L/2-.05,R),B(.5,.1,.07,.55,dh-.22,-L/2-.05,R),B(.5,.1,.07,-.55,dh-.22,-L/2-.05,R));return o},mx:1.7,ac:1.75,sp:1,d:[4.95,2.03,1.14,.7,.82,.45,-.2,-1.15,-1.8],ex(P,bx,K,ch,L,w,H,hh,dh,gc,z1,z2,z3){const B=[.03,.03,.04];P.push(bx(w*.78,.035,1.5,0,hh+.02,L/2-1.5,B),bx(w*.62,.04,(z2-z3)*.9,0,H+.01,(z2+z3)/2,B),bx(w+.15,.06,.55,0,dh+.62,-L/2+.05,B),bx(.05,.5,.55,w/2+.07,dh+.4,-L/2+.05,B),bx(.05,.5,.55,-w/2-.07,dh+.4,-L/2+.05,B),bx(.08,.5,.08,.6,dh+.3,-L/2+.1,B),bx(.08,.5,.08,-.6,dh+.3,-L/2+.1,B),bx(w-.2,.08,.5,0,gc+.05,-L/2+.1,B))}},
Ferrari12:{n:'Ferrari 12Cilindri',p:420000,c:0xb3111a,lx(L,w,H,hh,dh,B,C){const W=[1,1,1],R=[1,.05,.05],o=[];for(const s of[1,-1])o.push(B(.75,.05,.07,s*.68,hh-.3,L/2+.04,W,0,0,s*.12),B(.5,.03,.07,s*.7,hh-.38,L/2+.04,W,0,0,s*.12),C(.15,.07,s*.55,dh-.14,-L/2-.05,R),C(.15,.07,s*.85,dh-.14,-L/2-.05,R));return o},mx:1.6,ac:1.5,sp:0,d:[4.73,1.94,1.29,.78,.88,.32,-.55,-1.25,-1.85],ex(P,bx,K,ch,L,w,H,hh,dh,gc,z1,z2,z3){const B=[.03,.03,.04];P.push(bx(w*.5,.03,1.2,0,hh+.015,L/2-1.2,B),bx(w*.6,.04,(z2-z3)*.85,0,H+.01,(z2+z3)/2,B),bx(w-.3,.05,.3,0,dh+.06,-L/2+.2,B))}},
JeepCJ:{n:'Classic Off-road Jeep CJ',p:9000,c:0xd0262b,lx(L,w,H,hh,dh,B,C){const W=[1,1,.9],R=[1,.05,.05],o=[];for(const s of[1,-1])o.push(C(.22,.1,s*.62,hh-.35,L/2+.05,W),C(.09,.1,s*.3,.62,L/2+.28,W),B(.14,.1,.06,s*.7,dh-.12,-L/2-.06,R));for(let i=-2;i<=2;i++)o.push(C(.09,.1,i*.22,H+.14,.7,W));return o},mx:1,ac:1.1,sp:0,d:[3.7,1.75,1.4,1,1.08,.55,.45,-1.55,-1.75],ex(P,bx,K,ch,L,w,H,hh,dh,gc){P.push(bx(w-.3,.1,.1,0,gc+.62,L/2+.2,ch),bx(.1,.5,.1,.5,gc+.4,L/2+.15,ch),bx(.1,.5,.1,-.5,gc+.4,L/2+.15,ch),bx(.1,.1,.1,.0,gc+.4,L/2+.15,ch),bx(.08,.65,.08,w/2-.1,H+.1,-1.55,K),bx(.08,.65,.08,-w/2+.1,H+.1,-1.55,K),bx(w-.2,.08,.08,0,H+.42,-1.55,K),{g:new THREE.CylinderGeometry(.36,.36,.26,14).rotateX(Math.PI/2).translate(0,.95,-L/2-.2),c:K},bx(w+.2,.08,.2,0,gc+.1,L/2+.05,K))}},
Jeep:{n:'Off-road Jeep',p:3500,c:0x4a6b2a,mx:.95,ac:1.05,d:[4.1,1.9,1.85,1.15,1.6,.95,.3,-1.9,-2]},Coupe:{n:'Sport Coupe',p:5500,c:0x8a1ab5,mx:1.12,ac:1.18,d:[4.3,1.8,1.25,.8,.9,.55,-.3,-1,-1.6]},Wagon:{n:'Family Wagon',p:2800,c:0x556b7a,mx:.95,ac:.95,d:[4.9,1.85,1.45,.85,1.1,.7,-.1,-2,-2.3]},Minibus:{n:'City Minibus',p:3800,c:0xf0f0f0,mx:.9,ac:.9,d:[5,2,2.1,1.2,2,1.5,1,-2.3,-2.4]},Lowrider:{n:'Lowrider Cruiser',p:6000,c:0xd4a017,mx:.9,ac:1,d:[5.2,1.95,1.25,.8,.9,.6,-.2,-1.5,-2.2]},Roadster:{n:'Roadster GT',p:11000,c:0xe01070,mx:1.28,ac:1.35,sp:1,d:[3.9,1.75,1.1,.7,.85,.4,-.1,-.8,-1.4]},Lambo:{n:'Lamborghini Aventador',p:18000,c:0xf2c200,mx:1.4,ac:1.5,sp:1,d:[4.8,2.05,1.14,.68,.9,.95,-.05,-1.1,-1.8]}},
MOTOS={Scooter:{n:'City Scooter',p:600,c:0xe8e8e8,mx:.75,ac:.8,sc:[.9,.9,.9]},Naked:{n:'Street Naked',p:1500,c:0x2ecc71,mx:1,ac:1},Chopper:{n:'Harley Chopper',p:3000,c:0x111111,mx:.95,ac:1,sc:[1,1,1.2]},
 Dirt:{n:'Dirt Bike',p:1200,c:0xff8a00,mx:.9,ac:1.1,sc:[.9,1,.95]},Cafe:{n:'Triumph Cafe Racer',p:2800,c:0x3a4a3a,mx:1,ac:1.1},Hayabusa:{n:'Suzuki Hayabusa',p:9000,c:0x222a55,mx:1.5,ac:1.6},Ducati:{n:'Ducati Panigale',p:4000,c:0xd10000,mx:1.2,ac:1.3},Ninja:{n:'Kawasaki Ninja H2',p:7500,c:0x18c93a,mx:1.35,ac:1.5}},NPCM=['Sedan','Muscle','SUV','Porsche','Pickup','Van','BMW','Taxi','Corvette','Hatch','Jeep','Coupe','Wagon','Minibus','Lowrider','Roadster','JeepCJ','Ferrari12','RevueltoSV','RevueltoBlack'];
CARMODELS.RevueltoBlack={...CARMODELS.RevueltoSV,n:'Lamborghini Revuelto (Matte Black)',c:0x0a0a0c,p:360000};CARMODELS.Batmobile={n:'Batmobile 1989',p:150000,c:0x0a0a0d,mx:1.55,ac:1.6,sp:1,d:[5.6,2.1,1.0,.6,.78,.45,-.1,-1.0,-1.7],ex(P,bx,K,ch,L,w,H,hh,dh,gc,z1,z2,z3){const B=[.04,.04,.05],G=[.1,.1,.12],Y=[1,.8,.1];for(const s of[1,-1])P.push(bx(.07,1.0,1.7,s*(w/2-.15),dh+.55,-L/2+.9,B),bx(.5,.14,2.4,s*(w/2-.05),hh+.05,L/2-1.5,B),bx(.4,.4,.6,s*.55,hh-.05,L/2+.1,G));P.push(bx(.6,.55,.9,0,hh+.15,L/2-.4,G),bx(.5,.45,.12,0,hh+.15,L/2+.1,Y),bx(.55,.1,2.0,0,H+.12,-.4,B),bx(w-.3,.1,.8,0,dh+.3,-L/2+.25,B))}};
CARMODELS.StealthGT={n:'Stealth GT (Matte Black)',p:45000,c:0x0b0b0e,mx:1.5,ac:1.55,sp:1,d:[4.8,2.02,1.12,.68,.85,.5,-.2,-1.1,-1.8]};
CARMODELS.BoxTruck={n:'Box Truck',p:7500,c:0xeeeeee,mx:.8,ac:.85,ci:[-2.4,-1.2,0,1.2,2.4],d:[7.6,2.4,2.8,1.5,1.2,2.9,2.4,1.3,1.2],ex(P,bx,K,ch,L,w,H,hh,dh,gc,z1,z2,z3){P.push(bx(w-.1,2.5,z3+L/2-.15,0,dh+1.3,(z3-.15-L/2)/2,[1,1,1]))}};
CARMODELS.FireTruck={n:'Fire Truck',p:24000,c:0xc40000,mx:.85,ac:.9,ci:[-2.8,-1.4,0,1.4,2.8],d:[8.4,2.5,3,1.6,1.3,3.1,2.6,1.5,1.4],ex(P,bx,K,ch,L,w,H,hh,dh,gc,z1,z2,z3){const l=z3+L/2-.15,c=(z3-.15-L/2)/2;P.push(bx(w-.1,1.6,l,0,dh+.8,c,[1,1,1]),bx(.7,.35,l*.9,0,dh+1.9,c,[.85,.85,.9]),bx(1.6,.2,.5,0,H+.12,z2-.3,[.1,.1,.6]),bx(2.6,.25,.5,0,dh+.25,-L/2-.1,K))}};
CARMODELS.ArmyTruck={n:'Army Truck',p:18000,c:0x55633a,mx:.9,ac:.95,ci:[-2.4,-1.2,0,1.2,2.4],d:[7.8,2.5,2.9,1.7,1.5,3,2.5,1.4,1.3],ex(P,bx,K,ch,L,w,H,hh,dh,gc,z1,z2,z3){const l=z3+L/2-.15,c=(z3-.15-L/2)/2;P.push(bx(w-.4,2.1,l,0,dh+1.25,c,[.9,.95,.8]),bx(w-.1,.35,l,0,dh+.1,c,K))}};
CARMODELS.SemiTruck={n:'Semi Truck + Trailer',p:28000,c:0xcfd6df,mx:.85,ac:.8,ci:[-4.2,-2.8,-1.4,0,1.4,2.8,4.2],d:[11.4,2.5,3.6,1.9,1.4,4.7,4.1,2.7,2.6],ex(P,bx,K,ch,L,w,H,hh,dh,gc,z1,z2,z3){P.push(bx(w,2.9,z3+L/2-.2,0,dh+1.6,(z3-.2-L/2)/2,[1,1,1]),bx(w-.2,.3,z3+L/2-.2,0,dh,(z3-.2-L/2)/2,K))}};
MOTOS.Vario={n:'Honda Vario (Black/Gold)',p:2400,c:0x0e0e10,mx:.95,ac:1,sc:[.95,.95,.95]};
Object.assign(MOTOS.Scooter,{nk:.7,fc:0x99ddff,dust:.8});Object.assign(MOTOS.Naked,{nk:1,fc:0xffa030,dust:1});Object.assign(MOTOS.Cafe,{nk:1,fc:0xffd060,dust:1});Object.assign(MOTOS.Dirt,{nk:1.1,fc:0xff7a20,dust:2.2});Object.assign(MOTOS.Chopper,{nk:.9,fc:0xff4020,dust:1.3});Object.assign(MOTOS.Ducati,{nk:1.2,fc:0xff3030,dust:.9});Object.assign(MOTOS.Ninja,{nk:1.35,fc:0x33ff77,dust:.9});Object.assign(MOTOS.Hayabusa,{nk:1.5,fc:0xaa55ff,dust:1});
const ld=(k,d)=>{try{return{...d,...JSON.parse(localStorage.getItem(k))}}catch(e){return d}},sv=(k,v)=>{try{localStorage.setItem(k,JSON.stringify(v))}catch(e){}},kn=c=>c.replace(/^Key|^Digit/,'');
const S=ld('gtaelfo_s',{mode:'pc',q:'high',vol:.8,fov:70,sens:1,fps:false,lang:'en'}),KB=ld('gtaelfo_k',{}),MBL=ld('gtaelfo_m',{});
const FAX={'ON':'روشن','OFF':'خاموش','Back':'بازگشت','Reset':'بازنشانی','Done':'تمام','Close':'بستن','Left':'چپ','Right':'راست','Forward':'جلو','Horn':'بوق','Punch':'مشت','Map':'نقشه','Shop':'شاپ','Pause':'توقف','Language':'زبان','Fullscreen':'تمام‌صفحه','Size':'اندازه','Armor':'زره','Medkit':'کمک‌های اولیه','Settings':'تنظیمات','Controls':'کنترل‌ها','Pistol':'تپانچه','SMG':'مسلسل SMG','Shotgun':'شاتگان','Rifle':'تفنگ تهاجمی','Sniper':'اسنایپر','Stock':'قنداق','Low':'پایین','Medium':'متوسط'};
const FA={'City posters (up to 5, any image size)':'پوسترهای شهر (تا ۵ عدد، هر سایز)','City posters':'پوسترهای شهر','Poster':'پوستر','Clear':'پاک کردن','Interact / talk':'تعامل / صحبت','Edit':'ویرایش','Posters appear on billboards along the city roads.':'پوسترها روی بیلبوردهای کنار خیابان‌ها نمایش داده می‌شن.','Start GTA_elfo':'شروع GTA_elfo','Resume GTA_elfo':'ادامه GTA_elfo','Paused':'مکث','SETTINGS':'تنظیمات','Control mode':'حالت کنترل','PC (default)':'کامپیوتر (پیش‌فرض)','MOBILE':'موبایل','Edit keys':'ویرایش کلیدها','Edit touch layout':'ویرایش چیدمان لمسی','Graphics quality':'کیفیت گرافیک','High (native pixels)':'بالا (پیکسل اصلی)','Ultra (1px, supersampled)':'اولترا (دقت ۱ پیکسل)','Field of view':'میدان دید','Master volume':'صدای کلی','Mouse / touch sensitivity':'حساسیت موس / لمس','Show FPS':'نمایش FPS','Camera view':'نمای دوربین','First person':'اول‌شخص','Third person':'سوم‌شخص','Cheat codes (type during play)':'کدهای تقلب (حین بازی تایپ کن)','PC KEYS — click an action, then press the new key':'کلیدهای کامپیوتر — روی یک عمل کلیک کن و کلید جدید را بزن','Restore defaults':'بازگرداندن پیش‌فرض','press a key…':'یک کلید بزن…',
'Back / brake':'عقب / ترمز','Sprint / Nitro':'دویدن / نیترو','Jump / handbrake':'پرش / ترمز دستی','Enter / exit vehicle':'سوار / پیاده شدن','Reload / Radio':'ریلود / رادیو','Reload / radio':'ریلود / رادیو','Shoot':'شلیک','Switch weapon':'تعویض سلاح','C4 place / detonate':'کار گذاشتن / منفجر کردن C4','C4 place / blow':'C4 کار بگذار / منفجر کن','Aim / Scope':'نشانه‌گیری / اسکوپ','Aim / scope':'نشانه‌گیری / اسکوپ','Air-suspension hop':'پرش تعلیق بادی','Forward / accelerate':'جلو / گاز',
'drag any button to move it':'هر دکمه را بکش تا جابه‌جا شود','Opacity %':'شفافیت ٪','Reset layout':'بازنشانی چیدمان',
'Infinite health (toggle)':'جان بی‌نهایت (روشن/خاموش)','Infinite money':'پول بی‌نهایت','All weapons + ammo':'همه سلاح‌ها + مهمات','Armor + full health':'زره + جان کامل','Clear wanted level':'پاک کردن ستاره‌ها','Wanted +2':'۲ ستاره بیشتر','Spawn Lamborghini':'ساخت لامبورگینی','Spawn Ferrari':'ساخت فراری','Full nitro (in vehicle)':'نیترو کامل','Blow up nearby cars':'منفجر کردن ماشین‌های اطراف','Unlimited upgrades (garage limits removed)':'ارتقای نامحدود (حذف محدودیت گاراژ)','Hyper-tune current vehicle + 9999 NOS':'تیون شدید ماشین فعلی + ۹۹۹۹ نیترو',
'HARBOR ARMS — weapons':'اسلحه‌فروشی — سلاح‌ها','ATTACHMENT LAB':'آزمایشگاه اتچمنت','PREMIUM MOTORS — cars':'نمایشگاه ماشین','TWO WHEELS — bikes':'نمایشگاه موتور','ELFO GARAGE — tuning':'گاراژ الفو — تیونینگ','CHALLENGE HALL — win cash':'سالن چالش — پول ببر','B closes.':'B برای بستن.',
'Ammo (equipped gun)':'مهمات (سلاح فعلی)','Armor plating':'زره‌پوش ماشین','Suppressor':'صداخفه‌کن','Long barrel':'لوله بلند','Short barrel':'لوله کوتاه','Scope (aim: RMB / Z)':'اسکوپ (نشانه: کلیک راست / Z)','Extended magazine':'خشاب بزرگ‌تر','Buy and equip a gun first.':'اول یک اسلحه بخر و بردار.','Nitro refill +100':'شارژ نیترو +۱۰۰','hold Shift':'نگه‌داشتن Shift','Engine / top speed':'موتور / سرعت','Handling / steering':'فرمان‌پذیری','Tires & brakes':'لاستیک و ترمز','Lv ':'سطح ','Spring height ▼ lower':'ارتفاع فنر ▼ پایین','Spring height ▲ raise':'ارتفاع فنر ▲ بالا','Wheel size ▼ smaller':'سایز چرخ ▼ کوچک‌تر','Wheel size ▲ bigger':'سایز چرخ ▲ بزرگ‌تر','Air suspension (V = hop)':'تعلیق بادی (V = پرش)','Air suspension kit':'کیت تعلیق بادی','Repaint (next color)':'رنگ بعدی','UNLIMITED mode on':'حالت نامحدود فعال','Drive a vehicle into the garage marker to tune it.':'برای تیون، با ماشین وارد نشانگر گاراژ شو.',
'Street Brawl: 8 KOs in 60s':'دعوای خیابانی: ۸ ناک‌اوت در ۶۰ ثانیه','win $2,500':'جایزه $2,500','Time Attack: reach the red marker (drive!)':'مسابقه زمانی: برو به نقطه قرمز (با ماشین!)','Survive the Heat: 3 stars for 60s':'فرار از پلیس: ۶۰ ثانیه با ۳ ستاره','win $6,000':'جایزه $6,000','Abandon current challenge':'رها کردن چالش','Pick a challenge. Fight, race or survive.':'یک چالش انتخاب کن.',
'Press F to enter vehicle':'برای سوار شدن F را بزن','Press F to exit (when landed)':'برای پیاده شدن F را بزن (بعد از فرود)','Press F to board':'F را بزن تا سوار شوی:','Press B —':'برای ورود B —',
'3 STARS — POLICE HELICOPTER!':'۳ ستاره — هلیکوپتر پلیس!','5 STARS — TANK DEPLOYED!':'۵ ستاره — تانک آمد!','C4 detonated':'C4 منفجر شد','C4 placed — press X again to detonate':'C4 کار گذاشته شد — دوباره X بزن','Carjacked! The driver is on the ground':'ماشین را گرفتی! راننده روی زمین افتاد','Challenge failed':'چالش شکست خورد','Challenge started!':'چالش شروع شد!','CHALLENGE COMPLETE!':'چالش کامل شد!','Cheat: ':'تقلب: ','Crashed: ':'سقوط: ','hard landing':'فرود سخت','collision':'برخورد','Equip a gun first':'اول یک اسلحه بردار','Land and slow below 90 km/h first':'اول فرود بیا و سرعت را زیر ۹۰ کم کن','Mission failed: out of time':'ماموریت شکست خورد: زمان تمام شد','Not enough cash':'پول کافی نیست','Out of ammo':'مهمات تمام شد','Turn back: edge of the city':'برگرد: لبه شهر','Waypoint set':'نقطه مسیر گذاشته شد','delivered outside':'بیرون تحویل داده شد','purchased':'خریداری شد','equipped':'برداشته شد','MISSION PASSED!':'ماموریت موفق!','WASTED':'مردی','Get in a vehicle':'سوار ماشین شو','Drive to the red marker':'برو به نقطه قرمز','Radio off':'رادیو خاموش','Walk into a shop marker (map: M)':'وارد نشانگر شاپ شو (نقشه: M)','Buy a gun at Harbor Arms (B)':'از اسلحه‌فروشی اسلحه بخر (B)','Shift: throttle':'Shift: گاز','Space: brake':'Space: ترمز','W/S: pitch':'W/S: بالا/پایین','A/D: bank':'A/D: چرخش','J: missile (jets)':'J: موشک (جنگنده)','BRAWL':'دعوا','SURVIVE THE HEAT':'فرار از پلیس','TIME ATTACK':'مسابقه زمانی','reach the red marker in time':'به موقع به نقطه قرمز برس'};
Object.assign(FA,{'ASTRA SPACEWORKS — spacecraft':'آسترا اسپیس‌ورکس — فضاپیما','Press F to leave the ship':'برای پیاده شدن از فضاپیما F را بزن','LIFTOFF!':'پرتاب!','AUTO LAND engaged — G to cancel':'فرود خودکار فعال شد — برای لغو G بزن','Manual control':'کنترل دستی','AUTO LANDING':'فرود خودکار','AUTO LAND: ON':'فرود خودکار: روشن','AUTO LAND':'فرود خودکار','Auto land (on Nova)':'فرود خودکار (روی نوا)','You jumped! Press SPACE to open the parachute':'پریدی! اسپیس رو بزن تا چتر باز بشه','Parachute open — steer with W/A/S/D':'چتر باز شد — با W/A/S/D هدایت کن','Press SPACE to open the parachute!':'اسپیس رو بزن تا چتر باز بشه!','Too late for the parachute!':'برای چتر خیلی دیر شد!','Soft landing':'فرود نرم','Press F: exit when landed · in the air: jump out (then SPACE = parachute)':'F: پیاده شدن بعد از فرود · توی هوا: پریدن بیرون (بعد اسپیس = چتر)','WARP DRIVE':'موتور پرش','APPROACHING NOVA':'نزدیک شدن به سیاره نوا','CRASHED':'سقوط کردی','PERFECT LANDING':'فرود عالی','LANDING COMPLETE':'فرود موفق','from center':'از مرکز','Landed off the pad — no bonus':'خارج از سکو نشستی — جایزه نداره','Shift: thrust · Space: hover · W/A/S/D: tilt · land softly on the glowing pad':'Shift: نیرو · Space: ثابت ماندن · W/A/S/D: کج کردن · آروم روی سکوی درخشان بشین','Press T: warp to planet NOVA · F: return to Earth':'برای پرش به سیاره نوا T و برای برگشت به زمین F را بزن','Warp to Nova (in orbit)':'پرش به نوا (در مدار)','MAX-Q':'فشار بیشینه','STAGE SEPARATION':'جدا شدن مرحله','ORBIT ACHIEVED':'رسیدیم به مدار','Press L to launch · F to leave the ship':'برای پرتاب L و برای پیاده شدن F را بزن','Press F to return to Earth':'برای بازگشت به زمین F را بزن','Back on Earth':'بازگشت به زمین','Launch (in spacecraft)':'پرتاب (داخل فضاپیما)','Spacecraft are delivered to the pad outside. Walk up and press F to board.':'فضاپیما روی سکوی بیرون تحویل می‌شه. برو جلو و F بزن تا سوار شی.','Boarded. Press L to launch.':'سوار شدی. برای پرتاب L را بزن.','GHOST MODE ON: pass through everything':'حالت روح روشن: عبور از همه چیز','Ghost mode OFF':'حالت روح خاموش','Ghost mode':'حالت روح','GHOST':'روح','Press F: exit the ship · L: return to Earth':'F: پیاده شدن از فضاپیما · L: برگشت به زمین','Press F to board the ship · L: return to Earth':'F: سوار شدن به فضاپیما · L: برگشت به زمین','Go back to your ship first':'اول برگرد کنار فضاپیما','Back aboard · L: return to Earth':'سوار شدی · L: برگشت به زمین','Nova City · walk to the ship and press F to board':'شهر نوا · برای سوار شدن برگرد کنار فضاپیما و F بزن','NOVA CITY':'شهر نوا','GAMEPAD':'دسته بازی','Previous weapon':'سلاح قبلی','Previous radio station':'ایستگاه رادیو قبلی','Toggle fullscreen':'تمام‌صفحه','Cycle graphics quality':'تغییر کیفیت گرافیک','Screenshot':'اسکرین‌شات','Mute / unmute':'قطع / وصل صدا','FOV −':'کاهش میدان دید','FOV +':'افزایش میدان دید','FPS counter':'نمایشگر FPS','Fists / unarmed':'مشت (بدون سلاح)','INSANE (4x supersampling)':'دیوانه‌وار (۴ برابر پیکسل)','Screenshot saved':'اسکرین‌شات ذخیره شد','Weapon slot 1':'اسلات سلاح 1','Weapon slot 2':'اسلات سلاح 2','Weapon slot 3':'اسلات سلاح 3','Weapon slot 4':'اسلات سلاح 4','Weapon slot 5':'اسلات سلاح 5','Weapon slot 6':'اسلات سلاح 6','Gamepad connected — GAMEPAD mode on':'دسته وصل شد — حالت دسته فعال شد','Gamepad connected — press any button':'دسته وصل شد — یک دکمه بزن','Gamepad disconnected':'دسته قطع شد','Edit gamepad buttons':'ویرایش دکمه‌های دسته','GAMEPAD BUTTONS — click an action, then press a button on the pad':'دکمه‌های دسته — روی یک عمل کلیک کن و دکمه جدید رو روی دسته بزن','Gamepad connected':'دسته وصل شد','No gamepad detected — press any button on it':'دسته‌ای پیدا نشد — یک دکمه روش بزن','Left stick: move · Right stick: camera · In vehicles RT/LT = gas/brake':'استیک چپ: حرکت · استیک راست: دوربین · داخل ماشین RT/LT = گاز/ترمز'});
let FAK=[],tr=s=>{if(S.lang!=='fa'||typeof s!=='string')return s;if(FAX[s])return FAX[s];let o=s;for(const k of FAK)if(o.includes(k))o=o.split(k).join(FA[k]);return o};
Object.assign(FA,{'Press F to board the Nova Hover':'برای سوار شدن به Nova Hover کلید F را بزن','Press F to board Nova Hover':'برای سوار شدن به Nova Hover کلید F را بزن','F: exit (land first) · Shift: rise · Space: descend/land':'F: پیاده شدن (اول فرود) · Shift: بالا · Space: پایین آمدن/فرود','NOVA CITY · JETPACK: buy at Nova Outfitters (B)':'شهر نوا · جت‌پک: از Nova Outfitters بخر (B)','NOVA CITY':'شهر نوا','Jetpack grip pack — low-gravity flight':'کوله جت‌پک — پرواز در جاذبه کم','✓ Jetpack (equipped)':'✓ جت‌پک (نصب شده)','Jetpack already equipped':'جت‌پک قبلاً نصبه','Jetpack equipped — jump, then hold SPACE':'جت‌پک نصب شد — بپر و بعد SPACE را نگه دار','Buy the jetpack first':'اول جت‌پک بخر','Jetpack refilled':'سوخت جت پر شد','Jet fuel refill (':'سوخت جت (','Nova has low gravity: jump first, then hold SPACE to fly. Fuel refills on the ground.':'نوا جاذبه کم دارد: اول بپر بعد SPACE را نگه دار تا پرواز کنی. سوخت روی زمین پر می‌شود.','Nova City · low gravity: jump + hold SPACE to jetpack · F: hover car / ship · L: Earth':'شهر نوا · جاذبه کم: بپر و SPACE را نگه دار تا جت‌پک · F: ماشین پرنده/فضاپیما · L: زمین','Nova City · jetpack for sale at Nova Outfitters (B) · F: hover car / ship · L: Earth':'شهر نوا · جت‌پک در Nova Outfitters فروخته می‌شود (B) · F: ماشین پرنده/فضاپیما · L: زمین','Land and exit the hover car first (F)':'اول فرود بیا و از ماشین پرنده پیاده شو (F)'});
Object.assign(FA,{'WING TORN OFF!':'بال کنده شد!','Lost control — press F to bail out!':'کنترل از دست رفت — F بزن تا بپری بیرون!','Crashed: crashed after losing a wing':'سقوط کردی'});FAK=Object.keys(FA).sort((a,b)=>b.length-a.length);
const BINDS=[['Forward','KeyW'],['Back / brake','KeyS'],['Left','KeyA'],['Right','KeyD'],['Sprint / Nitro','ShiftLeft'],['Jump / handbrake','Space'],['Enter / exit vehicle','KeyF'],['Horn','KeyH'],['Reload / Radio','KeyR'],['Shoot','KeyJ'],['Punch','KeyK'],['Switch weapon','KeyQ'],['C4 place / detonate','KeyX'],['Shop','KeyB'],['Map','KeyM'],['Aim / Scope','KeyZ'],['Air-suspension hop','KeyV'],['Pause','KeyP'],['Interact / talk','KeyE'],['Launch (in spacecraft)','KeyL'],['Warp to Nova (in orbit)','KeyT'],['Auto land (on Nova)','KeyG'],['Previous weapon','KeyC'],['Previous radio station','KeyN'],['Toggle fullscreen','KeyU'],['Cycle graphics quality','KeyI'],['Screenshot','KeyO'],['Mute / unmute','KeyY'],['FOV −','BracketLeft'],['FOV +','BracketRight'],['FPS counter','F3'],['Fists / unarmed','Digit0'],['Weapon slot 1','Digit1'],['Weapon slot 2','Digit2'],['Weapon slot 3','Digit3'],['Weapon slot 4','Digit4'],['Weapon slot 5','Digit5'],['Weapon slot 6','Digit6']];
const MB=[['JOY','KeyW',13,66,'Joystick (forward / back / left / right)'],['SPR','ShiftLeft',31,80,'Sprint / Nitro'],['JMP','Space',72,82,'Jump / handbrake'],['SHT','KeyJ',90,66,'Shoot'],['AIM','KeyZ',79,60,'Aim / scope'],['RLD','KeyR',64,70,'Reload / radio'],['ENT','KeyF',90,42,'Enter / exit vehicle'],['PUN','KeyK',88,86,'Punch'],['WPN','KeyQ',76,38,'Switch weapon'],['HRN','KeyH',5,50,'Horn'],['C4','KeyX',5,36,'C4 place / blow'],['HOP','KeyV',62,86,'Air-suspension hop'],['SHP','KeyB',36,12,'Shop'],['MAP','KeyM',46,12,'Map'],['PSE','KeyP',56,12,'Pause'],['INT','KeyE',90,24,'Interact / talk'],['LCH','KeyL',24,12,'Launch'],['WRP','KeyT',24,26,'Warp'],['ALD','KeyG',76,26,'Auto land']];
const CHEATS=[['wwsdsksadsjj_ffwsdsa',G=>{G.god=!G.god;G.health=100},'Infinite health (toggle)'],['wsdawdsawds__qkj',G=>{G.rich=true;G.money=999999999;G.cash(0)},'Infinite money'],
['sdwajk_wdsa',G=>{for(const n of GUNS){G.own.add(n);G.am[n]=(G.am[n]||0)+WEAP[n].ammo*3;G.mag[n]=MAG[n]}},'All weapons + ammo'],['wasdwasd_kk',G=>{G.armor=100;G.health=100},'Armor + full health'],
['ssaawwdd_jk',G=>G.setWanted(0),'Clear wanted level'],['wdwdwd_jjk',G=>G.addWanted(2),'Wanted +2'],['dsaw_ffdwas',G=>G.spawnCar('Lambo'),'Spawn Lamborghini'],['dsaw_ffsawd',G=>G.spawnCar('Ferrari'),'Spawn Ferrari'],
['aawwddsskkhjjllmmk_',G=>{G.god=true;G.health=100;G.armor=100;G.rich=true;G.over=true;G.money=999999999;G.nit=9999;G.cash(0);for(const n of GUNS){G.own.add(n);G.am[n]=999;G.mag[n]=MAG[n]}},'EVERYTHING: god mode, infinite money, all weapons, nitro, all upgrades'],['wawdsw__fj',G=>{G.nit=500},'Full nitro (in vehicle)'],['aadwwss_jj',G=>{for(const c of G.cars.slice())if(!c.wreck&&c!==G.driving&&Math.hypot(c.x-G.player.x,c.z-G.player.z)<40)G.explode(c)},'Blow up nearby cars'],['wwddaa_ssjk_f',G=>{G.over=true},'Unlimited upgrades (garage limits removed)'],['ssddww_aajj_k',G=>{G.nit=9999;if(G.driving){G.driving.f.max*=1.5;G.driving.f.acc*=1.5;G.driving.hp+=300}},'Hyper-tune current vehicle + 9999 NOS']];
function push(x,z,r,b){const cx=U.clamp(x,b.x0,b.x1),cz=U.clamp(z,b.z0,b.z1),dx=x-cx,dz=z-cz,d2=dx*dx+dz*dz;
 if(d2>=r*r)return null;if(d2>1e-8){const d=Math.sqrt(d2);return[dx/d,dz/d,r-d]}
 const l=x-b.x0,rr=b.x1-x,t=z-b.z0,bt=b.z1-z,m=Math.min(l,rr,t,bt);
 return m===l?[-1,0,l+r]:m===rr?[1,0,rr+r]:m===t?[0,-1,t+r]:[0,1,bt+r]}
function merge(parts){const P=[],N=[],T=[],K=[],I=[];let o=0;
 for(const p of parts){const g=p.g,pa=g.attributes.position,na=g.attributes.normal,ua=g.attributes.uv;
  for(let i=0;i<pa.count;i++){P.push(pa.getX(i),pa.getY(i),pa.getZ(i));N.push(na.getX(i),na.getY(i),na.getZ(i));
   let u=ua.getX(i),v=ua.getY(i);if(p.uv)[u,v]=p.uv(i>>2,u,v);T.push(u,v);K.push(p.c[0],p.c[1],p.c[2])}
  for(const x of(g.index?g.index.array:[...Array(pa.count).keys()]))I.push(x+o);o+=pa.count}
 const m=new THREE.BufferGeometry();m.setAttribute('position',new THREE.Float32BufferAttribute(P,3));m.setAttribute('normal',new THREE.Float32BufferAttribute(N,3));
 m.setAttribute('uv',new THREE.Float32BufferAttribute(T,2));m.setAttribute('color',new THREE.Float32BufferAttribute(K,3));m.setIndex(I);return m}
/* ===== INPUT ===== */
const GPD={ShiftLeft:10,Space:0,KeyF:1,KeyR:2,KeyQ:3,KeyH:4,KeyK:5,KeyZ:6,KeyJ:7,KeyM:8,KeyP:9,KeyV:11,KeyB:12,KeyE:13,KeyL:14,KeyT:15},GP=ld('gtaelfo_g',GPD),GPN=['A','B','X','Y','LB','RB','LT','RT','Select','Start','L3','R3','D-Up','D-Down','D-Left','D-Right','Home'],PAD={prev:[],act:{},pb:null,gp:false};
const padSet=(c,v)=>{if(!!Game.inp.k[c]===!!v)return;Game.inp.k[c]=v?1:0;if(v&&Game.state==='PLAYING')Game.onKey(c)};
function pollPad(){if(typeof Game==='undefined'||!Game||!Game.inp)return;const gp=(navigator.getGamepads?[...navigator.getGamepads()]:[]).find(g=>g&&g.connected);PAD.gp=!!gp;const st=document.getElementById('padst');if(st)st.textContent=tr(gp?'Gamepad connected':'No gamepad detected — press any button on it')+(gp?' — '+gp.id.slice(0,36):'');
 if(gp&&S.mode!=='pad'&&gp.buttons.some((x,n)=>(x.pressed||x.value>.5)&&!PAD.prev[n])){S.mode='pad';sv('gtaelfo_s',S);Game.showMob();if(Game.toast)Game.toast('Gamepad connected — GAMEPAD mode on');if($('set').style.display==='flex')Game.drawSet();PAD.prev=gp.buttons.map(x=>x.pressed);return}
 if(!gp||S.mode!=='pad'){for(const c in PAD.act)if(PAD.act[c])padSet(c,0);PAD.act={};if(gp)PAD.prev=gp.buttons.map(x=>x.pressed);return}
 const b=gp.buttons.map(x=>x.pressed||x.value>.5),pv=PAD.prev,ax=gp.axes;
 if(PAD.pb){const i=b.findIndex((v,n)=>v&&!pv[n]);if(i>=0){for(const k in GP)if(GP[k]===i)GP[k]=-1;GP[PAD.pb]=i;sv('gtaelfo_g',GP);PAD.pb=null;Game.drawSet()}PAD.prev=b;return}
 if($('screen').style.display!=='none'&&$('set').style.display!=='flex'){if((b[0]&&!pv[0])||(b[9]&&!pv[9]))$('bStart').click();PAD.prev=b;return}
 const want={},dr=!!Game.driving;for(const[n,d]of BINDS){const i=GP[d];if(i>=0&&b[i])want[d]=1}
 if(dr){if(GP.KeyJ===7)want.KeyJ=0;if(GP.KeyZ===6)want.KeyZ=0;if(b[7])want.KeyW=1;if(b[6])want.KeyS=1}
 const lx=ax[0]||0,ly=ax[1]||0;if(lx<-.35)want.KeyA=1;if(lx>.35)want.KeyD=1;if(ly<-.35)want.KeyW=1;if(ly>.35)want.KeyS=1;
 for(const c of new Set([...Object.keys(PAD.act),...Object.keys(want)]))padSet(c,!!want[c]);PAD.act=want;
 if(Game.state==='PLAYING'){const rx=ax[2]||0,ry=ax[3]||0;if(Math.abs(rx)>.15)Game.inp.dx+=rx*14*S.sens;if(Math.abs(ry)>.15)Game.inp.dy+=ry*10*S.sens}
 PAD.prev=b}
setInterval(pollPad,16);addEventListener('gamepadconnected',()=>{if(window.Game&&Game.toast)Game.toast('Gamepad connected — press any button')});addEventListener('gamepaddisconnected',()=>{if(window.Game&&Game.toast)Game.toast('Gamepad disconnected')});
class Input{constructor(){this.k={};this.dx=0;this.dy=0;this.btn=false;this.locked=false;
 addEventListener('keydown',e=>{if(['Space','F3'].includes(e.code))e.preventDefault();if(Game.binding){e.preventDefault();Game.bindKey(e.code);return}Game.cheatKey(e);const c=Game.kmap(e.code);this.k[c]=1;if(!e.repeat)Game.onKey(c)});
 addEventListener('keyup',e=>this.k[Game.kmap(e.code)]=0);addEventListener('contextmenu',e=>e.preventDefault());
 addEventListener('mousedown',e=>{if(e.button===0)this.btn=true;if(e.button===2)this.k.KeyZ=1});addEventListener('mouseup',e=>{this.btn=false;if(e.button===2)this.k.KeyZ=0});
 addEventListener('mousemove',e=>{if(this.locked||this.btn){this.dx+=e.movementX;this.dy+=e.movementY}})}}
/* ===== AUDIO ===== */
const RADIO=[null,{name:'NEON WAVE 88.1',bpm:104,wave:'sawtooth',root:55,seq:[0,0,12,0,7,7,12,5,0,0,12,0,10,10,7,5],lead:[12,15,19,15,12,10,7,10],kick:4},
 {name:'HARBOR FM 94.5',bpm:88,wave:'triangle',root:41.2,seq:[0,0,-1,0,3,3,0,-5],lead:[7,10,12,10,7,5],kick:3},
 {name:'K-ROCKET 101.1',bpm:140,wave:'square',root:82.4,seq:[0,0,0,7,0,0,5,3],lead:null,kick:2},
 {name:'DESERT STORM 97.3',bpm:120,wave:'sawtooth',root:49,seq:[0,0,1,0,4,4,5,4,7,7,5,4,1,1,0,0],lead:[12,13,16,17,16,13,12,9],kick:4},
 {name:'LO-FI NIGHTS 90.2',bpm:74,wave:'triangle',root:55,seq:[0,0,-2,-2,3,3,-5,-5],lead:[12,15,14,10,7,10],kick:4},
 {name:'DISCO FEVER 111.0',bpm:118,wave:'sawtooth',root:65.4,seq:[0,12,0,12,5,17,5,17,7,19,7,19,3,15,3,15],lead:[19,24,22,19,17,19],kick:4},
 {name:'JAZZ HARBOR 106.4',bpm:96,wave:'triangle',root:73.4,seq:[0,4,7,11,9,5,2,-1,0,3,7,10,8,5,3,0],lead:[14,16,19,21,19,16,14,11],kick:8},
 {name:'ELFO TRAP 99.9',bpm:142,wave:'square',root:36.7,seq:[0,0,0,0,-2,-2,3,3],lead:[24,22,19,22,24,27],kick:6},
 {name:'METAL 666 FM',bpm:168,wave:'square',root:41.2,seq:[0,0,1,0,0,3,0,-2,0,0,1,0,6,5,3,1],lead:[12,13,12,15,12,18],kick:2},
 {name:'CLASSIC ORCHESTRA 88.8',bpm:66,wave:'sine',root:98,seq:[0,4,7,12,7,4,0,-5,-3,0,4,9,7,4,0,-3],lead:[24,23,19,16,19,24,28,24],kick:16},
 {name:'PERSIAN GROOVE 103.7',bpm:100,wave:'sawtooth',root:55,seq:[0,1,4,5,7,5,4,1,0,1,4,5,8,7,5,4],lead:[12,13,16,17,19,17,16,13],kick:4}];
class Sfx{constructor(){this.on=false}
 init(){if(this.on)return;try{const c=this.c=new(window.AudioContext||window.webkitAudioContext)(),o=c.createOscillator();o.type='sawtooth';const mg=c.createGain();mg.gain.value=S.vol;mg.connect(c.destination);Object.defineProperty(c,'destination',{value:mg});this.mg=mg;
  const f=c.createBiquadFilter();f.type='lowpass';f.frequency.value=380;this.ef=f;this.eg=c.createGain();this.eg.gain.value=0;o.connect(f);f.connect(this.eg);this.eg.connect(c.destination);o.start();this.eo=o;
  this.hg=c.createGain();this.hg.gain.value=0;this.hg.connect(c.destination);for(const fr of[400,500]){const h=c.createOscillator();h.type='square';h.frequency.value=fr;h.connect(this.hg);h.start()}
  const b=c.createBuffer(1,c.sampleRate,c.sampleRate),d=b.getChannelData(0);for(let i=0;i<d.length;i++)d[i]=Math.random()*2-1;
  const n=c.createBufferSource();n.buffer=b;n.loop=true;const bp=c.createBiquadFilter();bp.type='bandpass';bp.frequency.value=1800;bp.Q.value=2;
  this.sg=c.createGain();this.sg.gain.value=0;n.connect(bp);bp.connect(this.sg);this.sg.connect(c.destination);n.start();this.nb=b;{const jn=c.createBufferSource();jn.buffer=b;jn.loop=true;const jf=this.jf=c.createBiquadFilter();jf.type='lowpass';jf.frequency.value=900;this.jg=c.createGain();this.jg.gain.value=0;jn.connect(jf);jf.connect(this.jg);this.jg.connect(c.destination);jn.start()}const so=this.so=c.createOscillator();so.type='triangle';this.sn=c.createGain();this.sn.gain.value=0;so.connect(this.sn);this.sn.connect(c.destination);so.start();this.on=true}catch(e){}}
 beep(fr=660){if(!this.on)return;const c=this.c,o=c.createOscillator(),g=c.createGain();o.frequency.value=fr;g.gain.setValueAtTime(.06,c.currentTime);g.gain.exponentialRampToValueAtTime(.001,c.currentTime+.15);o.connect(g);g.connect(c.destination);o.start();o.stop(c.currentTime+.16)}
 shot(v=1){if(!this.on)return;const c=this.c,n=c.createBufferSource(),g=c.createGain();n.buffer=this.nb;g.gain.setValueAtTime(.25*v,c.currentTime);g.gain.exponentialRampToValueAtTime(.001,c.currentTime+.18);n.connect(g);g.connect(c.destination);n.start(c.currentTime,Math.random()*.5,.2)}

 msl(){if(!this.on)return;const c=this.c,t=c.currentTime,n=c.createBufferSource(),g=c.createGain(),f=c.createBiquadFilter();n.buffer=this.nb;n.loop=true;f.type='bandpass';f.Q.value=.8;f.frequency.setValueAtTime(3000,t);f.frequency.exponentialRampToValueAtTime(300,t+1.4);g.gain.setValueAtTime(.35,t);g.gain.exponentialRampToValueAtTime(.001,t+1.5);n.connect(f);f.connect(g);g.connect(c.destination);n.start(t);n.stop(t+1.6);const o=c.createOscillator(),og=c.createGain();o.type='sawtooth';o.frequency.setValueAtTime(400,t);o.frequency.exponentialRampToValueAtTime(70,t+.6);og.gain.setValueAtTime(.12,t);og.gain.exponentialRampToValueAtTime(.001,t+.7);o.connect(og);og.connect(c.destination);o.start(t);o.stop(t+.8)}
 bm(r){if(!this.on)return;const c=this.c,t=c.currentTime,o=c.createOscillator(),g=c.createGain();o.type='sine';o.frequency.setValueAtTime(110,t);o.frequency.exponentialRampToValueAtTime(30,t+.6);g.gain.setValueAtTime(.5,t);g.gain.exponentialRampToValueAtTime(.001,t+.8);o.connect(g);g.connect(c.destination);o.start(t);o.stop(t+.9);this.shot(1.6)}
 radio(n){clearInterval(this.ri);if(!this.on||!n)return;const S=RADIO[n],c=this.c,dur=30/S.bpm;let k=0;
  this.ri=setInterval(()=>{const t=c.currentTime+.05,st=k++%16,o=c.createOscillator(),g=c.createGain();
   o.type=S.wave;o.frequency.value=S.root*Math.pow(2,S.seq[st%S.seq.length]/12);g.gain.setValueAtTime(.07,t);g.gain.exponentialRampToValueAtTime(.001,t+dur*.9);o.connect(g);g.connect(c.destination);o.start(t);o.stop(t+dur);
   if(S.lead&&st%2===0){const l=c.createOscillator(),lg=c.createGain();l.type='square';l.frequency.value=S.root*4*Math.pow(2,S.lead[(st>>1)%S.lead.length]/12);lg.gain.setValueAtTime(.025,t);lg.gain.exponentialRampToValueAtTime(.001,t+dur*1.6);l.connect(lg);lg.connect(c.destination);l.start(t);l.stop(t+dur*1.7)}
   if(st%S.kick===0){const b=c.createOscillator(),bg=c.createGain();b.frequency.setValueAtTime(140,t);b.frequency.exponentialRampToValueAtTime(40,t+.12);bg.gain.setValueAtTime(.25,t);bg.gain.exponentialRampToValueAtTime(.001,t+.15);b.connect(bg);bg.connect(c.destination);b.start(t);b.stop(t+.16)}
   if(st%2===1){const h=c.createBufferSource(),hg=c.createGain();h.buffer=this.nb;hg.gain.setValueAtTime(.05,t);hg.gain.exponentialRampToValueAtTime(.001,t+.04);h.connect(hg);hg.connect(c.destination);h.start(t,0,.05)}},dur*1000)}
 update(sp,drv,horn,slip,sir,kd){if(!this.on)return;const t=this.c.currentTime;this.so.frequency.setTargetAtTime(850+250*Math.sin(t*7),t,.02);this.sn.gain.setTargetAtTime(sir?.03:0,t,.1);const k=kd||'car';let ty='sawtooth',f0=45,f1=140,ff=380,g0=.04,g1=.05,jg=0,jf=1200;
  if(k==='moto'){ty='square';f0=80;f1=300;ff=900;g0=.03;g1=.04}else if(k==='prop'){f0=62;f1=110;ff=700;g0=.05;g1=.05}else if(k==='jet'){f0=90;f1=240;ff=1800;g0=.015;g1=.03;jg=.06+.16*sp;jf=500+sp*1800}else if(k==='heli'){ty='square';f0=22;f1=14;ff=260;g0=.06;g1=.03;jg=.03}
  if(this.ty!==ty){this.eo.type=ty;this.ty=ty}this.eo.frequency.setTargetAtTime(f0+sp*f1,t,.05);this.ef.frequency.setTargetAtTime(ff,t,.1);this.jg.gain.setTargetAtTime(drv?jg:0,t,.15);this.jf.frequency.setTargetAtTime(jf,t,.1);const ch=k==='heli'?.6+.4*Math.sin(t*38):1;
  this.eg.gain.setTargetAtTime(drv?(g0+g1*sp)*ch:0,t,k==='heli'?.02:.1);this.hg.gain.setTargetAtTime(horn?.08:0,t,.02);this.sg.gain.setTargetAtTime(slip?.05:0,t,.05)}}
/* ===== WORLD ===== */
class Grid{constructor(c){this.c=c;this.m=new Map()}
 key(i,j){return(i+100)*1000+j+100}
 add(b,p=3){const c=this.c;for(let i=Math.floor((b.x0-p)/c);i<=Math.floor((b.x1+p)/c);i++)for(let j=Math.floor((b.z0-p)/c);j<=Math.floor((b.z1+p)/c);j++){const k=this.key(i,j);if(!this.m.has(k))this.m.set(k,[]);this.m.get(k).push(b)}}
 at(x,z){return this.m.get(this.key(Math.floor(x/this.c),Math.floor(z/this.c)))||EMPTY}}
const TOPD=new THREE.Color(0x2f62b8),TOPN=new THREE.Color(0x01020a),NIGHT=new THREE.Color(0x070b1a),DAY=new THREE.Color(0x87b5e8),DUSK=new THREE.Color(0xff8a5c);
class World{
 tex(w,h,draw,rep){const c=document.createElement('canvas');c.width=w;c.height=h;draw(c.getContext('2d'),w,h);const t=new THREE.CanvasTexture(c);t.anisotropy=16;if(rep){t.wrapS=t.wrapT=THREE.RepeatWrapping;t.repeat.set(rep,rep)}return t}
 constructor(scene){
  const R=this.R=U.rng(C.seed),L=this.L=[];for(let i=0;i<=10;i++)L.push(-600+C.step*i);
  this.scene=scene;this.grid=new Grid(C.cell);this.boxes=[];this.parks=[];this.edge=false;this.hour=C.start;this.night=0;this.sky=new THREE.Color();
  const hw=this.hw=i=>(C.aves.includes(i)?C.aveW:C.roadW)/2;
  const near=c=>{const i=U.clamp(Math.round((c+600)/C.step),0,10);return Math.abs(c-L[i])<hw(i)+2};
  const D=new THREE.Object3D(),put=(m,n,x,y,z,sx,sy,sz,ry=0)=>{D.position.set(x,y,z);D.scale.set(sx,sy,sz);D.rotation.y=ry;D.updateMatrix();m.setMatrixAt(n,D.matrix)};
  const inst=(g,m,n)=>{const o=new THREE.InstancedMesh(g,m,n);o.frustumCulled=false;scene.add(o);return o};
  const std=(c,r=.9)=>new THREE.MeshStandardMaterial({color:c,roughness:r});
  const tbox=(x,z,k)=>{const b={x0:x-.55*k,x1:x+.55*k,z0:z-.55*k,z1:z+.55*k,h:7,tr:1};this.boxes.push(b);this.grid.add(b)};
  scene.background=this.sky;scene.fog=new THREE.Fog(0x88aacc,160,1000);
  this.du={top:{value:new THREE.Color(0x2f62b8)},hor:{value:new THREE.Color(0x88aacc)},sd:{value:new THREE.Vector3(0,1,0)},nt:{value:0}};
  this.dome=new THREE.Mesh(new THREE.SphereGeometry(700,24,12),new THREE.ShaderMaterial({uniforms:this.du,side:THREE.BackSide,depthWrite:false,fog:false,
   vertexShader:'varying vec3 vP;void main(){vP=normalize(position);gl_Position=projectionMatrix*modelViewMatrix*vec4(position,1.);}',
   fragmentShader:'uniform vec3 top,hor,sd;uniform float nt;varying vec3 vP;float h(vec3 p){return fract(sin(dot(p,vec3(12.9,78.2,37.7)))*43758.5);}void main(){float y=max(vP.y,0.);vec3 c=mix(hor,top,pow(y,.55));float g=max(dot(vP,sd),0.);c+=vec3(1.,.85,.6)*pow(g,220.)*(1.-nt*.5)+vec3(1.,.6,.3)*pow(g,6.)*.18;float st=step(.9972,h(floor(vP*240.)))*nt*step(.08,vP.y);c+=vec3(st);gl_FragColor=vec4(c,1.);}'}));
  this.dome.renderOrder=-10;this.dome.frustumCulled=false;scene.add(this.dome);
  this.hemi=new THREE.HemisphereLight(0xcfe4ff,0x555555,.7);this.sun=new THREE.DirectionalLight(0xffffff,1);
  const sc=this.sun.shadow.camera;sc.left=sc.bottom=-90;sc.right=sc.top=90;sc.near=1;sc.far=500;sc.updateProjectionMatrix();
  this.sun.shadow.mapSize.set(2048,2048);this.sun.shadow.bias=-.0005;this.sun.shadow.normalBias=.4;this.sun.castShadow=true;scene.add(this.hemi,this.sun,this.sun.target);
  // ground + harbor water
  const gt=this.tex(128,128,(g,w,h)=>{g.fillStyle='#8a8d92';g.fillRect(0,0,w,h);for(let i=0;i<900;i++){const v=110+R()*50|0;g.fillStyle=`rgb(${v},${v},${v+4})`;g.fillRect(R()*w,R()*h,2,2)}},50);
  const gr=new THREE.Mesh(new THREE.PlaneGeometry(1500,1368).rotateX(-Math.PI/2),new THREE.MeshStandardMaterial({map:gt,roughness:1}));gr.position.z=-66;gr.receiveShadow=true;scene.add(gr);{const og=new THREE.Mesh(new THREE.PlaneGeometry(3000,1918).rotateX(-Math.PI/2),new THREE.MeshStandardMaterial({color:0x4f6b3c,roughness:1}));og.position.set(0,-.12,-341);og.receiveShadow=true;scene.add(og)}
  
  // roads + lane dashes
  const OR=[[-600,-881,16,538],[600,-881,16,538],[0,-1150,2316,16],[-1150,-275,16,1766],[1150,-275,16,1766],[-881,-600,538,16],[881,-600,538,16],[881,0,538,16],[-881,600,538,16],[881,600,538,16]];const rd=inst(new THREE.BoxGeometry(1,1,1),std(0x23272e,.95),22+OR.length);
  for(let i=0;i<=10;i++){put(rd,i*2,L[i],.03,0,hw(i)*2,.06,1224);put(rd,i*2+1,0,.03,L[i],1224,.06,hw(i)*2)}OR.forEach((r,n)=>put(rd,22+n,r[0],.03,r[1],r[2],.06,r[3]));
  const ds=[];for(let i=0;i<=10;i++)for(let c=-596;c<600;c+=14)if(!near(c)){ds.push([L[i],c,0],[c,L[i],Math.PI/2])}for(const r of OR){if(r[2]>r[3]){for(let c=r[0]-r[2]/2+8;c<r[0]+r[2]/2-4;c+=14)ds.push([c,r[1],Math.PI/2])}else{for(let c=r[1]-r[3]/2+8;c<r[1]+r[3]/2-4;c+=14)ds.push([r[0],c,0])}}
  const dm=inst(new THREE.BoxGeometry(.3,.02,4),new THREE.MeshStandardMaterial({color:0xd9b84a,emissive:0x3a2f08}),ds.length);ds.forEach((d,n)=>put(dm,n,d[0],.065,d[1],1,1,1,d[2]));
  // street lights
  const lp=[];for(let i=0;i<=10;i++)for(let c=-600;c<=600;c+=30)if(!near(c)){const o=hw(i)+1.5;lp.push([L[i]+o,c],[c,L[i]+o])}
  this.lampMat=new THREE.MeshStandardMaterial({color:0x222222,emissive:0xffd890,emissiveIntensity:0});
  const pm=inst(new THREE.CylinderGeometry(.12,.15,7,6).translate(0,3.5,0),std(0x4a4f58),lp.length),hm=inst(new THREE.SphereGeometry(.5,6,4).translate(0,7.2,0),this.lampMat,lp.length);
  lp.forEach((p,n)=>{put(pm,n,p[0],0,p[1],1,1,1);put(hm,n,p[0],0,p[1],1,1,1)});
  // traffic lights
  {const tp=[];for(let i=0;i<=10;i++)for(let j=0;j<=10;j++){const a=hw(i)+1.3,b=hw(j)+1.3;tp.push([L[i]+a,L[j]+b,0],[L[i]-a,L[j]-b,0],[L[i]+a,L[j]-b,1],[L[i]-a,L[j]+b,1])}
   const po=inst(new THREE.CylinderGeometry(.1,.12,6,6).translate(0,3,0),std(0x2a2d33),tp.length),hd=inst(new THREE.BoxGeometry(.5,1.2,.4).translate(0,6.2,0),std(0x111111),tp.length),bb=inst(new THREE.SphereGeometry(.42,8,6).translate(0,6.3,0),new THREE.MeshBasicMaterial({color:0xffffff,fog:false}),tp.length);
   tp.forEach((p,n)=>{put(po,n,p[0],0,p[1],1,1,1);put(hd,n,p[0],0,p[1],1,1,1);put(bb,n,p[0],0,p[1],1,1,1);bb.setColorAt(n,new THREE.Color(0xff2a2a))});this.tlb=bb;this.tla=tp.map(p=>p[2])}
  // blocks
  const parts=[],trees=[],pal=[[.62,.62,.6],[.62,.3,.24],[.35,.55,.75],[.8,.7,.5]];
  for(let ix=0;ix<10;ix++)for(let iz=0;iz<10;iz++){
   const x0=L[ix]+hw(ix)+4,x1=L[ix+1]-hw(ix+1)-4,z0=L[iz]+hw(iz)+4,z1=L[iz+1]-hw(iz+1)-4,cx=(x0+x1)/2,cz=(z0+z1)/2;
   if(ix>=7&&ix<=8&&iz>=1&&iz<=2){const p=new THREE.Mesh(new THREE.PlaneGeometry(x1-x0,z1-z0).rotateX(-Math.PI/2),std(0x2f6b3a,1));p.position.set(cx,.02,cz);p.receiveShadow=true;scene.add(p);
    this.parks.push({x0,x1,z0,z1});for(let k=0;k<14;k++)trees.push([x0+3+R()*(x1-x0-6),z0+3+R()*(z1-z0-6),.8+R()*.6])}
   else if(LOTS[ix+','+iz]){const t=LOTS[ix+','+iz],p=new THREE.Mesh(new THREE.PlaneGeometry(x1-x0,z1-z0).rotateX(-Math.PI/2),std(0x55585f,.9));p.position.set(cx,.02,cz);p.receiveShadow=true;scene.add(p);SHOPS.push({...SHOPDEF[t],id:t,w:14,d:10,x:cx,z:cz,mz:cz-1.5})}
   else if(ix===4&&iz===5){const p=new THREE.Mesh(new THREE.PlaneGeometry(x1-x0,z1-z0).rotateX(-Math.PI/2),std(0xb9b4a8,.8));p.position.set(cx,.02,cz);p.receiveShadow=true;scene.add(p);
    const f=(g,m,y)=>{const o=new THREE.Mesh(g,m);o.position.set(cx,y,cz);o.castShadow=true;scene.add(o)};
    f(new THREE.CylinderGeometry(6,6.5,.9,18),std(0x888888),.45);f(new THREE.CylinderGeometry(5.2,5.2,.95,18),new THREE.MeshStandardMaterial({color:0x2a8fd0,emissive:0x0a3a5a,roughness:.2}),.48);f(new THREE.CylinderGeometry(.5,.8,4,8),std(0xaaaaaa),2.5);
    const b={x0:cx-6.5,x1:cx+6.5,z0:cz-6.5,z1:cz+6.5,h:1};this.boxes.push(b);this.grid.add(b)}
   else if(iz<9){
    const mx=cx,mz=cz,cells=[[x0,mx,z0,mz],[mx,x1,z0,mz],[x0,mx,mz,z1],[mx,x1,mz,z1]];let placed=0;
    cells.forEach((c,k)=>{if(R()<.7||(k===3&&!placed)){placed++;const cw=c[1]-c[0],cd=c[3]-c[2],w=14+R()*(Math.min(40,cw-2)-14),d=14+R()*(Math.min(40,cd-2)-14),
     hmax=U.lerp(110,24,U.clamp(Math.hypot(cx,cz)/850,0,1)),h=12+R()*(hmax-12),px=c[0]+w/2+R()*(cw-w),pz=c[2]+d/2+R()*(cd-d),j=(R()-.5)*.16,p=pal[Math.floor(R()*4)];
     parts.push({g:new THREE.BoxGeometry(w,h,d).translate(px,h/2,pz),c:[p[0]+j,p[1]+j,p[2]+j],uv:(f,u,v)=>f<2?[u*d/16,v*h/16]:f<4?[0,0]:[u*w/16,v*h/16]});
     const b={x0:px-w/2,x1:px+w/2,z0:pz-d/2,z1:pz+d/2,h};this.boxes.push(b);this.grid.add(b)}})}}
  const cells=Array.from({length:16},()=>R()<.45),cv=(lit)=>(g,w,h)=>{g.fillStyle=lit?'#000':'#cfcfcf';g.fillRect(0,0,w,h);cells.forEach((on,n)=>{g.fillStyle=lit?(on?'#ffd98a':'#000'):'#566a85';g.fillRect((n%4)*32+6,(n>>2)*32+6,20,20)})};
  this.winMat=new THREE.MeshStandardMaterial({vertexColors:true,map:this.tex(128,128,cv(false),1),emissiveMap:this.tex(128,128,cv(true),1),emissive:0xffffff,emissiveIntensity:0,roughness:.5,metalness:.22,envMap:(Car.init(),Car.env),envMapIntensity:.55});
  const bm=new THREE.Mesh(merge(parts),this.winMat);bm.castShadow=bm.receiveShadow=true;scene.add(bm);

  // ===== sidewalks, curbs, boulevards =====
  const side=(XS,ZS,hx,hz)=>{const sw=[],cb=[];
   for(let i=0;i<XS.length;i++)for(let j=0;j<ZS.length-1;j++){const a=ZS[j]+hz(j)+4,b=ZS[j+1]-hz(j+1)-4,zc=(a+b)/2,len=b-a;if(len<=0)continue;for(const q of[-1,1]){sw.push([XS[i]+q*(hx(i)+2),zc,4,len]);cb.push([XS[i]+q*(hx(i)+.17),zc,.34,len])}}
   for(let j=0;j<ZS.length;j++)for(let i=0;i<XS.length-1;i++){const a=XS[i]+hx(i)+4,b=XS[i+1]-hx(i+1)-4,xc=(a+b)/2,len=b-a;if(len<=0)continue;for(const q of[-1,1]){sw.push([xc,ZS[j]+q*(hz(j)+2),len,4]);cb.push([xc,ZS[j]+q*(hz(j)+.17),len,.34])}}
   for(let i=0;i<XS.length;i++)for(let j=0;j<ZS.length;j++)for(const a of[-1,1])for(const b of[-1,1])sw.push([XS[i]+a*(hx(i)+2),ZS[j]+b*(hz(j)+2),4,4]);
   return[sw,cb]};
  const mkI=(arr,col,hg,y,rg)=>{if(!arr.length)return;const m=inst(new THREE.BoxGeometry(1,hg,1),std(col,rg||.95),arr.length);arr.forEach((a,n)=>put(m,n,a[0],y,a[1],a[2],1,a[3]))};
  {const[sw,cb]=side(L,L,hw,hw),md=[],gm=[],solidB=(x0,x1,z0,z1)=>{const q={x0,x1,z0,z1,h:.6,tr:1};this.boxes.push(q);this.grid.add(q)};
   for(const i of C.aves)for(let j=0;j<10;j++){const a=L[j]+hw(j)+16,b=L[j+1]-hw(j+1)-16,c=(a+b)/2,l=b-a;
    md.push([L[i],c,4.6,l],[c,L[i],l,4.6]);gm.push([L[i],c,3.8,l],[c,L[i],l,3.8]);solidB(L[i]-2.3,L[i]+2.3,a,b);solidB(a,b,L[i]-2.3,L[i]+2.3);
    for(let z=a+8;z<b-4;z+=16){trees.push([L[i],z,.7]);trees.push([z,L[i],.7])}}
   mkI(sw,0x9b9da3,.16,.08);mkI(cb,0xd4d4d8,.2,.1);mkI(md,0xc9c9cd,.28,.14);mkI(gm,0x2f6b3a,.3,.16,1)}
  // trees
  const tt=inst(new THREE.CylinderGeometry(.3,.4,3,6).translate(0,1.5,0),std(0x5a3d22),trees.length),tc=inst(new THREE.ConeGeometry(2.2,6,7).translate(0,6,0),std(0x1f6a30),trees.length);
  trees.forEach((t,n)=>{put(tt,n,t[0],0,t[1],t[2],t[2],t[2]);put(tc,n,t[0],0,t[1],t[2],t[2],t[2]);tbox(t[0],t[1],t[2])});
  // billboards
  const bt=this.tex(256,108,(g,w,h)=>{g.fillStyle='#0b1022';g.fillRect(0,0,w,h);g.strokeStyle='#36f1ff';g.lineWidth=4;g.strokeRect(4,4,w-8,h-8);g.textAlign='center';g.fillStyle='#36f1ff';g.font='bold 40px sans-serif';g.fillText('NEON HARBOR',w/2,58);g.fillStyle='#ff3d8b';g.font='bold 20px sans-serif';g.fillText('DRIVE AFTER DARK',w/2,86)});
  for(const [x,z,ry] of[[-130,10,Math.PI],[130,-10,0],[10,-130,-Math.PI/2],[-10,130,Math.PI/2]]){const g=new THREE.Group(),p=new THREE.Mesh(new THREE.PlaneGeometry(14,6),new THREE.MeshBasicMaterial({map:bt,side:THREE.DoubleSide})),s=new THREE.Mesh(new THREE.BoxGeometry(.4,9,.4),std(0x333333));
   p.position.y=10;s.position.y=4.5;g.add(p,s);g.position.set(x,0,z);g.rotation.y=ry;scene.add(g)}
  // airport (north strip)
  {const slab=(w,d,x,z,c,y)=>{const p=new THREE.Mesh(new THREE.PlaneGeometry(w,d).rotateX(-Math.PI/2),std(c,.9));p.position.set(x,y,z);p.receiveShadow=true;scene.add(p)};
   slab(1900,62,0,-641,0x4a4d54,.04);slab(1900,36,0,-690,0x2a2c31,.05);
   const dm2=inst(new THREE.BoxGeometry(14,.02,.8),new THREE.MeshBasicMaterial({color:0xf2f2f2}),70);for(let i=0;i<70;i++)put(dm2,i,-930+i*27,.07,-690,1,1,1);
   const tw=inst(new THREE.BoxGeometry(.5,.02,12),new THREE.MeshBasicMaterial({color:0xf2f2f2}),12);for(let i=0;i<6;i++){put(tw,i,-545,.07,-696+i*2.4,1,1,1);put(tw,i+6,545,.07,-696+i*2.4,1,1,1)}
   const bld=(w,h,d,x,z,c,gl)=>{const m=new THREE.Mesh(new THREE.BoxGeometry(w,h,d),gl?new THREE.MeshStandardMaterial({color:c,roughness:.15,metalness:.6}):std(c));m.position.set(x,h/2,z);m.castShadow=m.receiveShadow=true;scene.add(m);const b={x0:x-w/2,x1:x+w/2,z0:z-d/2,z1:z+d/2,h};this.boxes.push(b);this.grid.add(b)};
   bld(120,14,36,480,-748,0x9aa6b5,true);bld(90,20,36,-520,-748,0x7a808a);bld(60,18,36,-640,-748,0x6a707a);
   const tc=new THREE.Mesh(new THREE.CylinderGeometry(2.6,3.2,38,10),std(0xcfcfcf));tc.position.set(360,19,-745);tc.castShadow=true;scene.add(tc);const tk=new THREE.Mesh(new THREE.CylinderGeometry(6,4,6,10),new THREE.MeshStandardMaterial({color:0x2a5a7a,roughness:.1,metalness:.7,emissive:0x0a2a3a}));tk.position.set(360,41,-745);scene.add(tk);
   const tb={x0:357,x1:363,z0:-748,z1:-742,h:38};this.boxes.push(tb);this.grid.add(tb);
   const rl=inst(new THREE.BoxGeometry(.6,.4,.6),new THREE.MeshBasicMaterial({color:0xffe9a0}),88);for(let i=0;i<44;i++){put(rl,i,-540+i*25,.25,-673,1,1,1);put(rl,i+44,-540+i*25,.25,-609,1,1,1)}
   const bl=inst(new THREE.BoxGeometry(.5,.4,.5),new THREE.MeshBasicMaterial({color:0x4aa0ff}),44);for(let i=0;i<44;i++)put(bl,i,-540+i*25,.25,-708,1,1,1);
   const mt=std(0x7a8794,.6),dm=std(0x2a2f36,.8);for(const hx of[-420,-290,-160,-30]){const hb=new THREE.Mesh(new THREE.BoxGeometry(40,9,28),mt),ha=new THREE.Mesh(new THREE.CylinderGeometry(20,20,28,16,1,false,-Math.PI/2,Math.PI).rotateX(-Math.PI/2).rotateZ(Math.PI/2).scale(1,.35,1),mt),hd=new THREE.Mesh(new THREE.BoxGeometry(30,8,.3),dm);
    hb.position.set(hx,4.5,-738);ha.position.set(hx,9,-738);hd.position.set(hx,4,-723.8);for(const o of[hb,ha,hd]){o.castShadow=o.receiveShadow=true;scene.add(o)}const q={x0:hx-20,x1:hx+20,z0:-752,z1:-724,h:11};this.boxes.push(q);this.grid.add(q)}
   for(let i=0;i<3;i++){const t=new THREE.Mesh(new THREE.CylinderGeometry(5,5,8,14),std(0xe8e8e8,.5));t.position.set(150+i*14,4,-738);t.castShadow=true;scene.add(t);const q={x0:145+i*14,x1:155+i*14,z0:-743,z1:-733,h:8};this.boxes.push(q);this.grid.add(q)}
   const hp=new THREE.Mesh(new THREE.CircleGeometry(10,24).rotateX(-Math.PI/2),std(0x33363c,.9));hp.position.set(330,.08,-650);scene.add(hp);const hr=new THREE.Mesh(new THREE.RingGeometry(8.4,9.2,32).rotateX(-Math.PI/2),new THREE.MeshBasicMaterial({color:0xf2f2f2}));hr.position.set(330,.1,-650);scene.add(hr);
   for(const[a,b,c]of[[.7,.1,5],[.7,.1,5],[4,.1,.7]]){}const H=(w,d,x)=>{const m=new THREE.Mesh(new THREE.BoxGeometry(w,.05,d),new THREE.MeshBasicMaterial({color:0xf2f2f2}));m.position.set(330+x,.12,-650);scene.add(m)};H(.8,5,-1.8);H(.8,5,1.8);H(3.8,.8,0);
   const ws=new THREE.Mesh(new THREE.CylinderGeometry(.1,.1,8,6),std(0xcccccc,.5));ws.position.set(-545,4,-603);scene.add(ws);const sk=new THREE.Mesh(new THREE.ConeGeometry(.7,3.5,8).rotateZ(-Math.PI/2),new THREE.MeshBasicMaterial({color:0xff7a2a}));sk.position.set(-543.4,7.5,-603);scene.add(sk)}
  // outer lands: suburbs, forests, mountains
  {const R2=U.rng(4242),pp=[],pal2=[[.62,.62,.6],[.62,.3,.24],[.35,.55,.75],[.8,.7,.5]],bandZ=[-600,0,600],bandX=[-600,600];
   const onR=(x,z,m)=>{if(Math.abs(x)>740||z<-740){for(const c of bandZ)if(Math.abs(z-c)<8+m&&Math.abs(x)>605)return true;for(const c of bandX)if(Math.abs(x-c)<8+m&&z<-605)return true;if(Math.abs(Math.abs(x)-1150)<8+m||Math.abs(z+1150)<8+m)return true}return false};
   for(let xc=-1080;xc<=1080;xc+=90)for(let zc=-1080;zc<=540;zc+=90){
    if(Math.abs(xc)<760&&zc>-760)continue;
    if(bandZ.some(c=>Math.abs(zc-c)<58&&Math.abs(xc)>600)||bandX.some(c=>Math.abs(xc-c)<58&&zc<-600))continue;
    const n=R2()<.8?(R2()<.5?1:2):0;let prev=null;
    for(let k=0;k<n;k++){const w=14+R2()*26,d=14+R2()*26,h=8+R2()*(Math.hypot(xc,zc)>1000?30:46),px=xc+(R2()-.5)*(80-w),pz=zc+(R2()-.5)*(80-d),j=(R2()-.5)*.16,p=pal2[Math.floor(R2()*4)];
     if(prev&&Math.abs(px-prev.x)<(w+prev.w)/2+3&&Math.abs(pz-prev.z)<(d+prev.d)/2+3)continue;
     pp.push({g:new THREE.BoxGeometry(w,h,d).translate(px,h/2,pz),c:[p[0]+j,p[1]+j,p[2]+j],uv:(f,u,v)=>f<2?[u*d/16,v*h/16]:f<4?[0,0]:[u*w/16,v*h/16]});
     const b={x0:px-w/2,x1:px+w/2,z0:pz-d/2,z1:pz+d/2,h};b.mt=1;this.boxes.push(b);this.grid.add(b);prev={x:px,z:pz,w,d}}}
   if(pp.length){const m2=new THREE.Mesh(merge(pp),this.winMat);m2.castShadow=m2.receiveShadow=true;scene.add(m2)}
   const tp=[];for(let t=0;t<4000&&tp.length<900;t++){const x=(R2()-.5)*2500,z=-1280+R2()*1880;if(Math.abs(x)<760&&z>-760)continue;if(onR(x,z,6)||!this.free(x,z,4))continue;tp.push([x,z,.8+R2()*.9])}
   const t1=inst(new THREE.CylinderGeometry(.3,.4,3,6).translate(0,1.5,0),std(0x5a3d22),tp.length),t2=inst(new THREE.ConeGeometry(2.2,6,7).translate(0,6,0),std(0x1f6a30),tp.length);
   tp.forEach((t,n)=>{put(t1,n,t[0],0,t[1],t[2],t[2],t[2]);put(t2,n,t[0],0,t[1],t[2],t[2],t[2]);tbox(t[0],t[1],t[2])});
   const mt=[];for(let i=0;i<60;i++){let x,z;if(i<20){x=-1350-R2()*150;z=-1350+R2()*1900}else if(i<40){x=1350+R2()*150;z=-1350+R2()*1900}else{x=-1350+R2()*2700;z=-1350-R2()*150}mt.push([x,z,90+R2()*110,160+R2()*260,16,0])}
   this.mt=mt;const mo=inst(new THREE.ConeGeometry(1,1,16).translate(0,.5,0),std(0x56606a,1),mt.length);mt.forEach((m,n)=>put(mo,n,m[0],0,m[1],m[2],m[3],m[2]))}

  // ===== EXTENSION: south valley behind the mountain ridge =====
  {const R4=U.rng(9090),G3=new THREE.Mesh(new THREE.PlaneGeometry(3400,2900).rotateX(-Math.PI/2),std(0x4f6b3c,1));G3.position.set(0,-.12,2050);G3.receiveShadow=true;scene.add(G3);
   // solid mountains: ridge with a pass at x=0, side walls, south wall
   const nm=[],ad=(x,z,r,h)=>nm.push([x,z,r,h]);
   for(let x=-1700;x<=1700;x+=135)for(const[dz,o]of[[0,0],[110,67]]){const xx=x+o+(R4()-.5)*40;if(Math.abs(xx)<340)continue;ad(xx,880+dz+(R4()-.5)*50,150+R4()*60,230+R4()*190)}
   for(let z=930;z<=3400;z+=120)for(const sg of[-1,1])ad(sg*(1390+R4()*90),z+(R4()-.5)*30,150+R4()*50,220+R4()*200);
   for(let x=-1500;x<=1500;x+=120)ad(x,3340+R4()*60,160+R4()*60,250+R4()*170);
   nm.forEach((m,n)=>{m[4]=16;m[5]=n;this.mt.push(m)});
   const mo=inst(new THREE.ConeGeometry(1,1,16).translate(0,.5,0),new THREE.MeshStandardMaterial({color:0x5b6670,roughness:1,flatShading:true}),nm.length),sn=inst(new THREE.ConeGeometry(1,1,9).translate(0,.5,0),new THREE.MeshStandardMaterial({color:0xf2f5f8,roughness:.8,flatShading:true}),nm.length);
   nm.forEach((m,n)=>{put(mo,n,m[0],0,m[1],m[2],m[3],m[2],n);put(sn,n,m[0],m[3]*.7,m[1],m[2]*.3,m[3]*.3,m[2]*.3,n)});
   // roads
   const NX=[],NZ=[];for(let a=0;a<=6;a++){NX.push(-360+120*a);NZ.push(1640+120*a)}
   const rd=[[0,1126,16,1028],[0,2460,16,200]];for(const x of NX)rd.push([x,2000,16,720]);for(const z of NZ)rd.push([0,z,720,16]);
   mkI(rd,0x23272e,.06,.03,.95);
   const ds=[];for(let z=640;z<1640;z+=14)ds.push([0,z,.3,4]);for(let z=2380;z<2560;z+=14)ds.push([0,z,.3,4]);for(const x of NX)for(let z=1650;z<2350;z+=14)if(Math.abs(((z-1640)%120)-60)<50)ds.push([x,z,.3,4]);for(const z of NZ)for(let x=-350;x<350;x+=14)if(Math.abs(((x+360)%120)-60)<50)ds.push([x,z,4,.3]);
   mkI(ds,0xd9b84a,.02,.065,.9);
   const[sw,cb]=side(NX,NZ,()=>8,()=>8);mkI(sw,0x9b9da3,.16,.08);mkI(cb,0xd4d4d8,.2,.1);
   const cg=new THREE.Mesh(new THREE.PlaneGeometry(900,900).rotateX(-Math.PI/2),std(0x80838a,.95));cg.position.set(0,.005,2000);cg.receiveShadow=true;scene.add(cg);
   // blocks
   const NL={'0,0':'gun','2,0':'att','4,0':'car','1,2':'moto','3,2':'garage','5,2':'arena','0,4':'air','2,4':'mil','4,4':'skin'},PK={'2,1':1,'3,3':1,'5,4':1},vp=[],vtr=[];
   for(let ia=0;ia<6;ia++)for(let ib=0;ib<6;ib++){const k=ia+','+ib,x0=NX[ia]+12,x1=NX[ia+1]-12,z0=NZ[ib]+12,z1=NZ[ib+1]-12,cx=(x0+x1)/2,cz=(z0+z1)/2,pl=(c)=>{const p=new THREE.Mesh(new THREE.PlaneGeometry(x1-x0,z1-z0).rotateX(-Math.PI/2),std(c,.9));p.position.set(cx,.02,cz);p.receiveShadow=true;scene.add(p)};
    if(NL[k]){pl(0x55585f);const t=NL[k],sh={...SHOPDEF[t],id:t,w:14,d:10,x:cx,z:cz,mz:cz-1.5};if(t==='air')sh.ap=[0,2620];SHOPS.push(sh)}
    else if(PK[k]){pl(0x2f6b3a);this.parks.push({x0,x1,z0,z1});for(let q=0;q<10;q++)vtr.push([x0+4+R4()*(x1-x0-8),z0+4+R4()*(z1-z0-8),.8+R4()*.6])}
    else{const mx=cx,mz=cz;[[x0,mx,z0,mz],[mx,x1,z0,mz],[x0,mx,mz,z1],[mx,x1,mz,z1]].forEach((c,q)=>{if(R4()<.75||q===3){const cw=c[1]-c[0],cd=c[3]-c[2],w=14+R4()*(Math.min(38,cw-2)-14),d=14+R4()*(Math.min(38,cd-2)-14),dist=Math.hypot(cx,cz-2000),h=12+R4()*(U.lerp(95,26,U.clamp(dist/420,0,1))-12),px=c[0]+w/2+R4()*(cw-w),pz=c[2]+d/2+R4()*(cd-d),j=(R4()-.5)*.16,p=pal[Math.floor(R4()*4)];
      vp.push({g:new THREE.BoxGeometry(w,h,d).translate(px,h/2,pz),c:[p[0]+j,p[1]+j,p[2]+j],uv:(f,u,v)=>f<2?[u*d/16,v*h/16]:f<4?[0,0]:[u*w/16,v*h/16]});
      const b={x0:px-w/2,x1:px+w/2,z0:pz-d/2,z1:pz+d/2,h};this.boxes.push(b);this.grid.add(b)}})}}
   {const m=new THREE.Mesh(merge(vp),this.winMat);m.castShadow=m.receiveShadow=true;scene.add(m)}
   // valley trees (solid)
   for(let t=0;t<3000&&vtr.length<760;t++){const x=(R4()-.5)*2700,z=1010+R4()*2250;if(Math.abs(x)<30&&z<2700)continue;if(Math.abs(x)<460&&z>1590&&z<2410)continue;if(z>2530&&z<2720&&Math.abs(x)<1000)continue;if(Math.abs(x)>1330)continue;vtr.push([x,z,.8+R4()*.9])}
   {const a=inst(new THREE.CylinderGeometry(.3,.4,3,6).translate(0,1.5,0),std(0x5a3d22),vtr.length),b=inst(new THREE.ConeGeometry(2.2,6,7).translate(0,6,0),std(0x1f6a30),vtr.length);vtr.forEach((t,n)=>{put(a,n,t[0],0,t[1],t[2],t[2],t[2]);put(b,n,t[0],0,t[1],t[2],t[2],t[2]);tbox(t[0],t[1],t[2])})}
   // airport 2 (south of the valley city)
   const slab=(w,d,x,z,c,y)=>{const p=new THREE.Mesh(new THREE.PlaneGeometry(w,d).rotateX(-Math.PI/2),std(c,.9));p.position.set(x,y,z);p.receiveShadow=true;scene.add(p)};
   slab(1900,44,0,2660,0x4a4d54,.04);slab(1900,26,0,2620,0x2a2c31,.05);slab(700,50,0,2575,0x3a3d44,.045);
   const rm=[];for(let i=0;i<70;i++)rm.push([-930+i*27,2660,14,.8]);mkI(rm,0xf2f2f2,.02,.07,.9);
   const rl=[];for(let i=0;i<76;i++)rl.push([-940+i*25,2639,.6,.6],[-940+i*25,2681,.6,.6]);mkI(rl,0xffe9a0,.4,.25,.9);
   const bld=(w,h,d,x,z,c,gl)=>{const m=new THREE.Mesh(new THREE.BoxGeometry(w,h,d),gl?new THREE.MeshStandardMaterial({color:c,roughness:.15,metalness:.6}):std(c));m.position.set(x,h/2,z);m.castShadow=m.receiveShadow=true;scene.add(m);const b={x0:x-w/2,x1:x+w/2,z0:z-d/2,z1:z+d/2,h};this.boxes.push(b);this.grid.add(b)};
   bld(120,14,36,230,2560,0x9aa6b5,true);for(let i=0;i<4;i++)bld(40,10,28,-640+i*60,2560,0x6a707a);
   {const t=new THREE.Mesh(new THREE.CylinderGeometry(2.6,3.2,38,10),std(0xcfcfcf));t.position.set(340,19,2560);t.castShadow=true;scene.add(t);const k=new THREE.Mesh(new THREE.CylinderGeometry(6,4,6,10),new THREE.MeshStandardMaterial({color:0x2a5a7a,roughness:.1,metalness:.7,emissive:0x0a2a3a}));k.position.set(340,41,2560);scene.add(k);const b={x0:337,x1:343,z0:2557,z1:2563,h:38};this.boxes.push(b);this.grid.add(b);
    const hp=new THREE.Mesh(new THREE.CircleGeometry(10,24).rotateX(-Math.PI/2),std(0x33363c,.9));hp.position.set(470,.08,2585);scene.add(hp);const hr=new THREE.Mesh(new THREE.RingGeometry(8.4,9.2,32).rotateX(-Math.PI/2),new THREE.MeshBasicMaterial({color:0xf2f2f2}));hr.position.set(470,.1,2585);scene.add(hr)}
   MAPLBL.push(['RIDGE CITY',0,2000],['RIDGE AIRPORT',0,2720],['MOUNTAIN PASS',0,1120],['SOUTH RIDGE',-700,820]);POI.push({x:0,z:2630,c:'#ffffff',t:'AIRPORT'});
   this.ridgeCity={NX,NZ,rd}}
  // minimap base layer
  const S=.5,mm=this.mm=document.createElement('canvas');mm.width=1600;mm.height=2500;const g=mm.getContext('2d'),X=v=>(v+1600)*S;g.fillStyle='#15261a';g.fillRect(0,0,1600,2500);g.fillStyle='#14171d';g.fillRect(X(-750),X(-750),1500*S,1368*S);
  g.fillStyle='#1d2f22';g.fillRect(0,X(612),1600,2500-X(612));g.fillStyle='#454d56';for(const m of this.mt){g.beginPath();g.arc(X(m[0]),X(m[1]),m[2]*.8*S,0,7);g.fill()}
  g.fillStyle='#15301f';for(const p of this.parks)g.fillRect(X(p.x0),X(p.z0),(p.x1-p.x0)*S,(p.z1-p.z0)*S);
  g.fillStyle='#262b35';for(const b of this.boxes)if(!b.tr)g.fillRect(X(b.x0),X(b.z0),(b.x1-b.x0)*S,(b.z1-b.z0)*S);
  for(const[c,e]of[['#07090c',2.5],['#59606c',0]])for(let i=0;i<=10;i++){g.fillStyle=c;g.fillRect((L[i]-hw(i)-e+1600)*S,988*S,(hw(i)+e)*2*S,1224*S);g.fillRect(988*S,(L[i]-hw(i)-e+1600)*S,1224*S,(hw(i)+e)*2*S)}g.fillStyle='#59606c';for(const r of OR)g.fillRect(X(r[0]-r[2]/2),X(r[1]-r[3]/2),r[2]*S,r[3]*S);
  g.fillStyle='#3a3e48';g.fillRect(X(-550),X(-672),1100*S,62*S);g.fillStyle='#2c2f37';g.fillRect(X(-550),X(-708),1100*S,36*S);g.fillStyle='#fff';for(let i=0;i<40;i++)g.fillRect(X(-520+i*27),X(-690),8,1.5);g.fillStyle='#8a6d2a';g.fillRect(X(-90),X(-640),180*S,24*S)
  {const rc=this.ridgeCity;g.fillStyle='#14171d';g.fillRect(X(-450),X(1550),900*S,900*S);g.fillStyle='#59606c';for(const r of rc.rd)g.fillRect(X(r[0]-r[2]/2),X(r[1]-r[3]/2),r[2]*S,r[3]*S);
   g.fillStyle='#15301f';for(const p of this.parks)if(p.z0>1400)g.fillRect(X(p.x0),X(p.z0),(p.x1-p.x0)*S,(p.z1-p.z0)*S);g.fillStyle='#262b35';for(const b of this.boxes)if(!b.tr&&b.z0>1400)g.fillRect(X(b.x0),X(b.z0),(b.x1-b.x0)*S,(b.z1-b.z0)*S);
   g.fillStyle='#3a3e48';g.fillRect(X(-950),X(2638),1900*S,44*S);g.fillStyle='#2c2f37';g.fillRect(X(-950),X(2607),1900*S,26*S);g.fillStyle='#8a6d2a';g.fillRect(X(-90),X(-640),0,0)}
 }
 free(x,z,r){for(const b of this.grid.at(x,z))if(push(x,z,r,b))return false;return true}
 tick(dt,fx,fz,t){
  this.hour=(this.hour+dt*24/C.cycle)%24;const a=(this.hour-6)/24*Math.PI*2,s=Math.sin(a),co=Math.cos(a),day=U.sm(-.12,.3,s);this.night=1-U.sm(-.15,.2,s);
  this.sky.copy(NIGHT).lerp(DAY,day).lerp(DUSK,Math.max(0,1-Math.abs(s)/.3)*.6);this.scene.fog.color.copy(this.sky);this.du.top.value.copy(TOPN).lerp(TOPD,day);this.du.hor.value.copy(this.sky);this.du.nt.value=this.night;
  const k=s>=0?1:-1,vx=co*k,vy=s*k,vz=.25*k,l=Math.hypot(vx,vy,vz);
  this.sun.position.set(fx+vx/l*250,vy/l*250,fz+vz/l*250);this.sun.target.position.set(fx,0,fz);this.du.sd.value.set(vx/l,vy/l,vz/l);
  if(s>=0){this.sun.color.setHex(0xfff1d8);this.sun.intensity=Math.min(1.1,s*3)}else{this.sun.color.setHex(0x6f8fff);this.sun.intensity=.35*Math.min(1,-s*3)}
  this.hemi.intensity=U.lerp(.28,.75,day);this.winMat.emissiveIntensity=this.night*1.3;this.lampMat.emissiveIntensity=this.night*2.5;Car.lm.color.setScalar(.35+.65*this.night);
  }}
/* ===== PLAYER ===== */
let OV=null;function ghOf(x,z,y){const o=OV;if(!o||Math.abs(x-o.x)>o.hw||z<o.a||z>o.d)return 0;const g=z<o.b?o.h*(z-o.a)/(o.b-o.a):z<o.c?o.h:o.h*(o.d-z)/(o.d-o.c);return(y!==undefined&&g>2.5&&y<g-2.5)?0:g}
function mkHuman(sh,sk,pn,hr,sho){const g=new THREE.Group(),M=c=>new THREE.MeshStandardMaterial({color:c,roughness:.8}),dk=M(0x111111),wh=M(0xf4f4f4),
 S=(geo,m,x,y,z,p,sx,sy,sz)=>{const o=new THREE.Mesh(geo,m);o.position.set(x,y,z);if(sx)o.scale.set(sx,sy,sz);o.castShadow=true;(p||g).add(o);return o},
 sp=(r,w,h)=>new THREE.SphereGeometry(r,w||12,h||8),cy=(a,b,h,s)=>new THREE.CylinderGeometry(a,b,h,s||12);sho=sho||dk;
 S(cy(.27,.21,.74,14),sh,0,1.35,0,0,1,1,.6);S(sp(.275,14,8),sh,0,1.62,0,0,1,.5,.62);S(sp(.21,12,8),pn,0,1.03,0,0,1,.6,.68);S(cy(.225,.225,.07,14),dk,0,1.08,0,0,1,1,.62);
 S(sp(.12,10,8),sh,.34,1.66,0);S(sp(.12,10,8),sh,-.34,1.66,0);S(cy(.07,.08,.14,8),sk,0,1.77,0);
 const head=new THREE.Group();head.position.set(0,1.95,0);g.add(head);
 S(sp(.2,16,12),sk,0,0,0,head,.92,1.12,1);S(new THREE.SphereGeometry(.212,14,10,0,Math.PI*2,0,Math.PI*.58),hr,0,.02,-.015,head,.93,1.12,1.02);S(sp(.19,10,8),hr,0,-.02,-.08,head,.9,1,.8);
 for(const s of[1,-1]){S(sp(.04,6,5),sk,s*.19,0,0,head,.6,1,1);S(sp(.03,8,6),wh,s*.075,.04,.17,head,1,.8,.6);S(sp(.017,6,5),dk,s*.075,.04,.19,head);S(new THREE.BoxGeometry(.07,.015,.02),hr,s*.075,.09,.18,head)}
 S(new THREE.ConeGeometry(.035,.09,6).rotateX(Math.PI/2),sk,0,-.03,.2,head);S(new THREE.BoxGeometry(.08,.014,.02),M(0x7a2a2a),0,-.09,.185,head);
 const arm=sx=>{const p=new THREE.Group();p.position.set(sx*.41,1.67,0);g.add(p);S(cy(.088,.068,.7,10).translate(0,-.35,0),sh,0,0,0,p);S(sp(.075,8,6),sk,0,-.78,0,p);return p},
 leg=sx=>{const p=new THREE.Group();p.position.set(sx*.13,1,0);g.add(p);S(cy(.12,.088,1,10).translate(0,-.5,0),pn,0,0,0,p);S(new THREE.BoxGeometry(.19,.1,.3),sho,0,-.96,.06,p);S(sp(.1,8,6),sho,0,-.95,.17,p,1,.7,1);return p};
 return{g,head,aL:arm(1),aR:arm(-1),lL:leg(1),lR:leg(-1)}}
function humG(){const T=(geo,x,y,z,sx,sy,sz)=>{if(sx)geo.scale(sx,sy,sz);return geo.translate(x,y,z)},sp=(r,w,h)=>new THREE.SphereGeometry(r,w||10,h||7),cy=(a,b,h,sg)=>new THREE.CylinderGeometry(a,b,h,sg||10),W=[1,1,1],D=[.07,.07,.07];
 const tor=[{g:T(cy(.27,.21,.74,12),0,1.35,0,1,1,.6),c:W},{g:T(sp(.275,12,7),0,1.62,0,1,.5,.62),c:W},{g:T(sp(.21,10,7),0,1.03,0,1,.6,.68),c:W},{g:T(sp(.12,8,6),.34,1.66,0),c:W},{g:T(sp(.12,8,6),-.34,1.66,0),c:W},{g:T(cy(.225,.225,.07,12),0,1.08,0,1,1,.62),c:D}];
 const hd=[{g:T(sp(.2,14,10),0,1.95,0,.92,1.12,1),c:W},{g:T(cy(.07,.08,.14,8),0,1.77,0),c:W},{g:T(sp(.04,6,5),.19,1.95,0,.6,1,1),c:W},{g:T(sp(.04,6,5),-.19,1.95,0,.6,1,1),c:W},{g:T(new THREE.ConeGeometry(.035,.09,6).rotateX(Math.PI/2),0,1.92,.2),c:W},
  {g:T(sp(.03,8,6),.075,1.99,.17,1,.8,.6),c:[1,1,1]},{g:T(sp(.03,8,6),-.075,1.99,.17,1,.8,.6),c:[1,1,1]},{g:T(sp(.017,6,5),.075,1.99,.19),c:D},{g:T(sp(.017,6,5),-.075,1.99,.19),c:D},{g:T(new THREE.BoxGeometry(.08,.014,.02),0,1.86,.185),c:[.35,.1,.1]}];
 const hr=[{g:T(new THREE.SphereGeometry(.212,12,8,0,Math.PI*2,0,Math.PI*.58),0,1.97,-.015,.93,1.12,1.02),c:W},{g:T(sp(.19,8,6),0,1.93,-.08,.9,1,.8),c:W}];
 return{tor:merge(tor),hd:merge(hd),hr:merge(hr),arm:merge([{g:T(cy(.088,.068,.7,8),0,-.35,0),c:W}]),hand:merge([{g:T(sp(.075,8,6),0,-.78,0),c:W}]),leg:merge([{g:T(cy(.12,.088,1,8),0,-.5,0),c:W}]),shoe:merge([{g:T(new THREE.BoxGeometry(.19,.1,.3),0,-.96,.06),c:W},{g:T(sp(.1,8,6),0,-.95,.17,1,.7,1),c:W}])}}
class Player{constructor(scene){this.g=new THREE.Group();const M=c=>new THREE.MeshStandardMaterial({color:c,roughness:.8}),sk=M(0xe0b090),sh=M(0x2b6cff),pn=M(0x222a3a);
 const box=(w,h,d,m,x,y,z,p)=>{const o=new THREE.Mesh(new THREE.BoxGeometry(w,h,d),m);o.position.set(x,y,z);o.castShadow=true;p.add(o)};
 const limb=(w,h,m,x,y)=>{const p=new THREE.Group();p.position.set(x,y,0);this.g.add(p);box(w,h,w,m,0,-h/2,0,p);return p};
 const H=mkHuman(sh,sk,pn,M(0x2a1a10));this.g.add(H.g);this.aL=H.aL;this.aR=H.aR;this.guns={};const gm=M(0x1c1f26),wd=M(0x6b4a2b);
 for(const[n,W]of Object.entries(WEAP)){const g=new THREE.Group(),bx=(w,h,l,m,x,y,z)=>{const o=new THREE.Mesh(new THREE.BoxGeometry(w,h,l),m);o.position.set(x,y,z);o.castShadow=true;g.add(o)};
  bx(.09,.13,W.len,gm,0,0,0);bx(.07,.18,.12,gm,0,-.14,-W.len/2+.15);if(n==='Shotgun'||n==='Rifle'||n==='Sniper')bx(.09,.14,.28,wd,0,-.02,-W.len/2-.1);if(n==='Sniper')bx(.06,.07,.3,gm,0,.11,.05);if(n==='SMG')bx(.06,.22,.08,gm,0,-.2,.05);
  const ab=(w,h,l,m,x,y,z)=>{const o=new THREE.Mesh(new THREE.BoxGeometry(w,h,l),m);o.position.set(x,y,z);o.visible=false;g.add(o);return o};g.at={sil:ab(.07,.07,.28,gm,0,0,W.len/2+.2),scp:ab(.07,.08,.32,gm,0,.14,.05),lng:ab(.06,.06,.25,gm,0,0,W.len/2+.1),stk:ab(.08,.16,.2,wd,0,-.03,-W.len/2-.15)};
  g.position.set(-.4,1.6,.7);g.visible=false;this.g.add(g);this.guns[n]=g}
 this.flashM=new THREE.Mesh(new THREE.SphereGeometry(.14,6,5),new THREE.MeshBasicMaterial({color:0xffd070,fog:false}));this.flashM.visible=false;this.g.add(this.flashM);this.armed=false;this.lL=H.lL;this.lR=H.lR;
 this.g.rotation.order='YXZ';this.mat={sk,sh,pn};scene.add(this.g);this.x=20;this.z=10;this.y=0;this.vx=this.vz=this.vy=0;this.face=0;this.ph=0;this.jet=100;
 this.jetM=new THREE.Mesh(new THREE.ConeGeometry(.14,.75,8).rotateX(Math.PI),new THREE.MeshBasicMaterial({color:0x66e8ff,transparent:true,opacity:.85,blending:THREE.AdditiveBlending,depthWrite:false,fog:false}));this.jetM.position.set(0,.55,-.36);this.jetM.visible=false;this.g.add(this.jetM);
 this.jetP=new THREE.Group();{const bm=new THREE.MeshStandardMaterial({color:0x1b2a33,metalness:.6,roughness:.35}),tm=new THREE.MeshStandardMaterial({color:0x36f1ff,emissive:0x36f1ff,emissiveIntensity:.7,metalness:.8,roughness:.25}),
  b=new THREE.Mesh(new THREE.BoxGeometry(.52,.66,.26),bm);b.position.set(0,1.28,-.34);this.jetP.add(b);
  for(const s of[-1,1]){const t=new THREE.Mesh(new THREE.CylinderGeometry(.1,.1,.58,8),tm);t.position.set(s*.18,1.26,-.36);this.jetP.add(t)}
  this.jetP.visible=false;this.g.add(this.jetP)}}
 step(dt,inp,yaw,w){const k=inp.k,ix=(k.KeyD?1:0)-(k.KeyA?1:0),iz=(k.KeyW?1:0)-(k.KeyS?1:0),sy=Math.sin(yaw),cy=Math.cos(yaw);
  const nv=typeof Game!=='undefined'&&Game.lau&&Game.lau.walk&&Game.lau.nova;
  let wx=iz*sy-ix*cy,wz=iz*cy+ix*sy;const len=Math.hypot(wx,wz);if(len>1e-6){wx/=len;wz/=len}else wx=wz=0;
  const sp=(k.ShiftLeft||k.ShiftRight)?(nv?10.5:C.sprint):(nv?5.5:C.walk),f=1-Math.exp(-dt*10);this.vx=U.lerp(this.vx,wx*sp,f);this.vz=U.lerp(this.vz,wz*sp,f);
  let gp0=ghOf(this.x,this.z,this.y);for(const b of w.grid.at(this.x,this.z))if(this.y>=b.h-.75&&this.x>b.x0-C.pr&&this.x<b.x1+C.pr&&this.z>b.z0-C.pr&&this.z<b.z1+C.pr)gp0=Math.max(gp0,b.h);
  const gnd=this.y<=gp0+.05;if(gnd&&k.Space)this.vy=nv?14:C.jump;
  let jet=false;if(nv&&Game.jetOwn&&!gnd&&k.Space&&this.jet>0&&this.vy<10){this.vy=Math.min(10,this.vy+34*dt);this.jet=Math.max(0,this.jet-30*dt);jet=true}
  if(gnd&&!k.Space)this.jet=Math.min(100,this.jet+45*dt);
  this.vy+=(nv?C.grav*.28:C.grav)*dt;this.y+=this.vy*dt;if(this.y<gp0){this.y=gp0;this.vy=0}
  this.jetM.visible=jet&&nv;if(this.jetM.visible){this.jetM.scale.set(1,.75+Math.random()*.5,1)}this.jetP.visible=!!(nv&&window.Game&&window.Game.jetOwn);
  this.x+=this.vx*dt;this.z+=this.vz*dt;
  for(let it=0;it<2;it++)for(const b of w.grid.at(this.x,this.z)){if(Game.ghost)continue;if(this.y>=b.h-.75)continue;const r=push(this.x,this.z,C.pr,b);if(r){this.x+=r[0]*r[2];this.z+=r[1]*r[2]}}
  {const q=Game.solidPts(this.x,this.z,C.pr,null,false);this.x+=q[0];this.z+=q[1]}if(nv){this.x=U.clamp(this.x,30000-1450,30000+1450);this.z=U.clamp(this.z,-1450,1450);w.edge=false}else{if(this.x<1400&&Math.abs(this.x)>C.half){this.x=Math.sign(this.x)*C.half;w.edge=true}if(this.x<1400&&(this.z<-C.half||this.z>C.zs)){this.z=U.clamp(this.z,-C.half,C.zs);w.edge=true}}
  if(len>1e-6)this.face=U.lerpA(this.face,Math.atan2(wx,wz),1-Math.exp(-dt*12));
  const spd=Math.hypot(this.vx,this.vz);this.ph+=spd*dt*1.6;const sw=Math.sin(this.ph)*Math.min(1,spd/4)*.9;
  this.aL.rotation.x=sw;this.aR.rotation.x=-sw;this.lL.rotation.x=-sw;this.lR.rotation.x=sw;
  this.g.position.set(this.x,this.y+(this.y<=0?Math.abs(Math.sin(this.ph))*.05*Math.min(1,spd/4):0),this.z);this.g.rotation.y=this.face;this.g.rotation.x=Math.min(1,spd/8)*.12}}
/* ===== VEHICLE ===== */
class Car{
 static wg(){return Car._wg||(Car._wg=merge([{g:new THREE.CylinderGeometry(.38,.38,.3,16).rotateZ(Math.PI/2),c:[.04,.04,.04]},{g:new THREE.CylinderGeometry(.24,.24,.32,12).rotateZ(Math.PI/2),c:[.8,.8,.85]}]))}
 static mod(k){const M=CARMODELS[k];if(M.geo)return M.geo;const[L,w,H,hh,dh,z1,z2,z3,z4]=M.d,gc=.3,
  P=[[-L/2,gc],[-L/2,dh-.1],[z4,dh],[z3,H],[z2,H],[z1,hh],[L/2-.35,hh-.08],[L/2,hh-.28],[L/2,gc]],Gl=[[z4+.1,dh+.1],[z3+.03,H-.08],[z2-.03,H-.08],[z1-.1,hh+.1]],
  ex=(pts,wd)=>{const sh=new THREE.Shape();pts.forEach((p,i)=>i?sh.lineTo(p[0],p[1]):sh.moveTo(p[0],p[1]));const d=wd-.16,g=new THREE.ExtrudeGeometry(sh,{depth:d,bevelEnabled:true,bevelSize:.08,bevelThickness:.08,bevelSegments:2});g.translate(0,0,-d/2);g.rotateY(-Math.PI/2);return g},
  wh=(x,z)=>[{g:new THREE.CylinderGeometry(.38,.38,.3,14).rotateZ(Math.PI/2).translate(x,.38,z),c:[.04,.04,.04]},{g:new THREE.CylinderGeometry(.24,.24,.32,10).rotateZ(Math.PI/2).translate(x,.38,z),c:[.75,.75,.8]}],
  parts=[{g:ex(P,w),c:[1,1,1]},{g:ex(Gl,w+.1),c:[.07,.09,.12]}];
  if(M.sp)parts.push({g:new THREE.BoxGeometry(w-.2,.06,.45).translate(0,dh+.3,-L/2+.1),c:[.05,.05,.06]},{g:new THREE.BoxGeometry(.06,.22,.06).translate(.55,dh+.18,-L/2+.2),c:[.05,.05,.06]},{g:new THREE.BoxGeometry(.06,.22,.06).translate(-.55,dh+.18,-L/2+.2),c:[.05,.05,.06]});
  const K=[.04,.04,.05],bx=(a,b,c,x,y,z,col)=>({g:new THREE.BoxGeometry(a,b,c).translate(x,y,z),c:col}),ch=[.85,.86,.9];
  parts.push(bx(w-.05,.17,.14,0,gc+.1,L/2-.04,K),bx(w-.05,.17,.14,0,gc+.1,-L/2+.04,K),bx(w*.55,.13,.05,0,gc+.38,L/2+.02,K),bx(w*.5,.03,.05,0,gc+.3,L/2+.03,ch),
   bx(.07,.1,.5*L*.6,w/2+.01,gc+.14,0,K),bx(.07,.1,.5*L*.6,-w/2-.01,gc+.14,0,K),
   bx(.14,.1,.2,w/2+.06,hh+.06,z1-.2,[1,1,1]),bx(.14,.1,.2,-w/2-.06,hh+.06,z1-.2,[1,1,1]),
   bx(w-.3,.05,.04,0,dh-.12,-L/2-.02,[1,.05,.05]),bx(.02,H-hh-.25,.03,w/2+.01,(H+hh)/2-.05,(z2+z3)/2,K),bx(.02,H-hh-.25,.03,-w/2-.01,(H+hh)/2-.05,(z2+z3)/2,K),
   {g:new THREE.CylinderGeometry(.06,.06,.2,8).rotateX(Math.PI/2).translate(.5,gc+.06,-L/2-.06),c:ch},{g:new THREE.CylinderGeometry(.06,.06,.2,8).rotateX(Math.PI/2).translate(-.5,gc+.06,-L/2-.06),c:ch});
  if(M.sp)parts.push(bx(.5,.05,.7,0,hh+.02,L/2-.9,K));
  if(M.ex)M.ex(parts,bx,K,ch,L,w,H,hh,dh,gc,z1,z2,z3);return M.geo=merge(parts)}
 static lmod(k){const M=CARMODELS[k];if(M.lg)return M.lg;const[L,w,H,hh,dh]=M.d,b=(x,y,z,c)=>({g:new THREE.BoxGeometry(.42,.12,.1).translate(x,y,z),c});
  if(M.lx)return M.lg=merge(M.lx(L,w,H,hh,dh,(a,bb,c,x,y,z,col,rx,ry,rz)=>({g:new THREE.BoxGeometry(a,bb,c).rotateX(rx||0).rotateY(ry||0).rotateZ(rz||0).translate(x,y,z),c:col}),(r,l,x,y,z,col)=>({g:new THREE.CylinderGeometry(r,r,l,14).rotateX(Math.PI/2).translate(x,y,z),c:col})));return M.lg=merge([b(.6,hh-.33,L/2+.09,[1,.95,.7]),b(-.6,hh-.33,L/2+.09,[1,.95,.7]),b(.6,dh-.12,-L/2-.09,[1,.1,.1]),b(-.6,dh-.12,-L/2-.09,[1,.1,.1])])}
 static init(){if(Car.sg)return;const B=(w,h,d,x,y,z,c)=>({g:new THREE.BoxGeometry(w,h,d).translate(x,y,z),c}),W=(x,z)=>({g:new THREE.CylinderGeometry(.38,.38,.3,10).rotateZ(Math.PI/2).translate(x,.38,z),c:[.04,.04,.04]});
  Car.sg=merge([B(2,.7,4.4,0,.75,0,[1,1,1]),B(1.7,.6,2.2,0,1.4,-.2,[.15,.2,.3]),W(1,1.4),W(-1,1.4),W(1,-1.4),W(-1,-1.4)]);
  Car.lg=merge([B(.4,.2,.1,.7,.8,2.2,[1,.95,.7]),B(.4,.2,.1,-.7,.8,2.2,[1,.95,.7]),B(.4,.2,.1,.7,.8,-2.2,[1,.1,.1]),B(.4,.2,.1,-.7,.8,-2.2,[1,.1,.1])]);
  const ec=document.createElement('canvas');ec.width=256;ec.height=128;const eg=ec.getContext('2d'),gr=eg.createLinearGradient(0,0,0,128);gr.addColorStop(0,'#5d93d8');gr.addColorStop(.5,'#e6eef8');gr.addColorStop(.52,'#555a60');gr.addColorStop(1,'#202226');eg.fillStyle=gr;eg.fillRect(0,0,256,128);
  Car.env=new THREE.CanvasTexture(ec);Car.env.mapping=THREE.EquirectangularReflectionMapping;
  const Mp=(g,c)=>({g,c}),bg=(a,b,c,x,y,z,rx=0)=>new THREE.BoxGeometry(a,b,c).rotateX(rx).translate(x,y,z),wh=z=>Mp(new THREE.CylinderGeometry(.42,.42,.18,16).rotateZ(Math.PI/2).translate(0,.42,z),[.04,.04,.04]);
  Car.mg=merge([wh(.95),wh(-.95),Mp(bg(.26,.34,.9,0,.72,0),[.12,.12,.14]),Mp(bg(.3,.3,.55,0,1.08,.22),[1,1,1]),Mp(bg(.3,.1,.55,0,.98,-.4),[.06,.06,.06]),Mp(bg(.3,.07,.4,0,.9,-.9,.15),[1,1,1]),
   Mp(bg(.06,.95,.06,.13,.86,.86,-.23),[.7,.7,.75]),Mp(bg(.06,.95,.06,-.13,.86,.86,-.23),[.7,.7,.75]),Mp(bg(.9,.05,.05,0,1.32,.76),[.7,.7,.75]),Mp(bg(.3,.12,.3,0,.5,.95),[1,1,1]),
   Mp(bg(.14,.14,.6,.22,.45,-.35),[.75,.75,.8]),Mp(bg(.3,.3,.3,0,.55,.1),[.18,.18,.2])]);
  Car.mlg=merge([Mp(bg(.2,.2,.12,0,1.2,1.02),[1,.95,.7]),Mp(bg(.18,.1,.08,0,.95,-1.08),[1,.1,.1])]);
  Car.lm=new THREE.MeshBasicMaterial({vertexColors:true})}
 constructor(scene,color,type,model){Car.init();this.m=new THREE.Group();const mo=type==='motorcycle',MD=model&&(mo?MOTOS:CARMODELS)[model];this.f={...(mo?C.moto:C.car)};if(MD){this.f.max*=MD.mx;this.f.acc*=MD.ac}this.col=color;this.ci=(MD&&MD.ci)||CIRC;this.model=model||null;this.nk=(MD&&MD.nk)||1;this.fc=MD&&MD.fc;this.dust=(MD&&MD.dust)||1;this.hp=type==='tank'?700:100;this.y=0;this.vy=0;this.rh=0;this.nit=0;this.nb=false;this.rx=this.rz=0;const s=new THREE.Mesh(mo?Car.mg:(MD?Car.mod(model):Car.sg),(()=>{const m=new THREE.MeshPhysicalMaterial({color,vertexColors:true,roughness:.28,metalness:.6,clearcoat:1,clearcoatRoughness:.06,envMap:Car.env,envMapIntensity:1.1});ENVM.push(m);return m})());s.castShadow=true;
  this.lmesh=new THREE.Mesh(mo?Car.mlg:(MD?Car.lmod(model):Car.lg),Car.lm);this.m.add(s,this.lmesh);this.wsz=1;this.wh=null;if(MD&&!mo){const[L2,w2]=MD.d;this.wh=[];Car._wm=Car._wm||new THREE.MeshStandardMaterial({vertexColors:true,roughness:.6});for(const[sx,sz]of[[1,1],[-1,1],[1,-1],[-1,-1]]){const gp=new THREE.Group();gp.position.set(sx*(w2/2-.1),.38,sz*L2*.31);const wm=new THREE.Mesh(Car.wg(),Car._wm);wm.castShadow=true;gp.add(wm);this.m.add(gp);this.wh.push({gp,wm,fr:sz>0})}};scene.add(this.m);this.x=this.z=this.h=this.vx=this.vz=this.sp=this.stun=0;this.ai=null;this.slip=false;this.hit=0;this.sk=0;this.body=s;this.type=type||null;if(type==='police')s.material.emissiveIntensity=.6;if(type==='tank')this.m.scale.set(1.25,1.4,1.5);if(mo&&MD&&MD.sc)this.m.scale.set(...MD.sc);this.sc0=this.m.scale.clone();if(mo){const M=c=>new THREE.MeshStandardMaterial({color:c,roughness:.8}),r=this.rider=new THREE.Group(),b=(w,h,d,m,x,y,z,rx)=>{const o=new THREE.Mesh(new THREE.BoxGeometry(w,h,d),m);o.position.set(x,y,z);o.rotation.x=rx||0;o.castShadow=true;r.add(o)};
   this.rmat=[M(0x2b6cff),M(0x222a3a),M(0xe0b090)];const H=mkHuman(this.rmat[0],this.rmat[2],this.rmat[1],M(0x2a1a10),M(0x111111));H.g.rotation.x=.42;H.aL.rotation.x=-1.15;H.aR.rotation.x=-1.15;H.lL.rotation.x=-1.55;H.lR.rotation.x=-1.55;r.add(H.g);r.position.set(0,.5,-.3);r.scale.setScalar(.85);r.visible=false;this.m.add(r)}}
 air(dt){const g0=ghOf(this.x,this.z,this.y);if(this.y>g0+.35||this.vy>0){this.vy-=22*dt;this.y+=this.vy*dt;if(this.spin){this.rx+=this.spin[0]*dt;this.rz+=this.spin[1]*dt}if(this.y<=g0){this.y=g0;if(this.vy<-4)this.vy*=-.25;else{this.vy=0;this.spin=null;this.rx=this.rz=0}}}else{this.y=g0;this.vy=0;this.spin=null;if(this.type!=='motorcycle')this.rx=0;this.rz=0}}
 step(dt,thr,st,brake,hb){const f=this.f,nb=this.nb,sn=Math.sin(this.h),cs=Math.cos(this.h);let vf=this.vx*sn+this.vz*cs,vl=this.vx*cs-this.vz*sn;
  if(thr>0)vf+=(vf<-.5?f.brake*thr:f.acc*(nb?(this.type==='motorcycle'?3.4*this.nk:3.2):1)*thr*(1-vf/(f.max*(nb?(this.type==='motorcycle'?1.35+.15*this.nk:1.7):1))))*dt;else if(thr<0)vf+=(vf>.5?f.brake*thr:f.acc*.6*thr*(1+vf/f.rev))*dt;
  if(brake)vf*=Math.exp(-3*dt);if(hb)vf-=Math.sign(vf)*Math.min(Math.abs(vf),10*dt);
  vf-=vf*f.drag*dt;if(nb)vf+=(this.type==='motorcycle'?18*this.nk:16)*dt;vf-=Math.sign(vf)*Math.min(Math.abs(vf),f.roll*dt);
  const ang=st*f.steer/(1+Math.abs(vf)*.06);this.h+=U.clamp(vf*Math.tan(ang)/f.wb,-2.6,2.6)*dt;
  const hbd=!!hb&&Math.abs(vf)>6&&this.y<=.3&&!this.wreck;
  this.gr=U.lerp(this.gr===undefined?f.grip:this.gr,hbd?2.1:f.grip,Math.min(1,dt*(hbd?14:4.5)));
  if(hbd){const sg=vf>0?1:-1,kk=Math.min(1,Math.abs(vf)/24);this.h+=st*sg*1.0*kk*dt;vf-=sg*Math.min(Math.abs(vf),(6+Math.abs(vl)*.45)*dt)}
  vl*=Math.exp(-this.gr*dt);this.drift=hbd&&Math.abs(vl)>2.2;this.dsl=Math.abs(vl);this.slip=this.drift;
  this.vx=sn*vf+cs*vl;this.vz=cs*vf-sn*vl;this.x+=this.vx*dt;this.z+=this.vz*dt;this.sp=vf;
  if(this.type==='motorcycle'&&!this.wreck)this.rx=U.lerp(this.rx,this.nb?-.32:0,Math.min(1,dt*5));this.air(dt);if(this.wh){const off=this.rh+(this.wsz-1)*.38,sp=vf*dt/(.38*this.wsz);this.m.position.set(this.x,this.y,this.z);this.body.position.y=off;this.lmesh.position.y=off;for(const w of this.wh){w.wm.rotation.x+=sp;w.gp.scale.setScalar(this.wsz);w.gp.position.y=.38*this.wsz;if(w.fr)w.gp.rotation.y=st*.45}}else this.m.position.set(this.x,this.y+this.rh,this.z);this.m.rotation.set(this.rx,this.h,this.rz);if(this.rider)this.m.rotation.z=this.lean=U.lerp(this.lean||0,U.clamp(-st*Math.min(1,Math.abs(vf)/18)*.55,-.55,.55),.12)}
 collide(w){const sn=Math.sin(this.h),cs=Math.cos(this.h);let imp=0;
  for(const o of this.ci){const cx=this.x+sn*o,cz=this.z+cs*o;
   for(const b of w.grid.at(cx,cz)){if(this.gh)continue;const r=push(cx,cz,1.05,b);if(r){if(b.tw)this.twb=b.tw;this.x+=r[0]*r[2];this.z+=r[1]*r[2];const vn=this.vx*r[0]+this.vz*r[1];
    if(vn<0){this.vx-=1.3*vn*r[0];this.vz-=1.3*vn*r[1];this.vx*=.88;this.vz*=.88;imp=Math.max(imp,-vn)}break}}}
  for(const o of this.ci){const q=Game.solidPts(this.x+sn*o,this.z+cs*o,1.05,this,true);if(q[0]||q[1]){this.x+=q[0];this.z+=q[1];const m=Math.hypot(q[0],q[1]),vn=-(this.vx*q[0]+this.vz*q[1])/m;if(vn>0){this.vx*=.6;this.vz*=.6;imp=Math.max(imp,vn)}}}if(Math.abs(this.x)>C.half){this.x=Math.sign(this.x)*C.half;this.vx=0;w.edge=true}if(this.z<-C.half||this.z>C.zs){this.z=U.clamp(this.z,-C.half,C.zs);this.vz=0;w.edge=true}
  this.hit=imp;if(this.ai&&imp>2)this.stun=2}}
function crash(cars){for(let i=0;i<cars.length;i++){const a=cars[i];for(let j=i+1;j<cars.length;j++){const b=cars[j];if(a.gh||b.gh)continue;const dx=b.x-a.x,dz=b.z-a.z;if(dx*dx+dz*dz>144||Math.abs((a.y||0)-(b.y||0))>2.5)continue;
 const as=Math.sin(a.h),ac=Math.cos(a.h),bs=Math.sin(b.h),bc=Math.cos(b.h);
 for(const p of a.ci)for(const q of b.ci){const ex=b.x+bs*q-(a.x+as*p),ez=b.z+bc*q-(a.z+ac*p),d=Math.hypot(ex,ez);
  if(d<2.1&&d>1e-4){const nx=ex/d,nz=ez/d,pen=(2.1-d)/2;a.x-=nx*pen;a.z-=nz*pen;b.x+=nx*pen;b.z+=nz*pen;const rel=(b.vx-a.vx)*nx+(b.vz-a.vz)*nz;
   if(rel<0){const ji=-1.4*rel/2;a.vx-=ji*nx;a.vz-=ji*nz;b.vx+=ji*nx;b.vz+=ji*nz;if(a.ai&&-rel>1.5)a.stun=2;if(b.ai&&-rel>1.5)b.stun=2}}}}}}

/* ===== DRIFT FX: soft tyre smoke + skid marks ===== */
class DriftFX{
 constructor(scene){
  const N=520;this.N=N;this.i=0;this.acc=[0,0];
  this.pos=new Float32Array(N*3).fill(-500);this.sz=new Float32Array(N);this.al=new Float32Array(N);this.rot=new Float32Array(N);
  this.vel=new Float32Array(N*3);this.age=new Float32Array(N).fill(99);this.life=new Float32Array(N).fill(1);
  this.s0=new Float32Array(N);this.s1=new Float32Array(N);this.a0=new Float32Array(N);this.rs=new Float32Array(N);this.hot=new Float32Array(N);this.ah=new Float32Array(N);
  const g=this.g=new THREE.BufferGeometry();
  g.setAttribute('position',new THREE.BufferAttribute(this.pos,3));
  g.setAttribute('aSize',new THREE.BufferAttribute(this.sz,1));
  g.setAttribute('aAlpha',new THREE.BufferAttribute(this.al,1));
  g.setAttribute('aRot',new THREE.BufferAttribute(this.rot,1));g.setAttribute('aHot',new THREE.BufferAttribute(this.ah,1));
  const cv=document.createElement('canvas');cv.width=cv.height=96;const c=cv.getContext('2d');
  for(let k=0;k<9;k++){const a=Math.random()*6.283,d=Math.random()*20,x=48+Math.cos(a)*d,y=48+Math.sin(a)*d,r=16+Math.random()*14,gr=c.createRadialGradient(x,y,0,x,y,r);gr.addColorStop(0,'rgba(255,255,255,.55)');gr.addColorStop(.6,'rgba(255,255,255,.22)');gr.addColorStop(1,'rgba(255,255,255,0)');c.fillStyle=gr;c.fillRect(0,0,96,96)}
  c.globalCompositeOperation='destination-in';const m=c.createRadialGradient(48,48,6,48,48,47);m.addColorStop(0,'rgba(0,0,0,1)');m.addColorStop(.75,'rgba(0,0,0,.6)');m.addColorStop(1,'rgba(0,0,0,0)');c.fillStyle=m;c.fillRect(0,0,96,96);
  const tx=new THREE.CanvasTexture(cv);
  this.mat=new THREE.ShaderMaterial({transparent:true,depthWrite:false,uniforms:{map:{value:tx},uScale:{value:600},uColor:{value:new THREE.Color(0xc4c8d0)}},
   vertexShader:'attribute float aSize;attribute float aAlpha;attribute float aRot;attribute float aHot;varying float vH;varying float vA;varying float vR;uniform float uScale;void main(){vH=aHot;vA=aAlpha;vR=aRot;vec4 mv=modelViewMatrix*vec4(position,1.);gl_Position=projectionMatrix*mv;gl_PointSize=min(aSize*uScale/max(-mv.z,.1),320.);}',
   fragmentShader:'uniform sampler2D map;uniform vec3 uColor;varying float vH;varying float vA;varying float vR;void main(){vec2 p=gl_PointCoord-.5;float c=cos(vR),s=sin(vR);p=vec2(c*p.x-s*p.y,s*p.x+c*p.y)+.5;float a=texture2D(map,p).a*vA;if(a<.004)discard;gl_FragColor=vec4(mix(uColor,vec3(1.,.5,.12),vH),a);}'});
  this.pts=new THREE.Points(g,this.mat);this.pts.frustumCulled=false;this.pts.renderOrder=3;scene.add(this.pts);
  // skid marks
  const M=700;this.M=M;this.mi=0;this.kp=new Float32Array(M*12);const ix=new Uint16Array(M*6);for(let q=0;q<M;q++){const b=q*4;ix.set([b,b+1,b+2,b+2,b+1,b+3],q*6)}
  const kg=this.kg=new THREE.BufferGeometry();kg.setAttribute('position',new THREE.BufferAttribute(this.kp,3));kg.setIndex(new THREE.BufferAttribute(ix,1));
  this.km=new THREE.Mesh(kg,new THREE.MeshBasicMaterial({color:0x0b0b0d,transparent:true,opacity:.55,depthWrite:false,polygonOffset:true,polygonOffsetFactor:-3,polygonOffsetUnits:-3}));this.km.frustumCulled=false;scene.add(this.km);
  this.prev=[null,null];
 }
 spawn(x,y,z,vx,vz,k,hot,sm){
  const i=this.i++%this.N,a=Math.random()*6.283,h=hot||0,m=sm||1,f=h?1.9:1;
  this.pos[i*3]=x+(Math.random()-.5)*.35;this.pos[i*3+1]=y;this.pos[i*3+2]=z+(Math.random()-.5)*.35;
  this.vel[i*3]=vx*.22+(Math.random()-.5)*1.6*f;this.vel[i*3+1]=(.5+Math.random()*1.1)*f;this.vel[i*3+2]=vz*.22+(Math.random()-.5)*1.6*f;
  this.age[i]=0;this.life[i]=(1.3+Math.random()*1.1)*(h?.5:1);this.s0[i]=(.6+Math.random()*.5)*m;this.s1[i]=(3.2+Math.random()*2.6)*m*(h?.7:1);
  this.a0[i]=(.16+Math.random()*.16)*k*(h?2.2:1);this.rot[i]=a;this.rs[i]=(Math.random()-.5)*.9;this.hot[i]=h;
 }
 skid(w,x,y,z){
  const pv=this.prev[w];this.prev[w]=[x,y,z];if(!pv)return;
  const dx=x-pv[0],dz=z-pv[2],d=Math.hypot(dx,dz);if(d<.12||d>3)return;
  const nx=-dz/d*.15,nz=dx/d*.15,q=(this.mi++%this.M)*12,P=this.kp;
  P[q]=pv[0]+nx;P[q+1]=pv[1]+.045;P[q+2]=pv[2]+nz;P[q+3]=pv[0]-nx;P[q+4]=pv[1]+.045;P[q+5]=pv[2]-nz;
  P[q+6]=x+nx;P[q+7]=y+.045;P[q+8]=z+nz;P[q+9]=x-nx;P[q+10]=y+.045;P[q+11]=z-nz;this.kd=1;
 }
 update(dt,car,cam,r,night){
  const N=this.N,A=this.age,k=Math.exp(-1.5*dt);
  for(let i=0;i<N;i++){const a=A[i];if(a>=this.life[i]){if(this.al[i]!==0){this.al[i]=0;this.ah[i]=0;this.sz[i]=0;this.pos[i*3+1]=-500}continue}
   const t=(A[i]=a+dt)/this.life[i],e=1-(1-t)*(1-t);
   this.vel[i*3]*=k;this.vel[i*3+2]*=k;this.vel[i*3+1]=this.vel[i*3+1]*k+.25*dt;
   this.pos[i*3]+=this.vel[i*3]*dt;this.pos[i*3+1]+=this.vel[i*3+1]*dt;this.pos[i*3+2]+=this.vel[i*3+2]*dt;
   this.sz[i]=this.s0[i]+(this.s1[i]-this.s0[i])*e;this.rot[i]+=this.rs[i]*dt;
   this.al[i]=this.a0[i]*Math.min(1,t*12)*Math.pow(1-t,1.6);this.ah[i]=this.hot[i]*Math.max(0,1-t*2.4)}
  if(car&&car.drift&&!car.wreck){
   const sn=Math.sin(car.h),cs=Math.cos(car.h),mo=car.type==='motorcycle',ws=mo?[0]:[1,-1],kk=Math.min(1,.45+car.dsl/12),rate=70*kk;
   for(let w=0;w<ws.length;w++){const s=ws[w]*.95,x=car.x+cs*s-sn*1.4,z=car.z-sn*s-cs*1.4,y=(car.y||0)+.2;
    this.acc[w]+=rate*dt;while(this.acc[w]>=1){this.acc[w]--;const f=Math.random();this.spawn(x-car.vx*dt*f,y,z-car.vz*dt*f,car.vx,car.vz,kk)}
    this.skid(w,x,(car.y||0),z)}
   if(mo)this.prev[1]=null}
  else{this.prev[0]=this.prev[1]=null;this.acc[0]=this.acc[1]=0}
  const gh=Math.max(1,(r.getDrawingBufferSize?r.getDrawingBufferSize(new THREE.Vector2()).y:innerHeight));
  this.mat.uniforms.uScale.value=gh*.5/Math.tan(cam.fov*Math.PI/360);
  this.mat.uniforms.uColor.value.setScalar(.82-.5*(night||0));
  this.g.attributes.position.needsUpdate=this.g.attributes.aSize.needsUpdate=this.g.attributes.aAlpha.needsUpdate=this.g.attributes.aRot.needsUpdate=this.g.attributes.aHot.needsUpdate=true;
  if(this.kd){this.kg.attributes.position.needsUpdate=true;this.kd=0}
 }
}
/* ===== TRAFFIC ===== */
class Traffic{constructor(w){this.w=w;this.R=w.R;this.t=0}
 st(ax){const u=(this.t+(ax?20:0))%40;return u<16?0:u<19?1:2}
 ri(n){return Math.floor(this.R()*(n?7:11))}
 nt(n){const r=this.w.ridgeCity;return n?{X:r.NX,Z:r.NZ}:{X:this.w.L,Z:this.w.L}}
 nb(i,j,ex,n){const M=n?6:10,o=[[i+1,j],[i-1,j],[i,j+1],[i,j-1]].filter(q=>q[0]>=0&&q[0]<=M&&q[1]>=0&&q[1]<=M&&!(ex&&q[0]===ex[0]&&q[1]===ex[1]));return o[Math.floor(this.R()*o.length)]}
 geo(a){const T=this.nt(a.n),Ax=T.X[a.i],Az=T.Z[a.j],dx=Math.sign(T.X[a.k]-Ax),dz=Math.sign(T.Z[a.l]-Az),ln=(a.n?8:this.w.hw(dx?a.j:a.i))/2;
  return{x:Ax-dz*ln,z:Az+dx*ln,dx,dz,len:Math.abs(T.X[a.k]-Ax)+Math.abs(T.Z[a.l]-Az)}}
 place(car,i,j,n){n=n||0;const[k,l]=this.nb(i,j,0,n);car.ai={i,j,k,l,n,v:11+this.R()*6};const g=this.geo(car.ai),s=20+this.R()*(g.len-40);
  car.x=g.x+g.dx*s;car.z=g.z+g.dz*s;car.h=Math.atan2(g.dx,g.dz);car.vx=g.dx*8;car.vz=g.dz*8;car.stun=0}
 respawn(car,px,pz){car.rx=car.rz=0;car.spin=null;car.vy=0;car.y=0;const n=pz>700&&Math.abs(px)<520?1:0,T=this.nt(n);for(let t=0;t<40;t++){const i=this.ri(n),j=this.ri(n),d=Math.hypot(T.X[i]-px,T.Z[j]-pz);if(d>C.npc.near&&d<C.npc.far){this.place(car,i,j,n);return}}}
 drive(car,dt,cars,pl){if(car.stun>0){car.stun-=dt;car.step(dt,0,0,true,false);return}
  let a=car.ai,g=this.geo(a),s=(car.x-g.x)*g.dx+(car.z-g.z)*g.dz;
  if(s>g.len-14){const[ni,nj]=this.nb(a.k,a.l,[a.i,a.j],a.n);a=car.ai={i:a.k,j:a.l,k:ni,l:nj,n:a.n,v:a.v};g=this.geo(a);s=(car.x-g.x)*g.dx+(car.z-g.z)*g.dz}
  const ts=U.clamp(Math.max(s+10,5),0,g.len),err=U.wrap(Math.atan2(g.x+g.dx*ts-car.x,g.z+g.dz*ts-car.z)-car.h);
  let tv=a.v;if(g.len-s<22)tv=7;{const rem=g.len-s,ls=this.st(g.dx?0:1);if(!a.n&&rem>16&&rem<70&&(ls===2||(ls===1&&rem>24)))tv=Math.min(tv,Math.max(0,(rem-17)*.7))}
  const sn=Math.sin(car.h),cs=Math.cos(car.h),chk=(ox,oz)=>{const rx=ox-car.x,rz=oz-car.z,ah=rx*sn+rz*cs;if(ah>0&&ah<C.npc.follow&&Math.abs(rx*cs-rz*sn)<2)tv=Math.min(tv,Math.max(0,(ah-6)*1.2))};
  for(const o of cars)if(o!==car)chk(o.x,o.z);if(pl)chk(pl.x,pl.z);
  car.step(dt,U.clamp((tv-car.sp)*.6,-1,1),U.clamp(err*1.8,-1,1),false,false)}}
/* ===== PEDESTRIANS ===== */
class Peds{constructor(w,scene){this.w=w;this.D=new THREE.Object3D();this.Lm=new THREE.Object3D();this.M=new THREE.Matrix4();this.p=[];const n=C.ped.n,R=w.R,tones=[0xe0b090,0xc68c62,0x8d5a3b,0xf1cfb0],hairs=[0x1a1208,0x4a2a14,0xc9a227,0x777777],
 bx=(a,b,c,x,y,z)=>new THREE.BoxGeometry(a,b,c).translate(x,y,z),mk=(g,cnt)=>{const m=new THREE.InstancedMesh(g,new THREE.MeshStandardMaterial({roughness:.8,vertexColors:true}),cnt);m.frustumCulled=false;m.castShadow=true;scene.add(m);return m};
 const HG=humG();this.tor=mk(HG.tor,n);this.hd=mk(HG.hd,n);this.hr=mk(HG.hr,n);this.arm=mk(HG.arm,2*n);this.hand=mk(HG.hand,2*n);this.leg=mk(HG.leg,2*n);this.shoe=mk(HG.shoe,2*n);
 for(let i=0;i<n;i++){const q={x:0,z:0,t:0,line:0,axis:0,dir:1,sp:1.5,dead:0,down:0,vx:0,vz:0,cd:0,hd:0,free:false,hp:100,gun:false};this.p.push(q);this.place(q,20,10);
  const sh=new THREE.Color().setHSL(R(),.45,.4),pn=new THREE.Color().setHSL(R(),.3,.22),sk=new THREE.Color(tones[i%4]),hr=new THREE.Color(hairs[i%4]),bk=new THREE.Color(0x111111);
  this.tor.setColorAt(i,sh);this.hd.setColorAt(i,sk);this.hr.setColorAt(i,hr);for(let s=0;s<2;s++){this.arm.setColorAt(2*i+s,sh);this.hand.setColorAt(2*i+s,sk);this.leg.setColorAt(2*i+s,pn);this.shoe.setColorAt(2*i+s,bk)}}
 this.all=[this.tor,this.hd,this.hr,this.arm,this.hand,this.leg,this.shoe]}
 place(q,px,pz){const R=this.w.R,L=this.w.L,s=R()<.5?-1:1,rg=this.w.ridgeCity;if(rg&&pz>700&&Math.abs(px)<520){q.axis=R()<.5?1:0;const A=q.axis?rg.NZ:rg.NX,i=U.clamp(Math.round(((q.axis?pz:px)-A[0])/120)+Math.floor(R()*3)-1,0,6);q.line=A[i]+10*s;q.lo=q.axis?-350:1650;q.hi=q.axis?350:2350;q.t=U.clamp((q.axis?px:pz)+(R()-.5)*C.ped.spread,q.lo,q.hi);q.dir=R()<.5?-1:1;q.sp=1.2+R()*1.6;q.dead=0;q.down=0;q.free=false;q.hp=100;q.gun=R()<.3;q.pull=0;return}q.lo=-585;q.hi=585;q.axis=R()<.5?1:0;const i=U.clamp(Math.round(((q.axis?pz:px)+600)/C.step)+Math.floor(R()*3)-1,0,10);
  q.line=L[i]+(this.w.hw(i)+2)*s;q.t=U.clamp((q.axis?px:pz)+(R()-.5)*C.ped.spread,-585,585);q.dir=R()<.5?-1:1;q.sp=1.2+R()*1.6;q.dead=0;q.down=0;q.free=false;q.hp=100;q.gun=R()<.3;q.pull=0}
 update(dt,px,pz,t,G){const D=this.D,Lm=this.Lm,M=this.M;let n=0;for(const q of this.p){const lie=(q.dead>0||q.down>0)&&!(q.pull>0);
  if(q.dead>0){q.dead-=dt;if(q.dead<=0)this.place(q,px,pz)}
  else if(q.down>0){q.down-=dt;if(q.pull>0){q.pull-=dt;q.x+=q.jv[0]*.5*dt;q.z+=q.jv[1]*.5*dt;if(q.pull<=0){q.vx=q.jv[0];q.vz=q.jv[1];q.fv=9;q.fy=.2;q.bn=0}}
   else{q.x+=q.vx*dt;q.z+=q.vz*dt;q.vx*=.93;q.vz*=.93;q.fv=(q.fv||0)-24*dt;q.fy=Math.max(0,(q.fy||0)+q.fv*dt);if(q.fy<=0){if(q.fv<-6&&!q.bn){q.fv*=-.3;q.bn=1}else q.fv=0}}}
  else if(q.free){const dx=px-q.x,dz=pz-q.z,d=Math.hypot(dx,dz)||1;q.cd-=dt;q.hd=Math.atan2(dx,dz);
   if(q.gun&&d<24&&d>2.5){if(q.cd<=0&&G){q.cd=1.3;G.pedShoot(q)}}
   else if(d>1.6){q.x+=dx/d*5.5*dt;q.z+=dz/d*5.5*dt}
   else if(q.cd<=0&&G&&!G.driving){q.cd=.9;q.atk=.35;G.hurt(7)}
   for(const b of this.w.grid.at(q.x,q.z)){const r=push(q.x,q.z,.5,b);if(r){q.x+=r[0]*r[2];q.z+=r[1]*r[2]}}
   if(d>C.ped.cull)this.place(q,px,pz)}
  else{q.t+=q.dir*q.sp*dt;if(q.t>q.hi||q.t<q.lo)q.dir=-q.dir}
  if(!q.free){q.x=q.axis?q.t:q.line;q.z=q.axis?q.line:q.t;if(q.dead<=0&&(q.x-px)**2+(q.z-pz)**2>C.ped.cull*C.ped.cull){this.place(q,px,pz);q.x=q.axis?q.t:q.line;q.z=q.axis?q.line:q.t}}
  const ry=q.free?q.hd:q.axis?(q.dir>0?Math.PI/2:-Math.PI/2):(q.dir>0?0:Math.PI),air=(q.fy||0)>.05,mv=!lie&&!(q.pull>0)&&(!q.free||Math.hypot(q.x-px,q.z-pz)>1.7),ph=t*(q.free?11:q.sp*2.6)+n*1.7;
  let aL=0,aR=0,lL=0,lR=0,bob=0;if(mv){const a=Math.sin(ph)*(q.free?1.15:.85);aL=a;aR=-a;lL=-a;lR=a;bob=Math.abs(Math.sin(ph))*.07}
  if(q.atk>0){q.atk-=dt;aR=-1.8*Math.sin((1-q.atk/.35)*Math.PI)}else if(q.free&&q.gun&&!lie&&Math.hypot(q.x-px,q.z-pz)<24)aR=-1.5;
  if(q.pull>0)aL=aR=-2.6;if(lie){aL=air?-2.4:-.5;aR=air?2.4:.5;lL=.25;lR=-.25}
  const rx=lie?(air?-(q.rt=(q.rt||0)+dt*11):-Math.PI/2):0;if(!air)q.rt=0;
  D.position.set(q.x,lie?.3+(q.fy||0):bob,q.z);D.rotation.set(rx,ry,0);D.updateMatrix();this.tor.setMatrixAt(n,D.matrix);this.hd.setMatrixAt(n,D.matrix);this.hr.setMatrixAt(n,D.matrix);
  for(let s=0;s<2;s++){const sd=s?-1:1;Lm.position.set(.4*sd,1.7,0);Lm.rotation.set(s?aR:aL,0,0);Lm.updateMatrix();M.multiplyMatrices(D.matrix,Lm.matrix);this.arm.setMatrixAt(2*n+s,M);this.hand.setMatrixAt(2*n+s,M);
   Lm.position.set(.15*sd,1,0);Lm.rotation.set(s?lR:lL,0,0);Lm.updateMatrix();M.multiplyMatrices(D.matrix,Lm.matrix);this.leg.setMatrixAt(2*n+s,M);this.shoe.setMatrixAt(2*n+s,M)}
  n++}
  for(const m of this.all)m.instanceMatrix.needsUpdate=true}}
const PM=(c,mt=.4,r=.45)=>{const m=new THREE.MeshStandardMaterial({color:c,metalness:mt,roughness:r,side:THREE.DoubleSide,envMap:(Car.init(),Car.env),envMapIntensity:.8});ENVM.push(m);m.clone=function(){const q=THREE.MeshStandardMaterial.prototype.clone.call(this);ENVM.push(q);return q};return m},
PF=(r0,r1,len,z,x=0,y=0)=>new THREE.CylinderGeometry(r1,r0,len,12).rotateX(Math.PI/2).translate(x,y,z),
PW=(pts,th,y,z)=>{const sh=new THREE.Shape();pts.forEach((p,i)=>i?sh.lineTo(p[0],p[1]):sh.moveTo(p[0],p[1]));const g=new THREE.ExtrudeGeometry(sh,{depth:th,bevelEnabled:false});g.rotateX(-Math.PI/2);g.translate(0,y,z);return g},
PA=(g,mt,gr,x=0,y=0,z=0)=>{const o=new THREE.Mesh(g,mt);o.position.set(x,y,z);o.castShadow=true;gr.add(o);return o},
PG=(gr,mt,list,r)=>{for(const[x,y,z]of list)PA(new THREE.CylinderGeometry(r,r,r*.7,10).rotateZ(Math.PI/2),mt,gr,x,y,z)},
PLANES={
 Cessna:{name:'Cessna 172',vm:62,vs:24,gy:1.05,camd:17,span:8,jet:0,x:-300,build(){const g=new THREE.Group(),w=PM(0xf2f2f2),r=PM(0xc0392b),k=PM(0x222222),gl=PM(0x2a4a6a,.8,.1);
  PA(PF(.25,.55,7,0),w,g);PA(PW([[-5.5,0],[5.5,0],[5.5,1.5],[-5.5,1.5]],.12,.62,1.2),w,g);PA(PW([[-1.9,0],[1.9,0],[1.9,.9],[-1.9,.9]],.1,.3,-3.1),w,g);PA(new THREE.BoxGeometry(.1,1.3,1.1),r,g,0,.9,-3.1);
  const c=PA(new THREE.SphereGeometry(.5,10,8),gl,g,0,.5,.7);c.scale.set(.9,.7,1.5);g.prop=new THREE.Group();g.prop.position.z=3.55;g.add(g.prop);PA(new THREE.BoxGeometry(.12,2,.1),k,g.prop);PA(new THREE.BoxGeometry(2,.12,.1),k,g.prop);PG(g,k,[[.8,-.75,.9],[-.8,-.75,.9],[0,-.75,2.5]],.25);return g}},
 Boeing:{name:'Boeing 737',vm:118,vs:46,gy:3,camd:42,span:20,jet:0,x:-170,build(){const g=new THREE.Group(),w=PM(0xf4f6f8),b=PM(0x1f4e8c),k=PM(0x222222),gl=PM(0x1a2a3a,.8,.1);
  PA(PF(1.9,1.9,30,0),w,g);PA(PF(1.9,.4,8,19),w,g);PA(PF(.5,1.9,9,-19.5),w,g);PA(PW([[-17,5.5],[-17,7.7],[0,9],[17,7.7],[17,5.5],[0,0]],.3,-.9,4),w,g);
  for(const s of[1,-1]){PA(PF(.8,.9,3.4,5,s*6,-2),k,g)}PA(PW([[-6.5,3],[-6.5,4.6],[0,5],[6.5,4.6],[6.5,3],[0,0]],.2,.9,-17),w,g);PA(new THREE.BoxGeometry(.25,6,5),b,g,0,4.2,-19);
  const c=PA(new THREE.SphereGeometry(.9,10,8),gl,g,0,.8,20.2);c.scale.set(1,.5,.8);PG(g,k,[[2,-2.4,3],[-2,-2.4,3],[0,-2.4,16]],.55);return g}},
 F35:{name:'F-35 Lightning II',vm:235,vs:42,gy:1.6,camd:26,span:8,jet:1,x:-30,build(){const g=new THREE.Group(),w=PM(0x5c636c,.6,.35),d=PM(0x2a2d33),gl=PM(0xd8a030,.9,.05);
  PA(PF(.95,.95,12,0),w,g);PA(PF(.95,.1,5,8.5),w,g);PA(PF(.55,.95,3.5,-7.75),w,g);PA(PF(.5,.6,1.2,-10),d,g);
  PA(PW([[-5.5,3],[-5.5,4.4],[0,5.6],[5.5,4.4],[5.5,3],[0,0]],.15,-.1,1.6),w,g);PA(PW([[-3,1.6],[-3,3],[0,3.4],[3,3],[3,1.6],[0,0]],.12,0,-6),w,g);
  for(const s of[1,-1]){const f=PA(new THREE.BoxGeometry(.1,2.1,2),w,g,s*.95,1.5,-7);f.rotation.z=-s*.28}
  const c=PA(new THREE.SphereGeometry(.7,10,8),gl,g,0,.85,3);c.scale.set(.8,.7,2.6);PG(g,d,[[1.2,-1.2,0],[-1.2,-1.2,0],[0,-1.2,6]],.3);return g}},
 Sukhoi:{name:'Sukhoi Su-57',vm:255,vs:40,gy:1.6,camd:28,span:10,jet:1,x:100,build(){const g=new THREE.Group(),w=PM(0x4d555e,.6,.35),d=PM(0x15171a),gl=PM(0xb08a30,.9,.05);
  PA(PF(.8,.8,13,0),w,g);PA(PF(.8,.08,6,9.5),w,g);PA(PF(.5,.8,3,-8),w,g);
  for(const s of[1,-1]){PA(PF(.6,.65,7,-6,s*1.25,-.2),w,g);PA(PF(.5,.55,1,-10,s*1.25,-.2),d,g);const f=PA(new THREE.BoxGeometry(.1,2.6,2.2),w,g,s*1.9,1.4,-7.5);f.rotation.z=-s*.3}
  PA(PW([[-7.4,2.8],[-7.4,4.4],[0,6.2],[7.4,4.4],[7.4,2.8],[0,0]],.16,-.1,2),w,g);PA(PW([[-3.8,1.8],[-3.8,3.2],[0,3.8],[3.8,3.2],[3.8,1.8],[0,0]],.12,0,-6.5),w,g);
  const c=PA(new THREE.SphereGeometry(.7,10,8),gl,g,0,.8,4);c.scale.set(.75,.65,2.8);PG(g,d,[[1.4,-1.1,0],[-1.4,-1.1,0],[0,-1.1,6.5]],.3);return g}},
 B2:{name:'B-2 Spirit',vm:160,vs:48,gy:1.5,camd:44,span:28,jet:1,x:250,build(){const g=new THREE.Group(),w=PM(0x2b2e33,.5,.5),gl=PM(0x111418,.9,.05);
  PA(PW([[0,0],[26,13],[26,15.5],[14,14],[9,14.5],[4,18.5],[0,16.5],[-4,18.5],[-9,14.5],[-14,14],[-26,15.5],[-26,13]],1.1,-.55,9),w,g);
  const c=PA(new THREE.SphereGeometry(1,10,8),w,g,0,.5,2);c.scale.set(2.2,.9,5);for(const s of[1,-1]){const e=PA(new THREE.SphereGeometry(1,10,8),w,g,s*3.2,.5,-3);e.scale.set(1.5,.8,4)}
  const k=PA(new THREE.SphereGeometry(.8,10,8),gl,g,0,.9,5.5);k.scale.set(1.2,.6,1.8);PG(g,gl,[[2.6,-1.2,0],[-2.6,-1.2,0],[0,-1.2,5]],.45);return g}}};
{const RC=(k,m)=>function(){const g=PLANES[k].build();g.traverse(o=>{if(o.isMesh&&o.material&&o.material.color){const h=o.material.color.getHex();if(m[h]!=null){o.material=o.material.clone();o.material.color.setHex(m[h])}}});return g};
Object.assign(PLANES,{
Biplane:{name:'Vintage Biplane',vm:48,vs:20,gy:.95,camd:15,span:5,jet:0,x:-450,z:-690,build(){const g=new THREE.Group(),w=PM(0xd8c070),r=PM(0xb03030),k=PM(0x222222),gl=PM(0x2a4a6a,.8,.1);
 PA(PF(.35,.6,5.5,0),r,g);const wp=[[-4.6,0],[4.6,0],[4.6,1.3],[-4.6,1.3]];PA(PW(wp,.1,-.1,1),w,g);PA(PW(wp,.1,1.5,1),w,g);
 for(const s of[1,-1])for(const z of[.3,1.8])PA(new THREE.BoxGeometry(.08,1.6,.08),k,g,s*2.4,.7,z);
 PA(PW([[-1.6,0],[1.6,0],[1.6,.8],[-1.6,.8]],.08,.2,-2.9),w,g);PA(new THREE.BoxGeometry(.08,1.1,.9),r,g,0,.75,-2.9);const c=PA(new THREE.SphereGeometry(.4,8,6),gl,g,0,.6,.5);c.scale.set(.9,.7,1.3);
 g.prop=new THREE.Group();g.prop.position.z=3.15;g.add(g.prop);PA(new THREE.BoxGeometry(.1,2.2,.1),k,g.prop);PA(new THREE.BoxGeometry(2.2,.1,.1),k,g.prop);PG(g,k,[[.7,-.75,.9],[-.7,-.75,.9],[0,-.6,-2.6]],.22);return g}},
Learjet:{name:'Learjet 75',vm:150,vs:36,gy:1.4,camd:22,span:8,jet:0,x:-235,build(){const g=new THREE.Group(),w=PM(0xf4f6f8),b=PM(0x2c3e66),k=PM(0x222222),gl=PM(0x1a2a3a,.8,.1);
 PA(PF(.9,.9,10,0),w,g);PA(PF(.9,.15,3.5,6.75),w,g);PA(PF(.25,.9,4,-7),w,g);PA(PW([[-5.5,2],[-5.5,3],[0,3.6],[5.5,3],[5.5,2],[0,0]],.15,-.3,1.5),w,g);
 PA(PW([[-2.2,1],[-2.2,1.8],[0,2.1],[2.2,1.8],[2.2,1],[0,0]],.1,1.7,-6),w,g);PA(new THREE.BoxGeometry(.12,2.2,1.8),b,g,0,1.6,-6.6);
 for(const s of[1,-1])PA(PF(.4,.45,2.4,-5,s*1.3,.5),k,g);const c=PA(new THREE.SphereGeometry(.7,10,8),gl,g,0,.5,5);c.scale.set(.9,.6,1.4);PG(g,k,[[.9,-1.1,.5],[-.9,-1.1,.5],[0,-1.1,5]],.3);return g}},
Concorde:{name:'Concorde',vm:210,vs:56,gy:2.8,camd:36,span:9,jet:0,z:-690,x:-100,build(){const g=new THREE.Group(),w=PM(0xf6f6f6),k=PM(0x222222),gl=PM(0x1a2a3a,.8,.1);
 PA(PF(1,1,26,0),w,g);PA(PF(1,.2,8,17),w,g);PA(PF(.4,1,5,-15.5),w,g);PA(PW([[0,0],[9,16],[-9,16]],.3,-.6,6),w,g);PA(new THREE.BoxGeometry(.2,4,4),w,g,0,3,-13);
 for(const s of[1,-1])for(const x of[2.2,3.8])PA(PF(.6,.7,5,-8,s*x,-1.3),k,g);const c=PA(new THREE.SphereGeometry(.8,10,8),gl,g,0,.7,15);c.scale.set(.8,.5,1.2);PG(g,k,[[2.3,-2.3,-3],[-2.3,-2.3,-3],[0,-2.3,11]],.5);return g}},
Heli:{name:'Apache Helicopter',vm:62,vs:1,gy:1.15,camd:20,span:5,jet:1,heli:1,x:330,build(){const g=new THREE.Group(),w=PM(0x2d3b2a,.5,.4),k=PM(0x1a1a1a),gl=PM(0x2a4a6a,.9,.1);
 const bd=PA(new THREE.SphereGeometry(1,12,10),w,g,0,0,0);bd.scale.set(1.1,1.05,2.7);PA(PF(.2,.55,5,-3.8),w,g);PA(new THREE.BoxGeometry(.1,1.4,.9),w,g,0,.9,-6);PA(new THREE.BoxGeometry(2.4,.08,.5),w,g,0,-.1,-6.2);
 const c=PA(new THREE.SphereGeometry(.8,10,8),gl,g,0,.45,1.9);c.scale.set(.8,.7,1.4);PA(new THREE.BoxGeometry(3.8,.1,.7),w,g,0,.1,.2);
 for(const s of[1,-1]){PA(PF(.18,.18,1.8,.3,s*1.9,-.1),k,g);PA(new THREE.BoxGeometry(.1,.1,3.4),k,g,s*.95,-1.05,0);PA(new THREE.BoxGeometry(.08,.9,.08),k,g,s*.9,-.6,.8);PA(new THREE.BoxGeometry(.08,.9,.08),k,g,s*.9,-.6,-.8)}
 PA(new THREE.CylinderGeometry(.12,.12,.8,6),k,g,0,1.2,0);g.prop=new THREE.Group();g.prop.position.y=1.65;g.add(g.prop);PA(new THREE.BoxGeometry(9,.05,.3),k,g.prop);PA(new THREE.BoxGeometry(.3,.05,9),k,g.prop);return g}},
Airbus:{name:'Airbus A320',vm:112,vs:44,gy:3,camd:40,span:18,jet:0,z:-690,x:-300,build:RC('Boeing',{0x1f4e8c:0xd03a2a})},
Raptor:{name:'F-22 Raptor',vm:260,vs:42,gy:1.6,camd:28,span:9,jet:1,x:35,build:RC('Sukhoi',{0x4d555e:0x8a96a6})},
Stunt:{name:'Stunt Plane',vm:70,vs:24,gy:1.05,camd:17,span:7,jet:0,x:-390,z:-690,build:RC('Cessna',{0xc0392b:0xf1c40f,0xf2f2f2:0x222222})}})}
{const V=(base,name,map,o)=>{const B=PLANES[base];return{...B,name,...(o||{}),build(){const g=B.build();g.traverse(m=>{if(m.isMesh&&m.material&&m.material.color){const h=m.material.color.getHex();if(map[h]!=null){m.material=m.material.clone();m.material.color.setHex(map[h])}}});return g}}};
const VS=(b,n,m,sc,o)=>{const v=V(b,n,m,o),f=v.build;v.build=function(){const g=f();g.scale.setScalar(sc);return g};v.gy=PLANES[b].gy*sc;v.camd=PLANES[b].camd*sc;v.span=PLANES[b].span*sc;return v};
Object.assign(PLANES,{F16:V('F35','F-16 Fighting Falcon',{0x5c636c:0x7b838d},{vm:245,vs:38}),F15:V('Sukhoi','F-15 Eagle',{0x4d555e:0x8c97a3},{vm:250}),F18:V('F35','F/A-18 Super Hornet',{0x5c636c:0x3d4f6e},{vm:240}),MiG29:V('Sukhoi','MiG-29 Fulcrum',{0x4d555e:0x5d6b4a},{vm:240}),Su35:V('Sukhoi','Su-35 Flanker',{0x4d555e:0x2f343b,0xb08a30:0x30a0d0},{vm:265}),Typhoon:V('Raptor','Eurofighter Typhoon',{0x8a96a6:0xcdd3da},{vm:255}),A10:V('F35','A-10 Warthog',{0x5c636c:0x4b5a3a},{vm:175,vs:34}),SR71:VS('Sukhoi','SR-71 Blackbird',{0x4d555e:0x101114,0xb08a30:0x222222},1.25,{vm:360,vs:55}),Tornado:V('F35','Tornado GR4',{0x5c636c:0x9a9f6a},{vm:225}),F117:V('B2','F-117 Nighthawk',{0x2b2e33:0x1a1c20},{vm:200}),A380:VS('Boeing','Airbus A380',{0xf4f6f8:0xf0f0f4,0x1f4e8c:0x6a2a8c},1.5,{vm:125,vs:50}),Gulfstream:V('Learjet','Gulfstream G650',{0x2c3e66:0xb8923a},{vm:165}),Heli4:V('Heli','Black Hawk Combat',{0x2d3b2a:0x111111}),Heli5:V('Heli','Desert Apache',{0x2d3b2a:0xb59a6a}),Cessna4:V('Cessna','Cessna Yellow',{0xc0392b:0xf1c40f}),Stunt3:V('Stunt','Stunt Plane Blue',{0xf1c40f:0x2c7be5})});
Object.assign(PLANES,{Cessna2:V('Cessna','Cessna Sky Blue',{0xc0392b:0x2c7be5}),Cessna3:V('Cessna','Cessna Green',{0xc0392b:0x27ae60}),Stunt2:V('Stunt','Stunt Plane Red',{0xf1c40f:0xe74c3c}),Biplane2:V('Biplane','Blue Biplane',{0xd8c070:0x4a90d9}),Learjet2:V('Learjet','Learjet Red',{0x2c3e66:0xc0392b}),
Boeing2:V('Boeing','Boeing 737 Green',{0x1f4e8c:0x2e8b57}),Cargo:V('Boeing','Cargo Freighter',{0xf4f6f8:0xc9a46a,0x1f4e8c:0x7a5a2a}),Airbus2:V('Airbus','Airbus A320 Blue',{0xd03a2a:0x2c3e66}),F35b:V('F35','F-35B Navy',{0x5c636c:0x3a4a6a}),Sukhoi2:V('Sukhoi','Su-57 Desert',{0x4d555e:0xb59a6a}),
Raptor2:V('Raptor','F-22 Shadow',{0x8a96a6:0x1a1c20}),B2b:V('B2','B-2 Steel',{0x2b2e33:0x555a63}),Heli2:V('Heli','Police Helicopter',{0x2d3b2a:0x1c2a48}),Heli3:V('Heli','Rescue Helicopter',{0x2d3b2a:0xb03030})})}
function mkShip(kind){const g=new THREE.Group(),M=(c,e,em,m,r)=>new THREE.MeshStandardMaterial({color:c,roughness:r==null?.4:r,metalness:m==null?.6:m,emissive:e||0,emissiveIntensity:em||0}),
 A=(geo,mat,x,y,z,rx,rz)=>{const o=new THREE.Mesh(geo,mat);o.position.set(x,y,z);if(rx)o.rotation.x=rx;if(rz)o.rotation.z=rz;o.castShadow=true;g.add(o);return o},
 cy=(a,b,h,s)=>new THREE.CylinderGeometry(a,b,h,s||16),W=M(0xeeeeee),K=M(0x15151a),R=M(0xc83a12,0,0,.3),F=M(0xff9a30,0xff6a10,1.6,0,.5),O=M(0xe07a30,0,0,.1,.8);
 if(kind==='shuttle'){A(cy(1.7,1.7,15),O,0,7.5,0);A(new THREE.ConeGeometry(1.7,3,16),O,0,16.5,0);A(cy(1.05,1.05,9),W,0,6.5,2.9);A(new THREE.ConeGeometry(1.05,3,16),K,0,12.5,2.9);A(new THREE.BoxGeometry(7.5,.3,4.2),W,0,3.2,2.9);A(new THREE.BoxGeometry(.3,3.5,2.5),W,0,3.4,1.5);
  for(const s of[1,-1]){(g.bs=g.bs||[]).push(A(cy(.75,.75,12),W,s*3,6,0),A(new THREE.ConeGeometry(.75,2.4,12),W,s*3,13.2,0),A(new THREE.ConeGeometry(.6,1.6,10),F,s*3,-.8,0,Math.PI));A(new THREE.ConeGeometry(.5,1.4,10),F,s*.7,.1,2.9,Math.PI)}A(new THREE.ConeGeometry(.9,1.8,10),F,0,-.9,0,Math.PI)}
 else if(kind==='capsule'){A(cy(1.9,1.9,17),W,0,8.5,0);A(cy(1.92,1.92,1.2),K,0,5,0);A(cy(1.92,1.92,1.2),K,0,11,0);A(cy(.9,1.9,3.5),M(0xc9ccd4),0,19.2,0);A(new THREE.ConeGeometry(.9,2,16),W,0,22,0);g.es=[A(cy(.1,.1,3.5,6),K,0,25.5,0),A(new THREE.ConeGeometry(.25,.9,8),R,0,27.6,0)];
  for(let i=0;i<4;i++){const a=i*Math.PI/2+Math.PI/4;A(new THREE.BoxGeometry(.25,4,3),R,Math.cos(a)*2.4,2,Math.sin(a)*2.4).rotation.y=-a}A(new THREE.ConeGeometry(1.4,2.2,14),F,0,-1.1,0,Math.PI)}
 else{const C=M(0x1a2640,0x36f1ff,.25,.9,.2),G2=M(0x36f1ff,0x36f1ff,2,0,.3);A(new THREE.ConeGeometry(2.4,12,20),M(0xdfe8f2,0,0,.9,.15),0,15,0);A(cy(2.4,2.4,8,20),C,0,5,0);A(new THREE.ConeGeometry(2.4,3,20),K,0,-1.5,0,Math.PI);
  g.ring=A(new THREE.TorusGeometry(5.2,.3,10,48),G2,0,8,0,Math.PI/2);A(new THREE.SphereGeometry(1.1,16,12),G2,0,8,0);
  for(let i=0;i<3;i++){const a=i*Math.PI*2/3;const f=A(new THREE.BoxGeometry(.2,6,3.6),C,Math.cos(a)*3.4,3,Math.sin(a)*3.4);f.rotation.y=-a;A(new THREE.ConeGeometry(.5,1.2,8),G2,Math.cos(a)*3.4,-.7,Math.sin(a)*3.4,Math.PI)}}
 return g}

PLANES.Hauler={...PLANES.Boeing,name:'Cargo Hauler (carries cars)',vm:105,vs:42,gy:3.2,camd:62,span:36,heli:0,x:-200,bay:1,build(){
 const g=new THREE.Group(),M=(c,r=.7,m=.1)=>new THREE.MeshStandardMaterial({color:c,roughness:r,metalness:m}),G=-3.2,B=(w,h,d)=>new THREE.BoxGeometry(w,h,d),
 A=(geo,mt,x,y,z)=>{const o=new THREE.Mesh(geo,mt);o.position.set(x,y,z);o.castShadow=o.receiveShadow=true;g.add(o);return o},
 hull=M(0x5d6b4a),inn=M(0x3a3e45,.9,.2),fl=G+.25,H=5.6,cy=fl+H/2;
 A(B(7,.3,44),inn,0,G+.1,0);A(B(.3,H,44),hull,3.5,cy,0);A(B(.3,H,44),hull,-3.5,cy,0);A(B(7.3,.3,44),hull,0,fl+H,0);A(B(7,H,.3),hull,0,cy,22);
 A(new THREE.ConeGeometry(3.6,9,14).rotateX(Math.PI/2),hull,0,cy+.2,26.5);A(B(5,1,2),M(0x15222e,.2,.6),0,cy+1.6,24.5);
 A(B(.5,7,7),hull,0,fl+H+3.2,-17.5);A(B(15,.4,4),hull,0,fl+H+3,-18);A(B(38,.6,6.5),hull,0,fl+H+.5,3);
 for(const x of[-14,-8,8,14])A(new THREE.CylinderGeometry(1,1,3.6,12).rotateX(Math.PI/2),M(0x30343a),x,fl+H-.9,5.5);
 for(const s of[-1,1])for(const z of[-7,7]){A(new THREE.CylinderGeometry(.85,.85,.9,12).rotateZ(Math.PI/2),M(0x111111,.9,0),s*4.4,G+.85,z);A(B(.5,1.2,.5),M(0x555555),s*4.1,G+1.5,z)}
 for(const z of[-16,-8,0,8,16])A(B(.8,.15,3),new THREE.MeshBasicMaterial({color:0xffe9a0}),0,fl+H-.2,z);
 for(const s of[-1,1])A(B(.3,.04,43),new THREE.MeshBasicMaterial({color:0xffd24a}),s*3,fl+.03,0);
 const rp=new THREE.Group();rp.position.set(0,fl,-22);g.add(rp);const pl=new THREE.Mesh(B(6.9,H,.3),hull);pl.position.set(0,H/2,0);pl.castShadow=true;rp.add(pl);g.ramp=rp;return g}};
function mkSkin(g){g.updateMatrixWorld(true);const inv=new THREE.Matrix4().copy(g.matrixWorld).invert(),v=new THREE.Vector3(),tri=[],inSub=(o,t)=>{for(let p=o;p&&p!==g;p=p.parent)if(p===t)return 1;return 0};
let x0=1e9,x1=-1e9,z0=1e9,z1=-1e9;
g.traverse(o=>{if(!o.isMesh||!o.geometry.attributes.position||(g.prop&&inSub(o,g.prop)))return;const m=new THREE.Matrix4().multiplyMatrices(inv,o.matrixWorld),pa=o.geometry.attributes.position,ix=o.geometry.index,V=[];
 for(let i=0;i<pa.count;i++){v.fromBufferAttribute(pa,i).applyMatrix4(m);V.push(v.x,v.y,v.z);x0=Math.min(x0,v.x);x1=Math.max(x1,v.x);z0=Math.min(z0,v.z);z1=Math.max(z1,v.z)}
 const n=ix?ix.count:pa.count,rp=g.ramp&&inSub(o,g.ramp)?1:0;for(let i=0;i<n;i+=3)tri.push([V,(ix?ix.getX(i):i)*3,(ix?ix.getX(i+1):i+1)*3,(ix?ix.getX(i+2):i+2)*3,rp])});
const c=Math.max(.3,Math.max(x1-x0,z1-z0)/110),nx=Math.ceil((x1-x0)/c)+2,nz=Math.ceil((z1-z0)/c)+2,N=nx*nz,mn=new Float32Array(N).fill(1e9),mx=new Float32Array(N).fill(-1e9),rmn=new Float32Array(N).fill(1e9),rmx=new Float32Array(N).fill(-1e9);
x0-=c;z0-=c;
for(const[V,a,b,d,rp]of tri){const A=[V[a],V[a+1],V[a+2]],B=[V[b],V[b+1],V[b+2]],D=[V[d],V[d+1],V[d+2]],e=Math.max(Math.hypot(B[0]-A[0],B[2]-A[2]),Math.hypot(D[0]-A[0],D[2]-A[2]),Math.hypot(D[0]-B[0],D[2]-B[2])),k=Math.max(1,Math.ceil(e/(c*.55))),lo=rp?rmn:mn,hi=rp?rmx:mx;
 for(let i=0;i<=k;i++)for(let j=0;j<=k-i;j++){const u=i/k,w=j/k,t=1-u-w,x=A[0]*t+B[0]*u+D[0]*w,y=A[1]*t+B[1]*u+D[1]*w,z=A[2]*t+B[2]*u+D[2]*w,ci=Math.floor((x-x0)/c),cj=Math.floor((z-z0)/c);if(ci<0||cj<0||ci>=nx||cj>=nz)continue;const q=cj*nx+ci;if(y<lo[q])lo[q]=y;if(y>hi[q])hi[q]=y}}
if(g.ramp)for(let j=0;j<nz;j++)for(let i=0;i<nx;i++){const x=x0+(i+.5)*c,z=z0+(j+.5)*c;if(Math.abs(x)<3.3&&z>-22.6&&z<21.8&&mx[j*nx+i]>-1e8)mn[j*nx+i]=Math.max(mn[j*nx+i],2.55)}
const pts=[];for(let j=0;j<nz;j+=2)for(let i=0;i<nx;i+=2){const q=j*nx+i;if(mx[q]>-1e8){const x=x0+(i+.5)*c,z=z0+(j+.5)*c;pts.push(x,mn[q],z);if(mx[q]-mn[q]>.3)pts.push(x,mx[q],z)}}
return{c,nx,nz,x0,z0,mn,mx,rmn,rmx,pts:pts}}
function subdivGeo(geo,n){const g=geo.index?geo.toNonIndexed():geo,pa=g.attributes.position,o=[];
 for(let i=0;i<pa.count;i+=3){const A=[pa.getX(i),pa.getY(i),pa.getZ(i)],B=[pa.getX(i+1),pa.getY(i+1),pa.getZ(i+1)],C=[pa.getX(i+2),pa.getY(i+2),pa.getZ(i+2)],P=(r,c)=>[A[0]+(B[0]-A[0])*c/n+(C[0]-A[0])*r/n,A[1]+(B[1]-A[1])*c/n+(C[1]-A[1])*r/n,A[2]+(B[2]-A[2])*c/n+(C[2]-A[2])*r/n];
  for(let r=0;r<n;r++)for(let c=0;c<n-r;c++){o.push(...P(r,c),...P(r,c+1),...P(r+1,c));if(c<n-r-1)o.push(...P(r,c+1),...P(r+1,c+1),...P(r+1,c))}}
 const r=new THREE.BufferGeometry();r.setAttribute('position',new THREE.Float32BufferAttribute(o,3));return r}
function jagX(z,y,ph){return .55*Math.sin(z*2.3+ph)+.4*Math.sin(z*5.1+y*3+ph*2)+.25*Math.sin(z*9.7+ph*3)}
function clipGeo(geo,f){const g=geo.index?geo.toNonIndexed():geo,pa=g.attributes.position,o=[];
 for(let i=0;i<pa.count;i+=3){const T=[0,1,2].map(k=>[pa.getX(i+k),pa.getY(i+k),pa.getZ(i+k)]),poly=[];
  for(let k=0;k<3;k++){const a=T[k],b=T[(k+1)%3],fa=f(a),fb=f(b);if(fa>=0)poly.push(a);if((fa>=0)!==(fb>=0)){const t=fa/(fa-fb);poly.push([a[0]+(b[0]-a[0])*t,a[1]+(b[1]-a[1])*t,a[2]+(b[2]-a[2])*t])}}
  for(let k=1;k<poly.length-1;k++)o.push(...poly[0],...poly[k],...poly[k+1])}
 const r=new THREE.BufferGeometry();r.setAttribute('position',new THREE.Float32BufferAttribute(o,3));r.computeVertexNormals();return r}
function B_(pl,st){pl.brk.sp=st}
function pdebStep(G,dt){const a=G.pdeb;if(!a||!a.length)return;for(let i=a.length-1;i>=0;i--){const d=a[i],m=d.m;d.t+=dt;
  if(m.position.y>.15||d.vy>0){d.vy-=24*dt;m.position.x+=d.vx*dt;m.position.y+=d.vy*dt;m.position.z+=d.vz*dt;m.rotation.x+=d.wx*dt;m.rotation.y+=d.wy*dt;m.rotation.z+=d.wz*dt;
   if(d.fire&&d.t<5&&G.dfx){G.dfx.spawn(m.position.x,m.position.y,m.position.z,d.vx,d.vz,1.4,Math.random()<.6?1:0,.8)}
   if(m.position.y<=.15&&d.vy<0){m.position.y=.15;if(d.vy<-6){d.vy*=-.25;d.vx*=.5;d.vz*=.5;d.wx*=.4;d.wy*=.4;d.wz*=.4;if(G.dfx&&d.big)for(let k=0;k<8;k++)G.dfx.spawn(m.position.x+(Math.random()-.5)*3,.5,m.position.z+(Math.random()-.5)*3,0,0,1.3,k<3?1:0,1.2)}else{d.vy=0;d.vx=d.vz=0;d.wx=d.wy=d.wz=0}}}
  if(d.t>25){G.scene.remove(m);m.geometry.dispose();a.splice(i,1)}}}
class Plane{constructor(sc,key){const P=PLANES[key];this.P=P;this.g=P.build();this.prop=this.g.prop;sc.add(this.g);this.sk=P.sk||(P.sk=mkSkin(this.g));this.hx=P.x;this.hz=P.z||-650;this.hh=Math.PI/2;this.fl=true;this.camd=P.camd;this.gy=P.gy;this.reset()}
 flyH(dt,k,G){const P=this.P,up=(k.ShiftLeft?1:0)-(k.Space?1:0),pit=(k.KeyS?1:0)-(k.KeyW?1:0),rol=(k.KeyA?1:0)-(k.KeyD?1:0),e=m=>1-Math.exp(-dt*m),f0=this.gl||0;
  let vt=up*14;if(vt<0)vt=Math.max(vt,-(Math.max(0,this.y-f0)*1.5+1.2));
  this.th=U.lerp(this.th,(this.y-f0>.1||up>0)?1:0,e(2));this.vy=U.lerp(this.vy||0,vt,e(2.5));this.p=U.lerp(this.p,pit*.3,e(2.5));this.r=U.lerp(this.r,rol*.35,e(3));
  this.v=U.lerp(this.v,pit<0?P.vm:pit>0?-P.vm*.35:0,e(.9));this.h+=rol*1.3*dt;const ox=this.x,oz=this.z,oy=this.y;this.y+=this.vy*dt;this.x+=Math.sin(this.h)*this.v*dt;this.z+=Math.cos(this.h)*this.v*dt;this.sp=Math.abs(this.v);
  this.col();let crash=null,fl=0;const bs=G.world.grid.at(this.x,this.z).filter(b=>!G.ghost);for(const b of bs)if(this.x>b.x0&&this.x<b.x1&&this.z>b.z0&&this.z<b.z1&&oy>=b.h-.6)fl=Math.max(fl,b.h);
  if(!G.ghost){const b=this.bHit(G,(b,y)=>y<b.h-.6&&!(this.x>b.x0&&this.x<b.x1&&this.z>b.z0&&this.z<b.z1&&oy>=b.h-.6));if(b){if(this.y>1&&Math.abs(this.v)>14){crash='collision';this.hb=b}this.x=ox;this.z=oz;this.v=0}}
  if(this.mtHit(G.world.mt))crash='mountain collision';if(this.v>1&&G.hitObj(this)){if(this.y>1&&Math.abs(this.v)>14)crash='collision';this.x=ox;this.z=oz;this.v=0}this.gl=fl;if(this.y<=fl){if(this.vy<-14)crash='hard landing';this.y=fl;this.vy=Math.max(0,this.vy);if(!up)this.v*=Math.exp(-2*dt)}
  this.x=U.clamp(this.x,-1250,1250);this.z=U.clamp(this.z,-1250,3250);if(this.prop)this.prop.rotation.y+=dt*(12+this.th*45);this.place();return crash}
 reset(){this.brk=null;this.vy=0;this.x=this.hx;this.z=this.hz;this.h=this.hh;this.y=0;this.v=0;this.th=0;this.p=0;this.r=0;this.sp=0;this.alive=true;this.dead=0;this.g.visible=true;this.g.rotation.order='YXZ';this.place()}
 place(){this.g.position.set(this.x,this.y+this.gy,this.z);this.g.rotation.set(-this.p,this.h,-this.r)}
 fly(dt,k,G){if(this.P.heli)return this.flyH(dt,k,G);if(this.brk)return this.brokenStep(dt,G);const P=this.P,ctrl=U.clamp(this.v/P.vs,0,1);this.th=U.clamp(this.th+((k.ShiftLeft?1:0)-(k.Space?1:0))*.45*dt,0,1);
  this.v+=(this.th*P.vm-this.v)*(1-Math.exp(-dt*(this.th*P.vm>this.v?.45:.6)));
  const gnd=this.y<=.05,pit=(gnd&&this.v/P.vs>=.85&&this.th>.5)?1:(k.KeyS?1:0)-(k.KeyW?1:0),rol=(k.KeyA?1:0)-(k.KeyD?1:0);if(gnd&&this.th<.02)this.v*=Math.exp(-.5*dt);
  const lift=U.clamp((this.v/P.vs-.75)/.25,0,1);this.p+=pit*(gnd&&lift<1?0:1)*(P.jet?1.5:.9)*dt*Math.max(ctrl,.15);if(!pit){if(!gnd&&Math.abs(this.p)>1.57)this.p+=Math.sign(this.p)*1.3*dt;else this.p*=Math.exp(-.3*dt)}if(gnd)this.p=U.clamp(this.p,0,1.2);else this.p=U.wrap(this.p);if(!gnd&&lift<1)this.p-=(1-lift)*.6*dt;
  this.r=U.lerp(this.r,gnd?0:rol*1.05,1-Math.exp(-dt*3));this.h+=gnd?rol*.7*dt*U.clamp(this.v/12,0,1):Math.sin(this.r)*1.15*dt*(.4+ctrl*.6);
  const vy=Math.sin(this.p)*this.v*(.3+.7*lift)-(1-lift)*(gnd?0:26),hv=Math.cos(this.p)*this.v;this.y+=vy*dt;const ox=this.x,oz=this.z;this.x+=Math.sin(this.h)*hv*dt;this.z+=Math.cos(this.h)*hv*dt;this.sp=this.v;
  this.col();let crash=null;if(this.y<=0){if(!gnd&&(vy<-13||Math.abs(this.r)>.6))crash='hard landing';this.y=0;if(this.p<0)this.p=0}
  if(!G.ghost){const b=this.bHit(G);if(b){if(this.y<=.05&&this.v<18){const nx=this.x,nz=this.z;this.x=ox;this.z=oz;this.col();const b0=this.bHit(G);if(b0){const cx=(b0.x0+b0.x1)/2,cz=(b0.z0+b0.z1)/2,dx=ox-cx,dz=oz-cz,d=Math.hypot(dx,dz)||1;this.x=nx+dx/d*7*dt;this.z=nz+dz/d*7*dt}else this.v=0;this.col()}else{const wi=!b.tw&&this.y>3&&this.v>=14?this.wingHit(G):null;if(wi&&Math.abs(wi.lx)>this.P.span*.3){this.x=ox;this.z=oz;this.sever(G,wi.lx)}else{crash='collision';this.hb=b}}}}
  if(this.mtHit(G.world.mt))crash='mountain collision';if(this.v>1&&G.hitObj(this)){if(this.y>1&&Math.abs(this.v)>14)crash='collision';this.x=ox;this.z=oz;this.v=0}this.x=U.clamp(this.x,-1250,1250);this.z=U.clamp(this.z,-1250,3250);if(this.prop)this.prop.rotation.z+=dt*(10+this.th*60);this.place();return crash}}
Object.assign(Plane.prototype,{
 wp(){this.g.updateMatrixWorld(true);const m=this.g.matrixWorld,v=new THREE.Vector3(),p=this.sk.pts,o=[],B=this.brk;for(let i=0;i<p.length;i+=3){if(B&&Math.sign(p[i])===B.side&&Math.abs(p[i])>B.cut)continue;v.set(p[i],p[i+1],p[i+2]).applyMatrix4(m);o.push(v.x,v.y,v.z)}return o},
 col(){this.place();this.W=this.wp()},
  wingMesh(){if(this.wm!==undefined)return this.wm;let best=null,bw=0;for(const o of this.g.children){if(!o.isMesh||!o.geometry)continue;o.geometry.computeBoundingBox();const bb=o.geometry.boundingBox,w=bb.max.x-bb.min.x;if(bb.min.x<-1&&bb.max.x>1&&w>bw){bw=w;best=o}}return this.wm=best},
  wingHit(G){const w=this.W,p=this.sk.pts;for(let i=0;i<w.length;i+=3){const x=w[i],y=w[i+1],z=w[i+2];for(const b of G.world.grid.at(x,z))if(b.h>.7&&x>b.x0&&x<b.x1&&z>b.z0&&z<b.z1&&y<b.h)return{b,lx:p[i]}}return null},
  sever(G,lx){const s=lx>0?1:-1,cut=Math.max(1.2,Math.abs(lx)-2.5),sn=Math.sin(this.h),cs=Math.cos(this.h),hv=Math.cos(this.p)*this.v,R=Math.random;this.brk={side:s,cut,t:0};
   const wm=this.wingMesh();let stump=new THREE.Vector3(s*cut,1,0);
   if(wm){const gm=wm.geometry;gm.computeBoundingBox();const bb=gm.boundingBox,tip=s>0?bb.max.x:-bb.min.x,xc=s*cut-wm.position.x,yc=(bb.min.y+bb.max.y)/2,zc=(bb.min.z+bb.max.z)/2,zs=(bb.max.z-bb.min.z)*.32,len=tip-cut;
    stump.set(s*cut,yc+wm.position.y,zc+wm.position.z);
    const mat=wm.material.clone();mat.side=THREE.DoubleSide;const sub=subdivGeo(gm,10),ph=R()*6.28,ph2=R()*6.28,
     c2=len>6?xc+s*len*(.45+R()*.1):null,
     fa=v=>s*(v[0]-xc)-jagX(v[2],v[1],ph),                       // >=0 : outboard of 1st break
     inner=clipGeo(sub,v=>-fa(v)),
     smat=new THREE.MeshStandardMaterial({color:0x6b7078,roughness:.5,metalness:.7}),
     spars=(par,x,dir)=>{for(let k=0;k<3;k++){const l=.8+R()*1.6,b=new THREE.Mesh(new THREE.BoxGeometry(l,.09+R()*.05,.09),smat);b.position.set(x+dir*l*.4,yc,zc+(k-1)*zs+(R()-.5)*.4);b.rotation.set((R()-.5)*.25,(R()-.5)*.3,(R()-.5)*.25);par.add(b)}
      for(let k=0;k<2;k++){const b=new THREE.Mesh(new THREE.BoxGeometry(.06,.5+R()*.4,zs*.9),smat);b.position.set(x+dir*(.3+R()*.5),yc,zc+(k?1:-1)*zs*.45);par.add(b)}};
    this.g.updateMatrixWorld(true);
    const mk=(geo,vx,vz,vy,fire,big)=>{const d=new THREE.Mesh(geo,mat);d.castShadow=true;wm.getWorldPosition(d.position);wm.getWorldQuaternion(d.quaternion);d.scale.copy(this.g.scale);G.scene.add(d);
     (G.pdeb||(G.pdeb=[])).push({m:d,vx,vy,vz,wx:(R()-.5)*5,wy:(R()-.5)*5,wz:s*(3+R()*4),t:0,fire,big});return d};
    const lat=()=>s*(4+R()*5),vx0=sn*hv*.75,vz0=cs*hv*.75;
    let out=clipGeo(sub,fa);
    if(c2!==null){const fb=v=>s*(v[0]-c2)-jagX(v[2],v[1],ph2),mid=clipGeo(out,v=>-fb(v)),tp=clipGeo(out,fb);
     const dm=mk(mid,vx0+cs*lat(),vz0-sn*lat(),3+R()*4,1,1);spars(dm,xc,-s);const dm2=mk(tp,vx0+cs*lat()*1.4,vz0-sn*lat()*1.4,4+R()*4,0,0)}
    else{const dm=mk(out,vx0+cs*lat(),vz0-sn*lat(),3+R()*4,1,1);spars(dm,xc,-s)}
    wm.geometry=inner;wm.material=mat;spars(wm,xc,s);
    // skin shards / panels
    for(let i=0;i<12;i++){const w=.4+R()*1.3,d=.3+R()*.9,sh=new THREE.Mesh(new THREE.BoxGeometry(w,.05,d),mat);sh.castShadow=true;const q=new THREE.Vector3(stump.x+(R()-.5)*2,stump.y,stump.z+(R()-.5)*3);this.g.localToWorld(q);sh.position.copy(q);G.scene.add(sh);
     (G.pdeb||(G.pdeb=[])).push({m:sh,vx:vx0*(.5+R()*.4)+(R()-.5)*14,vy:2+R()*7,vz:vz0*(.5+R()*.4)+(R()-.5)*14,wx:(R()-.5)*14,wy:(R()-.5)*14,wz:(R()-.5)*14,t:0,fire:R()<.25,big:0})}}
   B_(this,stump);
   this.bvx=sn*hv*.85;this.bvz=cs*hv*.85;this.bvy=Math.sin(this.p)*this.v*.5;this.v*=.85;this.r+=s*.35;this.hb=null;this.col();
   {const q=this.g.localToWorld(stump.clone());for(let i=0;i<34;i++)G.dfx.spawn(q.x+(R()-.5)*2,q.y+(R()-.3)*1.5,q.z+(R()-.5)*2,this.bvx,this.bvz,1.3,i<22?1:0,i<22?.9:1.6)}
   for(let i=0;i<12;i++)G.puff(this.x+(R()-.5)*6,this.y+this.gy+R()*2,this.z+(R()-.5)*6);
   G.sfx.shot&&G.sfx.shot(3);G.say('WING TORN OFF!',2200);G.toast('Lost control — press F to bail out!')},
  brokenStep(dt,G){const B=this.brk;B.t+=dt;const t=B.t,s=B.side;
   this.r+=s*Math.min(7,1.6+t*2.2)*dt;this.h+=s*Math.min(3.2,.9+t*.9)*dt;
   this.p=U.lerp(this.p,-.95,1-Math.exp(-dt*.7))+Math.sin(t*6)*.5*dt;
   const dr=Math.exp(-.12*dt);this.bvx*=dr;this.bvz*=dr;this.bvy=Math.max(-70,this.bvy-24*dt);
   this.x+=this.bvx*dt;this.z+=this.bvz*dt;this.y+=this.bvy*dt;this.v=Math.hypot(this.bvx,this.bvz);this.sp=this.v;this.th*=Math.exp(-dt);
   this.col();let crash=null;
   if(this.y<=0){this.y=0;crash='crashed after losing a wing'}
   if(!crash&&!G.ghost){const hb=this.bHit(G);if(hb){crash='collision';this.hb=hb}}
   if(!crash&&this.mtHit(G.world.mt))crash='mountain collision';
   if(G.dfx){for(let i=0;i<2;i++)G.dfx.spawn(this.x+(Math.random()-.5)*2.5,this.y+this.gy+.4,this.z+(Math.random()-.5)*2.5,this.bvx*.5,this.bvz*.5,1.7);
    if(B.sp&&t<12){const q=this.g.localToWorld(B.sp.clone());for(let i=0;i<3;i++)G.dfx.spawn(q.x+(Math.random()-.5),q.y+(Math.random()-.5),q.z+(Math.random()-.5),this.bvx,this.bvz,1.3,i<2?1:0,i<2?.9:1.5)}}
   if(this.prop)this.prop.rotation.z+=dt*8;
   this.x=U.clamp(this.x,-1250,1250);this.z=U.clamp(this.z,-1250,3250);this.place();return crash},
 cells(x,y0,y1,r,fn){const k=this.sk,s=this.g.scale.x,c=Math.cos(this.h),n=Math.sin(this.h),dx=x[0]-this.x,dz=x[1]-this.z,lx=(dx*c-dz*n)/s,lz=(dx*n+dz*c)/s,rr=r/s,ym=this.y+this.gy,a0=(y0-ym)/s,a1=(y1-ym)/s,open=(this.dra||0)>.5;
  const i0=Math.floor((lx-rr-k.x0)/k.c),i1=Math.floor((lx+rr-k.x0)/k.c),j0=Math.floor((lz-rr-k.z0)/k.c),j1=Math.floor((lz+rr-k.z0)/k.c);
  for(let j=j0;j<=j1;j++)for(let i=i0;i<=i1;i++){if(i<0||j<0||i>=k.nx||j>=k.nz)continue;const q=j*k.nx+i;if(!((k.mx[q]>=a0&&k.mn[q]<=a1)||(!open&&k.rmx[q]>=a0&&k.rmn[q]<=a1)))continue;fn(lx-(k.x0+(i+.5)*k.c),lz-(k.z0+(j+.5)*k.c),rr+k.c*.5,s,c,n)}},
 push(x,z,r,y0,y1){let ax=0,az=0,cnt=0,cc=1,nn=0,ss=1;this.cells([x,z],y0,y1,r,(ex,ez,m,s,c,n)=>{const d=Math.hypot(ex,ez);if(d<m){const f=d>1e-4?(m-d)/d:0;ax+=ex*f;az+=ez*f;cnt++;cc=c;nn=n;ss=s}});if(!cnt)return null;ax=ax/cnt*ss;az=az/cnt*ss;return[ax*cc+az*nn,-ax*nn+az*cc]},
 hits(x,y,z,r){let h=false;this.cells([x,z],y-r,y+r,r,(ex,ez,m)=>{if(Math.hypot(ex,ez)<m)h=true});return h},
 bHit(G,fn){const w=this.W;for(let i=0;i<w.length;i+=3){const x=w[i],y=w[i+1],z=w[i+2];for(const b of G.world.grid.at(x,z))if(b.h>.7&&x>b.x0&&x<b.x1&&z>b.z0&&z<b.z1&&y<b.h&&(!fn||fn(b,y)))return b}return null},
 mtHit(mt){const w=this.W||(this.W=this.wp()),R=this.P.span*1.6+10;for(const m of mt){if(Math.abs(this.x-m[0])>m[2]+R||Math.abs(this.z-m[1])>m[2]+R)continue;for(let i=0;i<w.length;i+=3)if(mtIn(m,w[i],w[i+2],w[i+1]-.4))return true}return false}});
class Heli{constructor(sc){const M=(c,m=.5)=>new THREE.MeshStandardMaterial({color:c,roughness:.4,metalness:m}),g=this.g=new THREE.Group(),P=(geo,mt,x,y,z,p=g)=>{const o=new THREE.Mesh(geo,mt);o.position.set(x,y,z);o.castShadow=true;p.add(o);return o},bm=M(0x1c2a48);
 P(new THREE.SphereGeometry(1.4,14,10).scale(.9,.85,1.7),bm,0,0,0);P(new THREE.CylinderGeometry(.18,.5,5,8).rotateX(Math.PI/2),bm,0,.3,-3.2);P(new THREE.BoxGeometry(.12,1.3,.7),bm,0,.9,-5.5);P(new THREE.SphereGeometry(.95,12,8).scale(.95,.75,1),M(0x6fb4d8,.9),0,.35,1.2);P(new THREE.BoxGeometry(.2,.4,.2),bm,0,1.5,0);
 P(new THREE.CylinderGeometry(.06,.06,3,6).rotateX(Math.PI/2),bm,.9,-1.25,.2);P(new THREE.CylinderGeometry(.06,.06,3,6).rotateX(Math.PI/2),bm,-.9,-1.25,.2);
 const r=this.rot=new THREE.Group();r.position.y=1.7;g.add(r);P(new THREE.BoxGeometry(.3,.05,8.5),M(0x111111),0,0,0,r);P(new THREE.BoxGeometry(8.5,.05,.3),M(0x111111),0,0,0,r);
 this.tr=new THREE.Group();this.tr.position.set(.2,.9,-5.5);g.add(this.tr);P(new THREE.BoxGeometry(.05,1.6,.15),M(0x111111),0,0,0,this.tr);
 this.bc=P(new THREE.SphereGeometry(.25,8,6),new THREE.MeshBasicMaterial({color:0xff0000,fog:false}),0,-1.2,0);sc.add(g);this.x=this.z=0;this.y=26;this.a=0;this.cd=1}}
class Hover{constructor(sc,x,z,col,tv){const M=(c,e,m,r)=>new THREE.MeshStandardMaterial({color:c,emissive:e||0,emissiveIntensity:.7,metalness:m==null?.7:m,roughness:r==null?.28:r}),g=this.g=new THREE.Group();
 if(tv){const vb=new THREE.Group();vb.position.y=-.15;g.add(vb);
  vb.add(new THREE.Mesh(tv.body,new THREE.MeshStandardMaterial({vertexColors:true,metalness:.6,roughness:.32,emissive:0x0b1520,color:col})));
  vb.add(new THREE.Mesh(tv.glow,new THREE.MeshBasicMaterial({color:0x36f1ff,transparent:true,opacity:.24,blending:THREE.AdditiveBlending,depthWrite:false,fog:false})));
  vb.add(new THREE.Mesh(tv.tail,new THREE.MeshBasicMaterial({color:0xff3d6e,fog:false})));
  vb.add(new THREE.Mesh(tv.head,new THREE.MeshBasicMaterial({color:0xfff1cc,fog:false})));
 }else{
 const bd=new THREE.Mesh(new THREE.BoxGeometry(2.1,.5,4.4),M(col,0x0a1a2a));bd.position.y=.62;g.add(bd);
 const ns=new THREE.Mesh(new THREE.BoxGeometry(1.5,.32,1.2),M(col,0x0a1a2a));ns.position.set(0,.55,-2.4);g.add(ns);
 const cp=new THREE.Mesh(new THREE.BoxGeometry(1.45,.5,1.9),new THREE.MeshStandardMaterial({color:0x061826,emissive:0x1a86b8,emissiveIntensity:.8,metalness:.9,roughness:.12}));cp.position.set(0,1.02,.1);g.add(cp);
 for(const s of[1,-1]){const f=new THREE.Mesh(new THREE.BoxGeometry(.5,.14,1.5),M(0x1a2433));f.position.set(s*1.18,.58,1.4);g.add(f);
  const n=new THREE.Mesh(new THREE.CylinderGeometry(.26,.32,.5,10).rotateX(Math.PI/2),M(0x101820));n.position.set(s*1.02,.5,1.15);g.add(n);
  const ring=new THREE.Mesh(new THREE.TorusGeometry(.33,.06,6,18).rotateX(Math.PI/2),new THREE.MeshBasicMaterial({color:0x36f1ff,fog:false}));ring.position.set(s*1.02,.25,1.15);g.add(ring);
  const fl=new THREE.Mesh(new THREE.ConeGeometry(.2,.8,8).rotateX(Math.PI),new THREE.MeshBasicMaterial({color:0x36f1ff,transparent:true,opacity:.75,blending:THREE.AdditiveBlending,depthWrite:false,fog:false}));fl.position.set(s*1.02,.04,1.15);g.add(fl);
  const hl=new THREE.Mesh(new THREE.BoxGeometry(.4,.1,.12),new THREE.MeshBasicMaterial({color:0xffeebb,fog:false}));hl.position.set(s*.62,.58,-2.85);g.add(hl)}
 const ug=new THREE.Mesh(new THREE.PlaneGeometry(2.8,4.8).rotateX(-Math.PI/2),new THREE.MeshBasicMaterial({color:0x36f1ff,transparent:true,opacity:.3,blending:THREE.AdditiveBlending,depthWrite:false,fog:false}));ug.position.y=.1;g.add(ug)}
 sc.add(g);this.P={name:'Nova Hover',hover:1,span:2.6,vm:34};this.gy=1.05;this.camd=8.5;this.flp=tv?0:Math.PI;this.hx=x;this.hz=z;this.alive=true;this.dead=0;this.reset()}
 reset(){this.x=this.hx;this.z=this.hz;this.h=0;this.y=0;this.v=0;this.vy=0;this.th=0;this.sp=0;this.gl=0;this.alive=true;this.dead=0;this.g.visible=true;this.place()}
 place(){this.g.position.set(this.x,this.y+this.gy,this.z);this.g.rotation.set(0,this.h+this.flp,0)}
 fly(dt,k,G){const up=(k.ShiftLeft?1:0)-(k.Space?1:0),fw=(k.KeyW?1:0)-(k.KeyS?1:0),tr=(k.KeyA?1:0)-(k.KeyD?1:0);
  let gl=0;for(const b of G.world.grid.at(this.x,this.z))if(this.x>b.x0-1&&this.x<b.x1+1&&this.z>b.z0-1&&this.z<b.z1+1&&this.y>=b.h-.4)gl=Math.max(gl,b.h);this.gl=gl;
  const vt=up>0?9:up<0?-9:U.clamp((gl+1.4-this.y)*1.1,-7,7);this.vy=U.lerp(this.vy,vt,1-Math.exp(-dt*4));
  this.v=U.lerp(this.v,fw>0?34:fw<0?-14:0,1-Math.exp(-dt*1.7));this.h+=tr*1.25*dt;
  const ox=this.x,oz=this.z;this.x+=Math.sin(this.h)*this.v*dt;this.z+=Math.cos(this.h)*this.v*dt;this.y+=this.vy*dt;
  let hit=false;for(const b of G.world.grid.at(this.x,this.z))if(this.x>b.x0-.8&&this.x<b.x1+.8&&this.z>b.z0-.8&&this.z<b.z1+.8&&this.y<b.h-.25){hit=true;break}
  if(hit){this.x=ox;this.z=oz;this.v*=-.15}
  if(this.y<gl){this.y=gl;this.vy=Math.max(0,this.vy)}
  this.y=Math.min(this.y,320);this.x=U.clamp(this.x,30000-1450,30000+1450);this.z=U.clamp(this.z,-1450,1450);
  this.th=Math.max(up>0?1:0,Math.min(1,Math.abs(this.v)/20));this.sp=Math.abs(this.v);this.place();return null}}
/* ===== CAMERA ===== */
class Rig{constructor(cam){this.c=cam;this.yaw=0;this.pit=.25;this.idle=0;this.p=new THREE.Vector3();this.t=new THREE.Vector3();this.init=false}
 update(dt,G){const inp=G.inp,w=G.world,car=G.driving||G.flying,pl=G.player;
  if(inp.dx||inp.dy){const sn=G.sens*this.c.fov/70*.0025;this.yaw-=inp.dx*sn;this.pit=U.clamp(this.pit+inp.dy*sn,-.44,1.05);this.idle=0;inp.dx=inp.dy=0}else this.idle+=dt;
  if(G.lau&&!G.lau.walk){G.lauCam(dt);return}let d,fy,fx=pl.x,fz=pl.z;
  if(car){fx=car.x;fz=car.z;fy=1.4+(car.y||0)+(car.gy||0);d=car.camd||C.cam.cd;if(this.idle>C.cam.idle||car.fl){const k=1-Math.exp(-2*dt);this.yaw=U.lerpA(this.yaw,car.h,k);this.pit=U.lerp(this.pit,Math.atan2(C.cam.ch,d),k)}}
  else{fy=pl.y+C.cam.fh*.8;d=G.sit?34:C.cam.fd}
  const cp=Math.cos(this.pit),ox=-Math.sin(this.yaw)*cp*d,oy=Math.sin(this.pit)*d,oz=-Math.cos(this.yaw)*cp*d;let k=1;
  for(let i=1;i<=8&&k===1;i++){const t=i/8,x=fx+ox*t,z=fz+oz*t,y=fy+oy*t;for(const b of w.grid.at(x,z))if(!G.ghost&&x>b.x0-.3&&x<b.x1+.3&&z>b.z0-.3&&z<b.z1+.3&&y<b.h){k=Math.max(.12,(i-1)/8);break}}
  const tx=fx+ox*k,ty=Math.max(.5,fy+oy*k),tz=fz+oz*k;
  if(!this.init){this.p.set(tx,ty,tz);this.t.set(fx,fy,fz);this.init=true}else{this.p.lerp(new THREE.Vector3(tx,ty,tz),1-Math.exp(-dt*8));this.t.lerp(new THREE.Vector3(fx,fy,fz),1-Math.exp(-dt*14))}
  if(G.fp&&!car){const hx=pl.x+Math.sin(this.yaw)*.3,hy=pl.y+1.95,hz=pl.z+Math.cos(this.yaw)*.3,cp2=Math.cos(this.pit);this.p.set(hx,hy,hz);this.t.set(hx+Math.sin(this.yaw)*cp2,hy-Math.sin(this.pit),hz+Math.cos(this.yaw)*cp2)}
  this.c.position.copy(this.p);this.c.lookAt(this.t);
  let f=car?C.cam.fov+(C.cam.fovMax-C.cam.fov)*Math.min(1,Math.abs(car.sp)/C.car.max):C.cam.fov;if(car&&car.nb)f+=car.type==='motorcycle'?16:12;if(G.aiming)f=G.scopeFov;
  if(Math.abs(this.c.fov-f)>.05){this.c.fov=U.lerp(this.c.fov,f,1-Math.exp(-dt*4));this.c.updateProjectionMatrix()}}}
/* ===== GAME ===== */
class GameCls{
 constructor(){
  this.state='MENU';this.money=5000;this.health=100;this.armor=0;this.wanted=0;this.c4=[];this.policeSpawned=0;this.tankSpawned=false;this.weaponName='Fist';this.weaponCooldown=0;this.shopOpen=false;this.ammo=60;this.dead=0;this.fee=0;this.bust=0;this.evade=0;this.bigT=0;this.hitT=0;this.radio=0;this.tt=0;this.pn=0;this.kin={k:NOKEY};this.mapOpen=false;this.wp=null;this.owned=new Set([0]);this.skinI=0;this.am={Pistol:48};this.own=new Set(['Pistol']);this.weaponName='Pistol';this.fireT=0;this.flash=0;this.driving=null;this.near=null;this.acc=0;this.last=performance.now();this.loc='';this.fc=0;this.ft=0;this.showFps=false;this.toastT=0;this.hadLock=false;this.jetOwn=false;
  const cv=$('gl'),r=this.r=new THREE.WebGLRenderer({canvas:cv,antialias:true,powerPreference:'high-performance'});this.rs=1;this.fr=0;r.setPixelRatio(Math.min(devicePixelRatio,1.5));r.toneMapping=THREE.ACESFilmicToneMapping;r.toneMappingExposure=1.22;r.shadowMap.autoUpdate=false;r.shadowMap.needsUpdate=true;r.shadowMap.enabled=true;r.shadowMap.type=THREE.PCFSoftShadowMap;
  const scene=this.scene=new THREE.Scene(),cam=this.cam=new THREE.PerspectiveCamera(C.cam.fov,1,.5,1300);
  this.inp=new Input();this.sfx=new Sfx();this.world=new World(scene);this.player=new Player(scene);this.rig=new Rig(cam);this.traffic=new Traffic(this.world);
  const R=this.world.R,L=this.world.L,hw=this.world.hw,cols=[0xc0392b,0x2c7be5,0xe8c547,0x2ecc71,0xecf0f1,0x8e44ad,0xe67e22,0x16a085];
  this.cars=[];const near=c=>{const i=U.clamp(Math.round((c+600)/C.step),0,10);return Math.abs(c-L[i])<hw(i)+8};
  const first=new Car(scene,0xff3d8b,null,'Sedan');first.x=20;first.z=6.4;first.h=Math.PI/2;this.cars.push(first);[0xe74c3c,0x2c7be5,0xf1c40f].forEach((cl,n)=>{const b=new Car(scene,cl,'motorcycle');b.x=30+n*4;b.z=8;b.h=Math.PI/2;this.cars.push(b)});
  for(let n=1;n<C.npc.parked;n++){const c=new Car(scene,cols[Math.floor(R()*8)],null,NPCM[Math.floor(Math.random()*NPCM.length)]),i=Math.floor(R()*11),side=R()<.5?1:-1;let p=-560+R()*1120;while(near(p))p=-560+R()*1120;
   if(R()<.5){c.x=L[i]+(hw(i)-1.6)*side;c.z=p;c.h=side>0?Math.PI:0}else{c.z=L[i]+(hw(i)-1.6)*side;c.x=p;c.h=side>0?Math.PI/2:-Math.PI/2}this.cars.push(c)}
  {const mk=['Scooter','Naked','Chopper','Dirt','Cafe','Ducati','Vario'];for(let n=0;n<14;n++){const k=mk[n%7],c=new Car(scene,MOTOS[k].c,'motorcycle',k);let t=0;do{this.traffic.place(c,this.traffic.ri(),this.traffic.ri())}while(Math.hypot(c.x,c.z)<100&&t++<20);c.rmat[0].color.setHSL(R(),.55,.45);c.rmat[1].color.setHSL(R(),.3,.2);c.rider.visible=true;c.rs=1;this.cars.push(c)}}
   for(let n=0;n<C.npc.n;n++){const c=new Car(scene,cols[Math.floor(R()*8)],null,NPCM[Math.floor(Math.random()*NPCM.length)]);let t=0;do{this.traffic.place(c,this.traffic.ri(),this.traffic.ri())}while(Math.hypot(c.x,c.z)<100&&t++<20);this.cars.push(c)}
  // tire smoke
  this.sg=new THREE.BufferGeometry();this.sp=new Float32Array(60*3).fill(-100);this.sl=new Float32Array(60);this.sg.setAttribute('position',new THREE.BufferAttribute(this.sp,3));this.si=0;
  const pts=new THREE.Points(this.sg,new THREE.PointsMaterial({color:0xcccccc,size:2.2,transparent:true,opacity:.45,depthWrite:false}));pts.frustumCulled=false;scene.add(pts);this.dp=new Float32Array(120*3).fill(-100);this.dl=new Float32Array(120);this.di=0;{const dg=new THREE.BufferGeometry();dg.setAttribute('position',new THREE.BufferAttribute(this.dp,3));this.dg=dg;const dpts=new THREE.Points(dg,new THREE.PointsMaterial({color:0xb9a37a,size:1,transparent:true,opacity:.55,depthWrite:false}));dpts.frustumCulled=false;scene.add(dpts)}
  this.dfx=new DriftFX(scene);this.mg=$('mini').getContext('2d');this.peds=new Peds(this.world,scene);
  this.mk=new THREE.Mesh(new THREE.CylinderGeometry(5,5,60,20,1,true),new THREE.MeshBasicMaterial({color:0xff2a2a,transparent:true,opacity:.35,side:THREE.DoubleSide,depthWrite:false,blending:THREE.AdditiveBlending,fog:false}));scene.add(this.mk);this.nextMission();this.peds.update(0,20,10,0);SHOPS.push({...SHOPDEF.air,id:'air',w:14,d:10,x:70,z:-722,mz:-723.5});this.initSpace();this.lau=null;this.abn=[];this.sky=null;this.buildShops();this.buildSkins();this.planes=[];
  this.fx=[];this.nit=100;this.over=false;this.ch=null;this.msls=[];this.flying=null;this.nearAir=null;this.punchT=0;this.pf=0;this.tl0=-1;this.tl1=-1;this.fl=[0,1].map(()=>{const m=new THREE.Mesh(new THREE.ConeGeometry(.25,2,8).rotateX(-Math.PI/2),new THREE.MeshBasicMaterial({color:0x66b0ff,transparent:true,opacity:.85,blending:THREE.AdditiveBlending,depthWrite:false,fog:false}));m.visible=false;scene.add(m);return m});this.bl=new THREE.PointLight(0xff8830,0,70);scene.add(this.bl);this.polT=0;this.mag={Pistol:12};this.att={};this.attOwn=new Set();this.rl=0;this.rlT=1;this.rlW='';this.god=false;this.rich=false;this.heli=null;this.aiming=false;this.sens=1;this.cb='';this.scopeFov=50;this.editing=false;this.binding=null;
  this.player.magM=new THREE.Mesh(new THREE.BoxGeometry(.06,.16,.08),new THREE.MeshStandardMaterial({color:0x111111}));this.player.magM.visible=false;this.player.g.add(this.player.magM);
  this.trs=[];const tg=new THREE.BoxGeometry(.05,.05,1),tm=new THREE.MeshBasicMaterial({color:0xffe08a,fog:false});for(let i=0;i<24;i++){const m=new THREE.Mesh(tg,tm);m.visible=false;m.life=0;scene.add(m);this.trs.push(m)}
  this.hl=[0,1].map(()=>{const l=new THREE.SpotLight(0xfff2d0,0,80,.55,.6,1);scene.add(l,l.target);return l});
  addEventListener('mousedown',e=>{if(e.button===0&&this.inp.locked&&this.state==='PLAYING'&&(!this.driving||this.driving.mytank))this.shoot()});{const cv=$('mapc'),G=this,P=new Map();let dr=0;cv.style.touchAction='none';this.mz={z:1,x:0,y:0};
 cv.addEventListener('wheel',e=>{e.preventDefault();const m=G.mapXY(e);G.mapZoom(e.deltaY<0?1.3:1/1.3,m.px,m.py)},{passive:false});
 cv.addEventListener('pointerdown',e=>{cv.setPointerCapture(e.pointerId);P.set(e.pointerId,[e.clientX,e.clientY]);if(P.size===1)dr=0});
 cv.addEventListener('pointermove',e=>{const o=P.get(e.pointerId);if(!o)return;const Z=G.mz,sx=cv.width/cv.getBoundingClientRect().width;
  if(P.size===2){const a=[...P.values()],d0=Math.hypot(a[0][0]-a[1][0],a[0][1]-a[1][1]);P.set(e.pointerId,[e.clientX,e.clientY]);const b=[...P.values()],d1=Math.hypot(b[0][0]-b[1][0],b[0][1]-b[1][1]);if(d0>0){const c=G.mapXY({clientX:(b[0][0]+b[1][0])/2,clientY:(b[0][1]+b[1][1])/2});G.mapZoom(d1/d0,c.px,c.py)}dr=99;return}
  const dx=e.clientX-o[0],dy=e.clientY-o[1];dr+=Math.abs(dx)+Math.abs(dy);if(dr>6){Z.x-=dx*sx/Z.z;Z.y-=dy*sx/Z.z;G.mapClamp();G.drawMap()}P.set(e.pointerId,[e.clientX,e.clientY])});
 cv.addEventListener('pointerup',e=>{const had=P.delete(e.pointerId);if(had&&dr<=6&&!P.size){const m=G.mapXY(e);G.wp={x:m.x,z:m.z};G.toast('Waypoint set');G.drawMap()}});
 cv.addEventListener('pointercancel',e=>P.delete(e.pointerId));
 const zb=(id,f)=>$(id).addEventListener('click',()=>{const W=cv.width/2,H=cv.height/2;if(f)G.mapZoom(f,W,H);else{G.mz={z:1,x:0,y:0};G.drawMap()}});zb('mzp',1.5);zb('mzm',1/1.5);zb('mzr',0)}
  addEventListener('resize',()=>this.resize());this.resize();this.mkRev();this.applyGfx();this.applyLang();this.renderMob();this.showMob();
  {let t=null;cv.addEventListener('pointerdown',e=>{if(e.pointerType==='touch')t={id:e.pointerId,x:e.clientX,y:e.clientY}});cv.addEventListener('pointermove',e=>{if(t&&e.pointerId===t.id&&this.state==='PLAYING'){this.inp.dx+=(e.clientX-t.x)*1.4;this.inp.dy+=(e.clientY-t.y)*1.4;t.x=e.clientX;t.y=e.clientY}});addEventListener('pointerup',e=>{if(t&&e.pointerId===t.id)t=null})}
  $('bStart').onclick=()=>this.resume();cv.addEventListener('click',()=>{if(this.state==='PLAYING'&&S.mode==='pc'&&!this.shopOpen&&!this.mapOpen&&!document.pointerLockElement)this.relock()});$('bSet').onclick=()=>this.openSet();
  document.addEventListener('pointerlockchange',()=>{const l=document.pointerLockElement===cv;this.inp.locked=l;if(l)this.hadLock=true;else if(this.state==='PLAYING'&&this.hadLock&&!this.shopOpen&&!this.mapOpen)this.pause();if(!l)this.hadLock=false});
  $('shop').querySelectorAll('button').forEach(b=>b.addEventListener('click',()=>this.buyItem(b.dataset.item)));
  this.cv=cv;requestAnimationFrame(t=>this.loop(t));setTimeout(()=>{try{if(!this.xin)this.xi()}catch(e){console.error('preload',e)}try{this.r.compile(this.scene,this.cam)}catch(e){}},60)}
 resize(){const w=innerWidth,h=innerHeight;this.r.setSize(w,h,false);this.cam.aspect=w/h;this.cam.updateProjectionMatrix()}
 resume(){this.state='PLAYING';$('screen').style.display='none';this.sfx.init();this.applyGfx();this.showMob();this.last=performance.now();try{if(S.mode!=='pc')throw 0;const p=this.cv.requestPointerLock();if(p&&p.catch)p.catch(()=>{})}catch(e){}}
 pause(){if(this.state!=='PLAYING')return;this.state='PAUSED';this.inp.k={};$('sub').textContent=tr('Paused');$('bStart').textContent=tr('Resume GTA_elfo');$('screen').style.display='flex';this.showMob()}
 onKey(c){if(c==='Escape'&&this.state==='PLAYING'&&(this.mapOpen||this.shopOpen)){if(this.mapOpen)this.toggleMap();else this.closeShop();return}if(c==='F3'){this.showFps=!this.showFps;$('fps').style.display=this.showFps?'block':'none'}
  else if(c==='Escape'||c==='KeyP'){if(this.state==='PLAYING')this.pause();else if(this.state==='PAUSED'&&c==='KeyP')this.resume()}
  else if(c==='KeyE'&&this.state==='PLAYING')this.xe();    else if(c==='KeyF'&&this.state==='PLAYING')this.spaceF()||this.toggleCar();
   else if(c==='KeyB'&&this.state==='PLAYING')this.toggleShop();else if(c==='KeyL'&&this.state==='PLAYING'&&this.sit&&!this.lau)this.startLaunch();else if(c==='KeyL'&&this.state==='PLAYING'&&this.lau&&this.lau.nova&&this.lau.ph==='landed')this.novaHome();else if(c==='KeyT'&&this.state==='PLAYING')this.warp();else if(c==='KeyG'&&this.state==='PLAYING')this.autoLand();
   else if(c==='KeyJ'&&this.state==='PLAYING')this.shoot();
   else if(c==='KeyK'&&this.state==='PLAYING')this.punch();
   else if(c==='KeyX'&&this.state==='PLAYING'){if(this.c4.length)this.detonateC4();else this.placeC4();}
   else if(c==='KeyQ'&&this.state==='PLAYING'){const l=this.list();this.weaponName=l[(l.indexOf(this.weaponName)+1)%l.length];this.toast(this.weaponName)}
   else if(/^Digit[0-9]$/.test(c)&&this.state==='PLAYING')this.equip(+c.slice(5));
   else if(c==='KeyM'&&this.state==='PLAYING'&&!this.shopOpen)this.toggleMap();
   else if(c==='KeyR'&&this.state==='PLAYING'&&this.driving){this.radio=(this.radio+1)%RADIO.length;this.sfx.radio(this.radio);this.toast(this.radio?'♪ '+RADIO[this.radio].name:'Radio off')}
   else if(c==='KeyR'&&this.state==='PLAYING')this.reload();else if(c==='KeyV'&&this.state==='PLAYING'&&this.driving&&this.driving.air&&this.driving.y<=0){this.driving.vy=6.5;this.sfx.beep(200)}else if(c==='KeyH'&&this.state==='PLAYING')this.sfx.beep(240);else if(this.state==='PLAYING')this.xtra(c)}
 xtra(c){const l=this.list();
 if(c==='KeyC'){this.weaponName=l[(l.indexOf(this.weaponName)+l.length-1)%l.length];this.toast(this.weaponName)}
 else if(c==='KeyN'&&this.driving){this.radio=(this.radio+RADIO.length-1)%RADIO.length;this.sfx.radio(this.radio);this.toast(this.radio?'♪ '+RADIO[this.radio].name:'Radio off')}
 else if(c==='KeyU'){const d=document,e=d.documentElement;if(d.fullscreenElement)d.exitFullscreen();else(e.requestFullscreen||e.webkitRequestFullscreen).call(e)}
 else if(c==='KeyI'){S.q={low:'med',med:'high',high:'ultra',ultra:'insane',insane:'low'}[S.q]||'high';sv('gtaelfo_s',S);this.applyGfx();this.toast('Graphics: '+S.q.toUpperCase())}
 else if(c==='KeyO')this._shot=1;
 else if(c==='KeyY'){this._mute=!this._mute;if(this.sfx.mg)this.sfx.mg.gain.value=this._mute?0:S.vol;this.toast(this._mute?'Sound off':'Sound on')}
 else if(c==='BracketLeft'||c==='BracketRight'){S.fov=U.clamp(S.fov+(c==='BracketRight'?5:-5),50,110);sv('gtaelfo_s',S);this.applyGfx();this.toast('FOV '+S.fov)}}
  relock(){try{const p=this.cv.requestPointerLock();if(p&&p.catch)p.catch(()=>{})}catch(e){}}
  closeShop(){this.shopOpen=false;$('shop').style.display=$('skin').style.display='none';this.relock()}
  toggleShop(){if(this.shopOpen){this.closeShop();return}if(this.mapOpen)return;const s=this.nearShop;if(!s){this.toast('Walk into a shop marker (map: M)');return}
   this.shopOpen=s.id;this.buildShop(s.id);document.exitPointerLock()}
  toggleMap(){this.mapOpen=!this.mapOpen;$('mapv').style.display=this.mapOpen?'flex':'none';if(this.mapOpen){document.exitPointerLock();this.mz={z:1,x:0,y:0};this.drawMap()}else this.relock()}
  drawMap(){const cv=$('mapc'),n=Math.floor(Math.min(innerWidth,innerHeight)*.86),mw=Math.round(n*.64);if(cv.width!==mw||cv.height!==n){cv.width=mw;cv.height=n}const g=cv.getContext('2d'),k=n/5000,P=v=>(v+1600)*k,Z=this.mz||(this.mz={z:1,x:0,y:0});g.setTransform(1,0,0,1,0,0);g.clearRect(0,0,mw,n);g.save();g.translate(mw/2,n/2);g.scale(Z.z,Z.z);g.translate(-mw/2-Z.x,-n/2-Z.y);g.drawImage(this.world.mm,0,0,mw,n);
   const tz=Math.pow(Z.z,-1.2),iz=1/Z.z,fs=Math.max(8,(n/46|0))*tz;g.lineJoin='round';g.textAlign='center';g.textBaseline='alphabetic';g.font='bold '+fs+'px Rajdhani,sans-serif';g.lineWidth=3*iz;g.strokeStyle='rgba(0,0,0,.65)';g.fillStyle='rgba(225,232,245,.85)';for(const l of MAPLBL){g.strokeText(l[0],P(l[1]),P(l[2]));g.fillText(l[0],P(l[1]),P(l[2]))}g.font=Math.max(14,n/30|0)*iz+'px sans-serif';g.fillText('\u2708',P(0),P(-600));g.font='bold '+Math.max(8,(n/58|0))*tz+'px Rajdhani,sans-serif';
   const dot=(wx,wz,col,r,t)=>{r*=iz*(.55+.45*Math.pow(Z.z,.15));g.fillStyle=col;g.beginPath();g.arc(P(wx),P(wz),r,0,7);g.fill();if(t){g.lineWidth=3*iz;g.strokeStyle='rgba(0,0,0,.75)';g.strokeText(t,P(wx),P(wz)-r-4*iz);g.fillStyle='#fff';g.fillText(t,P(wx),P(wz)-r-4*iz)}};
   for(const o of this.cars)if(o.type==='police'||o.type==='tank')dot(o.x,o.z,'#4da3ff',3);
   for(const q of SHOPS)dot(q.x,q.mz,q.css,6,q.name);for(const o of POI)dot(o.x,o.z,o.c,6,o.t);dot(0,-641,'#ffffff',7,'AIRPORT');dot(this.mis.x,this.mis.z,'#ff3030',7,'MISSION');if(this.wp)dot(this.wp.x,this.wp.z,'#ff4bd8',6,'WAYPOINT');
   const f=this.driving||this.player,h=this.driving?this.driving.h:this.player.face;g.save();g.translate(P(f.x),P(f.z));g.rotate(Math.PI-h);g.scale(iz*(.6+.4*Math.pow(Z.z,.15)),iz*(.6+.4*Math.pow(Z.z,.15)));g.fillStyle='#36f1ff';g.strokeStyle='#000';g.beginPath();g.moveTo(0,-9);g.lineTo(-6,7);g.lineTo(6,7);g.closePath();g.fill();g.stroke();g.restore();g.restore()}
  mapXY(e){const cv=$('mapc'),r=cv.getBoundingClientRect(),Z=this.mz,px=(e.clientX-r.left)/r.width*cv.width,py=(e.clientY-r.top)/r.height*cv.height,u=(px-cv.width/2)/Z.z+cv.width/2+Z.x,v=(py-cv.height/2)/Z.z+cv.height/2+Z.y;return{x:u/cv.width*3200-1600,z:v/cv.height*5000-1600,px,py}}
  mapClamp(){const cv=$('mapc'),Z=this.mz,a=cv.width/2*(1-1/Z.z),b=cv.height/2*(1-1/Z.z);Z.x=U.clamp(Z.x,-a,a);Z.y=U.clamp(Z.y,-b,b)}
  mapZoom(f,px,py){const cv=$('mapc'),Z=this.mz,W=cv.width,H=cv.height,u=(px-W/2)/Z.z+W/2+Z.x,v=(py-H/2)/Z.z+H/2+Z.y;Z.z=U.clamp(Z.z*f,1,14);Z.x=u-(px-W/2)/Z.z-W/2;Z.y=v-(py-H/2)/Z.z-H/2;this.mapClamp();this.drawMap()}
  buildShops(){const w=this.world,M=(c,r=.8)=>new THREE.MeshStandardMaterial({color:c,roughness:r});
   const add=(o,x,y,z)=>{o.position.set(x,y,z);o.castShadow=o.receiveShadow=true;this.scene.add(o);return o},bx=(a,b,c,m,x,y,z)=>add(new THREE.Mesh(new THREE.BoxGeometry(a,b,c),m),x,y,z),
    solid=(x0,x1,z0,z1)=>{const q={x0,x1,z0,z1,h:5};w.boxes.push(q);w.grid.add(q)},
    man=(sh,pn,sk,x,z,ry)=>{const g=new THREE.Group(),p=(a,b,c,m,px,py)=>{const o=new THREE.Mesh(new THREE.BoxGeometry(a,b,c),m);o.position.set(px,py,0);o.castShadow=true;g.add(o)};
     p(.6,.7,.35,M(sh),0,1.35);p(.4,.4,.4,M(sk),0,1.95);p(.25,1,.25,M(pn),.15,.5);p(.25,1,.25,M(pn),-.15,.5);p(.2,.7,.2,M(sh),.4,1.3);p(.2,.7,.2,M(sh),-.4,1.3);g.position.set(x,0,z);g.rotation.y=ry;this.scene.add(g)};
   for(const s of SHOPS){const x=s.x,z=s.z,hw=s.w/2,z0=z-s.d/2,z1=z+s.d/2,wm=M(s.col);
    bx(s.w,.1,s.d,M(0x2b2d33,.9),x,.06,z);bx(s.w,.4,s.d,wm,x,5.2,z);bx(s.w,5,.4,wm,x,2.5,z1-.2);bx(.4,5,s.d,wm,x-hw+.2,2.5,z);bx(.4,5,s.d,wm,x+hw-.2,2.5,z);
    solid(x-hw,x+hw,z1-.4,z1);solid(x-hw,x-hw+.4,z0,z1);solid(x+hw-.4,x+hw,z0,z1);
    const t=w.tex(256,64,(g,W,H)=>{g.fillStyle='#0b1022';g.fillRect(0,0,W,H);g.strokeStyle=s.css;g.lineWidth=4;g.strokeRect(3,3,W-6,H-6);g.fillStyle=s.css;g.font='bold 30px sans-serif';g.textAlign='center';g.fillText(s.name,W/2,43)});
    const sg=new THREE.Mesh(new THREE.PlaneGeometry(s.w-1,2.2),new THREE.MeshBasicMaterial({map:t}));sg.position.set(x,6.5,z0-.05);sg.rotation.y=Math.PI;this.scene.add(sg);
    
    if(s.id==='gun'||s.id==='att'){bx(8,1.1,1.1,M(0x4a3a2a),x,.6,z1-3);solid(x-4,x+4,z1-3.55,z1-2.45);bx(10,2.6,.1,M(0x1a1c22),x,2.7,z1-.5);
     for(let i=0;i<6;i++)bx(1.3,.14,.12,M(i%2?0x3a3a42:0x22242a),x-4.2+i*1.68,3.4-(i%2)*.9,z1-.62);man(0x8a2b2b,0x222222,0xc68c62,x,z1-1.8,Math.PI)}
    else if(s.id==='skin'){for(let i=0;i<8;i++)bx(.5,1.2,.15,M(SKINS[i].sh),x-5+i*1.4,3,z1-.6);man(SKINS[3].sh,SKINS[3].pn,0xe0b090,x-4,z1-2,Math.PI);man(SKINS[6].sh,SKINS[6].pn,0xc68c62,x,z1-2,Math.PI);man(SKINS[7].sh,SKINS[7].pn,0x8d5a3b,x+4,z1-2,Math.PI)}
    else if(s.id==='arena'){man(0xff7a3d,0x222222,0xc68c62,x-3,z1-2,Math.PI);man(0xc0392b,0x222222,0x8d5a3b,x+3,z1-2,Math.PI)}
    else{const mo=s.id==='moto',d=new Car(this.scene,mo?0xd10000:0xf2c200,mo?'motorcycle':null,mo?'Ducati':'Lambo');d.x=x;d.z=z+.5;d.h=2.4;d.step(0,0,0,true,false);man(0x333333,0x222222,0xc68c62,x+4.5,z1-1.8,Math.PI)}
    const mk=new THREE.Mesh(new THREE.CylinderGeometry(2.5,2.5,40,16,1,true),new THREE.MeshBasicMaterial({color:new THREE.Color(s.css),transparent:true,opacity:.3,side:THREE.DoubleSide,depthWrite:false,blending:THREE.AdditiveBlending,fog:false}));mk.position.set(x,20,s.mz);this.scene.add(mk)}}
  buildSkins(){const e=$('skin');e.innerHTML='<h2>URBAN THREADS</h2><p>Pick an outfit. B closes the store.</p><div class="shopgrid"></div>';const gr=e.lastChild;
   SKINS.forEach((k,i)=>{const b=document.createElement('button');b.textContent=k.n+(this.owned.has(i)?(i===this.skinI?' ✓':''):' — $'+k.price);b.onclick=()=>this.pickSkin(i);gr.appendChild(b)});
   const x=document.createElement('button');x.textContent='Close store';x.onclick=()=>this.closeShop();gr.appendChild(x)}
  pickSkin(i){const k=SKINS[i];if(!this.owned.has(i)){if(this.money<k.price){this.toast('Not enough cash');return}this.cash(-k.price);this.owned.add(i)}this.skinI=i;const m=this.player.mat;m.sh.color.setHex(k.sh);m.pn.color.setHex(k.pn);m.sk.color.setHex(k.sk);this.toast(k.n+' equipped');this.buildSkins()}
  buyItem(n){if(n==='Close'){this.closeShop();return}const P={Pistol:300,SMG:900,Shotgun:1200,Rifle:1800,Sniper:2200,Grenade:250,C4:500,Armor:700,Medkit:150,Ammo:100,Motorcycle:1000},pr=P[n]||0;if(this.money<pr){this.toast('Not enough cash');return}
   if(n==='Ammo'&&!WEAP[this.weaponName]){this.toast('Equip a gun first');return}this.cash(-pr);const p=this.player;
   if(n==='Motorcycle'){const c=new Car(this.scene,0x26d6d0,'motorcycle');c.x=p.x+3;c.z=p.z;c.h=p.face;this.cars.push(c)}
   else if(n==='Armor')this.armor=100;else if(n==='Medkit')this.health=100;
   else if(n==='Ammo')this.am[this.weaponName]+=WEAP[this.weaponName].ammo;
   else if(WEAP[n]){this.own.add(n);this.am[n]=(this.am[n]||0)+WEAP[n].ammo;this.weaponName=n}else this.weaponName=n;
   this.toast(n+' purchased')}
  shoot(){this.xshot();if(this.flying){this.fireMsl();return}const dv=this.driving;if(dv&&dv.mytank){if(this.weaponCooldown>0)return;this.weaponCooldown=1.1;const tx=dv.x+Math.sin(dv.h)*38,tz=dv.z+Math.cos(dv.h)*38;this.tracer(dv.x,2.6,dv.z,tx,1,tz);this.boom(tx,tz,9,90);this.sfx.shot(1.6);return}const W=WEAP[this.weaponName]&&this.eff(this.weaponName);if(this.driving||this.weaponCooldown>0||this.dead>0)return;
   if(!W){if(this.weaponName==='Fist')this.punch();else this.toast('Buy a gun at Harbor Arms (B)');return}
   if(this.rl>0)return;const wn=this.weaponName;if(!(this.mag[wn]>0)){if(this.am[wn]>0)this.reload();else{this.toast('Out of ammo');this.weaponCooldown=.4}return}
   this.weaponCooldown=W.rate;this.mag[wn]--;this.quiet=W.sil;const p=this.player,f=this.rig.yaw;p.face=f;p.g.rotation.y=f;this.fireT=.8;this.flash=.05;this.sfx.shot(W.sil?.12:1);
   const tz=.7+W.len/2,mx=p.x+Math.sin(f)*tz-Math.cos(f)*.4,mz=p.z+Math.cos(f)*tz+Math.sin(f)*.4;p.flashM.position.set(-.4,1.6,tz+.1);let hitCar=null;
   for(let k=0;k<W.pel;k++){const a=f+(Math.random()-.5)*W.spr*(this.aiming?.5:1)*2,dx=Math.sin(a),dz=Math.cos(a);let best=W.rng;
    wall:for(let d=1.5;d<best;d+=1.5){const x=p.x+dx*d,z=p.z+dz*d;for(const b of this.world.grid.at(x,z))if(x>b.x0&&x<b.x1&&z>b.z0&&z<b.z1){best=d;break wall}}
    let car=null,ped=null;
    for(const c of this.cars){const rx=c.x-p.x,rz=c.z-p.z,al=rx*dx+rz*dz;if(al>0&&al<best&&Math.abs(rx*dz-rz*dx)<1.2){best=al;car=c}}
    for(const q of this.peds.p){if(q.dead>0)continue;const rx=q.x-p.x,rz=q.z-p.z,al=rx*dx+rz*dz;if(al>0&&al<best&&Math.abs(rx*dz-rz*dx)<.7){best=al;ped=q;car=null}}
    this.tracer(mx,1.55,mz,p.x+dx*best,1.3,p.z+dz*best);
    if(ped)this.hitPed(ped,W.dmg,true);else if(car){car.stun=2;car.vx+=dx*3;car.vz+=dz*3;hitCar=car;this.dmgCar(car,W.dmg*.8)}}
   if(hitCar&&this.wanted<1&&!W.sil)this.addWanted(1);this.quiet=false}
  punch(){if(this.driving||this.flying||this.dead>0||this.weaponCooldown>0)return;this.weaponCooldown=.4;this.punchT=.3;this.pf^=1;const p=this.player;p.face=this.rig.yaw;
   for(const q of this.peds.p)if(q.dead<=0&&q.down<=0&&Math.hypot(q.x-p.x,q.z-p.z)<2){this.hitPed(q,12,true);return}
   for(const c of this.cars)if(Math.hypot(c.x-p.x,c.z-p.z)<2.8){c.stun=2;c.vx+=Math.sin(p.face)*4;c.vz+=Math.cos(p.face)*4;if(this.wanted<1)this.addWanted(1);return}}
  hitPed(q,dmg,by){q.hp-=dmg;this.sfx.beep(120);q.free=true;if(q.hp<=0)this.killPed(q,by)}
  tracer(x0,y0,z0,x1,y1,z1){const t=this.trs.find(o=>!o.visible);if(!t)return;t.position.set((x0+x1)/2,(y0+y1)/2,(z0+z1)/2);t.scale.set(1,1,Math.hypot(x1-x0,y1-y0,z1-z0)||1);t.lookAt(x1,y1,z1);t.visible=true;t.life=.07}
  pedShoot(q){const p=this.driving||this.player;this.tracer(q.x,1.4,q.z,p.x+(Math.random()-.5)*2,1.2,p.z+(Math.random()-.5)*2);this.sfx.shot();if(Math.random()<.45)this.hurt(6)}
  jack(c){const q=this.peds.p.find(o=>o.dead<=0&&!o.free)||this.peds.p[0],sn=Math.sin(c.h),cs=Math.cos(c.h);q.x=c.x+cs*.9;q.z=c.z-sn*.9;q.free=true;q.down=3.5;q.dead=0;q.hp=100;q.vx=q.vz=0;q.jv=[cs*7,-sn*7];q.pull=.45;q.hd=c.h;q.fy=0;q.fv=0;q.rt=0;q.gun=Math.random()<.4;q.cd=1;
   if(c.type==='police'){c.type=null;c.body.material.emissive.setHex(0);this.policeSpawned=Math.max(0,this.policeSpawned-1);this.addWanted(2)}this.toast('Carjacked! The driver is on the ground');this.sfx.beep(180)}
  list(){return['Fist',...GUNS.filter(n=>this.own.has(n))]}
  equip(i){const l=this.list();if(l[i]){this.weaponName=l[i];this.toast(l[i])}}
  placeC4(){if(this.driving)return;const p=this.player;this.c4.push({x:p.x,z:p.z,t:0,mesh:new THREE.Mesh(new THREE.BoxGeometry(.25,.12,.25),new THREE.MeshStandardMaterial({color:0x222222,emissive:0x551100}))});const o=this.c4[this.c4.length-1];o.mesh.position.set(o.x,.12,o.z);this.scene.add(o.mesh);this.toast('C4 placed — press X again to detonate')}
  detonateC4(){if(!this.c4.length)return;for(const b of this.c4){this.boom(b.x,b.z,9,90);this.scene.remove(b.mesh)}this.c4=[];this.addWanted(2);this.toast('C4 detonated')}
  addWanted(n){this.setWanted(this.wanted+n);this.cops()}
  setWanted(n){n=U.clamp(n,0,5);this.wanted=n;this.evade=0;if(n<3&&this.heli){this.scene.remove(this.heli.g);this.heli=null}$('wanted').textContent='★'.repeat(n)+'☆'.repeat(5-n);if(n)return;const p=this.player;
   for(const c of this.cars.slice()){if(c.type==='tank'){this.scene.remove(c.m);this.cars.splice(this.cars.indexOf(c),1)}else if(c.type==='police'){c.type=null;c.body.material.emissive.setHex(0);this.traffic.respawn(c,p.x,p.z)}}this.policeSpawned=0;this.tankSpawned=false}
  spawnPolice(){const c=new Car(this.scene,0x202a42,'police');this.traffic.respawn(c,this.player.x,this.player.z);this.cars.push(c);this.policeSpawned++;this.sfx.beep(520)}
  killPed(q,by){q.dead=10;this.sfx.beep(90);if(by){if(this.ch&&this.ch.type==='kill')this.ch.n++;this.cash(20+Math.round(Math.random()*120));if(this.wanted<2&&!this.quiet)this.addWanted(1)}}
  cash(n){if(this.rich&&n<0)n=0;this.money+=n;$('money').textContent='$ '+this.money.toLocaleString();if(n>0)this.toast('+$'+n)}
  hurt(n){if(this.dead>0||this.god)return;if(this.armor>0){const a=Math.min(this.armor,n*.7);this.armor-=a;n-=a}this.health-=n;this.hitT=.4;if(this.health<=0){this.health=0;this.die('WASTED','#d4d4d4',Math.min(this.money,500))}}

 xL(a,b){return S.lang==='fa'?b:a}
 xtp(x,z,yaw,zone){const p=this.player;p.x=x;p.z=z;p.y=0;p.vx=p.vz=0;p.face=yaw;this.rig.yaw=yaw;this.rig.init=false;this.zone=zone;this.sfx.beep(520)}
 xnpc(c,x,z,ry,gun,tint){const sc=this.scene,M=k=>new THREE.MeshStandardMaterial({color:k,roughness:.8}),H=mkHuman(M(c),M(tint||0xe0b090),M(0x22252c),M([0x1a1208,0x4a2a14,0xc9a227,0x777777][Math.floor(Math.random()*4)]));
  if(gun){const o=new THREE.Mesh(new THREE.BoxGeometry(.1,.12,.5),M(0x111111));o.position.set(.4,1.15,.35);H.g.add(o)}H.g.position.set(x,0,z);H.g.rotation.y=ry;sc.add(H.g);return{g:H.g,head:H.head,aL:H.aL,aR:H.aR,lL:H.lL,lR:H.lR,t:Math.random()*6,hp:60}}
 xan(n,dt,walk){n.t+=dt;const pl=this.player,gp=n.g.position,dx=pl.x-gp.x,dz=pl.z-gp.z,d=Math.hypot(dx,dz);
  if(!walk&&d<9)n.g.rotation.y=U.lerpA(n.g.rotation.y,Math.atan2(dx,dz),Math.min(1,dt*4));
  const s=walk?Math.sin(n.t*8)*.7:0;n.lL.rotation.x=s;n.lR.rotation.x=-s;n.aL.rotation.x=-s*.8+(walk?0:Math.sin(n.t*1.7)*.06);n.aR.rotation.x=s*.8+(walk?0:Math.cos(n.t*1.9)*.06);
  if(!walk&&!n.nw&&d<6)n.aR.rotation.x=-2.2+Math.sin(n.t*6)*.3;n.head.rotation.y=Math.sin(n.t*.9)*.25;gp.y=walk?Math.abs(Math.sin(n.t*8))*.06:Math.sin(n.t*2)*.015}
 xi(){const G=this,sc=this.scene,W=this.world,L=W.L,M=(c,r=.8,m=0)=>new THREE.MeshStandardMaterial({color:c,roughness:r,metalness:m}),Lg=(a,b)=>G.xL(a,b);
  this.xin=1;this.zone='city';this.xs=[];this.xn=[];this.xcp=[];this.xc=null;this.xj=null;this.xloot=-9999;this.xdoors=[];this.xg=[];this.xback={x:20,z:10};this.xparts=[];this.xneon();
  const bx=(w,h,d,c,x,y,z,sd,em)=>{const o=new THREE.Mesh(new THREE.BoxGeometry(w,h,d),em?new THREE.MeshBasicMaterial({color:c}):M(c));o.position.set(x,y,z);o.castShadow=o.receiveShadow=true;sc.add(o);let q=null;if(sd){q={x0:x-w/2,x1:x+w/2,z0:z-d/2,z1:z+d/2,h:h+y};W.boxes.push(q);W.grid.add(q)}return{o,q}},
  P=(x,z,r,t,fn,cond)=>{const p={x,z,r,t,fn,if:cond};this.xs.push(p);return p},
  room=(cx,w,d,h,fl,wl,lc)=>{bx(w,.2,d,fl,cx,-.1,0);bx(w,.2,d,0x1b1d24,cx,h+.1,0);bx(w+1.2,h,.6,wl,cx,h/2,-d/2-.3,1);bx(w+1.2,h,.6,wl,cx,h/2,d/2+.3,1);bx(.6,h,d,wl,cx-w/2-.3,h/2,0,1);bx(.6,h,d,wl,cx+w/2+.3,h/2,0,1);const l=new THREE.PointLight(lc,1.4,w*1.6);l.position.set(cx,h-1,0);sc.add(l)},
  npc=(c,x,z,ry,gun,tint)=>{const n=this.xnpc(c,x,z,ry,gun,tint);this.xn.push(n);return n};
  const e1=document.createElement('div');e1.id='xp';e1.className='hud';e1.style.cssText='left:50%;bottom:30%;transform:translateX(-50%);display:none;color:#9dffb0;z-index:6';document.body.appendChild(e1);
  const e2=document.createElement('div');e2.id='xo';e2.className='hud';e2.style.cssText='left:16px;top:56px;display:none;color:#ffd24a;z-index:6';document.body.appendChild(e2);
  this.xm=new THREE.Mesh(new THREE.CylinderGeometry(1.6,1.6,80,14,1,true),new THREE.MeshBasicMaterial({color:0xffd24a,transparent:true,opacity:.4,side:THREE.DoubleSide,depthWrite:false,blending:THREE.AdditiveBlending,fog:false}));this.xm.visible=false;sc.add(this.xm);
  /* ---- OFFICE interior (x=1500) ---- */
  room(1500,30,22,6,0x6a5a48,0x8a8f99,0xfff0d0);bx(8,1,2.4,0x5a3a22,1500,.5,-7.6,1);bx(5,.9,2,0x2a4a7a,1489,.45,6,1);bx(5,.9,2,0x2a4a7a,1511,.45,6,1);bx(10,3,.1,0xc03070,1500,3.3,-10.6,0,1);bx(.8,2,.8,0x2a7a3a,1486,1,-9,1);bx(.8,2,.8,0x2a7a3a,1514,1,-9,1);bx(26,.15,.15,0x36f1ff,1500,5.6,0,0,1);
  const fx=npc(0x3a2a5a,1500,-5.4,0,0),ht=npc(0x1a1a1a,1491,-8,0,1,0x8d5a3b),dl=npc(0x4a5a2a,1509,-8,0,0,0xc68c62);
  P(1500,-5.4,3.6,()=>Lg('Press E — talk to Vince (heists)','E — صحبت با وینس (سرقت)'),()=>this.xgive('rob'));
  P(1491,-8,3.4,()=>Lg('Press E — talk to Mako (hits)','E — صحبت با ماکو (ترور)'),()=>this.xgive('kill'));
  P(1509,-8,3.4,()=>Lg('Press E — talk to Dutch (tank job)','E — صحبت با داچ (تانک)'),()=>this.xgive('tank'));
  P(1500,9.2,3,()=>Lg('Press E — leave the building','E — خروج از ساختمان'),()=>{const b=this.xback;this.xtp(b.x,b.z,0,'city')});
  /* ---- PRISON interior (x=1700) ---- */
  room(1700,44,30,6,0x55585f,0x6a6d74,0xcfe0ff);
  const bars=(x0,z0,x1,z1,n)=>{const gr=new THREE.Group();for(let i=0;i<=n;i++){const o=new THREE.Mesh(new THREE.BoxGeometry(.12,3.6,.12),M(0x222226,.4,.7));o.position.set(x0+(x1-x0)*i/n,1.8,z0+(z1-z0)*i/n);gr.add(o)}sc.add(gr);return gr};
  bars(1688,-15,1688,-9,8);bars(1678,-6,1688,-6,12);const dg=bars(1688,-9,1688,-6.4,4),dq=bx(.4,3.6,2.6,0x222226,1688,1.8,-7.7,1).q;this.xdoor={g:dg,q:dq,o:{x0:dq.x0,x1:dq.x1,z0:dq.z0,z1:dq.z1}};bx(.5,3.6,6,0x222226,1688,1.8,-12,1).o.visible=false;bx(10,3.6,.5,0x222226,1683,1.8,-6,1).o.visible=false;
  bx(2.2,.5,1,0x777777,1680.2,.45,-13,1);bx(1.2,.2,.9,0x777777,1679.8,.6,-9.4,1);bx(8,1,2,0x4a4a52,1712,.5,-10,1);bx(.2,3,.6,0x35c27a,1713,1.7,-13.8,0,1);bx(1,2.2,1,0x3a3a42,1720.5,1.1,12,1);bx(.3,4.2,6,0x44ffb0,1721.7,2.1,12,0,1);
  this.xg=[0,1].map(i=>{const n=this.xnpc(0x16264a,1704,i?5:-1,0,1);n.ph=i*3;n.r=i?9:12;n.z0=i?5:-1;n.walk=1;this.xn.push(n);return n});
  P(1680.4,-12,2.6,()=>Lg('Press E — search the loose brick','E — جستجوی آجر شل'),()=>{this.xj.open=1;this.xdoor.g.visible=false;const q=this.xdoor.q;q.x0=q.x1=q.z0=q.z1=9e9;this.toast(Lg('You found a spoon and dug the lock — the cell is open! Avoid the guards','قاشق پیدا کردی و قفل را باز کردی! از نگهبان‌ها دوری کن'))},()=>this.xj&&!this.xj.open);
  P(1712,-12,3.2,()=>Lg('Press E — take the guard keycard','E — برداشتن کارت نگهبان'),()=>{this.xj.key=1;this.toast(Lg('Keycard taken! Now reach the exit gate','کارت را برداشتی! به دروازه خروج برو'))},()=>this.xj&&this.xj.open&&!this.xj.key);
  P(1720,12,3.4,()=>Lg('Press E — exit gate','E — دروازه خروج'),()=>{if(this.xj.key){this.xj=null;this.xtp(14,12,0,'city');this.setWanted(0);this.big(Lg('ESCAPED!','فرار موفق!'),'','#9dffb0',3)}else this.toast(Lg('Gate locked — you need the keycard','دروازه قفل است — کارت لازم داری'))},()=>this.xj);
  /* ---- UNDERGROUND (x=1900) ---- */
  room(1900,60,12,4,0x2a2a30,0x3a3a40,0xff9a50);for(let i=0;i<4;i++){const o=new THREE.Mesh(new THREE.CylinderGeometry(.25,.25,60,8).rotateZ(Math.PI/2),M(0x884422,.6,.5));o.position.set(1900,3.4-i*.0,-5.4+i*.1);sc.add(o)}
  for(let i=0;i<6;i++)bx(1.6,1.6,1.6,i%2?0x6a4a2a:0x4a5a3a,1912+i*3,.8,-3.5+((i*7)%5)*.4,1);bx(2.5,2,2.5,0xd4a017,1926,1,2,1);
  const sm=npc(0x2a2a2a,1900,-3,0,1,0x8d5a3b);P(1900,-3,3.4,()=>Lg('Press E — talk to the Smuggler (heists)','E — صحبت با قاچاقچی (سرقت)'),()=>this.xgive('rob'));
  npc(0x4a1a1a,1890,-3,0,1,0x8d5a3b);P(1890,-3,3.2,()=>Lg('Press E — talk to Mako (hits)','E — صحبت با ماکو (ترور)'),()=>this.xgive('kill'));npc(0x2a4a2a,1908,-3,0,0,0xc68c62);P(1908,-3,3.2,()=>Lg('Press E — talk to Dutch (tank job)','E — صحبت با داچ (تانک)'),()=>this.xgive('tank'));P(1926,2,3.6,()=>Lg('Press E — loot the stash','E — غارت مخفیگاه'),()=>{const n=performance.now()/1000;if(n-this.xloot<600){this.toast(Lg('The stash is empty — come back later','مخفیگاه خالی است — بعداً بیا'));return}this.xloot=n;this.cash(15000);this.big(Lg('SECRET STASH','مخفیگاه مخفی'),'$ 15,000','#ffd24a',3)});
  P(1872.5,0,3,()=>Lg('Press E — climb the ladder','E — بالا رفتن از نردبان'),()=>{const b=this.xmh;this.xtp(b.x,b.z+3,0,'city')});
  bx(.3,4,1,0x888888,1870.4,2,0,0);
  /* manhole (secret entrance) */
  {const mx=L[4],mz=L[5]+30,o=new THREE.Mesh(new THREE.CylinderGeometry(1,1,.06,16),M(0x2a2a2e,.5,.8));o.position.set(mx,.07,mz);sc.add(o);this.xmh={x:mx,z:mz};
   P(mx,mz,2.4,()=>Lg('Press E — secret manhole','E — دریچه مخفی'),()=>this.xtp(1875,0,Math.PI/2,'und'))}
  /* ---- CASINO interior (x=2100) ---- */
  room(2100,44,30,7,0x6a1426,0x2a1030,0xffe2a8);bx(42,.03,28,0x7a1a2a,2100,.01,0,0,1);
  bx(40,.12,.12,0xff2d95,2100,6.6,-8,0,1);bx(40,.12,.12,0x2de2ff,2100,6.6,8,0,1);bx(4,.3,4,0xffe9a0,2100,6.3,0,0,1);
  for(const sx of[-1,1])for(const sz of[-1,1])bx(1,7,1,0xd4a017,2100+sx*20,3.5,sz*13.5,1);
  for(let i=0;i<8;i++){const x=2083+i*4.6;bx(1.4,2.4,1.1,0x22222a,x,1.2,-13.9,1);bx(1.1,.8,.1,[0xff2d95,0x2de2ff,0xffd12d,0x7dff3d][i%4],x,1.7,-13.3,0,1);P(x,-11.8,2.3,()=>Lg('Press E — slot machine ($1,000 · 777 = $50,000)','E — اسلات ($1,000 · 777 = $50,000)'),()=>this.xslot())}
  bx(10,1,6,0x0a5a2a,2108,.5,1,1);bx(9.4,.05,5.4,0x16803a,2108,1.02,1,0,1);bx(1.8,.3,1.8,0xd4a017,2105,1.15,0,0,1);npc(0xaa1133,2108,-2.5,0,0,0xf1cfb0);
  P(2104.3,5.6,1.8,()=>Lg('Press E — roulette: $2,000 on RED','E — رولت: ۲۰۰۰ دلار روی قرمز'),()=>this.xroul('red'));
  P(2108,5.6,1.8,()=>Lg('Press E — roulette: $500 on GREEN (pays 36x)','E — رولت: ۵۰۰ دلار روی سبز (۳۶ برابر)'),()=>this.xroul('green'));
  P(2111.7,5.6,1.8,()=>Lg('Press E — roulette: $2,000 on BLACK','E — رولت: ۲۰۰۰ دلار روی مشکی'),()=>this.xroul('black'));
  bx(8,1,4.5,0x14423a,2090,.5,1.5,1);bx(7.4,.05,3.9,0x1c6b4e,2090,1.02,1.5,0,1);npc(0x111111,2090,-1.2,0,0,0xc68c62);
  P(2090,5.3,2.8,()=>Lg('Press E — blackjack ($3,000 bet)','E — بلک‌جک (شرط ۳۰۰۰ دلار)'),()=>this.xbj());
  npc(0x111111,2096,10,0,0,0xc68c62);npc(0x222233,2105,10,0,0,0x8d5a3b);
  P(2100,12.4,3,()=>Lg('Press E — leave the casino','E — خروج از کازینو'),()=>{const b=this.xback;this.xtp(b.x,b.z,0,'city')});

  this.xcity();/* ---- posters ---- */
  this.xpo=[];const saved=ld('gtaelfo_p',{a:[]}).a,pp=[[1,2],[2,5],[4,1],[5,6],[6,3]];
  pp.forEach((q,i)=>{const px=L[q[0]]+10.5,pz=L[q[1]]+60,c=document.createElement('canvas');c.width=512;c.height=256;this.xdef(c);const t=new THREE.CanvasTexture(c),m=new THREE.Mesh(new THREE.PlaneGeometry(10,5),new THREE.MeshBasicMaterial({map:t,side:THREE.DoubleSide}));
   m.position.set(px-.2,9.5,pz);m.rotation.y=-Math.PI/2;sc.add(m);bx(.3,5.4,10.4,0x15181e,px,9.5,pz);bx(.3,7,.3,0x30343c,px,3.5,pz-3.5);bx(.3,7,.3,0x30343c,px,3.5,pz+3.5);this.xpo[i]={c,t};if(saved[i])this.xposter(i,saved[i])})}
 xdef(c){const g=c.getContext('2d'),gr=g.createLinearGradient(0,0,512,256);gr.addColorStop(0,'#1b0b3a');gr.addColorStop(1,'#0b3a4a');g.fillStyle=gr;g.fillRect(0,0,512,256);g.strokeStyle='#36f1ff';g.lineWidth=6;g.strokeRect(8,8,496,240);g.fillStyle='#ff3d8b';g.font='bold 64px sans-serif';g.textAlign='center';g.fillText('YOUR AD',256,125);g.fillStyle='#36f1ff';g.fillText('HERE',256,200)}
 xposter(i,u){const P=this.xpo&&this.xpo[i];if(!P)return;if(!u){this.xdef(P.c);P.t.needsUpdate=true;return}const im=new Image();im.onload=()=>{P.c.getContext('2d').drawImage(im,0,0,512,256);P.t.needsUpdate=true};im.src=u}
 xfile(i,f,clr){const st=ld('gtaelfo_p',{a:[]}).a;if(clr){st[i]=null;sv('gtaelfo_p',{a:st});if(this.xin)this.xposter(i,null);return}if(!f)return;const r=new FileReader();r.onload=()=>{const im=new Image();im.onload=()=>{const c=document.createElement('canvas');c.width=512;c.height=256;const g=c.getContext('2d'),s=Math.max(512/im.width,256/im.height),w=im.width*s,h=im.height*s;g.drawImage(im,(512-w)/2,(256-h)/2,w,h);const u=c.toDataURL('image/jpeg',.82),a=ld('gtaelfo_p',{a:[]}).a;a[i]=u;sv('gtaelfo_p',{a});if(this.xin)this.xposter(i,u);this.toast(this.xL('Poster '+(i+1)+' updated','پوستر '+(i+1)+' به‌روز شد'))};im.src=r.result};r.readAsDataURL(f)}
 xgive(k){if(this.xc){this.toast(this.xL('Finish your current challenge first','اول چالش فعلی را تمام کن'));return}const rw={rob:7000,kill:4000,tank:9000}[k];this.xc={k,t:k==='tank'?300:240,rw,tg:null};
  if(k==='rob'){let j,t=0;do{j=Math.floor(Math.random()*this.xdoors.length)}while(this.xdoors.length>1&&j===this.xcur&&t++<20);this.xc.door=j}
  this.toast({rob:this.xL('Job: rob the marked building (yellow beacon). Leave and go there.','کار: از ساختمان علامت‌خورده سرقت کن (نور زرد).'),kill:this.xL('Hit: a man is marked. Take him out.','ترور: یک نفر علامت‌خورده، او را بزن.'),tank:this.xL('Job: destroy the marked tank!','کار: تانک علامت‌خورده را نابود کن!')}[k]);this.sfx.beep(660)}
 xchal(dt){const c=this.xc,o=$('xo'),m=this.xm;if(!c){o.style.display='none';m.visible=false;return}
  c.t-=dt;if(c.t<=0){this.toast(this.xL('Challenge failed: time is up','چالش شکست خورد: زمان تمام شد'));this.xc=null;return}
  let tx=null,tz=null,txt='';const pl=this.player;
  if(c.k==='rob'){const d=this.xdoors[c.door];if(d){tx=d.x;tz=d.z;txt=this.xL('Rob: ','سرقت: ')+d.n}}
  else if(c.k==='kill'){txt=this.xL('Hit: eliminate the target','ترور: هدف را بزن');if(!c.tg&&this.zone==='city'){let b=1e9;for(const q of this.peds.p){if(q.dead>0||q.free)continue;const d=Math.hypot(q.x-pl.x,q.z-pl.z);if(d>40&&d<220&&d<b){b=d;c.tg=q}}}
   if(c.tg){tx=c.tg.x;tz=c.tg.z;if(c.tg.dead>0)return this.xdone()}}
  else{txt=this.xL('Destroy the tank','تانک را نابود کن');if(!c.tg&&this.zone==='city'){const t=new Car(this.scene,0x536b4a,'tank');t.x=pl.x+80;t.z=pl.z+60;t.h=0;this.cars.push(t);c.tg=t;this.addWanted(1)}
   if(c.tg){if(c.tg.wreck)return this.xdone();if(!this.cars.includes(c.tg))c.tg=null;else{tx=c.tg.x;tz=c.tg.z}}}
  o.style.display='block';o.textContent=txt+' · '+(c.t|0)+'s · $'+c.rw;if(tx!=null){m.visible=true;m.position.set(tx,40,tz)}else m.visible=false}
 xdone(){const c=this.xc;this.cash(c.rw);this.big(this.xL('CHALLENGE COMPLETE','چالش کامل شد'),'$ '+c.rw.toLocaleString(),'#9dffb0',3);this.sfx.beep(880);this.xc=null}
 xguards(dt){if(this.zone!=='pri'||!this.xj)return;const pl=this.player;for(const g of this.xg){g.ph+=dt*.5;const x=1704+Math.sin(g.ph)*g.r;g.g.position.x=x;g.g.position.z=g.z0;g.g.rotation.y=Math.cos(g.ph)>0?Math.PI/2:-Math.PI/2;
   if(!this.driving&&pl.x>1689&&Math.hypot(x-pl.x,g.z0-pl.z)<4.2&&this.dead<=0){this.toast(this.xL('A guard spotted you! Back to the cell','نگهبان تو را دید! بازگشت به سلول'));this.xtp(1684,-10.5,Math.PI/2,'pri');this.xj.t=Math.max(this.xj.t,60);this.xj.key=0;break}}
  this.xj.t-=dt;if(this.xj.t<=0){this.xj=null;this.xtp(14,12,0,'city');this.toast(this.xL('You served your time — released','دوران حبس تمام شد — آزاد شدی'))}}
 xjail(){const q=this.xdoor.q,o=this.xdoor.o;q.x0=o.x0;q.x1=o.x1;q.z0=o.z0;q.z1=o.z1;this.xdoor.g.visible=true;this.xj={t:150,key:0,open:0};this.xtp(1684,-10.5,Math.PI/2,'pri');this.setWanted(0);this.toast(this.xL('PRISON: find a way out before your sentence ends (150s)','زندان: قبل از پایان حکم (۱۵۰ ثانیه) راه فرار پیدا کن'))}
 xcops(dt){const pl=this.player,w=this.wanted,tgt=this.driving||pl;const al=this.xcp.filter(c=>!c.gone);if(al.length!==this.xcp.length){for(const c of this.xcp)if(c.gone)this.scene.remove(c.g);this.xcp=al}
  for(const c of al){if(c.dead){c.dt+=dt;c.g.rotation.x=Math.min(1.5,c.dt*4);if(c.dt>6){c.gone=1;c.g.visible=false}continue}
   if(w<=0||this.zone!=='city'){c.gone=1;c.g.visible=false;continue}
   const gp=c.g.position,dx=tgt.x-gp.x,dz=tgt.z-gp.z,d=Math.hypot(dx,dz);c.g.rotation.y=U.lerpA(c.g.rotation.y,Math.atan2(dx,dz),Math.min(1,dt*6));
   if(d>90){c.gone=1;c.g.visible=false;continue}
   const mv=d>11;if(mv){const nx=gp.x+dx/d*4.6*dt,nz=gp.z+dz/d*4.6*dt;if(this.world.free(nx,gp.z,.5))gp.x=nx;if(this.world.free(gp.x,nz,.5))gp.z=nz}
   for(const k of this.cars){if(k.wreck)continue;const ex=gp.x-k.x,ez=gp.z-k.z,ed=Math.hypot(ex,ez);if(ed<2.5&&ed>.01){if(k===this.driving&&Math.abs(k.sp)>7)c.hp=0;else{gp.x=k.x+ex/ed*2.5;gp.z=k.z+ez/ed*2.5}}}this.xan(c,dt,mv);c.g.rotation.y=U.lerpA(c.g.rotation.y,Math.atan2(dx,dz),1);
   if(!mv&&this.dead<=0){c.cd-=dt;if(c.cd<=0){c.cd=1.1;this.tracer(gp.x,1.4,gp.z,tgt.x+(Math.random()-.5)*2,1.2,tgt.z+(Math.random()-.5)*2);this.sfx.shot(.7);if(Math.random()<.5)this.hurt(5)}}
   if(this.driving&&Math.abs(this.driving.sp)>9&&d<2.6){c.hp=0}
   if(c.hp<=0){c.dead=1;c.dt=0;this.addWanted(0)}}
  if(w>0&&this.zone==='city'&&this.state==='PLAYING'){this.xcT=(this.xcT||0)-dt;if(this.xcT<=0&&al.filter(c=>!c.dead).length<Math.min(6,w*2)){this.xcT=2.5;for(const o of this.cars){if(o.type!=='police'||o.wreck)continue;const d=Math.hypot(o.x-tgt.x,o.z-tgt.z);if(d<45&&d>6&&Math.abs(o.sp)<4){const n=this.xnpc(0x16264a,o.x+Math.cos(o.h)*1.8,o.z-Math.sin(o.h)*1.8,0,1);n.cd=.8;n.dead=0;this.xcp.push(n);break}}}}}
 xshot(){if(this.driving||this.flying||this.weaponCooldown>0||this.dead>0||this.zone!=='city')return;const Wp=WEAP[this.weaponName];if(!Wp||!(this.mag[this.weaponName]>0)||this.rl>0)return;const pl=this.player,y=this.rig.yaw,fx=Math.sin(y),fz=Math.cos(y);
  for(const c of this.xcp){if(c.gone||c.dead)continue;const dx=c.g.position.x-pl.x,dz=c.g.position.z-pl.z,d=Math.hypot(dx,dz);if(d>Wp.rng||d<.5)continue;const f=(dx*fx+dz*fz)/d;if(f>0&&d*Math.sqrt(Math.max(0,1-f*f))<1.3){c.hp-=Wp.dmg*Wp.pel}}}
 xhd(a){if(a.y>1||Math.abs(a.sp||0)>3||this.flying===a){this.toast(this.xL('Park the plane and stop first','اول هواپیما رو فرود بیار و کامل نگه دار'));return}a.dro=a.dro?0:1;const ch=Math.cos(a.h),sh=Math.sin(a.h);let n=0;
  if(a.dro){for(const c of this.cars)if(c.xh===a)c.xh=null;this.toast(this.xL('Cargo door OPEN — drive a car inside','درِ بار باز شد — ماشین رو ببر داخل'))}
  else{for(const c of this.cars){if(c.wreck||c===this.driving)continue;const dx=c.x-a.x,dz=c.z-a.z,lx=dx*ch-dz*sh,lz=dx*sh+dz*ch;if(Math.abs(lx)<3.3&&lz>-19.5&&lz<19.5){c.xh=a;c.ai=null;c.xl=[lx,lz,U.wrap(c.h-a.h)];n++}}this.toast(n?this.xL('Door closed — '+n+' vehicle(s) secured','در بسته شد — '+n+' وسیله بار شد'):this.xL('Cargo door closed','درِ بار بسته شد'))}this.sfx.beep(n?520:380)}
 xhaulMarker(a){const Lg=(x,y)=>this.xL(x,y);a.xp={x:a.x-Math.sin(a.h)*22,z:a.z-Math.cos(a.h)*22,r:10,t:()=>a.dro?Lg('Press E — CLOSE cargo door','E — بستن درِ بار'):Lg('Press E — OPEN cargo door','E — باز کردن درِ بار'),fn:()=>this.xhd(a),if:()=>a.alive&&this.flying!==a};this.xs.push(a.xp);return a}
 xhaul(dt){for(const a of this.planes){if(!a.P.bay)continue;a.dra=U.lerp(a.dra||0,a.dro?1:0,1-Math.exp(-dt*2));if(a.g.ramp)a.g.ramp.rotation.x=-a.dra*(Math.PI/2+.045);const sn=Math.sin(a.h),cs=Math.cos(a.h);if(a.xp){a.xp.x=a.x-sn*28;a.xp.z=a.z-cs*28}
  for(const c of this.cars){if(c.xh!==a)continue;if(!a.alive){c.xh=null;this.explode(c);continue}const l=c.xl,v=this._hv||(this._hv=new THREE.Vector3());a.g.updateMatrixWorld(true);v.set(l[0],-2.95,l[1]).applyMatrix4(a.g.matrixWorld);c.x=v.x;c.z=v.z;c.h=a.h+l[2];c.vx=c.vz=0;c.sp=0;c.step(0,0,0,true,false);c.y=v.y;c.m.position.y=v.y+(c.wh?0:c.rh);c.m.quaternion.copy(a.g.quaternion).multiply((this._hq||(this._hq=new THREE.Quaternion())).setFromAxisAngle(new THREE.Vector3(0,1,0),l[2]))}}}
 xt(dt){if(!this.xin)this.xi();this.xex(dt);if(this.state!=='PLAYING')return;const pl=this.player,on=!this.driving&&!this.flying&&this.dead<=0;
  for(const n of this.xn)this.xan(n,dt,n.walk);this.xguards(dt);this.xcops(dt);this.xchal(dt);this.xentU(dt);this.xcar(dt);this.xhaul(dt);
  let b=null,bd=1e9;if(on)for(const p of this.xs){const d=Math.hypot(p.x-pl.x,p.z-pl.z);if(d<p.r&&d<bd&&(!p.if||p.if())){b=p;bd=d}}
  this.xnear=b;const e=$('xp');if(b){e.textContent=typeof b.t==='function'?b.t():b.t;e.style.display='block'}else e.style.display='none'}
  xthug(dt){const pl=this.player,th=this.xth;
  if(!th){const d=this.driving;this.xcd=(this.xcd||0)-dt;if(!d||this.zone!=='city'||d.type==='tank'||d.type==='mytank'||d.wreck||Math.abs(d.sp||0)>5||this.xcd>0)return;this.xtm=(this.xtm||0)+dt;if(this.xtm<4)return;this.xtm=0;if(Math.random()>.3)return;
   const car=d;this.toggleCar();const n=this.xnpc(0x7a1f1f,car.x+Math.cos(car.h)*2.5,car.z-Math.sin(car.h)*2.5,0,0,0x9a6a4a);this.xth={n,car,ph:'run',t:0,hit:0};this.xcd=60;this.toast(this.xL('A thug dragged you out of your car!','یه گردن‌کلفت تو را از ماشین بیرون کشید!'));this.sfx.beep(180);return}
  const n=th.n,gp=n.g.position,car=th.car;th.t+=dt;
  if(th.ph==='run'||th.ph==='beat'){const dx=pl.x-gp.x,dz=pl.z-gp.z,d=Math.hypot(dx,dz);n.g.rotation.y=U.lerpA(n.g.rotation.y,Math.atan2(dx,dz),Math.min(1,dt*8));
   if(d>1.5&&th.ph==='run'){gp.x+=dx/d*5.5*dt;gp.z+=dz/d*5.5*dt;this.xan(n,dt,1);if(th.t>8)th.ph='steal'}
   else{if(th.ph==='run'){th.ph='beat';th.t=0}this.xan(n,dt,0);n.aR.rotation.x=-1.6+Math.sin(th.t*14)*.9;n.aL.rotation.x=-1.6+Math.cos(th.t*14)*.9;th.hit-=dt;if(th.hit<=0){th.hit=.55;this.hurt(6);this.sfx.beep(140);pl.vx+=dx/Math.max(d,.1)*-2;pl.vz+=dz/Math.max(d,.1)*-2}if(th.t>2.6){th.ph='steal';th.t=0}}}
  else if(th.ph==='steal'){const dx=car.x-gp.x,dz=car.z-gp.z,d=Math.hypot(dx,dz);n.g.rotation.y=Math.atan2(dx,dz);if(d>1.8){gp.x+=dx/d*6*dt;gp.z+=dz/d*6*dt;this.xan(n,dt,1)}else{n.g.visible=false;th.ph='drive';th.t=0;this.toast(this.xL('He stole your car!','ماشینت را دزدید!'));car.ai=false}}
  else{car.step(dt,1,Math.sin(th.t*.8)*.35,false,false);if(th.t>9||car.wreck){this.xth=null}}}
 xdim(c){const d=c.model&&CARMODELS[c.model]?CARMODELS[c.model].d:null;return d?{L:d[0],w:d[1],hh:d[3],dh:d[4],z1:d[5],z2:d[6],z3:d[7]}:{L:4.4,w:1.8,hh:.85,dh:.95,z1:.6,z2:-.2,z3:-.7}}
 xdent(c,px,pz,mag){const D=this.xdim(c);if(!c.dg){c.dg={h:0,t:0,l:0,r:0};c.body.geometry=c.body.geometry.clone();c.dg0=c.body.geometry.attributes.position.array.slice()}
  const g=c.body.geometry,pa=g.attributes.position,co=g.attributes.color,a=pa.array,R=1.35,m=Math.min(.6,mag*.07),l=Math.hypot(px,pz)||1,nx=-px/l,nz=-pz/l;
  for(let i=0;i<pa.count;i++){const x=a[i*3],y=a[i*3+1],z=a[i*3+2],d=Math.hypot(x-px,z-pz);if(d<R){const f=Math.pow(1-d/R,1.4)*m,r1=.55+.45*Math.sin(i*12.9),r2=.55+.45*Math.cos(i*7.3);a[i*3]+=nx*f*r1;a[i*3+2]+=nz*f*r2;a[i*3+1]-=f*.22*Math.abs(Math.sin(i*3.1))}}
  const k=mag;if(pz>D.L*.18&&Math.abs(px)<D.w*.45)c.dg.h+=k;else if(pz<-D.L*.18&&Math.abs(px)<D.w*.45)c.dg.t+=k;else if(Math.abs(px)>D.w*.28&&Math.abs(pz)<D.L*.3)c.dg[px>0?'r':'l']+=k;
  const th=18;if(c.dg.h>th&&!c.dgh){c.dgh=1;this.xrip(c,'h',D)}if(c.dg.t>th&&!c.dgt){c.dgt=1;this.xrip(c,'t',D)}if(c.dg.r>th&&!c.dgr){c.dgr=1;this.xrip(c,'r',D)}if(c.dg.l>th&&!c.dgl){c.dgl=1;this.xrip(c,'l',D)}
  pa.needsUpdate=true;g.computeVertexNormals()}
 xrip(c,w,D){const g=c.body.geometry,pa=g.attributes.position,co=g.attributes.color,a=pa.array,o=c.dg0;let sx,sy,sz,px,py,pz;
  if(w==='h'){sx=D.w*.8;sy=.07;sz=D.L*.3;px=0;py=D.hh;pz=D.L/2-sz/2-.1}else if(w==='t'){sx=D.w*.8;sy=.07;sz=D.L*.24;px=0;py=D.dh;pz=-D.L/2+sz/2+.1}else{sx=.07;sy=D.hh*.6;sz=D.L*.24;px=(w==='r'?1:-1)*D.w/2;py=D.hh*.55;pz=(D.z1+D.z3)/2-.2}
  for(let i=0;i<pa.count;i++){const x=o[i*3],y=o[i*3+1],z=o[i*3+2];if(Math.abs(x-px)<=sx/2+.06&&Math.abs(z-pz)<=sz/2+.06&&(w==='r'||w==='l'?(y>.4&&y<D.hh+.1):y>py-.3)){a[i*3+1]-=.1;if(co){co.array[i*3]=.1;co.array[i*3+1]=.1;co.array[i*3+2]=.11}}}
  pa.needsUpdate=true;if(co)co.needsUpdate=true;g.computeVertexNormals();
  const sn=Math.sin(c.h),cs=Math.cos(c.h),wx=c.x+px*cs+pz*sn,wz=c.z-px*sn+pz*cs,mesh=new THREE.Mesh(new THREE.BoxGeometry(sx,sy,sz),new THREE.MeshStandardMaterial({color:c.col,roughness:.4,metalness:.6}));mesh.position.set(wx,(c.y||0)+py,wz);mesh.rotation.y=c.h;mesh.castShadow=true;this.scene.add(mesh);
  const side=(w==='r'?1:w==='l'?-1:0),v=Math.hypot(c.vx||0,c.vz||0);this.xparts.push({m:mesh,vx:(c.vx||0)*.6+cs*side*5+(Math.random()-.5)*3,vz:(c.vz||0)*.6-sn*side*5+(Math.random()-.5)*3,vy:5+Math.random()*4,wx:(Math.random()-.5)*8,wz:(Math.random()-.5)*8,t:0,sy});this.sfx.beep(110);this.toast(this.xL('A part was torn off the car!','یک قطعه از ماشین کنده شد!'))}
 xcar(dt){this.xparts=this.xparts||[];const pl=this.player;
  for(const c of this.cars){if(c.dgR&&!c.wreck){c.body.geometry=c.model?Car.mod(c.model):Car.sg;c.dg=null;c.dgh=c.dgt=c.dgr=c.dgl=0;c.dgR=0}if(c.wreck){if(c.dg)c.dgR=1;continue}if(c.type==='motorcycle'||c.type==='tank'||c.type==='mytank')continue;const d=Math.hypot(c.x-pl.x,c.z-pl.z);if(d>70){c.xv=null;continue}
   const vx=c.vx||0,vz=c.vz||0,p=c.xv;if(p&&c.xhp!=null){const dx=vx-p[0],dz=vz-p[1],dv=Math.hypot(dx,dz);if(dv>4&&c.hp<c.xhp-.5){const wx=-dx,wz=-dz,sn=Math.sin(c.h),cs=Math.cos(c.h),lx=wx*cs-wz*sn,lz=wx*sn+wz*cs,l=Math.hypot(lx,lz)||1,D=this.xdim(c);this.xdent(c,lx/l*D.w*.5,lz/l*D.L*.5,Math.min(12,dv))}}
   c.xv=[vx,vz];c.xhp=c.hp}
  for(let i=this.xparts.length-1;i>=0;i--){const q=this.xparts[i],m=q.m;q.t+=dt;q.vy-=22*dt;m.position.x+=q.vx*dt;m.position.z+=q.vz*dt;m.position.y+=q.vy*dt;if(m.position.y<q.sy/2+.02){m.position.y=q.sy/2+.02;q.vy=-q.vy*.25;q.vx*=.7;q.vz*=.7;q.wx*=.6;q.wz*=.6}m.rotation.x+=q.wx*dt;m.rotation.z+=q.wz*dt;if(q.t>14){this.scene.remove(m);this.xparts.splice(i,1)}}
  for(const c of this.cars){if(c.xdman!=null&&c.xdm){c.xdm.visible=c.xdman>.01;const u=c.xdman;c.xdm.rotation.y=-1.15*(u*u*(3-2*u));continue}const a=c.xd;if(!a)continue;a.t+=dt;const T=a.t,u=T<.4?T/.4:T<.75?1:Math.max(0,1-(T-.75)/.4);if(T>1.2){a.g.visible=false;c.xd=null;continue}a.g.visible=true;a.g.rotation.y=-1.15*(u*u*(3-2*u))}}
 xdoorA(c,mk){if((c.xd&&!mk)||c.wreck)return;const D=this.xdim(c);if(!c.xdm){const g=new THREE.Group(),dm=new THREE.Mesh(new THREE.BoxGeometry(.05,D.hh*.6,1.15),new THREE.MeshStandardMaterial({color:c.col,roughness:.3,metalness:.6})),gl=new THREE.Mesh(new THREE.BoxGeometry(.04,D.hh*.28,.9),new THREE.MeshStandardMaterial({color:0x10151c,roughness:.1,metalness:.8}));dm.position.set(0,D.hh*.3+.35,-.58);gl.position.set(.01,D.hh*.62+.4,-.6);g.add(dm,gl);g.position.set(D.w/2+.03,0,D.z1-.3);g.visible=false;c.m.add(g);c.xdm=g}
  if(!mk)c.xd={g:c.xdm,t:0}}
 xneon(){const W=this.world,sc=this.scene,t=W.boxes.filter(b=>b.h>22&&b.x1-b.x0>8).slice(0,160),n=t.length;if(!n)return;const cl=[0xff2d95,0x2de2ff,0xffd12d,0x7dff3d,0xb04dff],im=new THREE.InstancedMesh(new THREE.BoxGeometry(1,1,1),new THREE.MeshBasicMaterial({color:0xffffff}),n*2),D=new THREE.Object3D(),C=new THREE.Color();
  t.forEach((b,i)=>{const cz=(b.z0+b.z1)/2,cx=(b.x0+b.x1)/2;D.position.set(b.x0-.35,b.h*(.45+W.R()*.3),cz+(W.R()-.5)*(b.z1-b.z0)*.5);D.scale.set(.5,7+W.R()*6,2.2);D.rotation.set(0,0,0);D.updateMatrix();im.setMatrixAt(i*2,D.matrix);C.setHex(cl[Math.floor(W.R()*5)]);im.setColorAt(i*2,C);
   D.position.set(cx,b.h+.8,cz);D.scale.set(1.2,1.6,1.2);D.updateMatrix();im.setMatrixAt(i*2+1,D.matrix);C.setHex(0xff2020);im.setColorAt(i*2+1,C)});im.instanceMatrix.needsUpdate=true;if(im.instanceColor)im.instanceColor.needsUpdate=true;sc.add(im)}
 xslot(){if(!this.pay(1000))return;const S5=['🍒','🍋','🔔','⭐','7'],r=[0,0,0].map(()=>Math.floor(Math.random()*5)),t=r.map(i=>S5[i]).join('  ');let w=0;if(r[0]===r[1]&&r[1]===r[2])w=r[0]===4?50000:10000;this.sfx.beep(w?880:200);if(w){this.cash(w);this.big(t,'+$'+w.toLocaleString(),'#ffd24a',3)}else this.big(t,this.xL('No luck','باختی'),'#ff7a7a',2)}
 xroul(m){const bet=m==='green'?500:2000;if(!this.pay(bet))return;const n=Math.floor(Math.random()*37),isRed=[1,3,5,7,9,12,14,16,18,19,21,23,25,27,30,32,34,36].includes(n),col=n===0?'green':isRed?'red':'black',win=col===m;this.sfx.beep(win?880:200);const t=n+' '+(col==='green'?this.xL('GREEN','سبز'):col==='red'?this.xL('RED','قرمز'):this.xL('BLACK','مشکی'));if(win){const g=m==='green'?bet*36:bet*2;this.cash(g);this.big(t,'+$'+g.toLocaleString(),'#ffd24a',3)}else this.big(t,this.xL('You lost $','باختی $')+bet.toLocaleString(),'#ff7a7a',2)}
 xbj(){if(!this.pay(3000))return;const d=()=>Math.min(10,1+Math.floor(Math.random()*13)),hv=h=>{const s=h.reduce((a,b)=>a+b,0);return h.includes(1)&&s+10<=21?s+10:s},p=[d(),d()],q=[d(),d()];while(hv(p)<17)p.push(d());while(hv(q)<17)q.push(d());const a=hv(p),b=hv(q),r=a>21?-1:b>21?1:a>b?1:a<b?-1:0,t=this.xL('You ','تو ')+a+' - '+this.xL('Dealer ','دیلر ')+b;this.sfx.beep(r>0?880:200);if(r>0){this.cash(6000);this.big(t,'+$6,000','#ffd24a',3)}else if(r===0){this.cash(3000);this.big(t,this.xL('Push - bet returned','مساوی - پول برگشت'),'#ffffff',3)}else this.big(t,this.xL('You lost $3,000','۳۰۰۰ دلار باختی'),'#ff7a7a',2)}
 xentS(c){if(this.xent)return;this.xent={c,ph:0,t:0};c.xdm||this.xdoorA(c,1);}
 xentU(dt){const e=this.xent;if(!e)return;const c=e.c,pl=this.player,k=this.inp.k;for(const n of['KeyW','KeyA','KeyS','KeyD','Space','ShiftLeft'])k[n]=0;
  if(c.wreck||Math.hypot(c.x-pl.x,c.z-pl.z)>14||this.dead>0){this.xent=null;c.xdman=0;return}
  const D=this.xdim(c),sn=Math.sin(c.h),cs=Math.cos(c.h),lx=D.w/2+.8,lz=D.z1-.75,tx=c.x+lx*cs+lz*sn,tz=c.z-lx*sn+lz*cs;e.t+=dt;c.stun=3;
  const ease=u=>u*u*(3-2*u),face=Math.atan2(-cs,sn);
  if(e.ph===0){const dx=tx-pl.x,dz=tz-pl.z,d=Math.hypot(dx,dz);if(d>.3&&e.t<3){pl.x+=dx/d*Math.min(d,3.6*dt);pl.z+=dz/d*Math.min(d,3.6*dt);pl.face=Math.atan2(dx,dz);pl.vx=dx/d*3.6;pl.vz=dz/d*3.6}else{pl.vx=pl.vz=0;pl.face=face;e.ph=1;e.t=0}}
  else if(e.ph===1){pl.face=face;c.xdman=Math.min(1,e.t/.55);if(e.t>.6){e.ph=2;e.t=0;if(c.ai){this.jack(c);c.ai=null;e.drv=1}}}
  else if(e.ph===2){pl.face=face;c.xdman=1;if(e.drv){pl.aimArm=1;const q=Math.sin(Math.min(1,e.t/.5)*Math.PI);pl.x=tx-cs*.25*q;pl.z=tz+sn*.25*q}if(e.t>(e.drv?1.1:.15)){e.ph=3;e.t=0}}
  else if(e.ph===3){const u=Math.min(1,e.t/.55),dx=c.x-tx,dz=c.z-tz;pl.x=tx+dx*ease(u);pl.z=tz+dz*ease(u);pl.face=face;if(u>=1){this.xbyp=1;this.near=c;this.toggleCar();this.xbyp=0;e.ph=4;e.t=0}}
  else{c.xdman=Math.max(0,1-e.t/.4);if(e.t>.45){c.xdman=null;if(c.xdm)c.xdm.visible=false;this.xent=null}}}
 xcity(){const G=this,sc=this.scene,W=this.world,Lg=(a,b)=>G.xL(a,b);G.xtm=[];
  const solid=(x0,x1,z0,z1,h)=>{const q={x0,x1,z0,z1,h};W.boxes.push(q);W.grid.add(q);return q},
  MS=(c,r=.7,m=0)=>new THREE.MeshStandardMaterial({color:c,roughness:r,metalness:m}),BS=c=>new THREE.MeshBasicMaterial({color:c}),
  mk=(w,h,d,m,x,y,z)=>{const o=new THREE.Mesh(new THREE.BoxGeometry(w,h,d),m);o.position.set(x,y,z);o.castShadow=o.receiveShadow=true;sc.add(o);return o},
  flat=(w,d,c,x,y,z)=>{const o=new THREE.Mesh(new THREE.PlaneGeometry(w,d).rotateX(-Math.PI/2),MS(c,.9));o.position.set(x,y,z);o.receiveShadow=true;sc.add(o)},
  win=(col,lit)=>{const c=document.createElement('canvas');c.width=c.height=128;const g=c.getContext('2d');g.fillStyle=col;g.fillRect(0,0,128,128);for(let i=0;i<8;i++)for(let j=0;j<8;j++){g.fillStyle=Math.random()<.6?lit:'#10161f';g.fillRect(i*16+3,j*16+4,10,9)}const t=new THREE.CanvasTexture(c);t.wrapS=t.wrapT=THREE.RepeatWrapping;return t},
  tower=(x,z,w,h,col,lit)=>{const t=win(col,lit);t.repeat.set(w/14,h/14);const m=new THREE.MeshStandardMaterial({map:t,emissiveMap:t,emissive:0xffffff,emissiveIntensity:.3,roughness:.25,metalness:.5});G.xtm.push(m);
   mk(w,h,w,m,x,h/2,z);mk(w+2,2,w+2,MS(0x222831,.4,.6),x,h+1,z);mk(w*.5,6,w*.5,MS(0x333a44,.5,.5),x,h+5,z);const a=mk(.6,28,.6,MS(0x999999,.4,.8),x,h+22,z);mk(1.2,1.2,1.2,BS(0xff2020),x,h+36,z);solid(x-w/2,x+w/2,z-w/2,z+w/2,h)},
  sign=(txt,css,w,h,x,y,z,ry)=>{const c=document.createElement('canvas');c.width=512;c.height=Math.round(512*h/w);const g=c.getContext('2d');g.fillStyle='#0b0612';g.fillRect(0,0,c.width,c.height);g.strokeStyle=css;g.lineWidth=10;g.strokeRect(8,8,c.width-16,c.height-16);g.fillStyle=css;g.shadowColor=css;g.shadowBlur=24;g.font='bold '+(c.height*.42|0)+'px Rajdhani,Impact,sans-serif';g.textAlign='center';g.textBaseline='middle';g.fillText(txt,c.width/2,c.height/2);
   const o=new THREE.Mesh(new THREE.PlaneGeometry(w,h),new THREE.MeshBasicMaterial({map:new THREE.CanvasTexture(c)}));o.position.set(x,y,z);o.rotation.y=ry;sc.add(o)};
  // TWIN TOWERS (east-north)
  {const TW=G.xtw={tw:[],br:[],on:false,t:0};
 for(const z of[-540,-490]){const w=30,h=260,x=675,tx=win('#9fb4c8','#ffe9a8');tx.repeat.set(w/14,h/14);
  const m=new THREE.MeshStandardMaterial({map:tx,emissiveMap:tx,emissive:0xffffff,emissiveIntensity:.3,roughness:.25,metalness:.5,envMap:(Car.init(),Car.env),envMapIntensity:.55});G.xtm.push(m);ENVM.push(m);
  const g=new THREE.Group();g.position.set(x,0,z);sc.add(g);
  const bx=(a,b,c,mt,px,py,pz,par)=>{const o=new THREE.Mesh(new THREE.BoxGeometry(a,b,c),mt);o.position.set(px,py,pz);o.castShadow=o.receiveShadow=true;par.add(o);return o};
  const body=bx(w,h,w,m,0,h/2,0,g),cg=new THREE.Group();g.add(cg);
  bx(w+2,2,w+2,MS(0x222831,.4,.6),0,h+1,0,cg);bx(w*.5,6,w*.5,MS(0x333a44,.5,.5),0,h+5,0,cg);bx(.6,28,.6,MS(0x999999,.4,.8),0,h+22,0,cg);bx(1.2,1.2,1.2,BS(0xff2020),0,h+36,0,cg);
  const box=solid(x-w/2,x+w/2,z-w/2,z+w/2,h),T={x,z,w,h,g,body,cg,box,o:{x0:box.x0,x1:box.x1,z0:box.z0,z1:box.z1},st:'up',t:0,dl:0,go:0};box.tw=T;TW.tw.push(T)}
 for(const y of[190,120])TW.br.push({o:mk(10,5,20,MS(0x8a99aa,.3,.6),675,y,-515),x:675,y,z:-515,vx:0,vy:0,vz:0,r:0});
 G.xtwInit()}
  // CASINO STRIP (east): 3 casinos only, entrance faces the city
  const CN=[['ROYAL CASINO','#ffd24a'],['NEON PALACE','#ff2d95'],['GOLDEN ACE','#2de2ff']];
  CN.forEach((n,k)=>{const z=-380+k*130,x0=632,x1=692,cx=662;mk(60,38,70,MS(0x24122e,.5,.3),cx,19,z);mk(60.4,3,70.4,BS(new THREE.Color(n[1])),cx,39.5,z);
   mk(.4,36,.6,BS(new THREE.Color(n[1])),x0-.1,19,z-34);mk(.4,36,.6,BS(new THREE.Color(n[1])),x0-.1,19,z+34);
   sign(n[0],n[1],40,9,x0-.3,31,z,-Math.PI/2);mk(14,.8,14,MS(0x1a1a22,.4,.6),x0-7,7,z);mk(.7,7,.7,MS(0xd4a017,.3,.9),x0-13,3.5,z-6.5);mk(.7,7,.7,MS(0xd4a017,.3,.9),x0-13,3.5,z+6.5);
   mk(.5,5.5,8,BS(0xffd890),x0-.1,2.8,z);flat(12,8,0xaa0f2a,x0-6,.1,z);flat(12,28,0x2b2d33,x0-6,.05,z);for(let i=-3;i<=3;i++)mk(.8,.8,.8,BS(0xffd24a),x0-12,.6,z+i*2.2);
   solid(x0,x1,z-35,z+35,38);G.xdoors.push({x:x0-4,z,n:n[0]});G.xs.push({x:x0-4,z,r:5,t:()=>{const c=G.xc;return(c&&c.k==='rob'&&c.door===k)?Lg('Press E — ROB '+n[0],'E — سرقت از '+n[0]):Lg('Press E — enter '+n[0],'E — ورود به '+n[0])},fn:()=>{const c=G.xc;if(c&&c.k==='rob'&&c.door===k){G.cash(c.rw);G.big(Lg('HEIST COMPLETE','سرقت موفق'),'$ '+c.rw.toLocaleString(),'#ffd24a',3);G.addWanted(3);G.xc=null;return}G.xback={x:x0-5,z};G.xtp(2100,9,Math.PI,'cas')}})});
  // SKY NEEDLE (north-west)
  {const m=MS(0xcfd6de,.3,.6),x=-660,z=-560;mk(7,160,7,m,x,80,z);const d=mk(30,5,30,MS(0x2de2ff,.3,.4),x,150,z);d.material.emissive=new THREE.Color(0x0b6070);mk(2,35,2,MS(0xaaaaaa),x,178,z);solid(x-3.5,x+3.5,z-3.5,z+3.5,160)}
  // AIRPORTS
  const strip=(x,z0,z1,nm)=>{const len=z1-z0,zc=(z0+z1)/2;flat(26,len,0x2f3238,x,.045,zc);flat(1.2,len,0x2f3238,x,.05,zc);for(let z=z0+15;z<z1-10;z+=24)mk(.8,.04,10,BS(0xf2f2f2),x,.09,z);for(let z=z0+4;z<z1;z+=30){mk(.7,.4,.7,BS(0xffe9a0),x-14,.25,z);mk(.7,.4,.7,BS(0xffe9a0),x+14,.25,z)}
   for(let i=0;i<6;i++){mk(1.4,.04,12,BS(0xffffff),x-9+i*3.6,.09,z0+8);mk(1.4,.04,12,BS(0xffffff),x-9+i*3.6,.09,z1-8)}};
  strip(-700,-580,570);{const x=-650,z=0;flat(40,220,0x3a3d44,x,.04,z);mk(24,16,120,MS(0x9aa6b5,.15,.6),x,8,z);solid(x-12,x+12,z-60,z+60,16);mk(10,32,10,MS(0xcfcfcf,.5),x,16,z+75);mk(12,6,12,MS(0x2a4a6a,.1,.8),x,34,z+75);solid(x-5,x+5,z+70,z+80,34);sign('WEST INTERNATIONAL','#ffffff',50,7,x+12.3,13,z,Math.PI/2)}
  strip(702,40,580);{const x=650,z=310;flat(30,100,0x3a3d44,x,.04,z);mk(16,10,50,MS(0xb9a98a,.7),x,5,z);solid(x-8,x+8,z-25,z+25,10);mk(5,18,5,MS(0xcfcfcf),x,9,z+34);solid(x-2.5,x+2.5,z+31.5,z+36.5,18);sign('EAST AIRFIELD','#ffd24a',30,5,x-8.3,8,z,-Math.PI/2)}
  const put=(k,x,z,h)=>{const a=new Plane(sc,k);a.hx=x;a.hz=z;a.hh=h;a.reset();G.planes.push(a)};
  for(const[hx,hz]of[[-200,-690],[-150,2620]]){const a=new Plane(sc,'Hauler');a.hx=hx;a.hz=hz;a.hh=Math.PI/2;a.reset();a.dro=0;G.planes.push(a);G.xhaulMarker(a)}


  POI.push({x:632,z:-380,c:'#ffd24a',t:'CASINO'},{x:632,z:-250,c:'#ff2d95',t:'CASINO'},{x:632,z:-120,c:'#2de2ff',t:'CASINO'},{x:-650,z:0,c:'#ffffff',t:'AIRPORT'},{x:650,z:310,c:'#ffffff',t:'AIRPORT'});
  G.wp={x:615,z:-250};
  ['RevueltoSV','RevueltoBlack','Ferrari12','JeepCJ','Vario'].forEach((k,i)=>{G.spawnCar(k,622,-310+i*14,Math.PI);G.spawnCar(k,45+i*10,-4.5,Math.PI/2)});
  MAPLBL.push(['WEST INTL AIRPORT',-690,10],['EAST AIRFIELD',700,310],['CASINO STRIP',662,-250],['TWIN TOWERS',675,-515])}
 xex(dt){this.xtwStep(dt);this.aiStep();this.envStep();const W=this.world;if(this.xtm){const e=.12+W.night*1.3;for(const m of this.xtm)m.emissiveIntensity=e}
  for(const c of this.cars){if(!c.rider)continue;if(c.ai&&!c.rider.visible&&c!==this.driving){c.rider.visible=true;c.rs=1}if(!c.rider.visible){c.rs=0;continue}c.rs=Math.min(1,(c.rs||0)+dt*3.2);const u=c.rs*c.rs*(3-2*c.rs);c.rider.position.set(0,.5+(1-u)*.7,-.3-(1-u)*.9);c.rider.scale.setScalar(.85*(.5+.5*u))}}


 xsoft(){if(this.xst)return this.xst;const c=document.createElement('canvas');c.width=c.height=128;const g=c.getContext('2d');for(const[x,y,r]of[[64,64,50],[40,70,34],[90,66,36],[62,44,32],[66,86,30]]){const q=g.createRadialGradient(x,y,0,x,y,r);q.addColorStop(0,'rgba(255,255,255,.55)');q.addColorStop(1,'rgba(255,255,255,0)');g.fillStyle=q;g.fillRect(0,0,128,128)}return this.xst=new THREE.CanvasTexture(c)}

 xtwInit(){const TW=this.xtw,sc=this.scene,tx=this.xsoft();TW.dust=[];for(let i=0;i<180;i++){const s=new THREE.Sprite(new THREE.SpriteMaterial({map:tx,color:0xbab4aa,transparent:true,opacity:0,depthWrite:false}));s.visible=false;s.userData={l:0,L:1,vx:0,vy:0,vz:0,s0:10,s1:30};sc.add(s);TW.dust.push(s)}TW.di=0;
  const N=160,im=new THREE.InstancedMesh(new THREE.BoxGeometry(1,1,1),new THREE.MeshStandardMaterial({color:0x6a6e75,roughness:.9}),N),z=new THREE.Object3D();im.instanceMatrix.setUsage(THREE.DynamicDrawUsage);im.frustumCulled=false;z.scale.set(0,0,0);z.updateMatrix();TW.deb=[];for(let i=0;i<N;i++){im.setMatrixAt(i,z.matrix);TW.deb.push({l:0,x:0,y:0,z:0,vx:0,vy:0,vz:0,s:1,rx:0,ry:0,rz:0,wx:0,wy:0,wz:0})}sc.add(im);TW.im=im;TW.dn=0;
  const rm=new THREE.MeshStandardMaterial({color:0x4b4e54,roughness:.95});for(const T of TW.tw){const r=new THREE.Group();r.position.set(T.x,0,T.z);for(let i=0;i<14;i++){const w=4+Math.random()*9,h=2+Math.random()*5,o=new THREE.Mesh(new THREE.BoxGeometry(w,h,w*(.6+Math.random()*.8)),rm);o.position.set((Math.random()-.5)*T.w*.9,h*.4,(Math.random()-.5)*T.w*.9);o.rotation.set((Math.random()-.5)*.5,Math.random()*3,(Math.random()-.5)*.5);o.castShadow=o.receiveShadow=true;r.add(o)}r.visible=false;r.scale.y=.01;sc.add(r);T.rub=r;this.xtwParts(T)}this.xtwFireInit()}


 xtwParts(T){const m0=T.body.material,mk=()=>{const m=m0.clone();m.map=m0.map.clone();m.map.needsUpdate=true;m.emissiveMap=m.map;this.xtm&&this.xtm.push(m);if(typeof ENVM!=='undefined')ENVM.push(m);return m};
  T.lo=new THREE.Mesh(new THREE.BoxGeometry(T.w,1,T.w),mk());T.up=new THREE.Group();T.um=new THREE.Mesh(new THREE.BoxGeometry(T.w,1,T.w),mk());
  for(const o of[T.lo,T.um])o.castShadow=o.receiveShadow=true;T.up.add(T.um);T.g.add(T.lo);T.g.add(T.up);T.lo.visible=T.up.visible=false}
 xtwFireInit(){const TW=this.xtw,tx=this.xsoft();TW.fire=[];for(let i=0;i<80;i++){const s=new THREE.Sprite(new THREE.SpriteMaterial({map:tx,color:0xff8a2a,transparent:true,opacity:0,depthWrite:false,blending:THREE.AdditiveBlending,fog:false}));s.visible=false;s.userData={l:0,L:1,vy:0,s0:6,s1:16};this.scene.add(s);TW.fire.push(s)}TW.fi=0}
 xtwFace(x,z,w){const r=Math.random,f=(r()*4)|0,u=(r()-.5)*w;return f<2?[x+(f?1:-1)*w/2,z+u]:[x+u,z+(f===2?1:-1)*w/2]}
 xtwFire(x,y,z,w,n){const TW=this.xtw;if(!TW.fire)return;for(let i=0;i<n;i++){const s=TW.fire[TW.fi++%TW.fire.length],u=s.userData,q=this.xtwFace(x,z,w);u.L=u.l=.6+Math.random()*.8;u.vy=4+Math.random()*7;u.s0=5+Math.random()*3;u.s1=14+Math.random()*12;s.position.set(q[0],y+(Math.random()-.4)*14,q[1]);s.scale.set(u.s0,u.s0,1);s.material.color.setRGB(1,.55,.15);s.visible=true}}
 xtwSmoke(x,y,z,n,w){const TW=this.xtw,L=TW.dust.length;for(let i=0;i<n;i++){const q=this.xtwFace(x,z,w||30);this.xtwDust(q[0],y,q[1],1,16,56,5,5);TW.dust[(TW.di-1+L)%L].material.color.setRGB(.1,.1,.11)}}

 xtwDeb(x,y,z,n,sp){const TW=this.xtw;for(let i=0;i<n;i++){const d=TW.deb[TW.dn++%TW.deb.length],a=Math.random()*6.283,v=sp*(.4+Math.random());d.l=4+Math.random()*3;d.x=x+(Math.random()-.5)*8;d.y=y;d.z=z+(Math.random()-.5)*8;d.vx=Math.cos(a)*v;d.vz=Math.sin(a)*v;d.vy=Math.random()*sp*.4;d.s=1.2+Math.random()*3.2;d.rx=d.ry=d.rz=Math.random()*3;d.wx=(Math.random()-.5)*6;d.wy=(Math.random()-.5)*6;d.wz=(Math.random()-.5)*6}}

 xtwDust(x,y,z,n,s0,s1,sp,up){const TW=this.xtw,br=.78-.55*this.world.night;for(let i=0;i<n;i++){const s=TW.dust[TW.di++%TW.dust.length],u=s.userData,a=Math.random()*6.283;u.L=u.l=3+Math.random()*2.5;u.s0=s0;u.s1=s1*(.7+Math.random()*.6);u.vx=Math.cos(a)*sp*Math.random();u.vz=Math.sin(a)*sp*Math.random();u.vy=up*(.3+Math.random());s.position.set(x+(Math.random()-.5)*6,y,z+(Math.random()-.5)*6);s.material.color.setRGB(br,br*.97,br*.93);s.visible=true;s.scale.set(s0,s0,1)}}

 xtwHit(T0,y){const TW=this.xtw;if(!TW||TW.on||!TW.im)return;TW.on=true;TW.t=0;const hf0=y>25?U.clamp(y,80,TW.tw[0].h*.85):TW.tw[0].h*.62;for(const T of TW.tw){T.st='fall';T.t=0;T.dl=T===T0?0:1.5;T.go=0;T.e1=T.e2=0;T.hf=hf0;T.fn=-1;T.f3=0}for(const b of TW.br){b.vy=0;b.vx=(Math.random()-.5)*8;b.vz=(Math.random()-.5)*8;b.r=(Math.random()-.5)*3}this.say('TWIN TOWERS COLLAPSING',2600)}

 xtwStep(dt){const TW=this.xtw;if(!TW||!TW.im)return;dt=Math.min(dt||.016,.05);const R0=26,R1=30,D=9;
  if(!TW.on)for(const c of this.cars){if(c.twb){if(c.hit>14&&!c.wreck)this.xtwHit(c.twb);c.twb=null}}
  if(TW.on){TW.t+=dt;
   for(const T of TW.tw){
    if(T.st==='fall'){T.t+=dt;const t=T.t-T.dl;if(t<0)continue;
     const TF=1.8,hf=T.hf||T.h*.62,rn=Math.random;
     if(!T.go){T.go=1;T.f2=0;T.body.visible=false;T.lo.visible=T.up.visible=true;T.lo.scale.set(1,hf,1);T.lo.position.y=hf/2;T.um.scale.set(1,T.h-hf,1);T.um.position.y=(T.h-hf)/2;
      for(const q of[[T.lo,hf,0],[T.um,T.h-hf,hf]]){const m=q[0].material.map;m.repeat.set(T.w/14,q[1]/14);m.offset.set(0,q[2]/14);m.needsUpdate=true}
      T.up.position.set(0,hf,0);T.up.rotation.set(0,0,0);T.up.add(T.cg);T.cg.position.set(0,-hf,0);T.cg.rotation.set(0,0,0);T.cg.visible=true;T.rub.visible=false;
      T.dx=rn()<.5?1:-1;this.xtwFire(T.x,hf,T.z,T.w,24);this.xtwSmoke(T.x,hf,T.z,8,T.w);this.xtwDeb(T.x,hf,T.z,14,22)}
     if(t<TF){const k=t/TF;T.g.position.set(T.x+(rn()-.5)*1.1*k,0,T.z+(rn()-.5)*1.1*k);T.up.rotation.z=-T.dx*.005*Math.sin(t*14)*k;
      if(rn()<dt*45)this.xtwFire(T.x,hf,T.z,T.w,1);if(rn()<dt*24)this.xtwSmoke(T.x,hf+rn()*10,T.z,1,T.w);if(rn()<dt*8)this.xtwDeb(T.x,hf,T.z,1,10)}
     else{
      if(!T.f2){T.f2=1;const bx=T.box;bx.x0=bx.x1=bx.z0=bx.z1=1e7;this.boom(T.x,T.z,24,0);this.xtwDeb(T.x,hf,T.z,44,32);this.xtwDust(T.x,hf,T.z,26,34,110,16,6);T.rub.visible=true;T.fn=-1}
      const s2=t-TF,NF=16,prog=U.clamp(s2/(D-TF),0,1),fr2=prog*NF,fl=Math.min(NF-1,Math.floor(fr2)),snap=U.sm(0,.3,fr2-fl),sy=Math.max(.02,1-(fl+snap)/NF),u=1-sy;
      if(T.fn!==fl){T.fn=fl;const fy=hf*sy;this.xtwDust(T.x,fy+2,T.z,7,26,88,16,3);this.xtwDust(T.x,2,T.z,3,46,155,24,1.2);this.xtwDeb(T.x,fy,T.z,5,16);this.xtwFire(T.x,fy,T.z,T.w,2);this.sfx.beep(96+fl*5)}
      T.g.position.set(T.x+(rn()-.5)*.9*u,0,T.z+(rn()-.5)*.9*u);T.lo.scale.y=hf*sy;T.lo.position.y=hf*sy/2;
      if(T.up.visible){const ang=.05*s2*s2,sh=.6*s2*s2;T.up.rotation.z=-T.dx*ang;T.up.position.set(T.dx*sh,hf*sy,0);
       if(rn()<dt*38)this.xtwDeb(T.x+T.dx*sh,hf*sy,T.z,1,16);if(rn()<dt*28)this.xtwFire(T.x+T.dx*sh*.4,hf*sy,T.z,T.w,1);
       if(s2>4.2){T.up.visible=false;const ux=T.x+T.dx*11,uy=hf*sy;this.xtwDeb(ux,uy,T.z,52,44);this.xtwDust(ux,uy,T.z,26,50,150,20,6);this.xtwDust(ux,4,T.z,16,55,160,24,2.5);this.xtwFire(ux,uy,T.z,T.w,6);this.boom(ux,T.z,18,0)}}
      T.rub.scale.y=Math.min(1,Math.max(.01,u*1.35));
      {const fy=hf*sy;if(rn()<dt*42)this.xtwDust(T.x,fy*(.4+rn()*.6),T.z,1,26,76,10,2.5);if(rn()<dt*24)this.xtwDust(T.x,2,T.z,1,44,140,18,1.5);if(rn()<dt*20)this.xtwDeb(T.x,fy,T.z,1,20);if(rn()<dt*6)this.xtwFire(T.x,fy,T.z,T.w,1)}
      if(prog>=.985&&!T.f3){T.f3=1;this.xtwDust(T.x,2,T.z,20,60,200,34,2);this.xtwDeb(T.x,3,T.z,34,26);this.xtwDust(T.x,hf*.25,T.z,10,50,160,26,3);this.sfx.beep(72)}}
     if(t>=D){T.st='down';T.body.visible=false;T.lo.visible=T.up.visible=false;T.g.add(T.cg);T.cg.position.set(0,0,0);T.cg.rotation.set(0,0,0);T.cg.visible=false;T.g.position.set(T.x,0,T.z);T.g.rotation.set(0,0,0);T.rub.scale.y=1}
    }else if(T.st==='down'){if(TW.t>R0){T.st='rise';T.body.visible=true;T.body.scale.y=.03;T.body.position.y=T.h*.015;T.cg.rotation.z=0;T.cg.position.set(0,T.h*(.03-1),0);T.cg.visible=false}}
    else if(T.st==='rise'){const u=Math.min(1,(TW.t-R0)/(R1-R0)),e=u*u*(3-2*u),sy=Math.max(.03,e);T.body.scale.y=sy;T.body.position.y=T.h*sy/2;T.cg.visible=u>.35;T.cg.position.set(0,T.h*(sy-1),0);T.rub.scale.y=Math.max(.01,1-u*1.2);if(Math.random()<dt*10)this.xtwDust(T.x,2,T.z,1,30,80,12,2);
     if(u>=1){T.st='up';T.go=0;T.t=0;T.body.scale.y=1;T.body.position.y=T.h/2;T.cg.position.set(0,0,0);T.cg.visible=true;T.rub.visible=false;const b=T.box,o=T.o;b.x0=o.x0;b.x1=o.x1;b.z0=o.z0;b.z1=o.z1}}
   }
   for(const b of TW.br){const o=b.o;if(TW.t<.8)continue;if(TW.t<R0){if(o.visible){b.vy-=22*dt;o.position.x+=b.vx*dt;o.position.z+=b.vz*dt;o.position.y+=b.vy*dt;o.rotation.x+=dt*b.r;o.rotation.z+=dt*b.r*.6;if(o.position.y<3){o.visible=false;this.xtwDust(o.position.x,3,o.position.z,6,30,80,12,3);this.xtwDeb(o.position.x,3,o.position.z,6,14)}}}else{o.rotation.set(0,0,0);o.position.set(b.x,b.y,b.z);o.visible=TW.t>R0+(R1-R0)*.7}}
   if(TW.tw.every(T=>T.st==='up')){TW.on=false;TW.t=0;for(const b of TW.br){b.o.visible=true;b.o.rotation.set(0,0,0);b.o.position.set(b.x,b.y,b.z)}}
  }
  if(TW.fire)for(const f of TW.fire){if(!f.visible)continue;const u=f.userData;u.l-=dt;if(u.l<=0){f.visible=false;continue}const k=1-u.l/u.L,z=u.s0+(u.s1-u.s0)*k;f.position.y+=u.vy*dt;f.scale.set(z,z,1);f.material.opacity=.9*(1-k)*Math.min(1,k*6+.2);f.material.color.setRGB(1,.55-.35*k,.15-.1*k)}
  const im=TW.im,Dm=this._o3||(this._o3=new THREE.Object3D());let ch=false;
  for(let i=0;i<TW.deb.length;i++){const d=TW.deb[i];if(d.l<=0)continue;ch=true;d.l-=dt;if(d.y>.5||d.vy>0){d.vy-=26*dt;d.x+=d.vx*dt;d.y+=d.vy*dt;d.z+=d.vz*dt;d.rx+=d.wx*dt;d.ry+=d.wy*dt;d.rz+=d.wz*dt;if(d.y<=.5&&d.vy<0){d.y=.5;d.vy=0;d.vx=d.vz=0;d.wx=d.wy=d.wz=0}}
   Dm.position.set(d.x,d.y,d.z);Dm.rotation.set(d.rx,d.ry,d.rz);Dm.scale.setScalar(d.l<=0?0:d.s*(d.l<1?Math.max(.001,d.l):1));Dm.updateMatrix();im.setMatrixAt(i,Dm.matrix)}
  if(ch)im.instanceMatrix.needsUpdate=true;
  for(const s of TW.dust){if(!s.visible)continue;const u=s.userData;u.l-=dt;if(u.l<=0){s.visible=false;continue}const k=1-u.l/u.L,sz=u.s0+(u.s1-u.s0)*Math.sqrt(k);s.scale.set(sz,sz,1);s.position.x+=u.vx*dt*(1-k);s.position.z+=u.vz*dt*(1-k);s.position.y+=u.vy*dt*(1-k*.6);s.material.opacity=.62*(1-k)*Math.min(1,k*8)}}

 aiStep(){const a=this.flying;let c=this.aic;if(!a||this.state!=='PLAYING'){if(c)c.style.display='none';return}
  if(!c){c=this.aic=document.createElement('canvas');c.width=240;c.height=284;c.style.cssText='position:fixed;left:50%;bottom:calc(10px + env(safe-area-inset-bottom,0px));transform:translateX(-50%);width:min(170px,34vw);height:auto;pointer-events:none;z-index:6;filter:drop-shadow(0 4px 10px rgba(0,0,0,.65))';document.body.appendChild(c)}
  c.style.display='block';const g=c.getContext('2d'),cx=120,cy=120,R=104,K=2.1*57.2958,p=a.p||0,r=a.r||0,inv=Math.cos(p)<0,pe=Math.asin(Math.sin(p)),re=r+(inv?Math.PI:0),PI=Math.PI;
  g.clearRect(0,0,240,284);
  g.save();g.beginPath();g.arc(cx,cy,R,0,PI*2);g.clip();g.translate(cx,cy);g.rotate(re);g.translate(0,pe*K);
  let q=g.createLinearGradient(0,-300,0,0);q.addColorStop(0,'#1a56b0');q.addColorStop(1,'#78bff0');g.fillStyle=q;g.fillRect(-400,-400,800,400);
  q=g.createLinearGradient(0,0,0,300);q.addColorStop(0,'#8a6a3e');q.addColorStop(1,'#33230f');g.fillStyle=q;g.fillRect(-400,0,800,400);
  g.strokeStyle='#fff';g.lineWidth=2.5;g.beginPath();g.moveTo(-400,0);g.lineTo(400,0);g.stroke();
  g.lineWidth=2;g.fillStyle='#fff';g.font='700 14px Rajdhani,sans-serif';g.textAlign='center';g.textBaseline='middle';
  for(let d=-40;d<=40;d+=5){if(!d)continue;const y=-d*2.1,w=d%10?11:24;g.beginPath();g.moveTo(-w,y);g.lineTo(w,y);g.stroke();if(!(d%10)){g.fillText(String(Math.abs(d)),-w-14,y);g.fillText(String(Math.abs(d)),w+14,y)}}
  g.restore();
  g.save();g.translate(cx,cy);g.strokeStyle='#fff';g.lineWidth=2.5;
  for(const d of[-60,-45,-30,-20,-10,10,20,30,45,60]){g.save();g.rotate(d*PI/180);g.beginPath();g.moveTo(0,-R+2);g.lineTo(0,-R+((Math.abs(d)%30===0||Math.abs(d)===45)?15:8));g.stroke();g.restore()}
  g.fillStyle='#ffd24a';g.beginPath();g.moveTo(0,-R+3);g.lineTo(-8,-R-9);g.lineTo(8,-R-9);g.closePath();g.fill();
  g.save();g.rotate(re);g.fillStyle='#fff';g.beginPath();g.moveTo(0,-R+17);g.lineTo(-7,-R+30);g.lineTo(7,-R+30);g.closePath();g.fill();g.restore();
  g.strokeStyle='#ffb020';g.lineWidth=5;g.lineJoin='round';g.beginPath();g.moveTo(-64,0);g.lineTo(-24,0);g.lineTo(-24,11);g.moveTo(64,0);g.lineTo(24,0);g.lineTo(24,11);g.stroke();g.fillStyle='#ffb020';g.fillRect(-4,-4,8,8);
  g.restore();
  g.lineWidth=7;g.strokeStyle='#0b0f14';g.beginPath();g.arc(cx,cy,R+3.5,0,PI*2);g.stroke();g.lineWidth=2;g.strokeStyle='rgba(54,241,255,.85)';g.beginPath();g.arc(cx,cy,R+7,0,PI*2);g.stroke();
  const bk=((re+PI)%(PI*2)+PI*2)%(PI*2)-PI,pd=Math.round(pe*57.2958),bd=Math.round(Math.abs(bk)*57.2958);
  g.fillStyle='rgba(7,13,24,.78)';g.fillRect(8,236,224,44);g.strokeStyle='rgba(54,241,255,.45)';g.lineWidth=1.5;g.strokeRect(8,236,224,44);
  g.fillStyle='#cfeaf0';g.font='700 17px Rajdhani,sans-serif';g.textAlign='center';g.textBaseline='middle';
  g.fillText('ALT '+Math.round(Math.max(0,a.y))+' m   SPD '+Math.round(Math.abs(a.v||0)*3.6)+' km/h',120,250);
  g.fillStyle='#36f1ff';g.fillText('PITCH '+(pd>0?'+':'')+pd+'\u00b0   BANK '+(bd<1?'0':bd+'\u00b0'+(bk>0?' L':' R')),120,269)}

 envStep(){const W=this.world;if(!W||!this.cam)return;const n=W.night,k=.15+.85*(1-n);
  if(Math.abs(k-(this.xek===undefined?-9:this.xek))>.01||ENVM.length!==this.xen){this.xek=k;this.xen=ENVM.length;for(const m of ENVM){const u=m.userData;if(u.eb==null)u.eb=m.envMapIntensity;m.envMapIntensity=u.eb*k}}
  if(!this.xcl){const tx=this.xsoft();this.xcl=[];for(let i=0;i<46;i++){const s=new THREE.Sprite(new THREE.SpriteMaterial({map:tx,transparent:true,opacity:.85,depthWrite:false})),w=280+Math.random()*380;s.scale.set(w,w*(.32+Math.random()*.18),1);s.userData={bx:Math.random()*1800,bz:Math.random()*1800,y:200+Math.random()*280,sp:2+Math.random()*4};this.scene.add(s);this.xcl.push(s)}}
  const cx=this.cam.position.x,cz=this.cam.position.z,t=performance.now()/1000,cr=.07+.93*(1-n),cg=.09+.91*(1-n),cb=.15+.85*(1-n),vis=!this.lau&&(!this.zone||this.zone==='city');
  for(const s of this.xcl){const u=s.userData;s.visible=vis;if(!vis)continue;s.position.set(cx+((u.bx+t*u.sp-cx)%1800+2700)%1800-900,u.y,cz+((u.bz-cz)%1800+2700)%1800-900);s.material.color.setRGB(cr,cg,cb)}}

 xe(){const b=this.xnear;if(b&&b.fn)b.fn()}
  die(a,col,fee){if(this.flying){const f=this.flying;f.alive=false;f.dead=15;f.g.visible=false;this.flying=null}this.ch=null;this.dead=3.5;this.fee=fee;this.big(a,'',col,3.5);if(a==='WASTED')$('gl').classList.add('dead');this.jail=a==='BUSTED'}
  big(a,b,col,sec=3){$('ovl').style.display='block';$('ot').textContent=tr(a);$('ot').style.color=col;$('os').textContent=tr(b);this.bigT=sec}
  revive(){const p=this.player;this.zone='city';this.xj=null;this.xent=null;if(this.xth){this.xth.n.g.visible=false;this.xth=null}this.rig.init=false;this.driving=null;this.flying=null;for(const o of this.cars)if(o.rider)o.rider.visible=false;p.g.visible=true;p.x=20;p.z=10;p.y=0;p.vx=p.vz=0;this.health=100;this.armor=0;this.setWanted(0);this.sfx.radio(0);$('gl').classList.remove('dead');this.cash(-this.fee);if(this.jail){this.jail=0;this.xi&&(this.xin||this.xi());this.xjail();return}this.toast('Discharged from Harbor General. -$'+this.fee)}
  nextMission(){const L=this.world.L,f=this.driving||this.player;let x,z,t=0;do{x=L[Math.floor(this.world.R()*11)];z=L[Math.floor(this.world.R()*11)];t++}while(t<30&&Math.hypot(x-f.x,z-f.z)<350);
   const d=Math.hypot(x-f.x,z-f.z);this.mis={x,z,d,time:d/14+25};this.mk.position.set(x,30,z)}
mkRev(){this.rev={};this.dset=new Set(BINDS.map(b=>b[1]));for(const[n,d]of BINDS)this.rev[KB[d]||d]=d}
 kmap(c){return this.rev[c]||(this.dset.has(c)?'None':c)}
 bindKey(c){const d=this.binding;this.binding=null;if(c!=='Escape'){KB[d]=c;this.mkRev();sv('gtaelfo_k',KB)}this.drawSet()}
 cheatKey(e){if(this.state!=='PLAYING'||e.repeat)return;const ch=e.code==='Space'?'_':/^Key/.test(e.code)?e.code[3].toLowerCase():'';if(!ch)return;this.cb=(this.cb+ch).slice(-40);for(const c of CHEATS)if(this.cb.endsWith(c[0])){this.cb='';c[1](this);this.toast('Cheat: '+c[2]);this.sfx.beep(700);break}}
 applyGfx(){const q=S.q,dp=devicePixelRatio||1,rs=this.rs||1;this.pxBase=q==='low'?1:q==='med'?Math.min(dp,1.25):q==='high'?Math.min(dp,1.35):q==='ultra'?Math.min(dp,1.5):Math.min(dp,2);this.r.setPixelRatio(this.pxBase*rs);this.r.setSize(innerWidth,innerHeight,false);this.world.sun.castShadow=q!=='low';const sh=this.world.sun.shadow,sm=q==='low'?512:q==='med'?1024:q==='high'?1536:2048;if(sh.mapSize.x!==sm){sh.mapSize.set(sm,sm);if(sh.map){sh.map.dispose();sh.map=null;this.r.shadowMap.needsUpdate=true}}$('gl').style.filter='';C.cam.fov=S.fov;C.cam.fovMax=S.fov+15;this.sens=S.sens;this.showFps=S.fps;$('fps').style.display=S.fps?'block':'none';if(this.sfx.mg)this.sfx.mg.gain.value=S.vol}
 applyLang(){document.body.classList.toggle('fa',S.lang==='fa');$('bSet').textContent=tr('Settings');$('bStart').textContent=tr(this.state==='PAUSED'?'Resume GTA_elfo':'Start GTA_elfo');if(this.state==='PAUSED')$('sub').textContent=tr('Paused');else $('sub').textContent=S.lang==='fa'?'GTA_elfo · نسخه v12 آپدیت نوا':'GTA_elfo · v12 NOVA UPDATE';$('build').textContent=S.lang==='fa'?'ساخت v12 · آپدیت نوا':'BUILD v12 · NOVA UPDATE';$('sub2').textContent=S.lang==='fa'?'شهر نوا · ماشین پرنده · جت‌پک · موجودات فضایی · بهینه‌سازی':'Nova City · Flying cars · Jetpack · Aliens · Performance boost'}
 openSet(p){$('set').style.display='flex';$('screen').style.display='none';this.setPage=p||'main';this.drawSet()}
 closeSet(){$('set').style.display='none';$('screen').style.display='flex';sv('gtaelfo_s',S)}
 drawSet(){const G=this,box=document.createElement('div');box.className='sb';const e=$('set');e.innerHTML='';e.appendChild(box);
  const add=(h,fn)=>{const d=document.createElement('div');d.innerHTML=h;const x=d.firstChild;if(fn)fn(x);box.appendChild(x)},
  btn=(l,t,fn)=>add('<div class="r"><span>'+tr(l)+'</span><button></button></div>',x=>{const b=x.lastChild;b.textContent=tr(t);b.onclick=fn}),
  rng=(l,k,mn,mx,st)=>add('<div class="r"><span>'+tr(l)+'</span><input type="range" min="'+mn+'" max="'+mx+'" step="'+st+'" value="'+S[k]+'"></div>',x=>x.lastChild.oninput=ev=>{S[k]=+ev.target.value;G.applyGfx()});
  if(this.setPage==='keys'){add('<h2>'+tr('PC KEYS — click an action, then press the new key')+'</h2>');for(const[n,d]of BINDS)btn(n,this.binding===d?'press a key…':kn(KB[d]||d),()=>{G.binding=d;G.drawSet()});
   btn('Restore defaults','Reset',()=>{for(const k in KB)delete KB[k];G.mkRev();sv('gtaelfo_k',KB);G.drawSet()});btn('','Back',()=>{G.setPage='main';G.drawSet()});return}
  if(this.setPage==='padkeys'){add('<h2>'+tr('GAMEPAD BUTTONS — click an action, then press a button on the pad')+'</h2>');add('<div class="ch" id="padst">'+tr(PAD.gp?'Gamepad connected':'No gamepad detected — press any button on it')+'</div>');
   for(const[n,d]of BINDS){if(['KeyW','KeyS','KeyA','KeyD'].includes(d))continue;btn(n,PAD.pb===d?'press a button…':(GP[d]>=0?GPN[GP[d]]:'—'),()=>{PAD.pb=PAD.pb===d?null:d;G.drawSet()})}
   add('<div class="ch">'+tr('Left stick: move · Right stick: camera · In vehicles RT/LT = gas/brake')+'</div>');btn('Restore defaults','Reset',()=>{for(const k in GP)delete GP[k];Object.assign(GP,GPD);sv('gtaelfo_g',GP);G.drawSet()});btn('','Back',()=>{PAD.pb=null;G.setPage='main';G.drawSet()});return}
  if(this.setPage==='posters'){add('<h2>'+tr('City posters (up to 5, any image size)')+'</h2>');for(let i=0;i<5;i++){add('<div class="r"><span>'+tr('Poster')+' '+(i+1)+'</span><input type="file" accept="image/*" style="max-width:190px"><button>'+tr('Clear')+'</button></div>',x=>{x.children[1].onchange=ev=>G.xfile(i,ev.target.files[0]);x.lastChild.onclick=()=>G.xfile(i,null,1)})}add('<div class="ch">'+tr('Posters appear on billboards along the city roads.')+'</div>');btn('','Back',()=>{G.setPage='main';G.drawSet()});return}
  add('<h2>'+tr('SETTINGS')+'</h2>');btn('City posters','Edit',()=>{G.setPage='posters';G.drawSet()});btn('Control mode',{pc:'PC (default)',mobile:'MOBILE',pad:'GAMEPAD'}[S.mode]||'PC (default)',()=>{S.mode={pc:'mobile',mobile:'pad',pad:'pc'}[S.mode]||'mobile';sv('gtaelfo_s',S);G.showMob();G.drawSet()});
  btn('Controls',{pc:'Edit keys',mobile:'Edit touch layout',pad:'Edit gamepad buttons'}[S.mode]||'Edit keys',()=>{if(S.mode==='pc'){G.setPage='keys';G.drawSet()}else if(S.mode==='pad'){G.setPage='padkeys';G.drawSet()}else G.editMob()});
  btn('Graphics quality',{low:'Low',med:'Medium',high:'High (native pixels)',ultra:'Ultra (1px, supersampled)',insane:'INSANE (4x supersampling)'}[S.q]||'High (native pixels)',()=>{S.q={low:'med',med:'high',high:'ultra',ultra:'insane',insane:'low'}[S.q]||'high';G.applyGfx();G.drawSet()});
  btn('Camera view',S.view==='first'?'First person':'Third person',()=>{S.view=S.view==='first'?'third':'first';sv('gtaelfo_s',S);G.drawSet()});rng('Field of view','fov',60,100,1);rng('Master volume','vol',0,1,.05);rng('Mouse / touch sensitivity','sens',.3,2.5,.1);btn('Show FPS',S.fps?'ON':'OFF',()=>{S.fps=!S.fps;G.applyGfx();G.drawSet()});btn('Language',S.lang==='fa'?'فارسی':'English',()=>{S.lang=S.lang==='fa'?'en':'fa';sv('gtaelfo_s',S);G.applyLang();G.drawSet()});
  btn('Fullscreen',document.fullscreenElement?'ON':'OFF',()=>{const d=document,e=d.documentElement;try{if(d.fullscreenElement)d.exitFullscreen();else{(e.requestFullscreen||e.webkitRequestFullscreen).call(e);try{screen.orientation.lock('landscape').catch(()=>{})}catch(x){}}}catch(x){}setTimeout(()=>G.drawSet(),400)});
  add('<h3>'+tr('Cheat codes (type during play)')+'</h3>');for(const c of CHEATS)add('<div class="ch"><b>'+tr(c[2])+'</b>: '+c[0].replace(/_/g,' (space) ')+'</div>');add('<div class="r"><button>'+tr('Back')+'</button></div>',x=>x.lastChild.onclick=()=>G.closeSet())}
 showMob(){$('mob').style.display=(S.mode==='mobile'&&(this.state==='PLAYING'||this.editing))?'block':'none'}
 mc(id){const d=MB.find(b=>b[0]===id);return MBL[id]||(MBL[id]={x:d[2],y:d[3],s:58,o:75})}
 renderMob(){const m=$('mob');m.innerHTML='';for(const[id,code]of MB){const c=this.mc(id),b=document.createElement('div');b.className='mbt'+(this.editing&&this.mobSel===id?' sel':'');b.textContent=id==='JOY'?'':id;
   if(id==='JOY'){const sz=Math.max(110,c.s*2.3),R=sz/2,kn=document.createElement('div');Object.assign(b.style,{left:c.x+'%',top:c.y+'%',width:sz+'px',height:sz+'px',opacity:c.o/100,borderRadius:'50%',border:'2px solid rgba(255,255,255,.55)',background:'radial-gradient(circle,rgba(255,255,255,.12),rgba(255,255,255,.04))',touchAction:'none'});
    Object.assign(kn.style,{position:'absolute',left:'50%',top:'50%',width:sz*.42+'px',height:sz*.42+'px',marginLeft:-sz*.21+'px',marginTop:-sz*.21+'px',borderRadius:'50%',background:'radial-gradient(circle at 35% 30%,#fff,#9ab 70%)',boxShadow:'0 2px 8px #0008',pointerEvents:'none'});b.appendChild(kn);
    const set=(dx,dy)=>{const k=this.inp.k,t=R*.22;k.KeyW=dy<-t?1:0;k.KeyS=dy>t?1:0;k.KeyA=dx<-t?1:0;k.KeyD=dx>t?1:0},mv=e=>{const r=b.getBoundingClientRect();let dx=e.clientX-(r.left+R),dy=e.clientY-(r.top+R);const l=Math.hypot(dx,dy);if(l>R){dx*=R/l;dy*=R/l}kn.style.transform='translate('+dx+'px,'+dy+'px)';set(dx,dy)};
    b.onpointerdown=e=>{e.preventDefault();b.setPointerCapture(e.pointerId);if(this.editing){this.mobSel=id;this.dr={id,ox:e.clientX,oy:e.clientY,x:c.x,y:c.y};this.drawMed();b.classList.add('sel')}else mv(e)};
    b.onpointermove=e=>{if(this.editing){if(this.dr&&this.dr.id===id){c.x=U.clamp(this.dr.x+(e.clientX-this.dr.ox)/innerWidth*100,2,98);c.y=U.clamp(this.dr.y+(e.clientY-this.dr.oy)/innerHeight*100,2,98);b.style.left=c.x+'%';b.style.top=c.y+'%'}}else if(e.buttons||e.pointerType==='touch')mv(e)};
    b.onpointerup=b.onpointercancel=()=>{this.dr=null;kn.style.transform='translate(0,0)';if(!this.editing)set(0,0)};m.appendChild(b);continue}
   Object.assign(b.style,{left:c.x+'%',top:c.y+'%',width:c.s+'px',height:c.s+'px',opacity:c.o/100,lineHeight:c.s+'px',fontSize:c.s*.28+'px'});
   b.onpointerdown=e=>{e.preventDefault();b.setPointerCapture(e.pointerId);if(this.editing){this.mobSel=id;this.dr={id,ox:e.clientX,oy:e.clientY,x:c.x,y:c.y};this.drawMed();b.classList.add('sel')}else{this.inp.k[code]=1;b.classList.add('on');this.onKey(code)}};
   b.onpointermove=e=>{if(this.editing&&this.dr&&this.dr.id===id){c.x=U.clamp(this.dr.x+(e.clientX-this.dr.ox)/innerWidth*100,2,98);c.y=U.clamp(this.dr.y+(e.clientY-this.dr.oy)/innerHeight*100,2,98);b.style.left=c.x+'%';b.style.top=c.y+'%'}};
   b.onpointerup=b.onpointercancel=()=>{this.dr=null;if(!this.editing){this.inp.k[code]=0;b.classList.remove('on')}};m.appendChild(b)}}
 editMob(){this.editing=true;this.mobSel=MB[0][0];$('set').style.display='none';$('med').style.display='flex';this.showMob();this.renderMob();this.drawMed()}
 drawMed(){const G=this,c=this.mc(this.mobSel),e=$('med');e.innerHTML='<div class="sb"><b>'+this.mobSel+'</b> — '+tr(MB.find(b=>b[0]===this.mobSel)[4])+' · '+tr('drag any button to move it')+'<div class="r"><span>'+tr('Size')+'</span><input id="ms" type="range" min="36" max="140" value="'+c.s+'"></div><div class="r"><span>'+tr('Opacity %')+'</span><input id="mo" type="range" min="10" max="100" value="'+c.o+'"></div><div class="r"><button id="mr">'+tr('Reset layout')+'</button><button id="md">'+tr('Done')+'</button></div><div class="lg">'+MB.map(b=>'<span><b>'+b[0]+'</b> = '+tr(b[4])+'</span>').join('')+'</div></div>';
  $('ms').oninput=ev=>{c.s=+ev.target.value;G.renderMob()};$('mo').oninput=ev=>{c.o=+ev.target.value;G.renderMob()};$('mr').onclick=()=>{for(const k in MBL)delete MBL[k];G.renderMob();G.drawMed()};
  $('md').onclick=()=>{G.editing=false;sv('gtaelfo_m',MBL);$('med').style.display='none';G.showMob();G.renderMob();G.openSet('main')}}
 pay(n){if(this.money<n){this.toast('Not enough cash');return false}this.cash(-n);return true}
 eff(n){const r={...WEAP[n]},a=this.att[n]||{};r.mag=MAG[n];r.rl=RL[n];r.sil=!!a.sil;if(a.long){r.rng*=1.35;r.dmg*=1.1;r.spr*=.7}if(a.short){r.rate*=.8;r.spr*=1.4;r.rng*=.75}if(a.stock)r.spr*=.55;if(a.mag){r.mag=Math.round(r.mag*1.8);r.rl+=.25}return r}
 reload(){const n=this.weaponName;if(!WEAP[n]||this.rl>0||this.driving)return;const e=this.eff(n);if((this.mag[n]||0)>=e.mag||!(this.am[n]>0))return;this.rl=this.rlT=e.rl;this.rlW=n;this.sfx.beep(300)}
 puff(x,y,z){const i=this.si++%60;this.sp[i*3]=x+(Math.random()-.5);this.sp[i*3+1]=y;this.sp[i*3+2]=z+(Math.random()-.5);this.sl[i]=1.2}
 dmgCar(c,n){if(c.wreck||n<=0)return;c.hp-=n;if(c.hp<=0)this.explode(c)}
 boom(x,z,r,dmg){this.sfx.bm&&this.sfx.bm(r);const m=new THREE.Mesh(new THREE.SphereGeometry(1,12,8),new THREE.MeshBasicMaterial({color:0xff9a2a,transparent:true,opacity:.9,blending:THREE.AdditiveBlending,depthWrite:false,fog:false}));m.position.set(x,1.5,z);m.life=.7;m.R=r;this.scene.add(m);this.fx.push(m);this.bl.position.set(x,4,z);this.bl.intensity=8;this.sfx.shot(3);
  for(let i=0;i<14;i++)this.puff(x+(Math.random()-.5)*r,1+Math.random()*3,z+(Math.random()-.5)*r);
  for(const c of this.cars){if(c.wreck)continue;const dx=c.x-x,dz=c.z-z,d=Math.hypot(dx,dz);if(d<r*1.6){const k=1-d/(r*1.6);c.vx+=dx/(d||1)*k*12;c.vz+=dz/(d||1)*k*12;c.stun=2;c.vy=Math.max(c.vy,k*5);this.dmgCar(c,dmg*k)}}
  const p=this.driving||this.player,d=Math.hypot(p.x-x,p.z-z);if(!this.ghost&&d<r*1.4)this.hurt(dmg*(1-d/(r*1.4))*.8);for(const q of this.peds.p)if(q.dead<=0&&Math.hypot(q.x-x,q.z-z)<r*1.5)this.killPed(q,true)}
 explode(c){if(c.wreck)return;c.wreck=true;c.wt=0;c.hp=0;c.ai=null;if(c.rider&&c!==this.driving)c.rider.visible=false;const dr=c===this.driving,tk=c.type==='tank';this.boom(c.x,c.z,tk?10:6,tk?0:55);
  if(c.type==='police')this.policeSpawned=Math.max(0,this.policeSpawned-1);if(tk){this.tankSpawned=false;c.m.scale.set(1,1,1);c.sc0.set(1,1,1)}if(c.type!=='motorcycle')c.type=null;
  c.vy=12;c.y=.05;c.spin=[(Math.random()-.5)*7,(Math.random()-.5)*7];c.body.material.color.setHex(0x151515);c.body.material.emissive.setHex(0);
  if(dr){this.toggleCar();this.player.vy=8;this.player.vx=(Math.random()-.5)*10;this.player.vz=(Math.random()-.5)*10}}
 cops(){const p=this.player,w=this.wanted;while(this.policeSpawned<Math.min(w+1,4))this.spawnPolice();
  if(w>=5&&!this.tankSpawned){const t=new Car(this.scene,0x536b4a,'tank');t.x=p.x-40;t.z=p.z-30;this.cars.push(t);this.tankSpawned=true;this.toast('5 STARS — TANK DEPLOYED!')}
  if(w>=3&&!this.heli){const h=this.heli=new Heli(this.scene);h.x=p.x+80;h.z=p.z+80;this.toast('3 STARS — POLICE HELICOPTER!')}}
 spawnCar(k,x,z,h){const p=this.player,y=this.rig.yaw,mo=!!MOTOS[k],M=mo?MOTOS[k]:CARMODELS[k],c=new Car(this.scene,M.c,mo?'motorcycle':null,k);c.x=x??p.x+Math.sin(y)*6;c.z=z??p.z+Math.cos(y)*6;c.h=h??y;c.rx=c.rz=0;c.spin=null;c.vy=0;c.step(0,0,0,true,false);this.cars.push(c);return c}
 chDone(r){this.cash(r);this.big('CHALLENGE COMPLETE!','$ '+r.toLocaleString(),'#ffd24a');this.sfx.beep(880);this.ch=null}
 fireMsl(){const a=this.flying;if(!a||!a.P.jet||this.weaponCooldown>0)return;this.weaponCooldown=.6;const f=[Math.sin(a.h)*Math.cos(a.p),Math.sin(a.p),Math.cos(a.h)*Math.cos(a.p)],sp=a.v+110,m=new THREE.Mesh(new THREE.CylinderGeometry(.12,.12,1.6,6).rotateX(Math.PI/2),new THREE.MeshBasicMaterial({color:0xffe9a0,fog:false}));
  m.position.set(a.x,a.y+a.gy-.6,a.z);m.vel=[f[0]*sp,f[1]*sp,f[2]*sp];m.t=4;m.lookAt(m.position.x+f[0],m.position.y+f[1],m.position.z+f[2]);this.scene.add(m);this.msls.push(m);this.sfx.msl()}
 tick2(dt){this.xt(dt);const pl=this.player,k=this.dead>0?NOKEY:this.inp.k,car=this.driving||this.flying,W=WEAP[this.weaponName];
  {const tr=this.traffic;tr.t+=dt;const s0=tr.st(0),s1=tr.st(1);if(s0!==this.tl0||s1!==this.tl1){this.tl0=s0;this.tl1=s1;const W2=this.world,cc=[new THREE.Color(0x22ff66),new THREE.Color(0xffc21a),new THREE.Color(0xff2a2a)];for(let i=0;i<W2.tla.length;i++)W2.tlb.setColorAt(i,cc[W2.tla[i]?s1:s0]);W2.tlb.instanceColor.needsUpdate=true}}
  for(let i=0;i<2;i++){const m=this.fl[i],d=this.driving,bk=d&&d.type==='motorcycle';if(d&&d.nb&&!(bk&&i)){m.visible=true;const fl=1+Math.random()*(bk?1.4:.8);m.scale.set(bk?.55:1,bk?.55:1,fl*(bk?1.25:1));m.material.color.setHex(bk?(d.fc||0xffa030):0x66b0ff);const sn=Math.sin(d.h),cs=Math.cos(d.h),o=bk?.28:(i?-.5:.5),bz=bk?2.7:3.3;m.position.set(d.x+cs*o-sn*bz,d.y+(bk?.45:.55),d.z-sn*o-cs*bz);m.rotation.set(d.rx||0,d.h,0)}else m.visible=false}
  {const dl=this.dl,d=this.driving;for(let i=0;i<120;i++)if(dl[i]>0){dl[i]-=dt;this.dp[i*3+1]+=dt*.6;this.dp[i*3]+=(Math.random()-.5)*dt*1.5;if(dl[i]<=0)this.dp[i*3+1]=-100}
   if(false&&d&&d.type==='motorcycle'&&d.y<=.05&&Math.abs(d.sp)>6){const sn=Math.sin(d.h),cs=Math.cos(d.h),n=Math.min(3,1+(Math.abs(d.sp)/14|0))*(d.dust>1.5?2:1)+(d.slip?3:0)+(d.nb?2:0);for(let k=0;k<n;k++){const i=this.di++%120;this.dp[i*3]=d.x-sn*1.0+(Math.random()-.5)*.5;this.dp[i*3+1]=.12+Math.random()*.2;this.dp[i*3+2]=d.z-cs*1.0+(Math.random()-.5)*.5;dl[i]=.5+Math.random()*.5*d.dust}}
   this.dg.attributes.position.needsUpdate=true}
  for(let pi=this.planes.length-1;pi>=0;pi--){const a=this.planes[pi];if(!a.alive){if((a.dead-=dt)<=0){this.scene.remove(a.g);this.planes.splice(pi,1);if(this.nearAir===a)this.nearAir=null}}else a.g.visible=a===this.flying||Math.hypot(a.x-pl.x,a.z-pl.z)<480}
  for(let i=this.msls.length-1;i>=0;i--){const m=this.msls[i];m.t-=dt;m.position.x+=m.vel[0]*dt;m.position.y+=m.vel[1]*dt;m.position.z+=m.vel[2]*dt;this.puff(m.position.x,m.position.y,m.position.z);let hit=m.t<=0||m.position.y<=.6||this.mslHit(m);
   if(!hit)for(const b of this.world.grid.at(m.position.x,m.position.z))if(m.position.x>b.x0&&m.position.x<b.x1&&m.position.z>b.z0&&m.position.z<b.z1&&m.position.y<b.h)hit=true;
   if(!hit)for(const c of this.cars)if(!c.wreck&&Math.hypot(c.x-m.position.x,c.z-m.position.z)<3&&m.position.y<4)hit=true;
   if(hit){this.boom(m.position.x,m.position.z,11,95);this.scene.remove(m);this.msls.splice(i,1)}}
  if(this.punchT>0){this.punchT-=dt;const u=Math.sin((1-Math.max(0,this.punchT)/.3)*Math.PI),a1=this.pf?pl.aR:pl.aL,a2=this.pf?pl.aL:pl.aR;a1.rotation.x=-1.9*u;a2.rotation.x=.7*u;pl.g.rotation.x=.2*u}
  {const ch=this.ch;if(ch&&this.dead<=0){if(ch.type==='kill'){ch.t-=dt;ch.txt='BRAWL \u00b7 KO '+ch.n+'/'+ch.need+' \u00b7 '+Math.max(0,ch.t|0)+'s';if(ch.n>=ch.need)this.chDone(ch.r);else if(ch.t<=0){this.toast('Challenge failed');this.ch=null}}
   else if(ch.type==='heat'){ch.t-=dt;ch.txt='SURVIVE THE HEAT \u00b7 '+Math.max(0,ch.t|0)+'s';if(ch.t<=0){this.setWanted(0);this.chDone(ch.r)}}else ch.txt='TIME ATTACK \u00b7 reach the red marker in time'}}
  for(let i=this.fx.length-1;i>=0;i--){const m=this.fx[i];m.life-=dt;const u=Math.max(0,m.life/.7);m.scale.setScalar(m.R*(1-u*u)+.5);m.material.opacity=u;if(m.life<=0){this.scene.remove(m);this.fx.splice(i,1)}}
  this.bl.intensity=Math.max(0,this.bl.intensity-dt*40);
  for(const c of this.cars){if(c.wreck||c.hp>=45)continue;if(Math.random()<.2)this.puff(c.x,1.3,c.z);c.hp-=(c.hp<20?6:1)*dt;if(c.hp<=0)this.explode(c)}
  if(this.rl>0){if(this.rlW!==this.weaponName||car)this.rl=0;else if((this.rl-=dt)<=0){const n=this.weaponName,e=this.eff(n),t=Math.min(e.mag-(this.mag[n]||0),this.am[n]||0);this.mag[n]=(this.mag[n]||0)+t;this.am[n]-=t;this.sfx.beep(420)}}
  this.aiming=!car&&!!W&&!!k.KeyZ;this.fp=!car&&(S.view==='first'||this.aiming);for(const o of pl.g.children){if(o===pl.flashM||o===pl.magM||o===pl.jetP||o===pl.jetM||Object.values(pl.guns).includes(o))continue;o.visible=!this.fp}const a=this.att[this.weaponName]||{};this.scopeFov=a.scp?(this.weaponName==='Sniper'?12:24):this.weaponName==='Sniper'?30:52;$('scope').style.display=this.aiming&&a.scp?'block':'none';if(this.aiming&&a.scp)for(const o of pl.g.children)o.visible=false;
  const g=pl.armed&&pl.guns[this.weaponName];if(g){g.at.sil.visible=!!a.sil;g.at.scp.visible=!!a.scp;g.at.lng.visible=!!a.long;g.at.stk.visible=!!a.stock;
   const p=this.rl>0?1-this.rl/this.rlT:0,s=this.rl>0?Math.sin(p*Math.PI):0;g.rotation.x=s*.8;g.position.set(-.4,1.6-s*.3,.7-(p>.85?.1*Math.sin((p-.85)/.15*Math.PI):0));pl.aL.rotation.z=-1.1*s;if(s)pl.aL.rotation.x=-1.25*s;
   const mm=pl.magM;mm.visible=this.rl>0&&(p<.3||(p>.55&&p<.88));if(mm.visible){if(p<.3)mm.position.set(-.4,1.4-p/.3*.9,.7);else{const u=(p-.55)/.33;mm.position.set(U.lerp(.15,-.4,u),U.lerp(1,1.4,u),.7)}}}else pl.magM.visible=false;
  const h=this.heli;if(h){h.a+=dt*.5;const f=Math.min(1,dt*1.2);h.x+=(pl.x+Math.cos(h.a)*26-h.x)*f;h.z+=(pl.z+Math.sin(h.a)*26-h.z)*f;h.y=24+Math.sin(this.tt)*2;h.g.position.set(h.x,h.y,h.z);h.g.rotation.set(.08,Math.atan2(pl.x-h.x,pl.z-h.z),0);h.rot.rotation.y+=dt*35;h.tr.rotation.x+=dt*40;h.bc.material.color.setHex(((this.tt*5)|0)%2?0xff2020:0x2060ff);
   h.cd-=dt;if(h.cd<=0&&this.dead<=0&&this.zone==='city'){h.cd=.45;const t=car||pl;this.tracer(h.x,h.y-1,h.z,t.x+(Math.random()-.5)*4,1,t.z+(Math.random()-.5)*4);if(Math.random()<.3)this.hurt(4)}}
  if(this.wanted>0&&(this.polT-=dt)<=0){this.polT=3;this.cops()}}
 initSpace(){const w=this.world,sc=this.scene,ok=(cx,cz)=>{for(let x=cx-34;x<=cx+34;x+=6)for(let z=cz-62;z<=cz+10;z+=6)if(!w.free(x,z,3))return false;return true};let P=null;for(const z of[595,570,545])for(const x of[-690,690,-650,650,-610,610])if(!P&&ok(x,z))P=[x,z];P=P||[-690,595];const cx=P[0],cz=P[1];this.sp0={x:cx,z:cz};
  SHOPS.push({...SHOPDEF.space,id:'space',w:16,d:10,x:cx,z:cz,mz:cz-1.5});this.shipOwn=new Set();this.sh={};this.sit=null;
  const pad=new THREE.Mesh(new THREE.CylinderGeometry(40,40,.2,48),new THREE.MeshStandardMaterial({color:0x23252d,roughness:.9}));pad.position.set(cx,.12,cz-34);pad.scale.set(1,1,.62);pad.receiveShadow=true;sc.add(pad);
  const tw=new THREE.Mesh(new THREE.BoxGeometry(2,26,2),new THREE.MeshStandardMaterial({color:0x8a7fd0,metalness:.7,roughness:.3}));tw.position.set(cx+5,13,cz);sc.add(tw);const bm=new THREE.Mesh(new THREE.CylinderGeometry(1.2,1.2,70,12,1,true),new THREE.MeshBasicMaterial({color:0xb58cff,transparent:true,opacity:.3,blending:THREE.AdditiveBlending,depthWrite:false,fog:false}));bm.position.set(cx+5,60,cz);sc.add(bm);
  for(const k in SHIPS){const S=SHIPS[k],x=cx+(S.i-1)*20,z=cz-34,m=mkShip(k),ring=new THREE.Mesh(new THREE.TorusGeometry(7.5,.25,8,40),new THREE.MeshBasicMaterial({color:0xb58cff,fog:false}));ring.rotation.x=Math.PI/2;ring.position.set(x,.35,z);sc.add(ring);m.position.set(x,.2,z);m.scale.setScalar(.45);sc.add(m);this.sh[k]={m,ring,x,z}}}
 upShip(){for(const k in this.sh){const o=this.sh[k],ow=this.shipOwn.has(k);o.m.scale.setScalar(ow?1:.45);o.ring.material.color.setHex(ow?0x3dff8a:0xb58cff)}}
 spHud(){const pl=this.player;if(this.sky){const S=this.sky,pp=$('prompt');$('obj').textContent='ALT '+Math.max(0,Math.round(S.agl))+' m | FALL '+Math.round(-S.vy*3.6)+' km/h';pp.textContent=S.ch?'':tr('Press SPACE to open the parachute!');pp.style.display=S.ch?'none':'block';return}if(this.lau&&this.lau.walk){const L=this.lau,pp=$('prompt'),d=Math.hypot(pl.x-L.pos.x,pl.z-L.pos.z),na=this.nearAir;$('obj').textContent=tr('NOVA CITY'+(this.jetOwn?'':' · JETPACK: buy at Nova Outfitters (B)'));$('alb').style.display='none';if(this.nearShop){pp.textContent=tr('Press B — '+this.nearShop.name);pp.style.display='block'}else if(d<14){pp.textContent=tr('Press F to board the ship · L: return to Earth');pp.style.display='block'}else if(na&&na.P.hover){pp.textContent=tr('Press F to board '+na.P.name);pp.style.display='block'}else if(this.nearTv){pp.textContent=tr('Press F to board the Nova Hover');pp.style.display='block'}else{pp.textContent='';pp.style.display='none'}return}if(this.lau){const L=this.lau,pp=$('prompt'),land=L.ph==='land'||L.ph==='landed'||L.ph==='crash';$('obj').textContent=land?'ALT '+Math.max(0,Math.round(L.pos.y))+' m | VS '+L.v.y.toFixed(0)+' | HS '+Math.hypot(L.v.x,L.v.z).toFixed(0)+' | FUEL '+Math.round(L.fuel)+' | PAD '+Math.round(Math.hypot(L.pos.x-L.cx,L.pos.z-L.cz))+' m':'ALT '+((L.alt||0)*5/1000).toFixed(1)+' km  |  '+Math.round(L.s*7.2)+' km/h'+(L.ph==='orbit'?'  |  ORBIT':'')+(L.auto?'  |  AUTO':'');$('alb').style.display=L.ph==='land'?'block':'none';$('alb').textContent=tr(L.auto?'AUTO LAND: ON':'AUTO LAND')+' [G]';const tx=L.ph==='orbit'?'Press T: warp to planet NOVA · F: return to Earth':L.ph==='landed'?(L.nova?'Press F: exit the ship · L: return to Earth':'Press F to return to Earth'):'';pp.textContent=tr(tx);pp.style.display=tx?'block':'none';return}for(const k in this.sh){const g=this.sh[k].m.ring;if(g)g.rotation.z=performance.now()/900}let n=null;if(!this.driving&&!this.flying&&!this.sit)for(const k of this.shipOwn){const o=this.sh[k];if(Math.hypot(pl.x-o.x,pl.z-o.z)<11)n=k}this.nsh=n;if(this.sit){$('prompt').textContent=tr('Press L to launch · F to leave the ship');$('prompt').style.display='block'}else if(n&&!this.nearShop){$('prompt').textContent=tr('Press F to board')+' '+SHIPS[n].n;$('prompt').style.display='block'}}
 novaHome(){const L=this.lau,pl=this.player;if(this.flying){this.toast('Land and exit the hover car first (F)');return}if(L.walk){if(Math.hypot(pl.x-L.pos.x,pl.z-L.pos.z)>=14){this.toast('Go back to your ship first');return}L.walk=false;this.sit=L.sk}pl.x=L.o.x;pl.z=L.o.z;pl.y=7;pl.vx=pl.vz=0;pl.g.visible=false;this.lauEnd()}
 spaceF(){const pl=this.player;if(this.driving||this.flying)return false;if(this.sky)return true;if(this.lau){const L=this.lau;if(L.nova&&L.ph==='landed'){if(L.walk){if(Math.hypot(pl.x-L.pos.x,pl.z-L.pos.z)<14){L.walk=false;this.sit=L.sk;pl.g.visible=false;pl.x=L.pos.x;pl.z=L.pos.z;pl.vx=pl.vz=0;this.toast('Back aboard · L: return to Earth');return true}return false}
 if(!this._ec){this._ec=this.cars;this.cars=[]}L.sk=this.sit;L.walk=true;this.sit=null;pl.x=L.pos.x+9;pl.z=L.pos.z;pl.y=.6;pl.vx=pl.vz=0;pl.g.visible=true;this.rig.init=false;this.rig.yaw=-Math.PI/2;this.toast('Nova City · '+(this.jetOwn?'low gravity: jump + hold SPACE to jetpack':'jetpack for sale at Nova Outfitters (B)')+' · F: hover car / ship · L: Earth');return true}this.lauEnd();return true}if(this.sit){const o=this.sh[this.sit];pl.x=o.x;pl.z=o.z-12;pl.y=0;pl.g.visible=true;this.sit=null;this.sfx.beep();return true}if(this.nsh&&!this.driving&&!this.flying){const o=this.sh[this.nsh];this.sit=this.nsh;pl.x=o.x;pl.z=o.z;pl.y=7;pl.vx=pl.vz=0;pl.g.visible=false;this.sfx.beep(700);this.toast('Boarded. Press L to launch.');return true}return false}

 solidPts(x,z,r,self,noCars){let ax=0,az=0;const P=(cx,cz,m)=>{const dx=x-cx,dz=z-cz,d=Math.hypot(dx,dz);if(d<m&&d>1e-4){ax+=dx/d*(m-d);az+=dz/d*(m-d)}};
  if(!noCars)for(const c of this.cars){if(c===self||Math.abs(c.x-x)>7||Math.abs(c.z-z)>7)continue;const sn=Math.sin(c.h),cs=Math.cos(c.h);for(const o of c.ci)P(c.x+sn*o,c.z+cs*o,r+.95)}
  for(const a of this.planes){const e=a.P.span*1.7+12;if(!a.alive||a===this.flying||Math.abs(a.x-x)>e||Math.abs(a.z-z)>e)continue;const y0=self?self.y||0:this.player.y,q=a.push(x,z,r+.05,y0,y0+1.7);if(q){ax+=q[0];az+=q[1]}}
  for(const k in this.sh){const o=this.sh[k];P(o.x,o.z,r+(this.shipOwn.has(k)?2.8:1.6))}
  if(this.hovers)for(const h of this.hovers)if(h.alive&&h!==this.flying&&h.y<3)P(h.x,h.z,r+2.2);
  for(const q of this.world.mt){const dx=x-q[0],dz=z-q[1],rr=q[2]+r;if(dx*dx+dz*dz>rr*rr)continue;const d=Math.sqrt(dx*dx+dz*dz),R0=mtR(q,x,z)*(1-1.5/q[3])+r;if(d<R0&&d>1e-4){ax+=dx/d*(R0-d);az+=dz/d*(R0-d)}}
  return[ax,az]}
 hitObj(p){const w=p.W||(p.W=p.wp()),E=p.P.span*1.4+8;for(const c of this.cars){if(c===this.driving||c.wreck||c.xh===p||Math.abs(c.x-p.x)>E||Math.abs(c.z-p.z)>E)continue;const sn=Math.sin(c.h),cs=Math.cos(c.h);for(const o of c.ci)if(p.hits(c.x+sn*o,(c.y||0)+.9,c.z+cs*o,1.0))return true}
  for(const a of this.planes){if(a===p||!a.alive||Math.hypot(a.x-p.x,a.z-p.z)>(a.P.span+p.P.span)*.9+10)continue;const wa=a.wp();for(let i=0;i<wa.length;i+=3)if(p.hits(wa[i],wa[i+1],wa[i+2],.3))return true}return false}
 mslHit(m){const x=m.position.x,y=m.position.y,z=m.position.z;for(const b of this.world.grid.at(x,z))if(x>b.x0&&x<b.x1&&z>b.z0&&z<b.z1&&y<b.h){if(b.tw)this.xtwHit(b.tw,y);return true}for(const q of this.world.mt)if(mtIn(q,x,z,y))return true;for(const c of this.cars){if(c===this.driving)continue;if(Math.abs(c.x-x)<2.4&&Math.abs(c.z-z)<2.4&&y<3)return true}for(const a of this.planes)if(a.alive&&a!==this.flying&&Math.hypot(a.x-x,a.z-z)<a.P.span*1.6+10&&a.hits(x,y,z,.5))return true;return false}
 say(t,ms){const e=$('lcd');e.textContent=tr(t);e.style.display='block';clearTimeout(this.lt);this.lt=setTimeout(()=>e.style.display='none',ms||1100)}
 emit(x,y,z,vx,vy,vz,l){const i=this.lpI++%400;this.lpP[i*3]=x;this.lpP[i*3+1]=y;this.lpP[i*3+2]=z;this.lpV[i*3]=vx;this.lpV[i*3+1]=vy;this.lpV[i*3+2]=vz;this.lpL[i]=l}
 startLaunch(){const k=this.sit,o=this.sh[k],sc=this.scene;if(!k||this.lau)return;
  if(!this.ea){const cv=document.createElement('canvas');cv.width=1024;cv.height=512;const g=cv.getContext('2d'),R=U.rng(77);g.fillStyle='#10408a';g.fillRect(0,0,1024,512);
   for(let i=0;i<260;i++){const r=14+R()*46;g.fillStyle=['#2f7a3a','#3d8a45','#8a7a4a','#5a8a3a'][i%4];g.beginPath();g.ellipse(R()*1024,60+R()*390,r*1.5,r,R()*3,0,7);g.fill()}
   g.fillStyle='#e8f0f8';g.fillRect(0,0,1024,26);g.fillRect(0,486,1024,26);
   for(let i=0;i<200;i++){g.fillStyle='rgba(255,255,255,'+(.15+R()*.25)+')';g.beginPath();g.ellipse(R()*1024,R()*512,20+R()*60,6+R()*14,R()*3,0,7);g.fill()}
   const tx=this.eaMap=new THREE.CanvasTexture(cv),R0=9000;
   this.ea=new THREE.Mesh(new THREE.SphereGeometry(R0,64,40),new THREE.MeshStandardMaterial({map:tx,emissiveMap:tx,emissive:0xffffff,emissiveIntensity:.3,roughness:1,transparent:true,opacity:0}));
   this.at=new THREE.Mesh(new THREE.SphereGeometry(R0*1.03,48,32),new THREE.MeshBasicMaterial({color:0x5ab4ff,transparent:true,opacity:0,side:THREE.BackSide,blending:THREE.AdditiveBlending,depthWrite:false,fog:false}));
   const sg=new THREE.BufferGeometry(),sp=new Float32Array(9000);for(let i=0;i<3000;i++){const a=R()*6.283,b=Math.acos(2*R()-1);sp[i*3]=150000*Math.sin(b)*Math.cos(a);sp[i*3+1]=150000*Math.cos(b);sp[i*3+2]=150000*Math.sin(b)*Math.sin(a)}sg.setAttribute('position',new THREE.BufferAttribute(sp,3));
   this.st=new THREE.Points(sg,new THREE.PointsMaterial({color:0xffffff,size:2.2,sizeAttenuation:false,transparent:true,opacity:0,fog:false,depthWrite:false}));
   const pg=new THREE.BufferGeometry();this.lpP=new Float32Array(1200).fill(-1e5);pg.setAttribute('position',new THREE.BufferAttribute(this.lpP,3));this.lpV=new Float32Array(1200);this.lpL=new Float32Array(400);this.lpI=0;
   this.lpt=new THREE.Points(pg,new THREE.PointsMaterial({color:0xe6e6e6,size:16,transparent:true,opacity:.42,depthWrite:false,fog:false}));
   for(const m of[this.ea,this.at,this.st,this.lpt]){m.visible=false;m.frustumCulled=false;sc.add(m)}}
  const fm=new THREE.Mesh(new THREE.ConeGeometry(1.5,10,14).rotateX(Math.PI),new THREE.MeshBasicMaterial({color:k==='cruiser'?0x66ccff:0xffa840,transparent:true,opacity:.85,blending:THREE.AdditiveBlending,depthWrite:false,fog:false}));fm.position.y=-5;fm.scale.setScalar(.01);o.m.add(fm);
  this.lauH=sc.children.filter(c=>!c.isLight&&c!==o.m&&c!==this.ea&&c!==this.at&&c!==this.st&&c!==this.lpt&&c!==this.world.dome&&c.visible);
  this.lau={cx:o.x,cz:o.z,v:new THREE.Vector3(),k,o,t:-5,ph:'count',dir:new THREE.Vector3(0,1,0),pos:new THREE.Vector3(o.x,.2,o.z),s:0,fm,sep:0,deb:[],hid:false,f:0,alt:0,n:0,p:0};
  this.cam.near=2;this.cam.far=400000;this.cam.updateProjectionMatrix();this.say('5');this.sfx.beep(600)}
 lauStep(dt){const L=this.lau;if(L.ph==='ending')return;const o=L.o,m=o.m,r=Math.random;L.t+=dt;
  if(L.ph==='warp')this.warpStep(dt);else if(L.ph==='land'||L.ph==='landed'||L.ph==='crash')this.landStep(dt);else if(L.ph==='count'){const n=Math.ceil(-L.t);if(n!==L.n&&n>0){L.n=n;this.say(String(n));this.sfx.beep(500)}L.fm.scale.setScalar(U.sm(-2.2,0,L.t)*.8+.01);
   if(L.t>-2.2)for(let i=0;i<2;i++){const a=r()*6.283;this.emit(o.x+Math.cos(a)*3,1,o.z+Math.sin(a)*3,Math.cos(a)*7,1+r()*2,Math.sin(a)*7,3)}
   if(L.t>=0){L.ph='asc';this.say('LIFTOFF!',1500);this.sfx.beep(900)}}
  else{const t=L.t;L.p=U.sm(5,17,t)*1.15;L.dir.set(0,Math.cos(L.p),Math.sin(L.p));
   if(L.ph==='asc'){L.s=12*t*t;if(t>17.5){L.ph='orbit';this.say('ORBIT ACHIEVED',2500);this.sfx.beep(1100)}}else L.s*=Math.exp(-dt*.5);
   L.pos.addScaledVector(L.dir,L.s*dt);m.position.copy(L.pos);m.rotation.set(L.p,0,0);
   if(L.ph==='asc'){L.fm.scale.set(1+.15*r(),.9+.4*r(),1+.15*r());if(t>5.5&&!L.mq){L.mq=1;this.say('MAX-Q',1200)}
    if(!L.sep&&t>(L.k==='shuttle'?8:11)&&L.k!=='cruiser'){L.sep=t;this.say('STAGE SEPARATION',1800);const parts=m.bs||m.es||[];m.updateMatrixWorld(true);for(const q of parts){this.scene.attach(q);L.deb.push({m:q,v:new THREE.Vector3((r()-.5)*8,(r()-.3)*3,(r()-.5)*8).addScaledVector(L.dir,L.s*.9),w:(r()-.5)*3})}}
    for(let i=0;i<2;i++)this.emit(L.pos.x-L.dir.x*5+(r()-.5)*2,L.pos.y-L.dir.y*5,L.pos.z-L.dir.z*5+(r()-.5)*2,(r()-.5)*3,(r()-.5)*3,(r()-.5)*3,2.5)}
   else{L.fm.scale.multiplyScalar(Math.exp(-dt*2));L.fm.visible=L.fm.scale.x>.05}
   if(m.ring)m.ring.rotation.z+=dt*(2+(L.ph==='asc'?t:0))}
  for(let i=L.deb.length-1;i>=0;i--){const d=L.deb[i];d.m.position.addScaledVector(d.v,dt);d.v.multiplyScalar(Math.exp(-dt*.6));d.m.rotation.x+=d.w*dt;if(L.t>L.sep+9){this.scene.remove(d.m);L.deb.splice(i,1)}}
  for(let i=0;i<400;i++)if(this.lpL[i]>0){this.lpL[i]-=dt;this.lpP[i*3]+=this.lpV[i*3]*dt;this.lpP[i*3+1]+=this.lpV[i*3+1]*dt;this.lpP[i*3+2]+=this.lpV[i*3+2]*dt;if(this.lpL[i]<=0)this.lpP[i*3+1]=-1e5}this.lpt.geometry.attributes.position.needsUpdate=true;
  const p=L.pos,R0=9000;this.ea.position.set(L.cx,-R0,L.cz);this.at.position.copy(this.ea.position);this.ea.rotation.y+=dt*.03;
  const alt=Math.hypot(p.x-L.cx,p.y+R0,p.z-L.cz)-R0;L.alt=alt;const ea=U.sm(600,2600,alt);this.ea.visible=this.at.visible=ea>.01;this.ea.material.opacity=ea;this.at.material.opacity=.35*ea;L.f=U.sm(500,6000,alt);this.st.visible=L.f>.05;this.st.material.opacity=U.sm(500,5000,alt);
  if(!L.hid&&alt>2700){L.hid=1;for(const c of this.lauH)c.visible=false}
  this.bl.position.set(p.x,p.y-3,p.z);this.bl.intensity=L.ph==='count'?U.sm(-2,0,L.t)*6:Math.max(0,6-L.t)}
 lauSky(){if(!this.lau)return;const L=this.lau,f=L.f||0,w=this.world,B=this.blk=this.blk||new THREE.Color(0);if(L.nova){w.sky.setHex(0x8a64c8);w.du.top.value.setHex(0x3a2a9a);w.du.hor.value.setHex(0xb08ae8)}w.sky.lerp(B,f);this.scene.fog.color.copy(w.sky);w.du.top.value.lerp(B,f);w.du.hor.value.lerp(B,f);w.du.nt.value=Math.max(w.du.nt.value,f);w.dome.visible=f<.97}
 lauCam(dt){const L=this.lau,c=this.cam,p=L.o.m.position,r=this.rig,t=L.t;
  if(L.ph==='count'){const sh=U.sm(-3,0,t)*.4;c.position.set(L.o.x+26+(Math.random()-.5)*sh,10+(Math.random()-.5)*sh,L.o.z-52);c.lookAt(L.o.x,15,L.o.z)}
  else{if(r.idle>3&&L.ph==='orbit')r.yaw+=dt*.08;const d=(L.ph==='land'||L.ph==='landed')?58:75+Math.min(60,Math.max(0,t)*4),cp=Math.cos(r.pit),sh=L.ph==='asc'?.5*(1-U.sm(2,8,t)):0;
   c.position.set(p.x-Math.sin(r.yaw)*cp*d+(Math.random()-.5)*sh,p.y+Math.sin(r.pit)*d+4+(Math.random()-.5)*sh,p.z-Math.cos(r.yaw)*cp*d);c.lookAt(p.x+L.dir.x*10,p.y+L.dir.y*10,p.z+L.dir.z*10)}if(c.position.y<2)c.position.y=2}
 lauEnd(){const L=this.lau,S=this,f=$('fade');if(!L||!['orbit','landed','crash'].includes(L.ph))return;L.ph='ending';f.style.opacity=1;
  setTimeout(()=>{for(const c of S.lauH)c.visible=true;for(const d of L.deb)S.scene.remove(d.m);S.scene.remove(L.o.m);const m=mkShip(L.k);m.position.set(L.o.x,.2,L.o.z);S.scene.add(m);L.o.m=m;for(const x of[S.ea,S.at,S.st,S.lpt])x.visible=false;S.lpP.fill(-1e5);S.lpL.fill(0);
   $('alb').style.display='none';if(S.nv)S.nv.visible=false;S.ea.material.map=S.eaMap;S.ea.material.emissiveMap=S.eaMap;S.ea.material.needsUpdate=true;S.at.material.color.setHex(0x5ab4ff);S.cam.fov=70;S.cam.near=.5;S.cam.far=900;S.cam.updateProjectionMatrix();S.world.dome.visible=true;S.bl.intensity=0;S.player.g.visible=false;S.player.jetM.visible=false;S.player.jetP.visible=false;if(S._ec){S.cars=S._ec;S._ec=null}S.lau=null;S.rig.init=false;f.style.opacity=0;S.toast('Back on Earth')},1100)}

 warp(){const L=this.lau;if(!L||L.ph!=='orbit')return;this.buildNova();L.ph='warp';L.wt=0;L.fm.visible=true;L.fm.scale.set(1,1,1);this.say('WARP DRIVE',1500);this.sfx.beep(300)}
 warpStep(dt){const L=this.lau,t=(L.wt+=dt),r=Math.random,f=$('fade');this.cam.fov=70+50*U.sm(0,2.5,t)*(1-U.sm(3.8,4.4,t));this.cam.updateProjectionMatrix();
  this.st.rotation.y+=dt*(.5+t*.6);L.fm.visible=true;L.fm.scale.set(1.1,1.6+r()*.6,1.1);L.cz-=t*t*8000*dt;
  if(t>3.2&&!L.w1){L.w1=1;f.style.background='#fff';f.style.opacity=1}
  if(t>4.2&&!L.w2){L.w2=1;this.toNova()}}
 toNova(){const L=this.lau,f=$('fade'),NX=30000,NZ=0;this.nv.visible=true;this.ea.material.map=this.novaMap;this.ea.material.emissiveMap=this.novaMap;this.ea.material.needsUpdate=true;this.at.material.color.setHex(0xa88aff);
  L.cx=NX;L.cz=NZ;L.nova=1;L.pos.set(NX+280,4200,NZ-320);L.v.set(-5,-45,5);L.a=L.b=0;L.fuel=SHIPST[L.k].fuel;L.dir.set(0,1,0);L.p=0;L.ph='land';L.fm.scale.setScalar(.01);L.o.m.rotation.set(0,0,0);
  this.rig.pit=.25;this.rig.yaw=0;$('alb').onclick=()=>{this.autoLand();$('alb').blur()};this.cam.fov=70;this.cam.near=.5;this.cam.far=12000;this.cam.updateProjectionMatrix();f.style.opacity=0;setTimeout(()=>{f.style.background='#000'},1200);this.say('APPROACHING NOVA',2500);this.toast('Shift: thrust · Space: hover · W/A/S/D: tilt · land softly on the glowing pad')}
 landStep(dt){const L=this.lau,k=this.inp.k,m=L.o.m,S=SHIPST[L.k],g=8,r=Math.random;for(const t of this.nvR||[]){t.rotation.y+=dt*.5;t.rotation.x+=dt*.2}if(this.nvT&&this.nv&&this.nv.visible)this.nvT(dt);
  if(L.ph!=='land')return;
  const yw=this.rig.yaw,fx=Math.sin(yw),fz=Math.cos(yw),iz=(k.KeyW?1:0)-(k.KeyS?1:0),ix=(k.KeyD?1:0)-(k.KeyA?1:0);let dx=fx*iz-fz*ix,dz=fz*iz+fx*ix;const e=Math.min(1,S.rcs*dt*1.6);let auV=null;
  if(L.auto){const ex=L.cx-L.pos.x,ez=L.cz-L.pos.z,dd=Math.hypot(ex,ez),alt=Math.max(0,L.pos.y);let sp=Math.min(45,Math.sqrt(5*dd)),vx=0,vz=0;if(alt<40){sp=Math.min(sp,Math.max(0,dd*.12));}if(dd>1e-3){vx=ex/dd*sp;vz=ez/dd*sp}
   const ax=U.clamp((vx-L.v.x)*1,-3.4,3.4),az=U.clamp((vz-L.v.z)*1,-3.4,3.4);dx=Math.atan2(ax,g)/.5;dz=Math.atan2(az,g)/.5;
   let vd;if(dd>140){vd=alt>360?-Math.sqrt(10*(alt-360)):Math.min(25,(360-alt)*.4)}else{const s=U.clamp(1.2-dd/(alt*.8+25),.15,1);vd=-(.8+Math.sqrt(6*alt))*s}auV=U.clamp(vd,-80,25)}
  L.a=U.lerp(L.a,U.clamp(dz,-1,1)*.5,e);L.b=U.lerp(L.b,U.clamp(dx,-1,1)*.5,e);
  const tilt=Math.hypot(L.a,L.b),cs=Math.cos(L.a)*Math.cos(L.b);let th=0;
  if(L.fuel>0){if(auV!==null)th=U.clamp((g+U.clamp((auV-L.v.y)*2.2,-6,14))/(S.thr*Math.max(.3,cs)),0,1);else if(k.ShiftLeft||k.ShiftRight)th=1;else if(k.Space)th=Math.min(1,g/(S.thr*Math.max(.3,cs)))}
  L.fuel=Math.max(0,L.fuel-th*dt*S.burn);const T=S.thr*th;
  L.v.x+=T*Math.sin(L.b)*dt;L.v.z+=T*Math.sin(L.a)*dt;L.v.y+=(T*cs-g)*dt;const dh=Math.exp(-dt*.12);L.v.x*=dh;L.v.z*=dh;L.pos.addScaledVector(L.v,dt);
  m.position.copy(L.pos);m.rotation.set(L.a,0,-L.b);L.fm.visible=th>.02;L.fm.scale.set(1,th*1.2+.3+r()*.25,1);
  if(th>.02)for(let i=0;i<2;i++)this.emit(L.pos.x-Math.sin(L.b)*5+(r()-.5)*2,L.pos.y-4.5,L.pos.z-Math.sin(L.a)*5+(r()-.5)*2,(r()-.5)*4,-6*th-2,(r()-.5)*4,1.1);
  const px=L.pos.x,pz=L.pos.z;let hit=false;for(const b of this.world.grid.at(px,pz))if(b.h>.9&&px>b.x0-2&&px<b.x1+2&&pz>b.z0-2&&pz<b.z1+2&&L.pos.y<b.h+2)hit=true;
  const vs=-L.v.y,hs=Math.hypot(L.v.x,L.v.z),d=Math.min(...(this.nvP&&L.nova?this.nvP:[[L.cx,L.cz]]).map(q=>Math.hypot(px-q[0],pz-q[1])));
  if(hit||L.pos.y<=.5){const ok=!hit&&vs<7&&hs<5&&tilt<.3;
   if(ok){L.pos.y=.5;L.v.set(0,0,0);L.a=L.b=0;m.position.copy(L.pos);m.rotation.set(0,0,0);L.fm.visible=false;L.ph='landed';this.sfx.beep(1000);
    if(d<=PADR){const pr=1-d/PADR,rw=Math.round((10000+40000*pr*pr+L.fuel*50)*(L.auto?.4:1));this.cash(rw);this.big(L.auto?'AUTO LANDING':pr>.8?'PERFECT LANDING':'LANDING COMPLETE','$ '+rw.toLocaleString()+' · '+(Math.round(d*10)/10)+' m from center','#36f1ff')}else this.toast('Landed off the pad — no bonus')}
   else{L.ph='crash';this.boom(px,pz,14,0);m.visible=false;L.fm.visible=false;this.say('CRASHED',2500);setTimeout(()=>{if(this.lau===L)this.lauEnd()},3200)}}}
 buildNova(){if(this.nv)return;const sc=this.scene,NX=30000,NZ=0,g=this.nv=new THREE.Group(),R=U.rng(2024);this.nvX=NX;this.nvZ=NZ;
  {const cv=document.createElement('canvas');cv.width=1024;cv.height=512;const c=cv.getContext('2d');c.fillStyle='#0b4a78';c.fillRect(0,0,1024,512);for(let i=0;i<240;i++){const r=14+R()*46;c.fillStyle=['#5a3a9a','#2a9a8a','#7a4aa8','#3aaa9a'][i%4];c.beginPath();c.ellipse(R()*1024,50+R()*410,r*1.5,r,R()*3,0,7);c.fill()}
   c.fillStyle='#ffe9a8';for(let i=0;i<1500;i++)c.fillRect(R()*1024,50+R()*410,1.6,1.6);c.fillStyle='rgba(255,210,240,.25)';for(let i=0;i<160;i++){c.beginPath();c.ellipse(R()*1024,R()*512,20+R()*60,6+R()*14,R()*3,0,7);c.fill()}this.novaMap=new THREE.CanvasTexture(cv)}
  const gc=document.createElement('canvas');gc.width=gc.height=256;{const c=gc.getContext('2d'),R2=U.rng(909);c.fillStyle='#2b2e34';c.fillRect(0,0,256,256);
   for(let i=0;i<2400;i++){c.fillStyle=i%3?'rgba(48,51,58,.55)':'rgba(66,70,80,.5)';c.fillRect(R2()*256,R2()*256,2,2)}
   c.strokeStyle='#383c44';c.lineWidth=4;c.strokeRect(2,2,252,252);c.strokeStyle='#34373e';c.lineWidth=2;c.beginPath();c.moveTo(128,0);c.lineTo(128,256);c.moveTo(0,128);c.lineTo(256,128);c.stroke()}
  const gt=new THREE.CanvasTexture(gc);gt.wrapS=gt.wrapT=THREE.RepeatWrapping;gt.repeat.set(40,40);gt.anisotropy=4;
  const gr=new THREE.Mesh(new THREE.PlaneGeometry(6000,6000).rotateX(-Math.PI/2),new THREE.MeshStandardMaterial({map:gt,color:0xd2d5da,roughness:.96,metalness:.02}));gr.position.set(NX,0,NZ);g.add(gr);
  const PT=150,K=9,RG=1560,rw=i=>i%3?18:44,O=new THREE.Object3D(),cl=new THREE.Color(),PAD=[[0,0],[525,525],[-525,525],[525,-525],[-525,-525]];this.nvP=PAD.map(p=>[NX+p[0],NZ+p[1]]);
  const mi=(geo,mat,n)=>{const m=new THREE.InstancedMesh(geo,mat,Math.max(1,n));m.frustumCulled=false;g.add(m);return m},bx1=()=>new THREE.BoxGeometry(1,1,1),
   st=(m,i,x,y,z,sx,sy,sz,ry,col)=>{O.position.set(NX+x,y,NZ+z);O.scale.set(sx,sy,sz);O.rotation.set(0,ry||0,0);O.updateMatrix();m.setMatrixAt(i,O.matrix);if(col!=null)m.setColorAt(i,cl.set(col))},
   addB=(x0,x1,z0,z1,h)=>{const b={x0:NX+x0,x1:NX+x1,z0:NZ+z0,z1:NZ+z1,h};this.world.boxes.push(b);this.world.grid.add(b)};
  const RS=[];for(let i=-K;i<=K;i++)RS.push([0,i*PT,rw(i)],[1,i*PT,rw(i)]);RS.push([0,RG,40],[0,-RG,40],[1,RG,40],[1,-RG,40]);
  const LEN=RG*2+40,ro=mi(bx1(),new THREE.MeshStandardMaterial({color:0x15181d,roughness:.97,metalness:.02}),RS.length);RS.forEach((r,i)=>r[0]?st(ro,i,0,.06,r[1],LEN,.12,r[2]):st(ro,i,r[1],.06,0,r[2],.12,LEN));
  const ed=mi(bx1(),new THREE.MeshBasicMaterial({color:0x9aa3b2}),RS.length*2);let ei=0;
  RS.forEach(r=>{if(r[0]){st(ed,ei++,r[1]-r[2]/2+1.2,.135,0,.32,.04,LEN);st(ed,ei++,r[1]+r[2]/2-1.2,.135,0,.32,.04,LEN)}else{st(ed,ei++,0,.135,r[1]-r[2]/2+1.2,LEN,.04,.32);st(ed,ei++,0,.135,r[1]+r[2]/2-1.2,LEN,.04,.32)}});
  const DL=[];for(const r of RS)for(const o of(r[2]>20?[-r[2]/4,r[2]/4]:[0]))DL.push([r[0],r[1],o,r[2]>20?0xe8f4ff:0xffd860]);
  const nd=Math.floor(LEN/24),dm=mi(bx1(),new THREE.MeshBasicMaterial({color:0xffffff}),DL.length*nd);let q=0;
  for(const[a,c,o,col]of DL)for(let s=0;s<nd;s++){const t=-RG+s*24;a?st(dm,q++,t,.13,c+o,7,.03,.5,0,col):st(dm,q++,c+o,.13,t,.5,.03,7,0,col)}
  const MS=[];for(let i=-K;i<=K;i+=3)for(let a=-3;a<3;a++){const c=(a+.5)*450;MS.push([0,i*PT,c],[1,i*PT,c])}
  const md=mi(bx1(),new THREE.MeshStandardMaterial({color:0x2a6a3a,roughness:.9}),MS.length),lp=mi(bx1(),new THREE.MeshStandardMaterial({color:0x8a94a8}),MS.length*8),lh=mi(bx1(),new THREE.MeshBasicMaterial({color:0x36f1ff}),MS.length*8);q=0;
  MS.forEach(([a,c,t],i)=>{a?st(md,i,t,.3,c,360,.5,6):st(md,i,c,.3,t,6,.5,360);for(let k=0;k<8;k++){const u=t-157+k*45;a?(st(lp,q,u,5,c,.5,10,.5),st(lh,q,u,10.2,c,.9,.4,3)):(st(lp,q,c,5,u,.5,10,.5),st(lh,q,c,10.2,u,3,.4,.9));q++}});
  const RB=[];for(let a=-3;a<=3;a++)for(let b=-3;b<=3;b++)if(a||b)RB.push([a*450,b*450]);
  const ra=mi(new THREE.CylinderGeometry(47,47,.08,36),new THREE.MeshStandardMaterial({color:0x23262c,roughness:.95}),RB.length),rr=mi(new THREE.RingGeometry(15,32,40).rotateX(-Math.PI/2),new THREE.MeshStandardMaterial({color:0x3b3f47,roughness:.95}),RB.length),ri=mi(new THREE.CylinderGeometry(15,15,.6,28),new THREE.MeshStandardMaterial({color:0x2a7a45,roughness:.95}),RB.length),rn=mi(new THREE.TorusGeometry(15.4,.3,6,36).rotateX(Math.PI/2),new THREE.MeshBasicMaterial({color:0xff3dd8}),RB.length),rs=mi(new THREE.ConeGeometry(2.4,38,6).translate(0,19,0),new THREE.MeshStandardMaterial({color:0xcfd8ff,emissive:0x36f1ff,emissiveIntensity:.8,metalness:.8,roughness:.2}),RB.length);
  RB.forEach(([x,z],i)=>{st(ra,i,x,.04,z,1,1,1);st(rr,i,x,.2,z,1,1,1);st(ri,i,x,.3,z,1,1,1);st(rn,i,x,.65,z,1,1,1);st(rs,i,x,.6,z,1,1,1);addB(x-15,x+15,z-15,z+15,.6);addB(x-2.6,x+2.6,z-2.6,z+2.6,38)});
  const TW=[],PK=[],SD=[];
  for(let i=-K;i<K;i++)for(let j=-K;j<K;j++){const x0=i*PT+rw(i)/2+6,x1=(i+1)*PT-rw(i+1)/2-6,z0=j*PT+rw(j)/2+6,z1=(j+1)*PT-rw(j+1)/2-6,cx=(x0+x1)/2,cz=(z0+z1)/2,ds=Math.hypot(cx,cz);
   if(Math.abs(cx)<100&&Math.abs(cz)<100)continue;if(PAD.some(p=>p[0]&&Math.hypot(cx-p[0],cz-p[1])<75))continue;
   if((i===-4&&j===1)||(i===4&&j===-3)){SD.push([cx,cz]);continue}const r=R();if(r<.13){PK.push([x0,x1,z0,z1]);continue}
   const nx=r<.5?1:2,nz=R()<.5?1:2,cw=(x1-x0)/nx,cd=(z1-z0)/nz;
   for(let a=0;a<nx;a++)for(let b=0;b<nz;b++){const w=cw*(.5+.38*R()),d=cd*(.5+.38*R()),x=x0+cw*(a+.5),z=z0+cd*(b+.5),h=20+R()*R()*(130+120*Math.exp(-ds/600));TW.push([x,z,w,d,h]);addB(x-w/2,x+w/2,z-d/2,z+d/2,h)}}
  const bm=mi(new THREE.BoxGeometry(1,1,1).translate(0,.5,0),new THREE.MeshStandardMaterial({color:0xffffff,metalness:.6,roughness:.25,emissive:0x1a5aff,emissiveIntensity:.3}),TW.length),tm=mi(bx1(),new THREE.MeshBasicMaterial({color:0xffffff}),TW.length);
  TW.forEach(([x,z,w,d,h],i)=>{st(bm,i,x,0,z,w,h,d,0,cl.setHSL(.55+R()*.2,.45,.28+R()*.15).getHex());st(tm,i,x,h,z,w*1.03,.8,d*1.03,0,cl.setHSL(R()<.5?.5:.88,1,.6).getHex())});
  const pk=mi(bx1(),new THREE.MeshStandardMaterial({color:0x1f7a3a,roughness:.95,emissive:0x06220f}),PK.length),tr=mi(new THREE.ConeGeometry(2.6,8,7).translate(0,4,0),new THREE.MeshStandardMaterial({color:0x2fae55,roughness:.9}),PK.length*14);
  PK.forEach(([x0,x1,z0,z1],i)=>{st(pk,i,(x0+x1)/2,.2,(z0+z1)/2,x1-x0,.3,z1-z0);for(let k=0;k<14;k++){const tx=x0+8+R()*(x1-x0-16),tz=z0+8+R()*(z1-z0-16);st(tr,i*14+k,tx,.3,tz,1,.8+R()*.8,1);addB(tx-1.4,tx+1.4,tz-1.4,tz+1.4,8)}});
  for(const[x,z]of SD){const w=new THREE.Mesh(new THREE.CylinderGeometry(46,38,16,32,1,true),new THREE.MeshStandardMaterial({color:0x8f98a6,metalness:.25,roughness:.82,side:THREE.DoubleSide})),f=new THREE.Mesh(new THREE.CircleGeometry(36,28).rotateX(-Math.PI/2),new THREE.MeshStandardMaterial({color:0x2a7a45,roughness:.95})),t=new THREE.Mesh(new THREE.TorusGeometry(46,.8,6,40).rotateX(Math.PI/2),new THREE.MeshBasicMaterial({color:0xff3dd8}));
   w.position.set(NX+x,8,NZ+z);f.position.set(NX+x,.4,NZ+z);t.position.set(NX+x,16.4,NZ+z);g.add(w,f,t);addB(x-46,x+46,z-46,z+46,16)}
  for(const[px,pz]of PAD.slice(1)){const pd=new THREE.Mesh(new THREE.CylinderGeometry(PADR+4,PADR+4,.5,48),new THREE.MeshStandardMaterial({color:0x2e3239,roughness:.95,metalness:.05}));pd.position.set(NX+px,.25,NZ+pz);g.add(pd);addB(px-PADR-4,px+PADR+4,pz-PADR-4,pz+PADR+4,.5);
   for(const[r,c]of[[PADR,0x36f1ff],[PADR*.62,0xff3dd8],[PADR*.25,0x36f1ff]]){const t=new THREE.Mesh(new THREE.TorusGeometry(r,.4,8,64).rotateX(Math.PI/2),new THREE.MeshBasicMaterial({color:c}));t.position.set(NX+px,.55,NZ+pz);g.add(t)}
   const bc=new THREE.Mesh(new THREE.CylinderGeometry(1.2,1.2,160,12,1,true),new THREE.MeshBasicMaterial({color:0xff3dd8,transparent:true,opacity:.3,blending:THREE.AdditiveBlending,depthWrite:false,fog:false}));bc.position.set(NX+px,80,NZ+pz);g.add(bc)}
  const NC=180,CS=[],
   HVB=merge([{g:new THREE.SphereGeometry(1,10,7).scale(1,.42,2.25).translate(0,.62,0),c:[1,1,1]},
    {g:new THREE.BoxGeometry(1.72,.26,3.5).translate(0,.37,0),c:[.55,.6,.66]},
    {g:new THREE.SphereGeometry(.72,8,6).scale(.82,.52,1.25).translate(0,1.0,-.05),c:[.07,.13,.17]},
    {g:new THREE.BoxGeometry(.34,.24,1.9).translate(-1.02,.52,.1),c:[.62,.67,.73]},
    {g:new THREE.BoxGeometry(.34,.24,1.9).translate(1.02,.52,.1),c:[.62,.67,.73]},
    {g:new THREE.CylinderGeometry(.19,.24,.6,8).rotateX(Math.PI/2).translate(-.62,.55,-1.9),c:[.08,.1,.14]},
    {g:new THREE.CylinderGeometry(.19,.24,.6,8).rotateX(Math.PI/2).translate(.62,.55,-1.9),c:[.08,.1,.14]},
    {g:new THREE.BoxGeometry(.07,.34,.5).translate(-.98,.86,-1.45),c:[.7,.75,.8]},
    {g:new THREE.BoxGeometry(.07,.34,.5).translate(.98,.86,-1.45),c:[.7,.75,.8]}]),
   hvB=mi(HVB,new THREE.MeshStandardMaterial({vertexColors:true,metalness:.6,roughness:.32,emissive:0x0b1520}),NC),
   hvG=mi(new THREE.CircleGeometry(1,16).rotateX(-Math.PI/2).scale(1.3,1,2.35).translate(0,-.62,0),new THREE.MeshBasicMaterial({color:0x36f1ff,transparent:true,opacity:.24,blending:THREE.AdditiveBlending,depthWrite:false,fog:false}),NC),
   hvT=mi(merge([{g:new THREE.BoxGeometry(.55,.14,.1).translate(-.58,.66,-2.18),c:[1,1,1]},{g:new THREE.BoxGeometry(.55,.14,.1).translate(.58,.66,-2.18),c:[1,1,1]}]),new THREE.MeshBasicMaterial({color:0xff3d6e,fog:false}),NC),
   hvH=mi(merge([{g:new THREE.BoxGeometry(.5,.11,.08).translate(-.55,.64,2.18),c:[1,1,1]},{g:new THREE.BoxGeometry(.5,.11,.08).translate(.55,.64,2.18),c:[1,1,1]}]),new THREE.MeshBasicMaterial({color:0xfff1cc,fog:false}),NC);
  for(let n=0;n<NC;n++){const r=RS[Math.floor(R()*RS.length)],dir=R()<.5?1:-1;CS.push({a:r[0],c:r[1]+dir*(r[2]>20?16.5:4.5),dir,s:(R()-.5)*2*RG,v:(r[2]>20?28:16)+R()*24,ph:R()*6.283});const h=R(),cc=cl.setHSL(h<.62?.52+h*.22:h<.85?.88:0,.58,.42+R()*.2),col=cc.getHex();CS[n].col=col;hvB.setColorAt(n,cc)}
  hvB.instanceColor.needsUpdate=true;this.nvCS=CS;this.nvHVB=HVB;this.nvHG=hvG.geometry;this.nvHT=hvT.geometry;this.nvHH=hvH.geometry;
  
  const AP=[[2100,0,1],[-2100,0,1],[0,-2100,0],[0,2100,0]],MAT=(c,e)=>new THREE.MeshStandardMaterial({color:c,roughness:.8,emissive:e||0}),wm=new THREE.MeshBasicMaterial({color:0xf2f2f2}),lm=new THREE.MeshBasicMaterial({color:0xffe9a0});
  AP.forEach(([cx,cz,ax])=>{const T=(u,v)=>ax?[cx+v,cz+u]:[cx+u,cz+v],sl=(W,D,u,v,c)=>{const t=T(u,v),m=new THREE.Mesh(new THREE.BoxGeometry(ax?W:D,.2,ax?D:W),MAT(c));m.position.set(NX+t[0],.1,NZ+t[1]);g.add(m)};
   sl(40,1000,0,0,0x23262e);sl(14,1000,0,-45,0x2e3139);
   const dm=mi(bx1(),wm,32),lt=mi(bx1(),lm,80);for(let i=0;i<32;i++){const t=T(-480+i*30,0);st(dm,i,t[0],.25,t[1],ax?.8:14,.05,ax?14:.8)}
   for(let i=0;i<40;i++)for(let s=0;s<2;s++){const t=T(-490+i*25,s?21:-21);st(lt,i*2+s,t[0],.4,t[1],.6,.5,.6)}
   let t=T(0,-85);const W=ax?[30,18,130]:[130,18,30],tm2=new THREE.Mesh(new THREE.BoxGeometry(...W),new THREE.MeshStandardMaterial({color:0x9aa6b5,roughness:.15,metalness:.6,emissive:0x0a2a4a}));tm2.position.set(NX+t[0],9,NZ+t[1]);g.add(tm2);addB(t[0]-W[0]/2,t[0]+W[0]/2,t[1]-W[2]/2,t[1]+W[2]/2,18);
   t=T(120,-85);const tc=new THREE.Mesh(new THREE.CylinderGeometry(2.6,3.2,40,10),MAT(0xcfcfcf)),tk=new THREE.Mesh(new THREE.CylinderGeometry(6,4,6,10),MAT(0x2a5a7a,0x0a2a3a));tc.position.set(NX+t[0],20,NZ+t[1]);tk.position.set(NX+t[0],43,NZ+t[1]);g.add(tc,tk);addB(t[0]-3,t[0]+3,t[1]-3,t[1]+3,40);
   t=T(300,-150);const pd=new THREE.Mesh(new THREE.CylinderGeometry(42,42,.3,40),MAT(0x23252d));pd.position.set(NX+t[0],.15,NZ+t[1]);g.add(pd);
   ['shuttle','capsule','cruiser'].forEach((k,i)=>{const u=T(300+(i-1)*24,-150),m=mkShip(k),rg=new THREE.Mesh(new THREE.TorusGeometry(8,.3,8,36).rotateX(Math.PI/2),new THREE.MeshBasicMaterial({color:0xb58cff}));m.position.set(NX+u[0],.3,NZ+u[1]);rg.position.set(NX+u[0],.5,NZ+u[1]);g.add(m,rg);addB(u[0]-4,u[0]+4,u[1]-6,u[1]+6,5)});
   const bc=new THREE.Mesh(new THREE.CylinderGeometry(1.2,1.2,120,12,1,true),new THREE.MeshBasicMaterial({color:0xb58cff,transparent:true,opacity:.3,blending:THREE.AdditiveBlending,depthWrite:false,fog:false}));bc.position.set(NX+t[0],60,NZ+t[1]);g.add(bc)});
  this.hovers=[];{const HC=[0x36f1ff,0xff3d8b,0x9dffb0,0xffd24a,0xb58cff,0xf2f2f2],
   HP=[[-16,-52,0],[16,-86,Math.PI],[-16,58,Math.PI],[16,96,0],[-64,16,Math.PI/2],[64,-16,-Math.PI/2],[-124,16,Math.PI/2],[124,-16,-Math.PI/2],[-16,-132,0],[16,140,Math.PI],[-184,-16,-Math.PI/2],[184,16,Math.PI/2],[-16,196,Math.PI],[16,-228,0]];
   HP.forEach(([x,z,h],i)=>{const hv=new Hover(g,NX+x,NZ+z,HC[i%HC.length]);hv.h=h;hv.place();this.hovers.push(hv)})}
  {const AN=54,AO=new THREE.Object3D(),AC=new THREE.Color(),AM=(geo,mat,n)=>{const pc=geo.attributes.position.count;geo.setAttribute('color',new THREE.BufferAttribute(new Float32Array(pc*3).fill(1),3));const m=new THREE.InstancedMesh(geo,mat,n);m.instanceMatrix.setUsage(THREE.DynamicDrawUsage);m.frustumCulled=false;g.add(m);return m},
   ab=AM(new THREE.SphereGeometry(.36,10,8).scale(1,1.45,1).translate(0,1.02,0),new THREE.MeshStandardMaterial({roughness:.6,vertexColors:true}),AN),
   ah=AM(new THREE.SphereGeometry(.42,12,9).scale(1,.92,1.06).translate(0,1.8,0),new THREE.MeshStandardMaterial({roughness:.55,vertexColors:true}),AN),
   ae=AM(new THREE.BoxGeometry(.46,.13,.06).translate(0,1.84,.39),new THREE.MeshBasicMaterial({color:0xd6ff9d,fog:false}),AN),
   aa=AM(new THREE.CylinderGeometry(.02,.03,.42,5).translate(0,2.36,0),new THREE.MeshStandardMaterial({roughness:.6,vertexColors:true}),AN),
   alL=AM(new THREE.BoxGeometry(.16,.62,.18).translate(-.14,.31,0),new THREE.MeshStandardMaterial({color:0x1a2433,roughness:.8}),AN),
   alR=AM(new THREE.BoxGeometry(.16,.62,.18).translate(.14,.31,0),new THREE.MeshStandardMaterial({color:0x1a2433,roughness:.8}),AN),
   PAL=[0x6fda7a,0x4fd8c8,0x9d7bff,0x5fb8ff,0xd6ff6a,0xff9de0],AL=[];
   for(let i=0;i<AN;i++){const w=Math.floor(R()*17)-8,ax=R()<.5,ln=w*150+(Math.abs(w)%3===0?24:11)*(R()<.5?-1:1),dir=R()<.5?1:-1,c=PAL[i%PAL.length];
    AL.push({ax,ln,t:(R()*2-1)*1520,dir,sp:1.1+R()*1.5,h:dir>0?(ax?Math.PI/2:0):(ax?-Math.PI/2:Math.PI),ph:R()*6.283});
    ab.setColorAt(i,AC.set(c));ah.setColorAt(i,AC.set(c).offsetHSL(0,0,.1));aa.setColorAt(i,AC.set(c))}
   ab.instanceColor.needsUpdate=ah.instanceColor.needsUpdate=aa.instanceColor.needsUpdate=true;
   AO.rotation.order='YXZ';this.nvA={list:AL,O:AO,parts:[ab,ah,ae,aa,alL,alR],legL:alL,legR:alR,L1:new THREE.Object3D(),L2:new THREE.Object3D(),ph:0};this.nvA.L1.rotation.order=this.nvA.L2.rotation.order='YXZ'}
  this.nvT=dt=>{CS.forEach((c,n)=>{if(c.taken){st(hvB,n,0,-600,0,0,0,0);st(hvG,n,0,-600,0,0,0,0);st(hvT,n,0,-600,0,0,0,0);st(hvH,n,0,-600,0,0,0,0);return}c.s+=c.dir*c.v*dt;if(c.s>RG)c.s-=2*RG;if(c.s<-RG)c.s+=2*RG;const ry=c.a?(c.dir>0?Math.PI/2:-Math.PI/2):(c.dir>0?0:Math.PI),x=c.a?c.s:c.c,z=c.a?c.c:c.s,y=1.25+Math.sin(c.s*.055+c.ph)*.06;c.wx=NX+x;c.wz=NZ+z;st(hvB,n,x,y,z,1,1,1,ry);st(hvG,n,x,y,z,1,1,1,ry);st(hvT,n,x,y,z,1,1,1,ry);st(hvH,n,x,y,z,1,1,1,ry)});hvB.instanceMatrix.needsUpdate=hvG.instanceMatrix.needsUpdate=hvT.instanceMatrix.needsUpdate=hvH.instanceMatrix.needsUpdate=true;const A=this.nvA;if(A){A.ph+=dt;const O=A.O;for(let i=0;i<A.list.length;i++){const a=A.list[i];a.t+=a.dir*a.sp*dt;if(a.t>1520||a.t<-1520){a.dir*=-1;a.h=a.dir>0?(a.ax?Math.PI/2:0):(a.ax?-Math.PI/2:Math.PI)}const x=a.ax?a.t:a.ln,z=a.ax?a.ln:a.t,wx=this.nvX+x,wz=this.nvZ+z;let gy=0;for(const b of this.world.grid.at(wx,wz))if(b.h<=.9&&wx>b.x0&&wx<b.x1&&wz>b.z0&&wz<b.z1)gy=Math.max(gy,b.h);const ph=A.ph*a.sp*3.2+a.ph;O.position.set(wx,gy+Math.abs(Math.sin(ph))*.06,wz);O.rotation.set(Math.sin(ph)*.04,a.h,Math.sin(ph)*.05);O.updateMatrix();const sw=Math.sin(ph*1.4)*.55,L1=A.L1,L2=A.L2;L1.position.copy(O.position);L1.rotation.set(O.rotation.x+sw,a.h,O.rotation.z);L1.updateMatrix();L2.position.copy(O.position);L2.rotation.set(O.rotation.x-sw,a.h,O.rotation.z);L2.updateMatrix();for(const m of A.parts)m.setMatrixAt(i,m===A.legL?L1.matrix:m===A.legR?L2.matrix:O.matrix)}for(const m of A.parts)m.instanceMatrix.needsUpdate=true}};this.nvT(0);
  for(let i=0;i<12;i++){const a=i/12*6.283,r=620+R()*380,x=NX+Math.cos(a)*r,z=NZ+Math.sin(a)*r,s=new THREE.Mesh(new THREE.ConeGeometry(7,420,6).translate(0,210,0),new THREE.MeshStandardMaterial({color:0xcfd8ff,emissive:0xff3dd8,emissiveIntensity:.8,metalness:.8,roughness:.2}));s.position.set(x,0,z);g.add(s);const b={x0:x-6,x1:x+6,z0:z-6,z1:z+6,h:200};this.world.boxes.push(b);this.world.grid.add(b)}
  this.nvR=[];for(let i=0;i<7;i++){const a=i*.9,t=new THREE.Mesh(new THREE.TorusGeometry(40,2.2,10,48),new THREE.MeshBasicMaterial({color:i%2?0x36f1ff:0xff3dd8}));t.position.set(NX+Math.cos(a)*(250+i*60),200+i*35,NZ+Math.sin(a)*(250+i*60));g.add(t);this.nvR.push(t)}
  const pd=new THREE.Mesh(new THREE.CylinderGeometry(PADR+4,PADR+4,.5,48),new THREE.MeshStandardMaterial({color:0x2e3239,roughness:.95,metalness:.05}));pd.position.set(NX,.25,NZ);g.add(pd);addB(-PADR-4,PADR+4,-PADR-4,PADR+4,.5);
  for(const[r,c]of[[PADR,0x36f1ff],[PADR*.62,0xff3dd8],[PADR*.25,0x36f1ff]]){const t=new THREE.Mesh(new THREE.TorusGeometry(r,.4,8,64).rotateX(Math.PI/2),new THREE.MeshBasicMaterial({color:c}));t.position.set(NX,.55,NZ);g.add(t)}
  for(const a of[[PADR*1.7,.1,2],[2,.1,PADR*1.7]]){const q=new THREE.Mesh(new THREE.BoxGeometry(...a),new THREE.MeshBasicMaterial({color:0x36f1ff}));q.position.set(NX,.56,NZ);g.add(q)}
  const bc=new THREE.Mesh(new THREE.CylinderGeometry(1.2,1.2,160,12,1,true),new THREE.MeshBasicMaterial({color:0x36f1ff,transparent:true,opacity:.3,blending:THREE.AdditiveBlending,depthWrite:false,fog:false}));bc.position.set(NX,80,NZ);g.add(bc);
  {const KX=NX+34,KZ=NZ+34,KM=(c,r,e)=>new THREE.MeshStandardMaterial({color:c,roughness:r==null?.8:r,metalness:.08,emissive:e||0,emissiveIntensity:e?.6:0});
   const fl=new THREE.Mesh(new THREE.BoxGeometry(10,.2,8),KM(0x2b2f36,.95));fl.position.set(KX,.1,KZ);g.add(fl);
   const bw=new THREE.Mesh(new THREE.BoxGeometry(9,4.6,.4),KM(0x1f4a42,.7));bw.position.set(KX,2.3,KZ+3.2);g.add(bw);
   for(const s of[-1,1]){const sw=new THREE.Mesh(new THREE.BoxGeometry(.4,4.6,6.4),KM(0x1f4a42,.7));sw.position.set(KX+s*4.4,2.3,KZ);g.add(sw)}
   const rf=new THREE.Mesh(new THREE.BoxGeometry(9.6,.5,7.4),KM(0x0d2b27,.5,0x2affc4));rf.position.set(KX,4.85,KZ);g.add(rf);
   const ct=new THREE.Mesh(new THREE.BoxGeometry(7,1.1,.9),KM(0x2f6a60,.6));ct.position.set(KX,.55,KZ-2.6);g.add(ct);
   for(const s of[-1,1]){const bp=new THREE.Mesh(new THREE.BoxGeometry(.8,1.1,.45),KM(0x14343a,.5,0x1fb8a0));bp.position.set(KX+s*2.1,1.35,KZ+1.2);g.add(bp);for(const t of[-1,1]){const tnk=new THREE.Mesh(new THREE.CylinderGeometry(.16,.16,.9,8),KM(0x8fe8ff,.4,0x36f1ff));tnk.position.set(KX+s*2.1+t*.22,1.75,KZ+1.2);g.add(tnk)}}
   const sk=this.world.tex(256,64,(c,W,H)=>{c.fillStyle='#07130f';c.fillRect(0,0,W,H);c.strokeStyle='#7dffd0';c.lineWidth=4;c.strokeRect(3,3,W-6,H-6);c.fillStyle='#7dffd0';c.font='bold 24px sans-serif';c.textAlign='center';c.fillText('NOVA OUTFITTERS',W/2,40)});
   const sg=new THREE.Mesh(new THREE.PlaneGeometry(7.8,1.3),new THREE.MeshBasicMaterial({map:sk}));sg.position.set(KX,5.85,KZ-3.74);sg.rotation.y=Math.PI;g.add(sg);
   const mr=new THREE.Mesh(new THREE.TorusGeometry(3,.14,6,28).rotateX(Math.PI/2),new THREE.MeshBasicMaterial({color:0x7dffd0}));mr.position.set(KX,.2,KZ-7);g.add(mr);
   const mb=new THREE.Mesh(new THREE.CylinderGeometry(2.2,2.2,26,14,1,true),new THREE.MeshBasicMaterial({color:0x7dffd0,transparent:true,opacity:.3,side:THREE.DoubleSide,depthWrite:false,blending:THREE.AdditiveBlending,fog:false}));mb.position.set(KX,13,KZ-7);g.add(mb);
   addB(29.4,38.6,30.4,37.6,4.9);SHOPS.push({...SHOPDEF.nova,id:'nova',w:9,d:7,x:KX,z:KZ,mz:KZ-7})}
  for(const[x,y,z,r,c]of[[NX-2400,2500,NZ+3600,320,0xd8c8ff],[NX+2800,3100,NZ-2600,240,0xffb8c8]]){const mo=new THREE.Mesh(new THREE.SphereGeometry(r,24,16),new THREE.MeshBasicMaterial({color:c,fog:false}));mo.position.set(x,y,z);g.add(mo)}
  const lt=new THREE.DirectionalLight(0xdfe4ff,1.2);lt.position.set(NX+500,900,NZ-400);lt.target.position.set(NX,0,NZ);g.add(lt,lt.target);g.visible=false;sc.add(g)}

 bail(a){const p=this.player,sn=Math.sin(a.h),cs=Math.cos(a.h);this.flying=null;p.x=a.x;p.z=a.z;p.y=a.y+1;p.vx=p.vz=0;p.g.visible=true;a.th=0;a.ab=0;this.abn.push(a);
  this.sky={vx:sn*a.v*.8,vz:cs*a.v*.8,vy:Math.min(0,a.vy||0),ch:0,cd:0,armed:false,agl:0};this.sfx.beep(400);this.toast('You jumped! Press SPACE to open the parachute')}
 abnStep(dt){for(let i=this.abn.length-1;i>=0;i--){const a=this.abn[i];if(a.brk){const cr=a.brokenStep(dt,this);if(cr){if(a.hb&&a.hb.tw)this.xtwHit(a.hb.tw,a.y);a.hb=null;this.boom(a.x,a.z,14,0);a.alive=false;a.dead=20;a.g.visible=false;this.abn.splice(i,1)}continue}a.ab+=dt;a.p=Math.min(.5,a.p+dt*.15);a.y-=(10+a.ab*6)*dt;a.x+=Math.sin(a.h)*a.v*dt;a.z+=Math.cos(a.h)*a.v*dt;a.place();if(a.y<=(a.gl||0)+1){this.boom(a.x,a.z,14,0);a.alive=false;a.dead=20;a.g.visible=false;this.abn.splice(i,1)}}}
 skyStep(dt,k){const S=this.sky,p=this.player,w=this.world;if(!k.Space)S.armed=true;
  if(k.Space&&S.armed&&!S.ch){S.ch=1;S.cd=0;this.sfx.beep(600);this.toast('Parachute open — steer with W/A/S/D')}
  if(S.ch)S.cd=Math.min(1,S.cd+dt/1.4);
  const tgt=S.ch?U.lerp(-55,-5,U.sm(0,1,S.cd)):-55;if(S.vy>tgt)S.vy=Math.max(tgt,S.vy-20*dt);else S.vy=Math.min(tgt,S.vy+45*dt);
  const yw=this.rig.yaw,fx=Math.sin(yw),fz=Math.cos(yw),iz=(k.KeyW?1:0)-(k.KeyS?1:0),ix=(k.KeyD?1:0)-(k.KeyA?1:0);let wx=iz*fx-ix*fz,wz=iz*fz+ix*fx;const ln=Math.hypot(wx,wz)||1,sp=(iz||ix)?(S.ch?10:14):0,e=1-Math.exp(-dt*(S.ch?1.2:.6));
  S.vx=U.lerp(S.vx,wx/ln*sp,e);S.vz=U.lerp(S.vz,wz/ln*sp,e);p.x+=S.vx*dt;p.z+=S.vz*dt;p.y+=S.vy*dt;
  for(const b of w.grid.at(p.x,p.z))if(p.y<b.h-4){const r=push(p.x,p.z,C.pr,b);if(r){p.x+=r[0]*r[2];p.z+=r[1]*r[2]}}
  if(Math.abs(p.x)>C.half&&p.x<1400)p.x=Math.sign(p.x)*C.half;if(p.x<1400)p.z=U.clamp(p.z,-C.half,C.zs);
  let gl=0;for(const b of w.grid.at(p.x,p.z))if(p.x>b.x0&&p.x<b.x1&&p.z>b.z0&&p.z<b.z1&&p.y>=b.h-4)gl=Math.max(gl,b.h);
  for(const q of w.mt){const d=Math.hypot(p.x-q[0],p.z-q[1]);if(d<q[2])gl=Math.max(gl,q[3]*(1-d/q[2]))}gl=Math.max(gl,ghOf(p.x,p.z,p.y));S.agl=p.y-gl;
  p.g.rotation.order='YXZ';p.g.position.set(p.x,p.y,p.z);if(Math.hypot(S.vx,S.vz)>1)p.face=Math.atan2(S.vx,S.vz);p.g.rotation.y=p.face;p.g.rotation.x=S.ch?0:1.25;
  if(!this.chm){const g=this.chm=new THREE.Group(),cm=new THREE.MeshStandardMaterial({color:0xff6a2a,side:THREE.DoubleSide,roughness:.8}),c=new THREE.Mesh(new THREE.SphereGeometry(4.5,20,10,0,Math.PI*2,0,Math.PI/2),cm);c.position.y=5.5;g.add(c);
   const pts=[];for(let i=0;i<6;i++){const a=i/6*6.283;pts.push(new THREE.Vector3(Math.cos(a)*4.4,5.5,Math.sin(a)*4.4),new THREE.Vector3(0,1.6,0))}g.add(new THREE.LineSegments(new THREE.BufferGeometry().setFromPoints(pts),new THREE.LineBasicMaterial({color:0xdddddd})));this.scene.add(g)}
  this.chm.visible=!!S.ch;if(S.ch){const s=.15+.85*U.sm(0,1,S.cd);this.chm.scale.setScalar(s);this.chm.position.set(p.x,p.y,p.z)}
  if(p.y<=gl+.05){const vy=S.vy;p.y=gl;p.vx=p.vz=0;p.g.rotation.order='XYZ';p.g.rotation.x=0;this.chm.visible=false;this.sky=null;if(vy<-9){this.toast('Too late for the parachute!');this.hurt(999)}else this.toast('Soft landing')}}
 autoLand(){const L=this.lau;if(!L||L.ph!=='land')return;L.auto=!L.auto;this.toast(L.auto?'AUTO LAND engaged — G to cancel':'Manual control')}

 toggleGhost(){this.ghost=!this.ghost;$('gho').style.display=this.ghost?'block':'none';this.toast(this.ghost?'GHOST MODE ON: pass through everything':'Ghost mode OFF');this.sfx.beep(this.ghost?900:500)}
 buildShop(id){const e=$('shop'),G=this,w=this.weaponName,s=this.nearShop||{},R=[],c=this.driving;e.style.display=id==='skin'?'none':'block';$('skin').style.display=id==='skin'?'block':'none';if(id==='skin')return;
  const T={gun:'HARBOR ARMS — weapons',att:'ATTACHMENT LAB',car:'PREMIUM MOTORS — cars',moto:'TWO WHEELS — bikes',garage:'ELFO GARAGE — tuning',arena:'CHALLENGE HALL — win cash',mil:'MILITARY DEPOT — vehicles',air:'AIRCRAFT DEALER — planes',space:'ASTRA SPACEWORKS — spacecraft',nova:'NOVA OUTFITTERS — gear'}[id],P={Pistol:300,SMG:900,Shotgun:1200,Rifle:1800,Sniper:2200};let note='';
  if(id==='gun'){for(const n of GUNS)R.push([(this.own.has(n)?'✓ ':'')+n,this.own.has(n)?0:P[n],()=>{if(G.own.has(n)){G.weaponName=n;return}if(G.pay(P[n])){G.own.add(n);G.am[n]=(G.am[n]||0)+WEAP[n].ammo;G.mag[n]=MAG[n];G.weaponName=n}}]);
   R.push(['Ammo (equipped gun)',100,()=>{if(WEAP[w]&&G.pay(100))G.am[w]+=WEAP[w].ammo}],['Armor',700,()=>{if(G.pay(700))G.armor=100}],['Medkit',150,()=>{if(G.pay(150))G.health=100}])}
  else if(id==='att'){for(const n of GUNS)if(this.own.has(n))R.push([(n===w?'» ':'')+n,0,()=>{G.weaponName=n}]);
   if(WEAP[w])for(const[k,l,pr]of ATT){const A=this.att[w]||{},ow=this.attOwn.has(w+k);R.push([(A[k]?'● ':'○ ')+l,ow?0:pr,()=>{if(!ow&&!G.pay(pr))return;G.attOwn.add(w+k);const B=G.att[w]=G.att[w]||{};B[k]=!B[k];if(B[k]){if(k==='long')B.short=false;if(k==='short')B.long=false}}])}else note='Buy and equip a gun first.'}
  else if(id==='car'||id==='moto'){const D=id==='car'?CARMODELS:MOTOS;for(const k in D)R.push([D[k].n,D[k].p,()=>{if(G.pay(D[k].p)){G.spawnCar(k,s.x,s.z-11,Math.PI);G.toast(D[k].n+' delivered outside')}}]);
 if(id==='car'){const tk=(nm,pr,hp,sc)=>R.push([nm+' (F: drive, fire: cannon)',pr,()=>{if(!G.pay(pr))return;const c=new Car(G.scene,0x536b4a,'tank');c.type='mytank';c.mytank=1;c.f.max*=.4;c.f.acc*=.55;c.hp=hp;c.x=s.x;c.z=s.z-12;c.h=Math.PI;const M=new THREE.MeshStandardMaterial({color:0x3f5a38,roughness:.6,metalness:.4}),t=new THREE.Mesh(new THREE.BoxGeometry(1.6,.5,2.2),M),b=new THREE.Mesh(new THREE.CylinderGeometry(.09,.09,2.6,8).rotateX(Math.PI/2),M);t.position.set(0,1.45,-.1);b.position.set(0,1.5,1.9);c.m.add(t,b);if(sc){c.m.scale.multiplyScalar(sc);c.sc0.copy(c.m.scale)}c.step(0,0,0,true,false);G.cars.push(c);G.toast(nm+' delivered outside')}]);tk('Battle Tank',45000,1600);tk('Heavy Tank',90000,3500,1.25)}}
  else if(id==='mil'){const B=(n,p,fn)=>R.push([n,p,()=>{if(G.pay(p)){fn();G.toast(n+' delivered')}}]),
  air=(k,jet)=>()=>{const a=new Plane(G.scene,k);if(jet){a.hx=-450+Math.random()*350;a.hz=-690;a.hh=Math.PI/2}else{a.hx=s.x+(Math.random()-.5)*8;a.hz=s.z-14;a.hh=0}a.reset();G.planes.push(a);if(jet)G.toast('Parked on the airport taxiway')};
  B('Battle Tank (F: drive, fire: cannon)',45000,()=>{const c=new Car(G.scene,0x536b4a,'tank');c.type='mytank';c.mytank=1;c.f.max*=.4;c.f.acc*=.55;c.hp=1600;c.x=s.x;c.z=s.z-12;c.h=Math.PI;const M=new THREE.MeshStandardMaterial({color:0x3f5a38,roughness:.6,metalness:.4}),t=new THREE.Mesh(new THREE.BoxGeometry(1.6,.5,2.2),M),b=new THREE.Mesh(new THREE.CylinderGeometry(.09,.09,2.6,8).rotateX(Math.PI/2),M);t.position.set(0,1.45,-.1);b.position.set(0,1.5,1.9);c.m.add(t,b);c.step(0,0,0,true,false);G.cars.push(c)});
  B('Attack Helicopter',60000,air('Heli',0));}
  else if(id==='space'){for(const k in SHIPS){const S=SHIPS[k],ow=G.shipOwn.has(k);R.push([(ow?'\u2713 ':'')+S.n,ow?0:S.p,()=>{if(ow){G.toast(S.n+' is parked on the Astra launch pad');return}if(G.pay(S.p)){G.shipOwn.add(k);G.upShip();G.toast(S.n+' delivered to the Astra launch pad')}}])}note='Spacecraft are delivered to the pad outside. Walk up and press F to board.'}
  else if(id==='nova'){R.push([G.jetOwn?'\u2713 Jetpack (equipped)':'Jetpack grip pack — low-gravity flight',G.jetOwn?0:3500,()=>{if(G.jetOwn){G.toast('Jetpack already equipped');return}if(G.pay(3500)){G.jetOwn=true;G.player.jet=100;G.toast('Jetpack equipped — jump, then hold SPACE')}}]);
   R.push(['Jet fuel refill ('+Math.round(G.player.jet)+'%)',150,()=>{if(!G.jetOwn){G.toast('Buy the jetpack first');return}if(G.pay(150)){G.player.jet=100;G.toast('Jetpack refilled')}}]);
   note='Nova has low gravity: jump first, then hold SPACE to fly. Fuel refills on the ground.'}
  else if(id==='air'){const PR={F16:100000,F15:140000,F18:135000,MiG29:110000,Su35:150000,Typhoon:145000,A10:90000,SR71:260000,Tornado:100000,F117:220000,A380:140000,Gulfstream:75000,Heli4:80000,Heli5:70000,Cessna4:8000,Stunt3:15000,Cessna:8000,Stunt:15000,Biplane:12000,Learjet:55000,Airbus:70000,Boeing:90000,Concorde:90000,F35:150000,Sukhoi:130000,Raptor:120000,B2:200000,Heli:60000,Cessna2:8000,Cessna3:8000,Stunt2:15000,Biplane2:12000,Learjet2:55000,Boeing2:90000,Cargo:95000,Airbus2:70000,F35b:150000,Sukhoi2:130000,Raptor2:125000,B2b:200000,Heli2:60000,Heli3:60000};for(const k of Object.keys(PLANES)){const p=PR[k]||50000;R.push([PLANES[k].name,p,()=>{if(!G.pay(p))return;const a=new Plane(G.scene,k),ap=G.nearShop&&G.nearShop.ap;if(PLANES[k].heli){a.hx=ap?ap[0]+470:330;a.hz=ap?ap[1]-35:-650;a.hh=0}else{a.hx=ap?ap[0]-700+Math.random()*380:-450+Math.random()*380;a.hz=ap?ap[1]:-690;a.hh=Math.PI/2}a.reset();G.planes.push(a);if(PLANES[k].bay){G.xhaulMarker(a);G.toast(PLANES[k].name+' delivered — walk behind it and press E to open the cargo door')}else G.toast(PLANES[k].name+' delivered to the '+(PLANES[k].heli?'helipad':'taxiway'))}])}note='Delivered to the airport. Hold Shift on the runway to take off.'}
   else if(id==='arena'){const go=(o)=>{G.ch=o;G.toast('Challenge started!');G.closeShop();return true};
   R.push(['Street Brawl: 8 KOs in 60s \u2192 win $2,500',0,()=>go({type:'kill',n:0,need:8,t:60,r:2500,txt:''})],['Time Attack: reach the red marker (drive!) \u2192 +$4,000',0,()=>{G.nextMission();G.mis.time=Math.round(G.mis.time*.6);return go({type:'race',bonus:4000,txt:''})}],
    ['Survive the Heat: 3 stars for 60s \u2192 win $6,000',0,()=>{G.setWanted(0);G.addWanted(3);return go({type:'heat',t:60,r:6000,txt:''})}]);if(G.ch)R.push(['Abandon current challenge',0,()=>{G.ch=null}]);note='Pick a challenge. Fight, race or survive.'}
  else if(c){const o=G.over,cap=o?25:3;c.lv=c.lv||{e:0,h:0,t:0,a:0};const PAL=[0xd10000,0x2c7be5,0xf2c200,0x1fbf3a,0xf4f4f4,0x111111,0x8e44ad,0xff6a00,0xff3d8b,0x00e5ff],
   up=(lab,k,base,fn)=>R.push([lab+' Lv '+c.lv[k]+'/'+cap,c.lv[k]<cap?base*(c.lv[k]+1):0,()=>{if(c.lv[k]<cap&&G.pay(base*(c.lv[k]+1))){c.lv[k]++;fn()}}]),nm=o?9999:300;
   R.push(['Nitro refill +100 ('+(G.nit|0)+'/'+nm+', hold Shift)',500,()=>{if(G.nit<nm&&G.pay(500))G.nit=Math.min(nm,G.nit+100)}]);
   up('Engine / top speed','e',1500,()=>{c.f.max*=1.08;c.f.acc*=1.12});up('Handling / steering','h',1200,()=>{c.f.steer*=1.08;c.f.grip*=1.06});up('Tires & brakes','t',1000,()=>{c.f.brake*=1.1;c.f.grip*=1.05});up('Armor plating','a',1300,()=>{c.hp+=60});
   const lo=o?-.3:-.15,hi=o?1.5:.45;R.push(['Spring height \u25bc lower ('+c.rh.toFixed(2)+')',100,()=>{if(c.rh>lo&&G.pay(100))c.rh=Math.max(lo,c.rh-.1)}],['Spring height \u25b2 raise',100,()=>{if(c.rh<hi&&G.pay(100))c.rh=Math.min(hi,c.rh+.1)}]);
   if(c.wh)R.push(['Wheel size \u25bc smaller ('+c.wsz.toFixed(2)+'x)',150,()=>{if(c.wsz>(o?.5:.8)&&G.pay(150))c.wsz=Math.max(o?.5:.8,c.wsz-.1)}],['Wheel size \u25b2 bigger',150,()=>{if(c.wsz<(o?3:1.4)&&G.pay(150))c.wsz=Math.min(o?3:1.4,c.wsz+.1)}]);
   R.push([c.air?'\u2713 Air suspension (V = hop)':'Air suspension kit',c.air?0:2500,()=>{if(!c.air&&G.pay(2500))c.air=true}],['Repaint (next color)',200,()=>{if(G.pay(200)){c.pi=((c.pi||0)+1)%PAL.length;c.col=PAL[c.pi];c.body.material.color.setHex(c.col)}}]);if(o)note='UNLIMITED mode on'}
  else note='Drive a vehicle into the garage marker to tune it.';
  e.innerHTML='<h2>'+tr(T)+'</h2><p>$ '+this.money.toLocaleString()+' · '+tr('B closes.')+' '+tr(note)+'</p>';const gr=document.createElement('div');gr.className='shopgrid';
  R.forEach(r=>{const b=document.createElement('button');b.textContent=tr(r[0])+(r[1]?' — $'+r[1].toLocaleString():'');b.onclick=()=>{if(r[2]()===true)return;G.buildShop(id)};gr.appendChild(b)});
  const x=document.createElement('button');x.textContent=tr('Close');x.onclick=()=>G.closeShop();gr.appendChild(x);e.appendChild(gr)}
 toggleCar(){const p=this.player;if(this.xent&&!this.xbyp)return;if(!this.driving&&!this.flying&&this.near&&!this.xbyp&&this.xin){const nc=this.near;if(nc.type!=='motorcycle'&&nc.type!=='tank'&&nc.type!=='mytank'&&!nc.wreck&&Math.abs(nc.sp||0)<5){this.xentS(nc);return}}if(this.driving&&!this.flying&&this.driving.type!=='motorcycle'&&this.driving.type!=='tank'&&this.driving.type!=='mytank')this.xdoorA(this.driving);
  if(this.flying){const a=this.flying;if(a.P.hover){if(a.y-(a.gl||0)>2.8||a.v>6){this.toast(this.xL('Land the hover car first (hold Space)','اول ماشین پرنده را فرود بیاور (Space)'));return}const ex=3.2;p.x=a.x+Math.cos(a.h)*ex;p.z=a.z-Math.sin(a.h)*ex;p.y=(a.gl||0)+.05;p.vx=p.vz=0;p.g.visible=true;this.flying=null;a.v=0;a.th=0;this.sfx.beep();return}if(a.y-(a.gl||0)>8){this.bail(a);return}if(a.y-(a.gl||0)>.3||a.v>(a.P.heli?6:25)){this.toast(a.P.heli?'Land the helicopter first (hold Space)':'Land and slow below 90 km/h first');return}const ex=a.P.heli?a.P.span*.8:a.P.span+2;p.x=a.x+Math.cos(a.h)*ex;p.z=a.z-Math.sin(a.h)*ex;p.y=a.gl||0;p.vx=p.vz=0;p.g.visible=true;this.flying=null;a.v=0;a.th=0;this.sfx.beep();return}
  if(!this.driving&&!this.near&&this.nearAir){this.flying=this.nearAir;p.g.visible=false;this.sfx.beep();this.toast(this.nearAir.P.hover?'W: thrust · S: reverse · A/D: steer · Shift: ascend · Space: descend/land · F: exit':'Hold Shift: throttle (auto takeoff) \u00b7 Shift: throttle \u00b7 Space: brake \u00b7 W/S: pitch \u00b7 A/D: bank \u00b7 J: missile (jets)');return}
  if(!this.driving&&!this.flying&&!this.near&&!this.nearAir&&this.nearTv){const c=this.nearTv,ry=c.a?(c.dir>0?Math.PI/2:-Math.PI/2):(c.dir>0?0:Math.PI),tv=this.nvHVB?{body:this.nvHVB,glow:this.nvHG,tail:this.nvHT,head:this.nvHH}:null,hv=new Hover(this.nv,c.wx,c.wz,c.col==null?0x36f1ff:c.col,tv);hv.h=ry;hv.y=.35;hv.place();this.hovers.push(hv);c.taken=true;this.nearTv=null;this.flying=hv;p.g.visible=false;this.sfx.beep();this.toast('W: thrust \u00b7 S: reverse \u00b7 A/D: steer \u00b7 Shift: ascend \u00b7 Space: descend/land \u00b7 F: exit');return}
  if(this.driving){const c=this.driving,sn=Math.sin(c.h),cs=Math.cos(c.h),sp=[[c.x+cs*2.6,c.z-sn*2.6],[c.x-cs*2.6,c.z+sn*2.6],[c.x-sn*4,c.z-cs*4]];
   const ok=sp.find(([x,z])=>this.world.free(x,z,.7)&&!this.cars.some(o=>o!==c&&Math.hypot(o.x-x,o.z-z)<2))||sp[0];
   p.x=ok[0];p.z=ok[1];p.y=0;p.vx=p.vz=0;p.g.visible=true;this.driving=null;c.nb=false;if(c.rider)c.rider.visible=false;this.sfx.radio(0)}
  else if(this.near){if(this.near.xh&&this.near.xh.alive){this.toast(this.xL('Open the cargo door first','اول درِ بار را باز کن'));return}if(this.near.ai)this.jack(this.near);this.driving=this.near;this.near.ai=null;this.near.stun=0;p.g.visible=false;this.sfx.beep();this.sfx.radio(this.radio);const rm=this.near.rmat;if(rm){rm[0].color.copy(p.mat.sh.color);rm[1].color.copy(p.mat.pn.color);rm[2].color.copy(p.mat.sk.color);this.near.rider.visible=true}}}
 toast(t){const e=$('toast');e.textContent=tr(t);e.style.display='block';this.toastT=2}
 fixed(dt){if(this.lau)this.lauStep(dt);if(this.abn.length)this.abnStep(dt);if(this.dead>0&&(this.dead-=dt)<=0)this.revive();const k=this.dead>0?NOKEY:this.inp.k,car=this.driving,pl=this.player;const nvw=!!(this.lau&&this.lau.walk&&this.lau.nova);pl.jetP.visible=!!(nvw&&this.jetOwn);if(!nvw||this.sky||car||this.flying||this.sit)pl.jetM.visible=false;this.weaponCooldown=Math.max(0,this.weaponCooldown-dt);if(this.flash>0)this.flash-=dt;for(const o of this.trs)if(o.visible&&(o.life-=dt)<=0)o.visible=false;
  if(car){car.nb=!!(k.ShiftLeft&&k.KeyW&&this.nit>0&&!car.wreck);if(car.nb)this.nit=Math.max(0,this.nit-14*dt*(car.type==='motorcycle'?1.25:1));car.step(dt,(k.KeyW?1:0)-(k.KeyS?1:0),(k.KeyA?1:0)-(k.KeyD?1:0),false,!!k.Space);pl.x=car.x;pl.z=car.z}else if(this.flying){const a=this.flying,cr=a.fly(dt,k,this);pl.x=a.x;pl.z=a.z;pl.face=a.h;pl.g.visible=false;if(cr){if(a.hb&&a.hb.tw)this.xtwHit(a.hb.tw,a.y);a.hb=null;this.toast('Crashed: '+cr+' - aircraft lost, buy it again');this.boom(a.x,a.z,14,100);a.alive=false;a.dead=20;a.g.visible=false;this.flying=null;pl.g.visible=true;this.hurt(999)}}else if(this.sky)this.skyStep(dt,k);else if(!this.sit){this.kin.k=k;pl.step(dt,this.kin,this.rig.yaw,this.world)}
  {const W=WEAP[this.weaponName];pl.armed=!car&&!!W;for(const n in pl.guns)pl.guns[n].visible=pl.armed&&n===this.weaponName;pl.flashM.visible=pl.armed&&this.flash>0;
   if(pl.armed){pl.aR.rotation.x=-1.45;if(this.fireT>0){this.fireT-=dt;pl.face=this.rig.yaw;pl.g.rotation.y=pl.face}}
   if(W&&W.auto&&!car&&this.dead<=0&&(k.KeyJ||(this.inp.locked&&this.inp.btn)))this.shoot()}
  const pp=car?null:pl;
  for(const c of this.cars){if(c===car)continue;if(this.xth&&this.xth.car===c&&this.xth.ph==='drive')continue;{const dd=Math.hypot(c.x-pl.x,c.z-pl.z),far=dd>300&&!c.wreck&&c.type!=='police'&&c.type!=='tank';if(far!==c.far){c.far=far;c.m.visible=!far}if(far)continue}
   if(c.wreck){c.step(dt,0,0,true,false);c.wt+=dt;if(c.wt>7)c.m.scale.copy(c.sc0).multiplyScalar(Math.max(.01,1-(c.wt-7)/2));if(c.wt>9){c.m.scale.copy(c.sc0);c.wreck=false;c.hp=100;c.y=0;c.vy=0;c.rx=c.rz=0;c.spin=null;c.m.rotation.set(0,c.h,0);c.body.material.color.setHex(c.col);this.traffic.respawn(c,pl.x,pl.z)}continue}if(c.type==='police'||c.type==='tank'){const dx=pl.x-c.x,dz=pl.z-c.z;const d=Math.hypot(dx,dz);if(c.type==='tank'&&d<55&&this.dead<=0){c.sk2=(c.sk2||0)-dt;if(c.sk2<=0){c.sk2=3.2;this.tracer(c.x,2.6,c.z,pl.x,1,pl.z);this.boom(pl.x+(Math.random()-.5)*10,pl.z+(Math.random()-.5)*10,5,30)}}if(d>4){c.h=U.lerpA(c.h,Math.atan2(dx,dz),dt*1.5);c.step(dt,c.type==='tank'?.35:.5,U.clamp(U.wrap(Math.atan2(dx,dz)-c.h)*2,-1,1),false,false)}else c.step(dt,0,0,true,false);
   c.sk=Math.abs(c.sp)<2&&d>8?c.sk+dt:0;if(c.sk>2.5||d>C.npc.cull){c.sk=0;if(c.type==='tank'){c.x=pl.x-40;c.z=pl.z}else this.traffic.respawn(c,pl.x,pl.z)}continue}if(c.ai){this.traffic.drive(c,dt,this.cars,pp);if(Math.hypot(c.x-pl.x,c.z-pl.z)>C.npc.cull)this.traffic.respawn(c,pl.x,pl.z)}else c.step(dt,0,0,true,false)}
  for(const c of this.cars)c.gh=!!this.ghost&&c===car;for(const c of this.cars)if(!c.far||c===car)c.collide(this.world);crash(this.cars);if(car&&car.hit>9)this.hurt((car.hit-9)*2.2);for(const c of this.cars)if(c.hit>9)this.dmgCar(c,(c.hit-9)*4);this.tt+=dt;if(!(this.lau&&this.lau.walk))this.peds.update(dt,pl.x,pl.z,this.tt,this);
  for(const q of this.peds.p){if(q.dead>0||q.down>0)continue;for(const c of this.cars)if(Math.abs(c.sp)>5&&Math.hypot(c.x-q.x,c.z-q.z)<C.ped.hit){this.killPed(q,c===car);break}}
  let pn=0,pc=0;for(const c of this.cars)if(c.type==='police'||c.type==='tank'){const d=Math.hypot(c.x-pl.x,c.z-pl.z);if(d<22)pn++;if(d<6)pc++;if(c.type==='tank'&&d<30)pn+=3}this.pn=pn;
  if(this.wanted>0&&this.dead<=0){if(pn)this.hurt(1.2*this.wanted*pn*dt);const slow=car?Math.abs(car.sp)<3:Math.hypot(pl.vx,pl.vz)<1.5;this.bust=pc&&slow?this.bust+dt:Math.max(0,this.bust-dt);
   if(this.bust>2.5){this.bust=0;this.die('BUSTED','#6fa8ff',Math.min(this.money,300))}this.evade=pn?0:this.evade+dt;if(this.evade>12)this.setWanted(this.wanted-1)}
  const m=this.mis;if(car&&this.dead<=0){m.time-=dt;if(Math.hypot(car.x-m.x,car.z-m.z)<C.mis.r){const r=Math.round(C.mis.reward+m.d*1.5);if(this.ch&&this.ch.type==='race'){this.cash(this.ch.bonus);this.ch=null}this.cash(r);this.big('MISSION PASSED!','$ '+r.toLocaleString(),'#ffd24a');this.sfx.beep(880);this.nextMission()}else if(m.time<=0){if(this.ch&&this.ch.type==='race')this.ch=null;this.toast('Mission failed: out of time');this.nextMission()}}
  const a=this.sl;for(let i=0;i<60;i++)if(a[i]>0){a[i]-=dt;this.sp[i*3+1]+=dt*1.2;if(a[i]<=0)this.sp[i*3+1]=-100}
  this.dfx.update(dt,car,this.cam,this.r,this.world.night);pdebStep(this,dt);
  this.tick2(dt);this.sg.attributes.position.needsUpdate=true}
 mini(x,z,h){const g=this.mg,yaw=this.rig.yaw,th=yaw+Math.PI;g.clearRect(0,0,200,200);
  if(this.lau&&this.lau.walk){g.save();g.beginPath();g.arc(100,100,98,0,7);g.clip();g.fillStyle='#0b0f1e';g.fillRect(0,0,200,200);g.translate(100,100);g.rotate(th);
   const sc=.06,c=Math.cos(th),s=Math.sin(th),pt=(wx,wz,col,r)=>{const X=((wx-x)*c-(wz-z)*s)*sc,Y=((wx-x)*s+(wz-z)*c)*sc;g.fillStyle=col;g.beginPath();g.arc(X,Y,r,0,7);g.fill()};
   g.strokeStyle='#1c2b4a';g.lineWidth=1;for(let i=-10;i<=10;i++){const u=i*150*sc;g.beginPath();g.moveTo(u,-100);g.lineTo(u,100);g.stroke();g.beginPath();g.moveTo(-100,u);g.lineTo(100,u);g.stroke()}
   for(const p of this.nvP||[])pt(p[0],p[1],'#36f1ff',5);for(const hv of this.hovers)if(hv.g.visible)pt(hv.x,hv.z,hv===this.flying?'#ffffff':'#36f1ff',hv===this.flying?4:2.5);
   g.restore();g.save();g.translate(100,100);g.rotate(yaw-h);g.fillStyle='#ffd24a';g.beginPath();g.moveTo(0,-10);g.lineTo(-6,8);g.lineTo(6,8);g.fill();g.restore();return}
  g.save();g.beginPath();g.arc(100,100,98,0,7);g.clip();g.translate(100,100);g.rotate(th);
  g.drawImage(this.world.mm,-(x+1600)*.5,-(z+1600)*.5);g.restore();
  const c=Math.cos(th),s=Math.sin(th);g.fillStyle='#ff3d8b';
  for(const o of this.cars){if(!o.ai&&o.type!=='tank')continue;g.fillStyle=o.type==='police'?'#4da3ff':o.type==='tank'?'#9bd15a':'#ff3d8b';const dx=(o.x-x)*.5,dz=(o.z-z)*.5,X=100+dx*c-dz*s,Y=100+dx*s+dz*c;if((X-100)**2+(Y-100)**2<9000)g.fillRect(X-1.5,Y-1.5,3,3)}
  {const pt=(wx,wz,col,r)=>{const dx=(wx-x)*.5,dz=(wz-z)*.5;let X=dx*c-dz*s,Y=dx*s+dz*c;const d=Math.hypot(X,Y);if(d>88){X*=88/d;Y*=88/d}g.fillStyle=col;g.beginPath();g.arc(100+X,100+Y,r,0,7);g.fill()};
  for(const q of SHOPS)if(q.id!=='nova'||(this.lau&&this.lau.walk))pt(q.x,q.mz,q.css,4);for(const o of POI)pt(o.x,o.z,o.c,4);pt(0,-641,'#ffffff',5);if(this.wp)pt(this.wp.x,this.wp.z,'#ff4bd8',4);pt(this.mis.x,this.mis.z,'#ff3030',5)}
  g.save();g.translate(100,100);g.rotate(yaw-h);g.fillStyle='#36f1ff';g.beginPath();g.moveTo(0,-10);g.lineTo(-6,8);g.lineTo(6,8);g.fill();g.restore()}
 hud(){const w=this.world,c=this.driving,pl=this.player,x=c?c.x:pl.x,z=c?c.z:pl.z,h=Math.floor(w.hour),m=Math.floor(w.hour%1*60);
  $('clock').textContent=String(h).padStart(2,'0')+':'+String(m).padStart(2,'0');
  const loc=this.lau&&this.lau.walk?'Nova City':x>1400?'Interior':(Math.abs(x)>760||z<-760)?'Outskirts':z<-610?'Airport':z>480?'Harbor Docks':(x>240&&x<480&&z>-480&&z<-120)?'Greenfield Park':Math.hypot(x,z)<90?'Central Plaza':Math.hypot(x,z)<300?'Downtown':x<0?'Westgate':'Eastside';
  if(loc!==this.loc){this.loc=loc;$('loc').textContent=loc;const e=$('zone');e.textContent=loc;e.style.animation='none';void e.offsetWidth;e.style.animation='zn 4s forwards'}
  $('speed').style.display=c?'block':'none';if(c){const k=Math.abs(c.sp);$('spd').textContent=Math.round(k*3.6);$('arc').style.strokeDashoffset=226.2*(1-Math.min(1,k/C.car.max))}
  this.near=null;if(!c){let best=C.enter;for(const o of this.cars){if(o.wreck)continue;const d=Math.hypot(o.x-pl.x,o.z-pl.z);if(d<best){best=d;this.near=o}}}
  let ns=null;for(const q of SHOPS)if((!c||q.id==='garage')&&Math.hypot(x-q.x,z-q.mz)<4)ns=q;this.nearShop=ns;if(this.wp&&Math.hypot(x-this.wp.x,z-this.wp.z)<12)this.wp=null;
  this.nearAir=null;this.nearTv=null;if(!c&&!this.flying)for(const a of this.planes)if(a.alive&&Math.hypot(a.x-pl.x,a.z-pl.z)<a.P.span+5)this.nearAir=a;if(!c&&!this.flying&&this.hovers&&this.lau&&this.lau.walk){let bd=1e9;for(const a of this.hovers){const d=Math.hypot(a.x-pl.x,a.z-pl.z);if(d<bd&&d<12){bd=d;this.nearAir=a}}if(this.nvCS)for(const a of this.nvCS){if(a.taken||a.wx===undefined)continue;const d=Math.hypot(a.wx-pl.x,a.wz-pl.z);if(d<12&&d<bd){bd=d;this.nearTv=a}}if(this.nearTv)this.nearAir=null}$('prompt').textContent=tr(this.flying&&this.flying.P.hover?'F: exit (land first) · Shift: rise · Space: descend/land':this.flying?'Press F: exit when landed · in the air: jump out (then SPACE = parachute)':ns?'Press B — '+ns.name:this.nearTv?'Press F to board the Nova Hover':(!this.near&&this.nearAir)?'Press F to board '+this.nearAir.P.name:'Press F to enter vehicle');$('prompt').style.display=(this.near||ns||this.nearAir||this.nearTv||this.flying)?'block':'none';if(!this.mmT||this.tt-this.mmT>.12){this.mmT=this.tt;this.mini(x,z,c?c.h:pl.face)}
  const nvw=this.lau&&this.lau.walk;$('jetw').style.display=$('jetb').style.display=(nvw&&this.jetOwn)?'block':'none';if(nvw&&this.jetOwn)$('jbi').style.width=Math.max(0,pl.jet)+'%';$('abi').style.width=this.armor+'%';$('wp').textContent=this.weaponName.toUpperCase()+(WEAP[this.weaponName]?' \u00b7 '+(this.mag[this.weaponName]||0)+'/'+(this.am[this.weaponName]||0)+(this.rl>0?' RELOAD':''):'')+(c?' \u00b7 NOS '+(this.nit|0):'');$('hit').style.opacity=Math.min(1,this.hitT*2);$('xh').style.display=(pl.armed&&!c)?'block':'none';
  const mi=this.mis;let ob='Get in a vehicle';if(c){const t=Math.max(0,mi.time|0);ob='Drive to the red marker \u00b7 '+Math.round(Math.hypot(c.x-mi.x,c.z-mi.z))+' m \u00b7 '+(t/60|0)+':'+String(t%60).padStart(2,'0')}if(this.flying){const a=this.flying;ob=a.P.name+' \u00b7 '+Math.round(a.v*3.6)+' km/h \u00b7 ALT '+Math.round(a.y)+' m \u00b7 THR '+Math.round(a.th*100)+'%'}else if(this.ch)ob=this.ch.txt;$('obj').textContent=tr(ob)}
 loop(t){requestAnimationFrame(t2=>this.loop(t2));document.body.classList.toggle('nc',this.state==='PLAYING'&&!this.shopOpen&&!this.mapOpen&&!this.editing);const dt=Math.min(.1,(t-this.last)/1000);this.last=t;
  if(this.state==='PLAYING'&&!this.shopOpen&&!this.mapOpen){this.acc+=dt;while(this.acc>=1/60){this.fixed(1/60);this.acc-=1/60}
   const c=this.driving,fa=this.flying;this.sfx.update(fa?(fa.P.heli?.4+.6*fa.th:Math.max(fa.th*.85,Math.min(1,fa.sp/fa.P.vm))):c?Math.min(1,Math.abs(c.sp)/C.car.max):0,!!(c||fa),c&&this.inp.k.KeyH,c&&c.slip&&Math.abs(c.sp)>5,this.pn>0&&this.wanted>0,fa?(fa.P.heli?'heli':fa.P.jet?'jet':'prop'):(c&&c.type==='motorcycle'?'moto':'car'));
   if(this.world.edge){this.toast('Turn back: edge of the city');this.world.edge=false}
   if(this.toastT>0&&(this.toastT-=dt)<=0)$('toast').style.display='none';
   if(this.bigT>0&&(this.bigT-=dt)<=0)$('ovl').style.display='none';this.hitT=Math.max(0,this.hitT-dt);this.mk.rotation.y=t/700;
   {const ei=.15+.7*(1-this.world.night);for(const o of this.cars){o.body.material.envMapIntensity=ei;if(o.type==='police')o.body.material.emissive.setHex(((t/160)|0)%2?0xff0000:0x0000ff)}}
   {const c=this.driving,I=c?this.world.night*2.4:0;for(let i=0;i<2;i++){const l=this.hl[i];l.intensity=I;if(c){const sn=Math.sin(c.h),cs=Math.cos(c.h),o=i?-.7:.7;l.position.set(c.x+sn*2.1+cs*o,.9,c.z+cs*2.1-sn*o);l.target.position.set(c.x+sn*30+cs*o,0,c.z+cs*30-sn*o)}}}
   this.rig.update(dt,this);this.hf=(this.hf||0)+1;if((this.hf&3)===0){this.hud();this.spHud()}
   this.fc++;this.ft+=dt;if(this.ft>.5){$('fps').textContent=Math.round(this.fc/this.ft)+' FPS';this.fc=0;this.ft=0}
   this.pf=(this.pf||0)+1;this.pt=(this.pt||0)+dt;if(this.pt>2){const fps=this.pf/this.pt;this.pf=0;this.pt=0;
    if(fps<42&&this.rs>.6){this.rs=Math.max(.6,this.rs-.1);this.applyGfx()}
    else if(fps>58&&this.rs<1){this.rs=Math.min(1,this.rs+.05);this.applyGfx()}}}
  else if(this.state==='MENU')this.rig.update(dt,this);
  if(this.state!=='PAUSED'){const f=this.driving||this.player;this.world.tick(dt,f.x,f.z,t/1000);this.lauSky()}
  this.fr++;this.r.shadowMap.needsUpdate=(this.fr&1)===0;
  if(this.mapOpen&&(!this.mpT||t-this.mpT>110)){this.mpT=t;this.drawMap()};this.world.dome.position.copy(this.cam.position);this.r.render(this.scene,this.cam);if(this._shot){this._shot=0;try{const a=document.createElement('a');a.href=this.r.domElement.toDataURL('image/png');a.download='GTA_elfo_'+Date.now()+'.png';a.click();this.toast('Screenshot saved')}catch(e){}}}}
Game=new GameCls();window.Game=Game;
})();
</script></body></html>
