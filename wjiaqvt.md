代发 wailian999

TS:   Number() String() Boolean() x as number
来源：http://www.m.share.tarul.cn/Article/details/godmcyrqc.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.share.bbcook.cn/Article/details/ghpimgoja.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.share.sjlbkw.cn/Article/details/gnxyubaah.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://3g.bbcook.cn/Article/details/gnhmmsxqo.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://read.share.tarul.cn/Article/details/ggalhodgf.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gssgwaoee.sHtML

B. 流程控制
来源：http://www.m.share.epnwcf.com/Article/details/gwquvzwmi.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gktnfdshm.sHtML

[B01] 条件判断 if / else
来源：http://wap.tarul.cn/Article/details/gvdjtounw.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.m.share.fktsv.cn/Article/details/gjqxxhpwa.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://blog.bbcook.cn/Article/details/gbgwcrdpd.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.vehdjk.com/Article/details/ghltrllcl.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.tarul.cn/Article/details/gvslyrklo.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://baike.sjlbkw.cn/Article/details/gurexnrre.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://baike.epnwcf.com/Article/details/gsvuoeftr.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.blog.vehdjk.com/Article/details/glfjngrpi.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.m.share.bbcook.cn/Article/details/ghapiaetn.sHtML

[B02] 多分支 else if / elif
来源：http://m.share.sjlbkw.cn/Article/details/grnqldvkb.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://3g.fktsv.cn/Article/details/geqrosrgh.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://blog.bbcook.cn/Article/details/guqhdfnwv.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.yfazqb.com/Article/details/gmuasohhv.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.bbcook.cn/Article/details/gimdaylfy.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.epnwcf.com/Article/details/gausytfuv.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://3g.bbcook.cn/Article/details/gexawgqzv.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://baike.yfazqb.com/Article/details/ghzhnyhwb.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.sjlbkw.cn/Article/details/gpyruhvcf.sHtML

[B03] switch / match / case
来源：http://read.share.vehdjk.com/Article/details/gimgwpimd.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.share.yfazqb.com/Article/details/gvivitksm.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.m.share.yfazqb.com/Article/details/gaqyfwdgk.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.vehdjk.com/Article/details/glgszykzf.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.vehdjk.com/Article/details/gxzxhnbnd.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://m.share.fktsv.cn/Article/details/gfhdajqpo.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://baike.tarul.cn/Article/details/gqrnyidun.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://baike.bbcook.cn/Article/details/ghfsrwlmn.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.share.tarul.cn/Article/details/gwcpcabmu.sHtML

[B04] for 计数循环
来源：http://blog.tarul.cn/Article/details/gwoahpcbq.sHtML

Py:   for i in range(10): print(i)
来源：http://www.share.sjlbkw.cn/Article/details/gmsfptoqi.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.m.share.vehdjk.com/Article/details/ghjqaqkkn.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.vehdjk.com/Article/details/gdwifbstb.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.bbcook.cn/Article/details/gouvqqaga.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mobile.sjlbkw.cn/Article/details/gbtmjjqrx.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.m.share.tarul.cn/Article/details/gbvygowye.sHtML

Ruby: 10.times { |i| puts i }
来源：http://mobile.tarul.cn/Article/details/guicclmxj.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://m.share.bbcook.cn/Article/details/ghkorfxiv.sHtML

[B05] 遍历数组 / 列表
来源：http://www.share.bbcook.cn/Article/details/gfqpqlcxn.sHtML

Py:   for item in arr: print(item)
来源：http://wap.fktsv.cn/Article/details/ggqnnfysh.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://m.share.vehdjk.com/Article/details/gyqglgmlu.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://read.share.tarul.cn/Article/details/ggulhvdpr.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.tarul.cn/Article/details/gashlkeoj.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://baike.sjlbkw.cn/Article/details/gincgzwcy.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.blog.bbcook.cn/Article/details/ghjbhczcb.sHtML

Ruby: arr.each { |item| puts item }
来源：http://mobile.tarul.cn/Article/details/ggndmrpsr.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gjxsvrpme.sHtML

[B06] 遍历字典 / 对象
来源：http://www.m.share.epnwcf.com/Article/details/gbbximecv.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.tarul.cn/Article/details/gzwsxgyey.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://3g.yfazqb.com/Article/details/gzisnlxvh.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.fktsv.cn/Article/details/gzfiqqysu.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.tarul.cn/Article/details/gwszlmjao.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://blog.tarul.cn/Article/details/gwzybwyaq.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.epnwcf.com/Article/details/grrsmzaph.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.vehdjk.com/Article/details/gyzocxoxu.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wap.vehdjk.com/Article/details/gkjunlvgb.sHtML

[B07] while 循环
来源：http://baike.bbcook.cn/Article/details/gdnpiiiif.sHtML

Py:   while i < 10: i += 1
来源：http://blog.sjlbkw.cn/Article/details/gqmweblqr.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.bbcook.cn/Article/details/gnaskxllu.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.tarul.cn/Article/details/gplirqvrs.sHtML

TS:   while (i < 10) { i++; }
来源：http://mobile.fktsv.cn/Article/details/gmdcjjosy.sHtML

Java: while (i < 10) { i++; }
来源：http://mobile.sjlbkw.cn/Article/details/grislmowo.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.sjlbkw.cn/Article/details/gpzqssclm.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.tarul.cn/Article/details/gnemixgef.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.vehdjk.com/Article/details/gmnagstgn.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.yfazqb.com/Article/details/gdqvzrbhl.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://mobile.vehdjk.com/Article/details/gbzomvywl.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.bbcook.cn/Article/details/gyxtfayjc.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.sjlbkw.cn/Article/details/gzqsdxwfk.sHtML

TS:   do { i++; } while (i < 10);
来源：http://baike.bbcook.cn/Article/details/gtcqmdkot.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.share.sjlbkw.cn/Article/details/gyesspyvv.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://read.share.sjlbkw.cn/Article/details/gvgxayitd.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.sjlbkw.cn/Article/details/ghgsixsev.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.bbcook.cn/Article/details/gbrawvrtl.sHtML

[B09] break 与 continue
来源：http://www.m.share.epnwcf.com/Article/details/gaejbsmmr.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.epnwcf.com/Article/details/gjkrdvqwu.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.tarul.cn/Article/details/gdwpktwwl.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.yfazqb.com/Article/details/gskejwzen.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.sjlbkw.cn/Article/details/grqdpszff.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.vehdjk.com/Article/details/gxdnlfnbw.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.vehdjk.com/Article/details/gfrsaruwb.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.yfazqb.com/Article/details/gwwefwxbt.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.tarul.cn/Article/details/gkjafcyno.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.vehdjk.com/Article/details/gdgamysri.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.fktsv.cn/Article/details/gcbzvhioa.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.yfazqb.com/Article/details/gegnkiiba.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.yfazqb.com/Article/details/gpvhabtzy.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.epnwcf.com/Article/details/gdaihrkql.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.vehdjk.com/Article/details/ganqhwvvx.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.bbcook.cn/Article/details/gfrbcosmr.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.sjlbkw.cn/Article/details/gqvubjiys.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.yfazqb.com/Article/details/gvttynauf.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.fktsv.cn/Article/details/gkirwkzjp.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.yfazqb.com/Article/details/grvppmojo.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.sjlbkw.cn/Article/details/gfnkclvis.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.epnwcf.com/Article/details/grmwnfczb.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.yfazqb.com/Article/details/gxshyeabp.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.vehdjk.com/Article/details/gfcinyaxr.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.vehdjk.com/Article/details/glkxzhhqw.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.epnwcf.com/Article/details/gcbwmxbig.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.sjlbkw.cn/Article/details/gwpuurpwn.sHtML

[B12] 跳出多层循环
来源：http://www.blog.fktsv.cn/Article/details/gfgyyarkp.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.bbcook.cn/Article/details/gtmvwrghl.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.bbcook.cn/Article/details/gryjvkcqx.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fktsv.cn/Article/details/gjtuqrqvt.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.sjlbkw.cn/Article/details/gdpjcwfmg.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.yfazqb.com/Article/details/gmkqzjyjc.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.fktsv.cn/Article/details/gafzmjwav.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.yfazqb.com/Article/details/goohihpeo.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.yfazqb.com/Article/details/gqdspcsqt.sHtML

[B13] 判断是否为数字
来源：http://baike.vehdjk.com/Article/details/grmbtqcuj.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.epnwcf.com/Article/details/gtkgobggq.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.tarul.cn/Article/details/gjfpxzcof.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.epnwcf.com/Article/details/gcfmnotwb.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.tarul.cn/Article/details/gklkgtpoa.sHtML

Java: x instanceof Number
来源：http://mobile.yfazqb.com/Article/details/gtinleywo.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.vehdjk.com/Article/details/gvqdlqcae.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.tarul.cn/Article/details/gujjqklis.sHtML

C#:   x is int or double or decimal
来源：http://3g.epnwcf.com/Article/details/gnbbmaezq.sHtML

[B14] 判断值是否在集合内
来源：http://blog.yfazqb.com/Article/details/gffjuuiak.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.fktsv.cn/Article/details/glqqshadf.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.epnwcf.com/Article/details/gmzslzzje.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.yfazqb.com/Article/details/gwkicjwoj.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.epnwcf.com/Article/details/guoaimjmw.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.epnwcf.com/Article/details/gxrlukoka.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.tarul.cn/Article/details/ghqqglhji.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.fktsv.cn/Article/details/gbmzeedqc.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.sjlbkw.cn/Article/details/gfvqlwzpr.sHtML

[B15] 布尔运算与取反
来源：http://3g.bbcook.cn/Article/details/gipuqkcih.sHtML

Py:   a and b or not c
来源：http://www.blog.tarul.cn/Article/details/gvkgvhfte.sHtML

PHP:  $a && $b || !$c
来源：http://blog.vehdjk.com/Article/details/gcjazxltx.sHtML

JS:   a && b || !c
来源：http://mobile.bbcook.cn/Article/details/gnfaxairz.sHtML

TS:   a && b || !c
来源：http://mobile.vehdjk.com/Article/details/glrzdqcgh.sHtML

Java: a && b || !c
来源：http://www.share.vehdjk.com/Article/details/gzlijgnzd.sHtML

Go:   a && b || !c
来源：http://baike.sjlbkw.cn/Article/details/gtdhqgban.sHtML

Ruby: a && b || !c
来源：http://www.blog.epnwcf.com/Article/details/gzxrxyjcd.sHtML

C#:   a && b || !c
来源：http://read.share.bbcook.cn/Article/details/gwcelubmo.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.fktsv.cn/Article/details/gcepuoyef.sHtML

Py:   if not data: return
来源：http://wap.bbcook.cn/Article/details/gldrtfxoa.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.bbcook.cn/Article/details/gzhepsini.sHtML

JS:   if (!data) return;
来源：http://baike.yfazqb.com/Article/details/gyhfhuwxx.sHtML

TS:   if (!data) return;
来源：http://wap.vehdjk.com/Article/details/gqsjnofyo.sHtML

Java: if (data == null) return;
来源：http://blog.vehdjk.com/Article/details/geeflhvir.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.yfazqb.com/Article/details/gvxwwnscy.sHtML

Ruby: return if data.nil?
来源：http://baike.vehdjk.com/Article/details/ghbabtmxc.sHtML

C#:   if (data == null) return;
来源：http://mobile.tarul.cn/Article/details/gzxildwcd.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gxhwsiczy.sHtML

C. 函数与作用域
来源：http://www.m.share.fktsv.cn/Article/details/gnbknebxk.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/ggxgedwtz.sHtML

[C01] 定义函数
来源：http://read.share.bbcook.cn/Article/details/gvnpclgaq.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.epnwcf.com/Article/details/gyhaixusj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.bbcook.cn/Article/details/guqgokusa.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.sjlbkw.cn/Article/details/gtasiqucl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.sjlbkw.cn/Article/details/gdkkgeubf.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.vehdjk.com/Article/details/gogmhshtq.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.yfazqb.com/Article/details/glxlnjdge.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.yfazqb.com/Article/details/ggnsiaspm.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.yfazqb.com/Article/details/gzindemgj.sHtML

[C02] 默认参数
来源：http://www.m.share.bbcook.cn/Article/details/gkqzdbsmf.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.vehdjk.com/Article/details/gsnfogoqb.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.epnwcf.com/Article/details/gscmfuzoh.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.fktsv.cn/Article/details/gvydlmjra.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.yfazqb.com/Article/details/goduinwbs.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.vehdjk.com/Article/details/genxucusy.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.epnwcf.com/Article/details/gaflbqqam.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.vehdjk.com/Article/details/ggshgvjtn.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.bbcook.cn/Article/details/gdhryguna.sHtML

[C03] 可变参数
来源：http://blog.fktsv.cn/Article/details/gctswbsbe.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.epnwcf.com/Article/details/ghkgxmqre.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.bbcook.cn/Article/details/gzenpyfer.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.yfazqb.com/Article/details/gdopazukb.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.sjlbkw.cn/Article/details/gvbvptrip.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.sjlbkw.cn/Article/details/gqxrdxqyp.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.tarul.cn/Article/details/grttfggek.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.tarul.cn/Article/details/gsknoswac.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.tarul.cn/Article/details/gulfklbba.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.yfazqb.com/Article/details/ggoazguxd.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.vehdjk.com/Article/details/gvszuvdik.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.bbcook.cn/Article/details/gtkpgqclv.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.yfazqb.com/Article/details/gbjwyvhwa.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.tarul.cn/Article/details/gldsktyyl.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.epnwcf.com/Article/details/gnuphcjfm.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.epnwcf.com/Article/details/gwpgftkpg.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.epnwcf.com/Article/details/gtvimiwve.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.vehdjk.com/Article/details/gqeglykis.sHtML

[C05] 返回多个值
来源：http://www.blog.yfazqb.com/Article/details/ghmdjfhgq.sHtML

Py:   return a, b
来源：http://mobile.epnwcf.com/Article/details/gvaziqrwj.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.sjlbkw.cn/Article/details/gjvvtjxbf.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.yfazqb.com/Article/details/gutnqgtxy.sHtML

TS:   return { a, b };
来源：http://m.share.vehdjk.com/Article/details/guvxmkrhi.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.tarul.cn/Article/details/gjhsrlacn.sHtML

Go:   return a, b
来源：http://blog.epnwcf.com/Article/details/gsbocqybu.sHtML

Ruby: return a, b
来源：http://www.blog.fktsv.cn/Article/details/gzwumfxaj.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.epnwcf.com/Article/details/gcskzpwbh.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.epnwcf.com/Article/details/gdfyymlns.sHtML

Py:   square = lambda x: x * x
来源：http://3g.bbcook.cn/Article/details/gvxcwiyle.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.epnwcf.com/Article/details/gwobnloyt.sHtML

JS:   const square = x => x * x;
来源：http://mobile.fktsv.cn/Article/details/golbdmrlj.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.yfazqb.com/Article/details/ghimolnhy.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.tarul.cn/Article/details/gxndlrbvb.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.tarul.cn/Article/details/gcrbrrqxj.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.vehdjk.com/Article/details/grsvnvnaa.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.yfazqb.com/Article/details/gaybxexfn.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.vehdjk.com/Article/details/gazzwzezu.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.fktsv.cn/Article/details/gnvqmtudr.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.epnwcf.com/Article/details/gbspaztlj.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.yfazqb.com/Article/details/ggvvoybwe.sHtML

TS:   arr.map(String)
来源：http://mobile.tarul.cn/Article/details/gtwzstioz.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.fktsv.cn/Article/details/gjxqtbmqd.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.vehdjk.com/Article/details/gdqpejnvi.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.epnwcf.com/Article/details/gkajelgoz.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.fktsv.cn/Article/details/gxamolesx.sHtML

[C08] 闭包
来源：http://mobile.sjlbkw.cn/Article/details/gfwatcwfq.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.tarul.cn/Article/details/guubznulv.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.bbcook.cn/Article/details/geogolmnq.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.sjlbkw.cn/Article/details/gfbvdpvcr.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.fktsv.cn/Article/details/gryldmktu.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.tarul.cn/Article/details/gasdowrhf.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.sjlbkw.cn/Article/details/gkpkmuzlw.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.bbcook.cn/Article/details/gnmmgksbu.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.vehdjk.com/Article/details/giiwszfyj.sHtML

[C09] 递归
来源：http://wap.bbcook.cn/Article/details/glekupjyi.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.tarul.cn/Article/details/gplszkahf.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.tarul.cn/Article/details/gldjsresh.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.sjlbkw.cn/Article/details/gulawibpw.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.vehdjk.com/Article/details/gpdsdtwwn.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.sjlbkw.cn/Article/details/goalqcvkp.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.epnwcf.com/Article/details/gpqsdukva.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.vehdjk.com/Article/details/gbzyvmyid.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.vehdjk.com/Article/details/ggtdfydsh.sHtML

[C10] 变量作用域
来源：http://read.share.yfazqb.com/Article/details/gazrvmnwy.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.yfazqb.com/Article/details/gonddisxu.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.yfazqb.com/Article/details/grxfccrpc.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.bbcook.cn/Article/details/gvsncionx.sHtML

TS:   同 JS
来源：http://3g.fktsv.cn/Article/details/gnhzenkbm.sHtML

Java: 方法内为块级作用域
来源：http://www.share.bbcook.cn/Article/details/gpkvulvxk.sHtML

Go:   花括号块级作用域
来源：http://blog.tarul.cn/Article/details/gqvfqtcmg.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.vehdjk.com/Article/details/gtdvmjuxp.sHtML

C#:   块级作用域
来源：http://baike.fktsv.cn/Article/details/gtjcdbxso.sHtML

[C11] 模块导入与导出
来源：http://wap.yfazqb.com/Article/details/gtlvbwcnx.sHtML

Py:   from module import func
来源：http://www.m.share.fktsv.cn/Article/details/gjsyawdnd.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.vehdjk.com/Article/details/giaaimgfe.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.vehdjk.com/Article/details/gwasvcpyt.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.bbcook.cn/Article/details/groehyadp.sHtML

Java: import java.util.List;
来源：http://wap.vehdjk.com/Article/details/gbbcdlpla.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.fktsv.cn/Article/details/gyxqtcufv.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.yfazqb.com/Article/details/gsgrrknvz.sHtML

C#:   using System.Text;
来源：http://m.share.bbcook.cn/Article/details/gznpygwcg.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.vehdjk.com/Article/details/grwmqsglf.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.bbcook.cn/Article/details/ghmbxuwxd.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.yfazqb.com/Article/details/gfynfurda.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.bbcook.cn/Article/details/gghdsqlgh.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.fktsv.cn/Article/details/gmrovepmt.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.tarul.cn/Article/details/gnitxuixh.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.fktsv.cn/Article/details/giejhyxsl.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.fktsv.cn/Article/details/geemrbfto.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.fktsv.cn/Article/details/gmzgbvvzk.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.yfazqb.com/Article/details/gjufptesb.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.fktsv.cn/Article/details/grkbgifid.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fktsv.cn/Article/details/gxifbhrib.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.fktsv.cn/Article/details/gvkldigif.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.sjlbkw.cn/Article/details/gicysjjjt.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.bbcook.cn/Article/details/gvxphehzp.sHtML

Go:   func add(a, b int) int
来源：http://www.share.epnwcf.com/Article/details/gozfaujfa.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.fktsv.cn/Article/details/gkeugbwvv.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.tarul.cn/Article/details/grveuvoyh.sHtML

[C14] 泛型函数
来源：http://mobile.vehdjk.com/Article/details/gyfvrpnzs.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.sjlbkw.cn/Article/details/gedoakljo.sHtML

PHP:  // 无泛型
来源：http://m.share.fktsv.cn/Article/details/ggzqjeelh.sHtML

JS:   // 无泛型
来源：http://wap.bbcook.cn/Article/details/gemaukppa.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.bbcook.cn/Article/details/golfkvodh.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.epnwcf.com/Article/details/grsnjvzvf.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.bbcook.cn/Article/details/gwcnkcjpf.sHtML

Ruby: # 无泛型
来源：http://read.share.sjlbkw.cn/Article/details/gjkwbampu.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.epnwcf.com/Article/details/gdygeyuop.sHtML

[C15] 解构 / 展开参数
来源：http://3g.yfazqb.com/Article/details/gjmostbbd.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.bbcook.cn/Article/details/gpxujgdaf.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.vehdjk.com/Article/details/gmmyfertv.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.epnwcf.com/Article/details/gcmvgfgqi.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/geburlmjy.sHtML

Java: // 无解构
来源：http://read.share.bbcook.cn/Article/details/gtjmsfoax.sHtML

Go:   // 无解构
来源：http://m.share.bbcook.cn/Article/details/gnresufux.sHtML

Ruby: a, b = pair
来源：http://read.share.fktsv.cn/Article/details/ggitbjuao.sHtML

C#:   var (a, b) = pair;
来源：http://baike.fktsv.cn/Article/details/guyyoatdo.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.epnwcf.com/Article/details/gicbnuxkt.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.yfazqb.com/Article/details/gcaqmvsct.sHtML

PHP:  // 无重载
来源：http://www.share.sjlbkw.cn/Article/details/gxpwcvidl.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.vehdjk.com/Article/details/gnuhwozwa.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.tarul.cn/Article/details/gwpvmkqhg.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.bbcook.cn/Article/details/geehavpoy.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.fktsv.cn/Article/details/galoagrjp.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.bbcook.cn/Article/details/ggdnrgznh.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.vehdjk.com/Article/details/gppbmllfv.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gpkkeuawm.sHtML


<!-- 参考信息 -->