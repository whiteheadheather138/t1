代发 wailian999

Java: Math.abs(-5); Math.max(1, 2)
来源：http://baike.tarul.cn/Article/details/gwqslljlc.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.m.share.epnwcf.com/Article/details/gsyiotlll.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wap.epnwcf.com/Article/details/gejsiowev.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://m.share.vehdjk.com/Article/details/gzliialtc.sHtML

[A10] 生成随机数
来源：http://www.blog.vehdjk.com/Article/details/guhvabnrb.sHtML

Py:   import random; random.randint(1, 100)
来源：http://m.share.vehdjk.com/Article/details/gqxiholgs.sHtML

PHP:  random_int(1, 100);
来源：http://read.share.tarul.cn/Article/details/gibocpfnf.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.epnwcf.com/Article/details/gmmauntkb.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.tarul.cn/Article/details/gvxxxlqto.sHtML

Java: new Random().nextInt(100) + 1
来源：http://read.share.tarul.cn/Article/details/gsgbnbyag.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://m.share.vehdjk.com/Article/details/gfsvouyod.sHtML

Ruby: rand(1..100)
来源：http://www.blog.bbcook.cn/Article/details/gavvdvasu.sHtML

C#:   new Random().Next(1, 101)
来源：http://blog.vehdjk.com/Article/details/gbdtzdcub.sHtML

[A11] 条件表达式（三元）
来源：http://read.share.epnwcf.com/Article/details/gjjmncnkd.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://read.share.yfazqb.com/Article/details/gsnspwmld.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.blog.fktsv.cn/Article/details/grkeoybmk.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://m.share.vehdjk.com/Article/details/gtwbloepy.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://wap.yfazqb.com/Article/details/gdpqrmfjt.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://m.share.sjlbkw.cn/Article/details/gechwrwap.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://read.share.bbcook.cn/Article/details/gjmeoyfhw.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://mobile.epnwcf.com/Article/details/gatconstw.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://read.share.vehdjk.com/Article/details/gqpcrdxsy.sHtML

[A12] 字符串插值 / 格式化
来源：http://read.share.vehdjk.com/Article/details/gksvscdmf.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.blog.yfazqb.com/Article/details/ggnigubwo.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.share.bbcook.cn/Article/details/gzzzwyass.sHtML

JS:   `Hello, ${name}!`
来源：http://m.share.tarul.cn/Article/details/gecysyxeg.sHtML

TS:   `Hello, ${name}!`
来源：http://mobile.sjlbkw.cn/Article/details/ghiitwlup.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.m.share.tarul.cn/Article/details/gcoordlrb.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://m.share.yfazqb.com/Article/details/gqroeuaqk.sHtML

Ruby: "Hello, #{name}!"
来源：http://wap.sjlbkw.cn/Article/details/glxzcwajh.sHtML

C#:   $"Hello, {name}!"
来源：http://3g.sjlbkw.cn/Article/details/ggwwcbnfu.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.m.share.yfazqb.com/Article/details/gzurqamwa.sHtML

Py:   "第一行\n第二行"
来源：http://www.blog.vehdjk.com/Article/details/gcqtgypub.sHtML

PHP:  "第一行\n第二行"
来源：http://m.share.fktsv.cn/Article/details/gakukhkot.sHtML

JS:   "第一行\n第二行"
来源：http://www.share.bbcook.cn/Article/details/gjwytzlla.sHtML

TS:   "第一行\n第二行"
来源：http://3g.sjlbkw.cn/Article/details/gwmsjeemg.sHtML

Java: "第一行\n第二行"
来源：http://www.m.share.epnwcf.com/Article/details/gonxrwahn.sHtML

Go:   "第一行\n第二行"
来源：http://3g.epnwcf.com/Article/details/giqztvyzx.sHtML

Ruby: "第一行\n第二行"
来源：http://baike.fktsv.cn/Article/details/gxqjmrfzq.sHtML

C#:   "第一行\n第二行"
来源：http://www.blog.yfazqb.com/Article/details/gpbxqaasd.sHtML

[A14] 注释写法
来源：http://baike.tarul.cn/Article/details/graajmyxu.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.blog.yfazqb.com/Article/details/ggspqvvmu.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.share.vehdjk.com/Article/details/gklvudwvv.sHtML

JS:   // 单行；/* 多行 */
来源：http://baike.vehdjk.com/Article/details/gjmegoirb.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.m.share.vehdjk.com/Article/details/gpesajwax.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mobile.sjlbkw.cn/Article/details/ghnpjlclv.sHtML

Go:   // 单行；/* 多行 */
来源：http://wap.fktsv.cn/Article/details/gdbodizix.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://baike.epnwcf.com/Article/details/gmhnzgudr.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.share.epnwcf.com/Article/details/gumkojjzo.sHtML

[A15] 空值判断与默认值
来源：http://www.blog.bbcook.cn/Article/details/gazemttnj.sHtML

Py:   value = data or "默认值"
来源：http://m.share.fktsv.cn/Article/details/giuvvtian.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://mobile.bbcook.cn/Article/details/gezwmyeoq.sHtML

JS:   const value = data ?? "默认值";
来源：http://wap.sjlbkw.cn/Article/details/gedsnrgpd.sHtML

TS:   const value = data ?? "默认值";
来源：http://wap.yfazqb.com/Article/details/gldrxfcdo.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://mobile.epnwcf.com/Article/details/gwkegivuq.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://mobile.bbcook.cn/Article/details/gmhcphzps.sHtML

Ruby: value = data || "默认值"
来源：http://3g.bbcook.cn/Article/details/gxuhchers.sHtML

C#:   var value = data ?? "默认值";
来源：http://mobile.bbcook.cn/Article/details/gikajgchr.sHtML

[A16] 真假值判断规则
来源：http://wap.sjlbkw.cn/Article/details/gpoqkrxuj.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://baike.sjlbkw.cn/Article/details/gxwuemris.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://wap.fktsv.cn/Article/details/gincxofdx.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.blog.sjlbkw.cn/Article/details/gaqkynzlb.sHtML

TS:   if (!x) {}
来源：http://baike.epnwcf.com/Article/details/gozoztmzk.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://m.share.sjlbkw.cn/Article/details/grcqgjccx.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://read.share.epnwcf.com/Article/details/gmroyaaan.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://wap.vehdjk.com/Article/details/gnzeejlss.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.share.epnwcf.com/Article/details/gzrkkojzm.sHtML

[A17] 位运算
来源：http://m.share.fktsv.cn/Article/details/gznxyvnzw.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.epnwcf.com/Article/details/gwfjxhgsp.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mobile.epnwcf.com/Article/details/glbhrresy.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.sjlbkw.cn/Article/details/gdnlrjfyr.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://m.share.tarul.cn/Article/details/gonslmndn.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.epnwcf.com/Article/details/gofxotlni.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://mobile.fktsv.cn/Article/details/ggtgensvy.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.tarul.cn/Article/details/garnambir.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.bbcook.cn/Article/details/gkahbmouf.sHtML

[A18] 字符与 ASCII 码互转
来源：http://read.share.sjlbkw.cn/Article/details/gisdzcvwm.sHtML

Py:   ord("A"); chr(65)
来源：http://baike.yfazqb.com/Article/details/glqnjeeig.sHtML

PHP:  ord("A"); chr(65)
来源：http://mobile.yfazqb.com/Article/details/gwnzihvfk.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.fktsv.cn/Article/details/gxvvmtbaz.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.epnwcf.com/Article/details/gdsdvdrmw.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.blog.vehdjk.com/Article/details/gmzmmgcgo.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mobile.yfazqb.com/Article/details/gldanlhna.sHtML

Ruby: "A".ord; 65.chr
来源：http://baike.fktsv.cn/Article/details/gagtbmzjg.sHtML

C#:   (int)'A'; (char)65
来源：http://baike.epnwcf.com/Article/details/gszlkhbqb.sHtML

[A19] 交换两个变量
来源：http://www.blog.yfazqb.com/Article/details/gusmwjqrz.sHtML

Py:   a, b = b, a
来源：http://mobile.vehdjk.com/Article/details/gnqyjuffp.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://3g.tarul.cn/Article/details/gxrgcezjs.sHtML

JS:   [a, b] = [b, a];
来源：http://m.share.vehdjk.com/Article/details/ghdjiapak.sHtML

TS:   [a, b] = [b, a];
来源：http://3g.vehdjk.com/Article/details/gygpoebbt.sHtML

Java: int t = a; a = b; b = t;
来源：http://read.share.vehdjk.com/Article/details/gvdbqyein.sHtML

Go:   a, b = b, a
来源：http://3g.yfazqb.com/Article/details/gplqmaoeo.sHtML

Ruby: a, b = b, a
来源：http://mobile.fktsv.cn/Article/details/gsdrqiigc.sHtML

C#:   (a, b) = (b, a);
来源：http://read.share.yfazqb.com/Article/details/gtrdnluqk.sHtML

[A20] 读取标准输入
来源：http://mobile.epnwcf.com/Article/details/glnjrvugl.sHtML

Py:   name = input("请输入：")
来源：http://mobile.bbcook.cn/Article/details/gdkunvjvf.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://baike.vehdjk.com/Article/details/gixdhdaln.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://baike.yfazqb.com/Article/details/gixvoozwa.sHtML

TS:   // Node.js：readline 模块
来源：http://www.blog.vehdjk.com/Article/details/gtxxpnlki.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://blog.tarul.cn/Article/details/gsjgenxek.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://baike.sjlbkw.cn/Article/details/gwcplzjij.sHtML

Ruby: gets.chomp
来源：http://www.blog.yfazqb.com/Article/details/geneujdvq.sHtML

C#:   Console.ReadLine();
来源：http://read.share.tarul.cn/Article/details/gsumwbvuv.sHtML

[A21] 保留指定小数位输出
来源：http://3g.epnwcf.com/Article/details/ggznecdiu.sHtML

Py:   f"{3.14159:.2f}"
来源：http://wap.yfazqb.com/Article/details/gdcitzhsg.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://m.share.vehdjk.com/Article/details/gkdgdfbgb.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.blog.vehdjk.com/Article/details/gklugrumm.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.share.tarul.cn/Article/details/gkhdsgoyl.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://read.share.sjlbkw.cn/Article/details/ghkrhhndm.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://m.share.epnwcf.com/Article/details/gtbohavub.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://mobile.fktsv.cn/Article/details/gnbqxosdq.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.share.tarul.cn/Article/details/geovgmavg.sHtML

[A22] 获取字符串长度
来源：http://baike.yfazqb.com/Article/details/gjkthutny.sHtML

Py:   len(s)
来源：http://blog.tarul.cn/Article/details/gbhhamhkk.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.blog.bbcook.cn/Article/details/gbzyxbwlf.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://blog.epnwcf.com/Article/details/gzfbsygty.sHtML

TS:   s.length
来源：http://wap.tarul.cn/Article/details/gyziuwjqt.sHtML

Java: s.length()
来源：http://baike.yfazqb.com/Article/details/golytlpag.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.share.fktsv.cn/Article/details/gvxogizfn.sHtML

Ruby: s.length
来源：http://wap.yfazqb.com/Article/details/gtqqqwrcz.sHtML

C#:   s.Length
来源：http://www.m.share.tarul.cn/Article/details/gyelmzxcl.sHtML

[A23] 大小写转换
来源：http://mobile.fktsv.cn/Article/details/gzwfmoxlg.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://3g.tarul.cn/Article/details/gmgxiigam.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://blog.vehdjk.com/Article/details/glsmgboll.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.bbcook.cn/Article/details/guojtwdqp.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.tarul.cn/Article/details/gvwcufnpy.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://baike.epnwcf.com/Article/details/gxyodocuz.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://read.share.vehdjk.com/Article/details/gbqdbgliw.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://read.share.tarul.cn/Article/details/gmjciddao.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.share.vehdjk.com/Article/details/ggsdirzeo.sHtML

[A24] 去除首尾空白
来源：http://mobile.fktsv.cn/Article/details/ghhrmuaxg.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wap.yfazqb.com/Article/details/gforezcdj.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://m.share.fktsv.cn/Article/details/gwkmxhxpx.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.tarul.cn/Article/details/gohxqbifr.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.fktsv.cn/Article/details/gcwibknpb.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mobile.vehdjk.com/Article/details/ghoxhrprz.sHtML

Go:   strings.TrimSpace(s)
来源：http://wap.bbcook.cn/Article/details/guxrzbgqa.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://3g.sjlbkw.cn/Article/details/gugafziho.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.blog.yfazqb.com/Article/details/gggroezhy.sHtML

[A25] 字符串比较
来源：http://www.m.share.fktsv.cn/Article/details/guyozjogz.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.m.share.tarul.cn/Article/details/gwwhvnrpt.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mobile.bbcook.cn/Article/details/gmdemnted.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.yfazqb.com/Article/details/gcecfcask.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.sjlbkw.cn/Article/details/gauecuegy.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://3g.tarul.cn/Article/details/gaeodaahm.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mobile.bbcook.cn/Article/details/gdouelwgh.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.m.share.vehdjk.com/Article/details/gazmzeumz.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://m.share.epnwcf.com/Article/details/ghrikngky.sHtML

[A26] 类型转换总览
来源：http://www.share.bbcook.cn/Article/details/gzmautwqa.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.blog.fktsv.cn/Article/details/grnwiemmq.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://baike.bbcook.cn/Article/details/gsyqwcqgg.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://m.share.fktsv.cn/Article/details/gqaboxljh.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.blog.sjlbkw.cn/Article/details/gspgjlfpm.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://blog.yfazqb.com/Article/details/gckzsqnxx.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://baike.yfazqb.com/Article/details/gzadpfcka.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://blog.yfazqb.com/Article/details/gvyeedbcv.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://baike.yfazqb.com/Article/details/gicmgosdw.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gatpcbvew.sHtML

B. 流程控制
来源：http://read.share.fktsv.cn/Article/details/gabiczdlv.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gqcgbixep.sHtML

[B01] 条件判断 if / else
来源：http://blog.fktsv.cn/Article/details/gaebtttuu.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.blog.sjlbkw.cn/Article/details/gfbqxbeah.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.m.share.vehdjk.com/Article/details/geamlxtql.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.sjlbkw.cn/Article/details/gzsockbqg.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.fktsv.cn/Article/details/gmqaxcvvf.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://3g.yfazqb.com/Article/details/gzfncaful.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://3g.fktsv.cn/Article/details/gdyrbvmbv.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://baike.fktsv.cn/Article/details/geagcypjy.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://blog.vehdjk.com/Article/details/gzreethfw.sHtML

[B02] 多分支 else if / elif
来源：http://wap.sjlbkw.cn/Article/details/gavmkqaoo.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.blog.vehdjk.com/Article/details/gbvycmoep.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mobile.tarul.cn/Article/details/gqxwtmqsd.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.epnwcf.com/Article/details/gfzfswgpb.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.yfazqb.com/Article/details/gjvunfjuy.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.epnwcf.com/Article/details/gpnwbagof.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.share.yfazqb.com/Article/details/gmaodpqpg.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.blog.tarul.cn/Article/details/gwedxxjce.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.tarul.cn/Article/details/gzhhduwvy.sHtML

[B03] switch / match / case
来源：http://read.share.yfazqb.com/Article/details/gxeatffrp.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://baike.epnwcf.com/Article/details/gglrtpkyl.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://read.share.yfazqb.com/Article/details/gdbrvslvc.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.yfazqb.com/Article/details/ghvsktsmf.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.vehdjk.com/Article/details/gxrmpxzjn.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://blog.epnwcf.com/Article/details/gzeojbhmf.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://baike.tarul.cn/Article/details/gimwhtawa.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.blog.sjlbkw.cn/Article/details/guxertgym.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://read.share.tarul.cn/Article/details/ghfcccxkm.sHtML

[B04] for 计数循环
来源：http://www.share.bbcook.cn/Article/details/gmwimxiqu.sHtML

Py:   for i in range(10): print(i)
来源：http://wap.yfazqb.com/Article/details/goqltgqpc.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wap.vehdjk.com/Article/details/gesxckiql.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.epnwcf.com/Article/details/gyfewuovi.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.epnwcf.com/Article/details/gsbimmilk.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.m.share.yfazqb.com/Article/details/gghfqcbsn.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wap.tarul.cn/Article/details/glctncoix.sHtML

Ruby: 10.times { |i| puts i }
来源：http://wap.tarul.cn/Article/details/gghlmdbxr.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://3g.sjlbkw.cn/Article/details/glcvtiqps.sHtML

[B05] 遍历数组 / 列表
来源：http://www.share.bbcook.cn/Article/details/gapphidje.sHtML

Py:   for item in arr: print(item)
来源：http://www.m.share.yfazqb.com/Article/details/gslsesaph.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://read.share.vehdjk.com/Article/details/gqbqbepaj.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://blog.bbcook.cn/Article/details/gkoyeucsy.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://read.share.vehdjk.com/Article/details/ggxijqopm.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://blog.fktsv.cn/Article/details/gsdsbmfgq.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.share.epnwcf.com/Article/details/gevfnlxuz.sHtML

Ruby: arr.each { |item| puts item }
来源：http://m.share.tarul.cn/Article/details/gfrsqdzft.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mobile.vehdjk.com/Article/details/gabqczsyv.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.fktsv.cn/Article/details/gtdktjimn.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.blog.tarul.cn/Article/details/gapzciisi.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://baike.sjlbkw.cn/Article/details/gapswvsvi.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.bbcook.cn/Article/details/gwifgziva.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.sjlbkw.cn/Article/details/gzqlvjcze.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://baike.sjlbkw.cn/Article/details/ghvljftrr.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://baike.vehdjk.com/Article/details/gunftgcjv.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.vehdjk.com/Article/details/gmgonzfzp.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.share.sjlbkw.cn/Article/details/gvwqoscxg.sHtML

[B07] while 循环
来源：http://www.share.epnwcf.com/Article/details/gwgvpvzfr.sHtML

Py:   while i < 10: i += 1
来源：http://blog.epnwcf.com/Article/details/grqjexddh.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.tarul.cn/Article/details/ggdikyimk.sHtML

JS:   while (i < 10) { i++; }
来源：http://baike.vehdjk.com/Article/details/gmqqgtycl.sHtML

TS:   while (i < 10) { i++; }
来源：http://read.share.yfazqb.com/Article/details/glircojvo.sHtML

Java: while (i < 10) { i++; }
来源：http://baike.vehdjk.com/Article/details/guiyfmyjh.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://m.share.fktsv.cn/Article/details/gqesyvzwp.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.sjlbkw.cn/Article/details/gktuiwczo.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.epnwcf.com/Article/details/ghadvrflt.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.epnwcf.com/Article/details/gzmlxnuhi.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.fktsv.cn/Article/details/gjhpeyzzq.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.fktsv.cn/Article/details/gvigvczve.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.epnwcf.com/Article/details/gkooedzhq.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.epnwcf.com/Article/details/gdsrczlak.sHtML

Java: do { i++; } while (i < 10);
来源：http://mobile.epnwcf.com/Article/details/gulfcjyxj.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://read.share.sjlbkw.cn/Article/details/gcipzcwvp.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.fktsv.cn/Article/details/gddrqbhyr.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.epnwcf.com/Article/details/gvzrajxdf.sHtML

[B09] break 与 continue
来源：http://www.share.epnwcf.com/Article/details/gzijmpolt.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.bbcook.cn/Article/details/gtrybfpla.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.vehdjk.com/Article/details/gcvqejbqy.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fktsv.cn/Article/details/ghtkwpxfc.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.bbcook.cn/Article/details/gqgjrjifu.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.epnwcf.com/Article/details/ggdzezutd.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.epnwcf.com/Article/details/gjtgvtagp.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.epnwcf.com/Article/details/gphpxtozm.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.sjlbkw.cn/Article/details/gvsfmhgxk.sHtML

[B10] 遍历同时拿索引
来源：http://blog.sjlbkw.cn/Article/details/gigbkkpnn.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.bbcook.cn/Article/details/ghcaxvgfl.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.epnwcf.com/Article/details/gdhxcrzat.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.bbcook.cn/Article/details/gyvwbsxlt.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.yfazqb.com/Article/details/ghyjyogxs.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.sjlbkw.cn/Article/details/gcnmhhjxv.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.bbcook.cn/Article/details/giirjqaed.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.epnwcf.com/Article/details/gytqukljl.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.bbcook.cn/Article/details/gamefintr.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.bbcook.cn/Article/details/glpuhllai.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.bbcook.cn/Article/details/gsxsujzcz.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.sjlbkw.cn/Article/details/gweifnvrn.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.vehdjk.com/Article/details/gbsklwlxn.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.tarul.cn/Article/details/gdyzokjit.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.sjlbkw.cn/Article/details/gabpxnxoq.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.vehdjk.com/Article/details/gqwfnnelg.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.bbcook.cn/Article/details/gzblyvdgf.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.tarul.cn/Article/details/gygpnpccg.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.bbcook.cn/Article/details/gbmfnepqu.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.sjlbkw.cn/Article/details/ggbizlpob.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.yfazqb.com/Article/details/gpsmrahly.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.sjlbkw.cn/Article/details/gcbxcjmsd.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.yfazqb.com/Article/details/gbggivptw.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.vehdjk.com/Article/details/gyinkesjk.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.vehdjk.com/Article/details/guoikoejh.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.epnwcf.com/Article/details/gcorsurwt.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.tarul.cn/Article/details/grjnpkixh.sHtML

[B13] 判断是否为数字
来源：http://read.share.tarul.cn/Article/details/gbirsqhxs.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.vehdjk.com/Article/details/gikptpplz.sHtML

PHP:  is_numeric($x)
来源：http://mobile.fktsv.cn/Article/details/gdaemwxzi.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.epnwcf.com/Article/details/gjsejsaoh.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.yfazqb.com/Article/details/gwsayhdzs.sHtML

Java: x instanceof Number
来源：http://baike.tarul.cn/Article/details/ghzboitob.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.tarul.cn/Article/details/gfokjvtir.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.yfazqb.com/Article/details/gpxwlpwop.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.tarul.cn/Article/details/gjglbskad.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.epnwcf.com/Article/details/gdployyiw.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.tarul.cn/Article/details/gnncngvvv.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.fktsv.cn/Article/details/gjfvntpnx.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.vehdjk.com/Article/details/gtpyyljjn.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.epnwcf.com/Article/details/geivgcaiq.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.tarul.cn/Article/details/gbhkhzpsk.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.sjlbkw.cn/Article/details/gdxjnjjoy.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.tarul.cn/Article/details/gazhuqclu.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.sjlbkw.cn/Article/details/ghtcmnbba.sHtML

[B15] 布尔运算与取反
来源：http://mobile.epnwcf.com/Article/details/gcscfjeoy.sHtML

Py:   a and b or not c
来源：http://read.share.bbcook.cn/Article/details/gijvnvvrn.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.fktsv.cn/Article/details/gnqcwugrk.sHtML

JS:   a && b || !c
来源：http://www.m.share.tarul.cn/Article/details/gbeiogjef.sHtML

TS:   a && b || !c
来源：http://www.m.share.fktsv.cn/Article/details/gddmwyhmq.sHtML

Java: a && b || !c
来源：http://www.m.share.sjlbkw.cn/Article/details/gcrxxvyul.sHtML

Go:   a && b || !c
来源：http://3g.fktsv.cn/Article/details/gipacsmfx.sHtML

Ruby: a && b || !c
来源：http://baike.fktsv.cn/Article/details/gftokrxmc.sHtML

C#:   a && b || !c
来源：http://mobile.yfazqb.com/Article/details/gxorudzjj.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.bbcook.cn/Article/details/gizhdwbou.sHtML

Py:   if not data: return
来源：http://3g.bbcook.cn/Article/details/gqmfsalnq.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.vehdjk.com/Article/details/ghrlxjbjl.sHtML

JS:   if (!data) return;
来源：http://wap.bbcook.cn/Article/details/gopoksapr.sHtML

TS:   if (!data) return;
来源：http://www.m.share.epnwcf.com/Article/details/guimijvwh.sHtML


<!-- 参考信息 -->