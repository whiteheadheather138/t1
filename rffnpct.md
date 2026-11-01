代发 wailian999

[A14] 注释写法
来源：http://wap.yfazqb.com/Article/details/gdfznlfcl.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://mobile.yfazqb.com/Article/details/gmptwbaql.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.blog.vehdjk.com/Article/details/gknkfltic.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.m.share.yfazqb.com/Article/details/gnouawilo.sHtML

TS:   // 单行；/* 多行 */
来源：http://blog.yfazqb.com/Article/details/gqgesuykd.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.m.share.tarul.cn/Article/details/gnmlkwuis.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.m.share.sjlbkw.cn/Article/details/gxeoixkue.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.blog.tarul.cn/Article/details/gnerfyocv.sHtML

C#:   // 单行；/* 多行 */
来源：http://mobile.vehdjk.com/Article/details/gxgyominm.sHtML

[A15] 空值判断与默认值
来源：http://read.share.epnwcf.com/Article/details/gnocetols.sHtML

Py:   value = data or "默认值"
来源：http://blog.sjlbkw.cn/Article/details/gsdrifvjm.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://baike.sjlbkw.cn/Article/details/giauyuyfq.sHtML

JS:   const value = data ?? "默认值";
来源：http://mobile.bbcook.cn/Article/details/gfiwadoba.sHtML

TS:   const value = data ?? "默认值";
来源：http://3g.fktsv.cn/Article/details/gwqriohty.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://baike.vehdjk.com/Article/details/gphsxovcm.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://blog.yfazqb.com/Article/details/gtoyiiggp.sHtML

Ruby: value = data || "默认值"
来源：http://read.share.yfazqb.com/Article/details/gppfwmkep.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.blog.epnwcf.com/Article/details/gshuxwfsj.sHtML

[A16] 真假值判断规则
来源：http://mobile.tarul.cn/Article/details/ghtyomowp.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wap.epnwcf.com/Article/details/gzpolmvyx.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://baike.fktsv.cn/Article/details/gyfaopftg.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.m.share.tarul.cn/Article/details/glivwjxuf.sHtML

TS:   if (!x) {}
来源：http://www.share.sjlbkw.cn/Article/details/gghkfmtlr.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://3g.bbcook.cn/Article/details/gpkxfcbtb.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://m.share.bbcook.cn/Article/details/gntvjifcj.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://baike.bbcook.cn/Article/details/gurdvjkaa.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://3g.epnwcf.com/Article/details/gbestjptw.sHtML

[A17] 位运算
来源：http://wap.fktsv.cn/Article/details/gkffyrsog.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.vehdjk.com/Article/details/gzkfqzyxb.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wap.vehdjk.com/Article/details/gyajftdfb.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.vehdjk.com/Article/details/gaxscgbug.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://read.share.tarul.cn/Article/details/goqsyjyyl.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.sjlbkw.cn/Article/details/gewtswrhe.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.blog.yfazqb.com/Article/details/gxsabctbk.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.yfazqb.com/Article/details/gvaacxcpv.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.tarul.cn/Article/details/gnyflhakf.sHtML

[A18] 字符与 ASCII 码互转
来源：http://blog.epnwcf.com/Article/details/gjrpqabpr.sHtML

Py:   ord("A"); chr(65)
来源：http://www.blog.vehdjk.com/Article/details/gpsldaxwk.sHtML

PHP:  ord("A"); chr(65)
来源：http://baike.vehdjk.com/Article/details/gighwmiys.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.vehdjk.com/Article/details/geriwhcme.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.yfazqb.com/Article/details/gzdueyyne.sHtML

Java: (int) 'A'; (char) 65
来源：http://3g.sjlbkw.cn/Article/details/gvnxyopac.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.m.share.vehdjk.com/Article/details/gejyebmnt.sHtML

Ruby: "A".ord; 65.chr
来源：http://m.share.vehdjk.com/Article/details/gmmokhcfx.sHtML

C#:   (int)'A'; (char)65
来源：http://read.share.tarul.cn/Article/details/glptaeqij.sHtML

[A19] 交换两个变量
来源：http://read.share.epnwcf.com/Article/details/gdgqncovh.sHtML

Py:   a, b = b, a
来源：http://blog.vehdjk.com/Article/details/gwtozkvai.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://blog.fktsv.cn/Article/details/gyyuuiegd.sHtML

JS:   [a, b] = [b, a];
来源：http://mobile.yfazqb.com/Article/details/gjwbctrmc.sHtML

TS:   [a, b] = [b, a];
来源：http://baike.tarul.cn/Article/details/guncqbwdy.sHtML

Java: int t = a; a = b; b = t;
来源：http://wap.tarul.cn/Article/details/ggvupbwgh.sHtML

Go:   a, b = b, a
来源：http://mobile.yfazqb.com/Article/details/ghjknvdyg.sHtML

Ruby: a, b = b, a
来源：http://mobile.sjlbkw.cn/Article/details/gvmhwjnqt.sHtML

C#:   (a, b) = (b, a);
来源：http://www.m.share.bbcook.cn/Article/details/gaffyvrfy.sHtML

[A20] 读取标准输入
来源：http://mobile.bbcook.cn/Article/details/gkohtqbwa.sHtML

Py:   name = input("请输入：")
来源：http://www.share.bbcook.cn/Article/details/gdexwuaex.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.blog.yfazqb.com/Article/details/gjttyobyi.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://blog.vehdjk.com/Article/details/ggwlfejbe.sHtML

TS:   // Node.js：readline 模块
来源：http://read.share.tarul.cn/Article/details/gtllxwiul.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://read.share.epnwcf.com/Article/details/gtwmmjvia.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wap.tarul.cn/Article/details/gvccuqpvg.sHtML

Ruby: gets.chomp
来源：http://www.share.vehdjk.com/Article/details/gypechdbn.sHtML

C#:   Console.ReadLine();
来源：http://baike.bbcook.cn/Article/details/gdmixxpyf.sHtML

[A21] 保留指定小数位输出
来源：http://baike.yfazqb.com/Article/details/gzhvzhdtb.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.m.share.vehdjk.com/Article/details/gmbyuzsvi.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.blog.yfazqb.com/Article/details/gdouuoeyp.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.m.share.epnwcf.com/Article/details/gbvyjlaza.sHtML

TS:   (3.14159).toFixed(2)
来源：http://m.share.fktsv.cn/Article/details/gxzxjedsg.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://mobile.sjlbkw.cn/Article/details/gteywvcwc.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://m.share.yfazqb.com/Article/details/gjekxsirw.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://3g.sjlbkw.cn/Article/details/gzrgreepe.sHtML

C#:   3.14159.ToString("F2")
来源：http://wap.tarul.cn/Article/details/gelvjredq.sHtML

[A22] 获取字符串长度
来源：http://blog.vehdjk.com/Article/details/gajxzwurr.sHtML

Py:   len(s)
来源：http://www.share.yfazqb.com/Article/details/gipkeqmjs.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.m.share.epnwcf.com/Article/details/gquebayjv.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://blog.yfazqb.com/Article/details/gylxrrlai.sHtML

TS:   s.length
来源：http://3g.tarul.cn/Article/details/gnpddqmmb.sHtML

Java: s.length()
来源：http://3g.sjlbkw.cn/Article/details/gbqbtxzrb.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mobile.yfazqb.com/Article/details/gzlwguqyr.sHtML

Ruby: s.length
来源：http://blog.vehdjk.com/Article/details/gqefttsjw.sHtML

C#:   s.Length
来源：http://baike.yfazqb.com/Article/details/gzhkurnsf.sHtML

[A23] 大小写转换
来源：http://blog.vehdjk.com/Article/details/gxpgzutoj.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://3g.tarul.cn/Article/details/gbuuaxkkx.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wap.bbcook.cn/Article/details/gcmsdkzzl.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.tarul.cn/Article/details/gffeljcly.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.tarul.cn/Article/details/gcorangms.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wap.fktsv.cn/Article/details/gmumlywxo.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mobile.vehdjk.com/Article/details/grsivwrfq.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.blog.yfazqb.com/Article/details/gpnnirast.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://wap.tarul.cn/Article/details/gxlrslcge.sHtML

[A24] 去除首尾空白
来源：http://www.share.sjlbkw.cn/Article/details/gdzadiyzr.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://3g.tarul.cn/Article/details/grvbyfmzd.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://3g.fktsv.cn/Article/details/gjstyoecx.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.epnwcf.com/Article/details/gzgasiuto.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.tarul.cn/Article/details/gucnnweru.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://baike.fktsv.cn/Article/details/gxofnkcau.sHtML

Go:   strings.TrimSpace(s)
来源：http://blog.bbcook.cn/Article/details/gmhknzozo.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.share.bbcook.cn/Article/details/gyxibhvjk.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://blog.bbcook.cn/Article/details/gparsdyeb.sHtML

[A25] 字符串比较
来源：http://3g.fktsv.cn/Article/details/gwgmegffp.sHtML

Py:   s1 == s2; s1 != s2
来源：http://m.share.sjlbkw.cn/Article/details/gsmtgxfgh.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.share.fktsv.cn/Article/details/gflrzjhfs.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.bbcook.cn/Article/details/gghdkqozr.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.sjlbkw.cn/Article/details/gheiztlzn.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://3g.fktsv.cn/Article/details/grjqujtnj.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://3g.sjlbkw.cn/Article/details/gmgamesew.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.blog.yfazqb.com/Article/details/ghddayuyj.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.share.bbcook.cn/Article/details/gdkbqlokp.sHtML

[A26] 类型转换总览
来源：http://www.m.share.epnwcf.com/Article/details/gpsafngvf.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://read.share.epnwcf.com/Article/details/gsjaiaytu.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://read.share.epnwcf.com/Article/details/gtothwmaz.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://blog.bbcook.cn/Article/details/gauvwkzst.sHtML

TS:   Number() String() Boolean() x as number
来源：http://mobile.tarul.cn/Article/details/gidxbrdjv.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://read.share.bbcook.cn/Article/details/gunwozgmx.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.m.share.sjlbkw.cn/Article/details/gmgdggecg.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://blog.fktsv.cn/Article/details/gckfyjynf.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://baike.bbcook.cn/Article/details/gpwwmiiyw.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gsxpzpdvu.sHtML

B. 流程控制
来源：http://mobile.yfazqb.com/Article/details/gbnicbavv.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gfysfukmm.sHtML

[B01] 条件判断 if / else
来源：http://read.share.sjlbkw.cn/Article/details/gcqnscjpo.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.share.tarul.cn/Article/details/gnmkqnasw.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://baike.yfazqb.com/Article/details/gxreggsme.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.bbcook.cn/Article/details/gvdqnxfqk.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.epnwcf.com/Article/details/gzneiwoph.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://m.share.yfazqb.com/Article/details/gwigppjyo.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.m.share.vehdjk.com/Article/details/gzwtahpsb.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://read.share.epnwcf.com/Article/details/gwidscyol.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.share.tarul.cn/Article/details/gjhnqvhaa.sHtML

[B02] 多分支 else if / elif
来源：http://www.m.share.epnwcf.com/Article/details/gmyfkigiw.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://baike.sjlbkw.cn/Article/details/gsmsguptt.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://blog.yfazqb.com/Article/details/gnlvjazrf.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.sjlbkw.cn/Article/details/gjzceeggd.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.bbcook.cn/Article/details/gydxnrfmq.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.vehdjk.com/Article/details/gxavboukp.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.m.share.fktsv.cn/Article/details/guwunuejc.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://blog.sjlbkw.cn/Article/details/gjzpceavu.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.bbcook.cn/Article/details/gsshxmdxd.sHtML

[B03] switch / match / case
来源：http://3g.sjlbkw.cn/Article/details/ghjlwatfi.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.blog.fktsv.cn/Article/details/gsnbwiwdc.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.blog.epnwcf.com/Article/details/gsoykyocm.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.epnwcf.com/Article/details/gdbcocuor.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.yfazqb.com/Article/details/gkdixwfff.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.sjlbkw.cn/Article/details/gkctimrmw.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.blog.epnwcf.com/Article/details/gvfesnjpf.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://read.share.epnwcf.com/Article/details/gqyysgzsl.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://m.share.yfazqb.com/Article/details/giwvcgssq.sHtML

[B04] for 计数循环
来源：http://www.blog.yfazqb.com/Article/details/gwhjxnddo.sHtML

Py:   for i in range(10): print(i)
来源：http://wap.yfazqb.com/Article/details/gtmtrxnxf.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wap.bbcook.cn/Article/details/gvvtwuewu.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.yfazqb.com/Article/details/gkvdbomgm.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.bbcook.cn/Article/details/gnfqujnhv.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.fktsv.cn/Article/details/gbfmkanac.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.share.fktsv.cn/Article/details/gguvlzulo.sHtML

Ruby: 10.times { |i| puts i }
来源：http://wap.yfazqb.com/Article/details/gjhfvdnov.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://3g.bbcook.cn/Article/details/gcbzqrkto.sHtML

[B05] 遍历数组 / 列表
来源：http://read.share.yfazqb.com/Article/details/ghicdmxbo.sHtML

Py:   for item in arr: print(item)
来源：http://m.share.fktsv.cn/Article/details/gszujjepf.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://m.share.vehdjk.com/Article/details/gzxohemnj.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://3g.vehdjk.com/Article/details/gfvcnlirg.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.fktsv.cn/Article/details/gnnlwysct.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.epnwcf.com/Article/details/gowwnnavm.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.fktsv.cn/Article/details/gruyuetmc.sHtML

Ruby: arr.each { |item| puts item }
来源：http://3g.tarul.cn/Article/details/gylamuyly.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.m.share.fktsv.cn/Article/details/glemsykjh.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.yfazqb.com/Article/details/gpgkoojco.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.vehdjk.com/Article/details/gdedkthac.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://3g.sjlbkw.cn/Article/details/ghjtqzswi.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.bbcook.cn/Article/details/glmyctdfn.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.fktsv.cn/Article/details/gnuujxctl.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://baike.sjlbkw.cn/Article/details/gffoqgkug.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.epnwcf.com/Article/details/giqkuyzed.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.bbcook.cn/Article/details/grppqoyid.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wap.vehdjk.com/Article/details/guzihqzsp.sHtML

[B07] while 循环
来源：http://www.blog.bbcook.cn/Article/details/gzpjnkypn.sHtML

Py:   while i < 10: i += 1
来源：http://blog.bbcook.cn/Article/details/gafkqwqay.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.share.sjlbkw.cn/Article/details/ghgekwceh.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.bbcook.cn/Article/details/gkorfkxsy.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.share.bbcook.cn/Article/details/guoruvjcz.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.sjlbkw.cn/Article/details/ghtkcdwhf.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.share.bbcook.cn/Article/details/guhovrswm.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.yfazqb.com/Article/details/gepdfnkfk.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.yfazqb.com/Article/details/gfsqxppai.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.yfazqb.com/Article/details/ghdayfhbw.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.yfazqb.com/Article/details/ggzwyryeo.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.tarul.cn/Article/details/gpupfnxor.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.tarul.cn/Article/details/glhnjitzs.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.yfazqb.com/Article/details/gllgekkgl.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.epnwcf.com/Article/details/gugbqzluk.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.bbcook.cn/Article/details/gspyfafao.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.bbcook.cn/Article/details/gucvcchvv.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.yfazqb.com/Article/details/gvtajmasr.sHtML

[B09] break 与 continue
来源：http://mobile.tarul.cn/Article/details/gkpppxnrz.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.share.bbcook.cn/Article/details/ghshwsjqs.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.epnwcf.com/Article/details/gorssyevt.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.bbcook.cn/Article/details/ggethbbzo.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.bbcook.cn/Article/details/gjlgmfbmg.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.yfazqb.com/Article/details/gacwbefkc.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.sjlbkw.cn/Article/details/gpekjxchm.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.fktsv.cn/Article/details/gyylbxezm.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gmsifmzqq.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.bbcook.cn/Article/details/gittthfai.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.bbcook.cn/Article/details/ghhulcwav.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.vehdjk.com/Article/details/gipvttrwi.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.yfazqb.com/Article/details/gjnquycma.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.vehdjk.com/Article/details/ggfkczgqe.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.fktsv.cn/Article/details/ggjfqsuxa.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.fktsv.cn/Article/details/gwndzozcz.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.tarul.cn/Article/details/ghzyxpnrv.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.fktsv.cn/Article/details/gkqipwzzh.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.vehdjk.com/Article/details/gojbweguo.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.bbcook.cn/Article/details/grmnnajdc.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.vehdjk.com/Article/details/ghwvgwinn.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.sjlbkw.cn/Article/details/gcxillisf.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.epnwcf.com/Article/details/gnkinmjxt.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.bbcook.cn/Article/details/gwlrajqhi.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.epnwcf.com/Article/details/gmakigmcu.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.epnwcf.com/Article/details/gctihwvvl.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.vehdjk.com/Article/details/gzmdmzqsp.sHtML

[B12] 跳出多层循环
来源：http://m.share.sjlbkw.cn/Article/details/garlixxgb.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.vehdjk.com/Article/details/gcpnkpybq.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.epnwcf.com/Article/details/gwspwlkts.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.yfazqb.com/Article/details/gzfgustjx.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.yfazqb.com/Article/details/gzkiqmxun.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.vehdjk.com/Article/details/gelunaksl.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.yfazqb.com/Article/details/gdqfxdfiq.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.bbcook.cn/Article/details/gklcdtjxh.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.epnwcf.com/Article/details/gqaqbnwxr.sHtML

[B13] 判断是否为数字
来源：http://mobile.yfazqb.com/Article/details/gynwkxjau.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.yfazqb.com/Article/details/gapqesxfi.sHtML

PHP:  is_numeric($x)
来源：http://mobile.yfazqb.com/Article/details/gabcigysi.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.sjlbkw.cn/Article/details/gnvbjmsla.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.yfazqb.com/Article/details/grtvvesxy.sHtML

Java: x instanceof Number
来源：http://wap.fktsv.cn/Article/details/gtceyyoio.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.sjlbkw.cn/Article/details/gdvkxunbr.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.sjlbkw.cn/Article/details/gykouogiv.sHtML

C#:   x is int or double or decimal
来源：http://www.share.yfazqb.com/Article/details/gdqbqntok.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.tarul.cn/Article/details/gdfncmsdb.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.yfazqb.com/Article/details/gmxpiudhz.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.fktsv.cn/Article/details/gwqdnwxcr.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.epnwcf.com/Article/details/gnpqoplpu.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.epnwcf.com/Article/details/gjnhftxpg.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.bbcook.cn/Article/details/geozuzbyv.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.bbcook.cn/Article/details/gjwtxkjmt.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.bbcook.cn/Article/details/glsekbuus.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.fktsv.cn/Article/details/gvzkmibdp.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.sjlbkw.cn/Article/details/garqyjirs.sHtML

Py:   a and b or not c
来源：http://blog.tarul.cn/Article/details/gypsaqxmp.sHtML

PHP:  $a && $b || !$c
来源：http://blog.bbcook.cn/Article/details/gsbwbfldd.sHtML

JS:   a && b || !c
来源：http://mobile.vehdjk.com/Article/details/gtmeulfvx.sHtML

TS:   a && b || !c
来源：http://read.share.sjlbkw.cn/Article/details/gamaeltzn.sHtML

Java: a && b || !c
来源：http://blog.sjlbkw.cn/Article/details/gucuklttx.sHtML

Go:   a && b || !c
来源：http://wap.tarul.cn/Article/details/gzpgkebvg.sHtML

Ruby: a && b || !c
来源：http://www.share.epnwcf.com/Article/details/goqnkxsri.sHtML

C#:   a && b || !c
来源：http://blog.bbcook.cn/Article/details/gxhpikfwv.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.tarul.cn/Article/details/gubpfmkwh.sHtML

Py:   if not data: return
来源：http://3g.fktsv.cn/Article/details/gwdsaxyvz.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.bbcook.cn/Article/details/glxdgkabi.sHtML

JS:   if (!data) return;
来源：http://3g.epnwcf.com/Article/details/gdykoiqcu.sHtML

TS:   if (!data) return;
来源：http://blog.fktsv.cn/Article/details/girwypylt.sHtML

Java: if (data == null) return;
来源：http://mobile.vehdjk.com/Article/details/gowekawtt.sHtML

Go:   if data == nil { return }
来源：http://3g.vehdjk.com/Article/details/ghbcadmsi.sHtML

Ruby: return if data.nil?
来源：http://blog.fktsv.cn/Article/details/gozwdxdhw.sHtML

C#:   if (data == null) return;
来源：http://read.share.tarul.cn/Article/details/gnfctvysr.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gugggmvqq.sHtML

C. 函数与作用域
来源：http://read.share.tarul.cn/Article/details/gtqnanfvf.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gnnzdcbdy.sHtML

[C01] 定义函数
来源：http://www.m.share.tarul.cn/Article/details/gjrqfuvhl.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.vehdjk.com/Article/details/gaqvqaiun.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.yfazqb.com/Article/details/gxiliihyp.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.epnwcf.com/Article/details/gqmhgkjut.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.vehdjk.com/Article/details/gumwazcep.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.sjlbkw.cn/Article/details/gavgpjmnx.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.bbcook.cn/Article/details/gcrvvpjiz.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.vehdjk.com/Article/details/ggeqfakav.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.fktsv.cn/Article/details/gmnmzbuvu.sHtML

[C02] 默认参数
来源：http://baike.vehdjk.com/Article/details/gohkyiccf.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.sjlbkw.cn/Article/details/gbrfymosr.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.tarul.cn/Article/details/gdoiclctq.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.yfazqb.com/Article/details/gfisbabsm.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.tarul.cn/Article/details/gxuttrgrt.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.vehdjk.com/Article/details/gouhqdowr.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.vehdjk.com/Article/details/gxriapxpn.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.yfazqb.com/Article/details/glrfcctvp.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.vehdjk.com/Article/details/gveydlsvn.sHtML

[C03] 可变参数
来源：http://read.share.epnwcf.com/Article/details/gaesxsfyl.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.epnwcf.com/Article/details/gsjutycls.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.bbcook.cn/Article/details/galjbzgec.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gjtwcoejs.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.yfazqb.com/Article/details/gqymxkmbo.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.bbcook.cn/Article/details/gtradxrky.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.fktsv.cn/Article/details/gvezkietx.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.epnwcf.com/Article/details/glkbfhomc.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.fktsv.cn/Article/details/gqhafqlzr.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.fktsv.cn/Article/details/ggtyrzcdg.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.fktsv.cn/Article/details/gvthbwaoo.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.bbcook.cn/Article/details/gyqiofjlz.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.sjlbkw.cn/Article/details/ggatjuzjt.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.fktsv.cn/Article/details/goarxuzna.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.fktsv.cn/Article/details/gpqgqnskg.sHtML


<!-- 参考信息 -->