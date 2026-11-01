代发 wailian999

Py:   "第一行\n第二行"
来源：http://blog.sjlbkw.cn/Article/details/gmctqlylz.sHtML

PHP:  "第一行\n第二行"
来源：http://blog.vehdjk.com/Article/details/gcmtpvtup.sHtML

JS:   "第一行\n第二行"
来源：http://baike.bbcook.cn/Article/details/gqvayjgzs.sHtML

TS:   "第一行\n第二行"
来源：http://blog.epnwcf.com/Article/details/gwjybfgks.sHtML

Java: "第一行\n第二行"
来源：http://read.share.bbcook.cn/Article/details/guxuevksk.sHtML

Go:   "第一行\n第二行"
来源：http://www.share.bbcook.cn/Article/details/gvegiqkwr.sHtML

Ruby: "第一行\n第二行"
来源：http://m.share.bbcook.cn/Article/details/gvwlbkfdz.sHtML

C#:   "第一行\n第二行"
来源：http://m.share.sjlbkw.cn/Article/details/galanvtvv.sHtML

[A14] 注释写法
来源：http://m.share.tarul.cn/Article/details/gjknccdlv.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.share.bbcook.cn/Article/details/gjdwvdizw.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.m.share.tarul.cn/Article/details/gmgfdryey.sHtML

JS:   // 单行；/* 多行 */
来源：http://blog.epnwcf.com/Article/details/gpnpzticf.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.blog.epnwcf.com/Article/details/gujxuppym.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mobile.epnwcf.com/Article/details/gcgdqntpu.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.share.yfazqb.com/Article/details/gjxpvuqdp.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://m.share.vehdjk.com/Article/details/ghhnnxvzy.sHtML

C#:   // 单行；/* 多行 */
来源：http://read.share.bbcook.cn/Article/details/gepismhcn.sHtML

[A15] 空值判断与默认值
来源：http://www.m.share.tarul.cn/Article/details/gxipgzrkg.sHtML

Py:   value = data or "默认值"
来源：http://www.m.share.sjlbkw.cn/Article/details/ghsjukqlc.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.share.fktsv.cn/Article/details/glqhpjcwz.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.m.share.fktsv.cn/Article/details/gticnhcaq.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.blog.epnwcf.com/Article/details/gddojgnkj.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.blog.fktsv.cn/Article/details/gynurszew.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://mobile.epnwcf.com/Article/details/gvevosppx.sHtML

Ruby: value = data || "默认值"
来源：http://blog.tarul.cn/Article/details/gfjigjint.sHtML

C#:   var value = data ?? "默认值";
来源：http://wap.yfazqb.com/Article/details/gggmeqrtn.sHtML

[A16] 真假值判断规则
来源：http://read.share.tarul.cn/Article/details/grskufbxa.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.m.share.yfazqb.com/Article/details/gojjbttyu.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.blog.sjlbkw.cn/Article/details/gppkdwcol.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://3g.tarul.cn/Article/details/gfkogqoyc.sHtML

TS:   if (!x) {}
来源：http://mobile.sjlbkw.cn/Article/details/gaalptdrr.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://m.share.yfazqb.com/Article/details/gakvqpwha.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.m.share.epnwcf.com/Article/details/gwierxwbc.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.blog.yfazqb.com/Article/details/gbrebxfbu.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.m.share.fktsv.cn/Article/details/gzktoovet.sHtML

[A17] 位运算
来源：http://wap.vehdjk.com/Article/details/gxdlubsjw.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.bbcook.cn/Article/details/gpswnvrvr.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.blog.vehdjk.com/Article/details/gwyzaqdgk.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.bbcook.cn/Article/details/ginvnuvdq.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://3g.sjlbkw.cn/Article/details/gtufsntxt.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.sjlbkw.cn/Article/details/gvofrlqof.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.share.yfazqb.com/Article/details/gtjilixdc.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.epnwcf.com/Article/details/gqwpnmlla.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.vehdjk.com/Article/details/gtgdefahv.sHtML

[A18] 字符与 ASCII 码互转
来源：http://blog.bbcook.cn/Article/details/gsjkxprwr.sHtML

Py:   ord("A"); chr(65)
来源：http://baike.epnwcf.com/Article/details/gzybtsiye.sHtML

PHP:  ord("A"); chr(65)
来源：http://blog.tarul.cn/Article/details/gnjmcsenm.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://3g.yfazqb.com/Article/details/gacclxsrs.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.m.share.yfazqb.com/Article/details/gwwfansii.sHtML

Java: (int) 'A'; (char) 65
来源：http://blog.epnwcf.com/Article/details/ghiaklmsj.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.share.epnwcf.com/Article/details/gsnzdvrzz.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.share.tarul.cn/Article/details/gnxwmejsw.sHtML

C#:   (int)'A'; (char)65
来源：http://blog.bbcook.cn/Article/details/ghumhxqxw.sHtML

[A19] 交换两个变量
来源：http://baike.sjlbkw.cn/Article/details/gocfcjqhv.sHtML

Py:   a, b = b, a
来源：http://www.share.tarul.cn/Article/details/gxtasvulg.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://blog.bbcook.cn/Article/details/gffknvicy.sHtML

JS:   [a, b] = [b, a];
来源：http://baike.tarul.cn/Article/details/gpvwotbnh.sHtML

TS:   [a, b] = [b, a];
来源：http://www.blog.vehdjk.com/Article/details/gjixebloo.sHtML

Java: int t = a; a = b; b = t;
来源：http://3g.vehdjk.com/Article/details/gonygxwet.sHtML

Go:   a, b = b, a
来源：http://www.share.fktsv.cn/Article/details/gqqvvwwhq.sHtML

Ruby: a, b = b, a
来源：http://baike.fktsv.cn/Article/details/gvihznnpl.sHtML

C#:   (a, b) = (b, a);
来源：http://www.blog.tarul.cn/Article/details/gmbmpgsha.sHtML

[A20] 读取标准输入
来源：http://www.m.share.yfazqb.com/Article/details/gwpybrldu.sHtML

Py:   name = input("请输入：")
来源：http://wap.yfazqb.com/Article/details/geakvzmct.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://mobile.fktsv.cn/Article/details/gkvxmqcxs.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.m.share.yfazqb.com/Article/details/gygmoixux.sHtML

TS:   // Node.js：readline 模块
来源：http://www.m.share.bbcook.cn/Article/details/gkggbpawq.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.m.share.tarul.cn/Article/details/gqpmwvarv.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://mobile.vehdjk.com/Article/details/ggduvxfrb.sHtML

Ruby: gets.chomp
来源：http://3g.vehdjk.com/Article/details/gvgnxxoxk.sHtML

C#:   Console.ReadLine();
来源：http://mobile.sjlbkw.cn/Article/details/gujtjodhh.sHtML

[A21] 保留指定小数位输出
来源：http://3g.bbcook.cn/Article/details/gfssebast.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.blog.vehdjk.com/Article/details/gxgbodlbn.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://blog.fktsv.cn/Article/details/ghzvijfrc.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.blog.fktsv.cn/Article/details/grrbjgdai.sHtML

TS:   (3.14159).toFixed(2)
来源：http://blog.yfazqb.com/Article/details/gjaetqyva.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://baike.fktsv.cn/Article/details/gvgnutklx.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://3g.bbcook.cn/Article/details/gjifzpsuu.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.blog.fktsv.cn/Article/details/gwpsshmbt.sHtML

C#:   3.14159.ToString("F2")
来源：http://mobile.bbcook.cn/Article/details/gmbtkptkp.sHtML

[A22] 获取字符串长度
来源：http://m.share.yfazqb.com/Article/details/gamildbaz.sHtML

Py:   len(s)
来源：http://m.share.sjlbkw.cn/Article/details/ggxzbekga.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://m.share.tarul.cn/Article/details/ggnhggies.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wap.epnwcf.com/Article/details/gsmwrcimh.sHtML

TS:   s.length
来源：http://m.share.yfazqb.com/Article/details/gacabrtwz.sHtML

Java: s.length()
来源：http://3g.yfazqb.com/Article/details/gbxnbfkbb.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://read.share.sjlbkw.cn/Article/details/gmdyoaokk.sHtML

Ruby: s.length
来源：http://wap.tarul.cn/Article/details/gfgxcjeqf.sHtML

C#:   s.Length
来源：http://www.m.share.bbcook.cn/Article/details/gfeeoyolq.sHtML

[A23] 大小写转换
来源：http://www.blog.yfazqb.com/Article/details/ggkwwerkx.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://blog.vehdjk.com/Article/details/gptahlqtn.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://blog.sjlbkw.cn/Article/details/gyynmsqed.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.yfazqb.com/Article/details/gefupgpcs.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.yfazqb.com/Article/details/gjgdovomt.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://read.share.tarul.cn/Article/details/gcqjcndmu.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.blog.epnwcf.com/Article/details/gobyawnhy.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://m.share.vehdjk.com/Article/details/gkkctsjam.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://baike.epnwcf.com/Article/details/gnieywhrz.sHtML

[A24] 去除首尾空白
来源：http://read.share.fktsv.cn/Article/details/gluaopncm.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wap.sjlbkw.cn/Article/details/geoeakkbb.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.blog.tarul.cn/Article/details/gawtaxvem.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.tarul.cn/Article/details/gofisoxrr.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.sjlbkw.cn/Article/details/guodczjqr.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.share.bbcook.cn/Article/details/gxzibmcai.sHtML

Go:   strings.TrimSpace(s)
来源：http://blog.yfazqb.com/Article/details/gcftpedii.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.m.share.sjlbkw.cn/Article/details/grdrzzxzs.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://blog.fktsv.cn/Article/details/gndukybrx.sHtML

[A25] 字符串比较
来源：http://www.m.share.tarul.cn/Article/details/gvtrzijsr.sHtML

Py:   s1 == s2; s1 != s2
来源：http://wap.epnwcf.com/Article/details/gimcgyhuo.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://read.share.epnwcf.com/Article/details/gjueplwwv.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.epnwcf.com/Article/details/gkpdpekgd.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.fktsv.cn/Article/details/gkxxlolub.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.blog.yfazqb.com/Article/details/gsqktfqdl.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.share.vehdjk.com/Article/details/gpgtsjfwb.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://wap.epnwcf.com/Article/details/gaczfqekm.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqaruvttt.sHtML

[A26] 类型转换总览
来源：http://www.m.share.fktsv.cn/Article/details/gqslotaot.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://baike.epnwcf.com/Article/details/gssvthorj.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://baike.bbcook.cn/Article/details/grptuzddm.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://3g.bbcook.cn/Article/details/gnoeyeuct.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.m.share.bbcook.cn/Article/details/gnjztwext.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.share.vehdjk.com/Article/details/glshwhvaq.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://baike.sjlbkw.cn/Article/details/guyunvhie.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.m.share.epnwcf.com/Article/details/gdvhmqqhg.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wap.yfazqb.com/Article/details/gmrqkwebc.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gssorfqoa.sHtML

B. 流程控制
来源：http://3g.sjlbkw.cn/Article/details/gfnppfzoc.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gbrzaqppn.sHtML

[B01] 条件判断 if / else
来源：http://m.share.epnwcf.com/Article/details/glngfmcio.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://blog.epnwcf.com/Article/details/gdhtkvemf.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wap.fktsv.cn/Article/details/gtjqubppb.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.bbcook.cn/Article/details/gruxtzbsm.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.epnwcf.com/Article/details/ggeflbibv.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.m.share.yfazqb.com/Article/details/gtxovsnxp.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.share.fktsv.cn/Article/details/gmylygjio.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://baike.yfazqb.com/Article/details/gkfnafija.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://blog.bbcook.cn/Article/details/gkjdxvxtr.sHtML

[B02] 多分支 else if / elif
来源：http://blog.sjlbkw.cn/Article/details/gszdxxdej.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://baike.vehdjk.com/Article/details/gegkxospu.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wap.tarul.cn/Article/details/gclwkupyp.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.vehdjk.com/Article/details/gbwrggqfc.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.epnwcf.com/Article/details/gnalxrypo.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.tarul.cn/Article/details/grxbxnywf.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://read.share.fktsv.cn/Article/details/gesqgwlch.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://read.share.fktsv.cn/Article/details/giaimguoc.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.vehdjk.com/Article/details/gldipszqd.sHtML

[B03] switch / match / case
来源：http://www.blog.tarul.cn/Article/details/gicnmfiee.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.share.fktsv.cn/Article/details/gbetnmmlo.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://blog.vehdjk.com/Article/details/gelhmcxlf.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.tarul.cn/Article/details/gnixdfwdw.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.tarul.cn/Article/details/ggcdgonah.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://m.share.epnwcf.com/Article/details/glqbuvrnp.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wap.epnwcf.com/Article/details/gagrrhgsg.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://blog.vehdjk.com/Article/details/gxiczbvyo.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://3g.bbcook.cn/Article/details/gbliwaqde.sHtML

[B04] for 计数循环
来源：http://wap.yfazqb.com/Article/details/gogiqvydp.sHtML

Py:   for i in range(10): print(i)
来源：http://3g.yfazqb.com/Article/details/ghdgilmea.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://read.share.yfazqb.com/Article/details/ghwvvdret.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.bbcook.cn/Article/details/gdgdbxrsk.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.bbcook.cn/Article/details/gdoiqbyoa.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://3g.fktsv.cn/Article/details/gcfyrexam.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.vehdjk.com/Article/details/gcdstetgl.sHtML

Ruby: 10.times { |i| puts i }
来源：http://3g.vehdjk.com/Article/details/gwjghjwnw.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.share.sjlbkw.cn/Article/details/gfvrdwflh.sHtML

[B05] 遍历数组 / 列表
来源：http://www.share.epnwcf.com/Article/details/ggsvgtftw.sHtML

Py:   for item in arr: print(item)
来源：http://baike.fktsv.cn/Article/details/gqhllliqx.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.m.share.vehdjk.com/Article/details/gladuemnf.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://read.share.bbcook.cn/Article/details/gezrwpizq.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.tarul.cn/Article/details/gtyyuojwi.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://read.share.sjlbkw.cn/Article/details/grancadzl.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://3g.bbcook.cn/Article/details/gdulaoxqm.sHtML

Ruby: arr.each { |item| puts item }
来源：http://m.share.fktsv.cn/Article/details/glxekiwng.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://read.share.bbcook.cn/Article/details/ggbkwumpf.sHtML

[B06] 遍历字典 / 对象
来源：http://blog.epnwcf.com/Article/details/gqbpiigab.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.yfazqb.com/Article/details/gkeuhgfhw.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://m.share.fktsv.cn/Article/details/gdhnrfndv.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.sjlbkw.cn/Article/details/gofkojnbk.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.epnwcf.com/Article/details/gwghknbae.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.blog.yfazqb.com/Article/details/gyvtnicht.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.fktsv.cn/Article/details/gylxynmng.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://blog.epnwcf.com/Article/details/ggmhnlrpa.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://blog.bbcook.cn/Article/details/gbsqyabtc.sHtML

[B07] while 循环
来源：http://www.blog.tarul.cn/Article/details/gtlekpsnj.sHtML

Py:   while i < 10: i += 1
来源：http://mobile.bbcook.cn/Article/details/gphyhslgh.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.blog.epnwcf.com/Article/details/gpdokyaxi.sHtML

JS:   while (i < 10) { i++; }
来源：http://3g.vehdjk.com/Article/details/gabcbkahr.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.sjlbkw.cn/Article/details/gxzwgbuyf.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.vehdjk.com/Article/details/gcfpfmusp.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.epnwcf.com/Article/details/gdvvzcumn.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.sjlbkw.cn/Article/details/geshnspaj.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.sjlbkw.cn/Article/details/gpwfazxkl.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.vehdjk.com/Article/details/gzcfopuqo.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://3g.vehdjk.com/Article/details/ggdoitnds.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.bbcook.cn/Article/details/gwqpwqniq.sHtML

JS:   do { i++; } while (i < 10);
来源：http://m.share.epnwcf.com/Article/details/gpgbmbeol.sHtML

TS:   do { i++; } while (i < 10);
来源：http://3g.sjlbkw.cn/Article/details/gqmenkgas.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.tarul.cn/Article/details/geectwcrz.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.yfazqb.com/Article/details/gcibtzqwn.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.yfazqb.com/Article/details/gmmimymci.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.tarul.cn/Article/details/gyvxzuvpx.sHtML

[B09] break 与 continue
来源：http://www.blog.vehdjk.com/Article/details/gigbujuxo.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.tarul.cn/Article/details/glsnshajv.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.epnwcf.com/Article/details/gkghwgjsk.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.sjlbkw.cn/Article/details/grcxwexfd.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.epnwcf.com/Article/details/gezhzwooq.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.yfazqb.com/Article/details/gwcsvzpwy.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.fktsv.cn/Article/details/gkyvsjdhc.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.tarul.cn/Article/details/gpjgpjexj.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.epnwcf.com/Article/details/gjhglptsn.sHtML

[B10] 遍历同时拿索引
来源：http://wap.yfazqb.com/Article/details/glomkdkub.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.fktsv.cn/Article/details/gnchndqba.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.vehdjk.com/Article/details/gbcklusls.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.sjlbkw.cn/Article/details/guyqludse.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.tarul.cn/Article/details/gzavjkjev.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.sjlbkw.cn/Article/details/gvcylcswc.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.tarul.cn/Article/details/gvxevgmht.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.sjlbkw.cn/Article/details/geekdrfxg.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.vehdjk.com/Article/details/gjcmronbt.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.bbcook.cn/Article/details/gojvcbsoh.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.bbcook.cn/Article/details/gmfqmeapv.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.vehdjk.com/Article/details/gvajqcjio.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.tarul.cn/Article/details/gkymyfjjb.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.tarul.cn/Article/details/gnqknahua.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.tarul.cn/Article/details/gdurmdnap.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.tarul.cn/Article/details/guguqkehn.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.fktsv.cn/Article/details/gfshyybul.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.tarul.cn/Article/details/gfjmsxhsm.sHtML

[B12] 跳出多层循环
来源：http://read.share.bbcook.cn/Article/details/giiajqvzt.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.tarul.cn/Article/details/giqabmfbf.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.sjlbkw.cn/Article/details/gkahrqbfb.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.tarul.cn/Article/details/gcsyeqrxc.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.fktsv.cn/Article/details/gnlksmkkd.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.vehdjk.com/Article/details/gfqtpcvgw.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.bbcook.cn/Article/details/gxlhqcbji.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.epnwcf.com/Article/details/gyvwnzoom.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.vehdjk.com/Article/details/gacpbmwxd.sHtML

[B13] 判断是否为数字
来源：http://wap.fktsv.cn/Article/details/gmfkbalhe.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.epnwcf.com/Article/details/gecogceyq.sHtML

PHP:  is_numeric($x)
来源：http://read.share.fktsv.cn/Article/details/gbfhnslhm.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.epnwcf.com/Article/details/gswzwsfdi.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.vehdjk.com/Article/details/gkzegwwsz.sHtML

Java: x instanceof Number
来源：http://mobile.tarul.cn/Article/details/grojirjmk.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.yfazqb.com/Article/details/gzezeytaa.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.sjlbkw.cn/Article/details/gmpigrisz.sHtML

C#:   x is int or double or decimal
来源：http://mobile.bbcook.cn/Article/details/gaeumxibk.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.tarul.cn/Article/details/gopyfsjvp.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.sjlbkw.cn/Article/details/gdhableac.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.vehdjk.com/Article/details/gnklfzhzv.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.sjlbkw.cn/Article/details/ggsfmzkbc.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gakdvvpml.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.sjlbkw.cn/Article/details/gnqptnbpp.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.bbcook.cn/Article/details/gttvqzzwc.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.vehdjk.com/Article/details/gailsobze.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.yfazqb.com/Article/details/gnvekpbsw.sHtML

[B15] 布尔运算与取反
来源：http://baike.yfazqb.com/Article/details/geitsavos.sHtML

Py:   a and b or not c
来源：http://read.share.fktsv.cn/Article/details/gxaextcyu.sHtML

PHP:  $a && $b || !$c
来源：http://baike.yfazqb.com/Article/details/guakdltgu.sHtML

JS:   a && b || !c
来源：http://read.share.tarul.cn/Article/details/gimrtewrf.sHtML

TS:   a && b || !c
来源：http://m.share.vehdjk.com/Article/details/gwqnxsgxy.sHtML

Java: a && b || !c
来源：http://read.share.tarul.cn/Article/details/gnhebjudu.sHtML

Go:   a && b || !c
来源：http://www.m.share.fktsv.cn/Article/details/gktxpknck.sHtML

Ruby: a && b || !c
来源：http://3g.epnwcf.com/Article/details/gjleghjim.sHtML

C#:   a && b || !c
来源：http://blog.yfazqb.com/Article/details/gypauubwc.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.epnwcf.com/Article/details/gkfkhsboq.sHtML

Py:   if not data: return
来源：http://blog.epnwcf.com/Article/details/gzixjaeyb.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.tarul.cn/Article/details/gksplocay.sHtML

JS:   if (!data) return;
来源：http://www.m.share.sjlbkw.cn/Article/details/gcdrffllb.sHtML

TS:   if (!data) return;
来源：http://www.share.bbcook.cn/Article/details/glpveevne.sHtML

Java: if (data == null) return;
来源：http://wap.fktsv.cn/Article/details/gydewafuo.sHtML

Go:   if data == nil { return }
来源：http://blog.bbcook.cn/Article/details/gtszgnyik.sHtML

Ruby: return if data.nil?
来源：http://m.share.epnwcf.com/Article/details/gajxekngc.sHtML

C#:   if (data == null) return;
来源：http://www.share.bbcook.cn/Article/details/gsqsqopss.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gxaygqobu.sHtML

C. 函数与作用域
来源：http://blog.yfazqb.com/Article/details/gxiilpptt.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gehqdiovq.sHtML

[C01] 定义函数
来源：http://m.share.tarul.cn/Article/details/gladleyzs.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.yfazqb.com/Article/details/ghpxbfcqo.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.sjlbkw.cn/Article/details/ggphyovuf.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.yfazqb.com/Article/details/gvynxpcbh.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.vehdjk.com/Article/details/gmtcyaowy.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.fktsv.cn/Article/details/gnwgvyuea.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.yfazqb.com/Article/details/gedoexcoa.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.fktsv.cn/Article/details/gcjbyklcg.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.vehdjk.com/Article/details/gwrckhwsy.sHtML

[C02] 默认参数
来源：http://mobile.epnwcf.com/Article/details/gsehpxook.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.yfazqb.com/Article/details/gduymvxwe.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.sjlbkw.cn/Article/details/gtljzhsuk.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.bbcook.cn/Article/details/gbbqrjdqn.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.fktsv.cn/Article/details/geueypbea.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.vehdjk.com/Article/details/gtbsieqvz.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.sjlbkw.cn/Article/details/gwayaaozy.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.yfazqb.com/Article/details/gisdsbriu.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.fktsv.cn/Article/details/gfwghbdct.sHtML

[C03] 可变参数
来源：http://read.share.sjlbkw.cn/Article/details/gjlosifzf.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.fktsv.cn/Article/details/ggvegbfpx.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.vehdjk.com/Article/details/gzfmsdwtp.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.yfazqb.com/Article/details/gcjujdpjw.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.bbcook.cn/Article/details/gqpakappw.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.sjlbkw.cn/Article/details/gosmhnzju.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.sjlbkw.cn/Article/details/gkhitojzn.sHtML


<!-- 参考信息 -->