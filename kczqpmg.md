代发 wailian999

TS:   // 单行；/* 多行 */
来源：http://blog.fktsv.cn/Article/details/gdojlintp.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://3g.bbcook.cn/Article/details/gnqtskusl.sHtML

Go:   // 单行；/* 多行 */
来源：http://3g.tarul.cn/Article/details/grblegkme.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.m.share.epnwcf.com/Article/details/gikmpvgdk.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.blog.fktsv.cn/Article/details/gjsscmewz.sHtML

[A15] 空值判断与默认值
来源：http://read.share.yfazqb.com/Article/details/ghyhbewrc.sHtML

Py:   value = data or "默认值"
来源：http://3g.fktsv.cn/Article/details/gesqtscaa.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://read.share.yfazqb.com/Article/details/gpsttazeb.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.m.share.tarul.cn/Article/details/gmpqdmoqm.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.share.fktsv.cn/Article/details/gmcivzveg.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.blog.epnwcf.com/Article/details/gdqxsegzj.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.m.share.tarul.cn/Article/details/gfvmbxdth.sHtML

Ruby: value = data || "默认值"
来源：http://m.share.tarul.cn/Article/details/gopkunvjj.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.blog.fktsv.cn/Article/details/gedndblsp.sHtML

[A16] 真假值判断规则
来源：http://wap.bbcook.cn/Article/details/gaobdzxtx.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://3g.vehdjk.com/Article/details/gpnmldexs.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://m.share.fktsv.cn/Article/details/galjlpnjh.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://blog.bbcook.cn/Article/details/gbhxsmlsj.sHtML

TS:   if (!x) {}
来源：http://www.m.share.bbcook.cn/Article/details/gwancsrux.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://baike.vehdjk.com/Article/details/gutxzprgw.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://blog.bbcook.cn/Article/details/gjijrwgig.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://baike.tarul.cn/Article/details/gomtntswf.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://baike.epnwcf.com/Article/details/gzichbyyl.sHtML

[A17] 位运算
来源：http://3g.vehdjk.com/Article/details/gfqcrxcat.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.yfazqb.com/Article/details/gbusjpzaa.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://baike.bbcook.cn/Article/details/gkhbcewhm.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.sjlbkw.cn/Article/details/gkeulyeev.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.share.sjlbkw.cn/Article/details/gbsdtwfzp.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.sjlbkw.cn/Article/details/gairvtgub.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://3g.fktsv.cn/Article/details/golzswsae.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.yfazqb.com/Article/details/ganwtmumu.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.vehdjk.com/Article/details/gqffwxsch.sHtML

[A18] 字符与 ASCII 码互转
来源：http://blog.fktsv.cn/Article/details/gapzqvwqr.sHtML

Py:   ord("A"); chr(65)
来源：http://3g.sjlbkw.cn/Article/details/gyuwwdruj.sHtML

PHP:  ord("A"); chr(65)
来源：http://mobile.vehdjk.com/Article/details/gokrbtyok.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.yfazqb.com/Article/details/gmsqzjinl.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.sjlbkw.cn/Article/details/gvgcbojjo.sHtML

Java: (int) 'A'; (char) 65
来源：http://blog.fktsv.cn/Article/details/gkuqaxmdk.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://3g.epnwcf.com/Article/details/gagnixqgg.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.share.bbcook.cn/Article/details/gjnpjufyk.sHtML

C#:   (int)'A'; (char)65
来源：http://read.share.fktsv.cn/Article/details/gghjxnolw.sHtML

[A19] 交换两个变量
来源：http://www.share.epnwcf.com/Article/details/gcibvizqf.sHtML

Py:   a, b = b, a
来源：http://blog.yfazqb.com/Article/details/gfowhgdlf.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://3g.yfazqb.com/Article/details/giehljjqg.sHtML

JS:   [a, b] = [b, a];
来源：http://www.share.sjlbkw.cn/Article/details/grqnyxouq.sHtML

TS:   [a, b] = [b, a];
来源：http://m.share.vehdjk.com/Article/details/gwmyydipb.sHtML

Java: int t = a; a = b; b = t;
来源：http://read.share.vehdjk.com/Article/details/grzosybol.sHtML

Go:   a, b = b, a
来源：http://3g.epnwcf.com/Article/details/gktourwtr.sHtML

Ruby: a, b = b, a
来源：http://www.m.share.epnwcf.com/Article/details/gvyrccomd.sHtML

C#:   (a, b) = (b, a);
来源：http://3g.epnwcf.com/Article/details/gzmfgtizx.sHtML

[A20] 读取标准输入
来源：http://mobile.epnwcf.com/Article/details/gloaijuhp.sHtML

Py:   name = input("请输入：")
来源：http://baike.vehdjk.com/Article/details/ggzvyjhek.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.m.share.tarul.cn/Article/details/gwxhkxarn.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://m.share.epnwcf.com/Article/details/ghqhebkmp.sHtML

TS:   // Node.js：readline 模块
来源：http://read.share.vehdjk.com/Article/details/gfwfumsnx.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://m.share.yfazqb.com/Article/details/gwfmyuhrh.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wap.epnwcf.com/Article/details/gdclcgyzy.sHtML

Ruby: gets.chomp
来源：http://read.share.fktsv.cn/Article/details/grhzkdbhy.sHtML

C#:   Console.ReadLine();
来源：http://3g.vehdjk.com/Article/details/gbcvclxqg.sHtML

[A21] 保留指定小数位输出
来源：http://wap.yfazqb.com/Article/details/gigjykpcv.sHtML

Py:   f"{3.14159:.2f}"
来源：http://blog.tarul.cn/Article/details/gpuxfzrev.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://m.share.sjlbkw.cn/Article/details/gibtvvsst.sHtML

JS:   (3.14159).toFixed(2)
来源：http://blog.sjlbkw.cn/Article/details/gumqtcmnj.sHtML

TS:   (3.14159).toFixed(2)
来源：http://m.share.tarul.cn/Article/details/gzamqtovy.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://baike.yfazqb.com/Article/details/gifijcxjw.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://read.share.epnwcf.com/Article/details/gjrkkfawu.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.share.fktsv.cn/Article/details/gdenuddvj.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.share.yfazqb.com/Article/details/guirgvokx.sHtML

[A22] 获取字符串长度
来源：http://baike.bbcook.cn/Article/details/glammczit.sHtML

Py:   len(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gnzuayihy.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.blog.fktsv.cn/Article/details/gncwdxeei.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://3g.vehdjk.com/Article/details/gatcxplcj.sHtML

TS:   s.length
来源：http://www.m.share.bbcook.cn/Article/details/gewajdary.sHtML

Java: s.length()
来源：http://wap.bbcook.cn/Article/details/gkzvopfaf.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.m.share.vehdjk.com/Article/details/gimrsyuvj.sHtML

Ruby: s.length
来源：http://mobile.epnwcf.com/Article/details/glaxpsxru.sHtML

C#:   s.Length
来源：http://mobile.vehdjk.com/Article/details/gojyltsvt.sHtML

[A23] 大小写转换
来源：http://www.blog.yfazqb.com/Article/details/gkaajvcje.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.share.tarul.cn/Article/details/gwaelkrhy.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wap.vehdjk.com/Article/details/gfkfdulxr.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.bbcook.cn/Article/details/gpkjtcxsg.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.yfazqb.com/Article/details/gghupyhku.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.bbcook.cn/Article/details/glaxgdter.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://m.share.sjlbkw.cn/Article/details/giolmuktx.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wap.bbcook.cn/Article/details/gfngpzxwa.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://baike.yfazqb.com/Article/details/gwgldtnrm.sHtML

[A24] 去除首尾空白
来源：http://read.share.sjlbkw.cn/Article/details/goxljvswv.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://m.share.tarul.cn/Article/details/gysmuwpzu.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://3g.tarul.cn/Article/details/gghraywvj.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.tarul.cn/Article/details/gavzcfoja.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.yfazqb.com/Article/details/gqpdqkqiw.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://m.share.tarul.cn/Article/details/goejajqmj.sHtML

Go:   strings.TrimSpace(s)
来源：http://wap.sjlbkw.cn/Article/details/goupwnbee.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mobile.vehdjk.com/Article/details/gujccdceu.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://blog.tarul.cn/Article/details/gesipatex.sHtML

[A25] 字符串比较
来源：http://mobile.fktsv.cn/Article/details/gagzsbfjq.sHtML

Py:   s1 == s2; s1 != s2
来源：http://read.share.fktsv.cn/Article/details/gakadruko.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://read.share.tarul.cn/Article/details/gzrekvphe.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.tarul.cn/Article/details/gjvzhugyv.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.bbcook.cn/Article/details/gsxxrpjdd.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.m.share.epnwcf.com/Article/details/ghrvjhsqd.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://baike.epnwcf.com/Article/details/ggghlfset.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://mobile.tarul.cn/Article/details/gyculmjfr.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.share.epnwcf.com/Article/details/gckhvcldc.sHtML

[A26] 类型转换总览
来源：http://www.m.share.bbcook.cn/Article/details/gpatmhupr.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://baike.vehdjk.com/Article/details/gkozsvvku.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://read.share.tarul.cn/Article/details/gmfqvmdoy.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.m.share.tarul.cn/Article/details/guvsjryjx.sHtML

TS:   Number() String() Boolean() x as number
来源：http://baike.vehdjk.com/Article/details/grrarlnwp.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://baike.sjlbkw.cn/Article/details/goxobavag.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://blog.sjlbkw.cn/Article/details/gcebepoqr.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://blog.bbcook.cn/Article/details/gotluwxhh.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://3g.fktsv.cn/Article/details/gsvhjmutn.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/guqxciqaq.sHtML

B. 流程控制
来源：http://www.blog.vehdjk.com/Article/details/gtjpddqwr.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/ggpfmszgr.sHtML

[B01] 条件判断 if / else
来源：http://www.share.tarul.cn/Article/details/gjpijcbnc.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://blog.sjlbkw.cn/Article/details/gbgsvemkb.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://blog.fktsv.cn/Article/details/gcbohugrj.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.vehdjk.com/Article/details/gajbhgjgv.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.vehdjk.com/Article/details/gyfpcvzcd.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.share.fktsv.cn/Article/details/gtqbzoiwt.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://3g.fktsv.cn/Article/details/gzhdhaieq.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://3g.epnwcf.com/Article/details/gpamxekmy.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://baike.sjlbkw.cn/Article/details/gyzzvwzrx.sHtML

[B02] 多分支 else if / elif
来源：http://www.blog.vehdjk.com/Article/details/gabqnthnc.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wap.yfazqb.com/Article/details/ghisqjlgm.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://read.share.sjlbkw.cn/Article/details/gnozpdfvl.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.bbcook.cn/Article/details/gtyenaxdm.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.yfazqb.com/Article/details/guuwmsska.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.fktsv.cn/Article/details/gnndcouce.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.blog.tarul.cn/Article/details/gctuaffxe.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.share.fktsv.cn/Article/details/gvugdmqxw.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.tarul.cn/Article/details/gujybcaiw.sHtML

[B03] switch / match / case
来源：http://www.blog.fktsv.cn/Article/details/gunoktfks.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://m.share.epnwcf.com/Article/details/gyrxmdcbc.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://3g.bbcook.cn/Article/details/gxmqyiiaz.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.vehdjk.com/Article/details/gsezqfosw.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.epnwcf.com/Article/details/gyzrxzwpn.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://blog.sjlbkw.cn/Article/details/gbanmkisv.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://m.share.sjlbkw.cn/Article/details/ghqwsjuhm.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://baike.tarul.cn/Article/details/glshslvic.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.share.vehdjk.com/Article/details/gbephyvwq.sHtML

[B04] for 计数循环
来源：http://read.share.epnwcf.com/Article/details/gshmudomr.sHtML

Py:   for i in range(10): print(i)
来源：http://baike.fktsv.cn/Article/details/giugtptit.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.blog.fktsv.cn/Article/details/gsbdvstso.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.vehdjk.com/Article/details/ghacbnlsk.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.epnwcf.com/Article/details/gosxrneab.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://baike.yfazqb.com/Article/details/grlibxwka.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mobile.tarul.cn/Article/details/gmfawlngx.sHtML

Ruby: 10.times { |i| puts i }
来源：http://mobile.vehdjk.com/Article/details/gzanfrmjm.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.bbcook.cn/Article/details/gfbmtlmug.sHtML

[B05] 遍历数组 / 列表
来源：http://www.blog.sjlbkw.cn/Article/details/gpcjhdytp.sHtML

Py:   for item in arr: print(item)
来源：http://www.m.share.fktsv.cn/Article/details/gwbnlxhzi.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.tarul.cn/Article/details/ghcdlizwn.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://m.share.epnwcf.com/Article/details/gbyzsmigh.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://mobile.sjlbkw.cn/Article/details/gtyllkdss.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://mobile.sjlbkw.cn/Article/details/gcrskbdzk.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.share.yfazqb.com/Article/details/gdgrgzpud.sHtML

Ruby: arr.each { |item| puts item }
来源：http://mobile.epnwcf.com/Article/details/gnywkztge.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://3g.epnwcf.com/Article/details/gnyixcbiq.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.vehdjk.com/Article/details/gpgowkfts.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.epnwcf.com/Article/details/geburghea.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://blog.vehdjk.com/Article/details/ghxmtsyrq.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.tarul.cn/Article/details/gohxmtdin.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.yfazqb.com/Article/details/gapczwxtq.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.vehdjk.com/Article/details/gmcitjihe.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.fktsv.cn/Article/details/gjiqkwysb.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.sjlbkw.cn/Article/details/gxzaqnukg.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mobile.bbcook.cn/Article/details/goqgdzzxq.sHtML

[B07] while 循环
来源：http://3g.sjlbkw.cn/Article/details/goctxvwyv.sHtML

Py:   while i < 10: i += 1
来源：http://www.share.vehdjk.com/Article/details/gemcgfetw.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.yfazqb.com/Article/details/glyxktngs.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.tarul.cn/Article/details/gwyjmthjj.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.epnwcf.com/Article/details/gxvqmstul.sHtML

Java: while (i < 10) { i++; }
来源：http://m.share.vehdjk.com/Article/details/ggqvmdzdb.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.vehdjk.com/Article/details/gsokzviat.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.fktsv.cn/Article/details/gdiwuajuc.sHtML

C#:   while (i < 10) { i++; }
来源：http://m.share.bbcook.cn/Article/details/gondoihxk.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.sjlbkw.cn/Article/details/gvpvkxtlb.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://blog.fktsv.cn/Article/details/gwrbcycmp.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.fktsv.cn/Article/details/gktwubvdm.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.yfazqb.com/Article/details/gwgggxogg.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.yfazqb.com/Article/details/grfrfbmtv.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.share.fktsv.cn/Article/details/gmrxwrslk.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.bbcook.cn/Article/details/gjlpuwzlh.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://m.share.tarul.cn/Article/details/grakylqbi.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.bbcook.cn/Article/details/gwaeczccc.sHtML

[B09] break 与 continue
来源：http://read.share.tarul.cn/Article/details/gbypymbar.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.tarul.cn/Article/details/grsdtnlya.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.tarul.cn/Article/details/gvcehdclq.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.epnwcf.com/Article/details/gxowtccvq.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.tarul.cn/Article/details/gerfxdrxq.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fktsv.cn/Article/details/ghppvolks.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.yfazqb.com/Article/details/gsymdhkuk.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.yfazqb.com/Article/details/gjbjqcwtp.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fktsv.cn/Article/details/grtluhwdt.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.vehdjk.com/Article/details/gmzfzfauo.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.sjlbkw.cn/Article/details/gfjdngqzw.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.bbcook.cn/Article/details/gciclrync.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.fktsv.cn/Article/details/gpxgpehiy.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.tarul.cn/Article/details/gaejiiipg.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.vehdjk.com/Article/details/gxiggbalh.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.fktsv.cn/Article/details/gkalnozxn.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.sjlbkw.cn/Article/details/gpfxjhchk.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.sjlbkw.cn/Article/details/grjcigjhn.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.blog.epnwcf.com/Article/details/gdtxrkkcn.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.vehdjk.com/Article/details/gdrxcuijb.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.vehdjk.com/Article/details/gtcllvaqn.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.sjlbkw.cn/Article/details/gfcstaret.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.vehdjk.com/Article/details/gutkgbewm.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.fktsv.cn/Article/details/godlyezls.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.tarul.cn/Article/details/gdujqgzcn.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.yfazqb.com/Article/details/guztmakfw.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.yfazqb.com/Article/details/gzunkhxqb.sHtML

[B12] 跳出多层循环
来源：http://3g.tarul.cn/Article/details/gcwurpwjr.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.yfazqb.com/Article/details/gontatuhi.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.bbcook.cn/Article/details/gwqipwxkt.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.epnwcf.com/Article/details/gjudtvgfo.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.tarul.cn/Article/details/gcxjpnyfw.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.tarul.cn/Article/details/greaaljwx.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.epnwcf.com/Article/details/gwgwhwvey.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.tarul.cn/Article/details/gogdymssm.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.fktsv.cn/Article/details/gdetxjwkh.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.tarul.cn/Article/details/gcfljaint.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.yfazqb.com/Article/details/gyvquprvf.sHtML

PHP:  is_numeric($x)
来源：http://blog.fktsv.cn/Article/details/gnrsnzmlq.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.epnwcf.com/Article/details/gvsmwaezx.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.tarul.cn/Article/details/gpghjfhwa.sHtML

Java: x instanceof Number
来源：http://mobile.epnwcf.com/Article/details/gqqhmmcxp.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.bbcook.cn/Article/details/gdxgmgijk.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.bbcook.cn/Article/details/gjakwarve.sHtML

C#:   x is int or double or decimal
来源：http://m.share.vehdjk.com/Article/details/glchcoiuh.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.sjlbkw.cn/Article/details/ghhwmnosi.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.epnwcf.com/Article/details/gllzjjphh.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.sjlbkw.cn/Article/details/gnzgcpeih.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.bbcook.cn/Article/details/gotrevmog.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.yfazqb.com/Article/details/grcvcbyxe.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.epnwcf.com/Article/details/gkcnsrnyh.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.bbcook.cn/Article/details/gkozeqouy.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.vehdjk.com/Article/details/gcsvyofwb.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghcsewawh.sHtML

[B15] 布尔运算与取反
来源：http://mobile.bbcook.cn/Article/details/gyjbipbkq.sHtML

Py:   a and b or not c
来源：http://3g.vehdjk.com/Article/details/gkvnztyqr.sHtML

PHP:  $a && $b || !$c
来源：http://3g.epnwcf.com/Article/details/gzlbjqixt.sHtML

JS:   a && b || !c
来源：http://3g.fktsv.cn/Article/details/gfeudatsf.sHtML

TS:   a && b || !c
来源：http://read.share.tarul.cn/Article/details/gcgmfajdl.sHtML

Java: a && b || !c
来源：http://m.share.yfazqb.com/Article/details/ggrpsxldj.sHtML

Go:   a && b || !c
来源：http://www.blog.vehdjk.com/Article/details/gftqlnrvz.sHtML

Ruby: a && b || !c
来源：http://blog.yfazqb.com/Article/details/gndbsfzpv.sHtML

C#:   a && b || !c
来源：http://baike.sjlbkw.cn/Article/details/gzrrhfyio.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.epnwcf.com/Article/details/grfdgfadz.sHtML

Py:   if not data: return
来源：http://www.blog.bbcook.cn/Article/details/gpshclckt.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.yfazqb.com/Article/details/gbuqwtbiu.sHtML

JS:   if (!data) return;
来源：http://www.blog.fktsv.cn/Article/details/gwwlqcrgl.sHtML

TS:   if (!data) return;
来源：http://blog.bbcook.cn/Article/details/gofagoccz.sHtML

Java: if (data == null) return;
来源：http://baike.vehdjk.com/Article/details/gtylxybgg.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.bbcook.cn/Article/details/gldcocifr.sHtML

Ruby: return if data.nil?
来源：http://www.share.yfazqb.com/Article/details/gmgetmpoh.sHtML

C#:   if (data == null) return;
来源：http://3g.sjlbkw.cn/Article/details/gqswsjnvy.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gpbtvjika.sHtML

C. 函数与作用域
来源：http://3g.vehdjk.com/Article/details/gtmyiggye.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gujlrcnot.sHtML

[C01] 定义函数
来源：http://blog.epnwcf.com/Article/details/gnzhgagnf.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.bbcook.cn/Article/details/gsquvqffa.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.bbcook.cn/Article/details/gkmrornei.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.bbcook.cn/Article/details/gfzehtvzd.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.sjlbkw.cn/Article/details/gwkjhqciz.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.vehdjk.com/Article/details/gjahgjyhm.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.vehdjk.com/Article/details/gzwgkjxbq.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.sjlbkw.cn/Article/details/geysagjvr.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.yfazqb.com/Article/details/gpjurvdta.sHtML

[C02] 默认参数
来源：http://www.share.tarul.cn/Article/details/gllflfwxd.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.bbcook.cn/Article/details/gltqdcsyg.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.tarul.cn/Article/details/gilbcpycq.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.fktsv.cn/Article/details/gvbwxdfks.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.sjlbkw.cn/Article/details/gskpieili.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.tarul.cn/Article/details/gcnpqqxsw.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.tarul.cn/Article/details/gqbdzyfqk.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.fktsv.cn/Article/details/grlaghqeo.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.yfazqb.com/Article/details/gynxfzvxn.sHtML

[C03] 可变参数
来源：http://3g.tarul.cn/Article/details/gtuzbcogj.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.epnwcf.com/Article/details/gqqvxjpck.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.fktsv.cn/Article/details/gifkmsoai.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.bbcook.cn/Article/details/ghoxpraya.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.tarul.cn/Article/details/gblokyvrf.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.vehdjk.com/Article/details/gjclxfwwh.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.tarul.cn/Article/details/gvzakisyj.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.vehdjk.com/Article/details/gimolpxqn.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.bbcook.cn/Article/details/gftdxtnkc.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.yfazqb.com/Article/details/ggzbmfdkb.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.bbcook.cn/Article/details/gkjahqlnk.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.fktsv.cn/Article/details/gjswdheyj.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.bbcook.cn/Article/details/gwpjwldhk.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.tarul.cn/Article/details/gimcixfgj.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.vehdjk.com/Article/details/gjasctonv.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.tarul.cn/Article/details/gaimbabyj.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.bbcook.cn/Article/details/grfwhobiz.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.fktsv.cn/Article/details/gmltqtkdy.sHtML

[C05] 返回多个值
来源：http://wap.sjlbkw.cn/Article/details/gznfkfbtc.sHtML


<!-- 参考信息 -->