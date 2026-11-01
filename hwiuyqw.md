代发 wailian999

Ruby: value = data || "默认值"
来源：http://www.share.fktsv.cn/Article/details/gdpbcnysy.sHtML

C#:   var value = data ?? "默认值";
来源：http://3g.epnwcf.com/Article/details/gnzrywmfl.sHtML

[A16] 真假值判断规则
来源：http://3g.vehdjk.com/Article/details/gwgocqrym.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.share.tarul.cn/Article/details/gfdqworhe.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://3g.bbcook.cn/Article/details/giyivhyie.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.blog.vehdjk.com/Article/details/gjqmzrdhg.sHtML

TS:   if (!x) {}
来源：http://read.share.yfazqb.com/Article/details/geoprrwgv.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wap.bbcook.cn/Article/details/gxfhihycf.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://m.share.fktsv.cn/Article/details/gzkxwdzji.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.blog.fktsv.cn/Article/details/grwayrdda.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://read.share.epnwcf.com/Article/details/gldyltunj.sHtML

[A17] 位运算
来源：http://mobile.epnwcf.com/Article/details/giuovvcha.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.tarul.cn/Article/details/gvhavhkrr.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.share.sjlbkw.cn/Article/details/giwjaoqic.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.fktsv.cn/Article/details/gsiaowfgt.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://read.share.bbcook.cn/Article/details/gltumyaaj.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.bbcook.cn/Article/details/gxkwecixe.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://baike.epnwcf.com/Article/details/glcsxxufx.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.epnwcf.com/Article/details/gozasoovf.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fktsv.cn/Article/details/gfgqexrqr.sHtML

[A18] 字符与 ASCII 码互转
来源：http://baike.epnwcf.com/Article/details/gsvfyvlkg.sHtML

Py:   ord("A"); chr(65)
来源：http://3g.vehdjk.com/Article/details/giyohwzyd.sHtML

PHP:  ord("A"); chr(65)
来源：http://mobile.sjlbkw.cn/Article/details/gituoyjfn.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.sjlbkw.cn/Article/details/gzbskapip.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://3g.epnwcf.com/Article/details/gewpaseef.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.share.bbcook.cn/Article/details/gwntbefyt.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.m.share.bbcook.cn/Article/details/grjrxujqf.sHtML

Ruby: "A".ord; 65.chr
来源：http://baike.tarul.cn/Article/details/grfwbbxgu.sHtML

C#:   (int)'A'; (char)65
来源：http://www.m.share.sjlbkw.cn/Article/details/gopdrxgwe.sHtML

[A19] 交换两个变量
来源：http://mobile.tarul.cn/Article/details/gbeyblyqw.sHtML

Py:   a, b = b, a
来源：http://baike.fktsv.cn/Article/details/gwvxakihn.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://wap.bbcook.cn/Article/details/gmrsphpzq.sHtML

JS:   [a, b] = [b, a];
来源：http://www.blog.bbcook.cn/Article/details/gmpdfhemj.sHtML

TS:   [a, b] = [b, a];
来源：http://www.share.tarul.cn/Article/details/gzxommaem.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.m.share.bbcook.cn/Article/details/gldencsfx.sHtML

Go:   a, b = b, a
来源：http://www.blog.tarul.cn/Article/details/glcxjxfie.sHtML

Ruby: a, b = b, a
来源：http://www.m.share.sjlbkw.cn/Article/details/gbhhhhhjb.sHtML

C#:   (a, b) = (b, a);
来源：http://www.m.share.sjlbkw.cn/Article/details/gsqlqmzjk.sHtML

[A20] 读取标准输入
来源：http://m.share.epnwcf.com/Article/details/gyjrmrvdp.sHtML

Py:   name = input("请输入：")
来源：http://3g.bbcook.cn/Article/details/gesvdmlvb.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://mobile.sjlbkw.cn/Article/details/gurwljgki.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://mobile.yfazqb.com/Article/details/gzhopaizj.sHtML

TS:   // Node.js：readline 模块
来源：http://blog.epnwcf.com/Article/details/grfkzlciz.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://wap.vehdjk.com/Article/details/ghxhbniro.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://blog.yfazqb.com/Article/details/gflqmweeb.sHtML

Ruby: gets.chomp
来源：http://www.blog.vehdjk.com/Article/details/gpzjwyliv.sHtML

C#:   Console.ReadLine();
来源：http://mobile.fktsv.cn/Article/details/gtzoyecqk.sHtML

[A21] 保留指定小数位输出
来源：http://www.m.share.vehdjk.com/Article/details/gudrftajc.sHtML

Py:   f"{3.14159:.2f}"
来源：http://mobile.vehdjk.com/Article/details/gualkuuzv.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.blog.vehdjk.com/Article/details/gyhjqojwr.sHtML

JS:   (3.14159).toFixed(2)
来源：http://3g.bbcook.cn/Article/details/gvexlkife.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.blog.yfazqb.com/Article/details/gqlnpaerx.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.m.share.vehdjk.com/Article/details/gypwxbudg.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wap.yfazqb.com/Article/details/ghowdgonk.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://baike.yfazqb.com/Article/details/gitulhjwc.sHtML

C#:   3.14159.ToString("F2")
来源：http://wap.fktsv.cn/Article/details/gaxnrlxfg.sHtML

[A22] 获取字符串长度
来源：http://mobile.yfazqb.com/Article/details/gtfwmudcd.sHtML

Py:   len(s)
来源：http://blog.yfazqb.com/Article/details/gcpnhtohw.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://m.share.vehdjk.com/Article/details/gqcpebkjh.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://m.share.epnwcf.com/Article/details/gvtsqrbtg.sHtML

TS:   s.length
来源：http://blog.tarul.cn/Article/details/gejiqybqn.sHtML

Java: s.length()
来源：http://mobile.epnwcf.com/Article/details/gbaornuay.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wap.vehdjk.com/Article/details/griognkng.sHtML

Ruby: s.length
来源：http://3g.epnwcf.com/Article/details/ghfoazxyt.sHtML

C#:   s.Length
来源：http://www.blog.fktsv.cn/Article/details/gjmpddwvm.sHtML

[A23] 大小写转换
来源：http://wap.vehdjk.com/Article/details/gaigwklzk.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://blog.vehdjk.com/Article/details/gyftbcxwx.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wap.epnwcf.com/Article/details/gqanlwars.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.bbcook.cn/Article/details/gliuzbhne.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.sjlbkw.cn/Article/details/gmihhxkqt.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.vehdjk.com/Article/details/gdentfixp.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://read.share.tarul.cn/Article/details/ghqtymver.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wap.sjlbkw.cn/Article/details/gwhdgeayo.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.blog.epnwcf.com/Article/details/glqsnnuut.sHtML

[A24] 去除首尾空白
来源：http://wap.vehdjk.com/Article/details/grvtcuwen.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.blog.tarul.cn/Article/details/gxuesdmhw.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.share.fktsv.cn/Article/details/gozrnqlnq.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.epnwcf.com/Article/details/gakflpeyi.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.fktsv.cn/Article/details/gqwtyhaml.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://m.share.fktsv.cn/Article/details/gkjytaucx.sHtML

Go:   strings.TrimSpace(s)
来源：http://blog.sjlbkw.cn/Article/details/ggptfvzgh.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.blog.tarul.cn/Article/details/guoscimpj.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://m.share.yfazqb.com/Article/details/gksudlcgh.sHtML

[A25] 字符串比较
来源：http://www.m.share.yfazqb.com/Article/details/gyqeldotz.sHtML

Py:   s1 == s2; s1 != s2
来源：http://mobile.fktsv.cn/Article/details/glzezufad.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://m.share.epnwcf.com/Article/details/gkwfiguqb.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.sjlbkw.cn/Article/details/gtozhhakd.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.yfazqb.com/Article/details/gyfwvybjz.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.m.share.yfazqb.com/Article/details/gelwnpqup.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.m.share.fktsv.cn/Article/details/gvsfvakuc.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://baike.tarul.cn/Article/details/ggzpamxwb.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.blog.epnwcf.com/Article/details/gqvmovxqp.sHtML

[A26] 类型转换总览
来源：http://www.m.share.yfazqb.com/Article/details/gmiewknmv.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mobile.epnwcf.com/Article/details/gxezhaqny.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.blog.epnwcf.com/Article/details/gpwzfmyku.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.m.share.fktsv.cn/Article/details/gzwvyoyws.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.blog.fktsv.cn/Article/details/gyxdgtcqf.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.m.share.epnwcf.com/Article/details/gwjlrsiue.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://blog.tarul.cn/Article/details/gjyenhiyv.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://3g.vehdjk.com/Article/details/gvzgptspo.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://3g.tarul.cn/Article/details/ggoyrlnxf.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gmqpftcti.sHtML

B. 流程控制
来源：http://mobile.bbcook.cn/Article/details/gxwnibyxs.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gxknnhjbc.sHtML

[B01] 条件判断 if / else
来源：http://m.share.vehdjk.com/Article/details/gocziasef.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://m.share.bbcook.cn/Article/details/glotdwvho.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://baike.vehdjk.com/Article/details/gpewqdcvi.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.sjlbkw.cn/Article/details/gsievesuq.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.vehdjk.com/Article/details/gppdhsvyk.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.m.share.vehdjk.com/Article/details/gpyexppry.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://m.share.vehdjk.com/Article/details/gjbetrxkf.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.m.share.fktsv.cn/Article/details/gizajhfbp.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://read.share.fktsv.cn/Article/details/gjzmkslut.sHtML

[B02] 多分支 else if / elif
来源：http://www.blog.tarul.cn/Article/details/gtaslxtbb.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.blog.sjlbkw.cn/Article/details/gyukikkzr.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mobile.yfazqb.com/Article/details/gbklahgrk.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.yfazqb.com/Article/details/ggrgqpvsc.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.yfazqb.com/Article/details/gujmblvzu.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.sjlbkw.cn/Article/details/gkhficvsv.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://read.share.tarul.cn/Article/details/gyqafnepz.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://read.share.sjlbkw.cn/Article/details/gsexbxalp.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.fktsv.cn/Article/details/gecmdwpnz.sHtML

[B03] switch / match / case
来源：http://mobile.tarul.cn/Article/details/gwpsabswx.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://baike.tarul.cn/Article/details/ghimkijpa.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://read.share.bbcook.cn/Article/details/gtpqpxqip.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.sjlbkw.cn/Article/details/gvljzsboz.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.sjlbkw.cn/Article/details/gainmapil.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.share.bbcook.cn/Article/details/gexbzbcep.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://blog.fktsv.cn/Article/details/ghpunxxqa.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://m.share.epnwcf.com/Article/details/gdciifwxq.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.m.share.epnwcf.com/Article/details/gcdcrhqjk.sHtML

[B04] for 计数循环
来源：http://www.blog.yfazqb.com/Article/details/gnoterycc.sHtML

Py:   for i in range(10): print(i)
来源：http://www.blog.fktsv.cn/Article/details/gzzpisken.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mobile.sjlbkw.cn/Article/details/giowdtpxt.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.tarul.cn/Article/details/gkagkwhiu.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.sjlbkw.cn/Article/details/gzzwjeyeb.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://3g.fktsv.cn/Article/details/gopitxesh.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.sjlbkw.cn/Article/details/gflanphoa.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.blog.epnwcf.com/Article/details/gdphhfwto.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.blog.fktsv.cn/Article/details/gkjqfronm.sHtML

[B05] 遍历数组 / 列表
来源：http://www.share.vehdjk.com/Article/details/gnfxqpdxw.sHtML

Py:   for item in arr: print(item)
来源：http://3g.bbcook.cn/Article/details/guakvuzdm.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.bbcook.cn/Article/details/gpgznslta.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://read.share.bbcook.cn/Article/details/gtfzqbtzq.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://m.share.sjlbkw.cn/Article/details/gohedezdj.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://mobile.tarul.cn/Article/details/gxdsbeewm.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.blog.sjlbkw.cn/Article/details/ghygjzvee.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.share.bbcook.cn/Article/details/gxbchqxcg.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://3g.fktsv.cn/Article/details/ghpxxlfev.sHtML

[B06] 遍历字典 / 对象
来源：http://m.share.sjlbkw.cn/Article/details/gfhtumqns.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://baike.bbcook.cn/Article/details/glnwerkbs.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://read.share.epnwcf.com/Article/details/goyptvvuh.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.fktsv.cn/Article/details/gsawpojwc.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.vehdjk.com/Article/details/gbflkcvrh.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://3g.tarul.cn/Article/details/gqwjbrhvu.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.epnwcf.com/Article/details/guwgtussm.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.blog.sjlbkw.cn/Article/details/gtgubnjud.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://read.share.yfazqb.com/Article/details/gxqtgwdhc.sHtML

[B07] while 循环
来源：http://www.m.share.vehdjk.com/Article/details/gmqhjvdxg.sHtML

Py:   while i < 10: i += 1
来源：http://m.share.vehdjk.com/Article/details/gcjutooqs.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.vehdjk.com/Article/details/gypubsymj.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.yfazqb.com/Article/details/ghcrfhhsn.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.bbcook.cn/Article/details/gsddspslt.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.vehdjk.com/Article/details/gjviihzpc.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.share.yfazqb.com/Article/details/gkbfvelyz.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.fktsv.cn/Article/details/gspczpaqd.sHtML

C#:   while (i < 10) { i++; }
来源：http://m.share.fktsv.cn/Article/details/gfnwambmm.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.epnwcf.com/Article/details/gpdiegabs.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://3g.yfazqb.com/Article/details/ggujvlavi.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.bbcook.cn/Article/details/gbmmazwkz.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.epnwcf.com/Article/details/glcbgivvg.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.bbcook.cn/Article/details/gahmrxdfi.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.epnwcf.com/Article/details/gxaeuowhk.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.sjlbkw.cn/Article/details/gtcwchwmo.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://read.share.tarul.cn/Article/details/ghbhghoqd.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.yfazqb.com/Article/details/gfimimaou.sHtML

[B09] break 与 continue
来源：http://wap.vehdjk.com/Article/details/gymrwghol.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.tarul.cn/Article/details/gqjdihwtq.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.vehdjk.com/Article/details/gonffdnem.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.sjlbkw.cn/Article/details/glvunbdmf.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fktsv.cn/Article/details/gnbkdewqy.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.yfazqb.com/Article/details/gnvdfxuym.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.yfazqb.com/Article/details/gbuhslcil.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.tarul.cn/Article/details/gtlpnbrfo.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.epnwcf.com/Article/details/gmgsvrsea.sHtML

[B10] 遍历同时拿索引
来源：http://blog.epnwcf.com/Article/details/gkasunfbb.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.epnwcf.com/Article/details/gtsbbuwzi.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.epnwcf.com/Article/details/gbyxogzze.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.epnwcf.com/Article/details/gtzkjbykk.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.epnwcf.com/Article/details/gxamcnmyi.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://3g.bbcook.cn/Article/details/ggketqmdg.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.tarul.cn/Article/details/gjxrzdogs.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.bbcook.cn/Article/details/gigdagjpx.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.yfazqb.com/Article/details/gnoeohzpl.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.bbcook.cn/Article/details/gupvdwzir.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.fktsv.cn/Article/details/gletegskx.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.bbcook.cn/Article/details/gzicamgea.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.epnwcf.com/Article/details/gwxeoxvve.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.bbcook.cn/Article/details/gfjqxfsnl.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.fktsv.cn/Article/details/ginutzour.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.epnwcf.com/Article/details/gtgmdvvvm.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.vehdjk.com/Article/details/gilwfgvbb.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.sjlbkw.cn/Article/details/grxttvfcc.sHtML

[B12] 跳出多层循环
来源：http://read.share.sjlbkw.cn/Article/details/gjpxexrcf.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.yfazqb.com/Article/details/ghkaervil.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.bbcook.cn/Article/details/gqrmsvwnm.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.tarul.cn/Article/details/gkdvgkrza.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.vehdjk.com/Article/details/gisqfufsr.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.yfazqb.com/Article/details/gmhngncjy.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.fktsv.cn/Article/details/glrqwxdgq.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.bbcook.cn/Article/details/gprhfrfiv.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.epnwcf.com/Article/details/gwgzudlmb.sHtML

[B13] 判断是否为数字
来源：http://mobile.fktsv.cn/Article/details/ghnmnsxgo.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.epnwcf.com/Article/details/gndwncazf.sHtML

PHP:  is_numeric($x)
来源：http://blog.bbcook.cn/Article/details/gvhpufnlq.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.sjlbkw.cn/Article/details/gxohgrgpw.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.tarul.cn/Article/details/gcdzsobjs.sHtML

Java: x instanceof Number
来源：http://read.share.tarul.cn/Article/details/gqmpxfvzs.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.bbcook.cn/Article/details/gkvivczso.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.vehdjk.com/Article/details/gsthntptg.sHtML

C#:   x is int or double or decimal
来源：http://read.share.epnwcf.com/Article/details/gauxuccnb.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.bbcook.cn/Article/details/gorlybchn.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.vehdjk.com/Article/details/gzkounogq.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.vehdjk.com/Article/details/gowpuiqdp.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.tarul.cn/Article/details/gmcgcxegw.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.bbcook.cn/Article/details/gszjryvpr.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.tarul.cn/Article/details/gtkdagpjd.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.sjlbkw.cn/Article/details/gqchbwtjd.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.sjlbkw.cn/Article/details/gpyokccra.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.fktsv.cn/Article/details/gaagcljpn.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.fktsv.cn/Article/details/gxkyruqyj.sHtML

Py:   a and b or not c
来源：http://wap.vehdjk.com/Article/details/ghfeyamaj.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.yfazqb.com/Article/details/glcrixfgr.sHtML

JS:   a && b || !c
来源：http://3g.tarul.cn/Article/details/gthikkqly.sHtML

TS:   a && b || !c
来源：http://www.m.share.vehdjk.com/Article/details/gpvoijxfq.sHtML

Java: a && b || !c
来源：http://baike.tarul.cn/Article/details/geoephfcg.sHtML

Go:   a && b || !c
来源：http://m.share.tarul.cn/Article/details/gqlelxvwb.sHtML

Ruby: a && b || !c
来源：http://3g.sjlbkw.cn/Article/details/gosemfasd.sHtML

C#:   a && b || !c
来源：http://3g.tarul.cn/Article/details/gvymdpjsr.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.tarul.cn/Article/details/gnwrsbrww.sHtML

Py:   if not data: return
来源：http://www.blog.tarul.cn/Article/details/giszftlrb.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.epnwcf.com/Article/details/gbcdeolbe.sHtML

JS:   if (!data) return;
来源：http://www.m.share.vehdjk.com/Article/details/gzvkimlem.sHtML

TS:   if (!data) return;
来源：http://baike.fktsv.cn/Article/details/gcjjjjjdq.sHtML

Java: if (data == null) return;
来源：http://3g.fktsv.cn/Article/details/gdemudewj.sHtML

Go:   if data == nil { return }
来源：http://www.blog.yfazqb.com/Article/details/gxpsfnqim.sHtML

Ruby: return if data.nil?
来源：http://www.share.epnwcf.com/Article/details/gzapubsqw.sHtML

C#:   if (data == null) return;
来源：http://read.share.bbcook.cn/Article/details/gpovwqvff.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gzhaqfgkg.sHtML

C. 函数与作用域
来源：http://3g.vehdjk.com/Article/details/gzxgfyilu.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gqzqcjcsp.sHtML

[C01] 定义函数
来源：http://mobile.fktsv.cn/Article/details/gykzuelht.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.sjlbkw.cn/Article/details/gjmgqnafc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.vehdjk.com/Article/details/gvamoooug.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.bbcook.cn/Article/details/gycaunyhl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.vehdjk.com/Article/details/gtfksztgz.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.fktsv.cn/Article/details/gkbnxymmr.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.tarul.cn/Article/details/gljqsumdx.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.epnwcf.com/Article/details/gbrrtrvtx.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.bbcook.cn/Article/details/govdakafe.sHtML

[C02] 默认参数
来源：http://mobile.epnwcf.com/Article/details/gxeecthbt.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.epnwcf.com/Article/details/gkuwgikyo.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.yfazqb.com/Article/details/gklofkiet.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.sjlbkw.cn/Article/details/gtpvliohx.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.bbcook.cn/Article/details/gpcvzmxxk.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.sjlbkw.cn/Article/details/gtfpzywmb.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.vehdjk.com/Article/details/gcevkiwjf.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.tarul.cn/Article/details/gotzgjemm.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.epnwcf.com/Article/details/gzxfztzki.sHtML

[C03] 可变参数
来源：http://baike.vehdjk.com/Article/details/grhqftbht.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.vehdjk.com/Article/details/goyyezlfy.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.epnwcf.com/Article/details/guqeqvmjx.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.vehdjk.com/Article/details/gutuqagfm.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.tarul.cn/Article/details/gnahbqxmr.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.yfazqb.com/Article/details/gygrwweot.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.fktsv.cn/Article/details/gyuhxzuut.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.vehdjk.com/Article/details/gfwannpcp.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.tarul.cn/Article/details/gybemmaxs.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.vehdjk.com/Article/details/ggajvzwki.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.epnwcf.com/Article/details/gbxesxrnl.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.yfazqb.com/Article/details/gsopaauyb.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.vehdjk.com/Article/details/ghdlvaifh.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.epnwcf.com/Article/details/gengmtksj.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.epnwcf.com/Article/details/gxjwlayce.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.yfazqb.com/Article/details/gednoouxr.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.yfazqb.com/Article/details/gvpnnnoit.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.fktsv.cn/Article/details/gdvysztpo.sHtML

[C05] 返回多个值
来源：http://blog.epnwcf.com/Article/details/gxaqrvfbl.sHtML

Py:   return a, b
来源：http://www.blog.bbcook.cn/Article/details/gspmhtfye.sHtML

PHP:  return [$a, $b];
来源：http://read.share.yfazqb.com/Article/details/gvldghlod.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.fktsv.cn/Article/details/gikkqfzgo.sHtML

TS:   return { a, b };
来源：http://read.share.bbcook.cn/Article/details/gwyxiepkw.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.bbcook.cn/Article/details/gdhdsfluu.sHtML

Go:   return a, b
来源：http://blog.bbcook.cn/Article/details/gmjstvfer.sHtML

Ruby: return a, b
来源：http://mobile.vehdjk.com/Article/details/gsygoexsm.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.vehdjk.com/Article/details/gyqualrgu.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.fktsv.cn/Article/details/gryfyqtlp.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.bbcook.cn/Article/details/gbmluranm.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.tarul.cn/Article/details/gnqbgpmfw.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.yfazqb.com/Article/details/ggivkacxp.sHtML


<!-- 参考信息 -->