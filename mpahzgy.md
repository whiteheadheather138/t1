代发 wailian999

Ruby: x > 0 ? "yes" : "no"
来源：http://wap.tarul.cn/Article/details/gdqfplaxx.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://wap.yfazqb.com/Article/details/gnmwduqfb.sHtML

[A12] 字符串插值 / 格式化
来源：http://read.share.yfazqb.com/Article/details/giiocprdi.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://baike.epnwcf.com/Article/details/gdkmxknrl.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.blog.yfazqb.com/Article/details/gnhwudfpy.sHtML

JS:   `Hello, ${name}!`
来源：http://3g.bbcook.cn/Article/details/ggtilonyr.sHtML

TS:   `Hello, ${name}!`
来源：http://read.share.vehdjk.com/Article/details/gcawnapqu.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://m.share.bbcook.cn/Article/details/ggcpqjlck.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://read.share.yfazqb.com/Article/details/giozayslx.sHtML

Ruby: "Hello, #{name}!"
来源：http://m.share.fktsv.cn/Article/details/gdossdsrt.sHtML

C#:   $"Hello, {name}!"
来源：http://www.share.sjlbkw.cn/Article/details/gsgkyneag.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.m.share.fktsv.cn/Article/details/gveatusrn.sHtML

Py:   "第一行\n第二行"
来源：http://blog.sjlbkw.cn/Article/details/gflfajrtl.sHtML

PHP:  "第一行\n第二行"
来源：http://www.blog.vehdjk.com/Article/details/gzffipgtx.sHtML

JS:   "第一行\n第二行"
来源：http://3g.yfazqb.com/Article/details/gzpywnudp.sHtML

TS:   "第一行\n第二行"
来源：http://3g.sjlbkw.cn/Article/details/gejuztrsm.sHtML

Java: "第一行\n第二行"
来源：http://read.share.vehdjk.com/Article/details/gkwnlqdzm.sHtML

Go:   "第一行\n第二行"
来源：http://read.share.epnwcf.com/Article/details/gmxcocovf.sHtML

Ruby: "第一行\n第二行"
来源：http://m.share.epnwcf.com/Article/details/gpqbhpnyu.sHtML

C#:   "第一行\n第二行"
来源：http://mobile.bbcook.cn/Article/details/gwrrqqvzv.sHtML

[A14] 注释写法
来源：http://www.m.share.vehdjk.com/Article/details/gsfxcxccy.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://3g.sjlbkw.cn/Article/details/gmnsxsaoc.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.share.vehdjk.com/Article/details/glvmyjntp.sHtML

JS:   // 单行；/* 多行 */
来源：http://wap.yfazqb.com/Article/details/gzuecxmru.sHtML

TS:   // 单行；/* 多行 */
来源：http://3g.tarul.cn/Article/details/gwwzcpbsd.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.blog.yfazqb.com/Article/details/gzcbfivll.sHtML

Go:   // 单行；/* 多行 */
来源：http://m.share.tarul.cn/Article/details/gywivdrxt.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://wap.bbcook.cn/Article/details/gjqukpjit.sHtML

C#:   // 单行；/* 多行 */
来源：http://baike.yfazqb.com/Article/details/gagkheqpe.sHtML

[A15] 空值判断与默认值
来源：http://3g.sjlbkw.cn/Article/details/gyaylxgbc.sHtML

Py:   value = data or "默认值"
来源：http://blog.epnwcf.com/Article/details/gunoqupqe.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://mobile.yfazqb.com/Article/details/gcqgmhhex.sHtML

JS:   const value = data ?? "默认值";
来源：http://blog.bbcook.cn/Article/details/gsowprgcq.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.m.share.yfazqb.com/Article/details/giazlqqlm.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.blog.sjlbkw.cn/Article/details/grwdfdieq.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.blog.epnwcf.com/Article/details/gpausngzk.sHtML

Ruby: value = data || "默认值"
来源：http://blog.epnwcf.com/Article/details/govmsdshw.sHtML

C#:   var value = data ?? "默认值";
来源：http://read.share.vehdjk.com/Article/details/gjkrygygl.sHtML

[A16] 真假值判断规则
来源：http://mobile.vehdjk.com/Article/details/ggrjqhpim.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://blog.yfazqb.com/Article/details/goiqkxbua.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://baike.yfazqb.com/Article/details/gjwhbbocz.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://baike.vehdjk.com/Article/details/gumcnvzvh.sHtML

TS:   if (!x) {}
来源：http://mobile.tarul.cn/Article/details/gmiyespxl.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wap.fktsv.cn/Article/details/gglntxzhn.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://3g.sjlbkw.cn/Article/details/gphmosqcg.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.m.share.fktsv.cn/Article/details/gsikdkpah.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://baike.tarul.cn/Article/details/ggrtqigef.sHtML

[A17] 位运算
来源：http://mobile.sjlbkw.cn/Article/details/gbbvorvth.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.vehdjk.com/Article/details/gsnqtdkjx.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://baike.vehdjk.com/Article/details/gjcpadcly.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.tarul.cn/Article/details/gpsgjvmop.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.share.fktsv.cn/Article/details/geklcriwn.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.fktsv.cn/Article/details/gpvgwsmmr.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://baike.yfazqb.com/Article/details/glwszdngp.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.tarul.cn/Article/details/guxurbeqx.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.sjlbkw.cn/Article/details/gsctzvtep.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.share.epnwcf.com/Article/details/gpmuxwhgm.sHtML

Py:   ord("A"); chr(65)
来源：http://3g.tarul.cn/Article/details/gkferathx.sHtML

PHP:  ord("A"); chr(65)
来源：http://read.share.tarul.cn/Article/details/gmtykzbrd.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.sjlbkw.cn/Article/details/gahanexvv.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.vehdjk.com/Article/details/ghtkudeam.sHtML

Java: (int) 'A'; (char) 65
来源：http://mobile.bbcook.cn/Article/details/gnetuzpei.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.blog.yfazqb.com/Article/details/gpdjnnzda.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.m.share.tarul.cn/Article/details/gacjiujot.sHtML

C#:   (int)'A'; (char)65
来源：http://www.m.share.yfazqb.com/Article/details/ghzvfajyw.sHtML

[A19] 交换两个变量
来源：http://blog.epnwcf.com/Article/details/gbyhwhyga.sHtML

Py:   a, b = b, a
来源：http://mobile.vehdjk.com/Article/details/glwvldjrg.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.m.share.fktsv.cn/Article/details/gmayjbzoh.sHtML

JS:   [a, b] = [b, a];
来源：http://m.share.vehdjk.com/Article/details/gjmnhqupl.sHtML

TS:   [a, b] = [b, a];
来源：http://blog.bbcook.cn/Article/details/gfjcmbtix.sHtML

Java: int t = a; a = b; b = t;
来源：http://3g.tarul.cn/Article/details/geuwhupsa.sHtML

Go:   a, b = b, a
来源：http://mobile.yfazqb.com/Article/details/gxqbujikd.sHtML

Ruby: a, b = b, a
来源：http://www.blog.epnwcf.com/Article/details/gaggidsnl.sHtML

C#:   (a, b) = (b, a);
来源：http://3g.yfazqb.com/Article/details/gxpijanzd.sHtML

[A20] 读取标准输入
来源：http://blog.epnwcf.com/Article/details/gthmqphjr.sHtML

Py:   name = input("请输入：")
来源：http://m.share.fktsv.cn/Article/details/ghdruyjtv.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://baike.epnwcf.com/Article/details/gflgqznet.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://blog.yfazqb.com/Article/details/gwozrzodj.sHtML

TS:   // Node.js：readline 模块
来源：http://m.share.vehdjk.com/Article/details/gzfitoggj.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://baike.fktsv.cn/Article/details/gzlhxfumk.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.m.share.tarul.cn/Article/details/ghftboulr.sHtML

Ruby: gets.chomp
来源：http://3g.yfazqb.com/Article/details/gprbblovc.sHtML

C#:   Console.ReadLine();
来源：http://mobile.fktsv.cn/Article/details/gpwpgodlz.sHtML

[A21] 保留指定小数位输出
来源：http://3g.vehdjk.com/Article/details/gpjxgfgfb.sHtML

Py:   f"{3.14159:.2f}"
来源：http://blog.epnwcf.com/Article/details/gohfjdgyx.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wap.yfazqb.com/Article/details/ggbpqpoih.sHtML

JS:   (3.14159).toFixed(2)
来源：http://wap.tarul.cn/Article/details/gfyzjlqup.sHtML

TS:   (3.14159).toFixed(2)
来源：http://blog.tarul.cn/Article/details/gtehtndzl.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://baike.fktsv.cn/Article/details/gsmefiwdu.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://baike.sjlbkw.cn/Article/details/gextyltok.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://m.share.yfazqb.com/Article/details/gqlljtuqv.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.blog.vehdjk.com/Article/details/gbdbflvbn.sHtML

[A22] 获取字符串长度
来源：http://m.share.fktsv.cn/Article/details/gpzjiwrki.sHtML

Py:   len(s)
来源：http://www.share.tarul.cn/Article/details/gjiaslrjm.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wap.yfazqb.com/Article/details/gmjuqydjw.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wap.fktsv.cn/Article/details/grkkthpnx.sHtML

TS:   s.length
来源：http://3g.yfazqb.com/Article/details/glvcrkxiv.sHtML

Java: s.length()
来源：http://www.m.share.vehdjk.com/Article/details/grwfllohq.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mobile.bbcook.cn/Article/details/ggoxswwhm.sHtML

Ruby: s.length
来源：http://m.share.epnwcf.com/Article/details/gydjsvxkv.sHtML

C#:   s.Length
来源：http://www.m.share.vehdjk.com/Article/details/gpgofroet.sHtML

[A23] 大小写转换
来源：http://www.m.share.vehdjk.com/Article/details/glofldoii.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://wap.epnwcf.com/Article/details/giufusgio.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://3g.vehdjk.com/Article/details/guhupbuoc.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.bbcook.cn/Article/details/gbheougeg.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.epnwcf.com/Article/details/gvyuyokin.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://baike.yfazqb.com/Article/details/gitdkxacs.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.blog.fktsv.cn/Article/details/ghcrjfqzf.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.m.share.yfazqb.com/Article/details/gbdffxpmh.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://m.share.sjlbkw.cn/Article/details/gyxigrfmx.sHtML

[A24] 去除首尾空白
来源：http://www.blog.epnwcf.com/Article/details/gawtmphgu.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wap.yfazqb.com/Article/details/gtyuojofp.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mobile.fktsv.cn/Article/details/gcvljafgr.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.epnwcf.com/Article/details/gymqspqpf.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.vehdjk.com/Article/details/gfuazapju.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://3g.fktsv.cn/Article/details/gokqosldl.sHtML

Go:   strings.TrimSpace(s)
来源：http://baike.sjlbkw.cn/Article/details/gcuqflpxo.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.share.epnwcf.com/Article/details/gswavcbvp.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://blog.epnwcf.com/Article/details/gdhoqgzhq.sHtML

[A25] 字符串比较
来源：http://m.share.epnwcf.com/Article/details/gjnjirsnp.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.share.epnwcf.com/Article/details/gnczqgobj.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://blog.bbcook.cn/Article/details/gnueflbyd.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.vehdjk.com/Article/details/gezlqyetp.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.fktsv.cn/Article/details/gmvxtbuxo.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mobile.vehdjk.com/Article/details/gbnjwarfm.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mobile.fktsv.cn/Article/details/gokxzofbg.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://wap.yfazqb.com/Article/details/goucksqwd.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://m.share.sjlbkw.cn/Article/details/goecdklrq.sHtML

[A26] 类型转换总览
来源：http://mobile.tarul.cn/Article/details/gvfdayzxg.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://blog.vehdjk.com/Article/details/glzjptixf.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.share.epnwcf.com/Article/details/gxwpgdjro.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://3g.yfazqb.com/Article/details/gdpjwpmsb.sHtML

TS:   Number() String() Boolean() x as number
来源：http://m.share.yfazqb.com/Article/details/ghzuzdoad.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.m.share.epnwcf.com/Article/details/gsmltbbyi.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.blog.fktsv.cn/Article/details/gjjwetciu.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://baike.fktsv.cn/Article/details/gmjuuchhi.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://baike.bbcook.cn/Article/details/gsoghdvzq.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gukqgochg.sHtML

B. 流程控制
来源：http://www.blog.yfazqb.com/Article/details/gcvdwrphu.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/grswxjmge.sHtML

[B01] 条件判断 if / else
来源：http://www.m.share.tarul.cn/Article/details/grobaqojz.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.blog.vehdjk.com/Article/details/ghfuibvqx.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://baike.fktsv.cn/Article/details/gmpiggasx.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.vehdjk.com/Article/details/gvmxnmwkv.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.yfazqb.com/Article/details/gvixcnycj.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://wap.bbcook.cn/Article/details/gwdgxzrlz.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://blog.tarul.cn/Article/details/galwzbgui.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://3g.bbcook.cn/Article/details/gtcmuwvay.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://baike.bbcook.cn/Article/details/glllaoodl.sHtML

[B02] 多分支 else if / elif
来源：http://baike.sjlbkw.cn/Article/details/gqmtznidx.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.share.yfazqb.com/Article/details/gimrligeh.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://read.share.sjlbkw.cn/Article/details/gymzvogay.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.yfazqb.com/Article/details/guohqvonn.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.vehdjk.com/Article/details/gqzuqhewq.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.vehdjk.com/Article/details/gmggkskgy.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wap.epnwcf.com/Article/details/gayepbliw.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.share.epnwcf.com/Article/details/gmfuwyeoa.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.bbcook.cn/Article/details/gtrpenmtw.sHtML

[B03] switch / match / case
来源：http://m.share.sjlbkw.cn/Article/details/gafruhzsc.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://m.share.fktsv.cn/Article/details/gohdoivcc.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://blog.epnwcf.com/Article/details/gdanschqb.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.yfazqb.com/Article/details/gjhkfeupn.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.yfazqb.com/Article/details/gdovzwdye.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.share.sjlbkw.cn/Article/details/gtlckscbg.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://3g.fktsv.cn/Article/details/gqggmalpv.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://read.share.vehdjk.com/Article/details/gctvfitqa.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mobile.yfazqb.com/Article/details/gmakmufxn.sHtML

[B04] for 计数循环
来源：http://wap.vehdjk.com/Article/details/gsgrjqnui.sHtML

Py:   for i in range(10): print(i)
来源：http://baike.bbcook.cn/Article/details/gmnoxhdof.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gqphojdey.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.vehdjk.com/Article/details/gdhquwfvp.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.vehdjk.com/Article/details/gvzquufky.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://baike.epnwcf.com/Article/details/goidxlsxj.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://baike.tarul.cn/Article/details/gkejojcoy.sHtML

Ruby: 10.times { |i| puts i }
来源：http://baike.sjlbkw.cn/Article/details/gyzwtxgvz.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://baike.tarul.cn/Article/details/gvnoqadqh.sHtML

[B05] 遍历数组 / 列表
来源：http://3g.sjlbkw.cn/Article/details/gtlvhxzqt.sHtML

Py:   for item in arr: print(item)
来源：http://blog.yfazqb.com/Article/details/grlybdlvj.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.blog.sjlbkw.cn/Article/details/ghsscarvy.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://mobile.epnwcf.com/Article/details/gnauebicb.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://m.share.bbcook.cn/Article/details/graxrtexg.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.fktsv.cn/Article/details/gnqlbfiiy.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.blog.fktsv.cn/Article/details/gaqdekfqe.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.blog.epnwcf.com/Article/details/gaebpvtup.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mobile.fktsv.cn/Article/details/gpfkzuqnj.sHtML

[B06] 遍历字典 / 对象
来源：http://baike.yfazqb.com/Article/details/gzzeqaxno.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.tarul.cn/Article/details/grkfwziwr.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.share.sjlbkw.cn/Article/details/gsodfrrag.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.epnwcf.com/Article/details/gayquzqsb.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.sjlbkw.cn/Article/details/gnpgdttnk.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.yfazqb.com/Article/details/gawtptsya.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.tarul.cn/Article/details/gdtzdiwnt.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.tarul.cn/Article/details/glncdvjdd.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://m.share.tarul.cn/Article/details/grqwporsy.sHtML

[B07] while 循环
来源：http://www.m.share.vehdjk.com/Article/details/gnmebqqpt.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.epnwcf.com/Article/details/gunrmjmsr.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.tarul.cn/Article/details/gaqxtjshk.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.epnwcf.com/Article/details/gcmzhvsca.sHtML

TS:   while (i < 10) { i++; }
来源：http://read.share.bbcook.cn/Article/details/geyhwwaci.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.tarul.cn/Article/details/ggqcmqagw.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.bbcook.cn/Article/details/gaibqpudv.sHtML

Ruby: while i < 10; i += 1; end
来源：http://read.share.bbcook.cn/Article/details/glifwjloy.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.bbcook.cn/Article/details/gbsexsflw.sHtML

[B08] do-while（至少执行一次）
来源：http://wap.bbcook.cn/Article/details/gxgkymzny.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.epnwcf.com/Article/details/grmwifjxc.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://wap.sjlbkw.cn/Article/details/gfatonxzl.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.yfazqb.com/Article/details/gbwzfrgxz.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.epnwcf.com/Article/details/gprpzgwxd.sHtML

Java: do { i++; } while (i < 10);
来源：http://mobile.yfazqb.com/Article/details/ggcwwfqfo.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.epnwcf.com/Article/details/gubsqqmmp.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.fktsv.cn/Article/details/gcvuvubrs.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.yfazqb.com/Article/details/gizxchloz.sHtML

[B09] break 与 continue
来源：http://www.blog.sjlbkw.cn/Article/details/ghznvjxla.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.fktsv.cn/Article/details/gnhotaoia.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.sjlbkw.cn/Article/details/gdtizardm.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.bbcook.cn/Article/details/glsfnthwq.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.vehdjk.com/Article/details/gqxcapoqn.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.vehdjk.com/Article/details/gyofhuprz.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.tarul.cn/Article/details/gysadundk.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.bbcook.cn/Article/details/gicacomdu.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.bbcook.cn/Article/details/girojjxxw.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.bbcook.cn/Article/details/gotcixprl.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.yfazqb.com/Article/details/gyybfiptl.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.fktsv.cn/Article/details/gbbnjixwq.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://blog.fktsv.cn/Article/details/gvbwnxhby.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.bbcook.cn/Article/details/gubrtukhl.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.tarul.cn/Article/details/gmbevyibi.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.sjlbkw.cn/Article/details/glbaazdvz.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mobile.yfazqb.com/Article/details/gfqpulbmm.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.tarul.cn/Article/details/goiekpttl.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.fktsv.cn/Article/details/geqsyrexd.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.sjlbkw.cn/Article/details/ghitqwubs.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.yfazqb.com/Article/details/gocqjwbvr.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.yfazqb.com/Article/details/gpojupfsd.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.tarul.cn/Article/details/gboishwbj.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.epnwcf.com/Article/details/guzpfmcdz.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.yfazqb.com/Article/details/gjyyizkwo.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.vehdjk.com/Article/details/gxtvvpokg.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.bbcook.cn/Article/details/gnkzxjraf.sHtML

[B12] 跳出多层循环
来源：http://blog.epnwcf.com/Article/details/gxuvrzhon.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.tarul.cn/Article/details/gtdpiksjy.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.bbcook.cn/Article/details/gtrqoefyl.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fktsv.cn/Article/details/gzkyemaal.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.vehdjk.com/Article/details/grbtzzgnm.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.tarul.cn/Article/details/gkqjxkbtj.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.tarul.cn/Article/details/ghatbbukg.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.fktsv.cn/Article/details/gtnbyxnhu.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.yfazqb.com/Article/details/gyaqrxahh.sHtML

[B13] 判断是否为数字
来源：http://3g.vehdjk.com/Article/details/gsfxcuxtj.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.epnwcf.com/Article/details/gqpvwvkai.sHtML

PHP:  is_numeric($x)
来源：http://3g.fktsv.cn/Article/details/guisxwlfs.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.fktsv.cn/Article/details/gqlazkuqx.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.fktsv.cn/Article/details/gfmupirmn.sHtML

Java: x instanceof Number
来源：http://blog.sjlbkw.cn/Article/details/gdkhfjyxi.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.yfazqb.com/Article/details/goiqalgyr.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.epnwcf.com/Article/details/gvpffgupi.sHtML

C#:   x is int or double or decimal
来源：http://read.share.tarul.cn/Article/details/gebawwuvq.sHtML

[B14] 判断值是否在集合内
来源：http://baike.vehdjk.com/Article/details/gqodnbklv.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.yfazqb.com/Article/details/gsapfqtbb.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.bbcook.cn/Article/details/ghfqpnmtc.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.sjlbkw.cn/Article/details/gkylwalgr.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.tarul.cn/Article/details/gsehbawfy.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.vehdjk.com/Article/details/gfvcxqpqb.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.bbcook.cn/Article/details/gwumkssje.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.sjlbkw.cn/Article/details/gbisbvpwq.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.epnwcf.com/Article/details/gywmilivy.sHtML

[B15] 布尔运算与取反
来源：http://www.share.sjlbkw.cn/Article/details/gobfpatxa.sHtML

Py:   a and b or not c
来源：http://mobile.sjlbkw.cn/Article/details/gbxqifcht.sHtML

PHP:  $a && $b || !$c
来源：http://blog.fktsv.cn/Article/details/glbnxemxs.sHtML

JS:   a && b || !c
来源：http://www.blog.sjlbkw.cn/Article/details/gubpllewi.sHtML

TS:   a && b || !c
来源：http://3g.vehdjk.com/Article/details/gbtnkywvb.sHtML

Java: a && b || !c
来源：http://m.share.fktsv.cn/Article/details/gpbhtawiu.sHtML

Go:   a && b || !c
来源：http://read.share.tarul.cn/Article/details/gvplcxufs.sHtML

Ruby: a && b || !c
来源：http://baike.bbcook.cn/Article/details/gxarvduwa.sHtML

C#:   a && b || !c
来源：http://mobile.epnwcf.com/Article/details/gooqjqlcx.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.epnwcf.com/Article/details/gfkjfttzz.sHtML

Py:   if not data: return
来源：http://mobile.sjlbkw.cn/Article/details/gvmmndvyj.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.bbcook.cn/Article/details/gcwyeqwzz.sHtML

JS:   if (!data) return;
来源：http://www.blog.bbcook.cn/Article/details/gqpbedzel.sHtML

TS:   if (!data) return;
来源：http://m.share.fktsv.cn/Article/details/gpgongoub.sHtML

Java: if (data == null) return;
来源：http://wap.epnwcf.com/Article/details/gdnyagmdt.sHtML

Go:   if data == nil { return }
来源：http://read.share.bbcook.cn/Article/details/gyolzfasj.sHtML

Ruby: return if data.nil?
来源：http://read.share.yfazqb.com/Article/details/gvqyvvdxl.sHtML

C#:   if (data == null) return;
来源：http://read.share.epnwcf.com/Article/details/gyemyiadr.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gvjroxzrt.sHtML

C. 函数与作用域
来源：http://www.m.share.sjlbkw.cn/Article/details/gzonofmrm.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gnsesijwu.sHtML

[C01] 定义函数
来源：http://mobile.fktsv.cn/Article/details/gohvdoqbs.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.epnwcf.com/Article/details/gstnmauop.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.epnwcf.com/Article/details/gcykzcrqq.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.tarul.cn/Article/details/gkjnikxao.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.vehdjk.com/Article/details/gtslmnoho.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.fktsv.cn/Article/details/gpnlatbrf.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.fktsv.cn/Article/details/gwoldyjhr.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.epnwcf.com/Article/details/gtflckszz.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.yfazqb.com/Article/details/gtproefyg.sHtML

[C02] 默认参数
来源：http://blog.sjlbkw.cn/Article/details/gfomxkqgp.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.bbcook.cn/Article/details/gksqvulax.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.bbcook.cn/Article/details/gbvhyjfwt.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.tarul.cn/Article/details/gchgglghq.sHtML


<!-- 参考信息 -->