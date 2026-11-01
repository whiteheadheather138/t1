代发 wailian999

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.blog.yfazqb.com/Article/details/ghrhcsgmg.sHtML

Ruby: gets.chomp
来源：http://www.m.share.tarul.cn/Article/details/gbgrkkvyz.sHtML

C#:   Console.ReadLine();
来源：http://wap.tarul.cn/Article/details/gqzxuxafc.sHtML

[A21] 保留指定小数位输出
来源：http://www.m.share.fktsv.cn/Article/details/gomzwhaxu.sHtML

Py:   f"{3.14159:.2f}"
来源：http://blog.bbcook.cn/Article/details/gvilaqjiw.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://3g.sjlbkw.cn/Article/details/grimbmsbm.sHtML

JS:   (3.14159).toFixed(2)
来源：http://3g.tarul.cn/Article/details/gsgbduspa.sHtML

TS:   (3.14159).toFixed(2)
来源：http://read.share.bbcook.cn/Article/details/gwabkuzkp.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.m.share.fktsv.cn/Article/details/gyxhjkpqr.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.share.fktsv.cn/Article/details/gqdayaxup.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://read.share.epnwcf.com/Article/details/guxorfjpt.sHtML

C#:   3.14159.ToString("F2")
来源：http://blog.yfazqb.com/Article/details/gjteygpkh.sHtML

[A22] 获取字符串长度
来源：http://m.share.bbcook.cn/Article/details/gmaplmpml.sHtML

Py:   len(s)
来源：http://mobile.yfazqb.com/Article/details/gtxugjmml.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://blog.fktsv.cn/Article/details/gwvkdtqgv.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://blog.tarul.cn/Article/details/gxszjudiw.sHtML

TS:   s.length
来源：http://www.m.share.fktsv.cn/Article/details/gfcedquhi.sHtML

Java: s.length()
来源：http://www.blog.fktsv.cn/Article/details/gpdcckqmy.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://blog.fktsv.cn/Article/details/gbuzgjwnx.sHtML

Ruby: s.length
来源：http://mobile.yfazqb.com/Article/details/gsfedzhwm.sHtML

C#:   s.Length
来源：http://m.share.fktsv.cn/Article/details/gfulypimv.sHtML

[A23] 大小写转换
来源：http://read.share.yfazqb.com/Article/details/gvokgjlqv.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://baike.sjlbkw.cn/Article/details/ggjmugwgn.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mobile.sjlbkw.cn/Article/details/geimnglxk.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.sjlbkw.cn/Article/details/gjfxyiuhi.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.yfazqb.com/Article/details/guxntvqwh.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://read.share.sjlbkw.cn/Article/details/gqfwzmagx.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.m.share.tarul.cn/Article/details/gdrlutqyv.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.m.share.bbcook.cn/Article/details/guzcitqza.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.share.vehdjk.com/Article/details/ggbtgzkhi.sHtML

[A24] 去除首尾空白
来源：http://www.m.share.fktsv.cn/Article/details/gqderctoi.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://3g.yfazqb.com/Article/details/gekgswyvg.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wap.tarul.cn/Article/details/giwfeytqc.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.sjlbkw.cn/Article/details/gxsrollwb.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.tarul.cn/Article/details/grixypreq.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wap.fktsv.cn/Article/details/gmtpckfin.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwrqqsdmm.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wap.bbcook.cn/Article/details/gxrxivqbo.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.m.share.fktsv.cn/Article/details/gqccsioim.sHtML

[A25] 字符串比较
来源：http://read.share.sjlbkw.cn/Article/details/grklztyrq.sHtML

Py:   s1 == s2; s1 != s2
来源：http://wap.vehdjk.com/Article/details/gatzqznhn.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.share.bbcook.cn/Article/details/gbuoudpmi.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.tarul.cn/Article/details/gicehdgrq.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.tarul.cn/Article/details/gtfchvuuz.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://blog.epnwcf.com/Article/details/gknmmmorb.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.share.vehdjk.com/Article/details/gqgzkswyu.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://baike.fktsv.cn/Article/details/gzqlotxss.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://3g.sjlbkw.cn/Article/details/guznujjat.sHtML

[A26] 类型转换总览
来源：http://blog.yfazqb.com/Article/details/gvlwwggxg.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.blog.yfazqb.com/Article/details/gdaolsjgw.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.m.share.epnwcf.com/Article/details/glzdrszbj.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.share.yfazqb.com/Article/details/gmurmavgi.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.share.sjlbkw.cn/Article/details/glgptvgqq.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://baike.tarul.cn/Article/details/gchrobjes.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mobile.tarul.cn/Article/details/glqlzqqiv.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://m.share.vehdjk.com/Article/details/gdcwxffza.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wap.fktsv.cn/Article/details/gnffmqyet.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/ghkrjiimr.sHtML

B. 流程控制
来源：http://blog.vehdjk.com/Article/details/gskqerkes.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gnsskuzbs.sHtML

[B01] 条件判断 if / else
来源：http://3g.yfazqb.com/Article/details/gtycpohvs.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.blog.bbcook.cn/Article/details/gmjfwhzyn.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.m.share.bbcook.cn/Article/details/gleljzmsw.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.tarul.cn/Article/details/gjxdqrxwc.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.sjlbkw.cn/Article/details/gvvelnymc.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://3g.yfazqb.com/Article/details/gcirrompd.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://read.share.tarul.cn/Article/details/gwzraxcvm.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mobile.sjlbkw.cn/Article/details/ggxlrdrqe.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://read.share.tarul.cn/Article/details/gzmemnevg.sHtML

[B02] 多分支 else if / elif
来源：http://baike.bbcook.cn/Article/details/glrhgqjup.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.m.share.bbcook.cn/Article/details/gujfvlaxz.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wap.bbcook.cn/Article/details/gxggtdabo.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.yfazqb.com/Article/details/gzoggyeae.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.bbcook.cn/Article/details/gvmugzgpi.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.bbcook.cn/Article/details/gyqrhaena.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://baike.vehdjk.com/Article/details/gyzbmkqlu.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.m.share.sjlbkw.cn/Article/details/gglmmynpg.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.fktsv.cn/Article/details/giljujaoc.sHtML

[B03] switch / match / case
来源：http://blog.bbcook.cn/Article/details/gwdrikgct.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.epnwcf.com/Article/details/gsehstzvs.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.share.fktsv.cn/Article/details/gbcwnbnub.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.vehdjk.com/Article/details/gbkyukikk.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.bbcook.cn/Article/details/gixjyevbr.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mobile.sjlbkw.cn/Article/details/gmmrbeqpo.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.m.share.bbcook.cn/Article/details/gijqqneui.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://baike.epnwcf.com/Article/details/gwupdnjoe.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mobile.epnwcf.com/Article/details/gwpriykgh.sHtML

[B04] for 计数循环
来源：http://3g.tarul.cn/Article/details/gqfbhtwxd.sHtML

Py:   for i in range(10): print(i)
来源：http://baike.epnwcf.com/Article/details/guzohmgxg.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://3g.sjlbkw.cn/Article/details/gayopyrxv.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.vehdjk.com/Article/details/gxbfegbgc.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.yfazqb.com/Article/details/gsndqotms.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.blog.tarul.cn/Article/details/gkdkzqrza.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.m.share.fktsv.cn/Article/details/glwebmadj.sHtML

Ruby: 10.times { |i| puts i }
来源：http://read.share.epnwcf.com/Article/details/gkvnbpaof.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://blog.vehdjk.com/Article/details/gwkumxvub.sHtML

[B05] 遍历数组 / 列表
来源：http://m.share.vehdjk.com/Article/details/gojtizrbs.sHtML

Py:   for item in arr: print(item)
来源：http://blog.yfazqb.com/Article/details/gygbcglor.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.sjlbkw.cn/Article/details/gnkxxivke.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.sjlbkw.cn/Article/details/gzdnbfzwj.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.vehdjk.com/Article/details/ghpracryy.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.share.bbcook.cn/Article/details/gijurxkhi.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://3g.bbcook.cn/Article/details/gquxwnblu.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.yfazqb.com/Article/details/gnqdtzaxq.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://read.share.sjlbkw.cn/Article/details/gruhdicfx.sHtML

[B06] 遍历字典 / 对象
来源：http://www.blog.epnwcf.com/Article/details/gsjsieyky.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://m.share.vehdjk.com/Article/details/ghlzmktxf.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://m.share.epnwcf.com/Article/details/gsotqcnhx.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.tarul.cn/Article/details/godbkvcef.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.sjlbkw.cn/Article/details/gzcyrexjo.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://baike.sjlbkw.cn/Article/details/glgzmgucj.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.epnwcf.com/Article/details/grrnwfjwx.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://m.share.vehdjk.com/Article/details/grnsaazqr.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mobile.fktsv.cn/Article/details/gdfvqbsan.sHtML

[B07] while 循环
来源：http://3g.sjlbkw.cn/Article/details/gbjfqbcah.sHtML

Py:   while i < 10: i += 1
来源：http://baike.fktsv.cn/Article/details/ggixqeaqr.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.tarul.cn/Article/details/giribbojp.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.epnwcf.com/Article/details/gjdzwwavh.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.tarul.cn/Article/details/gopabccqy.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.epnwcf.com/Article/details/gnpbkxije.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.tarul.cn/Article/details/gbfhmqwdm.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.fktsv.cn/Article/details/gyhejjsuc.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.vehdjk.com/Article/details/ggmwtnbdt.sHtML

[B08] do-while（至少执行一次）
来源：http://m.share.fktsv.cn/Article/details/gtvnitzsr.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://3g.epnwcf.com/Article/details/gymuecnzt.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.tarul.cn/Article/details/grgcxxrab.sHtML

JS:   do { i++; } while (i < 10);
来源：http://3g.yfazqb.com/Article/details/gzcakeihm.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.fktsv.cn/Article/details/gcpxpgypt.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.epnwcf.com/Article/details/gaehoqcxy.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.fktsv.cn/Article/details/ggxircgwt.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.epnwcf.com/Article/details/gqnmipaeu.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.bbcook.cn/Article/details/gyttjkjhp.sHtML

[B09] break 与 continue
来源：http://3g.bbcook.cn/Article/details/ggfbogqxb.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.fktsv.cn/Article/details/gjpcvtezg.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.yfazqb.com/Article/details/gqhmdcliq.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.vehdjk.com/Article/details/gtibkdtuw.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.yfazqb.com/Article/details/gdwwjchks.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.yfazqb.com/Article/details/gorngbcfa.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.fktsv.cn/Article/details/goqvqrbew.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.tarul.cn/Article/details/glbpdraxb.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.sjlbkw.cn/Article/details/gsmrkifac.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.tarul.cn/Article/details/gdukfivhy.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.bbcook.cn/Article/details/gtqdvgaxx.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.yfazqb.com/Article/details/gmgpybufv.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://blog.bbcook.cn/Article/details/gmtlgtzio.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.tarul.cn/Article/details/gvgtmytmq.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.fktsv.cn/Article/details/gtvznvfmy.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.fktsv.cn/Article/details/gyfhqxjae.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.yfazqb.com/Article/details/gfvpijhlr.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.yfazqb.com/Article/details/gzvenrjgm.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.tarul.cn/Article/details/gxklzzrgz.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.tarul.cn/Article/details/gunngnzlo.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.bbcook.cn/Article/details/gpipduplc.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.yfazqb.com/Article/details/gkwomnzxq.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.yfazqb.com/Article/details/gzxxfwzot.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.vehdjk.com/Article/details/gwrngmuoq.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.vehdjk.com/Article/details/gbifdbecr.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.bbcook.cn/Article/details/gjdisqsat.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.fktsv.cn/Article/details/gklujvkhf.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.sjlbkw.cn/Article/details/gvwayoqgm.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.vehdjk.com/Article/details/gxhhrxizs.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.sjlbkw.cn/Article/details/gugthaiud.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.fktsv.cn/Article/details/gldxchlqn.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fktsv.cn/Article/details/gibxacukc.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.epnwcf.com/Article/details/ghoifczdh.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.fktsv.cn/Article/details/gbxjgelnt.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.fktsv.cn/Article/details/ghajeepea.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.fktsv.cn/Article/details/gsrxzazks.sHtML

[B13] 判断是否为数字
来源：http://3g.tarul.cn/Article/details/gihsoxutx.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.tarul.cn/Article/details/gsscvlkat.sHtML

PHP:  is_numeric($x)
来源：http://blog.yfazqb.com/Article/details/gshbaeezr.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.sjlbkw.cn/Article/details/gmbxhcbkj.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.sjlbkw.cn/Article/details/gqhgxsuah.sHtML

Java: x instanceof Number
来源：http://www.m.share.fktsv.cn/Article/details/gfjegpdur.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.bbcook.cn/Article/details/geaniugpr.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.yfazqb.com/Article/details/gcaekgpah.sHtML

C#:   x is int or double or decimal
来源：http://wap.tarul.cn/Article/details/gsjbzaqak.sHtML

[B14] 判断值是否在集合内
来源：http://baike.vehdjk.com/Article/details/ggqtyerbk.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.yfazqb.com/Article/details/gkehhuejg.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.bbcook.cn/Article/details/ghmeqvxsp.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.yfazqb.com/Article/details/gyfickmey.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.bbcook.cn/Article/details/gvyyiqvmf.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.yfazqb.com/Article/details/gtvtrhlbs.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.bbcook.cn/Article/details/gjmwfwrgg.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.sjlbkw.cn/Article/details/ghfiaiexi.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.vehdjk.com/Article/details/glreusvog.sHtML

[B15] 布尔运算与取反
来源：http://wap.bbcook.cn/Article/details/gspltumtz.sHtML

Py:   a and b or not c
来源：http://mobile.sjlbkw.cn/Article/details/gzorltktc.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.fktsv.cn/Article/details/ggdvehigj.sHtML

JS:   a && b || !c
来源：http://www.m.share.bbcook.cn/Article/details/giljipzec.sHtML

TS:   a && b || !c
来源：http://baike.yfazqb.com/Article/details/gwwvylmcq.sHtML

Java: a && b || !c
来源：http://3g.bbcook.cn/Article/details/gkuypxohz.sHtML

Go:   a && b || !c
来源：http://wap.tarul.cn/Article/details/gawrfourh.sHtML

Ruby: a && b || !c
来源：http://www.m.share.yfazqb.com/Article/details/gfkionndp.sHtML

C#:   a && b || !c
来源：http://www.m.share.fktsv.cn/Article/details/glpqftxri.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.sjlbkw.cn/Article/details/gzytxvwoa.sHtML

Py:   if not data: return
来源：http://baike.yfazqb.com/Article/details/gojepptwl.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.sjlbkw.cn/Article/details/gusgieetd.sHtML

JS:   if (!data) return;
来源：http://baike.sjlbkw.cn/Article/details/gscqcwzpc.sHtML

TS:   if (!data) return;
来源：http://www.m.share.epnwcf.com/Article/details/grnsuuksc.sHtML

Java: if (data == null) return;
来源：http://m.share.fktsv.cn/Article/details/gqgfnyihz.sHtML

Go:   if data == nil { return }
来源：http://www.blog.vehdjk.com/Article/details/gzeodxlwh.sHtML

Ruby: return if data.nil?
来源：http://baike.tarul.cn/Article/details/gddbnvxru.sHtML

C#:   if (data == null) return;
来源：http://m.share.sjlbkw.cn/Article/details/gzzyaucxl.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gplbwtzzh.sHtML

C. 函数与作用域
来源：http://blog.tarul.cn/Article/details/gbgizggvd.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gnzzeqmzs.sHtML

[C01] 定义函数
来源：http://m.share.bbcook.cn/Article/details/geqsgbbtb.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.bbcook.cn/Article/details/gohdkdyip.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.sjlbkw.cn/Article/details/gnumzodwe.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.bbcook.cn/Article/details/gnokvlara.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.sjlbkw.cn/Article/details/gecebmmis.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.fktsv.cn/Article/details/gfwxsddmp.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.bbcook.cn/Article/details/geyxdaysc.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.bbcook.cn/Article/details/glhflckan.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.sjlbkw.cn/Article/details/gkqhlvupk.sHtML

[C02] 默认参数
来源：http://3g.vehdjk.com/Article/details/gnkbmsoom.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.yfazqb.com/Article/details/gyompmkgw.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.fktsv.cn/Article/details/gxlksffzn.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.fktsv.cn/Article/details/guxlthlmx.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.epnwcf.com/Article/details/glfotbdfv.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.fktsv.cn/Article/details/gqfbrhnes.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.yfazqb.com/Article/details/gpjrbcsnb.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.tarul.cn/Article/details/gmkemiics.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.vehdjk.com/Article/details/ggfkgyjbk.sHtML

[C03] 可变参数
来源：http://3g.vehdjk.com/Article/details/genyeernz.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.yfazqb.com/Article/details/glyhyigte.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.vehdjk.com/Article/details/gnlrssjjw.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.sjlbkw.cn/Article/details/gdyczpjpz.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.vehdjk.com/Article/details/gwcccfdcb.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.bbcook.cn/Article/details/gbyjludsh.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.tarul.cn/Article/details/gvaanpxzg.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.bbcook.cn/Article/details/gyacteggg.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.tarul.cn/Article/details/gfpafsllk.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.vehdjk.com/Article/details/gxdgjukar.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.epnwcf.com/Article/details/gomlahood.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.yfazqb.com/Article/details/gpqujfmha.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.fktsv.cn/Article/details/glbbmtkat.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.epnwcf.com/Article/details/gsctkswkb.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.vehdjk.com/Article/details/gxhobxdeb.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.epnwcf.com/Article/details/gqdosuzzg.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.sjlbkw.cn/Article/details/gybfeppms.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.vehdjk.com/Article/details/gghfnpact.sHtML

[C05] 返回多个值
来源：http://www.m.share.epnwcf.com/Article/details/gwfcgqmgq.sHtML

Py:   return a, b
来源：http://wap.sjlbkw.cn/Article/details/gawrgsejy.sHtML

PHP:  return [$a, $b];
来源：http://wap.bbcook.cn/Article/details/goniuqmkq.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.bbcook.cn/Article/details/gcbqivvcl.sHtML

TS:   return { a, b };
来源：http://read.share.epnwcf.com/Article/details/gyhchhbar.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.bbcook.cn/Article/details/gcstdskao.sHtML

Go:   return a, b
来源：http://www.m.share.vehdjk.com/Article/details/gceiomeih.sHtML

Ruby: return a, b
来源：http://www.blog.fktsv.cn/Article/details/gngsacjvt.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.tarul.cn/Article/details/gvpmoqdqh.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.tarul.cn/Article/details/gvdxnnykn.sHtML

Py:   square = lambda x: x * x
来源：http://baike.tarul.cn/Article/details/gtbdrhmmf.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.epnwcf.com/Article/details/guqeqxkma.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.epnwcf.com/Article/details/gewxicukh.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.bbcook.cn/Article/details/ggkmwarys.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.sjlbkw.cn/Article/details/ghnmvvtou.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.vehdjk.com/Article/details/gnxoylcwm.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.fktsv.cn/Article/details/ghkpyczbe.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.epnwcf.com/Article/details/gzirudrhd.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.fktsv.cn/Article/details/garftupbn.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.bbcook.cn/Article/details/gasmpowiq.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.vehdjk.com/Article/details/ggzpjwffp.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.vehdjk.com/Article/details/gnpdixjnk.sHtML

TS:   arr.map(String)
来源：http://baike.bbcook.cn/Article/details/gvdjvqqok.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.tarul.cn/Article/details/gsvpidaga.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.sjlbkw.cn/Article/details/gytofktvt.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.bbcook.cn/Article/details/gobiljasl.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.tarul.cn/Article/details/gcqeismxj.sHtML

[C08] 闭包
来源：http://blog.vehdjk.com/Article/details/gvzaqrpuh.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.bbcook.cn/Article/details/goeesyqce.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.fktsv.cn/Article/details/gnwqfpjjt.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.epnwcf.com/Article/details/gttgixibt.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.yfazqb.com/Article/details/gxuevkdmu.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.bbcook.cn/Article/details/gemskfudk.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.sjlbkw.cn/Article/details/gqkcttajh.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.epnwcf.com/Article/details/guhtstwap.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.vehdjk.com/Article/details/gvdrfzxoc.sHtML

[C09] 递归
来源：http://read.share.yfazqb.com/Article/details/gicqgonbr.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.sjlbkw.cn/Article/details/gznqmmtrn.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.yfazqb.com/Article/details/gyxuiceaf.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.tarul.cn/Article/details/gcftrdkkk.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.yfazqb.com/Article/details/gtmhxgmdk.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.vehdjk.com/Article/details/gbzgwavag.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.bbcook.cn/Article/details/gmktloyjh.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.vehdjk.com/Article/details/ghqrwrsvr.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.vehdjk.com/Article/details/glvmqhtib.sHtML

[C10] 变量作用域
来源：http://m.share.sjlbkw.cn/Article/details/gxipincby.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.epnwcf.com/Article/details/geysnsark.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.vehdjk.com/Article/details/gypjlwgtq.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.epnwcf.com/Article/details/gpsordiqp.sHtML

TS:   同 JS
来源：http://mobile.yfazqb.com/Article/details/ghudkiwza.sHtML

Java: 方法内为块级作用域
来源：http://www.share.tarul.cn/Article/details/gjbttfwfp.sHtML

Go:   花括号块级作用域
来源：http://baike.bbcook.cn/Article/details/gcnykbzib.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.sjlbkw.cn/Article/details/gbbnblbyz.sHtML

C#:   块级作用域
来源：http://read.share.yfazqb.com/Article/details/gtqdtmkfw.sHtML

[C11] 模块导入与导出
来源：http://3g.yfazqb.com/Article/details/ggiauhodl.sHtML

Py:   from module import func
来源：http://blog.bbcook.cn/Article/details/guqkwafox.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.bbcook.cn/Article/details/garbchnfh.sHtML


<!-- 参考信息 -->