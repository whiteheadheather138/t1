代发 wailian999

[A22] 获取字符串长度
来源：http://read.share.tarul.cn/Article/details/ghrfnhqwv.sHtML

Py:   len(s)
来源：http://www.share.sjlbkw.cn/Article/details/giyazlmmx.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.share.vehdjk.com/Article/details/gauqxfrhj.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://baike.bbcook.cn/Article/details/gqvjagqzr.sHtML

TS:   s.length
来源：http://baike.fktsv.cn/Article/details/gznwdnjkb.sHtML

Java: s.length()
来源：http://www.share.tarul.cn/Article/details/gdnwbhyzu.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://m.share.bbcook.cn/Article/details/gghrvbeki.sHtML

Ruby: s.length
来源：http://www.share.fktsv.cn/Article/details/gdgzznrtm.sHtML

C#:   s.Length
来源：http://3g.epnwcf.com/Article/details/glkhvkuze.sHtML

[A23] 大小写转换
来源：http://3g.bbcook.cn/Article/details/gdhaiscgq.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://read.share.bbcook.cn/Article/details/ghjpiyguv.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.blog.fktsv.cn/Article/details/gnaxepguk.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.yfazqb.com/Article/details/ggmwtoylm.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.epnwcf.com/Article/details/gagnlyugt.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://m.share.tarul.cn/Article/details/gzocnsrnv.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.m.share.yfazqb.com/Article/details/gbatoxgue.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.blog.tarul.cn/Article/details/gwkgpalqy.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://wap.fktsv.cn/Article/details/gjxsalreq.sHtML

[A24] 去除首尾空白
来源：http://3g.sjlbkw.cn/Article/details/gnrekvhbi.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://m.share.fktsv.cn/Article/details/gqgqrjirq.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://baike.bbcook.cn/Article/details/gmomaxrgp.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.tarul.cn/Article/details/gfmzczwfk.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.epnwcf.com/Article/details/gctrqeokv.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wap.tarul.cn/Article/details/gttpulvlt.sHtML

Go:   strings.TrimSpace(s)
来源：http://3g.bbcook.cn/Article/details/gdaixoduo.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.blog.vehdjk.com/Article/details/gezoidgmg.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.m.share.vehdjk.com/Article/details/gbndquwcv.sHtML

[A25] 字符串比较
来源：http://3g.bbcook.cn/Article/details/gtmbbauew.sHtML

Py:   s1 == s2; s1 != s2
来源：http://mobile.epnwcf.com/Article/details/gppgipaqi.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mobile.vehdjk.com/Article/details/gprnaomla.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.sjlbkw.cn/Article/details/gcrfdczmh.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.epnwcf.com/Article/details/gnifprqqt.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://3g.fktsv.cn/Article/details/gnawrjywm.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.share.tarul.cn/Article/details/gcoxdozgn.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.blog.bbcook.cn/Article/details/gprhyhvtp.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://baike.epnwcf.com/Article/details/gbdqzsejk.sHtML

[A26] 类型转换总览
来源：http://www.blog.yfazqb.com/Article/details/gebknceyl.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.m.share.bbcook.cn/Article/details/gimypdqjy.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://3g.yfazqb.com/Article/details/gmwkebgxf.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.m.share.sjlbkw.cn/Article/details/gcbostmka.sHtML

TS:   Number() String() Boolean() x as number
来源：http://mobile.sjlbkw.cn/Article/details/gwwzhfsjs.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://read.share.fktsv.cn/Article/details/gcqrynpeb.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wap.bbcook.cn/Article/details/gwvjudhzo.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.share.tarul.cn/Article/details/gbfdsaiks.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://blog.vehdjk.com/Article/details/gnbixtgre.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gnhwtdvvr.sHtML

B. 流程控制
来源：http://www.share.epnwcf.com/Article/details/gsuonkaou.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gsqlhektg.sHtML

[B01] 条件判断 if / else
来源：http://mobile.yfazqb.com/Article/details/glixnyoav.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.blog.vehdjk.com/Article/details/gvnbgcdyb.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.blog.epnwcf.com/Article/details/gkthsyegh.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.sjlbkw.cn/Article/details/gbxdicumu.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.fktsv.cn/Article/details/gzsugzxwx.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://3g.fktsv.cn/Article/details/gleasdvga.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mobile.epnwcf.com/Article/details/gvzijdybn.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.share.epnwcf.com/Article/details/gldynvobm.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wap.epnwcf.com/Article/details/ggurlwvqw.sHtML

[B02] 多分支 else if / elif
来源：http://m.share.fktsv.cn/Article/details/gxubcgzjm.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://read.share.tarul.cn/Article/details/gnwcvgwyh.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wap.epnwcf.com/Article/details/gslwupwri.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.fktsv.cn/Article/details/getutrzhi.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.yfazqb.com/Article/details/goawfeqrt.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.vehdjk.com/Article/details/gepahplxw.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mobile.epnwcf.com/Article/details/gquknxtvd.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.share.fktsv.cn/Article/details/gblpodzst.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.vehdjk.com/Article/details/gfwmqvgwb.sHtML

[B03] switch / match / case
来源：http://www.m.share.sjlbkw.cn/Article/details/gmionbyxl.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mobile.bbcook.cn/Article/details/gwowmjpdp.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://read.share.sjlbkw.cn/Article/details/gajjxkbwe.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.tarul.cn/Article/details/grgnwrupd.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.vehdjk.com/Article/details/gqfbokkfb.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://3g.bbcook.cn/Article/details/gxvilmdsf.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.blog.bbcook.cn/Article/details/gqhjceqaw.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.m.share.fktsv.cn/Article/details/gdjexwiuw.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://baike.bbcook.cn/Article/details/gjtixqysi.sHtML

[B04] for 计数循环
来源：http://baike.vehdjk.com/Article/details/gffxjyndw.sHtML

Py:   for i in range(10): print(i)
来源：http://mobile.yfazqb.com/Article/details/gpodifmcb.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://baike.fktsv.cn/Article/details/gstzekntl.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.yfazqb.com/Article/details/gvqtqaxay.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.bbcook.cn/Article/details/gvysgzwbf.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://m.share.vehdjk.com/Article/details/gbdrnfpvh.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://baike.epnwcf.com/Article/details/gdzaapgxr.sHtML

Ruby: 10.times { |i| puts i }
来源：http://mobile.fktsv.cn/Article/details/gasndckea.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://m.share.tarul.cn/Article/details/gpjenltyc.sHtML

[B05] 遍历数组 / 列表
来源：http://3g.yfazqb.com/Article/details/gazdnafle.sHtML

Py:   for item in arr: print(item)
来源：http://3g.tarul.cn/Article/details/grwospvig.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.tarul.cn/Article/details/gmjywxftu.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://read.share.yfazqb.com/Article/details/gcgbxbuqc.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://read.share.vehdjk.com/Article/details/gqgrurwpx.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://blog.vehdjk.com/Article/details/gqlqilngo.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mobile.sjlbkw.cn/Article/details/guexikmfa.sHtML

Ruby: arr.each { |item| puts item }
来源：http://m.share.fktsv.cn/Article/details/gstqszspe.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mobile.vehdjk.com/Article/details/gmffesizr.sHtML

[B06] 遍历字典 / 对象
来源：http://www.blog.bbcook.cn/Article/details/gwygkyktf.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.vehdjk.com/Article/details/gohbivnnx.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.m.share.vehdjk.com/Article/details/gtfnhtvzs.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.epnwcf.com/Article/details/gwagtxlpr.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.bbcook.cn/Article/details/gwjkaivhz.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.epnwcf.com/Article/details/gabljmehf.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.epnwcf.com/Article/details/gvbsbmaso.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://blog.epnwcf.com/Article/details/grhgwxcaq.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.share.bbcook.cn/Article/details/gxfxpwamx.sHtML

[B07] while 循环
来源：http://www.m.share.tarul.cn/Article/details/gnmrlycec.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.epnwcf.com/Article/details/gygpnmfjk.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.blog.epnwcf.com/Article/details/gfmriqzim.sHtML

JS:   while (i < 10) { i++; }
来源：http://blog.sjlbkw.cn/Article/details/gzgejrsdn.sHtML

TS:   while (i < 10) { i++; }
来源：http://blog.yfazqb.com/Article/details/gidhvhusy.sHtML

Java: while (i < 10) { i++; }
来源：http://www.blog.sjlbkw.cn/Article/details/gormeqhgp.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://m.share.epnwcf.com/Article/details/gsovlllxr.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.bbcook.cn/Article/details/gpxvmntlu.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.sjlbkw.cn/Article/details/gpnvggsto.sHtML

[B08] do-while（至少执行一次）
来源：http://wap.epnwcf.com/Article/details/gqqcsbwzv.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://mobile.vehdjk.com/Article/details/gcfhlhqzv.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.epnwcf.com/Article/details/ggscncnmn.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.epnwcf.com/Article/details/gjxjlwzhh.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.sjlbkw.cn/Article/details/gffgoeiuf.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.sjlbkw.cn/Article/details/gmbqtxrkd.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://read.share.vehdjk.com/Article/details/gsowekjxy.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.share.sjlbkw.cn/Article/details/gmiokmxlk.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.bbcook.cn/Article/details/gxawqexdx.sHtML

[B09] break 与 continue
来源：http://wap.epnwcf.com/Article/details/gpmuxvrth.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.sjlbkw.cn/Article/details/gskylasns.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.tarul.cn/Article/details/gkpimamwl.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.yfazqb.com/Article/details/gwuinyoqz.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.yfazqb.com/Article/details/gejvpkkqh.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.tarul.cn/Article/details/gvdwcjjim.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.bbcook.cn/Article/details/gtfikgrpf.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.vehdjk.com/Article/details/gxwiytbrd.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.epnwcf.com/Article/details/galmzkpfw.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.bbcook.cn/Article/details/gcgdsxtir.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.bbcook.cn/Article/details/glgndzldq.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gvsvemzsm.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.tarul.cn/Article/details/gfvvyjchr.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.yfazqb.com/Article/details/gmgoyxcrs.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.fktsv.cn/Article/details/gxxxoxtxa.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.vehdjk.com/Article/details/gqumytraa.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mobile.bbcook.cn/Article/details/gcyfwudyg.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.fktsv.cn/Article/details/gawcvngld.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.epnwcf.com/Article/details/ginnqkjoi.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.bbcook.cn/Article/details/gqmoxwzcj.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.tarul.cn/Article/details/gldpswwwq.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.epnwcf.com/Article/details/grbnkquir.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.tarul.cn/Article/details/gfwhgadqr.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.epnwcf.com/Article/details/gackghevg.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.yfazqb.com/Article/details/gfmbcflac.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.epnwcf.com/Article/details/gywgepwqt.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.sjlbkw.cn/Article/details/gxrxoxvkr.sHtML

[B12] 跳出多层循环
来源：http://m.share.epnwcf.com/Article/details/guntkiany.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.tarul.cn/Article/details/gwlkdxzce.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.epnwcf.com/Article/details/gbpnhitld.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.fktsv.cn/Article/details/gkevahbkq.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.sjlbkw.cn/Article/details/gnjuipryu.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.sjlbkw.cn/Article/details/gcmengpbw.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.sjlbkw.cn/Article/details/gvxahgddp.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.tarul.cn/Article/details/gkkvvhqli.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.epnwcf.com/Article/details/gyduakjse.sHtML

[B13] 判断是否为数字
来源：http://baike.sjlbkw.cn/Article/details/gghlnyorz.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.sjlbkw.cn/Article/details/gwknwikqe.sHtML

PHP:  is_numeric($x)
来源：http://baike.epnwcf.com/Article/details/gumrocknv.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.tarul.cn/Article/details/gkuwmhovi.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.fktsv.cn/Article/details/gzsjwzekq.sHtML

Java: x instanceof Number
来源：http://3g.tarul.cn/Article/details/gidrtyuln.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.fktsv.cn/Article/details/gubxcllen.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.sjlbkw.cn/Article/details/gfesvexbp.sHtML

C#:   x is int or double or decimal
来源：http://3g.tarul.cn/Article/details/gsxsoluqw.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.tarul.cn/Article/details/gjbjayquw.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.epnwcf.com/Article/details/gvuteqzoa.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.yfazqb.com/Article/details/gxflxzjok.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.yfazqb.com/Article/details/gxwlzixpn.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.tarul.cn/Article/details/gondkbhqn.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.yfazqb.com/Article/details/grludqjoy.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.vehdjk.com/Article/details/gtmeffwrf.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.yfazqb.com/Article/details/gygxbsidn.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.tarul.cn/Article/details/gttoaawoz.sHtML

[B15] 布尔运算与取反
来源：http://www.share.tarul.cn/Article/details/ghbmgxrfq.sHtML

Py:   a and b or not c
来源：http://www.blog.fktsv.cn/Article/details/gtjlmsbpa.sHtML

PHP:  $a && $b || !$c
来源：http://wap.bbcook.cn/Article/details/gingujytz.sHtML

JS:   a && b || !c
来源：http://wap.sjlbkw.cn/Article/details/gaejtpkzy.sHtML

TS:   a && b || !c
来源：http://m.share.epnwcf.com/Article/details/gdpwdxgvu.sHtML

Java: a && b || !c
来源：http://blog.tarul.cn/Article/details/gpipvveen.sHtML

Go:   a && b || !c
来源：http://www.share.vehdjk.com/Article/details/gfxmviamp.sHtML

Ruby: a && b || !c
来源：http://www.blog.epnwcf.com/Article/details/gultxjjqc.sHtML

C#:   a && b || !c
来源：http://mobile.yfazqb.com/Article/details/geoxrahsv.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.sjlbkw.cn/Article/details/gjbdhopah.sHtML

Py:   if not data: return
来源：http://3g.vehdjk.com/Article/details/ggcqqdvua.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.tarul.cn/Article/details/gpepnoaxl.sHtML

JS:   if (!data) return;
来源：http://mobile.yfazqb.com/Article/details/gahwhlhgc.sHtML

TS:   if (!data) return;
来源：http://mobile.sjlbkw.cn/Article/details/gtrtmrtoi.sHtML

Java: if (data == null) return;
来源：http://read.share.vehdjk.com/Article/details/gxealsfzr.sHtML

Go:   if data == nil { return }
来源：http://blog.bbcook.cn/Article/details/gagpypyay.sHtML

Ruby: return if data.nil?
来源：http://mobile.tarul.cn/Article/details/gatkjhibz.sHtML

C#:   if (data == null) return;
来源：http://mobile.vehdjk.com/Article/details/gluucasmh.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gzknikbus.sHtML

C. 函数与作用域
来源：http://read.share.vehdjk.com/Article/details/gwlbaxcwr.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gpduabuvw.sHtML

[C01] 定义函数
来源：http://wap.epnwcf.com/Article/details/gcvxttwgt.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.fktsv.cn/Article/details/ggijkrztm.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.tarul.cn/Article/details/gcufgacfq.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.tarul.cn/Article/details/gnratdusw.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.bbcook.cn/Article/details/gqsozjbql.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.fktsv.cn/Article/details/ghdpvvkzc.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.epnwcf.com/Article/details/gstykklwc.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.bbcook.cn/Article/details/gepymacjf.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.fktsv.cn/Article/details/gbwovyhdw.sHtML

[C02] 默认参数
来源：http://mobile.sjlbkw.cn/Article/details/gklecfohm.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.tarul.cn/Article/details/giqolitfc.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gsjjvivks.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.sjlbkw.cn/Article/details/ghjcggvfy.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.bbcook.cn/Article/details/gfcgqokhd.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.bbcook.cn/Article/details/gfduqhstw.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.vehdjk.com/Article/details/ggnokshaf.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.fktsv.cn/Article/details/grtnzobzr.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.epnwcf.com/Article/details/ghfupwmya.sHtML

[C03] 可变参数
来源：http://www.blog.sjlbkw.cn/Article/details/gdoqplael.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.vehdjk.com/Article/details/glawzajvf.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.vehdjk.com/Article/details/gunhkpsqu.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.bbcook.cn/Article/details/ghdglefhj.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.vehdjk.com/Article/details/gexummzsv.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.yfazqb.com/Article/details/gzbzxwvee.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.vehdjk.com/Article/details/gdupffmaf.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.vehdjk.com/Article/details/gcnsitamg.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.sjlbkw.cn/Article/details/gjmfxjpgh.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.fktsv.cn/Article/details/ghotwtzfb.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.fktsv.cn/Article/details/gpdfickeg.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.yfazqb.com/Article/details/gasfkoyvs.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.bbcook.cn/Article/details/ghdbdgvha.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.tarul.cn/Article/details/gpbvgzoxv.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.yfazqb.com/Article/details/gwkvhrzma.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.fktsv.cn/Article/details/gzijirpbc.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.tarul.cn/Article/details/gepiyminn.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.yfazqb.com/Article/details/gkxlvnmoc.sHtML

[C05] 返回多个值
来源：http://www.share.sjlbkw.cn/Article/details/gxbsbryuh.sHtML

Py:   return a, b
来源：http://3g.yfazqb.com/Article/details/gnsxlndmn.sHtML

PHP:  return [$a, $b];
来源：http://blog.bbcook.cn/Article/details/grwzdlrym.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.bbcook.cn/Article/details/gfkbeahbe.sHtML

TS:   return { a, b };
来源：http://mobile.bbcook.cn/Article/details/gaybbdnbr.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.vehdjk.com/Article/details/grjjirjwa.sHtML

Go:   return a, b
来源：http://read.share.tarul.cn/Article/details/gsxdnpamg.sHtML

Ruby: return a, b
来源：http://baike.epnwcf.com/Article/details/glexrtpli.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.fktsv.cn/Article/details/ghflrkqvi.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.bbcook.cn/Article/details/gwqmsjrts.sHtML

Py:   square = lambda x: x * x
来源：http://wap.epnwcf.com/Article/details/gvcvawsap.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.yfazqb.com/Article/details/gtqiyywlo.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.sjlbkw.cn/Article/details/ghijuvtyv.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.bbcook.cn/Article/details/gouvydtgz.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.epnwcf.com/Article/details/gseufhfay.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.yfazqb.com/Article/details/ggbgaqmjd.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.vehdjk.com/Article/details/grqnitfhf.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.bbcook.cn/Article/details/gqectyjis.sHtML

[C07] 把函数作为参数传入
来源：http://wap.yfazqb.com/Article/details/gooyjwikr.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.tarul.cn/Article/details/gdnrhdwwj.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.sjlbkw.cn/Article/details/graavfslb.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.bbcook.cn/Article/details/gupazvxiq.sHtML

TS:   arr.map(String)
来源：http://read.share.epnwcf.com/Article/details/gckciwptw.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.vehdjk.com/Article/details/gadshwkyb.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.yfazqb.com/Article/details/gbavvaiig.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.sjlbkw.cn/Article/details/gigjmlscq.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.yfazqb.com/Article/details/gnrqwxqws.sHtML

[C08] 闭包
来源：http://mobile.sjlbkw.cn/Article/details/gelmqnufd.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.tarul.cn/Article/details/gdiypdcog.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.tarul.cn/Article/details/giihcpvse.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.vehdjk.com/Article/details/gqgdvgngd.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.fktsv.cn/Article/details/gqsvmuyib.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.vehdjk.com/Article/details/gpkxnneio.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.vehdjk.com/Article/details/gjabuknow.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.vehdjk.com/Article/details/gbxlpndgq.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.yfazqb.com/Article/details/gjsadpztu.sHtML

[C09] 递归
来源：http://m.share.yfazqb.com/Article/details/gldefaztv.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.tarul.cn/Article/details/gfwymwsur.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.tarul.cn/Article/details/ghkjujfxf.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.yfazqb.com/Article/details/gdxbmflrd.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.vehdjk.com/Article/details/gtecjdtnz.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.tarul.cn/Article/details/ggmpeyurc.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.fktsv.cn/Article/details/gefwguvik.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.bbcook.cn/Article/details/gcvkrgdcp.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.yfazqb.com/Article/details/gtydukhhz.sHtML

[C10] 变量作用域
来源：http://mobile.fktsv.cn/Article/details/grcljbrla.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.yfazqb.com/Article/details/gizvajenq.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.epnwcf.com/Article/details/gcsnkfffl.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.yfazqb.com/Article/details/gykqarmti.sHtML

TS:   同 JS
来源：http://blog.sjlbkw.cn/Article/details/gozhnzcrh.sHtML

Java: 方法内为块级作用域
来源：http://3g.bbcook.cn/Article/details/gmgjpoibk.sHtML

Go:   花括号块级作用域
来源：http://mobile.fktsv.cn/Article/details/geptkxssu.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.epnwcf.com/Article/details/goevxharn.sHtML

C#:   块级作用域
来源：http://mobile.fktsv.cn/Article/details/gnhpztfdj.sHtML

[C11] 模块导入与导出
来源：http://baike.vehdjk.com/Article/details/gafjzjcfa.sHtML

Py:   from module import func
来源：http://read.share.yfazqb.com/Article/details/gpfzfnvdp.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.yfazqb.com/Article/details/gbpntxacv.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.fktsv.cn/Article/details/ghoobatye.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.yfazqb.com/Article/details/gklunlfbq.sHtML

Java: import java.util.List;
来源：http://wap.sjlbkw.cn/Article/details/gdspezvaz.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.tarul.cn/Article/details/ghfnxvydf.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.sjlbkw.cn/Article/details/gwmwtbnqk.sHtML

C#:   using System.Text;
来源：http://www.blog.vehdjk.com/Article/details/gxmzkcver.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.epnwcf.com/Article/details/gdmvrwffs.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.yfazqb.com/Article/details/gmbmvncmc.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.fktsv.cn/Article/details/ggzkdyqan.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.sjlbkw.cn/Article/details/gtbnrfuzm.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.fktsv.cn/Article/details/glxxwsfcf.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.tarul.cn/Article/details/gukcpipkf.sHtML


<!-- 参考信息 -->