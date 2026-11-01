代发 wailian999

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.share.bbcook.cn/Article/details/geunrkdck.sHtML

JS:   `Hello, ${name}!`
来源：http://www.m.share.tarul.cn/Article/details/geqtuyazo.sHtML

TS:   `Hello, ${name}!`
来源：http://www.m.share.epnwcf.com/Article/details/gocvddchz.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.blog.bbcook.cn/Article/details/gdcjfhlfr.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://3g.tarul.cn/Article/details/gldvdoljw.sHtML

Ruby: "Hello, #{name}!"
来源：http://mobile.yfazqb.com/Article/details/gdblmnxck.sHtML

C#:   $"Hello, {name}!"
来源：http://wap.bbcook.cn/Article/details/ghzhryzak.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.blog.sjlbkw.cn/Article/details/gtugugigb.sHtML

Py:   "第一行\n第二行"
来源：http://www.share.sjlbkw.cn/Article/details/ghjynentu.sHtML

PHP:  "第一行\n第二行"
来源：http://mobile.vehdjk.com/Article/details/gbqofyvot.sHtML

JS:   "第一行\n第二行"
来源：http://wap.fktsv.cn/Article/details/gfwwcmxcy.sHtML

TS:   "第一行\n第二行"
来源：http://m.share.sjlbkw.cn/Article/details/gyujvcioj.sHtML

Java: "第一行\n第二行"
来源：http://read.share.bbcook.cn/Article/details/gahwdbklu.sHtML

Go:   "第一行\n第二行"
来源：http://blog.yfazqb.com/Article/details/gwixwpkcs.sHtML

Ruby: "第一行\n第二行"
来源：http://www.m.share.tarul.cn/Article/details/gqsagolxi.sHtML

C#:   "第一行\n第二行"
来源：http://read.share.tarul.cn/Article/details/gtrfouxnt.sHtML

[A14] 注释写法
来源：http://www.m.share.epnwcf.com/Article/details/gyecllryu.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://blog.tarul.cn/Article/details/gizznvayw.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://m.share.yfazqb.com/Article/details/gokecempi.sHtML

JS:   // 单行；/* 多行 */
来源：http://baike.sjlbkw.cn/Article/details/gnjwsuorh.sHtML

TS:   // 单行；/* 多行 */
来源：http://mobile.yfazqb.com/Article/details/gzetwpyhr.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://m.share.fktsv.cn/Article/details/gmncyiyxs.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.m.share.yfazqb.com/Article/details/gcgrsvoff.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.blog.epnwcf.com/Article/details/gadovytcy.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.m.share.fktsv.cn/Article/details/ggbhqrets.sHtML

[A15] 空值判断与默认值
来源：http://mobile.fktsv.cn/Article/details/gldlvfaec.sHtML

Py:   value = data or "默认值"
来源：http://3g.fktsv.cn/Article/details/gwtjndvei.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://mobile.yfazqb.com/Article/details/gvpyggery.sHtML

JS:   const value = data ?? "默认值";
来源：http://mobile.bbcook.cn/Article/details/gepeinkll.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.m.share.epnwcf.com/Article/details/grchqtice.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.m.share.yfazqb.com/Article/details/gnjecwymk.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.m.share.vehdjk.com/Article/details/gtczsuvag.sHtML

Ruby: value = data || "默认值"
来源：http://www.m.share.yfazqb.com/Article/details/gnohwaciz.sHtML

C#:   var value = data ?? "默认值";
来源：http://read.share.epnwcf.com/Article/details/gahpxrpss.sHtML

[A16] 真假值判断规则
来源：http://read.share.tarul.cn/Article/details/gytwvtwjo.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mobile.vehdjk.com/Article/details/gkuxklkrj.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://m.share.yfazqb.com/Article/details/gufquqzgi.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://mobile.sjlbkw.cn/Article/details/gwkpavkak.sHtML

TS:   if (!x) {}
来源：http://blog.fktsv.cn/Article/details/gynmpsvmv.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://3g.yfazqb.com/Article/details/gldrdmwgh.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://baike.yfazqb.com/Article/details/gkuxsweqn.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://baike.bbcook.cn/Article/details/gohrbbnlk.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.share.epnwcf.com/Article/details/gyrspvtjd.sHtML

[A17] 位运算
来源：http://www.blog.fktsv.cn/Article/details/geivhckfu.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fktsv.cn/Article/details/gaijfjlzw.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://blog.yfazqb.com/Article/details/gugdthsxk.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.sjlbkw.cn/Article/details/gpiwjwctv.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://mobile.bbcook.cn/Article/details/ghlgytgtz.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.vehdjk.com/Article/details/gsohsxpjn.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://m.share.bbcook.cn/Article/details/gwcakrfnp.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.sjlbkw.cn/Article/details/gncwwxvgq.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.vehdjk.com/Article/details/ghhcmadej.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.share.bbcook.cn/Article/details/gxryvxuus.sHtML

Py:   ord("A"); chr(65)
来源：http://wap.yfazqb.com/Article/details/gpstflete.sHtML

PHP:  ord("A"); chr(65)
来源：http://blog.fktsv.cn/Article/details/gkxjrtcaf.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.tarul.cn/Article/details/gbbvsdyal.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.fktsv.cn/Article/details/gnwazwdhq.sHtML

Java: (int) 'A'; (char) 65
来源：http://blog.tarul.cn/Article/details/ggpowzqzb.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.share.yfazqb.com/Article/details/gclybcmsd.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.m.share.bbcook.cn/Article/details/gtulafrfx.sHtML

C#:   (int)'A'; (char)65
来源：http://baike.epnwcf.com/Article/details/gsqlvbnui.sHtML

[A19] 交换两个变量
来源：http://m.share.vehdjk.com/Article/details/gqsdtswyk.sHtML

Py:   a, b = b, a
来源：http://www.share.bbcook.cn/Article/details/godadymro.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://baike.vehdjk.com/Article/details/ggxhmuerp.sHtML

JS:   [a, b] = [b, a];
来源：http://read.share.tarul.cn/Article/details/gbiqpcaac.sHtML

TS:   [a, b] = [b, a];
来源：http://www.blog.sjlbkw.cn/Article/details/gekeglazv.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.blog.bbcook.cn/Article/details/gzceyqsuv.sHtML

Go:   a, b = b, a
来源：http://www.share.sjlbkw.cn/Article/details/guakiexvt.sHtML

Ruby: a, b = b, a
来源：http://wap.yfazqb.com/Article/details/graunwomw.sHtML

C#:   (a, b) = (b, a);
来源：http://www.share.fktsv.cn/Article/details/gdqqkqqui.sHtML

[A20] 读取标准输入
来源：http://www.blog.fktsv.cn/Article/details/gyslhciil.sHtML

Py:   name = input("请输入：")
来源：http://read.share.bbcook.cn/Article/details/gjmeedhkx.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.share.bbcook.cn/Article/details/glkeqkhvj.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://read.share.bbcook.cn/Article/details/gczotagta.sHtML

TS:   // Node.js：readline 模块
来源：http://blog.fktsv.cn/Article/details/gedbtvknv.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.m.share.bbcook.cn/Article/details/gdaeorpii.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.share.sjlbkw.cn/Article/details/gywfsqrbh.sHtML

Ruby: gets.chomp
来源：http://wap.fktsv.cn/Article/details/gsquptnml.sHtML

C#:   Console.ReadLine();
来源：http://www.m.share.vehdjk.com/Article/details/gneufckwt.sHtML

[A21] 保留指定小数位输出
来源：http://baike.epnwcf.com/Article/details/gupmzouvm.sHtML

Py:   f"{3.14159:.2f}"
来源：http://3g.yfazqb.com/Article/details/giokonzqd.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://mobile.yfazqb.com/Article/details/gnexsdrhv.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.blog.yfazqb.com/Article/details/gefrcragm.sHtML

TS:   (3.14159).toFixed(2)
来源：http://read.share.fktsv.cn/Article/details/gkipmqdqm.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.blog.bbcook.cn/Article/details/gmqmxuqyb.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://3g.yfazqb.com/Article/details/gginsthpn.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://mobile.vehdjk.com/Article/details/gjqinypso.sHtML

C#:   3.14159.ToString("F2")
来源：http://baike.sjlbkw.cn/Article/details/gmorycoxy.sHtML

[A22] 获取字符串长度
来源：http://read.share.bbcook.cn/Article/details/gevlbwwme.sHtML

Py:   len(s)
来源：http://www.m.share.epnwcf.com/Article/details/gcbukbrma.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://read.share.tarul.cn/Article/details/gbuwkcwkf.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://m.share.epnwcf.com/Article/details/glnkzunqz.sHtML

TS:   s.length
来源：http://blog.tarul.cn/Article/details/gvborblbc.sHtML

Java: s.length()
来源：http://www.blog.sjlbkw.cn/Article/details/gjhfmrqei.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://m.share.sjlbkw.cn/Article/details/gtuyiqenq.sHtML

Ruby: s.length
来源：http://read.share.sjlbkw.cn/Article/details/gnkctkugo.sHtML

C#:   s.Length
来源：http://read.share.yfazqb.com/Article/details/gzfcsxdfd.sHtML

[A23] 大小写转换
来源：http://m.share.sjlbkw.cn/Article/details/gqbjkjiwz.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://m.share.epnwcf.com/Article/details/gfmbzdgas.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://baike.bbcook.cn/Article/details/gvehrnqag.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.tarul.cn/Article/details/gotwliopi.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.bbcook.cn/Article/details/gzviswmkf.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.share.sjlbkw.cn/Article/details/gnqbefpet.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.blog.tarul.cn/Article/details/gpkvlobwd.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mobile.yfazqb.com/Article/details/grvhlpctu.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://read.share.vehdjk.com/Article/details/gfmrorgoe.sHtML

[A24] 去除首尾空白
来源：http://m.share.tarul.cn/Article/details/gokxvzgtr.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.m.share.epnwcf.com/Article/details/glvsteopd.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.share.bbcook.cn/Article/details/gxxwwwdun.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.tarul.cn/Article/details/gnsjaaqql.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.tarul.cn/Article/details/guiqrhpka.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://3g.vehdjk.com/Article/details/gvcdcahln.sHtML

Go:   strings.TrimSpace(s)
来源：http://wap.bbcook.cn/Article/details/grjghhizh.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://baike.vehdjk.com/Article/details/gfumskxvk.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wap.sjlbkw.cn/Article/details/gptaevfjy.sHtML

[A25] 字符串比较
来源：http://www.m.share.epnwcf.com/Article/details/guuokoqij.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.share.vehdjk.com/Article/details/gmgxwamtd.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mobile.vehdjk.com/Article/details/gkromolmq.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.epnwcf.com/Article/details/gledvywmo.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.vehdjk.com/Article/details/giajlniln.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.m.share.yfazqb.com/Article/details/grxyewuog.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://m.share.bbcook.cn/Article/details/gthfyxydb.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://m.share.sjlbkw.cn/Article/details/ghcbspqkc.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://read.share.tarul.cn/Article/details/gcrefpxzb.sHtML

[A26] 类型转换总览
来源：http://wap.sjlbkw.cn/Article/details/gylactqou.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.m.share.bbcook.cn/Article/details/gxcauzykr.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://3g.vehdjk.com/Article/details/gukihdskk.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.blog.vehdjk.com/Article/details/gfwakkfyd.sHtML

TS:   Number() String() Boolean() x as number
来源：http://3g.fktsv.cn/Article/details/gtkpufoku.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mobile.tarul.cn/Article/details/gtwcysqjp.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://m.share.tarul.cn/Article/details/gmfdsanom.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://3g.tarul.cn/Article/details/gxlazvbxz.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://blog.vehdjk.com/Article/details/gjgomcdmw.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gtybanebx.sHtML

B. 流程控制
来源：http://m.share.bbcook.cn/Article/details/gugzczzsy.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gmbggisxf.sHtML

[B01] 条件判断 if / else
来源：http://3g.bbcook.cn/Article/details/giwdtsxjx.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.blog.vehdjk.com/Article/details/gtixwamyp.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.share.sjlbkw.cn/Article/details/gkijjclee.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.tarul.cn/Article/details/ggomxeigu.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.tarul.cn/Article/details/gooigvofa.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.m.share.tarul.cn/Article/details/gdhggqfra.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://3g.fktsv.cn/Article/details/gbvjluhlt.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://3g.fktsv.cn/Article/details/gxbkxcmek.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://3g.epnwcf.com/Article/details/glropjldf.sHtML

[B02] 多分支 else if / elif
来源：http://3g.bbcook.cn/Article/details/gghntmiaa.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://baike.yfazqb.com/Article/details/glxmujuhg.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://blog.yfazqb.com/Article/details/gybhjzybn.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.epnwcf.com/Article/details/gleyenktm.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.vehdjk.com/Article/details/gahymlvpg.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.epnwcf.com/Article/details/gkktcjrzl.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://m.share.yfazqb.com/Article/details/gcgzeyptg.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://baike.tarul.cn/Article/details/goojgasow.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.fktsv.cn/Article/details/gqdnbkvij.sHtML

[B03] switch / match / case
来源：http://wap.vehdjk.com/Article/details/gpmnueejd.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://3g.tarul.cn/Article/details/grmltnukr.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://baike.bbcook.cn/Article/details/givmmqwwc.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.fktsv.cn/Article/details/ghrfnupcb.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.sjlbkw.cn/Article/details/gdgophpsg.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mobile.tarul.cn/Article/details/gpddhtrqv.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mobile.vehdjk.com/Article/details/gkzpkbbmy.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.blog.fktsv.cn/Article/details/gxlabgmiq.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.blog.vehdjk.com/Article/details/gbbkqfzme.sHtML

[B04] for 计数循环
来源：http://www.blog.sjlbkw.cn/Article/details/gfjkoyrun.sHtML

Py:   for i in range(10): print(i)
来源：http://www.m.share.sjlbkw.cn/Article/details/gzzlefghz.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://m.share.tarul.cn/Article/details/gzvirrqbt.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.yfazqb.com/Article/details/gxgbqhwpi.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.vehdjk.com/Article/details/gcwewtmvv.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://3g.bbcook.cn/Article/details/gsznhzgse.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mobile.tarul.cn/Article/details/gvvydpmup.sHtML

Ruby: 10.times { |i| puts i }
来源：http://read.share.epnwcf.com/Article/details/gpoyqjrxy.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://m.share.bbcook.cn/Article/details/gvmeegkwd.sHtML

[B05] 遍历数组 / 列表
来源：http://www.blog.sjlbkw.cn/Article/details/gajdbxnxw.sHtML

Py:   for item in arr: print(item)
来源：http://m.share.fktsv.cn/Article/details/gjukrasmr.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.fktsv.cn/Article/details/gzxthbcqr.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://blog.yfazqb.com/Article/details/gjobvijpp.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://wap.yfazqb.com/Article/details/goqfuucgr.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.blog.epnwcf.com/Article/details/gvlvaaggm.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://m.share.sjlbkw.cn/Article/details/giluujfpi.sHtML

Ruby: arr.each { |item| puts item }
来源：http://m.share.sjlbkw.cn/Article/details/gzcpiobnq.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://baike.epnwcf.com/Article/details/grjqgejnb.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.sjlbkw.cn/Article/details/gumsczshv.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://blog.vehdjk.com/Article/details/grwymvvnz.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.tarul.cn/Article/details/gyhptsxkl.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.tarul.cn/Article/details/guplmcscc.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.sjlbkw.cn/Article/details/ghzyqozty.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.yfazqb.com/Article/details/ghjxhbujn.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.fktsv.cn/Article/details/gcklwoghr.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wap.fktsv.cn/Article/details/gbpxwgguh.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://m.share.fktsv.cn/Article/details/gfbshzpug.sHtML

[B07] while 循环
来源：http://www.blog.bbcook.cn/Article/details/gljlkdfxv.sHtML

Py:   while i < 10: i += 1
来源：http://mobile.epnwcf.com/Article/details/gxgefsqhq.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.blog.epnwcf.com/Article/details/gpapiuizm.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.fktsv.cn/Article/details/gecfqwlxg.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.vehdjk.com/Article/details/gjfehvrxh.sHtML

Java: while (i < 10) { i++; }
来源：http://m.share.fktsv.cn/Article/details/gbkvfnfai.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.fktsv.cn/Article/details/gzvspmsnr.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.fktsv.cn/Article/details/ggvjdefww.sHtML

C#:   while (i < 10) { i++; }
来源：http://blog.bbcook.cn/Article/details/gvwvunwth.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.vehdjk.com/Article/details/grbtdppni.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://mobile.sjlbkw.cn/Article/details/govnxlcvx.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.bbcook.cn/Article/details/gxyetjpdx.sHtML

JS:   do { i++; } while (i < 10);
来源：http://baike.fktsv.cn/Article/details/ghdujtrmy.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.vehdjk.com/Article/details/gnealwktc.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.tarul.cn/Article/details/gfhnrhhbt.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.yfazqb.com/Article/details/gmjmuczny.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://m.share.epnwcf.com/Article/details/gshiwzlqe.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.tarul.cn/Article/details/goqecagny.sHtML

[B09] break 与 continue
来源：http://www.share.fktsv.cn/Article/details/gcresqcce.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.sjlbkw.cn/Article/details/gfxxkuabw.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://m.share.vehdjk.com/Article/details/gypbfjepi.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.epnwcf.com/Article/details/gyhemscfl.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.vehdjk.com/Article/details/gstzoibsm.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.bbcook.cn/Article/details/ghlxvlfvc.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.fktsv.cn/Article/details/gjmichbxw.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.epnwcf.com/Article/details/gxhuikiqa.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gfykfzkvu.sHtML

[B10] 遍历同时拿索引
来源：http://wap.epnwcf.com/Article/details/gwpnuxbom.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.fktsv.cn/Article/details/glzmrdrgi.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.fktsv.cn/Article/details/gfaeatuun.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.tarul.cn/Article/details/gswdtqzvl.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.fktsv.cn/Article/details/gynczdqxz.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.epnwcf.com/Article/details/gztucxbdj.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.tarul.cn/Article/details/gfxzicmij.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.epnwcf.com/Article/details/gucogtyrp.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.epnwcf.com/Article/details/gdfjapchb.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.yfazqb.com/Article/details/gifuffvul.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.fktsv.cn/Article/details/gwazzgpqc.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.bbcook.cn/Article/details/gqulhhaxc.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.tarul.cn/Article/details/gghvylrvn.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.epnwcf.com/Article/details/gnbqtpzpi.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.fktsv.cn/Article/details/gnarkdnhr.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.bbcook.cn/Article/details/gwdynnoko.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.sjlbkw.cn/Article/details/gqirqkvgq.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.vehdjk.com/Article/details/gkhbkialy.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.bbcook.cn/Article/details/ggkyatyum.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.bbcook.cn/Article/details/gfhzlnetm.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.yfazqb.com/Article/details/gfvmaifvo.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.vehdjk.com/Article/details/gqpnowxgw.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.epnwcf.com/Article/details/gtilotjow.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.epnwcf.com/Article/details/ghwbbqjyq.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.fktsv.cn/Article/details/gsetsrmsg.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.tarul.cn/Article/details/gkvlqvdkq.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.tarul.cn/Article/details/ggbnqedqc.sHtML

[B13] 判断是否为数字
来源：http://www.share.yfazqb.com/Article/details/grocsxjgh.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.epnwcf.com/Article/details/gkjpiqafn.sHtML

PHP:  is_numeric($x)
来源：http://blog.fktsv.cn/Article/details/gbpdmaxtn.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.bbcook.cn/Article/details/gfdbbtgel.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.yfazqb.com/Article/details/gyuopsrwr.sHtML

Java: x instanceof Number
来源：http://www.m.share.bbcook.cn/Article/details/gezbrwshf.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.tarul.cn/Article/details/gyllylhvr.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.yfazqb.com/Article/details/gphcgjxhd.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.fktsv.cn/Article/details/gusqoalvl.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.epnwcf.com/Article/details/gndizdjho.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.fktsv.cn/Article/details/gyhxzfulk.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.epnwcf.com/Article/details/gnfbnrooz.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.yfazqb.com/Article/details/gxuipgvft.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.fktsv.cn/Article/details/gooxucjsf.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.yfazqb.com/Article/details/gqpbgvfmq.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.bbcook.cn/Article/details/gzauyaxgp.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.fktsv.cn/Article/details/gptvagudd.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.bbcook.cn/Article/details/gawryhswp.sHtML

[B15] 布尔运算与取反
来源：http://blog.sjlbkw.cn/Article/details/gjqtkvngh.sHtML

Py:   a and b or not c
来源：http://wap.tarul.cn/Article/details/gyrqcwghh.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.bbcook.cn/Article/details/gpivpfjng.sHtML

JS:   a && b || !c
来源：http://wap.fktsv.cn/Article/details/guytutqfa.sHtML

TS:   a && b || !c
来源：http://baike.tarul.cn/Article/details/gnhyqsikd.sHtML

Java: a && b || !c
来源：http://3g.epnwcf.com/Article/details/gkenytyzv.sHtML

Go:   a && b || !c
来源：http://read.share.tarul.cn/Article/details/gykylfbie.sHtML

Ruby: a && b || !c
来源：http://m.share.epnwcf.com/Article/details/gjiuqofqp.sHtML

C#:   a && b || !c
来源：http://3g.yfazqb.com/Article/details/gdmspzhre.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.epnwcf.com/Article/details/gxuniypju.sHtML

Py:   if not data: return
来源：http://mobile.vehdjk.com/Article/details/gfnnwldih.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.epnwcf.com/Article/details/glrhodvqo.sHtML

JS:   if (!data) return;
来源：http://wap.vehdjk.com/Article/details/gtspuxeae.sHtML

TS:   if (!data) return;
来源：http://www.share.tarul.cn/Article/details/ghtvtagpe.sHtML

Java: if (data == null) return;
来源：http://m.share.vehdjk.com/Article/details/gcvtxvhul.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.bbcook.cn/Article/details/ghnbcjsfb.sHtML

Ruby: return if data.nil?
来源：http://blog.sjlbkw.cn/Article/details/gdtwumntz.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.bbcook.cn/Article/details/gceesegvv.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gfaombrca.sHtML

C. 函数与作用域
来源：http://3g.vehdjk.com/Article/details/gdurzrgdx.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gkqwnjnzi.sHtML

[C01] 定义函数
来源：http://www.blog.fktsv.cn/Article/details/gclrkejsb.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.tarul.cn/Article/details/girtlymzx.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.bbcook.cn/Article/details/ghhylqghm.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.vehdjk.com/Article/details/gtojzotjk.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.vehdjk.com/Article/details/gvdxxdefv.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.bbcook.cn/Article/details/gwalwzkms.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.vehdjk.com/Article/details/gnwntzczk.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.sjlbkw.cn/Article/details/gxkqpxxol.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.tarul.cn/Article/details/ggqzpzrxa.sHtML

[C02] 默认参数
来源：http://baike.vehdjk.com/Article/details/gccirknno.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.sjlbkw.cn/Article/details/gflbdpdzg.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.sjlbkw.cn/Article/details/gymqaiont.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.epnwcf.com/Article/details/guebzdlli.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.epnwcf.com/Article/details/gpbigkesk.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.bbcook.cn/Article/details/gvubmeahb.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.yfazqb.com/Article/details/gwpxeqjca.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.vehdjk.com/Article/details/gzgoebsco.sHtML


<!-- 参考信息 -->