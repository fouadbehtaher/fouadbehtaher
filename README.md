<h2>Hey 👋, I'm <a href="https://d9f0z96nghtsz.cloudfront.net/">Fouad Taher</a></h2>
<p>I'm currently a CyberSecurity Engineer. I am working on some side projects, learning a couple new dishes,Currently pursuing a Bachelor’s degree in Information Technology and Computing with a focus on Cyber Security at Arab Open University and The Open University. Actively contributing as a member of the Student Council at AOU, showcasing leadership and collaboration.  
.</p>
<p><a href="https://d9f0z96nghtsz.cloudfront.net/"><img src="https://img.shields.io/badge/-d9f0z96nghtsz.cloudfront.net-4E69C8?style=flat-square&amp;labelColor=4E69C8&amp;logo=Firefox" alt="Website Badge"></a> <a href="https://medium.com/@fouadbehtaher"><img src="https://img.shields.io/badge/-@fouadbehtaher-14c767?style=flat-square&amp;labelColor=14c767&amp;logo=Medium" alt="Medium Badge"></a> <a href="https://www.linkedin.com/in/fouadbehtaher/"><img src="https://img.shields.io/badge/-@fouadbehtaher-0077B5?style=flat-square&amp;labelColor=0077B5&amp;logo=LinkedIn" alt="LinkedIn Badge"></a> <a href="#"><img src="https://img.shields.io/badge/-@Fouad%20Taher-1ED760?style=flat-square&amp;labelColor=fff&amp;logo=Spotify" alt="Spotify Badge"></a></p>
<p>🍌 Don't forget to get some Potassium 🍌</p>
<img align="right" src="https://media1.giphy.com/media/13HgwGsXF0aiGY/giphy.gif" />
<h2>⚡️ A Few Quick Facts</h2>
<ul>
<li>🔭 I’m currently working on <a href="https://github.com/fouadbehtaher/waff-app-new">WAF</a>.</li>
<li>🧐 Learning about <strong>serverless architectures</strong>, <strong>distributed systems</strong>, and a bit of <strong>ML</strong>.</li>
<li>👨‍💻 Most of my projects are available on <a href="https://github.com/fouadbehtaher/">Github</a>.</li>
<li>📝 I <del>regularly</del> write articles on <a href="https://d9f0z96nghtsz.cloudfront.net/">my site</a>.</li>
<li>💬 Ping me about <strong>react, koa, security, and cloud stuff</strong>.</li>
<li>📙 Check out my <a href="https://d9f0z96nghtsz.cloudfront.net/">resume</a>.</li>
<li>🎉 Fun Fact: 我也会讲中文。</li>
</ul>
<h2>🤝 Open Source Contributions</h2>
<h3>✅ Merged: <a href="https://github.com/msoedov/agentic_security">msoedov/agentic_security</a> (2,000+ ⭐) — Agentic LLM Vulnerability Scanner / AI red-teaming kit</h3>
<p><strong><a href="https://github.com/msoedov/agentic_security/pull/404">PR #404 — fix(http_spec): make LLMSpec.model_name always return a string</a></strong> · reviewed and merged by the maintainer on Nov 27, 2026 (<em>"LGTM, thx for the patch"</em>).</p>
<ul>
<li><strong>The find:</strong> while reading the scanner's request-handling code, <code>LLMSpec.model_name</code> was documented to return the request body's <code>model</code> field, or <code>"unknown"</code>. Two edge cases broke that contract: (1) a body that is valid JSON but not an object (<code>[1, 2]</code>, <code>"text"</code>, <code>null</code>) raised <code>AttributeError</code> on <code>.get</code> — the fuzzer only survived because a <code>getattr(..., "unknown")</code> happened to swallow it; (2) a non-string <code>model</code> (<code>null</code>, a number, a list, an object) was returned as-is, and a list or dict then reached <code>calculate_cost</code>, where <code>model not in PRICING</code> raised <code>TypeError: unhashable type</code>, crashing cost accounting mid-scan.</li>
<li><strong>The fix:</strong> <code>model_name</code> now returns <code>"unknown"</code> unless the body is a JSON object whose <code>model</code> is a non-empty string (+11/−2 lines, one behavior only).</li>
<li><strong>The proof:</strong> 14 new tests (13 parametrized edge cases plus a check that the result is safe to pass to <code>calculate_cost</code>); 10 of them fail against the original code and pass with the fix. Full suite: 538 passed, 2 skipped; <code>black</code> and <code>flake8</code> clean.</li>
</ul>
<h3>🔍 More contributions in review</h3>
<ul>
<li><a href="https://github.com/NVIDIA/garak/pull/2534">NVIDIA/garak #2534</a> (10k ⭐ LLM vulnerability scanner) — new <code>lmrc.Misogyny</code> probe and detector.</li>
<li><a href="https://github.com/promptfoo/promptfoo/pull/12656">promptfoo/promptfoo #12656</a> — legal-vertical red team plugins.</li>
<li><a href="https://github.com/Skyscanner/cfripper/pull/483">Skyscanner/cfripper #483</a> — new <code>RDSInstancePubliclyAccessibleRule</code> flagging publicly accessible RDS databases (HIGH risk).</li>
<li><a href="https://github.com/cisco-ai-defense/mcp-scanner/pull/328">cisco-ai-defense/mcp-scanner #328</a> — detect instructions hidden by Unicode obfuscation before YARA rule matching.</li>
<li><a href="https://github.com/CERT-Polska/Artemis/pull/3506">CERT-Polska/Artemis #3506</a> — keep <code>www.&lt;domain&gt;</code> in the wildcard subdomain filter instead of a bare "www".</li>
<li><a href="https://github.com/projectdiscovery/nuclei-templates/pull/18132">projectdiscovery/nuclei-templates #18132</a> — detection template for CVE-2026-136716 (Drupal core exposed-installer access bypass).</li>
<li><a href="https://github.com/Monesgoda/AgntX-Hunter/pull/3">Monesgoda/AgntX-Hunter #3</a> — fix three fail-open bugs in scope gating, with unit tests.</li>
</ul>
<h2>✒️ Recent Posts</h2>
<p><a target="_blank" href="https://d9f0z96nghtsz.cloudfront.net/">Visit my website</a></p>
<h2>🚀 Some Tools I Use</h2>
<p align="left">
<img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/react/react-original-wordmark.svg" alt="react" width="25" />
<img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/angularjs/angularjs-original.svg" alt="angular-js" width="25" />
<img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/vuejs/vuejs-original.svg" alt="vue" width="25" />
<img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/bootstrap/bootstrap-plain.svg" alt="bootstrap" width="25" />
<img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/css3/css3-original-wordmark.svg" alt="css3" width="25" />
<img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/gulp/gulp-plain.svg" alt="gulp" width="25" />
<img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/java/java-original-wordmark.svg" alt="java" width="25" />
<img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/javascript/javascript-original.svg" alt="javascript" width="25" />
<img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/typescript/typescript-original.svg" alt="typescript" width="25" />
<img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/dot-net/dot-net-original.svg" alt=".NET" width="25" />
<img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/mongodb/mongodb-original.svg" alt="mongodb" width="25" />
<img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/mysql/mysql-original-wordmark.svg" alt="mysql" width="25" />
<img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/redis/redis-original-wordmark.svg" alt="redis" width="25" />
<img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/nodejs/nodejs-original-wordmark.svg" alt="nodejs" width="25" />
<img src="https://www.vectorlogo.zone/logos/springio/springio-icon.svg" alt="spring" width="25" />
<img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/python/python-original-wordmark.svg" alt="python" width="25" />
<img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/nginx/nginx-original.svg" alt="nginx" width="25" />
<img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/cucumber/cucumber-plain.svg" alt="cucumber" width="25" />
<img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/heroku/heroku-plain.svg" alt="heroku" width="25" />
<img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/travis/travis-plain.svg" alt="travis" width="25" />
<img src="https://raw.githubusercontent.com/github/explore/80688e429a7d4ef2fca1e82350fe8e3517d3494d/topics/aws/aws.png" alt="aws" width="25" />
<img src="https://www.vectorlogo.zone/logos/google_cloud/google_cloud-icon.svg" alt="gcp" width="25" />
<img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/docker/docker-original.svg" alt="Docker" width="25" />
<img src="https://www.vectorlogo.zone/logos/kubernetes/kubernetes-icon.svg" alt="Kubernetes" width="25" />
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/go/go-original.svg" alt="Go" width="25" />
</p>
<img src="https://github-readme-stats.vercel.app/api?username=fouadbehtaher&show_icons=true&count_private=true" alt="fouadbehtaher" />
<p><a href="http://hits.dwyl.com/fouadbehtaher/fouadbehtaher/fouadbehtaher.svg?style=flat-square"><img src="https://hits.dwyl.com/fouadbehtaher/fouadbehtaher/fouadbehtaher.svg?style=flat-square" alt="HitCount"></a></p>
