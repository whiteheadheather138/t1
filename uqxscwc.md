代发 wailian999

C#:   (int)'A'; (char)65
来源：http://read.share.yfazqb.com/Article/details/gjxvzuuhu.sHtML

[A19] 交换两个变量
来源：http://read.share.vehdjk.com/Article/details/gvvlfhmqp.sHtML

Py:   a, b = b, a
来源：http://www.blog.epnwcf.com/Article/details/gxgoptaro.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://m.share.epnwcf.com/Article/details/gfcluntxf.sHtML

JS:   [a, b] = [b, a];
来源：http://read.share.vehdjk.com/Article/details/gewrcshsp.sHtML

TS:   [a, b] = [b, a];
来源：http://3g.epnwcf.com/Article/details/gpoihrddd.sHtML

Java: int t = a; a = b; b = t;
来源：http://read.share.tarul.cn/Article/details/glnakwalg.sHtML

Go:   a, b = b, a
来源：http://wap.sjlbkw.cn/Article/details/ghlwzeswz.sHtML

Ruby: a, b = b, a
来源：http://www.m.share.fktsv.cn/Article/details/gduxofqsv.sHtML

C#:   (a, b) = (b, a);
来源：http://read.share.fktsv.cn/Article/details/gdiiueeze.sHtML

[A20] 读取标准输入
来源：http://mobile.yfazqb.com/Article/details/guhsodsaw.sHtML

Py:   name = input("请输入：")
来源：http://www.share.yfazqb.com/Article/details/gjnddoehi.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.share.fktsv.cn/Article/details/gwclyrlmi.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://m.share.tarul.cn/Article/details/gaoksapph.sHtML

TS:   // Node.js：readline 模块
来源：http://blog.vehdjk.com/Article/details/ghcbrkkes.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.blog.yfazqb.com/Article/details/gxmwbfnuk.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://mobile.epnwcf.com/Article/details/gbdglrfsz.sHtML

Ruby: gets.chomp
来源：http://www.share.bbcook.cn/Article/details/ghspzlinj.sHtML

C#:   Console.ReadLine();
来源：http://www.blog.epnwcf.com/Article/details/guizlvsva.sHtML

[A21] 保留指定小数位输出
来源：http://m.share.tarul.cn/Article/details/gunrduqdn.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.blog.sjlbkw.cn/Article/details/gboigamao.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.share.yfazqb.com/Article/details/gupkjbfbg.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.share.vehdjk.com/Article/details/gkqhxshpr.sHtML

TS:   (3.14159).toFixed(2)
来源：http://mobile.sjlbkw.cn/Article/details/gcjkmtioo.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://blog.vehdjk.com/Article/details/glfpzlhfo.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://baike.vehdjk.com/Article/details/gahwbqbod.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.m.share.epnwcf.com/Article/details/gmpvbcfts.sHtML

C#:   3.14159.ToString("F2")
来源：http://3g.tarul.cn/Article/details/gsxfgqscr.sHtML

[A22] 获取字符串长度
来源：http://m.share.tarul.cn/Article/details/gogjhopii.sHtML

Py:   len(s)
来源：http://baike.yfazqb.com/Article/details/gzcsgjbve.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://baike.sjlbkw.cn/Article/details/gufwleddi.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.blog.fktsv.cn/Article/details/geokxktlf.sHtML

TS:   s.length
来源：http://read.share.bbcook.cn/Article/details/gteocltmk.sHtML

Java: s.length()
来源：http://baike.vehdjk.com/Article/details/gavfmxtfv.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mobile.epnwcf.com/Article/details/gphxfsfjk.sHtML

Ruby: s.length
来源：http://read.share.tarul.cn/Article/details/gbavmiiud.sHtML

C#:   s.Length
来源：http://www.blog.bbcook.cn/Article/details/gjvaowfjp.sHtML

[A23] 大小写转换
来源：http://baike.yfazqb.com/Article/details/grxtammnv.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://baike.tarul.cn/Article/details/gheyhwdda.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wap.bbcook.cn/Article/details/gkrbzmpyf.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.tarul.cn/Article/details/gubdiyefx.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.bbcook.cn/Article/details/gesbtucbn.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.tarul.cn/Article/details/gnnlcrooe.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gswkjheae.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://blog.vehdjk.com/Article/details/gthckiwvq.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://read.share.vehdjk.com/Article/details/gbhtdxekg.sHtML

[A24] 去除首尾空白
来源：http://www.share.vehdjk.com/Article/details/gwugaqevk.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.m.share.tarul.cn/Article/details/gjsupnwsm.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.blog.epnwcf.com/Article/details/gzzikoczq.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.fktsv.cn/Article/details/gjakgxxak.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.bbcook.cn/Article/details/gggzoolgj.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.m.share.tarul.cn/Article/details/grvaquhaf.sHtML

Go:   strings.TrimSpace(s)
来源：http://read.share.vehdjk.com/Article/details/gtabxoiwn.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://blog.bbcook.cn/Article/details/ggqqrnuib.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wap.bbcook.cn/Article/details/gkpwjyzaz.sHtML

[A25] 字符串比较
来源：http://mobile.sjlbkw.cn/Article/details/gbjoxgcay.sHtML

Py:   s1 == s2; s1 != s2
来源：http://mobile.fktsv.cn/Article/details/gmlpmiuuu.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mobile.tarul.cn/Article/details/gbrbduwyk.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.bbcook.cn/Article/details/gcqfzvwih.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.bbcook.cn/Article/details/gnmhrcqni.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.blog.epnwcf.com/Article/details/gglnthxji.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.m.share.vehdjk.com/Article/details/gtfwpobam.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://read.share.yfazqb.com/Article/details/gavxubekq.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wap.vehdjk.com/Article/details/geichdkok.sHtML

[A26] 类型转换总览
来源：http://m.share.epnwcf.com/Article/details/gqjivoqyi.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://blog.sjlbkw.cn/Article/details/gyxldhkex.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.blog.fktsv.cn/Article/details/guzacjdme.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.m.share.fktsv.cn/Article/details/giesofjzu.sHtML

TS:   Number() String() Boolean() x as number
来源：http://read.share.sjlbkw.cn/Article/details/glhjqdlvl.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.share.epnwcf.com/Article/details/gqhzlzeva.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://m.share.vehdjk.com/Article/details/gheieczom.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://wap.fktsv.cn/Article/details/glsrvffiz.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.blog.tarul.cn/Article/details/gpzpljkzs.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gimqjuyyl.sHtML

B. 流程控制
来源：http://www.blog.yfazqb.com/Article/details/gwvtluncw.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/glhheiprb.sHtML

[B01] 条件判断 if / else
来源：http://www.share.vehdjk.com/Article/details/gthuxorus.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://wap.tarul.cn/Article/details/gykqcoaog.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://baike.yfazqb.com/Article/details/gmhoaqpar.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.yfazqb.com/Article/details/gnxmnekol.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.sjlbkw.cn/Article/details/gcisnnuey.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://mobile.bbcook.cn/Article/details/gjpnxtzyw.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://baike.yfazqb.com/Article/details/gzakufnxz.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://blog.bbcook.cn/Article/details/ggiagwtgr.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.m.share.sjlbkw.cn/Article/details/gsqxgxcej.sHtML

[B02] 多分支 else if / elif
来源：http://wap.fktsv.cn/Article/details/gjaoyasle.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.m.share.fktsv.cn/Article/details/gpcdfpovg.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wap.fktsv.cn/Article/details/gyequllyt.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.fktsv.cn/Article/details/gdihojtig.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.bbcook.cn/Article/details/gewvwqsrw.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.epnwcf.com/Article/details/gmlxjmdew.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wap.vehdjk.com/Article/details/gddziwebs.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://baike.vehdjk.com/Article/details/gprrmcyty.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.yfazqb.com/Article/details/gndaqsyxj.sHtML

[B03] switch / match / case
来源：http://www.share.sjlbkw.cn/Article/details/ghngrlkge.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.share.vehdjk.com/Article/details/gneasnnbl.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://baike.tarul.cn/Article/details/gftaijebv.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.vehdjk.com/Article/details/gqysgvlal.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.vehdjk.com/Article/details/gomrdtkwf.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mobile.fktsv.cn/Article/details/gaugdifse.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.m.share.bbcook.cn/Article/details/gbnsvmqkk.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://baike.yfazqb.com/Article/details/gnjgqujph.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.share.yfazqb.com/Article/details/geppxwfcw.sHtML

[B04] for 计数循环
来源：http://baike.sjlbkw.cn/Article/details/ghbmdpeml.sHtML

Py:   for i in range(10): print(i)
来源：http://www.share.yfazqb.com/Article/details/ggusdgjfc.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://m.share.fktsv.cn/Article/details/gkgproptk.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.fktsv.cn/Article/details/gpwwjmtyy.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.fktsv.cn/Article/details/gvxfapndv.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.share.yfazqb.com/Article/details/ggzluoerc.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.m.share.fktsv.cn/Article/details/gggkdmgeo.sHtML

Ruby: 10.times { |i| puts i }
来源：http://mobile.epnwcf.com/Article/details/gssgtvdpx.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://read.share.tarul.cn/Article/details/gaqeoovwx.sHtML

[B05] 遍历数组 / 列表
来源：http://www.share.epnwcf.com/Article/details/gscisdduq.sHtML

Py:   for item in arr: print(item)
来源：http://3g.fktsv.cn/Article/details/gywwhykxe.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://read.share.vehdjk.com/Article/details/gbfmdtlpz.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://3g.yfazqb.com/Article/details/gkdrbfwdv.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://3g.vehdjk.com/Article/details/gxqrbttzr.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.blog.yfazqb.com/Article/details/glhmzjxgl.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.share.vehdjk.com/Article/details/gtxnjnnhu.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.share.yfazqb.com/Article/details/grldfviwp.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://m.share.vehdjk.com/Article/details/ggizhsveu.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.vehdjk.com/Article/details/ghsqbvzpp.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.yfazqb.com/Article/details/gxgnxlnrp.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://3g.bbcook.cn/Article/details/gesytlyxe.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.fktsv.cn/Article/details/gncbxdvca.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.tarul.cn/Article/details/gfnpopboj.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.tarul.cn/Article/details/ghdmnmwfy.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.fktsv.cn/Article/details/gykqihadi.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.blog.sjlbkw.cn/Article/details/gzqkpozvt.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.bbcook.cn/Article/details/gpnlldipz.sHtML

[B07] while 循环
来源：http://www.blog.epnwcf.com/Article/details/gkgqdsfiu.sHtML

Py:   while i < 10: i += 1
来源：http://www.share.fktsv.cn/Article/details/gnjckigtx.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://read.share.bbcook.cn/Article/details/ggrihrfog.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.fktsv.cn/Article/details/glbxqiplv.sHtML

TS:   while (i < 10) { i++; }
来源：http://blog.epnwcf.com/Article/details/gflgybhmt.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.tarul.cn/Article/details/geunmpgvm.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.tarul.cn/Article/details/gzbrfvtuk.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.bbcook.cn/Article/details/gnkucuxpz.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.sjlbkw.cn/Article/details/gaeaohbed.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.vehdjk.com/Article/details/gzfxyeytt.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.epnwcf.com/Article/details/gdzohsvxj.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.tarul.cn/Article/details/gedubsexj.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.epnwcf.com/Article/details/giwnfynip.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.epnwcf.com/Article/details/gokyleltx.sHtML

Java: do { i++; } while (i < 10);
来源：http://blog.tarul.cn/Article/details/gsoktgaax.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.yfazqb.com/Article/details/gjsxwnkmy.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.yfazqb.com/Article/details/gkxhmtnvy.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.fktsv.cn/Article/details/gyqbjjkdl.sHtML

[B09] break 与 continue
来源：http://read.share.bbcook.cn/Article/details/gugyqouuk.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.bbcook.cn/Article/details/gcqroxljo.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://m.share.bbcook.cn/Article/details/guzfuabqj.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.sjlbkw.cn/Article/details/gueaoicfu.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.sjlbkw.cn/Article/details/gofftppcp.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.sjlbkw.cn/Article/details/gnabhlegb.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.bbcook.cn/Article/details/ggukrcrge.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.yfazqb.com/Article/details/ghasresmg.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.vehdjk.com/Article/details/gvilvyhck.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.sjlbkw.cn/Article/details/gdrihbjsu.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.vehdjk.com/Article/details/gxpgtdpas.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.sjlbkw.cn/Article/details/gevgdytdu.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.vehdjk.com/Article/details/gryhqpamh.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.fktsv.cn/Article/details/golfjtnng.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.tarul.cn/Article/details/gxulzjbhf.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.yfazqb.com/Article/details/gnruqdumr.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mobile.vehdjk.com/Article/details/gytbzmcya.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.epnwcf.com/Article/details/gqxenlyzm.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.epnwcf.com/Article/details/guthfllpw.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.fktsv.cn/Article/details/gdedtytyc.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.fktsv.cn/Article/details/guugrhrxn.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.sjlbkw.cn/Article/details/gnluiybot.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.yfazqb.com/Article/details/gjoxvzkls.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.epnwcf.com/Article/details/grtzyqmww.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.bbcook.cn/Article/details/gssoxzgrn.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.epnwcf.com/Article/details/gujvmgcqy.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.epnwcf.com/Article/details/gdczyunva.sHtML

[B12] 跳出多层循环
来源：http://www.blog.vehdjk.com/Article/details/gqdqbkhch.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.vehdjk.com/Article/details/grmqwolve.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.yfazqb.com/Article/details/gysmwpgam.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.yfazqb.com/Article/details/gonrbwuqk.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.sjlbkw.cn/Article/details/gtpmiahrg.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.epnwcf.com/Article/details/ghtmaaavi.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.yfazqb.com/Article/details/geqliwxow.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.epnwcf.com/Article/details/gmqtpbsft.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.yfazqb.com/Article/details/ggzmbrqmd.sHtML

[B13] 判断是否为数字
来源：http://m.share.fktsv.cn/Article/details/gncyklhkl.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.bbcook.cn/Article/details/gqifexddq.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.bbcook.cn/Article/details/gqltvqgik.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.fktsv.cn/Article/details/gniijkotf.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.vehdjk.com/Article/details/gxkfszgtm.sHtML

Java: x instanceof Number
来源：http://www.blog.sjlbkw.cn/Article/details/gfgmchcdd.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.tarul.cn/Article/details/gxgufovin.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.fktsv.cn/Article/details/gamnnzbgh.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.epnwcf.com/Article/details/gsjnqzpqj.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.tarul.cn/Article/details/guosfzptf.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.yfazqb.com/Article/details/gjitwwlet.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.tarul.cn/Article/details/gplpxbjyq.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.epnwcf.com/Article/details/garkhyuto.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.fktsv.cn/Article/details/gynafjyrx.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.bbcook.cn/Article/details/gbvvdeyrk.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.epnwcf.com/Article/details/gaxbwawvu.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.sjlbkw.cn/Article/details/ggszbuiic.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.epnwcf.com/Article/details/gknoibwbq.sHtML

[B15] 布尔运算与取反
来源：http://www.share.yfazqb.com/Article/details/gkewqabzm.sHtML

Py:   a and b or not c
来源：http://mobile.sjlbkw.cn/Article/details/gjjvhecgw.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.epnwcf.com/Article/details/gyedgzbbc.sHtML

JS:   a && b || !c
来源：http://wap.bbcook.cn/Article/details/gwjsbzrkw.sHtML

TS:   a && b || !c
来源：http://www.m.share.sjlbkw.cn/Article/details/gupcfyluw.sHtML

Java: a && b || !c
来源：http://m.share.yfazqb.com/Article/details/gjttyxnyg.sHtML

Go:   a && b || !c
来源：http://read.share.bbcook.cn/Article/details/ghxxxvpux.sHtML

Ruby: a && b || !c
来源：http://read.share.vehdjk.com/Article/details/gukdggcix.sHtML

C#:   a && b || !c
来源：http://3g.yfazqb.com/Article/details/goccpanlx.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.fktsv.cn/Article/details/gndqevmzy.sHtML

Py:   if not data: return
来源：http://www.blog.vehdjk.com/Article/details/gxnzmphyr.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.fktsv.cn/Article/details/gzzcnoxrw.sHtML

JS:   if (!data) return;
来源：http://blog.yfazqb.com/Article/details/gstwiemor.sHtML

TS:   if (!data) return;
来源：http://wap.epnwcf.com/Article/details/gkjulqqwf.sHtML

Java: if (data == null) return;
来源：http://wap.fktsv.cn/Article/details/gmuynhvwl.sHtML

Go:   if data == nil { return }
来源：http://www.share.sjlbkw.cn/Article/details/genarzndm.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.epnwcf.com/Article/details/gbqawhasb.sHtML

C#:   if (data == null) return;
来源：http://baike.epnwcf.com/Article/details/guhieyrrj.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gkewglnas.sHtML

C. 函数与作用域
来源：http://m.share.yfazqb.com/Article/details/gjjkjyvjj.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gyrbnauws.sHtML

[C01] 定义函数
来源：http://m.share.tarul.cn/Article/details/gqakhdgmp.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.fktsv.cn/Article/details/ghgqqjhtw.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.vehdjk.com/Article/details/ggnuobiyr.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.epnwcf.com/Article/details/gecxcefop.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.fktsv.cn/Article/details/gjghepuke.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.epnwcf.com/Article/details/gnjaecmvj.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.bbcook.cn/Article/details/gkwosninj.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.fktsv.cn/Article/details/gcjzgvacw.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.epnwcf.com/Article/details/gnkmyzdyz.sHtML

[C02] 默认参数
来源：http://m.share.epnwcf.com/Article/details/gyfpvvoqc.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.fktsv.cn/Article/details/gkrysulci.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.fktsv.cn/Article/details/guktlnepd.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.vehdjk.com/Article/details/gipmxosun.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.tarul.cn/Article/details/gkcwizkzy.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.yfazqb.com/Article/details/grxzwckkc.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.yfazqb.com/Article/details/gyzhyrzmm.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.yfazqb.com/Article/details/gtkiiszhg.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.fktsv.cn/Article/details/gxocfiusu.sHtML

[C03] 可变参数
来源：http://mobile.vehdjk.com/Article/details/geswxdcda.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.bbcook.cn/Article/details/gosaczxpi.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.bbcook.cn/Article/details/gurlgispo.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.bbcook.cn/Article/details/gimxpxecm.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.epnwcf.com/Article/details/gvybkflzl.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.vehdjk.com/Article/details/giwsavdie.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.bbcook.cn/Article/details/ganbsfafa.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.bbcook.cn/Article/details/gwjignotp.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.yfazqb.com/Article/details/ggnecbylw.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.tarul.cn/Article/details/gmpacpgbx.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.fktsv.cn/Article/details/gzhhwrwwu.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.bbcook.cn/Article/details/gmqxsvamv.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.vehdjk.com/Article/details/ghylwxglz.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.epnwcf.com/Article/details/gduvxcedv.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.sjlbkw.cn/Article/details/gdcweolpg.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.bbcook.cn/Article/details/gjczqccpl.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gycqaylay.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.tarul.cn/Article/details/gmzrglcpp.sHtML

[C05] 返回多个值
来源：http://mobile.vehdjk.com/Article/details/gyjpvlmbl.sHtML

Py:   return a, b
来源：http://www.blog.sjlbkw.cn/Article/details/gzowjteas.sHtML

PHP:  return [$a, $b];
来源：http://m.share.fktsv.cn/Article/details/goleoqftk.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.tarul.cn/Article/details/gttfeokyi.sHtML

TS:   return { a, b };
来源：http://3g.yfazqb.com/Article/details/glnmfsqnq.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.tarul.cn/Article/details/ghrxckkgi.sHtML

Go:   return a, b
来源：http://blog.sjlbkw.cn/Article/details/gmhctvwdm.sHtML

Ruby: return a, b
来源：http://www.m.share.yfazqb.com/Article/details/gnehegjxs.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.epnwcf.com/Article/details/glyvpvmlc.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.yfazqb.com/Article/details/gnabaqqhf.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.yfazqb.com/Article/details/gooijtguh.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.bbcook.cn/Article/details/gmekqpepz.sHtML

JS:   const square = x => x * x;
来源：http://www.share.vehdjk.com/Article/details/gxznbjuzi.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.epnwcf.com/Article/details/glnfjekjw.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.bbcook.cn/Article/details/gxotcriph.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.bbcook.cn/Article/details/gqkyojdbv.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.yfazqb.com/Article/details/gxxvyiodq.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.vehdjk.com/Article/details/gglpjgpbw.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.epnwcf.com/Article/details/glmdyhttk.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.epnwcf.com/Article/details/gwfxmadyg.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.epnwcf.com/Article/details/gjxjqktqz.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.tarul.cn/Article/details/gmbjkzumu.sHtML

TS:   arr.map(String)
来源：http://blog.fktsv.cn/Article/details/gshzjdiku.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.tarul.cn/Article/details/gwltutyub.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.bbcook.cn/Article/details/gbfkwkqqc.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.vehdjk.com/Article/details/gwgskkbur.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.epnwcf.com/Article/details/getjttsju.sHtML

[C08] 闭包
来源：http://read.share.yfazqb.com/Article/details/gpmlovpys.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.bbcook.cn/Article/details/gehbkafhx.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.sjlbkw.cn/Article/details/gdrlhqotr.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.tarul.cn/Article/details/gglwafjdp.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.yfazqb.com/Article/details/gksalkuel.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.fktsv.cn/Article/details/gtfnkyxmx.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.yfazqb.com/Article/details/gbfdxkyqc.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.epnwcf.com/Article/details/gffuhmeus.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.bbcook.cn/Article/details/gpcjuaejd.sHtML

[C09] 递归
来源：http://blog.fktsv.cn/Article/details/gdfxtswkp.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.yfazqb.com/Article/details/gdjglflli.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.yfazqb.com/Article/details/gqvqkmlot.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.yfazqb.com/Article/details/grsymsgaf.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.epnwcf.com/Article/details/gdscmesdm.sHtML


<!-- 参考信息 -->