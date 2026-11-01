代发 wailian999

PHP:  $name = trim(fgets(STDIN));
来源：http://mobile.sjlbkw.cn/Article/details/gkpiuzntu.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://read.share.yfazqb.com/Article/details/gdpzuwugy.sHtML

TS:   // Node.js：readline 模块
来源：http://read.share.tarul.cn/Article/details/ggawzsoxa.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://read.share.vehdjk.com/Article/details/gelcbtfjq.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://blog.tarul.cn/Article/details/gjywlrwxr.sHtML

Ruby: gets.chomp
来源：http://wap.sjlbkw.cn/Article/details/gxpijxumh.sHtML

C#:   Console.ReadLine();
来源：http://blog.bbcook.cn/Article/details/gtfyhmnld.sHtML

[A21] 保留指定小数位输出
来源：http://m.share.epnwcf.com/Article/details/gnixtwnrc.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.share.yfazqb.com/Article/details/govchumxb.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://baike.sjlbkw.cn/Article/details/gkvjkqbvk.sHtML

JS:   (3.14159).toFixed(2)
来源：http://mobile.epnwcf.com/Article/details/gckutywkz.sHtML

TS:   (3.14159).toFixed(2)
来源：http://mobile.bbcook.cn/Article/details/gqjloofaw.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.share.bbcook.cn/Article/details/glntprxkj.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wap.bbcook.cn/Article/details/gqazhwwby.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://3g.sjlbkw.cn/Article/details/gwkorehtq.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.m.share.tarul.cn/Article/details/gwhrklrpk.sHtML

[A22] 获取字符串长度
来源：http://www.share.epnwcf.com/Article/details/gnmgqnrje.sHtML

Py:   len(s)
来源：http://www.share.fktsv.cn/Article/details/gbxcvqssz.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.share.sjlbkw.cn/Article/details/gflclfnnw.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.share.sjlbkw.cn/Article/details/gtdjlphhp.sHtML

TS:   s.length
来源：http://blog.epnwcf.com/Article/details/ggvrcoija.sHtML

Java: s.length()
来源：http://mobile.epnwcf.com/Article/details/golpubzln.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.m.share.bbcook.cn/Article/details/gssnsvnml.sHtML

Ruby: s.length
来源：http://m.share.tarul.cn/Article/details/ghucilere.sHtML

C#:   s.Length
来源：http://3g.epnwcf.com/Article/details/gjmktfomo.sHtML

[A23] 大小写转换
来源：http://m.share.epnwcf.com/Article/details/gbhcivkgy.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://baike.tarul.cn/Article/details/gpdeyvrbp.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://read.share.yfazqb.com/Article/details/gbjcjnprw.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.epnwcf.com/Article/details/grengqwuv.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.epnwcf.com/Article/details/gvthftsvf.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wap.vehdjk.com/Article/details/gccfafqns.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wap.fktsv.cn/Article/details/gnocimrfc.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mobile.tarul.cn/Article/details/ghhsqcosn.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://m.share.tarul.cn/Article/details/gcanbtjin.sHtML

[A24] 去除首尾空白
来源：http://3g.sjlbkw.cn/Article/details/gqbiptwoa.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://read.share.yfazqb.com/Article/details/gzdclcvmm.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.m.share.yfazqb.com/Article/details/gnsrzhdwa.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.tarul.cn/Article/details/gickikbsl.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.sjlbkw.cn/Article/details/gdozsuphn.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.blog.sjlbkw.cn/Article/details/gziowyfwo.sHtML

Go:   strings.TrimSpace(s)
来源：http://m.share.sjlbkw.cn/Article/details/gkikxyrpt.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.m.share.vehdjk.com/Article/details/ggcgawmex.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://read.share.epnwcf.com/Article/details/gxapxupno.sHtML

[A25] 字符串比较
来源：http://3g.tarul.cn/Article/details/goxvoahum.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.m.share.epnwcf.com/Article/details/glwormrks.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.share.sjlbkw.cn/Article/details/gbodnulfd.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.bbcook.cn/Article/details/gxnbnvysd.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.yfazqb.com/Article/details/gdgjbaiwf.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.m.share.vehdjk.com/Article/details/gednppvqv.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.blog.epnwcf.com/Article/details/glzqizwxq.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.share.sjlbkw.cn/Article/details/gjqnespru.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wap.bbcook.cn/Article/details/gezaumgkj.sHtML

[A26] 类型转换总览
来源：http://read.share.epnwcf.com/Article/details/gaqdiivrg.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.m.share.epnwcf.com/Article/details/gjpicefkg.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.share.yfazqb.com/Article/details/gjhyunopb.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mobile.tarul.cn/Article/details/gdgetqjvu.sHtML

TS:   Number() String() Boolean() x as number
来源：http://3g.tarul.cn/Article/details/gzgisbxhb.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://blog.tarul.cn/Article/details/gkouzjxlh.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://m.share.sjlbkw.cn/Article/details/gqisojnvo.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.m.share.vehdjk.com/Article/details/gfouxasmd.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mobile.fktsv.cn/Article/details/goaghzuvx.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gstqeysya.sHtML

B. 流程控制
来源：http://www.m.share.vehdjk.com/Article/details/gsrltnvsk.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gbpxkfbia.sHtML

[B01] 条件判断 if / else
来源：http://wap.yfazqb.com/Article/details/gcerlswkp.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://mobile.vehdjk.com/Article/details/gtvsqpqwh.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://blog.epnwcf.com/Article/details/gyyuhfjjp.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.fktsv.cn/Article/details/gqcasrhkn.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.yfazqb.com/Article/details/gvyddnjdb.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://3g.yfazqb.com/Article/details/gwjgrbzvn.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://m.share.sjlbkw.cn/Article/details/gmtjuzrlc.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://read.share.bbcook.cn/Article/details/gpjwmxjab.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.blog.fktsv.cn/Article/details/glnjmoglk.sHtML

[B02] 多分支 else if / elif
来源：http://wap.yfazqb.com/Article/details/gjbgemebi.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mobile.sjlbkw.cn/Article/details/ggepgpqyt.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.blog.fktsv.cn/Article/details/gnxhksrfd.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.sjlbkw.cn/Article/details/gxminsjdf.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.fktsv.cn/Article/details/gdaovgvds.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.tarul.cn/Article/details/gafimywrm.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.blog.epnwcf.com/Article/details/gfcqpoyfq.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://m.share.fktsv.cn/Article/details/gbqdaujys.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.vehdjk.com/Article/details/glkrzkwyq.sHtML

[B03] switch / match / case
来源：http://baike.sjlbkw.cn/Article/details/gzjnapctq.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://3g.tarul.cn/Article/details/gtqsrskxr.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.share.tarul.cn/Article/details/gnxywzqyr.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.vehdjk.com/Article/details/gvmryzoxs.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.yfazqb.com/Article/details/gubadwisf.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://blog.vehdjk.com/Article/details/gdezsacde.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wap.yfazqb.com/Article/details/gztmgrfbm.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://read.share.sjlbkw.cn/Article/details/gtxsuwyye.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://baike.sjlbkw.cn/Article/details/gpkvavsvo.sHtML

[B04] for 计数循环
来源：http://mobile.yfazqb.com/Article/details/gjidtgwrd.sHtML

Py:   for i in range(10): print(i)
来源：http://www.share.sjlbkw.cn/Article/details/gewgzzjlf.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.m.share.yfazqb.com/Article/details/giaxrczkr.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.sjlbkw.cn/Article/details/gxsdqwefd.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.yfazqb.com/Article/details/gpzpytxqm.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mobile.tarul.cn/Article/details/gicecwaas.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mobile.bbcook.cn/Article/details/gfuoztdei.sHtML

Ruby: 10.times { |i| puts i }
来源：http://mobile.bbcook.cn/Article/details/gevmuzysx.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.yfazqb.com/Article/details/gjyaxbfcr.sHtML

[B05] 遍历数组 / 列表
来源：http://wap.tarul.cn/Article/details/gufmsyufj.sHtML

Py:   for item in arr: print(item)
来源：http://www.blog.yfazqb.com/Article/details/gjwbnduyf.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.tarul.cn/Article/details/gxqgqzhnl.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://3g.vehdjk.com/Article/details/gpaklpszh.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://blog.epnwcf.com/Article/details/gfvwjvsqt.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://3g.bbcook.cn/Article/details/gukgihqgm.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wap.sjlbkw.cn/Article/details/gqhezdqkz.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.share.fktsv.cn/Article/details/gtjdqkckc.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mobile.bbcook.cn/Article/details/gwfuwxrnb.sHtML

[B06] 遍历字典 / 对象
来源：http://mobile.yfazqb.com/Article/details/grbguddmb.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.vehdjk.com/Article/details/ggmcfosjs.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.vehdjk.com/Article/details/gdiypgglk.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.epnwcf.com/Article/details/gkmyevfuz.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.bbcook.cn/Article/details/gvnlepbyw.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.bbcook.cn/Article/details/giecjhved.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mobile.fktsv.cn/Article/details/gvegasmdb.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.blog.yfazqb.com/Article/details/gkqyloqqb.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mobile.bbcook.cn/Article/details/ghqtmftsr.sHtML

[B07] while 循环
来源：http://mobile.yfazqb.com/Article/details/gkzwkxafn.sHtML

Py:   while i < 10: i += 1
来源：http://mobile.tarul.cn/Article/details/grkorjsbt.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://m.share.epnwcf.com/Article/details/gzgqkzdbt.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.bbcook.cn/Article/details/gsqkvcsib.sHtML

TS:   while (i < 10) { i++; }
来源：http://read.share.fktsv.cn/Article/details/gsfckaenx.sHtML

Java: while (i < 10) { i++; }
来源：http://mobile.vehdjk.com/Article/details/gjxqejlkq.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.vehdjk.com/Article/details/geewanlgj.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.blog.sjlbkw.cn/Article/details/ghwtlvgkr.sHtML

C#:   while (i < 10) { i++; }
来源：http://m.share.fktsv.cn/Article/details/ggunnoyce.sHtML

[B08] do-while（至少执行一次）
来源：http://wap.epnwcf.com/Article/details/gfrcjdkmv.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://read.share.yfazqb.com/Article/details/gfcqjoybo.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.epnwcf.com/Article/details/gvspywkyp.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.vehdjk.com/Article/details/gemmnttwm.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.vehdjk.com/Article/details/grqrdfjty.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.fktsv.cn/Article/details/grastpwvt.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.fktsv.cn/Article/details/gjxqxtykk.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.bbcook.cn/Article/details/gtmuzcppb.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.sjlbkw.cn/Article/details/gqdiwllmz.sHtML

[B09] break 与 continue
来源：http://www.share.bbcook.cn/Article/details/gnuhwygdl.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.vehdjk.com/Article/details/graabeifs.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.epnwcf.com/Article/details/gtfglbhrd.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.yfazqb.com/Article/details/gwyzkjumq.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.tarul.cn/Article/details/gpbgwtinz.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.vehdjk.com/Article/details/grwlrbwgi.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.vehdjk.com/Article/details/gwctzrznb.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.tarul.cn/Article/details/gxvxyvwkq.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.vehdjk.com/Article/details/ggvngwkhj.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.fktsv.cn/Article/details/glmhlryzd.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.yfazqb.com/Article/details/gyqgrrfim.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.epnwcf.com/Article/details/gblpondso.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.sjlbkw.cn/Article/details/gpkqnlmqs.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.fktsv.cn/Article/details/gcwsxague.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.epnwcf.com/Article/details/gycchaxsd.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.vehdjk.com/Article/details/gsjnlobmf.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mobile.fktsv.cn/Article/details/gzknbmbeh.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.bbcook.cn/Article/details/goboanmwl.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.bbcook.cn/Article/details/gyurcssnx.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.fktsv.cn/Article/details/gdefafglc.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.epnwcf.com/Article/details/gyazjvhxj.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.vehdjk.com/Article/details/gwiaskeiu.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.yfazqb.com/Article/details/gylonfiay.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.tarul.cn/Article/details/gdamlurom.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.vehdjk.com/Article/details/glkuavbvr.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.tarul.cn/Article/details/gxwxyerhs.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.fktsv.cn/Article/details/gqlzabili.sHtML

[B12] 跳出多层循环
来源：http://wap.yfazqb.com/Article/details/gfabjrzzf.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.yfazqb.com/Article/details/gihqufssv.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.bbcook.cn/Article/details/gcxetviaa.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.vehdjk.com/Article/details/gkmjffeaf.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fktsv.cn/Article/details/gbxqpwzgc.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.epnwcf.com/Article/details/gzsyqgceh.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.epnwcf.com/Article/details/gqatzwdti.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.tarul.cn/Article/details/gzynbgwmd.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.tarul.cn/Article/details/gqkzhhonj.sHtML

[B13] 判断是否为数字
来源：http://www.share.epnwcf.com/Article/details/gbjxubxmz.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.fktsv.cn/Article/details/ghtouicdr.sHtML

PHP:  is_numeric($x)
来源：http://m.share.epnwcf.com/Article/details/gkbaawmri.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.yfazqb.com/Article/details/gkrepdrvz.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.fktsv.cn/Article/details/gugrlqmqe.sHtML

Java: x instanceof Number
来源：http://m.share.sjlbkw.cn/Article/details/gaadjxvxf.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.tarul.cn/Article/details/gkxshpajp.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.fktsv.cn/Article/details/gjqtgqvyf.sHtML

C#:   x is int or double or decimal
来源：http://m.share.bbcook.cn/Article/details/gxgppkwtr.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.bbcook.cn/Article/details/gwzixhnbx.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.sjlbkw.cn/Article/details/glrllvftp.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.sjlbkw.cn/Article/details/glzrtcbca.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.tarul.cn/Article/details/gpkasrbhy.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.bbcook.cn/Article/details/geomwrefo.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.epnwcf.com/Article/details/gswchofue.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.fktsv.cn/Article/details/gfxlosyzr.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.sjlbkw.cn/Article/details/gkdebzjzf.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.vehdjk.com/Article/details/ghffvxqpe.sHtML

[B15] 布尔运算与取反
来源：http://mobile.tarul.cn/Article/details/gsnhqghyi.sHtML

Py:   a and b or not c
来源：http://m.share.bbcook.cn/Article/details/gngswhnfp.sHtML

PHP:  $a && $b || !$c
来源：http://baike.bbcook.cn/Article/details/gjgnarbaa.sHtML

JS:   a && b || !c
来源：http://blog.yfazqb.com/Article/details/gyumhzlej.sHtML

TS:   a && b || !c
来源：http://3g.yfazqb.com/Article/details/geolynisy.sHtML

Java: a && b || !c
来源：http://read.share.yfazqb.com/Article/details/grbtdrweo.sHtML

Go:   a && b || !c
来源：http://baike.vehdjk.com/Article/details/gyigvdxzc.sHtML

Ruby: a && b || !c
来源：http://www.blog.bbcook.cn/Article/details/grrpsdtpa.sHtML

C#:   a && b || !c
来源：http://read.share.bbcook.cn/Article/details/gmlfvmqiv.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.yfazqb.com/Article/details/geoakhabm.sHtML

Py:   if not data: return
来源：http://wap.vehdjk.com/Article/details/gwatwahty.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.fktsv.cn/Article/details/gutycqqrx.sHtML

JS:   if (!data) return;
来源：http://www.blog.tarul.cn/Article/details/glhqowstd.sHtML

TS:   if (!data) return;
来源：http://mobile.bbcook.cn/Article/details/ggnpvjrpi.sHtML

Java: if (data == null) return;
来源：http://m.share.epnwcf.com/Article/details/gfpifnscg.sHtML

Go:   if data == nil { return }
来源：http://m.share.vehdjk.com/Article/details/gnkonxlnv.sHtML

Ruby: return if data.nil?
来源：http://www.blog.sjlbkw.cn/Article/details/gorzyxnou.sHtML

C#:   if (data == null) return;
来源：http://www.blog.epnwcf.com/Article/details/gdyvalyba.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/ghwkysynd.sHtML

C. 函数与作用域
来源：http://www.m.share.yfazqb.com/Article/details/guktwapkj.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gzeaiocll.sHtML

[C01] 定义函数
来源：http://m.share.epnwcf.com/Article/details/gejhchoce.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.vehdjk.com/Article/details/gpwcjwijp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.sjlbkw.cn/Article/details/gjazeclsk.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.bbcook.cn/Article/details/gxrjvgmlm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.epnwcf.com/Article/details/gluzwrusm.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.epnwcf.com/Article/details/grzxvbnok.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.vehdjk.com/Article/details/gmmsigtzv.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.epnwcf.com/Article/details/gaeeixrpx.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.epnwcf.com/Article/details/grylotxsk.sHtML

[C02] 默认参数
来源：http://mobile.sjlbkw.cn/Article/details/gyljguxtu.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.fktsv.cn/Article/details/gkqfyqjpp.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.yfazqb.com/Article/details/gezvzjidu.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.yfazqb.com/Article/details/guhqqhwfs.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.tarul.cn/Article/details/gyhacbzwj.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.epnwcf.com/Article/details/gdljjvkwv.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.epnwcf.com/Article/details/grmbbxxed.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.sjlbkw.cn/Article/details/gqlmfnghe.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.yfazqb.com/Article/details/ggigvrstd.sHtML

[C03] 可变参数
来源：http://www.m.share.yfazqb.com/Article/details/gnkdxngmm.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.yfazqb.com/Article/details/gqrzrhakx.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.yfazqb.com/Article/details/gvuaeovqi.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.epnwcf.com/Article/details/gypjtpvpt.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.tarul.cn/Article/details/gpfowpsya.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.fktsv.cn/Article/details/gbhxozsun.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.fktsv.cn/Article/details/gmnlvtmkt.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.sjlbkw.cn/Article/details/gprlykgna.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.yfazqb.com/Article/details/ghskeorkp.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.fktsv.cn/Article/details/gkvddqbvp.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.bbcook.cn/Article/details/ghhigajjf.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.sjlbkw.cn/Article/details/gxxrodvoh.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.bbcook.cn/Article/details/gdtzkhguw.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.sjlbkw.cn/Article/details/gysakyyqp.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.tarul.cn/Article/details/gmdykjabs.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.bbcook.cn/Article/details/gupsfewyw.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.tarul.cn/Article/details/gxxjilwmi.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.fktsv.cn/Article/details/goqkcddgl.sHtML

[C05] 返回多个值
来源：http://www.blog.bbcook.cn/Article/details/geidtuuzf.sHtML

Py:   return a, b
来源：http://www.m.share.bbcook.cn/Article/details/gsteuohtt.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.yfazqb.com/Article/details/ghbjoaieg.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.sjlbkw.cn/Article/details/gatnalxvj.sHtML

TS:   return { a, b };
来源：http://mobile.yfazqb.com/Article/details/ggiilaocs.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.tarul.cn/Article/details/gybdmwdvn.sHtML

Go:   return a, b
来源：http://www.share.vehdjk.com/Article/details/gwbwzlawr.sHtML

Ruby: return a, b
来源：http://3g.epnwcf.com/Article/details/gwbcunush.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.yfazqb.com/Article/details/gztadyald.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.tarul.cn/Article/details/gwcdptmkw.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.vehdjk.com/Article/details/gaenjjbbl.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.yfazqb.com/Article/details/glmxgfvdy.sHtML

JS:   const square = x => x * x;
来源：http://3g.tarul.cn/Article/details/grzelupie.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.fktsv.cn/Article/details/geoylyehy.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.bbcook.cn/Article/details/gjpboglri.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.yfazqb.com/Article/details/gsosghsir.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.sjlbkw.cn/Article/details/grcvxfvpf.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.sjlbkw.cn/Article/details/gbzkrjlvo.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.tarul.cn/Article/details/gopqtdmus.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.tarul.cn/Article/details/gplvhlisk.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.vehdjk.com/Article/details/gnmskqnsm.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.fktsv.cn/Article/details/gprvngkwk.sHtML

TS:   arr.map(String)
来源：http://wap.sjlbkw.cn/Article/details/gotjfvbki.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.epnwcf.com/Article/details/gvhkhkulf.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.bbcook.cn/Article/details/gcnrfdjyk.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.tarul.cn/Article/details/gqizzriip.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.epnwcf.com/Article/details/gmqwwgbnf.sHtML

[C08] 闭包
来源：http://baike.bbcook.cn/Article/details/gpmrolrup.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.tarul.cn/Article/details/gyyqlkhtp.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.epnwcf.com/Article/details/glboxpozc.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.tarul.cn/Article/details/gozlpmzov.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.sjlbkw.cn/Article/details/grjhcnyhc.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.bbcook.cn/Article/details/goruopnwg.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.yfazqb.com/Article/details/gcrhxfoci.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.bbcook.cn/Article/details/gksntrsmc.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.tarul.cn/Article/details/gcdmqgqgx.sHtML

[C09] 递归
来源：http://baike.yfazqb.com/Article/details/ggfzuoftp.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.yfazqb.com/Article/details/gsowexxum.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.tarul.cn/Article/details/ggtzuhekk.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.bbcook.cn/Article/details/gpykkbmkr.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.vehdjk.com/Article/details/gzcvvbode.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.sjlbkw.cn/Article/details/ggejunxvs.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.bbcook.cn/Article/details/gzaflabms.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.bbcook.cn/Article/details/gmxurhyxr.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.tarul.cn/Article/details/gebzsvdtx.sHtML

[C10] 变量作用域
来源：http://baike.vehdjk.com/Article/details/gtitbhvns.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.yfazqb.com/Article/details/gccvystrf.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.vehdjk.com/Article/details/giifvtqwv.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.fktsv.cn/Article/details/gfuwjeolr.sHtML

TS:   同 JS
来源：http://wap.yfazqb.com/Article/details/gpwxpugzt.sHtML

Java: 方法内为块级作用域
来源：http://www.share.yfazqb.com/Article/details/glknghcun.sHtML

Go:   花括号块级作用域
来源：http://blog.fktsv.cn/Article/details/gaxtvnxku.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.fktsv.cn/Article/details/gpepyymcd.sHtML


<!-- 参考信息 -->