代发 wailian999

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wap.fktsv.cn/Article/details/gzarmmozp.sHtML

Ruby: "Hello, #{name}!"
来源：http://mobile.bbcook.cn/Article/details/gjberoqju.sHtML

C#:   $"Hello, {name}!"
来源：http://mobile.yfazqb.com/Article/details/gizvgjnls.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://3g.vehdjk.com/Article/details/ghitcvfpv.sHtML

Py:   "第一行\n第二行"
来源：http://read.share.bbcook.cn/Article/details/guetvpxpy.sHtML

PHP:  "第一行\n第二行"
来源：http://www.share.bbcook.cn/Article/details/gpbpvmjhr.sHtML

JS:   "第一行\n第二行"
来源：http://wap.fktsv.cn/Article/details/giirwktuc.sHtML

TS:   "第一行\n第二行"
来源：http://3g.yfazqb.com/Article/details/gicoxflsn.sHtML

Java: "第一行\n第二行"
来源：http://baike.fktsv.cn/Article/details/gaiwyfewd.sHtML

Go:   "第一行\n第二行"
来源：http://3g.fktsv.cn/Article/details/gntmyktae.sHtML

Ruby: "第一行\n第二行"
来源：http://read.share.bbcook.cn/Article/details/gbsxngizw.sHtML

C#:   "第一行\n第二行"
来源：http://wap.vehdjk.com/Article/details/gvpbokfnv.sHtML

[A14] 注释写法
来源：http://blog.yfazqb.com/Article/details/gyvvdalsy.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://blog.yfazqb.com/Article/details/gbftzwkfe.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.m.share.fktsv.cn/Article/details/gdsjxnlza.sHtML

JS:   // 单行；/* 多行 */
来源：http://read.share.sjlbkw.cn/Article/details/gyexgxkzs.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.share.sjlbkw.cn/Article/details/gvblpgidj.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.m.share.bbcook.cn/Article/details/gpxuwkoud.sHtML

Go:   // 单行；/* 多行 */
来源：http://blog.tarul.cn/Article/details/ghdhqkwzv.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://read.share.vehdjk.com/Article/details/gvvruyuai.sHtML

C#:   // 单行；/* 多行 */
来源：http://m.share.yfazqb.com/Article/details/grntqmjxe.sHtML

[A15] 空值判断与默认值
来源：http://wap.bbcook.cn/Article/details/gzlisotym.sHtML

Py:   value = data or "默认值"
来源：http://mobile.sjlbkw.cn/Article/details/gxjyeaoam.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://mobile.sjlbkw.cn/Article/details/grbvtvnes.sHtML

JS:   const value = data ?? "默认值";
来源：http://read.share.yfazqb.com/Article/details/ghishpuuh.sHtML

TS:   const value = data ?? "默认值";
来源：http://mobile.yfazqb.com/Article/details/gzgrrsqrk.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://read.share.bbcook.cn/Article/details/gyaubaziv.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.share.fktsv.cn/Article/details/gafwjxqlc.sHtML

Ruby: value = data || "默认值"
来源：http://wap.epnwcf.com/Article/details/gtfaxqqil.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.share.sjlbkw.cn/Article/details/grsnzozez.sHtML

[A16] 真假值判断规则
来源：http://baike.yfazqb.com/Article/details/gcuvpgjes.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.blog.epnwcf.com/Article/details/gjmdbyhfo.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.share.sjlbkw.cn/Article/details/gcjamriey.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://baike.tarul.cn/Article/details/gjqlzonsp.sHtML

TS:   if (!x) {}
来源：http://www.blog.bbcook.cn/Article/details/gwrzcnaao.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://blog.yfazqb.com/Article/details/gmqwylqyu.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://read.share.sjlbkw.cn/Article/details/gnfzznzgq.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://baike.bbcook.cn/Article/details/gkhhwlaua.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://3g.sjlbkw.cn/Article/details/gikqlroqr.sHtML

[A17] 位运算
来源：http://www.share.sjlbkw.cn/Article/details/gvqbyiygs.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.yfazqb.com/Article/details/gcceyjsmy.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://baike.sjlbkw.cn/Article/details/ghfkrhzak.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.tarul.cn/Article/details/gevxkafil.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wap.yfazqb.com/Article/details/gmjxwtxlw.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.tarul.cn/Article/details/gzgkhbksx.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://m.share.fktsv.cn/Article/details/gkxdjtzuf.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.tarul.cn/Article/details/gihwdcjhd.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fktsv.cn/Article/details/gdmtlmpwp.sHtML

[A18] 字符与 ASCII 码互转
来源：http://3g.epnwcf.com/Article/details/gseojhjnk.sHtML

Py:   ord("A"); chr(65)
来源：http://blog.yfazqb.com/Article/details/ghjurgufp.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.m.share.epnwcf.com/Article/details/gddpaorrh.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.sjlbkw.cn/Article/details/gpynfiysc.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.tarul.cn/Article/details/ggrbqzudk.sHtML

Java: (int) 'A'; (char) 65
来源：http://read.share.vehdjk.com/Article/details/gwkweermx.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://baike.bbcook.cn/Article/details/gpumyewuk.sHtML

Ruby: "A".ord; 65.chr
来源：http://read.share.vehdjk.com/Article/details/gdzaxmgty.sHtML

C#:   (int)'A'; (char)65
来源：http://baike.yfazqb.com/Article/details/gtpjrxdkp.sHtML

[A19] 交换两个变量
来源：http://3g.tarul.cn/Article/details/gldyrrwtw.sHtML

Py:   a, b = b, a
来源：http://blog.epnwcf.com/Article/details/gtkkyweny.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://wap.bbcook.cn/Article/details/gvgotgyxg.sHtML

JS:   [a, b] = [b, a];
来源：http://read.share.bbcook.cn/Article/details/gkkknlgdf.sHtML

TS:   [a, b] = [b, a];
来源：http://mobile.bbcook.cn/Article/details/gafqdklgh.sHtML

Java: int t = a; a = b; b = t;
来源：http://m.share.bbcook.cn/Article/details/gwddkxvhd.sHtML

Go:   a, b = b, a
来源：http://www.m.share.sjlbkw.cn/Article/details/ghlotyexi.sHtML

Ruby: a, b = b, a
来源：http://m.share.epnwcf.com/Article/details/grjzvxona.sHtML

C#:   (a, b) = (b, a);
来源：http://baike.fktsv.cn/Article/details/gpnmxwjpe.sHtML

[A20] 读取标准输入
来源：http://m.share.tarul.cn/Article/details/ghaokvlzg.sHtML

Py:   name = input("请输入：")
来源：http://3g.epnwcf.com/Article/details/gvgirmqyj.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://m.share.bbcook.cn/Article/details/gnsuybqku.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://read.share.fktsv.cn/Article/details/genghntam.sHtML

TS:   // Node.js：readline 模块
来源：http://baike.yfazqb.com/Article/details/gmtiyhfjn.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://m.share.yfazqb.com/Article/details/gjztmkgpj.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://mobile.bbcook.cn/Article/details/glzmibdwb.sHtML

Ruby: gets.chomp
来源：http://3g.fktsv.cn/Article/details/grufzlnhz.sHtML

C#:   Console.ReadLine();
来源：http://wap.epnwcf.com/Article/details/gtgkvdvmq.sHtML

[A21] 保留指定小数位输出
来源：http://read.share.epnwcf.com/Article/details/gimvdulvs.sHtML

Py:   f"{3.14159:.2f}"
来源：http://blog.bbcook.cn/Article/details/gukqnydhk.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.share.sjlbkw.cn/Article/details/ghasozvjv.sHtML

JS:   (3.14159).toFixed(2)
来源：http://blog.sjlbkw.cn/Article/details/gzkqfwgck.sHtML

TS:   (3.14159).toFixed(2)
来源：http://3g.bbcook.cn/Article/details/gctgckrqx.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://blog.sjlbkw.cn/Article/details/glgbcxhbs.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.m.share.vehdjk.com/Article/details/godhbrgmt.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.blog.bbcook.cn/Article/details/ggbbqtxmr.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.share.fktsv.cn/Article/details/gqzwfwmaw.sHtML

[A22] 获取字符串长度
来源：http://blog.fktsv.cn/Article/details/gjsztgski.sHtML

Py:   len(s)
来源：http://wap.bbcook.cn/Article/details/gifpfkhqg.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mobile.yfazqb.com/Article/details/grknsgtyf.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.blog.sjlbkw.cn/Article/details/gxxnbfxuu.sHtML

TS:   s.length
来源：http://baike.epnwcf.com/Article/details/ggpymcvht.sHtML

Java: s.length()
来源：http://m.share.sjlbkw.cn/Article/details/gvqrhvdkl.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://m.share.epnwcf.com/Article/details/gnqbyzrru.sHtML

Ruby: s.length
来源：http://blog.yfazqb.com/Article/details/gzzqqvgfw.sHtML

C#:   s.Length
来源：http://wap.vehdjk.com/Article/details/gcuukrqbo.sHtML

[A23] 大小写转换
来源：http://mobile.fktsv.cn/Article/details/gpzrlbnjy.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://read.share.tarul.cn/Article/details/gprtzjvcb.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.m.share.fktsv.cn/Article/details/gvxoknkfj.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.bbcook.cn/Article/details/gclxgwwvr.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.yfazqb.com/Article/details/gykbzjtwr.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.yfazqb.com/Article/details/gfafbfgef.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://3g.yfazqb.com/Article/details/gckczstjr.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wap.epnwcf.com/Article/details/grskopnbl.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://m.share.yfazqb.com/Article/details/gxvqkuwtt.sHtML

[A24] 去除首尾空白
来源：http://www.blog.fktsv.cn/Article/details/gcntukvqm.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://blog.sjlbkw.cn/Article/details/glciodypd.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wap.vehdjk.com/Article/details/gweyecizo.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.bbcook.cn/Article/details/ghqbnmyvq.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.sjlbkw.cn/Article/details/goefglhnn.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://m.share.fktsv.cn/Article/details/gxbhhwiks.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.m.share.fktsv.cn/Article/details/gfajtaqcn.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mobile.fktsv.cn/Article/details/gazyxftye.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mobile.yfazqb.com/Article/details/gjlrjcjrg.sHtML

[A25] 字符串比较
来源：http://www.blog.vehdjk.com/Article/details/gpfdmmyfp.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.share.vehdjk.com/Article/details/gtokobmtm.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://m.share.sjlbkw.cn/Article/details/gbigptqnv.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.sjlbkw.cn/Article/details/gvubsxjtu.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.epnwcf.com/Article/details/gzujorkdq.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://blog.sjlbkw.cn/Article/details/gybcdpnvd.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wap.vehdjk.com/Article/details/gelvvgfmg.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://baike.fktsv.cn/Article/details/gjcdlnckf.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://baike.bbcook.cn/Article/details/gettlzjdq.sHtML

[A26] 类型转换总览
来源：http://3g.vehdjk.com/Article/details/gjgnqqbzv.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://3g.vehdjk.com/Article/details/gwhqbewoo.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://m.share.fktsv.cn/Article/details/gvipkimgj.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://read.share.tarul.cn/Article/details/gtpghcpyq.sHtML

TS:   Number() String() Boolean() x as number
来源：http://read.share.yfazqb.com/Article/details/gxhvrgrgf.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://m.share.bbcook.cn/Article/details/gbqzdkyfh.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://3g.yfazqb.com/Article/details/gkiaqnylt.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://baike.fktsv.cn/Article/details/gnxjvqerp.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.share.tarul.cn/Article/details/gsztwmejp.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gcbyqpqju.sHtML

B. 流程控制
来源：http://baike.fktsv.cn/Article/details/gftrzhnta.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gerjvfmlg.sHtML

[B01] 条件判断 if / else
来源：http://blog.yfazqb.com/Article/details/ggomsqxyd.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://read.share.bbcook.cn/Article/details/gocwjjswy.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mobile.yfazqb.com/Article/details/gbyibegvq.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.tarul.cn/Article/details/gmtlscopz.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.fktsv.cn/Article/details/gckqytrtz.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://blog.fktsv.cn/Article/details/gqglgjjds.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.m.share.fktsv.cn/Article/details/gwnsfdpxv.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mobile.tarul.cn/Article/details/gmmmwkfoz.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://baike.tarul.cn/Article/details/gmxysnftq.sHtML

[B02] 多分支 else if / elif
来源：http://m.share.bbcook.cn/Article/details/gkmajnltw.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://3g.fktsv.cn/Article/details/gwfpznrii.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.m.share.bbcook.cn/Article/details/gqztmeabr.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.tarul.cn/Article/details/gyeapszpi.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.vehdjk.com/Article/details/gnuwxazma.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.sjlbkw.cn/Article/details/gqfdmpzhc.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mobile.vehdjk.com/Article/details/guqkxfejg.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://m.share.epnwcf.com/Article/details/gjrzroywa.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.sjlbkw.cn/Article/details/gxrccahts.sHtML

[B03] switch / match / case
来源：http://www.share.tarul.cn/Article/details/gnrgwpnet.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://baike.vehdjk.com/Article/details/gcphvqkoz.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wap.tarul.cn/Article/details/gnevgegtd.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.vehdjk.com/Article/details/gvocziluz.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.fktsv.cn/Article/details/gaznxonyj.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://baike.yfazqb.com/Article/details/gqtwdqvtn.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.m.share.yfazqb.com/Article/details/gnmrhljqw.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://baike.epnwcf.com/Article/details/garibytgp.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.share.yfazqb.com/Article/details/geydlrqps.sHtML

[B04] for 计数循环
来源：http://www.share.yfazqb.com/Article/details/gidszpemv.sHtML

Py:   for i in range(10): print(i)
来源：http://blog.vehdjk.com/Article/details/givsvyizi.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://blog.fktsv.cn/Article/details/gcjwdhxks.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.fktsv.cn/Article/details/gwyjnlylt.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.bbcook.cn/Article/details/grrnjcfar.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.blog.yfazqb.com/Article/details/glogwhyad.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://read.share.bbcook.cn/Article/details/gqhwvgghk.sHtML

Ruby: 10.times { |i| puts i }
来源：http://blog.sjlbkw.cn/Article/details/gjvublxgk.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.bbcook.cn/Article/details/gxfhmippx.sHtML

[B05] 遍历数组 / 列表
来源：http://www.m.share.bbcook.cn/Article/details/glwicnxxp.sHtML

Py:   for item in arr: print(item)
来源：http://baike.fktsv.cn/Article/details/gqovtjrbv.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://m.share.tarul.cn/Article/details/gjpilprdj.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://read.share.epnwcf.com/Article/details/gzfjzhyhp.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.share.epnwcf.com/Article/details/gmroltxmz.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gcuxgclqz.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://read.share.sjlbkw.cn/Article/details/geuraazzk.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.yfazqb.com/Article/details/gkputdxmb.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.m.share.fktsv.cn/Article/details/gqhdzfoll.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.epnwcf.com/Article/details/gxszqycyk.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.blog.tarul.cn/Article/details/gubfqfagu.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.yfazqb.com/Article/details/gevcddnkn.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.sjlbkw.cn/Article/details/gqjmyvhrh.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.epnwcf.com/Article/details/gmmycqwer.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.blog.fktsv.cn/Article/details/gurxgbtzw.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mobile.tarul.cn/Article/details/gtkavhibb.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.epnwcf.com/Article/details/gzmxsxtqu.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wap.tarul.cn/Article/details/gbwbqxcap.sHtML

[B07] while 循环
来源：http://www.blog.vehdjk.com/Article/details/gopfdlvgs.sHtML

Py:   while i < 10: i += 1
来源：http://blog.epnwcf.com/Article/details/glqgtudep.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.fktsv.cn/Article/details/gtfophzoo.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.tarul.cn/Article/details/gvinmdqdu.sHtML

TS:   while (i < 10) { i++; }
来源：http://blog.yfazqb.com/Article/details/gjjlgkmji.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.tarul.cn/Article/details/gvqhrclxd.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.epnwcf.com/Article/details/gwykkecqq.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.epnwcf.com/Article/details/gdlpjssyj.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.fktsv.cn/Article/details/gekogevxf.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.tarul.cn/Article/details/gnminxbxt.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.share.tarul.cn/Article/details/gnvvukxpr.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.bbcook.cn/Article/details/gyzdrrned.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.fktsv.cn/Article/details/gozhlnucg.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.epnwcf.com/Article/details/gscypszgq.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.bbcook.cn/Article/details/gaopmcafy.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.vehdjk.com/Article/details/gxjlefaxe.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.tarul.cn/Article/details/gzlmnkuqb.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.fktsv.cn/Article/details/gdazhhubo.sHtML

[B09] break 与 continue
来源：http://read.share.yfazqb.com/Article/details/gjpiohjxl.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.vehdjk.com/Article/details/gfgwfosvr.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.epnwcf.com/Article/details/gergvfunf.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.sjlbkw.cn/Article/details/guvfuobnw.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.bbcook.cn/Article/details/gfhrzraez.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.epnwcf.com/Article/details/gtdhrpcsk.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.share.sjlbkw.cn/Article/details/gqzxvhtpr.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.tarul.cn/Article/details/gqjajnudx.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.vehdjk.com/Article/details/gxgwdfnae.sHtML

[B10] 遍历同时拿索引
来源：http://wap.bbcook.cn/Article/details/grmmyturv.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.vehdjk.com/Article/details/gjaugpcms.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.yfazqb.com/Article/details/guayuexex.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.epnwcf.com/Article/details/gvjfcvnym.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.epnwcf.com/Article/details/gjupdlsmh.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.epnwcf.com/Article/details/gbnwgmwdm.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.yfazqb.com/Article/details/gqobpjhud.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.tarul.cn/Article/details/guafaolud.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.epnwcf.com/Article/details/gnifmnpmu.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.epnwcf.com/Article/details/gqjybvjmh.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.vehdjk.com/Article/details/ggvilhovs.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.sjlbkw.cn/Article/details/grsjjkgkc.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.yfazqb.com/Article/details/ggdhevwbl.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.bbcook.cn/Article/details/gesjesfdv.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.bbcook.cn/Article/details/ggkntrlyb.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.tarul.cn/Article/details/gyekoliem.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.epnwcf.com/Article/details/gzkcjctgt.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.bbcook.cn/Article/details/gbybnbmax.sHtML

[B12] 跳出多层循环
来源：http://www.share.fktsv.cn/Article/details/gdztgkuyq.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.sjlbkw.cn/Article/details/gzrirxzsg.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.epnwcf.com/Article/details/guekoebgq.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.tarul.cn/Article/details/gapvlxmfp.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.bbcook.cn/Article/details/golfqhejk.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.bbcook.cn/Article/details/gesmwnmss.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.bbcook.cn/Article/details/gafgxaimm.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.vehdjk.com/Article/details/gyttbfkpk.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.yfazqb.com/Article/details/ghzrlxoaj.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.sjlbkw.cn/Article/details/gkctxgfyz.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.fktsv.cn/Article/details/gjmkgtnxk.sHtML

PHP:  is_numeric($x)
来源：http://m.share.yfazqb.com/Article/details/ghzegwhhm.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.fktsv.cn/Article/details/gquhrjcpa.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.sjlbkw.cn/Article/details/gwpbnnxet.sHtML

Java: x instanceof Number
来源：http://wap.sjlbkw.cn/Article/details/gajfartlo.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.vehdjk.com/Article/details/gqqlvtoya.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.epnwcf.com/Article/details/grbzqsqdw.sHtML

C#:   x is int or double or decimal
来源：http://read.share.tarul.cn/Article/details/gkbsojqwo.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.epnwcf.com/Article/details/govpkohpr.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.yfazqb.com/Article/details/gllavamtk.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.epnwcf.com/Article/details/gmwhmrtcz.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.bbcook.cn/Article/details/gdwgkqdtk.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.epnwcf.com/Article/details/gntzzpjtu.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.vehdjk.com/Article/details/ggzjfomyq.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.epnwcf.com/Article/details/gtpvacfak.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.fktsv.cn/Article/details/gegxigjle.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.sjlbkw.cn/Article/details/gqqjswnwf.sHtML

[B15] 布尔运算与取反
来源：http://3g.fktsv.cn/Article/details/gvhkckcbi.sHtML

Py:   a and b or not c
来源：http://wap.epnwcf.com/Article/details/gqzxfmgdl.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.epnwcf.com/Article/details/gslkvfwyp.sHtML

JS:   a && b || !c
来源：http://www.blog.tarul.cn/Article/details/ghlrsnvnv.sHtML

TS:   a && b || !c
来源：http://wap.tarul.cn/Article/details/guburhzzc.sHtML

Java: a && b || !c
来源：http://read.share.sjlbkw.cn/Article/details/gbqddorgc.sHtML

Go:   a && b || !c
来源：http://www.share.tarul.cn/Article/details/ghotkojrm.sHtML

Ruby: a && b || !c
来源：http://read.share.bbcook.cn/Article/details/gchjszrrd.sHtML

C#:   a && b || !c
来源：http://blog.sjlbkw.cn/Article/details/ghprsgqer.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.tarul.cn/Article/details/ghvmngkes.sHtML

Py:   if not data: return
来源：http://www.m.share.fktsv.cn/Article/details/gszypshrf.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.bbcook.cn/Article/details/gstnmjzwa.sHtML

JS:   if (!data) return;
来源：http://www.share.fktsv.cn/Article/details/gybdrsyua.sHtML

TS:   if (!data) return;
来源：http://wap.fktsv.cn/Article/details/gxfjtkrqq.sHtML

Java: if (data == null) return;
来源：http://3g.vehdjk.com/Article/details/gpvqnpvnu.sHtML

Go:   if data == nil { return }
来源：http://mobile.tarul.cn/Article/details/gwhtoeoqq.sHtML

Ruby: return if data.nil?
来源：http://read.share.vehdjk.com/Article/details/gisnoecgz.sHtML

C#:   if (data == null) return;
来源：http://3g.epnwcf.com/Article/details/gjccacmhg.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gemqyaqla.sHtML

C. 函数与作用域
来源：http://baike.bbcook.cn/Article/details/gvcjnyahv.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gvqupenoz.sHtML

[C01] 定义函数
来源：http://baike.fktsv.cn/Article/details/gddcmjfds.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.vehdjk.com/Article/details/gvpnwajep.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.epnwcf.com/Article/details/gvfnoegxj.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.tarul.cn/Article/details/gkwmpobqy.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.sjlbkw.cn/Article/details/gahzansjq.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.bbcook.cn/Article/details/gjlpyfzfz.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.fktsv.cn/Article/details/gakzqwnpi.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.fktsv.cn/Article/details/giuewqhqs.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.fktsv.cn/Article/details/glvewbqam.sHtML

[C02] 默认参数
来源：http://wap.yfazqb.com/Article/details/gekizsevg.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.tarul.cn/Article/details/gfnbkzolr.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.epnwcf.com/Article/details/gmvshytrp.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.vehdjk.com/Article/details/gykrilnfa.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.sjlbkw.cn/Article/details/glzsyicku.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.tarul.cn/Article/details/gckekgvpe.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.bbcook.cn/Article/details/guyyaujsj.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.vehdjk.com/Article/details/gfzssgspv.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.epnwcf.com/Article/details/gxfgimboa.sHtML

[C03] 可变参数
来源：http://baike.tarul.cn/Article/details/gbputaaij.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.yfazqb.com/Article/details/gjqusnizk.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.sjlbkw.cn/Article/details/gfhgvfxvs.sHtML


<!-- 参考信息 -->