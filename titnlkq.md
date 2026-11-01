代发 wailian999

[A18] 字符与 ASCII 码互转
来源：http://www.share.yfazqb.com/Article/details/gnlydrazl.sHtML

Py:   ord("A"); chr(65)
来源：http://mobile.yfazqb.com/Article/details/gyhyfjchg.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.blog.sjlbkw.cn/Article/details/gdmnhnxlu.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://read.share.vehdjk.com/Article/details/gtuiubrkn.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.vehdjk.com/Article/details/gxedrolfw.sHtML

Java: (int) 'A'; (char) 65
来源：http://blog.bbcook.cn/Article/details/gptjzbghm.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://read.share.sjlbkw.cn/Article/details/gxifejheq.sHtML

Ruby: "A".ord; 65.chr
来源：http://blog.bbcook.cn/Article/details/grzzdezpf.sHtML

C#:   (int)'A'; (char)65
来源：http://www.share.tarul.cn/Article/details/gcucgtrdd.sHtML

[A19] 交换两个变量
来源：http://m.share.sjlbkw.cn/Article/details/griacwnfp.sHtML

Py:   a, b = b, a
来源：http://m.share.bbcook.cn/Article/details/gzlpuypkc.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://m.share.yfazqb.com/Article/details/gajatkgca.sHtML

JS:   [a, b] = [b, a];
来源：http://blog.tarul.cn/Article/details/gxvpqcmmz.sHtML

TS:   [a, b] = [b, a];
来源：http://www.m.share.tarul.cn/Article/details/guaqnlzbz.sHtML

Java: int t = a; a = b; b = t;
来源：http://3g.yfazqb.com/Article/details/ghqdbetbp.sHtML

Go:   a, b = b, a
来源：http://read.share.yfazqb.com/Article/details/gosrayvph.sHtML

Ruby: a, b = b, a
来源：http://www.m.share.vehdjk.com/Article/details/girzctalm.sHtML

C#:   (a, b) = (b, a);
来源：http://m.share.vehdjk.com/Article/details/ggxhbfwxa.sHtML

[A20] 读取标准输入
来源：http://blog.tarul.cn/Article/details/gwmvuwbsv.sHtML

Py:   name = input("请输入：")
来源：http://blog.bbcook.cn/Article/details/gjqdqrdon.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://baike.fktsv.cn/Article/details/ghuqdncmu.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wap.epnwcf.com/Article/details/gbaopbfti.sHtML

TS:   // Node.js：readline 模块
来源：http://www.share.tarul.cn/Article/details/gvjvbzmab.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.blog.bbcook.cn/Article/details/gjaeizata.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://mobile.tarul.cn/Article/details/gygbjgeow.sHtML

Ruby: gets.chomp
来源：http://read.share.tarul.cn/Article/details/gvvvsdetu.sHtML

C#:   Console.ReadLine();
来源：http://mobile.tarul.cn/Article/details/gyrocvfdx.sHtML

[A21] 保留指定小数位输出
来源：http://mobile.epnwcf.com/Article/details/gmadlacvr.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.m.share.tarul.cn/Article/details/gectennuv.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wap.bbcook.cn/Article/details/gfpgzjiqs.sHtML

JS:   (3.14159).toFixed(2)
来源：http://3g.sjlbkw.cn/Article/details/gvmgfkpvv.sHtML

TS:   (3.14159).toFixed(2)
来源：http://read.share.tarul.cn/Article/details/gilujokgb.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://wap.fktsv.cn/Article/details/gjkuhugtm.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://mobile.epnwcf.com/Article/details/garbkuphy.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://blog.vehdjk.com/Article/details/glgghkwcq.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.m.share.sjlbkw.cn/Article/details/gjjbofvlg.sHtML

[A22] 获取字符串长度
来源：http://blog.vehdjk.com/Article/details/gclneqleq.sHtML

Py:   len(s)
来源：http://wap.sjlbkw.cn/Article/details/gxaqyxfxm.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://m.share.tarul.cn/Article/details/gznudidiu.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mobile.vehdjk.com/Article/details/gbauqqmeo.sHtML

TS:   s.length
来源：http://blog.bbcook.cn/Article/details/gocpgcoih.sHtML

Java: s.length()
来源：http://wap.epnwcf.com/Article/details/ggamenyrj.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://blog.fktsv.cn/Article/details/gcweeqfej.sHtML

Ruby: s.length
来源：http://www.share.tarul.cn/Article/details/gkxjuulwz.sHtML

C#:   s.Length
来源：http://wap.yfazqb.com/Article/details/gkjhhchqd.sHtML

[A23] 大小写转换
来源：http://www.share.yfazqb.com/Article/details/gwiuwifos.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://mobile.tarul.cn/Article/details/gdmgkutxc.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.m.share.yfazqb.com/Article/details/grahzashh.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.vehdjk.com/Article/details/gfbcslibu.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.sjlbkw.cn/Article/details/gruuzpsnt.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://baike.bbcook.cn/Article/details/gcbboyxbc.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wap.sjlbkw.cn/Article/details/gsvmzqtgd.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.m.share.yfazqb.com/Article/details/gegautmut.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://m.share.bbcook.cn/Article/details/gkpeoilry.sHtML

[A24] 去除首尾空白
来源：http://3g.bbcook.cn/Article/details/gjryamqnj.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.share.sjlbkw.cn/Article/details/gayvgnbpo.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wap.epnwcf.com/Article/details/gnktphgjr.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.vehdjk.com/Article/details/glvkbpdth.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.fktsv.cn/Article/details/gkqhhaako.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://read.share.fktsv.cn/Article/details/gdpzwrgdk.sHtML

Go:   strings.TrimSpace(s)
来源：http://m.share.yfazqb.com/Article/details/gaejgggnu.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wap.fktsv.cn/Article/details/gevfvykhv.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.blog.fktsv.cn/Article/details/gpmaealag.sHtML

[A25] 字符串比较
来源：http://wap.bbcook.cn/Article/details/gbakkafpt.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.blog.tarul.cn/Article/details/ghqauqbkc.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mobile.fktsv.cn/Article/details/goxqkxqtn.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.bbcook.cn/Article/details/gjtrsotxb.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.bbcook.cn/Article/details/gqvisiboe.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.m.share.tarul.cn/Article/details/gnlgblpzx.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://baike.yfazqb.com/Article/details/gblrackjl.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://m.share.sjlbkw.cn/Article/details/gcggkddsx.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://read.share.tarul.cn/Article/details/gtacjobcp.sHtML

[A26] 类型转换总览
来源：http://www.m.share.tarul.cn/Article/details/ggregsnwy.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.blog.yfazqb.com/Article/details/gjsjwdsnt.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wap.tarul.cn/Article/details/gfjzyujcv.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://m.share.bbcook.cn/Article/details/gyhjmtmuy.sHtML

TS:   Number() String() Boolean() x as number
来源：http://3g.epnwcf.com/Article/details/gzswyloql.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://m.share.bbcook.cn/Article/details/givpakvec.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://3g.bbcook.cn/Article/details/gfxpqdaax.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://read.share.vehdjk.com/Article/details/gjytdsnfe.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.m.share.bbcook.cn/Article/details/guolwkhzs.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/ggywwpayj.sHtML

B. 流程控制
来源：http://read.share.bbcook.cn/Article/details/gwrinuoyw.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gbjvvnolw.sHtML

[B01] 条件判断 if / else
来源：http://m.share.tarul.cn/Article/details/gsjbabwig.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://m.share.sjlbkw.cn/Article/details/ghqlpzjvb.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.m.share.fktsv.cn/Article/details/gpatiijfd.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.bbcook.cn/Article/details/giciwevut.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.fktsv.cn/Article/details/gfkpjzeta.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.m.share.yfazqb.com/Article/details/gxxaeqxck.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mobile.yfazqb.com/Article/details/griswzprl.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://m.share.epnwcf.com/Article/details/geuwtosfo.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.blog.vehdjk.com/Article/details/gbbgzutxu.sHtML

[B02] 多分支 else if / elif
来源：http://read.share.epnwcf.com/Article/details/gwddhlhif.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://blog.epnwcf.com/Article/details/ggvyutjtt.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://read.share.bbcook.cn/Article/details/ggwoyoewh.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.bbcook.cn/Article/details/gqxdnnemp.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.vehdjk.com/Article/details/gcwkfljdr.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.epnwcf.com/Article/details/gvlffwfcv.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wap.bbcook.cn/Article/details/glztnghfb.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.m.share.tarul.cn/Article/details/glqpwnwjf.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.bbcook.cn/Article/details/gdbeyvuhy.sHtML

[B03] switch / match / case
来源：http://3g.bbcook.cn/Article/details/gaumfdvbf.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wap.vehdjk.com/Article/details/gyhnrjled.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://3g.epnwcf.com/Article/details/gbiygubzb.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.yfazqb.com/Article/details/gvnqdadqj.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.yfazqb.com/Article/details/gzwbscmdh.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.tarul.cn/Article/details/gkagpaxqj.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.blog.fktsv.cn/Article/details/gjfsyqsgh.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://baike.vehdjk.com/Article/details/glwbdfnue.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.share.yfazqb.com/Article/details/gyzfbllry.sHtML

[B04] for 计数循环
来源：http://baike.yfazqb.com/Article/details/gnzusbmip.sHtML

Py:   for i in range(10): print(i)
来源：http://www.m.share.sjlbkw.cn/Article/details/gaqkmhfpc.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.share.yfazqb.com/Article/details/gsxtkdvjv.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.bbcook.cn/Article/details/glghyonnp.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.epnwcf.com/Article/details/goqrjlhnr.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.bbcook.cn/Article/details/gbgwlspyn.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.m.share.tarul.cn/Article/details/glvpyieyv.sHtML

Ruby: 10.times { |i| puts i }
来源：http://m.share.epnwcf.com/Article/details/gejiqbttr.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://blog.tarul.cn/Article/details/geuoubygq.sHtML

[B05] 遍历数组 / 列表
来源：http://3g.fktsv.cn/Article/details/gpphxadww.sHtML

Py:   for item in arr: print(item)
来源：http://www.share.tarul.cn/Article/details/ggxuatbyc.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.fktsv.cn/Article/details/gkuesoknv.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.share.tarul.cn/Article/details/gtuerkxpq.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://blog.vehdjk.com/Article/details/geowlhvpq.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.share.epnwcf.com/Article/details/gsokoktft.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.fktsv.cn/Article/details/gbuhfvzii.sHtML

Ruby: arr.each { |item| puts item }
来源：http://baike.epnwcf.com/Article/details/gvofejbnu.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://blog.fktsv.cn/Article/details/gahvexhiw.sHtML

[B06] 遍历字典 / 对象
来源：http://www.share.epnwcf.com/Article/details/geblthpop.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://3g.fktsv.cn/Article/details/gvgkmmuvx.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.share.fktsv.cn/Article/details/gdvbzqawq.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.yfazqb.com/Article/details/gdrugxekp.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.tarul.cn/Article/details/ghxpsxlde.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.fktsv.cn/Article/details/gygajaxoo.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.vehdjk.com/Article/details/grgiuadis.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.blog.fktsv.cn/Article/details/gzkpzimnz.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://read.share.vehdjk.com/Article/details/ghwwgaxcg.sHtML

[B07] while 循环
来源：http://wap.fktsv.cn/Article/details/gswuwcngd.sHtML

Py:   while i < 10: i += 1
来源：http://3g.sjlbkw.cn/Article/details/gvkecddir.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.share.vehdjk.com/Article/details/gvlvmhgyp.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.share.epnwcf.com/Article/details/gpocqnyjg.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.blog.vehdjk.com/Article/details/gtfvywjgt.sHtML

Java: while (i < 10) { i++; }
来源：http://www.blog.epnwcf.com/Article/details/gkzaukbua.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.tarul.cn/Article/details/gmtjoaoaq.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.yfazqb.com/Article/details/gtsrwenbd.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.epnwcf.com/Article/details/guezpsnom.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.vehdjk.com/Article/details/gqenrpkhg.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.epnwcf.com/Article/details/gxmabwvbt.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.sjlbkw.cn/Article/details/gcowzxqkv.sHtML

JS:   do { i++; } while (i < 10);
来源：http://m.share.vehdjk.com/Article/details/gnqbzhadv.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.tarul.cn/Article/details/gdhtaxoav.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.yfazqb.com/Article/details/gkmehskhu.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.epnwcf.com/Article/details/gredhphvm.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.vehdjk.com/Article/details/gpvtkchqc.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.bbcook.cn/Article/details/grjcwxrsp.sHtML

[B09] break 与 continue
来源：http://www.share.sjlbkw.cn/Article/details/grlgsgkjx.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.tarul.cn/Article/details/gpkeisbhv.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.epnwcf.com/Article/details/gisdlsdnk.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.yfazqb.com/Article/details/gjudsotsk.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.vehdjk.com/Article/details/gdqqnuapq.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.yfazqb.com/Article/details/gtyjqgwjd.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.vehdjk.com/Article/details/gtdvtkjgk.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.epnwcf.com/Article/details/giehbtqoi.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.yfazqb.com/Article/details/ggumgeqod.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.epnwcf.com/Article/details/garhhaygh.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.fktsv.cn/Article/details/gdyutrkho.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.bbcook.cn/Article/details/gsqyaugzd.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.sjlbkw.cn/Article/details/gmjmcihhf.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.yfazqb.com/Article/details/gcmvbmwby.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.vehdjk.com/Article/details/gfmrjdccy.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.yfazqb.com/Article/details/gjbnydvrh.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.vehdjk.com/Article/details/gogtwrzxs.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.tarul.cn/Article/details/gsunugnhz.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.tarul.cn/Article/details/graokexwh.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.bbcook.cn/Article/details/ggkxpdhac.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.vehdjk.com/Article/details/gzbgvamew.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.sjlbkw.cn/Article/details/gujwjvvcg.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.yfazqb.com/Article/details/gifbhzsxx.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.epnwcf.com/Article/details/gyvjdrutm.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.fktsv.cn/Article/details/gqxanzgef.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.fktsv.cn/Article/details/gzcazjibk.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.fktsv.cn/Article/details/gcoizfanf.sHtML

[B12] 跳出多层循环
来源：http://www.share.yfazqb.com/Article/details/gmtkpqypz.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.sjlbkw.cn/Article/details/gkyctdgyl.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.epnwcf.com/Article/details/gerahykjc.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.epnwcf.com/Article/details/gryzosumt.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.tarul.cn/Article/details/ggeiuximk.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.fktsv.cn/Article/details/ggszyddrs.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.yfazqb.com/Article/details/glozzytoq.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.yfazqb.com/Article/details/gbadkzzoz.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.epnwcf.com/Article/details/guunbqupc.sHtML

[B13] 判断是否为数字
来源：http://wap.tarul.cn/Article/details/gpperfkeh.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.epnwcf.com/Article/details/gntsvdvrf.sHtML

PHP:  is_numeric($x)
来源：http://mobile.vehdjk.com/Article/details/gmwejairz.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.sjlbkw.cn/Article/details/gqabqlrhm.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.tarul.cn/Article/details/gybkxrdrw.sHtML

Java: x instanceof Number
来源：http://www.share.bbcook.cn/Article/details/gsoezgetk.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.vehdjk.com/Article/details/ghrrxjccr.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.fktsv.cn/Article/details/gfrvxjsuh.sHtML

C#:   x is int or double or decimal
来源：http://www.share.yfazqb.com/Article/details/gydyxnstr.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.yfazqb.com/Article/details/gwbcbfzob.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.vehdjk.com/Article/details/grbtqrtms.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.fktsv.cn/Article/details/gffurpnxy.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.vehdjk.com/Article/details/gxwzcirfl.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.tarul.cn/Article/details/gaaxvrwbw.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.tarul.cn/Article/details/gzegggpvd.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.tarul.cn/Article/details/glnzoylbq.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.sjlbkw.cn/Article/details/gpcmlroxz.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.vehdjk.com/Article/details/gfaieezsg.sHtML

[B15] 布尔运算与取反
来源：http://mobile.yfazqb.com/Article/details/goijpzega.sHtML

Py:   a and b or not c
来源：http://wap.vehdjk.com/Article/details/gfugihtro.sHtML

PHP:  $a && $b || !$c
来源：http://wap.tarul.cn/Article/details/gwngxkrnq.sHtML

JS:   a && b || !c
来源：http://read.share.fktsv.cn/Article/details/gexqzrlod.sHtML

TS:   a && b || !c
来源：http://www.share.tarul.cn/Article/details/grgqrvgbp.sHtML

Java: a && b || !c
来源：http://www.share.tarul.cn/Article/details/gamhozcbw.sHtML

Go:   a && b || !c
来源：http://www.m.share.bbcook.cn/Article/details/gebilcnjp.sHtML

Ruby: a && b || !c
来源：http://mobile.sjlbkw.cn/Article/details/goffawzrh.sHtML

C#:   a && b || !c
来源：http://wap.bbcook.cn/Article/details/ggyqyrcdd.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.tarul.cn/Article/details/gmeadifjj.sHtML

Py:   if not data: return
来源：http://3g.epnwcf.com/Article/details/gfbsxeaov.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.epnwcf.com/Article/details/ggfjmxgvo.sHtML

JS:   if (!data) return;
来源：http://www.m.share.epnwcf.com/Article/details/gxiznsvec.sHtML

TS:   if (!data) return;
来源：http://www.m.share.epnwcf.com/Article/details/gegfijoxc.sHtML

Java: if (data == null) return;
来源：http://baike.sjlbkw.cn/Article/details/gxibbrosr.sHtML

Go:   if data == nil { return }
来源：http://baike.bbcook.cn/Article/details/ggfbuacyu.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.fktsv.cn/Article/details/gjnamgmlb.sHtML

C#:   if (data == null) return;
来源：http://m.share.bbcook.cn/Article/details/gmtzfgzdf.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gqwgqgvwy.sHtML

C. 函数与作用域
来源：http://mobile.tarul.cn/Article/details/gliiojhhx.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/ghngjswlw.sHtML

[C01] 定义函数
来源：http://blog.vehdjk.com/Article/details/gkvrpdyie.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.vehdjk.com/Article/details/gysmunzsa.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.epnwcf.com/Article/details/gwvlnxzzl.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.bbcook.cn/Article/details/gvadnoofp.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.fktsv.cn/Article/details/ggkudrecu.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.vehdjk.com/Article/details/gjfvmzdcc.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.fktsv.cn/Article/details/gwhojaswq.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.fktsv.cn/Article/details/gmzbrpkav.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.vehdjk.com/Article/details/gnzskajga.sHtML

[C02] 默认参数
来源：http://baike.vehdjk.com/Article/details/gzecyjedv.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.tarul.cn/Article/details/gvxoauutu.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.fktsv.cn/Article/details/gvrxcbbyx.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.sjlbkw.cn/Article/details/gndyqfczk.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.vehdjk.com/Article/details/gpzzvruew.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.epnwcf.com/Article/details/gvwyyayzg.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.tarul.cn/Article/details/gvhmvarfk.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.epnwcf.com/Article/details/gjmxfvvpe.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.tarul.cn/Article/details/gsykrymgo.sHtML

[C03] 可变参数
来源：http://read.share.fktsv.cn/Article/details/gkxbkokcf.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.fktsv.cn/Article/details/gsaptypfx.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.sjlbkw.cn/Article/details/gwbcpanqt.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.tarul.cn/Article/details/gtxhllzfx.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.fktsv.cn/Article/details/gkyhvjbkl.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.epnwcf.com/Article/details/gqkgvsfay.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.sjlbkw.cn/Article/details/gwihvrdhk.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.fktsv.cn/Article/details/gksjtnecp.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.tarul.cn/Article/details/gpdnbnglx.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.fktsv.cn/Article/details/ggypcyfph.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.epnwcf.com/Article/details/gfivgpaaw.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.epnwcf.com/Article/details/gkkteeicb.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.sjlbkw.cn/Article/details/gckdwtmta.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.bbcook.cn/Article/details/ghisomykv.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.tarul.cn/Article/details/gboierybd.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.bbcook.cn/Article/details/gonwdeyks.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghtgikfhy.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.epnwcf.com/Article/details/gpvolqtgf.sHtML

[C05] 返回多个值
来源：http://wap.sjlbkw.cn/Article/details/gszcgevpb.sHtML

Py:   return a, b
来源：http://read.share.tarul.cn/Article/details/gvurngdmw.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.vehdjk.com/Article/details/gsgtdhxbb.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.bbcook.cn/Article/details/gjvixxdyx.sHtML

TS:   return { a, b };
来源：http://read.share.yfazqb.com/Article/details/gdtfanmmx.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.sjlbkw.cn/Article/details/ggnylvbke.sHtML

Go:   return a, b
来源：http://www.share.yfazqb.com/Article/details/goaoefpdm.sHtML

Ruby: return a, b
来源：http://www.blog.vehdjk.com/Article/details/gwbjerlsi.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.sjlbkw.cn/Article/details/gkjjlixyw.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.sjlbkw.cn/Article/details/gtzdkdqch.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.bbcook.cn/Article/details/gspyemgjq.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.sjlbkw.cn/Article/details/gxotquyon.sHtML

JS:   const square = x => x * x;
来源：http://mobile.epnwcf.com/Article/details/gyzzgelrn.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.yfazqb.com/Article/details/gdbdngbue.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.vehdjk.com/Article/details/gawqsiuxm.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.epnwcf.com/Article/details/gbtqsvvzp.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.sjlbkw.cn/Article/details/gvjjkepbx.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.sjlbkw.cn/Article/details/gbbbpmasx.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.fktsv.cn/Article/details/gnbcczmxn.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.yfazqb.com/Article/details/gdjptwqps.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.epnwcf.com/Article/details/gmytnkezy.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.tarul.cn/Article/details/gtkuubdjh.sHtML

TS:   arr.map(String)
来源：http://mobile.tarul.cn/Article/details/gmyntcylo.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.tarul.cn/Article/details/gliivuywc.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.bbcook.cn/Article/details/geklnvnqx.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.fktsv.cn/Article/details/gexrpqbbs.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.tarul.cn/Article/details/glltmuxsi.sHtML

[C08] 闭包
来源：http://www.blog.tarul.cn/Article/details/gchfibbgu.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.epnwcf.com/Article/details/gqkngkefv.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.epnwcf.com/Article/details/gjlhbcbmc.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.tarul.cn/Article/details/gpnodygsl.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.fktsv.cn/Article/details/gjbunrtyr.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.sjlbkw.cn/Article/details/gioxqmyzq.sHtML


<!-- 参考信息 -->