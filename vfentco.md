代发 wailian999

[A18] 字符与 ASCII 码互转
来源：http://wap.sjlbkw.cn/Article/details/gkyseuxgm.sHtML

Py:   ord("A"); chr(65)
来源：http://m.share.fktsv.cn/Article/details/gdqgzshaz.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.m.share.fktsv.cn/Article/details/gqsjxhuyh.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.tarul.cn/Article/details/gmlfafrmv.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://read.share.epnwcf.com/Article/details/guznucmqj.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.share.vehdjk.com/Article/details/gqwfannsp.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.blog.yfazqb.com/Article/details/glnthegmd.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.blog.sjlbkw.cn/Article/details/gwlxwnush.sHtML

C#:   (int)'A'; (char)65
来源：http://read.share.fktsv.cn/Article/details/gfwsiakgo.sHtML

[A19] 交换两个变量
来源：http://www.m.share.vehdjk.com/Article/details/gdpbtuthl.sHtML

Py:   a, b = b, a
来源：http://baike.fktsv.cn/Article/details/gmcwtcasv.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://3g.bbcook.cn/Article/details/glsijxcms.sHtML

JS:   [a, b] = [b, a];
来源：http://blog.sjlbkw.cn/Article/details/gpkadbcul.sHtML

TS:   [a, b] = [b, a];
来源：http://read.share.yfazqb.com/Article/details/gxgmongek.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.blog.tarul.cn/Article/details/gbazcxmcl.sHtML

Go:   a, b = b, a
来源：http://mobile.bbcook.cn/Article/details/gwmggmaqz.sHtML

Ruby: a, b = b, a
来源：http://blog.bbcook.cn/Article/details/gaiwybpwh.sHtML

C#:   (a, b) = (b, a);
来源：http://www.share.epnwcf.com/Article/details/gxtbgdhie.sHtML

[A20] 读取标准输入
来源：http://blog.bbcook.cn/Article/details/gkddypaoy.sHtML

Py:   name = input("请输入：")
来源：http://www.m.share.sjlbkw.cn/Article/details/gwhwxlqag.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.blog.fktsv.cn/Article/details/gqypzwlfz.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://read.share.tarul.cn/Article/details/gfwxuyrgn.sHtML

TS:   // Node.js：readline 模块
来源：http://www.share.vehdjk.com/Article/details/gvixavqwa.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://wap.bbcook.cn/Article/details/gfyjnfxjw.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://3g.tarul.cn/Article/details/gyrtsovxm.sHtML

Ruby: gets.chomp
来源：http://mobile.bbcook.cn/Article/details/guevbpmml.sHtML

C#:   Console.ReadLine();
来源：http://wap.sjlbkw.cn/Article/details/givsxwbsk.sHtML

[A21] 保留指定小数位输出
来源：http://wap.fktsv.cn/Article/details/gfscixdfa.sHtML

Py:   f"{3.14159:.2f}"
来源：http://mobile.vehdjk.com/Article/details/gxrkcxmmp.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.blog.fktsv.cn/Article/details/gbdxwrsvj.sHtML

JS:   (3.14159).toFixed(2)
来源：http://m.share.tarul.cn/Article/details/gplqrltei.sHtML

TS:   (3.14159).toFixed(2)
来源：http://m.share.bbcook.cn/Article/details/gsiqgnkep.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://baike.bbcook.cn/Article/details/gvwlbmkqe.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.share.tarul.cn/Article/details/gcxpwzvjm.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.share.sjlbkw.cn/Article/details/gastazrda.sHtML

C#:   3.14159.ToString("F2")
来源：http://baike.bbcook.cn/Article/details/gangyuluo.sHtML

[A22] 获取字符串长度
来源：http://3g.vehdjk.com/Article/details/gkrwgncrl.sHtML

Py:   len(s)
来源：http://www.m.share.fktsv.cn/Article/details/gecyeehwf.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.m.share.epnwcf.com/Article/details/gesupfrhh.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://m.share.fktsv.cn/Article/details/gdwylcgvh.sHtML

TS:   s.length
来源：http://wap.tarul.cn/Article/details/gwalkamfb.sHtML

Java: s.length()
来源：http://wap.bbcook.cn/Article/details/gimcjfgoz.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mobile.sjlbkw.cn/Article/details/geymbzfpb.sHtML

Ruby: s.length
来源：http://3g.epnwcf.com/Article/details/gebysgpza.sHtML

C#:   s.Length
来源：http://wap.vehdjk.com/Article/details/gavtpdcyu.sHtML

[A23] 大小写转换
来源：http://www.share.epnwcf.com/Article/details/gezrbxsxj.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://m.share.fktsv.cn/Article/details/giozcfsvr.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mobile.vehdjk.com/Article/details/gkhtaedsf.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.tarul.cn/Article/details/giqejkckb.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.epnwcf.com/Article/details/gkngmbyqs.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://baike.vehdjk.com/Article/details/ghdjxjvyl.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wap.vehdjk.com/Article/details/ghjrlfswl.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.blog.fktsv.cn/Article/details/gubgyaypb.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://3g.epnwcf.com/Article/details/gpgaalgjq.sHtML

[A24] 去除首尾空白
来源：http://3g.epnwcf.com/Article/details/gjzioyryi.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://3g.fktsv.cn/Article/details/gnswhcftz.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.blog.tarul.cn/Article/details/gomvrewbr.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.vehdjk.com/Article/details/gypudgzwu.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.fktsv.cn/Article/details/gowjvjumu.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mobile.fktsv.cn/Article/details/gqpphkwug.sHtML

Go:   strings.TrimSpace(s)
来源：http://3g.sjlbkw.cn/Article/details/giouscand.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://m.share.epnwcf.com/Article/details/gkzvjpbrk.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wap.sjlbkw.cn/Article/details/gadscvvsn.sHtML

[A25] 字符串比较
来源：http://3g.tarul.cn/Article/details/gfvoedqed.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.share.vehdjk.com/Article/details/gdugmavhd.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://m.share.epnwcf.com/Article/details/gdrfeokff.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.bbcook.cn/Article/details/graqzzknf.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.epnwcf.com/Article/details/gjoowgpan.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://3g.yfazqb.com/Article/details/gcuwuedwk.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://read.share.bbcook.cn/Article/details/gryxkiodf.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://m.share.yfazqb.com/Article/details/goddijwjj.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://m.share.yfazqb.com/Article/details/gyknsgsat.sHtML

[A26] 类型转换总览
来源：http://wap.sjlbkw.cn/Article/details/gbczoaajh.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.m.share.epnwcf.com/Article/details/gocinncxu.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mobile.bbcook.cn/Article/details/gbzdruybr.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mobile.bbcook.cn/Article/details/guhnragoo.sHtML

TS:   Number() String() Boolean() x as number
来源：http://baike.yfazqb.com/Article/details/ghzoeatem.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.blog.tarul.cn/Article/details/grymuevbl.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.share.tarul.cn/Article/details/ghsiafegv.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://3g.bbcook.cn/Article/details/gcrrlsjtl.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.blog.fktsv.cn/Article/details/guvshzspc.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gicptyuyd.sHtML

B. 流程控制
来源：http://3g.bbcook.cn/Article/details/glxedaoof.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gulhvdjzy.sHtML

[B01] 条件判断 if / else
来源：http://baike.bbcook.cn/Article/details/gmqcqslce.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.share.vehdjk.com/Article/details/grorivrgn.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://m.share.yfazqb.com/Article/details/gxsefzkyt.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.tarul.cn/Article/details/gfydecive.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.sjlbkw.cn/Article/details/gniczlrme.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.blog.tarul.cn/Article/details/gdtyreuvu.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://m.share.bbcook.cn/Article/details/guaruqjvc.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.blog.bbcook.cn/Article/details/gwjnrhpei.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wap.epnwcf.com/Article/details/gwupdihmy.sHtML

[B02] 多分支 else if / elif
来源：http://mobile.epnwcf.com/Article/details/gybpjusfp.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://baike.tarul.cn/Article/details/gnzixvrra.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mobile.epnwcf.com/Article/details/guondwthg.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.yfazqb.com/Article/details/gswguguib.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.epnwcf.com/Article/details/gnqcrljcs.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.fktsv.cn/Article/details/ggxgwddxt.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://baike.fktsv.cn/Article/details/gnxbvogvt.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wap.tarul.cn/Article/details/gjmzfllnt.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.bbcook.cn/Article/details/ghwdawegm.sHtML

[B03] switch / match / case
来源：http://3g.vehdjk.com/Article/details/gvalyrpxu.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://m.share.sjlbkw.cn/Article/details/ghipmkxbt.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://m.share.fktsv.cn/Article/details/guvbjfprx.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.yfazqb.com/Article/details/genjcjmrw.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.epnwcf.com/Article/details/gvxdkzsks.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://blog.bbcook.cn/Article/details/gemevvttx.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://blog.yfazqb.com/Article/details/gddiemdki.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://baike.vehdjk.com/Article/details/gcecjuoaa.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://m.share.fktsv.cn/Article/details/gpjqtmvtb.sHtML

[B04] for 计数循环
来源：http://3g.bbcook.cn/Article/details/gecdvrngi.sHtML

Py:   for i in range(10): print(i)
来源：http://www.m.share.yfazqb.com/Article/details/gfoxqaonw.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mobile.yfazqb.com/Article/details/gjoqkraio.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.fktsv.cn/Article/details/gmqowxpgi.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.epnwcf.com/Article/details/ghahgjjpv.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://3g.vehdjk.com/Article/details/gaawwmkhq.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://3g.fktsv.cn/Article/details/gaqibfdpn.sHtML

Ruby: 10.times { |i| puts i }
来源：http://blog.bbcook.cn/Article/details/gucmzyaje.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://baike.epnwcf.com/Article/details/gshfdrdee.sHtML

[B05] 遍历数组 / 列表
来源：http://read.share.vehdjk.com/Article/details/gtaycfxpd.sHtML

Py:   for item in arr: print(item)
来源：http://3g.bbcook.cn/Article/details/gvprilwoq.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://read.share.epnwcf.com/Article/details/geulshmxd.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://read.share.bbcook.cn/Article/details/gadeidpvv.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://read.share.sjlbkw.cn/Article/details/gwbyhbaqr.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.bbcook.cn/Article/details/gsxwifqqv.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://blog.fktsv.cn/Article/details/gvrjkgsnu.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.vehdjk.com/Article/details/gehivklag.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://baike.bbcook.cn/Article/details/gwqvkckjp.sHtML

[B06] 遍历字典 / 对象
来源：http://mobile.fktsv.cn/Article/details/gutjcpncq.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://wap.fktsv.cn/Article/details/gcfezfkgd.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.tarul.cn/Article/details/gkghvrxii.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.bbcook.cn/Article/details/gaerdkxrt.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.fktsv.cn/Article/details/gzpenupqr.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://blog.tarul.cn/Article/details/gssojpebm.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://3g.vehdjk.com/Article/details/gmcubmrkp.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wap.sjlbkw.cn/Article/details/gpjtfarqt.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.share.sjlbkw.cn/Article/details/gvizxyggm.sHtML

[B07] while 循环
来源：http://www.blog.yfazqb.com/Article/details/gtwwlzmjw.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.yfazqb.com/Article/details/gbikpbvry.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.epnwcf.com/Article/details/girgojpgp.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.fktsv.cn/Article/details/gxpbkhcvp.sHtML

TS:   while (i < 10) { i++; }
来源：http://blog.sjlbkw.cn/Article/details/gmapxamex.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.fktsv.cn/Article/details/gfqdgdkmz.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.epnwcf.com/Article/details/gmartmnyy.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.sjlbkw.cn/Article/details/glafpqiee.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.sjlbkw.cn/Article/details/gsisrqhmt.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.vehdjk.com/Article/details/gecamopwy.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.epnwcf.com/Article/details/gsrqfkffw.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.vehdjk.com/Article/details/gowgqugpt.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.vehdjk.com/Article/details/gaudocoap.sHtML

TS:   do { i++; } while (i < 10);
来源：http://3g.fktsv.cn/Article/details/gpsdqqjxh.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.yfazqb.com/Article/details/gauvzqhjn.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.fktsv.cn/Article/details/gtwplfmks.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.yfazqb.com/Article/details/gvagzkegp.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.yfazqb.com/Article/details/gpbdjppjm.sHtML

[B09] break 与 continue
来源：http://blog.vehdjk.com/Article/details/gvkcrbjyp.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.bbcook.cn/Article/details/gzgoqxqoq.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.vehdjk.com/Article/details/ggvtfgcns.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.yfazqb.com/Article/details/gixusszah.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.bbcook.cn/Article/details/gkdbdluym.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.epnwcf.com/Article/details/gdvignjdo.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.sjlbkw.cn/Article/details/gsggnupew.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://read.share.yfazqb.com/Article/details/gemqzbymp.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.yfazqb.com/Article/details/gscfaziou.sHtML

[B10] 遍历同时拿索引
来源：http://3g.tarul.cn/Article/details/gnvdsmqgx.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.epnwcf.com/Article/details/gzeuqowym.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.sjlbkw.cn/Article/details/gujmcjxqk.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://m.share.bbcook.cn/Article/details/glnbghpiq.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.yfazqb.com/Article/details/gijqjcdlv.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.sjlbkw.cn/Article/details/gtimidhjx.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.fktsv.cn/Article/details/ggijvzngm.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.fktsv.cn/Article/details/gqudpwbfk.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://3g.bbcook.cn/Article/details/giqlafkwj.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.epnwcf.com/Article/details/gczhnwtqd.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.sjlbkw.cn/Article/details/gsryecwst.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.sjlbkw.cn/Article/details/ghchiztsg.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.fktsv.cn/Article/details/gzqqsivhr.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.fktsv.cn/Article/details/glekyuoyo.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.vehdjk.com/Article/details/gbpsbuxau.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.fktsv.cn/Article/details/gexeyjpho.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.sjlbkw.cn/Article/details/gaxptpejz.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.vehdjk.com/Article/details/gzuarleyv.sHtML

[B12] 跳出多层循环
来源：http://blog.epnwcf.com/Article/details/gomdfhvxq.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.yfazqb.com/Article/details/gnmjuqchi.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.vehdjk.com/Article/details/gsiaqwacw.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fktsv.cn/Article/details/gswsexlzt.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.bbcook.cn/Article/details/gvfdqkehq.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.yfazqb.com/Article/details/gllhjecuu.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.fktsv.cn/Article/details/gflcsidxr.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.bbcook.cn/Article/details/gxhsepuit.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.tarul.cn/Article/details/gybjpacqi.sHtML

[B13] 判断是否为数字
来源：http://mobile.epnwcf.com/Article/details/gevaktumr.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.fktsv.cn/Article/details/gculmkvhj.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.vehdjk.com/Article/details/ggcmqxrqy.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.yfazqb.com/Article/details/gluhgongn.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.sjlbkw.cn/Article/details/gyfnsiuar.sHtML

Java: x instanceof Number
来源：http://wap.vehdjk.com/Article/details/gibqcjjjw.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.bbcook.cn/Article/details/gzuyqmyxi.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.vehdjk.com/Article/details/gpprikfkk.sHtML

C#:   x is int or double or decimal
来源：http://baike.sjlbkw.cn/Article/details/gmpgrxwsc.sHtML

[B14] 判断值是否在集合内
来源：http://wap.vehdjk.com/Article/details/gnqgfeyan.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.bbcook.cn/Article/details/gzzfrlqtv.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.yfazqb.com/Article/details/gvugjuhgi.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.sjlbkw.cn/Article/details/gwgtdowls.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.bbcook.cn/Article/details/gtxjzczje.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.epnwcf.com/Article/details/gutwpubsw.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.fktsv.cn/Article/details/gvehfljfv.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.sjlbkw.cn/Article/details/ganpdkiyd.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.vehdjk.com/Article/details/glbehkquy.sHtML

[B15] 布尔运算与取反
来源：http://3g.bbcook.cn/Article/details/gwjkjhtsg.sHtML

Py:   a and b or not c
来源：http://www.m.share.bbcook.cn/Article/details/gfgoysvfn.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.vehdjk.com/Article/details/ggazkrlfz.sHtML

JS:   a && b || !c
来源：http://read.share.yfazqb.com/Article/details/gveqoxvch.sHtML

TS:   a && b || !c
来源：http://m.share.bbcook.cn/Article/details/gjxjskyuz.sHtML

Java: a && b || !c
来源：http://wap.sjlbkw.cn/Article/details/geqtyjjgk.sHtML

Go:   a && b || !c
来源：http://mobile.sjlbkw.cn/Article/details/ghnfforac.sHtML

Ruby: a && b || !c
来源：http://m.share.fktsv.cn/Article/details/gsygkwprc.sHtML

C#:   a && b || !c
来源：http://read.share.sjlbkw.cn/Article/details/groshsblm.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.vehdjk.com/Article/details/gshryckmq.sHtML

Py:   if not data: return
来源：http://m.share.vehdjk.com/Article/details/ghrnrkxnc.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.bbcook.cn/Article/details/gmobdkrdl.sHtML

JS:   if (!data) return;
来源：http://www.share.vehdjk.com/Article/details/gvevzesem.sHtML

TS:   if (!data) return;
来源：http://blog.bbcook.cn/Article/details/gfmfunsmo.sHtML

Java: if (data == null) return;
来源：http://www.blog.fktsv.cn/Article/details/gnwgjfvkh.sHtML

Go:   if data == nil { return }
来源：http://read.share.epnwcf.com/Article/details/gwwzxysra.sHtML

Ruby: return if data.nil?
来源：http://m.share.fktsv.cn/Article/details/gzocbfnvq.sHtML

C#:   if (data == null) return;
来源：http://wap.vehdjk.com/Article/details/gdsmxqsxi.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gfhrtmthz.sHtML

C. 函数与作用域
来源：http://wap.vehdjk.com/Article/details/gpzmtumki.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gksevginz.sHtML

[C01] 定义函数
来源：http://www.blog.vehdjk.com/Article/details/gmgmsgjjq.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.yfazqb.com/Article/details/gvhnrdgnp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.bbcook.cn/Article/details/gaxhwbywc.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.yfazqb.com/Article/details/gwutlntii.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.yfazqb.com/Article/details/guwqldijk.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.bbcook.cn/Article/details/gzijxovcs.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.sjlbkw.cn/Article/details/gcymzrwrs.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.sjlbkw.cn/Article/details/gmxznfktj.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.sjlbkw.cn/Article/details/gzrkwgarn.sHtML

[C02] 默认参数
来源：http://www.m.share.bbcook.cn/Article/details/gfywbpjzv.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.vehdjk.com/Article/details/ggxlkhsgm.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.yfazqb.com/Article/details/gqyiyazps.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.yfazqb.com/Article/details/godabshka.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gapdwppdc.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.yfazqb.com/Article/details/gyivpelmi.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.vehdjk.com/Article/details/gnxjciotr.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.tarul.cn/Article/details/grsiartza.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.fktsv.cn/Article/details/gndqiubkh.sHtML

[C03] 可变参数
来源：http://baike.fktsv.cn/Article/details/gmyjhqbfb.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.tarul.cn/Article/details/gskmidfyq.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.bbcook.cn/Article/details/gvrplgrsj.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.bbcook.cn/Article/details/gcjnntydo.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fktsv.cn/Article/details/gtkkkzyic.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.vehdjk.com/Article/details/gursbmntd.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.vehdjk.com/Article/details/gdqhcpfci.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.tarul.cn/Article/details/gdnqwaavx.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.sjlbkw.cn/Article/details/gwytyukct.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.tarul.cn/Article/details/gtgirfrro.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.yfazqb.com/Article/details/gyxtkughh.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.fktsv.cn/Article/details/ggvgnmubu.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.epnwcf.com/Article/details/gtbynvkzu.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.fktsv.cn/Article/details/gerlknrlh.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.yfazqb.com/Article/details/gkxtrvazl.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.tarul.cn/Article/details/gbdkjyqfz.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.fktsv.cn/Article/details/gqrkowvjl.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.epnwcf.com/Article/details/gopmuidog.sHtML

[C05] 返回多个值
来源：http://www.m.share.epnwcf.com/Article/details/glkqunsmj.sHtML

Py:   return a, b
来源：http://blog.fktsv.cn/Article/details/gxbeytzsd.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.epnwcf.com/Article/details/gqgbfovjh.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.vehdjk.com/Article/details/gszefyxvv.sHtML

TS:   return { a, b };
来源：http://read.share.yfazqb.com/Article/details/gpioecxjm.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.sjlbkw.cn/Article/details/gdgxwlcow.sHtML

Go:   return a, b
来源：http://www.m.share.fktsv.cn/Article/details/gztmrkozq.sHtML

Ruby: return a, b
来源：http://www.m.share.yfazqb.com/Article/details/gcpzoyena.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.tarul.cn/Article/details/gzxbvqlvk.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.tarul.cn/Article/details/gbbzhuadx.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.fktsv.cn/Article/details/geiztxqsw.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.tarul.cn/Article/details/gjmpvgxda.sHtML

JS:   const square = x => x * x;
来源：http://blog.tarul.cn/Article/details/gaavxliud.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.sjlbkw.cn/Article/details/gitdgovmq.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.fktsv.cn/Article/details/gnhtlqvww.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.fktsv.cn/Article/details/gtpzeiujt.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.epnwcf.com/Article/details/gftgizxix.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.yfazqb.com/Article/details/gqevgwntc.sHtML

[C07] 把函数作为参数传入
来源：http://wap.fktsv.cn/Article/details/ghvekozpc.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.epnwcf.com/Article/details/gdwksdwrq.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.tarul.cn/Article/details/gsfkueunt.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.vehdjk.com/Article/details/gfjpkippd.sHtML

TS:   arr.map(String)
来源：http://m.share.yfazqb.com/Article/details/gvnhhcgee.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.vehdjk.com/Article/details/guiscgkhm.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.bbcook.cn/Article/details/gqjyvtado.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.vehdjk.com/Article/details/gqhwlncny.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.tarul.cn/Article/details/grpygusrs.sHtML

[C08] 闭包
来源：http://wap.tarul.cn/Article/details/gkcxtywxf.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.bbcook.cn/Article/details/gfhdjukiw.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.sjlbkw.cn/Article/details/gcybbahpp.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.vehdjk.com/Article/details/gfxmhizfu.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.yfazqb.com/Article/details/ghnohmwqj.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.fktsv.cn/Article/details/gbahameww.sHtML


<!-- 参考信息 -->