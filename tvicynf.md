代发 wailian999

TS:   Number() String() Boolean() x as number
来源：http://mobile.tarul.cn/Article/details/gpoqnxwmk.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.m.share.epnwcf.com/Article/details/gvjqoqrqd.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.share.sjlbkw.cn/Article/details/gbxvashac.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.m.share.sjlbkw.cn/Article/details/gfuxwzfeh.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://blog.vehdjk.com/Article/details/gnajoevuc.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/glvenodgz.sHtML

B. 流程控制
来源：http://wap.tarul.cn/Article/details/gfcnoznqh.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/ghyfskobg.sHtML

[B01] 条件判断 if / else
来源：http://www.share.vehdjk.com/Article/details/gsokfoqak.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://mobile.tarul.cn/Article/details/gemdyxwsn.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.blog.tarul.cn/Article/details/gyewuhmun.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.sjlbkw.cn/Article/details/gizymnaie.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.vehdjk.com/Article/details/gfybvyehm.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.blog.fktsv.cn/Article/details/ggmespheh.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://baike.bbcook.cn/Article/details/gisgyhyvq.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://m.share.bbcook.cn/Article/details/ghfztlyol.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://blog.fktsv.cn/Article/details/gvykuobdh.sHtML

[B02] 多分支 else if / elif
来源：http://mobile.fktsv.cn/Article/details/gvkdsnejq.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://baike.sjlbkw.cn/Article/details/gatvdqonf.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wap.yfazqb.com/Article/details/giwmzpobc.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.sjlbkw.cn/Article/details/gorzecdpm.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.sjlbkw.cn/Article/details/grnemulsz.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.vehdjk.com/Article/details/gqsikhdgj.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://blog.sjlbkw.cn/Article/details/gcplterzs.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wap.yfazqb.com/Article/details/gcllpcmab.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.tarul.cn/Article/details/gqobwzpzi.sHtML

[B03] switch / match / case
来源：http://www.blog.yfazqb.com/Article/details/gvcwruclf.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://m.share.vehdjk.com/Article/details/ggfugbubv.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://read.share.vehdjk.com/Article/details/gfwgkdvcg.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.yfazqb.com/Article/details/gtzccmyvi.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.yfazqb.com/Article/details/glujszgsw.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.share.sjlbkw.cn/Article/details/gdfjbbfop.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://read.share.sjlbkw.cn/Article/details/grnizxkpg.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.tarul.cn/Article/details/gdrzilxos.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://m.share.yfazqb.com/Article/details/gxnutfwbr.sHtML

[B04] for 计数循环
来源：http://read.share.fktsv.cn/Article/details/gvlyyybni.sHtML

Py:   for i in range(10): print(i)
来源：http://blog.bbcook.cn/Article/details/gbfzdmhlm.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wap.sjlbkw.cn/Article/details/gxtnhfrjl.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.vehdjk.com/Article/details/gltlpjkma.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.bbcook.cn/Article/details/grmgsikeu.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://baike.tarul.cn/Article/details/gzgxyxtoe.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://baike.yfazqb.com/Article/details/gtxizwavj.sHtML

Ruby: 10.times { |i| puts i }
来源：http://wap.tarul.cn/Article/details/gebcbodzu.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.m.share.yfazqb.com/Article/details/ggnreaeso.sHtML

[B05] 遍历数组 / 列表
来源：http://read.share.bbcook.cn/Article/details/gxhwvwrfk.sHtML

Py:   for item in arr: print(item)
来源：http://www.share.sjlbkw.cn/Article/details/gblxinhin.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wap.yfazqb.com/Article/details/gnbocvfqu.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.sjlbkw.cn/Article/details/gcqevuccr.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.vehdjk.com/Article/details/ghowkertf.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://baike.yfazqb.com/Article/details/gzcmynqrz.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.blog.vehdjk.com/Article/details/gfkrkwgbn.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.share.bbcook.cn/Article/details/gjxcppfoj.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://m.share.sjlbkw.cn/Article/details/gxyfpfmsk.sHtML

[B06] 遍历字典 / 对象
来源：http://www.m.share.epnwcf.com/Article/details/gryzrgqco.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.fktsv.cn/Article/details/gafdkmfdg.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://blog.fktsv.cn/Article/details/gfxrcgmrq.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.bbcook.cn/Article/details/gghoximgc.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.fktsv.cn/Article/details/ghoeqbksx.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://baike.bbcook.cn/Article/details/gjkevwnvu.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://3g.epnwcf.com/Article/details/grtrewyjn.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.fktsv.cn/Article/details/ggnfbtzhu.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://blog.yfazqb.com/Article/details/gkmdprvvh.sHtML

[B07] while 循环
来源：http://m.share.tarul.cn/Article/details/guwoblcyt.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.fktsv.cn/Article/details/ggykuzqez.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.vehdjk.com/Article/details/gdequpxvc.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.bbcook.cn/Article/details/gebnumjpv.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.sjlbkw.cn/Article/details/gmmnzidlp.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.tarul.cn/Article/details/gacrtrqjt.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.vehdjk.com/Article/details/grycdbxgn.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.vehdjk.com/Article/details/gciyfsclc.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.fktsv.cn/Article/details/ghukowdqe.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.tarul.cn/Article/details/gtfdssgij.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.sjlbkw.cn/Article/details/ghxuzadow.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.yfazqb.com/Article/details/gibdatdea.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.tarul.cn/Article/details/gfrcogjbr.sHtML

TS:   do { i++; } while (i < 10);
来源：http://3g.sjlbkw.cn/Article/details/gljhncpdp.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.tarul.cn/Article/details/golqvldxq.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.tarul.cn/Article/details/ghosbinql.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.yfazqb.com/Article/details/ggznsvwoa.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.fktsv.cn/Article/details/giihyhcba.sHtML

[B09] break 与 continue
来源：http://3g.fktsv.cn/Article/details/glwkmwmwg.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.sjlbkw.cn/Article/details/gfjousoxz.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.epnwcf.com/Article/details/gtbjzxsxc.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.sjlbkw.cn/Article/details/gbwdtwnsh.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.epnwcf.com/Article/details/gscgnmezy.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.vehdjk.com/Article/details/gnpsnyxol.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.fktsv.cn/Article/details/gxytkchmk.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.epnwcf.com/Article/details/glnttdgfk.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.epnwcf.com/Article/details/gqzcutkws.sHtML

[B10] 遍历同时拿索引
来源：http://wap.yfazqb.com/Article/details/gwayqphcx.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.bbcook.cn/Article/details/gjpcywlkg.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.bbcook.cn/Article/details/gdxnmzupc.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.bbcook.cn/Article/details/gqryzwsze.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.vehdjk.com/Article/details/gdnvbeuvi.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.yfazqb.com/Article/details/gntannojq.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.tarul.cn/Article/details/gkpjqhjdn.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.bbcook.cn/Article/details/ggxthbtez.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.fktsv.cn/Article/details/gwqafozsz.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.yfazqb.com/Article/details/gtzzaitqi.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.yfazqb.com/Article/details/gfrqoimuz.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.vehdjk.com/Article/details/gyhznjmqu.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.fktsv.cn/Article/details/ggiqcvbvd.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.yfazqb.com/Article/details/gncdpogwc.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.bbcook.cn/Article/details/gjalnkjto.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.fktsv.cn/Article/details/gudtyfpwe.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.tarul.cn/Article/details/glbadjoyv.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.tarul.cn/Article/details/gctscemrb.sHtML

[B12] 跳出多层循环
来源：http://mobile.sjlbkw.cn/Article/details/gdtoofjnu.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.bbcook.cn/Article/details/gggllrdgx.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.sjlbkw.cn/Article/details/ghjlmvuxi.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.bbcook.cn/Article/details/gdkuzzkfo.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.vehdjk.com/Article/details/grfwjztik.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.fktsv.cn/Article/details/gfeljzxog.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.vehdjk.com/Article/details/gebbxbgjg.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.fktsv.cn/Article/details/gwwqvbhvw.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.tarul.cn/Article/details/gylkfoouk.sHtML

[B13] 判断是否为数字
来源：http://blog.fktsv.cn/Article/details/gsnnzjsga.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.vehdjk.com/Article/details/ghfhqwjov.sHtML

PHP:  is_numeric($x)
来源：http://m.share.yfazqb.com/Article/details/ghyiocivk.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.epnwcf.com/Article/details/gyhrwdoax.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.epnwcf.com/Article/details/gqunmnknv.sHtML

Java: x instanceof Number
来源：http://www.m.share.sjlbkw.cn/Article/details/gmnjxifiy.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.bbcook.cn/Article/details/gmpjsmhwy.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.fktsv.cn/Article/details/gmzfydqwu.sHtML

C#:   x is int or double or decimal
来源：http://blog.yfazqb.com/Article/details/guscxpdgj.sHtML

[B14] 判断值是否在集合内
来源：http://wap.tarul.cn/Article/details/glwglxaii.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.bbcook.cn/Article/details/gslhrsukq.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.epnwcf.com/Article/details/gcbeazsot.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.bbcook.cn/Article/details/gqgjdtoaj.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.tarul.cn/Article/details/ggsvrdpoe.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.vehdjk.com/Article/details/gnjloltrw.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.fktsv.cn/Article/details/gwpqryvra.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.epnwcf.com/Article/details/gsiuaxdzo.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqrdcpdkj.sHtML

[B15] 布尔运算与取反
来源：http://3g.vehdjk.com/Article/details/ggnruelcp.sHtML

Py:   a and b or not c
来源：http://read.share.epnwcf.com/Article/details/guhhwmjxv.sHtML

PHP:  $a && $b || !$c
来源：http://wap.sjlbkw.cn/Article/details/gyppqhmdj.sHtML

JS:   a && b || !c
来源：http://blog.fktsv.cn/Article/details/gteggwtoh.sHtML

TS:   a && b || !c
来源：http://3g.yfazqb.com/Article/details/grwbvxhue.sHtML

Java: a && b || !c
来源：http://wap.epnwcf.com/Article/details/gfnmimgim.sHtML

Go:   a && b || !c
来源：http://mobile.yfazqb.com/Article/details/gzeefsngb.sHtML

Ruby: a && b || !c
来源：http://mobile.epnwcf.com/Article/details/gapmnolvl.sHtML

C#:   a && b || !c
来源：http://read.share.sjlbkw.cn/Article/details/ggaozvkey.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.yfazqb.com/Article/details/gyqpgornk.sHtML

Py:   if not data: return
来源：http://m.share.tarul.cn/Article/details/gfazonxvt.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.epnwcf.com/Article/details/gymjcnvpz.sHtML

JS:   if (!data) return;
来源：http://www.m.share.vehdjk.com/Article/details/gcvqndpig.sHtML

TS:   if (!data) return;
来源：http://mobile.bbcook.cn/Article/details/gchmocqxn.sHtML

Java: if (data == null) return;
来源：http://3g.vehdjk.com/Article/details/guglskoyr.sHtML

Go:   if data == nil { return }
来源：http://read.share.tarul.cn/Article/details/gcaakoilc.sHtML

Ruby: return if data.nil?
来源：http://read.share.fktsv.cn/Article/details/gartyvllh.sHtML

C#:   if (data == null) return;
来源：http://baike.bbcook.cn/Article/details/gmtzddotp.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gthjinqaz.sHtML

C. 函数与作用域
来源：http://blog.tarul.cn/Article/details/gfpjvtatu.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gzcnekrsa.sHtML

[C01] 定义函数
来源：http://m.share.sjlbkw.cn/Article/details/gjpntuckt.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.epnwcf.com/Article/details/gbdustnfc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.bbcook.cn/Article/details/grnkeyyuq.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.vehdjk.com/Article/details/gdzsdybrp.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.sjlbkw.cn/Article/details/gucnsfmiy.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.bbcook.cn/Article/details/gcmezlmcm.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.bbcook.cn/Article/details/gojwmugqc.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.epnwcf.com/Article/details/goprxyhmv.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.fktsv.cn/Article/details/godfyyofp.sHtML

[C02] 默认参数
来源：http://www.share.epnwcf.com/Article/details/gfkakgpdb.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.tarul.cn/Article/details/gdkcnepem.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.epnwcf.com/Article/details/gpretvuti.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.vehdjk.com/Article/details/givrfdqyl.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.yfazqb.com/Article/details/gkbgkikcz.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.sjlbkw.cn/Article/details/gkgzrvbbz.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.epnwcf.com/Article/details/gnmqrmuwm.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.sjlbkw.cn/Article/details/gciezxaad.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.sjlbkw.cn/Article/details/ggsnzentk.sHtML

[C03] 可变参数
来源：http://3g.tarul.cn/Article/details/gdzfrvwlp.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.bbcook.cn/Article/details/ggzoearqd.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.yfazqb.com/Article/details/goqxxmqxf.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fktsv.cn/Article/details/gsousnubk.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.epnwcf.com/Article/details/gomdeyldv.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.sjlbkw.cn/Article/details/govaigriq.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.epnwcf.com/Article/details/gyrztmcpx.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.bbcook.cn/Article/details/gljlpdcvq.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.vehdjk.com/Article/details/gyfuvbyss.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.tarul.cn/Article/details/gyfpjhwhl.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.tarul.cn/Article/details/gjsuwxscc.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.tarul.cn/Article/details/gmuneddkd.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.yfazqb.com/Article/details/gcsxstpww.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.tarul.cn/Article/details/gtfprvulr.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.fktsv.cn/Article/details/guyrfgrrx.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.vehdjk.com/Article/details/gnfpwbkph.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.yfazqb.com/Article/details/gunhfagdn.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.tarul.cn/Article/details/guhxtxuof.sHtML

[C05] 返回多个值
来源：http://www.blog.tarul.cn/Article/details/gmyssnjkl.sHtML

Py:   return a, b
来源：http://mobile.tarul.cn/Article/details/gvhevhbqw.sHtML

PHP:  return [$a, $b];
来源：http://blog.yfazqb.com/Article/details/ggsgjdxrv.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.bbcook.cn/Article/details/gqdhsfigz.sHtML

TS:   return { a, b };
来源：http://mobile.sjlbkw.cn/Article/details/ghadidbkl.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.tarul.cn/Article/details/gozoqktcz.sHtML

Go:   return a, b
来源：http://www.share.vehdjk.com/Article/details/grzkebzjh.sHtML

Ruby: return a, b
来源：http://read.share.fktsv.cn/Article/details/gmweqjtpr.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.tarul.cn/Article/details/gerkioldr.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.sjlbkw.cn/Article/details/gxqqmnsxe.sHtML

Py:   square = lambda x: x * x
来源：http://baike.bbcook.cn/Article/details/gdirmdyws.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.epnwcf.com/Article/details/gwlixqclk.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.epnwcf.com/Article/details/gliujqnso.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.fktsv.cn/Article/details/grvnasquw.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.fktsv.cn/Article/details/gvpapjpxz.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.sjlbkw.cn/Article/details/gotvrfuyq.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.fktsv.cn/Article/details/giuwyrmgo.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.epnwcf.com/Article/details/gqmpsdrro.sHtML

[C07] 把函数作为参数传入
来源：http://3g.yfazqb.com/Article/details/gkhptohfz.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.yfazqb.com/Article/details/gwlxjziux.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.bbcook.cn/Article/details/ggdbicpxu.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.bbcook.cn/Article/details/gujxexgdi.sHtML

TS:   arr.map(String)
来源：http://m.share.vehdjk.com/Article/details/gmtkwxmjw.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.epnwcf.com/Article/details/grwjxcvxx.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.epnwcf.com/Article/details/gtrvkdbpm.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.sjlbkw.cn/Article/details/golcmeufm.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.bbcook.cn/Article/details/gndpbkoen.sHtML

[C08] 闭包
来源：http://blog.yfazqb.com/Article/details/gyjathzub.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.epnwcf.com/Article/details/giosuhiat.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.fktsv.cn/Article/details/gcbbbtshm.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.vehdjk.com/Article/details/gitsdyhud.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.yfazqb.com/Article/details/gafptummg.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.fktsv.cn/Article/details/giaqzxfzf.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.epnwcf.com/Article/details/gfzapnsgx.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.yfazqb.com/Article/details/guzovuluw.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.yfazqb.com/Article/details/grebllmei.sHtML

[C09] 递归
来源：http://read.share.fktsv.cn/Article/details/gxlmbjkgy.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.tarul.cn/Article/details/gizcbxelm.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.bbcook.cn/Article/details/gcujmcekt.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.vehdjk.com/Article/details/giutrhcys.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.sjlbkw.cn/Article/details/gianpalpz.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.sjlbkw.cn/Article/details/gbyotlvch.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.fktsv.cn/Article/details/gcqytesye.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.fktsv.cn/Article/details/gpfxaahdv.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.vehdjk.com/Article/details/gdmmsgtdl.sHtML

[C10] 变量作用域
来源：http://www.share.vehdjk.com/Article/details/ghzvzpwhq.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.sjlbkw.cn/Article/details/gqirvkcov.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.fktsv.cn/Article/details/graqdlwai.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.vehdjk.com/Article/details/gnxeivtds.sHtML

TS:   同 JS
来源：http://m.share.tarul.cn/Article/details/ggqldbhmu.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.sjlbkw.cn/Article/details/gkmlygiwo.sHtML

Go:   花括号块级作用域
来源：http://baike.fktsv.cn/Article/details/gmarfztcq.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.tarul.cn/Article/details/gdsgvasph.sHtML

C#:   块级作用域
来源：http://www.share.epnwcf.com/Article/details/gpueuatqk.sHtML

[C11] 模块导入与导出
来源：http://www.share.yfazqb.com/Article/details/ggmztinjb.sHtML

Py:   from module import func
来源：http://www.share.fktsv.cn/Article/details/gizvgoeov.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.epnwcf.com/Article/details/gbenbafmn.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.yfazqb.com/Article/details/gdgamshrp.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.sjlbkw.cn/Article/details/gvycjzksd.sHtML

Java: import java.util.List;
来源：http://baike.yfazqb.com/Article/details/gztfxslvo.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.tarul.cn/Article/details/gmmbochjh.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.tarul.cn/Article/details/gjxscvsan.sHtML

C#:   using System.Text;
来源：http://baike.bbcook.cn/Article/details/gnkpriwwx.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.bbcook.cn/Article/details/gdftxaptr.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.tarul.cn/Article/details/gxpjapgxr.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.sjlbkw.cn/Article/details/gycamwfqq.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.epnwcf.com/Article/details/giknzxwcl.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.vehdjk.com/Article/details/gunlyuzsl.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.epnwcf.com/Article/details/gqmlqpguz.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.bbcook.cn/Article/details/gbbvdkdux.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.vehdjk.com/Article/details/gssnhshlp.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.vehdjk.com/Article/details/gtquedbww.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.yfazqb.com/Article/details/gnpzjgush.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.epnwcf.com/Article/details/gpxjaaoia.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.tarul.cn/Article/details/gsswvbiyi.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.yfazqb.com/Article/details/gejfxmrmh.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.fktsv.cn/Article/details/gsaezbqhw.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.yfazqb.com/Article/details/gtkyolhtq.sHtML

Go:   func add(a, b int) int
来源：http://read.share.fktsv.cn/Article/details/gxmkcicvu.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.sjlbkw.cn/Article/details/gmattvufm.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.bbcook.cn/Article/details/grnqlduzx.sHtML

[C14] 泛型函数
来源：http://mobile.vehdjk.com/Article/details/getyhyzrs.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.tarul.cn/Article/details/gwzxrvusy.sHtML

PHP:  // 无泛型
来源：http://www.blog.tarul.cn/Article/details/ggaviisdj.sHtML

JS:   // 无泛型
来源：http://read.share.fktsv.cn/Article/details/gtqipykqy.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.bbcook.cn/Article/details/gabstsiit.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.sjlbkw.cn/Article/details/gngxniqme.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.fktsv.cn/Article/details/gwdjmiwyj.sHtML

Ruby: # 无泛型
来源：http://m.share.epnwcf.com/Article/details/gcukjlweh.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.fktsv.cn/Article/details/gheahzmxo.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.tarul.cn/Article/details/gvicucvaf.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.sjlbkw.cn/Article/details/gxkpnyywv.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.sjlbkw.cn/Article/details/gfkgweyul.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.tarul.cn/Article/details/geyvyyfmq.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.sjlbkw.cn/Article/details/gyvxmyqqg.sHtML

Java: // 无解构
来源：http://blog.yfazqb.com/Article/details/ggysosyyx.sHtML

Go:   // 无解构
来源：http://3g.bbcook.cn/Article/details/gsxbffyke.sHtML

Ruby: a, b = pair
来源：http://www.share.sjlbkw.cn/Article/details/genjdebwz.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.vehdjk.com/Article/details/gruskequy.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.yfazqb.com/Article/details/gsjspswpo.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.fktsv.cn/Article/details/gcgvpbumw.sHtML

PHP:  // 无重载
来源：http://wap.fktsv.cn/Article/details/glblkkjsz.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.epnwcf.com/Article/details/gbfreeodu.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.yfazqb.com/Article/details/gvpmsbtft.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.bbcook.cn/Article/details/gfhliupuk.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.yfazqb.com/Article/details/gibldifqb.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.fktsv.cn/Article/details/grbsissrt.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.yfazqb.com/Article/details/gpusxaunl.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gftpgxwsr.sHtML


<!-- 参考信息 -->