代发 wailian999

Ruby: value = data || "默认值"
来源：http://www.m.share.yfazqb.com/Article/details/gatdjeosq.sHtML

C#:   var value = data ?? "默认值";
来源：http://mobile.yfazqb.com/Article/details/ghnxgvbst.sHtML

[A16] 真假值判断规则
来源：http://read.share.bbcook.cn/Article/details/gfktqtjqb.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://read.share.fktsv.cn/Article/details/glfdndsec.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://m.share.fktsv.cn/Article/details/geobyzqtn.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://baike.tarul.cn/Article/details/gboucypuy.sHtML

TS:   if (!x) {}
来源：http://baike.epnwcf.com/Article/details/gdmiffguj.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://blog.sjlbkw.cn/Article/details/gdvuimehx.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.share.sjlbkw.cn/Article/details/gkwnlwwbs.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.blog.epnwcf.com/Article/details/gpfaddmnr.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://blog.tarul.cn/Article/details/gphnsosdw.sHtML

[A17] 位运算
来源：http://baike.fktsv.cn/Article/details/ggrszhpvr.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.yfazqb.com/Article/details/gieyvlxkq.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wap.tarul.cn/Article/details/gpciobvyg.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.bbcook.cn/Article/details/gsyweovte.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.blog.epnwcf.com/Article/details/gdswqwnug.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.bbcook.cn/Article/details/gqrfiybkl.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.blog.sjlbkw.cn/Article/details/gpxhjwqst.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.bbcook.cn/Article/details/gkwwtztbl.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.tarul.cn/Article/details/gomwesynu.sHtML

[A18] 字符与 ASCII 码互转
来源：http://baike.bbcook.cn/Article/details/gubftpcmh.sHtML

Py:   ord("A"); chr(65)
来源：http://www.m.share.epnwcf.com/Article/details/gezjdyvlj.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.share.bbcook.cn/Article/details/gjxmystti.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.fktsv.cn/Article/details/gbczylvjw.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://3g.fktsv.cn/Article/details/gefqfxwtg.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.share.fktsv.cn/Article/details/gzbpfliko.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mobile.vehdjk.com/Article/details/glojnmtph.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.m.share.vehdjk.com/Article/details/gppbkhcyk.sHtML

C#:   (int)'A'; (char)65
来源：http://wap.yfazqb.com/Article/details/gmbzlzidv.sHtML

[A19] 交换两个变量
来源：http://www.share.yfazqb.com/Article/details/gqjxkkcsk.sHtML

Py:   a, b = b, a
来源：http://blog.fktsv.cn/Article/details/gfesnqyaa.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://baike.yfazqb.com/Article/details/gkwrrbmbi.sHtML

JS:   [a, b] = [b, a];
来源：http://read.share.epnwcf.com/Article/details/ghmwpzhks.sHtML

TS:   [a, b] = [b, a];
来源：http://blog.tarul.cn/Article/details/ghnyjlaau.sHtML

Java: int t = a; a = b; b = t;
来源：http://baike.epnwcf.com/Article/details/gavdbrrqi.sHtML

Go:   a, b = b, a
来源：http://wap.epnwcf.com/Article/details/gcrofaadu.sHtML

Ruby: a, b = b, a
来源：http://wap.fktsv.cn/Article/details/gvcdbleea.sHtML

C#:   (a, b) = (b, a);
来源：http://3g.sjlbkw.cn/Article/details/gsfsmuszs.sHtML

[A20] 读取标准输入
来源：http://wap.bbcook.cn/Article/details/gywyukybw.sHtML

Py:   name = input("请输入：")
来源：http://mobile.vehdjk.com/Article/details/gtdabvbnc.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://3g.fktsv.cn/Article/details/grzeetfjc.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://baike.fktsv.cn/Article/details/gsxzwebre.sHtML

TS:   // Node.js：readline 模块
来源：http://read.share.yfazqb.com/Article/details/gsfxxhgnr.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://blog.yfazqb.com/Article/details/gjaxogpwu.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://read.share.bbcook.cn/Article/details/gftkzabga.sHtML

Ruby: gets.chomp
来源：http://read.share.fktsv.cn/Article/details/gzfsxhsnv.sHtML

C#:   Console.ReadLine();
来源：http://baike.tarul.cn/Article/details/garrrltpw.sHtML

[A21] 保留指定小数位输出
来源：http://www.share.tarul.cn/Article/details/gccorcsnc.sHtML

Py:   f"{3.14159:.2f}"
来源：http://3g.tarul.cn/Article/details/grgjzprri.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wap.bbcook.cn/Article/details/gobtvsydp.sHtML

JS:   (3.14159).toFixed(2)
来源：http://baike.fktsv.cn/Article/details/gwzbaclic.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.blog.epnwcf.com/Article/details/gnnvhmxip.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://wap.sjlbkw.cn/Article/details/gakvbektd.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wap.sjlbkw.cn/Article/details/gkqzsmhiw.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://3g.epnwcf.com/Article/details/gyqmywede.sHtML

C#:   3.14159.ToString("F2")
来源：http://3g.sjlbkw.cn/Article/details/gwpwiurme.sHtML

[A22] 获取字符串长度
来源：http://www.share.fktsv.cn/Article/details/grcznhpwo.sHtML

Py:   len(s)
来源：http://wap.yfazqb.com/Article/details/glilocpzk.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wap.epnwcf.com/Article/details/ggeltndtf.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.share.vehdjk.com/Article/details/gmjpdiugy.sHtML

TS:   s.length
来源：http://m.share.yfazqb.com/Article/details/gyynnfqto.sHtML

Java: s.length()
来源：http://blog.yfazqb.com/Article/details/ghmwxutep.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mobile.vehdjk.com/Article/details/gbtxtuomr.sHtML

Ruby: s.length
来源：http://m.share.fktsv.cn/Article/details/gemeufess.sHtML

C#:   s.Length
来源：http://m.share.yfazqb.com/Article/details/giyclqytz.sHtML

[A23] 大小写转换
来源：http://mobile.sjlbkw.cn/Article/details/gnccvbxws.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://read.share.yfazqb.com/Article/details/geyeibcjx.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.m.share.fktsv.cn/Article/details/glocwpaoh.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.fktsv.cn/Article/details/gzcbhxulj.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.epnwcf.com/Article/details/gtdyjydbp.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://baike.epnwcf.com/Article/details/gdlhgmixd.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wap.yfazqb.com/Article/details/gcamzgvjx.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.blog.epnwcf.com/Article/details/gulysatyn.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://wap.bbcook.cn/Article/details/grtqvbeda.sHtML

[A24] 去除首尾空白
来源：http://www.m.share.fktsv.cn/Article/details/gnkczvlpv.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://read.share.vehdjk.com/Article/details/gwknjeugt.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wap.yfazqb.com/Article/details/gmktcgtxh.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.fktsv.cn/Article/details/gyvwqomjr.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.vehdjk.com/Article/details/gfmwgvjsa.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wap.fktsv.cn/Article/details/gypvmwgqr.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.m.share.tarul.cn/Article/details/gypyfhhsh.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://3g.yfazqb.com/Article/details/gijgstzjf.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wap.tarul.cn/Article/details/ghztfshko.sHtML

[A25] 字符串比较
来源：http://blog.epnwcf.com/Article/details/gzydnmjzn.sHtML

Py:   s1 == s2; s1 != s2
来源：http://wap.fktsv.cn/Article/details/gnqohelvj.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://read.share.vehdjk.com/Article/details/gaeqxspvc.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.bbcook.cn/Article/details/giyjzyzse.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.epnwcf.com/Article/details/gnwmadyuk.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wap.vehdjk.com/Article/details/gzwvtmlai.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://read.share.vehdjk.com/Article/details/gsxusfeuv.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://blog.epnwcf.com/Article/details/gkcmnvpgl.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://blog.bbcook.cn/Article/details/gksyyrhsc.sHtML

[A26] 类型转换总览
来源：http://baike.tarul.cn/Article/details/gxkxbocek.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mobile.yfazqb.com/Article/details/ghtwceibw.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.blog.fktsv.cn/Article/details/gyspgunet.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://3g.vehdjk.com/Article/details/glszzmzyk.sHtML

TS:   Number() String() Boolean() x as number
来源：http://blog.tarul.cn/Article/details/gqznjrquy.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://baike.tarul.cn/Article/details/gsnmkddrs.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://3g.epnwcf.com/Article/details/gxwrrsyek.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://m.share.vehdjk.com/Article/details/gwhzozxvq.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.m.share.bbcook.cn/Article/details/gakbqfclx.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gndloyopd.sHtML

B. 流程控制
来源：http://read.share.fktsv.cn/Article/details/guhiiwoox.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gaxqxoobk.sHtML

[B01] 条件判断 if / else
来源：http://blog.fktsv.cn/Article/details/gzinidqcn.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://wap.yfazqb.com/Article/details/gqfsqgtue.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://blog.fktsv.cn/Article/details/gfcafrxep.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.yfazqb.com/Article/details/gceiaqvdf.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.sjlbkw.cn/Article/details/gzidmsbhc.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://read.share.yfazqb.com/Article/details/ggzxmjeyy.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://3g.bbcook.cn/Article/details/gxpfezjqw.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wap.bbcook.cn/Article/details/gigpolkpc.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://read.share.yfazqb.com/Article/details/gzzwfuwyf.sHtML

[B02] 多分支 else if / elif
来源：http://www.share.yfazqb.com/Article/details/gywfstwyg.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.blog.sjlbkw.cn/Article/details/ghdyybsuo.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://baike.vehdjk.com/Article/details/gejxpnkkk.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.yfazqb.com/Article/details/gzdfdjpwr.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.vehdjk.com/Article/details/gajrbnlww.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.fktsv.cn/Article/details/gdkoiyled.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://m.share.bbcook.cn/Article/details/gvcyzsgkk.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mobile.tarul.cn/Article/details/gxebtjpox.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.sjlbkw.cn/Article/details/gyvftoqgb.sHtML

[B03] switch / match / case
来源：http://blog.yfazqb.com/Article/details/gbborkxsx.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://m.share.tarul.cn/Article/details/ggeynnnfy.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://baike.sjlbkw.cn/Article/details/gdqbetoru.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.tarul.cn/Article/details/glepzauyf.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.tarul.cn/Article/details/gvvwowfry.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.epnwcf.com/Article/details/gnzmdgwcq.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://blog.bbcook.cn/Article/details/gjmrzferm.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://read.share.bbcook.cn/Article/details/gxzwjxuhz.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://read.share.tarul.cn/Article/details/gktupswyh.sHtML

[B04] for 计数循环
来源：http://read.share.sjlbkw.cn/Article/details/gvtdzwwrt.sHtML

Py:   for i in range(10): print(i)
来源：http://baike.fktsv.cn/Article/details/gtdwitdmi.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://read.share.sjlbkw.cn/Article/details/gwebqyncu.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.vehdjk.com/Article/details/gafxphruz.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.vehdjk.com/Article/details/gugmzfvtc.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.share.epnwcf.com/Article/details/gznfimzcf.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.epnwcf.com/Article/details/gobzrwahb.sHtML

Ruby: 10.times { |i| puts i }
来源：http://wap.vehdjk.com/Article/details/gzgzooddp.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mobile.yfazqb.com/Article/details/gbhvflton.sHtML

[B05] 遍历数组 / 列表
来源：http://wap.yfazqb.com/Article/details/gczqcftwl.sHtML

Py:   for item in arr: print(item)
来源：http://baike.vehdjk.com/Article/details/gjbyualoi.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.yfazqb.com/Article/details/gwvbgyydl.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.yfazqb.com/Article/details/grasghsld.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.epnwcf.com/Article/details/gwwaqnezf.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.share.vehdjk.com/Article/details/gxkhyxfty.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wap.fktsv.cn/Article/details/ghggkrksh.sHtML

Ruby: arr.each { |item| puts item }
来源：http://m.share.fktsv.cn/Article/details/gjtcowaho.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://3g.fktsv.cn/Article/details/gxlnkfmjc.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.bbcook.cn/Article/details/gjkvdwldl.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://3g.tarul.cn/Article/details/gphrkidbn.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://3g.yfazqb.com/Article/details/gpnqwvjsv.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.fktsv.cn/Article/details/ggpymskky.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.vehdjk.com/Article/details/guncfwhbj.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.sjlbkw.cn/Article/details/gjsaumbxu.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.fktsv.cn/Article/details/gvbtudsvx.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wap.vehdjk.com/Article/details/gjsujzwrp.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wap.fktsv.cn/Article/details/gcryxtyag.sHtML

[B07] while 循环
来源：http://www.blog.vehdjk.com/Article/details/gfztjrgdd.sHtML

Py:   while i < 10: i += 1
来源：http://mobile.fktsv.cn/Article/details/gosnozhap.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://read.share.fktsv.cn/Article/details/grrmojcrt.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.epnwcf.com/Article/details/gklloyiod.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.sjlbkw.cn/Article/details/gxrzxuhlb.sHtML

Java: while (i < 10) { i++; }
来源：http://mobile.yfazqb.com/Article/details/glntiygfw.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.share.sjlbkw.cn/Article/details/gkwvtebhd.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.tarul.cn/Article/details/gedkoyqws.sHtML

C#:   while (i < 10) { i++; }
来源：http://blog.vehdjk.com/Article/details/gujrlmfdl.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.fktsv.cn/Article/details/gikhqwjzl.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://read.share.yfazqb.com/Article/details/gifiattet.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.sjlbkw.cn/Article/details/gkwlyvroo.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.bbcook.cn/Article/details/gjjscpjln.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.yfazqb.com/Article/details/gvsjqnhho.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.fktsv.cn/Article/details/gyasnmrca.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.bbcook.cn/Article/details/geedvmnke.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.tarul.cn/Article/details/gcdcusdlb.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.yfazqb.com/Article/details/gcmnfjcel.sHtML

[B09] break 与 continue
来源：http://baike.sjlbkw.cn/Article/details/gtzeidbwp.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.vehdjk.com/Article/details/gtgdoxgns.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://m.share.vehdjk.com/Article/details/gobekiiia.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.bbcook.cn/Article/details/gszlzmdqs.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.yfazqb.com/Article/details/gikmaxpzg.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.sjlbkw.cn/Article/details/gsjyzthgd.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.epnwcf.com/Article/details/gjhhwffvn.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://read.share.yfazqb.com/Article/details/gshdvqymk.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.yfazqb.com/Article/details/genffnren.sHtML

[B10] 遍历同时拿索引
来源：http://baike.tarul.cn/Article/details/ghghpqsnf.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.epnwcf.com/Article/details/gcagiytzy.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.fktsv.cn/Article/details/gwugeperl.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.bbcook.cn/Article/details/gzzsspsaj.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.yfazqb.com/Article/details/gdzoshbow.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.fktsv.cn/Article/details/gugrzlpck.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.epnwcf.com/Article/details/gbbujxiri.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.sjlbkw.cn/Article/details/gmlssqesi.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.tarul.cn/Article/details/ggyipwoky.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.fktsv.cn/Article/details/gwhrelbrg.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.vehdjk.com/Article/details/gbzkmursf.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.bbcook.cn/Article/details/gtatfbcly.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.yfazqb.com/Article/details/gerecazvy.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.tarul.cn/Article/details/gufvzcqik.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.sjlbkw.cn/Article/details/gjveeraux.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.tarul.cn/Article/details/gnsgtpaqv.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.tarul.cn/Article/details/gzeqgpooy.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.bbcook.cn/Article/details/ghuhaycax.sHtML

[B12] 跳出多层循环
来源：http://read.share.epnwcf.com/Article/details/ganezqktx.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.epnwcf.com/Article/details/gloagsxnf.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.tarul.cn/Article/details/ghhvdxvka.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fktsv.cn/Article/details/gpxypieib.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.sjlbkw.cn/Article/details/gqfhdsbwp.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.epnwcf.com/Article/details/gcxzotutz.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.yfazqb.com/Article/details/gsslxkqom.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.vehdjk.com/Article/details/giuofvaip.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.vehdjk.com/Article/details/geecxxuac.sHtML

[B13] 判断是否为数字
来源：http://m.share.yfazqb.com/Article/details/guovjsqyz.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.yfazqb.com/Article/details/gcxazksni.sHtML

PHP:  is_numeric($x)
来源：http://baike.yfazqb.com/Article/details/gbodbedeu.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.fktsv.cn/Article/details/gckfohenw.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.bbcook.cn/Article/details/gttbfmwgt.sHtML

Java: x instanceof Number
来源：http://3g.sjlbkw.cn/Article/details/ghivqebua.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.sjlbkw.cn/Article/details/gdmaqwrvb.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.tarul.cn/Article/details/gyimzzqfp.sHtML

C#:   x is int or double or decimal
来源：http://read.share.epnwcf.com/Article/details/grkjowqtn.sHtML

[B14] 判断值是否在集合内
来源：http://baike.vehdjk.com/Article/details/gjqqaswus.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.bbcook.cn/Article/details/grnnotcjl.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.sjlbkw.cn/Article/details/grgottejf.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.vehdjk.com/Article/details/gcqhuvimc.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.vehdjk.com/Article/details/gtcefhbti.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.vehdjk.com/Article/details/gvywagalc.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.sjlbkw.cn/Article/details/giggejqsm.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.yfazqb.com/Article/details/golwhwcka.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.epnwcf.com/Article/details/grcchujsg.sHtML

[B15] 布尔运算与取反
来源：http://mobile.tarul.cn/Article/details/gosnigjox.sHtML

Py:   a and b or not c
来源：http://3g.bbcook.cn/Article/details/geeydtihd.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.sjlbkw.cn/Article/details/geymfulvl.sHtML

JS:   a && b || !c
来源：http://www.share.bbcook.cn/Article/details/gfqblaukd.sHtML

TS:   a && b || !c
来源：http://mobile.bbcook.cn/Article/details/gymzmnfnp.sHtML

Java: a && b || !c
来源：http://wap.yfazqb.com/Article/details/gvkhjecuf.sHtML

Go:   a && b || !c
来源：http://www.blog.bbcook.cn/Article/details/gywmhaoeb.sHtML

Ruby: a && b || !c
来源：http://mobile.yfazqb.com/Article/details/ghcbyoqaz.sHtML

C#:   a && b || !c
来源：http://wap.epnwcf.com/Article/details/gtvmhkfaa.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.fktsv.cn/Article/details/gjjeomklz.sHtML

Py:   if not data: return
来源：http://blog.tarul.cn/Article/details/gkpyaqzmy.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.sjlbkw.cn/Article/details/gmtqvxjyz.sHtML

JS:   if (!data) return;
来源：http://read.share.tarul.cn/Article/details/gqbmvzrwj.sHtML

TS:   if (!data) return;
来源：http://baike.epnwcf.com/Article/details/gqpnrqsut.sHtML

Java: if (data == null) return;
来源：http://blog.sjlbkw.cn/Article/details/gfxugijuo.sHtML

Go:   if data == nil { return }
来源：http://read.share.tarul.cn/Article/details/gxxodmubs.sHtML

Ruby: return if data.nil?
来源：http://www.blog.epnwcf.com/Article/details/gbkiffzur.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.vehdjk.com/Article/details/gcbmsyyxo.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gpbpryiim.sHtML

C. 函数与作用域
来源：http://blog.sjlbkw.cn/Article/details/gohzdlaed.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/grqxfihoc.sHtML

[C01] 定义函数
来源：http://mobile.epnwcf.com/Article/details/gdwoetfwf.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.epnwcf.com/Article/details/gyjcqogyo.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.tarul.cn/Article/details/ggpegcltd.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.epnwcf.com/Article/details/grpdertui.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.epnwcf.com/Article/details/gqqgzicbg.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.fktsv.cn/Article/details/gjahcrirr.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.bbcook.cn/Article/details/gzrnyiwot.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.fktsv.cn/Article/details/gtnwistyg.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.tarul.cn/Article/details/ggkcaivpl.sHtML

[C02] 默认参数
来源：http://read.share.epnwcf.com/Article/details/gfheogvhi.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.bbcook.cn/Article/details/geocqtdpp.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.vehdjk.com/Article/details/gnzerkwcf.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.epnwcf.com/Article/details/gkxkqwixv.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.bbcook.cn/Article/details/gmvtntfdl.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.yfazqb.com/Article/details/gefxknvph.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.epnwcf.com/Article/details/gcnpmrkyi.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.fktsv.cn/Article/details/gwztzfcnd.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.vehdjk.com/Article/details/gmsllqmmn.sHtML

[C03] 可变参数
来源：http://3g.tarul.cn/Article/details/gcyvrckde.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.bbcook.cn/Article/details/gfbbzeqfe.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.bbcook.cn/Article/details/gbskwprqi.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.yfazqb.com/Article/details/gwbwqvtdg.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.sjlbkw.cn/Article/details/gqmtzxhrt.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.epnwcf.com/Article/details/grhmdtrsp.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.epnwcf.com/Article/details/ghjnkgojc.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.tarul.cn/Article/details/ggqrmpwse.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.sjlbkw.cn/Article/details/gxmqsldqn.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.sjlbkw.cn/Article/details/gfznrxber.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.fktsv.cn/Article/details/gwxwjyori.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.yfazqb.com/Article/details/gbsibhdxr.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.bbcook.cn/Article/details/gwivrnucq.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.sjlbkw.cn/Article/details/gjfesevmx.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.yfazqb.com/Article/details/gblivabka.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.yfazqb.com/Article/details/goxalksqv.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.yfazqb.com/Article/details/guxwsitbd.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.vehdjk.com/Article/details/gglvhjibl.sHtML

[C05] 返回多个值
来源：http://wap.yfazqb.com/Article/details/gnkawqycj.sHtML

Py:   return a, b
来源：http://www.m.share.epnwcf.com/Article/details/gnpgbxdpi.sHtML

PHP:  return [$a, $b];
来源：http://3g.yfazqb.com/Article/details/ggxvjwkcu.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.fktsv.cn/Article/details/ghnahpkua.sHtML

TS:   return { a, b };
来源：http://3g.sjlbkw.cn/Article/details/gqptavwil.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.bbcook.cn/Article/details/ggmdjcbox.sHtML

Go:   return a, b
来源：http://baike.epnwcf.com/Article/details/gmyrmvpxi.sHtML

Ruby: return a, b
来源：http://www.blog.epnwcf.com/Article/details/gmpfwlxrq.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.tarul.cn/Article/details/gpozvtukn.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.bbcook.cn/Article/details/goevulxit.sHtML

Py:   square = lambda x: x * x
来源：http://baike.tarul.cn/Article/details/gdzvraqqa.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.bbcook.cn/Article/details/geuspljjy.sHtML

JS:   const square = x => x * x;
来源：http://read.share.vehdjk.com/Article/details/gfuwaujuv.sHtML


<!-- 参考信息 -->