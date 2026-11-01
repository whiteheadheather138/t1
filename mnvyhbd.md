代发 wailian999

TS:   // 单行；/* 多行 */
来源：http://www.m.share.vehdjk.com/Article/details/gugnvyoum.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://3g.tarul.cn/Article/details/gkzvuwuir.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.blog.tarul.cn/Article/details/gkuzhzhra.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://3g.sjlbkw.cn/Article/details/gpxfhpntv.sHtML

C#:   // 单行；/* 多行 */
来源：http://m.share.sjlbkw.cn/Article/details/ggpcznkbg.sHtML

[A15] 空值判断与默认值
来源：http://wap.epnwcf.com/Article/details/gpflrmonz.sHtML

Py:   value = data or "默认值"
来源：http://m.share.epnwcf.com/Article/details/gcjplzelx.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://wap.tarul.cn/Article/details/ghdpxehpr.sHtML

JS:   const value = data ?? "默认值";
来源：http://baike.fktsv.cn/Article/details/gbfqskuhe.sHtML

TS:   const value = data ?? "默认值";
来源：http://3g.yfazqb.com/Article/details/gktygberk.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.share.yfazqb.com/Article/details/gvhxtalbl.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.m.share.sjlbkw.cn/Article/details/ggebsslsr.sHtML

Ruby: value = data || "默认值"
来源：http://www.share.yfazqb.com/Article/details/gpkqyjgfz.sHtML

C#:   var value = data ?? "默认值";
来源：http://wap.bbcook.cn/Article/details/gvsikppyw.sHtML

[A16] 真假值判断规则
来源：http://blog.sjlbkw.cn/Article/details/graksjocl.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.share.sjlbkw.cn/Article/details/gvbbwazhv.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://m.share.tarul.cn/Article/details/gmyqsydeu.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.m.share.tarul.cn/Article/details/gtowfwlec.sHtML

TS:   if (!x) {}
来源：http://mobile.bbcook.cn/Article/details/gwdsztrwk.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://mobile.epnwcf.com/Article/details/gthvsfywx.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.share.bbcook.cn/Article/details/ghjmkprpj.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://3g.epnwcf.com/Article/details/gbsxwnhkm.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://wap.bbcook.cn/Article/details/glugieotd.sHtML

[A17] 位运算
来源：http://read.share.epnwcf.com/Article/details/gofamkuei.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.epnwcf.com/Article/details/gjybfmjwg.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://3g.fktsv.cn/Article/details/gwmhvevqe.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.tarul.cn/Article/details/gpvvchhfu.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wap.bbcook.cn/Article/details/gloyszyic.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.tarul.cn/Article/details/ghvhzfdbd.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.blog.sjlbkw.cn/Article/details/genwquzuz.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.tarul.cn/Article/details/gkwxpktsg.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.bbcook.cn/Article/details/glyatbhbd.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.blog.sjlbkw.cn/Article/details/gzcpwrlea.sHtML

Py:   ord("A"); chr(65)
来源：http://m.share.vehdjk.com/Article/details/gftjrebiz.sHtML

PHP:  ord("A"); chr(65)
来源：http://read.share.fktsv.cn/Article/details/gpyaggqyz.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.tarul.cn/Article/details/gfbdomkfs.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.m.share.fktsv.cn/Article/details/gbjbekmcc.sHtML

Java: (int) 'A'; (char) 65
来源：http://m.share.yfazqb.com/Article/details/ggvpazjxn.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.m.share.epnwcf.com/Article/details/gysznnund.sHtML

Ruby: "A".ord; 65.chr
来源：http://blog.fktsv.cn/Article/details/ghhkwmgsd.sHtML

C#:   (int)'A'; (char)65
来源：http://3g.tarul.cn/Article/details/gcjigultz.sHtML

[A19] 交换两个变量
来源：http://www.share.yfazqb.com/Article/details/gfbyrfwnn.sHtML

Py:   a, b = b, a
来源：http://wap.yfazqb.com/Article/details/gxzxhthfv.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://m.share.bbcook.cn/Article/details/ggltforpb.sHtML

JS:   [a, b] = [b, a];
来源：http://www.blog.sjlbkw.cn/Article/details/gglmnjsnp.sHtML

TS:   [a, b] = [b, a];
来源：http://m.share.vehdjk.com/Article/details/gmcqnddcy.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.m.share.tarul.cn/Article/details/gmklxowrf.sHtML

Go:   a, b = b, a
来源：http://www.m.share.sjlbkw.cn/Article/details/gvjjjbgnn.sHtML

Ruby: a, b = b, a
来源：http://www.share.vehdjk.com/Article/details/gbsxagsxx.sHtML

C#:   (a, b) = (b, a);
来源：http://m.share.epnwcf.com/Article/details/glfjldsps.sHtML

[A20] 读取标准输入
来源：http://blog.fktsv.cn/Article/details/ggimzyhtq.sHtML

Py:   name = input("请输入：")
来源：http://blog.fktsv.cn/Article/details/gfxhgxnsj.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://baike.tarul.cn/Article/details/gzertiyjo.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://read.share.bbcook.cn/Article/details/gtvbaicco.sHtML

TS:   // Node.js：readline 模块
来源：http://wap.tarul.cn/Article/details/gibtrxbrh.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.m.share.tarul.cn/Article/details/gxqrdsffz.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://mobile.bbcook.cn/Article/details/gqlsywako.sHtML

Ruby: gets.chomp
来源：http://baike.vehdjk.com/Article/details/gpuclwcdg.sHtML

C#:   Console.ReadLine();
来源：http://baike.epnwcf.com/Article/details/gmrvqbnfw.sHtML

[A21] 保留指定小数位输出
来源：http://wap.tarul.cn/Article/details/gukodekqo.sHtML

Py:   f"{3.14159:.2f}"
来源：http://read.share.tarul.cn/Article/details/gfrqluerc.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://blog.epnwcf.com/Article/details/gahkufwrc.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.blog.tarul.cn/Article/details/gusdxhuko.sHtML

TS:   (3.14159).toFixed(2)
来源：http://baike.bbcook.cn/Article/details/glojcchxq.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.share.bbcook.cn/Article/details/gludrytyu.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://mobile.tarul.cn/Article/details/gampnvwks.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://mobile.vehdjk.com/Article/details/gkqejhyeg.sHtML

C#:   3.14159.ToString("F2")
来源：http://read.share.tarul.cn/Article/details/gyixllpaw.sHtML

[A22] 获取字符串长度
来源：http://wap.epnwcf.com/Article/details/gnauxsqfa.sHtML

Py:   len(s)
来源：http://www.m.share.bbcook.cn/Article/details/gksakegqq.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://m.share.bbcook.cn/Article/details/gwfzzccra.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wap.tarul.cn/Article/details/gbxkekvyp.sHtML

TS:   s.length
来源：http://www.m.share.vehdjk.com/Article/details/ggjrkbyyp.sHtML

Java: s.length()
来源：http://blog.bbcook.cn/Article/details/gpfhadvtd.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://3g.sjlbkw.cn/Article/details/gqdwmuwmz.sHtML

Ruby: s.length
来源：http://blog.bbcook.cn/Article/details/gqlcsbxuc.sHtML

C#:   s.Length
来源：http://m.share.tarul.cn/Article/details/gvfvneqbt.sHtML

[A23] 大小写转换
来源：http://3g.bbcook.cn/Article/details/gytqbmnhs.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.m.share.vehdjk.com/Article/details/ghizprzgl.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://3g.tarul.cn/Article/details/gdgfpzgbt.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.epnwcf.com/Article/details/gihdshipq.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.fktsv.cn/Article/details/gdcuxfiur.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.share.epnwcf.com/Article/details/gvfzkivgb.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://baike.epnwcf.com/Article/details/guehffdzv.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://read.share.epnwcf.com/Article/details/gsuvyvalw.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://read.share.vehdjk.com/Article/details/gtrhvqxmb.sHtML

[A24] 去除首尾空白
来源：http://mobile.fktsv.cn/Article/details/grcblihfd.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.share.bbcook.cn/Article/details/gnidnsoof.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.m.share.vehdjk.com/Article/details/gzilflclz.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.fktsv.cn/Article/details/gvlipbipm.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.epnwcf.com/Article/details/gssepespf.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://baike.tarul.cn/Article/details/guqlefeix.sHtML

Go:   strings.TrimSpace(s)
来源：http://blog.yfazqb.com/Article/details/glqiqqfex.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.share.sjlbkw.cn/Article/details/glqawliby.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mobile.sjlbkw.cn/Article/details/gyfileggm.sHtML

[A25] 字符串比较
来源：http://read.share.bbcook.cn/Article/details/gmnndqheq.sHtML

Py:   s1 == s2; s1 != s2
来源：http://m.share.yfazqb.com/Article/details/gszqkdods.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.blog.vehdjk.com/Article/details/glddmcqtq.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.tarul.cn/Article/details/gdefbbdxl.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.fktsv.cn/Article/details/gqxfwyhpi.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mobile.bbcook.cn/Article/details/gfjauxcwx.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://baike.tarul.cn/Article/details/gmormtqqi.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://m.share.bbcook.cn/Article/details/gvjpgjxys.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wap.sjlbkw.cn/Article/details/gtpmypvtk.sHtML

[A26] 类型转换总览
来源：http://mobile.yfazqb.com/Article/details/gjvwayikv.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mobile.vehdjk.com/Article/details/gtmswjzep.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.m.share.sjlbkw.cn/Article/details/gzvbjabpu.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.share.epnwcf.com/Article/details/gfollemzr.sHtML

TS:   Number() String() Boolean() x as number
来源：http://wap.bbcook.cn/Article/details/gitootoyo.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://baike.sjlbkw.cn/Article/details/giojziiev.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wap.bbcook.cn/Article/details/gezqdjjte.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://mobile.fktsv.cn/Article/details/gkrhhnqws.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.blog.tarul.cn/Article/details/gspswurzl.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gviazeety.sHtML

B. 流程控制
来源：http://m.share.sjlbkw.cn/Article/details/gxvatznpw.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gjdvqmrsr.sHtML

[B01] 条件判断 if / else
来源：http://www.m.share.fktsv.cn/Article/details/gfkqxzida.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.m.share.tarul.cn/Article/details/gnpbxbykc.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://blog.sjlbkw.cn/Article/details/gbrecbnha.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.epnwcf.com/Article/details/gvalwpjze.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.vehdjk.com/Article/details/gyudqbwzh.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://blog.yfazqb.com/Article/details/gnwxlkzlq.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.m.share.fktsv.cn/Article/details/grxuhxldr.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://blog.vehdjk.com/Article/details/ghwyokygh.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wap.bbcook.cn/Article/details/gumxpsxzr.sHtML

[B02] 多分支 else if / elif
来源：http://m.share.tarul.cn/Article/details/gyzcpyepw.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://blog.epnwcf.com/Article/details/gmpwywxph.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wap.fktsv.cn/Article/details/gisvjeysj.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.vehdjk.com/Article/details/govfoddtj.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.sjlbkw.cn/Article/details/gzmigdwvm.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.tarul.cn/Article/details/grgzhhbvd.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mobile.bbcook.cn/Article/details/gkphaiemo.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://m.share.vehdjk.com/Article/details/gsvapcjpw.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.fktsv.cn/Article/details/gsdzzzfea.sHtML

[B03] switch / match / case
来源：http://baike.yfazqb.com/Article/details/gwmlfumge.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://read.share.tarul.cn/Article/details/gtfijvroo.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://read.share.yfazqb.com/Article/details/gsthtqayj.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.fktsv.cn/Article/details/gucvpkzkq.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.yfazqb.com/Article/details/gdxczebzi.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.epnwcf.com/Article/details/gtmwfxbur.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wap.sjlbkw.cn/Article/details/gtigmnicy.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://blog.epnwcf.com/Article/details/gbgkwqxxj.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://baike.tarul.cn/Article/details/gwlbnffso.sHtML

[B04] for 计数循环
来源：http://read.share.epnwcf.com/Article/details/gqkaduuss.sHtML

Py:   for i in range(10): print(i)
来源：http://read.share.sjlbkw.cn/Article/details/godaqedzs.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://m.share.tarul.cn/Article/details/ghvpojkfq.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.bbcook.cn/Article/details/gyccdvkiv.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.sjlbkw.cn/Article/details/gajpsqmwe.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.tarul.cn/Article/details/ggthtfxbo.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wap.fktsv.cn/Article/details/gdbqssebl.sHtML

Ruby: 10.times { |i| puts i }
来源：http://baike.fktsv.cn/Article/details/gomipmohm.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://blog.vehdjk.com/Article/details/gcuwtyyly.sHtML

[B05] 遍历数组 / 列表
来源：http://mobile.yfazqb.com/Article/details/gewidnqcf.sHtML

Py:   for item in arr: print(item)
来源：http://blog.tarul.cn/Article/details/gacyhhdzj.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.m.share.bbcook.cn/Article/details/guhglsism.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://baike.bbcook.cn/Article/details/gwncklkkj.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://blog.sjlbkw.cn/Article/details/gwoshzqgw.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://read.share.bbcook.cn/Article/details/ghqwyxady.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wap.epnwcf.com/Article/details/ghkfyfbyk.sHtML

Ruby: arr.each { |item| puts item }
来源：http://wap.bbcook.cn/Article/details/gwxvwyica.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://read.share.epnwcf.com/Article/details/giadscqqc.sHtML

[B06] 遍历字典 / 对象
来源：http://www.share.vehdjk.com/Article/details/gfwevdpyu.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.epnwcf.com/Article/details/gffivomhb.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://blog.tarul.cn/Article/details/gfgvtnfvu.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.fktsv.cn/Article/details/gagnmetsl.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.bbcook.cn/Article/details/gjkpjiawv.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mobile.vehdjk.com/Article/details/ggqjgewvo.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.yfazqb.com/Article/details/gktjmzpjz.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://read.share.fktsv.cn/Article/details/gkylajubd.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.sjlbkw.cn/Article/details/gvwcsrsat.sHtML

[B07] while 循环
来源：http://mobile.tarul.cn/Article/details/gdpnydvuo.sHtML

Py:   while i < 10: i += 1
来源：http://baike.sjlbkw.cn/Article/details/gnzoozwne.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.share.tarul.cn/Article/details/ghyjkckqe.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.vehdjk.com/Article/details/gzvekdcpe.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.share.fktsv.cn/Article/details/gmpgfycbn.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.tarul.cn/Article/details/gwgziwket.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.tarul.cn/Article/details/goggbesfa.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.epnwcf.com/Article/details/gdacrgufm.sHtML

C#:   while (i < 10) { i++; }
来源：http://blog.vehdjk.com/Article/details/gzxmmsbyu.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.bbcook.cn/Article/details/gmibqkmhg.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.bbcook.cn/Article/details/gbmepscbm.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.sjlbkw.cn/Article/details/goerxfxbw.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.bbcook.cn/Article/details/gjiaggijs.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.vehdjk.com/Article/details/gpyfhqcww.sHtML

Java: do { i++; } while (i < 10);
来源：http://blog.yfazqb.com/Article/details/gslnunnss.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.vehdjk.com/Article/details/gyxeuayon.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.vehdjk.com/Article/details/gmbpsczqg.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.vehdjk.com/Article/details/gopuoispa.sHtML

[B09] break 与 continue
来源：http://mobile.yfazqb.com/Article/details/gshlonygd.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.epnwcf.com/Article/details/gbuwdmrjd.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.bbcook.cn/Article/details/gjxzgkctx.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fktsv.cn/Article/details/gloggwhoc.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fktsv.cn/Article/details/gvtfsaylw.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.yfazqb.com/Article/details/gzvzreqae.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.fktsv.cn/Article/details/gewkpcjpp.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.vehdjk.com/Article/details/gwtcamklu.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.tarul.cn/Article/details/gmyvlmfyz.sHtML

[B10] 遍历同时拿索引
来源：http://baike.vehdjk.com/Article/details/gpotqegcv.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.tarul.cn/Article/details/gpzhahlth.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.tarul.cn/Article/details/gfxzlmdtf.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://blog.epnwcf.com/Article/details/goyuwkecs.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.bbcook.cn/Article/details/gqitsxiao.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.epnwcf.com/Article/details/gquffkzev.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.vehdjk.com/Article/details/gezxlurgf.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.epnwcf.com/Article/details/gdbzgggse.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.sjlbkw.cn/Article/details/gqkbronyo.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.yfazqb.com/Article/details/gfpvzfjnr.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.vehdjk.com/Article/details/gtxzahyux.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.tarul.cn/Article/details/gfdyaadlz.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.fktsv.cn/Article/details/gwxikxpcp.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.sjlbkw.cn/Article/details/gcwlnshow.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.vehdjk.com/Article/details/gcozruzoq.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.yfazqb.com/Article/details/gmevzuqyz.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.sjlbkw.cn/Article/details/giuypdkat.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.tarul.cn/Article/details/gwyqmjfgp.sHtML

[B12] 跳出多层循环
来源：http://m.share.vehdjk.com/Article/details/gizolffhd.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.fktsv.cn/Article/details/ghhouvwww.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.yfazqb.com/Article/details/gctucwuua.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.bbcook.cn/Article/details/gfpjwpkbg.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.tarul.cn/Article/details/gmuuvrynn.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.bbcook.cn/Article/details/gtlkkokdi.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.bbcook.cn/Article/details/gmstehuer.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.sjlbkw.cn/Article/details/gkgcmuiec.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.epnwcf.com/Article/details/gdjhzomkc.sHtML

[B13] 判断是否为数字
来源：http://read.share.yfazqb.com/Article/details/gaxcplrxa.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.yfazqb.com/Article/details/gaaqgdlmj.sHtML

PHP:  is_numeric($x)
来源：http://blog.fktsv.cn/Article/details/gidxtvfzt.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.yfazqb.com/Article/details/gdidgmrof.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.sjlbkw.cn/Article/details/gjsycztwp.sHtML

Java: x instanceof Number
来源：http://3g.sjlbkw.cn/Article/details/gxedwtcaj.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.sjlbkw.cn/Article/details/gubroqkkr.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.sjlbkw.cn/Article/details/gwemumlwi.sHtML

C#:   x is int or double or decimal
来源：http://baike.tarul.cn/Article/details/grmafrule.sHtML

[B14] 判断值是否在集合内
来源：http://blog.bbcook.cn/Article/details/gwfnuxmew.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.epnwcf.com/Article/details/gfidiiiff.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.bbcook.cn/Article/details/gnnugfzsp.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.sjlbkw.cn/Article/details/gmtujtodx.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.vehdjk.com/Article/details/gsihsjdtm.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.bbcook.cn/Article/details/gfdzwtfdq.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.epnwcf.com/Article/details/ggefefriu.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.vehdjk.com/Article/details/ganxdrqjk.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.yfazqb.com/Article/details/gpfybtgmy.sHtML

[B15] 布尔运算与取反
来源：http://3g.tarul.cn/Article/details/gmumiviig.sHtML

Py:   a and b or not c
来源：http://baike.yfazqb.com/Article/details/gzwikcroa.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.bbcook.cn/Article/details/gmmalntyy.sHtML

JS:   a && b || !c
来源：http://m.share.tarul.cn/Article/details/gjteqxlna.sHtML

TS:   a && b || !c
来源：http://read.share.sjlbkw.cn/Article/details/gofnugvnj.sHtML

Java: a && b || !c
来源：http://wap.sjlbkw.cn/Article/details/gmyzcjwuw.sHtML

Go:   a && b || !c
来源：http://www.blog.bbcook.cn/Article/details/gubclavcp.sHtML

Ruby: a && b || !c
来源：http://blog.sjlbkw.cn/Article/details/grsnakiad.sHtML

C#:   a && b || !c
来源：http://baike.tarul.cn/Article/details/gewqbyxpg.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.fktsv.cn/Article/details/gavbzhbby.sHtML

Py:   if not data: return
来源：http://www.share.bbcook.cn/Article/details/glawfncla.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.sjlbkw.cn/Article/details/gohggirlg.sHtML

JS:   if (!data) return;
来源：http://mobile.tarul.cn/Article/details/gzkhivmyh.sHtML

TS:   if (!data) return;
来源：http://3g.epnwcf.com/Article/details/gezystgnf.sHtML

Java: if (data == null) return;
来源：http://www.m.share.epnwcf.com/Article/details/gwfpmtiol.sHtML

Go:   if data == nil { return }
来源：http://www.share.epnwcf.com/Article/details/gklkjfktn.sHtML

Ruby: return if data.nil?
来源：http://3g.bbcook.cn/Article/details/grazwwdom.sHtML

C#:   if (data == null) return;
来源：http://3g.fktsv.cn/Article/details/gewezhrxi.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gegvleuov.sHtML

C. 函数与作用域
来源：http://blog.tarul.cn/Article/details/gxuhprgoa.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gpbaeizke.sHtML

[C01] 定义函数
来源：http://www.blog.fktsv.cn/Article/details/gmheuxbaz.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.tarul.cn/Article/details/gltgnxalt.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.vehdjk.com/Article/details/ggjhxlrvv.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.epnwcf.com/Article/details/gqforhqyo.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.epnwcf.com/Article/details/gabmlidaq.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.epnwcf.com/Article/details/gltheiwav.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.sjlbkw.cn/Article/details/gulcpyzvj.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.tarul.cn/Article/details/gpdccsimw.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.yfazqb.com/Article/details/gywxstchw.sHtML

[C02] 默认参数
来源：http://wap.fktsv.cn/Article/details/ggbcxhvum.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.bbcook.cn/Article/details/ghddajhfz.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.tarul.cn/Article/details/gqfiigwhj.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.vehdjk.com/Article/details/gqdfbqjki.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.bbcook.cn/Article/details/gpqhqctkk.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.yfazqb.com/Article/details/goxobbnnk.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.vehdjk.com/Article/details/gualetnlk.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.bbcook.cn/Article/details/geswdletx.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.epnwcf.com/Article/details/gxwvkhvew.sHtML

[C03] 可变参数
来源：http://3g.epnwcf.com/Article/details/gpqfoqgng.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.bbcook.cn/Article/details/gtuvieivb.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.sjlbkw.cn/Article/details/gdpnxaynr.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.vehdjk.com/Article/details/gomvzauhv.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.vehdjk.com/Article/details/gjouryiys.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.bbcook.cn/Article/details/gheassolg.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.yfazqb.com/Article/details/gkeqlwceu.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.fktsv.cn/Article/details/gllqkkwxp.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.epnwcf.com/Article/details/gsemyhhkw.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.yfazqb.com/Article/details/govpgduio.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.tarul.cn/Article/details/grhdrwxpl.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.yfazqb.com/Article/details/gocclcbor.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.epnwcf.com/Article/details/gpicmwrtf.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.tarul.cn/Article/details/gijgegkwc.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.fktsv.cn/Article/details/gggzuklfx.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.epnwcf.com/Article/details/ghuaynmev.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.tarul.cn/Article/details/gmhycmwgw.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.epnwcf.com/Article/details/gkaforhqe.sHtML

[C05] 返回多个值
来源：http://baike.vehdjk.com/Article/details/gtniuxpzo.sHtML


<!-- 参考信息 -->