代发 wailian999

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.fktsv.cn/Article/details/gjioaxbmx.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://baike.yfazqb.com/Article/details/gjhmfmmpi.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.bbcook.cn/Article/details/golqpvbtv.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.share.epnwcf.com/Article/details/gvqanlmqj.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.sjlbkw.cn/Article/details/guqjezmjf.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wap.tarul.cn/Article/details/gmjhrybyb.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.sjlbkw.cn/Article/details/ggmaeaopq.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.sjlbkw.cn/Article/details/gfavvcfug.sHtML

[A18] 字符与 ASCII 码互转
来源：http://read.share.yfazqb.com/Article/details/grquqbmzb.sHtML

Py:   ord("A"); chr(65)
来源：http://www.share.yfazqb.com/Article/details/gdokbqoog.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.blog.fktsv.cn/Article/details/gfapfuzsl.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.yfazqb.com/Article/details/gxhatxqdc.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.epnwcf.com/Article/details/glsnppvwr.sHtML

Java: (int) 'A'; (char) 65
来源：http://baike.vehdjk.com/Article/details/ghawuopav.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://blog.yfazqb.com/Article/details/guobkimwe.sHtML

Ruby: "A".ord; 65.chr
来源：http://blog.tarul.cn/Article/details/gbopljrpn.sHtML

C#:   (int)'A'; (char)65
来源：http://www.m.share.fktsv.cn/Article/details/grbsdmusp.sHtML

[A19] 交换两个变量
来源：http://mobile.tarul.cn/Article/details/geuxlujlb.sHtML

Py:   a, b = b, a
来源：http://www.share.yfazqb.com/Article/details/glatcnkss.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://read.share.tarul.cn/Article/details/ggjcyabua.sHtML

JS:   [a, b] = [b, a];
来源：http://www.blog.vehdjk.com/Article/details/gutlhzjvn.sHtML

TS:   [a, b] = [b, a];
来源：http://mobile.yfazqb.com/Article/details/golcmaidr.sHtML

Java: int t = a; a = b; b = t;
来源：http://baike.bbcook.cn/Article/details/gilxmacwc.sHtML

Go:   a, b = b, a
来源：http://www.m.share.epnwcf.com/Article/details/gtwojntnp.sHtML

Ruby: a, b = b, a
来源：http://blog.vehdjk.com/Article/details/grpfbpfdt.sHtML

C#:   (a, b) = (b, a);
来源：http://www.share.vehdjk.com/Article/details/gadiaipcd.sHtML

[A20] 读取标准输入
来源：http://m.share.yfazqb.com/Article/details/gymmkbkep.sHtML

Py:   name = input("请输入：")
来源：http://read.share.vehdjk.com/Article/details/gkavvirwj.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://3g.bbcook.cn/Article/details/gyeyfzvib.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://baike.fktsv.cn/Article/details/gjoaoytaf.sHtML

TS:   // Node.js：readline 模块
来源：http://m.share.epnwcf.com/Article/details/gmsafvwwi.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://m.share.tarul.cn/Article/details/gesvwlstz.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.share.bbcook.cn/Article/details/grkypmsxf.sHtML

Ruby: gets.chomp
来源：http://3g.bbcook.cn/Article/details/gnmakufko.sHtML

C#:   Console.ReadLine();
来源：http://read.share.tarul.cn/Article/details/ggzcbbpjk.sHtML

[A21] 保留指定小数位输出
来源：http://wap.yfazqb.com/Article/details/gndlyzojm.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.blog.bbcook.cn/Article/details/ghfbmkwmm.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://mobile.fktsv.cn/Article/details/gdqymamuc.sHtML

JS:   (3.14159).toFixed(2)
来源：http://mobile.bbcook.cn/Article/details/gogqjnpwc.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.blog.yfazqb.com/Article/details/glunthioc.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.share.vehdjk.com/Article/details/gcstsmemu.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://mobile.yfazqb.com/Article/details/glsxvsber.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://baike.sjlbkw.cn/Article/details/gnlfgkwkf.sHtML

C#:   3.14159.ToString("F2")
来源：http://wap.tarul.cn/Article/details/gzjdjqsbe.sHtML

[A22] 获取字符串长度
来源：http://www.blog.epnwcf.com/Article/details/gbzjcrjvz.sHtML

Py:   len(s)
来源：http://read.share.fktsv.cn/Article/details/gavzififm.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://m.share.tarul.cn/Article/details/gogohcrkm.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://baike.fktsv.cn/Article/details/gevryjnap.sHtML

TS:   s.length
来源：http://mobile.bbcook.cn/Article/details/gwfcxtdsi.sHtML

Java: s.length()
来源：http://read.share.tarul.cn/Article/details/gpifmeugv.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.m.share.bbcook.cn/Article/details/geqergwqu.sHtML

Ruby: s.length
来源：http://www.share.bbcook.cn/Article/details/gfkkqzxxd.sHtML

C#:   s.Length
来源：http://www.blog.sjlbkw.cn/Article/details/ggbclliyw.sHtML

[A23] 大小写转换
来源：http://m.share.fktsv.cn/Article/details/gjnqznnoh.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://wap.vehdjk.com/Article/details/gtzbibtnm.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.share.vehdjk.com/Article/details/gvhmwvvrn.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.fktsv.cn/Article/details/ghcsvffwt.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.tarul.cn/Article/details/gpwfwzwwk.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://3g.tarul.cn/Article/details/gnadsannk.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mobile.sjlbkw.cn/Article/details/gtlmclora.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.m.share.bbcook.cn/Article/details/grgcpdgcq.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.m.share.tarul.cn/Article/details/geivneodo.sHtML

[A24] 去除首尾空白
来源：http://read.share.sjlbkw.cn/Article/details/gprcrqdsk.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://baike.tarul.cn/Article/details/gkigytsnz.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://read.share.yfazqb.com/Article/details/gsxpnsjxs.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.vehdjk.com/Article/details/gwmskotur.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.tarul.cn/Article/details/gpjhvuovn.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://3g.fktsv.cn/Article/details/galstjfyo.sHtML

Go:   strings.TrimSpace(s)
来源：http://m.share.bbcook.cn/Article/details/gtlhpjbdg.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.blog.yfazqb.com/Article/details/gjbtnuyxo.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mobile.epnwcf.com/Article/details/gclikxmqh.sHtML

[A25] 字符串比较
来源：http://www.share.yfazqb.com/Article/details/gbqakritw.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.blog.vehdjk.com/Article/details/gwoamseso.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.m.share.fktsv.cn/Article/details/gnevusfis.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.tarul.cn/Article/details/gkezodusk.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.tarul.cn/Article/details/gseyazfwh.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://3g.fktsv.cn/Article/details/gfcsyijwo.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://baike.yfazqb.com/Article/details/gnawphfqw.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.m.share.fktsv.cn/Article/details/gejecdvsl.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wap.fktsv.cn/Article/details/gjcnuumqs.sHtML

[A26] 类型转换总览
来源：http://blog.sjlbkw.cn/Article/details/gxtavbgqn.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://blog.bbcook.cn/Article/details/gnpwpgzvp.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://m.share.fktsv.cn/Article/details/gjiuzsdjo.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://blog.epnwcf.com/Article/details/gripsdgid.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.m.share.yfazqb.com/Article/details/gygtaepit.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://blog.yfazqb.com/Article/details/gntyokygx.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.m.share.epnwcf.com/Article/details/gqwtxkejc.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.blog.sjlbkw.cn/Article/details/gbzdufide.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.m.share.yfazqb.com/Article/details/gmixaohms.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gwxmogvje.sHtML

B. 流程控制
来源：http://mobile.yfazqb.com/Article/details/gngjkgobt.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/ghvprsopp.sHtML

[B01] 条件判断 if / else
来源：http://wap.epnwcf.com/Article/details/gspzjmlfa.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://3g.tarul.cn/Article/details/gvtisndhq.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wap.sjlbkw.cn/Article/details/gtlogjhop.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.fktsv.cn/Article/details/gbzspxnyj.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.bbcook.cn/Article/details/gwneanjnl.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://3g.tarul.cn/Article/details/gqybbjrje.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://3g.vehdjk.com/Article/details/gmjetctow.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://read.share.bbcook.cn/Article/details/gfsaozsoy.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.share.tarul.cn/Article/details/gvaietfvl.sHtML

[B02] 多分支 else if / elif
来源：http://www.m.share.yfazqb.com/Article/details/grmsyxvmb.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://blog.vehdjk.com/Article/details/gyqxmoumr.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://baike.bbcook.cn/Article/details/gvoaqtwhp.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.bbcook.cn/Article/details/ggwjeqxni.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.epnwcf.com/Article/details/gpyzjthuj.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.sjlbkw.cn/Article/details/gwkicknhx.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://3g.fktsv.cn/Article/details/gzdfprkqr.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://3g.sjlbkw.cn/Article/details/gimwddngq.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.bbcook.cn/Article/details/gvcntcnmx.sHtML

[B03] switch / match / case
来源：http://3g.sjlbkw.cn/Article/details/grnsbnqtt.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://3g.tarul.cn/Article/details/gmaigwdef.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://baike.fktsv.cn/Article/details/glvbldkqb.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.tarul.cn/Article/details/guwcebqfp.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.tarul.cn/Article/details/gtqqrkisz.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mobile.vehdjk.com/Article/details/gcrehsdvy.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://m.share.tarul.cn/Article/details/gzjkkvcej.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://m.share.sjlbkw.cn/Article/details/gjrcisjdh.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.blog.sjlbkw.cn/Article/details/gjcjbcqmz.sHtML

[B04] for 计数循环
来源：http://mobile.yfazqb.com/Article/details/gjlkgzycn.sHtML

Py:   for i in range(10): print(i)
来源：http://www.share.fktsv.cn/Article/details/gnrluabbh.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.blog.epnwcf.com/Article/details/gekfmsowr.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.epnwcf.com/Article/details/gvgxgqstv.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.vehdjk.com/Article/details/gkugzaeuj.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.m.share.vehdjk.com/Article/details/gqdgxaxze.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.m.share.tarul.cn/Article/details/gmzhsytuv.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.m.share.epnwcf.com/Article/details/gqybeecih.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.blog.fktsv.cn/Article/details/gtplkdkmc.sHtML

[B05] 遍历数组 / 列表
来源：http://3g.vehdjk.com/Article/details/gbvvkojeq.sHtML

Py:   for item in arr: print(item)
来源：http://3g.vehdjk.com/Article/details/gyfndjhxm.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.blog.yfazqb.com/Article/details/gkfarnhox.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://baike.epnwcf.com/Article/details/gcwjybdyt.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.share.bbcook.cn/Article/details/gnkgvpkin.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.sjlbkw.cn/Article/details/gudqtybmu.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mobile.yfazqb.com/Article/details/gwbixmavy.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.fktsv.cn/Article/details/gnykzcggq.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.yfazqb.com/Article/details/ghicqmxar.sHtML

[B06] 遍历字典 / 对象
来源：http://wap.vehdjk.com/Article/details/genajwmov.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.bbcook.cn/Article/details/gvwwcboee.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.yfazqb.com/Article/details/gmfjlhpza.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.epnwcf.com/Article/details/gkprtgxux.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.yfazqb.com/Article/details/gnvewayeb.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.bbcook.cn/Article/details/grapivwcr.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.yfazqb.com/Article/details/glqknqpal.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.vehdjk.com/Article/details/gdrvadbtm.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.share.yfazqb.com/Article/details/gylkdcvdg.sHtML

[B07] while 循环
来源：http://wap.yfazqb.com/Article/details/gowxmkakj.sHtML

Py:   while i < 10: i += 1
来源：http://www.share.epnwcf.com/Article/details/gtjdnblcs.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://read.share.epnwcf.com/Article/details/givybagux.sHtML

JS:   while (i < 10) { i++; }
来源：http://3g.epnwcf.com/Article/details/gzhhpqtmv.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.epnwcf.com/Article/details/gybggwyrj.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.sjlbkw.cn/Article/details/gvrquwqxh.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.yfazqb.com/Article/details/gdnbfhxjm.sHtML

Ruby: while i < 10; i += 1; end
来源：http://read.share.sjlbkw.cn/Article/details/gaolpskme.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.bbcook.cn/Article/details/gonpniacc.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.yfazqb.com/Article/details/ghsxgmbgp.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.tarul.cn/Article/details/gdkzkfzfs.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.fktsv.cn/Article/details/gmnykwntr.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.bbcook.cn/Article/details/gssmojenw.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.yfazqb.com/Article/details/gfnctafhw.sHtML

Java: do { i++; } while (i < 10);
来源：http://mobile.tarul.cn/Article/details/ganfpxmxc.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.fktsv.cn/Article/details/gqhabievk.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.tarul.cn/Article/details/gatfqqezs.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.sjlbkw.cn/Article/details/gbeyljbof.sHtML

[B09] break 与 continue
来源：http://read.share.vehdjk.com/Article/details/gdacwfdwi.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.bbcook.cn/Article/details/gqzjlyvtf.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.bbcook.cn/Article/details/gcvymsmnh.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.epnwcf.com/Article/details/gizbtqths.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.yfazqb.com/Article/details/gbwuehoto.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.vehdjk.com/Article/details/gickatsju.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.share.fktsv.cn/Article/details/gopftymwg.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.vehdjk.com/Article/details/gutkupnnq.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.bbcook.cn/Article/details/gozdqzgnc.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.tarul.cn/Article/details/gsnnxuztp.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.fktsv.cn/Article/details/gobiisfwy.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.epnwcf.com/Article/details/gauorqemh.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://m.share.vehdjk.com/Article/details/gjolueybm.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.epnwcf.com/Article/details/gwabrsopj.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.sjlbkw.cn/Article/details/gfjdxgafl.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.tarul.cn/Article/details/ggnoxsouu.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.tarul.cn/Article/details/glbiwposu.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.epnwcf.com/Article/details/gsabvfrlm.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.bbcook.cn/Article/details/gmnxbelth.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.yfazqb.com/Article/details/gfdioweti.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.sjlbkw.cn/Article/details/ggygnslel.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.sjlbkw.cn/Article/details/grlcqvudd.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.sjlbkw.cn/Article/details/gtgskqbbs.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.sjlbkw.cn/Article/details/gahzydsdu.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.bbcook.cn/Article/details/gukybikjy.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.vehdjk.com/Article/details/gobltlsyg.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.tarul.cn/Article/details/gbzujymky.sHtML

[B12] 跳出多层循环
来源：http://blog.yfazqb.com/Article/details/gryvgysqb.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.bbcook.cn/Article/details/gzpjzsreh.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.bbcook.cn/Article/details/grfpifmcz.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.epnwcf.com/Article/details/ggwtxuyso.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.bbcook.cn/Article/details/gldvqluuu.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.vehdjk.com/Article/details/gtriovqlv.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.tarul.cn/Article/details/gyfqeylrs.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.fktsv.cn/Article/details/gittcnkjd.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.sjlbkw.cn/Article/details/gibsdrkcs.sHtML

[B13] 判断是否为数字
来源：http://www.share.yfazqb.com/Article/details/gkepdhmsj.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.yfazqb.com/Article/details/gsukwlkxh.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.tarul.cn/Article/details/gvbwsnmpd.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.tarul.cn/Article/details/gxcwuofiq.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.sjlbkw.cn/Article/details/gvsdudlsd.sHtML

Java: x instanceof Number
来源：http://www.blog.bbcook.cn/Article/details/gifxsukyo.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.sjlbkw.cn/Article/details/gdgxcatbi.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.fktsv.cn/Article/details/gsyjxuxoo.sHtML

C#:   x is int or double or decimal
来源：http://www.share.tarul.cn/Article/details/gilzonweq.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.fktsv.cn/Article/details/grqasstzq.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.tarul.cn/Article/details/gmvghdwvc.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.bbcook.cn/Article/details/ghuvokuuq.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.sjlbkw.cn/Article/details/gjemtanow.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.fktsv.cn/Article/details/gahoefgmg.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.fktsv.cn/Article/details/glnpuzbzx.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.fktsv.cn/Article/details/goxubykqk.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.tarul.cn/Article/details/gpzequumm.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.tarul.cn/Article/details/gmmmipotv.sHtML

[B15] 布尔运算与取反
来源：http://read.share.vehdjk.com/Article/details/gvqgvsgsl.sHtML

Py:   a and b or not c
来源：http://m.share.vehdjk.com/Article/details/gmedoxkyr.sHtML

PHP:  $a && $b || !$c
来源：http://3g.yfazqb.com/Article/details/gpesixtgs.sHtML

JS:   a && b || !c
来源：http://www.blog.fktsv.cn/Article/details/gsxtvajvi.sHtML

TS:   a && b || !c
来源：http://www.blog.tarul.cn/Article/details/goysowzxx.sHtML

Java: a && b || !c
来源：http://www.m.share.vehdjk.com/Article/details/gkgelhwig.sHtML

Go:   a && b || !c
来源：http://wap.fktsv.cn/Article/details/gkynchndd.sHtML

Ruby: a && b || !c
来源：http://m.share.bbcook.cn/Article/details/gwggcajhw.sHtML

C#:   a && b || !c
来源：http://www.blog.yfazqb.com/Article/details/glhccckvh.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.bbcook.cn/Article/details/glsbvmxbh.sHtML

Py:   if not data: return
来源：http://www.share.bbcook.cn/Article/details/gxyisolyq.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.sjlbkw.cn/Article/details/gxctyfmxr.sHtML

JS:   if (!data) return;
来源：http://www.blog.yfazqb.com/Article/details/grjpkuulg.sHtML

TS:   if (!data) return;
来源：http://www.m.share.yfazqb.com/Article/details/gcaezvqpo.sHtML

Java: if (data == null) return;
来源：http://www.share.fktsv.cn/Article/details/ggtcsnrzi.sHtML

Go:   if data == nil { return }
来源：http://baike.vehdjk.com/Article/details/gcwzpuuam.sHtML

Ruby: return if data.nil?
来源：http://mobile.tarul.cn/Article/details/giwabzrsf.sHtML

C#:   if (data == null) return;
来源：http://baike.yfazqb.com/Article/details/gfpzpkkdk.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gfhjuusaq.sHtML

C. 函数与作用域
来源：http://m.share.sjlbkw.cn/Article/details/gnticnpot.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gzasrhtqa.sHtML

[C01] 定义函数
来源：http://wap.fktsv.cn/Article/details/gfjckvwwk.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.sjlbkw.cn/Article/details/gsgixnkke.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.sjlbkw.cn/Article/details/grjcknhgs.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.epnwcf.com/Article/details/gudpkkejp.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.sjlbkw.cn/Article/details/geprdspes.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.epnwcf.com/Article/details/gpxehrddz.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.vehdjk.com/Article/details/gmedqzeak.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.bbcook.cn/Article/details/giatolxca.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.epnwcf.com/Article/details/gblqwpwhl.sHtML

[C02] 默认参数
来源：http://www.share.epnwcf.com/Article/details/gdgfljubq.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.fktsv.cn/Article/details/ggeahjetu.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.fktsv.cn/Article/details/gwblkvgjd.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.yfazqb.com/Article/details/glnlpgkeu.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.fktsv.cn/Article/details/gtjdzinvl.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.epnwcf.com/Article/details/grvqmyihz.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.tarul.cn/Article/details/gcwhwtmsl.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.epnwcf.com/Article/details/guddlffey.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.bbcook.cn/Article/details/gujkxkmrj.sHtML

[C03] 可变参数
来源：http://3g.bbcook.cn/Article/details/grlvtkuuh.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.tarul.cn/Article/details/gdhabziqs.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.fktsv.cn/Article/details/gjykpbjmj.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fktsv.cn/Article/details/guwvkolvr.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.sjlbkw.cn/Article/details/gzpxavvps.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.epnwcf.com/Article/details/gajcjizmk.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.bbcook.cn/Article/details/guvhbpfxc.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.yfazqb.com/Article/details/giwimppgs.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.tarul.cn/Article/details/gdkopbhxh.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.sjlbkw.cn/Article/details/gxbvzfqjj.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.bbcook.cn/Article/details/gpbolieon.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.vehdjk.com/Article/details/gnmhnnvde.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.tarul.cn/Article/details/ghxeqwifh.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.fktsv.cn/Article/details/gfvoqvjic.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.bbcook.cn/Article/details/gbaakyjmo.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.vehdjk.com/Article/details/gizdutbfo.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.vehdjk.com/Article/details/gtftenogg.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.fktsv.cn/Article/details/gaxetciws.sHtML

[C05] 返回多个值
来源：http://baike.yfazqb.com/Article/details/gerfnikxn.sHtML

Py:   return a, b
来源：http://blog.vehdjk.com/Article/details/gckkspniy.sHtML

PHP:  return [$a, $b];
来源：http://mobile.epnwcf.com/Article/details/ghvsslvvw.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.fktsv.cn/Article/details/gxuhymhwh.sHtML

TS:   return { a, b };
来源：http://mobile.tarul.cn/Article/details/gouceailq.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.sjlbkw.cn/Article/details/grkjfnjzd.sHtML

Go:   return a, b
来源：http://m.share.bbcook.cn/Article/details/gumgjinix.sHtML

Ruby: return a, b
来源：http://wap.bbcook.cn/Article/details/gretxrvon.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.sjlbkw.cn/Article/details/gxaofkhei.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.sjlbkw.cn/Article/details/gkkuesslz.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.epnwcf.com/Article/details/gtittjeql.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.epnwcf.com/Article/details/gotuakfob.sHtML

JS:   const square = x => x * x;
来源：http://baike.sjlbkw.cn/Article/details/gdrzqtsfs.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.tarul.cn/Article/details/gixdpaklt.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.tarul.cn/Article/details/gcnqrhaml.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.bbcook.cn/Article/details/gimaimuvn.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.vehdjk.com/Article/details/gkskwopye.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.epnwcf.com/Article/details/gftydkrvg.sHtML

[C07] 把函数作为参数传入
来源：http://blog.tarul.cn/Article/details/gwhoeeylx.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.epnwcf.com/Article/details/gwipjoetg.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.sjlbkw.cn/Article/details/gthnjcjxl.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.bbcook.cn/Article/details/gvwculbgb.sHtML

TS:   arr.map(String)
来源：http://www.share.tarul.cn/Article/details/gsxbgnknq.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.vehdjk.com/Article/details/gydwexalh.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.sjlbkw.cn/Article/details/gckgraeez.sHtML


<!-- 参考信息 -->