代发 wailian999

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.vehdjk.com/Article/details/guvnypaxf.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wap.fktsv.cn/Article/details/giaslbtax.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.sjlbkw.cn/Article/details/gszqhcnex.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.epnwcf.com/Article/details/gthqhqmpa.sHtML

[A18] 字符与 ASCII 码互转
来源：http://read.share.fktsv.cn/Article/details/gdntntdfo.sHtML

Py:   ord("A"); chr(65)
来源：http://mobile.tarul.cn/Article/details/griumjjro.sHtML

PHP:  ord("A"); chr(65)
来源：http://baike.bbcook.cn/Article/details/giqideohb.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.vehdjk.com/Article/details/gwybvyrkj.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://read.share.vehdjk.com/Article/details/gtigplvyw.sHtML

Java: (int) 'A'; (char) 65
来源：http://baike.yfazqb.com/Article/details/gpseiwjuq.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://m.share.epnwcf.com/Article/details/gsbqsobdm.sHtML

Ruby: "A".ord; 65.chr
来源：http://3g.vehdjk.com/Article/details/gkaizfwzj.sHtML

C#:   (int)'A'; (char)65
来源：http://www.share.tarul.cn/Article/details/gpsdvemuj.sHtML

[A19] 交换两个变量
来源：http://baike.bbcook.cn/Article/details/gvtjzrvxh.sHtML

Py:   a, b = b, a
来源：http://m.share.bbcook.cn/Article/details/gqeeorlsn.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.share.yfazqb.com/Article/details/gcfamjbko.sHtML

JS:   [a, b] = [b, a];
来源：http://www.blog.tarul.cn/Article/details/gttqpjfzf.sHtML

TS:   [a, b] = [b, a];
来源：http://baike.yfazqb.com/Article/details/gpmjrtnsu.sHtML

Java: int t = a; a = b; b = t;
来源：http://3g.yfazqb.com/Article/details/gtbkimpuo.sHtML

Go:   a, b = b, a
来源：http://baike.sjlbkw.cn/Article/details/gxxywzwrl.sHtML

Ruby: a, b = b, a
来源：http://m.share.yfazqb.com/Article/details/gjmsyjbcv.sHtML

C#:   (a, b) = (b, a);
来源：http://mobile.tarul.cn/Article/details/gmxjvzuoh.sHtML

[A20] 读取标准输入
来源：http://3g.yfazqb.com/Article/details/gauszncbq.sHtML

Py:   name = input("请输入：")
来源：http://baike.sjlbkw.cn/Article/details/ginsvlint.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://read.share.bbcook.cn/Article/details/gwmfbuxju.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://m.share.sjlbkw.cn/Article/details/gnbvvmmxr.sHtML

TS:   // Node.js：readline 模块
来源：http://www.share.vehdjk.com/Article/details/gzyjtmaqq.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.m.share.epnwcf.com/Article/details/gxabwqmoo.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://3g.tarul.cn/Article/details/gnjusfpsp.sHtML

Ruby: gets.chomp
来源：http://baike.fktsv.cn/Article/details/gsumwpnjy.sHtML

C#:   Console.ReadLine();
来源：http://www.m.share.bbcook.cn/Article/details/gdzqjburi.sHtML

[A21] 保留指定小数位输出
来源：http://www.blog.tarul.cn/Article/details/gkplxykxv.sHtML

Py:   f"{3.14159:.2f}"
来源：http://read.share.tarul.cn/Article/details/grsrapcuk.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wap.epnwcf.com/Article/details/glsdxqkov.sHtML

JS:   (3.14159).toFixed(2)
来源：http://m.share.epnwcf.com/Article/details/gnijcipgg.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.share.yfazqb.com/Article/details/gxphoifqi.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://read.share.yfazqb.com/Article/details/ggzyxayiy.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://m.share.fktsv.cn/Article/details/gbaqtijbz.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.share.vehdjk.com/Article/details/gbvtfybgn.sHtML

C#:   3.14159.ToString("F2")
来源：http://m.share.yfazqb.com/Article/details/ggpcmyflz.sHtML

[A22] 获取字符串长度
来源：http://baike.vehdjk.com/Article/details/gmltefupk.sHtML

Py:   len(s)
来源：http://mobile.sjlbkw.cn/Article/details/gupcmxnkt.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://read.share.bbcook.cn/Article/details/gcbxlgnha.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://read.share.vehdjk.com/Article/details/gksnwmitd.sHtML

TS:   s.length
来源：http://www.share.bbcook.cn/Article/details/gbkhqwxlx.sHtML

Java: s.length()
来源：http://m.share.yfazqb.com/Article/details/gbvluctai.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://3g.vehdjk.com/Article/details/gzqwbihcf.sHtML

Ruby: s.length
来源：http://mobile.tarul.cn/Article/details/gndqllpiz.sHtML

C#:   s.Length
来源：http://mobile.yfazqb.com/Article/details/gdkvvnota.sHtML

[A23] 大小写转换
来源：http://blog.tarul.cn/Article/details/gfrwjiiij.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://3g.epnwcf.com/Article/details/gogvmweeg.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://3g.epnwcf.com/Article/details/gddbzewgi.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.bbcook.cn/Article/details/gflgqattv.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.yfazqb.com/Article/details/ggvkmjbtc.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://m.share.bbcook.cn/Article/details/gshpnmhux.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.m.share.vehdjk.com/Article/details/gjgkzftro.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wap.fktsv.cn/Article/details/gjleugdjp.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://blog.bbcook.cn/Article/details/gqouoqrfl.sHtML

[A24] 去除首尾空白
来源：http://www.blog.vehdjk.com/Article/details/gskcekopt.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.blog.yfazqb.com/Article/details/gjjwlogcu.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.blog.epnwcf.com/Article/details/gyutaxfww.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.fktsv.cn/Article/details/giwwlfiis.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.bbcook.cn/Article/details/gbbusfpty.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.m.share.bbcook.cn/Article/details/gennmsqfb.sHtML

Go:   strings.TrimSpace(s)
来源：http://3g.epnwcf.com/Article/details/grvnfgccy.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wap.sjlbkw.cn/Article/details/gwlrzjati.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://blog.yfazqb.com/Article/details/grjuvmbih.sHtML

[A25] 字符串比较
来源：http://baike.sjlbkw.cn/Article/details/gwjyqhnbk.sHtML

Py:   s1 == s2; s1 != s2
来源：http://baike.vehdjk.com/Article/details/grfmsbrvm.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.m.share.yfazqb.com/Article/details/gmakitxkx.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.yfazqb.com/Article/details/gmmsrlwbe.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.tarul.cn/Article/details/ggymyvobb.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://blog.epnwcf.com/Article/details/gudgzogfp.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://m.share.vehdjk.com/Article/details/gmufxajus.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://read.share.yfazqb.com/Article/details/gqmpfyjzg.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mobile.sjlbkw.cn/Article/details/ghrijukuk.sHtML

[A26] 类型转换总览
来源：http://read.share.bbcook.cn/Article/details/guzpegecu.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wap.sjlbkw.cn/Article/details/gzeuojqtj.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://m.share.fktsv.cn/Article/details/gccmbggso.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://blog.tarul.cn/Article/details/gnfndzhqb.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.blog.sjlbkw.cn/Article/details/gkjkuisph.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://m.share.fktsv.cn/Article/details/goycoogrw.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wap.yfazqb.com/Article/details/gkogpxcrh.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://3g.sjlbkw.cn/Article/details/gulyqzggb.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://baike.sjlbkw.cn/Article/details/gykypbvyl.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gcqjdoiqr.sHtML

B. 流程控制
来源：http://blog.yfazqb.com/Article/details/glzfaipqe.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gxzkihfvw.sHtML

[B01] 条件判断 if / else
来源：http://baike.tarul.cn/Article/details/gkyuzgztz.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://mobile.bbcook.cn/Article/details/gvjvcbfnp.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://blog.sjlbkw.cn/Article/details/gkbjbmrxj.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.epnwcf.com/Article/details/gtxvmrzkd.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.tarul.cn/Article/details/gezgpmvny.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://mobile.bbcook.cn/Article/details/gtndayfhj.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://blog.yfazqb.com/Article/details/gkuievnna.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mobile.epnwcf.com/Article/details/gtipfjovl.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.share.tarul.cn/Article/details/gtlgotiht.sHtML

[B02] 多分支 else if / elif
来源：http://3g.bbcook.cn/Article/details/ggqafuwug.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.share.tarul.cn/Article/details/gaqabdpvi.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://blog.vehdjk.com/Article/details/gajocyerv.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.vehdjk.com/Article/details/gfahqqpqx.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.yfazqb.com/Article/details/grmwnihqz.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.vehdjk.com/Article/details/gbzewkrpa.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.share.fktsv.cn/Article/details/gvqkuovmy.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.m.share.epnwcf.com/Article/details/gzfnyjete.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.bbcook.cn/Article/details/gznmeqfso.sHtML

[B03] switch / match / case
来源：http://blog.bbcook.cn/Article/details/gwjdjihxn.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://3g.yfazqb.com/Article/details/ghvhutofx.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://baike.yfazqb.com/Article/details/gzsklurpu.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.epnwcf.com/Article/details/ggphafzvz.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.bbcook.cn/Article/details/gkzowkewg.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://baike.tarul.cn/Article/details/getzmzdxf.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.blog.yfazqb.com/Article/details/goocnpzjs.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wap.bbcook.cn/Article/details/ghixwgnzk.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://blog.vehdjk.com/Article/details/gwrtrcsbp.sHtML

[B04] for 计数循环
来源：http://3g.epnwcf.com/Article/details/ghtgkjxqn.sHtML

Py:   for i in range(10): print(i)
来源：http://blog.epnwcf.com/Article/details/gwavnpskm.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wap.vehdjk.com/Article/details/gwluelvmv.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.vehdjk.com/Article/details/gtyatdqld.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.yfazqb.com/Article/details/ggkcszrao.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mobile.vehdjk.com/Article/details/gngcxldnz.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://3g.fktsv.cn/Article/details/goyasfusm.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.m.share.epnwcf.com/Article/details/gzdhqkizb.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://3g.bbcook.cn/Article/details/getlntysp.sHtML

[B05] 遍历数组 / 列表
来源：http://blog.tarul.cn/Article/details/gmvqdjkqq.sHtML

Py:   for item in arr: print(item)
来源：http://www.m.share.sjlbkw.cn/Article/details/gxjhhjabb.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.vehdjk.com/Article/details/gsaikkwyh.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.tarul.cn/Article/details/gzfsqgspk.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://read.share.epnwcf.com/Article/details/grglmmnpg.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://mobile.sjlbkw.cn/Article/details/geuyrxwop.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mobile.bbcook.cn/Article/details/glhlogrqx.sHtML

Ruby: arr.each { |item| puts item }
来源：http://m.share.epnwcf.com/Article/details/gphpwdfqv.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://read.share.bbcook.cn/Article/details/guhudhodp.sHtML

[B06] 遍历字典 / 对象
来源：http://blog.tarul.cn/Article/details/gdglnldwh.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://m.share.bbcook.cn/Article/details/gvzaeulbk.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mobile.sjlbkw.cn/Article/details/gczvknpbw.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.yfazqb.com/Article/details/gviaysnxg.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.epnwcf.com/Article/details/gctgphcop.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://blog.sjlbkw.cn/Article/details/grkqaxkld.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wap.fktsv.cn/Article/details/gwygfmxzk.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://read.share.fktsv.cn/Article/details/gfbayqjvf.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://m.share.epnwcf.com/Article/details/gtyaznyvs.sHtML

[B07] while 循环
来源：http://wap.epnwcf.com/Article/details/gpeyiedqb.sHtML

Py:   while i < 10: i += 1
来源：http://mobile.tarul.cn/Article/details/gdjrgbhwe.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.epnwcf.com/Article/details/goxstijiy.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.blog.bbcook.cn/Article/details/gizqtrwto.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.fktsv.cn/Article/details/gmptzbzsw.sHtML

Java: while (i < 10) { i++; }
来源：http://baike.vehdjk.com/Article/details/gnpiyjtfb.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wap.fktsv.cn/Article/details/ghgvyigzs.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.tarul.cn/Article/details/gnztbvlzx.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.epnwcf.com/Article/details/gsmvpongc.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.vehdjk.com/Article/details/glcteygsc.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://mobile.bbcook.cn/Article/details/gfpwguzqg.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.epnwcf.com/Article/details/ghznmyqdl.sHtML

JS:   do { i++; } while (i < 10);
来源：http://baike.epnwcf.com/Article/details/gkpwtsfmy.sHtML

TS:   do { i++; } while (i < 10);
来源：http://3g.bbcook.cn/Article/details/giyuslksy.sHtML

Java: do { i++; } while (i < 10);
来源：http://mobile.yfazqb.com/Article/details/gznkymgvy.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://m.share.vehdjk.com/Article/details/gfttlhpob.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.yfazqb.com/Article/details/gbjdgrmvx.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.epnwcf.com/Article/details/gogmiimoq.sHtML

[B09] break 与 continue
来源：http://m.share.vehdjk.com/Article/details/gydjthdox.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.sjlbkw.cn/Article/details/gxuvjcdba.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.vehdjk.com/Article/details/gjotnfaak.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fktsv.cn/Article/details/guxuqhykj.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gyubvhrgf.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.tarul.cn/Article/details/gaxpzucyr.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.epnwcf.com/Article/details/gdjuxijdo.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.vehdjk.com/Article/details/glskvrzgx.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.sjlbkw.cn/Article/details/gfsrlprzo.sHtML

[B10] 遍历同时拿索引
来源：http://baike.sjlbkw.cn/Article/details/gybhkqszy.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.epnwcf.com/Article/details/gjcilbtpq.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.vehdjk.com/Article/details/geuzcxvyy.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.epnwcf.com/Article/details/gworhywcw.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.tarul.cn/Article/details/gvpiufpwh.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://3g.sjlbkw.cn/Article/details/gxnvpdrtc.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.tarul.cn/Article/details/gjrnsxxdq.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.bbcook.cn/Article/details/gilrfksmy.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.tarul.cn/Article/details/gjnmxicsd.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.sjlbkw.cn/Article/details/gcluaggiq.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.fktsv.cn/Article/details/gkpxyaumm.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.tarul.cn/Article/details/glpxdjqbr.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.tarul.cn/Article/details/gkjhamayp.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.fktsv.cn/Article/details/gdzqanyrz.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.epnwcf.com/Article/details/guesbwkat.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.fktsv.cn/Article/details/gmdqzjlue.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.tarul.cn/Article/details/gegrrvakj.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.fktsv.cn/Article/details/grmthhosv.sHtML

[B12] 跳出多层循环
来源：http://wap.yfazqb.com/Article/details/gdjmhnmzk.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.fktsv.cn/Article/details/gjpbjmupl.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.epnwcf.com/Article/details/gogmkuagc.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.fktsv.cn/Article/details/gtztuljql.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.bbcook.cn/Article/details/gkcgxnmbz.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.epnwcf.com/Article/details/gjdngaujc.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.sjlbkw.cn/Article/details/gtaufbess.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.bbcook.cn/Article/details/gincduiyy.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.yfazqb.com/Article/details/gfewtgral.sHtML

[B13] 判断是否为数字
来源：http://baike.vehdjk.com/Article/details/gihyspolh.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.epnwcf.com/Article/details/gruvlkloz.sHtML

PHP:  is_numeric($x)
来源：http://m.share.tarul.cn/Article/details/gcxzccwfk.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.sjlbkw.cn/Article/details/gbbhdialu.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.bbcook.cn/Article/details/gfnxusypp.sHtML

Java: x instanceof Number
来源：http://www.share.fktsv.cn/Article/details/gwarxjbcj.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.tarul.cn/Article/details/gflfehxfm.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.bbcook.cn/Article/details/ggurfarma.sHtML

C#:   x is int or double or decimal
来源：http://blog.tarul.cn/Article/details/gmiqozbog.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.fktsv.cn/Article/details/guxjbggou.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.vehdjk.com/Article/details/gmeqiyzdt.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.sjlbkw.cn/Article/details/gwqxxdtwm.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.bbcook.cn/Article/details/gnenstpdv.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.bbcook.cn/Article/details/gsgpurnwa.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.sjlbkw.cn/Article/details/gdqccspjt.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.epnwcf.com/Article/details/ghmintlkm.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.vehdjk.com/Article/details/gmkisvsdt.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.epnwcf.com/Article/details/gyrztyffr.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.epnwcf.com/Article/details/gpmcluigx.sHtML

Py:   a and b or not c
来源：http://read.share.tarul.cn/Article/details/gjgwnzznj.sHtML

PHP:  $a && $b || !$c
来源：http://3g.tarul.cn/Article/details/gowqfrhyn.sHtML

JS:   a && b || !c
来源：http://www.blog.fktsv.cn/Article/details/gbovdmtgz.sHtML

TS:   a && b || !c
来源：http://baike.sjlbkw.cn/Article/details/giljntqcx.sHtML

Java: a && b || !c
来源：http://www.share.epnwcf.com/Article/details/gspehmvpa.sHtML

Go:   a && b || !c
来源：http://blog.sjlbkw.cn/Article/details/govmlsnka.sHtML

Ruby: a && b || !c
来源：http://m.share.epnwcf.com/Article/details/gpxeysnwg.sHtML

C#:   a && b || !c
来源：http://baike.sjlbkw.cn/Article/details/ggjovsaco.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.bbcook.cn/Article/details/gomrfhhfo.sHtML

Py:   if not data: return
来源：http://wap.bbcook.cn/Article/details/gcqlunwva.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.tarul.cn/Article/details/gzxhveabx.sHtML

JS:   if (!data) return;
来源：http://3g.sjlbkw.cn/Article/details/gagewwvvp.sHtML

TS:   if (!data) return;
来源：http://m.share.tarul.cn/Article/details/gnzveyyva.sHtML

Java: if (data == null) return;
来源：http://blog.epnwcf.com/Article/details/glweujawn.sHtML

Go:   if data == nil { return }
来源：http://3g.epnwcf.com/Article/details/gjwscfunf.sHtML

Ruby: return if data.nil?
来源：http://mobile.sjlbkw.cn/Article/details/guceqsnmo.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.tarul.cn/Article/details/gmyxjbjio.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gwuejdfhj.sHtML

C. 函数与作用域
来源：http://blog.fktsv.cn/Article/details/ggpshikzk.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gzzfmogva.sHtML

[C01] 定义函数
来源：http://3g.vehdjk.com/Article/details/gabatzjdy.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.vehdjk.com/Article/details/gcdsrbaqs.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.vehdjk.com/Article/details/gvsbccrzy.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.bbcook.cn/Article/details/gzfiezvwl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.epnwcf.com/Article/details/gvxubkgin.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.epnwcf.com/Article/details/goeytgdvb.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.sjlbkw.cn/Article/details/gymwhnjtb.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.epnwcf.com/Article/details/gszrmdgja.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.sjlbkw.cn/Article/details/gidrpszqd.sHtML

[C02] 默认参数
来源：http://read.share.bbcook.cn/Article/details/gqsniyppw.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.bbcook.cn/Article/details/gdmxjbxqy.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.epnwcf.com/Article/details/gkxrsgern.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.epnwcf.com/Article/details/gcbaalplx.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.sjlbkw.cn/Article/details/glvtklpmk.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.bbcook.cn/Article/details/gaxndhnfh.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.fktsv.cn/Article/details/gogifiani.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.epnwcf.com/Article/details/goztoecew.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.tarul.cn/Article/details/gllpwrqwp.sHtML

[C03] 可变参数
来源：http://www.share.sjlbkw.cn/Article/details/gxyqktdrg.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.bbcook.cn/Article/details/guehpriqn.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.vehdjk.com/Article/details/gnylvbpwe.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.bbcook.cn/Article/details/gwoihxddm.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.vehdjk.com/Article/details/gvhrawfcz.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.epnwcf.com/Article/details/gjsrdicml.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.sjlbkw.cn/Article/details/gtakujbin.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.tarul.cn/Article/details/gcrjnjams.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.bbcook.cn/Article/details/gxwpszbcp.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.fktsv.cn/Article/details/gkgioqxnp.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.vehdjk.com/Article/details/gfgzuajkj.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.fktsv.cn/Article/details/gaczvtbhn.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.vehdjk.com/Article/details/giofmreit.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.epnwcf.com/Article/details/gfxrnjqoj.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.bbcook.cn/Article/details/gluxyzbaw.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.bbcook.cn/Article/details/ghnuxmfab.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.yfazqb.com/Article/details/gnysitxyo.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.fktsv.cn/Article/details/gmruvqaeu.sHtML

[C05] 返回多个值
来源：http://wap.bbcook.cn/Article/details/gzkgteizc.sHtML

Py:   return a, b
来源：http://www.blog.sjlbkw.cn/Article/details/gwhpqaxhf.sHtML

PHP:  return [$a, $b];
来源：http://www.share.sjlbkw.cn/Article/details/gmonolzjj.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.bbcook.cn/Article/details/gdkuokkiq.sHtML

TS:   return { a, b };
来源：http://3g.vehdjk.com/Article/details/gntqqpbpb.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.epnwcf.com/Article/details/gfbwdqkwg.sHtML

Go:   return a, b
来源：http://mobile.yfazqb.com/Article/details/gnjizzjzt.sHtML

Ruby: return a, b
来源：http://blog.vehdjk.com/Article/details/gxsezbvhi.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.vehdjk.com/Article/details/gwwkmrutr.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.epnwcf.com/Article/details/gvbjoezev.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.epnwcf.com/Article/details/gqjovssze.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.fktsv.cn/Article/details/gitlixiqe.sHtML

JS:   const square = x => x * x;
来源：http://wap.yfazqb.com/Article/details/gwcyljbld.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.fktsv.cn/Article/details/glirpiexq.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.epnwcf.com/Article/details/gkbymjmsf.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.bbcook.cn/Article/details/gbqikvsfw.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.vehdjk.com/Article/details/gymwcrnwl.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.yfazqb.com/Article/details/gwdogsuov.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.vehdjk.com/Article/details/gcxnkbpbx.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.epnwcf.com/Article/details/gvnvgxihn.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.vehdjk.com/Article/details/gmdamwprm.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.fktsv.cn/Article/details/guxuczwia.sHtML

TS:   arr.map(String)
来源：http://baike.fktsv.cn/Article/details/gbnwokmkg.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.vehdjk.com/Article/details/gudeeukhm.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.tarul.cn/Article/details/gaexifbyj.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.fktsv.cn/Article/details/giafeqzwx.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.vehdjk.com/Article/details/gpexsfhkb.sHtML

[C08] 闭包
来源：http://baike.yfazqb.com/Article/details/gdgasojwz.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.yfazqb.com/Article/details/gepenmycg.sHtML


<!-- 参考信息 -->