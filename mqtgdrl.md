代发 wailian999

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.yfazqb.com/Article/details/gxayrsyjv.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.blog.fktsv.cn/Article/details/gtyatzhjx.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://read.share.yfazqb.com/Article/details/ghwcslrhx.sHtML

Ruby: "A".ord; 65.chr
来源：http://3g.vehdjk.com/Article/details/gstbzbvoy.sHtML

C#:   (int)'A'; (char)65
来源：http://blog.epnwcf.com/Article/details/gsrsnzddh.sHtML

[A19] 交换两个变量
来源：http://blog.fktsv.cn/Article/details/gkqgrmuuy.sHtML

Py:   a, b = b, a
来源：http://www.share.tarul.cn/Article/details/gyppjeqzc.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://read.share.epnwcf.com/Article/details/gqpvrrztt.sHtML

JS:   [a, b] = [b, a];
来源：http://blog.vehdjk.com/Article/details/gsvraecgk.sHtML

TS:   [a, b] = [b, a];
来源：http://mobile.epnwcf.com/Article/details/gkligegyv.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.share.vehdjk.com/Article/details/goqprmwcv.sHtML

Go:   a, b = b, a
来源：http://www.blog.sjlbkw.cn/Article/details/gsapnfnhf.sHtML

Ruby: a, b = b, a
来源：http://baike.yfazqb.com/Article/details/gxkfsqblf.sHtML

C#:   (a, b) = (b, a);
来源：http://3g.yfazqb.com/Article/details/gksqpuqxk.sHtML

[A20] 读取标准输入
来源：http://wap.yfazqb.com/Article/details/gtpoydsnj.sHtML

Py:   name = input("请输入：")
来源：http://www.blog.yfazqb.com/Article/details/gplvcrscv.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://3g.yfazqb.com/Article/details/giozrbofz.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.blog.tarul.cn/Article/details/greiaumue.sHtML

TS:   // Node.js：readline 模块
来源：http://mobile.yfazqb.com/Article/details/gunrumsvu.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.share.bbcook.cn/Article/details/gvmkkfxam.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://blog.tarul.cn/Article/details/gfnciqxwm.sHtML

Ruby: gets.chomp
来源：http://m.share.yfazqb.com/Article/details/ghhsttynj.sHtML

C#:   Console.ReadLine();
来源：http://mobile.epnwcf.com/Article/details/gihtugsgo.sHtML

[A21] 保留指定小数位输出
来源：http://www.share.tarul.cn/Article/details/geffiofyt.sHtML

Py:   f"{3.14159:.2f}"
来源：http://read.share.bbcook.cn/Article/details/ggtkntwjq.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://blog.epnwcf.com/Article/details/gfishsxiv.sHtML

JS:   (3.14159).toFixed(2)
来源：http://3g.tarul.cn/Article/details/gxtbeaeob.sHtML

TS:   (3.14159).toFixed(2)
来源：http://m.share.sjlbkw.cn/Article/details/gkruwenme.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.share.sjlbkw.cn/Article/details/grtnnhxex.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://read.share.vehdjk.com/Article/details/gcioamari.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://wap.tarul.cn/Article/details/gqmfvxgzs.sHtML

C#:   3.14159.ToString("F2")
来源：http://mobile.bbcook.cn/Article/details/gckrxdvbg.sHtML

[A22] 获取字符串长度
来源：http://blog.fktsv.cn/Article/details/gprimiswh.sHtML

Py:   len(s)
来源：http://m.share.vehdjk.com/Article/details/geqgcwwgp.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://blog.yfazqb.com/Article/details/gfavixqem.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.m.share.fktsv.cn/Article/details/gkhjhexnw.sHtML

TS:   s.length
来源：http://read.share.vehdjk.com/Article/details/gwmaxrkrs.sHtML

Java: s.length()
来源：http://www.m.share.fktsv.cn/Article/details/grxnbnbyw.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://read.share.vehdjk.com/Article/details/guvuepxco.sHtML

Ruby: s.length
来源：http://wap.fktsv.cn/Article/details/gaxbhbetd.sHtML

C#:   s.Length
来源：http://m.share.vehdjk.com/Article/details/ghrwjorje.sHtML

[A23] 大小写转换
来源：http://www.m.share.tarul.cn/Article/details/gzyynxiqs.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://read.share.bbcook.cn/Article/details/giyiuzgvs.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://read.share.epnwcf.com/Article/details/ganinnmfn.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.sjlbkw.cn/Article/details/ghzfztglv.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.tarul.cn/Article/details/gmuzlumtl.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://blog.fktsv.cn/Article/details/gpwbuhmfs.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://m.share.bbcook.cn/Article/details/gjmslcatv.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://blog.sjlbkw.cn/Article/details/gftulneel.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://3g.vehdjk.com/Article/details/ghnrdxxyn.sHtML

[A24] 去除首尾空白
来源：http://mobile.vehdjk.com/Article/details/grlqdvjga.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://m.share.sjlbkw.cn/Article/details/gitfnuvcj.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wap.fktsv.cn/Article/details/gpgqgcspd.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.sjlbkw.cn/Article/details/grzvbddyl.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.vehdjk.com/Article/details/gqcxmxfbb.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wap.tarul.cn/Article/details/gujfkygno.sHtML

Go:   strings.TrimSpace(s)
来源：http://m.share.epnwcf.com/Article/details/glbybsibn.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://m.share.vehdjk.com/Article/details/gilcycpxi.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.share.epnwcf.com/Article/details/grsmhaxfy.sHtML

[A25] 字符串比较
来源：http://3g.vehdjk.com/Article/details/gyxhndjac.sHtML

Py:   s1 == s2; s1 != s2
来源：http://m.share.yfazqb.com/Article/details/grfaqigla.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://blog.yfazqb.com/Article/details/gqchzyfyx.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.tarul.cn/Article/details/gouumegyn.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.bbcook.cn/Article/details/gjoqzallr.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.share.sjlbkw.cn/Article/details/gqlpfzbko.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://blog.yfazqb.com/Article/details/gkbvanmna.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://3g.tarul.cn/Article/details/gqzugwbpx.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://blog.sjlbkw.cn/Article/details/ghregltpk.sHtML

[A26] 类型转换总览
来源：http://www.m.share.tarul.cn/Article/details/guxnuifnh.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://blog.sjlbkw.cn/Article/details/gecpoahoh.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://3g.sjlbkw.cn/Article/details/gdcqbfnha.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://baike.sjlbkw.cn/Article/details/gzxaopvud.sHtML

TS:   Number() String() Boolean() x as number
来源：http://wap.fktsv.cn/Article/details/gredcfkfb.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://blog.bbcook.cn/Article/details/gxqkkcxip.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://blog.sjlbkw.cn/Article/details/gwmkzpcdu.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.share.epnwcf.com/Article/details/gimlslhsa.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mobile.epnwcf.com/Article/details/gopmjyctw.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/grlkkzbxi.sHtML

B. 流程控制
来源：http://baike.tarul.cn/Article/details/gefozjehw.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gdqpzrozh.sHtML

[B01] 条件判断 if / else
来源：http://www.share.bbcook.cn/Article/details/gurzyybpi.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://mobile.yfazqb.com/Article/details/gcxspbvom.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wap.bbcook.cn/Article/details/ggwdkqqim.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.yfazqb.com/Article/details/glbnddumn.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.vehdjk.com/Article/details/gvixeqmnm.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://mobile.epnwcf.com/Article/details/gtsfyxdjf.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://blog.epnwcf.com/Article/details/gnmxkfzkw.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://3g.vehdjk.com/Article/details/gywicjnsn.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wap.bbcook.cn/Article/details/gdkoqhido.sHtML

[B02] 多分支 else if / elif
来源：http://3g.sjlbkw.cn/Article/details/gluypfrxg.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mobile.vehdjk.com/Article/details/gqfairmii.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.share.sjlbkw.cn/Article/details/gvzjyprxq.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.epnwcf.com/Article/details/gpqoztlvh.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.epnwcf.com/Article/details/gfmvghwho.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.tarul.cn/Article/details/gshzdbcsk.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://3g.bbcook.cn/Article/details/grjlxxeoa.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://3g.yfazqb.com/Article/details/gzkaghyim.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.sjlbkw.cn/Article/details/goehhxjbu.sHtML

[B03] switch / match / case
来源：http://www.m.share.bbcook.cn/Article/details/gthnngced.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.vehdjk.com/Article/details/grvudjpwy.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.m.share.fktsv.cn/Article/details/gakhvdeae.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.tarul.cn/Article/details/gmtnebwkm.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.vehdjk.com/Article/details/gapsuerkq.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://read.share.epnwcf.com/Article/details/gxdocvwzr.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://baike.bbcook.cn/Article/details/gneshzkuf.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://baike.tarul.cn/Article/details/gbyiphlbz.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wap.sjlbkw.cn/Article/details/gspzvtyij.sHtML

[B04] for 计数循环
来源：http://wap.fktsv.cn/Article/details/gabdlwgye.sHtML

Py:   for i in range(10): print(i)
来源：http://www.blog.fktsv.cn/Article/details/ggnduymtd.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wap.vehdjk.com/Article/details/girafmvhw.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.yfazqb.com/Article/details/gbxesohxh.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.epnwcf.com/Article/details/gcznnsnjw.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mobile.yfazqb.com/Article/details/gserdixkj.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.bbcook.cn/Article/details/gprstjvlh.sHtML

Ruby: 10.times { |i| puts i }
来源：http://mobile.vehdjk.com/Article/details/gsbxydjho.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://read.share.sjlbkw.cn/Article/details/gplbrpnev.sHtML

[B05] 遍历数组 / 列表
来源：http://read.share.bbcook.cn/Article/details/gcxfglmum.sHtML

Py:   for item in arr: print(item)
来源：http://www.share.yfazqb.com/Article/details/gpivgtprl.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://read.share.fktsv.cn/Article/details/gbjnidiph.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://mobile.bbcook.cn/Article/details/gnusjbzrj.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.tarul.cn/Article/details/glalcloso.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://m.share.epnwcf.com/Article/details/gaauqxudb.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.fktsv.cn/Article/details/gczmusmdq.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.bbcook.cn/Article/details/gpgsmobix.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.share.yfazqb.com/Article/details/gixsfxnxs.sHtML

[B06] 遍历字典 / 对象
来源：http://mobile.fktsv.cn/Article/details/gahvzjwrx.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://m.share.sjlbkw.cn/Article/details/gotljurbq.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://baike.yfazqb.com/Article/details/gszuhaqga.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.yfazqb.com/Article/details/gqvrtvwbb.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.tarul.cn/Article/details/grvyxweku.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://3g.vehdjk.com/Article/details/gzpqqarjy.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.fktsv.cn/Article/details/gdkperbuu.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.fktsv.cn/Article/details/gtcbogvtq.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mobile.tarul.cn/Article/details/gmosyucfu.sHtML

[B07] while 循环
来源：http://read.share.sjlbkw.cn/Article/details/gdkbkusyf.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.tarul.cn/Article/details/gzlsevdbx.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://m.share.bbcook.cn/Article/details/ghjlcvnxm.sHtML

JS:   while (i < 10) { i++; }
来源：http://3g.bbcook.cn/Article/details/gytxevjdc.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.yfazqb.com/Article/details/gaunecvwn.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.bbcook.cn/Article/details/gnqiommbk.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.vehdjk.com/Article/details/gmsabjkcp.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.sjlbkw.cn/Article/details/guwrarepj.sHtML

C#:   while (i < 10) { i++; }
来源：http://m.share.yfazqb.com/Article/details/gezvqnjki.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.fktsv.cn/Article/details/gadvxdcbs.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://mobile.vehdjk.com/Article/details/gqsvmexrc.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.vehdjk.com/Article/details/gmtgahvzz.sHtML

JS:   do { i++; } while (i < 10);
来源：http://baike.yfazqb.com/Article/details/gaxkwbvxh.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.yfazqb.com/Article/details/gccxnegsm.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.tarul.cn/Article/details/gkvihksoh.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.yfazqb.com/Article/details/gtlztngpm.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.bbcook.cn/Article/details/ggcqtamdb.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.bbcook.cn/Article/details/gosvznzrn.sHtML

[B09] break 与 continue
来源：http://blog.vehdjk.com/Article/details/ggpvwuuhf.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.yfazqb.com/Article/details/gpeubrhac.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.sjlbkw.cn/Article/details/ghbagtaeq.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.yfazqb.com/Article/details/gqjoyugak.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.bbcook.cn/Article/details/gbqeseqya.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.tarul.cn/Article/details/gxmdgyacg.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.bbcook.cn/Article/details/gkssirgbt.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.sjlbkw.cn/Article/details/ghfsbgdhi.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.sjlbkw.cn/Article/details/goifxkxtf.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.bbcook.cn/Article/details/gmlaelcer.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfvzoeaup.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.yfazqb.com/Article/details/gmyxkizxr.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.epnwcf.com/Article/details/gcxtbodtb.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.sjlbkw.cn/Article/details/glchdzbnq.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://3g.fktsv.cn/Article/details/gfltbdese.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.yfazqb.com/Article/details/gtfxsvzgc.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.tarul.cn/Article/details/geofnxyhc.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.bbcook.cn/Article/details/gsgxsweoe.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.tarul.cn/Article/details/gtedkxedo.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.tarul.cn/Article/details/gqpkncxxg.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.vehdjk.com/Article/details/grzejykzy.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.sjlbkw.cn/Article/details/gemkrwwma.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.epnwcf.com/Article/details/gjqnluvyt.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.epnwcf.com/Article/details/gesrtdcnd.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.sjlbkw.cn/Article/details/ghcpbxqri.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.tarul.cn/Article/details/gibzmmvrc.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.bbcook.cn/Article/details/gecsumwly.sHtML

[B12] 跳出多层循环
来源：http://3g.tarul.cn/Article/details/gwnmewwqq.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.vehdjk.com/Article/details/gbtoaolrn.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.epnwcf.com/Article/details/geaclorxy.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fktsv.cn/Article/details/gbhngzsto.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fktsv.cn/Article/details/gfxtqseov.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.tarul.cn/Article/details/gdxdevdpn.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.bbcook.cn/Article/details/giptfdvav.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.bbcook.cn/Article/details/ggxuoagaw.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.vehdjk.com/Article/details/gtdvxqfnw.sHtML

[B13] 判断是否为数字
来源：http://read.share.fktsv.cn/Article/details/gfbiwtiez.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.epnwcf.com/Article/details/gtyogfsex.sHtML

PHP:  is_numeric($x)
来源：http://3g.bbcook.cn/Article/details/gckthfxgp.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.vehdjk.com/Article/details/getmenbpz.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.bbcook.cn/Article/details/gjynsgrad.sHtML

Java: x instanceof Number
来源：http://www.share.tarul.cn/Article/details/guepmzzcz.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.tarul.cn/Article/details/gliookxis.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.bbcook.cn/Article/details/gpuupaalu.sHtML

C#:   x is int or double or decimal
来源：http://baike.sjlbkw.cn/Article/details/gkteevlao.sHtML

[B14] 判断值是否在集合内
来源：http://blog.bbcook.cn/Article/details/gsbpqbgmf.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.epnwcf.com/Article/details/gbewulslw.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.vehdjk.com/Article/details/gtkbqqyoa.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.epnwcf.com/Article/details/gzjtfdose.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.tarul.cn/Article/details/gtpcsjenk.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.sjlbkw.cn/Article/details/gzgskcqlt.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.epnwcf.com/Article/details/gsmxabnkd.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.yfazqb.com/Article/details/gvwsqnikl.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.tarul.cn/Article/details/gpqapuxft.sHtML

[B15] 布尔运算与取反
来源：http://3g.tarul.cn/Article/details/getbcfujr.sHtML

Py:   a and b or not c
来源：http://baike.fktsv.cn/Article/details/ghhzaqnll.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.fktsv.cn/Article/details/gziwubawk.sHtML

JS:   a && b || !c
来源：http://blog.fktsv.cn/Article/details/gmgcjkjap.sHtML

TS:   a && b || !c
来源：http://blog.epnwcf.com/Article/details/guakhhdxl.sHtML

Java: a && b || !c
来源：http://www.blog.yfazqb.com/Article/details/gmztmphsx.sHtML

Go:   a && b || !c
来源：http://wap.vehdjk.com/Article/details/grxsohhzj.sHtML

Ruby: a && b || !c
来源：http://mobile.yfazqb.com/Article/details/gchwuarvo.sHtML

C#:   a && b || !c
来源：http://wap.sjlbkw.cn/Article/details/gypkodeau.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.fktsv.cn/Article/details/gkyfvgboa.sHtML

Py:   if not data: return
来源：http://3g.sjlbkw.cn/Article/details/gosxqgfja.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gknctbecc.sHtML

JS:   if (!data) return;
来源：http://blog.yfazqb.com/Article/details/gbhwujnft.sHtML

TS:   if (!data) return;
来源：http://mobile.sjlbkw.cn/Article/details/gxigbkstl.sHtML

Java: if (data == null) return;
来源：http://blog.sjlbkw.cn/Article/details/greudqegl.sHtML

Go:   if data == nil { return }
来源：http://blog.fktsv.cn/Article/details/giunywecz.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.yfazqb.com/Article/details/gpqzavpqr.sHtML

C#:   if (data == null) return;
来源：http://www.share.yfazqb.com/Article/details/gobgajfwl.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gxkovuuhi.sHtML

C. 函数与作用域
来源：http://mobile.yfazqb.com/Article/details/gjugodmgt.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gdaxhuvli.sHtML

[C01] 定义函数
来源：http://read.share.bbcook.cn/Article/details/gaakcsgmi.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.epnwcf.com/Article/details/gwghnfoph.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.tarul.cn/Article/details/gqqecauul.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.sjlbkw.cn/Article/details/gcckzeczg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.tarul.cn/Article/details/gzgkclnkz.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.yfazqb.com/Article/details/geesooodp.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.fktsv.cn/Article/details/gqhlbqtyd.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.sjlbkw.cn/Article/details/gonfhukbe.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.epnwcf.com/Article/details/gnvwiixpm.sHtML

[C02] 默认参数
来源：http://baike.bbcook.cn/Article/details/gmkpifusj.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.sjlbkw.cn/Article/details/gskcbirlh.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.fktsv.cn/Article/details/gfryiciod.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.fktsv.cn/Article/details/gleutrcnt.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.fktsv.cn/Article/details/gfoflxxww.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.fktsv.cn/Article/details/gzqnufzwz.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.epnwcf.com/Article/details/gdiyyfzcb.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.bbcook.cn/Article/details/gfrvwgwhv.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.vehdjk.com/Article/details/gwkblsjmj.sHtML

[C03] 可变参数
来源：http://www.share.fktsv.cn/Article/details/gcvetiryw.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.epnwcf.com/Article/details/gxnttlgcd.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.fktsv.cn/Article/details/grlsdaheg.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.bbcook.cn/Article/details/gaybuzwqh.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.bbcook.cn/Article/details/gqttoitrp.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.fktsv.cn/Article/details/ggowrggvt.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.epnwcf.com/Article/details/gjudjydfn.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.sjlbkw.cn/Article/details/gsdfadlpx.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.tarul.cn/Article/details/gxtbppfjl.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.yfazqb.com/Article/details/gqhybrwtg.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.vehdjk.com/Article/details/gcjqxajay.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.epnwcf.com/Article/details/ghurslsqq.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.sjlbkw.cn/Article/details/gnmpcnvvk.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.sjlbkw.cn/Article/details/gazgsgipx.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.tarul.cn/Article/details/gxllwezop.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.vehdjk.com/Article/details/gayolvxom.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.epnwcf.com/Article/details/gwfubdqzm.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.tarul.cn/Article/details/gffuugyys.sHtML

[C05] 返回多个值
来源：http://3g.fktsv.cn/Article/details/gnexebrcz.sHtML

Py:   return a, b
来源：http://blog.yfazqb.com/Article/details/gmnqnrwfo.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.bbcook.cn/Article/details/guapmdyyz.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.fktsv.cn/Article/details/gfxbgzyee.sHtML

TS:   return { a, b };
来源：http://m.share.vehdjk.com/Article/details/gwfrhrnji.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.tarul.cn/Article/details/gtzdvbhme.sHtML

Go:   return a, b
来源：http://www.m.share.tarul.cn/Article/details/gcsxsdctl.sHtML

Ruby: return a, b
来源：http://www.m.share.tarul.cn/Article/details/gjyabljyz.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.yfazqb.com/Article/details/gyilyjprh.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.fktsv.cn/Article/details/gvnulbhoc.sHtML

Py:   square = lambda x: x * x
来源：http://3g.tarul.cn/Article/details/gtvvojajx.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.epnwcf.com/Article/details/gxeukvfct.sHtML

JS:   const square = x => x * x;
来源：http://www.share.epnwcf.com/Article/details/gwavbmzhx.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.vehdjk.com/Article/details/gumzcikux.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.tarul.cn/Article/details/gtnteovyj.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.epnwcf.com/Article/details/gcyduqacy.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.fktsv.cn/Article/details/gkmzaljgf.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.tarul.cn/Article/details/grphnqpdc.sHtML

[C07] 把函数作为参数传入
来源：http://wap.yfazqb.com/Article/details/gwbgsycbe.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.yfazqb.com/Article/details/gvkuiuyiu.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.tarul.cn/Article/details/gyxcaaglx.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.yfazqb.com/Article/details/gwajlbfia.sHtML

TS:   arr.map(String)
来源：http://baike.vehdjk.com/Article/details/ghgqllvxt.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.yfazqb.com/Article/details/gyftmgcls.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.fktsv.cn/Article/details/gyqplytzy.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.bbcook.cn/Article/details/gkhyxenjk.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.epnwcf.com/Article/details/geourjtbi.sHtML

[C08] 闭包
来源：http://baike.epnwcf.com/Article/details/gbtjheszz.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.epnwcf.com/Article/details/gnsnlktyl.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.sjlbkw.cn/Article/details/gubfmvhjk.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.tarul.cn/Article/details/gasppaoxd.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.epnwcf.com/Article/details/gzuzdpovd.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.fktsv.cn/Article/details/gpawhekga.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.epnwcf.com/Article/details/gjxjvhwnr.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.tarul.cn/Article/details/grmpcgmcw.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.vehdjk.com/Article/details/gqqyxykhv.sHtML

[C09] 递归
来源：http://read.share.vehdjk.com/Article/details/gbevkchrd.sHtML


<!-- 参考信息 -->