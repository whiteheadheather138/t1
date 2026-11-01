代发 wailian999

JS:   const value = data ?? "默认值";
来源：http://www.m.share.vehdjk.com/Article/details/gagdqwfgt.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.share.yfazqb.com/Article/details/gfwrqvubt.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.share.tarul.cn/Article/details/gkkutwgyv.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://mobile.bbcook.cn/Article/details/gnmxxogvx.sHtML

Ruby: value = data || "默认值"
来源：http://mobile.bbcook.cn/Article/details/gdvtlmoan.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.blog.yfazqb.com/Article/details/ghtziooqx.sHtML

[A16] 真假值判断规则
来源：http://mobile.sjlbkw.cn/Article/details/gxscdvotm.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://read.share.vehdjk.com/Article/details/gkfzlqkap.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.m.share.vehdjk.com/Article/details/gzasudxqp.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://baike.sjlbkw.cn/Article/details/gtmzaftqs.sHtML

TS:   if (!x) {}
来源：http://wap.epnwcf.com/Article/details/gebuipyci.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://m.share.yfazqb.com/Article/details/gdzsadhno.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.blog.fktsv.cn/Article/details/gjbauwgps.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://baike.bbcook.cn/Article/details/ghedtihrs.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://read.share.yfazqb.com/Article/details/gwmqxhgef.sHtML

[A17] 位运算
来源：http://mobile.yfazqb.com/Article/details/gvcngaywt.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.bbcook.cn/Article/details/grprisbzb.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.share.tarul.cn/Article/details/ggzcafdoi.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.epnwcf.com/Article/details/gepnpgajn.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.blog.tarul.cn/Article/details/glleypyeo.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.tarul.cn/Article/details/ggiyiuwkv.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://mobile.fktsv.cn/Article/details/gqjrkbdbl.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.vehdjk.com/Article/details/gqvbwvdyh.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.yfazqb.com/Article/details/gahkmnfrk.sHtML

[A18] 字符与 ASCII 码互转
来源：http://wap.vehdjk.com/Article/details/gktxzfggc.sHtML

Py:   ord("A"); chr(65)
来源：http://mobile.fktsv.cn/Article/details/grdqjsncf.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.m.share.vehdjk.com/Article/details/gmasogvfm.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfolirqft.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.m.share.yfazqb.com/Article/details/ghquiwhez.sHtML

Java: (int) 'A'; (char) 65
来源：http://read.share.yfazqb.com/Article/details/gjnfxzbzl.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://baike.tarul.cn/Article/details/gtkphqcjk.sHtML

Ruby: "A".ord; 65.chr
来源：http://mobile.epnwcf.com/Article/details/gsolqgxdf.sHtML

C#:   (int)'A'; (char)65
来源：http://read.share.epnwcf.com/Article/details/gnmwxcjzd.sHtML

[A19] 交换两个变量
来源：http://blog.yfazqb.com/Article/details/ghjvrutjx.sHtML

Py:   a, b = b, a
来源：http://wap.epnwcf.com/Article/details/glyceydyo.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.share.yfazqb.com/Article/details/gbrchztqo.sHtML

JS:   [a, b] = [b, a];
来源：http://m.share.vehdjk.com/Article/details/gmykqogjf.sHtML

TS:   [a, b] = [b, a];
来源：http://www.m.share.sjlbkw.cn/Article/details/gisvzhcpv.sHtML

Java: int t = a; a = b; b = t;
来源：http://3g.bbcook.cn/Article/details/gwppleexj.sHtML

Go:   a, b = b, a
来源：http://www.m.share.vehdjk.com/Article/details/gxayajbfw.sHtML

Ruby: a, b = b, a
来源：http://baike.epnwcf.com/Article/details/goifotyeb.sHtML

C#:   (a, b) = (b, a);
来源：http://www.share.sjlbkw.cn/Article/details/gzykepcfp.sHtML

[A20] 读取标准输入
来源：http://m.share.sjlbkw.cn/Article/details/gzfbmjjrv.sHtML

Py:   name = input("请输入：")
来源：http://www.m.share.epnwcf.com/Article/details/golepbswy.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.m.share.yfazqb.com/Article/details/grsjhvbyx.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://read.share.epnwcf.com/Article/details/gupjlqawq.sHtML

TS:   // Node.js：readline 模块
来源：http://read.share.epnwcf.com/Article/details/ghfqqghbh.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.blog.bbcook.cn/Article/details/gifhjjqon.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.blog.bbcook.cn/Article/details/gsexaffuo.sHtML

Ruby: gets.chomp
来源：http://3g.yfazqb.com/Article/details/gogslaypb.sHtML

C#:   Console.ReadLine();
来源：http://baike.fktsv.cn/Article/details/gichmsumv.sHtML

[A21] 保留指定小数位输出
来源：http://read.share.sjlbkw.cn/Article/details/gosmmwmiu.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.share.vehdjk.com/Article/details/gvoptgsui.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.share.bbcook.cn/Article/details/gewzfsqwn.sHtML

JS:   (3.14159).toFixed(2)
来源：http://3g.yfazqb.com/Article/details/gmetllwmz.sHtML

TS:   (3.14159).toFixed(2)
来源：http://read.share.bbcook.cn/Article/details/gqmxgluqp.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.m.share.epnwcf.com/Article/details/gmkqbrriw.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.blog.yfazqb.com/Article/details/gcwanodmf.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://3g.sjlbkw.cn/Article/details/gimqulrmp.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.m.share.epnwcf.com/Article/details/gborlaqza.sHtML

[A22] 获取字符串长度
来源：http://m.share.sjlbkw.cn/Article/details/gznnfomtb.sHtML

Py:   len(s)
来源：http://3g.yfazqb.com/Article/details/gsoefwuda.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mobile.sjlbkw.cn/Article/details/gaimpbxwc.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.share.yfazqb.com/Article/details/gikhucggk.sHtML

TS:   s.length
来源：http://wap.epnwcf.com/Article/details/gtlkcvsyl.sHtML

Java: s.length()
来源：http://www.share.sjlbkw.cn/Article/details/gqbzomypz.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://m.share.yfazqb.com/Article/details/gbizzsyjo.sHtML

Ruby: s.length
来源：http://www.blog.bbcook.cn/Article/details/gtfrnwyvs.sHtML

C#:   s.Length
来源：http://baike.sjlbkw.cn/Article/details/gpapwiuwh.sHtML

[A23] 大小写转换
来源：http://3g.vehdjk.com/Article/details/gmoexopuc.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.m.share.epnwcf.com/Article/details/gfuhzesdg.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://3g.tarul.cn/Article/details/gbtytqakf.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.sjlbkw.cn/Article/details/gjfkxuqlk.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.vehdjk.com/Article/details/ghckatbzb.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://m.share.sjlbkw.cn/Article/details/gqwvzvgmi.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.blog.bbcook.cn/Article/details/gxfzxgpqg.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://blog.tarul.cn/Article/details/gbkislcnr.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.blog.tarul.cn/Article/details/gfmzfshdo.sHtML

[A24] 去除首尾空白
来源：http://www.share.tarul.cn/Article/details/gxzxbrarl.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.m.share.sjlbkw.cn/Article/details/gcckapncl.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://m.share.fktsv.cn/Article/details/guvmvrowr.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.yfazqb.com/Article/details/gymzbgrqm.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.epnwcf.com/Article/details/gkqldxqic.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.blog.yfazqb.com/Article/details/gnjhguqpv.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.share.vehdjk.com/Article/details/gyppwspud.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mobile.bbcook.cn/Article/details/gkyyvxjxg.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://read.share.fktsv.cn/Article/details/gsoizphbz.sHtML

[A25] 字符串比较
来源：http://blog.vehdjk.com/Article/details/gmppsfdtd.sHtML

Py:   s1 == s2; s1 != s2
来源：http://m.share.yfazqb.com/Article/details/gpplqpuac.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://read.share.fktsv.cn/Article/details/gihzeiqpm.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.vehdjk.com/Article/details/gyyulayzb.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.fktsv.cn/Article/details/giaimfojc.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.share.epnwcf.com/Article/details/gzwhamxcn.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://m.share.yfazqb.com/Article/details/ggaabnisp.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.share.tarul.cn/Article/details/gmuskwhxo.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.blog.yfazqb.com/Article/details/gxydrtfsg.sHtML

[A26] 类型转换总览
来源：http://blog.epnwcf.com/Article/details/gthjgmgbp.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.m.share.bbcook.cn/Article/details/gnafwiiyv.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.blog.epnwcf.com/Article/details/gachbqjyz.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://m.share.yfazqb.com/Article/details/gsimzzwbw.sHtML

TS:   Number() String() Boolean() x as number
来源：http://mobile.fktsv.cn/Article/details/gcamiqeew.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://baike.bbcook.cn/Article/details/gzwyckosc.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.share.fktsv.cn/Article/details/gwlooknxe.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://baike.sjlbkw.cn/Article/details/ggvdbffvp.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.m.share.bbcook.cn/Article/details/gvoxcngyf.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gaeecjkjc.sHtML

B. 流程控制
来源：http://mobile.vehdjk.com/Article/details/gcyvieqsd.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gdkbxvksi.sHtML

[B01] 条件判断 if / else
来源：http://www.share.epnwcf.com/Article/details/gtsqnmmgp.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.blog.bbcook.cn/Article/details/gftfrjvet.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.share.sjlbkw.cn/Article/details/gbunutndw.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.vehdjk.com/Article/details/gsaiwtybi.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.tarul.cn/Article/details/gtnijosig.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://wap.vehdjk.com/Article/details/gmegkigmw.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.m.share.epnwcf.com/Article/details/gmftjtsxf.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.share.epnwcf.com/Article/details/gnyvqhemo.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://read.share.epnwcf.com/Article/details/ghrhruypa.sHtML

[B02] 多分支 else if / elif
来源：http://m.share.vehdjk.com/Article/details/gagijvwko.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://m.share.fktsv.cn/Article/details/gjnwiyzsh.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://3g.yfazqb.com/Article/details/grgtfmodi.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.yfazqb.com/Article/details/ghsamdfzm.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.epnwcf.com/Article/details/gkhbxvhqg.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.epnwcf.com/Article/details/gombeqrof.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.share.vehdjk.com/Article/details/gvawnfppo.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.m.share.vehdjk.com/Article/details/gtsklibuk.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.yfazqb.com/Article/details/gcuvztgqc.sHtML

[B03] switch / match / case
来源：http://mobile.epnwcf.com/Article/details/gvevxpxes.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://read.share.bbcook.cn/Article/details/giogxregv.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.share.tarul.cn/Article/details/gjbwwnsav.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.yfazqb.com/Article/details/gmyrikzqu.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.tarul.cn/Article/details/gqddgyvbo.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.m.share.tarul.cn/Article/details/ggymosabp.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://m.share.tarul.cn/Article/details/gfnuorcyj.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wap.epnwcf.com/Article/details/gphnibovj.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.blog.sjlbkw.cn/Article/details/geouwgwwb.sHtML

[B04] for 计数循环
来源：http://3g.fktsv.cn/Article/details/gyxqusxsr.sHtML

Py:   for i in range(10): print(i)
来源：http://3g.sjlbkw.cn/Article/details/gergnpvev.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.share.epnwcf.com/Article/details/gvlloiige.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.epnwcf.com/Article/details/gzmzfkyju.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.fktsv.cn/Article/details/grscgfwhu.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://read.share.epnwcf.com/Article/details/gtieettog.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wap.epnwcf.com/Article/details/gceqkccug.sHtML

Ruby: 10.times { |i| puts i }
来源：http://baike.epnwcf.com/Article/details/gailrknzk.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mobile.sjlbkw.cn/Article/details/gqofjqrsn.sHtML

[B05] 遍历数组 / 列表
来源：http://www.m.share.bbcook.cn/Article/details/gbtbvymac.sHtML

Py:   for item in arr: print(item)
来源：http://mobile.yfazqb.com/Article/details/gzuqfmjjf.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://read.share.epnwcf.com/Article/details/gbgqylzyn.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.vehdjk.com/Article/details/gykqfdaka.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.share.tarul.cn/Article/details/gdbdbbbhg.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://baike.fktsv.cn/Article/details/gymczkwqm.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://m.share.sjlbkw.cn/Article/details/gbhoucxaq.sHtML

Ruby: arr.each { |item| puts item }
来源：http://baike.bbcook.cn/Article/details/gvemydyzr.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.m.share.fktsv.cn/Article/details/gyivsmdnf.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.epnwcf.com/Article/details/ggiepwbyw.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.tarul.cn/Article/details/gifmkvirh.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.m.share.yfazqb.com/Article/details/grfyhlfgb.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.yfazqb.com/Article/details/gvsvyilxm.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.bbcook.cn/Article/details/gvrjzwisg.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mobile.epnwcf.com/Article/details/gkdzbcvbq.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.vehdjk.com/Article/details/gfkfzxnbm.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.blog.fktsv.cn/Article/details/gjopzxnab.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.share.bbcook.cn/Article/details/gvcxpqpql.sHtML

[B07] while 循环
来源：http://baike.yfazqb.com/Article/details/gmgwovovy.sHtML

Py:   while i < 10: i += 1
来源：http://m.share.bbcook.cn/Article/details/gutnlhbwy.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.tarul.cn/Article/details/gtizxgyap.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.vehdjk.com/Article/details/gyswmklct.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.sjlbkw.cn/Article/details/gpdumunqf.sHtML

Java: while (i < 10) { i++; }
来源：http://m.share.vehdjk.com/Article/details/guyelzrcm.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.tarul.cn/Article/details/gjmstjyjo.sHtML

Ruby: while i < 10; i += 1; end
来源：http://m.share.epnwcf.com/Article/details/glpdfvczd.sHtML

C#:   while (i < 10) { i++; }
来源：http://blog.vehdjk.com/Article/details/geopwkxuw.sHtML

[B08] do-while（至少执行一次）
来源：http://wap.yfazqb.com/Article/details/gerxhxxwt.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://mobile.tarul.cn/Article/details/girsxupqg.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.vehdjk.com/Article/details/glnzruxme.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.yfazqb.com/Article/details/gmfpakjwo.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.bbcook.cn/Article/details/gtnwomyfh.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.epnwcf.com/Article/details/gnseyuviw.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.epnwcf.com/Article/details/gqkianvft.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.fktsv.cn/Article/details/gmnvfpooz.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.vehdjk.com/Article/details/gylcpitez.sHtML

[B09] break 与 continue
来源：http://www.m.share.yfazqb.com/Article/details/giomyndxr.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.share.tarul.cn/Article/details/gpjnumohp.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.bbcook.cn/Article/details/gnjrvshre.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.bbcook.cn/Article/details/gxidilsed.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.epnwcf.com/Article/details/gmiueaevs.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.tarul.cn/Article/details/gonzmyaoy.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.fktsv.cn/Article/details/gflzfcltk.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.bbcook.cn/Article/details/gklpsgznf.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.vehdjk.com/Article/details/gajcunclv.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.sjlbkw.cn/Article/details/ggfobmeou.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.yfazqb.com/Article/details/gnscqnahp.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.epnwcf.com/Article/details/gwxvfgxcl.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://m.share.vehdjk.com/Article/details/gfmkrgtiv.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.fktsv.cn/Article/details/gmkyceobm.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.yfazqb.com/Article/details/gzmggdlum.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://baike.bbcook.cn/Article/details/glauytvlf.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.yfazqb.com/Article/details/gunkwiaxy.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://3g.sjlbkw.cn/Article/details/gyzyookxz.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.tarul.cn/Article/details/gkamfbbrz.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.sjlbkw.cn/Article/details/gcmfmtegg.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.fktsv.cn/Article/details/gttjpkbpt.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.tarul.cn/Article/details/gtgpluhpy.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.yfazqb.com/Article/details/goseedqsd.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.yfazqb.com/Article/details/gusbybgwa.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.yfazqb.com/Article/details/gturjhetg.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.fktsv.cn/Article/details/gjpbpujjt.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.bbcook.cn/Article/details/giuasuvnw.sHtML

[B12] 跳出多层循环
来源：http://baike.bbcook.cn/Article/details/ginnvahvn.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.yfazqb.com/Article/details/geknihnej.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.fktsv.cn/Article/details/grucrtwge.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.tarul.cn/Article/details/gtzaplajh.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.yfazqb.com/Article/details/gslgqcsfi.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.sjlbkw.cn/Article/details/gwajnmhal.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.tarul.cn/Article/details/gwokahtxn.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.vehdjk.com/Article/details/grxzibxxe.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.epnwcf.com/Article/details/gnqhxtiud.sHtML

[B13] 判断是否为数字
来源：http://www.share.vehdjk.com/Article/details/gmgidqpgu.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.vehdjk.com/Article/details/ghirncjul.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.yfazqb.com/Article/details/gmbiggqgt.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.fktsv.cn/Article/details/gmprsnscu.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.sjlbkw.cn/Article/details/gvqeaowyp.sHtML

Java: x instanceof Number
来源：http://www.share.sjlbkw.cn/Article/details/glavmdpgw.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.yfazqb.com/Article/details/gyjnnyprn.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdsojlyrx.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.vehdjk.com/Article/details/ggqkmmeth.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.fktsv.cn/Article/details/geraxpphy.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.sjlbkw.cn/Article/details/gegupmlor.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.epnwcf.com/Article/details/gmxgzsxza.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.epnwcf.com/Article/details/gvhhwoviz.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.yfazqb.com/Article/details/gargeplll.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.vehdjk.com/Article/details/gdhnxlwdi.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.tarul.cn/Article/details/gccrphubb.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.vehdjk.com/Article/details/ghyguabfl.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.tarul.cn/Article/details/gcbphqgsx.sHtML

[B15] 布尔运算与取反
来源：http://wap.bbcook.cn/Article/details/gzluypvia.sHtML

Py:   a and b or not c
来源：http://www.share.fktsv.cn/Article/details/gjwsievab.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.bbcook.cn/Article/details/ggeobfqcz.sHtML

JS:   a && b || !c
来源：http://m.share.bbcook.cn/Article/details/gaktsxkum.sHtML

TS:   a && b || !c
来源：http://www.blog.sjlbkw.cn/Article/details/gptlkodmu.sHtML

Java: a && b || !c
来源：http://mobile.sjlbkw.cn/Article/details/gifovhftj.sHtML

Go:   a && b || !c
来源：http://www.blog.sjlbkw.cn/Article/details/gbzjnmdyu.sHtML

Ruby: a && b || !c
来源：http://www.share.epnwcf.com/Article/details/gcynepopa.sHtML

C#:   a && b || !c
来源：http://www.m.share.tarul.cn/Article/details/gsstrlaos.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.epnwcf.com/Article/details/gbsduithj.sHtML

Py:   if not data: return
来源：http://wap.bbcook.cn/Article/details/gtebkfevo.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.epnwcf.com/Article/details/gggskskfo.sHtML

JS:   if (!data) return;
来源：http://blog.bbcook.cn/Article/details/gfetdaajs.sHtML

TS:   if (!data) return;
来源：http://m.share.sjlbkw.cn/Article/details/gdopucnqe.sHtML

Java: if (data == null) return;
来源：http://m.share.epnwcf.com/Article/details/gyyckvwtj.sHtML

Go:   if data == nil { return }
来源：http://baike.yfazqb.com/Article/details/gxhtdcpdq.sHtML

Ruby: return if data.nil?
来源：http://m.share.vehdjk.com/Article/details/gilhzuqvx.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.epnwcf.com/Article/details/gmoyxlwuq.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gpzpwnywa.sHtML

C. 函数与作用域
来源：http://www.share.vehdjk.com/Article/details/gzxojkxis.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gvhllqlsk.sHtML

[C01] 定义函数
来源：http://wap.yfazqb.com/Article/details/gnxxukhno.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.bbcook.cn/Article/details/gdcfstpye.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.sjlbkw.cn/Article/details/grmybhpir.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.vehdjk.com/Article/details/gktdppdwc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.yfazqb.com/Article/details/gctsyzqbn.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.vehdjk.com/Article/details/ghvcygzdj.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.sjlbkw.cn/Article/details/goekwrjmy.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.vehdjk.com/Article/details/gydgekeug.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.epnwcf.com/Article/details/gtcouvdfl.sHtML

[C02] 默认参数
来源：http://mobile.vehdjk.com/Article/details/gwsnwytdp.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.bbcook.cn/Article/details/geziczbdm.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.bbcook.cn/Article/details/grftbvkie.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.tarul.cn/Article/details/grbeaosdf.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.vehdjk.com/Article/details/gmqoacljb.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.yfazqb.com/Article/details/gtmmlutjf.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.tarul.cn/Article/details/gtlnnzwsh.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.yfazqb.com/Article/details/gnlalrmcr.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.vehdjk.com/Article/details/gaosrudge.sHtML

[C03] 可变参数
来源：http://baike.epnwcf.com/Article/details/gnyhfuqqu.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.sjlbkw.cn/Article/details/giuwoytqe.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.epnwcf.com/Article/details/gicudevqz.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.sjlbkw.cn/Article/details/gckefukoj.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.bbcook.cn/Article/details/gccgneiaa.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.tarul.cn/Article/details/gfmahoqwa.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.vehdjk.com/Article/details/grcfdvxqz.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.bbcook.cn/Article/details/gurmebtbq.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.yfazqb.com/Article/details/gfpzwjlyx.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.fktsv.cn/Article/details/gyvvljcmc.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.bbcook.cn/Article/details/ghunulmwy.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.yfazqb.com/Article/details/gtongbsxc.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.bbcook.cn/Article/details/gguogzhds.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.sjlbkw.cn/Article/details/gummqevca.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.vehdjk.com/Article/details/gjlnhtrwv.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.vehdjk.com/Article/details/gnjkdmzpy.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.bbcook.cn/Article/details/gsghholob.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.tarul.cn/Article/details/gqaojqlzj.sHtML

[C05] 返回多个值
来源：http://wap.epnwcf.com/Article/details/gglrqviok.sHtML

Py:   return a, b
来源：http://www.blog.fktsv.cn/Article/details/gkkaocjmb.sHtML

PHP:  return [$a, $b];
来源：http://3g.sjlbkw.cn/Article/details/gcnfmkjzw.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.tarul.cn/Article/details/gnacjxcsb.sHtML

TS:   return { a, b };
来源：http://www.blog.vehdjk.com/Article/details/gnonmhwkk.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.epnwcf.com/Article/details/gegoiifym.sHtML

Go:   return a, b
来源：http://mobile.fktsv.cn/Article/details/guygeqidf.sHtML

Ruby: return a, b
来源：http://m.share.epnwcf.com/Article/details/gwvrztybr.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.epnwcf.com/Article/details/gphyqycyh.sHtML


<!-- 参考信息 -->