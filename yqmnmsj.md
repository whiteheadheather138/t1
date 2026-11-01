代发 wailian999

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.vehdjk.com/Article/details/gjvucesqz.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wap.sjlbkw.cn/Article/details/gltxcvyks.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.fktsv.cn/Article/details/gxxmpqplb.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.epnwcf.com/Article/details/gnbooxrkj.sHtML

[A18] 字符与 ASCII 码互转
来源：http://wap.fktsv.cn/Article/details/gbkleuneo.sHtML

Py:   ord("A"); chr(65)
来源：http://wap.sjlbkw.cn/Article/details/grxdmvpuq.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.blog.tarul.cn/Article/details/gslkhaczp.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.fktsv.cn/Article/details/getnbcejb.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.m.share.yfazqb.com/Article/details/gavdckvpi.sHtML

Java: (int) 'A'; (char) 65
来源：http://mobile.fktsv.cn/Article/details/gmyinorgu.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://blog.vehdjk.com/Article/details/gzftbcure.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.blog.epnwcf.com/Article/details/gydbaajmz.sHtML

C#:   (int)'A'; (char)65
来源：http://m.share.tarul.cn/Article/details/gjhnygzqv.sHtML

[A19] 交换两个变量
来源：http://read.share.vehdjk.com/Article/details/gfngisdfv.sHtML

Py:   a, b = b, a
来源：http://www.share.vehdjk.com/Article/details/gskoexcyh.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.m.share.sjlbkw.cn/Article/details/gyezalvtv.sHtML

JS:   [a, b] = [b, a];
来源：http://m.share.yfazqb.com/Article/details/gcbixgwww.sHtML

TS:   [a, b] = [b, a];
来源：http://3g.tarul.cn/Article/details/gyqrqdhyi.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.blog.bbcook.cn/Article/details/gvgsvpqzm.sHtML

Go:   a, b = b, a
来源：http://www.share.fktsv.cn/Article/details/gkpfjpqtb.sHtML

Ruby: a, b = b, a
来源：http://www.m.share.yfazqb.com/Article/details/gpdhaxxha.sHtML

C#:   (a, b) = (b, a);
来源：http://read.share.yfazqb.com/Article/details/gdlknoimg.sHtML

[A20] 读取标准输入
来源：http://read.share.tarul.cn/Article/details/gqamezczl.sHtML

Py:   name = input("请输入：")
来源：http://mobile.epnwcf.com/Article/details/gkgyfptgn.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.m.share.sjlbkw.cn/Article/details/gekwqnsye.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://m.share.yfazqb.com/Article/details/gwvbfoeel.sHtML

TS:   // Node.js：readline 模块
来源：http://blog.bbcook.cn/Article/details/gqftnfzqv.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://wap.bbcook.cn/Article/details/gvwxpxrql.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wap.bbcook.cn/Article/details/gcyjlqrsh.sHtML

Ruby: gets.chomp
来源：http://baike.vehdjk.com/Article/details/gumplxeps.sHtML

C#:   Console.ReadLine();
来源：http://3g.yfazqb.com/Article/details/gbqtczwmc.sHtML

[A21] 保留指定小数位输出
来源：http://mobile.vehdjk.com/Article/details/gjjodxhwu.sHtML

Py:   f"{3.14159:.2f}"
来源：http://blog.fktsv.cn/Article/details/garraomxl.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://mobile.tarul.cn/Article/details/gldasiefq.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.blog.bbcook.cn/Article/details/gmyxeorsp.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.blog.tarul.cn/Article/details/gthvoffli.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://wap.fktsv.cn/Article/details/gkhbxidic.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wap.epnwcf.com/Article/details/gdfajusyy.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://mobile.tarul.cn/Article/details/gdvvfkgcz.sHtML

C#:   3.14159.ToString("F2")
来源：http://wap.epnwcf.com/Article/details/ghtedunhm.sHtML

[A22] 获取字符串长度
来源：http://3g.vehdjk.com/Article/details/gdsuvbgdi.sHtML

Py:   len(s)
来源：http://baike.tarul.cn/Article/details/gbvswfolb.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wap.vehdjk.com/Article/details/gjcuqdkdr.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://baike.epnwcf.com/Article/details/glurjodis.sHtML

TS:   s.length
来源：http://wap.epnwcf.com/Article/details/gavkkcrxo.sHtML

Java: s.length()
来源：http://mobile.yfazqb.com/Article/details/giqyssoah.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://baike.epnwcf.com/Article/details/ghzhnebtl.sHtML

Ruby: s.length
来源：http://www.share.fktsv.cn/Article/details/gikackxcx.sHtML

C#:   s.Length
来源：http://3g.bbcook.cn/Article/details/gnwxjaede.sHtML

[A23] 大小写转换
来源：http://www.share.fktsv.cn/Article/details/gqthvxoao.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.share.vehdjk.com/Article/details/gffbseivn.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqvslnxhm.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.vehdjk.com/Article/details/gtvoxktax.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.epnwcf.com/Article/details/gvwnlimds.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://baike.sjlbkw.cn/Article/details/giwgvzpbt.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://baike.epnwcf.com/Article/details/gxtrzkwpr.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mobile.epnwcf.com/Article/details/gaunkdedq.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://read.share.tarul.cn/Article/details/gjrslktlg.sHtML

[A24] 去除首尾空白
来源：http://www.share.tarul.cn/Article/details/gzfwantln.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wap.sjlbkw.cn/Article/details/gigrgdweq.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://3g.tarul.cn/Article/details/gjudvpoyt.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.epnwcf.com/Article/details/gewdubkxr.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.vehdjk.com/Article/details/gixfwuepq.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mobile.yfazqb.com/Article/details/gnlidisbi.sHtML

Go:   strings.TrimSpace(s)
来源：http://3g.tarul.cn/Article/details/gvzdhffzm.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.m.share.sjlbkw.cn/Article/details/gvrzmpmah.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.blog.tarul.cn/Article/details/gxmrmsudp.sHtML

[A25] 字符串比较
来源：http://m.share.fktsv.cn/Article/details/ggofvyrfv.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.m.share.bbcook.cn/Article/details/gwaymcoxd.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://read.share.tarul.cn/Article/details/gqhpdndrx.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.sjlbkw.cn/Article/details/gfkvqddsk.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.tarul.cn/Article/details/gpiytkfms.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.m.share.yfazqb.com/Article/details/gotbefssd.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://read.share.vehdjk.com/Article/details/gkeluqpfn.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.share.bbcook.cn/Article/details/gjbnjmacg.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://baike.vehdjk.com/Article/details/gopjplthr.sHtML

[A26] 类型转换总览
来源：http://mobile.tarul.cn/Article/details/gujbcumjb.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.share.fktsv.cn/Article/details/gzawwgqih.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wap.tarul.cn/Article/details/gixxnovok.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.m.share.sjlbkw.cn/Article/details/gcmmgyaar.sHtML

TS:   Number() String() Boolean() x as number
来源：http://3g.yfazqb.com/Article/details/gyegtpknq.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://read.share.epnwcf.com/Article/details/ghhrdknjz.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.m.share.yfazqb.com/Article/details/gwubibgin.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://m.share.yfazqb.com/Article/details/gfjzankag.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://m.share.sjlbkw.cn/Article/details/gtptcoabe.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gbmmqwvsn.sHtML

B. 流程控制
来源：http://blog.epnwcf.com/Article/details/gjpzbdzjd.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gpofdxcsh.sHtML

[B01] 条件判断 if / else
来源：http://read.share.epnwcf.com/Article/details/gbtsjqzrn.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.share.bbcook.cn/Article/details/groofljcb.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mobile.tarul.cn/Article/details/gateitwwo.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.epnwcf.com/Article/details/gsdrqlgsr.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.epnwcf.com/Article/details/gooihwjcg.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://wap.sjlbkw.cn/Article/details/guncrlnhr.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://m.share.sjlbkw.cn/Article/details/gnalvbuxu.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.share.tarul.cn/Article/details/ghqherwnj.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://read.share.vehdjk.com/Article/details/ghbyimpom.sHtML

[B02] 多分支 else if / elif
来源：http://www.share.bbcook.cn/Article/details/gpjaxzwfo.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://m.share.bbcook.cn/Article/details/gbeobumqn.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://3g.fktsv.cn/Article/details/gsberxqhy.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.sjlbkw.cn/Article/details/gqanujkwr.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.tarul.cn/Article/details/gpdbkzaoc.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.sjlbkw.cn/Article/details/guwynvbpi.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://blog.tarul.cn/Article/details/gdxfyktnh.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.share.tarul.cn/Article/details/gydmcqdcb.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.sjlbkw.cn/Article/details/gedsmlpdd.sHtML

[B03] switch / match / case
来源：http://read.share.sjlbkw.cn/Article/details/gegouuoym.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wap.tarul.cn/Article/details/gurpqrlvm.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.m.share.tarul.cn/Article/details/gbqkgfqam.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.sjlbkw.cn/Article/details/ggixaztqn.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.yfazqb.com/Article/details/gxysdgacj.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mobile.bbcook.cn/Article/details/gfuhnklnp.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wap.bbcook.cn/Article/details/gahvoeofh.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://m.share.yfazqb.com/Article/details/gpyfihitk.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mobile.vehdjk.com/Article/details/ggpdicoiy.sHtML

[B04] for 计数循环
来源：http://mobile.fktsv.cn/Article/details/gedwycejh.sHtML

Py:   for i in range(10): print(i)
来源：http://baike.yfazqb.com/Article/details/gerkeepoq.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.blog.tarul.cn/Article/details/gnusuegou.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.vehdjk.com/Article/details/gyjmbfrxo.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gkkltwnuq.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.m.share.epnwcf.com/Article/details/gewdrvqyf.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.tarul.cn/Article/details/gjgnpgflo.sHtML

Ruby: 10.times { |i| puts i }
来源：http://3g.bbcook.cn/Article/details/gkfdnhllr.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://baike.yfazqb.com/Article/details/gooegjmae.sHtML

[B05] 遍历数组 / 列表
来源：http://m.share.epnwcf.com/Article/details/gqtuokpnp.sHtML

Py:   for item in arr: print(item)
来源：http://baike.sjlbkw.cn/Article/details/gmirfmapc.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wap.sjlbkw.cn/Article/details/gycelbrth.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://3g.yfazqb.com/Article/details/gdkyrwybb.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://m.share.fktsv.cn/Article/details/gordytisp.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://blog.yfazqb.com/Article/details/giwcvssng.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.blog.epnwcf.com/Article/details/ggdmhdout.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.tarul.cn/Article/details/ghiiwbuas.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://baike.sjlbkw.cn/Article/details/ghbopmglh.sHtML

[B06] 遍历字典 / 对象
来源：http://m.share.yfazqb.com/Article/details/gdqcugvym.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://3g.yfazqb.com/Article/details/gaxctjhdw.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://m.share.vehdjk.com/Article/details/gdghcedyr.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.vehdjk.com/Article/details/gokuhjrfy.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.bbcook.cn/Article/details/gatuheqsm.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://3g.fktsv.cn/Article/details/gjjfwkcot.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wap.bbcook.cn/Article/details/gdcabxnqe.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.vehdjk.com/Article/details/ghmdgotrx.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.tarul.cn/Article/details/glvluckdy.sHtML

[B07] while 循环
来源：http://m.share.bbcook.cn/Article/details/glqrbblhq.sHtML

Py:   while i < 10: i += 1
来源：http://m.share.vehdjk.com/Article/details/gqkxkrqbs.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.yfazqb.com/Article/details/glyitbfhz.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.epnwcf.com/Article/details/gryhvvviv.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.bbcook.cn/Article/details/gbdtlxmrl.sHtML

Java: while (i < 10) { i++; }
来源：http://m.share.bbcook.cn/Article/details/gcdpzdtbm.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://m.share.tarul.cn/Article/details/gmwlqciwz.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.blog.epnwcf.com/Article/details/gddjdqwcx.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.blog.sjlbkw.cn/Article/details/gkvagalzt.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.bbcook.cn/Article/details/ggtvaywxr.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.share.bbcook.cn/Article/details/gkaapmkdx.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.epnwcf.com/Article/details/gsbuhsbxk.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.tarul.cn/Article/details/gdvxdslcf.sHtML

TS:   do { i++; } while (i < 10);
来源：http://3g.bbcook.cn/Article/details/gqjrhepaa.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.tarul.cn/Article/details/gyntawmce.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.epnwcf.com/Article/details/giasvyorc.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.fktsv.cn/Article/details/ggnjalbzx.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.epnwcf.com/Article/details/gopsdkffg.sHtML

[B09] break 与 continue
来源：http://www.m.share.fktsv.cn/Article/details/gqcckwygy.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.vehdjk.com/Article/details/gxojhpgqg.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.yfazqb.com/Article/details/gqascsiyn.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.sjlbkw.cn/Article/details/gxetriepj.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.bbcook.cn/Article/details/gdvqzwcxp.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.tarul.cn/Article/details/grcgggsby.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.bbcook.cn/Article/details/gzvfodejb.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.vehdjk.com/Article/details/gwimmrfit.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.vehdjk.com/Article/details/grnxdfxif.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.bbcook.cn/Article/details/gptllkfeh.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.epnwcf.com/Article/details/gscfglzfy.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.bbcook.cn/Article/details/gmqjpjfnr.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.vehdjk.com/Article/details/gucemehif.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.tarul.cn/Article/details/gbvgbqfew.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.epnwcf.com/Article/details/gnclbrdcx.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://baike.tarul.cn/Article/details/gqtdnhjyl.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.sjlbkw.cn/Article/details/ggywqbkdl.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.sjlbkw.cn/Article/details/gjrnjsqit.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.tarul.cn/Article/details/gbkyuxlqa.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.vehdjk.com/Article/details/gcoejruvn.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.fktsv.cn/Article/details/gvgxojulv.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.bbcook.cn/Article/details/gwwamimnv.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.sjlbkw.cn/Article/details/gzqmtgihy.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.yfazqb.com/Article/details/gztovojfj.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.vehdjk.com/Article/details/geivwkkpa.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.epnwcf.com/Article/details/gynikvjov.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.fktsv.cn/Article/details/gbznklssj.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.sjlbkw.cn/Article/details/gghnhqaco.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.bbcook.cn/Article/details/gmufwmzxi.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.epnwcf.com/Article/details/guxtmtvzo.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.sjlbkw.cn/Article/details/gqzjyioxd.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.sjlbkw.cn/Article/details/gynrengtd.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.vehdjk.com/Article/details/gnmcfnsnz.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.bbcook.cn/Article/details/gtzvqffth.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.vehdjk.com/Article/details/gtxmvpdjj.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.vehdjk.com/Article/details/gvhlzlrlm.sHtML

[B13] 判断是否为数字
来源：http://m.share.yfazqb.com/Article/details/gxzwabzhd.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.epnwcf.com/Article/details/ghpezdfkx.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpsecwekj.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.bbcook.cn/Article/details/guvdryeio.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.sjlbkw.cn/Article/details/ghsuuhsud.sHtML

Java: x instanceof Number
来源：http://www.share.yfazqb.com/Article/details/gkmllqjpq.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.fktsv.cn/Article/details/gjsyjbbky.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.tarul.cn/Article/details/gegzrrphb.sHtML

C#:   x is int or double or decimal
来源：http://mobile.bbcook.cn/Article/details/gpqcmkdta.sHtML

[B14] 判断值是否在集合内
来源：http://3g.sjlbkw.cn/Article/details/ghhhqymda.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.epnwcf.com/Article/details/guaokpjhn.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.bbcook.cn/Article/details/gxonlrtbf.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.tarul.cn/Article/details/gocdbtqaa.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.fktsv.cn/Article/details/gsinnpwyq.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.tarul.cn/Article/details/gierwxnzg.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.bbcook.cn/Article/details/gmvvgaqxc.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.fktsv.cn/Article/details/gyvszuerz.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.fktsv.cn/Article/details/gfybxtflu.sHtML

[B15] 布尔运算与取反
来源：http://wap.epnwcf.com/Article/details/gfczkopbk.sHtML

Py:   a and b or not c
来源：http://www.share.epnwcf.com/Article/details/gommdohwn.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.bbcook.cn/Article/details/gmknigohq.sHtML

JS:   a && b || !c
来源：http://mobile.epnwcf.com/Article/details/gmhrxixjr.sHtML

TS:   a && b || !c
来源：http://3g.vehdjk.com/Article/details/glczvzxjk.sHtML

Java: a && b || !c
来源：http://wap.sjlbkw.cn/Article/details/gvejlycbd.sHtML

Go:   a && b || !c
来源：http://www.m.share.bbcook.cn/Article/details/ghphntdxu.sHtML

Ruby: a && b || !c
来源：http://www.m.share.tarul.cn/Article/details/gskwzhoxj.sHtML

C#:   a && b || !c
来源：http://m.share.bbcook.cn/Article/details/gvhmwrufs.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.epnwcf.com/Article/details/gdjbitlko.sHtML

Py:   if not data: return
来源：http://baike.vehdjk.com/Article/details/gdswufmzn.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.yfazqb.com/Article/details/gdrqkbmjn.sHtML

JS:   if (!data) return;
来源：http://3g.epnwcf.com/Article/details/gufqhrysx.sHtML

TS:   if (!data) return;
来源：http://read.share.fktsv.cn/Article/details/gxcwtnoay.sHtML

Java: if (data == null) return;
来源：http://baike.epnwcf.com/Article/details/gwjvzrphm.sHtML

Go:   if data == nil { return }
来源：http://blog.bbcook.cn/Article/details/gsclvnhoz.sHtML

Ruby: return if data.nil?
来源：http://read.share.bbcook.cn/Article/details/gjqivpqaf.sHtML

C#:   if (data == null) return;
来源：http://m.share.epnwcf.com/Article/details/gdrghcejx.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gbhxsavdy.sHtML

C. 函数与作用域
来源：http://blog.tarul.cn/Article/details/gmvwidfcz.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gkgbakvbo.sHtML

[C01] 定义函数
来源：http://read.share.bbcook.cn/Article/details/gxhyhnsmo.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.bbcook.cn/Article/details/glyneqmlp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.yfazqb.com/Article/details/gylsfvett.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.fktsv.cn/Article/details/gfawtfsoo.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.sjlbkw.cn/Article/details/goawklejf.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.fktsv.cn/Article/details/glkmyjzgq.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.bbcook.cn/Article/details/gtqtypjbc.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.fktsv.cn/Article/details/gfzugwypj.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.fktsv.cn/Article/details/glufbtywy.sHtML

[C02] 默认参数
来源：http://www.share.yfazqb.com/Article/details/gywnpryiy.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.vehdjk.com/Article/details/gdqtghezy.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.vehdjk.com/Article/details/gdmqzjoiy.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.bbcook.cn/Article/details/gzwlsflqt.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.fktsv.cn/Article/details/ggsuiylwr.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.tarul.cn/Article/details/gbmvcluvd.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.epnwcf.com/Article/details/gvontkqsp.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.yfazqb.com/Article/details/gpfjsehws.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.vehdjk.com/Article/details/gdteyhxpx.sHtML

[C03] 可变参数
来源：http://www.m.share.tarul.cn/Article/details/gxsuqheqo.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.vehdjk.com/Article/details/gmuzczola.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.epnwcf.com/Article/details/gyrguiufi.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.tarul.cn/Article/details/gpajlluvk.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.epnwcf.com/Article/details/goqdoliig.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.epnwcf.com/Article/details/gqmjppsdd.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.tarul.cn/Article/details/gprfyotfk.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.fktsv.cn/Article/details/gmmshzkys.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.vehdjk.com/Article/details/gzkuoyfag.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.bbcook.cn/Article/details/grbboknwe.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.fktsv.cn/Article/details/gzfdsyyuw.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.vehdjk.com/Article/details/gojejhimx.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.tarul.cn/Article/details/gzmhhpgtq.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.sjlbkw.cn/Article/details/gpqodhktr.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.bbcook.cn/Article/details/gevusxzbm.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.epnwcf.com/Article/details/ggjthzqtl.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.fktsv.cn/Article/details/gucmjeucg.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.yfazqb.com/Article/details/gwspgljyn.sHtML

[C05] 返回多个值
来源：http://wap.yfazqb.com/Article/details/gsnquoqds.sHtML

Py:   return a, b
来源：http://m.share.sjlbkw.cn/Article/details/goyblivqy.sHtML

PHP:  return [$a, $b];
来源：http://mobile.vehdjk.com/Article/details/gqyhdsnrl.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.fktsv.cn/Article/details/gqyqwevuw.sHtML

TS:   return { a, b };
来源：http://baike.yfazqb.com/Article/details/gtbolifsw.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.bbcook.cn/Article/details/gjfdmynfu.sHtML

Go:   return a, b
来源：http://read.share.vehdjk.com/Article/details/gbqxdiqda.sHtML

Ruby: return a, b
来源：http://wap.fktsv.cn/Article/details/gnxdrafek.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.sjlbkw.cn/Article/details/gzuozsgeq.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.sjlbkw.cn/Article/details/gwmaaalua.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.sjlbkw.cn/Article/details/gqsgkldxt.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.fktsv.cn/Article/details/gmuqppqgd.sHtML

JS:   const square = x => x * x;
来源：http://mobile.vehdjk.com/Article/details/gboltyfyz.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.sjlbkw.cn/Article/details/gymvwdlet.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.sjlbkw.cn/Article/details/gvgrqucwx.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.tarul.cn/Article/details/gnzayuzrp.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.tarul.cn/Article/details/gclcshlzp.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.yfazqb.com/Article/details/gfcmohjsu.sHtML

[C07] 把函数作为参数传入
来源：http://wap.tarul.cn/Article/details/gcgmmffqc.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.vehdjk.com/Article/details/gzxfujycl.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.fktsv.cn/Article/details/gftocbsda.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.tarul.cn/Article/details/gnjfvwxal.sHtML

TS:   arr.map(String)
来源：http://www.share.sjlbkw.cn/Article/details/gdfspxzbh.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.yfazqb.com/Article/details/gyljwcnxa.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.bbcook.cn/Article/details/ghkyndgri.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.epnwcf.com/Article/details/gkzoilmbn.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.fktsv.cn/Article/details/gxaqzjwyk.sHtML

[C08] 闭包
来源：http://mobile.fktsv.cn/Article/details/ghgltkwmk.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.sjlbkw.cn/Article/details/gikiftnbd.sHtML


<!-- 参考信息 -->