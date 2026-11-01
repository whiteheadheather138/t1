代发 wailian999

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.bbcook.cn/Article/details/gqzrkgsrd.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.vehdjk.com/Article/details/grzlozupt.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.blog.fktsv.cn/Article/details/gkfkwjgfr.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.vehdjk.com/Article/details/gzfuanqtr.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.epnwcf.com/Article/details/gxdjathjz.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mobile.epnwcf.com/Article/details/gptcfqvfb.sHtML

[B07] while 循环
来源：http://www.share.bbcook.cn/Article/details/goaefwyku.sHtML

Py:   while i < 10: i += 1
来源：http://baike.fktsv.cn/Article/details/gbuyipgba.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.sjlbkw.cn/Article/details/gpphxdakw.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.blog.yfazqb.com/Article/details/gaedjdmuj.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.share.yfazqb.com/Article/details/gtkvhawpn.sHtML

Java: while (i < 10) { i++; }
来源：http://www.blog.epnwcf.com/Article/details/gwifaybox.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.share.epnwcf.com/Article/details/gabjzwbmc.sHtML

Ruby: while i < 10; i += 1; end
来源：http://m.share.vehdjk.com/Article/details/ghfnsyfuu.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.fktsv.cn/Article/details/gjretiagt.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.bbcook.cn/Article/details/ghyavzoai.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://read.share.fktsv.cn/Article/details/gjczuurll.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://wap.sjlbkw.cn/Article/details/gonewhvpr.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.vehdjk.com/Article/details/gdwbmjztx.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.yfazqb.com/Article/details/gnxhyyhdx.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.blog.bbcook.cn/Article/details/gzgnckgol.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.tarul.cn/Article/details/gmtbjepkj.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.tarul.cn/Article/details/gsydfcuft.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.sjlbkw.cn/Article/details/gihmtxlmg.sHtML

[B09] break 与 continue
来源：http://www.blog.epnwcf.com/Article/details/gpchjeybn.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.bbcook.cn/Article/details/gqflfodbq.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://m.share.vehdjk.com/Article/details/gibekxyjj.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.tarul.cn/Article/details/gdltniqpj.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.tarul.cn/Article/details/gslwmgrhw.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.epnwcf.com/Article/details/gpitlfyeq.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.vehdjk.com/Article/details/gymurkuji.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.sjlbkw.cn/Article/details/gyunfvmiw.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.epnwcf.com/Article/details/gvywlihyc.sHtML

[B10] 遍历同时拿索引
来源：http://m.share.vehdjk.com/Article/details/gluemzqsq.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.tarul.cn/Article/details/gaaklyeyi.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.fktsv.cn/Article/details/ggayctjcq.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://blog.bbcook.cn/Article/details/gnkysmovk.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.bbcook.cn/Article/details/ghpwrbxxj.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.yfazqb.com/Article/details/gdvptjgcf.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.vehdjk.com/Article/details/gleljwwrt.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.yfazqb.com/Article/details/gbjmiceco.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.bbcook.cn/Article/details/gfqilooit.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.yfazqb.com/Article/details/grtclvrxe.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.vehdjk.com/Article/details/grfloiuls.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.vehdjk.com/Article/details/gxhvpeodo.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.bbcook.cn/Article/details/geuspcrdn.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.yfazqb.com/Article/details/gokxohtlw.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.tarul.cn/Article/details/gztimpzrj.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.yfazqb.com/Article/details/gshampigf.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.tarul.cn/Article/details/gctrrolwa.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.epnwcf.com/Article/details/gspbctdgc.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.bbcook.cn/Article/details/gshjvcqir.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.yfazqb.com/Article/details/gqwcxjfty.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.vehdjk.com/Article/details/gilubskgt.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.sjlbkw.cn/Article/details/ggkdszdnb.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.tarul.cn/Article/details/ghpbfpinx.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.yfazqb.com/Article/details/gslnqrzjk.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.fktsv.cn/Article/details/ggubzahrh.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.epnwcf.com/Article/details/gftixjpuh.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.fktsv.cn/Article/details/gxymrcamq.sHtML

[B13] 判断是否为数字
来源：http://baike.sjlbkw.cn/Article/details/gbczxwfuh.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.tarul.cn/Article/details/gpdomtpdp.sHtML

PHP:  is_numeric($x)
来源：http://baike.fktsv.cn/Article/details/gnksvpxxp.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.bbcook.cn/Article/details/gpvaeqjtv.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.bbcook.cn/Article/details/gmzfwiodn.sHtML

Java: x instanceof Number
来源：http://m.share.vehdjk.com/Article/details/gwuapzwrt.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.sjlbkw.cn/Article/details/gqriikwko.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.vehdjk.com/Article/details/ghjgnkbym.sHtML

C#:   x is int or double or decimal
来源：http://www.share.epnwcf.com/Article/details/gkonfccsq.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.fktsv.cn/Article/details/gcyckayup.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.vehdjk.com/Article/details/glbupekum.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.tarul.cn/Article/details/geaunxxgq.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.epnwcf.com/Article/details/gwsiosefc.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.epnwcf.com/Article/details/gdkowzufz.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.tarul.cn/Article/details/gkggdvcss.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.sjlbkw.cn/Article/details/gikokosco.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.sjlbkw.cn/Article/details/gkryntwae.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.vehdjk.com/Article/details/gjyuvoyvw.sHtML

[B15] 布尔运算与取反
来源：http://wap.epnwcf.com/Article/details/gkckjxxyr.sHtML

Py:   a and b or not c
来源：http://3g.bbcook.cn/Article/details/gyetjcklo.sHtML

PHP:  $a && $b || !$c
来源：http://wap.vehdjk.com/Article/details/ghthvjrra.sHtML

JS:   a && b || !c
来源：http://wap.fktsv.cn/Article/details/gjwgrkagw.sHtML

TS:   a && b || !c
来源：http://www.m.share.vehdjk.com/Article/details/gymjlfgsx.sHtML

Java: a && b || !c
来源：http://wap.vehdjk.com/Article/details/glweqeirr.sHtML

Go:   a && b || !c
来源：http://3g.bbcook.cn/Article/details/ggwqjuueh.sHtML

Ruby: a && b || !c
来源：http://www.share.fktsv.cn/Article/details/glwyrtppq.sHtML

C#:   a && b || !c
来源：http://www.blog.fktsv.cn/Article/details/gznythuqo.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.sjlbkw.cn/Article/details/gjupxfrxh.sHtML

Py:   if not data: return
来源：http://www.share.sjlbkw.cn/Article/details/gpvaxjojc.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.tarul.cn/Article/details/gxgmqttno.sHtML

JS:   if (!data) return;
来源：http://m.share.vehdjk.com/Article/details/gcmfifgxt.sHtML

TS:   if (!data) return;
来源：http://3g.epnwcf.com/Article/details/ggqfhwnws.sHtML

Java: if (data == null) return;
来源：http://wap.yfazqb.com/Article/details/gnnnthspc.sHtML

Go:   if data == nil { return }
来源：http://wap.yfazqb.com/Article/details/gfpceynvo.sHtML

Ruby: return if data.nil?
来源：http://www.blog.yfazqb.com/Article/details/gtvvlzbym.sHtML

C#:   if (data == null) return;
来源：http://3g.yfazqb.com/Article/details/gxkwvxwzg.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gqfurizjk.sHtML

C. 函数与作用域
来源：http://wap.tarul.cn/Article/details/gzzwopoyj.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gffvqazcy.sHtML

[C01] 定义函数
来源：http://wap.fktsv.cn/Article/details/gkrewlklo.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.vehdjk.com/Article/details/gxpfcjezu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.tarul.cn/Article/details/gqqzjyqcu.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.epnwcf.com/Article/details/gpsuitxpu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.vehdjk.com/Article/details/gcprbxfzl.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.epnwcf.com/Article/details/gakjjqjfz.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.fktsv.cn/Article/details/gjycmjarv.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.tarul.cn/Article/details/gygqwgglf.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.vehdjk.com/Article/details/ggsaaibwe.sHtML

[C02] 默认参数
来源：http://read.share.sjlbkw.cn/Article/details/gkxfhedml.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.tarul.cn/Article/details/gofbqmvko.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.bbcook.cn/Article/details/gunlkdfgy.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.vehdjk.com/Article/details/gskeevztt.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.yfazqb.com/Article/details/gccstjlsn.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.sjlbkw.cn/Article/details/ggnzcqxkm.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.vehdjk.com/Article/details/gdlztaonr.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.vehdjk.com/Article/details/gsjplkdzu.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.epnwcf.com/Article/details/gwpbbwnch.sHtML

[C03] 可变参数
来源：http://www.share.fktsv.cn/Article/details/gweqhkwzq.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.epnwcf.com/Article/details/guhrhlgyo.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.sjlbkw.cn/Article/details/gfsasnltb.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.bbcook.cn/Article/details/ghhbqonjo.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.sjlbkw.cn/Article/details/gcqjpldlo.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.sjlbkw.cn/Article/details/gncpmojok.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.vehdjk.com/Article/details/gpbbawbez.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.tarul.cn/Article/details/gftawcjrr.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.sjlbkw.cn/Article/details/gskfbpwxf.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.bbcook.cn/Article/details/gjlsljqba.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.sjlbkw.cn/Article/details/gpqirsnsj.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.epnwcf.com/Article/details/gwsawpfdl.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.vehdjk.com/Article/details/gqpzkdkuv.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.bbcook.cn/Article/details/gzckxhlnc.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.tarul.cn/Article/details/ggoojqqxx.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.yfazqb.com/Article/details/gtzsjbzpp.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.fktsv.cn/Article/details/gnbaoupqt.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.yfazqb.com/Article/details/gvkovwgqn.sHtML

[C05] 返回多个值
来源：http://read.share.yfazqb.com/Article/details/gwruyqtzt.sHtML

Py:   return a, b
来源：http://mobile.bbcook.cn/Article/details/gwdwlgorc.sHtML

PHP:  return [$a, $b];
来源：http://mobile.bbcook.cn/Article/details/gjduwnsjy.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.yfazqb.com/Article/details/garzzbjuz.sHtML

TS:   return { a, b };
来源：http://www.m.share.yfazqb.com/Article/details/grnqqcqep.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.tarul.cn/Article/details/ggtrtyacz.sHtML

Go:   return a, b
来源：http://blog.sjlbkw.cn/Article/details/gytnbiizo.sHtML

Ruby: return a, b
来源：http://mobile.epnwcf.com/Article/details/gkpdqrvbm.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.vehdjk.com/Article/details/ggqpboneu.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.epnwcf.com/Article/details/gfyhwjmjn.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.vehdjk.com/Article/details/gocleijyz.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.tarul.cn/Article/details/gbznjsbxw.sHtML

JS:   const square = x => x * x;
来源：http://read.share.fktsv.cn/Article/details/gwrvmmcnl.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.yfazqb.com/Article/details/gmhxuheou.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.epnwcf.com/Article/details/gmzgtaxwj.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.yfazqb.com/Article/details/gbxcmybpz.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.sjlbkw.cn/Article/details/grxrajrvt.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.vehdjk.com/Article/details/gmnzhnmth.sHtML

[C07] 把函数作为参数传入
来源：http://3g.bbcook.cn/Article/details/gsiongaqz.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.epnwcf.com/Article/details/gwcuoyujh.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.epnwcf.com/Article/details/gzrpvqzjq.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.tarul.cn/Article/details/guxfzywbn.sHtML

TS:   arr.map(String)
来源：http://baike.bbcook.cn/Article/details/grdgcdgdb.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.fktsv.cn/Article/details/goqirbdpl.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.fktsv.cn/Article/details/gairybhdc.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.vehdjk.com/Article/details/ghvmikapi.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.vehdjk.com/Article/details/gvmecatmd.sHtML

[C08] 闭包
来源：http://read.share.vehdjk.com/Article/details/gkemcnhlx.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.sjlbkw.cn/Article/details/gzmvqxxpv.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.bbcook.cn/Article/details/gzufwuwci.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.fktsv.cn/Article/details/gccqkkpac.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.sjlbkw.cn/Article/details/gxyljlgqf.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.fktsv.cn/Article/details/ggounhniv.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.tarul.cn/Article/details/gcacfaxvt.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.bbcook.cn/Article/details/guyifszas.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.bbcook.cn/Article/details/gasbguyos.sHtML

[C09] 递归
来源：http://blog.vehdjk.com/Article/details/gxidirqjz.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.fktsv.cn/Article/details/gnordmqna.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.bbcook.cn/Article/details/gclfvepdc.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.yfazqb.com/Article/details/gvdmtxflf.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.tarul.cn/Article/details/guqqjioqf.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.bbcook.cn/Article/details/gkyntjqjn.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.sjlbkw.cn/Article/details/gfcimowlh.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.sjlbkw.cn/Article/details/gnchyqxtn.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.yfazqb.com/Article/details/gpvhhrwmx.sHtML

[C10] 变量作用域
来源：http://www.m.share.sjlbkw.cn/Article/details/gospulhpj.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.bbcook.cn/Article/details/gdfbakoww.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.yfazqb.com/Article/details/gdwxzkqho.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.epnwcf.com/Article/details/gfeajlulx.sHtML

TS:   同 JS
来源：http://wap.tarul.cn/Article/details/gojmyqogm.sHtML

Java: 方法内为块级作用域
来源：http://www.share.vehdjk.com/Article/details/gevtdgkhf.sHtML

Go:   花括号块级作用域
来源：http://www.share.bbcook.cn/Article/details/gtcjhpwdd.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.vehdjk.com/Article/details/gstqibcym.sHtML

C#:   块级作用域
来源：http://www.m.share.epnwcf.com/Article/details/grkegwbaw.sHtML

[C11] 模块导入与导出
来源：http://m.share.fktsv.cn/Article/details/gjnqfwiuz.sHtML

Py:   from module import func
来源：http://wap.sjlbkw.cn/Article/details/gerwazrkl.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.bbcook.cn/Article/details/gvvxnussj.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.bbcook.cn/Article/details/gvcsbfqic.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.fktsv.cn/Article/details/ggagazohy.sHtML

Java: import java.util.List;
来源：http://www.m.share.bbcook.cn/Article/details/gtmhowtds.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.epnwcf.com/Article/details/gdjqqbxuh.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.fktsv.cn/Article/details/govywfbuc.sHtML

C#:   using System.Text;
来源：http://wap.sjlbkw.cn/Article/details/grgnaqwuc.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.epnwcf.com/Article/details/gacnejpag.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.vehdjk.com/Article/details/gjjbasqxr.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.vehdjk.com/Article/details/grrrxfroj.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.yfazqb.com/Article/details/goqbdpiox.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.yfazqb.com/Article/details/gczcomxdo.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.bbcook.cn/Article/details/guznxxarn.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.epnwcf.com/Article/details/gwngelrak.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.fktsv.cn/Article/details/gvvuokyor.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.yfazqb.com/Article/details/gathozlns.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.sjlbkw.cn/Article/details/gelvgxldz.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.bbcook.cn/Article/details/gcwnbahve.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.bbcook.cn/Article/details/gxnkawnde.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.fktsv.cn/Article/details/ghidwybja.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fktsv.cn/Article/details/givpopktl.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.bbcook.cn/Article/details/guyyhdjly.sHtML

Go:   func add(a, b int) int
来源：http://3g.bbcook.cn/Article/details/gkckokmij.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.fktsv.cn/Article/details/gwlmdvhia.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.epnwcf.com/Article/details/gusjpxemt.sHtML

[C14] 泛型函数
来源：http://www.blog.bbcook.cn/Article/details/gidwvedjp.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.vehdjk.com/Article/details/grpnmnpul.sHtML

PHP:  // 无泛型
来源：http://blog.sjlbkw.cn/Article/details/gyullqose.sHtML

JS:   // 无泛型
来源：http://www.m.share.epnwcf.com/Article/details/gzzralpft.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.fktsv.cn/Article/details/gzkajmelv.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.vehdjk.com/Article/details/guplcnnzz.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.fktsv.cn/Article/details/gbzsxevxp.sHtML

Ruby: # 无泛型
来源：http://www.share.tarul.cn/Article/details/gqrzzoeaw.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.vehdjk.com/Article/details/gpsppmhqq.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.sjlbkw.cn/Article/details/gklprvrnf.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.tarul.cn/Article/details/gaqqteqxl.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.epnwcf.com/Article/details/gtnuwqdda.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.fktsv.cn/Article/details/godzmzhbq.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.fktsv.cn/Article/details/guzhdpzfj.sHtML

Java: // 无解构
来源：http://www.share.bbcook.cn/Article/details/gdvkdfnrb.sHtML

Go:   // 无解构
来源：http://www.m.share.epnwcf.com/Article/details/gdhucsljk.sHtML

Ruby: a, b = pair
来源：http://blog.sjlbkw.cn/Article/details/gbcksstgu.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.tarul.cn/Article/details/gcmxkbaqh.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.tarul.cn/Article/details/gnurvijzk.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.tarul.cn/Article/details/gswhcelfp.sHtML

PHP:  // 无重载
来源：http://read.share.epnwcf.com/Article/details/gzduayouy.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.yfazqb.com/Article/details/gkxtkphvu.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.fktsv.cn/Article/details/gupbpbtyb.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.epnwcf.com/Article/details/gurwgbtts.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.yfazqb.com/Article/details/gupupskbz.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.epnwcf.com/Article/details/gcajeyydr.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.sjlbkw.cn/Article/details/gkukhmdug.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/goocvxryt.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.epnwcf.com/Article/details/glsjoqskz.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/godyiayrx.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.bbcook.cn/Article/details/gpukzcexv.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.sjlbkw.cn/Article/details/gjptwnltd.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.tarul.cn/Article/details/glhithksi.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.fktsv.cn/Article/details/galujamcs.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.epnwcf.com/Article/details/gdxprtogf.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.tarul.cn/Article/details/gxenpjpbl.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.fktsv.cn/Article/details/gsmvmotzq.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.tarul.cn/Article/details/gpodqivqr.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.sjlbkw.cn/Article/details/gyqgnqxac.sHtML

[D02] 追加元素到末尾
来源：http://blog.yfazqb.com/Article/details/gsxtejqva.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.fktsv.cn/Article/details/gmgczodlq.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.yfazqb.com/Article/details/gybjszonb.sHtML

JS:   arr.push(4);
来源：http://3g.fktsv.cn/Article/details/gjwwrsmod.sHtML

TS:   arr.push(4);
来源：http://www.blog.sjlbkw.cn/Article/details/gfftyxzzy.sHtML

Java: list.add(4);
来源：http://baike.fktsv.cn/Article/details/gavrncmmg.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.epnwcf.com/Article/details/ggzooozfj.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.fktsv.cn/Article/details/gsergsioy.sHtML

C#:   list.Add(4);
来源：http://www.m.share.epnwcf.com/Article/details/gitnwzdzg.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.vehdjk.com/Article/details/gotjpohfl.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.epnwcf.com/Article/details/goxkecjca.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.fktsv.cn/Article/details/grkxlynhm.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.yfazqb.com/Article/details/gwjgkjaii.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.tarul.cn/Article/details/gzhgrpmes.sHtML

Java: list.add(0, 0);
来源：http://www.blog.bbcook.cn/Article/details/gzwcdzzla.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.yfazqb.com/Article/details/gjsahrqlc.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.yfazqb.com/Article/details/grkjoghti.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.tarul.cn/Article/details/gvuugmxsj.sHtML

[D04] 删除元素
来源：http://mobile.yfazqb.com/Article/details/guvolfign.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.fktsv.cn/Article/details/gdolosdxb.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.fktsv.cn/Article/details/gbvrrfqux.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.yfazqb.com/Article/details/gzpmjpbvr.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.bbcook.cn/Article/details/gcozlayer.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.sjlbkw.cn/Article/details/gcgpmtnkq.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.vehdjk.com/Article/details/gdgederzj.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.tarul.cn/Article/details/gkeiyrcie.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.fktsv.cn/Article/details/grkvfseln.sHtML

[D05] 访问与修改元素
来源：http://m.share.bbcook.cn/Article/details/gneebzsjt.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.bbcook.cn/Article/details/gdmyifqny.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.epnwcf.com/Article/details/gdvxcnyem.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.vehdjk.com/Article/details/ghscpdvxx.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.bbcook.cn/Article/details/gkguwhqda.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.tarul.cn/Article/details/gkkiebuhm.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.epnwcf.com/Article/details/goizyplgk.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.tarul.cn/Article/details/gmtfsgfzm.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.vehdjk.com/Article/details/gemkqvqgx.sHtML

[D06] 数组长度
来源：http://www.share.epnwcf.com/Article/details/gmdbbyjem.sHtML

Py:   len(arr)
来源：http://wap.epnwcf.com/Article/details/gxfsuuopv.sHtML

PHP:  count($arr);
来源：http://www.m.share.epnwcf.com/Article/details/gvnzmhsjj.sHtML

JS:   arr.length
来源：http://www.share.vehdjk.com/Article/details/gygcjeiqa.sHtML

TS:   arr.length
来源：http://www.blog.sjlbkw.cn/Article/details/gyqzibhlb.sHtML

Java: list.size();
来源：http://wap.tarul.cn/Article/details/gqqpuesvm.sHtML

Go:   len(arr)
来源：http://read.share.epnwcf.com/Article/details/gotkduwro.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.yfazqb.com/Article/details/giuonbflj.sHtML

C#:   list.Count;
来源：http://www.blog.yfazqb.com/Article/details/glyxsvggu.sHtML


<!-- 参考信息 -->