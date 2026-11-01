代发 wailian999

C#:   new Random().Next(1, 101)
来源：http://3g.vehdjk.com/Article/details/gglwreoyb.sHtML

[A11] 条件表达式（三元）
来源：http://www.blog.vehdjk.com/Article/details/gzcocxvpb.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.m.share.tarul.cn/Article/details/glyvwragl.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://read.share.yfazqb.com/Article/details/gsudwlker.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://3g.bbcook.cn/Article/details/gyojveqoe.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://wap.vehdjk.com/Article/details/gpetmckuu.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://wap.epnwcf.com/Article/details/gjutzmjpq.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://baike.vehdjk.com/Article/details/glcvoyoud.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.m.share.tarul.cn/Article/details/gflpstcpg.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://3g.yfazqb.com/Article/details/gbtzpmpab.sHtML

[A12] 字符串插值 / 格式化
来源：http://m.share.fktsv.cn/Article/details/ggkqyqgke.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://read.share.epnwcf.com/Article/details/gbafprbgo.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://read.share.tarul.cn/Article/details/gevokejjn.sHtML

JS:   `Hello, ${name}!`
来源：http://blog.fktsv.cn/Article/details/ghohcdjhs.sHtML

TS:   `Hello, ${name}!`
来源：http://www.share.tarul.cn/Article/details/gqhunlzkt.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://blog.tarul.cn/Article/details/gfgkvdrgd.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://baike.vehdjk.com/Article/details/gwqrgblqj.sHtML

Ruby: "Hello, #{name}!"
来源：http://3g.yfazqb.com/Article/details/gwwcjtstt.sHtML

C#:   $"Hello, {name}!"
来源：http://3g.yfazqb.com/Article/details/gbwuvksbm.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://3g.vehdjk.com/Article/details/gndovobgb.sHtML

Py:   "第一行\n第二行"
来源：http://www.share.bbcook.cn/Article/details/gjcbuwjux.sHtML

PHP:  "第一行\n第二行"
来源：http://www.share.epnwcf.com/Article/details/ggpfoutmg.sHtML

JS:   "第一行\n第二行"
来源：http://blog.tarul.cn/Article/details/gxuuvylto.sHtML

TS:   "第一行\n第二行"
来源：http://blog.tarul.cn/Article/details/glmeavxux.sHtML

Java: "第一行\n第二行"
来源：http://mobile.fktsv.cn/Article/details/grrijigbp.sHtML

Go:   "第一行\n第二行"
来源：http://blog.tarul.cn/Article/details/glghronre.sHtML

Ruby: "第一行\n第二行"
来源：http://mobile.epnwcf.com/Article/details/gdzvovlbt.sHtML

C#:   "第一行\n第二行"
来源：http://www.share.sjlbkw.cn/Article/details/ggxrwjjjo.sHtML

[A14] 注释写法
来源：http://3g.yfazqb.com/Article/details/godepteiz.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://m.share.bbcook.cn/Article/details/gvlydedxa.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://baike.vehdjk.com/Article/details/gtxubqghe.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.share.epnwcf.com/Article/details/gpdfyjyrk.sHtML

TS:   // 单行；/* 多行 */
来源：http://3g.epnwcf.com/Article/details/gmemqsdjf.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://blog.yfazqb.com/Article/details/gxllftjfg.sHtML

Go:   // 单行；/* 多行 */
来源：http://m.share.epnwcf.com/Article/details/gpnfbspqi.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://m.share.epnwcf.com/Article/details/gsowqsdtp.sHtML

C#:   // 单行；/* 多行 */
来源：http://wap.yfazqb.com/Article/details/gebxkadqr.sHtML

[A15] 空值判断与默认值
来源：http://mobile.vehdjk.com/Article/details/gwamejnfd.sHtML

Py:   value = data or "默认值"
来源：http://wap.yfazqb.com/Article/details/gposztuio.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://read.share.epnwcf.com/Article/details/gxixkvbin.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.share.fktsv.cn/Article/details/gmektktzs.sHtML

TS:   const value = data ?? "默认值";
来源：http://wap.sjlbkw.cn/Article/details/gofvwsssn.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wap.tarul.cn/Article/details/goydnmhxs.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://read.share.yfazqb.com/Article/details/geitpnzdh.sHtML

Ruby: value = data || "默认值"
来源：http://www.share.vehdjk.com/Article/details/gyvcjdibe.sHtML

C#:   var value = data ?? "默认值";
来源：http://m.share.fktsv.cn/Article/details/gcieoflxo.sHtML

[A16] 真假值判断规则
来源：http://baike.yfazqb.com/Article/details/ggzjwnphl.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wap.sjlbkw.cn/Article/details/gxgalwocf.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.m.share.vehdjk.com/Article/details/gnzhalghu.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.m.share.sjlbkw.cn/Article/details/grldnhsjm.sHtML

TS:   if (!x) {}
来源：http://www.share.yfazqb.com/Article/details/gxrpbddph.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.m.share.vehdjk.com/Article/details/gonhtipxa.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.share.vehdjk.com/Article/details/gybjgsdag.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://wap.bbcook.cn/Article/details/gtjlvyhsg.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.share.sjlbkw.cn/Article/details/gehwlqdue.sHtML

[A17] 位运算
来源：http://mobile.vehdjk.com/Article/details/gmjkxzewv.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.epnwcf.com/Article/details/gelradiog.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://baike.yfazqb.com/Article/details/grazopxvo.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.epnwcf.com/Article/details/gzkpkfqxy.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.blog.bbcook.cn/Article/details/ghzctoybl.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.tarul.cn/Article/details/gkzrbsbhj.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.blog.yfazqb.com/Article/details/gqhfvhxoy.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.vehdjk.com/Article/details/gvmffjwqw.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.yfazqb.com/Article/details/gezzwzmeg.sHtML

[A18] 字符与 ASCII 码互转
来源：http://baike.epnwcf.com/Article/details/gomwrfuoh.sHtML

Py:   ord("A"); chr(65)
来源：http://blog.yfazqb.com/Article/details/gqruzfdpa.sHtML

PHP:  ord("A"); chr(65)
来源：http://wap.yfazqb.com/Article/details/gfejbeugt.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.yfazqb.com/Article/details/gjhmtznox.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.m.share.fktsv.cn/Article/details/gqnwuzlld.sHtML

Java: (int) 'A'; (char) 65
来源：http://3g.bbcook.cn/Article/details/gydsuyegy.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.share.yfazqb.com/Article/details/gosggghyz.sHtML

Ruby: "A".ord; 65.chr
来源：http://mobile.vehdjk.com/Article/details/ghwmuvbyq.sHtML

C#:   (int)'A'; (char)65
来源：http://mobile.yfazqb.com/Article/details/gjatigols.sHtML

[A19] 交换两个变量
来源：http://m.share.yfazqb.com/Article/details/gucupcrbq.sHtML

Py:   a, b = b, a
来源：http://www.blog.vehdjk.com/Article/details/gchaneefh.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://baike.epnwcf.com/Article/details/gheabfqfg.sHtML

JS:   [a, b] = [b, a];
来源：http://read.share.sjlbkw.cn/Article/details/gxufvjsdd.sHtML

TS:   [a, b] = [b, a];
来源：http://mobile.yfazqb.com/Article/details/gntxyxqut.sHtML

Java: int t = a; a = b; b = t;
来源：http://blog.fktsv.cn/Article/details/gfpzradkw.sHtML

Go:   a, b = b, a
来源：http://wap.yfazqb.com/Article/details/gnhgfvqgj.sHtML

Ruby: a, b = b, a
来源：http://mobile.vehdjk.com/Article/details/gefycgjxb.sHtML

C#:   (a, b) = (b, a);
来源：http://m.share.epnwcf.com/Article/details/godnrttto.sHtML

[A20] 读取标准输入
来源：http://read.share.yfazqb.com/Article/details/gokmhyvkd.sHtML

Py:   name = input("请输入：")
来源：http://wap.yfazqb.com/Article/details/gdawrmmlx.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://3g.sjlbkw.cn/Article/details/gsovjnllp.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://mobile.vehdjk.com/Article/details/gdveqqwhd.sHtML

TS:   // Node.js：readline 模块
来源：http://m.share.tarul.cn/Article/details/gawcgrick.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://baike.bbcook.cn/Article/details/gjftgmtez.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://read.share.tarul.cn/Article/details/gsaegdeij.sHtML

Ruby: gets.chomp
来源：http://3g.yfazqb.com/Article/details/geyerlfwa.sHtML

C#:   Console.ReadLine();
来源：http://baike.sjlbkw.cn/Article/details/gzcxwnnzf.sHtML

[A21] 保留指定小数位输出
来源：http://m.share.tarul.cn/Article/details/gdbyplktg.sHtML

Py:   f"{3.14159:.2f}"
来源：http://3g.sjlbkw.cn/Article/details/gyjkszuzt.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://baike.tarul.cn/Article/details/gwqwmwauu.sHtML

JS:   (3.14159).toFixed(2)
来源：http://mobile.yfazqb.com/Article/details/ghtufjbsi.sHtML

TS:   (3.14159).toFixed(2)
来源：http://3g.tarul.cn/Article/details/gfjrilpdw.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://blog.epnwcf.com/Article/details/giupgsbjv.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://3g.yfazqb.com/Article/details/gjaodshrd.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.blog.tarul.cn/Article/details/gcjlrbtgg.sHtML

C#:   3.14159.ToString("F2")
来源：http://3g.bbcook.cn/Article/details/ggxfrpgmw.sHtML

[A22] 获取字符串长度
来源：http://www.blog.tarul.cn/Article/details/gucgceghi.sHtML

Py:   len(s)
来源：http://www.blog.vehdjk.com/Article/details/gjpfotemt.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://read.share.epnwcf.com/Article/details/grlqdfmdq.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://baike.tarul.cn/Article/details/grxahtcaz.sHtML

TS:   s.length
来源：http://www.share.tarul.cn/Article/details/gauszghqk.sHtML

Java: s.length()
来源：http://read.share.vehdjk.com/Article/details/ggajskmgy.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.share.tarul.cn/Article/details/gtkyzthjc.sHtML

Ruby: s.length
来源：http://blog.bbcook.cn/Article/details/gimjaapdn.sHtML

C#:   s.Length
来源：http://mobile.fktsv.cn/Article/details/gumtxzbbt.sHtML

[A23] 大小写转换
来源：http://read.share.sjlbkw.cn/Article/details/ggzemvadf.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://m.share.tarul.cn/Article/details/gflwtxolx.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://m.share.tarul.cn/Article/details/gfpuyufpn.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.yfazqb.com/Article/details/ghvriuvaa.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.epnwcf.com/Article/details/glagmdapr.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mobile.vehdjk.com/Article/details/gqkqkdnub.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://blog.bbcook.cn/Article/details/gbbthtqbz.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.share.yfazqb.com/Article/details/gyxotrxer.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://m.share.tarul.cn/Article/details/garovufkz.sHtML

[A24] 去除首尾空白
来源：http://mobile.vehdjk.com/Article/details/ggneculiy.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://m.share.sjlbkw.cn/Article/details/gwsifpsmu.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.m.share.tarul.cn/Article/details/gfaohqoss.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.yfazqb.com/Article/details/glpomurtt.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.yfazqb.com/Article/details/glthbnzna.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wap.fktsv.cn/Article/details/gzrhgawwg.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.share.yfazqb.com/Article/details/gwerkwxlq.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.m.share.epnwcf.com/Article/details/ghpezkshb.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.blog.vehdjk.com/Article/details/gmedkazlz.sHtML

[A25] 字符串比较
来源：http://read.share.vehdjk.com/Article/details/gvfjkmvow.sHtML

Py:   s1 == s2; s1 != s2
来源：http://read.share.tarul.cn/Article/details/ggvpwfsul.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.m.share.vehdjk.com/Article/details/gqzhegrha.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.yfazqb.com/Article/details/gnrdlmnkb.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.bbcook.cn/Article/details/gctuzdtja.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://baike.yfazqb.com/Article/details/gmjdpganp.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.m.share.bbcook.cn/Article/details/gqpzygjwv.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://wap.tarul.cn/Article/details/gmdhpctmz.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.share.yfazqb.com/Article/details/gyeqpkokt.sHtML

[A26] 类型转换总览
来源：http://wap.fktsv.cn/Article/details/gnuookghj.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.blog.tarul.cn/Article/details/githienxw.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://m.share.vehdjk.com/Article/details/gilsfawjn.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://read.share.epnwcf.com/Article/details/glvjkqwlo.sHtML

TS:   Number() String() Boolean() x as number
来源：http://read.share.fktsv.cn/Article/details/gppxnicgz.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://read.share.bbcook.cn/Article/details/gtjioapik.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://blog.epnwcf.com/Article/details/gadqypqvl.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://m.share.yfazqb.com/Article/details/gvempvkjh.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.m.share.tarul.cn/Article/details/gkktssztl.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gymaefjei.sHtML

B. 流程控制
来源：http://blog.tarul.cn/Article/details/godnzmzia.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gsdsssqso.sHtML

[B01] 条件判断 if / else
来源：http://wap.sjlbkw.cn/Article/details/gvqsfajnt.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://wap.yfazqb.com/Article/details/gtjbcirtk.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.share.sjlbkw.cn/Article/details/gcfrlvkkd.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.yfazqb.com/Article/details/gjenwvusa.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.bbcook.cn/Article/details/gniuhkdyf.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.share.fktsv.cn/Article/details/gmmzmenqp.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://blog.tarul.cn/Article/details/ggjshxaqy.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://baike.tarul.cn/Article/details/gsxgbjkss.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.blog.vehdjk.com/Article/details/gqkamyfbm.sHtML

[B02] 多分支 else if / elif
来源：http://3g.vehdjk.com/Article/details/gaepgnsrq.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.blog.fktsv.cn/Article/details/gofwmlukd.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mobile.bbcook.cn/Article/details/gwkzavibk.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.tarul.cn/Article/details/gtxczypvr.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fktsv.cn/Article/details/gkjkpscjm.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.sjlbkw.cn/Article/details/gagigubdw.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wap.bbcook.cn/Article/details/gpbcnuitp.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://blog.tarul.cn/Article/details/gnizeajbv.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.fktsv.cn/Article/details/gtnmfxuqq.sHtML

[B03] switch / match / case
来源：http://wap.bbcook.cn/Article/details/gbarvynih.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.blog.bbcook.cn/Article/details/glfgzeidi.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://m.share.epnwcf.com/Article/details/gdsgdsoli.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.epnwcf.com/Article/details/gvzvbzjpm.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.vehdjk.com/Article/details/gjxvqqagl.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gpxrulxzx.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://3g.sjlbkw.cn/Article/details/gbyvyjrrp.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.share.vehdjk.com/Article/details/gouhiiaee.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wap.tarul.cn/Article/details/gluyogafj.sHtML

[B04] for 计数循环
来源：http://baike.epnwcf.com/Article/details/gbguskgvu.sHtML

Py:   for i in range(10): print(i)
来源：http://m.share.tarul.cn/Article/details/gexhqkoca.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.m.share.bbcook.cn/Article/details/gvbauhebp.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.fktsv.cn/Article/details/gyhlmgywe.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.yfazqb.com/Article/details/gxzjszeud.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://baike.epnwcf.com/Article/details/gwdgdlkck.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.m.share.fktsv.cn/Article/details/gxgoowsxo.sHtML

Ruby: 10.times { |i| puts i }
来源：http://m.share.vehdjk.com/Article/details/gssmwofoa.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://3g.bbcook.cn/Article/details/gtytyugrc.sHtML

[B05] 遍历数组 / 列表
来源：http://www.m.share.sjlbkw.cn/Article/details/gyajmvkah.sHtML

Py:   for item in arr: print(item)
来源：http://read.share.bbcook.cn/Article/details/ggnwuzzkc.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.blog.tarul.cn/Article/details/ggyscftzc.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://mobile.bbcook.cn/Article/details/gzuvnmigu.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.fktsv.cn/Article/details/gdiezgtre.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://mobile.bbcook.cn/Article/details/gmaapsphz.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://m.share.vehdjk.com/Article/details/gjlghatef.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.blog.fktsv.cn/Article/details/gbcpnjrgp.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://read.share.tarul.cn/Article/details/gtnyhwkmw.sHtML

[B06] 遍历字典 / 对象
来源：http://wap.bbcook.cn/Article/details/ghxzfvewq.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://baike.vehdjk.com/Article/details/gsvmykoxa.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://m.share.sjlbkw.cn/Article/details/gmmamtkax.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.vehdjk.com/Article/details/gdbxmgnda.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.epnwcf.com/Article/details/gcftlpaee.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.bbcook.cn/Article/details/gnufrbmfs.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://3g.yfazqb.com/Article/details/gknjabjtb.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.epnwcf.com/Article/details/ggmtlueoi.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.epnwcf.com/Article/details/greizluem.sHtML

[B07] while 循环
来源：http://m.share.vehdjk.com/Article/details/gvmnexbiw.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.fktsv.cn/Article/details/gflyewnub.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.yfazqb.com/Article/details/gotaxzclg.sHtML

JS:   while (i < 10) { i++; }
来源：http://baike.tarul.cn/Article/details/gvyatzytb.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.epnwcf.com/Article/details/gntzokdmg.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.sjlbkw.cn/Article/details/gdozxpznu.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.share.vehdjk.com/Article/details/giqrqtqew.sHtML

Ruby: while i < 10; i += 1; end
来源：http://m.share.epnwcf.com/Article/details/gcjygokmh.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.fktsv.cn/Article/details/gkzesusup.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.vehdjk.com/Article/details/gsdyigday.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.bbcook.cn/Article/details/glchlfjxm.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.sjlbkw.cn/Article/details/gjdlxksek.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.sjlbkw.cn/Article/details/gimwzoams.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.fktsv.cn/Article/details/gcnuplpuj.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.blog.yfazqb.com/Article/details/gpkbutsqg.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://m.share.epnwcf.com/Article/details/geetgbaya.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://read.share.sjlbkw.cn/Article/details/gzylgygrl.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.tarul.cn/Article/details/gdworaonb.sHtML

[B09] break 与 continue
来源：http://www.blog.yfazqb.com/Article/details/gdyvlccjo.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.epnwcf.com/Article/details/gbdvgbacm.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.yfazqb.com/Article/details/gnbstirap.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.bbcook.cn/Article/details/gaknpycmd.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.sjlbkw.cn/Article/details/gcifoffke.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.sjlbkw.cn/Article/details/gapfbtldd.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.sjlbkw.cn/Article/details/gbquwyibl.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.sjlbkw.cn/Article/details/gtupuayjd.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.bbcook.cn/Article/details/gcsupbkib.sHtML

[B10] 遍历同时拿索引
来源：http://baike.sjlbkw.cn/Article/details/ggtstetdg.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.vehdjk.com/Article/details/gnwmggjik.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.yfazqb.com/Article/details/gudqecpfc.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.yfazqb.com/Article/details/gljaqiehl.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.sjlbkw.cn/Article/details/ggbeswpiw.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://3g.yfazqb.com/Article/details/gbouafupl.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.tarul.cn/Article/details/gwhtigahn.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.epnwcf.com/Article/details/gmzzcpckb.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.bbcook.cn/Article/details/gvcgxojio.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.sjlbkw.cn/Article/details/grhlwqhyz.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.tarul.cn/Article/details/giggyvsdy.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.tarul.cn/Article/details/gbszvtgxu.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.tarul.cn/Article/details/ggixamdvu.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.yfazqb.com/Article/details/gjmxwrcqh.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.sjlbkw.cn/Article/details/gmfceflqu.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.tarul.cn/Article/details/giolgxlqj.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.epnwcf.com/Article/details/gasnvesia.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.bbcook.cn/Article/details/gefdirgnb.sHtML

[B12] 跳出多层循环
来源：http://wap.yfazqb.com/Article/details/gnivfaifx.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.epnwcf.com/Article/details/glymufkkm.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.bbcook.cn/Article/details/gvozxmeug.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.tarul.cn/Article/details/gpppotbvu.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.yfazqb.com/Article/details/gnbsgwtgn.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.yfazqb.com/Article/details/ghoubepst.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.bbcook.cn/Article/details/gkjbnuqoy.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.bbcook.cn/Article/details/gghbgzxan.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.epnwcf.com/Article/details/gfpnuluiz.sHtML

[B13] 判断是否为数字
来源：http://blog.vehdjk.com/Article/details/gogqvawpb.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.fktsv.cn/Article/details/gzsmpievo.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.epnwcf.com/Article/details/gzjbwizho.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.fktsv.cn/Article/details/gnvfvgxoc.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.epnwcf.com/Article/details/gkmgmtxjk.sHtML

Java: x instanceof Number
来源：http://mobile.sjlbkw.cn/Article/details/gqdctkrwf.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.vehdjk.com/Article/details/gpybjerrg.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.yfazqb.com/Article/details/grjqajbyd.sHtML

C#:   x is int or double or decimal
来源：http://m.share.vehdjk.com/Article/details/gjtoaqpvd.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.tarul.cn/Article/details/gfelomfdk.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.tarul.cn/Article/details/gciiapsvd.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.vehdjk.com/Article/details/gdnhrtevx.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.yfazqb.com/Article/details/gdxhhpleg.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.bbcook.cn/Article/details/gnmvlywmu.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.tarul.cn/Article/details/ggjilwyxa.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.bbcook.cn/Article/details/gayqersjm.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.vehdjk.com/Article/details/gcrrslinr.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.fktsv.cn/Article/details/godgdtxwn.sHtML

[B15] 布尔运算与取反
来源：http://m.share.tarul.cn/Article/details/gmcveihms.sHtML

Py:   a and b or not c
来源：http://mobile.epnwcf.com/Article/details/gmrdekwbn.sHtML

PHP:  $a && $b || !$c
来源：http://wap.tarul.cn/Article/details/ghadaikjg.sHtML

JS:   a && b || !c
来源：http://m.share.bbcook.cn/Article/details/gauhsbjic.sHtML

TS:   a && b || !c
来源：http://www.share.fktsv.cn/Article/details/glsnmjcsq.sHtML

Java: a && b || !c
来源：http://3g.fktsv.cn/Article/details/gklptlvzn.sHtML

Go:   a && b || !c
来源：http://baike.bbcook.cn/Article/details/gznabdbxv.sHtML

Ruby: a && b || !c
来源：http://read.share.tarul.cn/Article/details/gsoirolgt.sHtML

C#:   a && b || !c
来源：http://mobile.bbcook.cn/Article/details/gwchxokya.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.bbcook.cn/Article/details/ggytrbpss.sHtML

Py:   if not data: return
来源：http://m.share.sjlbkw.cn/Article/details/guoburwyj.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.vehdjk.com/Article/details/gtorbbnrf.sHtML

JS:   if (!data) return;
来源：http://mobile.vehdjk.com/Article/details/gwyuiwfvh.sHtML

TS:   if (!data) return;
来源：http://baike.vehdjk.com/Article/details/gnhyyumft.sHtML

Java: if (data == null) return;
来源：http://3g.fktsv.cn/Article/details/glnjfliib.sHtML

Go:   if data == nil { return }
来源：http://3g.fktsv.cn/Article/details/gcspxvxoh.sHtML

Ruby: return if data.nil?
来源：http://read.share.tarul.cn/Article/details/gsrasvleu.sHtML

C#:   if (data == null) return;
来源：http://blog.tarul.cn/Article/details/gqwzlmfzh.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gjeemkakv.sHtML

C. 函数与作用域
来源：http://wap.yfazqb.com/Article/details/gpbuqbfqz.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gjuytzlnj.sHtML

[C01] 定义函数
来源：http://m.share.epnwcf.com/Article/details/ggewctcgd.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.tarul.cn/Article/details/gtttchmoj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.vehdjk.com/Article/details/geuqplyit.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.tarul.cn/Article/details/gnyjbynfa.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.sjlbkw.cn/Article/details/gegqyhnuv.sHtML


<!-- 参考信息 -->