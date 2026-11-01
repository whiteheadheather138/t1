代发 wailian999

[A14] 注释写法
来源：http://m.share.fktsv.cn/Article/details/grfctfogn.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://baike.fktsv.cn/Article/details/gtbkzhhhl.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://read.share.epnwcf.com/Article/details/gkctwohcj.sHtML

JS:   // 单行；/* 多行 */
来源：http://m.share.fktsv.cn/Article/details/gicpzhrtq.sHtML

TS:   // 单行；/* 多行 */
来源：http://read.share.fktsv.cn/Article/details/gtfumsnen.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://baike.sjlbkw.cn/Article/details/gyfjtprnc.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.share.fktsv.cn/Article/details/gvlzbxxfi.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://mobile.bbcook.cn/Article/details/giccjnthw.sHtML

C#:   // 单行；/* 多行 */
来源：http://blog.epnwcf.com/Article/details/gkjnhjrbm.sHtML

[A15] 空值判断与默认值
来源：http://baike.fktsv.cn/Article/details/gnxyurxfw.sHtML

Py:   value = data or "默认值"
来源：http://www.m.share.sjlbkw.cn/Article/details/gymfgglpx.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.share.epnwcf.com/Article/details/goopcvzsz.sHtML

JS:   const value = data ?? "默认值";
来源：http://baike.yfazqb.com/Article/details/gkmmevaml.sHtML

TS:   const value = data ?? "默认值";
来源：http://read.share.sjlbkw.cn/Article/details/gxbwbbcqw.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wap.tarul.cn/Article/details/ghrxkxavx.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.blog.bbcook.cn/Article/details/gvqnclmcp.sHtML

Ruby: value = data || "默认值"
来源：http://www.share.epnwcf.com/Article/details/gipmwrgqj.sHtML

C#:   var value = data ?? "默认值";
来源：http://3g.epnwcf.com/Article/details/gckubptxs.sHtML

[A16] 真假值判断规则
来源：http://www.blog.epnwcf.com/Article/details/gghlmtlmv.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.blog.yfazqb.com/Article/details/gfxtrgfot.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://m.share.tarul.cn/Article/details/gmobgopob.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://3g.yfazqb.com/Article/details/gplhockbt.sHtML

TS:   if (!x) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gozwjzqdi.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.blog.yfazqb.com/Article/details/gqqfsozjb.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://mobile.vehdjk.com/Article/details/gzhkzbexo.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://read.share.bbcook.cn/Article/details/gqmubqjkl.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://blog.tarul.cn/Article/details/gtqnsmhrj.sHtML

[A17] 位运算
来源：http://read.share.fktsv.cn/Article/details/gycmrplza.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.sjlbkw.cn/Article/details/gdwozqylx.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mobile.tarul.cn/Article/details/gtbyjvtkp.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.epnwcf.com/Article/details/gpkpmdmvd.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.m.share.vehdjk.com/Article/details/gzjprocwx.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.bbcook.cn/Article/details/gdpgkxegm.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://blog.vehdjk.com/Article/details/gwsfslhfp.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.epnwcf.com/Article/details/gidvmsjsa.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.epnwcf.com/Article/details/gmesrdohm.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.share.vehdjk.com/Article/details/gewjqmpcd.sHtML

Py:   ord("A"); chr(65)
来源：http://m.share.fktsv.cn/Article/details/gpztvadvj.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.share.fktsv.cn/Article/details/gznaojnuy.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.yfazqb.com/Article/details/gjznprwyc.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.fktsv.cn/Article/details/gpobtvuvf.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.share.yfazqb.com/Article/details/gixxtbltf.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://m.share.bbcook.cn/Article/details/gophonbmb.sHtML

Ruby: "A".ord; 65.chr
来源：http://3g.yfazqb.com/Article/details/glrvohsiv.sHtML

C#:   (int)'A'; (char)65
来源：http://blog.tarul.cn/Article/details/gzjfuppdj.sHtML

[A19] 交换两个变量
来源：http://read.share.bbcook.cn/Article/details/gwhewqduj.sHtML

Py:   a, b = b, a
来源：http://www.m.share.vehdjk.com/Article/details/gtqnpsiab.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://m.share.fktsv.cn/Article/details/gsngxnymb.sHtML

JS:   [a, b] = [b, a];
来源：http://www.blog.tarul.cn/Article/details/gtjrggdro.sHtML

TS:   [a, b] = [b, a];
来源：http://wap.epnwcf.com/Article/details/grwursxey.sHtML

Java: int t = a; a = b; b = t;
来源：http://read.share.bbcook.cn/Article/details/gosnlrbwe.sHtML

Go:   a, b = b, a
来源：http://blog.yfazqb.com/Article/details/gncklydqh.sHtML

Ruby: a, b = b, a
来源：http://m.share.bbcook.cn/Article/details/gyzhgmwjh.sHtML

C#:   (a, b) = (b, a);
来源：http://baike.tarul.cn/Article/details/gdicqzfpf.sHtML

[A20] 读取标准输入
来源：http://baike.yfazqb.com/Article/details/gkqywcjnh.sHtML

Py:   name = input("请输入：")
来源：http://wap.tarul.cn/Article/details/gxrswrgmf.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.blog.fktsv.cn/Article/details/gxggotzrf.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wap.sjlbkw.cn/Article/details/gruguxmbb.sHtML

TS:   // Node.js：readline 模块
来源：http://m.share.vehdjk.com/Article/details/gzkjiwjiq.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.share.tarul.cn/Article/details/gfubzterg.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.share.yfazqb.com/Article/details/gciyyrbgm.sHtML

Ruby: gets.chomp
来源：http://www.blog.vehdjk.com/Article/details/gwpinerae.sHtML

C#:   Console.ReadLine();
来源：http://wap.vehdjk.com/Article/details/gimchiaki.sHtML

[A21] 保留指定小数位输出
来源：http://baike.tarul.cn/Article/details/gwscnifec.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.share.vehdjk.com/Article/details/gybzfgvpr.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.m.share.tarul.cn/Article/details/gykjztsru.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.m.share.yfazqb.com/Article/details/gdmkbnwip.sHtML

TS:   (3.14159).toFixed(2)
来源：http://blog.yfazqb.com/Article/details/gjyfhjspb.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://mobile.tarul.cn/Article/details/ggytgjlcm.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://read.share.tarul.cn/Article/details/gxfunvmqk.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://baike.yfazqb.com/Article/details/ggoozhsli.sHtML

C#:   3.14159.ToString("F2")
来源：http://3g.vehdjk.com/Article/details/gubxfwlnh.sHtML

[A22] 获取字符串长度
来源：http://m.share.fktsv.cn/Article/details/gkqchctse.sHtML

Py:   len(s)
来源：http://blog.vehdjk.com/Article/details/gftzqxwjz.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://m.share.bbcook.cn/Article/details/gnkbebozr.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://3g.tarul.cn/Article/details/ghtxxawug.sHtML

TS:   s.length
来源：http://baike.tarul.cn/Article/details/gfsmmwqkx.sHtML

Java: s.length()
来源：http://www.share.sjlbkw.cn/Article/details/gmpvlrdjy.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.share.vehdjk.com/Article/details/gauvnptfr.sHtML

Ruby: s.length
来源：http://www.share.yfazqb.com/Article/details/gxdoktmmm.sHtML

C#:   s.Length
来源：http://www.m.share.sjlbkw.cn/Article/details/gzdwpbjtp.sHtML

[A23] 大小写转换
来源：http://www.blog.vehdjk.com/Article/details/goervuxli.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://m.share.fktsv.cn/Article/details/gwkserqch.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://baike.bbcook.cn/Article/details/gjqbruadl.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.sjlbkw.cn/Article/details/gwbyzsdtm.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.epnwcf.com/Article/details/gjlsaofke.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.share.tarul.cn/Article/details/gyybbcjpq.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mobile.bbcook.cn/Article/details/gdvwkutee.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.blog.tarul.cn/Article/details/greertiuz.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://read.share.vehdjk.com/Article/details/gwqcjhwle.sHtML

[A24] 去除首尾空白
来源：http://blog.fktsv.cn/Article/details/gbfsgkmly.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://read.share.fktsv.cn/Article/details/gqgzpnssb.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.share.sjlbkw.cn/Article/details/ggyrtcjdo.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.bbcook.cn/Article/details/gsbwvsjbq.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.epnwcf.com/Article/details/gqoezbzhz.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wap.fktsv.cn/Article/details/goigxbyyq.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.m.share.bbcook.cn/Article/details/gheigosof.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://baike.tarul.cn/Article/details/gzekafqzb.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wap.bbcook.cn/Article/details/ggmqbwauw.sHtML

[A25] 字符串比较
来源：http://blog.yfazqb.com/Article/details/gplnzdlag.sHtML

Py:   s1 == s2; s1 != s2
来源：http://baike.epnwcf.com/Article/details/gkodgjsuw.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://baike.vehdjk.com/Article/details/guelzsujz.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.fktsv.cn/Article/details/gdernrgyc.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.epnwcf.com/Article/details/gcncyppce.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://baike.vehdjk.com/Article/details/gxgqewrgs.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wap.epnwcf.com/Article/details/gctdxuugz.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.share.fktsv.cn/Article/details/gcpgdcvpv.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.blog.vehdjk.com/Article/details/gyabdduya.sHtML

[A26] 类型转换总览
来源：http://read.share.vehdjk.com/Article/details/gfambrfsw.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.m.share.yfazqb.com/Article/details/ghhsjskpw.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mobile.fktsv.cn/Article/details/gbcpsysoi.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://read.share.vehdjk.com/Article/details/gkpbwqlvq.sHtML

TS:   Number() String() Boolean() x as number
来源：http://m.share.epnwcf.com/Article/details/gzzvscgyx.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://read.share.epnwcf.com/Article/details/gwjziypbc.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://m.share.bbcook.cn/Article/details/gtkaxujvh.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://baike.vehdjk.com/Article/details/gauukjrom.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.blog.yfazqb.com/Article/details/gcbjhoqql.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/ggxxsmjlm.sHtML

B. 流程控制
来源：http://m.share.fktsv.cn/Article/details/gzmaqritc.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/glktxlpov.sHtML

[B01] 条件判断 if / else
来源：http://wap.tarul.cn/Article/details/grdatmplh.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.share.epnwcf.com/Article/details/gsixpiwzs.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.blog.vehdjk.com/Article/details/gfvydstjf.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.sjlbkw.cn/Article/details/gnisdpkhb.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.yfazqb.com/Article/details/gzclzxuja.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://3g.epnwcf.com/Article/details/gbgderrzg.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.share.bbcook.cn/Article/details/gddhkqkgy.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://read.share.sjlbkw.cn/Article/details/gsnovnqxq.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mobile.sjlbkw.cn/Article/details/gmuuljleb.sHtML

[B02] 多分支 else if / elif
来源：http://read.share.tarul.cn/Article/details/gnqbjvamg.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wap.vehdjk.com/Article/details/gnxzkwecj.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.share.sjlbkw.cn/Article/details/gbzuqvwgy.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.sjlbkw.cn/Article/details/gizzddbft.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.bbcook.cn/Article/details/gaoxkbzbp.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.fktsv.cn/Article/details/gasycbnop.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.share.tarul.cn/Article/details/gkrccwxpx.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wap.vehdjk.com/Article/details/gmcsdmemt.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.yfazqb.com/Article/details/gavpaqcqt.sHtML

[B03] switch / match / case
来源：http://m.share.sjlbkw.cn/Article/details/gmjqdiioe.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mobile.bbcook.cn/Article/details/gqnsxxmkx.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.share.epnwcf.com/Article/details/gphxamqez.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.sjlbkw.cn/Article/details/ggjbpkryl.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.epnwcf.com/Article/details/gvjqjjibj.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.yfazqb.com/Article/details/gtaqdyopm.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.blog.bbcook.cn/Article/details/gqebojcmj.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wap.tarul.cn/Article/details/gbcqgxwti.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mobile.sjlbkw.cn/Article/details/gtgxtkivn.sHtML

[B04] for 计数循环
来源：http://m.share.epnwcf.com/Article/details/gnevaekca.sHtML

Py:   for i in range(10): print(i)
来源：http://mobile.epnwcf.com/Article/details/grwcnjyhe.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wap.tarul.cn/Article/details/gjzydqlzu.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.tarul.cn/Article/details/gtvbwnsgw.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.tarul.cn/Article/details/gmlbpxenu.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.blog.sjlbkw.cn/Article/details/gislxamju.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.m.share.sjlbkw.cn/Article/details/gvoylgtay.sHtML

Ruby: 10.times { |i| puts i }
来源：http://mobile.tarul.cn/Article/details/gchwgdyak.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://read.share.yfazqb.com/Article/details/gwiircjrm.sHtML

[B05] 遍历数组 / 列表
来源：http://3g.fktsv.cn/Article/details/gdqivvqpa.sHtML

Py:   for item in arr: print(item)
来源：http://read.share.bbcook.cn/Article/details/gtmsewyuy.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://m.share.yfazqb.com/Article/details/gpxwgctjx.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.epnwcf.com/Article/details/goookyztq.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.tarul.cn/Article/details/gdmcvqwkn.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://mobile.sjlbkw.cn/Article/details/gvlxzgven.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://read.share.fktsv.cn/Article/details/glgnukwys.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.blog.fktsv.cn/Article/details/gfmwmhcjs.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.share.bbcook.cn/Article/details/gduuxuzaz.sHtML

[B06] 遍历字典 / 对象
来源：http://baike.vehdjk.com/Article/details/gmxrnqhqi.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.bbcook.cn/Article/details/gylbhfpfh.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://m.share.epnwcf.com/Article/details/gdhvsigjd.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.tarul.cn/Article/details/gvazdtjws.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.fktsv.cn/Article/details/gcdhpbhgc.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://3g.yfazqb.com/Article/details/gnvripshd.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://3g.fktsv.cn/Article/details/gixaozcog.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wap.fktsv.cn/Article/details/glvjffuoa.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wap.vehdjk.com/Article/details/gkssmyynh.sHtML

[B07] while 循环
来源：http://3g.bbcook.cn/Article/details/gcxbdxwys.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.epnwcf.com/Article/details/guoonktud.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.yfazqb.com/Article/details/gvlovepfr.sHtML

JS:   while (i < 10) { i++; }
来源：http://blog.fktsv.cn/Article/details/gshbrduro.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.blog.bbcook.cn/Article/details/ggfzigfry.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.fktsv.cn/Article/details/gnwakimrh.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.sjlbkw.cn/Article/details/grvmhggjb.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.epnwcf.com/Article/details/gpqglgzoc.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.yfazqb.com/Article/details/gnpxeenwx.sHtML

[B08] do-while（至少执行一次）
来源：http://www.blog.yfazqb.com/Article/details/gyfhrphih.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.epnwcf.com/Article/details/gaoaqtaxs.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.fktsv.cn/Article/details/goojhxabf.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.epnwcf.com/Article/details/gsvcfutyi.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.sjlbkw.cn/Article/details/gvndvhngz.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.sjlbkw.cn/Article/details/gffsasspm.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.fktsv.cn/Article/details/genkforzu.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.sjlbkw.cn/Article/details/gtmsgqogj.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.epnwcf.com/Article/details/gvbhgtnuu.sHtML

[B09] break 与 continue
来源：http://www.m.share.fktsv.cn/Article/details/gnvrvhlfy.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.fktsv.cn/Article/details/gmphooydh.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.tarul.cn/Article/details/gcrrjlpgo.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.epnwcf.com/Article/details/gmhurrazq.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.bbcook.cn/Article/details/gvdudplyq.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.yfazqb.com/Article/details/gsxvmazoq.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.sjlbkw.cn/Article/details/gzuhevdxo.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.bbcook.cn/Article/details/gxlvhjriu.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.epnwcf.com/Article/details/gfusgzeqf.sHtML

[B10] 遍历同时拿索引
来源：http://wap.vehdjk.com/Article/details/gxerzvioz.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.yfazqb.com/Article/details/gptakxrdb.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.sjlbkw.cn/Article/details/gxhmiqsyt.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.tarul.cn/Article/details/gpekkkzie.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.epnwcf.com/Article/details/gyowxkwnb.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.bbcook.cn/Article/details/gzlackqmk.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://baike.tarul.cn/Article/details/gmijzhexi.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.vehdjk.com/Article/details/gatkajuoh.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.bbcook.cn/Article/details/glkcefhea.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.fktsv.cn/Article/details/gxzwmtonq.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.fktsv.cn/Article/details/ghzhafkus.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.vehdjk.com/Article/details/gbnjjbffb.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.vehdjk.com/Article/details/gjzbdwriv.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.bbcook.cn/Article/details/gjemuwtaz.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.sjlbkw.cn/Article/details/gauvneelw.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.fktsv.cn/Article/details/gwyafosiy.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.fktsv.cn/Article/details/gztpcgprq.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.tarul.cn/Article/details/gjdbssoaj.sHtML

[B12] 跳出多层循环
来源：http://read.share.bbcook.cn/Article/details/gkrhctyvu.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.fktsv.cn/Article/details/gvtosubwz.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.vehdjk.com/Article/details/gzlunmzqo.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.sjlbkw.cn/Article/details/gjhxehkwc.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.tarul.cn/Article/details/gbqozhecn.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.bbcook.cn/Article/details/gvxkzvhot.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.epnwcf.com/Article/details/gmnlzubxb.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.vehdjk.com/Article/details/grlwsyhwe.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.fktsv.cn/Article/details/glnyttojx.sHtML

[B13] 判断是否为数字
来源：http://www.share.vehdjk.com/Article/details/gwvhlaksn.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.epnwcf.com/Article/details/gkyandopa.sHtML

PHP:  is_numeric($x)
来源：http://mobile.tarul.cn/Article/details/gamvpmnpl.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.epnwcf.com/Article/details/gtncdpxet.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.bbcook.cn/Article/details/gzuxfktzj.sHtML

Java: x instanceof Number
来源：http://m.share.sjlbkw.cn/Article/details/grjveftsd.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.vehdjk.com/Article/details/gsnoiycrg.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.fktsv.cn/Article/details/goykrnxwb.sHtML

C#:   x is int or double or decimal
来源：http://m.share.sjlbkw.cn/Article/details/gfjsofvtn.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.bbcook.cn/Article/details/gzprdbcyd.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.sjlbkw.cn/Article/details/gzidellhb.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.epnwcf.com/Article/details/gbzljgwpr.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.bbcook.cn/Article/details/grfmhjfes.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.bbcook.cn/Article/details/gopwazzqy.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.epnwcf.com/Article/details/gabncvspx.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.fktsv.cn/Article/details/gbpwrhgqu.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.vehdjk.com/Article/details/ghbrocyvo.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.tarul.cn/Article/details/gdzcdselo.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.tarul.cn/Article/details/gpxyrcjva.sHtML

Py:   a and b or not c
来源：http://read.share.epnwcf.com/Article/details/gdywaowbj.sHtML

PHP:  $a && $b || !$c
来源：http://3g.sjlbkw.cn/Article/details/gqhjnurcn.sHtML

JS:   a && b || !c
来源：http://3g.tarul.cn/Article/details/gnrvkwozk.sHtML

TS:   a && b || !c
来源：http://blog.tarul.cn/Article/details/guvsxtumi.sHtML

Java: a && b || !c
来源：http://wap.bbcook.cn/Article/details/gkhkxvqya.sHtML

Go:   a && b || !c
来源：http://3g.sjlbkw.cn/Article/details/gljqzufnf.sHtML

Ruby: a && b || !c
来源：http://blog.sjlbkw.cn/Article/details/gjacqlusb.sHtML

C#:   a && b || !c
来源：http://www.m.share.sjlbkw.cn/Article/details/gqkoraqgm.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.bbcook.cn/Article/details/gioomabps.sHtML

Py:   if not data: return
来源：http://3g.epnwcf.com/Article/details/gvsrsflxq.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.epnwcf.com/Article/details/gqsghiimx.sHtML

JS:   if (!data) return;
来源：http://www.m.share.fktsv.cn/Article/details/gapcpwxrz.sHtML

TS:   if (!data) return;
来源：http://wap.yfazqb.com/Article/details/gakadodpj.sHtML

Java: if (data == null) return;
来源：http://mobile.vehdjk.com/Article/details/ghluilnpt.sHtML

Go:   if data == nil { return }
来源：http://baike.epnwcf.com/Article/details/gsklfbncm.sHtML

Ruby: return if data.nil?
来源：http://read.share.sjlbkw.cn/Article/details/gyotivjvy.sHtML

C#:   if (data == null) return;
来源：http://wap.bbcook.cn/Article/details/gvteuylwc.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gmwndpmtw.sHtML

C. 函数与作用域
来源：http://read.share.sjlbkw.cn/Article/details/gpvzzngsx.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/glslfljfs.sHtML

[C01] 定义函数
来源：http://www.blog.vehdjk.com/Article/details/ghqripula.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.sjlbkw.cn/Article/details/gimaiuarh.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gcolkargg.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.fktsv.cn/Article/details/gusgrgorl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.bbcook.cn/Article/details/gjbykgjym.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.epnwcf.com/Article/details/gqfossght.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.sjlbkw.cn/Article/details/gesqlnhlc.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.yfazqb.com/Article/details/gmzvuxydh.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.yfazqb.com/Article/details/grpvgadud.sHtML

[C02] 默认参数
来源：http://read.share.tarul.cn/Article/details/ghxvfqndk.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.yfazqb.com/Article/details/gdsigxvzw.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.epnwcf.com/Article/details/gznhjdmur.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.bbcook.cn/Article/details/gtqluoxks.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.tarul.cn/Article/details/gpdpgdswq.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.fktsv.cn/Article/details/gycwznlwe.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.tarul.cn/Article/details/gfuimosod.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.yfazqb.com/Article/details/gklmmslzg.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.bbcook.cn/Article/details/grluoqaow.sHtML

[C03] 可变参数
来源：http://www.m.share.tarul.cn/Article/details/grzoonkru.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.epnwcf.com/Article/details/guxmkvrsz.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.sjlbkw.cn/Article/details/gwwqizyzc.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.sjlbkw.cn/Article/details/gnxsgtlfw.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.bbcook.cn/Article/details/gqrfvjxxi.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.bbcook.cn/Article/details/gydiebayc.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.bbcook.cn/Article/details/gkvwxcogj.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.bbcook.cn/Article/details/gycbxzslw.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.sjlbkw.cn/Article/details/gmkyhgoji.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.bbcook.cn/Article/details/gqeahames.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.epnwcf.com/Article/details/gaalpxhos.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.sjlbkw.cn/Article/details/gkxnjcgbd.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.vehdjk.com/Article/details/gqujodxaa.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.fktsv.cn/Article/details/gutmxjyiq.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.epnwcf.com/Article/details/glxsklkwm.sHtML


<!-- 参考信息 -->