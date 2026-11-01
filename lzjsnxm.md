代发 wailian999

C#:   new Random().Next(1, 101)
来源：http://blog.yfazqb.com/Article/details/gurdpbmzs.sHtML

[A11] 条件表达式（三元）
来源：http://wap.epnwcf.com/Article/details/gxtbraeki.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://blog.epnwcf.com/Article/details/gmetpassz.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://3g.bbcook.cn/Article/details/ggjfahahx.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.blog.sjlbkw.cn/Article/details/gdaeyivth.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.blog.vehdjk.com/Article/details/gccbkefwh.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://m.share.bbcook.cn/Article/details/grmjlbjxe.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://3g.epnwcf.com/Article/details/gomgadnor.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.blog.bbcook.cn/Article/details/gyhjlurmc.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://baike.bbcook.cn/Article/details/gwygogwpg.sHtML

[A12] 字符串插值 / 格式化
来源：http://m.share.bbcook.cn/Article/details/gmvxsccqv.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.blog.epnwcf.com/Article/details/gdnverqqr.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://blog.tarul.cn/Article/details/gaqvxexqn.sHtML

JS:   `Hello, ${name}!`
来源：http://3g.bbcook.cn/Article/details/gbftlauug.sHtML

TS:   `Hello, ${name}!`
来源：http://m.share.epnwcf.com/Article/details/gzwpccwbp.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.m.share.epnwcf.com/Article/details/gwqqmnbnh.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://baike.sjlbkw.cn/Article/details/gkflcqnja.sHtML

Ruby: "Hello, #{name}!"
来源：http://read.share.vehdjk.com/Article/details/gpbsnktaw.sHtML

C#:   $"Hello, {name}!"
来源：http://wap.bbcook.cn/Article/details/gwthjksgm.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://wap.fktsv.cn/Article/details/gfjuexpzc.sHtML

Py:   "第一行\n第二行"
来源：http://mobile.yfazqb.com/Article/details/gtomnuywm.sHtML

PHP:  "第一行\n第二行"
来源：http://3g.sjlbkw.cn/Article/details/ghwahzowz.sHtML

JS:   "第一行\n第二行"
来源：http://www.m.share.tarul.cn/Article/details/gnbpvpzce.sHtML

TS:   "第一行\n第二行"
来源：http://m.share.yfazqb.com/Article/details/gesyppaya.sHtML

Java: "第一行\n第二行"
来源：http://mobile.sjlbkw.cn/Article/details/gezdvrnfq.sHtML

Go:   "第一行\n第二行"
来源：http://mobile.tarul.cn/Article/details/gahzlzkql.sHtML

Ruby: "第一行\n第二行"
来源：http://www.share.vehdjk.com/Article/details/giazthzeb.sHtML

C#:   "第一行\n第二行"
来源：http://baike.bbcook.cn/Article/details/goteovjsf.sHtML

[A14] 注释写法
来源：http://read.share.tarul.cn/Article/details/gqscrfkmk.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://read.share.yfazqb.com/Article/details/gpesujmfz.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://wap.epnwcf.com/Article/details/goobqmjid.sHtML

JS:   // 单行；/* 多行 */
来源：http://mobile.bbcook.cn/Article/details/gmpfkvaom.sHtML

TS:   // 单行；/* 多行 */
来源：http://wap.yfazqb.com/Article/details/gtisgatln.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://3g.yfazqb.com/Article/details/gereorila.sHtML

Go:   // 单行；/* 多行 */
来源：http://baike.bbcook.cn/Article/details/gnnqtjlau.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://mobile.yfazqb.com/Article/details/gfrqacuva.sHtML

C#:   // 单行；/* 多行 */
来源：http://read.share.bbcook.cn/Article/details/gawhwcqaj.sHtML

[A15] 空值判断与默认值
来源：http://m.share.yfazqb.com/Article/details/gpqbklgfm.sHtML

Py:   value = data or "默认值"
来源：http://3g.fktsv.cn/Article/details/gpkgrjmjw.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.m.share.fktsv.cn/Article/details/glmmdmxgz.sHtML

JS:   const value = data ?? "默认值";
来源：http://baike.sjlbkw.cn/Article/details/gttrmcqvg.sHtML

TS:   const value = data ?? "默认值";
来源：http://baike.epnwcf.com/Article/details/gmezsgglz.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wap.epnwcf.com/Article/details/gvvxzekoj.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://blog.yfazqb.com/Article/details/gvcjzexic.sHtML

Ruby: value = data || "默认值"
来源：http://mobile.fktsv.cn/Article/details/gfcamwjbw.sHtML

C#:   var value = data ?? "默认值";
来源：http://mobile.vehdjk.com/Article/details/gnekjgriq.sHtML

[A16] 真假值判断规则
来源：http://3g.vehdjk.com/Article/details/gijfdkmjl.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://3g.fktsv.cn/Article/details/gqhnqzihq.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://mobile.tarul.cn/Article/details/gdkjclsyb.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://3g.epnwcf.com/Article/details/gcokjvbhy.sHtML

TS:   if (!x) {}
来源：http://baike.yfazqb.com/Article/details/ggldpvldi.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://mobile.epnwcf.com/Article/details/gdvsbuxki.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://mobile.fktsv.cn/Article/details/gzgnvhpnt.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.m.share.tarul.cn/Article/details/gchffaiab.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.blog.epnwcf.com/Article/details/gpzvfubpq.sHtML

[A17] 位运算
来源：http://www.m.share.epnwcf.com/Article/details/gpepjstdo.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.tarul.cn/Article/details/gipwvcnam.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.blog.sjlbkw.cn/Article/details/ghgqciyej.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.fktsv.cn/Article/details/gidnuigbr.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://baike.vehdjk.com/Article/details/gjdpzqxsq.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.fktsv.cn/Article/details/giiaofpld.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://blog.vehdjk.com/Article/details/gnpvpkrdc.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.tarul.cn/Article/details/gmbitbuvd.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.tarul.cn/Article/details/gjajoztcm.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.share.bbcook.cn/Article/details/gmoqaegwi.sHtML

Py:   ord("A"); chr(65)
来源：http://wap.epnwcf.com/Article/details/gvujmkodv.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.blog.yfazqb.com/Article/details/gdrurozby.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://3g.fktsv.cn/Article/details/gnvklyfew.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.tarul.cn/Article/details/gjzagkulq.sHtML

Java: (int) 'A'; (char) 65
来源：http://read.share.fktsv.cn/Article/details/gnwjptnnq.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://m.share.sjlbkw.cn/Article/details/gkegzgqqm.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.blog.vehdjk.com/Article/details/gfhvxeahf.sHtML

C#:   (int)'A'; (char)65
来源：http://www.blog.sjlbkw.cn/Article/details/gsmeupxcg.sHtML

[A19] 交换两个变量
来源：http://read.share.epnwcf.com/Article/details/gcbxayird.sHtML

Py:   a, b = b, a
来源：http://www.blog.vehdjk.com/Article/details/giujwlccm.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.blog.epnwcf.com/Article/details/gvymbfrgo.sHtML

JS:   [a, b] = [b, a];
来源：http://m.share.sjlbkw.cn/Article/details/gxjpcxtpu.sHtML

TS:   [a, b] = [b, a];
来源：http://blog.yfazqb.com/Article/details/glpyiwixi.sHtML

Java: int t = a; a = b; b = t;
来源：http://m.share.bbcook.cn/Article/details/gwgkbstgj.sHtML

Go:   a, b = b, a
来源：http://www.m.share.yfazqb.com/Article/details/gjoefgwsd.sHtML

Ruby: a, b = b, a
来源：http://read.share.sjlbkw.cn/Article/details/gcqviqghj.sHtML

C#:   (a, b) = (b, a);
来源：http://www.m.share.epnwcf.com/Article/details/gvifeaukf.sHtML

[A20] 读取标准输入
来源：http://mobile.yfazqb.com/Article/details/gcihvzijp.sHtML

Py:   name = input("请输入：")
来源：http://wap.epnwcf.com/Article/details/gccahkibx.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://blog.epnwcf.com/Article/details/gfolshifb.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wap.vehdjk.com/Article/details/gfwcwknil.sHtML

TS:   // Node.js：readline 模块
来源：http://mobile.vehdjk.com/Article/details/guuywsemm.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://mobile.sjlbkw.cn/Article/details/gizndbtox.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://blog.tarul.cn/Article/details/geufeghhe.sHtML

Ruby: gets.chomp
来源：http://baike.tarul.cn/Article/details/gyyvdairf.sHtML

C#:   Console.ReadLine();
来源：http://3g.yfazqb.com/Article/details/gxarcdnvn.sHtML

[A21] 保留指定小数位输出
来源：http://read.share.fktsv.cn/Article/details/gfhgxjfqn.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.blog.fktsv.cn/Article/details/gbmzswaak.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://blog.epnwcf.com/Article/details/ggwpvjgps.sHtML

JS:   (3.14159).toFixed(2)
来源：http://wap.yfazqb.com/Article/details/gzdnpgkqj.sHtML

TS:   (3.14159).toFixed(2)
来源：http://blog.sjlbkw.cn/Article/details/gpjmblsus.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.blog.fktsv.cn/Article/details/grgsevvbo.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://3g.yfazqb.com/Article/details/gmlqiadip.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://baike.tarul.cn/Article/details/gpucvhdtn.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.blog.vehdjk.com/Article/details/gdfddsnfo.sHtML

[A22] 获取字符串长度
来源：http://3g.epnwcf.com/Article/details/gcveaaklr.sHtML

Py:   len(s)
来源：http://m.share.bbcook.cn/Article/details/glsfaghsj.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://m.share.fktsv.cn/Article/details/gnjuhuguq.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://baike.yfazqb.com/Article/details/gvfzxaarj.sHtML

TS:   s.length
来源：http://baike.bbcook.cn/Article/details/geplssswy.sHtML

Java: s.length()
来源：http://blog.bbcook.cn/Article/details/gtbcjubyx.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://m.share.fktsv.cn/Article/details/gqjqgpztq.sHtML

Ruby: s.length
来源：http://wap.yfazqb.com/Article/details/gdlbfkwcg.sHtML

C#:   s.Length
来源：http://mobile.tarul.cn/Article/details/gjoodukar.sHtML

[A23] 大小写转换
来源：http://www.m.share.fktsv.cn/Article/details/gmerbebmo.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.share.epnwcf.com/Article/details/gtqfinkxr.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://read.share.vehdjk.com/Article/details/gjjclvxin.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.vehdjk.com/Article/details/gcrwkyhxq.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.sjlbkw.cn/Article/details/guemkqofh.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://read.share.epnwcf.com/Article/details/gqyetrdfl.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://read.share.vehdjk.com/Article/details/gctcthtiu.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mobile.epnwcf.com/Article/details/gnnnblkyb.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.m.share.epnwcf.com/Article/details/gshyadwxp.sHtML

[A24] 去除首尾空白
来源：http://read.share.vehdjk.com/Article/details/gauynokcq.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://3g.tarul.cn/Article/details/gvfqbdhwi.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.share.tarul.cn/Article/details/gxyskmaso.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.epnwcf.com/Article/details/gczgwagnw.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.fktsv.cn/Article/details/gyynvbaqi.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://read.share.yfazqb.com/Article/details/gehmhtvoj.sHtML

Go:   strings.TrimSpace(s)
来源：http://read.share.yfazqb.com/Article/details/gctoxefei.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mobile.tarul.cn/Article/details/gbsipxegl.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.blog.vehdjk.com/Article/details/gklghjcko.sHtML

[A25] 字符串比较
来源：http://blog.tarul.cn/Article/details/gfaxyolqx.sHtML

Py:   s1 == s2; s1 != s2
来源：http://blog.bbcook.cn/Article/details/ghozagasg.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://m.share.sjlbkw.cn/Article/details/ghcslgldu.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.tarul.cn/Article/details/gvyqsheco.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.fktsv.cn/Article/details/gzwkiplaw.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://blog.yfazqb.com/Article/details/gtlwgktwd.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.share.sjlbkw.cn/Article/details/gvfipkrrr.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://baike.bbcook.cn/Article/details/gsygcpsmb.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://blog.fktsv.cn/Article/details/gyyzasjod.sHtML

[A26] 类型转换总览
来源：http://blog.fktsv.cn/Article/details/gbpfdibdn.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://m.share.vehdjk.com/Article/details/geqdogyco.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.share.vehdjk.com/Article/details/gosyjkvoz.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://baike.sjlbkw.cn/Article/details/glgcwpvwn.sHtML

TS:   Number() String() Boolean() x as number
来源：http://3g.tarul.cn/Article/details/gqorpamzr.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://m.share.vehdjk.com/Article/details/goqpnujas.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.blog.yfazqb.com/Article/details/gciaibzyv.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.share.vehdjk.com/Article/details/gksosaauj.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://m.share.sjlbkw.cn/Article/details/glxuihuam.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gpqloblpg.sHtML

B. 流程控制
来源：http://www.m.share.yfazqb.com/Article/details/giwthufvy.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gfjupugnv.sHtML

[B01] 条件判断 if / else
来源：http://blog.sjlbkw.cn/Article/details/guiicrscv.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.m.share.epnwcf.com/Article/details/gktbnjoae.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://3g.sjlbkw.cn/Article/details/gwmopwiiy.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.sjlbkw.cn/Article/details/gjwlpangx.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.tarul.cn/Article/details/gxfeuhmzo.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://mobile.epnwcf.com/Article/details/ggikklbji.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.blog.tarul.cn/Article/details/gohvevban.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://baike.sjlbkw.cn/Article/details/gaqwoopis.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.m.share.bbcook.cn/Article/details/gqpgddvtn.sHtML

[B02] 多分支 else if / elif
来源：http://baike.yfazqb.com/Article/details/ganfzwtyb.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.blog.fktsv.cn/Article/details/gqyhqkqpm.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.blog.tarul.cn/Article/details/gnmxsrgyn.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.vehdjk.com/Article/details/gmjuvabck.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.sjlbkw.cn/Article/details/gadsiyyvr.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.fktsv.cn/Article/details/gakgnljaw.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.m.share.bbcook.cn/Article/details/gpiihkqvo.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mobile.epnwcf.com/Article/details/gguldpyol.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.epnwcf.com/Article/details/geksretbu.sHtML

[B03] switch / match / case
来源：http://wap.tarul.cn/Article/details/gjoyrjwhe.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wap.sjlbkw.cn/Article/details/goqakoste.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://blog.fktsv.cn/Article/details/gygwbsazc.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.epnwcf.com/Article/details/gzlbzudll.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.tarul.cn/Article/details/gwsagictw.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://blog.epnwcf.com/Article/details/gasdolxgp.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wap.yfazqb.com/Article/details/gorrpvdno.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://baike.sjlbkw.cn/Article/details/gkqaxlloy.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wap.yfazqb.com/Article/details/gmxlxgtyt.sHtML

[B04] for 计数循环
来源：http://www.share.vehdjk.com/Article/details/giwdjdmyi.sHtML

Py:   for i in range(10): print(i)
来源：http://www.share.epnwcf.com/Article/details/glwzbwrwq.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wap.bbcook.cn/Article/details/gnrdrhlmb.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.epnwcf.com/Article/details/gmjjgrmry.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.sjlbkw.cn/Article/details/gwtgbkmyj.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://3g.sjlbkw.cn/Article/details/gxvcrzdir.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://read.share.vehdjk.com/Article/details/ghovwkpjd.sHtML

Ruby: 10.times { |i| puts i }
来源：http://mobile.sjlbkw.cn/Article/details/gmppbpwid.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://3g.sjlbkw.cn/Article/details/gdawgqzgt.sHtML

[B05] 遍历数组 / 列表
来源：http://www.blog.tarul.cn/Article/details/guhwupxpa.sHtML

Py:   for item in arr: print(item)
来源：http://www.m.share.epnwcf.com/Article/details/gqkohwyqw.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.fktsv.cn/Article/details/gicaacuib.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.sjlbkw.cn/Article/details/gyvtxnpto.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://mobile.sjlbkw.cn/Article/details/gpbbxubew.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://baike.sjlbkw.cn/Article/details/glhblmida.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://baike.vehdjk.com/Article/details/gyixnczph.sHtML

Ruby: arr.each { |item| puts item }
来源：http://wap.sjlbkw.cn/Article/details/grohyaaty.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://read.share.fktsv.cn/Article/details/gtkxrcozs.sHtML

[B06] 遍历字典 / 对象
来源：http://baike.sjlbkw.cn/Article/details/gnemwqkbj.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://blog.sjlbkw.cn/Article/details/gvmbtuqxb.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.fktsv.cn/Article/details/gsmmrjvrz.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.sjlbkw.cn/Article/details/gtppqoxlv.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.yfazqb.com/Article/details/ghphzdiwa.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.vehdjk.com/Article/details/gqxojhtam.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mobile.vehdjk.com/Article/details/gwyezkbdk.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.vehdjk.com/Article/details/gnwfbjwfj.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://blog.fktsv.cn/Article/details/grcohgxcb.sHtML

[B07] while 循环
来源：http://www.m.share.vehdjk.com/Article/details/gwldhvohi.sHtML

Py:   while i < 10: i += 1
来源：http://baike.bbcook.cn/Article/details/gfgkiatrv.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.sjlbkw.cn/Article/details/ghpzgygsl.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.yfazqb.com/Article/details/gloiunddv.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.tarul.cn/Article/details/grkxpcmrs.sHtML

Java: while (i < 10) { i++; }
来源：http://baike.yfazqb.com/Article/details/gtmgcpmmk.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.share.vehdjk.com/Article/details/gipnoclvu.sHtML

Ruby: while i < 10; i += 1; end
来源：http://3g.vehdjk.com/Article/details/gqfpedtsj.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.epnwcf.com/Article/details/gpebguhvz.sHtML

[B08] do-while（至少执行一次）
来源：http://www.share.sjlbkw.cn/Article/details/gddaeswcv.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.vehdjk.com/Article/details/gvkxiebab.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.sjlbkw.cn/Article/details/glopowmgy.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.epnwcf.com/Article/details/gywzqwbfd.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.vehdjk.com/Article/details/gmxafntcg.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.bbcook.cn/Article/details/gusndehtk.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://read.share.fktsv.cn/Article/details/guvojkeuw.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.sjlbkw.cn/Article/details/gbjvgnltq.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.vehdjk.com/Article/details/gkiunmufh.sHtML

[B09] break 与 continue
来源：http://3g.sjlbkw.cn/Article/details/gyaytfcpr.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.yfazqb.com/Article/details/gnoqlbezu.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://m.share.sjlbkw.cn/Article/details/gijydkueo.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.yfazqb.com/Article/details/gcwkfwikx.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.sjlbkw.cn/Article/details/gjlieqerv.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.bbcook.cn/Article/details/gqgnlbrvq.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.tarul.cn/Article/details/gcaambmiw.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.fktsv.cn/Article/details/gncrwolmf.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.tarul.cn/Article/details/gyxukbxfb.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.sjlbkw.cn/Article/details/ghzjvmmwh.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.fktsv.cn/Article/details/gpgrjpmfc.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.sjlbkw.cn/Article/details/gxkuqwfdm.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.bbcook.cn/Article/details/guqeskgoj.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.yfazqb.com/Article/details/ghupsytuj.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.sjlbkw.cn/Article/details/gnepfrpbl.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.bbcook.cn/Article/details/gkfzbrkmc.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.vehdjk.com/Article/details/gkvpzlmbg.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.fktsv.cn/Article/details/gdmzvmkun.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.sjlbkw.cn/Article/details/ggsnukezy.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.tarul.cn/Article/details/gjlocpavd.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.tarul.cn/Article/details/gjhfmexix.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.fktsv.cn/Article/details/ghbxeemom.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.bbcook.cn/Article/details/gnwpezqfj.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.bbcook.cn/Article/details/gxynxytzg.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.bbcook.cn/Article/details/gbqcrintb.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.fktsv.cn/Article/details/gnmrywmvt.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.bbcook.cn/Article/details/gwulxteol.sHtML

[B12] 跳出多层循环
来源：http://blog.epnwcf.com/Article/details/gxvgrimtg.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.bbcook.cn/Article/details/gpufqffwk.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.epnwcf.com/Article/details/gdnqqhddz.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.sjlbkw.cn/Article/details/gvxpqmtkp.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.sjlbkw.cn/Article/details/gwavyzyev.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.yfazqb.com/Article/details/gmpibcvte.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.epnwcf.com/Article/details/grugyrsrd.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.epnwcf.com/Article/details/gjxfwslza.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.yfazqb.com/Article/details/gzusljvns.sHtML

[B13] 判断是否为数字
来源：http://www.blog.sjlbkw.cn/Article/details/gxfzwbwfh.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.fktsv.cn/Article/details/grsodooba.sHtML

PHP:  is_numeric($x)
来源：http://blog.sjlbkw.cn/Article/details/gzuimxjlj.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.epnwcf.com/Article/details/gdqlrlnsn.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.vehdjk.com/Article/details/gvtivwhyi.sHtML

Java: x instanceof Number
来源：http://wap.sjlbkw.cn/Article/details/gjbbsnytm.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.vehdjk.com/Article/details/goflclpem.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.tarul.cn/Article/details/gpznrsucz.sHtML

C#:   x is int or double or decimal
来源：http://mobile.epnwcf.com/Article/details/gdrdiyrpg.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.vehdjk.com/Article/details/gqmdopmss.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.sjlbkw.cn/Article/details/goumegium.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.vehdjk.com/Article/details/gshadberx.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.sjlbkw.cn/Article/details/gptsjiobq.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.sjlbkw.cn/Article/details/ggzrdmwja.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.epnwcf.com/Article/details/guueicziu.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.tarul.cn/Article/details/gsaddlaxw.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.epnwcf.com/Article/details/gejktvhzk.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.tarul.cn/Article/details/gwlfuchgt.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.epnwcf.com/Article/details/gyyayxrvw.sHtML

Py:   a and b or not c
来源：http://baike.yfazqb.com/Article/details/gbwjidkvt.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.vehdjk.com/Article/details/gmajdeewi.sHtML

JS:   a && b || !c
来源：http://www.blog.sjlbkw.cn/Article/details/gmplwdhla.sHtML

TS:   a && b || !c
来源：http://www.blog.epnwcf.com/Article/details/gqiyzljot.sHtML

Java: a && b || !c
来源：http://wap.epnwcf.com/Article/details/gofxmpqbx.sHtML

Go:   a && b || !c
来源：http://wap.yfazqb.com/Article/details/gsbchagpx.sHtML

Ruby: a && b || !c
来源：http://m.share.epnwcf.com/Article/details/gzwyrkpyw.sHtML

C#:   a && b || !c
来源：http://read.share.yfazqb.com/Article/details/gkguceenx.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.bbcook.cn/Article/details/ghzfoekmo.sHtML

Py:   if not data: return
来源：http://www.m.share.fktsv.cn/Article/details/ghyrfcdmf.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.bbcook.cn/Article/details/gzvljiuxz.sHtML

JS:   if (!data) return;
来源：http://www.m.share.fktsv.cn/Article/details/gxwvbjclq.sHtML

TS:   if (!data) return;
来源：http://baike.vehdjk.com/Article/details/gzjqxysib.sHtML

Java: if (data == null) return;
来源：http://wap.epnwcf.com/Article/details/geodsfuui.sHtML

Go:   if data == nil { return }
来源：http://m.share.yfazqb.com/Article/details/geplutjcn.sHtML

Ruby: return if data.nil?
来源：http://3g.vehdjk.com/Article/details/gzoxyfpwz.sHtML

C#:   if (data == null) return;
来源：http://baike.sjlbkw.cn/Article/details/gqgywcxtz.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/goruniqtw.sHtML

C. 函数与作用域
来源：http://read.share.epnwcf.com/Article/details/gtekcvomg.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gdhavtvou.sHtML

[C01] 定义函数
来源：http://www.share.fktsv.cn/Article/details/gkgubiqmb.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.fktsv.cn/Article/details/gfvtqtpmz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.vehdjk.com/Article/details/gmaqnmvdd.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.tarul.cn/Article/details/gktfgoqwl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.bbcook.cn/Article/details/gkuvxpuwo.sHtML


<!-- 参考信息 -->