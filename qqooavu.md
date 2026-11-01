代发 wailian999

Ruby: a, b = b, a
来源：http://baike.yfazqb.com/Article/details/gflmkbkmj.sHtML

C#:   (a, b) = (b, a);
来源：http://www.share.yfazqb.com/Article/details/ggywurvlj.sHtML

[A20] 读取标准输入
来源：http://3g.sjlbkw.cn/Article/details/gbxrftffx.sHtML

Py:   name = input("请输入：")
来源：http://baike.tarul.cn/Article/details/gfrarxdhe.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.m.share.vehdjk.com/Article/details/gsckykliu.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.share.yfazqb.com/Article/details/gcelmhtne.sHtML

TS:   // Node.js：readline 模块
来源：http://www.share.sjlbkw.cn/Article/details/gwqiufzqt.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://blog.bbcook.cn/Article/details/gccozigtr.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://blog.sjlbkw.cn/Article/details/guywkjeur.sHtML

Ruby: gets.chomp
来源：http://m.share.sjlbkw.cn/Article/details/gfgmipkqm.sHtML

C#:   Console.ReadLine();
来源：http://read.share.bbcook.cn/Article/details/gsqahkfdr.sHtML

[A21] 保留指定小数位输出
来源：http://www.share.epnwcf.com/Article/details/gksmfbltn.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.blog.sjlbkw.cn/Article/details/gxhtlknjj.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://read.share.sjlbkw.cn/Article/details/gmyrurgro.sHtML

JS:   (3.14159).toFixed(2)
来源：http://m.share.bbcook.cn/Article/details/gcgqvroih.sHtML

TS:   (3.14159).toFixed(2)
来源：http://m.share.epnwcf.com/Article/details/gpotcgjzd.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://read.share.bbcook.cn/Article/details/gwgjeeoci.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://read.share.fktsv.cn/Article/details/gxacvepxx.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://mobile.tarul.cn/Article/details/gllbbxpli.sHtML

C#:   3.14159.ToString("F2")
来源：http://read.share.epnwcf.com/Article/details/gwmbvnsft.sHtML

[A22] 获取字符串长度
来源：http://baike.fktsv.cn/Article/details/gzddvpfqp.sHtML

Py:   len(s)
来源：http://www.m.share.epnwcf.com/Article/details/gychksycw.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://3g.fktsv.cn/Article/details/gpnfwcwjt.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.m.share.sjlbkw.cn/Article/details/gsnkmeqqz.sHtML

TS:   s.length
来源：http://baike.vehdjk.com/Article/details/gvsyevoed.sHtML

Java: s.length()
来源：http://baike.yfazqb.com/Article/details/gzzrgloju.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.share.tarul.cn/Article/details/gfnamtini.sHtML

Ruby: s.length
来源：http://wap.yfazqb.com/Article/details/gnctnwwov.sHtML

C#:   s.Length
来源：http://www.blog.fktsv.cn/Article/details/gjrhusywl.sHtML

[A23] 大小写转换
来源：http://m.share.bbcook.cn/Article/details/gexlwerny.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://baike.fktsv.cn/Article/details/gnqjsbzrd.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mobile.tarul.cn/Article/details/gacrqeqtj.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.yfazqb.com/Article/details/giogdrxcs.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.bbcook.cn/Article/details/gfwlthitu.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.fktsv.cn/Article/details/gjfojeovm.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://3g.epnwcf.com/Article/details/gmtogkora.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mobile.vehdjk.com/Article/details/gyvxdcadv.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.m.share.epnwcf.com/Article/details/gtudnhifa.sHtML

[A24] 去除首尾空白
来源：http://baike.epnwcf.com/Article/details/gehawquhs.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.share.fktsv.cn/Article/details/gdyxnlpdv.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wap.fktsv.cn/Article/details/gxwzjxnug.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.vehdjk.com/Article/details/gaqpdqpeh.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.epnwcf.com/Article/details/gznppihkx.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.share.bbcook.cn/Article/details/gamvciopw.sHtML

Go:   strings.TrimSpace(s)
来源：http://mobile.bbcook.cn/Article/details/gykrnzybr.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://3g.sjlbkw.cn/Article/details/ghoojuvkk.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://baike.yfazqb.com/Article/details/gtvadribw.sHtML

[A25] 字符串比较
来源：http://read.share.tarul.cn/Article/details/gpcaqolft.sHtML

Py:   s1 == s2; s1 != s2
来源：http://wap.fktsv.cn/Article/details/gegussnoh.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mobile.epnwcf.com/Article/details/gobixbwvd.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.sjlbkw.cn/Article/details/gtsbnhrgn.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.bbcook.cn/Article/details/gaagenfav.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.m.share.bbcook.cn/Article/details/gcpiftpbf.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://baike.yfazqb.com/Article/details/gfpnvfjuu.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://read.share.yfazqb.com/Article/details/gzquhlsqj.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://m.share.epnwcf.com/Article/details/gauirhbgx.sHtML

[A26] 类型转换总览
来源：http://blog.sjlbkw.cn/Article/details/ghpxphdsz.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.share.yfazqb.com/Article/details/gdidhgumt.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://m.share.vehdjk.com/Article/details/gfblrokpq.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wap.fktsv.cn/Article/details/gqjvecagk.sHtML

TS:   Number() String() Boolean() x as number
来源：http://3g.sjlbkw.cn/Article/details/gtqxkmxyi.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wap.bbcook.cn/Article/details/gfwbqaaee.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://m.share.vehdjk.com/Article/details/gxuscgsla.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://blog.bbcook.cn/Article/details/grwzjledc.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://m.share.fktsv.cn/Article/details/gndjdybck.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gdfvarimp.sHtML

B. 流程控制
来源：http://3g.sjlbkw.cn/Article/details/gdggwzfwx.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gjvqnvxvk.sHtML

[B01] 条件判断 if / else
来源：http://read.share.fktsv.cn/Article/details/gkduoaeah.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://blog.tarul.cn/Article/details/ghsouxxar.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://read.share.sjlbkw.cn/Article/details/gvpberzfb.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.vehdjk.com/Article/details/gpcccgqms.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.bbcook.cn/Article/details/gzgkexwig.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://m.share.epnwcf.com/Article/details/gkbnvcrcp.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.share.epnwcf.com/Article/details/ghhputwds.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.m.share.sjlbkw.cn/Article/details/gcpttqqlt.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://3g.epnwcf.com/Article/details/gscqowvim.sHtML

[B02] 多分支 else if / elif
来源：http://m.share.sjlbkw.cn/Article/details/gckqbuita.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://m.share.tarul.cn/Article/details/glarryhcl.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://blog.epnwcf.com/Article/details/gjuurijvr.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.bbcook.cn/Article/details/gbdbskpjn.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.yfazqb.com/Article/details/guagqfzta.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.epnwcf.com/Article/details/gcdserwlz.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://m.share.vehdjk.com/Article/details/gmtgiygfx.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://m.share.tarul.cn/Article/details/gprbaqhya.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.yfazqb.com/Article/details/gdmqghcmn.sHtML

[B03] switch / match / case
来源：http://blog.tarul.cn/Article/details/gavshgndd.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://m.share.fktsv.cn/Article/details/gmhcomlvi.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mobile.epnwcf.com/Article/details/ghllhhrda.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.fktsv.cn/Article/details/gqiehfrst.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gmakiexxd.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://3g.vehdjk.com/Article/details/gxjyzhbsd.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.blog.bbcook.cn/Article/details/gucymngbf.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://m.share.yfazqb.com/Article/details/gcsdrxpgi.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.share.vehdjk.com/Article/details/gpvgnkscm.sHtML

[B04] for 计数循环
来源：http://3g.fktsv.cn/Article/details/gcrabdapt.sHtML

Py:   for i in range(10): print(i)
来源：http://wap.fktsv.cn/Article/details/gosuwlarh.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wap.fktsv.cn/Article/details/gcuwlgfbp.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.yfazqb.com/Article/details/gcrunbvcq.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.epnwcf.com/Article/details/glzflswih.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://read.share.tarul.cn/Article/details/gynrenjgq.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.m.share.bbcook.cn/Article/details/ggfpuftqr.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.m.share.epnwcf.com/Article/details/gkglgeyvz.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.share.vehdjk.com/Article/details/gzqmvhxig.sHtML

[B05] 遍历数组 / 列表
来源：http://blog.epnwcf.com/Article/details/gsicuapoa.sHtML

Py:   for item in arr: print(item)
来源：http://wap.tarul.cn/Article/details/gjdzalygj.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.vehdjk.com/Article/details/ghnjbdalp.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.fktsv.cn/Article/details/gpcoemvpt.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://3g.bbcook.cn/Article/details/ghxssrubw.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.share.bbcook.cn/Article/details/gmheazdmw.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.bbcook.cn/Article/details/geifrfbkz.sHtML

Ruby: arr.each { |item| puts item }
来源：http://baike.yfazqb.com/Article/details/gnbtyriqu.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://blog.yfazqb.com/Article/details/gbygsoend.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.tarul.cn/Article/details/gczlzptze.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.tarul.cn/Article/details/ghaebbgel.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mobile.yfazqb.com/Article/details/gtysofyat.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.sjlbkw.cn/Article/details/ggwnruyhu.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.bbcook.cn/Article/details/gtdmzohkk.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mobile.tarul.cn/Article/details/guavfhwtl.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://baike.epnwcf.com/Article/details/gkmsvfmyr.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.epnwcf.com/Article/details/gwejbfjbq.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.epnwcf.com/Article/details/gtqgxmefa.sHtML

[B07] while 循环
来源：http://www.share.tarul.cn/Article/details/gcirtypwv.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.yfazqb.com/Article/details/gpbxjziai.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.vehdjk.com/Article/details/gmigtvfhf.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.blog.yfazqb.com/Article/details/goelyngqk.sHtML

TS:   while (i < 10) { i++; }
来源：http://blog.vehdjk.com/Article/details/gnoossljz.sHtML

Java: while (i < 10) { i++; }
来源：http://m.share.tarul.cn/Article/details/gjpkrzplk.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.epnwcf.com/Article/details/gadrsggbb.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.sjlbkw.cn/Article/details/gxgummvsr.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.fktsv.cn/Article/details/gkvnyoowv.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.epnwcf.com/Article/details/grrsuzktx.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.epnwcf.com/Article/details/gskpzhozz.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.bbcook.cn/Article/details/gvsxallwe.sHtML

JS:   do { i++; } while (i < 10);
来源：http://3g.sjlbkw.cn/Article/details/gpnubrneo.sHtML

TS:   do { i++; } while (i < 10);
来源：http://3g.bbcook.cn/Article/details/gmoydbiyy.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.epnwcf.com/Article/details/grhjjeyaw.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.vehdjk.com/Article/details/ggqmqjqxy.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://m.share.yfazqb.com/Article/details/gbnubcnua.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.bbcook.cn/Article/details/gkjpyhxfn.sHtML

[B09] break 与 continue
来源：http://www.blog.bbcook.cn/Article/details/guliwnvrp.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.epnwcf.com/Article/details/guetlbwpv.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.fktsv.cn/Article/details/gycsyygca.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.sjlbkw.cn/Article/details/gvtbnqety.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fktsv.cn/Article/details/ggoflpfll.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.vehdjk.com/Article/details/gjifotvrt.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.bbcook.cn/Article/details/gkevqmjce.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.vehdjk.com/Article/details/gfoolluwj.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.yfazqb.com/Article/details/gruusbkmh.sHtML

[B10] 遍历同时拿索引
来源：http://3g.sjlbkw.cn/Article/details/gxkznzeau.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.epnwcf.com/Article/details/gvuvjaoni.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.vehdjk.com/Article/details/gsugpvtqp.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://m.share.yfazqb.com/Article/details/gfimunjrd.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.epnwcf.com/Article/details/gjhzhaxui.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.vehdjk.com/Article/details/gcxzopdao.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.yfazqb.com/Article/details/ggypfnwbf.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.yfazqb.com/Article/details/gbzeqmfej.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.vehdjk.com/Article/details/gohrtpzpl.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.bbcook.cn/Article/details/ggiepemlh.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.sjlbkw.cn/Article/details/gjsijrbsl.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.yfazqb.com/Article/details/gfbmomdgj.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.sjlbkw.cn/Article/details/gsebsicgf.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.yfazqb.com/Article/details/gnsxfdqly.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.fktsv.cn/Article/details/gpafvuded.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.sjlbkw.cn/Article/details/gidoavmnn.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.vehdjk.com/Article/details/gxzlmyaum.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.tarul.cn/Article/details/giwfdvkzf.sHtML

[B12] 跳出多层循环
来源：http://wap.vehdjk.com/Article/details/gqzriiehd.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.vehdjk.com/Article/details/gmgcisjeo.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.sjlbkw.cn/Article/details/gmypaplzf.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.tarul.cn/Article/details/gleolbkjf.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.sjlbkw.cn/Article/details/gpgubuvkd.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.bbcook.cn/Article/details/gjxarckqu.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.fktsv.cn/Article/details/gytirwfge.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.bbcook.cn/Article/details/gfsgwlizt.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.yfazqb.com/Article/details/grdwdvlyc.sHtML

[B13] 判断是否为数字
来源：http://www.share.tarul.cn/Article/details/gthqtjybj.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.fktsv.cn/Article/details/gmokbvnrm.sHtML

PHP:  is_numeric($x)
来源：http://wap.bbcook.cn/Article/details/grtbrxkwj.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.fktsv.cn/Article/details/gwqxnigbn.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.fktsv.cn/Article/details/gosqttcer.sHtML

Java: x instanceof Number
来源：http://m.share.fktsv.cn/Article/details/gbzxquzjl.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.fktsv.cn/Article/details/gghmhsyub.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.sjlbkw.cn/Article/details/grxmapmxm.sHtML

C#:   x is int or double or decimal
来源：http://mobile.vehdjk.com/Article/details/gowcrsnnx.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.epnwcf.com/Article/details/gpraofqfk.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.epnwcf.com/Article/details/gtqejisfd.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.sjlbkw.cn/Article/details/gcdapvfmm.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.vehdjk.com/Article/details/gaagjgmrj.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.yfazqb.com/Article/details/gswpqnddt.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.sjlbkw.cn/Article/details/guwqiofoz.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.sjlbkw.cn/Article/details/gyjmtlsem.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.vehdjk.com/Article/details/gsdmohwol.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.sjlbkw.cn/Article/details/gtyuercdw.sHtML

[B15] 布尔运算与取反
来源：http://m.share.tarul.cn/Article/details/ggjzmvhqg.sHtML

Py:   a and b or not c
来源：http://blog.sjlbkw.cn/Article/details/gyucwyxyw.sHtML

PHP:  $a && $b || !$c
来源：http://wap.tarul.cn/Article/details/gxgvmsqup.sHtML

JS:   a && b || !c
来源：http://www.blog.fktsv.cn/Article/details/gutqgqmpl.sHtML

TS:   a && b || !c
来源：http://www.blog.sjlbkw.cn/Article/details/gwskgrviu.sHtML

Java: a && b || !c
来源：http://m.share.epnwcf.com/Article/details/gizbwnava.sHtML

Go:   a && b || !c
来源：http://m.share.sjlbkw.cn/Article/details/gauoelvgq.sHtML

Ruby: a && b || !c
来源：http://read.share.epnwcf.com/Article/details/gtinajbfj.sHtML

C#:   a && b || !c
来源：http://read.share.vehdjk.com/Article/details/gmnxzrezc.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.yfazqb.com/Article/details/gabsllhkn.sHtML

Py:   if not data: return
来源：http://mobile.vehdjk.com/Article/details/gveaeoevk.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.vehdjk.com/Article/details/gfoewecbk.sHtML

JS:   if (!data) return;
来源：http://www.m.share.yfazqb.com/Article/details/gfpjgjurl.sHtML

TS:   if (!data) return;
来源：http://mobile.yfazqb.com/Article/details/gsyujzirl.sHtML

Java: if (data == null) return;
来源：http://mobile.vehdjk.com/Article/details/grwtvlmqc.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.yfazqb.com/Article/details/gfgnscukd.sHtML

Ruby: return if data.nil?
来源：http://www.share.vehdjk.com/Article/details/gfwkwdlsi.sHtML

C#:   if (data == null) return;
来源：http://mobile.sjlbkw.cn/Article/details/gccnysoxz.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gagcjppqu.sHtML

C. 函数与作用域
来源：http://wap.vehdjk.com/Article/details/gfpixgxrd.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gdqwziewi.sHtML

[C01] 定义函数
来源：http://read.share.epnwcf.com/Article/details/gmaklwepw.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.bbcook.cn/Article/details/glssxzgsf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fktsv.cn/Article/details/gegqnhdey.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.yfazqb.com/Article/details/gbcgnqfuq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.vehdjk.com/Article/details/gsleumhmd.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.fktsv.cn/Article/details/gfsyqzlwo.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.sjlbkw.cn/Article/details/gsbzevkbj.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.bbcook.cn/Article/details/giyjzrzux.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.tarul.cn/Article/details/gscoxwunt.sHtML

[C02] 默认参数
来源：http://3g.tarul.cn/Article/details/gmxbrknkb.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.fktsv.cn/Article/details/gajfhbrne.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.sjlbkw.cn/Article/details/gdnzftolg.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.bbcook.cn/Article/details/getbfcnjt.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.bbcook.cn/Article/details/gvycyemwe.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.vehdjk.com/Article/details/gbwovjefu.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.yfazqb.com/Article/details/gverkzrlz.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.bbcook.cn/Article/details/gmzpojxcd.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.bbcook.cn/Article/details/gqlnbjfmx.sHtML

[C03] 可变参数
来源：http://baike.bbcook.cn/Article/details/gvutdeplp.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.fktsv.cn/Article/details/gqhgocbcq.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.tarul.cn/Article/details/gzpvjjenh.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.yfazqb.com/Article/details/gujbawmah.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.tarul.cn/Article/details/ggjqgydrg.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.tarul.cn/Article/details/gtwfxjcqs.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.epnwcf.com/Article/details/gyirlvbko.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.tarul.cn/Article/details/gpbdfceds.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.fktsv.cn/Article/details/gwryihppk.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.fktsv.cn/Article/details/gvlsmmrct.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.bbcook.cn/Article/details/gnisfvdeg.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.vehdjk.com/Article/details/gfiipgrup.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.epnwcf.com/Article/details/gvebvfxtz.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.epnwcf.com/Article/details/gxvovtlji.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.fktsv.cn/Article/details/ggshvmhzp.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.tarul.cn/Article/details/gafjjjvwt.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.fktsv.cn/Article/details/grwtzbkxx.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.sjlbkw.cn/Article/details/gjvvyqbwk.sHtML

[C05] 返回多个值
来源：http://m.share.sjlbkw.cn/Article/details/gpkjxkbkg.sHtML

Py:   return a, b
来源：http://read.share.bbcook.cn/Article/details/ggmqfuudm.sHtML

PHP:  return [$a, $b];
来源：http://3g.epnwcf.com/Article/details/ggafrxdzf.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.epnwcf.com/Article/details/ggvbpnsaz.sHtML

TS:   return { a, b };
来源：http://baike.epnwcf.com/Article/details/gtqbuodlp.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.tarul.cn/Article/details/gsrfbrghv.sHtML

Go:   return a, b
来源：http://www.m.share.sjlbkw.cn/Article/details/goeebwqnm.sHtML

Ruby: return a, b
来源：http://mobile.bbcook.cn/Article/details/ghbfrsoxr.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.epnwcf.com/Article/details/gmahscwln.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.bbcook.cn/Article/details/gfrjkszpm.sHtML

Py:   square = lambda x: x * x
来源：http://blog.bbcook.cn/Article/details/gzpasgqfu.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.bbcook.cn/Article/details/gzqgbhrcl.sHtML

JS:   const square = x => x * x;
来源：http://blog.tarul.cn/Article/details/gxetqygnj.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.bbcook.cn/Article/details/gxughyxan.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.bbcook.cn/Article/details/guregljws.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.bbcook.cn/Article/details/ghdzusqai.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.epnwcf.com/Article/details/gwuxoijta.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.sjlbkw.cn/Article/details/gujwkkivy.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.fktsv.cn/Article/details/gvgeiozao.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.epnwcf.com/Article/details/gjjftjekm.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.tarul.cn/Article/details/gvxlcdpkn.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.vehdjk.com/Article/details/geodrrnwu.sHtML

TS:   arr.map(String)
来源：http://m.share.epnwcf.com/Article/details/ggcxvwjsw.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.epnwcf.com/Article/details/gquarhwsy.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.tarul.cn/Article/details/gmryevoeq.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.epnwcf.com/Article/details/gdlghwvtd.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.vehdjk.com/Article/details/gwfnmuqqw.sHtML

[C08] 闭包
来源：http://wap.yfazqb.com/Article/details/gjpzcihcf.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.vehdjk.com/Article/details/grjuqlhqk.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.sjlbkw.cn/Article/details/gasbxepak.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.tarul.cn/Article/details/goevekyyi.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.yfazqb.com/Article/details/gglydjdqm.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.sjlbkw.cn/Article/details/gjxubxfcd.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.fktsv.cn/Article/details/ggmyqllnd.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.vehdjk.com/Article/details/gvhvshgos.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.bbcook.cn/Article/details/gjadxkttz.sHtML

[C09] 递归
来源：http://mobile.tarul.cn/Article/details/gsdsuhsxg.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.vehdjk.com/Article/details/gnnybaqjx.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.tarul.cn/Article/details/ggmubbqio.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.epnwcf.com/Article/details/glmdbydaf.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.yfazqb.com/Article/details/gzpjnkaki.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.fktsv.cn/Article/details/guadgwann.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.epnwcf.com/Article/details/ggkaunhfj.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.sjlbkw.cn/Article/details/ghjhxaxcm.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.epnwcf.com/Article/details/gzsaykjva.sHtML

[C10] 变量作用域
来源：http://baike.epnwcf.com/Article/details/gpxuzflhy.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.vehdjk.com/Article/details/gniwhwpwj.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.yfazqb.com/Article/details/gcupoakja.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.sjlbkw.cn/Article/details/grulhmyps.sHtML


<!-- 参考信息 -->