[index.html](https://github.com/user-attachments/files/28448317/index.html)
<!DOCTYPE html PUBLIC "-//W3C//DTD HTML 4.01//EN" "http://www.w3.org/TR/html4/strict.dtd">
<html>
<head>
  <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
  <meta http-equiv="Content-Style-Type" content="text/css">
  <title></title>
  <meta name="Generator" content="Cocoa HTML Writer">
  <meta name="CocoaVersion" content="2685.5">
  <style type="text/css">
    p.p1 {margin: 0.0px 0.0px 0.0px 0.0px; font: 12.0px Helvetica}
    p.p2 {margin: 0.0px 0.0px 0.0px 0.0px; font: 12.0px Helvetica; min-height: 14.0px}
  </style>
</head>
<body>
<p class="p1">&lt;!DOCTYPE html&gt;</p>
<p class="p1">&lt;html lang="es"&gt;</p>
<p class="p1">&lt;head&gt;</p>
<p class="p1"><span class="Apple-converted-space">    </span>&lt;meta charset="UTF-8"&gt;</p>
<p class="p1"><span class="Apple-converted-space">    </span>&lt;meta name="viewport" content="width=device-width, initial-scale=1.0"&gt;</p>
<p class="p1"><span class="Apple-converted-space">    </span>&lt;title&gt;Helix Medic — Pitch Deck&lt;/title&gt;</p>
<p class="p1"><span class="Apple-converted-space">    </span>&lt;link href="https://fonts.googleapis.com/css2?family=Space+Grotesk:wght@300;400;500;600;700;800&amp;family=DM+Sans:ital,wght@0,300;0,400;0,500;0,600;0,700;1,400&amp;display=swap" rel="stylesheet"&gt;</p>
<p class="p1"><span class="Apple-converted-space">    </span>&lt;link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css"&gt;</p>
<p class="p1"><span class="Apple-converted-space">    </span>&lt;style&gt;</p>
<p class="p1"><span class="Apple-converted-space">        </span>:root{--bg:#060E0B;--card:#0D1F18;--accent:#00E5A0;--accent2:#FF6347;--fg:#E8F0EC;--muted:#5A7D6E;--border:#163025}</p>
<p class="p1"><span class="Apple-converted-space">        </span>*{margin:0;padding:0;box-sizing:border-box}</p>
<p class="p1"><span class="Apple-converted-space">        </span>html,body{font-family:'DM Sans',sans-serif;background:#000;color:var(--fg);overflow:hidden;height:100%;width:100%}</p>
<p class="p1"><span class="Apple-converted-space">        </span>.deck{width:100vw;height:100vh;position:relative}</p>
<p class="p2"><br></p>
<p class="p1"><span class="Apple-converted-space">        </span>.slide{</p>
<p class="p1"><span class="Apple-converted-space">            </span>position:absolute;inset:0;</p>
<p class="p1"><span class="Apple-converted-space">            </span>display:flex;align-items:center;justify-content:center;</p>
<p class="p1"><span class="Apple-converted-space">            </span>padding:60px 80px;</p>
<p class="p1"><span class="Apple-converted-space">            </span>opacity:0; transform:translateX(60px);</p>
<p class="p1"><span class="Apple-converted-space">            </span>transition:opacity 0.55s cubic-bezier(.16,1,.3,1),transform 0.55s cubic-bezier(.16,1,.3,1);</p>
<p class="p1"><span class="Apple-converted-space">            </span>pointer-events:none; overflow-y:auto;</p>
<p class="p1"><span class="Apple-converted-space">            </span>will-change:opacity,transform;</p>
<p class="p1"><span class="Apple-converted-space">        </span>}</p>
<p class="p1"><span class="Apple-converted-space">        </span>.slide.visible{opacity:1;transform:translateX(0);pointer-events:auto}</p>
<p class="p1"><span class="Apple-converted-space">        </span>.slide-inner{max-width:1100px;width:100%}</p>
<p class="p2"><br></p>
<p class="p1"><span class="Apple-converted-space">        </span>.controls{</p>
<p class="p1"><span class="Apple-converted-space">            </span>position:fixed;bottom:30px;left:50%;transform:translateX(-50%);</p>
<p class="p1"><span class="Apple-converted-space">            </span>display:flex;align-items:center;gap:16px;z-index:100;</p>
<p class="p1"><span class="Apple-converted-space">            </span>background:rgba(6,14,11,.88);backdrop-filter:blur(20px);</p>
<p class="p1"><span class="Apple-converted-space">            </span>padding:10px 20px;border-radius:40px;border:1px solid rgba(0,229,160,.1);</p>
<p class="p1"><span class="Apple-converted-space">        </span>}</p>
<p class="p1"><span class="Apple-converted-space">        </span>.ctrl-btn{</p>
<p class="p1"><span class="Apple-converted-space">            </span>width:36px;height:36px;border-radius:50%;</p>
<p class="p1"><span class="Apple-converted-space">            </span>border:1px solid rgba(0,229,160,.15);background:transparent;</p>
<p class="p1"><span class="Apple-converted-space">            </span>color:var(--muted);cursor:pointer;</p>
<p class="p1"><span class="Apple-converted-space">            </span>display:flex;align-items:center;justify-content:center;</p>
<p class="p1"><span class="Apple-converted-space">            </span>transition:all .2s;font-size:13px;</p>
<p class="p1"><span class="Apple-converted-space">        </span>}</p>
<p class="p1"><span class="Apple-converted-space">        </span>.ctrl-btn:hover{background:rgba(0,229,160,.08);color:var(--accent);border-color:rgba(0,229,160,.3)}</p>
<p class="p1"><span class="Apple-converted-space">        </span>.ctrl-btn:active{transform:scale(.9)}</p>
<p class="p1"><span class="Apple-converted-space">        </span>.slide-counter{</p>
<p class="p1"><span class="Apple-converted-space">            </span>font-family:'Space Grotesk',sans-serif;font-size:13px;font-weight:600;</p>
<p class="p1"><span class="Apple-converted-space">            </span>color:var(--muted);min-width:50px;text-align:center;</p>
<p class="p1"><span class="Apple-converted-space">        </span>}</p>
<p class="p1"><span class="Apple-converted-space">        </span>.slide-counter .cur{color:var(--accent)}</p>
<p class="p1"><span class="Apple-converted-space">        </span>.progress-bar{</p>
<p class="p1"><span class="Apple-converted-space">            </span>position:fixed;top:0;left:0;height:3px;</p>
<p class="p1"><span class="Apple-converted-space">            </span>background:linear-gradient(90deg,var(--accent),#00B8D4);</p>
<p class="p1"><span class="Apple-converted-space">            </span>transition:width .4s cubic-bezier(.16,1,.3,1);z-index:100;border-radius:0 2px 2px 0;</p>
<p class="p1"><span class="Apple-converted-space">        </span>}</p>
<p class="p2"><br></p>
<p class="p1"><span class="Apple-converted-space">        </span>.s-tag{</p>
<p class="p1"><span class="Apple-converted-space">            </span>display:inline-flex;align-items:center;gap:8px;padding:6px 16px;</p>
<p class="p1"><span class="Apple-converted-space">            </span>border-radius:20px;background:rgba(0,229,160,.06);</p>
<p class="p1"><span class="Apple-converted-space">            </span>border:1px solid rgba(0,229,160,.1);color:var(--accent);</p>
<p class="p1"><span class="Apple-converted-space">            </span>font-size:.75rem;font-weight:600;letter-spacing:.08em;text-transform:uppercase;margin-bottom:24px;</p>
<p class="p1"><span class="Apple-converted-space">        </span>}</p>
<p class="p1"><span class="Apple-converted-space">        </span>.s-title{</p>
<p class="p1"><span class="Apple-converted-space">            </span>font-family:'Space Grotesk',sans-serif;font-weight:800;</p>
<p class="p1"><span class="Apple-converted-space">            </span>font-size:clamp(2rem,4.5vw,3.8rem);line-height:1.1;</p>
<p class="p1"><span class="Apple-converted-space">            </span>margin-bottom:20px;letter-spacing:-.02em;</p>
<p class="p1"><span class="Apple-converted-space">        </span>}</p>
<p class="p1"><span class="Apple-converted-space">        </span>.s-sub{font-size:clamp(1rem,1.8vw,1.3rem);color:var(--muted);line-height:1.6;max-width:650px}</p>
<p class="p1"><span class="Apple-converted-space">        </span>.s-hl{</p>
<p class="p1"><span class="Apple-converted-space">            </span>background:linear-gradient(135deg,#00E5A0,#00B8D4);</p>
<p class="p1"><span class="Apple-converted-space">            </span>-webkit-background-clip:text;-webkit-text-fill-color:transparent;background-clip:text;</p>
<p class="p1"><span class="Apple-converted-space">        </span>}</p>
<p class="p1"><span class="Apple-converted-space">        </span>.s-big{</p>
<p class="p1"><span class="Apple-converted-space">            </span>font-family:'Space Grotesk',sans-serif;font-weight:800;</p>
<p class="p1"><span class="Apple-converted-space">            </span>font-size:clamp(4rem,10vw,8rem);line-height:1;</p>
<p class="p1"><span class="Apple-converted-space">            </span>background:linear-gradient(135deg,#00E5A0,#00B8D4);</p>
<p class="p1"><span class="Apple-converted-space">            </span>-webkit-background-clip:text;-webkit-text-fill-color:transparent;background-clip:text;</p>
<p class="p1"><span class="Apple-converted-space">        </span>}</p>
<p class="p1"><span class="Apple-converted-space">        </span>.s-source{font-size:.68rem;color:var(--muted);opacity:.7;margin-top:6px;font-style:italic}</p>
<p class="p2"><br></p>
<p class="p1"><span class="Apple-converted-space">        </span>/* Eslogan destacado */</p>
<p class="p1"><span class="Apple-converted-space">        </span>.s-eslogan{</p>
<p class="p1"><span class="Apple-converted-space">            </span>font-family:'DM Sans',sans-serif;</p>
<p class="p1"><span class="Apple-converted-space">            </span>font-size:clamp(1.1rem,1.8vw,1.35rem);</p>
<p class="p1"><span class="Apple-converted-space">            </span>font-weight:500;font-style:italic;</p>
<p class="p1"><span class="Apple-converted-space">            </span>color:var(--accent);opacity:.85;</p>
<p class="p1"><span class="Apple-converted-space">            </span>letter-spacing:.02em;margin-top:16px;</p>
<p class="p1"><span class="Apple-converted-space">            </span>text-align:center;max-width:560px;</p>
<p class="p1"><span class="Apple-converted-space">        </span>}</p>
<p class="p2"><br></p>
<p class="p1"><span class="Apple-converted-space">        </span>.sg{display:grid;gap:16px;margin-top:32px}</p>
<p class="p1"><span class="Apple-converted-space">        </span>.sg2{grid-template-columns:1fr 1fr}.sg3{grid-template-columns:1fr 1fr 1fr}.sg4{grid-template-columns:1fr 1fr 1fr 1fr}</p>
<p class="p1"><span class="Apple-converted-space">        </span>.sc{</p>
<p class="p1"><span class="Apple-converted-space">            </span>background:linear-gradient(145deg,rgba(13,31,24,.8),rgba(13,31,24,.3));</p>
<p class="p1"><span class="Apple-converted-space">            </span>border:1px solid rgba(0,229,160,.06);border-radius:16px;padding:24px;</p>
<p class="p1"><span class="Apple-converted-space">        </span>}</p>
<p class="p1"><span class="Apple-converted-space">        </span>.sc-i{</p>
<p class="p1"><span class="Apple-converted-space">            </span>width:40px;height:40px;border-radius:12px;</p>
<p class="p1"><span class="Apple-converted-space">            </span>display:flex;align-items:center;justify-content:center;margin-bottom:14px;font-size:16px;</p>
<p class="p1"><span class="Apple-converted-space">        </span>}</p>
<p class="p1"><span class="Apple-converted-space">        </span>.sc h4{font-family:'Space Grotesk',sans-serif;font-weight:700;font-size:.95rem;margin-bottom:6px}</p>
<p class="p1"><span class="Apple-converted-space">        </span>.sc p{font-size:.82rem;color:var(--muted);line-height:1.5}</p>
<p class="p2"><br></p>
<p class="p1"><span class="Apple-converted-space">        </span>.sn{font-family:'Space Grotesk',sans-serif;font-weight:800;font-size:2.8rem;line-height:1;color:var(--fg)}</p>
<p class="p1"><span class="Apple-converted-space">        </span>.sl{font-size:.82rem;color:var(--muted);margin-top:6px}</p>
<p class="p2"><br></p>
<p class="p1"><span class="Apple-converted-space">        </span>.stl{display:flex;flex-direction:column;gap:20px;margin-top:32px}</p>
<p class="p1"><span class="Apple-converted-space">        </span>.stl-i{display:flex;gap:20px;align-items:flex-start}</p>
<p class="p1"><span class="Apple-converted-space">        </span>.stl-d{</p>
<p class="p1"><span class="Apple-converted-space">            </span>width:44px;height:44px;border-radius:50%;</p>
<p class="p1"><span class="Apple-converted-space">            </span>display:flex;align-items:center;justify-content:center;flex-shrink:0;font-size:14px;</p>
<p class="p1"><span class="Apple-converted-space">        </span>}</p>
<p class="p1"><span class="Apple-converted-space">        </span>.stl-d.on{background:linear-gradient(135deg,#00E5A0,#00C28A);color:var(--bg);box-shadow:0 0 25px rgba(0,229,160,.25)}</p>
<p class="p1"><span class="Apple-converted-space">        </span>.stl-d.off{background:rgba(0,229,160,.06);border:1px solid rgba(0,229,160,.12);color:var(--muted)}</p>
<p class="p1"><span class="Apple-converted-space">        </span>.stl-c h4{font-family:'Space Grotesk',sans-serif;font-weight:700;font-size:1rem;margin-bottom:4px}</p>
<p class="p1"><span class="Apple-converted-space">        </span>.stl-c p{font-size:.85rem;color:var(--muted);line-height:1.5}</p>
<p class="p1"><span class="Apple-converted-space">        </span>.stl-t{font-family:'Space Grotesk',sans-serif;font-size:.7rem;font-weight:700;color:var(--muted);letter-spacing:.08em;text-transform:uppercase;margin-bottom:2px}</p>
<p class="p2"><br></p>
<p class="p1"><span class="Apple-converted-space">        </span>.sq{border-left:3px solid var(--accent);padding:20px 28px;margin-top:28px;background:rgba(0,229,160,.03);border-radius:0 12px 12px 0}</p>
<p class="p1"><span class="Apple-converted-space">        </span>.sq p{font-family:'Space Grotesk',sans-serif;font-weight:700;font-size:1.15rem;line-height:1.5;color:var(--accent)}</p>
<p class="p2"><br></p>
<p class="p1"><span class="Apple-converted-space">        </span>.rb{display:inline-flex;align-items:center;gap:6px;padding:6px 14px;border-radius:20px;font-weight:700;font-size:.8rem}</p>
<p class="p1"><span class="Apple-converted-space">        </span>.rb.l{background:rgba(0,229,160,.1);color:#00E5A0;border:1px solid rgba(0,229,160,.2)}</p>
<p class="p1"><span class="Apple-converted-space">        </span>.rb.m{background:rgba(255,176,32,.1);color:#FFB020;border:1px solid rgba(255,176,32,.2)}</p>
<p class="p1"><span class="Apple-converted-space">        </span>.rb.h{background:rgba(255,71,87,.1);color:#FF4757;border:1px solid rgba(255,71,87,.2)}</p>
<p class="p2"><br></p>
<p class="p1"><span class="Apple-converted-space">        </span>.slogo{display:inline-flex;align-items:center;gap:10px;margin-bottom:40px}</p>
<p class="p1"><span class="Apple-converted-space">        </span>.slogo-i{width:36px;height:36px;border-radius:10px;background:linear-gradient(135deg,#00E5A0,#00C28A);display:flex;align-items:center;justify-content:center;color:var(--bg);font-size:14px}</p>
<p class="p1"><span class="Apple-converted-space">        </span>.slogo-t{font-family:'Space Grotesk',sans-serif;font-weight:700;font-size:1.1rem}</p>
<p class="p2"><br></p>
<p class="p1"><span class="Apple-converted-space">        </span>.scover,.sclose{flex-direction:column;text-align:center}</p>
<p class="p1"><span class="Apple-converted-space">        </span>.scover{background:radial-gradient(ellipse at 50% 40%,rgba(0,229,160,.06) 0%,transparent 60%)}</p>
<p class="p1"><span class="Apple-converted-space">        </span>.sclose{background:radial-gradient(ellipse at 50% 50%,rgba(0,229,160,.05) 0%,transparent 50%)}</p>
<p class="p2"><br></p>
<p class="p1"><span class="Apple-converted-space">        </span>.sdv{width:60px;height:3px;background:linear-gradient(90deg,var(--accent),transparent);border-radius:2px;margin:20px 0}</p>
<p class="p2"><br></p>
<p class="p1"><span class="Apple-converted-space">        </span>.sflow{display:flex;align-items:center;gap:12px;margin-top:28px;flex-wrap:wrap;justify-content:center}</p>
<p class="p1"><span class="Apple-converted-space">        </span>.sflow-s{background:rgba(0,229,160,.05);border:1px solid rgba(0,229,160,.1);border-radius:12px;padding:14px 20px;text-align:center;min-width:140px}</p>
<p class="p1"><span class="Apple-converted-space">        </span>.sflow-s h5{font-family:'Space Grotesk',sans-serif;font-weight:700;font-size:.85rem;margin-bottom:4px}</p>
<p class="p1"><span class="Apple-converted-space">        </span>.sflow-s p{font-size:.72rem;color:var(--muted)}</p>
<p class="p1"><span class="Apple-converted-space">        </span>.sflow-a{color:var(--accent);font-size:18px;opacity:.4}</p>
<p class="p2"><br></p>
<p class="p1"><span class="Apple-converted-space">        </span>/* WhatsApp Mockup interactivo */</p>
<p class="p1"><span class="Apple-converted-space">        </span>.wa-mock{</p>
<p class="p1"><span class="Apple-converted-space">            </span>background:#0B1A12;border-radius:24px;padding:20px 16px;max-width:400px;margin:28px auto 0;</p>
<p class="p1"><span class="Apple-converted-space">            </span>border:1px solid rgba(0,229,160,.12);box-shadow:0 20px 40px rgba(0,0,0,.4);</p>
<p class="p1"><span class="Apple-converted-space">            </span>display:flex;flex-direction:column;height:440px;</p>
<p class="p1"><span class="Apple-converted-space">        </span>}</p>
<p class="p1"><span class="Apple-converted-space">        </span>.wa-header{display:flex;align-items:center;gap:12px;margin-bottom:16px;padding-bottom:12px;border-bottom:1px solid rgba(255,255,255,.05)}</p>
<p class="p1"><span class="Apple-converted-space">        </span>.wa-avatar{width:38px;height:38px;border-radius:50%;background:linear-gradient(135deg,#00E5A0,#00C28A);display:flex;align-items:center;justify-content:center;color:var(--bg);font-size:14px}</p>
<p class="p1"><span class="Apple-converted-space">        </span>.wa-name{font-family:'Space Grotesk',sans-serif;font-weight:700;font-size:.9rem}</p>
<p class="p1"><span class="Apple-converted-space">        </span>.wa-badge{font-size:.68rem;color:var(--accent);display:flex;align-items:center;gap:4px}</p>
<p class="p1"><span class="Apple-converted-space">        </span>.wa-body{flex:1;overflow-y:auto;display:flex;flex-direction:column;gap:10px;padding-right:4px}</p>
<p class="p1"><span class="Apple-converted-space">        </span>.wa-bubble{max-width:85%;padding:10px 14px;border-radius:16px;font-size:.82rem;line-height:1.5;position:relative}</p>
<p class="p1"><span class="Apple-converted-space">        </span>.wa-bot{background:rgba(0,229,160,.06);border:1px solid rgba(0,229,160,.1);border-radius:16px 16px 16px 4px;color:var(--fg);margin-right:auto}</p>
<p class="p1"><span class="Apple-converted-space">        </span>.wa-user{background:rgba(0,184,212,.08);border:1px solid rgba(0,184,212,.15);border-radius:16px 16px 4px 16px;color:var(--fg);margin-left:auto;text-align:right}</p>
<p class="p1"><span class="Apple-converted-space">        </span>.wa-typing{display:flex;gap:4px;align-items:center;padding:8px 14px}</p>
<p class="p1"><span class="Apple-converted-space">        </span>.wa-typing span{width:6px;height:6px;border-radius:50%;background:var(--accent);opacity:.4;animation:wa-dot 1.4s infinite}</p>
<p class="p1"><span class="Apple-converted-space">        </span>.wa-typing span:nth-child(2){animation-delay:.2s}</p>
<p class="p1"><span class="Apple-converted-space">        </span>.wa-typing span:nth-child(3){animation-delay:.4s}</p>
<p class="p1"><span class="Apple-converted-space">        </span>@keyframes wa-dot{0%,60%,100%{opacity:.4;transform:translateY(0)}30%{opacity:1;transform:translateY(-6px)}}</p>
<p class="p1"><span class="Apple-converted-space">        </span>.wa-input-row{display:flex;gap:8px;margin-top:12px;align-items:center}</p>
<p class="p1"><span class="Apple-converted-space">        </span>.wa-input{</p>
<p class="p1"><span class="Apple-converted-space">            </span>flex:1;background:rgba(255,255,255,.04);border:1px solid rgba(0,229,160,.15);</p>
<p class="p1"><span class="Apple-converted-space">            </span>border-radius:20px;padding:10px 16px;color:var(--fg);font-size:.82rem;outline:none;</p>
<p class="p1"><span class="Apple-converted-space">            </span>transition:border-color .2s;</p>
<p class="p1"><span class="Apple-converted-space">        </span>}</p>
<p class="p1"><span class="Apple-converted-space">        </span>.wa-input:focus{border-color:var(--accent)}</p>
<p class="p1"><span class="Apple-converted-space">        </span>.wa-send{</p>
<p class="p1"><span class="Apple-converted-space">            </span>width:36px;height:36px;border-radius:50%;background:var(--accent);border:none;</p>
<p class="p1"><span class="Apple-converted-space">            </span>color:var(--bg);cursor:pointer;display:flex;align-items:center;justify-content:center;</p>
<p class="p1"><span class="Apple-converted-space">            </span>font-size:14px;transition:opacity .2s;</p>
<p class="p1"><span class="Apple-converted-space">        </span>}</p>
<p class="p1"><span class="Apple-converted-space">        </span>.wa-send:disabled{opacity:.3;cursor:not-allowed}</p>
<p class="p1"><span class="Apple-converted-space">        </span>.wa-reset{</p>
<p class="p1"><span class="Apple-converted-space">            </span>font-size:.68rem;color:var(--muted);background:none;border:none;cursor:pointer;margin-left:4px;</p>
<p class="p1"><span class="Apple-converted-space">            </span>text-decoration:underline;transition:color .2s;</p>
<p class="p1"><span class="Apple-converted-space">        </span>}</p>
<p class="p1"><span class="Apple-converted-space">        </span>.wa-reset:hover{color:var(--accent)}</p>
<p class="p2"><br></p>
<p class="p1"><span class="Apple-converted-space">        </span>.fsb{</p>
<p class="p1"><span class="Apple-converted-space">            </span>position:fixed;top:20px;right:20px;z-index:100;</p>
<p class="p1"><span class="Apple-converted-space">            </span>width:36px;height:36px;border-radius:8px;</p>
<p class="p1"><span class="Apple-converted-space">            </span>border:1px solid rgba(0,229,160,.1);background:rgba(6,14,11,.8);</p>
<p class="p1"><span class="Apple-converted-space">            </span>backdrop-filter:blur(10px);color:var(--muted);cursor:pointer;</p>
<p class="p1"><span class="Apple-converted-space">            </span>display:flex;align-items:center;justify-content:center;font-size:13px;transition:all .2s;</p>
<p class="p1"><span class="Apple-converted-space">        </span>}</p>
<p class="p1"><span class="Apple-converted-space">        </span>.fsb:hover{color:var(--accent);border-color:rgba(0,229,160,.3)}</p>
<p class="p2"><br></p>
<p class="p1"><span class="Apple-converted-space">        </span>.qr{width:80px;height:80px;background:rgba(0,229,160,.05);border:1px solid rgba(0,229,160,.15);border-radius:12px;display:flex;align-items:center;justify-content:center;margin:20px auto 0;font-size:2rem;color:var(--accent)}</p>
<p class="p2"><br></p>
<p class="p1"><span class="Apple-converted-space">        </span>@media(max-width:768px){</p>
<p class="p1"><span class="Apple-converted-space">            </span>.slide{padding:40px 28px}</p>
<p class="p1"><span class="Apple-converted-space">            </span>.sg2,.sg3,.sg4{grid-template-columns:1fr}</p>
<p class="p1"><span class="Apple-converted-space">            </span>.sflow{flex-direction:column}</p>
<p class="p1"><span class="Apple-converted-space">            </span>.sflow-a{transform:rotate(90deg)}</p>
<p class="p1"><span class="Apple-converted-space">            </span>.controls{bottom:16px;padding:8px 14px;gap:10px}</p>
<p class="p1"><span class="Apple-converted-space">        </span>}</p>
<p class="p1"><span class="Apple-converted-space">        </span>@media(prefers-reduced-motion:reduce){</p>
<p class="p1"><span class="Apple-converted-space">            </span>.slide{transition-duration:.01ms!important;transform:none!important}</p>
<p class="p1"><span class="Apple-converted-space">        </span>}</p>
<p class="p1"><span class="Apple-converted-space">    </span>&lt;/style&gt;</p>
<p class="p1">&lt;/head&gt;</p>
<p class="p1">&lt;body&gt;</p>
<p class="p2"><br></p>
<p class="p1">&lt;div class="progress-bar" id="pb"&gt;&lt;/div&gt;</p>
<p class="p1">&lt;button class="fsb" onclick="toggleFS()" title="Pantalla completa" aria-label="Pantalla completa"&gt;&lt;i class="fa-solid fa-expand"&gt;&lt;/i&gt;&lt;/button&gt;</p>
<p class="p2"><br></p>
<p class="p1">&lt;div class="deck" id="deck"&gt;</p>
<p class="p2"><br></p>
<p class="p1"><span class="Apple-converted-space">    </span>&lt;!-- SLIDE 1: PORTADA --&gt;</p>
<p class="p1"><span class="Apple-converted-space">    </span>&lt;div class="slide scover visible" data-i="0"&gt;</p>
<p class="p1"><span class="Apple-converted-space">        </span>&lt;div class="slide-inner" style="display:flex;flex-direction:column;align-items:center;"&gt;</p>
<p class="p1"><span class="Apple-converted-space">            </span>&lt;div class="slogo"&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;div class="slogo-i"&gt;&lt;i class="fa-solid fa-dna"&gt;&lt;/i&gt;&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;div class="slogo-t"&gt;Helix&lt;span style="color:var(--accent)"&gt;Medic&lt;/span&gt;&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">            </span>&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">            </span>&lt;h1 class="s-title"&gt;El primer &lt;span class="s-hl"&gt;filtro médico digital&lt;/span&gt; para Latinoamérica&lt;/h1&gt;</p>
<p class="p1"><span class="Apple-converted-space">            </span>&lt;p class="s-sub" style="text-align:center;max-width:560px;margin-top:12px;"&gt;Evaluación clínica con IA en WhatsApp que conecta a pacientes con la atención correcta, en el momento correcto.&lt;/p&gt;</p>
<p class="p1"><span class="Apple-converted-space">            </span>&lt;p class="s-eslogan"&gt;"Tu bienestar a un mensaje de distancia"&lt;/p&gt;</p>
<p class="p1"><span class="Apple-converted-space">            </span>&lt;div style="margin-top:48px;display:flex;align-items:center;gap:8px;color:var(--muted);font-size:.85rem;"&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;i class="fa-solid fa-arrow-right" style="color:var(--accent);font-size:11px;"&gt;&lt;/i&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>Presiona &lt;kbd style="background:rgba(0,229,160,.08);border:1px solid rgba(0,229,160,.15);border-radius:6px;padding:2px 8px;font-family:'Space Grotesk';font-size:.8rem;color:var(--accent);"&gt;→&lt;/kbd&gt; para avanzar</p>
<p class="p1"><span class="Apple-converted-space">            </span>&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">        </span>&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">    </span>&lt;/div&gt;</p>
<p class="p2"><br></p>
<p class="p1"><span class="Apple-converted-space">    </span>&lt;!-- SLIDE 2: PROBLEMA --&gt;</p>
<p class="p1"><span class="Apple-converted-space">    </span>&lt;div class="slide" data-i="1"&gt;</p>
<p class="p1"><span class="Apple-converted-space">        </span>&lt;div class="slide-inner"&gt;</p>
<p class="p1"><span class="Apple-converted-space">            </span>&lt;div class="s-tag"&gt;El Problema&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">            </span>&lt;h1 class="s-title"&gt;El primer contacto médico&lt;br&gt;no es un doctor&lt;/h1&gt;</p>
<p class="p1"><span class="Apple-converted-space">            </span>&lt;p class="s-sub"&gt;Es Google. Es una farmacia. Es un vecino. Y para cuando el paciente llega al hospital, ya es tarde.&lt;/p&gt;</p>
<p class="p1"><span class="Apple-converted-space">            </span>&lt;div class="sg sg3" style="margin-top:40px;"&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;div class="sc"&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;div class="sc-i" style="background:rgba(255,99,71,.1);color:var(--accent2);"&gt;&lt;i class="fa-solid fa-hospital"&gt;&lt;/i&gt;&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;h4&gt;Urgencias colapsadas&lt;/h4&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;p&gt;El 70% de las visitas a urgencias podrían resolverse en primer nivel de atención.&lt;/p&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;p class="s-source"&gt;Secretaría de Salud, 2023&lt;/p&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;div class="sc"&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;div class="sc-i" style="background:rgba(255,99,71,.1);color:var(--accent2);"&gt;&lt;i class="fa-solid fa-coins"&gt;&lt;/i&gt;&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;h4&gt;Gasto de bolsillo extremo&lt;/h4&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;p&gt;Los mexicanos pagan de su bolsillo el 40.6% del gasto en salud, el doble del promedio OCDE.&lt;/p&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;p class="s-source"&gt;OCDE Health Statistics, 2023&lt;/p&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;div class="sc"&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;div class="sc-i" style="background:rgba(255,99,71,.1);color:var(--accent2);"&gt;&lt;i class="fa-solid fa-magnifying-glass"&gt;&lt;/i&gt;&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;h4&gt;Autodiagnóstico peligroso&lt;/h4&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;p&gt;El 72% de los mexicanos busca en internet antes de ir al médico, sin filtro clínico.&lt;/p&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;p class="s-source"&gt;INEGI ENIGH, 2022&lt;/p&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">            </span>&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">        </span>&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">    </span>&lt;/div&gt;</p>
<p class="p2"><br></p>
<p class="p1"><span class="Apple-converted-space">    </span>&lt;!-- SLIDE 3: DATOS --&gt;</p>
<p class="p1"><span class="Apple-converted-space">    </span>&lt;div class="slide" data-i="2"&gt;</p>
<p class="p1"><span class="Apple-converted-space">        </span>&lt;div class="slide-inner" style="display:flex;align-items:center;gap:80px;flex-wrap:wrap;"&gt;</p>
<p class="p1"><span class="Apple-converted-space">            </span>&lt;div style="flex:1;min-width:280px;"&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;div class="s-tag"&gt;Contexto&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;h1 class="s-title"&gt;El sistema de salud&lt;br&gt;perdió su filtro&lt;/h1&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;p class="s-sub"&gt;México tiene 2.4 médicos por cada 1,000 habitantes, muy por debajo del promedio OCDE de 3.7. No existe un primer nivel digital que evalúe antes de saturar hospitales.&lt;/p&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;div class="sdv" style="margin-left:0;"&gt;&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;p style="font-size:.88rem;color:var(--muted);line-height:1.6;max-width:420px;"&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>Según el CONEVAL, alrededor del 50% de la población carece de acceso efectivo a servicios de salud. Cuando alguien enferma, no tiene a quién consultar antes de que el caso se complique.</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;/p&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;p class="s-source" style="margin-top:10px;"&gt;CONEVAL 2022, INEGI ENADEP 2022&lt;/p&gt;</p>
<p class="p1"><span class="Apple-converted-space">            </span>&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">            </span>&lt;div style="flex:0 0 auto;text-align:center;"&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;div class="s-big"&gt;~50%&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;p class="sl"&gt;sin acceso regular&lt;br&gt;a servicios de salud&lt;/p&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;p class="s-source"&gt;CONEVAL, 2022&lt;/p&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;div style="margin-top:36px;"&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;div style="font-family:'Space Grotesk';font-weight:800;font-size:2.2rem;color:var(--fg);"&gt;2.4&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;p class="sl"&gt;médicos por cada&lt;br&gt;1,000 habitantes&lt;/p&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;p class="s-source"&gt;OCDE Health at a Glance&lt;/p&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">            </span>&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">        </span>&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">    </span>&lt;/div&gt;</p>
<p class="p2"><br></p>
<p class="p1"><span class="Apple-converted-space">    </span>&lt;!-- SLIDE 4: SOLUCION --&gt;</p>
<p class="p1"><span class="Apple-converted-space">    </span>&lt;div class="slide" data-i="3"&gt;</p>
<p class="p1"><span class="Apple-converted-space">        </span>&lt;div class="slide-inner"&gt;</p>
<p class="p1"><span class="Apple-converted-space">            </span>&lt;div class="s-tag"&gt;La Solución&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">            </span>&lt;h1 class="s-title"&gt;Helix Medic&lt;br&gt;&lt;span class="s-hl"&gt;Evaluación clínica con IA en WhatsApp&lt;/span&gt;&lt;/h1&gt;</p>
<p class="p1"><span class="Apple-converted-space">            </span>&lt;p class="s-sub"&gt;Sin apps. Sin descargas. Sin formularios. El paciente describe sus síntomas y el sistema evalúa, clasifica y conecta con la atención correcta.&lt;/p&gt;</p>
<p class="p1"><span class="Apple-converted-space">            </span>&lt;div class="sflow"&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;div class="sflow-s"&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;h5&gt;&lt;i class="fa-solid fa-comment-medical" style="color:var(--accent);margin-right:4px;"&gt;&lt;/i&gt; Síntomas&lt;/h5&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;p&gt;Voz o texto en lenguaje natural&lt;/p&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;div class="sflow-a"&gt;&lt;i class="fa-solid fa-arrow-right"&gt;&lt;/i&gt;&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;div class="sflow-s"&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;h5&gt;&lt;i class="fa-solid fa-brain" style="color:var(--accent);margin-right:4px;"&gt;&lt;/i&gt; IA evalúa&lt;/h5&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;p&gt;Clasifica riesgo en 3 niveles&lt;/p&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;div class="sflow-a"&gt;&lt;i class="fa-solid fa-arrow-right"&gt;&lt;/i&gt;&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;div class="sflow-s"&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;h5&gt;&lt;i class="fa-solid fa-user-doctor" style="color:var(--accent);margin-right:4px;"&gt;&lt;/i&gt; Conecta&lt;/h5&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;p&gt;Doctor, farmacia o urgencias&lt;/p&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">            </span>&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">            </span>&lt;div class="sq" style="margin-top:40px;"&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;p&gt;"No reemplazamos doctores. Los hacemos más eficientes."&lt;/p&gt;</p>
<p class="p1"><span class="Apple-converted-space">            </span>&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">        </span>&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">    </span>&lt;/div&gt;</p>
<p class="p2"><br></p>
<p class="p1"><span class="Apple-converted-space">    </span>&lt;!-- SLIDE 5: COMO FUNCIONA --&gt;</p>
<p class="p1"><span class="Apple-converted-space">    </span>&lt;div class="slide" data-i="4"&gt;</p>
<p class="p1"><span class="Apple-converted-space">        </span>&lt;div class="slide-inner"&gt;</p>
<p class="p1"><span class="Apple-converted-space">            </span>&lt;div class="s-tag"&gt;Producto&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">            </span>&lt;h1 class="s-title"&gt;Así funciona en 4 minutos&lt;/h1&gt;</p>
<p class="p1"><span class="Apple-converted-space">            </span>&lt;div class="sg sg2" style="margin-top:36px;"&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;div class="sc" style="border-left:3px solid var(--accent);"&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;div style="font-family:'Space Grotesk';font-weight:800;font-size:.7rem;color:var(--accent);letter-spacing:.1em;margin-bottom:10px;"&gt;PASO 01&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;h4&gt;Paciente describe síntomas&lt;/h4&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;p&gt;"Tengo fiebre y dolor de garganta desde hace 3 días"&lt;/p&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;div class="sc" style="border-left:3px solid var(--accent);"&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;div style="font-family:'Space Grotesk';font-weight:800;font-size:.7rem;color:var(--accent);letter-spacing:.1em;margin-bottom:10px;"&gt;PASO 02&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;h4&gt;Helix pregunta datos clave&lt;/h4&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;p&gt;Edad, duración, síntomas adicionales — en lenguaje conversacional&lt;/p&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;div class="sc" style="border-left:3px solid var(--accent);"&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;div style="font-family:'Space Grotesk';font-weight:800;font-size:.7rem;color:var(--accent);letter-spacing:.1em;margin-bottom:10px;"&gt;PASO 03&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;h4&gt;Clasificación de riesgo&lt;/h4&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;div style="display:flex;gap:8px;margin-top:8px;"&gt;</p>
<p class="p1"><span class="Apple-converted-space">                        </span>&lt;span class="rb l"&gt;&lt;i class="fa-solid fa-circle" style="font-size:5px;"&gt;&lt;/i&gt; Bajo&lt;/span&gt;</p>
<p class="p1"><span class="Apple-converted-space">                        </span>&lt;span class="rb m"&gt;&lt;i class="fa-solid fa-circle" style="font-size:5px;"&gt;&lt;/i&gt; Medio&lt;/span&gt;</p>
<p class="p1"><span class="Apple-converted-space">                        </span>&lt;span class="rb h"&gt;&lt;i class="fa-solid fa-circle" style="font-size:5px;"&gt;&lt;/i&gt; Alto&lt;/span&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;div class="sc" style="border-left:3px solid #06B6D4;"&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;div style="font-family:'Space Grotesk';font-weight:800;font-size:.7rem;color:#06B6D4;letter-spacing:.1em;margin-bottom:10px;"&gt;PASO 04&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;h4&gt;Conexión con doctor real&lt;/h4&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;p&gt;El doctor recibe el caso, se une al mismo chat de WhatsApp y atiende al paciente sin salir de la app.&lt;/p&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">            </span>&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">        </span>&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">    </span>&lt;/div&gt;</p>
<p class="p2"><br></p>
<p class="p1"><span class="Apple-converted-space">    </span>&lt;!-- SLIDE 6: DEMO INTERACTIVA --&gt;</p>
<p class="p1"><span class="Apple-converted-space">    </span>&lt;div class="slide" data-i="5" id="demo-slide"&gt;</p>
<p class="p1"><span class="Apple-converted-space">        </span>&lt;div class="slide-inner" style="display:flex;align-items:center;gap:60px;flex-wrap:wrap;"&gt;</p>
<p class="p1"><span class="Apple-converted-space">            </span>&lt;div style="flex:1;min-width:280px;"&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;div class="s-tag"&gt;Demo en vivo&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;h1 class="s-title"&gt;Interactúa con&lt;br&gt;&lt;span class="s-hl"&gt;Helix Medic ahora&lt;/span&gt;&lt;/h1&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;p class="s-sub" style="max-width:500px;"&gt;Escribe tus síntomas en el chat y experimenta la evaluación clínica. El médico se une a la conversación en el mismo chat.&lt;/p&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;div style="margin-top:24px;display:flex;gap:12px;flex-wrap:wrap;"&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;div class="rb l"&gt;✅ Evaluación en 4 min&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;div class="rb m"&gt;✅ Doctor en el chat&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;button class="wa-reset" onclick="resetDemo()" style="margin-top:16px;font-size:.8rem;"&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;i class="fa-solid fa-rotate-left"&gt;&lt;/i&gt; Reiniciar demo</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;/button&gt;</p>
<p class="p1"><span class="Apple-converted-space">            </span>&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">            </span>&lt;div class="wa-mock" id="wa-mock"&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;div class="wa-header"&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;div class="wa-avatar"&gt;&lt;i class="fa-solid fa-dna"&gt;&lt;/i&gt;&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;div&gt;</p>
<p class="p1"><span class="Apple-converted-space">                        </span>&lt;div class="wa-name"&gt;Helix Medic&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">                        </span>&lt;div class="wa-badge"&gt;&lt;i class="fa-solid fa-circle" style="font-size:5px;"&gt;&lt;/i&gt; en línea&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;div class="wa-body" id="wa-body"&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;div class="wa-bubble wa-bot"&gt;🩺 *Helix Medic* — Recuerda: soy un asistente de orientación clínica. Para comenzar, dime ¿qué síntomas tienes?&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;div class="wa-input-row"&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;input class="wa-input" id="wa-input" placeholder="Escribe un mensaje..." autocomplete="off" onkeydown="handleDemoKey(event)"&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;button class="wa-send" id="wa-send" onclick="handleDemoSend()"&gt;&lt;i class="fa-solid fa-paper-plane"&gt;&lt;/i&gt;&lt;/button&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">            </span>&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">        </span>&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">    </span>&lt;/div&gt;</p>
<p class="p2"><br></p>
<p class="p1"><span class="Apple-converted-space">    </span>&lt;!-- SLIDE 7: MODELO DE NEGOCIO --&gt;</p>
<p class="p1"><span class="Apple-converted-space">    </span>&lt;div class="slide" data-i="6"&gt;</p>
<p class="p1"><span class="Apple-converted-space">        </span>&lt;div class="slide-inner"&gt;</p>
<p class="p1"><span class="Apple-converted-space">            </span>&lt;div class="s-tag"&gt;Modelo de Negocio&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">            </span>&lt;h1 class="s-title"&gt;Ingresos desde el día uno&lt;/h1&gt;</p>
<p class="p1"><span class="Apple-converted-space">            </span>&lt;p class="s-sub"&gt;B2B: farmacias y clínicas pagan por cada paciente evaluado y conectado. El gasto de bolsillo en salud en México supera los $900 mil millones MXN al año.&lt;/p&gt;</p>
<p class="p1"><span class="Apple-converted-space">            </span>&lt;p class="s-source" style="margin-top:-16px;margin-bottom:8px;"&gt;OCDE, Banco Mundial, 2023&lt;/p&gt;</p>
<p class="p1"><span class="Apple-converted-space">            </span>&lt;div class="sg sg3" style="margin-top:28px;"&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;div class="sc"&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;div style="font-family:'Space Grotesk';font-weight:800;font-size:.7rem;color:var(--muted);letter-spacing:.08em;margin-bottom:8px;"&gt;OPCION 1 — ARRANQUE&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;div style="font-family:'Space Grotesk';font-weight:800;font-size:2rem;line-height:1;margin-bottom:4px;"&gt;$2-5&lt;span style="font-size:.9rem;font-weight:400;color:var(--muted);"&gt; MXN&lt;/span&gt;&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;p style="font-size:.85rem;color:var(--muted);margin-bottom:16px;"&gt;Por paciente evaluado&lt;/p&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;ul style="list-style:none;font-size:.82rem;color:var(--fg);display:flex;flex-direction:column;gap:8px;"&gt;</p>
<p class="p1"><span class="Apple-converted-space">                        </span>&lt;li&gt;&lt;i class="fa-solid fa-check" style="color:var(--accent);font-size:10px;margin-right:8px;"&gt;&lt;/i&gt;Pago por uso, sin riesgo&lt;/li&gt;</p>
<p class="p1"><span class="Apple-converted-space">                        </span>&lt;li&gt;&lt;i class="fa-solid fa-check" style="color:var(--accent);font-size:10px;margin-right:8px;"&gt;&lt;/i&gt;Farmacias pequeñas&lt;/li&gt;</p>
<p class="p1"><span class="Apple-converted-space">                        </span>&lt;li&gt;&lt;i class="fa-solid fa-check" style="color:var(--accent);font-size:10px;margin-right:8px;"&gt;&lt;/i&gt;Escala con volumen&lt;/li&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;/ul&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;div class="sc" style="border-color:rgba(0,229,160,.2);background:linear-gradient(160deg,rgba(0,229,160,.04),rgba(13,31,24,.5));"&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;div style="font-family:'Space Grotesk';font-weight:800;font-size:.7rem;color:var(--accent);letter-spacing:.08em;margin-bottom:8px;"&gt;OPCION 2 — ESCALA&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;div style="font-family:'Space Grotesk';font-weight:800;font-size:2rem;line-height:1;margin-bottom:4px;"&gt;$300-1k&lt;span style="font-size:.9rem;font-weight:400;color:var(--muted);"&gt; MXN&lt;/span&gt;&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;p style="font-size:.85rem;color:var(--muted);margin-bottom:16px;"&gt;Por negocio al mes&lt;/p&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;ul style="list-style:none;font-size:.82rem;color:var(--fg);display:flex;flex-direction:column;gap:8px;"&gt;</p>
<p class="p1"><span class="Apple-converted-space">                        </span>&lt;li&gt;&lt;i class="fa-solid fa-check" style="color:var(--accent);font-size:10px;margin-right:8px;"&gt;&lt;/i&gt;Evaluaciones ilimitadas&lt;/li&gt;</p>
<p class="p1"><span class="Apple-converted-space">                        </span>&lt;li&gt;&lt;i class="fa-solid fa-check" style="color:var(--accent);font-size:10px;margin-right:8px;"&gt;&lt;/i&gt;Dashboard de métricas&lt;/li&gt;</p>
<p class="p1"><span class="Apple-converted-space">                        </span>&lt;li&gt;&lt;i class="fa-solid fa-check" style="color:var(--accent);font-size:10px;margin-right:8px;"&gt;&lt;/i&gt;Integración inventario&lt;/li&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;/ul&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;div class="sc"&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;div style="font-family:'Space Grotesk';font-weight:800;font-size:.7rem;color:var(--muted);letter-spacing:.08em;margin-bottom:8px;"&gt;OPCION 3 — FUTURO&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;div style="font-family:'Space Grotesk';font-weight:800;font-size:2rem;line-height:1;margin-bottom:4px;"&gt;Data&lt;span style="font-size:.9rem;font-weight:400;color:var(--muted);"&gt; Analytics&lt;/span&gt;&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;p style="font-size:.85rem;color:var(--muted);margin-bottom:16px;"&gt;Aseguradoras y gobiernos&lt;/p&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;ul style="list-style:none;font-size:.82rem;color:var(--fg);display:flex;flex-direction:column;gap:8px;"&gt;</p>
<p class="p1"><span class="Apple-converted-space">                        </span>&lt;li&gt;&lt;i class="fa-solid fa-check" style="color:var(--accent);font-size:10px;margin-right:8px;"&gt;&lt;/i&gt;Datos epidemiológicos&lt;/li&gt;</p>
<p class="p1"><span class="Apple-converted-space">                        </span>&lt;li&gt;&lt;i class="fa-solid fa-check" style="color:var(--accent);font-size:10px;margin-right:8px;"&gt;&lt;/i&gt;Mapas de calor&lt;/li&gt;</p>
<p class="p1"><span class="Apple-converted-space">                        </span>&lt;li&gt;&lt;i class="fa-solid fa-check" style="color:var(--accent);font-size:10px;margin-right:8px;"&gt;&lt;/i&gt;Predicción de brotes&lt;/li&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;/ul&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">            </span>&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">        </span>&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">    </span>&lt;/div&gt;</p>
<p class="p2"><br></p>
<p class="p1"><span class="Apple-converted-space">    </span>&lt;!-- SLIDE 8: VALIDACIÓN (ACTUALIZADA: EN CONSTRUCCIÓN) --&gt;</p>
<p class="p1"><span class="Apple-converted-space">    </span>&lt;div class="slide" data-i="7"&gt;</p>
<p class="p1"><span class="Apple-converted-space">        </span>&lt;div class="slide-inner" style="display:flex;flex-direction:column;align-items:center;text-align:center;"&gt;</p>
<p class="p1"><span class="Apple-converted-space">            </span>&lt;div class="s-tag"&gt;Validación&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">            </span>&lt;h1 class="s-title"&gt;Fase de construcción&lt;/h1&gt;</p>
<p class="p1"><span class="Apple-converted-space">            </span>&lt;p class="s-sub" style="max-width:600px;"&gt;Actualmente nos encontramos afinando la tecnología y preparando el despliegue con las primeras farmacias piloto. La validación en campo comenzará próximamente.&lt;/p&gt;</p>
<p class="p1"><span class="Apple-converted-space">            </span>&lt;div class="sg sg3" style="margin-top:40px;max-width:800px;"&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;div class="sc" style="text-align:center;"&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;div class="sc-i" style="background:rgba(0,229,160,.1);color:var(--accent);margin:0 auto 14px;"&gt;&lt;i class="fa-solid fa-gear"&gt;&lt;/i&gt;&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;h4&gt;Backend operativo&lt;/h4&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;p&gt;Infraestructura tecnológica lista y funcionando en pruebas internas.&lt;/p&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;div class="sc" style="text-align:center;"&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;div class="sc-i" style="background:rgba(0,229,160,.1);color:var(--accent);margin:0 auto 14px;"&gt;&lt;i class="fa-solid fa-robot"&gt;&lt;/i&gt;&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;h4&gt;IA entrenada&lt;/h4&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;p&gt;Modelo de clasificación de riesgo afinado con datos clínicos en español.&lt;/p&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;div class="sc" style="text-align:center;"&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;div class="sc-i" style="background:rgba(0,229,160,.1);color:var(--accent);margin:0 auto 14px;"&gt;&lt;i class="fa-solid fa-store"&gt;&lt;/i&gt;&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;h4&gt;Próximamente&lt;/h4&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;p&gt;Piloto con farmacias para validar métricas de uso, precisión y satisfacción.&lt;/p&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">            </span>&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">            </span>&lt;div class="sq" style="margin-top:36px;"&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;p&gt;"La validación no es un requisito. Es la prueba de que esto ya está pasando."&lt;/p&gt;</p>
<p class="p1"><span class="Apple-converted-space">            </span>&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">        </span>&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">    </span>&lt;/div&gt;</p>
<p class="p2"><br></p>
<p class="p1"><span class="Apple-converted-space">    </span>&lt;!-- SLIDE 9: MERCADO --&gt;</p>
<p class="p1"><span class="Apple-converted-space">    </span>&lt;div class="slide" data-i="8"&gt;</p>
<p class="p1"><span class="Apple-converted-space">        </span>&lt;div class="slide-inner" style="display:flex;align-items:center;gap:80px;flex-wrap:wrap;"&gt;</p>
<p class="p1"><span class="Apple-converted-space">            </span>&lt;div style="flex:1;min-width:300px;"&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;div class="s-tag"&gt;Mercado&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;h1 class="s-title"&gt;Oportunidad masiva en México&lt;/h1&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;p class="s-sub"&gt;México tiene 128.9 millones de habitantes, 96% de penetración de smartphones, y un sistema de salud que necesita desesperadamente un filtro digital.&lt;/p&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;div style="margin-top:32px;display:flex;flex-direction:column;gap:18px;"&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;div style="display:flex;align-items:baseline;gap:12px;"&gt;</p>
<p class="p1"><span class="Apple-converted-space">                        </span>&lt;span style="font-family:'Space Grotesk';font-weight:800;font-size:1.8rem;color:var(--fg);"&gt;128.9M&lt;/span&gt;</p>
<p class="p1"><span class="Apple-converted-space">                        </span>&lt;span style="font-size:.85rem;color:var(--muted);"&gt;habitantes en México&lt;/span&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;div style="display:flex;align-items:baseline;gap:12px;"&gt;</p>
<p class="p1"><span class="Apple-converted-space">                        </span>&lt;span style="font-family:'Space Grotesk';font-weight:800;font-size:1.8rem;color:var(--fg);"&gt;96%&lt;/span&gt;</p>
<p class="p1"><span class="Apple-converted-space">                        </span>&lt;span style="font-size:.85rem;color:var(--muted);"&gt;penetración de smartphones&lt;/span&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;div style="display:flex;align-items:baseline;gap:12px;"&gt;</p>
<p class="p1"><span class="Apple-converted-space">                        </span>&lt;span style="font-family:'Space Grotesk';font-weight:800;font-size:1.8rem;color:var(--fg);"&gt;98.6M&lt;/span&gt;</p>
<p class="p1"><span class="Apple-converted-space">                        </span>&lt;span style="font-size:.85rem;color:var(--muted);"&gt;usuarios de WhatsApp&lt;/span&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;div style="display:flex;align-items:baseline;gap:12px;"&gt;</p>
<p class="p1"><span class="Apple-converted-space">                        </span>&lt;span style="font-family:'Space Grotesk';font-weight:800;font-size:1.8rem;color:var(--accent);"&gt;$52B&lt;/span&gt;</p>
<p class="p1"><span class="Apple-converted-space">                        </span>&lt;span style="font-size:.85rem;color:var(--muted);"&gt;MXN gasto en salud al año&lt;/span&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;p class="s-source" style="margin-top:8px;"&gt;INEGI Censo 2020, ITU 2023, OMS 2023, OCDE 2023&lt;/p&gt;</p>
<p class="p1"><span class="Apple-converted-space">            </span>&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">            </span>&lt;div style="flex:0 0 auto;"&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;div class="sc" style="width:300px;padding:32px;text-align:center;border-color:rgba(0,229,160,.15);"&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;p style="font-size:.85rem;color:var(--muted);line-height:1.7;"&gt;WhatsApp es la app más usada en México. No necesitamos convencer a nadie de descargar algo nuevo — el canal ya existe.&lt;/p&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;div style="margin-top:20px;"&gt;</p>
<p class="p1"><span class="Apple-converted-space">                        </span>&lt;i class="fa-brands fa-whatsapp" style="font-size:40px;color:var(--accent);opacity:.3;"&gt;&lt;/i&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">            </span>&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">        </span>&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">    </span>&lt;/div&gt;</p>
<p class="p2"><br></p>
<p class="p1"><span class="Apple-converted-space">    </span>&lt;!-- SLIDE 10: VENTAJA COMPETITIVA --&gt;</p>
<p class="p1"><span class="Apple-converted-space">    </span>&lt;div class="slide" data-i="9"&gt;</p>
<p class="p1"><span class="Apple-converted-space">        </span>&lt;div class="slide-inner" style="display:flex;align-items:center;gap:80px;flex-wrap:wrap;"&gt;</p>
<p class="p1"><span class="Apple-converted-space">            </span>&lt;div style="flex:1;min-width:300px;"&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;div class="s-tag"&gt;Moat&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;h1 class="s-title"&gt;Ventaja competitiva&lt;/h1&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;p class="s-sub"&gt;Lo que nos hace difíciles de copiar.&lt;/p&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;div class="sdv" style="margin-left:0;"&gt;&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;div style="margin-top:24px;display:flex;flex-direction:column;gap:24px;"&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;div&gt;</p>
<p class="p1"><span class="Apple-converted-space">                        </span>&lt;div style="font-family:'Space Grotesk';font-weight:800;font-size:1.1rem;color:var(--accent);margin-bottom:6px;"&gt;Datos&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">                        </span>&lt;p style="font-size:.88rem;color:var(--muted);line-height:1.6;"&gt;El dataset más grande de síntomas reales en español de LATAM. Cada evaluación alimenta y mejora el modelo. Los competidores no tienen acceso a estos datos.&lt;/p&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;div&gt;</p>
<p class="p1"><span class="Apple-converted-space">                        </span>&lt;div style="font-family:'Space Grotesk';font-weight:800;font-size:1.1rem;color:var(--accent);margin-bottom:6px;"&gt;Distribución&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">                        </span>&lt;p style="font-size:.88rem;color:var(--muted);line-height:1.6;"&gt;Red de farmacias socias como canal. No dependemos de marketing digital ni de app stores. La farmacia es el punto de venta.&lt;/p&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;div&gt;</p>
<p class="p1"><span class="Apple-converted-space">                        </span>&lt;div style="font-family:'Space Grotesk';font-weight:800;font-size:1.1rem;color:var(--accent);margin-bottom:6px;"&gt;Experiencia sin fricción&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">                        </span>&lt;p style="font-size:.88rem;color:var(--muted);line-height:1.6;"&gt;El paciente nunca sale de WhatsApp. El doctor se une al mismo chat. Sin instalar apps, sin compartir números externos. Una experiencia fluida que nadie más ofrece.&lt;/p&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">            </span>&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">            </span>&lt;div style="flex:0 0 auto;"&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;div class="sc" style="width:280px;padding:32px;text-align:center;"&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;div style="width:64px;height:64px;border-radius:20px;background:rgba(0,229,160,.08);display:flex;align-items:center;justify-content:center;margin:0 auto 20px;"&gt;</p>
<p class="p1"><span class="Apple-converted-space">                        </span>&lt;i class="fa-solid fa-chess-queen" style="color:var(--accent);font-size:24px;"&gt;&lt;/i&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;p style="font-size:.85rem;color:var(--muted);line-height:1.6;"&gt;Cada nueva evaluación hace el producto más inteligente. El efecto red de datos crea una barrera que crece sola.&lt;/p&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">            </span>&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">        </span>&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">    </span>&lt;/div&gt;</p>
<p class="p2"><br></p>
<p class="p1"><span class="Apple-converted-space">    </span>&lt;!-- SLIDE 11: ROADMAP --&gt;</p>
<p class="p1"><span class="Apple-converted-space">    </span>&lt;div class="slide" data-i="10"&gt;</p>
<p class="p1"><span class="Apple-converted-space">        </span>&lt;div class="slide-inner"&gt;</p>
<p class="p1"><span class="Apple-converted-space">            </span>&lt;div class="s-tag"&gt;Roadmap&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">            </span>&lt;h1 class="s-title"&gt;Cómo se vuelve gigante&lt;/h1&gt;</p>
<p class="p1"><span class="Apple-converted-space">            </span>&lt;div class="stl"&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;div class="stl-i"&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;div class="stl-d on"&gt;&lt;i class="fa-brands fa-whatsapp"&gt;&lt;/i&gt;&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;div class="stl-c"&gt;</p>
<p class="p1"><span class="Apple-converted-space">                        </span>&lt;div class="stl-t"&gt;Fase 1 — Completada&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">                        </span>&lt;h4&gt;Evaluación + Doctor en WhatsApp&lt;/h4&gt;</p>
<p class="p1"><span class="Apple-converted-space">                        </span>&lt;p&gt;Bot de evaluación clínica con conexión en tiempo real a doctores generales dentro del mismo chat. Próximamente piloto con farmacias.&lt;/p&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;div class="stl-i"&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;div class="stl-d off"&gt;&lt;i class="fa-solid fa-store"&gt;&lt;/i&gt;&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;div class="stl-c"&gt;</p>
<p class="p1"><span class="Apple-converted-space">                        </span>&lt;div class="stl-t"&gt;Fase 2 — 6 meses&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">                        </span>&lt;h4&gt;Integración con farmacias&lt;/h4&gt;</p>
<p class="p1"><span class="Apple-converted-space">                        </span>&lt;p&gt;Derivación directa con catálogo de productos, geolocalización y margen por venta referenciada.&lt;/p&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;div class="stl-i"&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;div class="stl-d off"&gt;&lt;i class="fa-solid fa-file-medical"&gt;&lt;/i&gt;&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;div class="stl-c"&gt;</p>
<p class="p1"><span class="Apple-converted-space">                        </span>&lt;div class="stl-t"&gt;Fase 3 — 12 meses&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">                        </span>&lt;h4&gt;Historial médico personal&lt;/h4&gt;</p>
<p class="p1"><span class="Apple-converted-space">                        </span>&lt;p&gt;Perfil de salud con historial de evaluaciones, tendencias y recordatorios de seguimiento automático.&lt;/p&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;div class="stl-i"&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;div class="stl-d off"&gt;&lt;i class="fa-solid fa-chart-line"&gt;&lt;/i&gt;&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;div class="stl-c"&gt;</p>
<p class="p1"><span class="Apple-converted-space">                        </span>&lt;div class="stl-t"&gt;Fase 4 — 18+ meses&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">                        </span>&lt;h4&gt;IA predictiva y data para aseguradoras&lt;/h4&gt;</p>
<p class="p1"><span class="Apple-converted-space">                        </span>&lt;p&gt;Mapas epidemiológicos en tiempo real, detección de brotes y modelo de datos para gobiernos y aseguradoras.&lt;/p&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">            </span>&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">        </span>&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">    </span>&lt;/div&gt;</p>
<p class="p2"><br></p>
<p class="p1"><span class="Apple-converted-space">    </span>&lt;!-- SLIDE 12: STACK TECNOLÓGICO --&gt;</p>
<p class="p1"><span class="Apple-converted-space">    </span>&lt;div class="slide" data-i="11"&gt;</p>
<p class="p1"><span class="Apple-converted-space">        </span>&lt;div class="slide-inner"&gt;</p>
<p class="p1"><span class="Apple-converted-space">            </span>&lt;div class="s-tag"&gt;Tecnología&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">            </span>&lt;h1 class="s-title"&gt;Stack simple y robusto&lt;/h1&gt;</p>
<p class="p1"><span class="Apple-converted-space">            </span>&lt;p class="s-sub"&gt;Construido con herramientas modernas, ligeras y escalables. Nada de monolitos ni apps pesadas.&lt;/p&gt;</p>
<p class="p1"><span class="Apple-converted-space">            </span>&lt;div class="sg sg4" style="margin-top:36px;"&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;div class="sc" style="text-align:center;"&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;div class="sc-i" style="background:rgba(0,229,160,.1);color:var(--accent);margin:0 auto 14px;"&gt;&lt;i class="fa-brands fa-whatsapp"&gt;&lt;/i&gt;&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;h4&gt;Canal&lt;/h4&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;p&gt;WhatsApp Business API&lt;br&gt;(Twilio)&lt;/p&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;div class="sc" style="text-align:center;"&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;div class="sc-i" style="background:rgba(0,229,160,.1);color:var(--accent);margin:0 auto 14px;"&gt;&lt;i class="fa-solid fa-server"&gt;&lt;/i&gt;&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;h4&gt;Backend&lt;/h4&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;p&gt;Node.js + Express&lt;br&gt;desplegado en Render&lt;/p&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;div class="sc" style="text-align:center;"&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;div class="sc-i" style="background:rgba(0,229,160,.1);color:var(--accent);margin:0 auto 14px;"&gt;&lt;i class="fa-solid fa-brain"&gt;&lt;/i&gt;&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;h4&gt;IA&lt;/h4&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;p&gt;OpenAI GPT-4o mini&lt;br&gt;clasificación de riesgo&lt;/p&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;div class="sc" style="text-align:center;"&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;div class="sc-i" style="background:rgba(0,229,160,.1);color:var(--accent);margin:0 auto 14px;"&gt;&lt;i class="fa-solid fa-table"&gt;&lt;/i&gt;&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;h4&gt;Métricas&lt;/h4&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;p&gt;Google Sheets API&lt;br&gt;+ Looker Studio&lt;/p&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">            </span>&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">            </span>&lt;div class="sq" style="margin-top:40px;"&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;p style="font-size:.95rem;"&gt;"Menos de 10 archivos de código. Un servidor. Una API de WhatsApp. Inteligencia Artificial. Así construimos el futuro de la salud."&lt;/p&gt;</p>
<p class="p1"><span class="Apple-converted-space">            </span>&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">        </span>&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">    </span>&lt;/div&gt;</p>
<p class="p2"><br></p>
<p class="p1"><span class="Apple-converted-space">    </span>&lt;!-- SLIDE 13: RIESGOS --&gt;</p>
<p class="p1"><span class="Apple-converted-space">    </span>&lt;div class="slide" data-i="12"&gt;</p>
<p class="p1"><span class="Apple-converted-space">        </span>&lt;div class="slide-inner"&gt;</p>
<p class="p1"><span class="Apple-converted-space">            </span>&lt;div class="s-tag"&gt;Gestión de Riesgos&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">            </span>&lt;h1 class="s-title"&gt;Lo que debes saber&lt;/h1&gt;</p>
<p class="p1"><span class="Apple-converted-space">            </span>&lt;div class="sg sg3" style="margin-top:36px;"&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;div class="sc"&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;div class="sc-i" style="background:rgba(255,99,71,.08);color:var(--accent2);"&gt;&lt;i class="fa-solid fa-scale-balanced"&gt;&lt;/i&gt;&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;h4&gt;Regulación&lt;/h4&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;p style="margin-bottom:12px;font-size:.82rem;color:var(--accent2);"&gt;El diagnóstico médico está regulado por COFEPRIS (Ley General de Salud, Art. 58).&lt;/p&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;div style="height:1px;background:var(--border);margin-bottom:12px;"&gt;&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;p style="font-size:.82rem;color:var(--fg);"&gt;&lt;i class="fa-solid fa-shield-halved" style="color:var(--accent);margin-right:6px;font-size:11px;"&gt;&lt;/i&gt;No diagnosticamos. El lenguaje siempre es "orientación clínica" y "evaluación". No emitimos recetas.&lt;/p&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;div class="sc"&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;div class="sc-i" style="background:rgba(255,99,71,.08);color:var(--accent2);"&gt;&lt;i class="fa-solid fa-brain"&gt;&lt;/i&gt;&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;h4&gt;Precisión de IA&lt;/h4&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;p style="margin-bottom:12px;font-size:.82rem;color:var(--accent2);"&gt;Errores en clasificación pueden ser peligrosos.&lt;/p&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;div style="height:1px;background:var(--border);margin-bottom:12px;"&gt;&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;p style="font-size:.82rem;color:var(--fg);"&gt;&lt;i class="fa-solid fa-shield-halved" style="color:var(--accent);margin-right:6px;font-size:11px;"&gt;&lt;/i&gt;Reglas duras + IA. Banderas rojas por keywords fijos. Avisos claros en cada interacción.&lt;/p&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;div class="sc"&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;div class="sc-i" style="background:rgba(255,99,71,.08);color:var(--accent2);"&gt;&lt;i class="fa-solid fa-shield-halved"&gt;&lt;/i&gt;&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;h4&gt;Confianza&lt;/h4&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;p style="margin-bottom:12px;font-size:.82rem;color:var(--accent2);"&gt;Los usuarios dudan de un bot para salud.&lt;/p&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;div style="height:1px;background:var(--border);margin-bottom:12px;"&gt;&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;p style="font-size:.82rem;color:var(--fg);"&gt;&lt;i class="fa-solid fa-shield-halved" style="color:var(--accent);margin-right:6px;font-size:11px;"&gt;&lt;/i&gt;El bot conecta con un profesional real. No reemplaza, facilita. Alianza con farmacias da respaldo físico.&lt;/p&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">            </span>&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">        </span>&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">    </span>&lt;/div&gt;</p>
<p class="p2"><br></p>
<p class="p1"><span class="Apple-converted-space">    </span>&lt;!-- SLIDE 14: CIERRE --&gt;</p>
<p class="p1"><span class="Apple-converted-space">    </span>&lt;div class="slide sclose" data-i="13"&gt;</p>
<p class="p1"><span class="Apple-converted-space">        </span>&lt;div class="slide-inner" style="display:flex;flex-direction:column;align-items:center;"&gt;</p>
<p class="p1"><span class="Apple-converted-space">            </span>&lt;div class="slogo"&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;div class="slogo-i"&gt;&lt;i class="fa-solid fa-dna"&gt;&lt;/i&gt;&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;div class="slogo-t"&gt;Helix&lt;span style="color:var(--accent)"&gt;Medic&lt;/span&gt;&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">            </span>&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">            </span>&lt;h1 class="s-title" style="font-size:clamp(2rem,5vw,3.5rem);max-width:700px;text-align:center;"&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>Estamos construyendo el primer filtro médico digital para Latinoamérica.</p>
<p class="p1"><span class="Apple-converted-space">            </span>&lt;/h1&gt;</p>
<p class="p1"><span class="Apple-converted-space">            </span>&lt;p class="s-eslogan" style="margin-top:8px;"&gt;"Tu bienestar a un mensaje de distancia"&lt;/p&gt;</p>
<p class="p1"><span class="Apple-converted-space">            </span>&lt;div class="sq" style="border-left:none;background:none;padding:0;margin-top:32px;"&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;p style="font-size:clamp(1.2rem,2.5vw,1.6rem);text-align:center;"&gt;"No reemplazamos doctores.&lt;br&gt;Los hacemos más eficientes."&lt;/p&gt;</p>
<p class="p1"><span class="Apple-converted-space">            </span>&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">            </span>&lt;div class="qr"&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;i class="fa-brands fa-whatsapp"&gt;&lt;/i&gt;</p>
<p class="p1"><span class="Apple-converted-space">            </span>&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">            </span>&lt;p style="margin-top:12px;font-size:.75rem;color:var(--muted);"&gt;Escanea y prueba Helix Medic ahora&lt;/p&gt;</p>
<p class="p1"><span class="Apple-converted-space">            </span>&lt;div style="margin-top:36px;display:flex;align-items:center;gap:24px;flex-wrap:wrap;justify-content:center;"&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;div style="text-align:center;"&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;div style="font-family:'Space Grotesk';font-weight:800;font-size:.75rem;color:var(--accent);letter-spacing:.1em;margin-bottom:6px;"&gt;CONTACTO&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;p style="font-size:.9rem;color:var(--fg);"&gt;hola@helixmedic.mx&lt;/p&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;div style="width:1px;height:30px;background:var(--border);"&gt;&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;div style="text-align:center;"&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;div style="font-family:'Space Grotesk';font-weight:800;font-size:.75rem;color:var(--accent);letter-spacing:.1em;margin-bottom:6px;"&gt;TECNOLOGÍA&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;p style="font-size:.9rem;color:var(--fg);"&gt;WhatsApp + IA&lt;/p&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">            </span>&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">            </span>&lt;p style="margin-top:60px;font-size:.75rem;color:var(--muted);letter-spacing:.05em;"&gt;GRACIAS&lt;/p&gt;</p>
<p class="p1"><span class="Apple-converted-space">        </span>&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">    </span>&lt;/div&gt;</p>
<p class="p2"><br></p>
<p class="p1">&lt;/div&gt;</p>
<p class="p2"><br></p>
<p class="p1">&lt;!-- Controles --&gt;</p>
<p class="p1">&lt;div class="controls"&gt;</p>
<p class="p1"><span class="Apple-converted-space">    </span>&lt;button class="ctrl-btn" onclick="go(-1)" aria-label="Anterior"&gt;&lt;i class="fa-solid fa-chevron-left"&gt;&lt;/i&gt;&lt;/button&gt;</p>
<p class="p1"><span class="Apple-converted-space">    </span>&lt;div class="slide-counter"&gt;&lt;span class="cur" id="cn"&gt;1&lt;/span&gt; / &lt;span id="tn"&gt;14&lt;/span&gt;&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">    </span>&lt;button class="ctrl-btn" onclick="go(1)" aria-label="Siguiente"&gt;&lt;i class="fa-solid fa-chevron-right"&gt;&lt;/i&gt;&lt;/button&gt;</p>
<p class="p1">&lt;/div&gt;</p>
<p class="p2"><br></p>
<p class="p1">&lt;script&gt;</p>
<p class="p1">// === NAVEGACIÓN ===</p>
<p class="p1">var slides = document.querySelectorAll('.slide');</p>
<p class="p1">var N = slides.length;</p>
<p class="p1">var cur = 0;</p>
<p class="p1">var busy = false;</p>
<p class="p2"><br></p>
<p class="p1">document.getElementById('tn').textContent = N;</p>
<p class="p1">upBar();</p>
<p class="p2"><br></p>
<p class="p1">function go(dir) {</p>
<p class="p1"><span class="Apple-converted-space">    </span>var next = cur + dir;</p>
<p class="p1"><span class="Apple-converted-space">    </span>if (busy || next &lt; 0 || next &gt;= N) return;</p>
<p class="p1"><span class="Apple-converted-space">    </span>busy = true;</p>
<p class="p2"><br></p>
<p class="p1"><span class="Apple-converted-space">    </span>var oldEl = slides[cur];</p>
<p class="p1"><span class="Apple-converted-space">    </span>var newEl = slides[next];</p>
<p class="p2"><br></p>
<p class="p1"><span class="Apple-converted-space">    </span>newEl.style.transition = 'none';</p>
<p class="p1"><span class="Apple-converted-space">    </span>newEl.style.opacity = '0';</p>
<p class="p1"><span class="Apple-converted-space">    </span>newEl.style.transform = dir &gt; 0 ? 'translateX(60px)' : 'translateX(-60px)';</p>
<p class="p1"><span class="Apple-converted-space">    </span>newEl.classList.add('visible');</p>
<p class="p2"><br></p>
<p class="p1"><span class="Apple-converted-space">    </span>void newEl.offsetHeight;</p>
<p class="p2"><br></p>
<p class="p1"><span class="Apple-converted-space">    </span>newEl.style.transition = '';</p>
<p class="p1"><span class="Apple-converted-space">    </span>oldEl.style.transform = dir &gt; 0 ? 'translateX(-60px)' : 'translateX(60px)';</p>
<p class="p1"><span class="Apple-converted-space">    </span>oldEl.style.opacity = '0';</p>
<p class="p1"><span class="Apple-converted-space">    </span>newEl.style.transform = 'translateX(0)';</p>
<p class="p1"><span class="Apple-converted-space">    </span>newEl.style.opacity = '1';</p>
<p class="p2"><br></p>
<p class="p1"><span class="Apple-converted-space">    </span>cur = next;</p>
<p class="p1"><span class="Apple-converted-space">    </span>upBar();</p>
<p class="p2"><br></p>
<p class="p1"><span class="Apple-converted-space">    </span>setTimeout(function() {</p>
<p class="p1"><span class="Apple-converted-space">        </span>oldEl.classList.remove('visible');</p>
<p class="p1"><span class="Apple-converted-space">        </span>oldEl.style.transform = '';</p>
<p class="p1"><span class="Apple-converted-space">        </span>oldEl.style.opacity = '';</p>
<p class="p1"><span class="Apple-converted-space">        </span>busy = false;</p>
<p class="p1"><span class="Apple-converted-space">    </span>}, 600);</p>
<p class="p1">}</p>
<p class="p2"><br></p>
<p class="p1">function upBar() {</p>
<p class="p1"><span class="Apple-converted-space">    </span>document.getElementById('cn').textContent = cur + 1;</p>
<p class="p1"><span class="Apple-converted-space">    </span>document.getElementById('pb').style.width = (cur / (N - 1) * 100) + '%';</p>
<p class="p1">}</p>
<p class="p2"><br></p>
<p class="p1">document.addEventListener('keydown', function(e) {</p>
<p class="p1"><span class="Apple-converted-space">    </span>if (e.key === 'ArrowRight' || e.key === ' ') { e.preventDefault(); go(1); }</p>
<p class="p1"><span class="Apple-converted-space">    </span>else if (e.key === 'ArrowLeft') { e.preventDefault(); go(-1); }</p>
<p class="p1"><span class="Apple-converted-space">    </span>else if (e.key === 'Home') { e.preventDefault(); jumpTo(0); }</p>
<p class="p1"><span class="Apple-converted-space">    </span>else if (e.key === 'End') { e.preventDefault(); jumpTo(N - 1); }</p>
<p class="p1">});</p>
<p class="p2"><br></p>
<p class="p1">function jumpTo(idx) {</p>
<p class="p1"><span class="Apple-converted-space">    </span>if (busy || idx === cur || idx &lt; 0 || idx &gt;= N) return;</p>
<p class="p1"><span class="Apple-converted-space">    </span>busy = true;</p>
<p class="p2"><br></p>
<p class="p1"><span class="Apple-converted-space">    </span>slides[cur].classList.remove('visible');</p>
<p class="p1"><span class="Apple-converted-space">    </span>slides[cur].style.transform = '';</p>
<p class="p1"><span class="Apple-converted-space">    </span>slides[cur].style.opacity = '';</p>
<p class="p2"><br></p>
<p class="p1"><span class="Apple-converted-space">    </span>slides[idx].style.transition = 'none';</p>
<p class="p1"><span class="Apple-converted-space">    </span>slides[idx].style.transform = '';</p>
<p class="p1"><span class="Apple-converted-space">    </span>slides[idx].style.opacity = '';</p>
<p class="p1"><span class="Apple-converted-space">    </span>slides[idx].classList.add('visible');</p>
<p class="p1"><span class="Apple-converted-space">    </span>void slides[idx].offsetHeight;</p>
<p class="p1"><span class="Apple-converted-space">    </span>slides[idx].style.transition = '';</p>
<p class="p2"><br></p>
<p class="p1"><span class="Apple-converted-space">    </span>cur = idx;</p>
<p class="p1"><span class="Apple-converted-space">    </span>upBar();</p>
<p class="p1"><span class="Apple-converted-space">    </span>setTimeout(function() { busy = false; }, 100);</p>
<p class="p1">}</p>
<p class="p2"><br></p>
<p class="p1">var tx0 = 0;</p>
<p class="p1">document.addEventListener('touchstart', function(e) { tx0 = e.changedTouches[0].screenX; }, { passive: true });</p>
<p class="p1">document.addEventListener('touchend', function(e) {</p>
<p class="p1"><span class="Apple-converted-space">    </span>var diff = tx0 - e.changedTouches[0].screenX;</p>
<p class="p1"><span class="Apple-converted-space">    </span>if (Math.abs(diff) &gt; 60) go(diff &gt; 0 ? 1 : -1);</p>
<p class="p1">}, { passive: true });</p>
<p class="p2"><br></p>
<p class="p1">document.getElementById('deck').addEventListener('click', function(e) {</p>
<p class="p1"><span class="Apple-converted-space">    </span>if (e.target.closest('.controls') || e.target.closest('.fsb') || e.target.closest('#wa-mock')) return;</p>
<p class="p1"><span class="Apple-converted-space">    </span>var x = e.clientX, w = window.innerWidth;</p>
<p class="p1"><span class="Apple-converted-space">    </span>if (x &gt; w * 0.6) go(1);</p>
<p class="p1"><span class="Apple-converted-space">    </span>else if (x &lt; w * 0.4) go(-1);</p>
<p class="p1">});</p>
<p class="p2"><br></p>
<p class="p1">function toggleFS() {</p>
<p class="p1"><span class="Apple-converted-space">    </span>if (!document.fullscreenElement) document.documentElement.requestFullscreen().catch(function(){});</p>
<p class="p1"><span class="Apple-converted-space">    </span>else document.exitFullscreen();</p>
<p class="p1">}</p>
<p class="p2"><br></p>
<p class="p1">// === DEMO INTERACTIVA ===</p>
<p class="p1">var demoState = 0;</p>
<p class="p1">var demoAge = null, demoDuration = null, demoSymptoms = null;</p>
<p class="p2"><br></p>
<p class="p1">function addBubble(text, cls) {</p>
<p class="p1"><span class="Apple-converted-space">    </span>var body = document.getElementById('wa-body');</p>
<p class="p1"><span class="Apple-converted-space">    </span>var bubble = document.createElement('div');</p>
<p class="p1"><span class="Apple-converted-space">    </span>bubble.className = 'wa-bubble ' + cls;</p>
<p class="p1"><span class="Apple-converted-space">    </span>bubble.textContent = text;</p>
<p class="p1"><span class="Apple-converted-space">    </span>body.appendChild(bubble);</p>
<p class="p1"><span class="Apple-converted-space">    </span>body.scrollTop = body.scrollHeight;</p>
<p class="p1">}</p>
<p class="p2"><br></p>
<p class="p1">function addTyping() {</p>
<p class="p1"><span class="Apple-converted-space">    </span>var body = document.getElementById('wa-body');</p>
<p class="p1"><span class="Apple-converted-space">    </span>var typing = document.createElement('div');</p>
<p class="p1"><span class="Apple-converted-space">    </span>typing.className = 'wa-bubble wa-bot wa-typing';</p>
<p class="p1"><span class="Apple-converted-space">    </span>typing.innerHTML = '&lt;span&gt;&lt;/span&gt;&lt;span&gt;&lt;/span&gt;&lt;span&gt;&lt;/span&gt;';</p>
<p class="p1"><span class="Apple-converted-space">    </span>typing.id = 'typing-indicator';</p>
<p class="p1"><span class="Apple-converted-space">    </span>body.appendChild(typing);</p>
<p class="p1"><span class="Apple-converted-space">    </span>body.scrollTop = body.scrollHeight;</p>
<p class="p1">}</p>
<p class="p2"><br></p>
<p class="p1">function removeTyping() {</p>
<p class="p1"><span class="Apple-converted-space">    </span>var typing = document.getElementById('typing-indicator');</p>
<p class="p1"><span class="Apple-converted-space">    </span>if (typing) typing.remove();</p>
<p class="p1">}</p>
<p class="p2"><br></p>
<p class="p1">function botReply(text) {</p>
<p class="p1"><span class="Apple-converted-space">    </span>removeTyping();</p>
<p class="p1"><span class="Apple-converted-space">    </span>addBubble(text, 'wa-bot');</p>
<p class="p1">}</p>
<p class="p2"><br></p>
<p class="p1">function disableInput(disabled) {</p>
<p class="p1"><span class="Apple-converted-space">    </span>document.getElementById('wa-input').disabled = disabled;</p>
<p class="p1"><span class="Apple-converted-space">    </span>document.getElementById('wa-send').disabled = disabled;</p>
<p class="p1">}</p>
<p class="p2"><br></p>
<p class="p1">function handleDemoSend() {</p>
<p class="p1"><span class="Apple-converted-space">    </span>var input = document.getElementById('wa-input');</p>
<p class="p1"><span class="Apple-converted-space">    </span>var text = input.value.trim();</p>
<p class="p1"><span class="Apple-converted-space">    </span>if (!text || busyDemo) return;</p>
<p class="p1"><span class="Apple-converted-space">    </span>busyDemo = true;</p>
<p class="p1"><span class="Apple-converted-space">    </span>addBubble(text, 'wa-user');</p>
<p class="p1"><span class="Apple-converted-space">    </span>input.value = '';</p>
<p class="p1"><span class="Apple-converted-space">    </span>disableInput(true);</p>
<p class="p1"><span class="Apple-converted-space">    </span>addTyping();</p>
<p class="p2"><br></p>
<p class="p1"><span class="Apple-converted-space">    </span>setTimeout(function() {</p>
<p class="p1"><span class="Apple-converted-space">        </span>processDemo(text);</p>
<p class="p1"><span class="Apple-converted-space">        </span>busyDemo = false;</p>
<p class="p1"><span class="Apple-converted-space">    </span>}, 800 + Math.random() * 600);</p>
<p class="p1">}</p>
<p class="p2"><br></p>
<p class="p1">var busyDemo = false;</p>
<p class="p2"><br></p>
<p class="p1">function handleDemoKey(e) {</p>
<p class="p1"><span class="Apple-converted-space">    </span>if (e.key === 'Enter') {</p>
<p class="p1"><span class="Apple-converted-space">        </span>e.preventDefault();</p>
<p class="p1"><span class="Apple-converted-space">        </span>handleDemoSend();</p>
<p class="p1"><span class="Apple-converted-space">    </span>}</p>
<p class="p1"><span class="Apple-converted-space">    </span>e.stopPropagation();</p>
<p class="p1">}</p>
<p class="p2"><br></p>
<p class="p1">function processDemo(text) {</p>
<p class="p1"><span class="Apple-converted-space">    </span>switch (demoState) {</p>
<p class="p1"><span class="Apple-converted-space">        </span>case 0:</p>
<p class="p1"><span class="Apple-converted-space">            </span>demoSymptoms = text;</p>
<p class="p1"><span class="Apple-converted-space">            </span>demoState = 1;</p>
<p class="p1"><span class="Apple-converted-space">            </span>botReply('¿Qué edad tienes?');</p>
<p class="p1"><span class="Apple-converted-space">            </span>disableInput(false);</p>
<p class="p1"><span class="Apple-converted-space">            </span>break;</p>
<p class="p1"><span class="Apple-converted-space">        </span>case 1:</p>
<p class="p1"><span class="Apple-converted-space">            </span>var age = parseInt(text, 10);</p>
<p class="p1"><span class="Apple-converted-space">            </span>if (isNaN(age) || age &lt; 0 || age &gt; 120) {</p>
<p class="p1"><span class="Apple-converted-space">                </span>botReply('Por favor, ingresa una edad válida (número).');</p>
<p class="p1"><span class="Apple-converted-space">                </span>disableInput(false);</p>
<p class="p1"><span class="Apple-converted-space">                </span>return;</p>
<p class="p1"><span class="Apple-converted-space">            </span>}</p>
<p class="p1"><span class="Apple-converted-space">            </span>demoAge = age;</p>
<p class="p1"><span class="Apple-converted-space">            </span>demoState = 2;</p>
<p class="p1"><span class="Apple-converted-space">            </span>botReply('¿Desde cuándo presentas estos síntomas? (Ejemplo: "hace 2 días", "desde ayer")');</p>
<p class="p1"><span class="Apple-converted-space">            </span>disableInput(false);</p>
<p class="p1"><span class="Apple-converted-space">            </span>break;</p>
<p class="p1"><span class="Apple-converted-space">        </span>case 2:</p>
<p class="p1"><span class="Apple-converted-space">            </span>demoDuration = text;</p>
<p class="p1"><span class="Apple-converted-space">            </span>demoState = 3;</p>
<p class="p1"><span class="Apple-converted-space">            </span>botReply('Cuéntame, ¿tienes algún otro síntoma además de lo que ya mencionaste?');</p>
<p class="p1"><span class="Apple-converted-space">            </span>disableInput(false);</p>
<p class="p1"><span class="Apple-converted-space">            </span>break;</p>
<p class="p1"><span class="Apple-converted-space">        </span>case 3:</p>
<p class="p1"><span class="Apple-converted-space">            </span>demoSymptoms += '. ' + text;</p>
<p class="p1"><span class="Apple-converted-space">            </span>demoState = 4;</p>
<p class="p1"><span class="Apple-converted-space">            </span>var risk = 'medio';</p>
<p class="p1"><span class="Apple-converted-space">            </span>var riskMsg = '🟡 *Riesgo Medio*\nTe sugerimos acudir a una farmacia para revisión.\n📍 Farmacia cercana sugerida: Farmacia del Carmen, Calle Hidalgo 45.\n\n¿Te gustaría que un *médico real* te atienda ahora mismo por este chat? Responde *Sí* o *No*.';</p>
<p class="p1"><span class="Apple-converted-space">            </span>botReply(riskMsg);</p>
<p class="p1"><span class="Apple-converted-space">            </span>disableInput(false);</p>
<p class="p1"><span class="Apple-converted-space">            </span>break;</p>
<p class="p1"><span class="Apple-converted-space">        </span>case 4:</p>
<p class="p1"><span class="Apple-converted-space">            </span>var answer = text.toLowerCase().trim();</p>
<p class="p1"><span class="Apple-converted-space">            </span>if (answer === 'sí' || answer === 'si' || answer === 'ok') {</p>
<p class="p1"><span class="Apple-converted-space">                </span>demoState = 5;</p>
<p class="p1"><span class="Apple-converted-space">                </span>botReply('🔔 Un médico se unirá a este chat en breve. Por favor, mantente atento.');</p>
<p class="p1"><span class="Apple-converted-space">                </span>setTimeout(function() {</p>
<p class="p1"><span class="Apple-converted-space">                    </span>addBubble('🩺 *Dr. García*: Hola, soy el doctor García. He revisado tu caso. ¿Tienes alguna alergia o condición preexistente?', 'wa-bot');</p>
<p class="p1"><span class="Apple-converted-space">                    </span>disableInput(false);</p>
<p class="p1"><span class="Apple-converted-space">                </span>}, 2000);</p>
<p class="p1"><span class="Apple-converted-space">            </span>} else if (answer === 'no') {</p>
<p class="p1"><span class="Apple-converted-space">                </span>demoState = 99;</p>
<p class="p1"><span class="Apple-converted-space">                </span>botReply('Entendido. Sigue las recomendaciones. Si empeoras, busca ayuda inmediata. ¡Cuídate!');</p>
<p class="p1"><span class="Apple-converted-space">                </span>disableInput(true);</p>
<p class="p1"><span class="Apple-converted-space">            </span>} else {</p>
<p class="p1"><span class="Apple-converted-space">                </span>botReply('Responde *Sí* para que un médico te atienda ahora en este chat, o *No* para terminar.');</p>
<p class="p1"><span class="Apple-converted-space">                </span>disableInput(false);</p>
<p class="p1"><span class="Apple-converted-space">            </span>}</p>
<p class="p1"><span class="Apple-converted-space">            </span>break;</p>
<p class="p1"><span class="Apple-converted-space">        </span>case 5:</p>
<p class="p1"><span class="Apple-converted-space">            </span>demoState = 6;</p>
<p class="p1"><span class="Apple-converted-space">            </span>botReply('Gracias por la información. Basado en lo que me has contado, te recomiendo:\n- Tomar paracetamol 500mg cada 8 horas\n- Mantener reposo e hidratación\n- Si presentas fiebre mayor a 39°C o dificultad para respirar, acude a urgencias.\n\nCuando termines, escribe *FIN* para recibir el resumen de tu consulta.');</p>
<p class="p1"><span class="Apple-converted-space">            </span>disableInput(false);</p>
<p class="p1"><span class="Apple-converted-space">            </span>break;</p>
<p class="p1"><span class="Apple-converted-space">        </span>case 6:</p>
<p class="p1"><span class="Apple-converted-space">            </span>if (text.toUpperCase() === 'FIN') {</p>
<p class="p1"><span class="Apple-converted-space">                </span>demoState = 99;</p>
<p class="p1"><span class="Apple-converted-space">                </span>botReply('📋 *Resumen de tu consulta en Helix Medic*\nEl médico ha finalizado la atención. Sigue las indicaciones proporcionadas. Si presentas nuevos síntomas, consulta nuevamente. ¡Cuídate!');</p>
<p class="p1"><span class="Apple-converted-space">                </span>disableInput(true);</p>
<p class="p1"><span class="Apple-converted-space">            </span>} else {</p>
<p class="p1"><span class="Apple-converted-space">                </span>botReply('El doctor ha recibido tu mensaje. Si ya terminaste, escribe *FIN* para cerrar la consulta.');</p>
<p class="p1"><span class="Apple-converted-space">                </span>disableInput(false);</p>
<p class="p1"><span class="Apple-converted-space">            </span>}</p>
<p class="p1"><span class="Apple-converted-space">            </span>break;</p>
<p class="p1"><span class="Apple-converted-space">        </span>default:</p>
<p class="p1"><span class="Apple-converted-space">            </span>botReply('Gracias por usar Helix Medic. Para reiniciar la demo presiona el botón "Reiniciar demo".');</p>
<p class="p1"><span class="Apple-converted-space">            </span>disableInput(true);</p>
<p class="p1"><span class="Apple-converted-space">    </span>}</p>
<p class="p1">}</p>
<p class="p2"><br></p>
<p class="p1">function resetDemo() {</p>
<p class="p1"><span class="Apple-converted-space">    </span>demoState = 0;</p>
<p class="p1"><span class="Apple-converted-space">    </span>demoAge = null;</p>
<p class="p1"><span class="Apple-converted-space">    </span>demoDuration = null;</p>
<p class="p1"><span class="Apple-converted-space">    </span>demoSymptoms = null;</p>
<p class="p1"><span class="Apple-converted-space">    </span>var body = document.getElementById('wa-body');</p>
<p class="p1"><span class="Apple-converted-space">    </span>body.innerHTML = '&lt;div class="wa-bubble wa-bot"&gt;🩺 *Helix Medic* — Recuerda: soy un asistente de orientación clínica. Para comenzar, dime ¿qué síntomas tienes?&lt;/div&gt;';</p>
<p class="p1"><span class="Apple-converted-space">    </span>disableInput(false);</p>
<p class="p1"><span class="Apple-converted-space">    </span>document.getElementById('wa-input').value = '';</p>
<p class="p1"><span class="Apple-converted-space">    </span>document.getElementById('wa-input').focus();</p>
<p class="p1">}</p>
<p class="p2"><br></p>
<p class="p1">var observer = new MutationObserver(function(mutations) {</p>
<p class="p1"><span class="Apple-converted-space">    </span>if (slides[5] &amp;&amp; slides[5].classList.contains('visible')) {</p>
<p class="p1"><span class="Apple-converted-space">        </span>document.getElementById('wa-input').focus();</p>
<p class="p1"><span class="Apple-converted-space">    </span>}</p>
<p class="p1">});</p>
<p class="p1">observer.observe(document.getElementById('demo-slide'), { attributes: true, attributeFilter: ['class'] });</p>
<p class="p1">&lt;/script&gt;</p>
<p class="p1">&lt;/body&gt;</p>
<p class="p1">&lt;/html&gt;</p>
</body>
</html>
