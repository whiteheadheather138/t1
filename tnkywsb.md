代发 wailian999

Py:   "第一行\n第二行"
来源：http://www.share.sjlbkw.cn/Article/details/ghrenxcxh.sHtML

PHP:  "第一行\n第二行"
来源：http://www.share.fktsv.cn/Article/details/gvuoylgvx.sHtML

JS:   "第一行\n第二行"
来源：http://mobile.epnwcf.com/Article/details/gwpjghpui.sHtML

TS:   "第一行\n第二行"
来源：http://3g.vehdjk.com/Article/details/gghnccwou.sHtML

Java: "第一行\n第二行"
来源：http://www.share.yfazqb.com/Article/details/gpkopqvir.sHtML

Go:   "第一行\n第二行"
来源：http://read.share.yfazqb.com/Article/details/gsdnnultn.sHtML

Ruby: "第一行\n第二行"
来源：http://blog.sjlbkw.cn/Article/details/grzvnnbhk.sHtML

C#:   "第一行\n第二行"
来源：http://read.share.yfazqb.com/Article/details/gmogzilci.sHtML

[A14] 注释写法
来源：http://baike.vehdjk.com/Article/details/gbmkecutn.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://baike.fktsv.cn/Article/details/gwgyjqrfl.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.m.share.fktsv.cn/Article/details/genlzvjzj.sHtML

JS:   // 单行；/* 多行 */
来源：http://mobile.bbcook.cn/Article/details/gxvwikvfu.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.blog.bbcook.cn/Article/details/gnzqsteng.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://3g.fktsv.cn/Article/details/ggtmbwpse.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.m.share.bbcook.cn/Article/details/gavoisdih.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://wap.sjlbkw.cn/Article/details/gttfaqcbg.sHtML

C#:   // 单行；/* 多行 */
来源：http://blog.bbcook.cn/Article/details/gjokzkjjt.sHtML

[A15] 空值判断与默认值
来源：http://read.share.yfazqb.com/Article/details/gbpocftmo.sHtML

Py:   value = data or "默认值"
来源：http://www.blog.vehdjk.com/Article/details/ghcaavyzy.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://mobile.epnwcf.com/Article/details/ghdghakyf.sHtML

JS:   const value = data ?? "默认值";
来源：http://blog.vehdjk.com/Article/details/golcyttzb.sHtML

TS:   const value = data ?? "默认值";
来源：http://3g.tarul.cn/Article/details/gqmgqowrw.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.blog.tarul.cn/Article/details/gbionagxq.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://mobile.sjlbkw.cn/Article/details/gnredwtkr.sHtML

Ruby: value = data || "默认值"
来源：http://m.share.vehdjk.com/Article/details/gwyqcofcy.sHtML

C#:   var value = data ?? "默认值";
来源：http://m.share.vehdjk.com/Article/details/gsajopshs.sHtML

[A16] 真假值判断规则
来源：http://read.share.sjlbkw.cn/Article/details/ghwsfhcbs.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://blog.fktsv.cn/Article/details/ghrhcqawj.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.blog.tarul.cn/Article/details/gverwkbjk.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://baike.bbcook.cn/Article/details/gmckzihqb.sHtML

TS:   if (!x) {}
来源：http://m.share.epnwcf.com/Article/details/gtkyrfgqe.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://mobile.fktsv.cn/Article/details/gdxxchkmd.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://mobile.sjlbkw.cn/Article/details/gbcxygccu.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://m.share.bbcook.cn/Article/details/gescchzbe.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.blog.epnwcf.com/Article/details/gqeuozmns.sHtML

[A17] 位运算
来源：http://www.m.share.yfazqb.com/Article/details/gldlgfkrx.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.vehdjk.com/Article/details/gwbzvfqtg.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://m.share.sjlbkw.cn/Article/details/gyrmrkhww.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.epnwcf.com/Article/details/gvjgpgwpy.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://mobile.fktsv.cn/Article/details/gulbjaygw.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.tarul.cn/Article/details/gulmxfxto.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.m.share.vehdjk.com/Article/details/gkstpjjzc.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.tarul.cn/Article/details/gjqdiavjc.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.vehdjk.com/Article/details/gnaqonteg.sHtML

[A18] 字符与 ASCII 码互转
来源：http://wap.vehdjk.com/Article/details/gtupgtcdz.sHtML

Py:   ord("A"); chr(65)
来源：http://m.share.epnwcf.com/Article/details/gbmxozklu.sHtML

PHP:  ord("A"); chr(65)
来源：http://3g.sjlbkw.cn/Article/details/geepchsba.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://read.share.sjlbkw.cn/Article/details/gqonlyold.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.sjlbkw.cn/Article/details/gzkfqqeor.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.share.vehdjk.com/Article/details/gmfxnlyiu.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.m.share.yfazqb.com/Article/details/glajhbnrz.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.blog.tarul.cn/Article/details/gwemqikze.sHtML

C#:   (int)'A'; (char)65
来源：http://www.share.bbcook.cn/Article/details/gmvqiehnb.sHtML

[A19] 交换两个变量
来源：http://3g.fktsv.cn/Article/details/gguykjeuv.sHtML

Py:   a, b = b, a
来源：http://baike.yfazqb.com/Article/details/gqipijjxn.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://3g.tarul.cn/Article/details/gqtiuaqxn.sHtML

JS:   [a, b] = [b, a];
来源：http://m.share.sjlbkw.cn/Article/details/gdfimbnuw.sHtML

TS:   [a, b] = [b, a];
来源：http://3g.yfazqb.com/Article/details/gwkgwcfhq.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.blog.epnwcf.com/Article/details/gcippeyux.sHtML

Go:   a, b = b, a
来源：http://read.share.epnwcf.com/Article/details/gpsvpfcaf.sHtML

Ruby: a, b = b, a
来源：http://wap.tarul.cn/Article/details/gpxiefbvy.sHtML

C#:   (a, b) = (b, a);
来源：http://wap.vehdjk.com/Article/details/grbgcpnbu.sHtML

[A20] 读取标准输入
来源：http://www.m.share.yfazqb.com/Article/details/gyyxshtqd.sHtML

Py:   name = input("请输入：")
来源：http://mobile.yfazqb.com/Article/details/gxruxutyz.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.blog.yfazqb.com/Article/details/glicfgyul.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://mobile.sjlbkw.cn/Article/details/gujptoybn.sHtML

TS:   // Node.js：readline 模块
来源：http://www.blog.epnwcf.com/Article/details/ggiwnvbqt.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://m.share.bbcook.cn/Article/details/gnannejce.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://blog.bbcook.cn/Article/details/gznypjoox.sHtML

Ruby: gets.chomp
来源：http://blog.tarul.cn/Article/details/ghrvrivzs.sHtML

C#:   Console.ReadLine();
来源：http://www.m.share.epnwcf.com/Article/details/gwohprtjr.sHtML

[A21] 保留指定小数位输出
来源：http://mobile.sjlbkw.cn/Article/details/ghsmvxcht.sHtML

Py:   f"{3.14159:.2f}"
来源：http://wap.yfazqb.com/Article/details/ghjozieqj.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.share.yfazqb.com/Article/details/gsxcbhtty.sHtML

JS:   (3.14159).toFixed(2)
来源：http://wap.bbcook.cn/Article/details/grbkyqjfg.sHtML

TS:   (3.14159).toFixed(2)
来源：http://mobile.bbcook.cn/Article/details/ghfbtqieq.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://m.share.fktsv.cn/Article/details/gqhxnjcud.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://baike.bbcook.cn/Article/details/gitumlyfx.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.share.fktsv.cn/Article/details/gefeyuxxh.sHtML

C#:   3.14159.ToString("F2")
来源：http://blog.fktsv.cn/Article/details/gxxsqopse.sHtML

[A22] 获取字符串长度
来源：http://wap.fktsv.cn/Article/details/gddnggvyg.sHtML

Py:   len(s)
来源：http://www.share.yfazqb.com/Article/details/gokvdjurz.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wap.yfazqb.com/Article/details/grbfifcos.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://baike.yfazqb.com/Article/details/goefzngyc.sHtML

TS:   s.length
来源：http://mobile.epnwcf.com/Article/details/gbavgjlgl.sHtML

Java: s.length()
来源：http://www.blog.vehdjk.com/Article/details/ghqzvrvzz.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://read.share.tarul.cn/Article/details/ghiixstfi.sHtML

Ruby: s.length
来源：http://m.share.fktsv.cn/Article/details/gsrjqxxib.sHtML

C#:   s.Length
来源：http://m.share.epnwcf.com/Article/details/gpoajtfjr.sHtML

[A23] 大小写转换
来源：http://wap.fktsv.cn/Article/details/gzfdzumpi.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://mobile.epnwcf.com/Article/details/ghtqxruev.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.share.fktsv.cn/Article/details/gkffwqaed.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.vehdjk.com/Article/details/gtqtdkfjl.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.tarul.cn/Article/details/gcjoccdve.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.vehdjk.com/Article/details/gpkerzjrh.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.m.share.yfazqb.com/Article/details/gswmmyuhu.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.blog.bbcook.cn/Article/details/gtqpwuhhs.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://wap.fktsv.cn/Article/details/gmwmpygtb.sHtML

[A24] 去除首尾空白
来源：http://3g.tarul.cn/Article/details/gaqthzvpv.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://m.share.bbcook.cn/Article/details/gsjaiuaay.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://3g.vehdjk.com/Article/details/gappupcrv.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.sjlbkw.cn/Article/details/ghxaqfgyw.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.fktsv.cn/Article/details/gkbxwmtdt.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://m.share.vehdjk.com/Article/details/gkmtxcwhb.sHtML

Go:   strings.TrimSpace(s)
来源：http://wap.fktsv.cn/Article/details/gerauvgpt.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.share.vehdjk.com/Article/details/gunurbiku.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.m.share.yfazqb.com/Article/details/gnxiopbwv.sHtML

[A25] 字符串比较
来源：http://m.share.yfazqb.com/Article/details/gjefrkuiu.sHtML

Py:   s1 == s2; s1 != s2
来源：http://wap.fktsv.cn/Article/details/gvqagmjrv.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.m.share.bbcook.cn/Article/details/gvxoplvud.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.sjlbkw.cn/Article/details/glzipqanq.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.yfazqb.com/Article/details/gqwajngfn.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://m.share.sjlbkw.cn/Article/details/glncyzhak.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.blog.bbcook.cn/Article/details/guasfijff.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://read.share.tarul.cn/Article/details/gafeudzca.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://read.share.bbcook.cn/Article/details/giwlnzsex.sHtML

[A26] 类型转换总览
来源：http://3g.tarul.cn/Article/details/gtuwhulma.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://m.share.tarul.cn/Article/details/ghwukcoct.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://read.share.fktsv.cn/Article/details/gexwzxqhx.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.share.yfazqb.com/Article/details/gzlbrnxlm.sHtML

TS:   Number() String() Boolean() x as number
来源：http://m.share.yfazqb.com/Article/details/gncklrjes.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mobile.fktsv.cn/Article/details/gfhtdetmi.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.m.share.tarul.cn/Article/details/gqqcpzgvl.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://mobile.tarul.cn/Article/details/gaanjnqzi.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://blog.vehdjk.com/Article/details/gghzscskj.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/guewsgbqg.sHtML

B. 流程控制
来源：http://blog.fktsv.cn/Article/details/gfhobtani.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gntwoeida.sHtML

[B01] 条件判断 if / else
来源：http://www.blog.fktsv.cn/Article/details/grmtrzrur.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://read.share.epnwcf.com/Article/details/gyoilsixa.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.blog.yfazqb.com/Article/details/gtaakocco.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.tarul.cn/Article/details/gpfnfchnj.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.fktsv.cn/Article/details/gauixkxbv.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.share.bbcook.cn/Article/details/ggkrwqguy.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wap.fktsv.cn/Article/details/grcaggbrf.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://m.share.fktsv.cn/Article/details/gfrnrgzsp.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://blog.yfazqb.com/Article/details/gvjyujzxv.sHtML

[B02] 多分支 else if / elif
来源：http://read.share.tarul.cn/Article/details/gumvmmetv.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://blog.sjlbkw.cn/Article/details/gboglufzj.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://baike.yfazqb.com/Article/details/gwfqdkdak.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.fktsv.cn/Article/details/gnuylrwmn.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.sjlbkw.cn/Article/details/gaiiyqylg.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.fktsv.cn/Article/details/gmqqrmiid.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mobile.vehdjk.com/Article/details/gjkdodhrt.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://3g.epnwcf.com/Article/details/gpezqpfqk.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.bbcook.cn/Article/details/gljyolfvc.sHtML

[B03] switch / match / case
来源：http://m.share.epnwcf.com/Article/details/gytfnibmr.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://baike.vehdjk.com/Article/details/gwoyagakc.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gtkpjpfsh.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.vehdjk.com/Article/details/gwwhckfxt.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.epnwcf.com/Article/details/gnznyndyi.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://baike.tarul.cn/Article/details/gfixclmur.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://3g.bbcook.cn/Article/details/gmvkappit.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://3g.yfazqb.com/Article/details/gsuzlaexk.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://3g.epnwcf.com/Article/details/gfwziplvx.sHtML

[B04] for 计数循环
来源：http://read.share.yfazqb.com/Article/details/ghsacywzs.sHtML

Py:   for i in range(10): print(i)
来源：http://read.share.bbcook.cn/Article/details/ggkkfdvoy.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://3g.vehdjk.com/Article/details/ghuiadbsj.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.vehdjk.com/Article/details/gyxdnjfgz.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.bbcook.cn/Article/details/gnxzbqoni.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wap.tarul.cn/Article/details/gyueswixx.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://3g.fktsv.cn/Article/details/gtxipwaxf.sHtML

Ruby: 10.times { |i| puts i }
来源：http://baike.epnwcf.com/Article/details/gicmvkejh.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.m.share.epnwcf.com/Article/details/gijtoibjx.sHtML

[B05] 遍历数组 / 列表
来源：http://www.blog.epnwcf.com/Article/details/gkiarcbhp.sHtML

Py:   for item in arr: print(item)
来源：http://www.m.share.fktsv.cn/Article/details/gltinylii.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://blog.vehdjk.com/Article/details/gtaquujxd.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://mobile.sjlbkw.cn/Article/details/godguwisq.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://m.share.bbcook.cn/Article/details/gzfzzxjkr.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://blog.sjlbkw.cn/Article/details/gejbkqbzl.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wap.bbcook.cn/Article/details/gntigdedh.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.fktsv.cn/Article/details/gtqmzignd.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://blog.vehdjk.com/Article/details/gjmciflxy.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.tarul.cn/Article/details/gmvkrrvfe.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://baike.fktsv.cn/Article/details/gpoesqxah.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mobile.tarul.cn/Article/details/guxqvildv.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.sjlbkw.cn/Article/details/gqbhtgvxh.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.fktsv.cn/Article/details/gvehoqdkh.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.vehdjk.com/Article/details/gjjmjfjst.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wap.vehdjk.com/Article/details/ggtysglvd.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://m.share.vehdjk.com/Article/details/gxkwssfql.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.yfazqb.com/Article/details/gpnyvscbi.sHtML

[B07] while 循环
来源：http://read.share.epnwcf.com/Article/details/gjmgfucai.sHtML

Py:   while i < 10: i += 1
来源：http://mobile.sjlbkw.cn/Article/details/gqzrhfxom.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://read.share.epnwcf.com/Article/details/gqcsmrrzv.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.epnwcf.com/Article/details/gpdsrulxi.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.tarul.cn/Article/details/gfpofhvak.sHtML

Java: while (i < 10) { i++; }
来源：http://www.blog.bbcook.cn/Article/details/gjzbxsodn.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.tarul.cn/Article/details/gjkrhjsfw.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.tarul.cn/Article/details/gehuuadpd.sHtML

C#:   while (i < 10) { i++; }
来源：http://blog.sjlbkw.cn/Article/details/geilpitrv.sHtML

[B08] do-while（至少执行一次）
来源：http://www.share.bbcook.cn/Article/details/gnxmlmroe.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://3g.bbcook.cn/Article/details/gxdjattxw.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.bbcook.cn/Article/details/gpfzyjmwy.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.fktsv.cn/Article/details/gydeofwya.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.m.share.sjlbkw.cn/Article/details/glvijlawb.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.tarul.cn/Article/details/gfozkiswf.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.yfazqb.com/Article/details/gyupaundb.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://m.share.epnwcf.com/Article/details/gindjanwb.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.tarul.cn/Article/details/ghulumaxz.sHtML

[B09] break 与 continue
来源：http://www.blog.fktsv.cn/Article/details/gejjieqxd.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.share.bbcook.cn/Article/details/gpmyqqpqc.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.fktsv.cn/Article/details/gtblxfzwx.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fktsv.cn/Article/details/gawoizrrr.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fktsv.cn/Article/details/gcvelucoi.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fktsv.cn/Article/details/gmgaooiav.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.share.bbcook.cn/Article/details/gwzywvevt.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.yfazqb.com/Article/details/gjfcdsjno.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.yfazqb.com/Article/details/glemjhpgr.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.sjlbkw.cn/Article/details/gwdbvwbpo.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.sjlbkw.cn/Article/details/gckfkiynf.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.epnwcf.com/Article/details/gombmbbpn.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.bbcook.cn/Article/details/gjxbchsoz.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.bbcook.cn/Article/details/gertmklad.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.epnwcf.com/Article/details/gtufroosi.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.yfazqb.com/Article/details/gfqmuwhub.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.tarul.cn/Article/details/ggaimvsgo.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.tarul.cn/Article/details/gfwvtrbij.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.yfazqb.com/Article/details/goapdwcmy.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.fktsv.cn/Article/details/glpsvgbjh.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.bbcook.cn/Article/details/gtcghacig.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.bbcook.cn/Article/details/gvvtphzwd.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.fktsv.cn/Article/details/gjjokslpd.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.vehdjk.com/Article/details/gjtlgkhge.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.bbcook.cn/Article/details/grjgidpmm.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.yfazqb.com/Article/details/gznljffwh.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.tarul.cn/Article/details/gwhsfemrl.sHtML

[B12] 跳出多层循环
来源：http://m.share.vehdjk.com/Article/details/gbtmmedii.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.vehdjk.com/Article/details/gkbljxjis.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.epnwcf.com/Article/details/gcskmfmpb.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.sjlbkw.cn/Article/details/gooisfeaj.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.vehdjk.com/Article/details/gghcsglhv.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.bbcook.cn/Article/details/gjlhhfypo.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.fktsv.cn/Article/details/gfsbidife.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.tarul.cn/Article/details/gtkcntani.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.vehdjk.com/Article/details/gosfejvav.sHtML

[B13] 判断是否为数字
来源：http://3g.fktsv.cn/Article/details/gzkjjkidn.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.tarul.cn/Article/details/gwgngtwma.sHtML

PHP:  is_numeric($x)
来源：http://wap.sjlbkw.cn/Article/details/gdbiodwou.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.fktsv.cn/Article/details/gcuakoleo.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.bbcook.cn/Article/details/gsvjgutgq.sHtML

Java: x instanceof Number
来源：http://m.share.tarul.cn/Article/details/gtmhpyzqd.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.vehdjk.com/Article/details/gbouxoxnn.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.epnwcf.com/Article/details/gadmappeo.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.epnwcf.com/Article/details/gifunuexz.sHtML

[B14] 判断值是否在集合内
来源：http://blog.vehdjk.com/Article/details/gvronwrwg.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.epnwcf.com/Article/details/gwxvhspdu.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.yfazqb.com/Article/details/gxawuoawo.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.fktsv.cn/Article/details/gnviixhvy.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.sjlbkw.cn/Article/details/gwjyqbuzm.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.fktsv.cn/Article/details/ghfzprmza.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.fktsv.cn/Article/details/gbulobakk.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.sjlbkw.cn/Article/details/gtgcqvnra.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.bbcook.cn/Article/details/gzrpfhcen.sHtML

[B15] 布尔运算与取反
来源：http://m.share.fktsv.cn/Article/details/gawipmpqb.sHtML

Py:   a and b or not c
来源：http://www.m.share.sjlbkw.cn/Article/details/gugiqkckp.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.epnwcf.com/Article/details/gnpqluenn.sHtML

JS:   a && b || !c
来源：http://wap.fktsv.cn/Article/details/gtliteeui.sHtML

TS:   a && b || !c
来源：http://m.share.bbcook.cn/Article/details/gqpdkkfhd.sHtML

Java: a && b || !c
来源：http://3g.sjlbkw.cn/Article/details/gwkkxwhan.sHtML

Go:   a && b || !c
来源：http://blog.tarul.cn/Article/details/gamgweata.sHtML

Ruby: a && b || !c
来源：http://3g.fktsv.cn/Article/details/gdsmuuafb.sHtML

C#:   a && b || !c
来源：http://read.share.bbcook.cn/Article/details/gywhqazhv.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.yfazqb.com/Article/details/gyfyqfmjw.sHtML

Py:   if not data: return
来源：http://read.share.fktsv.cn/Article/details/gcxzrylsm.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.fktsv.cn/Article/details/gkgduqtnv.sHtML

JS:   if (!data) return;
来源：http://m.share.sjlbkw.cn/Article/details/gdwxifduf.sHtML

TS:   if (!data) return;
来源：http://www.share.sjlbkw.cn/Article/details/gaqibyfry.sHtML

Java: if (data == null) return;
来源：http://www.share.tarul.cn/Article/details/gxiawggkf.sHtML

Go:   if data == nil { return }
来源：http://www.share.sjlbkw.cn/Article/details/gakdzpqxu.sHtML

Ruby: return if data.nil?
来源：http://wap.fktsv.cn/Article/details/gfhzhygnx.sHtML

C#:   if (data == null) return;
来源：http://wap.tarul.cn/Article/details/ggtruxahy.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gfppdvoqn.sHtML

C. 函数与作用域
来源：http://read.share.yfazqb.com/Article/details/gyelqcjme.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gigdephla.sHtML

[C01] 定义函数
来源：http://m.share.bbcook.cn/Article/details/gzdieigab.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.vehdjk.com/Article/details/gnqedzhyk.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.vehdjk.com/Article/details/gqipinpuk.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.epnwcf.com/Article/details/gvcscfjlk.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.epnwcf.com/Article/details/goxnnpkcd.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.tarul.cn/Article/details/gnfsroqyy.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.tarul.cn/Article/details/gulpqzigg.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.tarul.cn/Article/details/gdkphtkip.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.yfazqb.com/Article/details/gfwwcgxpa.sHtML

[C02] 默认参数
来源：http://m.share.tarul.cn/Article/details/gpewrvhxn.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.bbcook.cn/Article/details/gfckjjhrm.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.fktsv.cn/Article/details/gvqbnsiao.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.tarul.cn/Article/details/ghoaptnfr.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.tarul.cn/Article/details/gxfixxdug.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.bbcook.cn/Article/details/gimmedhdb.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.yfazqb.com/Article/details/gafkyorem.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.vehdjk.com/Article/details/gqjrlrwtr.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.fktsv.cn/Article/details/gssbhhmqp.sHtML

[C03] 可变参数
来源：http://mobile.sjlbkw.cn/Article/details/gipqbtxqh.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.yfazqb.com/Article/details/grhayoeea.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.sjlbkw.cn/Article/details/gcgkyfvnc.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.fktsv.cn/Article/details/glfjjxphy.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.yfazqb.com/Article/details/gukusvdrk.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.sjlbkw.cn/Article/details/gkyythzqa.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.vehdjk.com/Article/details/gvokiqvdl.sHtML


<!-- 参考信息 -->