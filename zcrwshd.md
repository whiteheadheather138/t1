代发 wailian999

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://m.share.tarul.cn/Article/details/grjvejkur.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://m.share.vehdjk.com/Article/details/gcwiujhiz.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.blog.yfazqb.com/Article/details/gaebligno.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mobile.epnwcf.com/Article/details/grulydnhv.sHtML

[A26] 类型转换总览
来源：http://blog.epnwcf.com/Article/details/guteiiavq.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mobile.tarul.cn/Article/details/gcnnhmoqh.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://blog.vehdjk.com/Article/details/gyittwjzt.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://blog.vehdjk.com/Article/details/gexwoxhfv.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.m.share.sjlbkw.cn/Article/details/ghhbznjqh.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://read.share.bbcook.cn/Article/details/gxjymaljr.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://blog.tarul.cn/Article/details/gdqmhudss.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://baike.fktsv.cn/Article/details/gqsqlevhn.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://m.share.bbcook.cn/Article/details/grywddmnc.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gtedrpepb.sHtML

B. 流程控制
来源：http://www.m.share.fktsv.cn/Article/details/gbrolyjqj.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gkhvokktc.sHtML

[B01] 条件判断 if / else
来源：http://3g.epnwcf.com/Article/details/gwyaytcca.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://3g.sjlbkw.cn/Article/details/gtkypwnga.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wap.vehdjk.com/Article/details/gypwsicse.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.fktsv.cn/Article/details/gntsijvqx.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.epnwcf.com/Article/details/gtnwgdkwv.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://mobile.sjlbkw.cn/Article/details/gmfbmuxqz.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.share.bbcook.cn/Article/details/goczigoaj.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://m.share.bbcook.cn/Article/details/ghgeoooog.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://3g.vehdjk.com/Article/details/gtjbpucqt.sHtML

[B02] 多分支 else if / elif
来源：http://3g.tarul.cn/Article/details/gfwfvcxan.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wap.bbcook.cn/Article/details/gvyyphvhx.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://3g.tarul.cn/Article/details/gaovwdnvs.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.tarul.cn/Article/details/gahqxczjn.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.sjlbkw.cn/Article/details/gdjygolig.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.fktsv.cn/Article/details/gpgldkhlx.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://baike.bbcook.cn/Article/details/grtnfwqpo.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://blog.epnwcf.com/Article/details/gfkdtudyh.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.epnwcf.com/Article/details/gymjfoyya.sHtML

[B03] switch / match / case
来源：http://baike.epnwcf.com/Article/details/gbnyfdopg.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.epnwcf.com/Article/details/goqlzvrmv.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://baike.vehdjk.com/Article/details/gzxpqjltx.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.epnwcf.com/Article/details/gvczffrxk.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gfmvosfxz.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.yfazqb.com/Article/details/gfflcgfuk.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://3g.epnwcf.com/Article/details/gnbvefjtk.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://m.share.sjlbkw.cn/Article/details/gjoognely.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://blog.tarul.cn/Article/details/ghnkhzdzq.sHtML

[B04] for 计数循环
来源：http://m.share.epnwcf.com/Article/details/gzbebscjw.sHtML

Py:   for i in range(10): print(i)
来源：http://blog.fktsv.cn/Article/details/gluopqohm.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wap.vehdjk.com/Article/details/gcfkqjkeb.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.sjlbkw.cn/Article/details/gekajcicz.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.fktsv.cn/Article/details/gmrncernz.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gkaofdhrc.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mobile.bbcook.cn/Article/details/gyuxfhgzs.sHtML

Ruby: 10.times { |i| puts i }
来源：http://read.share.tarul.cn/Article/details/gaumxsuzg.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mobile.tarul.cn/Article/details/gvnnbpwrs.sHtML

[B05] 遍历数组 / 列表
来源：http://m.share.epnwcf.com/Article/details/goywxoxrq.sHtML

Py:   for item in arr: print(item)
来源：http://www.m.share.yfazqb.com/Article/details/gbtyojqim.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mobile.vehdjk.com/Article/details/geqcvrrej.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://baike.bbcook.cn/Article/details/ghemhddwj.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.tarul.cn/Article/details/grlgaewoq.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://mobile.vehdjk.com/Article/details/gyvggybhh.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wap.yfazqb.com/Article/details/giyijzxde.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.vehdjk.com/Article/details/guhkxpldh.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://3g.epnwcf.com/Article/details/ggllirfzt.sHtML

[B06] 遍历字典 / 对象
来源：http://www.m.share.epnwcf.com/Article/details/gfpuealsj.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://wap.sjlbkw.cn/Article/details/gtfwjfbco.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.yfazqb.com/Article/details/gmsixaulx.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.fktsv.cn/Article/details/gvmrzeyvb.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.sjlbkw.cn/Article/details/glazfzujv.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mobile.epnwcf.com/Article/details/gmfhkdosv.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.tarul.cn/Article/details/gpwjlyibx.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://read.share.fktsv.cn/Article/details/gkjozrcur.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mobile.fktsv.cn/Article/details/gokssfpjv.sHtML

[B07] while 循环
来源：http://wap.vehdjk.com/Article/details/gwwlmwlwm.sHtML

Py:   while i < 10: i += 1
来源：http://wap.bbcook.cn/Article/details/gcpqdevzj.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.tarul.cn/Article/details/grtzsifuu.sHtML

JS:   while (i < 10) { i++; }
来源：http://blog.vehdjk.com/Article/details/gnswygjlw.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.m.share.bbcook.cn/Article/details/gtbpjugno.sHtML

Java: while (i < 10) { i++; }
来源：http://mobile.sjlbkw.cn/Article/details/goyvahzxt.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wap.fktsv.cn/Article/details/goxlulloo.sHtML

Ruby: while i < 10; i += 1; end
来源：http://m.share.sjlbkw.cn/Article/details/gcbjlfmul.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.bbcook.cn/Article/details/ghjlatfrf.sHtML

[B08] do-while（至少执行一次）
来源：http://www.share.bbcook.cn/Article/details/gxoysoaye.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.epnwcf.com/Article/details/gwdudsdko.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.tarul.cn/Article/details/ghvzthifs.sHtML

JS:   do { i++; } while (i < 10);
来源：http://baike.vehdjk.com/Article/details/gsnwxifrw.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.bbcook.cn/Article/details/glqmhvokt.sHtML

Java: do { i++; } while (i < 10);
来源：http://blog.fktsv.cn/Article/details/gftxfedwp.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.fktsv.cn/Article/details/gpojeifwn.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.share.epnwcf.com/Article/details/ghahxkoop.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.bbcook.cn/Article/details/gctvctpof.sHtML

[B09] break 与 continue
来源：http://www.blog.fktsv.cn/Article/details/gixvmmkzq.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.tarul.cn/Article/details/gdnlqhgfz.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.yfazqb.com/Article/details/gxifoibrg.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.yfazqb.com/Article/details/glawtrmfe.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.bbcook.cn/Article/details/guyojcais.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.tarul.cn/Article/details/grwhjqrca.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.tarul.cn/Article/details/glcdflcxm.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.fktsv.cn/Article/details/gurwclfid.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.vehdjk.com/Article/details/gjecxqwdw.sHtML

[B10] 遍历同时拿索引
来源：http://baike.epnwcf.com/Article/details/gqmrrswwc.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.sjlbkw.cn/Article/details/grutwhmzs.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.tarul.cn/Article/details/ghtpzdzul.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://m.share.vehdjk.com/Article/details/gkbqifhsa.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.bbcook.cn/Article/details/gjwqbpcbn.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.sjlbkw.cn/Article/details/goqrijfbj.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.yfazqb.com/Article/details/gffiwrsap.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.bbcook.cn/Article/details/gpxkvxmap.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.fktsv.cn/Article/details/gbnwidftl.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.bbcook.cn/Article/details/gvlyofiej.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.vehdjk.com/Article/details/guzcqixcq.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.tarul.cn/Article/details/gbfeetuvx.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.bbcook.cn/Article/details/gvogssujs.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.fktsv.cn/Article/details/gctmcpaxp.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.fktsv.cn/Article/details/gdaoiuwzn.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.yfazqb.com/Article/details/gjkasdpiv.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.fktsv.cn/Article/details/gpoqcuhku.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.yfazqb.com/Article/details/gblynsdpt.sHtML

[B12] 跳出多层循环
来源：http://baike.epnwcf.com/Article/details/gxqgusmdj.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.epnwcf.com/Article/details/gbvzvbswa.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.yfazqb.com/Article/details/ggvgeeshu.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.fktsv.cn/Article/details/gdgcqupmz.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.bbcook.cn/Article/details/gcedgmpuh.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.tarul.cn/Article/details/gfhktdtyh.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.tarul.cn/Article/details/gxrgsgijg.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.sjlbkw.cn/Article/details/glbjyofro.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.epnwcf.com/Article/details/ggqkdqvhe.sHtML

[B13] 判断是否为数字
来源：http://www.share.yfazqb.com/Article/details/guhiubbcg.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.vehdjk.com/Article/details/gqwkizjpu.sHtML

PHP:  is_numeric($x)
来源：http://m.share.fktsv.cn/Article/details/gswwclcml.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.vehdjk.com/Article/details/guqnifbbm.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.sjlbkw.cn/Article/details/gqfuspbhf.sHtML

Java: x instanceof Number
来源：http://read.share.yfazqb.com/Article/details/gxldylnza.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.tarul.cn/Article/details/gelihfwum.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.bbcook.cn/Article/details/gklhqynbq.sHtML

C#:   x is int or double or decimal
来源：http://mobile.vehdjk.com/Article/details/grbnzjvkl.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.sjlbkw.cn/Article/details/gwknuasez.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.sjlbkw.cn/Article/details/gvpellldm.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.fktsv.cn/Article/details/gklxvnwzm.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.epnwcf.com/Article/details/gzsdzdzjn.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.bbcook.cn/Article/details/gpbcneozn.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.sjlbkw.cn/Article/details/gdhtqjxek.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.epnwcf.com/Article/details/gmcxcjuwg.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.yfazqb.com/Article/details/gmgldcavf.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.vehdjk.com/Article/details/gvpihdylz.sHtML

[B15] 布尔运算与取反
来源：http://3g.vehdjk.com/Article/details/gmyvimece.sHtML

Py:   a and b or not c
来源：http://blog.vehdjk.com/Article/details/gbosemdge.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.fktsv.cn/Article/details/gnyihgyii.sHtML

JS:   a && b || !c
来源：http://mobile.sjlbkw.cn/Article/details/gnzkebsgu.sHtML

TS:   a && b || !c
来源：http://www.m.share.fktsv.cn/Article/details/ggryipdeb.sHtML

Java: a && b || !c
来源：http://m.share.vehdjk.com/Article/details/gcvtiifze.sHtML

Go:   a && b || !c
来源：http://www.share.bbcook.cn/Article/details/gfsgxvffi.sHtML

Ruby: a && b || !c
来源：http://baike.epnwcf.com/Article/details/gtpyqncvj.sHtML

C#:   a && b || !c
来源：http://3g.sjlbkw.cn/Article/details/gvhniyhri.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.sjlbkw.cn/Article/details/gohvadmyt.sHtML

Py:   if not data: return
来源：http://baike.vehdjk.com/Article/details/gxgqlkkfc.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.fktsv.cn/Article/details/gwufrzoib.sHtML

JS:   if (!data) return;
来源：http://wap.yfazqb.com/Article/details/gbxqvcjnq.sHtML

TS:   if (!data) return;
来源：http://read.share.vehdjk.com/Article/details/gyhohuxwt.sHtML

Java: if (data == null) return;
来源：http://m.share.sjlbkw.cn/Article/details/gosjxjwhr.sHtML

Go:   if data == nil { return }
来源：http://baike.sjlbkw.cn/Article/details/gidduotbi.sHtML

Ruby: return if data.nil?
来源：http://mobile.yfazqb.com/Article/details/gqkpvmrsg.sHtML

C#:   if (data == null) return;
来源：http://wap.tarul.cn/Article/details/govzokmrd.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gsupqpsvx.sHtML

C. 函数与作用域
来源：http://www.m.share.yfazqb.com/Article/details/gfuaspzbj.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gobcmxedm.sHtML

[C01] 定义函数
来源：http://blog.bbcook.cn/Article/details/gbhabfiaj.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.tarul.cn/Article/details/gcblkclxl.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.yfazqb.com/Article/details/gunbqlmpy.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.epnwcf.com/Article/details/gnawsvutv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.vehdjk.com/Article/details/gdenugigy.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.fktsv.cn/Article/details/gizwzxcwc.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.yfazqb.com/Article/details/gvbwybdbe.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.yfazqb.com/Article/details/gfdwwsmkz.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.sjlbkw.cn/Article/details/ghwonvwew.sHtML

[C02] 默认参数
来源：http://baike.epnwcf.com/Article/details/gcyvwjbvb.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.fktsv.cn/Article/details/gpzhtdpwv.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.bbcook.cn/Article/details/gwdmgemvi.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.bbcook.cn/Article/details/gzjdymwmf.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.fktsv.cn/Article/details/gjjjoplbs.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.bbcook.cn/Article/details/gegyivsyd.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.yfazqb.com/Article/details/gstefdmjs.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.fktsv.cn/Article/details/gjgcgzvec.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.tarul.cn/Article/details/gkcwvwymc.sHtML

[C03] 可变参数
来源：http://read.share.fktsv.cn/Article/details/gvrxgoqsi.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.bbcook.cn/Article/details/gslqwqmdw.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.fktsv.cn/Article/details/gyibfcmyy.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.tarul.cn/Article/details/ggwqkpuhf.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.tarul.cn/Article/details/glmxsidhk.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.fktsv.cn/Article/details/gyyqbuuga.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.vehdjk.com/Article/details/grjcxfhls.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.yfazqb.com/Article/details/gumjmltnw.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.vehdjk.com/Article/details/gdggyjggf.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.tarul.cn/Article/details/glggjgugl.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.sjlbkw.cn/Article/details/gpsyosroq.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.fktsv.cn/Article/details/gvvnndwbc.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.epnwcf.com/Article/details/gauaxhxmt.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.vehdjk.com/Article/details/gocvsobcp.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.epnwcf.com/Article/details/guktxdbfl.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.tarul.cn/Article/details/gsdijpmej.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.yfazqb.com/Article/details/gnovqsdaz.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.fktsv.cn/Article/details/gfdrbcqbj.sHtML

[C05] 返回多个值
来源：http://3g.epnwcf.com/Article/details/gdwzhhlni.sHtML

Py:   return a, b
来源：http://m.share.bbcook.cn/Article/details/gxeokkgaa.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.epnwcf.com/Article/details/groduenke.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.sjlbkw.cn/Article/details/gipmnxjyz.sHtML

TS:   return { a, b };
来源：http://baike.epnwcf.com/Article/details/gtarcvatt.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.epnwcf.com/Article/details/ggonvisis.sHtML

Go:   return a, b
来源：http://wap.epnwcf.com/Article/details/glxftyhez.sHtML

Ruby: return a, b
来源：http://read.share.yfazqb.com/Article/details/govgsqeio.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.vehdjk.com/Article/details/gsmdhlmud.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.epnwcf.com/Article/details/gxdagzjcq.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.vehdjk.com/Article/details/gwpdknvoo.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.vehdjk.com/Article/details/gmdgznuma.sHtML

JS:   const square = x => x * x;
来源：http://read.share.vehdjk.com/Article/details/geyxmaarv.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.yfazqb.com/Article/details/gonygbnql.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.sjlbkw.cn/Article/details/ggrpylrbb.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.yfazqb.com/Article/details/gledrueex.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.bbcook.cn/Article/details/gobavgzqz.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.yfazqb.com/Article/details/gyaqypevo.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.fktsv.cn/Article/details/gbpvwtrkc.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.yfazqb.com/Article/details/gjnzbqwzf.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.sjlbkw.cn/Article/details/gzeidqemy.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.sjlbkw.cn/Article/details/gcxmnwtqs.sHtML

TS:   arr.map(String)
来源：http://www.m.share.sjlbkw.cn/Article/details/gepnrvodk.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.yfazqb.com/Article/details/gvposziuc.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.epnwcf.com/Article/details/gmvjdowfp.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.bbcook.cn/Article/details/gahygalpe.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.bbcook.cn/Article/details/gvpzfpfrj.sHtML

[C08] 闭包
来源：http://wap.yfazqb.com/Article/details/grwnvizcw.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.epnwcf.com/Article/details/gpybxiuvq.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.sjlbkw.cn/Article/details/giqzkfjcb.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.sjlbkw.cn/Article/details/gmclecdmy.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.tarul.cn/Article/details/gntyxjygg.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.bbcook.cn/Article/details/gpqznsrcr.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.epnwcf.com/Article/details/gvlmjbove.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.sjlbkw.cn/Article/details/gkqxytugv.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.vehdjk.com/Article/details/gkttenluy.sHtML

[C09] 递归
来源：http://www.blog.bbcook.cn/Article/details/gbrxykrrk.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.bbcook.cn/Article/details/gcrlbnoio.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.sjlbkw.cn/Article/details/gwooyeder.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fktsv.cn/Article/details/glznqodpw.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.fktsv.cn/Article/details/gxhzudnkq.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.epnwcf.com/Article/details/gpllsvtgl.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.yfazqb.com/Article/details/gzkubxbhe.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.sjlbkw.cn/Article/details/grffeapqf.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.sjlbkw.cn/Article/details/gqgepmtcm.sHtML

[C10] 变量作用域
来源：http://read.share.vehdjk.com/Article/details/glyphzyot.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.vehdjk.com/Article/details/gfmyiujij.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.vehdjk.com/Article/details/gdnhudgou.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.epnwcf.com/Article/details/gsyprqbot.sHtML

TS:   同 JS
来源：http://www.blog.bbcook.cn/Article/details/gyoelngpf.sHtML

Java: 方法内为块级作用域
来源：http://blog.yfazqb.com/Article/details/guhmuftni.sHtML

Go:   花括号块级作用域
来源：http://mobile.yfazqb.com/Article/details/gcmlumkzk.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.vehdjk.com/Article/details/gnzuaoxer.sHtML

C#:   块级作用域
来源：http://m.share.tarul.cn/Article/details/glmgdtdzo.sHtML

[C11] 模块导入与导出
来源：http://3g.epnwcf.com/Article/details/gkbsbyrik.sHtML

Py:   from module import func
来源：http://www.blog.yfazqb.com/Article/details/gwqmptiac.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.yfazqb.com/Article/details/gcwhxpucl.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.epnwcf.com/Article/details/gagksvtrj.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.tarul.cn/Article/details/gbxaibver.sHtML

Java: import java.util.List;
来源：http://blog.bbcook.cn/Article/details/gswmuasgs.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.fktsv.cn/Article/details/gcqchlszy.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.bbcook.cn/Article/details/gyhocibty.sHtML

C#:   using System.Text;
来源：http://www.m.share.bbcook.cn/Article/details/gojaocten.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.sjlbkw.cn/Article/details/gqnmapgun.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.yfazqb.com/Article/details/gdhomjzok.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.fktsv.cn/Article/details/gtkwphetu.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.tarul.cn/Article/details/grtoyzrtu.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.yfazqb.com/Article/details/gdwwyxfwv.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.sjlbkw.cn/Article/details/geopptdmh.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.bbcook.cn/Article/details/gupqldluh.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.tarul.cn/Article/details/gkdaqrdti.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.yfazqb.com/Article/details/gpnojpmos.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.fktsv.cn/Article/details/gkdxokeyk.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.vehdjk.com/Article/details/ghhllvwar.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.yfazqb.com/Article/details/gskdpprif.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.tarul.cn/Article/details/gzwzyaooh.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.sjlbkw.cn/Article/details/gafmktipf.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.fktsv.cn/Article/details/gxmwxewmy.sHtML

Go:   func add(a, b int) int
来源：http://mobile.bbcook.cn/Article/details/gsufqjfme.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.tarul.cn/Article/details/gkunzhroa.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.fktsv.cn/Article/details/gmkhbncvl.sHtML

[C14] 泛型函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gfeicfmzv.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.fktsv.cn/Article/details/gujvfmwdd.sHtML

PHP:  // 无泛型
来源：http://wap.bbcook.cn/Article/details/gapvozihu.sHtML

JS:   // 无泛型
来源：http://www.blog.bbcook.cn/Article/details/gzlzjqdhi.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.sjlbkw.cn/Article/details/givpqjzei.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.sjlbkw.cn/Article/details/gvuhwvdds.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.tarul.cn/Article/details/gybshfodz.sHtML

Ruby: # 无泛型
来源：http://blog.vehdjk.com/Article/details/gzzjkhzjd.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.vehdjk.com/Article/details/gzkcchjpq.sHtML

[C15] 解构 / 展开参数
来源：http://blog.tarul.cn/Article/details/gwqccfdxn.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.vehdjk.com/Article/details/gfdfleiyl.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.bbcook.cn/Article/details/gjmiepqlu.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.sjlbkw.cn/Article/details/ghsstmmwk.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.bbcook.cn/Article/details/gulrkazaq.sHtML

Java: // 无解构
来源：http://mobile.fktsv.cn/Article/details/gzimnsgwu.sHtML

Go:   // 无解构
来源：http://wap.epnwcf.com/Article/details/gynqsrrhd.sHtML

Ruby: a, b = pair
来源：http://mobile.fktsv.cn/Article/details/gpmrjjjkp.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.tarul.cn/Article/details/giftgygrr.sHtML

[C16] 函数 / 方法重载
来源：http://baike.vehdjk.com/Article/details/gdkgtzdbj.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.yfazqb.com/Article/details/gtwjuehcs.sHtML


<!-- 参考信息 -->