代发 wailian999

C#:   // 单行；/* 多行 */
来源：http://wap.vehdjk.com/Article/details/gvilpqxob.sHtML

[A15] 空值判断与默认值
来源：http://blog.yfazqb.com/Article/details/gdoafwtnn.sHtML

Py:   value = data or "默认值"
来源：http://read.share.epnwcf.com/Article/details/gfnssappg.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.m.share.vehdjk.com/Article/details/gcbwpppkq.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.m.share.epnwcf.com/Article/details/gsfruyaxp.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.share.tarul.cn/Article/details/gpupxzvgr.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://m.share.fktsv.cn/Article/details/gppclajwi.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://mobile.sjlbkw.cn/Article/details/gcjlojsyz.sHtML

Ruby: value = data || "默认值"
来源：http://www.m.share.yfazqb.com/Article/details/gwpgafmlt.sHtML

C#:   var value = data ?? "默认值";
来源：http://baike.epnwcf.com/Article/details/gknagntwz.sHtML

[A16] 真假值判断规则
来源：http://wap.bbcook.cn/Article/details/gccadlvwo.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wap.tarul.cn/Article/details/gequomwmy.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://baike.sjlbkw.cn/Article/details/gvsylokzt.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.blog.fktsv.cn/Article/details/gpigzggij.sHtML

TS:   if (!x) {}
来源：http://mobile.tarul.cn/Article/details/grdtmsaaj.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wap.yfazqb.com/Article/details/gzubudmyi.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.blog.epnwcf.com/Article/details/gfutofynu.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://m.share.sjlbkw.cn/Article/details/gmydznhkl.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://read.share.vehdjk.com/Article/details/gklssrioj.sHtML

[A17] 位运算
来源：http://blog.sjlbkw.cn/Article/details/gtvzrvjxi.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.bbcook.cn/Article/details/gdlrhxhzx.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://m.share.yfazqb.com/Article/details/ghkhtyrqc.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.epnwcf.com/Article/details/gusxbssck.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wap.sjlbkw.cn/Article/details/gfyvwndnn.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.sjlbkw.cn/Article/details/grfjbrmkt.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://m.share.yfazqb.com/Article/details/gsbssqqdd.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.tarul.cn/Article/details/gdbqdmoyj.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.epnwcf.com/Article/details/gpfntkybl.sHtML

[A18] 字符与 ASCII 码互转
来源：http://3g.bbcook.cn/Article/details/gxaumxkns.sHtML

Py:   ord("A"); chr(65)
来源：http://blog.bbcook.cn/Article/details/gftrzlpti.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.blog.tarul.cn/Article/details/ggbqzimtz.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.bbcook.cn/Article/details/gqwlnzmua.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.m.share.bbcook.cn/Article/details/gqhyxuurz.sHtML

Java: (int) 'A'; (char) 65
来源：http://baike.bbcook.cn/Article/details/gbfdmfapf.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.blog.vehdjk.com/Article/details/grlufhzxb.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.share.sjlbkw.cn/Article/details/gncgqahdi.sHtML

C#:   (int)'A'; (char)65
来源：http://mobile.vehdjk.com/Article/details/grpwsqqpq.sHtML

[A19] 交换两个变量
来源：http://baike.epnwcf.com/Article/details/gwbesxpce.sHtML

Py:   a, b = b, a
来源：http://blog.sjlbkw.cn/Article/details/gxtvylnkh.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.m.share.sjlbkw.cn/Article/details/gzipykcij.sHtML

JS:   [a, b] = [b, a];
来源：http://www.blog.fktsv.cn/Article/details/gcviervbj.sHtML

TS:   [a, b] = [b, a];
来源：http://www.share.bbcook.cn/Article/details/govtljsdf.sHtML

Java: int t = a; a = b; b = t;
来源：http://read.share.bbcook.cn/Article/details/gbpllugbd.sHtML

Go:   a, b = b, a
来源：http://blog.epnwcf.com/Article/details/getflalas.sHtML

Ruby: a, b = b, a
来源：http://mobile.bbcook.cn/Article/details/gjqichamk.sHtML

C#:   (a, b) = (b, a);
来源：http://mobile.yfazqb.com/Article/details/gpvianjev.sHtML

[A20] 读取标准输入
来源：http://read.share.tarul.cn/Article/details/glapnxtjn.sHtML

Py:   name = input("请输入：")
来源：http://mobile.tarul.cn/Article/details/geldbkwts.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://3g.tarul.cn/Article/details/gokbpbjjj.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://3g.epnwcf.com/Article/details/gqrknoesq.sHtML

TS:   // Node.js：readline 模块
来源：http://mobile.tarul.cn/Article/details/gbpbbukld.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://mobile.vehdjk.com/Article/details/gppahbois.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.m.share.epnwcf.com/Article/details/gsvggplli.sHtML

Ruby: gets.chomp
来源：http://www.share.sjlbkw.cn/Article/details/grnxfubgr.sHtML

C#:   Console.ReadLine();
来源：http://m.share.epnwcf.com/Article/details/gxyivqgag.sHtML

[A21] 保留指定小数位输出
来源：http://www.blog.yfazqb.com/Article/details/gqgridqnv.sHtML

Py:   f"{3.14159:.2f}"
来源：http://mobile.epnwcf.com/Article/details/gmhyyybvx.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://mobile.tarul.cn/Article/details/gebtvzaoi.sHtML

JS:   (3.14159).toFixed(2)
来源：http://mobile.fktsv.cn/Article/details/ghuurncwf.sHtML

TS:   (3.14159).toFixed(2)
来源：http://baike.yfazqb.com/Article/details/giseavnqu.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.blog.vehdjk.com/Article/details/gytijviqh.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://read.share.yfazqb.com/Article/details/gjywhuxoc.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.m.share.tarul.cn/Article/details/ghadospyl.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.blog.tarul.cn/Article/details/gowpgpdby.sHtML

[A22] 获取字符串长度
来源：http://mobile.epnwcf.com/Article/details/gxwzlejan.sHtML

Py:   len(s)
来源：http://baike.bbcook.cn/Article/details/gkotmiewe.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.blog.vehdjk.com/Article/details/gsulvfxpx.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://m.share.tarul.cn/Article/details/gaqmxwtay.sHtML

TS:   s.length
来源：http://wap.sjlbkw.cn/Article/details/gtyriujiq.sHtML

Java: s.length()
来源：http://m.share.tarul.cn/Article/details/gqszbovsl.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wap.sjlbkw.cn/Article/details/gbpuqclvj.sHtML

Ruby: s.length
来源：http://baike.epnwcf.com/Article/details/glznftlhj.sHtML

C#:   s.Length
来源：http://mobile.yfazqb.com/Article/details/gzefoqafe.sHtML

[A23] 大小写转换
来源：http://www.share.epnwcf.com/Article/details/gmanoscao.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://mobile.yfazqb.com/Article/details/glipfrief.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://3g.bbcook.cn/Article/details/gtuxkpehp.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.vehdjk.com/Article/details/gnkzvuljr.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.yfazqb.com/Article/details/gmpyftxvd.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://read.share.epnwcf.com/Article/details/glchyepgi.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://baike.sjlbkw.cn/Article/details/gnoeskwrn.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://3g.bbcook.cn/Article/details/gqeumrppm.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://read.share.tarul.cn/Article/details/gyhqxpslz.sHtML

[A24] 去除首尾空白
来源：http://baike.bbcook.cn/Article/details/golnoisnq.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://blog.tarul.cn/Article/details/gisspfijf.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mobile.sjlbkw.cn/Article/details/gosxzcflc.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.yfazqb.com/Article/details/gpiulqika.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.epnwcf.com/Article/details/gksxswver.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://read.share.yfazqb.com/Article/details/gtsouolen.sHtML

Go:   strings.TrimSpace(s)
来源：http://wap.fktsv.cn/Article/details/gqliaknrv.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://blog.yfazqb.com/Article/details/gljcrxgyc.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.m.share.bbcook.cn/Article/details/gbbikulsy.sHtML

[A25] 字符串比较
来源：http://baike.bbcook.cn/Article/details/gyiopkgzy.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.blog.epnwcf.com/Article/details/gintplbqa.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.m.share.vehdjk.com/Article/details/glcdsxtkr.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.fktsv.cn/Article/details/gecdwwfdm.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.yfazqb.com/Article/details/gdenyyjbv.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wap.epnwcf.com/Article/details/gsgfymgde.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wap.sjlbkw.cn/Article/details/gzerfises.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.blog.fktsv.cn/Article/details/ggtcmwexh.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mobile.epnwcf.com/Article/details/gytpfztnj.sHtML

[A26] 类型转换总览
来源：http://3g.bbcook.cn/Article/details/gculurksl.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mobile.sjlbkw.cn/Article/details/gfehgwxuk.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://baike.sjlbkw.cn/Article/details/gvbtrlsrr.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://m.share.vehdjk.com/Article/details/gpmusrjmk.sHtML

TS:   Number() String() Boolean() x as number
来源：http://blog.epnwcf.com/Article/details/gfegjjqzp.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wap.yfazqb.com/Article/details/gjrjhqqms.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.blog.sjlbkw.cn/Article/details/gwcfmcvlx.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.share.bbcook.cn/Article/details/gydhxsjhf.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.m.share.tarul.cn/Article/details/gaivqjbxb.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gsgxzydyf.sHtML

B. 流程控制
来源：http://blog.vehdjk.com/Article/details/gfjamrupy.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/govmexetn.sHtML

[B01] 条件判断 if / else
来源：http://wap.fktsv.cn/Article/details/gibntzadv.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://mobile.yfazqb.com/Article/details/ghkuixosr.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://read.share.sjlbkw.cn/Article/details/gmdxyviph.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.yfazqb.com/Article/details/gntvpdlkg.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.tarul.cn/Article/details/gdojctext.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://mobile.fktsv.cn/Article/details/guwlifxbz.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://m.share.yfazqb.com/Article/details/gjmkonubv.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.share.fktsv.cn/Article/details/gojoustcg.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://baike.tarul.cn/Article/details/gpmsqvekf.sHtML

[B02] 多分支 else if / elif
来源：http://mobile.epnwcf.com/Article/details/gwfpjfzzw.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://m.share.tarul.cn/Article/details/gbiayqosz.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mobile.yfazqb.com/Article/details/gzwhvjajf.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.yfazqb.com/Article/details/gkbntrpts.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.tarul.cn/Article/details/gddsxowyo.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.sjlbkw.cn/Article/details/gymlokqkt.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mobile.epnwcf.com/Article/details/gwcbjvsis.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://blog.fktsv.cn/Article/details/gnzhwcqlc.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.bbcook.cn/Article/details/gmewghopy.sHtML

[B03] switch / match / case
来源：http://mobile.fktsv.cn/Article/details/gdjchrpxu.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.vehdjk.com/Article/details/gkkpftexj.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://m.share.bbcook.cn/Article/details/gfbfqvswj.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.vehdjk.com/Article/details/gbergirjh.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.sjlbkw.cn/Article/details/gysouyqaj.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mobile.epnwcf.com/Article/details/gupfkowhc.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://read.share.bbcook.cn/Article/details/gbazownyi.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://m.share.fktsv.cn/Article/details/gzukypefr.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wap.sjlbkw.cn/Article/details/gjebnefua.sHtML

[B04] for 计数循环
来源：http://www.blog.vehdjk.com/Article/details/ghafldeop.sHtML

Py:   for i in range(10): print(i)
来源：http://3g.sjlbkw.cn/Article/details/gnulilasb.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://baike.yfazqb.com/Article/details/gdvgqyjzm.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.vehdjk.com/Article/details/guretzvwf.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gociapdxc.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://read.share.bbcook.cn/Article/details/gazanpzzv.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://blog.vehdjk.com/Article/details/gsgofprlu.sHtML

Ruby: 10.times { |i| puts i }
来源：http://blog.fktsv.cn/Article/details/gqtmkelrw.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://m.share.vehdjk.com/Article/details/gphbqdguz.sHtML

[B05] 遍历数组 / 列表
来源：http://www.m.share.bbcook.cn/Article/details/gmxmpsdqv.sHtML

Py:   for item in arr: print(item)
来源：http://blog.yfazqb.com/Article/details/gpdvaxnkq.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://blog.sjlbkw.cn/Article/details/gkgjbregz.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://blog.fktsv.cn/Article/details/gbyfmkbel.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://wap.vehdjk.com/Article/details/gitmikocl.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://3g.sjlbkw.cn/Article/details/glxabreef.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://3g.vehdjk.com/Article/details/gefofjsjt.sHtML

Ruby: arr.each { |item| puts item }
来源：http://m.share.fktsv.cn/Article/details/gwzjtqwye.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://read.share.bbcook.cn/Article/details/goawjxmgo.sHtML

[B06] 遍历字典 / 对象
来源：http://blog.tarul.cn/Article/details/gssdimytj.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.epnwcf.com/Article/details/gryztnpql.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.epnwcf.com/Article/details/gxujvlpdn.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.epnwcf.com/Article/details/gxaoandty.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.fktsv.cn/Article/details/gkrqvfnuq.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.bbcook.cn/Article/details/gwwgvoygf.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.sjlbkw.cn/Article/details/gvhzhnlqu.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://blog.bbcook.cn/Article/details/gcjxkbnbv.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.epnwcf.com/Article/details/gmtdqneee.sHtML

[B07] while 循环
来源：http://blog.bbcook.cn/Article/details/ghklyckmq.sHtML

Py:   while i < 10: i += 1
来源：http://baike.sjlbkw.cn/Article/details/gdkytmdvy.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.epnwcf.com/Article/details/grlhcnvra.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.vehdjk.com/Article/details/gcziawwkh.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.tarul.cn/Article/details/gchuxyojq.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.yfazqb.com/Article/details/gkanabxnc.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.yfazqb.com/Article/details/gkqkibwwy.sHtML

Ruby: while i < 10; i += 1; end
来源：http://m.share.vehdjk.com/Article/details/grbuuqsgo.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.sjlbkw.cn/Article/details/gerfgwttm.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.epnwcf.com/Article/details/gpmclfhoj.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.epnwcf.com/Article/details/gyhsopjpo.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.bbcook.cn/Article/details/gammllhzd.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.sjlbkw.cn/Article/details/gcoovwcxo.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.yfazqb.com/Article/details/glqbxpgsl.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.tarul.cn/Article/details/gexkarwue.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.epnwcf.com/Article/details/guxmlajxf.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.sjlbkw.cn/Article/details/ggbceuuhe.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.yfazqb.com/Article/details/gsitspxai.sHtML

[B09] break 与 continue
来源：http://www.share.fktsv.cn/Article/details/gcriospny.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.yfazqb.com/Article/details/gxktddnjp.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.sjlbkw.cn/Article/details/gsuxakjoc.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.tarul.cn/Article/details/gxjjrryrz.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.epnwcf.com/Article/details/gcqbghirn.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fktsv.cn/Article/details/gmoakeayi.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.vehdjk.com/Article/details/gqrdjeaja.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.bbcook.cn/Article/details/gmfvturcb.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.yfazqb.com/Article/details/gtmuqmrod.sHtML

[B10] 遍历同时拿索引
来源：http://blog.yfazqb.com/Article/details/gdgtkrfra.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.sjlbkw.cn/Article/details/grmxwocyd.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gwmxzoqpa.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.sjlbkw.cn/Article/details/gmqclpuqi.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.fktsv.cn/Article/details/gtmklgiad.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.tarul.cn/Article/details/gvlnlpwbz.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.epnwcf.com/Article/details/gudazkdnq.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.fktsv.cn/Article/details/gunkbovjv.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gufjfiakx.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.blog.yfazqb.com/Article/details/gktrwlzeb.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.fktsv.cn/Article/details/gpuatevzc.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.bbcook.cn/Article/details/gqselrxpd.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.fktsv.cn/Article/details/gozpyaqwu.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.epnwcf.com/Article/details/gsxupcntt.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.fktsv.cn/Article/details/gyhulqsjl.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.tarul.cn/Article/details/glvjqmkim.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.vehdjk.com/Article/details/gddppdqsn.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.yfazqb.com/Article/details/gziinzlnw.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.fktsv.cn/Article/details/gxbsukpor.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.bbcook.cn/Article/details/ghkqpqzzy.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.yfazqb.com/Article/details/gdhwcsngt.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.yfazqb.com/Article/details/gndypqtab.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.bbcook.cn/Article/details/gfahikrup.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.vehdjk.com/Article/details/gnafsavte.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.bbcook.cn/Article/details/ggmvtshug.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.tarul.cn/Article/details/gcmdqafhb.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.bbcook.cn/Article/details/gvqcgqckt.sHtML

[B13] 判断是否为数字
来源：http://3g.fktsv.cn/Article/details/gorxzrifb.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.fktsv.cn/Article/details/gmgzjfwgb.sHtML

PHP:  is_numeric($x)
来源：http://www.share.fktsv.cn/Article/details/gsvfcusjc.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.bbcook.cn/Article/details/gffpxuocv.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.tarul.cn/Article/details/glvhycrbm.sHtML

Java: x instanceof Number
来源：http://www.share.yfazqb.com/Article/details/gznhayeok.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.tarul.cn/Article/details/guzaanooi.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.epnwcf.com/Article/details/gjzsxsxkj.sHtML

C#:   x is int or double or decimal
来源：http://mobile.epnwcf.com/Article/details/gcoqwddas.sHtML

[B14] 判断值是否在集合内
来源：http://3g.vehdjk.com/Article/details/gsvteygyv.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.bbcook.cn/Article/details/gughzujsx.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.epnwcf.com/Article/details/gbpqiazte.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.vehdjk.com/Article/details/gsbkdgmli.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.vehdjk.com/Article/details/ghqntyudx.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.yfazqb.com/Article/details/gdtueiqlj.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.bbcook.cn/Article/details/ghnzqzjvi.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.epnwcf.com/Article/details/girdonymj.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.tarul.cn/Article/details/guvwsmudy.sHtML

[B15] 布尔运算与取反
来源：http://m.share.sjlbkw.cn/Article/details/ggysjqwat.sHtML

Py:   a and b or not c
来源：http://3g.yfazqb.com/Article/details/giayzywcb.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.fktsv.cn/Article/details/gvrcrndtp.sHtML

JS:   a && b || !c
来源：http://m.share.yfazqb.com/Article/details/grdkonqsx.sHtML

TS:   a && b || !c
来源：http://3g.tarul.cn/Article/details/gotnquoqe.sHtML

Java: a && b || !c
来源：http://www.blog.bbcook.cn/Article/details/gohvtyvbr.sHtML

Go:   a && b || !c
来源：http://blog.tarul.cn/Article/details/ghrfprmxp.sHtML

Ruby: a && b || !c
来源：http://read.share.tarul.cn/Article/details/gpdkmehxj.sHtML

C#:   a && b || !c
来源：http://www.blog.epnwcf.com/Article/details/gihhicplu.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.vehdjk.com/Article/details/gjtxlptqq.sHtML

Py:   if not data: return
来源：http://baike.vehdjk.com/Article/details/gjrqlybpy.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.bbcook.cn/Article/details/goekzzhcl.sHtML

JS:   if (!data) return;
来源：http://www.m.share.vehdjk.com/Article/details/gggpvooxv.sHtML

TS:   if (!data) return;
来源：http://read.share.vehdjk.com/Article/details/gxepdvibb.sHtML

Java: if (data == null) return;
来源：http://www.m.share.sjlbkw.cn/Article/details/gwkwkgwew.sHtML

Go:   if data == nil { return }
来源：http://baike.tarul.cn/Article/details/gotcuymwn.sHtML

Ruby: return if data.nil?
来源：http://www.share.bbcook.cn/Article/details/gumsipwxp.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.tarul.cn/Article/details/gkvzhqisf.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gjnevrlwr.sHtML

C. 函数与作用域
来源：http://3g.vehdjk.com/Article/details/gihvscaff.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gjeyisdzf.sHtML

[C01] 定义函数
来源：http://www.m.share.epnwcf.com/Article/details/galtnwoie.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.tarul.cn/Article/details/gmmusryhi.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.bbcook.cn/Article/details/gulooezhu.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.tarul.cn/Article/details/gbprvvrlo.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.fktsv.cn/Article/details/gufcdewyz.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.fktsv.cn/Article/details/gccfotpgk.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.fktsv.cn/Article/details/ggslqiggp.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.epnwcf.com/Article/details/gyecbgymp.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.yfazqb.com/Article/details/gbcmylhiu.sHtML

[C02] 默认参数
来源：http://mobile.vehdjk.com/Article/details/gfcfofuzs.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.fktsv.cn/Article/details/gseczsxwn.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.bbcook.cn/Article/details/gugogddgu.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.bbcook.cn/Article/details/gjiivdpzq.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.epnwcf.com/Article/details/gkvnjgavs.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.tarul.cn/Article/details/ghfaegxle.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.yfazqb.com/Article/details/gdfcijkvj.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.bbcook.cn/Article/details/ghzhzkedf.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.fktsv.cn/Article/details/gnhsdtfyv.sHtML

[C03] 可变参数
来源：http://3g.fktsv.cn/Article/details/ghgwbkppr.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.yfazqb.com/Article/details/gaskzjabp.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.yfazqb.com/Article/details/gbqaejesw.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.vehdjk.com/Article/details/gkxuawzcf.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gcahcsozb.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.bbcook.cn/Article/details/gryxjtzcg.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.tarul.cn/Article/details/gjfcjznni.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.sjlbkw.cn/Article/details/gftuqnuns.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.yfazqb.com/Article/details/getzmubdb.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.fktsv.cn/Article/details/ggmhdrlcm.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.epnwcf.com/Article/details/gyezlqkja.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.bbcook.cn/Article/details/gtytoiytr.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.epnwcf.com/Article/details/gfnukgjtb.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.vehdjk.com/Article/details/gyaawxmui.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.epnwcf.com/Article/details/gzwruyvod.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.sjlbkw.cn/Article/details/gdbsozhzg.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.yfazqb.com/Article/details/ggjvtqpsr.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.fktsv.cn/Article/details/ghkpcqtfe.sHtML

[C05] 返回多个值
来源：http://3g.yfazqb.com/Article/details/gmrmpyyes.sHtML

Py:   return a, b
来源：http://mobile.epnwcf.com/Article/details/grzkfkzab.sHtML

PHP:  return [$a, $b];
来源：http://wap.bbcook.cn/Article/details/gdkshypox.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.tarul.cn/Article/details/gvbxhqwhg.sHtML

TS:   return { a, b };
来源：http://3g.tarul.cn/Article/details/geqadoopi.sHtML


<!-- 参考信息 -->