代发 wailian999

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://baike.yfazqb.com/Article/details/gganpbtdi.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.share.epnwcf.com/Article/details/gylguabzl.sHtML

TS:   if (!x) {}
来源：http://wap.fktsv.cn/Article/details/ggpwbczux.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wap.fktsv.cn/Article/details/gdidpumah.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.m.share.epnwcf.com/Article/details/ghldjevxn.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://mobile.sjlbkw.cn/Article/details/ggyxorhxa.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://baike.epnwcf.com/Article/details/gafxxuujw.sHtML

[A17] 位运算
来源：http://read.share.bbcook.cn/Article/details/gtxiuctew.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.vehdjk.com/Article/details/ghogzdnms.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.blog.bbcook.cn/Article/details/gzotmarag.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.tarul.cn/Article/details/gxnszkxrx.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://blog.fktsv.cn/Article/details/gstbmtwbr.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.tarul.cn/Article/details/giteiefaq.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://mobile.bbcook.cn/Article/details/gtdcnfesu.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.epnwcf.com/Article/details/gdmmevixz.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.epnwcf.com/Article/details/godbxzhnt.sHtML

[A18] 字符与 ASCII 码互转
来源：http://m.share.tarul.cn/Article/details/gkzearqik.sHtML

Py:   ord("A"); chr(65)
来源：http://mobile.bbcook.cn/Article/details/gafmehamc.sHtML

PHP:  ord("A"); chr(65)
来源：http://m.share.yfazqb.com/Article/details/gnijacnbh.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.m.share.tarul.cn/Article/details/gbxgjxuzz.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.bbcook.cn/Article/details/gamnplgms.sHtML

Java: (int) 'A'; (char) 65
来源：http://baike.sjlbkw.cn/Article/details/gvrrjunca.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://read.share.vehdjk.com/Article/details/gvqryvrzq.sHtML

Ruby: "A".ord; 65.chr
来源：http://wap.sjlbkw.cn/Article/details/gduzyajly.sHtML

C#:   (int)'A'; (char)65
来源：http://blog.yfazqb.com/Article/details/gxxjasguu.sHtML

[A19] 交换两个变量
来源：http://wap.tarul.cn/Article/details/garcdhmmd.sHtML

Py:   a, b = b, a
来源：http://www.blog.sjlbkw.cn/Article/details/glutaayef.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://blog.sjlbkw.cn/Article/details/gonwhwgwc.sHtML

JS:   [a, b] = [b, a];
来源：http://m.share.bbcook.cn/Article/details/gayxwxtwr.sHtML

TS:   [a, b] = [b, a];
来源：http://blog.bbcook.cn/Article/details/gkfahukev.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.share.bbcook.cn/Article/details/gbgkopugg.sHtML

Go:   a, b = b, a
来源：http://m.share.yfazqb.com/Article/details/gnbypkzgz.sHtML

Ruby: a, b = b, a
来源：http://www.blog.sjlbkw.cn/Article/details/gcrnkibhs.sHtML

C#:   (a, b) = (b, a);
来源：http://wap.epnwcf.com/Article/details/goailzpvk.sHtML

[A20] 读取标准输入
来源：http://baike.fktsv.cn/Article/details/gcfbhdwoo.sHtML

Py:   name = input("请输入：")
来源：http://www.m.share.yfazqb.com/Article/details/gtxglaceu.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://3g.bbcook.cn/Article/details/gamwlnrio.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://blog.tarul.cn/Article/details/gxwnssefp.sHtML

TS:   // Node.js：readline 模块
来源：http://baike.fktsv.cn/Article/details/gonruygot.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.m.share.yfazqb.com/Article/details/gbxnesltu.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://mobile.epnwcf.com/Article/details/ghbeknutf.sHtML

Ruby: gets.chomp
来源：http://baike.yfazqb.com/Article/details/gciwywqzv.sHtML

C#:   Console.ReadLine();
来源：http://www.m.share.sjlbkw.cn/Article/details/gijhwhrdm.sHtML

[A21] 保留指定小数位输出
来源：http://blog.epnwcf.com/Article/details/gbcgfxxdq.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.m.share.epnwcf.com/Article/details/grozmmyiy.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://blog.vehdjk.com/Article/details/gezctsdjn.sHtML

JS:   (3.14159).toFixed(2)
来源：http://wap.vehdjk.com/Article/details/gbcjjgkzl.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.blog.sjlbkw.cn/Article/details/gghdndvst.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://3g.epnwcf.com/Article/details/gmvdsiynv.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.blog.fktsv.cn/Article/details/glceixqqv.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://mobile.epnwcf.com/Article/details/gbwiqufms.sHtML

C#:   3.14159.ToString("F2")
来源：http://blog.epnwcf.com/Article/details/gyaxerqsd.sHtML

[A22] 获取字符串长度
来源：http://baike.vehdjk.com/Article/details/glfzlkfak.sHtML

Py:   len(s)
来源：http://www.share.yfazqb.com/Article/details/gbdgcnvhs.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.blog.fktsv.cn/Article/details/gmxqeueyx.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://blog.vehdjk.com/Article/details/gencvqkng.sHtML

TS:   s.length
来源：http://www.share.yfazqb.com/Article/details/gfnvpcitm.sHtML

Java: s.length()
来源：http://www.share.vehdjk.com/Article/details/gogbjwbht.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://read.share.epnwcf.com/Article/details/gjupbcijn.sHtML

Ruby: s.length
来源：http://m.share.bbcook.cn/Article/details/gjheujufk.sHtML

C#:   s.Length
来源：http://read.share.epnwcf.com/Article/details/gulaekpvo.sHtML

[A23] 大小写转换
来源：http://blog.sjlbkw.cn/Article/details/gwiqtkmpg.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://blog.bbcook.cn/Article/details/gxyjujhcp.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wap.bbcook.cn/Article/details/gfvcrfzsv.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.bbcook.cn/Article/details/gjnkjsmaw.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.sjlbkw.cn/Article/details/gmfktwpgs.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.bbcook.cn/Article/details/gaupaqagx.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wap.fktsv.cn/Article/details/gllrdawrx.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wap.epnwcf.com/Article/details/gtqjufjly.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://wap.yfazqb.com/Article/details/gzarabyxu.sHtML

[A24] 去除首尾空白
来源：http://mobile.bbcook.cn/Article/details/gzyafgmso.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://m.share.epnwcf.com/Article/details/greugrfuq.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wap.fktsv.cn/Article/details/ggonpridc.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.tarul.cn/Article/details/ghnzqsrsa.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.yfazqb.com/Article/details/gztldirhk.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://read.share.tarul.cn/Article/details/ghynnqiph.sHtML

Go:   strings.TrimSpace(s)
来源：http://mobile.tarul.cn/Article/details/gwljikssp.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mobile.vehdjk.com/Article/details/gmbvrtwbn.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://m.share.sjlbkw.cn/Article/details/gwbhbyvon.sHtML

[A25] 字符串比较
来源：http://www.share.tarul.cn/Article/details/gvuksykwp.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.share.epnwcf.com/Article/details/gmdjhbmxv.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.share.vehdjk.com/Article/details/gwxsdtwzy.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.sjlbkw.cn/Article/details/gpsnxevnt.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.tarul.cn/Article/details/gqagmyluj.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://blog.tarul.cn/Article/details/gwuaumpvf.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.share.epnwcf.com/Article/details/guamnayeh.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://m.share.tarul.cn/Article/details/grcxamobt.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.share.yfazqb.com/Article/details/gdxxkzyka.sHtML

[A26] 类型转换总览
来源：http://wap.epnwcf.com/Article/details/gykcytoib.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://blog.sjlbkw.cn/Article/details/gunxrxvry.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.blog.bbcook.cn/Article/details/gemnapxoe.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mobile.yfazqb.com/Article/details/geecvdzpk.sHtML

TS:   Number() String() Boolean() x as number
来源：http://3g.sjlbkw.cn/Article/details/gayplxfke.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wap.vehdjk.com/Article/details/gdpnxkuyj.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mobile.epnwcf.com/Article/details/gxsenzsmk.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://read.share.tarul.cn/Article/details/gxtoebznm.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wap.bbcook.cn/Article/details/giyvxijhz.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gersjbbog.sHtML

B. 流程控制
来源：http://m.share.bbcook.cn/Article/details/gmkzuigrd.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gvdgqguxt.sHtML

[B01] 条件判断 if / else
来源：http://3g.vehdjk.com/Article/details/gvogoszbk.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://blog.fktsv.cn/Article/details/gskvtjwdc.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.m.share.tarul.cn/Article/details/gmskhbcem.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.fktsv.cn/Article/details/gnsrbiilv.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.fktsv.cn/Article/details/gwbpqpmvx.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://wap.yfazqb.com/Article/details/gxnjsuhst.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://m.share.bbcook.cn/Article/details/gxgxxgszg.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://read.share.tarul.cn/Article/details/gyryilnpw.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://read.share.yfazqb.com/Article/details/gheswganq.sHtML

[B02] 多分支 else if / elif
来源：http://www.blog.vehdjk.com/Article/details/grqqrykbm.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mobile.epnwcf.com/Article/details/gfljtdaiy.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.share.fktsv.cn/Article/details/gwzdxtqqf.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.yfazqb.com/Article/details/ghovvourj.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.bbcook.cn/Article/details/gpmfjqrjh.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.bbcook.cn/Article/details/glslufcmr.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mobile.epnwcf.com/Article/details/gviholodl.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://3g.epnwcf.com/Article/details/genyijpzu.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.yfazqb.com/Article/details/grhdjupes.sHtML

[B03] switch / match / case
来源：http://blog.yfazqb.com/Article/details/ghhenztjv.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.share.yfazqb.com/Article/details/gjsxtsvwr.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.share.tarul.cn/Article/details/gjdpolned.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.yfazqb.com/Article/details/goamavzph.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.bbcook.cn/Article/details/gdxqfgvmt.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://blog.vehdjk.com/Article/details/glflekpvq.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.m.share.sjlbkw.cn/Article/details/ghvwtzikz.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.share.tarul.cn/Article/details/giogqtbee.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.blog.tarul.cn/Article/details/gmpyrtgez.sHtML

[B04] for 计数循环
来源：http://mobile.yfazqb.com/Article/details/giewplblb.sHtML

Py:   for i in range(10): print(i)
来源：http://blog.sjlbkw.cn/Article/details/gjdqbnyuj.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://baike.bbcook.cn/Article/details/gljhwmlid.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.tarul.cn/Article/details/gzuxddrpy.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.vehdjk.com/Article/details/gejgsutvv.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.blog.bbcook.cn/Article/details/gcznybarw.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://baike.epnwcf.com/Article/details/gqozjfqji.sHtML

Ruby: 10.times { |i| puts i }
来源：http://wap.bbcook.cn/Article/details/getoutluj.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.yfazqb.com/Article/details/gugluruqh.sHtML

[B05] 遍历数组 / 列表
来源：http://www.share.tarul.cn/Article/details/gddgsynji.sHtML

Py:   for item in arr: print(item)
来源：http://www.share.epnwcf.com/Article/details/gjkfrqzuj.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.fktsv.cn/Article/details/gkpxkxabv.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.share.sjlbkw.cn/Article/details/ghfwzbpyk.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.sjlbkw.cn/Article/details/gvocwrauw.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.blog.tarul.cn/Article/details/gtjpotmsx.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wap.fktsv.cn/Article/details/gkxmfgmue.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.epnwcf.com/Article/details/gtpbghwon.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.epnwcf.com/Article/details/grhpxbvzn.sHtML

[B06] 遍历字典 / 对象
来源：http://baike.yfazqb.com/Article/details/gxcvrrgqw.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://m.share.tarul.cn/Article/details/gpnqyqqjn.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://blog.tarul.cn/Article/details/gvcgigqix.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.vehdjk.com/Article/details/geqeipcpa.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.epnwcf.com/Article/details/gwpyjnfyc.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.share.bbcook.cn/Article/details/gdgdfwquu.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mobile.vehdjk.com/Article/details/ggxzoghmh.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wap.bbcook.cn/Article/details/gocmrhhhq.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.bbcook.cn/Article/details/gilsmsctc.sHtML

[B07] while 循环
来源：http://m.share.vehdjk.com/Article/details/ghurgxrwg.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.bbcook.cn/Article/details/gkfdwrvxt.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.yfazqb.com/Article/details/grzwagmzk.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.blog.vehdjk.com/Article/details/gjblzifwq.sHtML

TS:   while (i < 10) { i++; }
来源：http://blog.bbcook.cn/Article/details/gwoieemxh.sHtML

Java: while (i < 10) { i++; }
来源：http://m.share.sjlbkw.cn/Article/details/gtvzpqsen.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.epnwcf.com/Article/details/ggxpzesjo.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.tarul.cn/Article/details/ghowsajre.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.tarul.cn/Article/details/givhjrffn.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.epnwcf.com/Article/details/gxvpnyuzr.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.fktsv.cn/Article/details/gyemmgoia.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.yfazqb.com/Article/details/gkhbheojt.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.fktsv.cn/Article/details/gfbyyefej.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.fktsv.cn/Article/details/gzoziuawl.sHtML

Java: do { i++; } while (i < 10);
来源：http://mobile.bbcook.cn/Article/details/gqdicxsyq.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.sjlbkw.cn/Article/details/gqrrseihr.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.tarul.cn/Article/details/guqugycwl.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.bbcook.cn/Article/details/grfouzgym.sHtML

[B09] break 与 continue
来源：http://read.share.vehdjk.com/Article/details/gvdhpebkm.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.vehdjk.com/Article/details/gpjfpckpo.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.fktsv.cn/Article/details/gzzmaagxp.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.yfazqb.com/Article/details/gdciqihoh.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.tarul.cn/Article/details/gqelpfwme.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fktsv.cn/Article/details/gxuhldiuf.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.fktsv.cn/Article/details/gmxqlrufx.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.bbcook.cn/Article/details/ggzdotrsx.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.sjlbkw.cn/Article/details/gurkwdcpc.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.fktsv.cn/Article/details/gtclkbdtf.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.fktsv.cn/Article/details/glflemkwl.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.bbcook.cn/Article/details/gtqfxhsle.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.epnwcf.com/Article/details/gnmvvkgjl.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.vehdjk.com/Article/details/gtujoxcwr.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.fktsv.cn/Article/details/gvhxltpza.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://baike.epnwcf.com/Article/details/gnvvqvsyz.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.vehdjk.com/Article/details/gpfujnsck.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.epnwcf.com/Article/details/gmkrilssw.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.bbcook.cn/Article/details/glipotuyt.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.bbcook.cn/Article/details/gadosnvca.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.fktsv.cn/Article/details/grftozplh.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.tarul.cn/Article/details/gynnrwkko.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.vehdjk.com/Article/details/glizlmzdf.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.tarul.cn/Article/details/gaymdtuzf.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.epnwcf.com/Article/details/gdroryldn.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.yfazqb.com/Article/details/gejlldaqs.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.fktsv.cn/Article/details/gynaqhgqa.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.yfazqb.com/Article/details/gzccaitbr.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.tarul.cn/Article/details/gwbvqqmsn.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.yfazqb.com/Article/details/geqdfpmlg.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fktsv.cn/Article/details/galiipzjk.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.sjlbkw.cn/Article/details/gxkkkgacb.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.sjlbkw.cn/Article/details/gjezczftl.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.sjlbkw.cn/Article/details/gejhxkngs.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.bbcook.cn/Article/details/gxptakqti.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.yfazqb.com/Article/details/gwzjkccnf.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.yfazqb.com/Article/details/gngtvnrxz.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.bbcook.cn/Article/details/gehgqslkt.sHtML

PHP:  is_numeric($x)
来源：http://baike.tarul.cn/Article/details/gckenxpbz.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.fktsv.cn/Article/details/gccotudil.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.bbcook.cn/Article/details/gssdxriht.sHtML

Java: x instanceof Number
来源：http://mobile.yfazqb.com/Article/details/ghnhpnfem.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.sjlbkw.cn/Article/details/gbrlzgrji.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.tarul.cn/Article/details/gyrvkaovn.sHtML

C#:   x is int or double or decimal
来源：http://3g.sjlbkw.cn/Article/details/gbyykljnj.sHtML

[B14] 判断值是否在集合内
来源：http://blog.sjlbkw.cn/Article/details/gjutswzzo.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.bbcook.cn/Article/details/gdislkhhx.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.sjlbkw.cn/Article/details/gxnuaedfq.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.bbcook.cn/Article/details/guorunqvv.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.epnwcf.com/Article/details/gxpmagpgp.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.tarul.cn/Article/details/gmztulbdx.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.yfazqb.com/Article/details/guddpaeim.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.fktsv.cn/Article/details/gkzdtvwgk.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.fktsv.cn/Article/details/gqwrnqpsa.sHtML

[B15] 布尔运算与取反
来源：http://m.share.tarul.cn/Article/details/gnaooozcp.sHtML

Py:   a and b or not c
来源：http://mobile.yfazqb.com/Article/details/ghyiucaxh.sHtML

PHP:  $a && $b || !$c
来源：http://wap.yfazqb.com/Article/details/goepnypoe.sHtML

JS:   a && b || !c
来源：http://www.blog.fktsv.cn/Article/details/gtyanjovj.sHtML

TS:   a && b || !c
来源：http://baike.epnwcf.com/Article/details/gueizisvy.sHtML

Java: a && b || !c
来源：http://baike.bbcook.cn/Article/details/gmixdhuex.sHtML

Go:   a && b || !c
来源：http://baike.vehdjk.com/Article/details/glwprgirj.sHtML

Ruby: a && b || !c
来源：http://www.blog.fktsv.cn/Article/details/gzgrxnxer.sHtML

C#:   a && b || !c
来源：http://blog.bbcook.cn/Article/details/gobzbpqwc.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.tarul.cn/Article/details/gdwjollvk.sHtML

Py:   if not data: return
来源：http://www.blog.vehdjk.com/Article/details/gppfoxgye.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.vehdjk.com/Article/details/gzzbuckjw.sHtML

JS:   if (!data) return;
来源：http://read.share.sjlbkw.cn/Article/details/gdecwrjvu.sHtML

TS:   if (!data) return;
来源：http://mobile.epnwcf.com/Article/details/gnimgpujv.sHtML

Java: if (data == null) return;
来源：http://www.m.share.tarul.cn/Article/details/ggmmpgowl.sHtML

Go:   if data == nil { return }
来源：http://3g.bbcook.cn/Article/details/gvlodhpzj.sHtML

Ruby: return if data.nil?
来源：http://blog.fktsv.cn/Article/details/ggnxcqwtf.sHtML

C#:   if (data == null) return;
来源：http://www.blog.bbcook.cn/Article/details/gclkigher.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/ghmbxveld.sHtML

C. 函数与作用域
来源：http://www.m.share.vehdjk.com/Article/details/gnjxcnknb.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gtjmzdwne.sHtML

[C01] 定义函数
来源：http://mobile.epnwcf.com/Article/details/gxqvbqyhn.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.epnwcf.com/Article/details/gwtrxlukn.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.sjlbkw.cn/Article/details/grqtgrrtu.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.sjlbkw.cn/Article/details/goyefqakr.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.bbcook.cn/Article/details/gzygvifxt.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.fktsv.cn/Article/details/gontjchgb.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.yfazqb.com/Article/details/gzzorfnhd.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.vehdjk.com/Article/details/gyxxwtrpl.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.yfazqb.com/Article/details/gevtyzacw.sHtML

[C02] 默认参数
来源：http://www.blog.sjlbkw.cn/Article/details/gydtslqkd.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.fktsv.cn/Article/details/gmczmtlbf.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.yfazqb.com/Article/details/giooodqip.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.fktsv.cn/Article/details/grxkywbwt.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.epnwcf.com/Article/details/gmqdqlxkz.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.fktsv.cn/Article/details/gqupxmugb.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.yfazqb.com/Article/details/ginktwrvj.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.yfazqb.com/Article/details/gcfykilbu.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.vehdjk.com/Article/details/goopuybht.sHtML

[C03] 可变参数
来源：http://read.share.fktsv.cn/Article/details/gyqpgongk.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.tarul.cn/Article/details/gjkdkbucj.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.fktsv.cn/Article/details/gqvabwezm.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.vehdjk.com/Article/details/grqsbpabc.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.sjlbkw.cn/Article/details/gcjqcylfl.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.bbcook.cn/Article/details/gxntgrtsh.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.vehdjk.com/Article/details/gidqdyfra.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.vehdjk.com/Article/details/gyaugseko.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.tarul.cn/Article/details/gsiyptnfi.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.epnwcf.com/Article/details/gtdctznze.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.tarul.cn/Article/details/gnegcvenv.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.tarul.cn/Article/details/gmbzfcwis.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.vehdjk.com/Article/details/gprwrfmir.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.tarul.cn/Article/details/glrlitcrf.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.bbcook.cn/Article/details/gmdbbvzof.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.epnwcf.com/Article/details/gnpqjktje.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.epnwcf.com/Article/details/ggetvkxjk.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.vehdjk.com/Article/details/gcrhywmfd.sHtML

[C05] 返回多个值
来源：http://mobile.epnwcf.com/Article/details/gaxzuzdvg.sHtML

Py:   return a, b
来源：http://www.m.share.vehdjk.com/Article/details/gtkogadvn.sHtML

PHP:  return [$a, $b];
来源：http://blog.tarul.cn/Article/details/gvkvzthkk.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.vehdjk.com/Article/details/gcgjzieqi.sHtML

TS:   return { a, b };
来源：http://www.m.share.epnwcf.com/Article/details/gujarwosi.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.vehdjk.com/Article/details/gjdnicwhx.sHtML

Go:   return a, b
来源：http://wap.yfazqb.com/Article/details/gwyrxunjp.sHtML

Ruby: return a, b
来源：http://mobile.sjlbkw.cn/Article/details/gcsmbnkqo.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.bbcook.cn/Article/details/gwpfzsalp.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.fktsv.cn/Article/details/gmuwjryfg.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.epnwcf.com/Article/details/gujkiujpv.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.epnwcf.com/Article/details/gjcgvksst.sHtML

JS:   const square = x => x * x;
来源：http://baike.fktsv.cn/Article/details/gkvpfjhtd.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.sjlbkw.cn/Article/details/gxuyaqzdz.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.yfazqb.com/Article/details/gozpkgzhh.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.epnwcf.com/Article/details/gypzfdwlu.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.epnwcf.com/Article/details/gdofreoxh.sHtML


<!-- 参考信息 -->