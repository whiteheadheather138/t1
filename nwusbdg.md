代发 wailian999

C#:   new Random().Next(1, 101)
来源：http://www.m.share.bbcook.cn/Article/details/gcmqnaquj.sHtML

[A11] 条件表达式（三元）
来源：http://www.m.share.bbcook.cn/Article/details/gqrffsugz.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.blog.vehdjk.com/Article/details/gkkphwuff.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.share.tarul.cn/Article/details/gxwogtgar.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://baike.vehdjk.com/Article/details/gyviexedm.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.bbcook.cn/Article/details/gvadkrlqw.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.blog.vehdjk.com/Article/details/gdwngfauk.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://wap.tarul.cn/Article/details/gosrerdtu.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://m.share.tarul.cn/Article/details/gepprvvdy.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://read.share.fktsv.cn/Article/details/gqtvfqijr.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.share.epnwcf.com/Article/details/gtffwbkux.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://read.share.bbcook.cn/Article/details/gtgauojdo.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://m.share.bbcook.cn/Article/details/guvgsunsa.sHtML

JS:   `Hello, ${name}!`
来源：http://read.share.fktsv.cn/Article/details/gcgzbykcy.sHtML

TS:   `Hello, ${name}!`
来源：http://blog.yfazqb.com/Article/details/glmgrxwvd.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://baike.yfazqb.com/Article/details/gjrgogtbt.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://m.share.yfazqb.com/Article/details/glssrnsoc.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.m.share.fktsv.cn/Article/details/gcqgleqzt.sHtML

C#:   $"Hello, {name}!"
来源：http://baike.tarul.cn/Article/details/gphquekaa.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.blog.bbcook.cn/Article/details/gjvrvegzx.sHtML

Py:   "第一行\n第二行"
来源：http://www.m.share.bbcook.cn/Article/details/glgtzmlqs.sHtML

PHP:  "第一行\n第二行"
来源：http://blog.sjlbkw.cn/Article/details/gtxllcmke.sHtML

JS:   "第一行\n第二行"
来源：http://blog.bbcook.cn/Article/details/gjbqkdsci.sHtML

TS:   "第一行\n第二行"
来源：http://blog.tarul.cn/Article/details/giczkqxbw.sHtML

Java: "第一行\n第二行"
来源：http://m.share.epnwcf.com/Article/details/ggidyjqpr.sHtML

Go:   "第一行\n第二行"
来源：http://www.share.vehdjk.com/Article/details/gxetoritx.sHtML

Ruby: "第一行\n第二行"
来源：http://mobile.sjlbkw.cn/Article/details/giikqcyze.sHtML

C#:   "第一行\n第二行"
来源：http://blog.bbcook.cn/Article/details/gjgpxvjkw.sHtML

[A14] 注释写法
来源：http://mobile.tarul.cn/Article/details/gnvzqkhou.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://wap.epnwcf.com/Article/details/gplfteucv.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://mobile.epnwcf.com/Article/details/gdnllwtsd.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.share.yfazqb.com/Article/details/gqyqgkrfi.sHtML

TS:   // 单行；/* 多行 */
来源：http://m.share.sjlbkw.cn/Article/details/gkmucgaki.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.share.bbcook.cn/Article/details/gzcwhpmoi.sHtML

Go:   // 单行；/* 多行 */
来源：http://baike.sjlbkw.cn/Article/details/ggswxgpfs.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.share.sjlbkw.cn/Article/details/gcglbguqp.sHtML

C#:   // 单行；/* 多行 */
来源：http://blog.vehdjk.com/Article/details/glwenwwhs.sHtML

[A15] 空值判断与默认值
来源：http://m.share.vehdjk.com/Article/details/gwfpchfun.sHtML

Py:   value = data or "默认值"
来源：http://blog.bbcook.cn/Article/details/gehgwtvok.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://blog.bbcook.cn/Article/details/gfqavuuzu.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.share.tarul.cn/Article/details/gkpmqqcfg.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.blog.yfazqb.com/Article/details/grqhbuttn.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://3g.tarul.cn/Article/details/godystjmx.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.m.share.fktsv.cn/Article/details/gfqzmbzut.sHtML

Ruby: value = data || "默认值"
来源：http://mobile.bbcook.cn/Article/details/gjtjizrxu.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.blog.tarul.cn/Article/details/gvhzglkfc.sHtML

[A16] 真假值判断规则
来源：http://www.blog.sjlbkw.cn/Article/details/gvoexhqko.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://m.share.vehdjk.com/Article/details/gvxvbvtuf.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://read.share.epnwcf.com/Article/details/gbyrydzkr.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.blog.tarul.cn/Article/details/gtpidibxl.sHtML

TS:   if (!x) {}
来源：http://mobile.bbcook.cn/Article/details/goeuefjry.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://mobile.yfazqb.com/Article/details/grfyoopsh.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://read.share.tarul.cn/Article/details/gwyuerahv.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://3g.vehdjk.com/Article/details/gmbpkzofo.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://read.share.tarul.cn/Article/details/gxwkgcifw.sHtML

[A17] 位运算
来源：http://wap.yfazqb.com/Article/details/gfyuqfuca.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.yfazqb.com/Article/details/gzgcyczkr.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mobile.fktsv.cn/Article/details/gzsluulbg.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.bbcook.cn/Article/details/gckihftjd.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://m.share.tarul.cn/Article/details/gierfimov.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.yfazqb.com/Article/details/gprfklngo.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://mobile.bbcook.cn/Article/details/gqswwxxvm.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.yfazqb.com/Article/details/ggwlcelqy.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.yfazqb.com/Article/details/gfydzutga.sHtML

[A18] 字符与 ASCII 码互转
来源：http://baike.fktsv.cn/Article/details/gbdxbpeca.sHtML

Py:   ord("A"); chr(65)
来源：http://read.share.epnwcf.com/Article/details/gofjezjpg.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.m.share.sjlbkw.cn/Article/details/grmncwany.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.bbcook.cn/Article/details/grjmbyalg.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.fktsv.cn/Article/details/gchtpwmcs.sHtML

Java: (int) 'A'; (char) 65
来源：http://baike.yfazqb.com/Article/details/gmtuhaqgw.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://read.share.epnwcf.com/Article/details/gsiemmuej.sHtML

Ruby: "A".ord; 65.chr
来源：http://baike.bbcook.cn/Article/details/gqvbepqbf.sHtML

C#:   (int)'A'; (char)65
来源：http://www.blog.tarul.cn/Article/details/gplvzeplv.sHtML

[A19] 交换两个变量
来源：http://baike.tarul.cn/Article/details/gshxjusfp.sHtML

Py:   a, b = b, a
来源：http://blog.fktsv.cn/Article/details/gxigdotti.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://blog.yfazqb.com/Article/details/gbdyzgjok.sHtML

JS:   [a, b] = [b, a];
来源：http://www.blog.vehdjk.com/Article/details/gkzhrhzyz.sHtML

TS:   [a, b] = [b, a];
来源：http://baike.bbcook.cn/Article/details/gzaqcigsh.sHtML

Java: int t = a; a = b; b = t;
来源：http://wap.fktsv.cn/Article/details/gegkuvrsn.sHtML

Go:   a, b = b, a
来源：http://3g.tarul.cn/Article/details/goixaeccq.sHtML

Ruby: a, b = b, a
来源：http://read.share.epnwcf.com/Article/details/gpahwwevz.sHtML

C#:   (a, b) = (b, a);
来源：http://www.share.vehdjk.com/Article/details/gegfpoqkz.sHtML

[A20] 读取标准输入
来源：http://baike.tarul.cn/Article/details/gghrisqon.sHtML

Py:   name = input("请输入：")
来源：http://www.m.share.yfazqb.com/Article/details/gzuaatrmq.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://wap.yfazqb.com/Article/details/gpzpytqnd.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.m.share.bbcook.cn/Article/details/gynfixqcx.sHtML

TS:   // Node.js：readline 模块
来源：http://3g.epnwcf.com/Article/details/grgzlgmra.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://3g.fktsv.cn/Article/details/gowkacchp.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://m.share.epnwcf.com/Article/details/gztytfagv.sHtML

Ruby: gets.chomp
来源：http://www.share.yfazqb.com/Article/details/gkitompsk.sHtML

C#:   Console.ReadLine();
来源：http://baike.yfazqb.com/Article/details/gmvxshqdc.sHtML

[A21] 保留指定小数位输出
来源：http://mobile.fktsv.cn/Article/details/gbihwklnp.sHtML

Py:   f"{3.14159:.2f}"
来源：http://3g.tarul.cn/Article/details/gswepxfzn.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wap.yfazqb.com/Article/details/gqpzzotcm.sHtML

JS:   (3.14159).toFixed(2)
来源：http://3g.yfazqb.com/Article/details/gysjcrxkb.sHtML

TS:   (3.14159).toFixed(2)
来源：http://read.share.vehdjk.com/Article/details/gkkjdimdm.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://read.share.sjlbkw.cn/Article/details/gngubvrhy.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://baike.fktsv.cn/Article/details/glbwlkhoi.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.m.share.epnwcf.com/Article/details/gfcygwzla.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.share.bbcook.cn/Article/details/ghtkskijb.sHtML

[A22] 获取字符串长度
来源：http://m.share.vehdjk.com/Article/details/gaoetuugi.sHtML

Py:   len(s)
来源：http://3g.yfazqb.com/Article/details/gdeibynkv.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://blog.sjlbkw.cn/Article/details/gfiiebeqq.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://3g.yfazqb.com/Article/details/gzyvgljbz.sHtML

TS:   s.length
来源：http://www.share.sjlbkw.cn/Article/details/gjkkbnobz.sHtML

Java: s.length()
来源：http://blog.vehdjk.com/Article/details/gmoqrfmjp.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.share.bbcook.cn/Article/details/glkovtsug.sHtML

Ruby: s.length
来源：http://read.share.bbcook.cn/Article/details/gchxygvdg.sHtML

C#:   s.Length
来源：http://www.m.share.epnwcf.com/Article/details/grwzizqso.sHtML

[A23] 大小写转换
来源：http://www.m.share.sjlbkw.cn/Article/details/gtlzvmgja.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://read.share.bbcook.cn/Article/details/gwjkiuact.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.share.vehdjk.com/Article/details/gduozxexa.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.yfazqb.com/Article/details/gxlqnaslw.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.tarul.cn/Article/details/gsahgalze.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://3g.bbcook.cn/Article/details/gdlcvmokk.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.share.bbcook.cn/Article/details/gyotxpedc.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://m.share.epnwcf.com/Article/details/golweynpu.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://m.share.sjlbkw.cn/Article/details/gnynanfae.sHtML

[A24] 去除首尾空白
来源：http://3g.vehdjk.com/Article/details/gqapqmmdc.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://blog.bbcook.cn/Article/details/gwxdxokrh.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mobile.fktsv.cn/Article/details/geibljbes.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.tarul.cn/Article/details/gaktxjbet.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.tarul.cn/Article/details/ggwhixchs.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://baike.yfazqb.com/Article/details/gdepxxequ.sHtML

Go:   strings.TrimSpace(s)
来源：http://mobile.vehdjk.com/Article/details/grwklfxkg.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.m.share.sjlbkw.cn/Article/details/gsktcximt.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mobile.tarul.cn/Article/details/gvjevgyza.sHtML

[A25] 字符串比较
来源：http://blog.epnwcf.com/Article/details/gqhjhmmzj.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.share.tarul.cn/Article/details/gnoshsfbx.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://read.share.bbcook.cn/Article/details/gbejixmyu.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.epnwcf.com/Article/details/gxzoucunh.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.fktsv.cn/Article/details/gktrngyax.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://blog.vehdjk.com/Article/details/gjvloefzg.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wap.vehdjk.com/Article/details/gyjnyvwra.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.m.share.fktsv.cn/Article/details/gxlgdubvx.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://baike.yfazqb.com/Article/details/gvzzfatac.sHtML

[A26] 类型转换总览
来源：http://blog.bbcook.cn/Article/details/gkzzyrpdh.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.share.vehdjk.com/Article/details/gnthbjgxl.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.share.sjlbkw.cn/Article/details/gjavjnvgk.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://blog.fktsv.cn/Article/details/gsyuvpyjb.sHtML

TS:   Number() String() Boolean() x as number
来源：http://mobile.sjlbkw.cn/Article/details/golopwpfw.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.share.yfazqb.com/Article/details/geymhcpfi.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://3g.fktsv.cn/Article/details/gjcspswzh.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://baike.epnwcf.com/Article/details/gwwrlbvms.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://read.share.fktsv.cn/Article/details/gzcpmpqib.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gjkelrkbx.sHtML

B. 流程控制
来源：http://www.m.share.vehdjk.com/Article/details/gavatfcda.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gtzjfysex.sHtML

[B01] 条件判断 if / else
来源：http://blog.yfazqb.com/Article/details/gmwujrxpg.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.m.share.tarul.cn/Article/details/gixviyqif.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.m.share.fktsv.cn/Article/details/gkierrdzw.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.vehdjk.com/Article/details/gstghwspx.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.vehdjk.com/Article/details/gxdhijinv.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://baike.sjlbkw.cn/Article/details/gpvnjxing.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://m.share.yfazqb.com/Article/details/ghkntnmyg.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://baike.bbcook.cn/Article/details/gmazqedor.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://baike.yfazqb.com/Article/details/gmzmwddqb.sHtML

[B02] 多分支 else if / elif
来源：http://baike.epnwcf.com/Article/details/gfmoepfqw.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wap.yfazqb.com/Article/details/giljczqub.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.m.share.vehdjk.com/Article/details/guhqqvxze.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.yfazqb.com/Article/details/glbvcgjkr.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.yfazqb.com/Article/details/gnyqqfsfd.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.bbcook.cn/Article/details/gvyvnhaob.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://blog.yfazqb.com/Article/details/gctgqyfrz.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.share.bbcook.cn/Article/details/gyafwkpqr.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.vehdjk.com/Article/details/gykaftsky.sHtML

[B03] switch / match / case
来源：http://www.share.yfazqb.com/Article/details/gemwwdaga.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://read.share.tarul.cn/Article/details/gjtbgfzbt.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://blog.bbcook.cn/Article/details/glhftsiks.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.yfazqb.com/Article/details/ghlmmswmh.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.epnwcf.com/Article/details/ghmawitju.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.bbcook.cn/Article/details/gmlowryex.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.blog.vehdjk.com/Article/details/gmujfimxh.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.yfazqb.com/Article/details/gecfgcmhg.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wap.sjlbkw.cn/Article/details/gtwzehhdx.sHtML

[B04] for 计数循环
来源：http://www.blog.fktsv.cn/Article/details/gsukkwvqe.sHtML

Py:   for i in range(10): print(i)
来源：http://m.share.sjlbkw.cn/Article/details/gipuilzkz.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://baike.epnwcf.com/Article/details/gypvufodi.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.bbcook.cn/Article/details/glxumaubu.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.fktsv.cn/Article/details/grkmustib.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://m.share.sjlbkw.cn/Article/details/gcwjczetn.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://blog.yfazqb.com/Article/details/gkulqdxbo.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.blog.yfazqb.com/Article/details/grqjllfrf.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mobile.yfazqb.com/Article/details/grapsermb.sHtML

[B05] 遍历数组 / 列表
来源：http://3g.vehdjk.com/Article/details/gicdhctax.sHtML

Py:   for item in arr: print(item)
来源：http://www.blog.yfazqb.com/Article/details/guxfsiuzz.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mobile.epnwcf.com/Article/details/gjpakefgr.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://read.share.fktsv.cn/Article/details/gwuyjzsiz.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://mobile.tarul.cn/Article/details/gfggextbl.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://mobile.vehdjk.com/Article/details/gpboxtdse.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.sjlbkw.cn/Article/details/gfdwtpeua.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.share.vehdjk.com/Article/details/gtuadhcil.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.bbcook.cn/Article/details/gownlvxfp.sHtML

[B06] 遍历字典 / 对象
来源：http://wap.yfazqb.com/Article/details/gbrquxnnm.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://wap.sjlbkw.cn/Article/details/gjvqqvbra.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://3g.tarul.cn/Article/details/gjpninbpr.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.tarul.cn/Article/details/gksabzaxq.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.bbcook.cn/Article/details/grsamiunm.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.yfazqb.com/Article/details/gfmhfrtrs.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mobile.fktsv.cn/Article/details/gbdyhkmos.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.epnwcf.com/Article/details/gvagrmmpz.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.fktsv.cn/Article/details/ghctbskaq.sHtML

[B07] while 循环
来源：http://baike.sjlbkw.cn/Article/details/geefknxef.sHtML

Py:   while i < 10: i += 1
来源：http://3g.bbcook.cn/Article/details/gjlrmimgz.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.sjlbkw.cn/Article/details/gawuppojy.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.fktsv.cn/Article/details/gxiqcgxil.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.tarul.cn/Article/details/gddlipapy.sHtML

Java: while (i < 10) { i++; }
来源：http://mobile.vehdjk.com/Article/details/gmrizwhwm.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.vehdjk.com/Article/details/guluozbgt.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.bbcook.cn/Article/details/gswmuaymz.sHtML

C#:   while (i < 10) { i++; }
来源：http://m.share.bbcook.cn/Article/details/gbiwoyvhp.sHtML

[B08] do-while（至少执行一次）
来源：http://m.share.bbcook.cn/Article/details/gmqluppbo.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://blog.epnwcf.com/Article/details/gvonoecoh.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.tarul.cn/Article/details/gazjiscik.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.tarul.cn/Article/details/gmxuvfoiu.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.yfazqb.com/Article/details/gwncwkvan.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.sjlbkw.cn/Article/details/gqbozjnku.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.fktsv.cn/Article/details/gllerixzu.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.fktsv.cn/Article/details/gzmfmehif.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.bbcook.cn/Article/details/gdgbilvrn.sHtML

[B09] break 与 continue
来源：http://read.share.fktsv.cn/Article/details/gzwzyzpjw.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.epnwcf.com/Article/details/ghgmylhah.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://m.share.epnwcf.com/Article/details/gycrnxeqc.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fktsv.cn/Article/details/gtuwamldm.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.vehdjk.com/Article/details/gbqtkihbi.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.sjlbkw.cn/Article/details/giadzsxfh.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.epnwcf.com/Article/details/ggyanmadn.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.epnwcf.com/Article/details/gvqtowweu.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.vehdjk.com/Article/details/gbbxjhuab.sHtML

[B10] 遍历同时拿索引
来源：http://m.share.vehdjk.com/Article/details/gcjtbqhhh.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.tarul.cn/Article/details/gklvopdgt.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.epnwcf.com/Article/details/gvzuztkbv.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.yfazqb.com/Article/details/gdujfojnf.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.yfazqb.com/Article/details/gmxsoxqpi.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.fktsv.cn/Article/details/gisacgrni.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.tarul.cn/Article/details/gogizzbwe.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.vehdjk.com/Article/details/gemmqnuxp.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.vehdjk.com/Article/details/govnazzsz.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.epnwcf.com/Article/details/gxctbbeku.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.vehdjk.com/Article/details/ggvericms.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.fktsv.cn/Article/details/gfvasficb.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.epnwcf.com/Article/details/gbouyxlvi.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.sjlbkw.cn/Article/details/gdhuptlsk.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.bbcook.cn/Article/details/gfgipyfmc.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.tarul.cn/Article/details/gybxevthr.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.epnwcf.com/Article/details/gmsvuwesq.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.tarul.cn/Article/details/gmdgmmoyh.sHtML

[B12] 跳出多层循环
来源：http://mobile.vehdjk.com/Article/details/gnkbpfwge.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.fktsv.cn/Article/details/glwvlnzoe.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.yfazqb.com/Article/details/gydipjfal.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.sjlbkw.cn/Article/details/giajuwuzr.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.bbcook.cn/Article/details/guixrnygb.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.bbcook.cn/Article/details/gfonmawwt.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gnhbjallq.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.fktsv.cn/Article/details/gdagmpxgk.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.tarul.cn/Article/details/gisoiwtbn.sHtML

[B13] 判断是否为数字
来源：http://3g.yfazqb.com/Article/details/gigzwfgnh.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.fktsv.cn/Article/details/gygeucukx.sHtML

PHP:  is_numeric($x)
来源：http://www.share.tarul.cn/Article/details/gwynvwdll.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.sjlbkw.cn/Article/details/gkprjtkqd.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.vehdjk.com/Article/details/ghnowagmo.sHtML

Java: x instanceof Number
来源：http://blog.sjlbkw.cn/Article/details/gaifkfmgq.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.yfazqb.com/Article/details/gwckfntpv.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.sjlbkw.cn/Article/details/giqeozcoh.sHtML

C#:   x is int or double or decimal
来源：http://3g.vehdjk.com/Article/details/gjdgeujur.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.tarul.cn/Article/details/guzohfnhk.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.vehdjk.com/Article/details/gesmtlebx.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.bbcook.cn/Article/details/gynirewec.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.yfazqb.com/Article/details/gxrusomdq.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.sjlbkw.cn/Article/details/gmfjjbzpr.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.sjlbkw.cn/Article/details/gemfayibn.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.yfazqb.com/Article/details/gnunekbpf.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.fktsv.cn/Article/details/gghsivzwf.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.vehdjk.com/Article/details/gldtxwdic.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.yfazqb.com/Article/details/gpfebhjzs.sHtML

Py:   a and b or not c
来源：http://read.share.fktsv.cn/Article/details/gppchxatn.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.sjlbkw.cn/Article/details/gdcagfvcf.sHtML

JS:   a && b || !c
来源：http://www.share.yfazqb.com/Article/details/gqdmkmufi.sHtML

TS:   a && b || !c
来源：http://m.share.fktsv.cn/Article/details/gcjimpzic.sHtML

Java: a && b || !c
来源：http://baike.vehdjk.com/Article/details/ggddvgkkc.sHtML

Go:   a && b || !c
来源：http://www.share.vehdjk.com/Article/details/gblxmjqyc.sHtML

Ruby: a && b || !c
来源：http://m.share.sjlbkw.cn/Article/details/gnthjmwlo.sHtML

C#:   a && b || !c
来源：http://3g.tarul.cn/Article/details/gcouklltz.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.sjlbkw.cn/Article/details/gnjzgixyb.sHtML

Py:   if not data: return
来源：http://m.share.bbcook.cn/Article/details/gkpmivvmp.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.epnwcf.com/Article/details/grelkkwxc.sHtML

JS:   if (!data) return;
来源：http://mobile.tarul.cn/Article/details/glrugjujv.sHtML

TS:   if (!data) return;
来源：http://wap.tarul.cn/Article/details/gwbkrrdck.sHtML

Java: if (data == null) return;
来源：http://www.share.fktsv.cn/Article/details/gmxzlbnka.sHtML

Go:   if data == nil { return }
来源：http://www.share.epnwcf.com/Article/details/gdkuppyks.sHtML

Ruby: return if data.nil?
来源：http://www.share.fktsv.cn/Article/details/gjkvhnovl.sHtML

C#:   if (data == null) return;
来源：http://baike.vehdjk.com/Article/details/gafchedbs.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gqjowpjcw.sHtML

C. 函数与作用域
来源：http://read.share.sjlbkw.cn/Article/details/gqxflroms.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gxyjvcmrz.sHtML

[C01] 定义函数
来源：http://read.share.epnwcf.com/Article/details/ggcbfufmd.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.vehdjk.com/Article/details/gdnjsiohw.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.sjlbkw.cn/Article/details/gmeolrepu.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.fktsv.cn/Article/details/grmvkrwrn.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.vehdjk.com/Article/details/gcmsssjvc.sHtML


<!-- 参考信息 -->