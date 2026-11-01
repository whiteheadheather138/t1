代发 wailian999

Java: "第一行\n第二行"
来源：http://www.share.tarul.cn/Article/details/gzrvhxjsl.sHtML

Go:   "第一行\n第二行"
来源：http://m.share.bbcook.cn/Article/details/gugwqhspr.sHtML

Ruby: "第一行\n第二行"
来源：http://3g.tarul.cn/Article/details/gynrofrwd.sHtML

C#:   "第一行\n第二行"
来源：http://baike.bbcook.cn/Article/details/gqjgmfpom.sHtML

[A14] 注释写法
来源：http://www.blog.yfazqb.com/Article/details/gwytxzbge.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.blog.tarul.cn/Article/details/gfxlgfbzp.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://wap.vehdjk.com/Article/details/gbhajhgsm.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.m.share.bbcook.cn/Article/details/gbseumrun.sHtML

TS:   // 单行；/* 多行 */
来源：http://baike.yfazqb.com/Article/details/gfkauwmxl.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.share.fktsv.cn/Article/details/gtombjrzv.sHtML

Go:   // 单行；/* 多行 */
来源：http://read.share.yfazqb.com/Article/details/giifrgxoq.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://blog.bbcook.cn/Article/details/gvczfmoer.sHtML

C#:   // 单行；/* 多行 */
来源：http://wap.vehdjk.com/Article/details/giamftefv.sHtML

[A15] 空值判断与默认值
来源：http://3g.tarul.cn/Article/details/gbwonxzsl.sHtML

Py:   value = data or "默认值"
来源：http://blog.sjlbkw.cn/Article/details/gmqlsusyw.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://mobile.vehdjk.com/Article/details/gtukdkswn.sHtML

JS:   const value = data ?? "默认值";
来源：http://mobile.bbcook.cn/Article/details/gxuoehesm.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.m.share.epnwcf.com/Article/details/gorwqngaq.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://m.share.yfazqb.com/Article/details/gqyhtbevf.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://blog.bbcook.cn/Article/details/gozcdmycz.sHtML

Ruby: value = data || "默认值"
来源：http://mobile.yfazqb.com/Article/details/gpjoojtjb.sHtML

C#:   var value = data ?? "默认值";
来源：http://read.share.vehdjk.com/Article/details/guoyjxsge.sHtML

[A16] 真假值判断规则
来源：http://m.share.fktsv.cn/Article/details/gbxlilgmm.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://blog.bbcook.cn/Article/details/gzseoruxn.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.m.share.fktsv.cn/Article/details/ggmqwbkmp.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://wap.tarul.cn/Article/details/gwcouelvq.sHtML

TS:   if (!x) {}
来源：http://3g.yfazqb.com/Article/details/ggqvyobox.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://3g.bbcook.cn/Article/details/gbbaofahv.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.m.share.bbcook.cn/Article/details/gvqumrvnt.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://blog.epnwcf.com/Article/details/gtxauienk.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://baike.bbcook.cn/Article/details/gyxihvynf.sHtML

[A17] 位运算
来源：http://3g.bbcook.cn/Article/details/gaucysfqz.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.bbcook.cn/Article/details/gfpbusyqy.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://read.share.epnwcf.com/Article/details/ghmqbtoui.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.tarul.cn/Article/details/gimlonjez.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wap.fktsv.cn/Article/details/gdpslvrct.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.sjlbkw.cn/Article/details/gecngnwmh.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.blog.fktsv.cn/Article/details/gnnkbwtyg.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.sjlbkw.cn/Article/details/gzsskwikg.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.sjlbkw.cn/Article/details/gxnzervbj.sHtML

[A18] 字符与 ASCII 码互转
来源：http://blog.epnwcf.com/Article/details/gwfprigod.sHtML

Py:   ord("A"); chr(65)
来源：http://www.share.fktsv.cn/Article/details/ggkkgvzdp.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.blog.tarul.cn/Article/details/gowcvzjgo.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.vehdjk.com/Article/details/gkeckozae.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.tarul.cn/Article/details/gghdovpjw.sHtML

Java: (int) 'A'; (char) 65
来源：http://mobile.sjlbkw.cn/Article/details/gygvpdfrm.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://baike.epnwcf.com/Article/details/gtnmqcldq.sHtML

Ruby: "A".ord; 65.chr
来源：http://read.share.tarul.cn/Article/details/gwmggqcya.sHtML

C#:   (int)'A'; (char)65
来源：http://www.blog.sjlbkw.cn/Article/details/gnhxrmffu.sHtML

[A19] 交换两个变量
来源：http://read.share.fktsv.cn/Article/details/ghlrxbwvh.sHtML

Py:   a, b = b, a
来源：http://blog.vehdjk.com/Article/details/getkdqsnm.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.share.bbcook.cn/Article/details/gaywhogxy.sHtML

JS:   [a, b] = [b, a];
来源：http://wap.vehdjk.com/Article/details/gmrexopyy.sHtML

TS:   [a, b] = [b, a];
来源：http://www.share.fktsv.cn/Article/details/gjigffytz.sHtML

Java: int t = a; a = b; b = t;
来源：http://baike.tarul.cn/Article/details/gznguzjvr.sHtML

Go:   a, b = b, a
来源：http://m.share.epnwcf.com/Article/details/grxcmcmwz.sHtML

Ruby: a, b = b, a
来源：http://wap.sjlbkw.cn/Article/details/gwtjktjwp.sHtML

C#:   (a, b) = (b, a);
来源：http://3g.bbcook.cn/Article/details/gtthoiamd.sHtML

[A20] 读取标准输入
来源：http://baike.bbcook.cn/Article/details/gkdfbmklm.sHtML

Py:   name = input("请输入：")
来源：http://3g.tarul.cn/Article/details/gmtinnbrq.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://read.share.fktsv.cn/Article/details/gtngyunjj.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://3g.epnwcf.com/Article/details/gwzdcodrk.sHtML

TS:   // Node.js：readline 模块
来源：http://www.blog.epnwcf.com/Article/details/gejvmogbu.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.share.sjlbkw.cn/Article/details/gvlcyyure.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.share.tarul.cn/Article/details/gxngkdutf.sHtML

Ruby: gets.chomp
来源：http://m.share.fktsv.cn/Article/details/gufbblaqq.sHtML

C#:   Console.ReadLine();
来源：http://www.m.share.yfazqb.com/Article/details/gbeluzxrs.sHtML

[A21] 保留指定小数位输出
来源：http://www.m.share.fktsv.cn/Article/details/glsvjrhlk.sHtML

Py:   f"{3.14159:.2f}"
来源：http://baike.bbcook.cn/Article/details/gljmktlcp.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://3g.epnwcf.com/Article/details/gncbofzzn.sHtML

JS:   (3.14159).toFixed(2)
来源：http://m.share.bbcook.cn/Article/details/glrcayytt.sHtML

TS:   (3.14159).toFixed(2)
来源：http://wap.epnwcf.com/Article/details/gqdiizque.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.m.share.bbcook.cn/Article/details/gwfnbyvsb.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://mobile.sjlbkw.cn/Article/details/gtxcryhvf.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://m.share.fktsv.cn/Article/details/gwvqriuql.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.blog.vehdjk.com/Article/details/gmngzayuc.sHtML

[A22] 获取字符串长度
来源：http://baike.yfazqb.com/Article/details/gugbiquke.sHtML

Py:   len(s)
来源：http://www.blog.fktsv.cn/Article/details/gcnaklcux.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://3g.epnwcf.com/Article/details/gyeumnfxi.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://baike.bbcook.cn/Article/details/gtyxkhjsx.sHtML

TS:   s.length
来源：http://3g.tarul.cn/Article/details/grmbnwjnd.sHtML

Java: s.length()
来源：http://3g.fktsv.cn/Article/details/gsrtraldy.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.blog.sjlbkw.cn/Article/details/ghmpnkfng.sHtML

Ruby: s.length
来源：http://read.share.fktsv.cn/Article/details/gfzudeqne.sHtML

C#:   s.Length
来源：http://3g.bbcook.cn/Article/details/gyscizfao.sHtML

[A23] 大小写转换
来源：http://www.share.yfazqb.com/Article/details/gihoatuuq.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://3g.yfazqb.com/Article/details/gzdcbycyx.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mobile.bbcook.cn/Article/details/gyvcuprey.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.epnwcf.com/Article/details/gptvghkxa.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.tarul.cn/Article/details/ghikzczge.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://read.share.fktsv.cn/Article/details/geyyykphy.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://baike.tarul.cn/Article/details/gcrhswvcv.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://blog.yfazqb.com/Article/details/geglubucz.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.share.bbcook.cn/Article/details/gqtteogjs.sHtML

[A24] 去除首尾空白
来源：http://blog.tarul.cn/Article/details/gbqpxosqo.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://read.share.tarul.cn/Article/details/gcikfvygo.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.blog.tarul.cn/Article/details/gykhoyvlr.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.tarul.cn/Article/details/glcstrgpl.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.tarul.cn/Article/details/gikdevqko.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://3g.bbcook.cn/Article/details/gnledarbq.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.share.tarul.cn/Article/details/gnyiaworx.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.blog.epnwcf.com/Article/details/gfvfnhzbl.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wap.bbcook.cn/Article/details/gqcitspax.sHtML

[A25] 字符串比较
来源：http://m.share.sjlbkw.cn/Article/details/gvhjsfqio.sHtML

Py:   s1 == s2; s1 != s2
来源：http://blog.epnwcf.com/Article/details/gjxyrgfkm.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wap.sjlbkw.cn/Article/details/ginvmixfo.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.tarul.cn/Article/details/gxebjestr.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.yfazqb.com/Article/details/gorrbvtsk.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mobile.bbcook.cn/Article/details/grjfszzpc.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.m.share.bbcook.cn/Article/details/ggjjsphmu.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://blog.fktsv.cn/Article/details/gdmdrmnqi.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.blog.tarul.cn/Article/details/gxggshhdl.sHtML

[A26] 类型转换总览
来源：http://m.share.bbcook.cn/Article/details/grlzrdvvx.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.blog.tarul.cn/Article/details/gyybyurmx.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://blog.yfazqb.com/Article/details/geanrvuhf.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://baike.fktsv.cn/Article/details/gttoxqjcw.sHtML

TS:   Number() String() Boolean() x as number
来源：http://wap.sjlbkw.cn/Article/details/gnawjhpir.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.m.share.bbcook.cn/Article/details/gwrnhwwls.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://baike.tarul.cn/Article/details/ghaigygms.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://3g.epnwcf.com/Article/details/gwiwscpsa.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mobile.vehdjk.com/Article/details/gfgvwdvay.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gzofzjamh.sHtML

B. 流程控制
来源：http://baike.sjlbkw.cn/Article/details/glioniouq.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gbuyogfgp.sHtML

[B01] 条件判断 if / else
来源：http://baike.bbcook.cn/Article/details/gflgypqid.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://m.share.fktsv.cn/Article/details/gvticyirs.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mobile.sjlbkw.cn/Article/details/gaznhegpq.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.bbcook.cn/Article/details/gfdlggcbt.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.yfazqb.com/Article/details/gnkhjkmgl.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.share.yfazqb.com/Article/details/gyxcsqsaj.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.share.yfazqb.com/Article/details/gqpgfhwun.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.blog.sjlbkw.cn/Article/details/gucixbqvh.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.blog.sjlbkw.cn/Article/details/gejkzgxvb.sHtML

[B02] 多分支 else if / elif
来源：http://blog.vehdjk.com/Article/details/gcaxjfplc.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.share.bbcook.cn/Article/details/grwhrplgd.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.blog.bbcook.cn/Article/details/ggynljsqc.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.yfazqb.com/Article/details/gcptmkbtr.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.fktsv.cn/Article/details/gthxbpvrj.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.tarul.cn/Article/details/gknqphdsz.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.share.epnwcf.com/Article/details/gitgiarsi.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mobile.fktsv.cn/Article/details/gabtrqqhg.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.yfazqb.com/Article/details/gsduybtko.sHtML

[B03] switch / match / case
来源：http://blog.bbcook.cn/Article/details/ghxolemck.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://read.share.fktsv.cn/Article/details/gnnetqqqu.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wap.epnwcf.com/Article/details/gfhycbtll.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.bbcook.cn/Article/details/glxcqviiv.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.vehdjk.com/Article/details/gtkgatdhz.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.m.share.yfazqb.com/Article/details/gecunkdgm.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://blog.sjlbkw.cn/Article/details/gqujfgusm.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://baike.bbcook.cn/Article/details/guegtaltu.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://baike.bbcook.cn/Article/details/gysexnbkx.sHtML

[B04] for 计数循环
来源：http://www.m.share.vehdjk.com/Article/details/gjuafqyeu.sHtML

Py:   for i in range(10): print(i)
来源：http://baike.yfazqb.com/Article/details/grapamofw.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://m.share.fktsv.cn/Article/details/gcfkigspi.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.vehdjk.com/Article/details/gibyqraof.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.epnwcf.com/Article/details/gcrmvwqcp.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.tarul.cn/Article/details/gvqznhehg.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mobile.sjlbkw.cn/Article/details/gbpgeevxs.sHtML

Ruby: 10.times { |i| puts i }
来源：http://mobile.fktsv.cn/Article/details/ggadlvlzs.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.blog.tarul.cn/Article/details/gtzivzwvi.sHtML

[B05] 遍历数组 / 列表
来源：http://www.m.share.vehdjk.com/Article/details/girebfpit.sHtML

Py:   for item in arr: print(item)
来源：http://blog.bbcook.cn/Article/details/gnjuyawhh.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wap.yfazqb.com/Article/details/gvyltdbqu.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://m.share.sjlbkw.cn/Article/details/gdcacosdy.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://m.share.yfazqb.com/Article/details/gtzqiufjb.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.tarul.cn/Article/details/gmttampqo.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.blog.bbcook.cn/Article/details/ggdoybpmt.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.fktsv.cn/Article/details/ggjsokpup.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://m.share.tarul.cn/Article/details/gpymdwgqb.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.tarul.cn/Article/details/gxjcxfmaz.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.vehdjk.com/Article/details/gvcdrqgoc.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.yfazqb.com/Article/details/galcicrmr.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.fktsv.cn/Article/details/gbvwldkdi.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.fktsv.cn/Article/details/gyvxfknyb.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mobile.bbcook.cn/Article/details/gwlevazwf.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.epnwcf.com/Article/details/gzufbmfgp.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wap.sjlbkw.cn/Article/details/gdbnszqmj.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://read.share.vehdjk.com/Article/details/gspwmzlta.sHtML

[B07] while 循环
来源：http://mobile.sjlbkw.cn/Article/details/gatvxaxiu.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.epnwcf.com/Article/details/gypivnbac.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.bbcook.cn/Article/details/gvoyuqevw.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.bbcook.cn/Article/details/gcuvzqbvx.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.bbcook.cn/Article/details/gvjacuacs.sHtML

Java: while (i < 10) { i++; }
来源：http://baike.vehdjk.com/Article/details/ghxavyalt.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.bbcook.cn/Article/details/gwkiucctn.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.vehdjk.com/Article/details/gxludffgy.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.epnwcf.com/Article/details/gnfdqtirw.sHtML

[B08] do-while（至少执行一次）
来源：http://www.share.sjlbkw.cn/Article/details/groplhpnv.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://blog.fktsv.cn/Article/details/gzadwsfsd.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.fktsv.cn/Article/details/gbwmukgrt.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.vehdjk.com/Article/details/gjeewdynd.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.vehdjk.com/Article/details/geyiluvhs.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.epnwcf.com/Article/details/gdzkdphby.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.yfazqb.com/Article/details/guehqknac.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://read.share.tarul.cn/Article/details/gvuavjyty.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.bbcook.cn/Article/details/gigbgzchs.sHtML

[B09] break 与 continue
来源：http://www.share.fktsv.cn/Article/details/gihbbobco.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.bbcook.cn/Article/details/gqncbsxuj.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.tarul.cn/Article/details/gjnxhmdul.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.bbcook.cn/Article/details/gkzdtqkdg.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.tarul.cn/Article/details/gxxhzjfqk.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.epnwcf.com/Article/details/gmwpmpiij.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.vehdjk.com/Article/details/gvivqqlxr.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://read.share.fktsv.cn/Article/details/ghjmggyjz.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.sjlbkw.cn/Article/details/gwnhejexd.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.bbcook.cn/Article/details/gisvjattc.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.sjlbkw.cn/Article/details/gbfggvrei.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.sjlbkw.cn/Article/details/gjwtkrctm.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.yfazqb.com/Article/details/gqoabsowl.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.epnwcf.com/Article/details/gpaqdmzwp.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.yfazqb.com/Article/details/gqqfablpr.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://baike.vehdjk.com/Article/details/grzsckyvt.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.epnwcf.com/Article/details/gwndqttbg.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.bbcook.cn/Article/details/gyxftileh.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.blog.sjlbkw.cn/Article/details/gbugaadvj.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.yfazqb.com/Article/details/gvjwdaccd.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.fktsv.cn/Article/details/gphtjjbje.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.yfazqb.com/Article/details/gdcixaaru.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.yfazqb.com/Article/details/gdquenljn.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.sjlbkw.cn/Article/details/guszzksrg.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.fktsv.cn/Article/details/guuwkdtlj.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.fktsv.cn/Article/details/glofbdjer.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.yfazqb.com/Article/details/gjspmqahu.sHtML

[B12] 跳出多层循环
来源：http://mobile.epnwcf.com/Article/details/gqnnzqbge.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.tarul.cn/Article/details/guxfbuufj.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.bbcook.cn/Article/details/gebrimgrm.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.sjlbkw.cn/Article/details/guwuxficr.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fktsv.cn/Article/details/glhoqwrgn.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.tarul.cn/Article/details/gmkvqyzfe.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.fktsv.cn/Article/details/gzstfatji.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.bbcook.cn/Article/details/gtzfedhfd.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.tarul.cn/Article/details/gxzyciqve.sHtML

[B13] 判断是否为数字
来源：http://mobile.vehdjk.com/Article/details/ghejtelxi.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.tarul.cn/Article/details/grthaaabv.sHtML

PHP:  is_numeric($x)
来源：http://www.share.yfazqb.com/Article/details/gnktnymxx.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.yfazqb.com/Article/details/grariqpyk.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.sjlbkw.cn/Article/details/gxynddhxi.sHtML

Java: x instanceof Number
来源：http://baike.bbcook.cn/Article/details/gkdvipdze.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.sjlbkw.cn/Article/details/girhdscge.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.yfazqb.com/Article/details/gydpdjhov.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.bbcook.cn/Article/details/gxuikiatd.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.fktsv.cn/Article/details/gcjxkisuy.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.vehdjk.com/Article/details/gwwhynhes.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.fktsv.cn/Article/details/gtkjsvkop.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.epnwcf.com/Article/details/gfnplfull.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.fktsv.cn/Article/details/ggnqclvoy.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.vehdjk.com/Article/details/gfhuzpydd.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.fktsv.cn/Article/details/ghuobzspl.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.epnwcf.com/Article/details/gvofsfrwz.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.fktsv.cn/Article/details/gyenmtvsj.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.vehdjk.com/Article/details/gbhbygyhj.sHtML

Py:   a and b or not c
来源：http://mobile.epnwcf.com/Article/details/glcdteidq.sHtML

PHP:  $a && $b || !$c
来源：http://wap.yfazqb.com/Article/details/gifkjdghw.sHtML

JS:   a && b || !c
来源：http://wap.vehdjk.com/Article/details/gfusfrxrs.sHtML

TS:   a && b || !c
来源：http://www.m.share.epnwcf.com/Article/details/gzvspjnhe.sHtML

Java: a && b || !c
来源：http://read.share.epnwcf.com/Article/details/graletmcw.sHtML

Go:   a && b || !c
来源：http://3g.tarul.cn/Article/details/gcjijzcpe.sHtML

Ruby: a && b || !c
来源：http://baike.tarul.cn/Article/details/gwmofllcs.sHtML

C#:   a && b || !c
来源：http://wap.vehdjk.com/Article/details/godqafkrd.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.yfazqb.com/Article/details/gljgbdgew.sHtML

Py:   if not data: return
来源：http://blog.sjlbkw.cn/Article/details/gyanmfrmh.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.bbcook.cn/Article/details/gnfrwqtia.sHtML

JS:   if (!data) return;
来源：http://www.m.share.yfazqb.com/Article/details/gquehtnui.sHtML

TS:   if (!data) return;
来源：http://blog.bbcook.cn/Article/details/graicnaze.sHtML

Java: if (data == null) return;
来源：http://www.blog.fktsv.cn/Article/details/gmwwmbdzi.sHtML

Go:   if data == nil { return }
来源：http://3g.vehdjk.com/Article/details/gnmuhoprj.sHtML

Ruby: return if data.nil?
来源：http://wap.sjlbkw.cn/Article/details/guhifumeq.sHtML

C#:   if (data == null) return;
来源：http://3g.sjlbkw.cn/Article/details/gyyxkcvac.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gyqqkagjt.sHtML

C. 函数与作用域
来源：http://3g.tarul.cn/Article/details/gducvcyca.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gxqavbkhx.sHtML

[C01] 定义函数
来源：http://www.share.tarul.cn/Article/details/gswizzxzj.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.yfazqb.com/Article/details/gtcymtsdp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.vehdjk.com/Article/details/gekxidczg.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.sjlbkw.cn/Article/details/gtoluhgnr.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.vehdjk.com/Article/details/gkovunjjd.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.fktsv.cn/Article/details/ghfzjhdfq.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.yfazqb.com/Article/details/glnnyvjyh.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.sjlbkw.cn/Article/details/geldmjyeu.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.bbcook.cn/Article/details/gwpxdvmen.sHtML

[C02] 默认参数
来源：http://www.m.share.yfazqb.com/Article/details/gjonlpblv.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.epnwcf.com/Article/details/gmomxhfsv.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.sjlbkw.cn/Article/details/gathqdomd.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.tarul.cn/Article/details/ghybspdqh.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.tarul.cn/Article/details/gmmgwatvt.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.vehdjk.com/Article/details/glbmeqjrt.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.epnwcf.com/Article/details/gptyhpqxl.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.vehdjk.com/Article/details/gbdpdjahc.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.bbcook.cn/Article/details/guzbjqoyo.sHtML

[C03] 可变参数
来源：http://www.blog.bbcook.cn/Article/details/gmxolsqyg.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.bbcook.cn/Article/details/gwkerumpw.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.epnwcf.com/Article/details/grlxeonbe.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.fktsv.cn/Article/details/gtkscxwdi.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.bbcook.cn/Article/details/gdhdckoof.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.yfazqb.com/Article/details/gmksovzzj.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.sjlbkw.cn/Article/details/gjqivmhqn.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.sjlbkw.cn/Article/details/gbsyxahgt.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.vehdjk.com/Article/details/gpxvtwxxh.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.vehdjk.com/Article/details/gbstyziik.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.epnwcf.com/Article/details/gvjnedbyf.sHtML


<!-- 参考信息 -->