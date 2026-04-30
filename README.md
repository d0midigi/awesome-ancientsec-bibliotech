<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Cyber BiblioTech</title>
<style>
  *{margin:0;padding:0;box-sizing:border-box}
  body{background:#000;color:#e0e0e0;font-family:-apple-system,BlinkMacSystemFont,'Segoe UI',Roboto,sans-serif;line-height:1.6;padding:2rem 1rem}
  .wrap{max-width:1000px;margin:auto}

  /* Header */
  header{text-align:center;margin-bottom:3rem;padding:2rem 0;border-bottom:1px solid #1a1a1a}
  .badge-wrap{margin-bottom:1rem}
  .badge-wrap img{height:28px}
  h1{font-size:3rem;font-weight:800;letter-spacing:-2px;margin-bottom:.5rem;color:#fff}
  h1 span{color:#fe0942}
  .tagline{font-size:1.3rem;color:#888;font-style:italic;margin-bottom:1.5rem}
  p {
    text-align:justify;
  }
  .manifesto{color:#aaa;font-size:.95rem;max-width:700px;margin:0 auto 1.5rem;line-height:1.8}
  .manifesto strong{color:#fe0942}

  /* TOC */
  .toc{display:flex;flex-wrap:wrap;gap:.5rem;justify-content:center;margin-bottom:3rem;padding:1rem 0}
  .toc a{color:#666;text-decoration:none;font-size:.8rem;padding:.5rem 1rem;border:1px solid #32a;border-radius:20px;transition:.2s;text-transform:uppercase;letter-spacing:1px;font-weight:600}
  .toc a:hover{color:#fe0942;border-color:#fe0942}

  /* Sections */
  .sec{margin-bottom:3rem}
  .sec-header{display:flex;align-items:center;gap:.75rem;margin-bottom:1.5rem;padding-bottom:.75rem;border-bottom:2px solid #fe0942}
  .sec-header h2{font-size:1.4rem;font-weight:700;color:#fff}
  .sec-header .count{background:#fe0942;color:#000;font-size:.75rem;padding:.2rem .6rem;border-radius:12px;font-weight:700}

  /* Sub-section */
  .sub-sec{margin-bottom:2rem}
  .sub-sec h3{font-size:1.1rem;color:#fe0942;margin-bottom:1rem;padding-left:1rem;border-left:3px solid #fe0942}

  /* Items */
  .item{background:#0a0a0a;border:1px solid #1a1a1a;border-radius:12px;padding:1rem 1.25rem;margin-bottom:.6rem;transition:.2s;display:flex;gap:1rem;align-items:flex-start}
  .item:hover{border-color:#fe0942;transform:translateX(4px)}
  .item-num{color:#fe0942;font-weight:800;font-size:.9rem;min-width:24px;text-align:center;flex-shrink:0;opacity:.6}
  .item-logo{width:36px;height:36px;border-radius:8px;object-fit:cover;flex-shrink:0;background:#161b22;display:grid;place-items:center;font-size:1.2rem}
  .item-body{flex:1;min-width:0}
  .item-title{font-weight:600;color:#fff;font-size:.95rem;margin-bottom:.2rem;display:flex;align-items:center;gap:.5rem;flex-wrap:wrap}
  .item-title a{color:#fff;text-decoration:none}
  .item-title a:hover{color:#fe0942}
  .item-desc{color:#777;font-size:.85rem;line-height:1.5}
  .item-meta{display:flex;gap:.5rem;margin-top:.4rem;flex-wrap:wrap}
  .difficulty{font-size:.75rem;padding:.15rem .5rem;border-radius:4px;font-weight:600}
  .diff-easy{background:#1a3a1a;color:#4caf50}
  .diff-medium{background:#3a3a1a;color:#ffc107}
  .diff-hard{background:#3a1a1a;color:#f44336}
  .diff-insane{background:#2a0a2a;color:#e91e63}
  .diff-fundamental{background:#1a1a3a;color:#2196f3}
  .platform-tag{color:#fe0942;font-size:.75rem;border:1px solid #fe094233;padding:.15rem .5rem;border-radius:4px}
  .paid-tag{background:#fe0942;color:#000;font-size:.7rem;padding:.1rem .4rem;border-radius:4px;font-weight:700}

  /* Books special */
  .book-item .item-logo{font-size:.9rem}

  /* Footer */
  footer{text-align:center;margin-top:4rem;padding-top:2rem;border-top:1px solid #1a1a1a;color:#555;font-size:.85rem}
  footer a{color:#fe0942;text-decoration:none}
  footer img{height:31px;margin-top:1rem;opacity:.7}

  /* Responsive */
  @media(max-width:600px){
    h1{font-size:2rem}
    .item{gap:.75rem;padding:.875rem}
    .item-logo{width:32px;height:32px;font-size:1rem}
  }
</style>
</head>
<body>
<div class="wrap">
  <header>
    <div class="badge-wrap">
          <h1>Awesome AncientSec <span>Cyber BiblioTech</span></h1>

      <img src="https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg" alt="Awesome">
    </div>
    <p class="manifesto">
      Forget "new and improved." This is <strong>not</strong> another curated list of 2025 AI wrapper tools. 
      This is a collection of classic cybersecurity papers — the foundational, the forgotten, and the fundamentally useful. 
      While the industry chases the newest shiny object, this repository focuses on the papers, write-ups, walkthroughs, 
      and RTFMs from the mid-1990s up to current day. Because sometimes, learning about the future requires you to learn about the past.
    </p>
<h2><em>"Those who cannot remember the past <span style="color: #ff0942;">are condemned to repeat it.</span>"</em></h2>    
    <br>
    <p class="manifesto">
    Just because a technology is obsolete doesn't mean its security principles are useless. Often, modern vulnerabilities are just creative re-implementations of flaws discovered decades ago. This repo acts as a "BiblioTech" - a library for:</p>
    <p class="manifesto"><b>🏛️ <span style="color: #ff0942;">The Technical Archivist:</span></b> Preserving the digital blueprints of our computing heritage.</p>
    <p class="manifesto"><b>⚙️ <span style="color: #ff0942;">The Security Engineer:</span></b> Studying ancestral exploits to better understand modern threat vectors.</p>
    <p class="manifesto"><b>🧠 <span style="color: #ff0942;">The Naturally Curious:</span></b> Those with an insatiable need to understand the "first principles" of how things were made.</p>
    <p class="manifesto"><strong>🕵️ <span style="color: #ff0942;">The Digital Forensics Expert:</span></strong> Looking for the origins of logic flaws that still persist in legacy code today.</p>    <p class="manifesto"><b>🎓 <span style="color: #ff0942;">The Academic:</span></b> Connecting gaps between theoretical foundations and the current state of the art.</p>
<p class="manifesto"><hr /><br>
<h2>🤝 <span style="color: #32a;">C O N T R I B U T I O N &nbsp; G U I D E L I N E S</span></h2><p class="manifesto">We want this library to grow!🪴 If you have a document that changed your perspective on security, or a document you want to share, please share it!</p>
<h3><span style="color: #32a;">W H A T &nbsp; W E &nbsp; A R E &nbsp; L O O K I N G &nbsp; F O R</span></h3>
<p class="manifesto"><span style="color: #ff0942;"><strong>Historical Significance:</strong></span> Papers, manuals, technical "how-to's," walk-throughs, write-up's, whitepapers and any other form of documentation that has introduced a new concept or defined an era.</p>
<p class="manifesto"><span style="color: #ff0942;"><strong>High Quality:</strong></span> Scanned PDFs, original text files, or official mirrors (please avoid link-rot).</p><h3><span style="color: #32a;">H O W &nbsp; T O &nbsp; C O N T R I B U T E</span></h3><p class="manifesto">1. <span style="color: #ff0942;"><strong>Fork</strong> </span>the repository.</p><p class="manifesto">2. <span style="color: #ff0942;"><strong>Add your link</strong></span> to the appropriate category in the <code><span style="color: #ff0942;">README.MD</span>.</code></p><p class="manifesto">3. <span style="color: #ff0942;"><strong>Use the format:</strong> <code>[Title (Year) - Author](Link)</code></span> - Short description of what we can still learn from it.</p><p class="manifesto">4. <span style="color: #ff0942;"><strong>Submit a Pull Request</strong></span> with the title "Add [Document Name]."</p><p class="manifesto"><hr /><br>
<h2>⚠️ <span style="color: #ff9900;">D I S C L A I M E R</span></h2><p class="manifesto">The materials in this repository are provided for <b>educational, historical, and research purpose only.</b></p>
<p class="manifesto">
<h4>1. <span style="color: #32a;">E D U C A T I O N A L &nbsp;  U S E</span></h4><p class="manifesto">The "ancient" documentation provided here is often deprecated or technically "broken." It is intended to teach, provide background theory and perspectives into the history of security and aims to provide insights into the evolution of modern-day logic flaws and vulnerabilities.</p>
    
    <h4>2. <span style="color: #32a;">NO &nbsp; W A R R A N T Y</span></h4><p class="manifesto">The maintenance of <b>awesome-ancientsec-bibliotech</b> make no guarantees regarding the accuracy or safety of the information contained within these documents. Attempting to apply historical exploits or configurations to modern systems or networks with which you do not personally own, or do not have explicit written permission (authorization) from system/network owners to test against, is illegal and, therefore, may result in unintended damage, security vulnerabilities, or legal penalties.</p>
<h4>3. <span style="color: #32a;">E T H I C A L &nbsp; C O N D U C T</span></h4><p class="manifesto">We do not condone the use of this information for any illegal or malicious activities. By using this repository, you agree to use the knowledge gained here in an ethical and lawful manner to build more secure systems for our future.</p>
  </header>

  <nav class="toc">
    <a href="#oscp">OSCP Guides</a>
    <a href="#cheats">Cheatsheets</a>
    <a href="#buffer">Buffer Overflow</a>
    <a href="#privesc">Privesc</a>
    <a href="#ad">Active Directory</a>
    <a href="#resources">Resources</a>
    <a href="#books">Books</a>
  </nav>

  <section class="sec" id="oscp">
    <div class="sec-header">
      <h2>OSCP Reviews & Guides</h2>
      <span class="count">12</span>
    </div>

    <div class="item">
      <span class="item-num">01</span>
      <div class="item-logo">📋</div>
      <div class="item-body">
        <div class="item-title"><a href="https://help.offensive-security.com/hc/en-us/articles/360040165632-OSCP-Exam-Guide">Official OSCP Certification Exam Guide</a></div>
        <div class="item-desc">The official exam guide straight from Offensive Security.</div>
      </div>
    </div>

    <div class="item">
      <span class="item-num">02</span>
      <div class="item-logo">📝</div>
      <div class="item-body">
        <div class="item-title"><a href="https://medium.com/@hakluke/haklukes-ultimate-oscp-guide-part-1-is-oscp-for-you-b57cbcce7440">Luke's Ultimate OSCP Guide</a> <span style="color:#666;font-size:.8rem">(3 Parts)</span></div>
        <div class="item-desc">Hakluke's comprehensive three-part guide covering preparation, workflow, and practical hacking tips.</div>
      </div>
    </div>

    <div class="item">
      <span class="item-num">03</span>
      <div class="item-logo">🎯</div>
      <div class="item-body">
        <div class="item-title"><a href="https://www.abatchy.com/2017/03/how-to-prepare-for-pwkoscp-noob">How to Prepare for PWK/OSCP — A Noob-Friendly Guide</a></div>
        <div class="item-desc">Abatchy's beginner-friendly roadmap to OSCP success.</div>
      </div>
    </div>

    <div class="item">
      <span class="item-num">04</span>
      <div class="item-logo">🛡️</div>
      <div class="item-body">
        <div class="item-title"><a href="http://www.lucas-bader.com/certification/2015/05/27/oscp-offensive-security-certified-professional">n3ko1's OSCP Guide</a></div>
        <div class="item-desc">Classic write-up from Lucas Bader on the OSCP journey.</div>
      </div>
    </div>

    <div class="item">
      <span class="item-num">05</span>
      <div class="item-logo">🎥</div>
      <div class="item-body">
        <div class="item-title"><a href="https://www.youtube.com/playlist?list=PLyPJ3SHNkjIFITR-Lzsc0XSOBS7JUXsOy">Jan's "Path to OSCP" Videos</a></div>
        <div class="item-desc">Video playlist documenting the entire OSCP preparation path.</div>
      </div>
    </div>

    <div class="item">
      <span class="item-num">06</span>
      <div class="item-logo">⚔️</div>
      <div class="item-body">
        <div class="item-title"><a href="http://www.securitysift.com/offsec-pwb-oscp/">Offensive Security's PWB and OSCP — My Experience</a></div>
        <div class="item-desc">Security Sift's detailed experience write-up with bonus scripts.</div>
      </div>
    </div>

    <div class="item">
      <span class="item-num">07</span>
      <div class="item-logo">🔍</div>
      <div class="item-body">
        <div class="item-title"><a href="https://theslickgeek.com/oscp/">OSCP Lab and Exam Review</a></div>
        <div class="item-desc">The Slick Geek's review of the labs and exam experience.</div>
      </div>
    </div>

    <div class="item">
      <span class="item-num">08</span>
      <div class="item-logo">📚</div>
      <div class="item-body">
        <div class="item-title"><a href="https://www.jpsecnetworks.com/category/oscp/">OSCP Preparation Notes</a></div>
        <div class="item-desc">Categorized preparation notes from JP Sec Networks.</div>
      </div>
    </div>

    <div class="item">
      <span class="item-num">09</span>
      <div class="item-logo">🗺️</div>
      <div class="item-body">
        <div class="item-title"><a href="http://niiconsulting.com/checkmate/2017/06/a-detail-guide-on-oscp-preparation-from-newbie-to-oscp/">A Detailed Guide on OSCP Preparation — From Newbie to OSCP</a></div>
        <div class="item-desc">NII Consulting's comprehensive newbie-to-OSCP roadmap.</div>
      </div>
    </div>

    <div class="item">
      <span class="item-num">10</span>
      <div class="item-logo">💪</div>
      <div class="item-body">
        <div class="item-title"><a href="https://alphacybersecurity.tech/my-fight-for-the-oscp/">My Fight for OSCP</a></div>
        <div class="item-desc">Alpha Cyber Security's personal battle story with OSCP.</div>
      </div>
    </div>

    <div class="item">
      <span class="item-num">11</span>
      <div class="item-logo">🏆</div>
      <div class="item-body">
        <div class="item-title"><a href="https://johnjhacking.com/blog/the-oscp-preperation-guide-2020/">The Ultimate OSCP Preparation Guide</a></div>
        <div class="item-desc">JohnJHacking's ultimate preparation resource for 2020 and beyond.</div>
      </div>
    </div>

    <div class="item">
      <span class="item-num">12</span>
      <div class="item-logo">🔥</div>
      <div class="item-body">
        <div class="item-title"><a href="https://www.netsecfocus.com/oscp/2021/05/06/The_Journey_to_Try_Harder-_TJnull-s_Preparation_Guide_for_PEN-200_PWK_OSCP_2.0.html">The Journey to Try Harder: TJnull's Preparation Guide</a></div>
        <div class="item-desc">TJnull's legendary guide for PEN-200 PWK/OSCP 2.0.</div>
      </div>
    </div>
  </section>

  <section class="sec" id="cheats">
    <div class="sec-header">
      <h2>Cheatsheets & Scripts</h2>
      <span class="count">11</span>
    </div>

    <div class="item">
      <span class="item-num">01</span>
      <div class="item-logo">💡</div>
      <div class="item-body">
        <div class="item-title"><a href="https://medium.com/@hakluke/haklukes-ultimate-oscp-guide-part-3-practical-hacking-tips-and-tricks-c38486f5fc97">Luke's Practical Hacking Tips & Tricks</a></div>
        <div class="item-desc">Practical tips and tricks from Hakluke's OSCP guide part 3.</div>
      </div>
    </div>

    <div class="item">
      <span class="item-num">02</span>
      <div class="item-logo">📋</div>
      <div class="item-body">
        <div class="item-title"><a href="https://highon.coffee/blog/penetration-testing-tools-cheat-sheet/">Penetration Testing Tools Cheat Sheet</a></div>
        <div class="item-desc">HighOn.Coffee's comprehensive pentesting tools reference.</div>
      </div>
    </div>

    <div class="item">
      <span class="item-num">03</span>
      <div class="item-logo">🎓</div>
      <div class="item-body">
        <div class="item-title"><a href="https://gist.github.com/unfo/5ddc85671dcf39f877aaf5dce105fac3">How to Pass OSCP</a></div>
        <div class="item-desc">GitHub gist with practical advice for passing the exam.</div>
      </div>
    </div>

    <div class="item">
      <span class="item-num">04</span>
      <div class="item-logo">🐚</div>
      <div class="item-body">
        <div class="item-title"><a href="https://highon.coffee/blog/reverse-shell-cheat-sheet/">Reverse Shell Cheat Sheet</a></div>
        <div class="item-desc">Every reverse shell one-liner you'll ever need.</div>
      </div>
    </div>

    <div class="item">
      <span class="item-num">05</span>
      <div class="item-logo">⚙️</div>
      <div class="item-body">
        <div class="item-title"><a href="https://www.revshells.com/">Reverse Shell Generator</a></div>
        <div class="item-desc">Interactive generator for reverse shells in multiple languages.</div>
      </div>
    </div>

    <div class="item">
      <span class="item-num">06</span>
      <div class="item-logo">🐧</div>
      <div class="item-body">
        <div class="item-title"><a href="https://www.lanmaster53.com/2011/05/7-linux-shells-using-built-in-tools/">7 Linux Shells Using Built-in Tools</a></div>
        <div class="item-desc">Creative shell techniques using only built-in Linux utilities.</div>
      </div>
    </div>

    <div class="item">
      <span class="item-num">07</span>
      <div class="item-logo">🪟</div>
      <div class="item-body">
        <div class="item-title"><a href="https://github.com/GDSSecurity/Windows-Exploit-Suggester">Windows Exploit Suggester</a></div>
        <div class="item-desc">Python script to suggest exploits based on patch levels.</div>
      </div>
    </div>

    <div class="item">
      <span class="item-num">08</span>
      <div class="item-logo">🐧</div>
      <div class="item-body">
        <div class="item-title"><a href="https://github.com/InteliSecureLabs/Linux_Exploit_Suggester">Linux Exploit Suggester</a></div>
        <div class="item-desc">Linux kernel exploit suggestion tool for privilege escalation.</div>
      </div>
    </div>

    <div class="item">
      <span class="item-num">09</span>
      <div class="item-logo">📦</div>
      <div class="item-body">
        <div class="item-title"><a href="https://github.com/rewardone/OSCPRepo">OSCPRepo</a></div>
        <div class="item-desc">Curated repository of OSCP-related tools and resources.</div>
      </div>
    </div>

    <div class="item">
      <span class="item-num">10</span>
      <div class="item-logo">🚀</div>
      <div class="item-body">
        <div class="item-title"><a href="https://github.com/pythonmaster41/Go-For-OSCP">Go-for-OSCP</a></div>
        <div class="item-desc">Go-based tools and scripts for OSCP preparation.</div>
      </div>
    </div>

    <div class="item">
      <span class="item-num">11</span>
      <div class="item-logo">🔧</div>
      <div class="item-body">
        <div class="item-title"><a href="https://github.com/adon90/pentest_compilation">Pentest Compilation</a></div>
        <div class="item-desc">Compilation of penetration testing commands and techniques.</div>
      </div>
    </div>
  </section>

  <section class="sec" id="buffer">
    <div class="sec-header">
      <h2>Buffer Overflow</h2>
      <span class="count">6</span>
    </div>

    <div class="item">
      <span class="item-num">01</span>
      <div class="item-logo">📖</div>
      <div class="item-body">
        <div class="item-title"><a href="https://www.corelan.be/index.php/2009/07/19/exploit-writing-tutorial-part-1-stack-based-overflows/">Corelan's Exploit Writing Tutorial Part 1</a></div>
        <div class="item-desc">The legendary stack-based overflow tutorial from Corelan Team.</div>
      </div>
    </div>

    <div class="item">
      <span class="item-num">02</span>
      <div class="item-logo">🎓</div>
      <div class="item-body">
        <div class="item-title"><a href="https://github.com/justinsteven/dostackbufferoverflowgood">Justin's DoStackBufferOverflowGood</a></div>
        <div class="item-desc">Hands-on buffer overflow practice environment.</div>
      </div>
    </div>

    <div class="item">
      <span class="item-num">03</span>
      <div class="item-logo">✍️</div>
      <div class="item-body">
        <div class="item-title"><a href="https://www.nccgroup.trust/uk/about-us/newsroom-and-events/blogs/2016/june/writing-exploits-for-win32-systems-from-scratch/">Writing Exploits for Win32 Systems from Scratch</a></div>
        <div class="item-desc">NCC Group's guide to writing Win32 exploits from the ground up.</div>
      </div>
    </div>

    <div class="item">
      <span class="item-num">04</span>
      <div class="item-logo">🎯</div>
      <div class="item-body">
        <div class="item-title"><a href="https://veteransec.com/2018/09/10/32-bit-windows-buffer-overflows-made-easy/">32-Bit Windows Buffer Overflows Made Easy</a></div>
        <div class="item-desc">VeteranSec's simplified approach to 32-bit Windows BOFs.</div>
      </div>
    </div>

    <div class="item">
      <span class="item-num">05</span>
      <div class="item-logo">🎥</div>
      <div class="item-body">
        <div class="item-title"><a href="https://www.youtube.com/watch?v=1S0aBV-Waeo">Introduction to Buffer Overflow Video</a></div>
        <div class="item-desc">Video introduction to buffer overflow concepts.</div>
      </div>
    </div>

    <div class="item">
      <span class="item-num">06</span>
      <div class="item-logo">🎮</div>
      <div class="item-body">
        <div class="item-title"><a href="http://overthewire.org/wargames/narnia/">OverTheWire's Narnia Wargame</a></div>
        <div class="item-desc">Practice buffer overflows in a safe wargame environment.</div>
      </div>
    </div>
  </section>

  <section class="sec" id="privesc">
    <div class="sec-header">
      <h2>Privilege Escalation</h2>
      <span class="count">6</span>
    </div>

    <div class="item">
      <span class="item-num">01</span>
      <div class="item-logo">🪟</div>
      <div class="item-body">
        <div class="item-title"><a href="http://www.fuzzysecurity.com/tutorials/16.html">Windows Privilege Escalation Fundamentals</a></div>
        <div class="item-desc">FuzzySecurity's foundational guide to Windows privilege escalation.</div>
      </div>
    </div>

    <div class="item">
      <span class="item-num">02</span>
      <div class="item-logo">📋</div>
      <div class="item-body">
        <div class="item-title"><a href="https://toshellandback.com/2015/11/24/ms-priv-esc/">Common Windows Privilege Escalation Vectors</a></div>
        <div class="item-desc">To Shell and Back's catalog of common Windows privesc paths.</div>
      </div>
    </div>

    <div class="item">
      <span class="item-num">03</span>
      <div class="item-logo">🎥</div>
      <div class="item-body">
        <div class="item-title"><a href="https://www.youtube.com/watch?v=kMG8IsCohHA">Encyclopaedia Of Windows Privilege Escalation</a> <span style="color:#666;font-size:.8rem">— Brett Moore</span></div>
        <div class="item-desc">Comprehensive video encyclopedia of Windows privilege escalation techniques.</div>
      </div>
    </div>

    <div class="item">
      <span class="item-num">04</span>
      <div class="item-logo">🎥</div>
      <div class="item-body">
        <div class="item-title"><a href="https://www.youtube.com/watch?v=PC_iMqiuIRQ">Level Up! Practical Windows Privilege Escalation</a> <span style="color:#666;font-size:.8rem">— Andrew Smith</span></div>
        <div class="item-desc">Practical, hands-on Windows privilege escalation training.</div>
      </div>
    </div>

    <div class="item">
      <span class="item-num">05</span>
      <div class="item-logo">🐧</div>
      <div class="item-body">
        <div class="item-title"><a href="https://blog.g0tmi1k.com/2011/08/basic-linux-privilege-escalation/">Basic Linux Privilege Escalation</a></div>
        <div class="item-desc">g0tmi1k's essential guide to Linux privilege escalation basics.</div>
      </div>
    </div>

    <div class="item">
      <span class="item-num">06</span>
      <div class="item-logo">🎥</div>
      <div class="item-body">
        <div class="item-title"><a href="https://www.youtube.com/watch?v=dk2wsyFiosg">Linux Privilege Escalation</a> <span style="color:#666;font-size:.8rem">— Jake Williams</span></div>
        <div class="item-desc">Video deep-dive into Linux privilege escalation with Jake Williams.</div>
      </div>
    </div>
  </section>

  <section class="sec" id="ad">
    <div class="sec-header">
      <h2>Active Directory</h2>
      <span class="count">5</span>
    </div>

    <div class="item">
      <span class="item-num">01</span>
      <div class="item-logo">📖</div>
      <div class="item-body">
        <div class="item-title"><a href="https://book.hacktricks.xyz/windows/active-directory-methodology">Active Directory Methodology</a></div>
        <div class="item-desc">HackTricks' comprehensive AD attack methodology reference.</div>
      </div>
    </div>

    <div class="item">
      <span class="item-num">02</span>
      <div class="item-logo">📋</div>
      <div class="item-body">
        <div class="item-title"><a href="https://github.com/S1ckB0y1337/Active-Directory-Exploitation-Cheat-Sheet">Active Directory Exploitation Cheat Sheet</a></div>
        <div class="item-desc">GitHub cheat sheet covering common AD exploitation techniques.</div>
      </div>
    </div>

    <div class="item">
      <span class="item-num">03</span>
      <div class="item-logo">🎯</div>
      <div class="item-body">
        <div class="item-title"><a href="https://github.com/swisskyrepo/PayloadsAllTheThings/blob/master/Methodology%20and%20Resources/Active%20Directory%20Attack.md">PayloadsAllTheThings AD</a></div>
        <div class="item-desc">Swissky's massive collection of AD attack payloads and techniques.</div>
      </div>
    </div>

    <div class="item">
      <span class="item-num">04</span>
      <div class="item-logo">🗺️</div>
      <div class="item-body">
        <div class="item-title"><a href="https://zer1t0.gitlab.io/posts/attacking_ad/">Attacking Active Directory: 0 to 0.9</a></div>
        <div class="item-desc">Zer1t0's comprehensive guide from zero to AD compromise.</div>
      </div>
    </div>

    <div class="item">
      <span class="item-num">05</span>
      <div class="item-logo">💡</div>
      <div class="item-body">
        <div class="item-title"><a href="https://gist.github.com/HarmJ0y/184f9822b195c52dd50c379ed3117993#file-powerview-3-0-tricks-ps1">PowerView 3.0 Tips & Tricks</a></div>
        <div class="item-desc">HarmJ0y's essential PowerView 3.0 tricks and one-liners.</div>
      </div>
    </div>

    <div class="sub-sec">
      <h3>🎮 H A N D S - O N &nbsp; R E S O U R C E S</h3>

      <div class="item">
        <span class="item-num">THM</span>
        <div class="item-logo">🎯</div>
        <div class="item-body">
          <div class="item-title"><a href="https://tryhackme.com/room/activedirectorybasics">Active Directory Basics</a></div>
          <div class="item-desc">Learn the fundamentals of Active Directory in a guided environment.</div>
          <div class="item-meta">
            <span class="difficulty diff-easy">Easy</span>
            <span class="platform-tag">TryHackMe</span>
          </div>
        </div>
      </div>

      <div class="item">
        <span class="item-num">THM</span>
        <div class="item-logo">🔓</div>
        <div class="item-body">
          <div class="item-title"><a href="https://tryhackme.com/room/postexploit">Post-Exploitation Basics</a></div>
          <div class="item-desc">Practice post-exploitation techniques in AD environments.</div>
          <div class="item-meta">
            <span class="difficulty diff-easy">Easy</span>
            <span class="platform-tag">TryHackMe</span>
          </div>
        </div>
      </div>

      <div class="item">
        <span class="item-num">THM</span>
        <div class="item-logo">🍖</div>
        <div class="item-body">
          <div class="item-title"><a href="https://tryhackme.com/room/vulnnetroasted">Vulnnet: Roasted</a></div>
          <div class="item-desc">AD-focused room targeting Kerberoasting and AS-REP Roasting.</div>
          <div class="item-meta">
            <span class="difficulty diff-easy">Easy</span>
            <span class="platform-tag">TryHackMe</span>
          </div>
        </div>
      </div>

      <div class="item">
        <span class="item-num">THM</span>
        <div class="item-logo">⚔️</div>
        <div class="item-body">
          <div class="item-title"><a href="https://tryhackme.com/room/attacktivedirectory">Attacktive Directory</a></div>
          <div class="item-desc">Medium-difficulty AD exploitation room with multiple attack paths.</div>
          <div class="item-meta">
            <span class="difficulty diff-medium">Medium</span>
            <span class="platform-tag">TryHackMe</span>
          </div>
        </div>
      </div>

      <div class="item">
        <span class="item-num">THM</span>
        <div class="item-logo">⚫</div>
        <div class="item-body">
          <div class="item-title"><a href="https://tryhackme.com/room/raz0rblack">Raz0r Black</a></div>
          <div class="item-desc">Medium-difficulty AD room with realistic enterprise scenarios.</div>
          <div class="item-meta">
            <span class="difficulty diff-medium">Medium</span>
            <span class="platform-tag">TryHackMe</span>
          </div>
        </div>
      </div>

      <div class="item">
        <span class="item-num">THM</span>
        <div class="item-logo">🏢</div>
        <div class="item-body">
          <div class="item-title"><a href="https://tryhackme.com/room/enterprise">Enterprise</a></div>
          <div class="item-desc">Medium-difficulty enterprise AD environment for practice.</div>
          <div class="item-meta">
            <span class="difficulty diff-medium">Medium</span>
            <span class="platform-tag">TryHackMe</span>
          </div>
        </div>
      </div>

      <div class="item">
<p><span class="item-num" style="color: #32a;">THM</span></p>        <div class="item-logo">🎯</div>
        <div class="item-body">
          <div class="item-title"><a href="https://tryhackme.com/room/vulnnetactive">Vulnnet: Active</a></div>
          <div class="item-desc">Medium-difficulty AD room with multiple exploitation vectors.</div>
          <div class="item-meta">
            <span class="difficulty diff-medium">Medium</span>
            <span class="platform-tag">TryHackMe</span>
          </div>
        </div>
      </div>

      <div class="item">
<p><span class="item-num" style="color: #32a;">THM</span></p>        <div class="item-logo">0️⃣</div>
        <div class="item-body">
          <div class="item-title"><a href="https://tryhackme.com/room/zer0logon">Zero Logon</a></div>
          <div class="item-desc">Hard-difficulty room focused on the CVE-2020-1472 Zerologon vulnerability.</div>
          <div class="item-meta">
            <span class="difficulty diff-hard">Hard</span>
            <span class="platform-tag">TryHackMe</span>
          </div>
        </div>
      </div>

      <div class="item">
<p><span class="item-num" style="color: #32a;">THM</span></p>        <div class="item-logo">🔮</div>
        <div class="item-body">
          <div class="item-title"><a href="https://tryhackme.com/room/hololive">Holo</a></div>
          <div class="item-desc">Hard-difficulty AD room with advanced exploitation techniques.</div>
          <div class="item-meta">
            <span class="difficulty diff-hard">Hard</span>
            <span class="platform-tag">TryHackMe</span>
          </div>
        </div>
      </div>

      <div class="item">
<p><span class="item-num" style="color: #32a;">THM</span></p>        <div class="item-logo">🔄</div>
        <div class="item-body">
          <div class="item-title"><a href="https://tryhackme.com/network/throwback">Throwback</a></div>
          <div class="item-desc">Easy network-focused AD practice environment.</div>
          <div class="item-meta">
            <span class="difficulty diff-easy">Easy</span>
            <span class="platform-tag">TryHackMe</span>
          </div>
        </div>
      </div>

      <div class="item">
<p><span class="item-num" style="color: #ff0;">HTB</span></p>        <div class="item-logo">🌲</div>
        <div class="item-body">
          <div class="item-title"><a href="https://app.hackthebox.com/machines/212">Forest</a></div>
          <div class="item-desc">Easy HTB machine focusing on AD enumeration and exploitation.</div>
          <div class="item-meta">
            <span class="difficulty diff-easy">Easy</span>
            <span class="platform-tag">HackTheBox</span>
          </div>
        </div>
      </div>

      <div class="item">
<p><span class="item-num" style="color: #ff0;">HTB</span></p>        <div class="item-logo">🌲</div>
        <div class="item-logo">⚡</div>
        <div class="item-body">
          <div class="item-title"><a href="https://app.hackthebox.com/machines/148">Active</a></div>
          <div class="item-desc">Easy HTB machine with classic AD attack vectors.</div>
          <div class="item-meta">
            <span class="difficulty diff-easy">Easy</span>
            <span class="platform-tag">HackTheBox</span>
          </div>
        </div>
      </div>

      <div class="item">
        <span class="item-num">HTB</span>
        <div class="item-logo">🔌</div>
        <div class="item-body">
          <div class="item-title"><a href="https://app.hackthebox.com/machines/235">Fuse</a></div>
          <div class="item-desc">Medium-difficulty HTB machine with AD and web exploitation.</div>
          <div class="item-meta">
            <span class="difficulty diff-medium">Medium</span>
            <span class="platform-tag">HackTheBox</span>
          </div>
        </div>
      </div>

      <div class="item">
        <span class="item-num">HTB</span>
        <div class="item-logo">🏔️</div>
        <div class="item-body">
          <div class="item-title"><a href="https://app.hackthebox.com/machines/235">Cascade</a></div>
          <div class="item-desc">Medium-difficulty HTB machine with AD enumeration challenges.</div>
          <div class="item-meta">
            <span class="difficulty diff-medium">Medium</span>
            <span class="platform-tag">HackTheBox</span>
          </div>
        </div>
      </div>

      <div class="item">
        <span class="item-num">HTB</span>
        <div class="item-logo">🎯</div>
        <div class="item-body">
          <div class="item-title"><a href="https://app.hackthebox.com/machines/223">Monteverde</a></div>
          <div class="item-desc">Medium-difficulty HTB machine with Azure AD integration.</div>
          <div class="item-meta">
            <span class="difficulty diff-medium">Medium</span>
            <span class="platform-tag">HackTheBox</span>
          </div>
        </div>
      </div>

      <div class="item">
        <span class="item-num">HTB</span>
        <div class="item-logo">🎯</div>
        <div class="item-body">
          <div class="item-title"><a href="https://app.hackthebox.com/machines/220">Resolute</a></div>
          <div class="item-desc">Medium-difficulty HTB machine with AD privilege escalation.</div>
          <div class="item-meta">
            <span class="difficulty diff-medium">Medium</span>
            <span class="platform-tag">HackTheBox</span>
          </div>
        </div>
      </div>

      <div class="item">
        <span class="item-num">HTB</span>
        <div class="item-logo">🦇</div>
        <div class="item-body">
          <div class="item-title"><a href="https://app.hackthebox.com/machines/179">Arkham</a></div>
          <div class="item-desc">Medium-difficulty HTB machine with AD and deserialization attacks.</div>
          <div class="item-meta">
            <span class="difficulty diff-medium">Medium</span>
            <span class="platform-tag">HackTheBox</span>
          </div>
        </div>
      </div>

      <div class="item">
        <span class="item-num">HTB</span>
        <div class="item-logo">🦗</div>
        <div class="item-body">
          <div class="item-title"><a href="https://app.hackthebox.com/machines/98">Mantis</a></div>
          <div class="item-desc">Hard-difficulty HTB machine with advanced AD exploitation.</div>
          <div class="item-meta">
            <span class="difficulty diff-hard">Hard</span>
            <span class="platform-tag">HackTheBox</span>
          </div>
        </div>
      </div>

      <div class="item">
        <span class="item-num">HTB</span>
        <div class="item-logo">🎯</div>
        <div class="item-body">
          <div class="item-title"><a href="https://app.hackthebox.com/machines/296">APT</a></div>
          <div class="item-desc">Insane-difficulty HTB machine simulating APT-level AD attacks.</div>
          <div class="item-meta">
            <span class="difficulty diff-insane">Insane</span>
            <span class="platform-tag">HackTheBox</span>
          </div>
        </div>
      </div>

      <div class="item">
        <span class="item-num">HTB</span>
        <div class="item-logo">🔥</div>
        <div class="item-body">
          <div class="item-title"><a href="https://app.hackthebox.com/prolabs/overview/dante">Dante Pro Lab</a></div>
          <div class="item-desc">Beginner-friendly AD pro lab for enterprise penetration testing practice.</div>
          <div class="item-meta">
            <span class="difficulty diff-easy">Beginner</span>
            <span class="platform-tag">HackTheBox Pro Lab</span>
          </div>
        </div>
      </div>

      <div class="item">
        <span class="item-num">HTB</span>
        <div class="item-logo">🌊</div>
        <div class="item-body">
          <div class="item-title"><a href="https://app.hackthebox.com/prolabs/overview/offshore">Offshore Pro Lab</a></div>
          <div class="item-desc">Intermediate AD pro lab with realistic corporate network simulation.</div>
          <div class="item-meta">
            <span class="difficulty diff-medium">Intermediate</span>
            <span class="platform-tag">HackTheBox Pro Lab</span>
          </div>
        </div>
      </div>

      <div class="item">
        <span class="item-num">HTB</span>
        <div class="item-logo">🎸</div>
        <div class="item-body">
          <div class="item-title"><a href="https://app.hackthebox.com/prolabs/overview/rastalabs">RastaLabs Pro Lab</a></div>
          <div class="item-desc">Intermediate AD pro lab focusing on red team operations.</div>
          <div class="item-meta">
            <span class="difficulty diff-medium">Intermediate</span>
            <span class="platform-tag">HackTheBox Pro Lab</span>
          </div>
        </div>
      </div>

      <div class="item">
        <span class="item-num">HTB</span>
        <div class="item-logo">🤖</div>
        <div class="item-body">
          <div class="item-title"><a href="https://app.hackthebox.com/prolabs/overview/cybernetics">Cybernetics Pro Lab</a></div>
          <div class="item-desc">Advanced AD pro lab with complex multi-domain environments.</div>
          <div class="item-meta">
            <span class="difficulty diff-hard">Advanced</span>
            <span class="platform-tag">HackTheBox Pro Lab</span>
          </div>
        </div>
      </div>

      <div class="item">
        <span class="item-num">HTB</span>
        <div class="item-logo">🎯</div>
        <div class="item-body">
          <div class="item-title"><a href="https://app.hackthebox.com/prolabs/overview/aptlabs">APT Labs Pro Lab</a></div>
          <div class="item-desc">Advanced pro lab simulating APT-level adversary operations in AD.</div>
          <div class="item-meta">
            <span class="difficulty diff-hard">Advanced</span>
            <span class="platform-tag">HackTheBox Pro Lab</span>
          </div>
        </div>
      </div>

      <div class="item">
        <span class="item-num">HTB</span>
        <div class="item-logo">🎓</div>
        <div class="item-body">
          <div class="item-title"><a href="https://academy.hackthebox.com/module/details/74">Introduction to Active Directory</a> <span class="paid-tag">PAID</span></div>
          <div class="item-desc">Fundamental AD concepts and enumeration techniques.</div>
          <div class="item-meta">
            <span class="difficulty diff-fundamental">Fundamental</span>
            <span class="platform-tag">HTB Academy</span>
          </div>
        </div>
      </div>

      <div class="item">
        <span class="item-num">HTB</span>
        <div class="item-logo">📡</div>
        <div class="item-body">
          <div class="item-title"><a href="https://academy.hackthebox.com/course/preview/active-directory-ldap">Active Directory LDAP</a> <span class="paid-tag">PAID</span></div>
          <div class="item-desc">Deep dive into LDAP enumeration and exploitation in AD environments.</div>
          <div class="item-meta">
            <span class="difficulty diff-medium">Medium</span>
            <span class="platform-tag">HTB Academy</span>
          </div>
        </div>
      </div>

      <div class="item">
        <span class="item-num">HTB</span>
        <div class="item-logo">👁️</div>
        <div class="item-body">
          <div class="item-title"><a href="https://academy.hackthebox.com/module/details/68">Active Directory PowerView</a> <span class="paid-tag">PAID</span></div>
          <div class="item-desc">Master PowerView for AD reconnaissance and enumeration.</div>
          <div class="item-meta">
            <span class="difficulty diff-medium">Medium</span>
            <span class="platform-tag">HTB Academy</span>
          </div>
        </div>
      </div>

      <div class="item">
        <span class="item-num">HTB</span>
        <div class="item-logo">🩸</div>
        <div class="item-body">
          <div class="item-title"><a href="https://academy.hackthebox.com/module/details/69">Active Directory BloodHound</a> <span class="paid-tag">PAID</span></div>
          <div class="item-desc">Learn to use BloodHound for AD attack path visualization.</div>
          <div class="item-meta">
            <span class="difficulty diff-medium">Medium</span>
            <span class="platform-tag">HTB Academy</span>
          </div>
        </div>
      </div>

      <div class="item">
        <span class="item-num">HTB</span>
        <div class="item-logo">🎯</div>
        <div class="item-body">
          <div class="item-title"><a href="https://academy.hackthebox.com/module/details/143">Active Directory Enumeration & Attacks</a> <span class="paid-tag">PAID</span></div>
          <div class="item-desc">Comprehensive module covering AD enumeration and common attacks.</div>
          <div class="item-meta">
            <span class="difficulty diff-medium">Medium</span>
            <span class="platform-tag">HTB Academy</span>
          </div>
        </div>
      </div>

      <div class="item">
        <span class="item-num">PG</span>
        <div class="item-logo">🎯</div>
        <div class="item-body">
          <div class="item-title"><a href="https://portal.offsec.com/labs/practice">PG-Practice</a> <span class="paid-tag">PAID</span></div>
          <div class="item-desc">OffSec's practice labs — Hutch, Heist, Vault, and more.</div>
          <div class="item-meta">
            <span class="platform-tag">Proving Grounds</span>
          </div>
        </div>
      </div>
    </div>
  </section>

  <section class="sec" id="resources">
    <div class="sec-header">
      <h2>Other OSCP Resources</h2>
      <span class="count">12</span>
    </div>

    <div class="item">
      <span class="item-num">01</span>
      <div class="item-logo">📖</div>
      <div class="item-body">
        <div class="item-title"><a href="https://www.offensive-security.com/documentation/penetration-testing-with-kali.pdf">PWK Syllabus</a></div>
        <div class="item-desc">Official Penetration Testing with Kali Linux syllabus from OffSec.</div>
      </div>
    </div>

    <div class="item">
      <span class="item-num">02</span>
      <div class="item-logo">🎯</div>
      <div class="item-body">
        <div class="item-title"><a href="https://github.com/burntmybagel/OSCP-Prep">OSCP-Prep Resources</a></div>
        <div class="item-desc">Curated collection of OSCP preparation materials and notes.</div>
      </div>
    </div>

    <div class="item">
      <span class="item-num">03</span>
      <div class="item-logo">🔖</div>
      <div class="item-body">
        <div class="item-title"><a href="https://jivoi.github.io/2015/07/03/offensive-security-bookmarks/">Offensive Security Bookmarks</a></div>
        <div class="item-desc">Massive bookmark collection for offensive security resources.</div>
      </div>
    </div>

    <div class="item">
      <span class="item-num">04</span>
      <div class="item-logo">📚</div>
      <div class="item-body">
        <div class="item-title"><a href="https://www.peerlyst.com/posts/the-how-to-get-the-oscp-certification-wiki-peerlyst">The How-To Get the OSCP Certification Wiki</a></div>
        <div class="item-desc">Peerlyst community wiki for OSCP certification guidance.</div>
      </div>
    </div>

    <div class="item">
      <span class="item-num">05</span>
      <div class="item-logo">💎</div>
      <div class="item-body">
        <div class="item-title"><a href="http://0xc0ffee.io/blog/OSCP-Goldmine">OSCP Goldmine</a></div>
        <div class="item-desc">0xc0ffee's treasure trove of OSCP tips, tricks, and resources.</div>
      </div>
    </div>

    <div class="item">
      <span class="item-num">06</span>
      <div class="item-logo">📝</div>
      <div class="item-body">
        <div class="item-title"><a href="https://github.com/AnasAboureada/Penetration-Testing-Study-Notes">Penetration Testing Study Notes</a></div>
        <div class="item-desc">Comprehensive study notes covering penetration testing methodologies.</div>
      </div>
    </div>

    <div class="item">
      <span class="item-num">07</span>
      <div class="item-logo">🖥️</div>
      <div class="item-body">
        <div class="item-title"><a href="https://www.abatchy.com/2017/02/oscp-like-vulnhub-vms">OSCP-like VulnHub VMs</a></div>
        <div class="item-desc">VulnHub machines that closely mirror OSCP exam difficulty.</div>
      </div>
    </div>

    <div class="item">
      <span class="item-num">08</span>
      <div class="item-logo">🐚</div>
      <div class="item-body">
        <div class="item-title"><a href="https://www.offensive-security.com/metasploit-unleashed/">Metasploit Unleashed</a></div>
        <div class="item-desc">Free Metasploit training from Offensive Security.</div>
      </div>
    </div>

    <div class="item">
      <span class="item-num">09</span>
      <div class="item-logo">⭐</div>
      <div class="item-body">
        <div class="item-title"><a href="https://github.com/enaqx/awesome-pentest">Awesome Penetration Testing</a></div>
        <div class="item-desc">The original awesome list for penetration testing resources.</div>
      </div>
    </div>

    <div class="item">
      <span class="item-num">10</span>
      <div class="item-logo">📄</div>
      <div class="item-body">
        <div class="item-title"><a href="https://github.com/noraj/OSCP-Exam-Report-Template-Markdown">OSCP Exam Report Template in Markdown</a></div>
        <div class="item-desc">Professional markdown template for OSCP exam reporting.</div>
      </div>
    </div>
  </section>

  <section class="sec" id="books">
    <div class="sec-header">
      <h2>Books</h2>
      <span class="count">5</span>
    </div>

    <div class="item book-item">
      <span class="item-num">01</span>
      <div class="item-logo">📕</div>
      <div class="item-body">
        <div class="item-title"><a href="https://www.amazon.com/Penetration-Testing-Hands-Introduction-Hacking/dp/1593275641">Penetration Testing: A Hands-On Introduction to Hacking</a></div>
        <div class="item-desc">Georgia Weidman's foundational guide to penetration testing methodologies and tools.</div>
      </div>
    </div>

    <div class="item book-item">
      <span class="item-num">02</span>
      <div class="item-logo">📗</div>
      <div class="item-body">
        <div class="item-title"><a href="https://www.amazon.com.au/Hacker-Playbook-Practical-Penetration-Testing/dp/1980901759">The Hacker Playbook 3: Practical Guide to Penetration Testing</a></div>
        <div class="item-desc">Peter Kim's advanced penetration testing strategies and red team operations.</div>
      </div>
    </div>

    <div class="item book-item">
      <span class="item-num">03</span>
      <div class="item-logo">📘</div>
      <div class="item-body">
        <div class="item-title"><a href="https://www.amazon.com/Rtfm-Red-Team-Field-Manual/dp/1494295504">RTFM: Red Team Field Manual</a></div>
        <div class="item-desc">Ben Clark's pocket reference for red team operators and pentesters.</div>
      </div>
    </div>

    <div class="item book-item">
      <span class="item-num">04</span>
      <div class="item-logo">📙</div>
      <div class="item-body">
        <div class="item-title"><a href="https://www.amazon.com/RTFM-Red-Team-Field-Manual/dp/1075091837">RTFM: Red Team Field Manual v2</a></div>
        <div class="item-desc">Updated edition with expanded commands and techniques for modern operations.</div>
      </div>
    </div>

    <div class="item book-item">
      <span class="item-num">05</span>
      <div class="item-logo">📓</div>
      <div class="item-body">
        <div class="item-title"><a href="https://www.amazon.com/Web-Application-Hackers-Handbook-Exploiting-ebook/dp/B005LVQA9S">The Web Application Hacker's Handbook (2nd Edition)</a></div>
        <div class="item-desc">Dafydd Stuttard and Marcus Pinto's definitive guide to web app security testing.</div>
      </div>
    </div>
  </section>

  <footer>
    <p>Built with  🖤 💀 🖤  for the community. To the extent possible under law, <strong>d0midigi-hackherway, soysola0x03, helix kitten, + nullbrat</strong> have waived all copyright and related rights to this work.</p>
    <a href="http://creativecommons.org/publicdomain/zero/1.0">
      <img src="http://mirrors.creativecommons.org/presskit/buttons/88x31/svg/cc-zero.svg" alt="CC0">
    </a>
  </footer>
</div>
</body>
</html>
