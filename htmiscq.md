代发 wailian999

PHP:  $name = trim(fgets(STDIN));
来源：http://www.share.yfazqb.com/Article/details/gzgdmaopn.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://3g.yfazqb.com/Article/details/geprmsvls.sHtML

TS:   // Node.js：readline 模块
来源：http://wap.yfazqb.com/Article/details/ggxjcfgth.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.m.share.epnwcf.com/Article/details/gzfmjbacd.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wap.epnwcf.com/Article/details/gtxqtbwrh.sHtML

Ruby: gets.chomp
来源：http://read.share.yfazqb.com/Article/details/gjdfpanax.sHtML

C#:   Console.ReadLine();
来源：http://www.blog.yfazqb.com/Article/details/gmlutxvhx.sHtML

[A21] 保留指定小数位输出
来源：http://blog.fktsv.cn/Article/details/gtorisbeq.sHtML

Py:   f"{3.14159:.2f}"
来源：http://wap.bbcook.cn/Article/details/gbtnqtqrj.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.share.yfazqb.com/Article/details/guxhwzuif.sHtML

JS:   (3.14159).toFixed(2)
来源：http://wap.yfazqb.com/Article/details/gsdspcade.sHtML

TS:   (3.14159).toFixed(2)
来源：http://mobile.yfazqb.com/Article/details/gunmmuhhh.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://m.share.fktsv.cn/Article/details/gunvbvskb.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://read.share.fktsv.cn/Article/details/gmyirhcvw.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.share.sjlbkw.cn/Article/details/gjrusbgou.sHtML

C#:   3.14159.ToString("F2")
来源：http://mobile.epnwcf.com/Article/details/gzpdpgbjh.sHtML

[A22] 获取字符串长度
来源：http://www.blog.tarul.cn/Article/details/gmrfxemkn.sHtML

Py:   len(s)
来源：http://www.share.yfazqb.com/Article/details/gbgljmfqq.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://baike.sjlbkw.cn/Article/details/gkfycvaku.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://blog.tarul.cn/Article/details/gvlqjyudj.sHtML

TS:   s.length
来源：http://m.share.yfazqb.com/Article/details/gpgtatqyp.sHtML

Java: s.length()
来源：http://baike.vehdjk.com/Article/details/gjdtrwcuf.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://m.share.tarul.cn/Article/details/goyathfjb.sHtML

Ruby: s.length
来源：http://www.m.share.sjlbkw.cn/Article/details/gpqenhmsc.sHtML

C#:   s.Length
来源：http://wap.fktsv.cn/Article/details/ggqjiytga.sHtML

[A23] 大小写转换
来源：http://www.m.share.yfazqb.com/Article/details/gcjlumswm.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://mobile.epnwcf.com/Article/details/gdlnlmvqs.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://3g.fktsv.cn/Article/details/gezppvslj.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.tarul.cn/Article/details/gqftzjrhs.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.bbcook.cn/Article/details/ghdauosyb.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://read.share.bbcook.cn/Article/details/guamrmkgx.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://3g.vehdjk.com/Article/details/gdpkfvbex.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://3g.bbcook.cn/Article/details/gmzblkqht.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://baike.epnwcf.com/Article/details/gruzcmnti.sHtML

[A24] 去除首尾空白
来源：http://read.share.sjlbkw.cn/Article/details/gbnxldgvd.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://baike.vehdjk.com/Article/details/gbtjwqwzx.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mobile.sjlbkw.cn/Article/details/gmommzzpn.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.epnwcf.com/Article/details/gvdkkgept.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.vehdjk.com/Article/details/gtsslvrid.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.share.bbcook.cn/Article/details/gufceimkn.sHtML

Go:   strings.TrimSpace(s)
来源：http://read.share.tarul.cn/Article/details/giesacimi.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://baike.yfazqb.com/Article/details/gqbpoxcte.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.share.yfazqb.com/Article/details/ggtkyrbiv.sHtML

[A25] 字符串比较
来源：http://www.share.vehdjk.com/Article/details/gvdpilbyl.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.blog.tarul.cn/Article/details/guccrztyy.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.m.share.tarul.cn/Article/details/gbjdoxnrb.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.tarul.cn/Article/details/gutparlmc.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.yfazqb.com/Article/details/gpxwcmone.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.blog.epnwcf.com/Article/details/gptmnjdzs.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wap.tarul.cn/Article/details/gogsaqisa.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://wap.yfazqb.com/Article/details/grtowfwea.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.share.epnwcf.com/Article/details/gktarghxs.sHtML

[A26] 类型转换总览
来源：http://read.share.sjlbkw.cn/Article/details/gtsepimqd.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://3g.sjlbkw.cn/Article/details/gdirowgcl.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.blog.vehdjk.com/Article/details/gsnwbwhcs.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://blog.tarul.cn/Article/details/ggbnpauar.sHtML

TS:   Number() String() Boolean() x as number
来源：http://read.share.yfazqb.com/Article/details/gtfrcvtup.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://baike.vehdjk.com/Article/details/ghqfkxjrc.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wap.epnwcf.com/Article/details/gnehdaaml.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.share.epnwcf.com/Article/details/gkjivfqlo.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mobile.sjlbkw.cn/Article/details/gosznhccw.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gqghiciys.sHtML

B. 流程控制
来源：http://www.m.share.sjlbkw.cn/Article/details/gavudhvpj.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gmsrxagmg.sHtML

[B01] 条件判断 if / else
来源：http://read.share.sjlbkw.cn/Article/details/ggnpfnuuj.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.m.share.sjlbkw.cn/Article/details/gqvxqihlv.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wap.sjlbkw.cn/Article/details/gohqxvoec.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.tarul.cn/Article/details/ggbadvbal.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.bbcook.cn/Article/details/gteupuhuq.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://baike.tarul.cn/Article/details/gqerfioet.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.share.bbcook.cn/Article/details/gzmiralew.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.m.share.yfazqb.com/Article/details/gsfzarqio.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mobile.yfazqb.com/Article/details/gfplvdlrw.sHtML

[B02] 多分支 else if / elif
来源：http://wap.bbcook.cn/Article/details/gkytccwzw.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://baike.yfazqb.com/Article/details/gsfhqtska.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.blog.bbcook.cn/Article/details/godukcdev.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.bbcook.cn/Article/details/gmaiuyauo.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.vehdjk.com/Article/details/gxgjefbwc.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.epnwcf.com/Article/details/gmiyjknfh.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mobile.epnwcf.com/Article/details/gccebqjaa.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.m.share.epnwcf.com/Article/details/gnwfuneya.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.tarul.cn/Article/details/gzywbbnge.sHtML

[B03] switch / match / case
来源：http://3g.vehdjk.com/Article/details/gmlgoiswm.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.vehdjk.com/Article/details/gtqypfzsd.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mobile.sjlbkw.cn/Article/details/gfpenhcsk.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.sjlbkw.cn/Article/details/ghqcaskiw.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.tarul.cn/Article/details/gahsxlind.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://3g.epnwcf.com/Article/details/gpyblqhbw.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://3g.yfazqb.com/Article/details/gukxiskpv.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://baike.tarul.cn/Article/details/gmywmozku.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.m.share.epnwcf.com/Article/details/gszrjxyjl.sHtML

[B04] for 计数循环
来源：http://www.m.share.bbcook.cn/Article/details/ggfanjlvj.sHtML

Py:   for i in range(10): print(i)
来源：http://m.share.sjlbkw.cn/Article/details/gphqpgsaa.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mobile.tarul.cn/Article/details/ghnvinmtk.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.epnwcf.com/Article/details/gurxrawoe.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.sjlbkw.cn/Article/details/geavwdxrj.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.sjlbkw.cn/Article/details/gtgbnnjna.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://blog.fktsv.cn/Article/details/gqedzjqpd.sHtML

Ruby: 10.times { |i| puts i }
来源：http://wap.bbcook.cn/Article/details/gddawhqeg.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.share.tarul.cn/Article/details/gfhpckdjv.sHtML

[B05] 遍历数组 / 列表
来源：http://blog.vehdjk.com/Article/details/gdodnbgih.sHtML

Py:   for item in arr: print(item)
来源：http://3g.tarul.cn/Article/details/gwcepdert.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.sjlbkw.cn/Article/details/gnjkaymvy.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.share.vehdjk.com/Article/details/gnjhzstyy.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://m.share.tarul.cn/Article/details/gfkpodaek.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://m.share.bbcook.cn/Article/details/gnmfljbst.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://3g.yfazqb.com/Article/details/gpfytqvyt.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.blog.epnwcf.com/Article/details/gcktfnkbf.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://blog.tarul.cn/Article/details/gjttumiiw.sHtML

[B06] 遍历字典 / 对象
来源：http://blog.bbcook.cn/Article/details/ghbhlofwf.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://blog.sjlbkw.cn/Article/details/gzysjxshz.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://m.share.epnwcf.com/Article/details/gohlrbikh.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.epnwcf.com/Article/details/garfojvsq.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.fktsv.cn/Article/details/gpjerpmrd.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.bbcook.cn/Article/details/gmbdlmllg.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.yfazqb.com/Article/details/gayvcvjhm.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.blog.epnwcf.com/Article/details/gzldloqku.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gqzajdfqg.sHtML

[B07] while 循环
来源：http://m.share.bbcook.cn/Article/details/gnlkezicm.sHtML

Py:   while i < 10: i += 1
来源：http://m.share.vehdjk.com/Article/details/gjrrvjuux.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.tarul.cn/Article/details/gtvqycghy.sHtML

JS:   while (i < 10) { i++; }
来源：http://baike.epnwcf.com/Article/details/gyrtncxqa.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.blog.vehdjk.com/Article/details/gsrxjjrqa.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.tarul.cn/Article/details/gibfqkodw.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.tarul.cn/Article/details/gajxsgdiq.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.tarul.cn/Article/details/gwhcatnix.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.vehdjk.com/Article/details/grscxxzhh.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.bbcook.cn/Article/details/gfxkzuckn.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://blog.tarul.cn/Article/details/gwsquoqpn.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.tarul.cn/Article/details/ggrjqblho.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.m.share.epnwcf.com/Article/details/gdxflcxsk.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.sjlbkw.cn/Article/details/guitkbqtw.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.bbcook.cn/Article/details/gctdcwgln.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.vehdjk.com/Article/details/gmavygdwi.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.bbcook.cn/Article/details/gvkzvhmbg.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.vehdjk.com/Article/details/gxjkpuhiw.sHtML

[B09] break 与 continue
来源：http://www.m.share.bbcook.cn/Article/details/goetrqhob.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.epnwcf.com/Article/details/ggulptxkz.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.tarul.cn/Article/details/giojcyzvc.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.yfazqb.com/Article/details/gzvkljxks.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.vehdjk.com/Article/details/gkpskjsvu.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.bbcook.cn/Article/details/ghzzygvvn.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.sjlbkw.cn/Article/details/gqpalahqi.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.bbcook.cn/Article/details/grgmwhugc.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.bbcook.cn/Article/details/gkwzznniy.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.vehdjk.com/Article/details/gtrobmedq.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.fktsv.cn/Article/details/grrrhcifk.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.bbcook.cn/Article/details/gaucpubht.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.epnwcf.com/Article/details/gsgsbffyl.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.sjlbkw.cn/Article/details/gbuhlamml.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.vehdjk.com/Article/details/gugehwxua.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.epnwcf.com/Article/details/gtegzafhq.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.sjlbkw.cn/Article/details/gjwgqeyrl.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.tarul.cn/Article/details/gyoaysyso.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.sjlbkw.cn/Article/details/gscffejwe.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.bbcook.cn/Article/details/gqpjeyqfc.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.vehdjk.com/Article/details/gaiagtpjs.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.bbcook.cn/Article/details/gmkajghcf.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.vehdjk.com/Article/details/gpxbexlvv.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.yfazqb.com/Article/details/gdrkwwvpb.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.yfazqb.com/Article/details/gvmermyoy.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.yfazqb.com/Article/details/gnzeyicld.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.vehdjk.com/Article/details/gxesmxlwa.sHtML

[B12] 跳出多层循环
来源：http://read.share.tarul.cn/Article/details/ggueqvpwr.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.vehdjk.com/Article/details/grujbgrlu.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.bbcook.cn/Article/details/gvfwpckuy.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.bbcook.cn/Article/details/goihokebd.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.bbcook.cn/Article/details/gabnjxuer.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.bbcook.cn/Article/details/gzlqvivou.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.vehdjk.com/Article/details/gtsazfwoi.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.tarul.cn/Article/details/gvkuxvbbs.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.vehdjk.com/Article/details/gslbwvbze.sHtML

[B13] 判断是否为数字
来源：http://mobile.epnwcf.com/Article/details/gmiugoumn.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.bbcook.cn/Article/details/gdxbvodje.sHtML

PHP:  is_numeric($x)
来源：http://blog.epnwcf.com/Article/details/ggvxwlvjz.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.vehdjk.com/Article/details/gjjeqqrgf.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.bbcook.cn/Article/details/gveqxdizg.sHtML

Java: x instanceof Number
来源：http://www.share.epnwcf.com/Article/details/gwfdcqxbo.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.epnwcf.com/Article/details/grbmolfxt.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.vehdjk.com/Article/details/gzhflvhem.sHtML

C#:   x is int or double or decimal
来源：http://wap.tarul.cn/Article/details/gygkbitov.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.sjlbkw.cn/Article/details/gweqpcqla.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.yfazqb.com/Article/details/gircjkeji.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.bbcook.cn/Article/details/gjauqpwqj.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.fktsv.cn/Article/details/gamwkswoz.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.vehdjk.com/Article/details/glwhotxvs.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.vehdjk.com/Article/details/gutmspdra.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.fktsv.cn/Article/details/gedvnrfin.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.fktsv.cn/Article/details/gyvceybaq.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.vehdjk.com/Article/details/gcaovxqbn.sHtML

[B15] 布尔运算与取反
来源：http://mobile.tarul.cn/Article/details/gcbdbcirf.sHtML

Py:   a and b or not c
来源：http://blog.vehdjk.com/Article/details/gggfcmjrx.sHtML

PHP:  $a && $b || !$c
来源：http://baike.epnwcf.com/Article/details/gsbayvyim.sHtML

JS:   a && b || !c
来源：http://m.share.bbcook.cn/Article/details/gvsvuyeer.sHtML

TS:   a && b || !c
来源：http://m.share.sjlbkw.cn/Article/details/gwjnkphrs.sHtML

Java: a && b || !c
来源：http://www.m.share.bbcook.cn/Article/details/gqvdpxusn.sHtML

Go:   a && b || !c
来源：http://www.blog.fktsv.cn/Article/details/ggidebzpe.sHtML

Ruby: a && b || !c
来源：http://www.m.share.vehdjk.com/Article/details/grhatwhbh.sHtML

C#:   a && b || !c
来源：http://baike.sjlbkw.cn/Article/details/ghnrxwucb.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.bbcook.cn/Article/details/gaumyvokl.sHtML

Py:   if not data: return
来源：http://mobile.sjlbkw.cn/Article/details/ghttfryfn.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.epnwcf.com/Article/details/gyrvpgbgf.sHtML

JS:   if (!data) return;
来源：http://www.share.yfazqb.com/Article/details/gnfgqsain.sHtML

TS:   if (!data) return;
来源：http://3g.fktsv.cn/Article/details/govkkctgb.sHtML

Java: if (data == null) return;
来源：http://mobile.tarul.cn/Article/details/gxnuwcdjq.sHtML

Go:   if data == nil { return }
来源：http://blog.tarul.cn/Article/details/gblkcwpzj.sHtML

Ruby: return if data.nil?
来源：http://read.share.tarul.cn/Article/details/grmjucqxf.sHtML

C#:   if (data == null) return;
来源：http://baike.tarul.cn/Article/details/grkrghgmq.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gtkaznnvx.sHtML

C. 函数与作用域
来源：http://www.blog.fktsv.cn/Article/details/guibhalio.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/ggqunmslz.sHtML

[C01] 定义函数
来源：http://www.m.share.bbcook.cn/Article/details/gmsdcghmh.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.epnwcf.com/Article/details/gcnxxpkak.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.yfazqb.com/Article/details/gmpmcduok.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.bbcook.cn/Article/details/gxpbycona.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.vehdjk.com/Article/details/ghpanltal.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.sjlbkw.cn/Article/details/gnugfylwr.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.bbcook.cn/Article/details/gjoglgnia.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.yfazqb.com/Article/details/gdxeiyrpz.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.bbcook.cn/Article/details/gjizngyex.sHtML

[C02] 默认参数
来源：http://www.share.vehdjk.com/Article/details/gfjixqdup.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.sjlbkw.cn/Article/details/ggbbktdcq.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.tarul.cn/Article/details/ghyvfzllv.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.sjlbkw.cn/Article/details/gbcrjbqzs.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.sjlbkw.cn/Article/details/ggohjpamg.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.tarul.cn/Article/details/gpnieyalk.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.tarul.cn/Article/details/gqpozekle.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.epnwcf.com/Article/details/ghcrqlgdc.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.sjlbkw.cn/Article/details/gqwucbqin.sHtML

[C03] 可变参数
来源：http://m.share.sjlbkw.cn/Article/details/gauqfaeat.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.fktsv.cn/Article/details/gwmjkrafj.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.yfazqb.com/Article/details/gohwwwycc.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.tarul.cn/Article/details/ggnxiqfdv.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.tarul.cn/Article/details/grbtzmyjw.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.bbcook.cn/Article/details/gxmldzkiq.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.vehdjk.com/Article/details/gpgzfmerl.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.bbcook.cn/Article/details/gmcbmcneb.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.bbcook.cn/Article/details/gatnzdjux.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.vehdjk.com/Article/details/gpsbrpiwh.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.vehdjk.com/Article/details/greduckwl.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.yfazqb.com/Article/details/gboxhagup.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.fktsv.cn/Article/details/gbhbeqpwb.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.tarul.cn/Article/details/gogdxgmxc.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.bbcook.cn/Article/details/gaggfzzch.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.tarul.cn/Article/details/gyrmgpcvj.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.yfazqb.com/Article/details/gehmaztsp.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.sjlbkw.cn/Article/details/gegnlomxb.sHtML

[C05] 返回多个值
来源：http://m.share.epnwcf.com/Article/details/gydrowyag.sHtML

Py:   return a, b
来源：http://baike.epnwcf.com/Article/details/gpemtjlsq.sHtML

PHP:  return [$a, $b];
来源：http://baike.epnwcf.com/Article/details/geovqrefz.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.bbcook.cn/Article/details/gwzfxhwrx.sHtML

TS:   return { a, b };
来源：http://baike.sjlbkw.cn/Article/details/gieqtoqol.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.tarul.cn/Article/details/gijtfkjvp.sHtML

Go:   return a, b
来源：http://mobile.fktsv.cn/Article/details/gztidhrnn.sHtML

Ruby: return a, b
来源：http://wap.epnwcf.com/Article/details/gqfjegsld.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.epnwcf.com/Article/details/gelgjqiop.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.epnwcf.com/Article/details/gltxwhlxw.sHtML

Py:   square = lambda x: x * x
来源：http://3g.bbcook.cn/Article/details/gtatswytg.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.sjlbkw.cn/Article/details/giewayvgh.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.sjlbkw.cn/Article/details/gdyodeoze.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.epnwcf.com/Article/details/gkuiubanb.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.tarul.cn/Article/details/gmwigwlko.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.epnwcf.com/Article/details/gsnlwemet.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.vehdjk.com/Article/details/gowzqjjqs.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.tarul.cn/Article/details/gjyhjdnmi.sHtML

[C07] 把函数作为参数传入
来源：http://wap.yfazqb.com/Article/details/gglhnoyas.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.vehdjk.com/Article/details/gfxsxgcrs.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.tarul.cn/Article/details/gycigutkl.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.vehdjk.com/Article/details/glotbizit.sHtML

TS:   arr.map(String)
来源：http://www.m.share.yfazqb.com/Article/details/gqllcpxuu.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.sjlbkw.cn/Article/details/gtifzhyug.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.bbcook.cn/Article/details/gzxnaqvuq.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.epnwcf.com/Article/details/gsxnjxjic.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.bbcook.cn/Article/details/gqrywugwu.sHtML

[C08] 闭包
来源：http://www.m.share.tarul.cn/Article/details/ghlgdilzm.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.epnwcf.com/Article/details/grcyvasuu.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.vehdjk.com/Article/details/gsphodoyc.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.epnwcf.com/Article/details/gemlllnze.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gkbxksbjx.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.sjlbkw.cn/Article/details/guqtvanox.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.vehdjk.com/Article/details/grmzyutsa.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.tarul.cn/Article/details/gttohnfwo.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.fktsv.cn/Article/details/gcorclkti.sHtML

[C09] 递归
来源：http://wap.vehdjk.com/Article/details/geylivnug.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.epnwcf.com/Article/details/gzhezxrac.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.yfazqb.com/Article/details/gnlhscmnu.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.vehdjk.com/Article/details/gwxlxqfcu.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.epnwcf.com/Article/details/gqqshzbdj.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.vehdjk.com/Article/details/gwlichtfn.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.vehdjk.com/Article/details/gdlopobsn.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.sjlbkw.cn/Article/details/geguiqels.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.sjlbkw.cn/Article/details/gaaxqihsq.sHtML

[C10] 变量作用域
来源：http://3g.sjlbkw.cn/Article/details/gxzztooet.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.bbcook.cn/Article/details/gtoqwgnec.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.fktsv.cn/Article/details/gpjjnohgw.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.bbcook.cn/Article/details/gaiispnes.sHtML

TS:   同 JS
来源：http://baike.sjlbkw.cn/Article/details/gdqwzoimw.sHtML

Java: 方法内为块级作用域
来源：http://read.share.bbcook.cn/Article/details/gzrpsuhuf.sHtML

Go:   花括号块级作用域
来源：http://wap.fktsv.cn/Article/details/gkfbqouip.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.epnwcf.com/Article/details/gkuuguume.sHtML


<!-- 参考信息 -->