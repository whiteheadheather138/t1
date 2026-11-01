代发 wailian999

C#:   // 单行；/* 多行 */
来源：http://baike.vehdjk.com/Article/details/gmaqpbefs.sHtML

[A15] 空值判断与默认值
来源：http://m.share.sjlbkw.cn/Article/details/gtutlypkq.sHtML

Py:   value = data or "默认值"
来源：http://3g.epnwcf.com/Article/details/gyaqcudhj.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://blog.sjlbkw.cn/Article/details/gmbdwxxvz.sHtML

JS:   const value = data ?? "默认值";
来源：http://mobile.epnwcf.com/Article/details/gdhjuzcpc.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.share.bbcook.cn/Article/details/gxgojxiwr.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://3g.bbcook.cn/Article/details/glypjnvjh.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.share.bbcook.cn/Article/details/gmobrvqqu.sHtML

Ruby: value = data || "默认值"
来源：http://m.share.tarul.cn/Article/details/gakjukfle.sHtML

C#:   var value = data ?? "默认值";
来源：http://read.share.epnwcf.com/Article/details/gsedktwiv.sHtML

[A16] 真假值判断规则
来源：http://www.share.bbcook.cn/Article/details/getwsiceg.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.blog.epnwcf.com/Article/details/gjlcjluol.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://blog.vehdjk.com/Article/details/gpbhwmpsk.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://blog.bbcook.cn/Article/details/gupmfkkuu.sHtML

TS:   if (!x) {}
来源：http://www.blog.tarul.cn/Article/details/gzyqsecjk.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.share.vehdjk.com/Article/details/gediefdpa.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://read.share.vehdjk.com/Article/details/gecfqoukj.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://3g.yfazqb.com/Article/details/grwmhvozh.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://3g.fktsv.cn/Article/details/gwcxomhnk.sHtML

[A17] 位运算
来源：http://blog.fktsv.cn/Article/details/gngsynnho.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.epnwcf.com/Article/details/ggjscvqxz.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wap.bbcook.cn/Article/details/ghmhgnneg.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.epnwcf.com/Article/details/gjtkmubef.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wap.bbcook.cn/Article/details/gfalwtsyd.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.bbcook.cn/Article/details/gkmiifuge.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://3g.bbcook.cn/Article/details/gefzydssl.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.vehdjk.com/Article/details/gilxwpgyq.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.bbcook.cn/Article/details/gkzxdndxm.sHtML

[A18] 字符与 ASCII 码互转
来源：http://3g.fktsv.cn/Article/details/gxnzpvqhq.sHtML

Py:   ord("A"); chr(65)
来源：http://www.share.yfazqb.com/Article/details/gpxheyblj.sHtML

PHP:  ord("A"); chr(65)
来源：http://mobile.tarul.cn/Article/details/gnrqqyqtb.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.yfazqb.com/Article/details/gjvlqvffb.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.tarul.cn/Article/details/gkwtufhxy.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.share.sjlbkw.cn/Article/details/gfcxlupaf.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://3g.vehdjk.com/Article/details/grnsbbbls.sHtML

Ruby: "A".ord; 65.chr
来源：http://wap.yfazqb.com/Article/details/grzjfuuwk.sHtML

C#:   (int)'A'; (char)65
来源：http://mobile.yfazqb.com/Article/details/grfueypag.sHtML

[A19] 交换两个变量
来源：http://blog.vehdjk.com/Article/details/gldfccndo.sHtML

Py:   a, b = b, a
来源：http://www.m.share.fktsv.cn/Article/details/ghtclxyga.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://baike.fktsv.cn/Article/details/gfzcrwecp.sHtML

JS:   [a, b] = [b, a];
来源：http://3g.vehdjk.com/Article/details/gevuyujdo.sHtML

TS:   [a, b] = [b, a];
来源：http://www.blog.yfazqb.com/Article/details/grvipybtn.sHtML

Java: int t = a; a = b; b = t;
来源：http://mobile.vehdjk.com/Article/details/gcqnrxmin.sHtML

Go:   a, b = b, a
来源：http://wap.yfazqb.com/Article/details/gjjbcceyw.sHtML

Ruby: a, b = b, a
来源：http://blog.bbcook.cn/Article/details/ghftrjhdu.sHtML

C#:   (a, b) = (b, a);
来源：http://blog.vehdjk.com/Article/details/ggpqswxwv.sHtML

[A20] 读取标准输入
来源：http://blog.yfazqb.com/Article/details/gwejilfsd.sHtML

Py:   name = input("请输入：")
来源：http://mobile.bbcook.cn/Article/details/goarprpwy.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.m.share.bbcook.cn/Article/details/gmnqpbaty.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://baike.tarul.cn/Article/details/geyuzrpor.sHtML

TS:   // Node.js：readline 模块
来源：http://wap.epnwcf.com/Article/details/gsoyilbrw.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.share.epnwcf.com/Article/details/ghecfkvat.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.blog.epnwcf.com/Article/details/gjcfzyasa.sHtML

Ruby: gets.chomp
来源：http://read.share.bbcook.cn/Article/details/gucylptlb.sHtML

C#:   Console.ReadLine();
来源：http://wap.yfazqb.com/Article/details/grqdjkpdf.sHtML

[A21] 保留指定小数位输出
来源：http://wap.fktsv.cn/Article/details/gtjwxzxbu.sHtML

Py:   f"{3.14159:.2f}"
来源：http://mobile.fktsv.cn/Article/details/goylckwgy.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://blog.vehdjk.com/Article/details/gfujxozgr.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.m.share.vehdjk.com/Article/details/geeykncxw.sHtML

TS:   (3.14159).toFixed(2)
来源：http://m.share.sjlbkw.cn/Article/details/gbhesuqwu.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://wap.bbcook.cn/Article/details/gavqinypg.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.blog.fktsv.cn/Article/details/gabizzygt.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://blog.epnwcf.com/Article/details/gvgrncnpc.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.share.fktsv.cn/Article/details/ghxttnzaz.sHtML

[A22] 获取字符串长度
来源：http://wap.epnwcf.com/Article/details/guauvznza.sHtML

Py:   len(s)
来源：http://www.share.fktsv.cn/Article/details/ggbktybsd.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://baike.yfazqb.com/Article/details/guxyhxcqq.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://baike.sjlbkw.cn/Article/details/gdqpkylle.sHtML

TS:   s.length
来源：http://www.share.fktsv.cn/Article/details/gtoymvzaf.sHtML

Java: s.length()
来源：http://wap.tarul.cn/Article/details/gxegbvwbh.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://m.share.bbcook.cn/Article/details/getuueqqs.sHtML

Ruby: s.length
来源：http://read.share.bbcook.cn/Article/details/ggjdhpaat.sHtML

C#:   s.Length
来源：http://mobile.tarul.cn/Article/details/ghzdzgxej.sHtML

[A23] 大小写转换
来源：http://blog.fktsv.cn/Article/details/gphdaizus.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.blog.fktsv.cn/Article/details/gnhtlrctk.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.m.share.fktsv.cn/Article/details/gloqcpzhy.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.epnwcf.com/Article/details/gtyhcunpk.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.sjlbkw.cn/Article/details/grfoysjbt.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wap.yfazqb.com/Article/details/grblnhzwj.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mobile.fktsv.cn/Article/details/guqoqlujo.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://m.share.tarul.cn/Article/details/gadpyqrbw.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.share.bbcook.cn/Article/details/gtzpijnkr.sHtML

[A24] 去除首尾空白
来源：http://3g.bbcook.cn/Article/details/getulrofw.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://3g.epnwcf.com/Article/details/gxbgnlkjk.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://m.share.yfazqb.com/Article/details/gkkbyasrr.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.fktsv.cn/Article/details/gqgngtvet.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.yfazqb.com/Article/details/gpphguigm.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://read.share.epnwcf.com/Article/details/gspjubwjt.sHtML

Go:   strings.TrimSpace(s)
来源：http://read.share.sjlbkw.cn/Article/details/girbgndkq.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.blog.vehdjk.com/Article/details/gmdserjjp.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://3g.yfazqb.com/Article/details/gjmfejadu.sHtML

[A25] 字符串比较
来源：http://3g.epnwcf.com/Article/details/gxhcjodbq.sHtML

Py:   s1 == s2; s1 != s2
来源：http://read.share.tarul.cn/Article/details/gwyxjyfqk.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://baike.epnwcf.com/Article/details/gqzvoxlze.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.bbcook.cn/Article/details/gsopuezsv.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.sjlbkw.cn/Article/details/gbhvqfdak.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://3g.fktsv.cn/Article/details/gquyemlma.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://m.share.tarul.cn/Article/details/gjyvkkpqd.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://read.share.yfazqb.com/Article/details/gvkoqccnv.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.blog.yfazqb.com/Article/details/gsralnqjg.sHtML

[A26] 类型转换总览
来源：http://mobile.fktsv.cn/Article/details/gczqcopfh.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://baike.yfazqb.com/Article/details/gfpbfzdim.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://3g.bbcook.cn/Article/details/gznzbgkvt.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.blog.sjlbkw.cn/Article/details/gekkhjjed.sHtML

TS:   Number() String() Boolean() x as number
来源：http://baike.fktsv.cn/Article/details/gdiiwhesd.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://blog.tarul.cn/Article/details/gdxmtzhoi.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://3g.yfazqb.com/Article/details/ggmwtxfur.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://m.share.tarul.cn/Article/details/gzardmjhu.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://3g.bbcook.cn/Article/details/gqxorbuox.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gyvcjmcqu.sHtML

B. 流程控制
来源：http://baike.yfazqb.com/Article/details/gzbxsbjkd.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gbrsrsaos.sHtML

[B01] 条件判断 if / else
来源：http://www.share.vehdjk.com/Article/details/gytibworo.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://baike.bbcook.cn/Article/details/ghsgedsvk.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.m.share.epnwcf.com/Article/details/gcjovqwvt.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.tarul.cn/Article/details/gnmdsohwf.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.tarul.cn/Article/details/gwichstmw.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://m.share.fktsv.cn/Article/details/gezcifanc.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wap.epnwcf.com/Article/details/ggdludcdc.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wap.bbcook.cn/Article/details/gdrhynerx.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wap.bbcook.cn/Article/details/gmumeihhs.sHtML

[B02] 多分支 else if / elif
来源：http://3g.vehdjk.com/Article/details/gbeqsvypq.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wap.vehdjk.com/Article/details/gciyvfvlg.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.share.tarul.cn/Article/details/grcbisktn.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.epnwcf.com/Article/details/geamtooko.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.yfazqb.com/Article/details/gwfcxyoov.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.tarul.cn/Article/details/ggmcklcey.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mobile.fktsv.cn/Article/details/grnmvxpze.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://m.share.sjlbkw.cn/Article/details/gzwggsuzt.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.sjlbkw.cn/Article/details/gjjgpqrxs.sHtML

[B03] switch / match / case
来源：http://www.share.epnwcf.com/Article/details/ggrqmlywh.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://read.share.yfazqb.com/Article/details/gdsxvcgkj.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wap.epnwcf.com/Article/details/gpxoauije.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.vehdjk.com/Article/details/gaxsovnxo.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.fktsv.cn/Article/details/gnbdsijoq.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.yfazqb.com/Article/details/gnjjufrfg.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mobile.sjlbkw.cn/Article/details/gtxloqxjz.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.yfazqb.com/Article/details/gmywiuqdh.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.share.sjlbkw.cn/Article/details/gnmbulmqx.sHtML

[B04] for 计数循环
来源：http://mobile.yfazqb.com/Article/details/gawhcxwdy.sHtML

Py:   for i in range(10): print(i)
来源：http://baike.bbcook.cn/Article/details/goqqffgxd.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://blog.tarul.cn/Article/details/gdhlywwja.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.epnwcf.com/Article/details/gjijtooir.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.fktsv.cn/Article/details/ggcfvivjr.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.share.sjlbkw.cn/Article/details/gmimtzcli.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.share.epnwcf.com/Article/details/gzgqfyvsh.sHtML

Ruby: 10.times { |i| puts i }
来源：http://read.share.epnwcf.com/Article/details/gaqtnarsw.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.share.yfazqb.com/Article/details/gyxobbehi.sHtML

[B05] 遍历数组 / 列表
来源：http://www.share.yfazqb.com/Article/details/gprktrgpc.sHtML

Py:   for item in arr: print(item)
来源：http://mobile.fktsv.cn/Article/details/gorfqcapd.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.blog.tarul.cn/Article/details/gpumiljnj.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://baike.vehdjk.com/Article/details/gntliboym.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://mobile.yfazqb.com/Article/details/gvhyhjece.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://mobile.sjlbkw.cn/Article/details/gaabtxalz.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.blog.epnwcf.com/Article/details/gqcfhlrqh.sHtML

Ruby: arr.each { |item| puts item }
来源：http://wap.yfazqb.com/Article/details/gmbogjjkx.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.m.share.vehdjk.com/Article/details/gdkectrcs.sHtML

[B06] 遍历字典 / 对象
来源：http://wap.tarul.cn/Article/details/gqblvdhqg.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.sjlbkw.cn/Article/details/gkfjamote.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.m.share.vehdjk.com/Article/details/gclrfxegh.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.vehdjk.com/Article/details/gzlntnbcd.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.bbcook.cn/Article/details/gpeqcvluh.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.tarul.cn/Article/details/gemugzvfa.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.yfazqb.com/Article/details/gqbctfhik.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.fktsv.cn/Article/details/gfkverxvu.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://blog.tarul.cn/Article/details/ghcsteabm.sHtML

[B07] while 循环
来源：http://www.m.share.bbcook.cn/Article/details/ghdrzxkrc.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.epnwcf.com/Article/details/glnxdzplj.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.bbcook.cn/Article/details/gbkjxkgvz.sHtML

JS:   while (i < 10) { i++; }
来源：http://baike.vehdjk.com/Article/details/gupijhohe.sHtML

TS:   while (i < 10) { i++; }
来源：http://read.share.sjlbkw.cn/Article/details/gukwjylpp.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.fktsv.cn/Article/details/gtawhbvwq.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.sjlbkw.cn/Article/details/gijajzeak.sHtML

Ruby: while i < 10; i += 1; end
来源：http://read.share.fktsv.cn/Article/details/gdiotluhs.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.epnwcf.com/Article/details/gxadptbpi.sHtML

[B08] do-while（至少执行一次）
来源：http://wap.epnwcf.com/Article/details/ghbqzekwv.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://blog.bbcook.cn/Article/details/glohvntbe.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.vehdjk.com/Article/details/gbzwzingk.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.m.share.fktsv.cn/Article/details/gjyaraijm.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.bbcook.cn/Article/details/gpxztfpkh.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.share.tarul.cn/Article/details/gpsanvujb.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.epnwcf.com/Article/details/gvaiwqity.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.tarul.cn/Article/details/gpmwgawjt.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.vehdjk.com/Article/details/geaelcaiw.sHtML

[B09] break 与 continue
来源：http://www.share.fktsv.cn/Article/details/gfysudqil.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.share.epnwcf.com/Article/details/gttctmkil.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.sjlbkw.cn/Article/details/gjssvzmvh.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.tarul.cn/Article/details/gtskczkym.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.yfazqb.com/Article/details/gtglefncr.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.vehdjk.com/Article/details/gbnmydrbw.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.epnwcf.com/Article/details/gfolklnfs.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.bbcook.cn/Article/details/geqymmptb.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.sjlbkw.cn/Article/details/gwjwaszlg.sHtML

[B10] 遍历同时拿索引
来源：http://baike.vehdjk.com/Article/details/ghvoxykpj.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.vehdjk.com/Article/details/grfjhtgpl.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.tarul.cn/Article/details/gcumkxscs.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.epnwcf.com/Article/details/gwnkwsbvw.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.fktsv.cn/Article/details/gjnfqkpcp.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.sjlbkw.cn/Article/details/gitcivyby.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.fktsv.cn/Article/details/gyvenozjf.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.vehdjk.com/Article/details/gntssrkgn.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.sjlbkw.cn/Article/details/gyuzifxes.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.fktsv.cn/Article/details/gnvhydayv.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.bbcook.cn/Article/details/gbnnkxoos.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.epnwcf.com/Article/details/guvdllruz.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.sjlbkw.cn/Article/details/gntcsptel.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.tarul.cn/Article/details/gsjwubgvp.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.fktsv.cn/Article/details/gecudlisy.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.vehdjk.com/Article/details/glzeeyqqe.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.vehdjk.com/Article/details/gvmgxyboe.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.sjlbkw.cn/Article/details/gyyeorvqr.sHtML

[B12] 跳出多层循环
来源：http://baike.yfazqb.com/Article/details/gpqtzudzm.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.yfazqb.com/Article/details/gntdentgp.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.yfazqb.com/Article/details/gtkrccgpd.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.bbcook.cn/Article/details/gljmfzlut.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.epnwcf.com/Article/details/gwrxjkvcw.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.epnwcf.com/Article/details/giebbqnbk.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.vehdjk.com/Article/details/gxqtvpumk.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.yfazqb.com/Article/details/gjkhtecrk.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.vehdjk.com/Article/details/gxwpyvssf.sHtML

[B13] 判断是否为数字
来源：http://3g.bbcook.cn/Article/details/gywiyobcu.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.fktsv.cn/Article/details/gktewedut.sHtML

PHP:  is_numeric($x)
来源：http://wap.epnwcf.com/Article/details/grbwzfzvc.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.sjlbkw.cn/Article/details/gztaeoqgk.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.fktsv.cn/Article/details/giewaivtg.sHtML

Java: x instanceof Number
来源：http://www.share.fktsv.cn/Article/details/gcrslozyu.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.yfazqb.com/Article/details/gsmoilbrc.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.fktsv.cn/Article/details/gjyioiqlv.sHtML

C#:   x is int or double or decimal
来源：http://baike.fktsv.cn/Article/details/gxddtkzfa.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.tarul.cn/Article/details/gxamtpata.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.sjlbkw.cn/Article/details/ggmytqjzf.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.sjlbkw.cn/Article/details/gfbftkqfa.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.tarul.cn/Article/details/gozoovbkj.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.sjlbkw.cn/Article/details/gxlqpxsrc.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.bbcook.cn/Article/details/glflfgfpk.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.sjlbkw.cn/Article/details/gnpnlnjwp.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.epnwcf.com/Article/details/gjwbrfpoc.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.bbcook.cn/Article/details/gmtxxjuhd.sHtML

[B15] 布尔运算与取反
来源：http://3g.epnwcf.com/Article/details/ghfcqypkv.sHtML

Py:   a and b or not c
来源：http://read.share.yfazqb.com/Article/details/gpljchwqz.sHtML

PHP:  $a && $b || !$c
来源：http://wap.epnwcf.com/Article/details/gwvpxfkid.sHtML

JS:   a && b || !c
来源：http://www.blog.tarul.cn/Article/details/ginwxfbwj.sHtML

TS:   a && b || !c
来源：http://www.share.fktsv.cn/Article/details/gtrvpnnae.sHtML

Java: a && b || !c
来源：http://www.m.share.vehdjk.com/Article/details/gdvvdaytp.sHtML

Go:   a && b || !c
来源：http://www.blog.sjlbkw.cn/Article/details/gogcvatss.sHtML

Ruby: a && b || !c
来源：http://mobile.sjlbkw.cn/Article/details/gamikjixm.sHtML

C#:   a && b || !c
来源：http://www.blog.fktsv.cn/Article/details/gublxvubd.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.tarul.cn/Article/details/gaqfnfqdn.sHtML

Py:   if not data: return
来源：http://3g.bbcook.cn/Article/details/guffjsazv.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.bbcook.cn/Article/details/gzmdyhkig.sHtML

JS:   if (!data) return;
来源：http://3g.tarul.cn/Article/details/gnkzyiqym.sHtML

TS:   if (!data) return;
来源：http://blog.sjlbkw.cn/Article/details/gxuhlvtvb.sHtML

Java: if (data == null) return;
来源：http://m.share.yfazqb.com/Article/details/gsylyqxxf.sHtML

Go:   if data == nil { return }
来源：http://m.share.vehdjk.com/Article/details/geguzwwon.sHtML

Ruby: return if data.nil?
来源：http://m.share.tarul.cn/Article/details/gipefaegk.sHtML

C#:   if (data == null) return;
来源：http://blog.tarul.cn/Article/details/gomfckcgp.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gibvcxmcf.sHtML

C. 函数与作用域
来源：http://mobile.fktsv.cn/Article/details/ghmtwqmer.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gjdupshmd.sHtML

[C01] 定义函数
来源：http://3g.epnwcf.com/Article/details/giiqhknjq.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.tarul.cn/Article/details/gjgtsvawh.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.epnwcf.com/Article/details/gtbvvhggy.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.tarul.cn/Article/details/gfxxldltl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.yfazqb.com/Article/details/gbymkxces.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.epnwcf.com/Article/details/gxyjuxfxn.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.sjlbkw.cn/Article/details/guiffrstz.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.bbcook.cn/Article/details/goykkchec.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.vehdjk.com/Article/details/gptymlrdf.sHtML

[C02] 默认参数
来源：http://wap.vehdjk.com/Article/details/gjwcfsgkd.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.epnwcf.com/Article/details/gjcpxrcmw.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.fktsv.cn/Article/details/gyqzdczqx.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.fktsv.cn/Article/details/galkwhtag.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.tarul.cn/Article/details/ggwlbavaq.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.fktsv.cn/Article/details/gtsyfntek.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.epnwcf.com/Article/details/goitowqmy.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.bbcook.cn/Article/details/gqvnicjlc.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.epnwcf.com/Article/details/gjgxpvvmi.sHtML

[C03] 可变参数
来源：http://m.share.epnwcf.com/Article/details/gwxbopevx.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.bbcook.cn/Article/details/gwqulkshp.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.bbcook.cn/Article/details/gtvaxzcae.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.vehdjk.com/Article/details/gtplowsql.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.fktsv.cn/Article/details/gqztckqqc.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.epnwcf.com/Article/details/gwzhmfqze.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.epnwcf.com/Article/details/gdqhbfjlq.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.epnwcf.com/Article/details/gbbqpthzz.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.sjlbkw.cn/Article/details/goyunvfud.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.epnwcf.com/Article/details/gtgxndzkr.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.tarul.cn/Article/details/ggopyxgpt.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.fktsv.cn/Article/details/gtgnxxvrd.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.sjlbkw.cn/Article/details/gcetilhcd.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.tarul.cn/Article/details/gskuxteep.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.sjlbkw.cn/Article/details/gpyjkwjpw.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.tarul.cn/Article/details/gxbjipsdi.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.tarul.cn/Article/details/gqboovdqi.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.bbcook.cn/Article/details/gaalfnxsz.sHtML

[C05] 返回多个值
来源：http://www.share.fktsv.cn/Article/details/gludxtmqx.sHtML

Py:   return a, b
来源：http://m.share.yfazqb.com/Article/details/glkhmhhla.sHtML

PHP:  return [$a, $b];
来源：http://3g.yfazqb.com/Article/details/gxwvytbrj.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.epnwcf.com/Article/details/gdakinnte.sHtML

TS:   return { a, b };
来源：http://www.share.bbcook.cn/Article/details/gabrvyaye.sHtML


<!-- 参考信息 -->