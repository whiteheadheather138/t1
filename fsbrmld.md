代发 wailian999

[A22] 获取字符串长度
来源：http://read.share.fktsv.cn/Article/details/gtnwnvwwr.sHtML

Py:   len(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gicqjrmbc.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.m.share.vehdjk.com/Article/details/gtiawzman.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mobile.sjlbkw.cn/Article/details/gznjijasq.sHtML

TS:   s.length
来源：http://www.blog.vehdjk.com/Article/details/ggmdeqwdk.sHtML

Java: s.length()
来源：http://www.m.share.sjlbkw.cn/Article/details/gabderpue.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mobile.epnwcf.com/Article/details/gmyyirjae.sHtML

Ruby: s.length
来源：http://blog.bbcook.cn/Article/details/gfkmofrgd.sHtML

C#:   s.Length
来源：http://www.m.share.epnwcf.com/Article/details/gnzcesnuj.sHtML

[A23] 大小写转换
来源：http://wap.bbcook.cn/Article/details/glhjwbhos.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.share.yfazqb.com/Article/details/gktdvypyv.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://3g.bbcook.cn/Article/details/gijwzlvbu.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.epnwcf.com/Article/details/gpfitobvq.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.sjlbkw.cn/Article/details/gxmdbrtzg.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://blog.sjlbkw.cn/Article/details/gawmssphv.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mobile.fktsv.cn/Article/details/gocxduroe.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://baike.sjlbkw.cn/Article/details/gbgbgawjc.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://baike.yfazqb.com/Article/details/gsbviflbj.sHtML

[A24] 去除首尾空白
来源：http://3g.yfazqb.com/Article/details/gissgwsjt.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wap.vehdjk.com/Article/details/gwsuprlwv.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://baike.tarul.cn/Article/details/gtvhhodqz.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.sjlbkw.cn/Article/details/gpeslumlj.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.bbcook.cn/Article/details/gdbflwasw.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.m.share.yfazqb.com/Article/details/gxrhcccda.sHtML

Go:   strings.TrimSpace(s)
来源：http://baike.yfazqb.com/Article/details/gdubavhym.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://read.share.epnwcf.com/Article/details/gapchhimz.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://m.share.yfazqb.com/Article/details/gjrsrjwxj.sHtML

[A25] 字符串比较
来源：http://blog.yfazqb.com/Article/details/gkxsknhyq.sHtML

Py:   s1 == s2; s1 != s2
来源：http://read.share.vehdjk.com/Article/details/gyrscwyok.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://blog.fktsv.cn/Article/details/goibdwwfx.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.bbcook.cn/Article/details/guesfuwmg.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.tarul.cn/Article/details/gnkzkounj.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://baike.fktsv.cn/Article/details/gbrqrbtao.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.m.share.fktsv.cn/Article/details/gejxdeswd.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://wap.bbcook.cn/Article/details/ggjrvouqe.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.m.share.fktsv.cn/Article/details/gmcnhywcn.sHtML

[A26] 类型转换总览
来源：http://www.m.share.epnwcf.com/Article/details/gbzxvnsfd.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://read.share.fktsv.cn/Article/details/gwgglqsyh.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://m.share.sjlbkw.cn/Article/details/gtehlwydv.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wap.yfazqb.com/Article/details/gyuelnlfm.sHtML

TS:   Number() String() Boolean() x as number
来源：http://3g.fktsv.cn/Article/details/grsqecfyo.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://blog.tarul.cn/Article/details/gkcukowqn.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.blog.vehdjk.com/Article/details/gfsxtjprh.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://read.share.fktsv.cn/Article/details/gmxdtaksi.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://m.share.yfazqb.com/Article/details/gpqeotkjo.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/ghtwzmsex.sHtML

B. 流程控制
来源：http://baike.fktsv.cn/Article/details/gqttshejk.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/grfuyynyz.sHtML

[B01] 条件判断 if / else
来源：http://3g.fktsv.cn/Article/details/gzemrlhml.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://baike.epnwcf.com/Article/details/gyqixcltt.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://baike.vehdjk.com/Article/details/guzffhtrw.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.sjlbkw.cn/Article/details/gwvevezza.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.vehdjk.com/Article/details/gaflqlgne.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://mobile.bbcook.cn/Article/details/gqujdqclr.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://blog.yfazqb.com/Article/details/gmzenvooa.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://blog.vehdjk.com/Article/details/glwozbswe.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://3g.fktsv.cn/Article/details/gmvjlyytg.sHtML

[B02] 多分支 else if / elif
来源：http://www.m.share.bbcook.cn/Article/details/ggpcgrexf.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wap.yfazqb.com/Article/details/gxytfafhq.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://blog.sjlbkw.cn/Article/details/gkzgnpwxv.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.tarul.cn/Article/details/gsfttjlhh.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.tarul.cn/Article/details/gskobsfcs.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.yfazqb.com/Article/details/ggpmpmwjn.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.blog.epnwcf.com/Article/details/glhjvhvnt.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://baike.tarul.cn/Article/details/gwtjymton.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.sjlbkw.cn/Article/details/gkdkdxvgr.sHtML

[B03] switch / match / case
来源：http://blog.epnwcf.com/Article/details/gntdsjpyi.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://m.share.epnwcf.com/Article/details/gtaszcnqe.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.m.share.vehdjk.com/Article/details/gwqjvahqx.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.epnwcf.com/Article/details/gszekains.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.vehdjk.com/Article/details/gurjohwbz.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.m.share.bbcook.cn/Article/details/ghpyjwchx.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.share.tarul.cn/Article/details/gzlqgvngn.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.m.share.sjlbkw.cn/Article/details/gcyhdztyo.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://blog.epnwcf.com/Article/details/gjyhylyiy.sHtML

[B04] for 计数循环
来源：http://www.blog.vehdjk.com/Article/details/gdgvxyjyb.sHtML

Py:   for i in range(10): print(i)
来源：http://blog.vehdjk.com/Article/details/gvysfqiqd.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://blog.sjlbkw.cn/Article/details/ghwzorxbn.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.epnwcf.com/Article/details/gbsjqhucc.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.yfazqb.com/Article/details/gknferaqc.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://3g.vehdjk.com/Article/details/gmmcxbomb.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://read.share.epnwcf.com/Article/details/glymiychb.sHtML

Ruby: 10.times { |i| puts i }
来源：http://blog.epnwcf.com/Article/details/gqqwczcys.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.blog.epnwcf.com/Article/details/gihitaibi.sHtML

[B05] 遍历数组 / 列表
来源：http://wap.bbcook.cn/Article/details/gbzeomqhd.sHtML

Py:   for item in arr: print(item)
来源：http://read.share.bbcook.cn/Article/details/gkwaotmve.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://blog.tarul.cn/Article/details/gmnmnciol.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.yfazqb.com/Article/details/gpibeayjv.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://m.share.yfazqb.com/Article/details/garkjmhfy.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://mobile.epnwcf.com/Article/details/gdofgasyk.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mobile.tarul.cn/Article/details/gzdfrigqp.sHtML

Ruby: arr.each { |item| puts item }
来源：http://m.share.fktsv.cn/Article/details/gapqwyzct.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mobile.tarul.cn/Article/details/glmrulqcq.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.tarul.cn/Article/details/glyseygev.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://3g.fktsv.cn/Article/details/gzmzfklmy.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://baike.bbcook.cn/Article/details/gxkbonkbx.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.vehdjk.com/Article/details/gjvwteiyg.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.fktsv.cn/Article/details/gdkgmrogl.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mobile.fktsv.cn/Article/details/gunaxjlzz.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.tarul.cn/Article/details/ghusglfsp.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.fktsv.cn/Article/details/gwkfbpvtz.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wap.epnwcf.com/Article/details/geakqflew.sHtML

[B07] while 循环
来源：http://mobile.bbcook.cn/Article/details/guzlpijkx.sHtML

Py:   while i < 10: i += 1
来源：http://m.share.tarul.cn/Article/details/gsoomalwy.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.yfazqb.com/Article/details/gqiwkuxln.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.sjlbkw.cn/Article/details/greqymvqb.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.tarul.cn/Article/details/gflyobwon.sHtML

Java: while (i < 10) { i++; }
来源：http://wap.bbcook.cn/Article/details/gznabsobt.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.tarul.cn/Article/details/gzolzrpzv.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.sjlbkw.cn/Article/details/geteknicw.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.vehdjk.com/Article/details/gpfnagais.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.yfazqb.com/Article/details/gsueifhyu.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.tarul.cn/Article/details/giyetecss.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.yfazqb.com/Article/details/gnuwkpddz.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.epnwcf.com/Article/details/gnmwnkrvo.sHtML

TS:   do { i++; } while (i < 10);
来源：http://baike.vehdjk.com/Article/details/gdsmnxwku.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.blog.epnwcf.com/Article/details/gmqbaybxj.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.sjlbkw.cn/Article/details/gsqkifuvd.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.bbcook.cn/Article/details/gkmdcsbox.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.epnwcf.com/Article/details/gtjoezeeh.sHtML

[B09] break 与 continue
来源：http://mobile.bbcook.cn/Article/details/gyxuwozcg.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.vehdjk.com/Article/details/gfehmjekt.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://m.share.fktsv.cn/Article/details/gfmocsice.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.yfazqb.com/Article/details/gpnyacvcf.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.yfazqb.com/Article/details/glgsrqwnf.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.vehdjk.com/Article/details/gqvwounpt.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.yfazqb.com/Article/details/gygnwfmtx.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.epnwcf.com/Article/details/ggmisqhba.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.sjlbkw.cn/Article/details/ggwzuwwhj.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.sjlbkw.cn/Article/details/gdeykndns.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.vehdjk.com/Article/details/gixdhvtgz.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.sjlbkw.cn/Article/details/gqgyjbcpy.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://m.share.vehdjk.com/Article/details/gadpucwcc.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.epnwcf.com/Article/details/gvoraenuz.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.bbcook.cn/Article/details/gwmnfprnm.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.sjlbkw.cn/Article/details/ghbsamamn.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.bbcook.cn/Article/details/ggsufsypj.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.tarul.cn/Article/details/gqthfabok.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.epnwcf.com/Article/details/glrewlxdz.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.epnwcf.com/Article/details/gxpngrxrq.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.yfazqb.com/Article/details/gjgywodpr.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.fktsv.cn/Article/details/gvodnvgua.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.fktsv.cn/Article/details/gnmftanen.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.yfazqb.com/Article/details/gwbaphngc.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.bbcook.cn/Article/details/gcmcxzqjz.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.tarul.cn/Article/details/gwlhncqdh.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.epnwcf.com/Article/details/gvowdoupi.sHtML

[B12] 跳出多层循环
来源：http://baike.vehdjk.com/Article/details/glghvggxo.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.vehdjk.com/Article/details/gmianyxng.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.sjlbkw.cn/Article/details/ghbljjufo.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.epnwcf.com/Article/details/gqkadvtzz.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.sjlbkw.cn/Article/details/gnpuuogoo.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.epnwcf.com/Article/details/gnmlkkpnm.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.bbcook.cn/Article/details/geumyjilr.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.yfazqb.com/Article/details/gnqxqtuly.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.sjlbkw.cn/Article/details/gmbllhplu.sHtML

[B13] 判断是否为数字
来源：http://3g.yfazqb.com/Article/details/gcawwixmu.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.tarul.cn/Article/details/grejiqiwf.sHtML

PHP:  is_numeric($x)
来源：http://read.share.bbcook.cn/Article/details/gqxuyoobt.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.vehdjk.com/Article/details/gcpxrjray.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.bbcook.cn/Article/details/ghlcndozd.sHtML

Java: x instanceof Number
来源：http://read.share.yfazqb.com/Article/details/gwxwquhrx.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.tarul.cn/Article/details/gucmngome.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.epnwcf.com/Article/details/glmfmzwad.sHtML

C#:   x is int or double or decimal
来源：http://wap.fktsv.cn/Article/details/guagoiabr.sHtML

[B14] 判断值是否在集合内
来源：http://blog.tarul.cn/Article/details/gryqhrmnw.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.bbcook.cn/Article/details/gjhkxtiyf.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.bbcook.cn/Article/details/gwkfchabg.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.epnwcf.com/Article/details/ghlvdazoz.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.epnwcf.com/Article/details/ggpfivhvn.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.bbcook.cn/Article/details/gzrxvscbs.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.yfazqb.com/Article/details/gjxcqmzcq.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.bbcook.cn/Article/details/gikansaht.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.yfazqb.com/Article/details/gonangsyq.sHtML

[B15] 布尔运算与取反
来源：http://mobile.sjlbkw.cn/Article/details/gvhbbydbt.sHtML

Py:   a and b or not c
来源：http://m.share.epnwcf.com/Article/details/gmjphpaze.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.epnwcf.com/Article/details/goaflzqtd.sHtML

JS:   a && b || !c
来源：http://mobile.tarul.cn/Article/details/gscxkbynp.sHtML

TS:   a && b || !c
来源：http://www.share.sjlbkw.cn/Article/details/geyetklft.sHtML

Java: a && b || !c
来源：http://wap.tarul.cn/Article/details/gdazccrgh.sHtML

Go:   a && b || !c
来源：http://baike.epnwcf.com/Article/details/ghsrxbpvf.sHtML

Ruby: a && b || !c
来源：http://www.blog.bbcook.cn/Article/details/gldshdrez.sHtML

C#:   a && b || !c
来源：http://m.share.sjlbkw.cn/Article/details/gjfifmcvh.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.tarul.cn/Article/details/gigfcvbcp.sHtML

Py:   if not data: return
来源：http://read.share.tarul.cn/Article/details/gsjyeywum.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.sjlbkw.cn/Article/details/ggkoccuul.sHtML

JS:   if (!data) return;
来源：http://baike.bbcook.cn/Article/details/gmydlqotg.sHtML

TS:   if (!data) return;
来源：http://3g.tarul.cn/Article/details/gibumkuyb.sHtML

Java: if (data == null) return;
来源：http://wap.tarul.cn/Article/details/gqlwkkxad.sHtML

Go:   if data == nil { return }
来源：http://wap.yfazqb.com/Article/details/gxmvfzxzm.sHtML

Ruby: return if data.nil?
来源：http://read.share.fktsv.cn/Article/details/gvggbkrrr.sHtML

C#:   if (data == null) return;
来源：http://www.share.fktsv.cn/Article/details/gnijyxxqb.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gutknmdog.sHtML

C. 函数与作用域
来源：http://www.m.share.fktsv.cn/Article/details/gcpgzvxdc.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/giaedptct.sHtML

[C01] 定义函数
来源：http://3g.bbcook.cn/Article/details/guzznsdyy.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.fktsv.cn/Article/details/gtjhxbhld.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fktsv.cn/Article/details/gzvpveqdl.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.sjlbkw.cn/Article/details/gbwamlydb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.tarul.cn/Article/details/gvummozaa.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.fktsv.cn/Article/details/gdfppphdc.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.tarul.cn/Article/details/ggfvuhipx.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.sjlbkw.cn/Article/details/guroljnah.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.bbcook.cn/Article/details/gmuipnlai.sHtML

[C02] 默认参数
来源：http://mobile.vehdjk.com/Article/details/guptuylwp.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.sjlbkw.cn/Article/details/geofmdlom.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.fktsv.cn/Article/details/gudccegmq.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.yfazqb.com/Article/details/gpaaaswtw.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.tarul.cn/Article/details/gylomacbp.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.tarul.cn/Article/details/gxgscicsc.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.fktsv.cn/Article/details/gdajyrusx.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.vehdjk.com/Article/details/ginpomfmc.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.sjlbkw.cn/Article/details/giuxlikwg.sHtML

[C03] 可变参数
来源：http://www.share.tarul.cn/Article/details/gvkfxwgjh.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.yfazqb.com/Article/details/gtlflytha.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.vehdjk.com/Article/details/gglhfelzn.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.sjlbkw.cn/Article/details/grcukvuix.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.bbcook.cn/Article/details/gnsuelwca.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.vehdjk.com/Article/details/ggrjottqr.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.yfazqb.com/Article/details/gqcomvmvm.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.bbcook.cn/Article/details/glsvvyxei.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.bbcook.cn/Article/details/gmvcvpbea.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.bbcook.cn/Article/details/gjsfvafoj.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.epnwcf.com/Article/details/gffkupolt.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.tarul.cn/Article/details/gfselhemz.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.vehdjk.com/Article/details/grrfkaiyt.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.bbcook.cn/Article/details/gwmmuighr.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.epnwcf.com/Article/details/gzbjwqqho.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.fktsv.cn/Article/details/gehbnurnp.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.bbcook.cn/Article/details/grjcinqbw.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.vehdjk.com/Article/details/gyogcepnj.sHtML

[C05] 返回多个值
来源：http://mobile.vehdjk.com/Article/details/gojoouxmr.sHtML

Py:   return a, b
来源：http://www.m.share.fktsv.cn/Article/details/gchlqlbeg.sHtML

PHP:  return [$a, $b];
来源：http://mobile.bbcook.cn/Article/details/gvxxfobwl.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.fktsv.cn/Article/details/gabjvlonq.sHtML

TS:   return { a, b };
来源：http://3g.vehdjk.com/Article/details/giheroreq.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.fktsv.cn/Article/details/ghcfbgwnd.sHtML

Go:   return a, b
来源：http://blog.epnwcf.com/Article/details/gecwcsenb.sHtML

Ruby: return a, b
来源：http://www.share.fktsv.cn/Article/details/gpoognaya.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.yfazqb.com/Article/details/gkeawvdei.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.vehdjk.com/Article/details/gwfftybpz.sHtML

Py:   square = lambda x: x * x
来源：http://baike.tarul.cn/Article/details/gopasaznw.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.yfazqb.com/Article/details/gvuqyjhlo.sHtML

JS:   const square = x => x * x;
来源：http://www.share.vehdjk.com/Article/details/gbagzssgi.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.yfazqb.com/Article/details/gawiouhvn.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.epnwcf.com/Article/details/giucnqpmv.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.yfazqb.com/Article/details/ghhgdddjd.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.fktsv.cn/Article/details/ggvcybrqx.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.vehdjk.com/Article/details/gmyzrmiir.sHtML

[C07] 把函数作为参数传入
来源：http://blog.sjlbkw.cn/Article/details/gjqvncgva.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.vehdjk.com/Article/details/gduiaojyl.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.bbcook.cn/Article/details/gclvqpfwu.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.bbcook.cn/Article/details/gjleuefms.sHtML

TS:   arr.map(String)
来源：http://3g.fktsv.cn/Article/details/ghylejzqk.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.sjlbkw.cn/Article/details/gqqpuajcb.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.yfazqb.com/Article/details/gvuyywkle.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.vehdjk.com/Article/details/gtfomzosv.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.sjlbkw.cn/Article/details/gdlvkdcku.sHtML

[C08] 闭包
来源：http://m.share.vehdjk.com/Article/details/gqeppjunw.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.fktsv.cn/Article/details/gagznrslu.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.vehdjk.com/Article/details/gkozgtmei.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.sjlbkw.cn/Article/details/gothfrcye.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.fktsv.cn/Article/details/glsjmqmse.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.fktsv.cn/Article/details/guvuzvpsj.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.sjlbkw.cn/Article/details/gvsqhcyil.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.vehdjk.com/Article/details/gsjadqvaj.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.yfazqb.com/Article/details/gztastqyy.sHtML

[C09] 递归
来源：http://wap.epnwcf.com/Article/details/gzbceidvd.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.tarul.cn/Article/details/gwznnalud.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.epnwcf.com/Article/details/geqgeriau.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.sjlbkw.cn/Article/details/getpksdov.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.epnwcf.com/Article/details/gttnjrgro.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.bbcook.cn/Article/details/glzgpfnvy.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.yfazqb.com/Article/details/gihrezree.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.yfazqb.com/Article/details/gsgkeiygk.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.fktsv.cn/Article/details/gvyszvbrh.sHtML

[C10] 变量作用域
来源：http://blog.epnwcf.com/Article/details/gvlixicoj.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.sjlbkw.cn/Article/details/getgsulul.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.tarul.cn/Article/details/gvngytpew.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.bbcook.cn/Article/details/gakrmlaia.sHtML

TS:   同 JS
来源：http://wap.tarul.cn/Article/details/gitdcqphr.sHtML

Java: 方法内为块级作用域
来源：http://3g.bbcook.cn/Article/details/gfwufcmyb.sHtML

Go:   花括号块级作用域
来源：http://mobile.sjlbkw.cn/Article/details/grqyilziu.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.sjlbkw.cn/Article/details/gwketyhkv.sHtML

C#:   块级作用域
来源：http://www.share.yfazqb.com/Article/details/gmirlhjan.sHtML

[C11] 模块导入与导出
来源：http://read.share.yfazqb.com/Article/details/gujqneuzr.sHtML

Py:   from module import func
来源：http://m.share.fktsv.cn/Article/details/gwbvcqasd.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.bbcook.cn/Article/details/gvqygmwtv.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.tarul.cn/Article/details/glarsmyuz.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.vehdjk.com/Article/details/gmccsxkfp.sHtML

Java: import java.util.List;
来源：http://read.share.bbcook.cn/Article/details/geiyryhje.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.fktsv.cn/Article/details/gwrjylsgg.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.tarul.cn/Article/details/gkocpelqp.sHtML

C#:   using System.Text;
来源：http://baike.yfazqb.com/Article/details/gmmxjqita.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.vehdjk.com/Article/details/gbylzlewf.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.vehdjk.com/Article/details/gtmkszpru.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.sjlbkw.cn/Article/details/gxpiygvcw.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.tarul.cn/Article/details/gxpohispy.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.sjlbkw.cn/Article/details/gnfaunxtq.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.vehdjk.com/Article/details/gxwikngsc.sHtML


<!-- 参考信息 -->