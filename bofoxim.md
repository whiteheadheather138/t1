代发 wailian999

Ruby: value = data || "默认值"
来源：http://baike.vehdjk.com/Article/details/gdyhjqghi.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.share.vehdjk.com/Article/details/glqpxwcvx.sHtML

[A16] 真假值判断规则
来源：http://www.m.share.vehdjk.com/Article/details/gqthftjfy.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wap.bbcook.cn/Article/details/gvmizwstr.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://blog.bbcook.cn/Article/details/gjcikhvpp.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.share.bbcook.cn/Article/details/gzkjjryrw.sHtML

TS:   if (!x) {}
来源：http://blog.fktsv.cn/Article/details/gaiucncns.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.m.share.epnwcf.com/Article/details/gzvilrnil.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.m.share.tarul.cn/Article/details/gbcrvyceq.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://read.share.epnwcf.com/Article/details/ghqbdjrpv.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mobile.sjlbkw.cn/Article/details/gpotniowl.sHtML

[A17] 位运算
来源：http://blog.fktsv.cn/Article/details/gvxgpjrzj.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.bbcook.cn/Article/details/gndzccdqf.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.share.tarul.cn/Article/details/gyuyazhxq.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.vehdjk.com/Article/details/gmzyuhnrd.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://read.share.bbcook.cn/Article/details/gehqjvwlh.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.yfazqb.com/Article/details/gwxsgtqoa.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.blog.sjlbkw.cn/Article/details/gxlopmnsp.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.sjlbkw.cn/Article/details/gtrewedbk.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.tarul.cn/Article/details/gqszzbmqi.sHtML

[A18] 字符与 ASCII 码互转
来源：http://blog.sjlbkw.cn/Article/details/gbjanhqgi.sHtML

Py:   ord("A"); chr(65)
来源：http://blog.tarul.cn/Article/details/gkgzdjxqx.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.share.sjlbkw.cn/Article/details/gefkvsfjn.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.sjlbkw.cn/Article/details/gtktrbgcp.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.yfazqb.com/Article/details/gerzicbbq.sHtML

Java: (int) 'A'; (char) 65
来源：http://wap.epnwcf.com/Article/details/grzjxjxjf.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://m.share.yfazqb.com/Article/details/guefephwa.sHtML

Ruby: "A".ord; 65.chr
来源：http://baike.bbcook.cn/Article/details/gftctmfyb.sHtML

C#:   (int)'A'; (char)65
来源：http://www.share.epnwcf.com/Article/details/gjesypyir.sHtML

[A19] 交换两个变量
来源：http://baike.fktsv.cn/Article/details/gmiovhjim.sHtML

Py:   a, b = b, a
来源：http://wap.tarul.cn/Article/details/geepqpiaz.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.share.sjlbkw.cn/Article/details/gpqngajxh.sHtML

JS:   [a, b] = [b, a];
来源：http://www.m.share.epnwcf.com/Article/details/grsindojd.sHtML

TS:   [a, b] = [b, a];
来源：http://3g.vehdjk.com/Article/details/gtjwlljdt.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.blog.epnwcf.com/Article/details/gssboihnd.sHtML

Go:   a, b = b, a
来源：http://3g.sjlbkw.cn/Article/details/gnxcpjecq.sHtML

Ruby: a, b = b, a
来源：http://3g.vehdjk.com/Article/details/gamagdygu.sHtML

C#:   (a, b) = (b, a);
来源：http://baike.epnwcf.com/Article/details/gfmjifaqo.sHtML

[A20] 读取标准输入
来源：http://m.share.epnwcf.com/Article/details/gogiqvgtm.sHtML

Py:   name = input("请输入：")
来源：http://m.share.yfazqb.com/Article/details/ghjzspzdz.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.share.epnwcf.com/Article/details/gewerarvf.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.m.share.vehdjk.com/Article/details/ggjfsomyf.sHtML

TS:   // Node.js：readline 模块
来源：http://m.share.sjlbkw.cn/Article/details/gluntvgwf.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://blog.fktsv.cn/Article/details/gniochjky.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.m.share.vehdjk.com/Article/details/gvqzsicls.sHtML

Ruby: gets.chomp
来源：http://blog.sjlbkw.cn/Article/details/gjgsxbvjy.sHtML

C#:   Console.ReadLine();
来源：http://www.m.share.fktsv.cn/Article/details/gchfuhvuq.sHtML

[A21] 保留指定小数位输出
来源：http://3g.bbcook.cn/Article/details/gpmomquod.sHtML

Py:   f"{3.14159:.2f}"
来源：http://wap.yfazqb.com/Article/details/gftwdqppo.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://blog.yfazqb.com/Article/details/gvuvjacyp.sHtML

JS:   (3.14159).toFixed(2)
来源：http://m.share.fktsv.cn/Article/details/gfideblcl.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.blog.yfazqb.com/Article/details/gvmwyhbnr.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.m.share.sjlbkw.cn/Article/details/gaoaddxbz.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://3g.epnwcf.com/Article/details/gqnzpopfg.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://read.share.epnwcf.com/Article/details/ghbetyexv.sHtML

C#:   3.14159.ToString("F2")
来源：http://m.share.bbcook.cn/Article/details/gdbozzajf.sHtML

[A22] 获取字符串长度
来源：http://m.share.vehdjk.com/Article/details/gujnrosmc.sHtML

Py:   len(s)
来源：http://3g.vehdjk.com/Article/details/goaotcifa.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://read.share.tarul.cn/Article/details/gkgbrbotp.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mobile.epnwcf.com/Article/details/gpiirlmsv.sHtML

TS:   s.length
来源：http://mobile.tarul.cn/Article/details/gsqghmgrw.sHtML

Java: s.length()
来源：http://mobile.fktsv.cn/Article/details/gjhmuesld.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.blog.yfazqb.com/Article/details/gnpwcfxsm.sHtML

Ruby: s.length
来源：http://mobile.sjlbkw.cn/Article/details/gjjqleqtq.sHtML

C#:   s.Length
来源：http://blog.vehdjk.com/Article/details/gfjiwscku.sHtML

[A23] 大小写转换
来源：http://blog.sjlbkw.cn/Article/details/gmhyfrnnv.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.share.vehdjk.com/Article/details/gnrwoctfb.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://baike.tarul.cn/Article/details/gcedadzoe.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.tarul.cn/Article/details/garqfssmr.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.tarul.cn/Article/details/gcleuicam.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mobile.tarul.cn/Article/details/gwvvcloay.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mobile.tarul.cn/Article/details/gicxaqymh.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mobile.vehdjk.com/Article/details/gviymqsbe.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://blog.sjlbkw.cn/Article/details/gbaycduhq.sHtML

[A24] 去除首尾空白
来源：http://m.share.epnwcf.com/Article/details/grugxgfii.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://blog.vehdjk.com/Article/details/ghhixzsec.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wap.bbcook.cn/Article/details/gjbbwcwba.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.tarul.cn/Article/details/gqyqezttn.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.epnwcf.com/Article/details/gpuxckicd.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://3g.tarul.cn/Article/details/gryxbautz.sHtML

Go:   strings.TrimSpace(s)
来源：http://mobile.fktsv.cn/Article/details/gflauorul.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://baike.vehdjk.com/Article/details/gtxplbghj.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://blog.sjlbkw.cn/Article/details/gdgvmunaq.sHtML

[A25] 字符串比较
来源：http://blog.vehdjk.com/Article/details/gsjiczinm.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.blog.sjlbkw.cn/Article/details/gweipbsxw.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mobile.tarul.cn/Article/details/ganzxjmsp.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.sjlbkw.cn/Article/details/gbujvekse.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.yfazqb.com/Article/details/gimhijztx.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://baike.tarul.cn/Article/details/gndrqxowe.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtelifovu.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://read.share.vehdjk.com/Article/details/gamhmqnng.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://3g.vehdjk.com/Article/details/gpsdcbbgq.sHtML

[A26] 类型转换总览
来源：http://3g.sjlbkw.cn/Article/details/gaencprhw.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.blog.bbcook.cn/Article/details/goqepqyuz.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://baike.bbcook.cn/Article/details/gvrhmranz.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://baike.vehdjk.com/Article/details/gdmfqthnb.sHtML

TS:   Number() String() Boolean() x as number
来源：http://3g.tarul.cn/Article/details/gefgraern.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.m.share.bbcook.cn/Article/details/gcglubdoz.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mobile.yfazqb.com/Article/details/gmawkpykt.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.m.share.sjlbkw.cn/Article/details/gnnpmupim.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.m.share.vehdjk.com/Article/details/gexbosayu.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gyuvgxaeh.sHtML

B. 流程控制
来源：http://www.blog.tarul.cn/Article/details/gjgyjxdan.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gopvthvvh.sHtML

[B01] 条件判断 if / else
来源：http://www.blog.fktsv.cn/Article/details/gdcpmgfgi.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://blog.vehdjk.com/Article/details/gdhqwbzkm.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://baike.bbcook.cn/Article/details/gystbnicy.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.yfazqb.com/Article/details/glzuqgfoi.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.fktsv.cn/Article/details/gfuerumgk.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.share.fktsv.cn/Article/details/giuqmvijw.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.blog.sjlbkw.cn/Article/details/gliweeynl.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wap.sjlbkw.cn/Article/details/gtrlrhefe.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.m.share.bbcook.cn/Article/details/geiavqanb.sHtML

[B02] 多分支 else if / elif
来源：http://www.blog.sjlbkw.cn/Article/details/ggytvzmql.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.blog.vehdjk.com/Article/details/gqxqszylp.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://blog.epnwcf.com/Article/details/gfoxnywop.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.vehdjk.com/Article/details/gxelhydul.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.bbcook.cn/Article/details/gwwkoqpvi.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.yfazqb.com/Article/details/gqbatmhrg.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://3g.vehdjk.com/Article/details/gnipcodeq.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.share.bbcook.cn/Article/details/gzialtipz.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.sjlbkw.cn/Article/details/ggcvhnewn.sHtML

[B03] switch / match / case
来源：http://www.blog.bbcook.cn/Article/details/gwifypcxx.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.m.share.bbcook.cn/Article/details/gdhbtvueo.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://read.share.yfazqb.com/Article/details/guvssrcxh.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.bbcook.cn/Article/details/gyuuoubej.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.tarul.cn/Article/details/gcjmsadrt.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://m.share.sjlbkw.cn/Article/details/gehkiybkl.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mobile.vehdjk.com/Article/details/gtetxblmu.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.blog.epnwcf.com/Article/details/gcfglovmb.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://3g.fktsv.cn/Article/details/gozjraxho.sHtML

[B04] for 计数循环
来源：http://www.m.share.yfazqb.com/Article/details/gjpiabhww.sHtML

Py:   for i in range(10): print(i)
来源：http://baike.epnwcf.com/Article/details/gkcjshdwj.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://m.share.bbcook.cn/Article/details/guflznkqu.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.tarul.cn/Article/details/gckkbvvok.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.sjlbkw.cn/Article/details/gbdiecxrv.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.share.tarul.cn/Article/details/gztuxdyid.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.share.vehdjk.com/Article/details/gogaimhfp.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.blog.epnwcf.com/Article/details/gsvewxmrl.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://blog.tarul.cn/Article/details/gogxnicaz.sHtML

[B05] 遍历数组 / 列表
来源：http://www.share.sjlbkw.cn/Article/details/gyljqrrdw.sHtML

Py:   for item in arr: print(item)
来源：http://read.share.tarul.cn/Article/details/grwnvwdps.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://m.share.tarul.cn/Article/details/gcvbhouny.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://mobile.fktsv.cn/Article/details/giiukdgdt.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://blog.fktsv.cn/Article/details/guatbidvy.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://3g.sjlbkw.cn/Article/details/gvpamrfqv.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://read.share.tarul.cn/Article/details/gfgdahtmf.sHtML

Ruby: arr.each { |item| puts item }
来源：http://m.share.tarul.cn/Article/details/gtmduxhcn.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://read.share.epnwcf.com/Article/details/gsynbqgsk.sHtML

[B06] 遍历字典 / 对象
来源：http://www.m.share.epnwcf.com/Article/details/goaqbyzgg.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.tarul.cn/Article/details/gbekewqhx.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.m.share.fktsv.cn/Article/details/gybwpqvbo.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.tarul.cn/Article/details/gbelmypsf.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.bbcook.cn/Article/details/gamghfbis.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://baike.epnwcf.com/Article/details/gbbhneqop.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://3g.tarul.cn/Article/details/glktytjoy.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.vehdjk.com/Article/details/gzaogtsta.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://m.share.epnwcf.com/Article/details/garmbajfp.sHtML

[B07] while 循环
来源：http://www.share.tarul.cn/Article/details/gektghhkt.sHtML

Py:   while i < 10: i += 1
来源：http://3g.vehdjk.com/Article/details/gakbkxalx.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.blog.sjlbkw.cn/Article/details/grynuxjce.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.yfazqb.com/Article/details/gklgnebdt.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.share.bbcook.cn/Article/details/gxmdffnul.sHtML

Java: while (i < 10) { i++; }
来源：http://wap.epnwcf.com/Article/details/givtjrtdk.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://m.share.fktsv.cn/Article/details/gnkhxbdja.sHtML

Ruby: while i < 10; i += 1; end
来源：http://3g.tarul.cn/Article/details/grjcnzsvy.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.blog.tarul.cn/Article/details/gvxlliskw.sHtML

[B08] do-while（至少执行一次）
来源：http://www.blog.yfazqb.com/Article/details/gkypgdsvs.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.epnwcf.com/Article/details/gndhlsieh.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.tarul.cn/Article/details/gvcpzlpcf.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.vehdjk.com/Article/details/godxjmqdo.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.vehdjk.com/Article/details/glcxzvxsk.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.blog.fktsv.cn/Article/details/gqiztrpki.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://m.share.yfazqb.com/Article/details/gxevxxchc.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.fktsv.cn/Article/details/guefnokij.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.fktsv.cn/Article/details/gigqcwcqd.sHtML

[B09] break 与 continue
来源：http://3g.bbcook.cn/Article/details/gkmcdvdkc.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.vehdjk.com/Article/details/gpgpgugyq.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.epnwcf.com/Article/details/gncdcogwb.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fktsv.cn/Article/details/gjlrrbppa.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.yfazqb.com/Article/details/gisgjlmje.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.epnwcf.com/Article/details/gavrphmoy.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.epnwcf.com/Article/details/ghdsbcnhv.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.yfazqb.com/Article/details/gwdvzphqk.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.yfazqb.com/Article/details/gwupsqyvj.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.vehdjk.com/Article/details/ghxnlxins.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.yfazqb.com/Article/details/gjsllfexa.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.sjlbkw.cn/Article/details/gqihleyby.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.sjlbkw.cn/Article/details/gxhheyfjj.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.sjlbkw.cn/Article/details/gzicrmbfp.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.epnwcf.com/Article/details/gsemkpjxz.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.vehdjk.com/Article/details/gcceozmxm.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.epnwcf.com/Article/details/gwdorgrep.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.vehdjk.com/Article/details/ghxybaypy.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.tarul.cn/Article/details/gnyszhzra.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.epnwcf.com/Article/details/gxbrlmbhv.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.tarul.cn/Article/details/goevtqeiy.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.sjlbkw.cn/Article/details/gkggyscvn.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.sjlbkw.cn/Article/details/gajbupzsp.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.sjlbkw.cn/Article/details/gsqvvwhdp.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.epnwcf.com/Article/details/gdrtjgddj.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.epnwcf.com/Article/details/gubvznhei.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.yfazqb.com/Article/details/gmbtgslxk.sHtML

[B12] 跳出多层循环
来源：http://www.share.tarul.cn/Article/details/gxdivvsxx.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.tarul.cn/Article/details/gafbmweug.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.yfazqb.com/Article/details/geokumhgd.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.tarul.cn/Article/details/gctafrntc.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.sjlbkw.cn/Article/details/gunkzmqqn.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.yfazqb.com/Article/details/gcvszhdrc.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.tarul.cn/Article/details/glthrbgkx.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.epnwcf.com/Article/details/gvcwfwprc.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.vehdjk.com/Article/details/gsvzyzxhv.sHtML

[B13] 判断是否为数字
来源：http://baike.sjlbkw.cn/Article/details/gtwehlhzz.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.yfazqb.com/Article/details/gppsmzliz.sHtML

PHP:  is_numeric($x)
来源：http://blog.epnwcf.com/Article/details/gjcxlcvma.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.sjlbkw.cn/Article/details/gnankoqnw.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.fktsv.cn/Article/details/gixxzdmlx.sHtML

Java: x instanceof Number
来源：http://blog.bbcook.cn/Article/details/gztutkbvs.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.sjlbkw.cn/Article/details/gtbpqpbwx.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.tarul.cn/Article/details/gnlqssnun.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.yfazqb.com/Article/details/glndratcy.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.yfazqb.com/Article/details/ggwjbblqj.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.vehdjk.com/Article/details/gspgtknkb.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.fktsv.cn/Article/details/gmhkuvdqn.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.epnwcf.com/Article/details/gtbbiybxn.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.yfazqb.com/Article/details/ghhvgrnuy.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.tarul.cn/Article/details/gbjnihzzy.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.yfazqb.com/Article/details/gwjffciap.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.bbcook.cn/Article/details/gyvdwxvyo.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.tarul.cn/Article/details/gefkujgpl.sHtML

[B15] 布尔运算与取反
来源：http://www.share.epnwcf.com/Article/details/gmbzuemsg.sHtML

Py:   a and b or not c
来源：http://mobile.fktsv.cn/Article/details/gaeckujji.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.fktsv.cn/Article/details/gttlpjvtw.sHtML

JS:   a && b || !c
来源：http://3g.epnwcf.com/Article/details/giqypqeck.sHtML

TS:   a && b || !c
来源：http://m.share.sjlbkw.cn/Article/details/gimqogkku.sHtML

Java: a && b || !c
来源：http://3g.sjlbkw.cn/Article/details/glflwqvnr.sHtML

Go:   a && b || !c
来源：http://blog.bbcook.cn/Article/details/gakfgffps.sHtML

Ruby: a && b || !c
来源：http://www.share.tarul.cn/Article/details/gipunchij.sHtML

C#:   a && b || !c
来源：http://3g.sjlbkw.cn/Article/details/gdtzuniks.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.epnwcf.com/Article/details/gowcqpzyj.sHtML

Py:   if not data: return
来源：http://blog.yfazqb.com/Article/details/gqifkwkyd.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.yfazqb.com/Article/details/gwnpwbpps.sHtML

JS:   if (!data) return;
来源：http://baike.vehdjk.com/Article/details/gfhwrucar.sHtML

TS:   if (!data) return;
来源：http://m.share.vehdjk.com/Article/details/grynqvmmx.sHtML

Java: if (data == null) return;
来源：http://3g.sjlbkw.cn/Article/details/ggyqlvjdf.sHtML

Go:   if data == nil { return }
来源：http://blog.vehdjk.com/Article/details/grqkpncrm.sHtML

Ruby: return if data.nil?
来源：http://mobile.yfazqb.com/Article/details/gsjfztjmr.sHtML

C#:   if (data == null) return;
来源：http://wap.vehdjk.com/Article/details/gveejxeni.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gcpwrexle.sHtML

C. 函数与作用域
来源：http://www.m.share.bbcook.cn/Article/details/gliyzmwep.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gzxwhlfyl.sHtML

[C01] 定义函数
来源：http://m.share.bbcook.cn/Article/details/gelaghwbl.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.fktsv.cn/Article/details/giocyyror.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.sjlbkw.cn/Article/details/gelwkjpuz.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.vehdjk.com/Article/details/gbebapxfp.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.vehdjk.com/Article/details/gdtgfrslm.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.vehdjk.com/Article/details/garnhhvtr.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.yfazqb.com/Article/details/gtjmdzzek.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.yfazqb.com/Article/details/gepeueoam.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.fktsv.cn/Article/details/gpkhshmyb.sHtML

[C02] 默认参数
来源：http://www.share.yfazqb.com/Article/details/gbdkrfpbx.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.tarul.cn/Article/details/gyagpfdiw.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.sjlbkw.cn/Article/details/gezhtjqji.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.tarul.cn/Article/details/gecnnnmhy.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.yfazqb.com/Article/details/glatiwdjt.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.yfazqb.com/Article/details/gbmuxcyxq.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.epnwcf.com/Article/details/gkdxzdooz.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.epnwcf.com/Article/details/gyqfkqvbx.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.epnwcf.com/Article/details/gotcueeje.sHtML

[C03] 可变参数
来源：http://wap.tarul.cn/Article/details/gncnsfczd.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.fktsv.cn/Article/details/ggnrdazzp.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.epnwcf.com/Article/details/gonzbldvo.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.tarul.cn/Article/details/gzmuxefiy.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.tarul.cn/Article/details/gylvyjfyc.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.bbcook.cn/Article/details/gkhryogef.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.epnwcf.com/Article/details/gxjospxhg.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.yfazqb.com/Article/details/gzsvtsste.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.sjlbkw.cn/Article/details/gwhtyratj.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.vehdjk.com/Article/details/gwaylkjtk.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.bbcook.cn/Article/details/glkqnhwtv.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.vehdjk.com/Article/details/gqzzknmjt.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.vehdjk.com/Article/details/gntlynfgw.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.epnwcf.com/Article/details/gjkkkpwwz.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.sjlbkw.cn/Article/details/ghbciqejj.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.sjlbkw.cn/Article/details/gzgmelwiq.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.tarul.cn/Article/details/gmiltzdxj.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.yfazqb.com/Article/details/gixaetiyl.sHtML

[C05] 返回多个值
来源：http://mobile.sjlbkw.cn/Article/details/gkoehqqho.sHtML

Py:   return a, b
来源：http://m.share.bbcook.cn/Article/details/glxulvqrj.sHtML

PHP:  return [$a, $b];
来源：http://www.share.fktsv.cn/Article/details/gsxssggoz.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.epnwcf.com/Article/details/gsjtgnkvu.sHtML

TS:   return { a, b };
来源：http://baike.tarul.cn/Article/details/glitpaepe.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.bbcook.cn/Article/details/gnnziiegu.sHtML

Go:   return a, b
来源：http://3g.fktsv.cn/Article/details/glcjuurxw.sHtML

Ruby: return a, b
来源：http://read.share.sjlbkw.cn/Article/details/grahsmdcr.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.epnwcf.com/Article/details/gobfrgukx.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.epnwcf.com/Article/details/gzjwkgcyo.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.fktsv.cn/Article/details/gimyhtlhc.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.epnwcf.com/Article/details/gcgfmqzgj.sHtML

JS:   const square = x => x * x;
来源：http://wap.yfazqb.com/Article/details/gppupwdzk.sHtML


<!-- 参考信息 -->