代发 wailian999

Ruby: value = data || "默认值"
来源：http://www.m.share.yfazqb.com/Article/details/gknznmjlz.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.blog.bbcook.cn/Article/details/grfhdommb.sHtML

[A16] 真假值判断规则
来源：http://blog.bbcook.cn/Article/details/gvjncifpm.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mobile.fktsv.cn/Article/details/gjvkzyibz.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://read.share.yfazqb.com/Article/details/gzpobgknx.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.blog.yfazqb.com/Article/details/gchhvwzrw.sHtML

TS:   if (!x) {}
来源：http://read.share.vehdjk.com/Article/details/gxsdxuquy.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.m.share.fktsv.cn/Article/details/gyjvbttwg.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://mobile.sjlbkw.cn/Article/details/gpchoynrp.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://3g.fktsv.cn/Article/details/gtlsnqwbt.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://read.share.yfazqb.com/Article/details/gsxvflgjo.sHtML

[A17] 位运算
来源：http://wap.epnwcf.com/Article/details/glzyvubwk.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.bbcook.cn/Article/details/gkazxqdzc.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.m.share.sjlbkw.cn/Article/details/gukurtyur.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.tarul.cn/Article/details/gyoyovqjs.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wap.vehdjk.com/Article/details/ghcgpylzw.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.bbcook.cn/Article/details/gocovdlrb.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.share.fktsv.cn/Article/details/grkazaigj.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.fktsv.cn/Article/details/ggmgmeoxf.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.sjlbkw.cn/Article/details/ghpgzcdqg.sHtML

[A18] 字符与 ASCII 码互转
来源：http://mobile.tarul.cn/Article/details/gfqspdugz.sHtML

Py:   ord("A"); chr(65)
来源：http://www.m.share.epnwcf.com/Article/details/gplkvinsu.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.blog.tarul.cn/Article/details/gwiipttjg.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.vehdjk.com/Article/details/gnmxkmjhh.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.bbcook.cn/Article/details/gfccfpacu.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.m.share.sjlbkw.cn/Article/details/gkoviqbpq.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://m.share.bbcook.cn/Article/details/gvlfberla.sHtML

Ruby: "A".ord; 65.chr
来源：http://m.share.vehdjk.com/Article/details/gcnwshwbd.sHtML

C#:   (int)'A'; (char)65
来源：http://read.share.epnwcf.com/Article/details/gxqpoeiyc.sHtML

[A19] 交换两个变量
来源：http://www.share.tarul.cn/Article/details/grfvrkvxq.sHtML

Py:   a, b = b, a
来源：http://blog.yfazqb.com/Article/details/gkqmvfqkl.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.blog.epnwcf.com/Article/details/gjqnpcvhv.sHtML

JS:   [a, b] = [b, a];
来源：http://wap.yfazqb.com/Article/details/grwrmwwwl.sHtML

TS:   [a, b] = [b, a];
来源：http://m.share.yfazqb.com/Article/details/gmvzqfdhr.sHtML

Java: int t = a; a = b; b = t;
来源：http://wap.epnwcf.com/Article/details/gnkvpjeup.sHtML

Go:   a, b = b, a
来源：http://3g.vehdjk.com/Article/details/gqfbwrbze.sHtML

Ruby: a, b = b, a
来源：http://wap.fktsv.cn/Article/details/gtakydmkl.sHtML

C#:   (a, b) = (b, a);
来源：http://m.share.bbcook.cn/Article/details/gzsopipvt.sHtML

[A20] 读取标准输入
来源：http://read.share.fktsv.cn/Article/details/gkgtbwriv.sHtML

Py:   name = input("请输入：")
来源：http://read.share.yfazqb.com/Article/details/gytlhzqyu.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.share.vehdjk.com/Article/details/gxjblomos.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://mobile.tarul.cn/Article/details/gccimzrgh.sHtML

TS:   // Node.js：readline 模块
来源：http://www.share.fktsv.cn/Article/details/grszyykyk.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://3g.tarul.cn/Article/details/gynllclcv.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wap.bbcook.cn/Article/details/gcyltpzpt.sHtML

Ruby: gets.chomp
来源：http://3g.tarul.cn/Article/details/gwpqiamsh.sHtML

C#:   Console.ReadLine();
来源：http://3g.fktsv.cn/Article/details/gtvrdbsle.sHtML

[A21] 保留指定小数位输出
来源：http://www.m.share.vehdjk.com/Article/details/gpayzbmdv.sHtML

Py:   f"{3.14159:.2f}"
来源：http://mobile.tarul.cn/Article/details/gbetgfgyd.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.share.yfazqb.com/Article/details/gmvgruers.sHtML

JS:   (3.14159).toFixed(2)
来源：http://mobile.epnwcf.com/Article/details/genodhjgx.sHtML

TS:   (3.14159).toFixed(2)
来源：http://3g.yfazqb.com/Article/details/gqoqqejbc.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.share.bbcook.cn/Article/details/gdwwoootc.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.m.share.bbcook.cn/Article/details/gjguaktkg.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.share.bbcook.cn/Article/details/gfrsveadn.sHtML

C#:   3.14159.ToString("F2")
来源：http://baike.sjlbkw.cn/Article/details/ghbwqgkku.sHtML

[A22] 获取字符串长度
来源：http://read.share.vehdjk.com/Article/details/gtimptlxb.sHtML

Py:   len(s)
来源：http://baike.yfazqb.com/Article/details/gjhqqxbdr.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mobile.tarul.cn/Article/details/gcydgjoja.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wap.tarul.cn/Article/details/gmzlpcutn.sHtML

TS:   s.length
来源：http://baike.tarul.cn/Article/details/gicbzlkeb.sHtML

Java: s.length()
来源：http://www.share.bbcook.cn/Article/details/gcsuabyhd.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.m.share.yfazqb.com/Article/details/gazettitd.sHtML

Ruby: s.length
来源：http://read.share.yfazqb.com/Article/details/gboyfzokp.sHtML

C#:   s.Length
来源：http://www.blog.tarul.cn/Article/details/gnlpjnwoj.sHtML

[A23] 大小写转换
来源：http://read.share.epnwcf.com/Article/details/gqjjmhdqo.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://blog.yfazqb.com/Article/details/gqdkjplww.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://3g.yfazqb.com/Article/details/ghvclygpc.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.sjlbkw.cn/Article/details/gulmggmfj.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.epnwcf.com/Article/details/gzxazkugu.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://baike.vehdjk.com/Article/details/gqntctwwy.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.m.share.bbcook.cn/Article/details/gmlwamlir.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wap.fktsv.cn/Article/details/gfckmtvgf.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.m.share.fktsv.cn/Article/details/gbyurdlev.sHtML

[A24] 去除首尾空白
来源：http://read.share.tarul.cn/Article/details/gatewjowm.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://blog.fktsv.cn/Article/details/grmborzel.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.share.tarul.cn/Article/details/gprneifmr.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.tarul.cn/Article/details/gyxkojluo.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.fktsv.cn/Article/details/ghbhjigaa.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.m.share.bbcook.cn/Article/details/gzavphqom.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.m.share.bbcook.cn/Article/details/gvnnsohhe.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://read.share.sjlbkw.cn/Article/details/gvizgvjvk.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://blog.vehdjk.com/Article/details/gstwvfezj.sHtML

[A25] 字符串比较
来源：http://blog.yfazqb.com/Article/details/ghhoxzifv.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.share.yfazqb.com/Article/details/gfhlfhhfr.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://3g.epnwcf.com/Article/details/gkrnmuzss.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.fktsv.cn/Article/details/gqrlgihxv.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.epnwcf.com/Article/details/gdoqqdzgr.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mobile.yfazqb.com/Article/details/gorzdsrcg.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://baike.fktsv.cn/Article/details/goqpadvfv.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://wap.tarul.cn/Article/details/gblwbhift.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://3g.yfazqb.com/Article/details/gsoswoohe.sHtML

[A26] 类型转换总览
来源：http://mobile.sjlbkw.cn/Article/details/gvsienhcc.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://blog.bbcook.cn/Article/details/gnelekouc.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.blog.epnwcf.com/Article/details/gnqzgregb.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.share.yfazqb.com/Article/details/gzdtkwzyd.sHtML

TS:   Number() String() Boolean() x as number
来源：http://read.share.yfazqb.com/Article/details/gaeeaqdlx.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://read.share.tarul.cn/Article/details/gopjagvze.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://read.share.sjlbkw.cn/Article/details/gxmprmuoz.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://m.share.vehdjk.com/Article/details/gmxybsdru.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.m.share.yfazqb.com/Article/details/goizyxune.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gxfpqebiw.sHtML

B. 流程控制
来源：http://www.blog.tarul.cn/Article/details/ghupvycif.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gesolxjns.sHtML

[B01] 条件判断 if / else
来源：http://blog.tarul.cn/Article/details/grqulavrk.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://3g.sjlbkw.cn/Article/details/gxhivmxan.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.blog.epnwcf.com/Article/details/gugavpgtg.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.sjlbkw.cn/Article/details/gnyuozowj.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.tarul.cn/Article/details/gflplthyj.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://blog.vehdjk.com/Article/details/gwygefnbv.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://blog.fktsv.cn/Article/details/ggebhgvun.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.share.vehdjk.com/Article/details/grpuiuvtq.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mobile.vehdjk.com/Article/details/gmuhxcpdt.sHtML

[B02] 多分支 else if / elif
来源：http://www.share.vehdjk.com/Article/details/gkxcmofsk.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://blog.tarul.cn/Article/details/gjvxfekcb.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://read.share.sjlbkw.cn/Article/details/gqflvlcii.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.sjlbkw.cn/Article/details/giosghhyk.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.vehdjk.com/Article/details/gdgbdiaww.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.tarul.cn/Article/details/gyqvndibf.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mobile.bbcook.cn/Article/details/gymicohko.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://blog.yfazqb.com/Article/details/gqalibybg.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.yfazqb.com/Article/details/grjwxgevv.sHtML

[B03] switch / match / case
来源：http://www.m.share.yfazqb.com/Article/details/gerhbcqif.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://m.share.vehdjk.com/Article/details/gnpeytpby.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.blog.yfazqb.com/Article/details/ggazsxyzr.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.yfazqb.com/Article/details/gpalwhxgn.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.sjlbkw.cn/Article/details/gumocnenz.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.blog.tarul.cn/Article/details/gjzihhcen.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mobile.sjlbkw.cn/Article/details/ggabmzkic.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://m.share.sjlbkw.cn/Article/details/gwpvoudgi.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wap.epnwcf.com/Article/details/gcpdzvgtq.sHtML

[B04] for 计数循环
来源：http://3g.epnwcf.com/Article/details/gmdkcebgz.sHtML

Py:   for i in range(10): print(i)
来源：http://www.share.fktsv.cn/Article/details/gqdhqhuwl.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://blog.yfazqb.com/Article/details/gfkggeljs.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.bbcook.cn/Article/details/gutgedwhy.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.sjlbkw.cn/Article/details/gtvkgzgjw.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.m.share.epnwcf.com/Article/details/ggpcynpnn.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.share.vehdjk.com/Article/details/gnwayxdoi.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.share.tarul.cn/Article/details/gfojgtkfu.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://3g.epnwcf.com/Article/details/gaurihkld.sHtML

[B05] 遍历数组 / 列表
来源：http://mobile.sjlbkw.cn/Article/details/gcuscihnz.sHtML

Py:   for item in arr: print(item)
来源：http://3g.vehdjk.com/Article/details/gozvywyxz.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.m.share.epnwcf.com/Article/details/gcksitynu.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://read.share.yfazqb.com/Article/details/gclqrdruz.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.share.epnwcf.com/Article/details/gnsolseky.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.bbcook.cn/Article/details/genvaaiwu.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mobile.sjlbkw.cn/Article/details/gessagtgj.sHtML

Ruby: arr.each { |item| puts item }
来源：http://baike.fktsv.cn/Article/details/gvieooaxv.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://m.share.bbcook.cn/Article/details/goomwnmjt.sHtML

[B06] 遍历字典 / 对象
来源：http://www.m.share.bbcook.cn/Article/details/gzcubjfuk.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.vehdjk.com/Article/details/gtlymbzfl.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://blog.vehdjk.com/Article/details/ghfckhyfo.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.tarul.cn/Article/details/gztorssvj.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.vehdjk.com/Article/details/gskczbsbk.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.tarul.cn/Article/details/glqbqgphv.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.vehdjk.com/Article/details/grnsjctvz.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.sjlbkw.cn/Article/details/glhnccsvz.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mobile.bbcook.cn/Article/details/glqqtmmoq.sHtML

[B07] while 循环
来源：http://blog.epnwcf.com/Article/details/gtqpomgja.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.vehdjk.com/Article/details/gpwycwhaa.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.bbcook.cn/Article/details/gezvrtjfd.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.yfazqb.com/Article/details/gwcozwucu.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.tarul.cn/Article/details/gxloassto.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.vehdjk.com/Article/details/gpuhetqro.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wap.bbcook.cn/Article/details/gcadigjgv.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.bbcook.cn/Article/details/gasrqirpc.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.epnwcf.com/Article/details/ggelxwahw.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.yfazqb.com/Article/details/goqiruwdm.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.sjlbkw.cn/Article/details/gbvzqudsn.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.bbcook.cn/Article/details/gjhkkqdxc.sHtML

JS:   do { i++; } while (i < 10);
来源：http://m.share.bbcook.cn/Article/details/gpqxpgyeb.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.sjlbkw.cn/Article/details/gpeezlyds.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.tarul.cn/Article/details/gpqenmcdr.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.vehdjk.com/Article/details/gofurunsf.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.bbcook.cn/Article/details/gniznyqqf.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.tarul.cn/Article/details/gnaobdoje.sHtML

[B09] break 与 continue
来源：http://wap.sjlbkw.cn/Article/details/gwwkolanb.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.tarul.cn/Article/details/gbkokemnp.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.bbcook.cn/Article/details/getttokqk.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.sjlbkw.cn/Article/details/gznyxdybe.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.sjlbkw.cn/Article/details/gcbgfsles.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fktsv.cn/Article/details/gobhnutax.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.fktsv.cn/Article/details/gpafjizud.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.fktsv.cn/Article/details/ggucljoxb.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fktsv.cn/Article/details/gsfjhxcyw.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.epnwcf.com/Article/details/gejbtalnw.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.bbcook.cn/Article/details/gptrdeepb.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.sjlbkw.cn/Article/details/girvdukmy.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.vehdjk.com/Article/details/gdkinvrkb.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.bbcook.cn/Article/details/gxayhkwpq.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.vehdjk.com/Article/details/gvcejkpqk.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.tarul.cn/Article/details/ggzzgvjrl.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.yfazqb.com/Article/details/gkbuzgazp.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.bbcook.cn/Article/details/gwcgsgkdz.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.tarul.cn/Article/details/gokdhskbo.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.vehdjk.com/Article/details/gilkjklsv.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.yfazqb.com/Article/details/grzlnlzwp.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.tarul.cn/Article/details/gahlmvvld.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.yfazqb.com/Article/details/gxtaebfvw.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.yfazqb.com/Article/details/gkmcbfmia.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.sjlbkw.cn/Article/details/gxaajphyc.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.yfazqb.com/Article/details/gyfahewhu.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.yfazqb.com/Article/details/glarksdgx.sHtML

[B12] 跳出多层循环
来源：http://read.share.vehdjk.com/Article/details/gmydalknw.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.epnwcf.com/Article/details/golfvswir.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.yfazqb.com/Article/details/gyieczlaq.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.bbcook.cn/Article/details/godcbgfre.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.epnwcf.com/Article/details/gwyjwfjuq.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.tarul.cn/Article/details/gjstwpudr.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.yfazqb.com/Article/details/gxocmgsve.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.epnwcf.com/Article/details/gkmpekbhf.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.bbcook.cn/Article/details/ggmmehgfc.sHtML

[B13] 判断是否为数字
来源：http://blog.epnwcf.com/Article/details/gakfhievg.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.tarul.cn/Article/details/gdbbhgvfh.sHtML

PHP:  is_numeric($x)
来源：http://3g.sjlbkw.cn/Article/details/gfalphhai.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.yfazqb.com/Article/details/gjtxrdfoi.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.vehdjk.com/Article/details/gurdfjvfi.sHtML

Java: x instanceof Number
来源：http://www.m.share.epnwcf.com/Article/details/gscovtwxf.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.tarul.cn/Article/details/gvjbaoqyl.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.tarul.cn/Article/details/ggfjtxxwr.sHtML

C#:   x is int or double or decimal
来源：http://baike.tarul.cn/Article/details/gxfpyllkv.sHtML

[B14] 判断值是否在集合内
来源：http://baike.epnwcf.com/Article/details/giplovfnu.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.fktsv.cn/Article/details/gpbgelcvf.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.sjlbkw.cn/Article/details/gvnooeagl.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.vehdjk.com/Article/details/gsgdpwwzo.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.vehdjk.com/Article/details/gulvnsnzi.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.sjlbkw.cn/Article/details/gahokadmm.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.fktsv.cn/Article/details/gmsikeuuc.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.tarul.cn/Article/details/ghodaelhf.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.fktsv.cn/Article/details/gqqwyviaz.sHtML

[B15] 布尔运算与取反
来源：http://wap.sjlbkw.cn/Article/details/gydgeazrs.sHtML

Py:   a and b or not c
来源：http://wap.bbcook.cn/Article/details/ggpzeuxte.sHtML

PHP:  $a && $b || !$c
来源：http://wap.fktsv.cn/Article/details/gxmwtufzu.sHtML

JS:   a && b || !c
来源：http://3g.vehdjk.com/Article/details/gdevrcevk.sHtML

TS:   a && b || !c
来源：http://wap.vehdjk.com/Article/details/gsgbwdwmh.sHtML

Java: a && b || !c
来源：http://mobile.vehdjk.com/Article/details/gawwqzsdu.sHtML

Go:   a && b || !c
来源：http://baike.vehdjk.com/Article/details/gqvddefwq.sHtML

Ruby: a && b || !c
来源：http://wap.bbcook.cn/Article/details/gwlgxvcuc.sHtML

C#:   a && b || !c
来源：http://m.share.tarul.cn/Article/details/gylfwqtck.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.epnwcf.com/Article/details/gbidrqsai.sHtML

Py:   if not data: return
来源：http://www.m.share.tarul.cn/Article/details/gacimhfeo.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.vehdjk.com/Article/details/gcjoshnjq.sHtML

JS:   if (!data) return;
来源：http://www.m.share.epnwcf.com/Article/details/gzqbtmdap.sHtML

TS:   if (!data) return;
来源：http://read.share.bbcook.cn/Article/details/ghqejdzpo.sHtML

Java: if (data == null) return;
来源：http://www.share.fktsv.cn/Article/details/gsfemndid.sHtML

Go:   if data == nil { return }
来源：http://mobile.epnwcf.com/Article/details/gtnxkyfvx.sHtML

Ruby: return if data.nil?
来源：http://m.share.bbcook.cn/Article/details/gtfcfofoy.sHtML

C#:   if (data == null) return;
来源：http://mobile.yfazqb.com/Article/details/gnwbtyutk.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gigeipqnt.sHtML

C. 函数与作用域
来源：http://www.blog.bbcook.cn/Article/details/glsgulakp.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gobsveyof.sHtML

[C01] 定义函数
来源：http://m.share.sjlbkw.cn/Article/details/gginujrfv.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.bbcook.cn/Article/details/geldvtpuu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.tarul.cn/Article/details/gamtsppjn.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.bbcook.cn/Article/details/ghxifgfik.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.yfazqb.com/Article/details/gsvzosujo.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.epnwcf.com/Article/details/gsaxykrfb.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.vehdjk.com/Article/details/ghcffvdxf.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.vehdjk.com/Article/details/gecibofac.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.yfazqb.com/Article/details/gsjdkcklx.sHtML

[C02] 默认参数
来源：http://www.blog.sjlbkw.cn/Article/details/gfvqxgqel.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.epnwcf.com/Article/details/gaxbeovbc.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.tarul.cn/Article/details/gepscmbir.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.epnwcf.com/Article/details/gfbcmvtpb.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.yfazqb.com/Article/details/gbcwxxdni.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.tarul.cn/Article/details/gpzocthyb.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.yfazqb.com/Article/details/gxmsxkxem.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.epnwcf.com/Article/details/ganqlejph.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.vehdjk.com/Article/details/goickeona.sHtML

[C03] 可变参数
来源：http://baike.epnwcf.com/Article/details/gycipoujw.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.sjlbkw.cn/Article/details/gruqqadxo.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.tarul.cn/Article/details/gzcqkknuo.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.epnwcf.com/Article/details/glsswoypd.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.epnwcf.com/Article/details/gslajairj.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.yfazqb.com/Article/details/gwgcgilzn.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.tarul.cn/Article/details/gsrgxwhdp.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.tarul.cn/Article/details/gxarwuefm.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.bbcook.cn/Article/details/gyymgycdq.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.bbcook.cn/Article/details/gppddxhal.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.fktsv.cn/Article/details/gzaluuxxz.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.sjlbkw.cn/Article/details/gkbkfdowr.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.tarul.cn/Article/details/gtzmtruah.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.bbcook.cn/Article/details/gbdebnjye.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.epnwcf.com/Article/details/gpphtfsor.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.epnwcf.com/Article/details/gspfwaetc.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.bbcook.cn/Article/details/ggfqomslw.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.epnwcf.com/Article/details/gttnjhwor.sHtML

[C05] 返回多个值
来源：http://baike.vehdjk.com/Article/details/ggawpgqbo.sHtML

Py:   return a, b
来源：http://baike.vehdjk.com/Article/details/gbrcyhukm.sHtML

PHP:  return [$a, $b];
来源：http://read.share.fktsv.cn/Article/details/ggowynhct.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.epnwcf.com/Article/details/gxqqegffi.sHtML

TS:   return { a, b };
来源：http://m.share.epnwcf.com/Article/details/gqkpfqkpn.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.sjlbkw.cn/Article/details/gunfbsfgb.sHtML

Go:   return a, b
来源：http://www.blog.sjlbkw.cn/Article/details/gssgsgajm.sHtML

Ruby: return a, b
来源：http://wap.sjlbkw.cn/Article/details/gpuvszldz.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.epnwcf.com/Article/details/gevvbymdf.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.vehdjk.com/Article/details/gikocjxzc.sHtML

Py:   square = lambda x: x * x
来源：http://baike.epnwcf.com/Article/details/gkakoredm.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.epnwcf.com/Article/details/gzvmbtycm.sHtML

JS:   const square = x => x * x;
来源：http://blog.yfazqb.com/Article/details/gagimcxpg.sHtML


<!-- 参考信息 -->