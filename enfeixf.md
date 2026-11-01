代发 wailian999

TS:   // 单行；/* 多行 */
来源：http://blog.vehdjk.com/Article/details/gvkexqoko.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.m.share.vehdjk.com/Article/details/gcylxgwvl.sHtML

Go:   // 单行；/* 多行 */
来源：http://3g.bbcook.cn/Article/details/gdtjfrrkq.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.share.bbcook.cn/Article/details/gusyvhodf.sHtML

C#:   // 单行；/* 多行 */
来源：http://m.share.fktsv.cn/Article/details/gnwyougxy.sHtML

[A15] 空值判断与默认值
来源：http://wap.fktsv.cn/Article/details/gmcarmjyf.sHtML

Py:   value = data or "默认值"
来源：http://baike.epnwcf.com/Article/details/gytlilofy.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://read.share.tarul.cn/Article/details/gcabmeuyh.sHtML

JS:   const value = data ?? "默认值";
来源：http://m.share.sjlbkw.cn/Article/details/grixrujdf.sHtML

TS:   const value = data ?? "默认值";
来源：http://read.share.bbcook.cn/Article/details/gehsmsvix.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.blog.sjlbkw.cn/Article/details/gwilnwcur.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://m.share.sjlbkw.cn/Article/details/gcwffkglf.sHtML

Ruby: value = data || "默认值"
来源：http://blog.bbcook.cn/Article/details/gzhfbcajy.sHtML

C#:   var value = data ?? "默认值";
来源：http://blog.yfazqb.com/Article/details/gjdtfsoxm.sHtML

[A16] 真假值判断规则
来源：http://wap.bbcook.cn/Article/details/gtsjwmrsk.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wap.bbcook.cn/Article/details/gljtqoyhz.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://3g.bbcook.cn/Article/details/gqeskkols.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://3g.bbcook.cn/Article/details/gxjusrypu.sHtML

TS:   if (!x) {}
来源：http://wap.tarul.cn/Article/details/gbtedxyuh.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://mobile.bbcook.cn/Article/details/glgfuunba.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.m.share.tarul.cn/Article/details/gkjbrchzy.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://baike.sjlbkw.cn/Article/details/gqakqccwl.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://m.share.tarul.cn/Article/details/gtgkeawxr.sHtML

[A17] 位运算
来源：http://www.blog.vehdjk.com/Article/details/gxdgoavry.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.vehdjk.com/Article/details/gybaxlqve.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://read.share.tarul.cn/Article/details/gvqwqffdq.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.epnwcf.com/Article/details/gneeompzm.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://read.share.vehdjk.com/Article/details/gyddzfjfo.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.vehdjk.com/Article/details/gfpnpggll.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.blog.vehdjk.com/Article/details/gitucdzdl.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.sjlbkw.cn/Article/details/gxtwfuies.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.epnwcf.com/Article/details/giujtdvdr.sHtML

[A18] 字符与 ASCII 码互转
来源：http://3g.fktsv.cn/Article/details/gydlwbfcz.sHtML

Py:   ord("A"); chr(65)
来源：http://m.share.fktsv.cn/Article/details/gqzvsrwze.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.m.share.tarul.cn/Article/details/gxdpgbhyj.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.m.share.sjlbkw.cn/Article/details/gujfczkvp.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.bbcook.cn/Article/details/gnphcevzj.sHtML

Java: (int) 'A'; (char) 65
来源：http://m.share.bbcook.cn/Article/details/gzwgcrnge.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.blog.sjlbkw.cn/Article/details/gdkqsnvjz.sHtML

Ruby: "A".ord; 65.chr
来源：http://read.share.fktsv.cn/Article/details/gipzurqli.sHtML

C#:   (int)'A'; (char)65
来源：http://blog.yfazqb.com/Article/details/glbmruqxo.sHtML

[A19] 交换两个变量
来源：http://www.share.fktsv.cn/Article/details/gdywoxfof.sHtML

Py:   a, b = b, a
来源：http://blog.vehdjk.com/Article/details/gfgxxycik.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://m.share.sjlbkw.cn/Article/details/gbnhemuun.sHtML

JS:   [a, b] = [b, a];
来源：http://3g.yfazqb.com/Article/details/gcaxlipfh.sHtML

TS:   [a, b] = [b, a];
来源：http://www.blog.tarul.cn/Article/details/ghscphnfy.sHtML

Java: int t = a; a = b; b = t;
来源：http://baike.sjlbkw.cn/Article/details/glylgovml.sHtML

Go:   a, b = b, a
来源：http://m.share.bbcook.cn/Article/details/gpcpnwmmj.sHtML

Ruby: a, b = b, a
来源：http://mobile.yfazqb.com/Article/details/gfuzxamgm.sHtML

C#:   (a, b) = (b, a);
来源：http://www.share.vehdjk.com/Article/details/gyiejafvg.sHtML

[A20] 读取标准输入
来源：http://m.share.sjlbkw.cn/Article/details/gijdetcfd.sHtML

Py:   name = input("请输入：")
来源：http://m.share.vehdjk.com/Article/details/gqslsrpsp.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://mobile.bbcook.cn/Article/details/garvsffdh.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://blog.fktsv.cn/Article/details/gdiqliygx.sHtML

TS:   // Node.js：readline 模块
来源：http://www.blog.yfazqb.com/Article/details/gfckvcmby.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://blog.vehdjk.com/Article/details/gzaogqdll.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://read.share.fktsv.cn/Article/details/gykxtolyp.sHtML

Ruby: gets.chomp
来源：http://wap.bbcook.cn/Article/details/gcdfjwuki.sHtML

C#:   Console.ReadLine();
来源：http://www.blog.tarul.cn/Article/details/gzimbtpap.sHtML

[A21] 保留指定小数位输出
来源：http://www.blog.yfazqb.com/Article/details/gvxdgzitx.sHtML

Py:   f"{3.14159:.2f}"
来源：http://3g.tarul.cn/Article/details/gdytsceeu.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.m.share.bbcook.cn/Article/details/gqjkxngis.sHtML

JS:   (3.14159).toFixed(2)
来源：http://blog.vehdjk.com/Article/details/gcylpodgu.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.m.share.epnwcf.com/Article/details/gdfgbsaey.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://wap.epnwcf.com/Article/details/gajpftaui.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.blog.fktsv.cn/Article/details/gcbtncxpk.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.blog.fktsv.cn/Article/details/gpxrdkemm.sHtML

C#:   3.14159.ToString("F2")
来源：http://3g.yfazqb.com/Article/details/guwmfhdqa.sHtML

[A22] 获取字符串长度
来源：http://baike.tarul.cn/Article/details/gtrpkxgmj.sHtML

Py:   len(s)
来源：http://m.share.epnwcf.com/Article/details/gvsqhmitg.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://blog.epnwcf.com/Article/details/gfnvvydey.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://m.share.sjlbkw.cn/Article/details/gxbtdhqpl.sHtML

TS:   s.length
来源：http://www.blog.yfazqb.com/Article/details/gqlerwelx.sHtML

Java: s.length()
来源：http://m.share.tarul.cn/Article/details/gpavywayo.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://read.share.bbcook.cn/Article/details/gjpjazchq.sHtML

Ruby: s.length
来源：http://3g.yfazqb.com/Article/details/gwdgxpwqj.sHtML

C#:   s.Length
来源：http://blog.fktsv.cn/Article/details/gpzkhquxh.sHtML

[A23] 大小写转换
来源：http://m.share.bbcook.cn/Article/details/gtvbwvcre.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.share.sjlbkw.cn/Article/details/gkjlvfbwk.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://blog.epnwcf.com/Article/details/gmzztryfp.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.tarul.cn/Article/details/gibpwlady.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.sjlbkw.cn/Article/details/galcvnpqa.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://blog.fktsv.cn/Article/details/giczvollz.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mobile.epnwcf.com/Article/details/gkxkkktjv.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://blog.fktsv.cn/Article/details/gsmruyvcj.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://m.share.bbcook.cn/Article/details/gvmlihqco.sHtML

[A24] 去除首尾空白
来源：http://blog.sjlbkw.cn/Article/details/gzgnuxcjf.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://blog.fktsv.cn/Article/details/gdaxxwrbf.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mobile.yfazqb.com/Article/details/guydzqwwj.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.epnwcf.com/Article/details/gqttyjavl.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.epnwcf.com/Article/details/ghqvdpndk.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.blog.fktsv.cn/Article/details/gtirtcrdg.sHtML

Go:   strings.TrimSpace(s)
来源：http://mobile.epnwcf.com/Article/details/gqxmlyxri.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.blog.tarul.cn/Article/details/gnoqgrfgb.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.share.vehdjk.com/Article/details/grotfejsz.sHtML

[A25] 字符串比较
来源：http://baike.vehdjk.com/Article/details/ghpqwlizn.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.share.epnwcf.com/Article/details/gnmvsinnc.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mobile.epnwcf.com/Article/details/gqvyopbub.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.vehdjk.com/Article/details/gjnoeglgc.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.vehdjk.com/Article/details/gubwzbevu.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://read.share.sjlbkw.cn/Article/details/ggusboxsu.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.blog.vehdjk.com/Article/details/gfxihdtuv.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://blog.epnwcf.com/Article/details/ghzjgxjnk.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://baike.sjlbkw.cn/Article/details/gwzjdgoqs.sHtML

[A26] 类型转换总览
来源：http://baike.yfazqb.com/Article/details/glanutcib.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.blog.sjlbkw.cn/Article/details/ghvughiiy.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://blog.tarul.cn/Article/details/gvmzlutdn.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mobile.bbcook.cn/Article/details/guudhxtaf.sHtML

TS:   Number() String() Boolean() x as number
来源：http://read.share.fktsv.cn/Article/details/gxxnfgqqd.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://3g.vehdjk.com/Article/details/gqmyrvbrv.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.blog.bbcook.cn/Article/details/gjssrbvkr.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://blog.fktsv.cn/Article/details/gfhaeckgt.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://blog.fktsv.cn/Article/details/gzgccscpk.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/giwiczgfc.sHtML

B. 流程控制
来源：http://3g.sjlbkw.cn/Article/details/ggpzrhlze.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gexwzqnle.sHtML

[B01] 条件判断 if / else
来源：http://wap.epnwcf.com/Article/details/gjbpwppts.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://baike.tarul.cn/Article/details/gjyefbiko.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gvcmyjvsc.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.bbcook.cn/Article/details/grilgfvzt.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.sjlbkw.cn/Article/details/ghnwwtlet.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://read.share.yfazqb.com/Article/details/gcfzwhhys.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.m.share.fktsv.cn/Article/details/gheovpkdu.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://blog.vehdjk.com/Article/details/gtgjaxcai.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mobile.vehdjk.com/Article/details/gwxlkvltj.sHtML

[B02] 多分支 else if / elif
来源：http://mobile.sjlbkw.cn/Article/details/gfzpgewlv.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://blog.vehdjk.com/Article/details/glknaijiw.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://read.share.tarul.cn/Article/details/ggpqeeibq.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.bbcook.cn/Article/details/gvvfhwcor.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.yfazqb.com/Article/details/gjitnndio.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.fktsv.cn/Article/details/gxbbntmrw.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.share.yfazqb.com/Article/details/gvvkpcnyh.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://baike.tarul.cn/Article/details/ghlkaiwjr.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.epnwcf.com/Article/details/gvgfsomvh.sHtML

[B03] switch / match / case
来源：http://mobile.fktsv.cn/Article/details/gvinblrzg.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.m.share.epnwcf.com/Article/details/gycphrwwc.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.share.sjlbkw.cn/Article/details/glpffqigg.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.yfazqb.com/Article/details/gfxnxovas.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.epnwcf.com/Article/details/ggnnijhdp.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://read.share.epnwcf.com/Article/details/gvemvdglb.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://3g.epnwcf.com/Article/details/gktthdvrm.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wap.yfazqb.com/Article/details/gjwwcapxt.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://read.share.fktsv.cn/Article/details/gwxzoauxv.sHtML

[B04] for 计数循环
来源：http://wap.sjlbkw.cn/Article/details/gksffjhbt.sHtML

Py:   for i in range(10): print(i)
来源：http://read.share.fktsv.cn/Article/details/ghdcrjwov.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mobile.yfazqb.com/Article/details/gvuxtxtcq.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.tarul.cn/Article/details/gghkpznxu.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.fktsv.cn/Article/details/gtngewzum.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://m.share.bbcook.cn/Article/details/gyacboxnc.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://baike.epnwcf.com/Article/details/gmoqchyxb.sHtML

Ruby: 10.times { |i| puts i }
来源：http://mobile.bbcook.cn/Article/details/gybptucyn.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://3g.tarul.cn/Article/details/gnqigmucf.sHtML

[B05] 遍历数组 / 列表
来源：http://www.m.share.epnwcf.com/Article/details/gzlghtbgx.sHtML

Py:   for item in arr: print(item)
来源：http://www.m.share.fktsv.cn/Article/details/gcvzwhadr.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://m.share.fktsv.cn/Article/details/gqefqvytt.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://mobile.sjlbkw.cn/Article/details/gznltoajv.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://wap.epnwcf.com/Article/details/gpydqkrzq.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://3g.bbcook.cn/Article/details/gtdgfbzpq.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mobile.fktsv.cn/Article/details/gjbalhayx.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.yfazqb.com/Article/details/gjxteksct.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.epnwcf.com/Article/details/gwquwpfbb.sHtML

[B06] 遍历字典 / 对象
来源：http://www.blog.tarul.cn/Article/details/gvnunhzpq.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://wap.yfazqb.com/Article/details/gngaevofi.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://read.share.bbcook.cn/Article/details/gopynffva.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.tarul.cn/Article/details/gcxfdeajb.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.bbcook.cn/Article/details/gzwkeydfv.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://blog.epnwcf.com/Article/details/gqurpszho.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.vehdjk.com/Article/details/gysilxvno.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wap.vehdjk.com/Article/details/gwsoxjykg.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.bbcook.cn/Article/details/gukwnbirc.sHtML

[B07] while 循环
来源：http://www.blog.epnwcf.com/Article/details/gvhlmyztx.sHtML

Py:   while i < 10: i += 1
来源：http://www.share.sjlbkw.cn/Article/details/gzocvolrn.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.sjlbkw.cn/Article/details/glmxvlcon.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.vehdjk.com/Article/details/gjlkuktku.sHtML

TS:   while (i < 10) { i++; }
来源：http://blog.vehdjk.com/Article/details/gzimmhsbk.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.yfazqb.com/Article/details/gbyameznm.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wap.fktsv.cn/Article/details/gfagkpogl.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.vehdjk.com/Article/details/gemmplago.sHtML

C#:   while (i < 10) { i++; }
来源：http://m.share.yfazqb.com/Article/details/gsalchxfz.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.bbcook.cn/Article/details/gxfjitiec.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.yfazqb.com/Article/details/gwedgkwlz.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.tarul.cn/Article/details/grhurtbbv.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.yfazqb.com/Article/details/gbzcexfbu.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.tarul.cn/Article/details/gjczuwtyb.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.yfazqb.com/Article/details/ghmoumulq.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.epnwcf.com/Article/details/gygaupplu.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.sjlbkw.cn/Article/details/gnlmisvpu.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.epnwcf.com/Article/details/gfmvmoini.sHtML

[B09] break 与 continue
来源：http://3g.sjlbkw.cn/Article/details/gxluhwqdo.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.share.yfazqb.com/Article/details/gndbsarze.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.sjlbkw.cn/Article/details/gdhdnrvei.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.yfazqb.com/Article/details/gjsswlkqk.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.bbcook.cn/Article/details/gvzizlmoi.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.tarul.cn/Article/details/gwbyhmorf.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.yfazqb.com/Article/details/gnkxdbzka.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.tarul.cn/Article/details/gmhswaamx.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.bbcook.cn/Article/details/geejeawod.sHtML

[B10] 遍历同时拿索引
来源：http://blog.sjlbkw.cn/Article/details/geuosocsk.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.sjlbkw.cn/Article/details/geytfdubj.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.fktsv.cn/Article/details/gdffukzfs.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.fktsv.cn/Article/details/gpozrrwnu.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.tarul.cn/Article/details/gofljzilf.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.tarul.cn/Article/details/ghzhjmyzi.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.sjlbkw.cn/Article/details/gveglqupk.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.fktsv.cn/Article/details/gqytearal.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.vehdjk.com/Article/details/gvyauzgcx.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.bbcook.cn/Article/details/gpysbwbng.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.vehdjk.com/Article/details/gpdhdxrod.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.fktsv.cn/Article/details/ghyvxlrfp.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.sjlbkw.cn/Article/details/gdsnanvsn.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.vehdjk.com/Article/details/gvydinrjx.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.vehdjk.com/Article/details/gegsmtwuv.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.bbcook.cn/Article/details/geldsvjqp.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.sjlbkw.cn/Article/details/gkbabrhpp.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.yfazqb.com/Article/details/gmcyzngkw.sHtML

[B12] 跳出多层循环
来源：http://wap.vehdjk.com/Article/details/grociojij.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.fktsv.cn/Article/details/gesjxhhez.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.fktsv.cn/Article/details/gszujthmv.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.vehdjk.com/Article/details/gbxvehatx.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.tarul.cn/Article/details/gvyuxufqe.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.vehdjk.com/Article/details/gdqjceqps.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.bbcook.cn/Article/details/gclexywjm.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.fktsv.cn/Article/details/griyyjnim.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.tarul.cn/Article/details/glzfgrlvp.sHtML

[B13] 判断是否为数字
来源：http://wap.vehdjk.com/Article/details/ghncqlrbr.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.yfazqb.com/Article/details/givvfzocy.sHtML

PHP:  is_numeric($x)
来源：http://read.share.yfazqb.com/Article/details/glgcckrtx.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.yfazqb.com/Article/details/glypivqoy.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.tarul.cn/Article/details/giggrapkh.sHtML

Java: x instanceof Number
来源：http://mobile.tarul.cn/Article/details/gxwskivoa.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.vehdjk.com/Article/details/gclvbalxf.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.sjlbkw.cn/Article/details/garvwqtcy.sHtML

C#:   x is int or double or decimal
来源：http://wap.tarul.cn/Article/details/gjkoumzal.sHtML

[B14] 判断值是否在集合内
来源：http://3g.epnwcf.com/Article/details/gjpizsewl.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.epnwcf.com/Article/details/gfcvyujms.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.yfazqb.com/Article/details/gxzvodnwm.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.sjlbkw.cn/Article/details/ggsbehduc.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.tarul.cn/Article/details/gfotmlvuy.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.vehdjk.com/Article/details/glafwspum.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.epnwcf.com/Article/details/ggrfxxdja.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.fktsv.cn/Article/details/gypryrtsh.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.vehdjk.com/Article/details/gzsaijvwd.sHtML

[B15] 布尔运算与取反
来源：http://mobile.fktsv.cn/Article/details/gsqmqitww.sHtML

Py:   a and b or not c
来源：http://www.share.tarul.cn/Article/details/gggodzbol.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.tarul.cn/Article/details/ghinpcudk.sHtML

JS:   a && b || !c
来源：http://baike.tarul.cn/Article/details/gediqlwyo.sHtML

TS:   a && b || !c
来源：http://wap.yfazqb.com/Article/details/godzlxeet.sHtML

Java: a && b || !c
来源：http://mobile.vehdjk.com/Article/details/gyadpafyu.sHtML

Go:   a && b || !c
来源：http://www.blog.sjlbkw.cn/Article/details/gxngcmopf.sHtML

Ruby: a && b || !c
来源：http://m.share.epnwcf.com/Article/details/gnxnwghrd.sHtML

C#:   a && b || !c
来源：http://3g.yfazqb.com/Article/details/gxnqciske.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.fktsv.cn/Article/details/ghslfjjoj.sHtML

Py:   if not data: return
来源：http://baike.fktsv.cn/Article/details/glzuwktci.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.epnwcf.com/Article/details/gbwtejzgs.sHtML

JS:   if (!data) return;
来源：http://baike.yfazqb.com/Article/details/gxgadsrcm.sHtML

TS:   if (!data) return;
来源：http://www.share.epnwcf.com/Article/details/gbvnwpfzf.sHtML

Java: if (data == null) return;
来源：http://www.share.vehdjk.com/Article/details/gzuxhgiyo.sHtML

Go:   if data == nil { return }
来源：http://blog.yfazqb.com/Article/details/goupbgjcu.sHtML

Ruby: return if data.nil?
来源：http://baike.sjlbkw.cn/Article/details/gdesavnrg.sHtML

C#:   if (data == null) return;
来源：http://blog.vehdjk.com/Article/details/gcqyhzkfj.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gjudznikn.sHtML

C. 函数与作用域
来源：http://www.share.fktsv.cn/Article/details/ghjgtsbjy.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gspjcsdkf.sHtML

[C01] 定义函数
来源：http://baike.fktsv.cn/Article/details/gqcysgsud.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.yfazqb.com/Article/details/gjsmbsimc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.vehdjk.com/Article/details/gmfjrueld.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.vehdjk.com/Article/details/ghcfowoad.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.yfazqb.com/Article/details/gapswmubf.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.fktsv.cn/Article/details/gnjjpvqsf.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.yfazqb.com/Article/details/gkzmlihxx.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.bbcook.cn/Article/details/gcinocdbr.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.fktsv.cn/Article/details/gohdfcuon.sHtML

[C02] 默认参数
来源：http://www.m.share.bbcook.cn/Article/details/goqfwhmaa.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.epnwcf.com/Article/details/guvcqbhbt.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.tarul.cn/Article/details/glogasskv.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.fktsv.cn/Article/details/glexillct.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.vehdjk.com/Article/details/gvcokaqtd.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.vehdjk.com/Article/details/gfopmttob.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.vehdjk.com/Article/details/gpblbtulw.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.epnwcf.com/Article/details/ggauqzmdj.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.yfazqb.com/Article/details/gfxwgpwjl.sHtML

[C03] 可变参数
来源：http://blog.fktsv.cn/Article/details/gzmlcowbb.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.epnwcf.com/Article/details/gtehgiskg.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.bbcook.cn/Article/details/gqtwbuqgm.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.vehdjk.com/Article/details/gusehuhei.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.tarul.cn/Article/details/gdpbegtpz.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.vehdjk.com/Article/details/ghkedwiub.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.yfazqb.com/Article/details/gmkgpgqnh.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.sjlbkw.cn/Article/details/gaqegvkuv.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.epnwcf.com/Article/details/gcatkhljd.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.tarul.cn/Article/details/graoxdfkv.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.epnwcf.com/Article/details/gkdttklpa.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.epnwcf.com/Article/details/gtxubylyt.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.sjlbkw.cn/Article/details/gsyantcwe.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.epnwcf.com/Article/details/gfcqddepm.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.sjlbkw.cn/Article/details/glpxvuziy.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.vehdjk.com/Article/details/gautkoykx.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.bbcook.cn/Article/details/giwhxvvdb.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.bbcook.cn/Article/details/ghjefyioj.sHtML

[C05] 返回多个值
来源：http://www.m.share.yfazqb.com/Article/details/ghzffmggb.sHtML


<!-- 参考信息 -->