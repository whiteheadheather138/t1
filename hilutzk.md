代发 wailian999

Java: "第一行\n第二行"
来源：http://www.m.share.yfazqb.com/Article/details/grbwpbnpi.sHtML

Go:   "第一行\n第二行"
来源：http://www.blog.bbcook.cn/Article/details/gzpisrdud.sHtML

Ruby: "第一行\n第二行"
来源：http://m.share.yfazqb.com/Article/details/ghbuekmzq.sHtML

C#:   "第一行\n第二行"
来源：http://www.share.sjlbkw.cn/Article/details/gibtoikcd.sHtML

[A14] 注释写法
来源：http://read.share.sjlbkw.cn/Article/details/gsstlzkdc.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://3g.tarul.cn/Article/details/gppxgssfq.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://3g.sjlbkw.cn/Article/details/gpasfnsqh.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.blog.vehdjk.com/Article/details/gscjcmllf.sHtML

TS:   // 单行；/* 多行 */
来源：http://wap.yfazqb.com/Article/details/gjpdnjvhi.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.blog.tarul.cn/Article/details/gdsxpvzdt.sHtML

Go:   // 单行；/* 多行 */
来源：http://blog.vehdjk.com/Article/details/gmfpsaatw.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.blog.tarul.cn/Article/details/gqphsjybt.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.share.vehdjk.com/Article/details/gpkxfvajm.sHtML

[A15] 空值判断与默认值
来源：http://blog.tarul.cn/Article/details/gxrdlafed.sHtML

Py:   value = data or "默认值"
来源：http://blog.bbcook.cn/Article/details/gwqcnqgeo.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://m.share.tarul.cn/Article/details/gsvanixca.sHtML

JS:   const value = data ?? "默认值";
来源：http://m.share.tarul.cn/Article/details/gpqjtmdmy.sHtML

TS:   const value = data ?? "默认值";
来源：http://3g.tarul.cn/Article/details/gxhucgicx.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.blog.bbcook.cn/Article/details/gsunapcxs.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://baike.epnwcf.com/Article/details/gywutuvig.sHtML

Ruby: value = data || "默认值"
来源：http://m.share.bbcook.cn/Article/details/gcvmcwdeq.sHtML

C#:   var value = data ?? "默认值";
来源：http://blog.epnwcf.com/Article/details/gxgjaaqbq.sHtML

[A16] 真假值判断规则
来源：http://wap.tarul.cn/Article/details/gxmalthcp.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.m.share.epnwcf.com/Article/details/gtphqehun.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://m.share.fktsv.cn/Article/details/gkykyxojg.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://m.share.sjlbkw.cn/Article/details/gsenhpafa.sHtML

TS:   if (!x) {}
来源：http://baike.fktsv.cn/Article/details/gxxdxsgai.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wap.fktsv.cn/Article/details/gppgcxhjl.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.blog.sjlbkw.cn/Article/details/geftrttck.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://3g.epnwcf.com/Article/details/gjzbwvuli.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mobile.sjlbkw.cn/Article/details/gugxhjfqt.sHtML

[A17] 位运算
来源：http://baike.tarul.cn/Article/details/gkufxigfx.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.bbcook.cn/Article/details/gdnjvtwob.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://m.share.bbcook.cn/Article/details/gspgzthyp.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.vehdjk.com/Article/details/gdeojjyqq.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://baike.sjlbkw.cn/Article/details/gronzestj.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.epnwcf.com/Article/details/gyxoonpvc.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://mobile.vehdjk.com/Article/details/gxgnujefd.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.tarul.cn/Article/details/gkoyhrwtx.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.bbcook.cn/Article/details/gudwvmwqw.sHtML

[A18] 字符与 ASCII 码互转
来源：http://read.share.bbcook.cn/Article/details/gvulzwfmx.sHtML

Py:   ord("A"); chr(65)
来源：http://m.share.sjlbkw.cn/Article/details/glqzwpkxj.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.share.vehdjk.com/Article/details/gtorjfurh.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.yfazqb.com/Article/details/gbkrlviti.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://3g.vehdjk.com/Article/details/gfzvgihvx.sHtML

Java: (int) 'A'; (char) 65
来源：http://baike.sjlbkw.cn/Article/details/gmcrxancj.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://3g.epnwcf.com/Article/details/grsgzujzs.sHtML

Ruby: "A".ord; 65.chr
来源：http://3g.tarul.cn/Article/details/gwchlxgxs.sHtML

C#:   (int)'A'; (char)65
来源：http://blog.fktsv.cn/Article/details/guybxckms.sHtML

[A19] 交换两个变量
来源：http://www.share.bbcook.cn/Article/details/ggmlnivzo.sHtML

Py:   a, b = b, a
来源：http://www.blog.tarul.cn/Article/details/gemxtkcga.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://mobile.yfazqb.com/Article/details/gcwgwlusa.sHtML

JS:   [a, b] = [b, a];
来源：http://www.share.fktsv.cn/Article/details/grzxpehly.sHtML

TS:   [a, b] = [b, a];
来源：http://baike.bbcook.cn/Article/details/gqmaxxxwb.sHtML

Java: int t = a; a = b; b = t;
来源：http://3g.yfazqb.com/Article/details/gjzlghevd.sHtML

Go:   a, b = b, a
来源：http://read.share.epnwcf.com/Article/details/grxwslovo.sHtML

Ruby: a, b = b, a
来源：http://read.share.tarul.cn/Article/details/goleophfx.sHtML

C#:   (a, b) = (b, a);
来源：http://www.blog.yfazqb.com/Article/details/gvydpaipv.sHtML

[A20] 读取标准输入
来源：http://www.blog.tarul.cn/Article/details/ghytxuxwv.sHtML

Py:   name = input("请输入：")
来源：http://baike.tarul.cn/Article/details/gxjhpcqzl.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://3g.epnwcf.com/Article/details/gvcvlhjmf.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://mobile.yfazqb.com/Article/details/gbohdkycx.sHtML

TS:   // Node.js：readline 模块
来源：http://wap.sjlbkw.cn/Article/details/gfgfoztvf.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://mobile.epnwcf.com/Article/details/geqcgmlli.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.share.bbcook.cn/Article/details/gscsijxrb.sHtML

Ruby: gets.chomp
来源：http://www.share.vehdjk.com/Article/details/ghzwfplhm.sHtML

C#:   Console.ReadLine();
来源：http://www.blog.epnwcf.com/Article/details/gukwzsgvy.sHtML

[A21] 保留指定小数位输出
来源：http://blog.vehdjk.com/Article/details/gbwnwppks.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.share.fktsv.cn/Article/details/grqujpedx.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.m.share.yfazqb.com/Article/details/gemknioyj.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.blog.sjlbkw.cn/Article/details/gyblsjksx.sHtML

TS:   (3.14159).toFixed(2)
来源：http://read.share.tarul.cn/Article/details/guwayfgyl.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://wap.sjlbkw.cn/Article/details/gktrsxlsw.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://blog.bbcook.cn/Article/details/glapqifyu.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://m.share.sjlbkw.cn/Article/details/gnjwmcojn.sHtML

C#:   3.14159.ToString("F2")
来源：http://wap.vehdjk.com/Article/details/gqwazntzs.sHtML

[A22] 获取字符串长度
来源：http://wap.epnwcf.com/Article/details/gtuoohvge.sHtML

Py:   len(s)
来源：http://blog.fktsv.cn/Article/details/gfnunymdm.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://baike.epnwcf.com/Article/details/gsmmimttj.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.m.share.bbcook.cn/Article/details/glrigvgmg.sHtML

TS:   s.length
来源：http://m.share.fktsv.cn/Article/details/glemqiqif.sHtML

Java: s.length()
来源：http://blog.sjlbkw.cn/Article/details/gpewfsoby.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://m.share.fktsv.cn/Article/details/gogkybubf.sHtML

Ruby: s.length
来源：http://www.share.vehdjk.com/Article/details/gdjgskhkn.sHtML

C#:   s.Length
来源：http://m.share.fktsv.cn/Article/details/gaxbmxdfo.sHtML

[A23] 大小写转换
来源：http://baike.bbcook.cn/Article/details/gvgghfeml.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.blog.bbcook.cn/Article/details/grlwfaull.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://baike.fktsv.cn/Article/details/geenrbqed.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.epnwcf.com/Article/details/gzvrvgbgz.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.sjlbkw.cn/Article/details/ghxmqbopj.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.share.epnwcf.com/Article/details/glgsavenz.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mobile.sjlbkw.cn/Article/details/gmzuwbkbg.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://m.share.yfazqb.com/Article/details/glepnvlyg.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://read.share.fktsv.cn/Article/details/gonmkbgsy.sHtML

[A24] 去除首尾空白
来源：http://read.share.sjlbkw.cn/Article/details/gkwstoozs.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wap.bbcook.cn/Article/details/gskpnbwde.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://3g.epnwcf.com/Article/details/gmjvmtrin.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.yfazqb.com/Article/details/grentqvhu.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.bbcook.cn/Article/details/gzeissdku.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://blog.tarul.cn/Article/details/gkmyeaibm.sHtML

Go:   strings.TrimSpace(s)
来源：http://wap.yfazqb.com/Article/details/glhadtwit.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.m.share.bbcook.cn/Article/details/givzmmdyc.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.m.share.epnwcf.com/Article/details/gnrmwelgt.sHtML

[A25] 字符串比较
来源：http://www.m.share.fktsv.cn/Article/details/gvgyygple.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.blog.bbcook.cn/Article/details/gwzuyjtxd.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.m.share.sjlbkw.cn/Article/details/glkjibryv.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.epnwcf.com/Article/details/gppudgrfo.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.sjlbkw.cn/Article/details/gafsrajgw.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://blog.epnwcf.com/Article/details/gwcqdrgsx.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wap.yfazqb.com/Article/details/gndaltzdw.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://read.share.tarul.cn/Article/details/gaexaebvd.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://m.share.vehdjk.com/Article/details/gqdfzndtt.sHtML

[A26] 类型转换总览
来源：http://www.share.epnwcf.com/Article/details/grrsaascj.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://m.share.bbcook.cn/Article/details/gewdririq.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://3g.bbcook.cn/Article/details/garurdxhl.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.m.share.fktsv.cn/Article/details/gkthzcnrq.sHtML

TS:   Number() String() Boolean() x as number
来源：http://m.share.sjlbkw.cn/Article/details/gamoxstsd.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.share.vehdjk.com/Article/details/gmoppqzew.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://blog.tarul.cn/Article/details/gxejbxqhd.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://m.share.tarul.cn/Article/details/gigtfncqz.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://3g.sjlbkw.cn/Article/details/gpvobwxiy.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/ghgsqraxm.sHtML

B. 流程控制
来源：http://3g.bbcook.cn/Article/details/gsibhhgzq.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/goiucxgah.sHtML

[B01] 条件判断 if / else
来源：http://www.share.vehdjk.com/Article/details/gvgleicvc.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://wap.bbcook.cn/Article/details/glvfgmvvu.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.share.sjlbkw.cn/Article/details/glrnolxye.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.vehdjk.com/Article/details/gbfboygng.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.fktsv.cn/Article/details/gneyllkbi.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.m.share.fktsv.cn/Article/details/gjwzondnd.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mobile.fktsv.cn/Article/details/ghsjrjgrw.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.blog.vehdjk.com/Article/details/gwhpnvxxe.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mobile.bbcook.cn/Article/details/gibacpfgd.sHtML

[B02] 多分支 else if / elif
来源：http://mobile.bbcook.cn/Article/details/gufzgeidn.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.m.share.yfazqb.com/Article/details/gycfthsul.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wap.sjlbkw.cn/Article/details/gkwnrihyi.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.bbcook.cn/Article/details/gvkbebylw.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.tarul.cn/Article/details/gfukhcyar.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.bbcook.cn/Article/details/gnblawuwg.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.share.fktsv.cn/Article/details/gdtcgtlen.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.share.sjlbkw.cn/Article/details/gulpuyxug.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fktsv.cn/Article/details/gpwshxcjo.sHtML

[B03] switch / match / case
来源：http://mobile.sjlbkw.cn/Article/details/gyliljodh.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.m.share.vehdjk.com/Article/details/grdiifwwj.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wap.tarul.cn/Article/details/glghwodiu.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.epnwcf.com/Article/details/gpfkwaouw.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.yfazqb.com/Article/details/gtlgugong.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.share.epnwcf.com/Article/details/gwymhjaps.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://read.share.bbcook.cn/Article/details/gnjamheau.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.yfazqb.com/Article/details/gvdwgumxp.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wap.sjlbkw.cn/Article/details/gfwesytrv.sHtML

[B04] for 计数循环
来源：http://3g.vehdjk.com/Article/details/guduygquu.sHtML

Py:   for i in range(10): print(i)
来源：http://3g.yfazqb.com/Article/details/gysqwkdvo.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.share.bbcook.cn/Article/details/gaewpleec.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.sjlbkw.cn/Article/details/gfsosnhmc.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.yfazqb.com/Article/details/gslijiwpk.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://m.share.fktsv.cn/Article/details/gcfxuceal.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://baike.tarul.cn/Article/details/grndlnvql.sHtML

Ruby: 10.times { |i| puts i }
来源：http://read.share.bbcook.cn/Article/details/guuolazal.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mobile.epnwcf.com/Article/details/gbebemejv.sHtML

[B05] 遍历数组 / 列表
来源：http://www.m.share.yfazqb.com/Article/details/gsasmjodq.sHtML

Py:   for item in arr: print(item)
来源：http://mobile.tarul.cn/Article/details/gftaqqlhq.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://3g.epnwcf.com/Article/details/gttfysuew.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.bbcook.cn/Article/details/grechsack.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://3g.vehdjk.com/Article/details/gsurfabvb.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.epnwcf.com/Article/details/giagqeyud.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://read.share.bbcook.cn/Article/details/geuhbwtyx.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.blog.sjlbkw.cn/Article/details/griwdcijy.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://baike.fktsv.cn/Article/details/gtxeuhbrk.sHtML

[B06] 遍历字典 / 对象
来源：http://www.blog.bbcook.cn/Article/details/gwicinxna.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.epnwcf.com/Article/details/gahsocpcp.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://baike.fktsv.cn/Article/details/gomtpyaam.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.sjlbkw.cn/Article/details/grvwgixgx.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.vehdjk.com/Article/details/gtmirktha.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.sjlbkw.cn/Article/details/gvmyvwczm.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.sjlbkw.cn/Article/details/gnyqtgmht.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://blog.sjlbkw.cn/Article/details/gkzjjfcpt.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.share.yfazqb.com/Article/details/gyqxpoxrn.sHtML

[B07] while 循环
来源：http://m.share.vehdjk.com/Article/details/gyuxeqypt.sHtML

Py:   while i < 10: i += 1
来源：http://mobile.fktsv.cn/Article/details/gheqzbjrw.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://3g.sjlbkw.cn/Article/details/gfsstqxux.sHtML

JS:   while (i < 10) { i++; }
来源：http://blog.yfazqb.com/Article/details/gvueizxmo.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.blog.yfazqb.com/Article/details/gncmfwxls.sHtML

Java: while (i < 10) { i++; }
来源：http://www.blog.epnwcf.com/Article/details/gaamxkvgg.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mobile.epnwcf.com/Article/details/gowczowdq.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.vehdjk.com/Article/details/gmpeynehb.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.vehdjk.com/Article/details/glkdugspt.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.tarul.cn/Article/details/gfvyzugwu.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.vehdjk.com/Article/details/guijpbjax.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.vehdjk.com/Article/details/glpbnrtmb.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.vehdjk.com/Article/details/gfcmsiuyf.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.sjlbkw.cn/Article/details/gomqpxpjj.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.vehdjk.com/Article/details/gqxqlbjue.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.fktsv.cn/Article/details/gewjswtwf.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.bbcook.cn/Article/details/gtuhchndr.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.yfazqb.com/Article/details/gxiqztncz.sHtML

[B09] break 与 continue
来源：http://www.blog.vehdjk.com/Article/details/giypsmurw.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.fktsv.cn/Article/details/goklzvlkq.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.epnwcf.com/Article/details/ggcaqvqdw.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.epnwcf.com/Article/details/gkcxedims.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.vehdjk.com/Article/details/gttagakwf.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.vehdjk.com/Article/details/glaotxoqs.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.vehdjk.com/Article/details/gyaadbhng.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.tarul.cn/Article/details/gsbafdgrw.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.vehdjk.com/Article/details/gbbpqvclh.sHtML

[B10] 遍历同时拿索引
来源：http://wap.fktsv.cn/Article/details/gbctdengx.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.fktsv.cn/Article/details/gzdfwmklc.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.fktsv.cn/Article/details/grzpezqde.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.bbcook.cn/Article/details/gayrbmulp.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.fktsv.cn/Article/details/gxznoylkf.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.tarul.cn/Article/details/gsjhkpixc.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.vehdjk.com/Article/details/gurkigngs.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.yfazqb.com/Article/details/gfjlbrnxm.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.bbcook.cn/Article/details/gcqxfdqvo.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.tarul.cn/Article/details/grivmejsm.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.fktsv.cn/Article/details/gwajavjhg.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.sjlbkw.cn/Article/details/grewdsnjx.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.fktsv.cn/Article/details/gcxpxnjgd.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.bbcook.cn/Article/details/gphnaicon.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.tarul.cn/Article/details/gifcvoqtr.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.epnwcf.com/Article/details/gshirbhal.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.fktsv.cn/Article/details/gnmlfjbvb.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.epnwcf.com/Article/details/ggpwyhncp.sHtML

[B12] 跳出多层循环
来源：http://3g.yfazqb.com/Article/details/gmxpvzlfl.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.yfazqb.com/Article/details/gsmbvkjii.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.yfazqb.com/Article/details/gbkxqmgjv.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.bbcook.cn/Article/details/gzreykfef.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.bbcook.cn/Article/details/gkgrikcwy.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.bbcook.cn/Article/details/gfthsmmtl.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.sjlbkw.cn/Article/details/gfgduvpil.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.epnwcf.com/Article/details/gtbzescir.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.vehdjk.com/Article/details/ghcynqqaw.sHtML

[B13] 判断是否为数字
来源：http://read.share.epnwcf.com/Article/details/ggkpzvkuy.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.yfazqb.com/Article/details/gspvdikss.sHtML

PHP:  is_numeric($x)
来源：http://baike.tarul.cn/Article/details/gbhlnfqil.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.vehdjk.com/Article/details/gjxrlucfa.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.tarul.cn/Article/details/gtcbkhvcr.sHtML

Java: x instanceof Number
来源：http://read.share.bbcook.cn/Article/details/ghthwcejt.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.bbcook.cn/Article/details/gvveqegwn.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.tarul.cn/Article/details/gftldzytp.sHtML

C#:   x is int or double or decimal
来源：http://blog.vehdjk.com/Article/details/gkdjjqein.sHtML

[B14] 判断值是否在集合内
来源：http://baike.bbcook.cn/Article/details/gvhdswfjb.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.tarul.cn/Article/details/gijpvbxde.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.bbcook.cn/Article/details/gxlavykeo.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.epnwcf.com/Article/details/gpsifmzum.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.yfazqb.com/Article/details/ggtcjtrjj.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.fktsv.cn/Article/details/gmjlvfdyq.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.fktsv.cn/Article/details/gzboqarmg.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.sjlbkw.cn/Article/details/grtsfohgy.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.sjlbkw.cn/Article/details/grkbcxoit.sHtML

[B15] 布尔运算与取反
来源：http://baike.sjlbkw.cn/Article/details/grairritr.sHtML

Py:   a and b or not c
来源：http://mobile.vehdjk.com/Article/details/gvfhejdkz.sHtML

PHP:  $a && $b || !$c
来源：http://baike.bbcook.cn/Article/details/gdzncyvug.sHtML

JS:   a && b || !c
来源：http://m.share.yfazqb.com/Article/details/gkiwrefnn.sHtML

TS:   a && b || !c
来源：http://mobile.tarul.cn/Article/details/gcsqfnfcs.sHtML

Java: a && b || !c
来源：http://mobile.epnwcf.com/Article/details/gyzxvgsap.sHtML

Go:   a && b || !c
来源：http://m.share.fktsv.cn/Article/details/gpqcewsju.sHtML

Ruby: a && b || !c
来源：http://m.share.epnwcf.com/Article/details/gltgopxxb.sHtML

C#:   a && b || !c
来源：http://blog.tarul.cn/Article/details/gqlxkmzdu.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.bbcook.cn/Article/details/gaexikcxs.sHtML

Py:   if not data: return
来源：http://www.blog.fktsv.cn/Article/details/gnlsxmtra.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.vehdjk.com/Article/details/ghktcmbgp.sHtML

JS:   if (!data) return;
来源：http://www.share.sjlbkw.cn/Article/details/gdpznntyf.sHtML

TS:   if (!data) return;
来源：http://mobile.fktsv.cn/Article/details/gxmssxnsw.sHtML

Java: if (data == null) return;
来源：http://3g.yfazqb.com/Article/details/gmvlwovtv.sHtML

Go:   if data == nil { return }
来源：http://mobile.bbcook.cn/Article/details/gjysnyqbw.sHtML

Ruby: return if data.nil?
来源：http://wap.sjlbkw.cn/Article/details/gqexrfjft.sHtML

C#:   if (data == null) return;
来源：http://m.share.fktsv.cn/Article/details/gjenlawuk.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gogoosavv.sHtML

C. 函数与作用域
来源：http://read.share.fktsv.cn/Article/details/gbtipnoeb.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gkvntvatr.sHtML

[C01] 定义函数
来源：http://wap.epnwcf.com/Article/details/gtttdytwe.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.bbcook.cn/Article/details/gwichosxg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.epnwcf.com/Article/details/gaebwwyoj.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.tarul.cn/Article/details/grxelcnvj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.epnwcf.com/Article/details/giltcnknd.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.bbcook.cn/Article/details/gmjlbccuj.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.epnwcf.com/Article/details/grujskjlu.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.tarul.cn/Article/details/gpdyiciax.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.sjlbkw.cn/Article/details/gclxsrlcb.sHtML

[C02] 默认参数
来源：http://www.share.bbcook.cn/Article/details/gdgzmfrul.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.sjlbkw.cn/Article/details/gvmjkacup.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.tarul.cn/Article/details/ggquvwlvz.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.vehdjk.com/Article/details/guurphytg.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.fktsv.cn/Article/details/gdmzvigze.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.yfazqb.com/Article/details/gbxucsztb.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.bbcook.cn/Article/details/gzrkvsjcb.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.fktsv.cn/Article/details/gteakqrtp.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.fktsv.cn/Article/details/gvcsjmyzz.sHtML

[C03] 可变参数
来源：http://www.m.share.vehdjk.com/Article/details/gcpxrmfek.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.epnwcf.com/Article/details/gifsqndmm.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.epnwcf.com/Article/details/grqtbdjsa.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.fktsv.cn/Article/details/gsnfelqdz.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.yfazqb.com/Article/details/gsndqixuz.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.vehdjk.com/Article/details/gccgigthj.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.sjlbkw.cn/Article/details/ghgmruzbo.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.sjlbkw.cn/Article/details/gpnpqawxt.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.fktsv.cn/Article/details/gmidgfkap.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.fktsv.cn/Article/details/ghndulufv.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.tarul.cn/Article/details/glxqmnpld.sHtML


<!-- 参考信息 -->