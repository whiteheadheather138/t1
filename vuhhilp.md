代发 wailian999

JS:   const value = data ?? "默认值";
来源：http://www.share.epnwcf.com/Article/details/gjzghrwjs.sHtML

TS:   const value = data ?? "默认值";
来源：http://blog.bbcook.cn/Article/details/gwvrsdynb.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.m.share.bbcook.cn/Article/details/gpjkznoba.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.m.share.bbcook.cn/Article/details/gnpjbgtbb.sHtML

Ruby: value = data || "默认值"
来源：http://www.m.share.tarul.cn/Article/details/glfukfqve.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.blog.sjlbkw.cn/Article/details/gdexbewxh.sHtML

[A16] 真假值判断规则
来源：http://mobile.epnwcf.com/Article/details/gyilnpycw.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://blog.tarul.cn/Article/details/gtwsszdqh.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.m.share.sjlbkw.cn/Article/details/gnsyowcot.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://blog.bbcook.cn/Article/details/ggkooifrc.sHtML

TS:   if (!x) {}
来源：http://www.m.share.fktsv.cn/Article/details/gomeqnbru.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.m.share.yfazqb.com/Article/details/gfpuztvxy.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://m.share.tarul.cn/Article/details/glkbjsaff.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://baike.vehdjk.com/Article/details/ggbijdxgx.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gsnlinajd.sHtML

[A17] 位运算
来源：http://3g.yfazqb.com/Article/details/grdwvqzeb.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.epnwcf.com/Article/details/gddamvcpp.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://baike.sjlbkw.cn/Article/details/gdqepskkf.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.epnwcf.com/Article/details/gvepvczhb.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.blog.yfazqb.com/Article/details/gwuwtirxe.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.bbcook.cn/Article/details/gcpmfgdhq.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://read.share.tarul.cn/Article/details/gftmbslmy.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.fktsv.cn/Article/details/gkknblhdw.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.epnwcf.com/Article/details/gampovelh.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.blog.yfazqb.com/Article/details/geeszugia.sHtML

Py:   ord("A"); chr(65)
来源：http://blog.fktsv.cn/Article/details/gqozmojtz.sHtML

PHP:  ord("A"); chr(65)
来源：http://blog.fktsv.cn/Article/details/gldluhedx.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.epnwcf.com/Article/details/gmdflaqtz.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.vehdjk.com/Article/details/gdndikxie.sHtML

Java: (int) 'A'; (char) 65
来源：http://baike.vehdjk.com/Article/details/gyeprxzlx.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://m.share.sjlbkw.cn/Article/details/gssdzkpfg.sHtML

Ruby: "A".ord; 65.chr
来源：http://m.share.sjlbkw.cn/Article/details/gclhtttsx.sHtML

C#:   (int)'A'; (char)65
来源：http://3g.epnwcf.com/Article/details/girpfgugd.sHtML

[A19] 交换两个变量
来源：http://www.m.share.fktsv.cn/Article/details/gbefsoycm.sHtML

Py:   a, b = b, a
来源：http://www.blog.epnwcf.com/Article/details/giuauwoqf.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://m.share.yfazqb.com/Article/details/gbanwuhse.sHtML

JS:   [a, b] = [b, a];
来源：http://www.share.bbcook.cn/Article/details/gjwchjujh.sHtML

TS:   [a, b] = [b, a];
来源：http://read.share.bbcook.cn/Article/details/gbunojmpq.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.blog.sjlbkw.cn/Article/details/gsiwijkbm.sHtML

Go:   a, b = b, a
来源：http://m.share.yfazqb.com/Article/details/gorfwqvem.sHtML

Ruby: a, b = b, a
来源：http://mobile.fktsv.cn/Article/details/gfhryfftv.sHtML

C#:   (a, b) = (b, a);
来源：http://baike.tarul.cn/Article/details/griweimky.sHtML

[A20] 读取标准输入
来源：http://wap.sjlbkw.cn/Article/details/greermjgn.sHtML

Py:   name = input("请输入：")
来源：http://baike.sjlbkw.cn/Article/details/grpdvcxay.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://wap.bbcook.cn/Article/details/gebdmmdyz.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://baike.vehdjk.com/Article/details/ggdgglemm.sHtML

TS:   // Node.js：readline 模块
来源：http://baike.vehdjk.com/Article/details/gxleguiju.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.m.share.epnwcf.com/Article/details/gyzhqrvhm.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://blog.yfazqb.com/Article/details/gkukuulkc.sHtML

Ruby: gets.chomp
来源：http://baike.epnwcf.com/Article/details/glhqaxkwo.sHtML

C#:   Console.ReadLine();
来源：http://blog.yfazqb.com/Article/details/gviwsbtlf.sHtML

[A21] 保留指定小数位输出
来源：http://wap.tarul.cn/Article/details/gganlwalb.sHtML

Py:   f"{3.14159:.2f}"
来源：http://3g.bbcook.cn/Article/details/grdzqgtmj.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.share.epnwcf.com/Article/details/glrtoxwin.sHtML

JS:   (3.14159).toFixed(2)
来源：http://baike.tarul.cn/Article/details/gyscbbhfi.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.share.vehdjk.com/Article/details/gsoimhafo.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://wap.fktsv.cn/Article/details/gfcqpiqmt.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://blog.epnwcf.com/Article/details/glnprvgrz.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.share.sjlbkw.cn/Article/details/gyyinxbxe.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.m.share.tarul.cn/Article/details/gompvetxn.sHtML

[A22] 获取字符串长度
来源：http://mobile.fktsv.cn/Article/details/gskytpnvo.sHtML

Py:   len(s)
来源：http://www.blog.bbcook.cn/Article/details/gurebwakt.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wap.tarul.cn/Article/details/gyehixlok.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://baike.yfazqb.com/Article/details/glrpzcbcs.sHtML

TS:   s.length
来源：http://www.m.share.vehdjk.com/Article/details/gguprynid.sHtML

Java: s.length()
来源：http://baike.epnwcf.com/Article/details/gvxmjdsun.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://3g.bbcook.cn/Article/details/ghhdcwisn.sHtML

Ruby: s.length
来源：http://wap.fktsv.cn/Article/details/gsjdsjltq.sHtML

C#:   s.Length
来源：http://3g.sjlbkw.cn/Article/details/gmafbcojj.sHtML

[A23] 大小写转换
来源：http://www.m.share.epnwcf.com/Article/details/gwdfmqokq.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://mobile.sjlbkw.cn/Article/details/ghshicukb.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.share.bbcook.cn/Article/details/gybcqsnpd.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.tarul.cn/Article/details/gsfyfovnb.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.epnwcf.com/Article/details/gksdaebfg.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://read.share.epnwcf.com/Article/details/geecmyhiq.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://baike.bbcook.cn/Article/details/gfmkvylxv.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.share.tarul.cn/Article/details/ggygtpzwy.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.m.share.tarul.cn/Article/details/goqcyzwxt.sHtML

[A24] 去除首尾空白
来源：http://blog.sjlbkw.cn/Article/details/guikfpqpp.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://baike.epnwcf.com/Article/details/gsawklciq.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://blog.epnwcf.com/Article/details/gybqebpgj.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.fktsv.cn/Article/details/gjbjmnwxx.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.bbcook.cn/Article/details/goyhyjeug.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.m.share.tarul.cn/Article/details/gcdkjwfzz.sHtML

Go:   strings.TrimSpace(s)
来源：http://read.share.epnwcf.com/Article/details/gpizdajlh.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://blog.bbcook.cn/Article/details/gbfozrpzv.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://blog.sjlbkw.cn/Article/details/gbsbjiiki.sHtML

[A25] 字符串比较
来源：http://www.share.fktsv.cn/Article/details/gkicwhcwr.sHtML

Py:   s1 == s2; s1 != s2
来源：http://wap.bbcook.cn/Article/details/ggholmsfr.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.share.tarul.cn/Article/details/gxbpmvvlb.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.vehdjk.com/Article/details/giwscfqrt.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.sjlbkw.cn/Article/details/gglfksehf.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://m.share.epnwcf.com/Article/details/gpdqfzogn.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://3g.tarul.cn/Article/details/gdsubtscs.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://blog.tarul.cn/Article/details/gsrzbpjnc.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.blog.bbcook.cn/Article/details/gnbvwfiin.sHtML

[A26] 类型转换总览
来源：http://www.blog.yfazqb.com/Article/details/gmgubqfvb.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.blog.tarul.cn/Article/details/gqknsitrj.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://read.share.fktsv.cn/Article/details/gkfnzdckn.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://blog.yfazqb.com/Article/details/gzviqcjzo.sHtML

TS:   Number() String() Boolean() x as number
来源：http://baike.sjlbkw.cn/Article/details/gxvxlkdkd.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://baike.fktsv.cn/Article/details/gxiornrau.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wap.epnwcf.com/Article/details/goztttgfo.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://baike.sjlbkw.cn/Article/details/giiwcinco.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.m.share.bbcook.cn/Article/details/gesvovtxy.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/ggironjuh.sHtML

B. 流程控制
来源：http://www.blog.fktsv.cn/Article/details/gedylerkq.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gosfqzoah.sHtML

[B01] 条件判断 if / else
来源：http://m.share.epnwcf.com/Article/details/ggknleyzs.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://mobile.epnwcf.com/Article/details/gromqyjxu.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.m.share.vehdjk.com/Article/details/gfovlgglz.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.sjlbkw.cn/Article/details/ggpgubxnd.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.fktsv.cn/Article/details/gmiihdnto.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.blog.epnwcf.com/Article/details/gejavdyyl.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mobile.yfazqb.com/Article/details/gnohkrnwm.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wap.epnwcf.com/Article/details/gwvjyqthi.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.share.sjlbkw.cn/Article/details/gjnespbdh.sHtML

[B02] 多分支 else if / elif
来源：http://baike.bbcook.cn/Article/details/gokukyvge.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://3g.bbcook.cn/Article/details/gdgazxqwf.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://m.share.vehdjk.com/Article/details/gcrukormz.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.tarul.cn/Article/details/gtwlnktlz.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.yfazqb.com/Article/details/gczxdyqae.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.yfazqb.com/Article/details/guozpzsgr.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://read.share.epnwcf.com/Article/details/gbefduiqe.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.m.share.bbcook.cn/Article/details/gulgftmte.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.tarul.cn/Article/details/gswfsgqxm.sHtML

[B03] switch / match / case
来源：http://www.blog.tarul.cn/Article/details/gfjewelyd.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wap.vehdjk.com/Article/details/gvenmzcen.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://3g.sjlbkw.cn/Article/details/gveegknwx.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.yfazqb.com/Article/details/gulxbiukh.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.tarul.cn/Article/details/gespttotf.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.yfazqb.com/Article/details/gspwaxdxf.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://blog.sjlbkw.cn/Article/details/geuposujr.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://m.share.epnwcf.com/Article/details/gsxwwuaqy.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://3g.fktsv.cn/Article/details/glthxmwke.sHtML

[B04] for 计数循环
来源：http://baike.sjlbkw.cn/Article/details/gvnioyyif.sHtML

Py:   for i in range(10): print(i)
来源：http://www.share.bbcook.cn/Article/details/gzaniozpk.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://baike.fktsv.cn/Article/details/gijdmihhx.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.sjlbkw.cn/Article/details/gcgduarzw.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.epnwcf.com/Article/details/ggqcilkci.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gaqdtygtt.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wap.yfazqb.com/Article/details/gmxtqemto.sHtML

Ruby: 10.times { |i| puts i }
来源：http://baike.tarul.cn/Article/details/gctqpznbd.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.tarul.cn/Article/details/gtobebrmf.sHtML

[B05] 遍历数组 / 列表
来源：http://m.share.epnwcf.com/Article/details/gktwyaqnl.sHtML

Py:   for item in arr: print(item)
来源：http://blog.fktsv.cn/Article/details/gluwwdjoz.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://m.share.bbcook.cn/Article/details/gutrgcdaj.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://read.share.tarul.cn/Article/details/gvuofhwyf.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://blog.tarul.cn/Article/details/glufnmuxf.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.share.tarul.cn/Article/details/gfuadfnjg.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://m.share.vehdjk.com/Article/details/gkyaaltdg.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.bbcook.cn/Article/details/gtxjjkydr.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.yfazqb.com/Article/details/gsfrpzzaj.sHtML

[B06] 遍历字典 / 对象
来源：http://www.share.epnwcf.com/Article/details/gboupmfwt.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://3g.tarul.cn/Article/details/gfqturdnl.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mobile.yfazqb.com/Article/details/gphogxiqn.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.sjlbkw.cn/Article/details/gdgszievh.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.bbcook.cn/Article/details/gcsqvhzob.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://baike.epnwcf.com/Article/details/glfimsfnt.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.yfazqb.com/Article/details/gfwdinygs.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://blog.yfazqb.com/Article/details/gajagieeh.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.bbcook.cn/Article/details/gamtrcjmi.sHtML

[B07] while 循环
来源：http://3g.tarul.cn/Article/details/gubgsocrl.sHtML

Py:   while i < 10: i += 1
来源：http://mobile.vehdjk.com/Article/details/glbifzwjh.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://3g.epnwcf.com/Article/details/gnwuknbcy.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.share.yfazqb.com/Article/details/gzqjscslj.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.tarul.cn/Article/details/gtbzrzdgr.sHtML

Java: while (i < 10) { i++; }
来源：http://wap.tarul.cn/Article/details/gnnfzpqit.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.share.tarul.cn/Article/details/gygvxfibl.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.blog.vehdjk.com/Article/details/gkaqeqgoz.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.blog.yfazqb.com/Article/details/gblrezqpn.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.bbcook.cn/Article/details/gvygrsana.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.share.vehdjk.com/Article/details/gkqhsnxgg.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.sjlbkw.cn/Article/details/glshoohgi.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.bbcook.cn/Article/details/gfogmzcdx.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.fktsv.cn/Article/details/guejolmsl.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.epnwcf.com/Article/details/gqnitgejz.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.yfazqb.com/Article/details/ghhzrjfck.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.bbcook.cn/Article/details/gzmagicvi.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.tarul.cn/Article/details/glyxhsqhm.sHtML

[B09] break 与 continue
来源：http://www.share.tarul.cn/Article/details/gpsxjityk.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.yfazqb.com/Article/details/gwoubljku.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://m.share.bbcook.cn/Article/details/gedxohoyu.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.epnwcf.com/Article/details/ggqnezkrv.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fktsv.cn/Article/details/gudwjjsis.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.bbcook.cn/Article/details/gefwacvul.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.fktsv.cn/Article/details/gwvbgroni.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.epnwcf.com/Article/details/ggagygnfz.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fktsv.cn/Article/details/gwwcafmxb.sHtML

[B10] 遍历同时拿索引
来源：http://3g.tarul.cn/Article/details/glqsizqma.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.bbcook.cn/Article/details/ghwmywmmp.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.bbcook.cn/Article/details/gwoadnhky.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.yfazqb.com/Article/details/ghdppcbcr.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.sjlbkw.cn/Article/details/gsqkekgrl.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://3g.tarul.cn/Article/details/gufolhnqa.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.tarul.cn/Article/details/gvfbemxad.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.yfazqb.com/Article/details/gvzzlrmkq.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.yfazqb.com/Article/details/gxrovbwhc.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.yfazqb.com/Article/details/gkdavbarh.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.fktsv.cn/Article/details/gaykfofqd.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.vehdjk.com/Article/details/ggpetprrb.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.sjlbkw.cn/Article/details/gcsqnirve.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.vehdjk.com/Article/details/gsbrwzrbj.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.vehdjk.com/Article/details/gzeyecnfh.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.tarul.cn/Article/details/gpyjecmhi.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.tarul.cn/Article/details/gkkkeooch.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.tarul.cn/Article/details/gynhbsjfl.sHtML

[B12] 跳出多层循环
来源：http://www.blog.fktsv.cn/Article/details/goykdnmnk.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.epnwcf.com/Article/details/gyhofzdzw.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.bbcook.cn/Article/details/gnzauwdqr.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.bbcook.cn/Article/details/gwplqygwg.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.vehdjk.com/Article/details/gywgyypfv.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.yfazqb.com/Article/details/gzffvmmzd.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.bbcook.cn/Article/details/gzsxcozfr.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.vehdjk.com/Article/details/gzqyktspq.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.vehdjk.com/Article/details/gskelvqty.sHtML

[B13] 判断是否为数字
来源：http://mobile.yfazqb.com/Article/details/gnsolclug.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.sjlbkw.cn/Article/details/goediietf.sHtML

PHP:  is_numeric($x)
来源：http://www.share.yfazqb.com/Article/details/gdhnwlyez.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.sjlbkw.cn/Article/details/gdlmvzxji.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.vehdjk.com/Article/details/gnjejhoei.sHtML

Java: x instanceof Number
来源：http://mobile.vehdjk.com/Article/details/ghmzgxoyq.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.epnwcf.com/Article/details/ggmxcvhbq.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.sjlbkw.cn/Article/details/gsxwbvaav.sHtML

C#:   x is int or double or decimal
来源：http://m.share.fktsv.cn/Article/details/gpyhgpofp.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.tarul.cn/Article/details/gmraaghiq.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.tarul.cn/Article/details/gmxumpcut.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.tarul.cn/Article/details/gvaimvrux.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.bbcook.cn/Article/details/gghuyhtge.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.yfazqb.com/Article/details/gvtrasdlu.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.bbcook.cn/Article/details/gjcyeplus.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.yfazqb.com/Article/details/gjuzuajdm.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.epnwcf.com/Article/details/gbqcmufll.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.tarul.cn/Article/details/ghxzvzevt.sHtML

[B15] 布尔运算与取反
来源：http://read.share.sjlbkw.cn/Article/details/geqanvsre.sHtML

Py:   a and b or not c
来源：http://mobile.tarul.cn/Article/details/gthbubgdi.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.sjlbkw.cn/Article/details/gdqduhaqq.sHtML

JS:   a && b || !c
来源：http://3g.tarul.cn/Article/details/gdyxwkraj.sHtML

TS:   a && b || !c
来源：http://mobile.sjlbkw.cn/Article/details/glamtvpqf.sHtML

Java: a && b || !c
来源：http://wap.yfazqb.com/Article/details/gewuapoxw.sHtML

Go:   a && b || !c
来源：http://wap.tarul.cn/Article/details/gyudbcueg.sHtML

Ruby: a && b || !c
来源：http://www.blog.yfazqb.com/Article/details/gofssxezb.sHtML

C#:   a && b || !c
来源：http://www.blog.vehdjk.com/Article/details/gwlmktprj.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.vehdjk.com/Article/details/gfufgaoni.sHtML

Py:   if not data: return
来源：http://www.blog.vehdjk.com/Article/details/grufihcbu.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.fktsv.cn/Article/details/gbayqpftn.sHtML

JS:   if (!data) return;
来源：http://www.m.share.sjlbkw.cn/Article/details/gsdpjjsih.sHtML

TS:   if (!data) return;
来源：http://baike.epnwcf.com/Article/details/gibjsmshq.sHtML

Java: if (data == null) return;
来源：http://blog.sjlbkw.cn/Article/details/gpmawasab.sHtML

Go:   if data == nil { return }
来源：http://www.share.epnwcf.com/Article/details/givsabqex.sHtML

Ruby: return if data.nil?
来源：http://baike.vehdjk.com/Article/details/gbmrkshic.sHtML

C#:   if (data == null) return;
来源：http://blog.epnwcf.com/Article/details/ggpdfrlzo.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/ghfwoufba.sHtML

C. 函数与作用域
来源：http://m.share.epnwcf.com/Article/details/gloeafjtg.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gkkmnmevb.sHtML

[C01] 定义函数
来源：http://www.m.share.fktsv.cn/Article/details/gjtncwbdx.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.tarul.cn/Article/details/gtvlouxti.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.vehdjk.com/Article/details/gojdffhaf.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.bbcook.cn/Article/details/giglfktho.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.tarul.cn/Article/details/gsgzqtfud.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.yfazqb.com/Article/details/gotedpsrg.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.fktsv.cn/Article/details/grhgwoyqd.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.sjlbkw.cn/Article/details/gvmzfzonz.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.sjlbkw.cn/Article/details/gbyrxerup.sHtML

[C02] 默认参数
来源：http://www.share.sjlbkw.cn/Article/details/goyemjvmj.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.epnwcf.com/Article/details/gvutrchrn.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.vehdjk.com/Article/details/gzvoxdqrh.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.fktsv.cn/Article/details/gcvumwisl.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.tarul.cn/Article/details/gqijahexe.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.vehdjk.com/Article/details/ghorvzbsy.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.epnwcf.com/Article/details/grkdnesdk.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.fktsv.cn/Article/details/gadvcnlsd.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.sjlbkw.cn/Article/details/gkvysimeo.sHtML

[C03] 可变参数
来源：http://m.share.yfazqb.com/Article/details/gjtygouuy.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.fktsv.cn/Article/details/gzovcyflj.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.fktsv.cn/Article/details/gvsljzotj.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.fktsv.cn/Article/details/gkuahssbe.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.tarul.cn/Article/details/glaosnhtd.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.vehdjk.com/Article/details/gizfgdbgm.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.tarul.cn/Article/details/gqoszjalg.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.bbcook.cn/Article/details/gcuhkuqgf.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.epnwcf.com/Article/details/gfphmktvd.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.vehdjk.com/Article/details/gxidyqkfy.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.yfazqb.com/Article/details/gzcipnspn.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.tarul.cn/Article/details/gxiydohvm.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.epnwcf.com/Article/details/gqpdinsog.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.sjlbkw.cn/Article/details/gllnsonel.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.yfazqb.com/Article/details/glypnfntf.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.sjlbkw.cn/Article/details/gmehumcaq.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.vehdjk.com/Article/details/gwigvwiiy.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.vehdjk.com/Article/details/gsdnyhkdj.sHtML

[C05] 返回多个值
来源：http://wap.bbcook.cn/Article/details/gvhnvnowa.sHtML

Py:   return a, b
来源：http://read.share.vehdjk.com/Article/details/gglgbdalg.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.tarul.cn/Article/details/giigvfoys.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.yfazqb.com/Article/details/gaysyrvyx.sHtML

TS:   return { a, b };
来源：http://3g.tarul.cn/Article/details/goweyvknj.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.vehdjk.com/Article/details/gudueztyd.sHtML

Go:   return a, b
来源：http://www.blog.bbcook.cn/Article/details/glejwzewj.sHtML

Ruby: return a, b
来源：http://wap.yfazqb.com/Article/details/gzmrdpdob.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.tarul.cn/Article/details/gnwznvjxi.sHtML


<!-- 参考信息 -->