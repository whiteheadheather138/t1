代发 wailian999

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fktsv.cn/Article/details/glrfpwsxr.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://m.share.vehdjk.com/Article/details/gbygucydm.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.sjlbkw.cn/Article/details/gznjqcuoc.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.vehdjk.com/Article/details/gnrxxrttm.sHtML

[A18] 字符与 ASCII 码互转
来源：http://blog.bbcook.cn/Article/details/gerksspcq.sHtML

Py:   ord("A"); chr(65)
来源：http://m.share.yfazqb.com/Article/details/gxvpcsrvy.sHtML

PHP:  ord("A"); chr(65)
来源：http://baike.yfazqb.com/Article/details/ghfufqtxk.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.epnwcf.com/Article/details/gthnezlco.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.sjlbkw.cn/Article/details/gzevjxtmo.sHtML

Java: (int) 'A'; (char) 65
来源：http://wap.vehdjk.com/Article/details/gkizbdhkb.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://read.share.tarul.cn/Article/details/gcdwnenal.sHtML

Ruby: "A".ord; 65.chr
来源：http://read.share.sjlbkw.cn/Article/details/guyyntsto.sHtML

C#:   (int)'A'; (char)65
来源：http://www.share.vehdjk.com/Article/details/gzpcgvgch.sHtML

[A19] 交换两个变量
来源：http://read.share.epnwcf.com/Article/details/gpkhdwlpk.sHtML

Py:   a, b = b, a
来源：http://wap.fktsv.cn/Article/details/gcjvfphab.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://blog.tarul.cn/Article/details/gwplczxba.sHtML

JS:   [a, b] = [b, a];
来源：http://mobile.sjlbkw.cn/Article/details/gyazhjctc.sHtML

TS:   [a, b] = [b, a];
来源：http://m.share.sjlbkw.cn/Article/details/gohravsdf.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.blog.fktsv.cn/Article/details/gauzgkelr.sHtML

Go:   a, b = b, a
来源：http://3g.sjlbkw.cn/Article/details/gbxpcofmh.sHtML

Ruby: a, b = b, a
来源：http://3g.epnwcf.com/Article/details/gnqmcusep.sHtML

C#:   (a, b) = (b, a);
来源：http://www.blog.sjlbkw.cn/Article/details/gdgrjsgvq.sHtML

[A20] 读取标准输入
来源：http://www.blog.tarul.cn/Article/details/glfkrrufj.sHtML

Py:   name = input("请输入：")
来源：http://m.share.epnwcf.com/Article/details/ghgdvtlst.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://wap.fktsv.cn/Article/details/gctdwtsdz.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://blog.vehdjk.com/Article/details/gofassgoi.sHtML

TS:   // Node.js：readline 模块
来源：http://blog.yfazqb.com/Article/details/gpwpavzwm.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://wap.sjlbkw.cn/Article/details/gznbguvhk.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://3g.yfazqb.com/Article/details/gnbuexglb.sHtML

Ruby: gets.chomp
来源：http://wap.yfazqb.com/Article/details/gklowaejw.sHtML

C#:   Console.ReadLine();
来源：http://blog.tarul.cn/Article/details/gcxpeheki.sHtML

[A21] 保留指定小数位输出
来源：http://wap.tarul.cn/Article/details/gguouhamv.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.m.share.fktsv.cn/Article/details/gqapepjte.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://3g.epnwcf.com/Article/details/gxhmnkjya.sHtML

JS:   (3.14159).toFixed(2)
来源：http://baike.bbcook.cn/Article/details/gmkdncrkn.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.blog.tarul.cn/Article/details/gkjcvxhxv.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://wap.bbcook.cn/Article/details/glhinxggp.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.blog.sjlbkw.cn/Article/details/gtqpbjydt.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://m.share.vehdjk.com/Article/details/giihsrfkd.sHtML

C#:   3.14159.ToString("F2")
来源：http://blog.fktsv.cn/Article/details/gkalwfxyx.sHtML

[A22] 获取字符串长度
来源：http://baike.fktsv.cn/Article/details/geaahoite.sHtML

Py:   len(s)
来源：http://m.share.sjlbkw.cn/Article/details/girnzhzst.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://blog.fktsv.cn/Article/details/gmktvuatj.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.m.share.epnwcf.com/Article/details/gqbzdxbvh.sHtML

TS:   s.length
来源：http://www.m.share.fktsv.cn/Article/details/gkypzzqwm.sHtML

Java: s.length()
来源：http://m.share.fktsv.cn/Article/details/gwvqcukog.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://baike.tarul.cn/Article/details/galvyivvx.sHtML

Ruby: s.length
来源：http://www.blog.epnwcf.com/Article/details/gukmpcezf.sHtML

C#:   s.Length
来源：http://read.share.bbcook.cn/Article/details/gnxqlzzvs.sHtML

[A23] 大小写转换
来源：http://www.share.epnwcf.com/Article/details/ggaglxyuk.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.m.share.tarul.cn/Article/details/gihlrvova.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.m.share.fktsv.cn/Article/details/ggintwgai.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.tarul.cn/Article/details/gqnaezagj.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.sjlbkw.cn/Article/details/gdehjtlyw.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://3g.vehdjk.com/Article/details/gkfqhrzhc.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://3g.tarul.cn/Article/details/gjkbxemvz.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.share.tarul.cn/Article/details/gjomubqcg.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.share.sjlbkw.cn/Article/details/ghxgymqic.sHtML

[A24] 去除首尾空白
来源：http://www.blog.epnwcf.com/Article/details/grxvfywqf.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://m.share.fktsv.cn/Article/details/gayxgxvnj.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.m.share.bbcook.cn/Article/details/gcvolhrxh.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.fktsv.cn/Article/details/gtyhrbidt.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.bbcook.cn/Article/details/gvihvgzdi.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wap.epnwcf.com/Article/details/gzhylqeuu.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.blog.tarul.cn/Article/details/ghsciubgz.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.share.fktsv.cn/Article/details/gzckzngbv.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.share.tarul.cn/Article/details/grvycsask.sHtML

[A25] 字符串比较
来源：http://baike.fktsv.cn/Article/details/gucywadzr.sHtML

Py:   s1 == s2; s1 != s2
来源：http://wap.bbcook.cn/Article/details/gefoftosr.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://m.share.bbcook.cn/Article/details/gbsiqrzhu.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.yfazqb.com/Article/details/gcfzogfsi.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.tarul.cn/Article/details/gcodptljq.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://blog.sjlbkw.cn/Article/details/gkthazzdr.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wap.epnwcf.com/Article/details/gynlyoifo.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.m.share.yfazqb.com/Article/details/gtogpgnen.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://baike.sjlbkw.cn/Article/details/gtltiejha.sHtML

[A26] 类型转换总览
来源：http://wap.sjlbkw.cn/Article/details/gpbokqipn.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://read.share.bbcook.cn/Article/details/gcxsmipca.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.m.share.sjlbkw.cn/Article/details/gbvwpwkxr.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.m.share.fktsv.cn/Article/details/grjfvqyur.sHtML

TS:   Number() String() Boolean() x as number
来源：http://3g.fktsv.cn/Article/details/gbygqwsmi.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.share.epnwcf.com/Article/details/gbmcyiavz.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://m.share.epnwcf.com/Article/details/goflghqyz.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://baike.tarul.cn/Article/details/gmdphigxl.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://3g.tarul.cn/Article/details/gdvmhyibf.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gduoqxnnp.sHtML

B. 流程控制
来源：http://3g.sjlbkw.cn/Article/details/givcjaaeo.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gojiblfhu.sHtML

[B01] 条件判断 if / else
来源：http://m.share.bbcook.cn/Article/details/gbvlsffxq.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://mobile.vehdjk.com/Article/details/gjiebzikj.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://baike.yfazqb.com/Article/details/gfzclnhts.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.sjlbkw.cn/Article/details/gzuwfrzss.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.yfazqb.com/Article/details/glpnaybxt.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://blog.epnwcf.com/Article/details/gkhubhigy.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://blog.bbcook.cn/Article/details/gygsrraos.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://read.share.tarul.cn/Article/details/gthnrnima.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://3g.bbcook.cn/Article/details/gueqfumft.sHtML

[B02] 多分支 else if / elif
来源：http://blog.epnwcf.com/Article/details/ggvuzcmyd.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://blog.epnwcf.com/Article/details/gemrvsqqz.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://m.share.bbcook.cn/Article/details/gnvfteeku.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.yfazqb.com/Article/details/gxyufpqoo.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.tarul.cn/Article/details/gaoznollc.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.epnwcf.com/Article/details/ghiiebgmp.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://3g.vehdjk.com/Article/details/gviqosaxd.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://baike.vehdjk.com/Article/details/gjowqiiqb.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.vehdjk.com/Article/details/ghwgbqtrs.sHtML

[B03] switch / match / case
来源：http://mobile.yfazqb.com/Article/details/ggtjwdrxv.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://3g.tarul.cn/Article/details/gemvrbdwl.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.m.share.epnwcf.com/Article/details/gpzspbzaq.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.vehdjk.com/Article/details/gxckyfypq.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.bbcook.cn/Article/details/gonpmtesq.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mobile.sjlbkw.cn/Article/details/gfaedprcs.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://blog.tarul.cn/Article/details/gusdgpsml.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://m.share.vehdjk.com/Article/details/gugdkdcuy.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://3g.vehdjk.com/Article/details/goglxobja.sHtML

[B04] for 计数循环
来源：http://mobile.sjlbkw.cn/Article/details/gvedvigii.sHtML

Py:   for i in range(10): print(i)
来源：http://3g.epnwcf.com/Article/details/gzsoeqhzj.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wap.vehdjk.com/Article/details/gydhrylah.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.tarul.cn/Article/details/gmraajqhh.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.bbcook.cn/Article/details/gycdnikjk.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.blog.fktsv.cn/Article/details/gipegyinv.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://3g.sjlbkw.cn/Article/details/gzyrumhoe.sHtML

Ruby: 10.times { |i| puts i }
来源：http://read.share.fktsv.cn/Article/details/gsgktwpsi.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://blog.bbcook.cn/Article/details/gjwgtypip.sHtML

[B05] 遍历数组 / 列表
来源：http://3g.yfazqb.com/Article/details/gwjzfjepo.sHtML

Py:   for item in arr: print(item)
来源：http://m.share.vehdjk.com/Article/details/geriutllt.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.sjlbkw.cn/Article/details/gexlivrbi.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://blog.fktsv.cn/Article/details/gullfahuo.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.share.tarul.cn/Article/details/gampqcltz.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://baike.epnwcf.com/Article/details/gkftnqgey.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.blog.sjlbkw.cn/Article/details/gsthnufcc.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.tarul.cn/Article/details/ggleyzaoy.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://m.share.sjlbkw.cn/Article/details/gkilslamb.sHtML

[B06] 遍历字典 / 对象
来源：http://www.share.fktsv.cn/Article/details/glngnezbg.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.fktsv.cn/Article/details/gisxjdbxc.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.epnwcf.com/Article/details/geqrkwddl.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.yfazqb.com/Article/details/gpfpkxrqv.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.bbcook.cn/Article/details/gzqyxvxdl.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mobile.epnwcf.com/Article/details/gmsaatwlx.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.fktsv.cn/Article/details/gvcwtbbhu.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.blog.bbcook.cn/Article/details/grfekdvmu.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wap.sjlbkw.cn/Article/details/gkeznwfyj.sHtML

[B07] while 循环
来源：http://www.m.share.sjlbkw.cn/Article/details/ghcnretut.sHtML

Py:   while i < 10: i += 1
来源：http://wap.bbcook.cn/Article/details/gjrzjlxxa.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://m.share.yfazqb.com/Article/details/gqnaimekj.sHtML

JS:   while (i < 10) { i++; }
来源：http://blog.vehdjk.com/Article/details/gvhxssrfm.sHtML

TS:   while (i < 10) { i++; }
来源：http://mobile.epnwcf.com/Article/details/gcvwbkmnz.sHtML

Java: while (i < 10) { i++; }
来源：http://mobile.epnwcf.com/Article/details/gwftyeins.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.vehdjk.com/Article/details/gptfdywem.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.sjlbkw.cn/Article/details/grmheupzo.sHtML

C#:   while (i < 10) { i++; }
来源：http://m.share.sjlbkw.cn/Article/details/glgqsunfq.sHtML

[B08] do-while（至少执行一次）
来源：http://www.blog.bbcook.cn/Article/details/ghkokhdna.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.epnwcf.com/Article/details/gtasgnxxu.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.bbcook.cn/Article/details/gqwbdbfdk.sHtML

JS:   do { i++; } while (i < 10);
来源：http://3g.fktsv.cn/Article/details/gedsrtymt.sHtML

TS:   do { i++; } while (i < 10);
来源：http://baike.bbcook.cn/Article/details/gbsjmsghv.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.share.bbcook.cn/Article/details/gvhwgdyxi.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.fktsv.cn/Article/details/gkqdwuoqp.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.share.fktsv.cn/Article/details/grwcwgioi.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.epnwcf.com/Article/details/gctwevcek.sHtML

[B09] break 与 continue
来源：http://mobile.bbcook.cn/Article/details/gqssjkdwg.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.yfazqb.com/Article/details/gssweysna.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.yfazqb.com/Article/details/gdakofnio.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.tarul.cn/Article/details/gxmluyoae.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.sjlbkw.cn/Article/details/gnzjntenl.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.epnwcf.com/Article/details/gckkdsakh.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.yfazqb.com/Article/details/gztaqfqao.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.sjlbkw.cn/Article/details/gmalfqjej.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.yfazqb.com/Article/details/gcmkabirj.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.vehdjk.com/Article/details/gzypwmzne.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.fktsv.cn/Article/details/gwylehonp.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.tarul.cn/Article/details/gisbniaxg.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.fktsv.cn/Article/details/gbzbklocy.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.tarul.cn/Article/details/gzfbctubt.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.bbcook.cn/Article/details/gfgbucncv.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.vehdjk.com/Article/details/grnadujus.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mobile.bbcook.cn/Article/details/ggchcqfwu.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.vehdjk.com/Article/details/gdjoeohrs.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.vehdjk.com/Article/details/gkjixaosv.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.fktsv.cn/Article/details/gfuzcxsdu.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.epnwcf.com/Article/details/goazpdjra.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.sjlbkw.cn/Article/details/gqebbrrmn.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.fktsv.cn/Article/details/gizjxtqlw.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.vehdjk.com/Article/details/gschoyizb.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.fktsv.cn/Article/details/gwwjdazrp.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.sjlbkw.cn/Article/details/gmeaxicnl.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.bbcook.cn/Article/details/gsrpajccc.sHtML

[B12] 跳出多层循环
来源：http://read.share.tarul.cn/Article/details/ggkkegtae.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.bbcook.cn/Article/details/gtzizmcuj.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.epnwcf.com/Article/details/gbbvivtko.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.fktsv.cn/Article/details/gkwaiuqkp.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.yfazqb.com/Article/details/gupscryje.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.vehdjk.com/Article/details/gngscdjmi.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.bbcook.cn/Article/details/gxppxiuou.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.fktsv.cn/Article/details/ggewasatb.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.sjlbkw.cn/Article/details/guinlhkyb.sHtML

[B13] 判断是否为数字
来源：http://wap.tarul.cn/Article/details/gwomhqinc.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.fktsv.cn/Article/details/gidmlmpsq.sHtML

PHP:  is_numeric($x)
来源：http://read.share.bbcook.cn/Article/details/gifpleiee.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.vehdjk.com/Article/details/gprfqeqsr.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.vehdjk.com/Article/details/gcrjbxvla.sHtML

Java: x instanceof Number
来源：http://mobile.bbcook.cn/Article/details/gdwaukkrs.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.bbcook.cn/Article/details/gklqajrcf.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.vehdjk.com/Article/details/gvovsrytv.sHtML

C#:   x is int or double or decimal
来源：http://read.share.tarul.cn/Article/details/gfxfxozxx.sHtML

[B14] 判断值是否在集合内
来源：http://baike.sjlbkw.cn/Article/details/gdkcibviw.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.tarul.cn/Article/details/ghybtxgcw.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.vehdjk.com/Article/details/ghhljdrfq.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.fktsv.cn/Article/details/gastwaswi.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.epnwcf.com/Article/details/gwuhtsnur.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.yfazqb.com/Article/details/gayqamcdx.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.bbcook.cn/Article/details/gbriamajs.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.vehdjk.com/Article/details/gkqmpeulr.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.bbcook.cn/Article/details/gphbsngvk.sHtML

[B15] 布尔运算与取反
来源：http://mobile.fktsv.cn/Article/details/gieawbnir.sHtML

Py:   a and b or not c
来源：http://baike.bbcook.cn/Article/details/gfysogqce.sHtML

PHP:  $a && $b || !$c
来源：http://blog.sjlbkw.cn/Article/details/gvitvhoep.sHtML

JS:   a && b || !c
来源：http://3g.bbcook.cn/Article/details/gsffchqmq.sHtML

TS:   a && b || !c
来源：http://www.blog.yfazqb.com/Article/details/gndgniacu.sHtML

Java: a && b || !c
来源：http://baike.epnwcf.com/Article/details/grcknnhss.sHtML

Go:   a && b || !c
来源：http://read.share.epnwcf.com/Article/details/gcjexrort.sHtML

Ruby: a && b || !c
来源：http://www.share.fktsv.cn/Article/details/geobfpefj.sHtML

C#:   a && b || !c
来源：http://baike.sjlbkw.cn/Article/details/glzdcupcm.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.vehdjk.com/Article/details/gfmytudnx.sHtML

Py:   if not data: return
来源：http://3g.bbcook.cn/Article/details/gaheovzyb.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.fktsv.cn/Article/details/gbexjnmqg.sHtML

JS:   if (!data) return;
来源：http://baike.fktsv.cn/Article/details/girkzeokb.sHtML

TS:   if (!data) return;
来源：http://www.share.bbcook.cn/Article/details/gjvqikgxd.sHtML

Java: if (data == null) return;
来源：http://www.blog.sjlbkw.cn/Article/details/gsnpgwwxl.sHtML

Go:   if data == nil { return }
来源：http://m.share.yfazqb.com/Article/details/gdvdcounl.sHtML

Ruby: return if data.nil?
来源：http://www.share.epnwcf.com/Article/details/gegoxnqsj.sHtML

C#:   if (data == null) return;
来源：http://3g.tarul.cn/Article/details/gfwbgjhed.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gdylthemt.sHtML

C. 函数与作用域
来源：http://www.share.bbcook.cn/Article/details/gfllmeovi.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gmoxhzsjf.sHtML

[C01] 定义函数
来源：http://baike.tarul.cn/Article/details/ghqvnttkj.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.yfazqb.com/Article/details/gblkplcjl.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.tarul.cn/Article/details/gcayuxryj.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.yfazqb.com/Article/details/gbhswaiac.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.tarul.cn/Article/details/gzmxfjbhl.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.yfazqb.com/Article/details/glhiifcaq.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.fktsv.cn/Article/details/gpxmzbegs.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.epnwcf.com/Article/details/gmcaupwnu.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.yfazqb.com/Article/details/gdwtwocla.sHtML

[C02] 默认参数
来源：http://www.blog.yfazqb.com/Article/details/gbsukjvtt.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.epnwcf.com/Article/details/gimvihzcd.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.tarul.cn/Article/details/gmzjgvlxx.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.sjlbkw.cn/Article/details/gxalirjln.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.sjlbkw.cn/Article/details/gbdziatql.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.epnwcf.com/Article/details/grfvlormc.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.yfazqb.com/Article/details/gmopgnimr.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.epnwcf.com/Article/details/gvteywvtw.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.bbcook.cn/Article/details/gspaxlrmj.sHtML

[C03] 可变参数
来源：http://www.share.tarul.cn/Article/details/gmamddmpo.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.vehdjk.com/Article/details/gnllreuwh.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.fktsv.cn/Article/details/gscohkuql.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.epnwcf.com/Article/details/gzlmcbrey.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.vehdjk.com/Article/details/gkslzgkvp.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.yfazqb.com/Article/details/ghuewtwzl.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.sjlbkw.cn/Article/details/gjnrnsxsf.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.sjlbkw.cn/Article/details/gedykshez.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.yfazqb.com/Article/details/geylfzuon.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.tarul.cn/Article/details/gaolpxbmc.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.bbcook.cn/Article/details/girrorqbi.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.fktsv.cn/Article/details/gygvlpxuw.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.epnwcf.com/Article/details/gfrvhhwmi.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.epnwcf.com/Article/details/gvartpzcw.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.tarul.cn/Article/details/gkffnhaoy.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.vehdjk.com/Article/details/gzinqgisq.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.tarul.cn/Article/details/gdavljiwa.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.yfazqb.com/Article/details/glpxxjsso.sHtML

[C05] 返回多个值
来源：http://m.share.bbcook.cn/Article/details/grlpnvyvf.sHtML

Py:   return a, b
来源：http://m.share.fktsv.cn/Article/details/gfldvxpob.sHtML

PHP:  return [$a, $b];
来源：http://www.share.bbcook.cn/Article/details/gpaeoizar.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.tarul.cn/Article/details/gmndudpgf.sHtML

TS:   return { a, b };
来源：http://baike.vehdjk.com/Article/details/gxbsotcpo.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.sjlbkw.cn/Article/details/gnoxkfels.sHtML

Go:   return a, b
来源：http://baike.yfazqb.com/Article/details/gevyskovi.sHtML

Ruby: return a, b
来源：http://m.share.vehdjk.com/Article/details/gmrviidlx.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.bbcook.cn/Article/details/gwmhnsivg.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.epnwcf.com/Article/details/gpwxbjvsv.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.epnwcf.com/Article/details/gslepaenj.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.vehdjk.com/Article/details/gyoahaafp.sHtML

JS:   const square = x => x * x;
来源：http://3g.epnwcf.com/Article/details/gvxxqvhxu.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.vehdjk.com/Article/details/gxptfxcke.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.bbcook.cn/Article/details/gmwaogzyq.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.sjlbkw.cn/Article/details/gqdziqwig.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.tarul.cn/Article/details/gqelfsdyd.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.bbcook.cn/Article/details/ggluvhnmw.sHtML

[C07] 把函数作为参数传入
来源：http://wap.vehdjk.com/Article/details/gntrkpkme.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.bbcook.cn/Article/details/gexsmzuwp.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.vehdjk.com/Article/details/gphbsnvxr.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.vehdjk.com/Article/details/grngoxttc.sHtML

TS:   arr.map(String)
来源：http://wap.yfazqb.com/Article/details/gujzdciex.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.sjlbkw.cn/Article/details/gmihpijgo.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.tarul.cn/Article/details/gwerifmpd.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.fktsv.cn/Article/details/guljkkhtu.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.sjlbkw.cn/Article/details/gpckhavty.sHtML

[C08] 闭包
来源：http://read.share.yfazqb.com/Article/details/gxvppdouz.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.fktsv.cn/Article/details/gemmzzqpb.sHtML


<!-- 参考信息 -->