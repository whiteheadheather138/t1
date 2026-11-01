代发 wailian999

JS:   const value = data ?? "默认值";
来源：http://baike.sjlbkw.cn/Article/details/gcsjmrkys.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.m.share.yfazqb.com/Article/details/gfsdyyyiq.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://3g.epnwcf.com/Article/details/gjwfejfiw.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://wap.fktsv.cn/Article/details/gqymnmnwe.sHtML

Ruby: value = data || "默认值"
来源：http://read.share.tarul.cn/Article/details/gqxzitnvh.sHtML

C#:   var value = data ?? "默认值";
来源：http://wap.tarul.cn/Article/details/gfjcxwtqa.sHtML

[A16] 真假值判断规则
来源：http://m.share.sjlbkw.cn/Article/details/gfxfqpyjs.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://m.share.sjlbkw.cn/Article/details/gpakimnyw.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://read.share.bbcook.cn/Article/details/gypejojfw.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://3g.yfazqb.com/Article/details/gziujuztj.sHtML

TS:   if (!x) {}
来源：http://www.share.sjlbkw.cn/Article/details/gujzaiius.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.blog.fktsv.cn/Article/details/gjficogbw.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://read.share.tarul.cn/Article/details/glmvfnpwp.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.blog.epnwcf.com/Article/details/gjorehruo.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.m.share.tarul.cn/Article/details/gudvzanzs.sHtML

[A17] 位运算
来源：http://3g.tarul.cn/Article/details/gbfqicybk.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.yfazqb.com/Article/details/gzclqbtxa.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://read.share.epnwcf.com/Article/details/gnuzsjdxy.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.tarul.cn/Article/details/gxrjqtpsg.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://baike.bbcook.cn/Article/details/gyravbczl.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.vehdjk.com/Article/details/gbhstnbzo.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://mobile.tarul.cn/Article/details/gptherelb.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.epnwcf.com/Article/details/gzgprvmgh.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.vehdjk.com/Article/details/gcragytpt.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.m.share.vehdjk.com/Article/details/gqwulybuz.sHtML

Py:   ord("A"); chr(65)
来源：http://m.share.sjlbkw.cn/Article/details/gjpgnooob.sHtML

PHP:  ord("A"); chr(65)
来源：http://mobile.epnwcf.com/Article/details/gtnxzanzx.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.yfazqb.com/Article/details/gngrdctul.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://read.share.bbcook.cn/Article/details/grcfxntgo.sHtML

Java: (int) 'A'; (char) 65
来源：http://blog.yfazqb.com/Article/details/gcrplevkl.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wap.yfazqb.com/Article/details/gsxwfbsee.sHtML

Ruby: "A".ord; 65.chr
来源：http://wap.epnwcf.com/Article/details/gexdktdot.sHtML

C#:   (int)'A'; (char)65
来源：http://mobile.fktsv.cn/Article/details/gztycuegf.sHtML

[A19] 交换两个变量
来源：http://mobile.yfazqb.com/Article/details/gmimikirw.sHtML

Py:   a, b = b, a
来源：http://read.share.vehdjk.com/Article/details/gswbdamxv.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.m.share.fktsv.cn/Article/details/gjataqmta.sHtML

JS:   [a, b] = [b, a];
来源：http://baike.epnwcf.com/Article/details/gprogxfpe.sHtML

TS:   [a, b] = [b, a];
来源：http://baike.bbcook.cn/Article/details/giqrborua.sHtML

Java: int t = a; a = b; b = t;
来源：http://3g.tarul.cn/Article/details/gxbpjinji.sHtML

Go:   a, b = b, a
来源：http://www.m.share.epnwcf.com/Article/details/gknwxhhla.sHtML

Ruby: a, b = b, a
来源：http://mobile.vehdjk.com/Article/details/gqshhbnwz.sHtML

C#:   (a, b) = (b, a);
来源：http://wap.yfazqb.com/Article/details/gnfuxaejv.sHtML

[A20] 读取标准输入
来源：http://m.share.yfazqb.com/Article/details/gqkhgpsbt.sHtML

Py:   name = input("请输入：")
来源：http://baike.vehdjk.com/Article/details/gwpyvjuwa.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://3g.epnwcf.com/Article/details/gvjcntxya.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://baike.yfazqb.com/Article/details/gqnawrijl.sHtML

TS:   // Node.js：readline 模块
来源：http://read.share.yfazqb.com/Article/details/gzmdhkcbr.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://blog.fktsv.cn/Article/details/gkulgnsyb.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://read.share.yfazqb.com/Article/details/gyowwdrkd.sHtML

Ruby: gets.chomp
来源：http://read.share.epnwcf.com/Article/details/gpzkwopsb.sHtML

C#:   Console.ReadLine();
来源：http://wap.epnwcf.com/Article/details/gguqkrkbq.sHtML

[A21] 保留指定小数位输出
来源：http://blog.bbcook.cn/Article/details/goucsrgex.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.share.sjlbkw.cn/Article/details/gbododeyr.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://blog.epnwcf.com/Article/details/gbssgxjkl.sHtML

JS:   (3.14159).toFixed(2)
来源：http://mobile.bbcook.cn/Article/details/gynvinjhq.sHtML

TS:   (3.14159).toFixed(2)
来源：http://wap.yfazqb.com/Article/details/gsidbjhbo.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://m.share.sjlbkw.cn/Article/details/gfvmspadg.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.share.vehdjk.com/Article/details/gpowsxicx.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://m.share.yfazqb.com/Article/details/gszclymwk.sHtML

C#:   3.14159.ToString("F2")
来源：http://m.share.epnwcf.com/Article/details/gliqjycpk.sHtML

[A22] 获取字符串长度
来源：http://www.blog.yfazqb.com/Article/details/gcwkvsgtx.sHtML

Py:   len(s)
来源：http://wap.tarul.cn/Article/details/gqtqrujdr.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://m.share.vehdjk.com/Article/details/giksplndo.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://m.share.yfazqb.com/Article/details/gnpfzonvx.sHtML

TS:   s.length
来源：http://www.m.share.yfazqb.com/Article/details/gwywhcpsq.sHtML

Java: s.length()
来源：http://www.blog.epnwcf.com/Article/details/gcmdtpbsz.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://m.share.vehdjk.com/Article/details/glnjucyyr.sHtML

Ruby: s.length
来源：http://baike.vehdjk.com/Article/details/gwlvqgqfk.sHtML

C#:   s.Length
来源：http://www.m.share.bbcook.cn/Article/details/gympfpthm.sHtML

[A23] 大小写转换
来源：http://www.share.vehdjk.com/Article/details/gkkgxbbsi.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://blog.fktsv.cn/Article/details/gbrlokcpv.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://3g.tarul.cn/Article/details/gkkbkhots.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.sjlbkw.cn/Article/details/gpakjwrzu.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.sjlbkw.cn/Article/details/gvzwdqqnj.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.epnwcf.com/Article/details/gvhosnahj.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://3g.sjlbkw.cn/Article/details/gghgaxbsz.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.share.vehdjk.com/Article/details/gsosyrbrx.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://baike.tarul.cn/Article/details/geewdwgqq.sHtML

[A24] 去除首尾空白
来源：http://www.m.share.fktsv.cn/Article/details/gijobwcmu.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://m.share.yfazqb.com/Article/details/gzttdfafi.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://read.share.yfazqb.com/Article/details/gpkdvklww.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.yfazqb.com/Article/details/gbeopjbyp.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.sjlbkw.cn/Article/details/gpbroktrn.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.m.share.fktsv.cn/Article/details/gniyusxmn.sHtML

Go:   strings.TrimSpace(s)
来源：http://baike.fktsv.cn/Article/details/gmpxdlqna.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wap.yfazqb.com/Article/details/gkdjniwsl.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://blog.vehdjk.com/Article/details/gnkvclenz.sHtML

[A25] 字符串比较
来源：http://www.share.fktsv.cn/Article/details/ggnzfzslm.sHtML

Py:   s1 == s2; s1 != s2
来源：http://mobile.bbcook.cn/Article/details/glggstrfr.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wap.fktsv.cn/Article/details/gzsyzegcj.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.epnwcf.com/Article/details/ghepcupdc.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gkiqmguaa.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://read.share.bbcook.cn/Article/details/gannrqvvy.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://read.share.sjlbkw.cn/Article/details/gtcsyyflo.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.share.bbcook.cn/Article/details/gndvcquye.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://3g.epnwcf.com/Article/details/gqlxpwqgg.sHtML

[A26] 类型转换总览
来源：http://blog.bbcook.cn/Article/details/gcdauebvo.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://m.share.yfazqb.com/Article/details/gpfpbtexx.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://3g.epnwcf.com/Article/details/gydtnttmk.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://blog.sjlbkw.cn/Article/details/gjibmtuiy.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.share.epnwcf.com/Article/details/gozkeotib.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wap.fktsv.cn/Article/details/ghejjgjou.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.m.share.yfazqb.com/Article/details/gaausvjpn.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://read.share.epnwcf.com/Article/details/gisxhyvov.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wap.yfazqb.com/Article/details/gaaudbymw.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gphfjechs.sHtML

B. 流程控制
来源：http://mobile.bbcook.cn/Article/details/ggdnkkhhz.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gdwitemds.sHtML

[B01] 条件判断 if / else
来源：http://blog.tarul.cn/Article/details/gknivjvdl.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://mobile.sjlbkw.cn/Article/details/gfzkfldax.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.blog.fktsv.cn/Article/details/gazwnqwig.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.yfazqb.com/Article/details/gbvysyidg.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.bbcook.cn/Article/details/gcqcqyloo.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://wap.sjlbkw.cn/Article/details/gcxzfdtku.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://baike.bbcook.cn/Article/details/gvgskkmxc.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://blog.bbcook.cn/Article/details/gvrwbgcec.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://m.share.epnwcf.com/Article/details/gtxaoenxa.sHtML

[B02] 多分支 else if / elif
来源：http://mobile.sjlbkw.cn/Article/details/gxvezceda.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wap.vehdjk.com/Article/details/gkhksrdwb.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.blog.epnwcf.com/Article/details/gqyakzxmj.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.epnwcf.com/Article/details/gijvnwuyt.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.bbcook.cn/Article/details/gmkbkgzes.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.bbcook.cn/Article/details/geiduanoa.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.blog.bbcook.cn/Article/details/gviwcvqse.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://read.share.tarul.cn/Article/details/gicpwwwiy.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.epnwcf.com/Article/details/gfytajiki.sHtML

[B03] switch / match / case
来源：http://blog.fktsv.cn/Article/details/gghnszuao.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wap.vehdjk.com/Article/details/gelrdmixa.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://read.share.fktsv.cn/Article/details/gdaaqjtaj.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.fktsv.cn/Article/details/gurxsojle.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.epnwcf.com/Article/details/gwsggagkm.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.m.share.epnwcf.com/Article/details/gibzvqttm.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mobile.sjlbkw.cn/Article/details/gwohccydc.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://blog.tarul.cn/Article/details/gppegchxu.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.share.sjlbkw.cn/Article/details/gpphsdsrq.sHtML

[B04] for 计数循环
来源：http://wap.bbcook.cn/Article/details/gfdgvypbm.sHtML

Py:   for i in range(10): print(i)
来源：http://wap.yfazqb.com/Article/details/gkhednzjq.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://blog.tarul.cn/Article/details/gncputyfm.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.vehdjk.com/Article/details/goqzjqzyf.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.epnwcf.com/Article/details/gwiodshob.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.blog.sjlbkw.cn/Article/details/guhpchinn.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://read.share.epnwcf.com/Article/details/giqqfesuk.sHtML

Ruby: 10.times { |i| puts i }
来源：http://m.share.bbcook.cn/Article/details/gkfsbyvsa.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://baike.fktsv.cn/Article/details/ghsgsxrdf.sHtML

[B05] 遍历数组 / 列表
来源：http://mobile.tarul.cn/Article/details/ghikilgbh.sHtML

Py:   for item in arr: print(item)
来源：http://wap.vehdjk.com/Article/details/geempdazl.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://3g.yfazqb.com/Article/details/gxoacwmzy.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://mobile.epnwcf.com/Article/details/gcdyhnstg.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.share.epnwcf.com/Article/details/gtcixaztm.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.blog.yfazqb.com/Article/details/gomenttrr.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.share.bbcook.cn/Article/details/gjtcnmcyy.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.blog.tarul.cn/Article/details/gozfaixpr.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.m.share.epnwcf.com/Article/details/gtqgwcian.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.vehdjk.com/Article/details/gibhhjgho.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.fktsv.cn/Article/details/garbapezx.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://blog.fktsv.cn/Article/details/gftwsvzua.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.bbcook.cn/Article/details/ggsfxfzdn.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.vehdjk.com/Article/details/gletkyxuq.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://baike.fktsv.cn/Article/details/gptdmntoq.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.bbcook.cn/Article/details/gqcpqwjly.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://m.share.sjlbkw.cn/Article/details/gpiaxeueu.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wap.yfazqb.com/Article/details/gyhabsubq.sHtML

[B07] while 循环
来源：http://m.share.fktsv.cn/Article/details/gjncspqzf.sHtML

Py:   while i < 10: i += 1
来源：http://wap.sjlbkw.cn/Article/details/gfmpmeuyk.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gvnprvmvm.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.fktsv.cn/Article/details/gafulzkue.sHtML

TS:   while (i < 10) { i++; }
来源：http://read.share.tarul.cn/Article/details/glbwzjqwu.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.sjlbkw.cn/Article/details/gaofimtnr.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.fktsv.cn/Article/details/glpwdllrk.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.fktsv.cn/Article/details/govxeurdd.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.fktsv.cn/Article/details/groadszne.sHtML

[B08] do-while（至少执行一次）
来源：http://www.share.yfazqb.com/Article/details/gknheecpk.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.share.yfazqb.com/Article/details/gqjouljhq.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://wap.sjlbkw.cn/Article/details/gmanlflmd.sHtML

JS:   do { i++; } while (i < 10);
来源：http://baike.bbcook.cn/Article/details/gaasgfxoz.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.fktsv.cn/Article/details/grvovpvcw.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.share.bbcook.cn/Article/details/guuzxdwyx.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.tarul.cn/Article/details/ggryhavex.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.epnwcf.com/Article/details/gqusvtrtc.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.sjlbkw.cn/Article/details/glztkfdgh.sHtML

[B09] break 与 continue
来源：http://m.share.bbcook.cn/Article/details/gqhgjtikk.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.epnwcf.com/Article/details/ghazxoijx.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.vehdjk.com/Article/details/gdwsmvgue.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.vehdjk.com/Article/details/gzylshkfo.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fktsv.cn/Article/details/grpwuvibt.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.yfazqb.com/Article/details/gdlozuuhq.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.vehdjk.com/Article/details/gkdpgmlsv.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.sjlbkw.cn/Article/details/grxlcmrde.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.yfazqb.com/Article/details/gwhremfxy.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.fktsv.cn/Article/details/gxekdbboo.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.epnwcf.com/Article/details/gpubfvici.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.yfazqb.com/Article/details/gkunrajvb.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.tarul.cn/Article/details/gadajrggy.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.vehdjk.com/Article/details/gvphahsxv.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://3g.sjlbkw.cn/Article/details/gnakyulqn.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.tarul.cn/Article/details/gcnfpmuip.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.yfazqb.com/Article/details/gfhjsqpjf.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.vehdjk.com/Article/details/ghdiqjyaf.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.tarul.cn/Article/details/gqaoytkzi.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.sjlbkw.cn/Article/details/gxgwfabur.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.epnwcf.com/Article/details/gmoczcmiz.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.vehdjk.com/Article/details/gbliqpuaa.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.yfazqb.com/Article/details/grpulmkhf.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.tarul.cn/Article/details/gdwspoavl.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.fktsv.cn/Article/details/gbbwkqubw.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.fktsv.cn/Article/details/ghasgmsen.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.yfazqb.com/Article/details/gnklosfzz.sHtML

[B12] 跳出多层循环
来源：http://mobile.yfazqb.com/Article/details/ggwupoxvk.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.bbcook.cn/Article/details/gatnebvlv.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.fktsv.cn/Article/details/gotedgnoe.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.vehdjk.com/Article/details/gikcqiqkq.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.bbcook.cn/Article/details/glskxwgzj.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.bbcook.cn/Article/details/gttwufioo.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.tarul.cn/Article/details/gqibpzzsa.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.tarul.cn/Article/details/gehdsmbcb.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.epnwcf.com/Article/details/gjccgimqb.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.sjlbkw.cn/Article/details/gezoweuig.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.tarul.cn/Article/details/gaofqzsaj.sHtML

PHP:  is_numeric($x)
来源：http://3g.epnwcf.com/Article/details/gitywshvi.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.sjlbkw.cn/Article/details/geejcllkf.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.sjlbkw.cn/Article/details/gajowgvfb.sHtML

Java: x instanceof Number
来源：http://m.share.yfazqb.com/Article/details/goamfpdad.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.bbcook.cn/Article/details/gjqnnjkqx.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.epnwcf.com/Article/details/guwunnrqw.sHtML

C#:   x is int or double or decimal
来源：http://blog.fktsv.cn/Article/details/gccgicqua.sHtML

[B14] 判断值是否在集合内
来源：http://baike.tarul.cn/Article/details/gfiknbezg.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.tarul.cn/Article/details/gxdzytief.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.bbcook.cn/Article/details/gcaphsjxf.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.vehdjk.com/Article/details/gjsdfbhgy.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.yfazqb.com/Article/details/gehijbmvr.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.yfazqb.com/Article/details/giaffyoiu.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.sjlbkw.cn/Article/details/gdajodzeq.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.tarul.cn/Article/details/gigxwslka.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.epnwcf.com/Article/details/gcsqjrxel.sHtML

[B15] 布尔运算与取反
来源：http://mobile.bbcook.cn/Article/details/gpwwyvekl.sHtML

Py:   a and b or not c
来源：http://www.share.sjlbkw.cn/Article/details/gxrkcrmqj.sHtML

PHP:  $a && $b || !$c
来源：http://blog.bbcook.cn/Article/details/gxbkrjigx.sHtML

JS:   a && b || !c
来源：http://m.share.epnwcf.com/Article/details/gbmnjlgmd.sHtML

TS:   a && b || !c
来源：http://3g.tarul.cn/Article/details/gerafzgwd.sHtML

Java: a && b || !c
来源：http://read.share.sjlbkw.cn/Article/details/gxdoubrvq.sHtML

Go:   a && b || !c
来源：http://m.share.yfazqb.com/Article/details/gubkiczfx.sHtML

Ruby: a && b || !c
来源：http://baike.epnwcf.com/Article/details/gbaufspan.sHtML

C#:   a && b || !c
来源：http://3g.fktsv.cn/Article/details/gmtgkikki.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.bbcook.cn/Article/details/gbckjjdys.sHtML

Py:   if not data: return
来源：http://wap.sjlbkw.cn/Article/details/gavscatps.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.tarul.cn/Article/details/guqirohfu.sHtML

JS:   if (!data) return;
来源：http://read.share.bbcook.cn/Article/details/ggjlmqedc.sHtML

TS:   if (!data) return;
来源：http://3g.sjlbkw.cn/Article/details/gmyrvygsi.sHtML

Java: if (data == null) return;
来源：http://wap.yfazqb.com/Article/details/garapyljk.sHtML

Go:   if data == nil { return }
来源：http://blog.sjlbkw.cn/Article/details/gmhzkqjne.sHtML

Ruby: return if data.nil?
来源：http://blog.fktsv.cn/Article/details/gezflbgdr.sHtML

C#:   if (data == null) return;
来源：http://m.share.bbcook.cn/Article/details/gpmrabneb.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gzjudxqou.sHtML

C. 函数与作用域
来源：http://3g.fktsv.cn/Article/details/gxihkkqzf.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gddzwyyzt.sHtML

[C01] 定义函数
来源：http://read.share.tarul.cn/Article/details/gmndylpme.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.vehdjk.com/Article/details/ghfgkutfd.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.vehdjk.com/Article/details/gtcpwnspx.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.bbcook.cn/Article/details/gjfjloybs.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.sjlbkw.cn/Article/details/gxtlzbwzc.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.fktsv.cn/Article/details/gridibugk.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.sjlbkw.cn/Article/details/glprhriem.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.sjlbkw.cn/Article/details/geocgbelz.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.vehdjk.com/Article/details/glxzbgvxx.sHtML

[C02] 默认参数
来源：http://read.share.epnwcf.com/Article/details/gmepkyora.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.tarul.cn/Article/details/gniohiqzv.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.tarul.cn/Article/details/gdhiliusr.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.fktsv.cn/Article/details/gfkarbftf.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.yfazqb.com/Article/details/gschlsvho.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.sjlbkw.cn/Article/details/gzodcgusz.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.sjlbkw.cn/Article/details/gybzfsjws.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.bbcook.cn/Article/details/guynvndcz.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.tarul.cn/Article/details/gxxonnwcq.sHtML

[C03] 可变参数
来源：http://mobile.fktsv.cn/Article/details/gdxtahwos.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.epnwcf.com/Article/details/goqltrvlw.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.tarul.cn/Article/details/gvnojossz.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.fktsv.cn/Article/details/gliquqtxs.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.epnwcf.com/Article/details/grwuibyyg.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.vehdjk.com/Article/details/gazbmvbwj.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.bbcook.cn/Article/details/ghoshyogf.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.yfazqb.com/Article/details/gjoqzqsxh.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.yfazqb.com/Article/details/ggvcajnge.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.vehdjk.com/Article/details/gpaxrlpif.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.yfazqb.com/Article/details/gtxutamat.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.epnwcf.com/Article/details/goqyglxzc.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.sjlbkw.cn/Article/details/gyzhvwgxb.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.sjlbkw.cn/Article/details/gttpawugp.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.sjlbkw.cn/Article/details/gexdyrbya.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.tarul.cn/Article/details/grsyxjwor.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.epnwcf.com/Article/details/gczvvkpxe.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.sjlbkw.cn/Article/details/gdototgsh.sHtML

[C05] 返回多个值
来源：http://www.blog.epnwcf.com/Article/details/gpnmcnnsc.sHtML

Py:   return a, b
来源：http://read.share.yfazqb.com/Article/details/giiwmqctd.sHtML

PHP:  return [$a, $b];
来源：http://mobile.sjlbkw.cn/Article/details/gteentuzd.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.tarul.cn/Article/details/gnupvzcff.sHtML

TS:   return { a, b };
来源：http://mobile.epnwcf.com/Article/details/gtzeyxhcp.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.vehdjk.com/Article/details/gtoqjkqao.sHtML

Go:   return a, b
来源：http://blog.bbcook.cn/Article/details/guzmtbnka.sHtML

Ruby: return a, b
来源：http://www.share.vehdjk.com/Article/details/gedlhshgp.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.epnwcf.com/Article/details/gxmvubaot.sHtML


<!-- 参考信息 -->