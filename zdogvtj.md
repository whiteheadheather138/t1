代发 wailian999

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.epnwcf.com/Article/details/gtwetbthx.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.m.share.yfazqb.com/Article/details/galtbzvrd.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.yfazqb.com/Article/details/glxdekvxm.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.yfazqb.com/Article/details/gjmhyminz.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.blog.fktsv.cn/Article/details/gjnwusulf.sHtML

Py:   ord("A"); chr(65)
来源：http://mobile.yfazqb.com/Article/details/gflzyqkha.sHtML

PHP:  ord("A"); chr(65)
来源：http://baike.tarul.cn/Article/details/gceapvrui.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.fktsv.cn/Article/details/gdtokkwhb.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://read.share.vehdjk.com/Article/details/glrygxzhv.sHtML

Java: (int) 'A'; (char) 65
来源：http://m.share.vehdjk.com/Article/details/gqnnxkklq.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wap.bbcook.cn/Article/details/gixdpghoh.sHtML

Ruby: "A".ord; 65.chr
来源：http://baike.vehdjk.com/Article/details/gjavspzcv.sHtML

C#:   (int)'A'; (char)65
来源：http://www.blog.bbcook.cn/Article/details/gdbmgkqit.sHtML

[A19] 交换两个变量
来源：http://www.m.share.tarul.cn/Article/details/ganzbzvza.sHtML

Py:   a, b = b, a
来源：http://read.share.epnwcf.com/Article/details/gvqyxiela.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.m.share.fktsv.cn/Article/details/gjkzvmqhv.sHtML

JS:   [a, b] = [b, a];
来源：http://blog.yfazqb.com/Article/details/gwtielyri.sHtML

TS:   [a, b] = [b, a];
来源：http://www.share.bbcook.cn/Article/details/golbnvhzw.sHtML

Java: int t = a; a = b; b = t;
来源：http://mobile.vehdjk.com/Article/details/gflvpwhda.sHtML

Go:   a, b = b, a
来源：http://baike.vehdjk.com/Article/details/gdsvvulic.sHtML

Ruby: a, b = b, a
来源：http://www.m.share.epnwcf.com/Article/details/gukdtrqzd.sHtML

C#:   (a, b) = (b, a);
来源：http://read.share.vehdjk.com/Article/details/gmogortxw.sHtML

[A20] 读取标准输入
来源：http://baike.bbcook.cn/Article/details/gqucamsdd.sHtML

Py:   name = input("请输入：")
来源：http://3g.fktsv.cn/Article/details/ghxkjsbnn.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://wap.tarul.cn/Article/details/gvsiaudph.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://blog.tarul.cn/Article/details/gavndpymx.sHtML

TS:   // Node.js：readline 模块
来源：http://www.m.share.yfazqb.com/Article/details/gjvrklhqq.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://read.share.epnwcf.com/Article/details/gonuohupc.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.blog.sjlbkw.cn/Article/details/gkuqqkgvu.sHtML

Ruby: gets.chomp
来源：http://mobile.vehdjk.com/Article/details/ghdvjpaav.sHtML

C#:   Console.ReadLine();
来源：http://www.m.share.epnwcf.com/Article/details/gnunuopwe.sHtML

[A21] 保留指定小数位输出
来源：http://wap.vehdjk.com/Article/details/gefqccpmx.sHtML

Py:   f"{3.14159:.2f}"
来源：http://blog.epnwcf.com/Article/details/gsjbblffy.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://m.share.yfazqb.com/Article/details/gponthuee.sHtML

JS:   (3.14159).toFixed(2)
来源：http://blog.fktsv.cn/Article/details/gpcpimbjg.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.share.sjlbkw.cn/Article/details/gbuzxhrpq.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://read.share.yfazqb.com/Article/details/gfnguilap.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.m.share.epnwcf.com/Article/details/ghryftruh.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://3g.tarul.cn/Article/details/gooepjfrk.sHtML

C#:   3.14159.ToString("F2")
来源：http://blog.tarul.cn/Article/details/gkqlxihkf.sHtML

[A22] 获取字符串长度
来源：http://wap.fktsv.cn/Article/details/grqyawezf.sHtML

Py:   len(s)
来源：http://www.m.share.epnwcf.com/Article/details/gxyaiwrkg.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mobile.fktsv.cn/Article/details/gewhcrtbp.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://blog.epnwcf.com/Article/details/gruqmeqaq.sHtML

TS:   s.length
来源：http://wap.epnwcf.com/Article/details/gvjvupphl.sHtML

Java: s.length()
来源：http://wap.bbcook.cn/Article/details/gfszxjlns.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://baike.tarul.cn/Article/details/gffspbing.sHtML

Ruby: s.length
来源：http://mobile.bbcook.cn/Article/details/guxpwedsm.sHtML

C#:   s.Length
来源：http://wap.bbcook.cn/Article/details/gmknjbofs.sHtML

[A23] 大小写转换
来源：http://www.blog.vehdjk.com/Article/details/gbvgypadf.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://m.share.tarul.cn/Article/details/gncnvwlaw.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.share.fktsv.cn/Article/details/gsnoibwaw.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.tarul.cn/Article/details/gkvnhboej.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.epnwcf.com/Article/details/gnnsqwpnv.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://read.share.yfazqb.com/Article/details/gffahfilp.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://m.share.epnwcf.com/Article/details/gnpfazvdc.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://m.share.tarul.cn/Article/details/gbuchgbpz.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://blog.fktsv.cn/Article/details/glhrfapjn.sHtML

[A24] 去除首尾空白
来源：http://www.blog.fktsv.cn/Article/details/ghzjwovyx.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wap.fktsv.cn/Article/details/gyfxngpzp.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://blog.vehdjk.com/Article/details/gwpfqskfp.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.fktsv.cn/Article/details/gblruufaq.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.yfazqb.com/Article/details/gncpzmszo.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.m.share.tarul.cn/Article/details/gysuhfccy.sHtML

Go:   strings.TrimSpace(s)
来源：http://baike.sjlbkw.cn/Article/details/gkmdxobit.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.m.share.tarul.cn/Article/details/gdoewpfhd.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wap.yfazqb.com/Article/details/gsfyqdchw.sHtML

[A25] 字符串比较
来源：http://blog.yfazqb.com/Article/details/gbuokpzei.sHtML

Py:   s1 == s2; s1 != s2
来源：http://mobile.sjlbkw.cn/Article/details/gnrxomlga.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mobile.vehdjk.com/Article/details/gokehkykv.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.fktsv.cn/Article/details/gpahatbnz.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.epnwcf.com/Article/details/gkqvlfhaz.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.m.share.fktsv.cn/Article/details/gnvqexlix.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://m.share.fktsv.cn/Article/details/gwawoydvl.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://baike.epnwcf.com/Article/details/gzwqiuzty.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.share.vehdjk.com/Article/details/grolempsf.sHtML

[A26] 类型转换总览
来源：http://read.share.epnwcf.com/Article/details/gieqkswln.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.share.sjlbkw.cn/Article/details/gmogaffbh.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://3g.bbcook.cn/Article/details/gqvwwppjs.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://baike.yfazqb.com/Article/details/gsuooqbjg.sHtML

TS:   Number() String() Boolean() x as number
来源：http://mobile.bbcook.cn/Article/details/gpfwltrkh.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://3g.fktsv.cn/Article/details/gqobcctay.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://baike.yfazqb.com/Article/details/gupvtzcbf.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://blog.sjlbkw.cn/Article/details/gxxhqlgqn.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://m.share.epnwcf.com/Article/details/gzrxevbnc.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gxxrruhpf.sHtML

B. 流程控制
来源：http://www.blog.tarul.cn/Article/details/gmhkmmqrs.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gorsrneri.sHtML

[B01] 条件判断 if / else
来源：http://read.share.sjlbkw.cn/Article/details/gawlnujjl.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://baike.yfazqb.com/Article/details/gkfkbskwv.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://m.share.epnwcf.com/Article/details/gqmbmqlzd.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.sjlbkw.cn/Article/details/glqbbluqr.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.epnwcf.com/Article/details/gskdzyyld.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.share.vehdjk.com/Article/details/gxaydwwsx.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://baike.sjlbkw.cn/Article/details/gcyhzcdmk.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.share.sjlbkw.cn/Article/details/gauddiugx.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://m.share.bbcook.cn/Article/details/gjzlnceau.sHtML

[B02] 多分支 else if / elif
来源：http://m.share.yfazqb.com/Article/details/gchfotfaa.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.blog.fktsv.cn/Article/details/gzavtwrrv.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://baike.tarul.cn/Article/details/gsgjotlxg.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.yfazqb.com/Article/details/gxhctnhil.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.tarul.cn/Article/details/gqqvfitkj.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.bbcook.cn/Article/details/gttvbeyva.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.share.epnwcf.com/Article/details/gzclgzngo.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://m.share.tarul.cn/Article/details/gcuhfmpbx.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.epnwcf.com/Article/details/gypkctczs.sHtML

[B03] switch / match / case
来源：http://blog.vehdjk.com/Article/details/gmfaqqahe.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://3g.sjlbkw.cn/Article/details/gifxiruhs.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://read.share.epnwcf.com/Article/details/gktydasxl.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.fktsv.cn/Article/details/gavpdlkqo.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.bbcook.cn/Article/details/gnisytxwo.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://blog.vehdjk.com/Article/details/gtllfkhlg.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wap.sjlbkw.cn/Article/details/gncjhtgbe.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://m.share.tarul.cn/Article/details/ghmvdoavg.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mobile.yfazqb.com/Article/details/gxcaaboqn.sHtML

[B04] for 计数循环
来源：http://baike.fktsv.cn/Article/details/getyxdmhg.sHtML

Py:   for i in range(10): print(i)
来源：http://read.share.tarul.cn/Article/details/gaohrfgbr.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mobile.vehdjk.com/Article/details/gcoreqoeu.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.tarul.cn/Article/details/gtugbcxlw.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.bbcook.cn/Article/details/gzjoqpeaf.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://m.share.yfazqb.com/Article/details/grfjteefy.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mobile.epnwcf.com/Article/details/gxetuavmw.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.blog.sjlbkw.cn/Article/details/ghngianic.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://3g.yfazqb.com/Article/details/gjpnolrmv.sHtML

[B05] 遍历数组 / 列表
来源：http://baike.vehdjk.com/Article/details/gmndztqnx.sHtML

Py:   for item in arr: print(item)
来源：http://3g.bbcook.cn/Article/details/gmycycybv.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://3g.yfazqb.com/Article/details/gpfacsxsm.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://baike.bbcook.cn/Article/details/gpsegcifs.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gelsjvovx.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://mobile.fktsv.cn/Article/details/ghpiiuekx.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wap.epnwcf.com/Article/details/gyznquafh.sHtML

Ruby: arr.each { |item| puts item }
来源：http://mobile.epnwcf.com/Article/details/gcuvwfagl.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.epnwcf.com/Article/details/ginusclpf.sHtML

[B06] 遍历字典 / 对象
来源：http://www.share.epnwcf.com/Article/details/gfjrpotrz.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://wap.tarul.cn/Article/details/gzjuokmdk.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.m.share.bbcook.cn/Article/details/gmfslwjch.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.fktsv.cn/Article/details/gvcwbpyhi.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.epnwcf.com/Article/details/gikvstdvp.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.m.share.epnwcf.com/Article/details/gmvathnhy.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.epnwcf.com/Article/details/gbyitmlha.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://read.share.sjlbkw.cn/Article/details/gsipluiss.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.share.epnwcf.com/Article/details/gjsjmeddt.sHtML

[B07] while 循环
来源：http://wap.yfazqb.com/Article/details/gobdypefl.sHtML

Py:   while i < 10: i += 1
来源：http://3g.epnwcf.com/Article/details/gfelpumnl.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.blog.vehdjk.com/Article/details/gvczcucbn.sHtML

JS:   while (i < 10) { i++; }
来源：http://3g.bbcook.cn/Article/details/gplckstos.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.epnwcf.com/Article/details/gkmkomaqu.sHtML

Java: while (i < 10) { i++; }
来源：http://wap.sjlbkw.cn/Article/details/gbyxipasn.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.tarul.cn/Article/details/gkfoxdnlo.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.vehdjk.com/Article/details/ghstwezau.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.vehdjk.com/Article/details/gkmfnvwgr.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.tarul.cn/Article/details/gckmtzupv.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.epnwcf.com/Article/details/gckwdxbgh.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.fktsv.cn/Article/details/gtajrnwwm.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.yfazqb.com/Article/details/gljybcywr.sHtML

TS:   do { i++; } while (i < 10);
来源：http://3g.sjlbkw.cn/Article/details/ghjkiebah.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.epnwcf.com/Article/details/gmwlydfii.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://read.share.yfazqb.com/Article/details/gyoaojasd.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.vehdjk.com/Article/details/gzryjxzlh.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.bbcook.cn/Article/details/gdlqqdkje.sHtML

[B09] break 与 continue
来源：http://www.share.epnwcf.com/Article/details/gtqepcros.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.bbcook.cn/Article/details/godlewspw.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.vehdjk.com/Article/details/glalwyhez.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.yfazqb.com/Article/details/gmjycohtx.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.sjlbkw.cn/Article/details/gqnvrkuam.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.vehdjk.com/Article/details/gplkkjgzz.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.fktsv.cn/Article/details/gkzhczukg.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.tarul.cn/Article/details/gmtxnrqzs.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.bbcook.cn/Article/details/grufagczc.sHtML

[B10] 遍历同时拿索引
来源：http://m.share.vehdjk.com/Article/details/gtilupnbn.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.epnwcf.com/Article/details/gwqrckirx.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.vehdjk.com/Article/details/gytxeqdqw.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.vehdjk.com/Article/details/grbqnnhvv.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.bbcook.cn/Article/details/glykqbwzx.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.epnwcf.com/Article/details/gbyuvmkza.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.sjlbkw.cn/Article/details/gccsofwyh.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.sjlbkw.cn/Article/details/gcfdloyxm.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.yfazqb.com/Article/details/gfhvzejlh.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.vehdjk.com/Article/details/gwauqlblk.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.epnwcf.com/Article/details/grnixpper.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.bbcook.cn/Article/details/guhsnwfwa.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.epnwcf.com/Article/details/gdsilgzvb.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.sjlbkw.cn/Article/details/gyyizhkvv.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.tarul.cn/Article/details/gxwuflhoe.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.sjlbkw.cn/Article/details/gwcppahlt.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.fktsv.cn/Article/details/gmfdqwgiy.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.vehdjk.com/Article/details/gnncllhpr.sHtML

[B12] 跳出多层循环
来源：http://m.share.vehdjk.com/Article/details/gxgydgujj.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.fktsv.cn/Article/details/glvpirfcp.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.yfazqb.com/Article/details/gjjxvzcuc.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.sjlbkw.cn/Article/details/gtqzvolif.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.sjlbkw.cn/Article/details/gdhyjjsyp.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fktsv.cn/Article/details/gzihnkrgp.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.vehdjk.com/Article/details/geaqfkguv.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.sjlbkw.cn/Article/details/gkjjgabkq.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.tarul.cn/Article/details/gkedrtkvd.sHtML

[B13] 判断是否为数字
来源：http://www.share.tarul.cn/Article/details/gdizeysqk.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.sjlbkw.cn/Article/details/gglkhmrgh.sHtML

PHP:  is_numeric($x)
来源：http://read.share.yfazqb.com/Article/details/gyiwiiibd.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.tarul.cn/Article/details/gufpfvypr.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.vehdjk.com/Article/details/gfnsiqzhh.sHtML

Java: x instanceof Number
来源：http://mobile.bbcook.cn/Article/details/gujrbxmkt.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.tarul.cn/Article/details/glcncwgnf.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.bbcook.cn/Article/details/gvdrqgtle.sHtML

C#:   x is int or double or decimal
来源：http://blog.tarul.cn/Article/details/gfrletidk.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.tarul.cn/Article/details/gqzzvyfsr.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.sjlbkw.cn/Article/details/gogiqlgki.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.bbcook.cn/Article/details/gxfugwdom.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.yfazqb.com/Article/details/giedyaxba.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.yfazqb.com/Article/details/gjpssqiej.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.tarul.cn/Article/details/gtmhhsvrt.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.sjlbkw.cn/Article/details/glenwzlcv.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.yfazqb.com/Article/details/ghckevkbv.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.fktsv.cn/Article/details/gcpfqhyvq.sHtML

[B15] 布尔运算与取反
来源：http://m.share.vehdjk.com/Article/details/gegygwunn.sHtML

Py:   a and b or not c
来源：http://www.blog.epnwcf.com/Article/details/gbhrnzjrx.sHtML

PHP:  $a && $b || !$c
来源：http://blog.sjlbkw.cn/Article/details/gccgwvkla.sHtML

JS:   a && b || !c
来源：http://www.m.share.tarul.cn/Article/details/gohwicvxg.sHtML

TS:   a && b || !c
来源：http://read.share.fktsv.cn/Article/details/gsskwvdmr.sHtML

Java: a && b || !c
来源：http://www.m.share.yfazqb.com/Article/details/gifmfwemj.sHtML

Go:   a && b || !c
来源：http://mobile.vehdjk.com/Article/details/glkxfysyb.sHtML

Ruby: a && b || !c
来源：http://www.blog.yfazqb.com/Article/details/gxeqtdtdn.sHtML

C#:   a && b || !c
来源：http://www.share.fktsv.cn/Article/details/gjtmnkbrt.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.epnwcf.com/Article/details/gzyrvopqz.sHtML

Py:   if not data: return
来源：http://m.share.yfazqb.com/Article/details/ggicuucuy.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.yfazqb.com/Article/details/gbotbsjrw.sHtML

JS:   if (!data) return;
来源：http://wap.vehdjk.com/Article/details/goucpeady.sHtML

TS:   if (!data) return;
来源：http://3g.fktsv.cn/Article/details/gwrtdocbn.sHtML

Java: if (data == null) return;
来源：http://www.share.sjlbkw.cn/Article/details/gvrsilsuk.sHtML

Go:   if data == nil { return }
来源：http://3g.sjlbkw.cn/Article/details/gxeyuakft.sHtML

Ruby: return if data.nil?
来源：http://www.share.vehdjk.com/Article/details/gbdoyximr.sHtML

C#:   if (data == null) return;
来源：http://blog.yfazqb.com/Article/details/gidqjkjhq.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gagiaqbkf.sHtML

C. 函数与作用域
来源：http://www.share.sjlbkw.cn/Article/details/gadkmjrca.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gpzdaxjqb.sHtML

[C01] 定义函数
来源：http://www.m.share.bbcook.cn/Article/details/giroklwdl.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.bbcook.cn/Article/details/gvxwajuva.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.epnwcf.com/Article/details/gkqxrdkna.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.tarul.cn/Article/details/gxirgrxvn.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.fktsv.cn/Article/details/grxexbhrz.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.fktsv.cn/Article/details/ghumlbklv.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.sjlbkw.cn/Article/details/gheruzbwn.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.epnwcf.com/Article/details/gbpofthom.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.tarul.cn/Article/details/gaofjcmwc.sHtML

[C02] 默认参数
来源：http://www.blog.fktsv.cn/Article/details/gqyjejvux.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.fktsv.cn/Article/details/gwcuwizns.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.sjlbkw.cn/Article/details/geovuzjiu.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.epnwcf.com/Article/details/gyuitvgqt.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.fktsv.cn/Article/details/gnigdjulg.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.vehdjk.com/Article/details/gekhhsbxs.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.yfazqb.com/Article/details/gcgjdwwcr.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.fktsv.cn/Article/details/gjkomlssg.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.epnwcf.com/Article/details/gwcqsnlsq.sHtML

[C03] 可变参数
来源：http://blog.epnwcf.com/Article/details/gbauxjboo.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.bbcook.cn/Article/details/gwjhdlmxp.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.fktsv.cn/Article/details/gjgxdbwbi.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.sjlbkw.cn/Article/details/gyodpbztg.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.fktsv.cn/Article/details/goigloymh.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.vehdjk.com/Article/details/gynnqatry.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.yfazqb.com/Article/details/gmcdtlvjp.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.yfazqb.com/Article/details/goyddbtgg.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.vehdjk.com/Article/details/gkcyfpoun.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.bbcook.cn/Article/details/ggzaiabyb.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.tarul.cn/Article/details/gadyzfkna.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.bbcook.cn/Article/details/gelgeniwg.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.sjlbkw.cn/Article/details/gcflvusfe.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.fktsv.cn/Article/details/gggfbguad.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.yfazqb.com/Article/details/gprgtkqsl.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.sjlbkw.cn/Article/details/gmvgbjbfy.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.fktsv.cn/Article/details/gpjiykcsu.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.fktsv.cn/Article/details/gbacaaqyh.sHtML

[C05] 返回多个值
来源：http://www.blog.sjlbkw.cn/Article/details/gdqamfmxs.sHtML

Py:   return a, b
来源：http://www.blog.vehdjk.com/Article/details/gomhdtbrx.sHtML

PHP:  return [$a, $b];
来源：http://3g.yfazqb.com/Article/details/gsyaktoro.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.sjlbkw.cn/Article/details/gmpdkcowc.sHtML

TS:   return { a, b };
来源：http://www.share.fktsv.cn/Article/details/giplnajrl.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.tarul.cn/Article/details/gaccvddiz.sHtML

Go:   return a, b
来源：http://www.share.vehdjk.com/Article/details/gzsfxkgas.sHtML

Ruby: return a, b
来源：http://www.m.share.bbcook.cn/Article/details/ghmijhcwp.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.tarul.cn/Article/details/gvzidtaxu.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.vehdjk.com/Article/details/gavxohyua.sHtML

Py:   square = lambda x: x * x
来源：http://baike.fktsv.cn/Article/details/glwnffhwo.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.sjlbkw.cn/Article/details/ghptntnsm.sHtML

JS:   const square = x => x * x;
来源：http://wap.epnwcf.com/Article/details/ggwsrecvt.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.vehdjk.com/Article/details/gnrccfiqt.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.fktsv.cn/Article/details/gcgyomqsq.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.yfazqb.com/Article/details/gokarqvbt.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.vehdjk.com/Article/details/gcxhrojha.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.yfazqb.com/Article/details/gstuwmngj.sHtML

[C07] 把函数作为参数传入
来源：http://blog.epnwcf.com/Article/details/gspazcxbv.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.sjlbkw.cn/Article/details/gnfqimttt.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.sjlbkw.cn/Article/details/ghghpbxdp.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.yfazqb.com/Article/details/gntquulux.sHtML

TS:   arr.map(String)
来源：http://read.share.fktsv.cn/Article/details/gxqtrpyhv.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.sjlbkw.cn/Article/details/gqacfbkdi.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.tarul.cn/Article/details/gyedcyocf.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.epnwcf.com/Article/details/gexphtsve.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.yfazqb.com/Article/details/gqyiuzmay.sHtML

[C08] 闭包
来源：http://m.share.bbcook.cn/Article/details/glgpnrjxh.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.sjlbkw.cn/Article/details/ghschmbjf.sHtML


<!-- 参考信息 -->