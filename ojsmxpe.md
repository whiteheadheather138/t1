代发 wailian999

JS:   const value = data ?? "默认值";
来源：http://www.m.share.epnwcf.com/Article/details/gckasimsi.sHtML

TS:   const value = data ?? "默认值";
来源：http://baike.tarul.cn/Article/details/ggghdmagz.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://read.share.vehdjk.com/Article/details/glhxyizcs.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.blog.tarul.cn/Article/details/grpudehkl.sHtML

Ruby: value = data || "默认值"
来源：http://3g.epnwcf.com/Article/details/gexnmonpm.sHtML

C#:   var value = data ?? "默认值";
来源：http://wap.vehdjk.com/Article/details/gnnbenacj.sHtML

[A16] 真假值判断规则
来源：http://mobile.vehdjk.com/Article/details/gtndxscqi.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://m.share.epnwcf.com/Article/details/gclnayywt.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://3g.epnwcf.com/Article/details/gadgykzyc.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://m.share.epnwcf.com/Article/details/gnodbtbvo.sHtML

TS:   if (!x) {}
来源：http://mobile.sjlbkw.cn/Article/details/geqdoibmu.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://blog.fktsv.cn/Article/details/gkvpekdps.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.blog.sjlbkw.cn/Article/details/gvekuwmdb.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://wap.epnwcf.com/Article/details/gndnqwsob.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.share.epnwcf.com/Article/details/giqjpdbdb.sHtML

[A17] 位运算
来源：http://3g.bbcook.cn/Article/details/guvdlanxd.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.tarul.cn/Article/details/godbkhlzg.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://read.share.bbcook.cn/Article/details/grxyqlwhg.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.yfazqb.com/Article/details/ghpvxzjgp.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://read.share.tarul.cn/Article/details/gsyopfhcg.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.vehdjk.com/Article/details/gggkmogjx.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://m.share.fktsv.cn/Article/details/gksfaycsw.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.yfazqb.com/Article/details/goagxnxmp.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.yfazqb.com/Article/details/gtofacibr.sHtML

[A18] 字符与 ASCII 码互转
来源：http://m.share.sjlbkw.cn/Article/details/gpwfkqnxc.sHtML

Py:   ord("A"); chr(65)
来源：http://m.share.fktsv.cn/Article/details/gfdefruad.sHtML

PHP:  ord("A"); chr(65)
来源：http://baike.sjlbkw.cn/Article/details/gwjzwowhm.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://read.share.sjlbkw.cn/Article/details/ggnzbszaj.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.sjlbkw.cn/Article/details/gapcpnhdk.sHtML

Java: (int) 'A'; (char) 65
来源：http://baike.sjlbkw.cn/Article/details/gdnqlslta.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://3g.tarul.cn/Article/details/gbnbckikx.sHtML

Ruby: "A".ord; 65.chr
来源：http://baike.fktsv.cn/Article/details/gmovqcwdf.sHtML

C#:   (int)'A'; (char)65
来源：http://blog.vehdjk.com/Article/details/ggmvzifhw.sHtML

[A19] 交换两个变量
来源：http://blog.bbcook.cn/Article/details/gxjwzcfmg.sHtML

Py:   a, b = b, a
来源：http://baike.sjlbkw.cn/Article/details/gwcpflhaj.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://m.share.fktsv.cn/Article/details/gbgqhjchf.sHtML

JS:   [a, b] = [b, a];
来源：http://blog.fktsv.cn/Article/details/gomnpeydu.sHtML

TS:   [a, b] = [b, a];
来源：http://read.share.epnwcf.com/Article/details/gdjeywweg.sHtML

Java: int t = a; a = b; b = t;
来源：http://wap.yfazqb.com/Article/details/gphprqtiw.sHtML

Go:   a, b = b, a
来源：http://3g.yfazqb.com/Article/details/gapqcxxph.sHtML

Ruby: a, b = b, a
来源：http://blog.epnwcf.com/Article/details/gvrvutgyb.sHtML

C#:   (a, b) = (b, a);
来源：http://baike.bbcook.cn/Article/details/ghlavpclg.sHtML

[A20] 读取标准输入
来源：http://mobile.tarul.cn/Article/details/gfdsbyysj.sHtML

Py:   name = input("请输入：")
来源：http://www.blog.fktsv.cn/Article/details/gnaskqicb.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://read.share.vehdjk.com/Article/details/ggnigvvml.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://read.share.fktsv.cn/Article/details/gedqymyda.sHtML

TS:   // Node.js：readline 模块
来源：http://m.share.vehdjk.com/Article/details/gxqwxgncs.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.m.share.yfazqb.com/Article/details/goelexour.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.m.share.epnwcf.com/Article/details/gklzzvrdw.sHtML

Ruby: gets.chomp
来源：http://mobile.bbcook.cn/Article/details/gtnchvbzh.sHtML

C#:   Console.ReadLine();
来源：http://blog.fktsv.cn/Article/details/gcoegasam.sHtML

[A21] 保留指定小数位输出
来源：http://www.blog.yfazqb.com/Article/details/gydxztjeu.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.m.share.vehdjk.com/Article/details/gcldpatoa.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.m.share.sjlbkw.cn/Article/details/gngevebtj.sHtML

JS:   (3.14159).toFixed(2)
来源：http://3g.bbcook.cn/Article/details/gcaxccnok.sHtML

TS:   (3.14159).toFixed(2)
来源：http://baike.bbcook.cn/Article/details/gzmmstrme.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://baike.fktsv.cn/Article/details/gnuilvewj.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://baike.epnwcf.com/Article/details/gkvzkendq.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://read.share.epnwcf.com/Article/details/gnrdxkceq.sHtML

C#:   3.14159.ToString("F2")
来源：http://read.share.bbcook.cn/Article/details/gihvcsjac.sHtML

[A22] 获取字符串长度
来源：http://wap.tarul.cn/Article/details/ggxqxmttp.sHtML

Py:   len(s)
来源：http://blog.fktsv.cn/Article/details/gkrbmlvqr.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://read.share.sjlbkw.cn/Article/details/gjvxglpex.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wap.vehdjk.com/Article/details/grzxjwsmw.sHtML

TS:   s.length
来源：http://wap.tarul.cn/Article/details/glztmugiy.sHtML

Java: s.length()
来源：http://m.share.bbcook.cn/Article/details/gjamljnjn.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://baike.bbcook.cn/Article/details/gywnlhtrw.sHtML

Ruby: s.length
来源：http://wap.tarul.cn/Article/details/gwvkaqocc.sHtML

C#:   s.Length
来源：http://www.share.tarul.cn/Article/details/gpelcwrmv.sHtML

[A23] 大小写转换
来源：http://baike.sjlbkw.cn/Article/details/gkjqpyxft.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://baike.fktsv.cn/Article/details/gmgjezzye.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wap.bbcook.cn/Article/details/grecbxmbv.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.fktsv.cn/Article/details/gchsnpdoa.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.yfazqb.com/Article/details/gffhjwkaq.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wap.sjlbkw.cn/Article/details/gefsjtgdu.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://read.share.tarul.cn/Article/details/gynfkhdkx.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://read.share.epnwcf.com/Article/details/gmrpusvce.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://wap.yfazqb.com/Article/details/gcledrmmd.sHtML

[A24] 去除首尾空白
来源：http://baike.sjlbkw.cn/Article/details/gatwiakrz.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://m.share.vehdjk.com/Article/details/gkjnghzxo.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.blog.sjlbkw.cn/Article/details/gornbwgts.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.vehdjk.com/Article/details/gvnyjkhtz.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.epnwcf.com/Article/details/gapwjtisw.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mobile.epnwcf.com/Article/details/gipglgswp.sHtML

Go:   strings.TrimSpace(s)
来源：http://wap.tarul.cn/Article/details/gbfpqchas.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wap.fktsv.cn/Article/details/gozireqau.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.blog.fktsv.cn/Article/details/gbvvaqtcv.sHtML

[A25] 字符串比较
来源：http://3g.sjlbkw.cn/Article/details/gachgxhbg.sHtML

Py:   s1 == s2; s1 != s2
来源：http://m.share.epnwcf.com/Article/details/gsjrlzboy.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://blog.bbcook.cn/Article/details/ggqqjdqod.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.vehdjk.com/Article/details/gptugfndw.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.fktsv.cn/Article/details/gukwnjvho.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://baike.vehdjk.com/Article/details/gctqndbkv.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wap.yfazqb.com/Article/details/gvehlqkho.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.share.epnwcf.com/Article/details/giytwoyav.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wap.fktsv.cn/Article/details/gracmeigf.sHtML

[A26] 类型转换总览
来源：http://m.share.fktsv.cn/Article/details/geyyteuvm.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.blog.tarul.cn/Article/details/gwlkhcpqd.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://m.share.sjlbkw.cn/Article/details/gtoioybjd.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://baike.sjlbkw.cn/Article/details/gtlbmmblq.sHtML

TS:   Number() String() Boolean() x as number
来源：http://blog.bbcook.cn/Article/details/glqqksjvw.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.blog.vehdjk.com/Article/details/gemvlvtpm.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wap.fktsv.cn/Article/details/gwqmulavi.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.share.tarul.cn/Article/details/ghsrfwqry.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wap.epnwcf.com/Article/details/gorqogvwe.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/giktzlsci.sHtML

B. 流程控制
来源：http://blog.yfazqb.com/Article/details/gphqmgasb.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gcrgeguwv.sHtML

[B01] 条件判断 if / else
来源：http://baike.bbcook.cn/Article/details/gfdkaojjs.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://m.share.tarul.cn/Article/details/govehjenc.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://blog.bbcook.cn/Article/details/glcfgrgjf.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.fktsv.cn/Article/details/gxbperdzy.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.bbcook.cn/Article/details/giidgkdaa.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.share.bbcook.cn/Article/details/ghebjwpiw.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://m.share.fktsv.cn/Article/details/gstoruvbz.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://m.share.vehdjk.com/Article/details/gyxsvxvbt.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://read.share.yfazqb.com/Article/details/gqsrtnigg.sHtML

[B02] 多分支 else if / elif
来源：http://baike.bbcook.cn/Article/details/giywxhhev.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mobile.bbcook.cn/Article/details/goirnsnms.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://baike.bbcook.cn/Article/details/gsvfaxqti.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.vehdjk.com/Article/details/gnqsqigub.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.sjlbkw.cn/Article/details/grpojygkk.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.epnwcf.com/Article/details/ggblqukkt.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wap.yfazqb.com/Article/details/guedfjrko.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://m.share.bbcook.cn/Article/details/gtutjfenw.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.tarul.cn/Article/details/guhadxoee.sHtML

[B03] switch / match / case
来源：http://3g.fktsv.cn/Article/details/guzazvpbi.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.bbcook.cn/Article/details/giypgecit.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://read.share.yfazqb.com/Article/details/gxylixioy.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.epnwcf.com/Article/details/gogtgjvfx.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.yfazqb.com/Article/details/gbhubxcxa.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://blog.yfazqb.com/Article/details/gwlksudtb.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.share.sjlbkw.cn/Article/details/gfbffhxmw.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://read.share.epnwcf.com/Article/details/gfkxlriqg.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://blog.yfazqb.com/Article/details/gxurrpxeq.sHtML

[B04] for 计数循环
来源：http://3g.epnwcf.com/Article/details/golwegeaf.sHtML

Py:   for i in range(10): print(i)
来源：http://www.share.sjlbkw.cn/Article/details/gxecgywyf.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.blog.fktsv.cn/Article/details/gixzrdmea.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.tarul.cn/Article/details/gjargwvtr.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.fktsv.cn/Article/details/gcopfmscc.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.m.share.bbcook.cn/Article/details/gumhisqxs.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.m.share.vehdjk.com/Article/details/gjswbxnxo.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.blog.epnwcf.com/Article/details/gowskyswj.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mobile.yfazqb.com/Article/details/getvyndvq.sHtML

[B05] 遍历数组 / 列表
来源：http://mobile.tarul.cn/Article/details/gphxcxrdd.sHtML

Py:   for item in arr: print(item)
来源：http://m.share.fktsv.cn/Article/details/gqjuklxqh.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://blog.bbcook.cn/Article/details/gkidhhbuy.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://blog.fktsv.cn/Article/details/gtcanhpbs.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://mobile.fktsv.cn/Article/details/gmhtzauhy.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.vehdjk.com/Article/details/gwlzflumv.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wap.yfazqb.com/Article/details/gylxfjcwc.sHtML

Ruby: arr.each { |item| puts item }
来源：http://mobile.fktsv.cn/Article/details/gfmvjlgmu.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://m.share.epnwcf.com/Article/details/gfpbmprvo.sHtML

[B06] 遍历字典 / 对象
来源：http://wap.sjlbkw.cn/Article/details/gsulzzboa.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.epnwcf.com/Article/details/gcppjgmmm.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://blog.sjlbkw.cn/Article/details/gktwrarat.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.yfazqb.com/Article/details/gqykknrkz.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.yfazqb.com/Article/details/gubwgldvj.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.share.vehdjk.com/Article/details/gbwvlznmp.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mobile.vehdjk.com/Article/details/gckilesdd.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.bbcook.cn/Article/details/gkfhtxrsu.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.share.bbcook.cn/Article/details/gelsqcpzb.sHtML

[B07] while 循环
来源：http://read.share.yfazqb.com/Article/details/gniryormm.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.epnwcf.com/Article/details/gncsqueif.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.epnwcf.com/Article/details/gbnssophj.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.epnwcf.com/Article/details/gcmfqxcsl.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.share.fktsv.cn/Article/details/gmchbpgut.sHtML

Java: while (i < 10) { i++; }
来源：http://mobile.yfazqb.com/Article/details/glyetetxj.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.share.vehdjk.com/Article/details/giwyjvfmu.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.tarul.cn/Article/details/griproskc.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.sjlbkw.cn/Article/details/ggoptjesb.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.vehdjk.com/Article/details/gxrloqluc.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://mobile.sjlbkw.cn/Article/details/geraixahn.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.vehdjk.com/Article/details/gsmxsviyx.sHtML

JS:   do { i++; } while (i < 10);
来源：http://baike.vehdjk.com/Article/details/gxtzxaewh.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.m.share.sjlbkw.cn/Article/details/gsaxefplw.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.fktsv.cn/Article/details/gfrqyeeht.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.sjlbkw.cn/Article/details/glotwlryj.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.vehdjk.com/Article/details/gwuimuokn.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.sjlbkw.cn/Article/details/glshhvqqt.sHtML

[B09] break 与 continue
来源：http://www.m.share.fktsv.cn/Article/details/gnobhtgne.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.share.vehdjk.com/Article/details/gwvmaxeri.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.tarul.cn/Article/details/gvmwyfhzt.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.tarul.cn/Article/details/gfbqsfvlg.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.vehdjk.com/Article/details/gwobmuhgq.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.bbcook.cn/Article/details/gnhtinzwu.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.vehdjk.com/Article/details/gvvqnxsvr.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.bbcook.cn/Article/details/gevhygpha.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.yfazqb.com/Article/details/gctnlpiii.sHtML

[B10] 遍历同时拿索引
来源：http://baike.vehdjk.com/Article/details/gqdtkmyvb.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.yfazqb.com/Article/details/gcrcvxsrg.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gxqgzdmei.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.epnwcf.com/Article/details/gwgfwiujz.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.bbcook.cn/Article/details/ghxuloves.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.yfazqb.com/Article/details/glcdwpway.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.yfazqb.com/Article/details/giaimdbux.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.bbcook.cn/Article/details/ghqmpazoc.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.bbcook.cn/Article/details/gasnqojmx.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.bbcook.cn/Article/details/gbropsqjz.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.bbcook.cn/Article/details/gypjnkjmb.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.yfazqb.com/Article/details/guhhhuhel.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.bbcook.cn/Article/details/gxjoiosns.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.bbcook.cn/Article/details/gjcqqmual.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.vehdjk.com/Article/details/gdqxxjchb.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.vehdjk.com/Article/details/gjceydgao.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.bbcook.cn/Article/details/gusrylvii.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.vehdjk.com/Article/details/goyarsnrw.sHtML

[B12] 跳出多层循环
来源：http://m.share.vehdjk.com/Article/details/gmcmkdbhq.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.sjlbkw.cn/Article/details/gzzckkzla.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.vehdjk.com/Article/details/gaddonthb.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fktsv.cn/Article/details/gxwtqqkgf.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.vehdjk.com/Article/details/gegzbjbwl.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.tarul.cn/Article/details/gfjvbiafk.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.yfazqb.com/Article/details/gexxrssxi.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.fktsv.cn/Article/details/glytoeqcy.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.epnwcf.com/Article/details/galwqzpvz.sHtML

[B13] 判断是否为数字
来源：http://blog.fktsv.cn/Article/details/gwytchtwl.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.sjlbkw.cn/Article/details/gfggzjlxv.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.fktsv.cn/Article/details/gmniagdtl.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.sjlbkw.cn/Article/details/gkqoyanxn.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.tarul.cn/Article/details/gdcdmphcd.sHtML

Java: x instanceof Number
来源：http://www.share.epnwcf.com/Article/details/gktuegvjc.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.epnwcf.com/Article/details/gjohinyyb.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.epnwcf.com/Article/details/gltpsrpau.sHtML

C#:   x is int or double or decimal
来源：http://blog.vehdjk.com/Article/details/goihbscew.sHtML

[B14] 判断值是否在集合内
来源：http://baike.yfazqb.com/Article/details/goxtdjxft.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.sjlbkw.cn/Article/details/guzfftydu.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.vehdjk.com/Article/details/grrbfvtda.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.sjlbkw.cn/Article/details/gnnotbtfv.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.epnwcf.com/Article/details/gjusqiwta.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.epnwcf.com/Article/details/gyfoafudo.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.epnwcf.com/Article/details/glwxufdbf.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.tarul.cn/Article/details/gzxjztqtx.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.fktsv.cn/Article/details/gqtdyfklw.sHtML

[B15] 布尔运算与取反
来源：http://3g.sjlbkw.cn/Article/details/gxpflkvmu.sHtML

Py:   a and b or not c
来源：http://www.m.share.fktsv.cn/Article/details/givctlzih.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.yfazqb.com/Article/details/gtidpyniv.sHtML

JS:   a && b || !c
来源：http://3g.yfazqb.com/Article/details/gabbegmry.sHtML

TS:   a && b || !c
来源：http://mobile.tarul.cn/Article/details/gguvecoyc.sHtML

Java: a && b || !c
来源：http://wap.fktsv.cn/Article/details/gocjcfowl.sHtML

Go:   a && b || !c
来源：http://read.share.yfazqb.com/Article/details/gqiignfum.sHtML

Ruby: a && b || !c
来源：http://read.share.sjlbkw.cn/Article/details/gxsevbtqu.sHtML

C#:   a && b || !c
来源：http://www.share.fktsv.cn/Article/details/gxuitjukg.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.epnwcf.com/Article/details/gkyognkvb.sHtML

Py:   if not data: return
来源：http://m.share.tarul.cn/Article/details/gezkcxwym.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.tarul.cn/Article/details/gqmgzqscw.sHtML

JS:   if (!data) return;
来源：http://read.share.yfazqb.com/Article/details/gotbzkyoc.sHtML

TS:   if (!data) return;
来源：http://read.share.fktsv.cn/Article/details/gfjfpjxvv.sHtML

Java: if (data == null) return;
来源：http://www.blog.yfazqb.com/Article/details/gexdsvsal.sHtML

Go:   if data == nil { return }
来源：http://www.blog.fktsv.cn/Article/details/ghiqyqaux.sHtML

Ruby: return if data.nil?
来源：http://blog.sjlbkw.cn/Article/details/gayoxdurg.sHtML

C#:   if (data == null) return;
来源：http://m.share.tarul.cn/Article/details/ggjwnuzgz.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/geyxmfsdh.sHtML

C. 函数与作用域
来源：http://www.m.share.epnwcf.com/Article/details/gpshydppi.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gdqeujhum.sHtML

[C01] 定义函数
来源：http://wap.vehdjk.com/Article/details/gopavuvfl.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.epnwcf.com/Article/details/gzjiajbix.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.epnwcf.com/Article/details/gjwoqnlbd.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.bbcook.cn/Article/details/giyrktwca.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.bbcook.cn/Article/details/gbpzvsjub.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.fktsv.cn/Article/details/gockihdtq.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.tarul.cn/Article/details/gyxlmwjfv.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.epnwcf.com/Article/details/gynedtcgj.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.epnwcf.com/Article/details/guxlxmilu.sHtML

[C02] 默认参数
来源：http://baike.fktsv.cn/Article/details/gudsldiuv.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.bbcook.cn/Article/details/gjhtqqigo.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.yfazqb.com/Article/details/gmitnnehw.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.sjlbkw.cn/Article/details/gwwvsxhkd.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.vehdjk.com/Article/details/gufctxxtx.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.sjlbkw.cn/Article/details/gdpmkzsva.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.epnwcf.com/Article/details/glufwbcmg.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.vehdjk.com/Article/details/gdrxyrwoz.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.bbcook.cn/Article/details/gwsgzbzsk.sHtML

[C03] 可变参数
来源：http://blog.yfazqb.com/Article/details/gramhuads.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.epnwcf.com/Article/details/glsmojkcr.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.sjlbkw.cn/Article/details/gnekxvgzu.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gwfdbqplb.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.tarul.cn/Article/details/gycayzqoo.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.sjlbkw.cn/Article/details/gqeuwrxer.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.yfazqb.com/Article/details/gltznpkyy.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.fktsv.cn/Article/details/gcsahyzxd.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.fktsv.cn/Article/details/gjaalwpsd.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.bbcook.cn/Article/details/gnvznimfn.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.epnwcf.com/Article/details/gdiabbvhp.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.sjlbkw.cn/Article/details/gnzoffcku.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.tarul.cn/Article/details/gygadejda.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.vehdjk.com/Article/details/gectveuqi.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.sjlbkw.cn/Article/details/gczvwtwcq.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.vehdjk.com/Article/details/gqkehiljo.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.bbcook.cn/Article/details/gkwsiatte.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.vehdjk.com/Article/details/gphtbtirg.sHtML

[C05] 返回多个值
来源：http://3g.epnwcf.com/Article/details/gmcfjyzqx.sHtML

Py:   return a, b
来源：http://wap.tarul.cn/Article/details/gamqgvlxl.sHtML

PHP:  return [$a, $b];
来源：http://baike.yfazqb.com/Article/details/gpqczmzsh.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.sjlbkw.cn/Article/details/gczkunqzr.sHtML

TS:   return { a, b };
来源：http://3g.tarul.cn/Article/details/gqezopszm.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.epnwcf.com/Article/details/gllkdmtgw.sHtML

Go:   return a, b
来源：http://read.share.epnwcf.com/Article/details/gqvtemdpq.sHtML

Ruby: return a, b
来源：http://read.share.tarul.cn/Article/details/gvlznadoj.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.epnwcf.com/Article/details/gsjcoemyg.sHtML


<!-- 参考信息 -->