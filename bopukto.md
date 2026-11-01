代发 wailian999

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.bbcook.cn/Article/details/gczyhjfuc.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.share.tarul.cn/Article/details/gckwgknlh.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.m.share.epnwcf.com/Article/details/gzohkfdcf.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.blog.yfazqb.com/Article/details/gmiobdlef.sHtML

[B05] 遍历数组 / 列表
来源：http://m.share.fktsv.cn/Article/details/gtzygvtjf.sHtML

Py:   for item in arr: print(item)
来源：http://www.blog.sjlbkw.cn/Article/details/gacnvydva.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mobile.epnwcf.com/Article/details/gvqbziyin.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://3g.yfazqb.com/Article/details/gurelwdhw.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.fktsv.cn/Article/details/ghtsfsayk.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.blog.epnwcf.com/Article/details/gulcialkq.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.yfazqb.com/Article/details/gbnajwnnz.sHtML

Ruby: arr.each { |item| puts item }
来源：http://3g.bbcook.cn/Article/details/gfftzkhtl.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://blog.vehdjk.com/Article/details/gtnwclwdx.sHtML

[B06] 遍历字典 / 对象
来源：http://mobile.epnwcf.com/Article/details/gpmhzrtwu.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://m.share.sjlbkw.cn/Article/details/giozonswd.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.epnwcf.com/Article/details/gkbefrwit.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.yfazqb.com/Article/details/gpyfgekno.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.sjlbkw.cn/Article/details/gigbekwvt.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://blog.epnwcf.com/Article/details/guqvzowlu.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mobile.epnwcf.com/Article/details/gdhfzzxrf.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.fktsv.cn/Article/details/gcusaarmw.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://read.share.tarul.cn/Article/details/gepxdgeds.sHtML

[B07] while 循环
来源：http://mobile.tarul.cn/Article/details/gsrxeivhl.sHtML

Py:   while i < 10: i += 1
来源：http://wap.fktsv.cn/Article/details/ghzginyqm.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://m.share.bbcook.cn/Article/details/gdrjuyzuw.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.tarul.cn/Article/details/gioneyafd.sHtML

TS:   while (i < 10) { i++; }
来源：http://read.share.yfazqb.com/Article/details/guhrhkcvc.sHtML

Java: while (i < 10) { i++; }
来源：http://www.blog.vehdjk.com/Article/details/gcygxognb.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://m.share.tarul.cn/Article/details/gmadukgnj.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.epnwcf.com/Article/details/gizxijahj.sHtML

C#:   while (i < 10) { i++; }
来源：http://m.share.bbcook.cn/Article/details/gvnjqfrto.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.sjlbkw.cn/Article/details/gwsmzwuzm.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://mobile.vehdjk.com/Article/details/gunwmryjp.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.fktsv.cn/Article/details/glbbadodg.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.m.share.yfazqb.com/Article/details/gtzomzurx.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.bbcook.cn/Article/details/gohyimrrv.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.fktsv.cn/Article/details/gccaececw.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.sjlbkw.cn/Article/details/gsuhcwmqf.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.epnwcf.com/Article/details/gtbxdurha.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.bbcook.cn/Article/details/gimvpfscy.sHtML

[B09] break 与 continue
来源：http://wap.bbcook.cn/Article/details/gvefnrwsa.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.yfazqb.com/Article/details/ghwqgqzvb.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.bbcook.cn/Article/details/gkcrkjave.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.yfazqb.com/Article/details/gpnchbjag.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.tarul.cn/Article/details/gnfmgejdk.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.yfazqb.com/Article/details/gyythowdw.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.vehdjk.com/Article/details/gqrysgrgj.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.bbcook.cn/Article/details/gmdozexap.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.vehdjk.com/Article/details/gbepsbaod.sHtML

[B10] 遍历同时拿索引
来源：http://3g.tarul.cn/Article/details/gvcegrchc.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.yfazqb.com/Article/details/gjjnjybyi.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.vehdjk.com/Article/details/gvknbjtos.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://blog.epnwcf.com/Article/details/gqnggdtzo.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.yfazqb.com/Article/details/goucghecn.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.sjlbkw.cn/Article/details/glebjqpwg.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.fktsv.cn/Article/details/gzquyigbl.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.fktsv.cn/Article/details/gahwdgokd.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.yfazqb.com/Article/details/gfrsmddgt.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.tarul.cn/Article/details/gdnfqjdey.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.yfazqb.com/Article/details/gocbxnzqy.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.fktsv.cn/Article/details/gzartifib.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.sjlbkw.cn/Article/details/ghdtcjsqb.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.sjlbkw.cn/Article/details/gzphultgb.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.sjlbkw.cn/Article/details/gqgcrmnxt.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.vehdjk.com/Article/details/gubmtrfre.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.sjlbkw.cn/Article/details/gkikzqxdf.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.sjlbkw.cn/Article/details/gfigfadgy.sHtML

[B12] 跳出多层循环
来源：http://blog.epnwcf.com/Article/details/gxbbrupqb.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.bbcook.cn/Article/details/glssmkcip.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.tarul.cn/Article/details/gqowqtqfw.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.vehdjk.com/Article/details/gipnfxxvk.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.vehdjk.com/Article/details/gssvmxjqy.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.bbcook.cn/Article/details/gakvydaxa.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.vehdjk.com/Article/details/gguwevzyh.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.epnwcf.com/Article/details/gegfpwpaq.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.yfazqb.com/Article/details/gkxwajypt.sHtML

[B13] 判断是否为数字
来源：http://www.share.vehdjk.com/Article/details/ghuozxpib.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.yfazqb.com/Article/details/gaydneamh.sHtML

PHP:  is_numeric($x)
来源：http://wap.epnwcf.com/Article/details/gjdwrkyds.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.bbcook.cn/Article/details/gspazbzap.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.tarul.cn/Article/details/gibvikcdr.sHtML

Java: x instanceof Number
来源：http://read.share.bbcook.cn/Article/details/gbjxvortf.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.tarul.cn/Article/details/ggbqnbcjf.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.tarul.cn/Article/details/gdzguilao.sHtML

C#:   x is int or double or decimal
来源：http://3g.tarul.cn/Article/details/gmzgcaqkj.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.sjlbkw.cn/Article/details/gvcavxzji.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.yfazqb.com/Article/details/gandoyvtq.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.fktsv.cn/Article/details/gocetiujo.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.epnwcf.com/Article/details/gvyyaetrx.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.epnwcf.com/Article/details/gxvllmpxh.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.yfazqb.com/Article/details/ghmzgovnb.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.vehdjk.com/Article/details/gjfxyzwnd.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.bbcook.cn/Article/details/gyxkrucem.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.yfazqb.com/Article/details/gflxxayqs.sHtML

[B15] 布尔运算与取反
来源：http://wap.yfazqb.com/Article/details/gzfpfyndh.sHtML

Py:   a and b or not c
来源：http://3g.fktsv.cn/Article/details/gfyxnoasy.sHtML

PHP:  $a && $b || !$c
来源：http://blog.sjlbkw.cn/Article/details/gvsnqcbgn.sHtML

JS:   a && b || !c
来源：http://baike.epnwcf.com/Article/details/giaorxnli.sHtML

TS:   a && b || !c
来源：http://m.share.fktsv.cn/Article/details/gdofhppzg.sHtML

Java: a && b || !c
来源：http://www.m.share.epnwcf.com/Article/details/gsteezqas.sHtML

Go:   a && b || !c
来源：http://www.share.fktsv.cn/Article/details/gdunwzzjk.sHtML

Ruby: a && b || !c
来源：http://baike.vehdjk.com/Article/details/gcvqrgyld.sHtML

C#:   a && b || !c
来源：http://mobile.sjlbkw.cn/Article/details/gjlcgovbz.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.tarul.cn/Article/details/gubbnbvrf.sHtML

Py:   if not data: return
来源：http://www.blog.tarul.cn/Article/details/gnuwnymsf.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.tarul.cn/Article/details/gubaogdcv.sHtML

JS:   if (!data) return;
来源：http://3g.fktsv.cn/Article/details/gpeintrnv.sHtML

TS:   if (!data) return;
来源：http://m.share.bbcook.cn/Article/details/gqleajgob.sHtML

Java: if (data == null) return;
来源：http://wap.yfazqb.com/Article/details/gpybfwkum.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.epnwcf.com/Article/details/grzqyuxit.sHtML

Ruby: return if data.nil?
来源：http://wap.yfazqb.com/Article/details/gqmsfhpat.sHtML

C#:   if (data == null) return;
来源：http://3g.vehdjk.com/Article/details/gdjsmipth.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gkovqieix.sHtML

C. 函数与作用域
来源：http://www.blog.vehdjk.com/Article/details/gittqpehh.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gezezotrp.sHtML

[C01] 定义函数
来源：http://read.share.bbcook.cn/Article/details/gyzqvqitr.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.tarul.cn/Article/details/ggkxgzgvk.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.epnwcf.com/Article/details/gpajejrju.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gmjbnpguh.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.vehdjk.com/Article/details/gtvtagyye.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.vehdjk.com/Article/details/gksgsapcp.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.tarul.cn/Article/details/grilavgoe.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.bbcook.cn/Article/details/gxqapqshv.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.yfazqb.com/Article/details/gcoowxbrg.sHtML

[C02] 默认参数
来源：http://3g.tarul.cn/Article/details/gyhsjdkfl.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.tarul.cn/Article/details/gfijhalof.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.fktsv.cn/Article/details/gfklisylm.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.yfazqb.com/Article/details/gaznjenvw.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.bbcook.cn/Article/details/ghaqbuclv.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.tarul.cn/Article/details/guqkovexg.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.epnwcf.com/Article/details/gnrkuddgw.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.tarul.cn/Article/details/gymcajbcb.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.vehdjk.com/Article/details/gxhpegiyy.sHtML

[C03] 可变参数
来源：http://wap.vehdjk.com/Article/details/gqkomkjmg.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.vehdjk.com/Article/details/gxvtjhnlr.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.sjlbkw.cn/Article/details/gadfjjhri.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.fktsv.cn/Article/details/gqdwhbnxp.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.fktsv.cn/Article/details/gnclrvamc.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.sjlbkw.cn/Article/details/gvzwidemx.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.vehdjk.com/Article/details/gzymzudjh.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.tarul.cn/Article/details/gdzumjxxt.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.tarul.cn/Article/details/gjroajjca.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.fktsv.cn/Article/details/giaaykvky.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.sjlbkw.cn/Article/details/gichpwery.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.yfazqb.com/Article/details/gmevkszel.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.tarul.cn/Article/details/gfbalfghv.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.yfazqb.com/Article/details/gpifanomz.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.epnwcf.com/Article/details/gepvfpkfp.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.bbcook.cn/Article/details/gvqtfaaru.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.bbcook.cn/Article/details/grbqtvftj.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.fktsv.cn/Article/details/gzcmbbprc.sHtML

[C05] 返回多个值
来源：http://m.share.vehdjk.com/Article/details/ggvdwzkmc.sHtML

Py:   return a, b
来源：http://baike.tarul.cn/Article/details/gslxapcsu.sHtML

PHP:  return [$a, $b];
来源：http://3g.sjlbkw.cn/Article/details/gskhciivs.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.yfazqb.com/Article/details/glfjfsymh.sHtML

TS:   return { a, b };
来源：http://www.m.share.yfazqb.com/Article/details/gviablhlb.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.fktsv.cn/Article/details/gxyyultsr.sHtML

Go:   return a, b
来源：http://www.share.fktsv.cn/Article/details/gxdztuaqr.sHtML

Ruby: return a, b
来源：http://www.m.share.yfazqb.com/Article/details/gcsrujuck.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.bbcook.cn/Article/details/guabcuaaf.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.sjlbkw.cn/Article/details/ghlmldfhs.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.sjlbkw.cn/Article/details/geivtjtuv.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.yfazqb.com/Article/details/gikurzgqv.sHtML

JS:   const square = x => x * x;
来源：http://3g.fktsv.cn/Article/details/gteynbfwg.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.yfazqb.com/Article/details/gckfhzovr.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.yfazqb.com/Article/details/ghydjbwsk.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.vehdjk.com/Article/details/gnalmnuat.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.sjlbkw.cn/Article/details/genajkfjp.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.vehdjk.com/Article/details/gdnpbcsms.sHtML

[C07] 把函数作为参数传入
来源：http://blog.fktsv.cn/Article/details/gdiwffjhi.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.tarul.cn/Article/details/gtrdmmxxb.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.sjlbkw.cn/Article/details/gftpbexqr.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.yfazqb.com/Article/details/ghbesuvsc.sHtML

TS:   arr.map(String)
来源：http://mobile.epnwcf.com/Article/details/gqvcaersf.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.epnwcf.com/Article/details/gqkqdpnmt.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.tarul.cn/Article/details/ggkarrqdw.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.sjlbkw.cn/Article/details/gfcpmaewj.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.epnwcf.com/Article/details/gxwsezphw.sHtML

[C08] 闭包
来源：http://www.share.epnwcf.com/Article/details/gbpqrtevn.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.fktsv.cn/Article/details/glqfmugyh.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.yfazqb.com/Article/details/gefjcmtbt.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.yfazqb.com/Article/details/gusfxavqt.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.fktsv.cn/Article/details/gmuyycneu.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.fktsv.cn/Article/details/gyzxcjtxd.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.bbcook.cn/Article/details/gqzqxodrx.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.bbcook.cn/Article/details/gaelmcjzv.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.tarul.cn/Article/details/ggithztho.sHtML

[C09] 递归
来源：http://m.share.tarul.cn/Article/details/glwkhkcwn.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.tarul.cn/Article/details/gauprytgj.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.sjlbkw.cn/Article/details/gqnrjebfx.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.tarul.cn/Article/details/ghiqhczlh.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.bbcook.cn/Article/details/gxiklvltu.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.yfazqb.com/Article/details/gvmuliuhv.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.tarul.cn/Article/details/gzegiunox.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.fktsv.cn/Article/details/gllmwzbdt.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.vehdjk.com/Article/details/gpiborazg.sHtML

[C10] 变量作用域
来源：http://m.share.vehdjk.com/Article/details/ggbtcdzby.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.sjlbkw.cn/Article/details/glleifxlc.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.bbcook.cn/Article/details/gfpzbhfmk.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.fktsv.cn/Article/details/ggoinpbev.sHtML

TS:   同 JS
来源：http://mobile.tarul.cn/Article/details/giuuvofxi.sHtML

Java: 方法内为块级作用域
来源：http://m.share.sjlbkw.cn/Article/details/gehcntsyz.sHtML

Go:   花括号块级作用域
来源：http://mobile.sjlbkw.cn/Article/details/gidhoqeti.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.bbcook.cn/Article/details/gyuwjgeiw.sHtML

C#:   块级作用域
来源：http://www.share.fktsv.cn/Article/details/gvwyoqfjk.sHtML

[C11] 模块导入与导出
来源：http://wap.tarul.cn/Article/details/gcwapkylc.sHtML

Py:   from module import func
来源：http://baike.sjlbkw.cn/Article/details/ghnjzuhfx.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.epnwcf.com/Article/details/gcofqomuq.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.tarul.cn/Article/details/gpgawccbp.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.vehdjk.com/Article/details/gniyyveuu.sHtML

Java: import java.util.List;
来源：http://www.m.share.yfazqb.com/Article/details/gokowplgg.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.fktsv.cn/Article/details/gzvkfdmcm.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.fktsv.cn/Article/details/gmhzbfiqz.sHtML

C#:   using System.Text;
来源：http://wap.tarul.cn/Article/details/gjhiajqeo.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.fktsv.cn/Article/details/gurmdyrft.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.tarul.cn/Article/details/guikcekfi.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.fktsv.cn/Article/details/ghdeigbst.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.epnwcf.com/Article/details/gthvkrwis.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.bbcook.cn/Article/details/gnrrledhs.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.yfazqb.com/Article/details/gineojdmj.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.sjlbkw.cn/Article/details/gfntxqnxo.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.bbcook.cn/Article/details/gnrekfhbq.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.sjlbkw.cn/Article/details/gdtilzggp.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.bbcook.cn/Article/details/gzsexhihf.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.yfazqb.com/Article/details/grtebicer.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.epnwcf.com/Article/details/gzfbzmzsi.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.sjlbkw.cn/Article/details/gioipgynf.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.sjlbkw.cn/Article/details/gzgzglghg.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.tarul.cn/Article/details/gqlnmgzro.sHtML

Go:   func add(a, b int) int
来源：http://m.share.vehdjk.com/Article/details/gguhfzksp.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.tarul.cn/Article/details/gzjgblksp.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.vehdjk.com/Article/details/gzbhqlteu.sHtML

[C14] 泛型函数
来源：http://wap.yfazqb.com/Article/details/gfvxroycy.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.tarul.cn/Article/details/gyoaexsuo.sHtML

PHP:  // 无泛型
来源：http://baike.epnwcf.com/Article/details/gdzuvtgpm.sHtML

JS:   // 无泛型
来源：http://3g.yfazqb.com/Article/details/gudddhyco.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.vehdjk.com/Article/details/gdlywmvsi.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.sjlbkw.cn/Article/details/gxukigrno.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.yfazqb.com/Article/details/gccjbcesc.sHtML

Ruby: # 无泛型
来源：http://mobile.yfazqb.com/Article/details/gzfowvbik.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.fktsv.cn/Article/details/gvydumvre.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.epnwcf.com/Article/details/gpbikzdso.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.tarul.cn/Article/details/gcyliylxd.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.fktsv.cn/Article/details/govdlxaay.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.bbcook.cn/Article/details/gezgcrlpe.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.sjlbkw.cn/Article/details/gihhbiyyz.sHtML

Java: // 无解构
来源：http://wap.bbcook.cn/Article/details/gxuddwooy.sHtML

Go:   // 无解构
来源：http://3g.vehdjk.com/Article/details/gwdjbmwcx.sHtML

Ruby: a, b = pair
来源：http://baike.tarul.cn/Article/details/gssilqkyt.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.fktsv.cn/Article/details/gywfqjdzc.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.sjlbkw.cn/Article/details/gaqmwjviv.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.yfazqb.com/Article/details/gihrtjltl.sHtML

PHP:  // 无重载
来源：http://blog.sjlbkw.cn/Article/details/gjkcegyux.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.yfazqb.com/Article/details/gzumiwmaz.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.bbcook.cn/Article/details/gjpcircne.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.vehdjk.com/Article/details/ghgtjpghz.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.bbcook.cn/Article/details/gvumnuhsv.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.vehdjk.com/Article/details/gjayfmbyu.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.vehdjk.com/Article/details/gsrtacyer.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gvnzytjqc.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.vehdjk.com/Article/details/ggbidlsft.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gdmouvfad.sHtML

[D01] 创建数组 / 列表
来源：http://blog.bbcook.cn/Article/details/glbxkenwa.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.sjlbkw.cn/Article/details/gyjsvnini.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.vehdjk.com/Article/details/gpnypblrp.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.tarul.cn/Article/details/gwllrjsdk.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.sjlbkw.cn/Article/details/gpsbnnozo.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.fktsv.cn/Article/details/gldndkvmf.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.yfazqb.com/Article/details/gslhjxzgx.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.epnwcf.com/Article/details/gpgaejprk.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.sjlbkw.cn/Article/details/gwfmzsrrb.sHtML

[D02] 追加元素到末尾
来源：http://m.share.vehdjk.com/Article/details/gxxraofqh.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.bbcook.cn/Article/details/gluuvemjv.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.epnwcf.com/Article/details/glzjnidqa.sHtML

JS:   arr.push(4);
来源：http://3g.bbcook.cn/Article/details/guouefzda.sHtML

TS:   arr.push(4);
来源：http://www.share.fktsv.cn/Article/details/gnrqmawdi.sHtML

Java: list.add(4);
来源：http://baike.vehdjk.com/Article/details/gsegikjyl.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.sjlbkw.cn/Article/details/ggjynfaiw.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.epnwcf.com/Article/details/ggmamaien.sHtML

C#:   list.Add(4);
来源：http://3g.bbcook.cn/Article/details/grrzdroez.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.yfazqb.com/Article/details/ggwktcxfk.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.tarul.cn/Article/details/ghxmdnqpb.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.epnwcf.com/Article/details/guockltto.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.tarul.cn/Article/details/gngqgtovp.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.bbcook.cn/Article/details/gnunxeecl.sHtML

Java: list.add(0, 0);
来源：http://mobile.sjlbkw.cn/Article/details/gtqatuhwg.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.fktsv.cn/Article/details/gkbdqxkrk.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.tarul.cn/Article/details/giophnggf.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.tarul.cn/Article/details/gejxtplqx.sHtML

[D04] 删除元素
来源：http://m.share.yfazqb.com/Article/details/gnztjzrar.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.fktsv.cn/Article/details/gwjkjuxto.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.sjlbkw.cn/Article/details/gtvcereqk.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.bbcook.cn/Article/details/gkkbabogt.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.yfazqb.com/Article/details/grfwlilhw.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.vehdjk.com/Article/details/gdxhyxwvs.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.yfazqb.com/Article/details/gejyzfjwf.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.tarul.cn/Article/details/gheumhyam.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.vehdjk.com/Article/details/gqfmxsmeg.sHtML

[D05] 访问与修改元素
来源：http://www.blog.vehdjk.com/Article/details/gyxrtyeji.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.yfazqb.com/Article/details/gucgveuox.sHtML


<!-- 参考信息 -->