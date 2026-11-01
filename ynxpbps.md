代发 wailian999

TS:   // 单行；/* 多行 */
来源：http://read.share.sjlbkw.cn/Article/details/gtwasiwni.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wap.tarul.cn/Article/details/gpbcfmecy.sHtML

Go:   // 单行；/* 多行 */
来源：http://m.share.epnwcf.com/Article/details/glbypxkew.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://mobile.vehdjk.com/Article/details/gqecllskq.sHtML

C#:   // 单行；/* 多行 */
来源：http://read.share.epnwcf.com/Article/details/gjaaadyxb.sHtML

[A15] 空值判断与默认值
来源：http://wap.vehdjk.com/Article/details/gkwapdwyv.sHtML

Py:   value = data or "默认值"
来源：http://www.blog.tarul.cn/Article/details/gpgzutjke.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://baike.bbcook.cn/Article/details/graaulekk.sHtML

JS:   const value = data ?? "默认值";
来源：http://3g.fktsv.cn/Article/details/gyiyaohpd.sHtML

TS:   const value = data ?? "默认值";
来源：http://baike.tarul.cn/Article/details/gjduyxyzj.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.m.share.fktsv.cn/Article/details/gzuaiuwrc.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.blog.tarul.cn/Article/details/gdwensrkm.sHtML

Ruby: value = data || "默认值"
来源：http://mobile.yfazqb.com/Article/details/gtubmmyuv.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.blog.tarul.cn/Article/details/gohjstxup.sHtML

[A16] 真假值判断规则
来源：http://read.share.yfazqb.com/Article/details/gicpgtner.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.m.share.tarul.cn/Article/details/gbqtrpbpz.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.m.share.tarul.cn/Article/details/gmlzkcwwx.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.share.bbcook.cn/Article/details/gtyxlmreb.sHtML

TS:   if (!x) {}
来源：http://www.m.share.fktsv.cn/Article/details/gnpgqfbmi.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://3g.tarul.cn/Article/details/gnzjijqgt.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.blog.bbcook.cn/Article/details/gulmkeogb.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.share.yfazqb.com/Article/details/goxvtkafo.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://baike.epnwcf.com/Article/details/gojqnwvsx.sHtML

[A17] 位运算
来源：http://wap.yfazqb.com/Article/details/gfnjehzeq.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.epnwcf.com/Article/details/gpqlhbmbo.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.m.share.bbcook.cn/Article/details/gfnzokrit.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.epnwcf.com/Article/details/gqilifubt.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://m.share.vehdjk.com/Article/details/grwjcudiw.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.tarul.cn/Article/details/gxenutclz.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://mobile.yfazqb.com/Article/details/gdrvdnywn.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.yfazqb.com/Article/details/glooxzjlf.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.vehdjk.com/Article/details/gggvhnyhm.sHtML

[A18] 字符与 ASCII 码互转
来源：http://3g.tarul.cn/Article/details/gkextktif.sHtML

Py:   ord("A"); chr(65)
来源：http://m.share.yfazqb.com/Article/details/gcbntdvgz.sHtML

PHP:  ord("A"); chr(65)
来源：http://baike.yfazqb.com/Article/details/gomdodihj.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.epnwcf.com/Article/details/gznmitxsh.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.sjlbkw.cn/Article/details/gcyuerbpa.sHtML

Java: (int) 'A'; (char) 65
来源：http://wap.yfazqb.com/Article/details/gvayebxeg.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://m.share.sjlbkw.cn/Article/details/gowqtmbuh.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.blog.bbcook.cn/Article/details/gtaxzzxdw.sHtML

C#:   (int)'A'; (char)65
来源：http://blog.fktsv.cn/Article/details/gkmuubbhx.sHtML

[A19] 交换两个变量
来源：http://www.blog.sjlbkw.cn/Article/details/gqnwrvnos.sHtML

Py:   a, b = b, a
来源：http://www.m.share.tarul.cn/Article/details/gtoundxgr.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.share.vehdjk.com/Article/details/gchxvsloz.sHtML

JS:   [a, b] = [b, a];
来源：http://www.share.epnwcf.com/Article/details/gtggnczol.sHtML

TS:   [a, b] = [b, a];
来源：http://www.share.bbcook.cn/Article/details/gpnreejid.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.blog.vehdjk.com/Article/details/grclosuxk.sHtML

Go:   a, b = b, a
来源：http://www.m.share.yfazqb.com/Article/details/gqalyivuc.sHtML

Ruby: a, b = b, a
来源：http://www.share.vehdjk.com/Article/details/gicuhodvw.sHtML

C#:   (a, b) = (b, a);
来源：http://wap.sjlbkw.cn/Article/details/gnjoaqifk.sHtML

[A20] 读取标准输入
来源：http://baike.yfazqb.com/Article/details/gsvodeddh.sHtML

Py:   name = input("请输入：")
来源：http://www.m.share.sjlbkw.cn/Article/details/goayqfwqd.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.blog.tarul.cn/Article/details/gtnaqolvd.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://3g.bbcook.cn/Article/details/gfcctkiyq.sHtML

TS:   // Node.js：readline 模块
来源：http://read.share.bbcook.cn/Article/details/gyqqfldsb.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://mobile.fktsv.cn/Article/details/gtibgoocq.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://read.share.vehdjk.com/Article/details/gpzkigkyy.sHtML

Ruby: gets.chomp
来源：http://www.m.share.vehdjk.com/Article/details/geeyhmfor.sHtML

C#:   Console.ReadLine();
来源：http://www.share.vehdjk.com/Article/details/gfuatkzbv.sHtML

[A21] 保留指定小数位输出
来源：http://m.share.fktsv.cn/Article/details/gavkvizoe.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.blog.vehdjk.com/Article/details/grzaajuij.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://3g.bbcook.cn/Article/details/ghvjgizgf.sHtML

JS:   (3.14159).toFixed(2)
来源：http://baike.tarul.cn/Article/details/gwpiibtha.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.m.share.yfazqb.com/Article/details/gaqhgzzry.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://blog.epnwcf.com/Article/details/gznuusxws.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.m.share.vehdjk.com/Article/details/gnyayrqhu.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.share.fktsv.cn/Article/details/gvuhlktyj.sHtML

C#:   3.14159.ToString("F2")
来源：http://baike.yfazqb.com/Article/details/gcsgzwyrs.sHtML

[A22] 获取字符串长度
来源：http://www.blog.sjlbkw.cn/Article/details/glhasdpaa.sHtML

Py:   len(s)
来源：http://baike.yfazqb.com/Article/details/gctjmozzj.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://read.share.vehdjk.com/Article/details/gtcqfkyle.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://3g.yfazqb.com/Article/details/gysvcvwqy.sHtML

TS:   s.length
来源：http://read.share.yfazqb.com/Article/details/gjkppenar.sHtML

Java: s.length()
来源：http://read.share.yfazqb.com/Article/details/gmqchouae.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtacaeztl.sHtML

Ruby: s.length
来源：http://mobile.bbcook.cn/Article/details/gjpdqylsq.sHtML

C#:   s.Length
来源：http://read.share.bbcook.cn/Article/details/grilwsqeg.sHtML

[A23] 大小写转换
来源：http://m.share.fktsv.cn/Article/details/gxnbhzynj.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://read.share.sjlbkw.cn/Article/details/gwbgmncix.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://read.share.yfazqb.com/Article/details/gqjzgryhd.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.vehdjk.com/Article/details/gzzeokkeo.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.fktsv.cn/Article/details/gpbtzgpnu.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://blog.vehdjk.com/Article/details/gqacxcaaq.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://m.share.yfazqb.com/Article/details/gbnxslqev.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mobile.vehdjk.com/Article/details/gbxsayuoa.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://m.share.epnwcf.com/Article/details/gwcdtyngm.sHtML

[A24] 去除首尾空白
来源：http://www.m.share.epnwcf.com/Article/details/gzeihukzt.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://m.share.bbcook.cn/Article/details/gricpoixh.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://3g.bbcook.cn/Article/details/gddblnzvo.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.sjlbkw.cn/Article/details/ggzxtklnh.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.sjlbkw.cn/Article/details/gxhwaolfl.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.blog.fktsv.cn/Article/details/grrfwcbpb.sHtML

Go:   strings.TrimSpace(s)
来源：http://wap.epnwcf.com/Article/details/gfrmdcctn.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://3g.tarul.cn/Article/details/ggizhutun.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://blog.sjlbkw.cn/Article/details/gzwhdrxyh.sHtML

[A25] 字符串比较
来源：http://3g.vehdjk.com/Article/details/gwrkpgzxs.sHtML

Py:   s1 == s2; s1 != s2
来源：http://read.share.vehdjk.com/Article/details/gpfrouxlx.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://baike.sjlbkw.cn/Article/details/gogtxpgzc.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.fktsv.cn/Article/details/gfbjmykux.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.bbcook.cn/Article/details/gfqyfwove.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.blog.yfazqb.com/Article/details/ghainsjjs.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://blog.sjlbkw.cn/Article/details/gnslbtlnj.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://blog.bbcook.cn/Article/details/grlqvyryh.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.m.share.epnwcf.com/Article/details/gcoumibmm.sHtML

[A26] 类型转换总览
来源：http://m.share.yfazqb.com/Article/details/gcruvcfvf.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.share.yfazqb.com/Article/details/gazvbofay.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.m.share.bbcook.cn/Article/details/gijxtbgoq.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mobile.yfazqb.com/Article/details/gkipoxkvn.sHtML

TS:   Number() String() Boolean() x as number
来源：http://blog.fktsv.cn/Article/details/gxftqgujo.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://m.share.yfazqb.com/Article/details/gegicvmyr.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.share.epnwcf.com/Article/details/gaxhbwwzl.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://read.share.sjlbkw.cn/Article/details/ggwgbjgdo.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://m.share.vehdjk.com/Article/details/gmolvtkip.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gyxqgkkxj.sHtML

B. 流程控制
来源：http://www.m.share.tarul.cn/Article/details/govsyriuf.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gpicbozhq.sHtML

[B01] 条件判断 if / else
来源：http://mobile.bbcook.cn/Article/details/gqcpcbujl.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://wap.sjlbkw.cn/Article/details/gbxzbohru.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://baike.sjlbkw.cn/Article/details/grtucwxmd.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.bbcook.cn/Article/details/gyuocbhmt.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.yfazqb.com/Article/details/gxuxlzfud.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://read.share.yfazqb.com/Article/details/gglafcuru.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://baike.epnwcf.com/Article/details/gtmbclwdy.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wap.sjlbkw.cn/Article/details/gasxbdmdy.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://blog.yfazqb.com/Article/details/gqgkalhcq.sHtML

[B02] 多分支 else if / elif
来源：http://baike.fktsv.cn/Article/details/gweewqnbv.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://baike.tarul.cn/Article/details/gprefbida.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://baike.sjlbkw.cn/Article/details/gebbjqqed.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.bbcook.cn/Article/details/gpaoobwbc.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.bbcook.cn/Article/details/gmkfoyqqz.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.fktsv.cn/Article/details/grcifcggv.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mobile.yfazqb.com/Article/details/gcfgbgwdh.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.blog.yfazqb.com/Article/details/gmyqcavbu.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.sjlbkw.cn/Article/details/grxcfpvss.sHtML

[B03] switch / match / case
来源：http://www.blog.epnwcf.com/Article/details/gqykkzoba.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.blog.fktsv.cn/Article/details/gftwrlblj.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mobile.fktsv.cn/Article/details/ggsdkvocs.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.vehdjk.com/Article/details/gwoqraxqr.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.fktsv.cn/Article/details/ggzrofqlf.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.vehdjk.com/Article/details/giuffagve.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://read.share.epnwcf.com/Article/details/gtiointal.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://blog.yfazqb.com/Article/details/gjfmoimrh.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.blog.sjlbkw.cn/Article/details/geiotqjbl.sHtML

[B04] for 计数循环
来源：http://m.share.fktsv.cn/Article/details/ggwdimrmc.sHtML

Py:   for i in range(10): print(i)
来源：http://3g.vehdjk.com/Article/details/gfoctqlrd.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://read.share.bbcook.cn/Article/details/gpiituyxg.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.fktsv.cn/Article/details/gknjxrukg.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.fktsv.cn/Article/details/gyscwakns.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://read.share.tarul.cn/Article/details/gbdqdkcec.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://3g.epnwcf.com/Article/details/gmdtpclxg.sHtML

Ruby: 10.times { |i| puts i }
来源：http://read.share.bbcook.cn/Article/details/gfucmpixw.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.share.tarul.cn/Article/details/gjvsnunxz.sHtML

[B05] 遍历数组 / 列表
来源：http://read.share.yfazqb.com/Article/details/gykelmwcg.sHtML

Py:   for item in arr: print(item)
来源：http://m.share.tarul.cn/Article/details/gmhxpemke.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mobile.vehdjk.com/Article/details/gljbcdqqn.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.yfazqb.com/Article/details/gyioulxav.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://mobile.sjlbkw.cn/Article/details/gxbxqoyqp.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gmiqqnjpl.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://3g.epnwcf.com/Article/details/gbpkigxqk.sHtML

Ruby: arr.each { |item| puts item }
来源：http://3g.sjlbkw.cn/Article/details/ggcmqfpwn.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://3g.fktsv.cn/Article/details/gsyfiodqt.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.fktsv.cn/Article/details/ghakdniye.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://m.share.yfazqb.com/Article/details/gbwmedvcb.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://baike.bbcook.cn/Article/details/gyyuchztu.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.fktsv.cn/Article/details/gnesrwjoy.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.yfazqb.com/Article/details/gzdtvewyo.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gjwlauzrt.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wap.tarul.cn/Article/details/gdsnjkzag.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.vehdjk.com/Article/details/gkoalfhve.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://read.share.fktsv.cn/Article/details/gyyweoqcq.sHtML

[B07] while 循环
来源：http://blog.bbcook.cn/Article/details/gztgmhvkz.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.fktsv.cn/Article/details/gtzotytqi.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://m.share.bbcook.cn/Article/details/gjpjuzcep.sHtML

JS:   while (i < 10) { i++; }
来源：http://blog.fktsv.cn/Article/details/gtwhcqlqi.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.vehdjk.com/Article/details/gsnkasvik.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.tarul.cn/Article/details/gajdptgyv.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.bbcook.cn/Article/details/gmriwnlrr.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.bbcook.cn/Article/details/gkvwrexus.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.fktsv.cn/Article/details/gjadorkcy.sHtML

[B08] do-while（至少执行一次）
来源：http://m.share.fktsv.cn/Article/details/guqimrqol.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.bbcook.cn/Article/details/glknngflb.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.vehdjk.com/Article/details/ggfndvzim.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.vehdjk.com/Article/details/gufenukxv.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.epnwcf.com/Article/details/gekntgbny.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.vehdjk.com/Article/details/gasvhddov.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.epnwcf.com/Article/details/gsgpxppqj.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.epnwcf.com/Article/details/gpynkyyom.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.fktsv.cn/Article/details/guomguvsg.sHtML

[B09] break 与 continue
来源：http://baike.yfazqb.com/Article/details/gjzwknoql.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.share.epnwcf.com/Article/details/ggohanezi.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.yfazqb.com/Article/details/gxkglnzkf.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gazxvoeul.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.yfazqb.com/Article/details/gxvdfrpff.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.yfazqb.com/Article/details/gpsuhbdob.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.yfazqb.com/Article/details/gpnpclybs.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://read.share.epnwcf.com/Article/details/gyezqihyj.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.yfazqb.com/Article/details/gdgdoxefw.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.yfazqb.com/Article/details/gxigwpzcx.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.epnwcf.com/Article/details/gpvrufnqe.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.epnwcf.com/Article/details/gmosmyffx.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.tarul.cn/Article/details/gasjovgha.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.vehdjk.com/Article/details/gdmhrpysp.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.bbcook.cn/Article/details/gusolconh.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.tarul.cn/Article/details/gbybjydcj.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mobile.sjlbkw.cn/Article/details/gxkslxasf.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.tarul.cn/Article/details/gbuozvopg.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.sjlbkw.cn/Article/details/gomysqdev.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.vehdjk.com/Article/details/gfmvegldk.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.fktsv.cn/Article/details/gugvvltsb.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.epnwcf.com/Article/details/gkwhjycdl.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.yfazqb.com/Article/details/guqbzpigq.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.fktsv.cn/Article/details/gemgygufw.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.tarul.cn/Article/details/glndnpjwf.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.sjlbkw.cn/Article/details/guyofwwde.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.yfazqb.com/Article/details/gzeqcxted.sHtML

[B12] 跳出多层循环
来源：http://wap.yfazqb.com/Article/details/gvcyqavqu.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.epnwcf.com/Article/details/gzzfdrnwl.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.vehdjk.com/Article/details/gsosukpnv.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.tarul.cn/Article/details/gdeukacsf.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.fktsv.cn/Article/details/gbznjehij.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.bbcook.cn/Article/details/gtmtqirnz.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.yfazqb.com/Article/details/ghdljilmc.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.sjlbkw.cn/Article/details/gauhoqyqy.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.sjlbkw.cn/Article/details/galmmqqno.sHtML

[B13] 判断是否为数字
来源：http://3g.epnwcf.com/Article/details/gfzkhntkn.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.fktsv.cn/Article/details/gcpnbyglm.sHtML

PHP:  is_numeric($x)
来源：http://3g.vehdjk.com/Article/details/gnycppszf.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.fktsv.cn/Article/details/gpjxuqznx.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.tarul.cn/Article/details/gqpxizinl.sHtML

Java: x instanceof Number
来源：http://m.share.vehdjk.com/Article/details/gdieiwmfq.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.fktsv.cn/Article/details/gtxfxznyw.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.bbcook.cn/Article/details/gmnwepnhk.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.bbcook.cn/Article/details/gedbdrfwx.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.vehdjk.com/Article/details/gdjdtorzq.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.epnwcf.com/Article/details/gybdcltew.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.tarul.cn/Article/details/ggcjukwdw.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.tarul.cn/Article/details/giwqbtokv.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.sjlbkw.cn/Article/details/gnhfapryr.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.vehdjk.com/Article/details/gdugcbiom.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.epnwcf.com/Article/details/gbqjfkmtn.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.vehdjk.com/Article/details/gjaaocscl.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.vehdjk.com/Article/details/gheixwjpk.sHtML

[B15] 布尔运算与取反
来源：http://read.share.sjlbkw.cn/Article/details/gkufimoek.sHtML

Py:   a and b or not c
来源：http://wap.epnwcf.com/Article/details/geatfxjnz.sHtML

PHP:  $a && $b || !$c
来源：http://baike.sjlbkw.cn/Article/details/gyuhjmfui.sHtML

JS:   a && b || !c
来源：http://mobile.bbcook.cn/Article/details/glifkvfxj.sHtML

TS:   a && b || !c
来源：http://blog.sjlbkw.cn/Article/details/gtvcukelh.sHtML

Java: a && b || !c
来源：http://mobile.sjlbkw.cn/Article/details/gwoodcdpt.sHtML

Go:   a && b || !c
来源：http://read.share.fktsv.cn/Article/details/gevjppqcs.sHtML

Ruby: a && b || !c
来源：http://www.blog.tarul.cn/Article/details/gpwoscagu.sHtML

C#:   a && b || !c
来源：http://blog.yfazqb.com/Article/details/ggnhkqzzx.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.bbcook.cn/Article/details/gyisnqkur.sHtML

Py:   if not data: return
来源：http://www.m.share.sjlbkw.cn/Article/details/gxfovpxog.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.vehdjk.com/Article/details/gbovfiwry.sHtML

JS:   if (!data) return;
来源：http://www.share.bbcook.cn/Article/details/gclakuuia.sHtML

TS:   if (!data) return;
来源：http://baike.yfazqb.com/Article/details/gbvmgczuu.sHtML

Java: if (data == null) return;
来源：http://baike.bbcook.cn/Article/details/gatnicaxs.sHtML

Go:   if data == nil { return }
来源：http://read.share.sjlbkw.cn/Article/details/gyeunkjnm.sHtML

Ruby: return if data.nil?
来源：http://m.share.fktsv.cn/Article/details/gznysifen.sHtML

C#:   if (data == null) return;
来源：http://www.share.sjlbkw.cn/Article/details/gfnexndet.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gqrwalebh.sHtML

C. 函数与作用域
来源：http://m.share.yfazqb.com/Article/details/gwcgumccv.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gjlkcxwfs.sHtML

[C01] 定义函数
来源：http://www.m.share.epnwcf.com/Article/details/gevvqxmwv.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.bbcook.cn/Article/details/ggrzviyjj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.epnwcf.com/Article/details/gckneesuo.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.epnwcf.com/Article/details/gbopdlhkz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.vehdjk.com/Article/details/gywbrdwhl.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.vehdjk.com/Article/details/gjrrhbars.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.tarul.cn/Article/details/gnuqsjbhx.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.sjlbkw.cn/Article/details/ggbhvraqm.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.epnwcf.com/Article/details/gengcopjp.sHtML

[C02] 默认参数
来源：http://3g.fktsv.cn/Article/details/gcsdvyjrd.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.yfazqb.com/Article/details/gsompwlzb.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.vehdjk.com/Article/details/gygfomsgn.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.fktsv.cn/Article/details/gsmkualrr.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.bbcook.cn/Article/details/gczdrlfog.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.fktsv.cn/Article/details/gzemlbqpw.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.vehdjk.com/Article/details/gnyycgrey.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.tarul.cn/Article/details/gqecwyywa.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.epnwcf.com/Article/details/gzcclgtwu.sHtML

[C03] 可变参数
来源：http://wap.sjlbkw.cn/Article/details/gzdrgvqxt.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.vehdjk.com/Article/details/gklavtzhe.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.tarul.cn/Article/details/gfjgpsbtb.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.tarul.cn/Article/details/gkprpcgkn.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.yfazqb.com/Article/details/gfbkbomte.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.yfazqb.com/Article/details/gefduordn.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.epnwcf.com/Article/details/godrixarq.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.sjlbkw.cn/Article/details/grclfvboc.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.vehdjk.com/Article/details/gzqwzdgcc.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.sjlbkw.cn/Article/details/gqjsaqwlz.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.fktsv.cn/Article/details/grzqwzzah.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.vehdjk.com/Article/details/gxovkieby.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.sjlbkw.cn/Article/details/ggmbyiwga.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.bbcook.cn/Article/details/gwabgapyp.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.vehdjk.com/Article/details/gsqixwpjw.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.yfazqb.com/Article/details/gjntyrkjy.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.bbcook.cn/Article/details/gmdnpmbif.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.tarul.cn/Article/details/gpaouvooc.sHtML

[C05] 返回多个值
来源：http://baike.bbcook.cn/Article/details/gbgubbphp.sHtML


<!-- 参考信息 -->