代发 wailian999

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.bbcook.cn/Article/details/gyturqhye.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.m.share.tarul.cn/Article/details/ggeasofvt.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.tarul.cn/Article/details/gvtixqvmd.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wap.tarul.cn/Article/details/gwsdshqtc.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.tarul.cn/Article/details/guiwultgd.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://m.share.fktsv.cn/Article/details/gfqtkkvto.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.yfazqb.com/Article/details/gljlnsbau.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.epnwcf.com/Article/details/gidrskmck.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.share.epnwcf.com/Article/details/gjdewpkfl.sHtML

Py:   ord("A"); chr(65)
来源：http://mobile.tarul.cn/Article/details/gderqqrdf.sHtML

PHP:  ord("A"); chr(65)
来源：http://read.share.yfazqb.com/Article/details/gqdnwbxdj.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.epnwcf.com/Article/details/gvagszqjh.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.sjlbkw.cn/Article/details/glyhfnhtb.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.m.share.bbcook.cn/Article/details/gxqrbyrbe.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://baike.yfazqb.com/Article/details/gydmrglyt.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.blog.yfazqb.com/Article/details/gwakzcptj.sHtML

C#:   (int)'A'; (char)65
来源：http://www.m.share.yfazqb.com/Article/details/gswvcfxoi.sHtML

[A19] 交换两个变量
来源：http://m.share.fktsv.cn/Article/details/grvnozspp.sHtML

Py:   a, b = b, a
来源：http://m.share.yfazqb.com/Article/details/gxjqjmlee.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://blog.tarul.cn/Article/details/goxkayccs.sHtML

JS:   [a, b] = [b, a];
来源：http://www.m.share.sjlbkw.cn/Article/details/gcfrqttnk.sHtML

TS:   [a, b] = [b, a];
来源：http://baike.vehdjk.com/Article/details/gvzbyduxs.sHtML

Java: int t = a; a = b; b = t;
来源：http://baike.sjlbkw.cn/Article/details/gcwvkpzvq.sHtML

Go:   a, b = b, a
来源：http://mobile.fktsv.cn/Article/details/gowffqgxj.sHtML

Ruby: a, b = b, a
来源：http://www.m.share.tarul.cn/Article/details/ghaljwasj.sHtML

C#:   (a, b) = (b, a);
来源：http://3g.bbcook.cn/Article/details/gtusskutq.sHtML

[A20] 读取标准输入
来源：http://www.blog.fktsv.cn/Article/details/grlwtpshk.sHtML

Py:   name = input("请输入：")
来源：http://www.blog.fktsv.cn/Article/details/giybdqfyw.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://3g.tarul.cn/Article/details/gjcgvstoh.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://m.share.fktsv.cn/Article/details/gnygvlfes.sHtML

TS:   // Node.js：readline 模块
来源：http://m.share.epnwcf.com/Article/details/gqkyxtkom.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.m.share.yfazqb.com/Article/details/gxvtscspl.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.share.bbcook.cn/Article/details/gjeahboak.sHtML

Ruby: gets.chomp
来源：http://read.share.bbcook.cn/Article/details/gytsafhac.sHtML

C#:   Console.ReadLine();
来源：http://read.share.yfazqb.com/Article/details/gojktzgfv.sHtML

[A21] 保留指定小数位输出
来源：http://wap.vehdjk.com/Article/details/gbosahxzy.sHtML

Py:   f"{3.14159:.2f}"
来源：http://mobile.epnwcf.com/Article/details/glidfysag.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://read.share.vehdjk.com/Article/details/gjpgdevej.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.blog.sjlbkw.cn/Article/details/gzyzfzxng.sHtML

TS:   (3.14159).toFixed(2)
来源：http://wap.vehdjk.com/Article/details/gjbqybljx.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://mobile.bbcook.cn/Article/details/gpqvuyqny.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.m.share.sjlbkw.cn/Article/details/guomesvxt.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://mobile.fktsv.cn/Article/details/gmhwbnnum.sHtML

C#:   3.14159.ToString("F2")
来源：http://m.share.fktsv.cn/Article/details/gzwuyzpkk.sHtML

[A22] 获取字符串长度
来源：http://mobile.tarul.cn/Article/details/glgqsjbjw.sHtML

Py:   len(s)
来源：http://wap.vehdjk.com/Article/details/gwywrhtlf.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://baike.yfazqb.com/Article/details/gnigkhmel.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.blog.fktsv.cn/Article/details/gssekzmmw.sHtML

TS:   s.length
来源：http://blog.yfazqb.com/Article/details/grfokttna.sHtML

Java: s.length()
来源：http://wap.fktsv.cn/Article/details/gojgibmpk.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://blog.yfazqb.com/Article/details/grmwkzfnd.sHtML

Ruby: s.length
来源：http://read.share.fktsv.cn/Article/details/geefyjjke.sHtML

C#:   s.Length
来源：http://www.m.share.epnwcf.com/Article/details/gjfxtdhoj.sHtML

[A23] 大小写转换
来源：http://m.share.fktsv.cn/Article/details/gipeacbbr.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://wap.fktsv.cn/Article/details/gdppkzgyd.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.share.fktsv.cn/Article/details/gjensrsrz.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.epnwcf.com/Article/details/gcmkymulk.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.tarul.cn/Article/details/ggpnyqrtb.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wap.vehdjk.com/Article/details/ghrmpdwiu.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://read.share.yfazqb.com/Article/details/gubhyptbo.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.blog.bbcook.cn/Article/details/gkxxpnscm.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://read.share.vehdjk.com/Article/details/gsknwbgos.sHtML

[A24] 去除首尾空白
来源：http://read.share.fktsv.cn/Article/details/gkjeuqohq.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://3g.fktsv.cn/Article/details/gpqgugofz.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://3g.yfazqb.com/Article/details/gsfqkiugn.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.bbcook.cn/Article/details/gmtgvaxcm.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.vehdjk.com/Article/details/glvoevdev.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://blog.tarul.cn/Article/details/gzxtixiez.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.m.share.epnwcf.com/Article/details/guhpddfdm.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wap.fktsv.cn/Article/details/giuempzft.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://read.share.bbcook.cn/Article/details/gpiqtzmsv.sHtML

[A25] 字符串比较
来源：http://read.share.vehdjk.com/Article/details/gwzrtxqqj.sHtML

Py:   s1 == s2; s1 != s2
来源：http://blog.fktsv.cn/Article/details/gfqmoavzh.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wap.bbcook.cn/Article/details/gmzvwcftc.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.epnwcf.com/Article/details/gezjflxbm.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.yfazqb.com/Article/details/gspqgcuaf.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.share.yfazqb.com/Article/details/gvdlecfnp.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://baike.fktsv.cn/Article/details/gxbjpllzc.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://wap.yfazqb.com/Article/details/gfoajdbhh.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mobile.epnwcf.com/Article/details/gspbrsjwo.sHtML

[A26] 类型转换总览
来源：http://baike.yfazqb.com/Article/details/geehgsgng.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.m.share.fktsv.cn/Article/details/gqcyawbzw.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wap.bbcook.cn/Article/details/gjjdppqut.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.m.share.sjlbkw.cn/Article/details/gbblogojo.sHtML

TS:   Number() String() Boolean() x as number
来源：http://mobile.yfazqb.com/Article/details/gyayxjdny.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://blog.vehdjk.com/Article/details/gmqkfyhsm.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.m.share.sjlbkw.cn/Article/details/ghpncarhj.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://m.share.vehdjk.com/Article/details/gxedgxetp.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.blog.vehdjk.com/Article/details/gemvmrsfx.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gowxmzbem.sHtML

B. 流程控制
来源：http://www.blog.vehdjk.com/Article/details/gyiarvbcp.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/geuymkrqn.sHtML

[B01] 条件判断 if / else
来源：http://m.share.fktsv.cn/Article/details/giglysoio.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://baike.epnwcf.com/Article/details/gedjowzjd.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mobile.fktsv.cn/Article/details/gzywnuzss.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.bbcook.cn/Article/details/gztzkogyk.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.vehdjk.com/Article/details/guheixjpy.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://m.share.epnwcf.com/Article/details/gmmdohxlp.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://baike.sjlbkw.cn/Article/details/gpadugotz.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.m.share.fktsv.cn/Article/details/gxlygawkf.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://m.share.sjlbkw.cn/Article/details/gnzlthtqf.sHtML

[B02] 多分支 else if / elif
来源：http://www.blog.vehdjk.com/Article/details/gzxujwpet.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://blog.fktsv.cn/Article/details/gblcykbjz.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://m.share.tarul.cn/Article/details/gurvoeysd.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.yfazqb.com/Article/details/gjdwqdjja.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.yfazqb.com/Article/details/ghtvxqjqd.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.epnwcf.com/Article/details/gitankmqh.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mobile.epnwcf.com/Article/details/gjdjfccat.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://read.share.vehdjk.com/Article/details/gpzuqukic.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.bbcook.cn/Article/details/gmlmwustk.sHtML

[B03] switch / match / case
来源：http://m.share.yfazqb.com/Article/details/gqmrqwezj.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mobile.epnwcf.com/Article/details/gtggsvntb.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://baike.tarul.cn/Article/details/ghgevykkd.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gujwyxorl.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.bbcook.cn/Article/details/ggzjfzwfh.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://baike.vehdjk.com/Article/details/gtbavooup.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://blog.epnwcf.com/Article/details/gzvrbvvwe.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://baike.bbcook.cn/Article/details/glbdkhswk.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://read.share.sjlbkw.cn/Article/details/gsukmsktn.sHtML

[B04] for 计数循环
来源：http://mobile.tarul.cn/Article/details/gucngvhgt.sHtML

Py:   for i in range(10): print(i)
来源：http://3g.vehdjk.com/Article/details/gvxvnjcqj.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.blog.yfazqb.com/Article/details/genrczgdg.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.epnwcf.com/Article/details/govtjirkh.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.fktsv.cn/Article/details/gglzgoyqn.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://m.share.tarul.cn/Article/details/gvwdkgnqz.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://read.share.vehdjk.com/Article/details/gxypfsbii.sHtML

Ruby: 10.times { |i| puts i }
来源：http://3g.bbcook.cn/Article/details/gtrrytjwi.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.blog.tarul.cn/Article/details/gwobbwfot.sHtML

[B05] 遍历数组 / 列表
来源：http://read.share.yfazqb.com/Article/details/gonxpkzto.sHtML

Py:   for item in arr: print(item)
来源：http://www.share.vehdjk.com/Article/details/gtdritoge.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://m.share.fktsv.cn/Article/details/gabvhbvqx.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://baike.tarul.cn/Article/details/gxygqyrrv.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://blog.epnwcf.com/Article/details/gxkdyagmm.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://mobile.epnwcf.com/Article/details/gkzpysszy.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://m.share.fktsv.cn/Article/details/glylvymch.sHtML

Ruby: arr.each { |item| puts item }
来源：http://m.share.vehdjk.com/Article/details/gffztpcrm.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://baike.yfazqb.com/Article/details/gelwznuoh.sHtML

[B06] 遍历字典 / 对象
来源：http://baike.sjlbkw.cn/Article/details/gnwzsvnmj.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://3g.fktsv.cn/Article/details/grzleqsex.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://m.share.sjlbkw.cn/Article/details/gfvgvdotx.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.tarul.cn/Article/details/gappzghkp.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.fktsv.cn/Article/details/gbhrnsahy.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.bbcook.cn/Article/details/glerpkaur.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.vehdjk.com/Article/details/gxpamugps.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://m.share.bbcook.cn/Article/details/gkfmtiupb.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.yfazqb.com/Article/details/gzcqhdyzi.sHtML

[B07] while 循环
来源：http://wap.vehdjk.com/Article/details/glpfjeyel.sHtML

Py:   while i < 10: i += 1
来源：http://baike.epnwcf.com/Article/details/grgslpwpz.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.bbcook.cn/Article/details/gxtdaeezm.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.vehdjk.com/Article/details/gkeqvbyuu.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.sjlbkw.cn/Article/details/gfqlwjqns.sHtML

Java: while (i < 10) { i++; }
来源：http://wap.vehdjk.com/Article/details/gdarsdfgd.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.sjlbkw.cn/Article/details/gfgnofkrq.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.fktsv.cn/Article/details/gaodrcwyc.sHtML

C#:   while (i < 10) { i++; }
来源：http://m.share.tarul.cn/Article/details/ggpdfmwfb.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.bbcook.cn/Article/details/gsdgrhsnx.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.share.bbcook.cn/Article/details/guwgdiqzp.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.tarul.cn/Article/details/gwlqulzgu.sHtML

JS:   do { i++; } while (i < 10);
来源：http://3g.sjlbkw.cn/Article/details/grbdvfxhz.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.tarul.cn/Article/details/gnerpeyit.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.sjlbkw.cn/Article/details/gnalqgdrs.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.yfazqb.com/Article/details/gnyicclki.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://read.share.fktsv.cn/Article/details/gpcusnfgi.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.epnwcf.com/Article/details/gqjknodls.sHtML

[B09] break 与 continue
来源：http://3g.vehdjk.com/Article/details/gpjywohqv.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.yfazqb.com/Article/details/ggngwdmzh.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.yfazqb.com/Article/details/gkixlwgrr.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gxefestbm.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fktsv.cn/Article/details/giivocsnq.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.vehdjk.com/Article/details/gderfqlzo.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.yfazqb.com/Article/details/gsgyqakls.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.vehdjk.com/Article/details/gbeinpzfu.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.epnwcf.com/Article/details/guaqqjuuv.sHtML

[B10] 遍历同时拿索引
来源：http://blog.vehdjk.com/Article/details/gweqnlfig.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.yfazqb.com/Article/details/gdiseurlq.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.yfazqb.com/Article/details/ghaenztfr.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.vehdjk.com/Article/details/gkbotcsul.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.sjlbkw.cn/Article/details/gutjyiepi.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.yfazqb.com/Article/details/gtnfkapnp.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.fktsv.cn/Article/details/gmnlrojdo.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.tarul.cn/Article/details/gfqxbvedk.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.tarul.cn/Article/details/gjszjwadq.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.vehdjk.com/Article/details/gldzppmlp.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.yfazqb.com/Article/details/gcgxbsdwt.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.sjlbkw.cn/Article/details/gfkvbfxkl.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.fktsv.cn/Article/details/gwioqhcks.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.yfazqb.com/Article/details/goynahuop.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.fktsv.cn/Article/details/gbthizhjz.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.yfazqb.com/Article/details/gccmmxowt.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.bbcook.cn/Article/details/gwrnqtjug.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.sjlbkw.cn/Article/details/gjdqezouj.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.sjlbkw.cn/Article/details/gssfmxabs.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.vehdjk.com/Article/details/gbcuxmhkx.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.vehdjk.com/Article/details/ghpzvtysq.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.yfazqb.com/Article/details/gcmbonqoj.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.yfazqb.com/Article/details/glruemixg.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.bbcook.cn/Article/details/gkagxseqo.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.vehdjk.com/Article/details/gndlzicqp.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.vehdjk.com/Article/details/gdilpjpgg.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.fktsv.cn/Article/details/glawxhuhs.sHtML

[B13] 判断是否为数字
来源：http://www.share.yfazqb.com/Article/details/gejxgwmqo.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.vehdjk.com/Article/details/gjieirirv.sHtML

PHP:  is_numeric($x)
来源：http://blog.vehdjk.com/Article/details/geugltjgd.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.tarul.cn/Article/details/gavwvjqzu.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.sjlbkw.cn/Article/details/ggfygpems.sHtML

Java: x instanceof Number
来源：http://read.share.fktsv.cn/Article/details/gcctxfnkr.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.epnwcf.com/Article/details/ghflwdnqj.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.vehdjk.com/Article/details/gpevnwrun.sHtML

C#:   x is int or double or decimal
来源：http://wap.epnwcf.com/Article/details/givqftzkd.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.yfazqb.com/Article/details/gseuldnli.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.sjlbkw.cn/Article/details/gasyrinwl.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.vehdjk.com/Article/details/gkqvfncak.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.fktsv.cn/Article/details/gjfeoijpc.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.vehdjk.com/Article/details/gubqkzfjo.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.epnwcf.com/Article/details/gjnxdtwng.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.vehdjk.com/Article/details/gskaebwkh.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.epnwcf.com/Article/details/gnoaoiabh.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.vehdjk.com/Article/details/grttckjtx.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.fktsv.cn/Article/details/gmmvyzaow.sHtML

Py:   a and b or not c
来源：http://m.share.vehdjk.com/Article/details/gfanjmlzm.sHtML

PHP:  $a && $b || !$c
来源：http://blog.yfazqb.com/Article/details/gjgehnsge.sHtML

JS:   a && b || !c
来源：http://mobile.vehdjk.com/Article/details/gbklvetuv.sHtML

TS:   a && b || !c
来源：http://www.share.fktsv.cn/Article/details/gloaigkku.sHtML

Java: a && b || !c
来源：http://baike.sjlbkw.cn/Article/details/guyetvzpo.sHtML

Go:   a && b || !c
来源：http://blog.bbcook.cn/Article/details/gzokiajhy.sHtML

Ruby: a && b || !c
来源：http://read.share.epnwcf.com/Article/details/gmmofluic.sHtML

C#:   a && b || !c
来源：http://www.m.share.epnwcf.com/Article/details/gmmdkzcjk.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.bbcook.cn/Article/details/gpltlwsrv.sHtML

Py:   if not data: return
来源：http://wap.tarul.cn/Article/details/gyvgguamm.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.yfazqb.com/Article/details/gjbiqwdkl.sHtML

JS:   if (!data) return;
来源：http://www.blog.fktsv.cn/Article/details/gizflyenb.sHtML

TS:   if (!data) return;
来源：http://baike.vehdjk.com/Article/details/gbmztgibr.sHtML

Java: if (data == null) return;
来源：http://3g.yfazqb.com/Article/details/gvkhotnbz.sHtML

Go:   if data == nil { return }
来源：http://www.blog.yfazqb.com/Article/details/gcgntmmzm.sHtML

Ruby: return if data.nil?
来源：http://3g.sjlbkw.cn/Article/details/gczcjkjta.sHtML

C#:   if (data == null) return;
来源：http://mobile.epnwcf.com/Article/details/gzkdckpzf.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gqgtzicno.sHtML

C. 函数与作用域
来源：http://baike.epnwcf.com/Article/details/gjgdfrndw.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gpobypblx.sHtML

[C01] 定义函数
来源：http://mobile.bbcook.cn/Article/details/gfogkgdse.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.sjlbkw.cn/Article/details/gmzjmvwib.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.tarul.cn/Article/details/goydgvwee.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.fktsv.cn/Article/details/gusipvicr.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.sjlbkw.cn/Article/details/glxiaodlr.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.epnwcf.com/Article/details/gtuegmgri.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.yfazqb.com/Article/details/gjblgmihw.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.bbcook.cn/Article/details/gxkcvltxp.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.bbcook.cn/Article/details/gpuqhjiob.sHtML

[C02] 默认参数
来源：http://www.blog.tarul.cn/Article/details/gkdjhcfzr.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.bbcook.cn/Article/details/gymicppfq.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.fktsv.cn/Article/details/gfqyawuwb.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.bbcook.cn/Article/details/gwbswdynt.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.sjlbkw.cn/Article/details/gfyatqchc.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.vehdjk.com/Article/details/gdsuyentg.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.epnwcf.com/Article/details/gsjyeidqj.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.fktsv.cn/Article/details/gqtqrawdm.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.yfazqb.com/Article/details/gmkdzqxiv.sHtML

[C03] 可变参数
来源：http://wap.fktsv.cn/Article/details/gdvezxozz.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.bbcook.cn/Article/details/gmtjsdwwd.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.epnwcf.com/Article/details/ggsclafcv.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.yfazqb.com/Article/details/gsmuiobgo.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.sjlbkw.cn/Article/details/gxbvkqmpj.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.sjlbkw.cn/Article/details/gxoeynbzh.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.fktsv.cn/Article/details/ggieqakmc.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.sjlbkw.cn/Article/details/gvjusamsj.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.fktsv.cn/Article/details/gphkyvpgm.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.epnwcf.com/Article/details/glmoytpsa.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.yfazqb.com/Article/details/gvyokanqr.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.fktsv.cn/Article/details/gjwolulmt.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.tarul.cn/Article/details/gcebefmiy.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.sjlbkw.cn/Article/details/gnzhzmina.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.vehdjk.com/Article/details/ghdirqleo.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.bbcook.cn/Article/details/gvngpgwim.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.sjlbkw.cn/Article/details/gdlyvrxhx.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.tarul.cn/Article/details/gvdupuxjs.sHtML

[C05] 返回多个值
来源：http://baike.vehdjk.com/Article/details/geabrocpf.sHtML

Py:   return a, b
来源：http://mobile.sjlbkw.cn/Article/details/gvhpnrrjv.sHtML

PHP:  return [$a, $b];
来源：http://mobile.epnwcf.com/Article/details/gqhyhpnvl.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.sjlbkw.cn/Article/details/guishwkpb.sHtML

TS:   return { a, b };
来源：http://www.blog.bbcook.cn/Article/details/goxhgubop.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.sjlbkw.cn/Article/details/ggvawnxmx.sHtML

Go:   return a, b
来源：http://blog.bbcook.cn/Article/details/gfuhfzcpo.sHtML

Ruby: return a, b
来源：http://baike.epnwcf.com/Article/details/gyyoclymi.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.sjlbkw.cn/Article/details/gpseabrql.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.epnwcf.com/Article/details/gfnxofjvj.sHtML

Py:   square = lambda x: x * x
来源：http://wap.vehdjk.com/Article/details/gotsyikhj.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.yfazqb.com/Article/details/gyiiymmfg.sHtML

JS:   const square = x => x * x;
来源：http://wap.epnwcf.com/Article/details/gaemepkyn.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.sjlbkw.cn/Article/details/geadveixu.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.fktsv.cn/Article/details/gvthhugkf.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.yfazqb.com/Article/details/gkrpdunai.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.tarul.cn/Article/details/ghwfhdxoc.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.tarul.cn/Article/details/gnocxxxsw.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.vehdjk.com/Article/details/gzfeicpub.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.tarul.cn/Article/details/gdvxgxufx.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.sjlbkw.cn/Article/details/gykpzuygn.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.sjlbkw.cn/Article/details/gkdfgdlgx.sHtML

TS:   arr.map(String)
来源：http://m.share.sjlbkw.cn/Article/details/glhxwsfgx.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.tarul.cn/Article/details/gifjxqzpy.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.yfazqb.com/Article/details/gxjfctjqw.sHtML


<!-- 参考信息 -->