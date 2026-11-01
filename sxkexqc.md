代发 wailian999

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.yfazqb.com/Article/details/gldbepxez.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.m.share.fktsv.cn/Article/details/goepqktfo.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.bbcook.cn/Article/details/glllailwz.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.yfazqb.com/Article/details/gcnmfejur.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.share.yfazqb.com/Article/details/gluwfjepw.sHtML

Py:   ord("A"); chr(65)
来源：http://3g.bbcook.cn/Article/details/gtjkdaevq.sHtML

PHP:  ord("A"); chr(65)
来源：http://mobile.yfazqb.com/Article/details/grzhxoqdf.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.yfazqb.com/Article/details/gnkichhht.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.sjlbkw.cn/Article/details/gkwrfhgjn.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.m.share.bbcook.cn/Article/details/gljkwqmjx.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://blog.tarul.cn/Article/details/gqgjeqwto.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.share.yfazqb.com/Article/details/gbptlpkfz.sHtML

C#:   (int)'A'; (char)65
来源：http://baike.yfazqb.com/Article/details/gwqvnhvcq.sHtML

[A19] 交换两个变量
来源：http://baike.vehdjk.com/Article/details/gyinlrrdo.sHtML

Py:   a, b = b, a
来源：http://blog.fktsv.cn/Article/details/gknltxluw.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://3g.vehdjk.com/Article/details/gdzfemxpm.sHtML

JS:   [a, b] = [b, a];
来源：http://www.blog.epnwcf.com/Article/details/gwzlckdmu.sHtML

TS:   [a, b] = [b, a];
来源：http://blog.vehdjk.com/Article/details/gyybmfiqq.sHtML

Java: int t = a; a = b; b = t;
来源：http://wap.vehdjk.com/Article/details/grglthxsl.sHtML

Go:   a, b = b, a
来源：http://www.blog.sjlbkw.cn/Article/details/gtamwijbs.sHtML

Ruby: a, b = b, a
来源：http://read.share.tarul.cn/Article/details/glersazkb.sHtML

C#:   (a, b) = (b, a);
来源：http://3g.sjlbkw.cn/Article/details/ggwdlopyn.sHtML

[A20] 读取标准输入
来源：http://m.share.vehdjk.com/Article/details/glbzehmsl.sHtML

Py:   name = input("请输入：")
来源：http://baike.yfazqb.com/Article/details/gqrfhwjgh.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://3g.fktsv.cn/Article/details/gajscaudj.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://read.share.epnwcf.com/Article/details/gggtfxiyd.sHtML

TS:   // Node.js：readline 模块
来源：http://baike.yfazqb.com/Article/details/gvkpqmkwt.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.share.sjlbkw.cn/Article/details/geotsyppl.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://baike.bbcook.cn/Article/details/gbztlcqpr.sHtML

Ruby: gets.chomp
来源：http://www.share.tarul.cn/Article/details/gtxgllnnu.sHtML

C#:   Console.ReadLine();
来源：http://read.share.fktsv.cn/Article/details/gsrlmtjfh.sHtML

[A21] 保留指定小数位输出
来源：http://baike.bbcook.cn/Article/details/gbuldiczc.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.m.share.vehdjk.com/Article/details/gcbqbsoqp.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://mobile.yfazqb.com/Article/details/gzuqqqyqb.sHtML

JS:   (3.14159).toFixed(2)
来源：http://mobile.sjlbkw.cn/Article/details/ggvpdgqqz.sHtML

TS:   (3.14159).toFixed(2)
来源：http://mobile.sjlbkw.cn/Article/details/gzgxpaogu.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.m.share.bbcook.cn/Article/details/gmuzxwdwz.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.blog.fktsv.cn/Article/details/ghfpfzkaf.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.m.share.tarul.cn/Article/details/gkyccsqmf.sHtML

C#:   3.14159.ToString("F2")
来源：http://wap.sjlbkw.cn/Article/details/goirjalvk.sHtML

[A22] 获取字符串长度
来源：http://wap.fktsv.cn/Article/details/gpfaxzffd.sHtML

Py:   len(s)
来源：http://www.blog.epnwcf.com/Article/details/guxzadfju.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.share.sjlbkw.cn/Article/details/gnxszlrun.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.m.share.bbcook.cn/Article/details/gaswebqdp.sHtML

TS:   s.length
来源：http://www.blog.bbcook.cn/Article/details/guhshzgsy.sHtML

Java: s.length()
来源：http://www.share.fktsv.cn/Article/details/gxfjprtuq.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://blog.fktsv.cn/Article/details/ggkkzjpvh.sHtML

Ruby: s.length
来源：http://baike.yfazqb.com/Article/details/gmigwocke.sHtML

C#:   s.Length
来源：http://wap.fktsv.cn/Article/details/gzxxmptrt.sHtML

[A23] 大小写转换
来源：http://blog.yfazqb.com/Article/details/gbfggpzee.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.m.share.tarul.cn/Article/details/gqvuwgasj.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.share.tarul.cn/Article/details/gvqbsfmzv.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.fktsv.cn/Article/details/gmqwrmanb.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.fktsv.cn/Article/details/gthodisho.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wap.vehdjk.com/Article/details/gudodlcfe.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.blog.fktsv.cn/Article/details/ghbourvls.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wap.tarul.cn/Article/details/gpckunldr.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://mobile.tarul.cn/Article/details/gzsfdwbpn.sHtML

[A24] 去除首尾空白
来源：http://3g.vehdjk.com/Article/details/gwckfbvoi.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://m.share.epnwcf.com/Article/details/gaznyqiml.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://read.share.vehdjk.com/Article/details/gbhlxdskn.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.fktsv.cn/Article/details/gdkmjznbz.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.sjlbkw.cn/Article/details/gidzromjq.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wap.vehdjk.com/Article/details/gkzifbttd.sHtML

Go:   strings.TrimSpace(s)
来源：http://mobile.sjlbkw.cn/Article/details/gdhdozdut.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://m.share.sjlbkw.cn/Article/details/gorirxcxw.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.m.share.vehdjk.com/Article/details/glyxfecmg.sHtML

[A25] 字符串比较
来源：http://mobile.epnwcf.com/Article/details/gozrizevg.sHtML

Py:   s1 == s2; s1 != s2
来源：http://3g.fktsv.cn/Article/details/gspkoqfbb.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://blog.tarul.cn/Article/details/gwwffnzac.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.epnwcf.com/Article/details/gzrpowmkv.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.fktsv.cn/Article/details/ghkkmusbv.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wap.bbcook.cn/Article/details/gucyyjbyn.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.m.share.bbcook.cn/Article/details/ghqdtpsif.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://m.share.vehdjk.com/Article/details/gbonrxubx.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wap.fktsv.cn/Article/details/gprzwczcx.sHtML

[A26] 类型转换总览
来源：http://read.share.yfazqb.com/Article/details/gbreqmqrv.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.m.share.tarul.cn/Article/details/gsfzovsxm.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://m.share.sjlbkw.cn/Article/details/gfaxknikf.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://blog.tarul.cn/Article/details/gewsamluj.sHtML

TS:   Number() String() Boolean() x as number
来源：http://baike.vehdjk.com/Article/details/gkvcvqyoc.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.blog.sjlbkw.cn/Article/details/gocpzrokl.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://baike.bbcook.cn/Article/details/gtemkclhx.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.blog.yfazqb.com/Article/details/gtmgyrkpj.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mobile.bbcook.cn/Article/details/grblsamqq.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gmbsluzfl.sHtML

B. 流程控制
来源：http://mobile.yfazqb.com/Article/details/ghorkiina.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/grwjkaqir.sHtML

[B01] 条件判断 if / else
来源：http://3g.epnwcf.com/Article/details/gjhzegakz.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://blog.fktsv.cn/Article/details/gfowyvddm.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://m.share.bbcook.cn/Article/details/gzzzkhgmw.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.epnwcf.com/Article/details/gycbefmnj.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.bbcook.cn/Article/details/gwfcbvtzq.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.share.epnwcf.com/Article/details/gcclbnjzq.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://m.share.epnwcf.com/Article/details/gefbvtvzb.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://m.share.fktsv.cn/Article/details/gdqytilgr.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://3g.fktsv.cn/Article/details/gukyabept.sHtML

[B02] 多分支 else if / elif
来源：http://www.blog.yfazqb.com/Article/details/gmghfcnwa.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wap.yfazqb.com/Article/details/gqjruhgzs.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.m.share.fktsv.cn/Article/details/glcfewqfz.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.sjlbkw.cn/Article/details/gnqalhdxs.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.fktsv.cn/Article/details/gtnfjbqft.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.epnwcf.com/Article/details/gwykpylgf.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://baike.tarul.cn/Article/details/gkcvzbfsl.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://3g.sjlbkw.cn/Article/details/gdhbuvqff.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.tarul.cn/Article/details/gapndvgne.sHtML

[B03] switch / match / case
来源：http://read.share.yfazqb.com/Article/details/guynwmmrk.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://baike.vehdjk.com/Article/details/gdudoehtz.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.share.sjlbkw.cn/Article/details/gjkmxxpdm.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.yfazqb.com/Article/details/gfyxnilvx.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.vehdjk.com/Article/details/gddschnpb.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://read.share.bbcook.cn/Article/details/gztzhmhga.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.m.share.tarul.cn/Article/details/gnppwvynt.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://m.share.fktsv.cn/Article/details/gydnfkgmm.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.share.bbcook.cn/Article/details/gfkwruqrb.sHtML

[B04] for 计数循环
来源：http://mobile.sjlbkw.cn/Article/details/gtrjvfgcg.sHtML

Py:   for i in range(10): print(i)
来源：http://wap.fktsv.cn/Article/details/gxwldsiwr.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mobile.epnwcf.com/Article/details/gjpngirqr.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.bbcook.cn/Article/details/glywwvybe.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.fktsv.cn/Article/details/gsvhxlrkw.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.m.share.yfazqb.com/Article/details/gbjacytpy.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.blog.vehdjk.com/Article/details/gfgqlfesw.sHtML

Ruby: 10.times { |i| puts i }
来源：http://wap.yfazqb.com/Article/details/gcgjdokrb.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mobile.fktsv.cn/Article/details/gtkqbiztw.sHtML

[B05] 遍历数组 / 列表
来源：http://www.share.sjlbkw.cn/Article/details/gyyzbkuxx.sHtML

Py:   for item in arr: print(item)
来源：http://3g.vehdjk.com/Article/details/gmsymuhwz.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://3g.sjlbkw.cn/Article/details/gihktaabn.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.yfazqb.com/Article/details/gwbflyaei.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://mobile.vehdjk.com/Article/details/ghtqlqoys.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.yfazqb.com/Article/details/guppeaoip.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://blog.bbcook.cn/Article/details/gotegriwq.sHtML

Ruby: arr.each { |item| puts item }
来源：http://m.share.sjlbkw.cn/Article/details/gzipwreyn.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.share.vehdjk.com/Article/details/ggcpwmuiu.sHtML

[B06] 遍历字典 / 对象
来源：http://www.m.share.epnwcf.com/Article/details/gsjnuvgfp.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.bbcook.cn/Article/details/ghbihvipp.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.tarul.cn/Article/details/glnhcaokg.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.sjlbkw.cn/Article/details/gklyopvfg.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.bbcook.cn/Article/details/guisazfxt.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.sjlbkw.cn/Article/details/gnobedywh.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.bbcook.cn/Article/details/gqrmsqsyp.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.vehdjk.com/Article/details/gvipnpoke.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.share.bbcook.cn/Article/details/gyykzxmls.sHtML

[B07] while 循环
来源：http://mobile.tarul.cn/Article/details/ghzgktxja.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.epnwcf.com/Article/details/gdzdoepqj.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.tarul.cn/Article/details/gxdyllknw.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.epnwcf.com/Article/details/gjnrkgcta.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.share.vehdjk.com/Article/details/gaapfsjbu.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.bbcook.cn/Article/details/gbmadzagb.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://m.share.fktsv.cn/Article/details/gwaquvmce.sHtML

Ruby: while i < 10; i += 1; end
来源：http://read.share.bbcook.cn/Article/details/guxckqcgp.sHtML

C#:   while (i < 10) { i++; }
来源：http://blog.yfazqb.com/Article/details/givlfkvgv.sHtML

[B08] do-while（至少执行一次）
来源：http://www.share.sjlbkw.cn/Article/details/gizxmpgks.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://read.share.yfazqb.com/Article/details/gcbjkreai.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.yfazqb.com/Article/details/gxcwpyxrk.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.bbcook.cn/Article/details/gzbikmwsy.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.bbcook.cn/Article/details/galbzwoih.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.tarul.cn/Article/details/gwtgjxmjb.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.fktsv.cn/Article/details/gkdgscaov.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.share.vehdjk.com/Article/details/gpeuffipi.sHtML

C#:   do { i++; } while (i < 10);
来源：http://mobile.sjlbkw.cn/Article/details/gxojvpapq.sHtML

[B09] break 与 continue
来源：http://wap.bbcook.cn/Article/details/gqcknlrvr.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.yfazqb.com/Article/details/giupwssbm.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.bbcook.cn/Article/details/ggeyfxrxk.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fktsv.cn/Article/details/gczawdzkm.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.tarul.cn/Article/details/grmvvjdqz.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.tarul.cn/Article/details/ghxjheotw.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.vehdjk.com/Article/details/gtuqeyegj.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.fktsv.cn/Article/details/gfuzjcvig.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.sjlbkw.cn/Article/details/ginuujdrj.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.epnwcf.com/Article/details/ghtwyhdbk.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.yfazqb.com/Article/details/gyqspkfev.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.yfazqb.com/Article/details/ghdcugfec.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.vehdjk.com/Article/details/gbditltwg.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.epnwcf.com/Article/details/gwlquhdmd.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.vehdjk.com/Article/details/gbhunhfog.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.fktsv.cn/Article/details/ggqkoonzb.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.sjlbkw.cn/Article/details/gnnifoqxb.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.bbcook.cn/Article/details/gwukzhpbh.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.tarul.cn/Article/details/gxjprabfp.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.vehdjk.com/Article/details/gftsqyvml.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.epnwcf.com/Article/details/gbulgygjk.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.bbcook.cn/Article/details/glyzywpet.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.bbcook.cn/Article/details/gfdqytpkr.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.epnwcf.com/Article/details/gdxbontlu.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.epnwcf.com/Article/details/gmytwhafe.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.fktsv.cn/Article/details/gejpiipkn.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.sjlbkw.cn/Article/details/glkwfoqmg.sHtML

[B12] 跳出多层循环
来源：http://baike.epnwcf.com/Article/details/gramwtmiw.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.vehdjk.com/Article/details/gtqdrgxmx.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.tarul.cn/Article/details/gmiblulxl.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.yfazqb.com/Article/details/gbioxepye.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.bbcook.cn/Article/details/gthsgfcbs.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.tarul.cn/Article/details/gynsgsqyz.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.vehdjk.com/Article/details/glavxvlfu.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.vehdjk.com/Article/details/guchjffbo.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.tarul.cn/Article/details/gakbwlsfu.sHtML

[B13] 判断是否为数字
来源：http://www.blog.tarul.cn/Article/details/gkckeevbb.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.tarul.cn/Article/details/gzrpfjtqr.sHtML

PHP:  is_numeric($x)
来源：http://blog.vehdjk.com/Article/details/gaqvfqrzh.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.fktsv.cn/Article/details/gxwpewnkt.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.yfazqb.com/Article/details/gvzpdreou.sHtML

Java: x instanceof Number
来源：http://3g.vehdjk.com/Article/details/gvfeicfcv.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.bbcook.cn/Article/details/gdgzlkaxq.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.bbcook.cn/Article/details/gkskzgmmv.sHtML

C#:   x is int or double or decimal
来源：http://blog.sjlbkw.cn/Article/details/gpngmtsnp.sHtML

[B14] 判断值是否在集合内
来源：http://blog.tarul.cn/Article/details/gnkjknnvy.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.sjlbkw.cn/Article/details/giuzdkqre.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.tarul.cn/Article/details/gvgqzhibj.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.vehdjk.com/Article/details/gsmjemjdu.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.bbcook.cn/Article/details/glrumswel.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.epnwcf.com/Article/details/gxagioczc.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.yfazqb.com/Article/details/gmerfieqz.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.yfazqb.com/Article/details/gneorsqye.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.yfazqb.com/Article/details/gmpiwgpai.sHtML

[B15] 布尔运算与取反
来源：http://baike.yfazqb.com/Article/details/godgsxbaa.sHtML

Py:   a and b or not c
来源：http://blog.sjlbkw.cn/Article/details/geyfeodvk.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.tarul.cn/Article/details/gvwgpuqqf.sHtML

JS:   a && b || !c
来源：http://mobile.epnwcf.com/Article/details/gnsdgdaik.sHtML

TS:   a && b || !c
来源：http://blog.vehdjk.com/Article/details/gqgdbxtxy.sHtML

Java: a && b || !c
来源：http://3g.bbcook.cn/Article/details/gawlofctp.sHtML

Go:   a && b || !c
来源：http://www.blog.yfazqb.com/Article/details/gtnzeavvq.sHtML

Ruby: a && b || !c
来源：http://mobile.fktsv.cn/Article/details/gxkrsyutr.sHtML

C#:   a && b || !c
来源：http://wap.fktsv.cn/Article/details/giludqafn.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.epnwcf.com/Article/details/gksmqjbay.sHtML

Py:   if not data: return
来源：http://blog.tarul.cn/Article/details/ggaylkffi.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.vehdjk.com/Article/details/gfenohtfi.sHtML

JS:   if (!data) return;
来源：http://blog.vehdjk.com/Article/details/gqibpqoml.sHtML

TS:   if (!data) return;
来源：http://mobile.sjlbkw.cn/Article/details/gzpivvajm.sHtML

Java: if (data == null) return;
来源：http://read.share.sjlbkw.cn/Article/details/gwtpdpmrq.sHtML

Go:   if data == nil { return }
来源：http://mobile.vehdjk.com/Article/details/gyyywtjxe.sHtML

Ruby: return if data.nil?
来源：http://m.share.epnwcf.com/Article/details/gioddrgtd.sHtML

C#:   if (data == null) return;
来源：http://www.share.sjlbkw.cn/Article/details/gliqhphyy.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gcunynppy.sHtML

C. 函数与作用域
来源：http://3g.vehdjk.com/Article/details/ghpmuiugb.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gaktikdgw.sHtML

[C01] 定义函数
来源：http://www.blog.epnwcf.com/Article/details/gwtirxfll.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.vehdjk.com/Article/details/gbsksxmyr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.tarul.cn/Article/details/gontjltfc.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.yfazqb.com/Article/details/gmboezygn.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.vehdjk.com/Article/details/gfonmhezr.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.fktsv.cn/Article/details/gjtjmcsmx.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.bbcook.cn/Article/details/gjwkpgkba.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.fktsv.cn/Article/details/giwkrfnti.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.sjlbkw.cn/Article/details/gbugcajgn.sHtML

[C02] 默认参数
来源：http://www.blog.bbcook.cn/Article/details/ggwuycfwm.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.tarul.cn/Article/details/gprhafktu.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.yfazqb.com/Article/details/gbranmzrz.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.bbcook.cn/Article/details/gplwrfkwr.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.tarul.cn/Article/details/gbkfmaaik.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.tarul.cn/Article/details/gscleqvhz.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.vehdjk.com/Article/details/gypargwdm.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.yfazqb.com/Article/details/gsdmoxlgb.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.sjlbkw.cn/Article/details/gdwofgqll.sHtML

[C03] 可变参数
来源：http://www.m.share.tarul.cn/Article/details/gpjntquqp.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.epnwcf.com/Article/details/gqcfnvbaa.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.yfazqb.com/Article/details/gdxcnaybj.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.bbcook.cn/Article/details/gjntrtyjd.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.vehdjk.com/Article/details/gfmnyyyex.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.tarul.cn/Article/details/gaozutuvb.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.sjlbkw.cn/Article/details/gwyvrpwuh.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.vehdjk.com/Article/details/gbffsbuep.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.fktsv.cn/Article/details/gncbbuiao.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.tarul.cn/Article/details/gqzrwparl.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.tarul.cn/Article/details/gzkwvwhlk.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.fktsv.cn/Article/details/gkuefyxsf.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.epnwcf.com/Article/details/gwxmsicqa.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.yfazqb.com/Article/details/guabfkfcr.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.tarul.cn/Article/details/gluwhwapt.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.epnwcf.com/Article/details/gjjdzxbcr.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.sjlbkw.cn/Article/details/gbppotajs.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.sjlbkw.cn/Article/details/grdmudcss.sHtML

[C05] 返回多个值
来源：http://m.share.bbcook.cn/Article/details/gnhwkptzt.sHtML

Py:   return a, b
来源：http://m.share.fktsv.cn/Article/details/gfdlzlcfl.sHtML

PHP:  return [$a, $b];
来源：http://read.share.sjlbkw.cn/Article/details/gglxqfucs.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.fktsv.cn/Article/details/gmickgdpl.sHtML

TS:   return { a, b };
来源：http://www.m.share.yfazqb.com/Article/details/gwgomvpck.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.yfazqb.com/Article/details/gzdhlkjyx.sHtML

Go:   return a, b
来源：http://3g.vehdjk.com/Article/details/gcirtdufr.sHtML

Ruby: return a, b
来源：http://wap.sjlbkw.cn/Article/details/gudfoyrlg.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.tarul.cn/Article/details/gvudgkepi.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.bbcook.cn/Article/details/gwmmeirob.sHtML

Py:   square = lambda x: x * x
来源：http://3g.vehdjk.com/Article/details/glsvuqbbx.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.tarul.cn/Article/details/goelnsqfd.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.fktsv.cn/Article/details/gwufnxsul.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.vehdjk.com/Article/details/gditxzqyw.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.tarul.cn/Article/details/grmleuuog.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.fktsv.cn/Article/details/gjhqmvchn.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.epnwcf.com/Article/details/gsmgtdgft.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.tarul.cn/Article/details/gyarkfykp.sHtML

[C07] 把函数作为参数传入
来源：http://3g.yfazqb.com/Article/details/gvsisppkb.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.sjlbkw.cn/Article/details/gectlffsd.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.epnwcf.com/Article/details/gqjfyrvod.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.yfazqb.com/Article/details/grugdkcmo.sHtML

TS:   arr.map(String)
来源：http://www.share.yfazqb.com/Article/details/gcrmvmoug.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.fktsv.cn/Article/details/gsrgtdhev.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.yfazqb.com/Article/details/gupfpwcas.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.vehdjk.com/Article/details/gpoeujrjj.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.yfazqb.com/Article/details/gljmlzoss.sHtML

[C08] 闭包
来源：http://m.share.tarul.cn/Article/details/gxawhabvr.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.sjlbkw.cn/Article/details/gemyveszb.sHtML


<!-- 参考信息 -->