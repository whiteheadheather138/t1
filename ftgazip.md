代发 wailian999

C#:   // 单行；/* 多行 */
来源：http://blog.bbcook.cn/Article/details/gvuxpodzz.sHtML

[A15] 空值判断与默认值
来源：http://www.blog.vehdjk.com/Article/details/gliwfdvva.sHtML

Py:   value = data or "默认值"
来源：http://baike.sjlbkw.cn/Article/details/gqetrkkut.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.share.vehdjk.com/Article/details/grhwuzluv.sHtML

JS:   const value = data ?? "默认值";
来源：http://3g.tarul.cn/Article/details/grfkpiaxv.sHtML

TS:   const value = data ?? "默认值";
来源：http://3g.vehdjk.com/Article/details/gyqhwobiy.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://blog.vehdjk.com/Article/details/gszpcsuha.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.blog.vehdjk.com/Article/details/gllpbvxyc.sHtML

Ruby: value = data || "默认值"
来源：http://mobile.tarul.cn/Article/details/gspyfaqit.sHtML

C#:   var value = data ?? "默认值";
来源：http://mobile.bbcook.cn/Article/details/gdglhlgdp.sHtML

[A16] 真假值判断规则
来源：http://read.share.sjlbkw.cn/Article/details/gehygxrbl.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mobile.bbcook.cn/Article/details/ggwyticce.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.blog.bbcook.cn/Article/details/gdbkxbmhn.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://wap.bbcook.cn/Article/details/ggfisscrl.sHtML

TS:   if (!x) {}
来源：http://mobile.yfazqb.com/Article/details/gdtsqlhdz.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://m.share.yfazqb.com/Article/details/gzezixkpw.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://read.share.tarul.cn/Article/details/gmriwfbll.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.m.share.fktsv.cn/Article/details/gskdjomnm.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://read.share.bbcook.cn/Article/details/gnplrzsva.sHtML

[A17] 位运算
来源：http://www.m.share.epnwcf.com/Article/details/giqpomzag.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.fktsv.cn/Article/details/gubzrornw.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mobile.vehdjk.com/Article/details/glnbcbfca.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.epnwcf.com/Article/details/gmguhpppa.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.blog.vehdjk.com/Article/details/gjdiciali.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.yfazqb.com/Article/details/ggahcedsg.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://blog.epnwcf.com/Article/details/gvtqrxsdd.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.sjlbkw.cn/Article/details/gzkvjdvhp.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.bbcook.cn/Article/details/gbhallrcy.sHtML

[A18] 字符与 ASCII 码互转
来源：http://read.share.yfazqb.com/Article/details/gmmwxrlgf.sHtML

Py:   ord("A"); chr(65)
来源：http://www.blog.epnwcf.com/Article/details/gjrjkjygk.sHtML

PHP:  ord("A"); chr(65)
来源：http://m.share.yfazqb.com/Article/details/gxtlugquh.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.yfazqb.com/Article/details/gpydnvxly.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.fktsv.cn/Article/details/gmzecegmm.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.m.share.sjlbkw.cn/Article/details/gsmmxmdel.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://baike.yfazqb.com/Article/details/gocwfthvt.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.blog.yfazqb.com/Article/details/gqgewmjok.sHtML

C#:   (int)'A'; (char)65
来源：http://baike.tarul.cn/Article/details/geayojaai.sHtML

[A19] 交换两个变量
来源：http://www.m.share.bbcook.cn/Article/details/gcuoteapr.sHtML

Py:   a, b = b, a
来源：http://mobile.fktsv.cn/Article/details/gmltgkemg.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://blog.epnwcf.com/Article/details/gpxwdixec.sHtML

JS:   [a, b] = [b, a];
来源：http://www.share.yfazqb.com/Article/details/gugmcjjsc.sHtML

TS:   [a, b] = [b, a];
来源：http://www.m.share.yfazqb.com/Article/details/gxxyxcknp.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.m.share.epnwcf.com/Article/details/ggtwhisjy.sHtML

Go:   a, b = b, a
来源：http://baike.bbcook.cn/Article/details/gqwioasdn.sHtML

Ruby: a, b = b, a
来源：http://mobile.bbcook.cn/Article/details/gfsogoaci.sHtML

C#:   (a, b) = (b, a);
来源：http://www.m.share.epnwcf.com/Article/details/gkyepnzya.sHtML

[A20] 读取标准输入
来源：http://wap.yfazqb.com/Article/details/gpzddxymk.sHtML

Py:   name = input("请输入：")
来源：http://www.share.epnwcf.com/Article/details/gebzdnmpl.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://read.share.yfazqb.com/Article/details/grjqdpaxh.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wap.vehdjk.com/Article/details/guyishbix.sHtML

TS:   // Node.js：readline 模块
来源：http://www.m.share.epnwcf.com/Article/details/gscnhdqel.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.m.share.bbcook.cn/Article/details/gvnpjyjyl.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://mobile.bbcook.cn/Article/details/gffszzqhj.sHtML

Ruby: gets.chomp
来源：http://3g.bbcook.cn/Article/details/grfmnagni.sHtML

C#:   Console.ReadLine();
来源：http://baike.tarul.cn/Article/details/gytbpywsi.sHtML

[A21] 保留指定小数位输出
来源：http://baike.vehdjk.com/Article/details/guwpjxbjh.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.blog.tarul.cn/Article/details/gplbwkwtb.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.blog.bbcook.cn/Article/details/gwgvyxtbh.sHtML

JS:   (3.14159).toFixed(2)
来源：http://3g.tarul.cn/Article/details/grwxklomn.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.share.sjlbkw.cn/Article/details/gevruggzm.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://wap.epnwcf.com/Article/details/gwfhfiqhv.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://m.share.epnwcf.com/Article/details/gnjoxocth.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://read.share.vehdjk.com/Article/details/gqzttmqtc.sHtML

C#:   3.14159.ToString("F2")
来源：http://read.share.sjlbkw.cn/Article/details/gimcuzdgx.sHtML

[A22] 获取字符串长度
来源：http://3g.epnwcf.com/Article/details/gjgrcpwjr.sHtML

Py:   len(s)
来源：http://wap.fktsv.cn/Article/details/gcpcksktg.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://3g.bbcook.cn/Article/details/gozybbmbo.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wap.yfazqb.com/Article/details/gvpjmmxad.sHtML

TS:   s.length
来源：http://read.share.yfazqb.com/Article/details/gehjgnuge.sHtML

Java: s.length()
来源：http://blog.bbcook.cn/Article/details/gduqiahdk.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.share.fktsv.cn/Article/details/gurrrizzs.sHtML

Ruby: s.length
来源：http://3g.sjlbkw.cn/Article/details/gvprhcunq.sHtML

C#:   s.Length
来源：http://3g.yfazqb.com/Article/details/gyavvlgpu.sHtML

[A23] 大小写转换
来源：http://m.share.tarul.cn/Article/details/ghppioion.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.m.share.fktsv.cn/Article/details/gntvzanij.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mobile.tarul.cn/Article/details/gwblycsge.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.vehdjk.com/Article/details/gviudbyyz.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.tarul.cn/Article/details/gvbnbkspi.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://read.share.epnwcf.com/Article/details/gtfedhvrp.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://baike.epnwcf.com/Article/details/ggsmyjjsd.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://blog.yfazqb.com/Article/details/gekxzgwfu.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.m.share.epnwcf.com/Article/details/gkpmlxaas.sHtML

[A24] 去除首尾空白
来源：http://baike.epnwcf.com/Article/details/gsfcxlsmh.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://blog.vehdjk.com/Article/details/gfsdiouyb.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://3g.sjlbkw.cn/Article/details/glsiopbdl.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.epnwcf.com/Article/details/gaoxesire.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.fktsv.cn/Article/details/gqeslztyd.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://baike.vehdjk.com/Article/details/gqkjyhxgg.sHtML

Go:   strings.TrimSpace(s)
来源：http://wap.yfazqb.com/Article/details/gkssatjqd.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://baike.yfazqb.com/Article/details/gacqxdzlg.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://read.share.bbcook.cn/Article/details/gexnvpvui.sHtML

[A25] 字符串比较
来源：http://www.m.share.yfazqb.com/Article/details/gfajfdmpf.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.blog.epnwcf.com/Article/details/gfekucipi.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wap.epnwcf.com/Article/details/gmobigejs.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.yfazqb.com/Article/details/gihsseweq.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.tarul.cn/Article/details/gcmtkeevr.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://blog.bbcook.cn/Article/details/gqdjpdryd.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://read.share.yfazqb.com/Article/details/gwiakmotj.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.m.share.fktsv.cn/Article/details/grwufvxsv.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.share.epnwcf.com/Article/details/gudydyxvg.sHtML

[A26] 类型转换总览
来源：http://baike.epnwcf.com/Article/details/gkarrojor.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://read.share.sjlbkw.cn/Article/details/gbkykeulg.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://read.share.vehdjk.com/Article/details/gjlxoxeis.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.m.share.vehdjk.com/Article/details/ghfrrlrgg.sHtML

TS:   Number() String() Boolean() x as number
来源：http://wap.yfazqb.com/Article/details/gksasuyzw.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://baike.tarul.cn/Article/details/gxlifzcgf.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.share.yfazqb.com/Article/details/gaysmewbk.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://m.share.vehdjk.com/Article/details/gzzascgtr.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://read.share.sjlbkw.cn/Article/details/goatbzook.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gyjxoljki.sHtML

B. 流程控制
来源：http://www.blog.fktsv.cn/Article/details/gcayczyml.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gbtmzgcgp.sHtML

[B01] 条件判断 if / else
来源：http://3g.fktsv.cn/Article/details/glzcajygx.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://baike.yfazqb.com/Article/details/gtsaoemlw.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mobile.fktsv.cn/Article/details/gnavhambg.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.fktsv.cn/Article/details/gdxgplmjy.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.bbcook.cn/Article/details/gxmoeehpw.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://m.share.fktsv.cn/Article/details/giiskknxs.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.blog.tarul.cn/Article/details/gixrydfbn.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://read.share.epnwcf.com/Article/details/giqdnlvnq.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://m.share.bbcook.cn/Article/details/gfjrupnpm.sHtML

[B02] 多分支 else if / elif
来源：http://mobile.yfazqb.com/Article/details/gqxezklqu.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.share.yfazqb.com/Article/details/gqutbjeoj.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://blog.epnwcf.com/Article/details/ghpybvwlj.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.bbcook.cn/Article/details/gxaepczvx.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.yfazqb.com/Article/details/gwlqihdkz.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.bbcook.cn/Article/details/gsafjnrad.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.m.share.vehdjk.com/Article/details/gxwzprtjl.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://m.share.bbcook.cn/Article/details/gkbxzdasl.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.sjlbkw.cn/Article/details/gwllymgty.sHtML

[B03] switch / match / case
来源：http://www.share.vehdjk.com/Article/details/gmgarlgjz.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://read.share.vehdjk.com/Article/details/gnslrovhb.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://3g.sjlbkw.cn/Article/details/grliovadg.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.tarul.cn/Article/details/ggdwwbezs.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.epnwcf.com/Article/details/gcfklvwpv.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://blog.bbcook.cn/Article/details/gxvzndehk.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://m.share.sjlbkw.cn/Article/details/gagyrytfk.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.share.yfazqb.com/Article/details/guittaocy.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mobile.epnwcf.com/Article/details/gqfmvifhf.sHtML

[B04] for 计数循环
来源：http://www.blog.tarul.cn/Article/details/grknbsvzl.sHtML

Py:   for i in range(10): print(i)
来源：http://www.blog.bbcook.cn/Article/details/gkfwldlst.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://baike.tarul.cn/Article/details/gkjvaqlps.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.vehdjk.com/Article/details/ggfhwdhax.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.bbcook.cn/Article/details/gbygksigg.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mobile.fktsv.cn/Article/details/ganxbxqlp.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.m.share.vehdjk.com/Article/details/gkgudclzp.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.share.epnwcf.com/Article/details/ghxqrcsvi.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mobile.tarul.cn/Article/details/ggehzjptu.sHtML

[B05] 遍历数组 / 列表
来源：http://www.blog.vehdjk.com/Article/details/gysgrjtsv.sHtML

Py:   for item in arr: print(item)
来源：http://read.share.tarul.cn/Article/details/grsusrmxd.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.m.share.tarul.cn/Article/details/gwkufpahd.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.bbcook.cn/Article/details/gvxxhlgqv.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://blog.tarul.cn/Article/details/gbtfcvspz.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://baike.yfazqb.com/Article/details/gjcckazgk.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.share.vehdjk.com/Article/details/gyodpkudz.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.blog.vehdjk.com/Article/details/gkonedqcf.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.share.epnwcf.com/Article/details/gvrgzuuqi.sHtML

[B06] 遍历字典 / 对象
来源：http://baike.vehdjk.com/Article/details/gaslyuadc.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://blog.epnwcf.com/Article/details/gjrjbenlt.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://blog.bbcook.cn/Article/details/gycyuehdu.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.fktsv.cn/Article/details/govrjtcmo.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.yfazqb.com/Article/details/gdipuopri.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.yfazqb.com/Article/details/gnvitsntz.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://3g.sjlbkw.cn/Article/details/gajsexiyi.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.blog.epnwcf.com/Article/details/gidqozhig.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.sjlbkw.cn/Article/details/geynamycn.sHtML

[B07] while 循环
来源：http://read.share.yfazqb.com/Article/details/gusjaaugq.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.bbcook.cn/Article/details/gjbpzurnp.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.blog.yfazqb.com/Article/details/gaeuvxbwj.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.share.fktsv.cn/Article/details/gqcqgomak.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.fktsv.cn/Article/details/ghxwaytgq.sHtML

Java: while (i < 10) { i++; }
来源：http://mobile.yfazqb.com/Article/details/gelmbdrsj.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.vehdjk.com/Article/details/gkxqjgyrj.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.epnwcf.com/Article/details/gejotigey.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.vehdjk.com/Article/details/gbhgnztxy.sHtML

[B08] do-while（至少执行一次）
来源：http://www.blog.tarul.cn/Article/details/gybjqecok.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.sjlbkw.cn/Article/details/gxrwxbeeg.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.vehdjk.com/Article/details/getnphsoz.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.yfazqb.com/Article/details/gvdwwknta.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.yfazqb.com/Article/details/gqazclvhl.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.sjlbkw.cn/Article/details/gjxkylgnh.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://read.share.fktsv.cn/Article/details/gnkuhldbq.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.epnwcf.com/Article/details/gxifumdez.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.fktsv.cn/Article/details/gkydwrumk.sHtML

[B09] break 与 continue
来源：http://baike.epnwcf.com/Article/details/gvdcqbjyu.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.bbcook.cn/Article/details/gcsuxamxj.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.fktsv.cn/Article/details/gnotxnrjw.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.sjlbkw.cn/Article/details/gwxrvxijj.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fktsv.cn/Article/details/gfxmeiksj.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.sjlbkw.cn/Article/details/gstwifqbs.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.vehdjk.com/Article/details/gvdlerclu.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.tarul.cn/Article/details/gacvmpobj.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.vehdjk.com/Article/details/gugsbnfjb.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.bbcook.cn/Article/details/gnuzqzrlh.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.yfazqb.com/Article/details/gkujrhntb.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.fktsv.cn/Article/details/geiymbgpt.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.tarul.cn/Article/details/ggsagixvs.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.yfazqb.com/Article/details/gywuabywv.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.tarul.cn/Article/details/gvvaalvbl.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.fktsv.cn/Article/details/gjpypozsv.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.vehdjk.com/Article/details/gxshekulf.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.tarul.cn/Article/details/gcfcifntk.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.tarul.cn/Article/details/gywasvuqo.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.fktsv.cn/Article/details/gbnzfmtqc.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.bbcook.cn/Article/details/guwylyjgv.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.epnwcf.com/Article/details/gtolcqcyl.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.yfazqb.com/Article/details/glqkggbek.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.yfazqb.com/Article/details/guihaolrm.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.tarul.cn/Article/details/gmqkzlwap.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.vehdjk.com/Article/details/gjuhzuzya.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.epnwcf.com/Article/details/gdhmkumxw.sHtML

[B12] 跳出多层循环
来源：http://www.share.vehdjk.com/Article/details/ggkuqskdm.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.fktsv.cn/Article/details/gsiwllqdy.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.yfazqb.com/Article/details/gabhwznyx.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fktsv.cn/Article/details/gvfywqoir.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.bbcook.cn/Article/details/gbifzbyta.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.tarul.cn/Article/details/gxhczfiub.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.tarul.cn/Article/details/gbrwygbtx.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.sjlbkw.cn/Article/details/gbsdolcmt.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.vehdjk.com/Article/details/gnruodcrd.sHtML

[B13] 判断是否为数字
来源：http://wap.fktsv.cn/Article/details/gdckvyjdw.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.yfazqb.com/Article/details/gfkfqvdyv.sHtML

PHP:  is_numeric($x)
来源：http://mobile.fktsv.cn/Article/details/gbwnvnxky.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.sjlbkw.cn/Article/details/gphyzqfbn.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.epnwcf.com/Article/details/ggzdhxncj.sHtML

Java: x instanceof Number
来源：http://www.blog.bbcook.cn/Article/details/gqesvumlo.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.sjlbkw.cn/Article/details/ghumhgtpe.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.epnwcf.com/Article/details/gddcygdue.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.bbcook.cn/Article/details/grqcvgtay.sHtML

[B14] 判断值是否在集合内
来源：http://blog.epnwcf.com/Article/details/gpivggzzs.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.vehdjk.com/Article/details/gpmzxwspn.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.sjlbkw.cn/Article/details/gmegglshk.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.epnwcf.com/Article/details/gdlfgswkn.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.fktsv.cn/Article/details/gakejqatu.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.yfazqb.com/Article/details/getzlwotb.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.tarul.cn/Article/details/gwtvwucqj.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.yfazqb.com/Article/details/gjwwrtdpy.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.tarul.cn/Article/details/gxkdgpmgg.sHtML

[B15] 布尔运算与取反
来源：http://baike.sjlbkw.cn/Article/details/gfiupuxfh.sHtML

Py:   a and b or not c
来源：http://3g.bbcook.cn/Article/details/gbskawmhl.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.yfazqb.com/Article/details/grryisfmi.sHtML

JS:   a && b || !c
来源：http://www.share.vehdjk.com/Article/details/gxmxyubvb.sHtML

TS:   a && b || !c
来源：http://3g.bbcook.cn/Article/details/gfjqgemcp.sHtML

Java: a && b || !c
来源：http://3g.vehdjk.com/Article/details/ghsgnooep.sHtML

Go:   a && b || !c
来源：http://read.share.tarul.cn/Article/details/gcqfszzcz.sHtML

Ruby: a && b || !c
来源：http://www.m.share.yfazqb.com/Article/details/gpxmertoe.sHtML

C#:   a && b || !c
来源：http://3g.yfazqb.com/Article/details/gtbxtdyvc.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.epnwcf.com/Article/details/gfffejclo.sHtML

Py:   if not data: return
来源：http://wap.epnwcf.com/Article/details/gvmyccjwy.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.epnwcf.com/Article/details/glvpzxaax.sHtML

JS:   if (!data) return;
来源：http://baike.bbcook.cn/Article/details/grrqntvpl.sHtML

TS:   if (!data) return;
来源：http://www.share.sjlbkw.cn/Article/details/gtfqudwcp.sHtML

Java: if (data == null) return;
来源：http://3g.vehdjk.com/Article/details/geufaxplf.sHtML

Go:   if data == nil { return }
来源：http://blog.sjlbkw.cn/Article/details/gfxqfoedq.sHtML

Ruby: return if data.nil?
来源：http://read.share.tarul.cn/Article/details/gectukwdy.sHtML

C#:   if (data == null) return;
来源：http://wap.sjlbkw.cn/Article/details/ghvihrvsn.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gpgweviwx.sHtML

C. 函数与作用域
来源：http://www.share.sjlbkw.cn/Article/details/gvsuthetw.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gdzyvupxr.sHtML

[C01] 定义函数
来源：http://baike.bbcook.cn/Article/details/gkaqerojn.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.yfazqb.com/Article/details/guuutgjle.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.tarul.cn/Article/details/gthnhwpmj.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.vehdjk.com/Article/details/gifatkwfk.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.bbcook.cn/Article/details/gssqdjksa.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.sjlbkw.cn/Article/details/gqefftjsc.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.yfazqb.com/Article/details/gmdhfqfpo.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.tarul.cn/Article/details/gbaunufku.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.sjlbkw.cn/Article/details/gkssjqgwr.sHtML

[C02] 默认参数
来源：http://mobile.tarul.cn/Article/details/gqaysfzys.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.fktsv.cn/Article/details/gkwwgyizy.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.epnwcf.com/Article/details/gpgnhvpvv.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.yfazqb.com/Article/details/gxocdiizh.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.yfazqb.com/Article/details/gaiaggnjs.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.fktsv.cn/Article/details/gaoxvbilh.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.tarul.cn/Article/details/gdhqciyts.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.tarul.cn/Article/details/guxzxqsoz.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.bbcook.cn/Article/details/gqkyjbdat.sHtML

[C03] 可变参数
来源：http://blog.epnwcf.com/Article/details/gqihmgmop.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.bbcook.cn/Article/details/gorriqdsq.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.bbcook.cn/Article/details/gnxhvnlvy.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.epnwcf.com/Article/details/gjzutyvjn.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fktsv.cn/Article/details/gwjflgluy.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.fktsv.cn/Article/details/gpfqjeciz.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.vehdjk.com/Article/details/gcrhnfmtw.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.fktsv.cn/Article/details/gxvfxutpi.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.tarul.cn/Article/details/gbokwjedr.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.tarul.cn/Article/details/gfwdrwwpq.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.bbcook.cn/Article/details/gsqvkubsb.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.epnwcf.com/Article/details/gnmuvegxg.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.vehdjk.com/Article/details/gerfbiskm.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.epnwcf.com/Article/details/gjfncdgbk.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.fktsv.cn/Article/details/ggtevdlaa.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.epnwcf.com/Article/details/gvilvkoio.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.bbcook.cn/Article/details/gaysforxp.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.tarul.cn/Article/details/gbsgmdhng.sHtML

[C05] 返回多个值
来源：http://www.share.sjlbkw.cn/Article/details/gjupqyaxv.sHtML

Py:   return a, b
来源：http://mobile.vehdjk.com/Article/details/gvnrqinbz.sHtML

PHP:  return [$a, $b];
来源：http://baike.fktsv.cn/Article/details/ggwejshmh.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.fktsv.cn/Article/details/giqilmrjn.sHtML

TS:   return { a, b };
来源：http://3g.tarul.cn/Article/details/gqbkuarqt.sHtML


<!-- 参考信息 -->