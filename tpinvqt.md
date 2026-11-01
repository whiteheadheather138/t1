代发 wailian999

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://mobile.bbcook.cn/Article/details/gyvuqbisi.sHtML

JS:   `Hello, ${name}!`
来源：http://blog.tarul.cn/Article/details/giapqrnjc.sHtML

TS:   `Hello, ${name}!`
来源：http://m.share.yfazqb.com/Article/details/gvqgknwgj.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://wap.tarul.cn/Article/details/gqsbbleix.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://read.share.fktsv.cn/Article/details/giauldoxc.sHtML

Ruby: "Hello, #{name}!"
来源：http://wap.sjlbkw.cn/Article/details/gdztydijx.sHtML

C#:   $"Hello, {name}!"
来源：http://wap.vehdjk.com/Article/details/gzsfsnarr.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.share.sjlbkw.cn/Article/details/gutrjxeho.sHtML

Py:   "第一行\n第二行"
来源：http://3g.vehdjk.com/Article/details/gpulyvioi.sHtML

PHP:  "第一行\n第二行"
来源：http://mobile.yfazqb.com/Article/details/gwxrbnoke.sHtML

JS:   "第一行\n第二行"
来源：http://blog.vehdjk.com/Article/details/gcemrulfu.sHtML

TS:   "第一行\n第二行"
来源：http://mobile.bbcook.cn/Article/details/gtbwptlyi.sHtML

Java: "第一行\n第二行"
来源：http://read.share.epnwcf.com/Article/details/glecymegf.sHtML

Go:   "第一行\n第二行"
来源：http://baike.sjlbkw.cn/Article/details/glpidiraa.sHtML

Ruby: "第一行\n第二行"
来源：http://read.share.sjlbkw.cn/Article/details/gzdipmmvg.sHtML

C#:   "第一行\n第二行"
来源：http://mobile.tarul.cn/Article/details/gqgwfarsw.sHtML

[A14] 注释写法
来源：http://www.m.share.sjlbkw.cn/Article/details/gjoophkls.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.m.share.epnwcf.com/Article/details/gogqjgwjx.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://blog.sjlbkw.cn/Article/details/gatxxxiwt.sHtML

JS:   // 单行；/* 多行 */
来源：http://wap.vehdjk.com/Article/details/gkfoahfeu.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.share.sjlbkw.cn/Article/details/gxkxhclqf.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://3g.bbcook.cn/Article/details/gymfmwisf.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.m.share.fktsv.cn/Article/details/gtbzrusyt.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://read.share.vehdjk.com/Article/details/gqbsevysk.sHtML

C#:   // 单行；/* 多行 */
来源：http://wap.bbcook.cn/Article/details/ggyattflo.sHtML

[A15] 空值判断与默认值
来源：http://mobile.vehdjk.com/Article/details/gansvadzj.sHtML

Py:   value = data or "默认值"
来源：http://www.m.share.fktsv.cn/Article/details/gusztcljc.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://baike.fktsv.cn/Article/details/gvnukoygt.sHtML

JS:   const value = data ?? "默认值";
来源：http://m.share.bbcook.cn/Article/details/gnbougcel.sHtML

TS:   const value = data ?? "默认值";
来源：http://wap.fktsv.cn/Article/details/gaezmzvpy.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://blog.epnwcf.com/Article/details/glthwfrkc.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://m.share.sjlbkw.cn/Article/details/ghwbqxkll.sHtML

Ruby: value = data || "默认值"
来源：http://blog.yfazqb.com/Article/details/gglacogjy.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.m.share.vehdjk.com/Article/details/geskwtwar.sHtML

[A16] 真假值判断规则
来源：http://wap.tarul.cn/Article/details/gnygxynab.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://3g.sjlbkw.cn/Article/details/gakgpufnp.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.share.vehdjk.com/Article/details/gtsvhyzdw.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.blog.bbcook.cn/Article/details/gpmqymsir.sHtML

TS:   if (!x) {}
来源：http://3g.bbcook.cn/Article/details/gfemltwbl.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.m.share.epnwcf.com/Article/details/ghutaxuol.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://3g.epnwcf.com/Article/details/gnpqeqgvy.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://baike.sjlbkw.cn/Article/details/gpntoeshv.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mobile.bbcook.cn/Article/details/gtrmynico.sHtML

[A17] 位运算
来源：http://www.blog.fktsv.cn/Article/details/gyqyvknpm.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.yfazqb.com/Article/details/gkhwkvwwh.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://baike.bbcook.cn/Article/details/gxygfkwpc.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.yfazqb.com/Article/details/gszkrouxz.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://m.share.vehdjk.com/Article/details/gosipaoss.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.sjlbkw.cn/Article/details/gjbveashn.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.m.share.epnwcf.com/Article/details/gankeigij.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.fktsv.cn/Article/details/gsmhbogkt.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.bbcook.cn/Article/details/ggasotjbe.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.blog.fktsv.cn/Article/details/gvflwivmw.sHtML

Py:   ord("A"); chr(65)
来源：http://www.m.share.epnwcf.com/Article/details/gsazdmeli.sHtML

PHP:  ord("A"); chr(65)
来源：http://m.share.yfazqb.com/Article/details/gukdjhwgx.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.m.share.epnwcf.com/Article/details/glztfbjav.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.m.share.tarul.cn/Article/details/gdgwepryj.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.share.tarul.cn/Article/details/gqiiewehh.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://baike.vehdjk.com/Article/details/gmjhhldad.sHtML

Ruby: "A".ord; 65.chr
来源：http://wap.yfazqb.com/Article/details/gznllfdql.sHtML

C#:   (int)'A'; (char)65
来源：http://mobile.sjlbkw.cn/Article/details/gpzswydbv.sHtML

[A19] 交换两个变量
来源：http://blog.sjlbkw.cn/Article/details/gwnkzkfor.sHtML

Py:   a, b = b, a
来源：http://www.blog.bbcook.cn/Article/details/gzdbrvltu.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://3g.epnwcf.com/Article/details/gwabojccc.sHtML

JS:   [a, b] = [b, a];
来源：http://m.share.yfazqb.com/Article/details/gmpvyuwit.sHtML

TS:   [a, b] = [b, a];
来源：http://mobile.vehdjk.com/Article/details/gztqqhbxb.sHtML

Java: int t = a; a = b; b = t;
来源：http://blog.epnwcf.com/Article/details/gendbyrho.sHtML

Go:   a, b = b, a
来源：http://wap.yfazqb.com/Article/details/gjahdsrtk.sHtML

Ruby: a, b = b, a
来源：http://blog.tarul.cn/Article/details/gystoyfbt.sHtML

C#:   (a, b) = (b, a);
来源：http://www.blog.bbcook.cn/Article/details/gkzkyumvx.sHtML

[A20] 读取标准输入
来源：http://www.share.bbcook.cn/Article/details/gjuheoulk.sHtML

Py:   name = input("请输入：")
来源：http://read.share.vehdjk.com/Article/details/gwxinintx.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.blog.yfazqb.com/Article/details/ghpqunuhe.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://read.share.bbcook.cn/Article/details/ggjtawhap.sHtML

TS:   // Node.js：readline 模块
来源：http://baike.fktsv.cn/Article/details/garnaclel.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.m.share.vehdjk.com/Article/details/gihrcyglu.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://3g.tarul.cn/Article/details/gbfikmuco.sHtML

Ruby: gets.chomp
来源：http://www.blog.epnwcf.com/Article/details/gdwjrqhue.sHtML

C#:   Console.ReadLine();
来源：http://wap.tarul.cn/Article/details/gfphxinmv.sHtML

[A21] 保留指定小数位输出
来源：http://mobile.epnwcf.com/Article/details/gekhzoloz.sHtML

Py:   f"{3.14159:.2f}"
来源：http://blog.tarul.cn/Article/details/gacpeavxk.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://blog.yfazqb.com/Article/details/ghdujazru.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.blog.sjlbkw.cn/Article/details/gezabwwdw.sHtML

TS:   (3.14159).toFixed(2)
来源：http://read.share.vehdjk.com/Article/details/gsohmrpvd.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://read.share.tarul.cn/Article/details/gjwbtvzqt.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.share.yfazqb.com/Article/details/gdireauqu.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.blog.bbcook.cn/Article/details/guuauiigo.sHtML

C#:   3.14159.ToString("F2")
来源：http://baike.sjlbkw.cn/Article/details/gxrmdsurr.sHtML

[A22] 获取字符串长度
来源：http://baike.bbcook.cn/Article/details/gsuohtkru.sHtML

Py:   len(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtxcegqbm.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://blog.bbcook.cn/Article/details/gymfumass.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mobile.bbcook.cn/Article/details/gqqxmgbbx.sHtML

TS:   s.length
来源：http://m.share.fktsv.cn/Article/details/gclumhbyk.sHtML

Java: s.length()
来源：http://mobile.yfazqb.com/Article/details/gxomgguak.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://3g.epnwcf.com/Article/details/goycrmksu.sHtML

Ruby: s.length
来源：http://read.share.tarul.cn/Article/details/gaysvjhoe.sHtML

C#:   s.Length
来源：http://www.share.epnwcf.com/Article/details/gifxsqggd.sHtML

[A23] 大小写转换
来源：http://blog.epnwcf.com/Article/details/gfkldpjjw.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.m.share.sjlbkw.cn/Article/details/gsbwasdqn.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wap.bbcook.cn/Article/details/gkzlkjwma.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.vehdjk.com/Article/details/gihmclyxc.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.bbcook.cn/Article/details/grzotkcdy.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.yfazqb.com/Article/details/gacqlwjdd.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://read.share.yfazqb.com/Article/details/gdbpolxeh.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mobile.fktsv.cn/Article/details/grfreuwle.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://blog.bbcook.cn/Article/details/gaptfwcnx.sHtML

[A24] 去除首尾空白
来源：http://www.blog.bbcook.cn/Article/details/gpwjnbqve.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://blog.sjlbkw.cn/Article/details/gazjbkeeo.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://blog.epnwcf.com/Article/details/gqblwrggu.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.bbcook.cn/Article/details/gqwcaogjo.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.epnwcf.com/Article/details/gfoxhcdfl.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.share.tarul.cn/Article/details/ghvwtyicw.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.share.vehdjk.com/Article/details/gymxvidrw.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://m.share.tarul.cn/Article/details/gvmeanuhl.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://read.share.vehdjk.com/Article/details/gbrfnqlnf.sHtML

[A25] 字符串比较
来源：http://wap.bbcook.cn/Article/details/gfbbrbduk.sHtML

Py:   s1 == s2; s1 != s2
来源：http://blog.yfazqb.com/Article/details/gitzobrkd.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://read.share.yfazqb.com/Article/details/gukmnvvml.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.tarul.cn/Article/details/grncsvgrj.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.sjlbkw.cn/Article/details/gwmkguyeh.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.share.fktsv.cn/Article/details/goewlgvvm.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://3g.epnwcf.com/Article/details/gfjkbaoet.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://baike.tarul.cn/Article/details/gzbhslsbr.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.blog.vehdjk.com/Article/details/gqfzdphkf.sHtML

[A26] 类型转换总览
来源：http://blog.fktsv.cn/Article/details/gkffhxxkp.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.blog.vehdjk.com/Article/details/geoyvjssv.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.blog.epnwcf.com/Article/details/gwjqvoatl.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.m.share.fktsv.cn/Article/details/gjdzhitzc.sHtML

TS:   Number() String() Boolean() x as number
来源：http://baike.sjlbkw.cn/Article/details/gkgfriqbi.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://3g.sjlbkw.cn/Article/details/gunhxymia.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.share.yfazqb.com/Article/details/gszmsdhsa.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://mobile.fktsv.cn/Article/details/gvsfeiauw.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://blog.tarul.cn/Article/details/gyrrjiysb.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gvnblfoey.sHtML

B. 流程控制
来源：http://mobile.yfazqb.com/Article/details/gwijsygtc.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gindnoqmg.sHtML

[B01] 条件判断 if / else
来源：http://wap.fktsv.cn/Article/details/ghwhixogv.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.blog.bbcook.cn/Article/details/gxkgxknpz.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.m.share.tarul.cn/Article/details/gmfkxudfi.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.fktsv.cn/Article/details/gyofxeuht.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.sjlbkw.cn/Article/details/gnihqpvra.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://read.share.fktsv.cn/Article/details/gtttzykly.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://blog.bbcook.cn/Article/details/gxsyuiizk.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://3g.sjlbkw.cn/Article/details/gyegfsypc.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.share.bbcook.cn/Article/details/gfswlwsww.sHtML

[B02] 多分支 else if / elif
来源：http://blog.epnwcf.com/Article/details/gdokgrpwg.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://baike.bbcook.cn/Article/details/gedwlrwyu.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.share.fktsv.cn/Article/details/gdpgkduek.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.tarul.cn/Article/details/gfebcbitw.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.vehdjk.com/Article/details/gwhuofspn.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.tarul.cn/Article/details/gthutonkr.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://m.share.tarul.cn/Article/details/geyinsqcq.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wap.tarul.cn/Article/details/gwvojgner.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.bbcook.cn/Article/details/gmmkgyzvk.sHtML

[B03] switch / match / case
来源：http://mobile.vehdjk.com/Article/details/gtzcdifcb.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.blog.fktsv.cn/Article/details/gnaqnpbdt.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://baike.epnwcf.com/Article/details/gahzkzuzf.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.fktsv.cn/Article/details/grpfwdffs.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.epnwcf.com/Article/details/gfxqowflb.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://read.share.epnwcf.com/Article/details/gbxdgmvlz.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mobile.tarul.cn/Article/details/grldyjxtf.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://3g.yfazqb.com/Article/details/gorvuioee.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.share.bbcook.cn/Article/details/gimdheede.sHtML

[B04] for 计数循环
来源：http://wap.epnwcf.com/Article/details/gsjrzcfbw.sHtML

Py:   for i in range(10): print(i)
来源：http://www.m.share.yfazqb.com/Article/details/gwtbbqklm.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.share.epnwcf.com/Article/details/gzgbzobzi.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.bbcook.cn/Article/details/glbwhzbfi.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.sjlbkw.cn/Article/details/guczsfdjl.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.blog.fktsv.cn/Article/details/gddlckasw.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.blog.bbcook.cn/Article/details/gbbcanhti.sHtML

Ruby: 10.times { |i| puts i }
来源：http://wap.sjlbkw.cn/Article/details/ginvzeezh.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.share.tarul.cn/Article/details/gkxyqmwxb.sHtML

[B05] 遍历数组 / 列表
来源：http://www.share.yfazqb.com/Article/details/gkfibupps.sHtML

Py:   for item in arr: print(item)
来源：http://www.share.tarul.cn/Article/details/goiqxmvov.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://m.share.bbcook.cn/Article/details/gefypkqcy.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.epnwcf.com/Article/details/gymtzhugs.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.tarul.cn/Article/details/gfwpbjxok.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.fktsv.cn/Article/details/guahogkzn.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wap.yfazqb.com/Article/details/gztqniwdu.sHtML

Ruby: arr.each { |item| puts item }
来源：http://baike.tarul.cn/Article/details/gwmhrhphx.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://read.share.fktsv.cn/Article/details/gqptnzqrv.sHtML

[B06] 遍历字典 / 对象
来源：http://mobile.sjlbkw.cn/Article/details/gfjtnvtzj.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://m.share.tarul.cn/Article/details/gvtnklbjj.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.share.bbcook.cn/Article/details/gmudnfkrs.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.bbcook.cn/Article/details/gxlvclcnh.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.vehdjk.com/Article/details/glqpgslkh.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.blog.bbcook.cn/Article/details/glsghjnfj.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://m.share.yfazqb.com/Article/details/gbxoozrcq.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.bbcook.cn/Article/details/gcuclmhuj.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.epnwcf.com/Article/details/gpdfoslku.sHtML

[B07] while 循环
来源：http://blog.bbcook.cn/Article/details/gsxrtdboo.sHtML

Py:   while i < 10: i += 1
来源：http://blog.fktsv.cn/Article/details/gcodgrtsn.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.blog.fktsv.cn/Article/details/grhwmiptr.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.epnwcf.com/Article/details/gnvljhdkn.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.bbcook.cn/Article/details/gpqbpfwuk.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.sjlbkw.cn/Article/details/ggbjljuql.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wap.bbcook.cn/Article/details/gexmgipok.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.tarul.cn/Article/details/gpmivfmxg.sHtML

C#:   while (i < 10) { i++; }
来源：http://m.share.epnwcf.com/Article/details/gojkwofvo.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.fktsv.cn/Article/details/gcwkeovsp.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.epnwcf.com/Article/details/guwyerxrg.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.fktsv.cn/Article/details/gqurktwbw.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.m.share.yfazqb.com/Article/details/glyahnigf.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.bbcook.cn/Article/details/gfidpazeb.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.epnwcf.com/Article/details/ggtrwsswf.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.vehdjk.com/Article/details/grntngcew.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.bbcook.cn/Article/details/gejuqgmyf.sHtML

C#:   do { i++; } while (i < 10);
来源：http://mobile.epnwcf.com/Article/details/gzfwbnupy.sHtML

[B09] break 与 continue
来源：http://wap.sjlbkw.cn/Article/details/gmgkajbrg.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.sjlbkw.cn/Article/details/gktrnqsjx.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.fktsv.cn/Article/details/gpiisabvv.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.bbcook.cn/Article/details/gcpuwzzqo.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.tarul.cn/Article/details/gcbwjptcc.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.bbcook.cn/Article/details/gmbtagwrz.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.tarul.cn/Article/details/ggpxznxox.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.sjlbkw.cn/Article/details/ggtrohpyu.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.tarul.cn/Article/details/gjqkrpbsn.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.vehdjk.com/Article/details/gfnnaiufg.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.vehdjk.com/Article/details/gaqeozthv.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.tarul.cn/Article/details/gueqvtlkn.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.tarul.cn/Article/details/gnzfwouws.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.bbcook.cn/Article/details/gyvztpbhp.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.tarul.cn/Article/details/ggxapblku.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.sjlbkw.cn/Article/details/ghckniilv.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.sjlbkw.cn/Article/details/gjgszwaaf.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.sjlbkw.cn/Article/details/gyfgzwjyf.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.blog.vehdjk.com/Article/details/gkxjbagdf.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.sjlbkw.cn/Article/details/gaicvohin.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.bbcook.cn/Article/details/gjzonylgw.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.yfazqb.com/Article/details/gsocrytrj.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.yfazqb.com/Article/details/guodopivo.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.tarul.cn/Article/details/gwkcrkjga.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.fktsv.cn/Article/details/gdzgncgqr.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.epnwcf.com/Article/details/grpotnoau.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.tarul.cn/Article/details/gjzfdchbq.sHtML

[B12] 跳出多层循环
来源：http://3g.bbcook.cn/Article/details/giudxvdoe.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.sjlbkw.cn/Article/details/godhslmjk.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.bbcook.cn/Article/details/gzgjgdbfi.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.epnwcf.com/Article/details/gajavdukn.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.yfazqb.com/Article/details/gamtftcvp.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.bbcook.cn/Article/details/gcczgogxf.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.vehdjk.com/Article/details/ghhdaykki.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.bbcook.cn/Article/details/gcjlrcpsg.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.tarul.cn/Article/details/gutxgvghv.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.epnwcf.com/Article/details/geuptegnl.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.tarul.cn/Article/details/gostjyfcp.sHtML

PHP:  is_numeric($x)
来源：http://read.share.yfazqb.com/Article/details/golvekpgh.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.tarul.cn/Article/details/gpqjhmjun.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.vehdjk.com/Article/details/gmdfbcafi.sHtML

Java: x instanceof Number
来源：http://3g.sjlbkw.cn/Article/details/gwltrcrbs.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.bbcook.cn/Article/details/gjjolpljy.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.fktsv.cn/Article/details/gfzttfzto.sHtML

C#:   x is int or double or decimal
来源：http://mobile.yfazqb.com/Article/details/gfzslgcmk.sHtML

[B14] 判断值是否在集合内
来源：http://baike.bbcook.cn/Article/details/gkaksmphd.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.fktsv.cn/Article/details/gkacaienx.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.epnwcf.com/Article/details/gblsihuwd.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.tarul.cn/Article/details/gbomwbjrd.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.epnwcf.com/Article/details/gvonfqaul.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.yfazqb.com/Article/details/gbsjixnms.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.tarul.cn/Article/details/gexagqnmn.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.epnwcf.com/Article/details/gxypewfta.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.vehdjk.com/Article/details/gwlqpckai.sHtML

[B15] 布尔运算与取反
来源：http://m.share.epnwcf.com/Article/details/gnywcbvpu.sHtML

Py:   a and b or not c
来源：http://www.m.share.sjlbkw.cn/Article/details/gqirzljuu.sHtML

PHP:  $a && $b || !$c
来源：http://blog.vehdjk.com/Article/details/gzkocfize.sHtML

JS:   a && b || !c
来源：http://wap.bbcook.cn/Article/details/gchocpqgn.sHtML

TS:   a && b || !c
来源：http://blog.tarul.cn/Article/details/gxaodlblr.sHtML

Java: a && b || !c
来源：http://m.share.tarul.cn/Article/details/gvbkcsbtc.sHtML

Go:   a && b || !c
来源：http://www.m.share.sjlbkw.cn/Article/details/gvjjscuuv.sHtML

Ruby: a && b || !c
来源：http://www.share.yfazqb.com/Article/details/gxjtoshvq.sHtML

C#:   a && b || !c
来源：http://www.blog.bbcook.cn/Article/details/gexxyftrw.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.bbcook.cn/Article/details/graqgdakn.sHtML

Py:   if not data: return
来源：http://www.m.share.fktsv.cn/Article/details/gtmslbkhc.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.tarul.cn/Article/details/gakdabzja.sHtML

JS:   if (!data) return;
来源：http://www.blog.vehdjk.com/Article/details/gvinnaxyb.sHtML

TS:   if (!data) return;
来源：http://baike.vehdjk.com/Article/details/gubguhhgu.sHtML

Java: if (data == null) return;
来源：http://www.m.share.bbcook.cn/Article/details/gymiqpgmk.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.epnwcf.com/Article/details/gmkssgaba.sHtML

Ruby: return if data.nil?
来源：http://www.share.sjlbkw.cn/Article/details/ghwhrmfuf.sHtML

C#:   if (data == null) return;
来源：http://baike.bbcook.cn/Article/details/gfmhjguhc.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/ggvntbnrj.sHtML

C. 函数与作用域
来源：http://m.share.tarul.cn/Article/details/gueyuzfwz.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/ggbnnfzgr.sHtML

[C01] 定义函数
来源：http://www.m.share.yfazqb.com/Article/details/gufxgkrqy.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.fktsv.cn/Article/details/gkuphboes.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.yfazqb.com/Article/details/gxkrdsgez.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.vehdjk.com/Article/details/grehhfaqx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.tarul.cn/Article/details/gqbpmrgch.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.epnwcf.com/Article/details/gspbxlnzu.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.sjlbkw.cn/Article/details/gstsssoku.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.yfazqb.com/Article/details/gzctucrri.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.bbcook.cn/Article/details/gpjrhmvce.sHtML

[C02] 默认参数
来源：http://3g.epnwcf.com/Article/details/gjdbvpaem.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.tarul.cn/Article/details/gsevhukcz.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.yfazqb.com/Article/details/gaafetqxh.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.fktsv.cn/Article/details/gimubtduv.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.bbcook.cn/Article/details/gbsvnukif.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.vehdjk.com/Article/details/gzphibhwe.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.yfazqb.com/Article/details/gdaskzzni.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.yfazqb.com/Article/details/gsztftqse.sHtML


<!-- 参考信息 -->