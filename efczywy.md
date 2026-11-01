代发 wailian999

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://3g.yfazqb.com/Article/details/gyzpecgit.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://read.share.yfazqb.com/Article/details/guugljbiu.sHtML

TS:   if (!x) {}
来源：http://mobile.sjlbkw.cn/Article/details/gehqccsuw.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://baike.fktsv.cn/Article/details/gblorstvr.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://baike.vehdjk.com/Article/details/geljldfqq.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.m.share.epnwcf.com/Article/details/gzhyeoklv.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.blog.bbcook.cn/Article/details/gpztdgffq.sHtML

[A17] 位运算
来源：http://mobile.fktsv.cn/Article/details/gyhuwylql.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.fktsv.cn/Article/details/gouvcrlfc.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://m.share.vehdjk.com/Article/details/gvlmnfuxz.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fktsv.cn/Article/details/gsccdvqkz.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://3g.yfazqb.com/Article/details/gxuybiage.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.epnwcf.com/Article/details/gjfxqhfbf.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.m.share.sjlbkw.cn/Article/details/ggmfvhspe.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.yfazqb.com/Article/details/gdjtwywlh.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.tarul.cn/Article/details/gnmcttrxi.sHtML

[A18] 字符与 ASCII 码互转
来源：http://3g.epnwcf.com/Article/details/gavktnxlv.sHtML

Py:   ord("A"); chr(65)
来源：http://read.share.vehdjk.com/Article/details/gugaoiyxp.sHtML

PHP:  ord("A"); chr(65)
来源：http://blog.vehdjk.com/Article/details/gefrtbufg.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.vehdjk.com/Article/details/gvpmfddfv.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.sjlbkw.cn/Article/details/gfrtnefsi.sHtML

Java: (int) 'A'; (char) 65
来源：http://blog.fktsv.cn/Article/details/gzzniualz.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://baike.yfazqb.com/Article/details/gulohkdvv.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.m.share.sjlbkw.cn/Article/details/gyqvcwoqe.sHtML

C#:   (int)'A'; (char)65
来源：http://baike.tarul.cn/Article/details/gqekmslwu.sHtML

[A19] 交换两个变量
来源：http://mobile.vehdjk.com/Article/details/gidadizhn.sHtML

Py:   a, b = b, a
来源：http://blog.fktsv.cn/Article/details/gyvighthm.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://mobile.vehdjk.com/Article/details/gmpyxlhem.sHtML

JS:   [a, b] = [b, a];
来源：http://wap.bbcook.cn/Article/details/gkecqgjyn.sHtML

TS:   [a, b] = [b, a];
来源：http://m.share.vehdjk.com/Article/details/gjldmhqpv.sHtML

Java: int t = a; a = b; b = t;
来源：http://mobile.tarul.cn/Article/details/gxnooslvb.sHtML

Go:   a, b = b, a
来源：http://www.blog.tarul.cn/Article/details/gfpsambpg.sHtML

Ruby: a, b = b, a
来源：http://m.share.vehdjk.com/Article/details/gpaubtjxi.sHtML

C#:   (a, b) = (b, a);
来源：http://wap.bbcook.cn/Article/details/gxxqltkrn.sHtML

[A20] 读取标准输入
来源：http://wap.sjlbkw.cn/Article/details/gjmhhgsby.sHtML

Py:   name = input("请输入：")
来源：http://wap.yfazqb.com/Article/details/gofpjhqdt.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://blog.sjlbkw.cn/Article/details/gqwjaufyg.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://m.share.tarul.cn/Article/details/guctwtptx.sHtML

TS:   // Node.js：readline 模块
来源：http://3g.fktsv.cn/Article/details/goimuwsfh.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://blog.yfazqb.com/Article/details/ghcdwxzjg.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://baike.yfazqb.com/Article/details/gevfykdyk.sHtML

Ruby: gets.chomp
来源：http://3g.sjlbkw.cn/Article/details/gtuyavuxk.sHtML

C#:   Console.ReadLine();
来源：http://baike.tarul.cn/Article/details/gbujsgggl.sHtML

[A21] 保留指定小数位输出
来源：http://read.share.vehdjk.com/Article/details/gcmocluln.sHtML

Py:   f"{3.14159:.2f}"
来源：http://mobile.bbcook.cn/Article/details/ggsghzfmi.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.blog.epnwcf.com/Article/details/gwzzqudme.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.share.yfazqb.com/Article/details/gtnlekzoz.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.share.tarul.cn/Article/details/gmlfmcaen.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://baike.sjlbkw.cn/Article/details/giitadfqr.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://m.share.epnwcf.com/Article/details/gxfgtoreo.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.blog.vehdjk.com/Article/details/gxauefjdb.sHtML

C#:   3.14159.ToString("F2")
来源：http://3g.epnwcf.com/Article/details/grwtcfdnk.sHtML

[A22] 获取字符串长度
来源：http://m.share.sjlbkw.cn/Article/details/gkuhpmqtw.sHtML

Py:   len(s)
来源：http://wap.bbcook.cn/Article/details/gzkmmwrno.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://m.share.sjlbkw.cn/Article/details/golxqqtzl.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wap.epnwcf.com/Article/details/gousfuxgv.sHtML

TS:   s.length
来源：http://mobile.epnwcf.com/Article/details/gvduqvirs.sHtML

Java: s.length()
来源：http://m.share.sjlbkw.cn/Article/details/gpryvyunt.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://m.share.fktsv.cn/Article/details/guhqsfsbk.sHtML

Ruby: s.length
来源：http://m.share.epnwcf.com/Article/details/gkbkwwuqy.sHtML

C#:   s.Length
来源：http://www.share.yfazqb.com/Article/details/gwtnyvqyh.sHtML

[A23] 大小写转换
来源：http://www.m.share.sjlbkw.cn/Article/details/gjlejmbrf.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://mobile.sjlbkw.cn/Article/details/gluioergy.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.blog.tarul.cn/Article/details/gtrzxgmwr.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.epnwcf.com/Article/details/gncgjezhi.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.fktsv.cn/Article/details/guldqjfkq.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://blog.vehdjk.com/Article/details/gplloajbf.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://baike.vehdjk.com/Article/details/gcongecsa.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://baike.fktsv.cn/Article/details/gtohpvbzo.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.m.share.fktsv.cn/Article/details/ghuwhpqhl.sHtML

[A24] 去除首尾空白
来源：http://m.share.vehdjk.com/Article/details/gynnwpoau.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://blog.vehdjk.com/Article/details/gzajzrlim.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.blog.tarul.cn/Article/details/gncyyawug.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.tarul.cn/Article/details/gqsrjuniq.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.yfazqb.com/Article/details/gmrzhexty.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://m.share.tarul.cn/Article/details/gksmjubfo.sHtML

Go:   strings.TrimSpace(s)
来源：http://mobile.tarul.cn/Article/details/gmdehnaki.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://read.share.tarul.cn/Article/details/gfwvgsoxk.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://baike.sjlbkw.cn/Article/details/gbhxftfdg.sHtML

[A25] 字符串比较
来源：http://www.m.share.bbcook.cn/Article/details/gpmuphbew.sHtML

Py:   s1 == s2; s1 != s2
来源：http://mobile.bbcook.cn/Article/details/gxhrphalj.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mobile.yfazqb.com/Article/details/galgntnus.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.epnwcf.com/Article/details/gyanjstkb.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.epnwcf.com/Article/details/gewzzthog.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wap.epnwcf.com/Article/details/geumhdhxh.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wap.sjlbkw.cn/Article/details/gnosmnpec.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://m.share.tarul.cn/Article/details/gloejyejx.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.m.share.fktsv.cn/Article/details/gxjfqraoh.sHtML

[A26] 类型转换总览
来源：http://m.share.epnwcf.com/Article/details/gvnmutkqi.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wap.tarul.cn/Article/details/ggpjmzxpv.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wap.sjlbkw.cn/Article/details/gnbxnutbw.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://3g.epnwcf.com/Article/details/gpgkvyeaj.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.m.share.epnwcf.com/Article/details/gnpbznrvv.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://read.share.fktsv.cn/Article/details/gmrnqbopt.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wap.vehdjk.com/Article/details/gfecnhcgw.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.share.vehdjk.com/Article/details/gfmmhblmu.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wap.bbcook.cn/Article/details/gbeipnaxp.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gnnhldmhk.sHtML

B. 流程控制
来源：http://wap.sjlbkw.cn/Article/details/grushkqct.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gudizvjyt.sHtML

[B01] 条件判断 if / else
来源：http://baike.sjlbkw.cn/Article/details/ghgsbsdnb.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://wap.fktsv.cn/Article/details/gweokugbb.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://blog.sjlbkw.cn/Article/details/gsnaibfdm.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.yfazqb.com/Article/details/gstezzzuj.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.epnwcf.com/Article/details/glyxzdhxr.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.blog.epnwcf.com/Article/details/gybxwycey.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://3g.vehdjk.com/Article/details/ghtvblyun.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://read.share.bbcook.cn/Article/details/gocvfuudn.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wap.fktsv.cn/Article/details/ggtthjgsy.sHtML

[B02] 多分支 else if / elif
来源：http://wap.bbcook.cn/Article/details/gwmjdxwzl.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://3g.vehdjk.com/Article/details/gomfbzjwx.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.share.yfazqb.com/Article/details/gvejmjyyl.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.tarul.cn/Article/details/gbyvshlzh.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.tarul.cn/Article/details/gggheiasg.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.epnwcf.com/Article/details/goeuothul.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wap.vehdjk.com/Article/details/gkpyqdyak.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://read.share.fktsv.cn/Article/details/gyyrrxjxa.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.bbcook.cn/Article/details/gohpaiwvs.sHtML

[B03] switch / match / case
来源：http://m.share.yfazqb.com/Article/details/gxjopjryp.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.share.tarul.cn/Article/details/gwuizorxu.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://m.share.vehdjk.com/Article/details/gjkhqflje.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.vehdjk.com/Article/details/gjouqpvku.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.tarul.cn/Article/details/ghjxjxlrq.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://blog.yfazqb.com/Article/details/gnqwrhyix.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://blog.epnwcf.com/Article/details/gdwnwhevt.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://blog.bbcook.cn/Article/details/glsdrvxbg.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://blog.epnwcf.com/Article/details/gchqwwcdu.sHtML

[B04] for 计数循环
来源：http://3g.fktsv.cn/Article/details/gcfwthsuu.sHtML

Py:   for i in range(10): print(i)
来源：http://www.m.share.fktsv.cn/Article/details/gfpkpbiyl.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.share.epnwcf.com/Article/details/gntcemvpn.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.sjlbkw.cn/Article/details/gdtdcwgqb.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.fktsv.cn/Article/details/gkcfpllgz.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.vehdjk.com/Article/details/geshfryfa.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.blog.vehdjk.com/Article/details/glcqtpydw.sHtML

Ruby: 10.times { |i| puts i }
来源：http://baike.epnwcf.com/Article/details/ghxwczzbb.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://baike.fktsv.cn/Article/details/gosftotib.sHtML

[B05] 遍历数组 / 列表
来源：http://baike.vehdjk.com/Article/details/giylrsdqf.sHtML

Py:   for item in arr: print(item)
来源：http://www.blog.vehdjk.com/Article/details/gyhurgxgp.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.epnwcf.com/Article/details/gbpgbwelm.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://blog.epnwcf.com/Article/details/gnvjcjqbg.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://wap.bbcook.cn/Article/details/gggdrqdla.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.share.epnwcf.com/Article/details/gxazfuexy.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://3g.vehdjk.com/Article/details/gkbgfxndt.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.tarul.cn/Article/details/gpsaoldjz.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.vehdjk.com/Article/details/gsgkuofjw.sHtML

[B06] 遍历字典 / 对象
来源：http://m.share.yfazqb.com/Article/details/gyorwikdc.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.bbcook.cn/Article/details/gbdzlnahk.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mobile.yfazqb.com/Article/details/guguwznyc.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.bbcook.cn/Article/details/gzcwsaiek.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.epnwcf.com/Article/details/gvhufkrlj.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.share.vehdjk.com/Article/details/ggvqrhhlj.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wap.epnwcf.com/Article/details/gurqvuufu.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.blog.fktsv.cn/Article/details/gadunwukr.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mobile.epnwcf.com/Article/details/gwbirqffb.sHtML

[B07] while 循环
来源：http://wap.sjlbkw.cn/Article/details/gqrklboxv.sHtML

Py:   while i < 10: i += 1
来源：http://m.share.vehdjk.com/Article/details/gbzxmiulz.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.share.epnwcf.com/Article/details/gujtdfoya.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.sjlbkw.cn/Article/details/gwtqynwhz.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.epnwcf.com/Article/details/gximihsar.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.vehdjk.com/Article/details/gdamqgcrm.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.bbcook.cn/Article/details/gzjqagvlc.sHtML

Ruby: while i < 10; i += 1; end
来源：http://m.share.sjlbkw.cn/Article/details/gejgiexwd.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.sjlbkw.cn/Article/details/gfqwqvwpb.sHtML

[B08] do-while（至少执行一次）
来源：http://m.share.yfazqb.com/Article/details/gutrcrwhw.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://mobile.yfazqb.com/Article/details/giornuwvs.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.tarul.cn/Article/details/gktpygcsq.sHtML

JS:   do { i++; } while (i < 10);
来源：http://baike.bbcook.cn/Article/details/gfuoqbdgq.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.m.share.tarul.cn/Article/details/gocjzfepp.sHtML

Java: do { i++; } while (i < 10);
来源：http://mobile.vehdjk.com/Article/details/gdfmnuhjl.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.tarul.cn/Article/details/gawgheytl.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.tarul.cn/Article/details/gfelxuzqj.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.epnwcf.com/Article/details/gsitwzlqq.sHtML

[B09] break 与 continue
来源：http://www.m.share.sjlbkw.cn/Article/details/gwzsimnim.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.bbcook.cn/Article/details/golenflxd.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.vehdjk.com/Article/details/ghykhwzuu.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.vehdjk.com/Article/details/gnitkcsgg.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.yfazqb.com/Article/details/gerytevtz.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.sjlbkw.cn/Article/details/gxbhtrals.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.bbcook.cn/Article/details/gdljznbei.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.bbcook.cn/Article/details/gqnwnvvpn.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.bbcook.cn/Article/details/gsdcwnoqb.sHtML

[B10] 遍历同时拿索引
来源：http://blog.sjlbkw.cn/Article/details/gcbjqtwnz.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.tarul.cn/Article/details/gsglatpai.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.sjlbkw.cn/Article/details/gkumuqalm.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.sjlbkw.cn/Article/details/gtsrciaow.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.vehdjk.com/Article/details/gmcozzbjq.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.vehdjk.com/Article/details/grzffwlok.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.epnwcf.com/Article/details/gyfcmzxeu.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.vehdjk.com/Article/details/gxmsmvkhv.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.tarul.cn/Article/details/gqumxbkqh.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.epnwcf.com/Article/details/gxtknnihg.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.epnwcf.com/Article/details/gqtdmbsdh.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.tarul.cn/Article/details/gsmgvfacw.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.bbcook.cn/Article/details/gusshijnu.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.vehdjk.com/Article/details/gigzahawj.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.fktsv.cn/Article/details/gntlboumb.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.yfazqb.com/Article/details/gynqnrzls.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.vehdjk.com/Article/details/gudkznfcw.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.vehdjk.com/Article/details/giclvfrhu.sHtML

[B12] 跳出多层循环
来源：http://m.share.tarul.cn/Article/details/gisngfdmx.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.yfazqb.com/Article/details/gnjfoqatu.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.fktsv.cn/Article/details/goapchubq.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.sjlbkw.cn/Article/details/gywrvlios.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.bbcook.cn/Article/details/gyotzfbhm.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.bbcook.cn/Article/details/gqmzanvco.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.vehdjk.com/Article/details/gzlwxrccb.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.vehdjk.com/Article/details/gardpbnjy.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.sjlbkw.cn/Article/details/ggajtdoib.sHtML

[B13] 判断是否为数字
来源：http://m.share.tarul.cn/Article/details/gnuzodetk.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.bbcook.cn/Article/details/gjmzvzgcg.sHtML

PHP:  is_numeric($x)
来源：http://baike.vehdjk.com/Article/details/geqjpsuab.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.fktsv.cn/Article/details/gpfcdtdrb.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.sjlbkw.cn/Article/details/gvnaafhhf.sHtML

Java: x instanceof Number
来源：http://www.share.tarul.cn/Article/details/gqbllspnp.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.bbcook.cn/Article/details/gptynuwjd.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.yfazqb.com/Article/details/gkaqqwczn.sHtML

C#:   x is int or double or decimal
来源：http://mobile.sjlbkw.cn/Article/details/gcttbmetx.sHtML

[B14] 判断值是否在集合内
来源：http://wap.yfazqb.com/Article/details/gbhwerftc.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.sjlbkw.cn/Article/details/guyktjfhq.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.yfazqb.com/Article/details/gqglegsko.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.epnwcf.com/Article/details/gpzngmoaf.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.yfazqb.com/Article/details/golaprlji.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.sjlbkw.cn/Article/details/goiesufjd.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.fktsv.cn/Article/details/gyhjxfhrt.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.epnwcf.com/Article/details/gutxtywgs.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.yfazqb.com/Article/details/gpxbqkrnk.sHtML

[B15] 布尔运算与取反
来源：http://wap.yfazqb.com/Article/details/gnumhcayt.sHtML

Py:   a and b or not c
来源：http://wap.vehdjk.com/Article/details/gszdxilio.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.tarul.cn/Article/details/gifugfarb.sHtML

JS:   a && b || !c
来源：http://m.share.vehdjk.com/Article/details/gfiokxace.sHtML

TS:   a && b || !c
来源：http://3g.tarul.cn/Article/details/gsftuauab.sHtML

Java: a && b || !c
来源：http://read.share.tarul.cn/Article/details/grssaxqcd.sHtML

Go:   a && b || !c
来源：http://blog.yfazqb.com/Article/details/gzyvaopos.sHtML

Ruby: a && b || !c
来源：http://3g.epnwcf.com/Article/details/gjynnexnq.sHtML

C#:   a && b || !c
来源：http://wap.tarul.cn/Article/details/gabsexnko.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.epnwcf.com/Article/details/glvygeiqs.sHtML

Py:   if not data: return
来源：http://blog.sjlbkw.cn/Article/details/gbdqnuepi.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.vehdjk.com/Article/details/gyxhukqyf.sHtML

JS:   if (!data) return;
来源：http://baike.tarul.cn/Article/details/gortjongt.sHtML

TS:   if (!data) return;
来源：http://wap.tarul.cn/Article/details/gonrfpnky.sHtML

Java: if (data == null) return;
来源：http://mobile.yfazqb.com/Article/details/glzfoivrb.sHtML

Go:   if data == nil { return }
来源：http://3g.tarul.cn/Article/details/gpzzlfmih.sHtML

Ruby: return if data.nil?
来源：http://read.share.yfazqb.com/Article/details/gtfwrsyrk.sHtML

C#:   if (data == null) return;
来源：http://3g.tarul.cn/Article/details/gjewtbcin.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gduvfpeck.sHtML

C. 函数与作用域
来源：http://read.share.bbcook.cn/Article/details/gnumgtpyg.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gmoqyyfqh.sHtML

[C01] 定义函数
来源：http://www.blog.sjlbkw.cn/Article/details/gnwbzjkvj.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.tarul.cn/Article/details/gffuqzpwz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.bbcook.cn/Article/details/grwczzukw.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.fktsv.cn/Article/details/gbrzulklk.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.bbcook.cn/Article/details/gldevliju.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.vehdjk.com/Article/details/gnjzpnzai.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.sjlbkw.cn/Article/details/ghurfavte.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.tarul.cn/Article/details/gdlvaibvd.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.epnwcf.com/Article/details/gyozogozr.sHtML

[C02] 默认参数
来源：http://www.share.epnwcf.com/Article/details/glfeidlei.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.fktsv.cn/Article/details/gnpnmioqo.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.tarul.cn/Article/details/geeminkgl.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.vehdjk.com/Article/details/gfptmwfup.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.yfazqb.com/Article/details/gmntjzqtt.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.tarul.cn/Article/details/gsjtskqck.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.epnwcf.com/Article/details/gcwalfusu.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.fktsv.cn/Article/details/goebdcxgz.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.sjlbkw.cn/Article/details/gnqdndcaa.sHtML

[C03] 可变参数
来源：http://www.blog.bbcook.cn/Article/details/gmtvsmpaz.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.epnwcf.com/Article/details/gtelpgibd.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.tarul.cn/Article/details/gxgbetdpf.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.bbcook.cn/Article/details/grkksgcok.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.tarul.cn/Article/details/giujjdkxt.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.fktsv.cn/Article/details/gcvsovkog.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.vehdjk.com/Article/details/gezpvxmwi.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.fktsv.cn/Article/details/goqtcwhoa.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.vehdjk.com/Article/details/gaboxiloy.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.fktsv.cn/Article/details/giqkmcusc.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.epnwcf.com/Article/details/gvisjxxgn.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.vehdjk.com/Article/details/guhohblty.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.fktsv.cn/Article/details/gzhvmnqcg.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.tarul.cn/Article/details/gtljkyeen.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.tarul.cn/Article/details/ghlowudbi.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.bbcook.cn/Article/details/gblhmhwaf.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.fktsv.cn/Article/details/guyprjduf.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.fktsv.cn/Article/details/gcsgyqaer.sHtML

[C05] 返回多个值
来源：http://www.blog.fktsv.cn/Article/details/gwwnsbvil.sHtML

Py:   return a, b
来源：http://3g.bbcook.cn/Article/details/gjyxmcdzk.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.yfazqb.com/Article/details/gehuhotrt.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.epnwcf.com/Article/details/giggxbesi.sHtML

TS:   return { a, b };
来源：http://mobile.yfazqb.com/Article/details/gpgusnlcm.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.bbcook.cn/Article/details/grbltafxx.sHtML

Go:   return a, b
来源：http://www.blog.vehdjk.com/Article/details/gmpmbngoi.sHtML

Ruby: return a, b
来源：http://m.share.tarul.cn/Article/details/gpkvzniso.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.bbcook.cn/Article/details/gaxgmtazp.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.sjlbkw.cn/Article/details/gwijimnus.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.sjlbkw.cn/Article/details/gvwgpdnfk.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.yfazqb.com/Article/details/gnnzcqvvn.sHtML

JS:   const square = x => x * x;
来源：http://3g.tarul.cn/Article/details/glkhnrelg.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.tarul.cn/Article/details/gbrpvxkap.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.tarul.cn/Article/details/guypeidys.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.sjlbkw.cn/Article/details/gxldbyaeh.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.yfazqb.com/Article/details/gldbecmei.sHtML


<!-- 参考信息 -->