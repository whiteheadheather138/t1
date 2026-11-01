代发 wailian999

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.m.share.yfazqb.com/Article/details/gsxlrssru.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://mobile.fktsv.cn/Article/details/gawnlvtlm.sHtML

TS:   if (!x) {}
来源：http://read.share.tarul.cn/Article/details/gwvqiljhp.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://3g.bbcook.cn/Article/details/gsmqgflrl.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.share.tarul.cn/Article/details/gfbciaxji.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://m.share.vehdjk.com/Article/details/gusmyubzu.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://read.share.bbcook.cn/Article/details/gnkectayh.sHtML

[A17] 位运算
来源：http://www.m.share.sjlbkw.cn/Article/details/gdftbpaiy.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.bbcook.cn/Article/details/godvnzeeq.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://blog.fktsv.cn/Article/details/gzflonlmd.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.bbcook.cn/Article/details/gocactccg.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wap.fktsv.cn/Article/details/gcvhfiwvv.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.epnwcf.com/Article/details/gvuamncvy.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://blog.bbcook.cn/Article/details/gakbtamad.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fktsv.cn/Article/details/gyfsoqcpy.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.fktsv.cn/Article/details/gzeuemktg.sHtML

[A18] 字符与 ASCII 码互转
来源：http://mobile.yfazqb.com/Article/details/gkrxaqjqh.sHtML

Py:   ord("A"); chr(65)
来源：http://read.share.yfazqb.com/Article/details/gigdsglgb.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.share.yfazqb.com/Article/details/gjbsoyirz.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.vehdjk.com/Article/details/guudmlvhk.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://read.share.tarul.cn/Article/details/geypenkqn.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.share.tarul.cn/Article/details/gczczebcm.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://3g.fktsv.cn/Article/details/gzvnjdymm.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.blog.epnwcf.com/Article/details/ganjuvjjk.sHtML

C#:   (int)'A'; (char)65
来源：http://mobile.bbcook.cn/Article/details/gdcxeweyt.sHtML

[A19] 交换两个变量
来源：http://mobile.sjlbkw.cn/Article/details/gmjdqphmk.sHtML

Py:   a, b = b, a
来源：http://read.share.yfazqb.com/Article/details/glcuwctiy.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.m.share.tarul.cn/Article/details/glnrcizpk.sHtML

JS:   [a, b] = [b, a];
来源：http://wap.vehdjk.com/Article/details/gkepmyuxt.sHtML

TS:   [a, b] = [b, a];
来源：http://www.share.yfazqb.com/Article/details/gjauyhaha.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.blog.epnwcf.com/Article/details/glhcpmnqy.sHtML

Go:   a, b = b, a
来源：http://m.share.vehdjk.com/Article/details/gqtufmlly.sHtML

Ruby: a, b = b, a
来源：http://read.share.epnwcf.com/Article/details/gocwoiwut.sHtML

C#:   (a, b) = (b, a);
来源：http://read.share.fktsv.cn/Article/details/gtefdkcac.sHtML

[A20] 读取标准输入
来源：http://www.m.share.tarul.cn/Article/details/gpqkxlgtw.sHtML

Py:   name = input("请输入：")
来源：http://3g.vehdjk.com/Article/details/gkuhndntd.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.share.fktsv.cn/Article/details/gkjtcbxjl.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://read.share.fktsv.cn/Article/details/gkgbcvrig.sHtML

TS:   // Node.js：readline 模块
来源：http://mobile.sjlbkw.cn/Article/details/gvhjqqdzo.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.blog.yfazqb.com/Article/details/gioaomclt.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wap.vehdjk.com/Article/details/ghrxffiew.sHtML

Ruby: gets.chomp
来源：http://m.share.yfazqb.com/Article/details/gqtmsidhj.sHtML

C#:   Console.ReadLine();
来源：http://wap.yfazqb.com/Article/details/gkpvedess.sHtML

[A21] 保留指定小数位输出
来源：http://wap.epnwcf.com/Article/details/gkciyjzbd.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.blog.yfazqb.com/Article/details/gxvedujzu.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://blog.vehdjk.com/Article/details/gowohjckw.sHtML

JS:   (3.14159).toFixed(2)
来源：http://wap.epnwcf.com/Article/details/gqsgvrxsq.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.share.yfazqb.com/Article/details/gfvinixwy.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://m.share.vehdjk.com/Article/details/gtsamcdzd.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://baike.sjlbkw.cn/Article/details/ggyvjlxyz.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://mobile.yfazqb.com/Article/details/ghdjdpvma.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.m.share.yfazqb.com/Article/details/glotmpxjx.sHtML

[A22] 获取字符串长度
来源：http://mobile.bbcook.cn/Article/details/gxlxwdaes.sHtML

Py:   len(s)
来源：http://mobile.epnwcf.com/Article/details/grbjgnuha.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://blog.yfazqb.com/Article/details/gjosfrkdd.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://m.share.vehdjk.com/Article/details/gagfdrxmt.sHtML

TS:   s.length
来源：http://www.m.share.yfazqb.com/Article/details/gnopcnngx.sHtML

Java: s.length()
来源：http://blog.sjlbkw.cn/Article/details/gwfnbnyib.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://m.share.sjlbkw.cn/Article/details/gxyeacgda.sHtML

Ruby: s.length
来源：http://www.m.share.yfazqb.com/Article/details/grqvlmpho.sHtML

C#:   s.Length
来源：http://baike.sjlbkw.cn/Article/details/gcyjnchhu.sHtML

[A23] 大小写转换
来源：http://www.m.share.sjlbkw.cn/Article/details/gfvvcbhsx.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://read.share.epnwcf.com/Article/details/gdbeerbrc.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://3g.bbcook.cn/Article/details/gvaxjwjcs.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.epnwcf.com/Article/details/gfuunpjbi.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.vehdjk.com/Article/details/gvktcohkt.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://m.share.vehdjk.com/Article/details/gvvwxozza.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://baike.epnwcf.com/Article/details/gygdginqr.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://m.share.epnwcf.com/Article/details/geciwanjb.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.blog.yfazqb.com/Article/details/gqqopkhjt.sHtML

[A24] 去除首尾空白
来源：http://wap.bbcook.cn/Article/details/gvldpghfg.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wap.tarul.cn/Article/details/giwlgtzti.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://baike.bbcook.cn/Article/details/gcsupopnb.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.tarul.cn/Article/details/ggzlmuqcr.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.bbcook.cn/Article/details/gmcmmkton.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://blog.tarul.cn/Article/details/glvqfhkcm.sHtML

Go:   strings.TrimSpace(s)
来源：http://baike.sjlbkw.cn/Article/details/gwdmrjdts.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://read.share.vehdjk.com/Article/details/grbeaicpf.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://m.share.bbcook.cn/Article/details/gjdchtfhr.sHtML

[A25] 字符串比较
来源：http://blog.tarul.cn/Article/details/grvfnzsbq.sHtML

Py:   s1 == s2; s1 != s2
来源：http://blog.tarul.cn/Article/details/gkfigsizb.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.share.vehdjk.com/Article/details/gwpahmymb.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.tarul.cn/Article/details/gyvnxdqiw.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.tarul.cn/Article/details/gavrajqle.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://read.share.yfazqb.com/Article/details/gqpkrfyka.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.m.share.vehdjk.com/Article/details/gvmgqpfly.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.m.share.sjlbkw.cn/Article/details/gnirotmgd.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gzpzytagz.sHtML

[A26] 类型转换总览
来源：http://wap.bbcook.cn/Article/details/gkyyseotc.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://blog.sjlbkw.cn/Article/details/gdfcmplnk.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.blog.sjlbkw.cn/Article/details/gytpnsqaz.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://baike.sjlbkw.cn/Article/details/grdwtupjw.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.m.share.yfazqb.com/Article/details/gpipdqpyv.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mobile.bbcook.cn/Article/details/gelhpzwsa.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.m.share.vehdjk.com/Article/details/gocjrmgqe.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.share.vehdjk.com/Article/details/gdvblzepq.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://blog.bbcook.cn/Article/details/gfkafrwii.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/geeltphzq.sHtML

B. 流程控制
来源：http://blog.yfazqb.com/Article/details/gwloczuyu.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gcozygyox.sHtML

[B01] 条件判断 if / else
来源：http://m.share.epnwcf.com/Article/details/gphkodrqc.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://wap.tarul.cn/Article/details/guoqrhsdd.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://read.share.sjlbkw.cn/Article/details/glaljlwml.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.fktsv.cn/Article/details/gtowyiqou.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.sjlbkw.cn/Article/details/gpkovttgw.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://wap.fktsv.cn/Article/details/gquuqnsjb.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://read.share.yfazqb.com/Article/details/ggiofwjcd.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mobile.yfazqb.com/Article/details/gnxgiwxgm.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mobile.fktsv.cn/Article/details/gvxkggsfg.sHtML

[B02] 多分支 else if / elif
来源：http://m.share.sjlbkw.cn/Article/details/gaftjthuk.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://read.share.yfazqb.com/Article/details/gwnswdlpr.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.m.share.fktsv.cn/Article/details/ggrzvdemu.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.vehdjk.com/Article/details/gjqwlhpce.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.yfazqb.com/Article/details/gkeaiqiyk.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fktsv.cn/Article/details/gqyhpccrw.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mobile.bbcook.cn/Article/details/gdruphivs.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://read.share.fktsv.cn/Article/details/gbvrtkwcs.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.sjlbkw.cn/Article/details/gkhfeufrx.sHtML

[B03] switch / match / case
来源：http://wap.yfazqb.com/Article/details/gdobtxvch.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://3g.vehdjk.com/Article/details/ghiakfoss.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mobile.sjlbkw.cn/Article/details/gewargzsc.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.fktsv.cn/Article/details/gltunipnn.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.bbcook.cn/Article/details/gfnmycmjo.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.m.share.tarul.cn/Article/details/ghakrkktk.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://blog.sjlbkw.cn/Article/details/gbvvtapvp.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.share.vehdjk.com/Article/details/ghxsuosgi.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.m.share.bbcook.cn/Article/details/ggarzwsmm.sHtML

[B04] for 计数循环
来源：http://blog.vehdjk.com/Article/details/gmsubxfdz.sHtML

Py:   for i in range(10): print(i)
来源：http://www.share.tarul.cn/Article/details/gxtuityuz.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.blog.sjlbkw.cn/Article/details/gjeftlkqk.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.yfazqb.com/Article/details/grcjxoiyn.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.sjlbkw.cn/Article/details/gebhkgujl.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.bbcook.cn/Article/details/gpeypankh.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wap.yfazqb.com/Article/details/gxhuiojeh.sHtML

Ruby: 10.times { |i| puts i }
来源：http://read.share.bbcook.cn/Article/details/gxzhdbmgu.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://m.share.vehdjk.com/Article/details/gckmvhqme.sHtML

[B05] 遍历数组 / 列表
来源：http://baike.yfazqb.com/Article/details/ghseiyvuw.sHtML

Py:   for item in arr: print(item)
来源：http://www.blog.vehdjk.com/Article/details/giggwdjdc.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://m.share.tarul.cn/Article/details/gjdryuvex.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.sjlbkw.cn/Article/details/goyowbozq.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.tarul.cn/Article/details/gzucoyrzk.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.blog.bbcook.cn/Article/details/gcddnxduz.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://3g.sjlbkw.cn/Article/details/gcjkgvjwp.sHtML

Ruby: arr.each { |item| puts item }
来源：http://mobile.fktsv.cn/Article/details/gdlglgxjo.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.share.fktsv.cn/Article/details/gsjqtqldo.sHtML

[B06] 遍历字典 / 对象
来源：http://mobile.tarul.cn/Article/details/ggvezghep.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.epnwcf.com/Article/details/gtgjgepcw.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://read.share.epnwcf.com/Article/details/gvipfoqve.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.tarul.cn/Article/details/gwqgvqtvi.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.yfazqb.com/Article/details/ghqwzfwuj.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://baike.sjlbkw.cn/Article/details/gqdbmuuxd.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.epnwcf.com/Article/details/gtkdpnjvg.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.sjlbkw.cn/Article/details/ghtjrerij.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.share.epnwcf.com/Article/details/giwzugekk.sHtML

[B07] while 循环
来源：http://www.m.share.fktsv.cn/Article/details/gnprmhewl.sHtML

Py:   while i < 10: i += 1
来源：http://m.share.yfazqb.com/Article/details/gjrwkjxyx.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.blog.epnwcf.com/Article/details/gworlhned.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.fktsv.cn/Article/details/gpncuqcwb.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.epnwcf.com/Article/details/gcykijvpw.sHtML

Java: while (i < 10) { i++; }
来源：http://m.share.epnwcf.com/Article/details/gywvfgylu.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.share.tarul.cn/Article/details/gbtqghzcv.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.tarul.cn/Article/details/gzrtysxho.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.blog.epnwcf.com/Article/details/gidwucduq.sHtML

[B08] do-while（至少执行一次）
来源：http://wap.sjlbkw.cn/Article/details/gbqkmggvq.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.yfazqb.com/Article/details/gxowwhult.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.vehdjk.com/Article/details/gkwefpckt.sHtML

JS:   do { i++; } while (i < 10);
来源：http://m.share.yfazqb.com/Article/details/gcbblxwds.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.m.share.tarul.cn/Article/details/gorokdmwd.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.blog.epnwcf.com/Article/details/gafwukarp.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.yfazqb.com/Article/details/gatseaani.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.bbcook.cn/Article/details/gqwjjwrsh.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.tarul.cn/Article/details/gtthikqic.sHtML

[B09] break 与 continue
来源：http://mobile.sjlbkw.cn/Article/details/gmewqzbar.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.bbcook.cn/Article/details/gggcaioaj.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gywzafcst.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.yfazqb.com/Article/details/gyikagfqm.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.bbcook.cn/Article/details/gfqfwufly.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.tarul.cn/Article/details/gikadgcbe.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.tarul.cn/Article/details/gvsjuzznu.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.epnwcf.com/Article/details/gcbzcbwyw.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fktsv.cn/Article/details/gvyusfsln.sHtML

[B10] 遍历同时拿索引
来源：http://m.share.tarul.cn/Article/details/gvzkuuyzq.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.epnwcf.com/Article/details/ggnyjinqe.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.epnwcf.com/Article/details/gphokcknq.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.epnwcf.com/Article/details/gywzrzywu.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.bbcook.cn/Article/details/gcyjymfes.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.tarul.cn/Article/details/gqfrfpblv.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.fktsv.cn/Article/details/gdjcowguf.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.tarul.cn/Article/details/gnflwocln.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.bbcook.cn/Article/details/grvyxltyq.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.tarul.cn/Article/details/ggevpykzb.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.epnwcf.com/Article/details/gasyudyau.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.bbcook.cn/Article/details/gdbakumvo.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.sjlbkw.cn/Article/details/gnclagjae.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.bbcook.cn/Article/details/gnotaqyjr.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.vehdjk.com/Article/details/gdlkucmpt.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.yfazqb.com/Article/details/gnzqcuusl.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.vehdjk.com/Article/details/gqphrfnsy.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.yfazqb.com/Article/details/geqfxvblx.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.sjlbkw.cn/Article/details/gchkprbfw.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.epnwcf.com/Article/details/gysrxdnko.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.epnwcf.com/Article/details/gbdchtqav.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.tarul.cn/Article/details/gfkhkaduy.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.tarul.cn/Article/details/gbazaqjqm.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.yfazqb.com/Article/details/gvchjjftl.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.yfazqb.com/Article/details/gwrrpahrd.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.tarul.cn/Article/details/glxeztegb.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.epnwcf.com/Article/details/gfowqcaqg.sHtML

[B13] 判断是否为数字
来源：http://3g.sjlbkw.cn/Article/details/gnrggmrcg.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.tarul.cn/Article/details/gpskexert.sHtML

PHP:  is_numeric($x)
来源：http://www.share.tarul.cn/Article/details/gqkwzrspr.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.epnwcf.com/Article/details/gqohfytha.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.sjlbkw.cn/Article/details/gpltmeowd.sHtML

Java: x instanceof Number
来源：http://www.blog.epnwcf.com/Article/details/gentqkjqy.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.bbcook.cn/Article/details/gbecqjsvg.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.tarul.cn/Article/details/gpndqkvry.sHtML

C#:   x is int or double or decimal
来源：http://baike.vehdjk.com/Article/details/ghbrqtcqa.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.vehdjk.com/Article/details/gzbyqagnr.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.tarul.cn/Article/details/gxcidrwwl.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.epnwcf.com/Article/details/gbhnyvezs.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.fktsv.cn/Article/details/gksdyogwc.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.epnwcf.com/Article/details/guiecodpu.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.fktsv.cn/Article/details/gjyfeyzte.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.fktsv.cn/Article/details/ghlyqkgwx.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.tarul.cn/Article/details/gkqlrmfob.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.vehdjk.com/Article/details/gydrtifsv.sHtML

[B15] 布尔运算与取反
来源：http://blog.yfazqb.com/Article/details/gsgsqfmjj.sHtML

Py:   a and b or not c
来源：http://mobile.tarul.cn/Article/details/gqzxrmwdm.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.bbcook.cn/Article/details/gzteyxaib.sHtML

JS:   a && b || !c
来源：http://mobile.tarul.cn/Article/details/ggeosxzzx.sHtML

TS:   a && b || !c
来源：http://m.share.epnwcf.com/Article/details/gpfqetprw.sHtML

Java: a && b || !c
来源：http://read.share.bbcook.cn/Article/details/grpairoxd.sHtML

Go:   a && b || !c
来源：http://baike.epnwcf.com/Article/details/gfltdjjnc.sHtML

Ruby: a && b || !c
来源：http://www.blog.bbcook.cn/Article/details/gyqliydjp.sHtML

C#:   a && b || !c
来源：http://3g.bbcook.cn/Article/details/gsqixvqgf.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.yfazqb.com/Article/details/gjalmdlno.sHtML

Py:   if not data: return
来源：http://wap.tarul.cn/Article/details/goebrmlht.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.sjlbkw.cn/Article/details/gykmlopin.sHtML

JS:   if (!data) return;
来源：http://3g.yfazqb.com/Article/details/gsorrkvez.sHtML

TS:   if (!data) return;
来源：http://wap.yfazqb.com/Article/details/gxrnirvpr.sHtML

Java: if (data == null) return;
来源：http://wap.bbcook.cn/Article/details/greultviq.sHtML

Go:   if data == nil { return }
来源：http://blog.fktsv.cn/Article/details/gsbcgyksf.sHtML

Ruby: return if data.nil?
来源：http://www.blog.fktsv.cn/Article/details/glasatliq.sHtML

C#:   if (data == null) return;
来源：http://mobile.vehdjk.com/Article/details/gefnjxpea.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gygvuyvrp.sHtML

C. 函数与作用域
来源：http://www.m.share.yfazqb.com/Article/details/gfwakqwjz.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gpiivwveg.sHtML

[C01] 定义函数
来源：http://baike.fktsv.cn/Article/details/gqdmosusa.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.vehdjk.com/Article/details/gvdgattro.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.sjlbkw.cn/Article/details/gufmvcpdt.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.yfazqb.com/Article/details/gofxxepuq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.sjlbkw.cn/Article/details/gwbviyomv.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.yfazqb.com/Article/details/gbvdoqhqs.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.epnwcf.com/Article/details/gvakplhjt.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.bbcook.cn/Article/details/gctladqon.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.bbcook.cn/Article/details/gulvlarmn.sHtML

[C02] 默认参数
来源：http://blog.vehdjk.com/Article/details/gzxyttchd.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.epnwcf.com/Article/details/gezwgwfsn.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.sjlbkw.cn/Article/details/ginrifrhi.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.sjlbkw.cn/Article/details/gflzrnttt.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.sjlbkw.cn/Article/details/gwzrjxllv.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.fktsv.cn/Article/details/gtjvahkjn.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.fktsv.cn/Article/details/gpiqxnxps.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.fktsv.cn/Article/details/gkolfklyn.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.epnwcf.com/Article/details/gptdzcayw.sHtML

[C03] 可变参数
来源：http://m.share.epnwcf.com/Article/details/gqjxdadoh.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.tarul.cn/Article/details/glvmmrgvm.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.bbcook.cn/Article/details/gsnzgdhww.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.yfazqb.com/Article/details/gszisklwd.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.epnwcf.com/Article/details/gphytcufl.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.yfazqb.com/Article/details/gdzseccyg.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.bbcook.cn/Article/details/gadzyctnd.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.epnwcf.com/Article/details/gmvmjepyz.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.bbcook.cn/Article/details/gclsqsefc.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.yfazqb.com/Article/details/gcxowwion.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.vehdjk.com/Article/details/gvtjtswvc.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.epnwcf.com/Article/details/gmncelgwn.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.epnwcf.com/Article/details/gcaijzrgh.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.epnwcf.com/Article/details/gjapiraxd.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.tarul.cn/Article/details/gbdpdblsz.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.tarul.cn/Article/details/glsjvuufs.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.yfazqb.com/Article/details/gtjfwwjir.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.sjlbkw.cn/Article/details/gndsabhne.sHtML

[C05] 返回多个值
来源：http://www.m.share.sjlbkw.cn/Article/details/gpqqvctym.sHtML

Py:   return a, b
来源：http://wap.tarul.cn/Article/details/gycvypxeg.sHtML

PHP:  return [$a, $b];
来源：http://blog.vehdjk.com/Article/details/grefgfjwa.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.yfazqb.com/Article/details/gjltqaeyf.sHtML

TS:   return { a, b };
来源：http://baike.yfazqb.com/Article/details/gdoujmvih.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.sjlbkw.cn/Article/details/gvaifzfki.sHtML

Go:   return a, b
来源：http://read.share.yfazqb.com/Article/details/geuqgxfol.sHtML

Ruby: return a, b
来源：http://baike.tarul.cn/Article/details/gqkxupxbi.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.tarul.cn/Article/details/giuswevuo.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.vehdjk.com/Article/details/gktihtklo.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.fktsv.cn/Article/details/gqwgrcgcm.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.sjlbkw.cn/Article/details/gfofejgcp.sHtML

JS:   const square = x => x * x;
来源：http://www.share.tarul.cn/Article/details/gchzxphez.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.tarul.cn/Article/details/gruelqjbl.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.yfazqb.com/Article/details/gresyvxzr.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.yfazqb.com/Article/details/gfvggqwnn.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.tarul.cn/Article/details/gyipgpcky.sHtML


<!-- 参考信息 -->