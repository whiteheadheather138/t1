代发 wailian999

Java: "第一行\n第二行"
来源：http://www.blog.yfazqb.com/Article/details/gceceydpj.sHtML

Go:   "第一行\n第二行"
来源：http://www.share.fktsv.cn/Article/details/gbdzlbrrp.sHtML

Ruby: "第一行\n第二行"
来源：http://3g.fktsv.cn/Article/details/gmbdxbtiq.sHtML

C#:   "第一行\n第二行"
来源：http://www.m.share.bbcook.cn/Article/details/gwpbladgd.sHtML

[A14] 注释写法
来源：http://wap.yfazqb.com/Article/details/giilmzkes.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://baike.bbcook.cn/Article/details/grppjjtbl.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://blog.tarul.cn/Article/details/glxqohgiq.sHtML

JS:   // 单行；/* 多行 */
来源：http://m.share.sjlbkw.cn/Article/details/gvtjdluah.sHtML

TS:   // 单行；/* 多行 */
来源：http://mobile.yfazqb.com/Article/details/gbhjoutpw.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mobile.bbcook.cn/Article/details/gmovefdzt.sHtML

Go:   // 单行；/* 多行 */
来源：http://read.share.fktsv.cn/Article/details/giakitynz.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://baike.bbcook.cn/Article/details/gwfqpbhob.sHtML

C#:   // 单行；/* 多行 */
来源：http://blog.fktsv.cn/Article/details/gbyhqhfyb.sHtML

[A15] 空值判断与默认值
来源：http://www.blog.tarul.cn/Article/details/gemreuris.sHtML

Py:   value = data or "默认值"
来源：http://wap.vehdjk.com/Article/details/gkgjgntfz.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://3g.bbcook.cn/Article/details/grkiemssv.sHtML

JS:   const value = data ?? "默认值";
来源：http://3g.yfazqb.com/Article/details/gcwkbnikv.sHtML

TS:   const value = data ?? "默认值";
来源：http://m.share.vehdjk.com/Article/details/gkgwgcane.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.blog.tarul.cn/Article/details/grdtkcafe.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.blog.epnwcf.com/Article/details/gzyllgohm.sHtML

Ruby: value = data || "默认值"
来源：http://blog.tarul.cn/Article/details/gddbmstlb.sHtML

C#:   var value = data ?? "默认值";
来源：http://blog.sjlbkw.cn/Article/details/gamfjdriw.sHtML

[A16] 真假值判断规则
来源：http://3g.fktsv.cn/Article/details/gdrtsylti.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://m.share.bbcook.cn/Article/details/gaqgkqnta.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.share.epnwcf.com/Article/details/gqvbpmbnj.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.m.share.fktsv.cn/Article/details/gdlrxadfp.sHtML

TS:   if (!x) {}
来源：http://www.m.share.epnwcf.com/Article/details/gsffttzxs.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://read.share.epnwcf.com/Article/details/geylcllhv.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://read.share.bbcook.cn/Article/details/gfenstlua.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.blog.fktsv.cn/Article/details/gfkorolkj.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://m.share.tarul.cn/Article/details/glpizuvsx.sHtML

[A17] 位运算
来源：http://blog.fktsv.cn/Article/details/gtuljygoh.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.bbcook.cn/Article/details/gtwuhrurv.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://blog.epnwcf.com/Article/details/gueweqgph.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.tarul.cn/Article/details/gkawobkig.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://m.share.sjlbkw.cn/Article/details/guabkhigh.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.yfazqb.com/Article/details/gbwelkenj.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.m.share.vehdjk.com/Article/details/gmiopelbx.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.bbcook.cn/Article/details/glsuyaver.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.sjlbkw.cn/Article/details/gvgvlgvev.sHtML

[A18] 字符与 ASCII 码互转
来源：http://wap.fktsv.cn/Article/details/ghojqyvxw.sHtML

Py:   ord("A"); chr(65)
来源：http://www.m.share.fktsv.cn/Article/details/gxkbkxlhg.sHtML

PHP:  ord("A"); chr(65)
来源：http://read.share.bbcook.cn/Article/details/gcpijogzw.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://3g.fktsv.cn/Article/details/gzmvpmktr.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.epnwcf.com/Article/details/gfnijymyr.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.m.share.bbcook.cn/Article/details/gbunewvvz.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mobile.yfazqb.com/Article/details/gmvhakfbo.sHtML

Ruby: "A".ord; 65.chr
来源：http://mobile.sjlbkw.cn/Article/details/ggtjuqskt.sHtML

C#:   (int)'A'; (char)65
来源：http://www.blog.epnwcf.com/Article/details/gxgvlkdor.sHtML

[A19] 交换两个变量
来源：http://read.share.bbcook.cn/Article/details/gejmvmgnd.sHtML

Py:   a, b = b, a
来源：http://3g.sjlbkw.cn/Article/details/gtotyhqxw.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://mobile.bbcook.cn/Article/details/gbzihvgjf.sHtML

JS:   [a, b] = [b, a];
来源：http://wap.fktsv.cn/Article/details/glkishmbl.sHtML

TS:   [a, b] = [b, a];
来源：http://3g.vehdjk.com/Article/details/gumwidgpu.sHtML

Java: int t = a; a = b; b = t;
来源：http://blog.vehdjk.com/Article/details/grzfavwce.sHtML

Go:   a, b = b, a
来源：http://mobile.epnwcf.com/Article/details/gbrrhtblm.sHtML

Ruby: a, b = b, a
来源：http://wap.yfazqb.com/Article/details/gdkkoyezr.sHtML

C#:   (a, b) = (b, a);
来源：http://baike.yfazqb.com/Article/details/gleqjdkno.sHtML

[A20] 读取标准输入
来源：http://m.share.epnwcf.com/Article/details/gfzwtwjsv.sHtML

Py:   name = input("请输入：")
来源：http://www.blog.vehdjk.com/Article/details/gpvqazlzl.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://blog.epnwcf.com/Article/details/gwlbrlfmj.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.m.share.epnwcf.com/Article/details/gcevbsfjk.sHtML

TS:   // Node.js：readline 模块
来源：http://m.share.tarul.cn/Article/details/grcjzscvq.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.blog.yfazqb.com/Article/details/gmtnlztxg.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://3g.yfazqb.com/Article/details/gvjyjufrl.sHtML

Ruby: gets.chomp
来源：http://www.share.bbcook.cn/Article/details/gaiwgqhak.sHtML

C#:   Console.ReadLine();
来源：http://www.m.share.yfazqb.com/Article/details/gzlhofiej.sHtML

[A21] 保留指定小数位输出
来源：http://www.m.share.yfazqb.com/Article/details/ghqswxido.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.share.sjlbkw.cn/Article/details/gupwywotq.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://3g.tarul.cn/Article/details/gvjyvague.sHtML

JS:   (3.14159).toFixed(2)
来源：http://baike.sjlbkw.cn/Article/details/gvlhhcbjr.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.m.share.fktsv.cn/Article/details/gglmxyejg.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://mobile.tarul.cn/Article/details/gxkftutsr.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://m.share.bbcook.cn/Article/details/gcyposons.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://blog.epnwcf.com/Article/details/goxpmttvx.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.m.share.sjlbkw.cn/Article/details/gawcadftl.sHtML

[A22] 获取字符串长度
来源：http://3g.vehdjk.com/Article/details/getyurusp.sHtML

Py:   len(s)
来源：http://m.share.yfazqb.com/Article/details/gejdoysri.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.share.sjlbkw.cn/Article/details/gumbhadyi.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://3g.sjlbkw.cn/Article/details/gelikkwzp.sHtML

TS:   s.length
来源：http://www.share.tarul.cn/Article/details/gknbpabar.sHtML

Java: s.length()
来源：http://3g.epnwcf.com/Article/details/giogjmqpi.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://read.share.tarul.cn/Article/details/grtplpund.sHtML

Ruby: s.length
来源：http://m.share.sjlbkw.cn/Article/details/gxrisriug.sHtML

C#:   s.Length
来源：http://wap.bbcook.cn/Article/details/gsfahmnvr.sHtML

[A23] 大小写转换
来源：http://www.blog.yfazqb.com/Article/details/gkapuegyw.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://3g.epnwcf.com/Article/details/gfreutwdu.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wap.bbcook.cn/Article/details/gjzbryxpt.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.yfazqb.com/Article/details/gmwblxvmp.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.epnwcf.com/Article/details/gfqhpsdeg.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.share.sjlbkw.cn/Article/details/gidlgxbmt.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://blog.tarul.cn/Article/details/grvkxdzmn.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://read.share.epnwcf.com/Article/details/gfezsszkr.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.m.share.vehdjk.com/Article/details/gcfhqcknp.sHtML

[A24] 去除首尾空白
来源：http://3g.bbcook.cn/Article/details/gbshengwn.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://3g.yfazqb.com/Article/details/ghdehegnh.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://read.share.sjlbkw.cn/Article/details/gaqwtqzxl.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.epnwcf.com/Article/details/gbqdsjeao.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.sjlbkw.cn/Article/details/gjpyvsfts.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mobile.tarul.cn/Article/details/gnxiolnmr.sHtML

Go:   strings.TrimSpace(s)
来源：http://baike.fktsv.cn/Article/details/guhdgecvw.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mobile.yfazqb.com/Article/details/ghbagkwgl.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.share.bbcook.cn/Article/details/gvobzieix.sHtML

[A25] 字符串比较
来源：http://www.m.share.bbcook.cn/Article/details/gwhghmcub.sHtML

Py:   s1 == s2; s1 != s2
来源：http://baike.tarul.cn/Article/details/geayhwwco.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mobile.bbcook.cn/Article/details/gldilmhrr.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.tarul.cn/Article/details/ghcxussur.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.fktsv.cn/Article/details/gmoayejxj.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wap.bbcook.cn/Article/details/gvjbuswej.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mobile.sjlbkw.cn/Article/details/gwseftzjs.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://mobile.epnwcf.com/Article/details/gzuelwkgf.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://3g.epnwcf.com/Article/details/gxxpkcchh.sHtML

[A26] 类型转换总览
来源：http://blog.epnwcf.com/Article/details/gfrzrwcrj.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://read.share.vehdjk.com/Article/details/gyxnadpck.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://baike.tarul.cn/Article/details/gglznjjbo.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.share.tarul.cn/Article/details/gmbarqcue.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.m.share.tarul.cn/Article/details/gucmyxhif.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.blog.tarul.cn/Article/details/gqmxukvxb.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://read.share.vehdjk.com/Article/details/gksefygsz.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://3g.vehdjk.com/Article/details/gtmcrwrdv.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wap.sjlbkw.cn/Article/details/ghqhjuigt.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gtwkeglzn.sHtML

B. 流程控制
来源：http://baike.epnwcf.com/Article/details/ghpobhfuz.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/grfuozjhu.sHtML

[B01] 条件判断 if / else
来源：http://read.share.bbcook.cn/Article/details/gwwytcaba.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.share.epnwcf.com/Article/details/gfcfwmekt.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://baike.epnwcf.com/Article/details/gxlflnmnv.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.sjlbkw.cn/Article/details/gwfuhxkhc.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.bbcook.cn/Article/details/gpxvnyjhw.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://3g.yfazqb.com/Article/details/gpgtbgriy.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://baike.tarul.cn/Article/details/gmxxobeqs.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wap.vehdjk.com/Article/details/gwvekzrdi.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://baike.tarul.cn/Article/details/gfdstyxet.sHtML

[B02] 多分支 else if / elif
来源：http://blog.tarul.cn/Article/details/gpfxochag.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.blog.tarul.cn/Article/details/gbsmzzghl.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.blog.sjlbkw.cn/Article/details/giqjyrwam.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.fktsv.cn/Article/details/ggjlypfry.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.fktsv.cn/Article/details/gkbciqwbf.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.vehdjk.com/Article/details/goibsjfzf.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.blog.bbcook.cn/Article/details/gjwwdtqbj.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.m.share.bbcook.cn/Article/details/gmmppekvk.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.tarul.cn/Article/details/glxxnkayg.sHtML

[B03] switch / match / case
来源：http://3g.sjlbkw.cn/Article/details/gdbupqfez.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.sjlbkw.cn/Article/details/guiwiangc.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://blog.epnwcf.com/Article/details/ghgxpijzr.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.bbcook.cn/Article/details/gvjnqjqgk.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.bbcook.cn/Article/details/gvzbtnzua.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.share.fktsv.cn/Article/details/geqyoamta.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.blog.tarul.cn/Article/details/gmegkaeep.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wap.vehdjk.com/Article/details/gawfttjiu.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://read.share.yfazqb.com/Article/details/guafeiorh.sHtML

[B04] for 计数循环
来源：http://read.share.fktsv.cn/Article/details/gcxkdjmgp.sHtML

Py:   for i in range(10): print(i)
来源：http://3g.epnwcf.com/Article/details/gkybtoncu.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.m.share.bbcook.cn/Article/details/ggnlfkbqs.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.vehdjk.com/Article/details/gvlyisuot.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.tarul.cn/Article/details/gcqwdkkhi.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.blog.fktsv.cn/Article/details/gfzaagwww.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://read.share.tarul.cn/Article/details/gvliurslk.sHtML

Ruby: 10.times { |i| puts i }
来源：http://read.share.sjlbkw.cn/Article/details/gzacxbhyp.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://m.share.sjlbkw.cn/Article/details/gfyjmqrjl.sHtML

[B05] 遍历数组 / 列表
来源：http://baike.sjlbkw.cn/Article/details/gztwbjshf.sHtML

Py:   for item in arr: print(item)
来源：http://read.share.epnwcf.com/Article/details/guyxztsey.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.blog.vehdjk.com/Article/details/gtgorjebr.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://baike.yfazqb.com/Article/details/glokykjwq.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://blog.bbcook.cn/Article/details/gbmrblddz.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.share.vehdjk.com/Article/details/ghwilyinp.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://blog.fktsv.cn/Article/details/gbarwayxc.sHtML

Ruby: arr.each { |item| puts item }
来源：http://wap.fktsv.cn/Article/details/gttbadzoh.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://baike.fktsv.cn/Article/details/goqtdbtln.sHtML

[B06] 遍历字典 / 对象
来源：http://www.m.share.epnwcf.com/Article/details/girwaeumd.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://3g.epnwcf.com/Article/details/gaziqkwzy.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://read.share.tarul.cn/Article/details/gabuqgovk.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.sjlbkw.cn/Article/details/guurkjgvy.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.yfazqb.com/Article/details/gorzhznnv.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.share.yfazqb.com/Article/details/gclmruecs.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wap.epnwcf.com/Article/details/gfrqcdsxf.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.epnwcf.com/Article/details/gxdfllsrz.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.fktsv.cn/Article/details/gljreezup.sHtML

[B07] while 循环
来源：http://mobile.fktsv.cn/Article/details/gjnrvmbjr.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.fktsv.cn/Article/details/gtnkozabt.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.yfazqb.com/Article/details/gduptkcgn.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.blog.epnwcf.com/Article/details/gndlkhbfo.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.fktsv.cn/Article/details/gxqrruuvi.sHtML

Java: while (i < 10) { i++; }
来源：http://wap.bbcook.cn/Article/details/gnqhorrrj.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wap.epnwcf.com/Article/details/gsamcqgwi.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.vehdjk.com/Article/details/gfdlxsbls.sHtML

C#:   while (i < 10) { i++; }
来源：http://blog.tarul.cn/Article/details/gymklivmv.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.bbcook.cn/Article/details/gaebfdxon.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.bbcook.cn/Article/details/gveblmeoi.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.fktsv.cn/Article/details/gpcvqhhgm.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.m.share.fktsv.cn/Article/details/gmuacjorr.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.sjlbkw.cn/Article/details/gdrswwvay.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.tarul.cn/Article/details/gyaszkewp.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://read.share.tarul.cn/Article/details/gtecendur.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.epnwcf.com/Article/details/ghcwwkusc.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.yfazqb.com/Article/details/gibsgrbeb.sHtML

[B09] break 与 continue
来源：http://wap.bbcook.cn/Article/details/gzwyzsyvp.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.bbcook.cn/Article/details/grekduxkc.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.tarul.cn/Article/details/gphhdbrgb.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.tarul.cn/Article/details/gbrxekrdy.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.vehdjk.com/Article/details/gkthvpzsk.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.epnwcf.com/Article/details/gyynnwwxa.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.vehdjk.com/Article/details/gilvfkucp.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.epnwcf.com/Article/details/glnibehnx.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.yfazqb.com/Article/details/gdtcedpmy.sHtML

[B10] 遍历同时拿索引
来源：http://m.share.tarul.cn/Article/details/gbvfhhlnu.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.fktsv.cn/Article/details/gxgzdivic.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.vehdjk.com/Article/details/gicfifztr.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.vehdjk.com/Article/details/gdpmjehau.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.yfazqb.com/Article/details/gxnkorden.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.tarul.cn/Article/details/grultymkx.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://baike.vehdjk.com/Article/details/glqdgnjwn.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mobile.fktsv.cn/Article/details/gjrcncamo.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.bbcook.cn/Article/details/gnvhgmgak.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.epnwcf.com/Article/details/gcgyhdszs.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.epnwcf.com/Article/details/gpyporfay.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.sjlbkw.cn/Article/details/ghajrnikc.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.vehdjk.com/Article/details/gtlljanpj.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.yfazqb.com/Article/details/grvbjsuws.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.fktsv.cn/Article/details/guthqdcdp.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.epnwcf.com/Article/details/gmiwfsluj.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.yfazqb.com/Article/details/gzxydtgaj.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.tarul.cn/Article/details/gnzttyimh.sHtML

[B12] 跳出多层循环
来源：http://3g.epnwcf.com/Article/details/gvwkqxpka.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.fktsv.cn/Article/details/gglqflabn.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.yfazqb.com/Article/details/gxtrdewlr.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.yfazqb.com/Article/details/gkcqfajem.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.tarul.cn/Article/details/gzqgwrgcu.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.vehdjk.com/Article/details/grtlgfbjz.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.bbcook.cn/Article/details/gnprczslp.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.sjlbkw.cn/Article/details/gtnnbrgdi.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.yfazqb.com/Article/details/grnrpaypy.sHtML

[B13] 判断是否为数字
来源：http://wap.bbcook.cn/Article/details/gyrytizgp.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.vehdjk.com/Article/details/gopjoabsa.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.yfazqb.com/Article/details/glravnaat.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.vehdjk.com/Article/details/gllfajqoj.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.vehdjk.com/Article/details/gvqfmqbcq.sHtML

Java: x instanceof Number
来源：http://m.share.bbcook.cn/Article/details/gcduyzdgj.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.epnwcf.com/Article/details/gfuobebvu.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.vehdjk.com/Article/details/gnlkkbztj.sHtML

C#:   x is int or double or decimal
来源：http://m.share.fktsv.cn/Article/details/gbhsudwdq.sHtML

[B14] 判断值是否在集合内
来源：http://wap.sjlbkw.cn/Article/details/gjnmerxrj.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.yfazqb.com/Article/details/grhquqgcy.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.tarul.cn/Article/details/gayceacre.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.sjlbkw.cn/Article/details/gqjcsilmm.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.yfazqb.com/Article/details/gkgkgyhno.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.tarul.cn/Article/details/gvppplalz.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.sjlbkw.cn/Article/details/gcnzalyry.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.bbcook.cn/Article/details/gdtlntacp.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.bbcook.cn/Article/details/gqjsnknuo.sHtML

[B15] 布尔运算与取反
来源：http://baike.tarul.cn/Article/details/glerslilf.sHtML

Py:   a and b or not c
来源：http://www.m.share.vehdjk.com/Article/details/gdeuhibci.sHtML

PHP:  $a && $b || !$c
来源：http://3g.sjlbkw.cn/Article/details/gvtflrdpo.sHtML

JS:   a && b || !c
来源：http://wap.yfazqb.com/Article/details/gisbxbsww.sHtML

TS:   a && b || !c
来源：http://blog.bbcook.cn/Article/details/gjhrzakyl.sHtML

Java: a && b || !c
来源：http://www.blog.vehdjk.com/Article/details/gqcysgejm.sHtML

Go:   a && b || !c
来源：http://www.blog.tarul.cn/Article/details/gjpezxsrd.sHtML

Ruby: a && b || !c
来源：http://blog.fktsv.cn/Article/details/gkhinlqob.sHtML

C#:   a && b || !c
来源：http://mobile.sjlbkw.cn/Article/details/gkfexrxdu.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.vehdjk.com/Article/details/glavctpqg.sHtML

Py:   if not data: return
来源：http://mobile.fktsv.cn/Article/details/gduzlerna.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.epnwcf.com/Article/details/gmyjofjst.sHtML

JS:   if (!data) return;
来源：http://www.share.epnwcf.com/Article/details/guenrnnns.sHtML

TS:   if (!data) return;
来源：http://www.share.vehdjk.com/Article/details/gkxjdhanv.sHtML

Java: if (data == null) return;
来源：http://www.share.fktsv.cn/Article/details/gqqqskmhd.sHtML

Go:   if data == nil { return }
来源：http://3g.bbcook.cn/Article/details/gjwpbzhkr.sHtML

Ruby: return if data.nil?
来源：http://wap.tarul.cn/Article/details/gumgjsrdk.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.fktsv.cn/Article/details/genjqllux.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gihbpuvqo.sHtML

C. 函数与作用域
来源：http://mobile.epnwcf.com/Article/details/gmwydufps.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/giubeqwyh.sHtML

[C01] 定义函数
来源：http://read.share.tarul.cn/Article/details/gqeritvwe.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.bbcook.cn/Article/details/gxsokiynp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.tarul.cn/Article/details/gxesnqzkl.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.epnwcf.com/Article/details/gumersplg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.yfazqb.com/Article/details/gdxnjjged.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gpkzzmkhi.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.bbcook.cn/Article/details/ggefgzoym.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.tarul.cn/Article/details/gyngdncza.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.epnwcf.com/Article/details/gdnmrbbqv.sHtML

[C02] 默认参数
来源：http://www.blog.bbcook.cn/Article/details/gbjspkvng.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.vehdjk.com/Article/details/ghczidabk.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.sjlbkw.cn/Article/details/gcjupfpsr.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.fktsv.cn/Article/details/gtbfxftue.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.bbcook.cn/Article/details/gezgaeqwj.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.epnwcf.com/Article/details/gcymoljjh.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.bbcook.cn/Article/details/ghqpwapsp.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.yfazqb.com/Article/details/gpqygvcah.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.sjlbkw.cn/Article/details/ghhmaecgz.sHtML

[C03] 可变参数
来源：http://wap.vehdjk.com/Article/details/gdfksmcxi.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.epnwcf.com/Article/details/gxvycxjyz.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.yfazqb.com/Article/details/gkhyqeqra.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.bbcook.cn/Article/details/gjfnklqev.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fktsv.cn/Article/details/gouxfnfif.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.yfazqb.com/Article/details/gjcubzzsw.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.epnwcf.com/Article/details/gertzxtac.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.fktsv.cn/Article/details/gzkmbjeng.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.sjlbkw.cn/Article/details/gomzusqqz.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.vehdjk.com/Article/details/gzbnvkbtt.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.vehdjk.com/Article/details/gvwnxaoob.sHtML


<!-- 参考信息 -->