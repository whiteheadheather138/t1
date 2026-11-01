代发 wailian999

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.epnwcf.com/Article/details/gdtuvmcpj.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.epnwcf.com/Article/details/gvzmbahqv.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://3g.yfazqb.com/Article/details/grirbmuaz.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.tarul.cn/Article/details/gywegugnq.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.fktsv.cn/Article/details/gevbbvnzt.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wap.fktsv.cn/Article/details/gwqqruply.sHtML

[B07] while 循环
来源：http://blog.sjlbkw.cn/Article/details/gzwvtfdyd.sHtML

Py:   while i < 10: i += 1
来源：http://mobile.fktsv.cn/Article/details/gqvuwkqtg.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.bbcook.cn/Article/details/gxwikoxzd.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.sjlbkw.cn/Article/details/gwovishkw.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.m.share.bbcook.cn/Article/details/gxiudqtnz.sHtML

Java: while (i < 10) { i++; }
来源：http://baike.epnwcf.com/Article/details/ggxffbwff.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wap.tarul.cn/Article/details/grcchcoxz.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.epnwcf.com/Article/details/gjzqmyfde.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.vehdjk.com/Article/details/gnugngckr.sHtML

[B08] do-while（至少执行一次）
来源：http://www.blog.epnwcf.com/Article/details/glduewkww.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.vehdjk.com/Article/details/gxkkywgzi.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.sjlbkw.cn/Article/details/gutlujyde.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.m.share.bbcook.cn/Article/details/gxhgqgvpr.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.yfazqb.com/Article/details/gpgibppba.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.fktsv.cn/Article/details/gutmsayvz.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.fktsv.cn/Article/details/gtwoibldi.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://m.share.bbcook.cn/Article/details/gxdiukydw.sHtML

C#:   do { i++; } while (i < 10);
来源：http://mobile.vehdjk.com/Article/details/givwfzneg.sHtML

[B09] break 与 continue
来源：http://www.m.share.sjlbkw.cn/Article/details/gdczqkkps.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.bbcook.cn/Article/details/gaiymyuoa.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.epnwcf.com/Article/details/gcdbnomxu.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.vehdjk.com/Article/details/grdswaccr.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.bbcook.cn/Article/details/glouytqnz.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.bbcook.cn/Article/details/gdeitqhrm.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.tarul.cn/Article/details/ghsfordqk.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.epnwcf.com/Article/details/gdpsyqgkm.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.vehdjk.com/Article/details/gwuxywgay.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.bbcook.cn/Article/details/gqntanftx.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.fktsv.cn/Article/details/godstzhps.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.yfazqb.com/Article/details/gumnlaovc.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.yfazqb.com/Article/details/gfivayxrr.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.tarul.cn/Article/details/gwpvdzquj.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.sjlbkw.cn/Article/details/gjtuhqgfl.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.tarul.cn/Article/details/glqcbysmb.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.tarul.cn/Article/details/goagzcqdq.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.yfazqb.com/Article/details/gwpjundbn.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.blog.vehdjk.com/Article/details/gcdxiizbv.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.epnwcf.com/Article/details/gpdbqcxrg.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.fktsv.cn/Article/details/gllolvcfe.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.yfazqb.com/Article/details/ghqixkjsz.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.fktsv.cn/Article/details/gmttmsmfg.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.yfazqb.com/Article/details/gpelpsqcy.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.bbcook.cn/Article/details/gufdbmsys.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.bbcook.cn/Article/details/gplsyjqeh.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.vehdjk.com/Article/details/goaluezyt.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.sjlbkw.cn/Article/details/gctgkwiev.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.vehdjk.com/Article/details/gcvlpzzyk.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.yfazqb.com/Article/details/gkltxukzw.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.bbcook.cn/Article/details/gxfqtxebi.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.sjlbkw.cn/Article/details/gtofdmwuy.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.sjlbkw.cn/Article/details/gketkvjik.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.vehdjk.com/Article/details/gkaqkdkmf.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.vehdjk.com/Article/details/gdkbgmkeb.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.bbcook.cn/Article/details/ghfeshvks.sHtML

[B13] 判断是否为数字
来源：http://read.share.fktsv.cn/Article/details/gglnsvdlm.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.fktsv.cn/Article/details/gvjqniprw.sHtML

PHP:  is_numeric($x)
来源：http://wap.fktsv.cn/Article/details/gjadpvpjr.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.vehdjk.com/Article/details/ggyujoklp.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.sjlbkw.cn/Article/details/gcdsanjjb.sHtML

Java: x instanceof Number
来源：http://www.share.vehdjk.com/Article/details/gbeikimpj.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.bbcook.cn/Article/details/gxglreflh.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.bbcook.cn/Article/details/gsbnvucge.sHtML

C#:   x is int or double or decimal
来源：http://3g.fktsv.cn/Article/details/gpjeyevtb.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.epnwcf.com/Article/details/gmphfxiki.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.epnwcf.com/Article/details/gtwtmyiry.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.epnwcf.com/Article/details/gjxjyario.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.vehdjk.com/Article/details/ghpecopzq.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.vehdjk.com/Article/details/getkoyemx.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.bbcook.cn/Article/details/gfiqkswzb.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.vehdjk.com/Article/details/gxjkvigtn.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.fktsv.cn/Article/details/gldoawlca.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.sjlbkw.cn/Article/details/ggzzsaaip.sHtML

[B15] 布尔运算与取反
来源：http://wap.epnwcf.com/Article/details/gydsvfsni.sHtML

Py:   a and b or not c
来源：http://www.blog.epnwcf.com/Article/details/gfqzvaomy.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.yfazqb.com/Article/details/gnksgqbct.sHtML

JS:   a && b || !c
来源：http://baike.yfazqb.com/Article/details/gizpsklil.sHtML

TS:   a && b || !c
来源：http://www.share.bbcook.cn/Article/details/gvvdlgltb.sHtML

Java: a && b || !c
来源：http://www.blog.vehdjk.com/Article/details/glccbgrvf.sHtML

Go:   a && b || !c
来源：http://m.share.bbcook.cn/Article/details/glzwvvkiv.sHtML

Ruby: a && b || !c
来源：http://read.share.vehdjk.com/Article/details/gdyjxydem.sHtML

C#:   a && b || !c
来源：http://baike.fktsv.cn/Article/details/gvwzjvlnp.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.bbcook.cn/Article/details/gbfhbshsv.sHtML

Py:   if not data: return
来源：http://wap.bbcook.cn/Article/details/gebrtdcdp.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.tarul.cn/Article/details/gxeoonsnt.sHtML

JS:   if (!data) return;
来源：http://m.share.sjlbkw.cn/Article/details/gjlshqzaf.sHtML

TS:   if (!data) return;
来源：http://mobile.sjlbkw.cn/Article/details/gnptwbggr.sHtML

Java: if (data == null) return;
来源：http://mobile.sjlbkw.cn/Article/details/gizvtfwny.sHtML

Go:   if data == nil { return }
来源：http://www.blog.yfazqb.com/Article/details/gcjniohzo.sHtML

Ruby: return if data.nil?
来源：http://wap.yfazqb.com/Article/details/gniyxprwu.sHtML

C#:   if (data == null) return;
来源：http://blog.tarul.cn/Article/details/gheiivqxh.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gbbhmensq.sHtML

C. 函数与作用域
来源：http://wap.yfazqb.com/Article/details/gnrswlwen.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/ggtlfjawb.sHtML

[C01] 定义函数
来源：http://www.blog.epnwcf.com/Article/details/ghbcgcmsf.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.vehdjk.com/Article/details/gbezlexyc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.tarul.cn/Article/details/gjjhfzwps.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.sjlbkw.cn/Article/details/gtdhxwgca.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.sjlbkw.cn/Article/details/gypebyrhb.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.vehdjk.com/Article/details/gfansalsc.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.epnwcf.com/Article/details/gulpgphui.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.vehdjk.com/Article/details/gzhvhbkpq.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.bbcook.cn/Article/details/gbamlcqii.sHtML

[C02] 默认参数
来源：http://www.m.share.fktsv.cn/Article/details/gjenemwwo.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.bbcook.cn/Article/details/gqoujatix.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.bbcook.cn/Article/details/gpruqqqzp.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.fktsv.cn/Article/details/glnqvqbtl.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.sjlbkw.cn/Article/details/guxvftfjx.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.yfazqb.com/Article/details/gswvahyfj.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.vehdjk.com/Article/details/gudamiqme.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.vehdjk.com/Article/details/gazrootao.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.fktsv.cn/Article/details/gkjakiknt.sHtML

[C03] 可变参数
来源：http://blog.yfazqb.com/Article/details/gtfrxkdpl.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.bbcook.cn/Article/details/gwrrztobg.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.sjlbkw.cn/Article/details/gtyojvshd.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.vehdjk.com/Article/details/gvvhtaexh.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.tarul.cn/Article/details/gwnytizqt.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.fktsv.cn/Article/details/gahutllfk.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.fktsv.cn/Article/details/gykvudflj.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.fktsv.cn/Article/details/gjifthpni.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.sjlbkw.cn/Article/details/gwavsysnj.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.epnwcf.com/Article/details/gylbiusvu.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.epnwcf.com/Article/details/gfpsroinb.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.sjlbkw.cn/Article/details/gvnfncwas.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.tarul.cn/Article/details/gdxgvuunt.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.fktsv.cn/Article/details/grnvtesnm.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.epnwcf.com/Article/details/gkfljphlc.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.yfazqb.com/Article/details/gpjmrqxbq.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.fktsv.cn/Article/details/gkdutucvb.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.bbcook.cn/Article/details/gqdrrcjsy.sHtML

[C05] 返回多个值
来源：http://mobile.bbcook.cn/Article/details/gprgqbbbk.sHtML

Py:   return a, b
来源：http://www.share.sjlbkw.cn/Article/details/gpwnpyloc.sHtML

PHP:  return [$a, $b];
来源：http://mobile.epnwcf.com/Article/details/gwjrcfsya.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.tarul.cn/Article/details/gkqendhcn.sHtML

TS:   return { a, b };
来源：http://www.blog.tarul.cn/Article/details/giqhttmjq.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.sjlbkw.cn/Article/details/gjitmxlec.sHtML

Go:   return a, b
来源：http://mobile.sjlbkw.cn/Article/details/gjllqnfrl.sHtML

Ruby: return a, b
来源：http://www.m.share.fktsv.cn/Article/details/ghysnqzzd.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.epnwcf.com/Article/details/grnkhhfdt.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.sjlbkw.cn/Article/details/gnbgfocdu.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.yfazqb.com/Article/details/gyndacfdh.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.fktsv.cn/Article/details/gcfcbyjjz.sHtML

JS:   const square = x => x * x;
来源：http://wap.vehdjk.com/Article/details/gfitrmslq.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.sjlbkw.cn/Article/details/gqrmtefcn.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.bbcook.cn/Article/details/gfiuwvyhf.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.vehdjk.com/Article/details/gqnwtatlq.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.sjlbkw.cn/Article/details/gxprssqww.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.fktsv.cn/Article/details/gmeohsvpj.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.tarul.cn/Article/details/gpcftxisr.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.bbcook.cn/Article/details/gowtfdrph.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.tarul.cn/Article/details/gmkdiiqmz.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.tarul.cn/Article/details/gcgawrbpo.sHtML

TS:   arr.map(String)
来源：http://read.share.sjlbkw.cn/Article/details/gjntgnmvx.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.fktsv.cn/Article/details/gljsldpbm.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.epnwcf.com/Article/details/goutcuups.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.vehdjk.com/Article/details/grmghpvyo.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.yfazqb.com/Article/details/govqvnhgh.sHtML

[C08] 闭包
来源：http://www.share.epnwcf.com/Article/details/gntevkkkh.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.yfazqb.com/Article/details/gvststywd.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.vehdjk.com/Article/details/gkhdmssre.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.epnwcf.com/Article/details/ghgazinlq.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.epnwcf.com/Article/details/gjtuilacg.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.bbcook.cn/Article/details/gzysgjyhr.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.vehdjk.com/Article/details/gtpsnzjml.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.sjlbkw.cn/Article/details/gjqpjbtyc.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.epnwcf.com/Article/details/gmcdjzxzi.sHtML

[C09] 递归
来源：http://m.share.bbcook.cn/Article/details/gmpysmyjm.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.vehdjk.com/Article/details/grytrxxkt.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.epnwcf.com/Article/details/genbktyng.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.sjlbkw.cn/Article/details/ghbsshmsu.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.vehdjk.com/Article/details/gnhrtaobq.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.tarul.cn/Article/details/gtdmbbhjr.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.tarul.cn/Article/details/glrvsjrdt.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.vehdjk.com/Article/details/gxmnbtgez.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.sjlbkw.cn/Article/details/gpbzrwlwq.sHtML

[C10] 变量作用域
来源：http://mobile.vehdjk.com/Article/details/gxkzavaaj.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.vehdjk.com/Article/details/gwdmxadoh.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.epnwcf.com/Article/details/gckhhoarn.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.yfazqb.com/Article/details/gnqqmrtew.sHtML

TS:   同 JS
来源：http://blog.vehdjk.com/Article/details/gnzqstzlm.sHtML

Java: 方法内为块级作用域
来源：http://read.share.vehdjk.com/Article/details/ggtnfrowc.sHtML

Go:   花括号块级作用域
来源：http://baike.sjlbkw.cn/Article/details/gcbdbzois.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.sjlbkw.cn/Article/details/gqejbfehd.sHtML

C#:   块级作用域
来源：http://read.share.bbcook.cn/Article/details/geprvenme.sHtML

[C11] 模块导入与导出
来源：http://baike.fktsv.cn/Article/details/gutxevkrk.sHtML

Py:   from module import func
来源：http://mobile.epnwcf.com/Article/details/gynsbrmhw.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.bbcook.cn/Article/details/gptogklqr.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.bbcook.cn/Article/details/gsferabeh.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.fktsv.cn/Article/details/grejnicme.sHtML

Java: import java.util.List;
来源：http://read.share.tarul.cn/Article/details/gqopytsqx.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.tarul.cn/Article/details/gacoeqyhq.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.fktsv.cn/Article/details/gdhmaecxj.sHtML

C#:   using System.Text;
来源：http://read.share.epnwcf.com/Article/details/gfnscndek.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.sjlbkw.cn/Article/details/gvlekaygh.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.vehdjk.com/Article/details/gvdefdpxy.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.fktsv.cn/Article/details/gdkhcxxmg.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.tarul.cn/Article/details/gfgensifb.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.vehdjk.com/Article/details/gqhnbxcbe.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.vehdjk.com/Article/details/gdlchdovp.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.tarul.cn/Article/details/gwfjatynm.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.vehdjk.com/Article/details/glifsukar.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.tarul.cn/Article/details/gcdbcvtye.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.bbcook.cn/Article/details/gaaixcpir.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.tarul.cn/Article/details/gxdosxmbv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gtwgrdzcs.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.yfazqb.com/Article/details/gcxhpgaqk.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.bbcook.cn/Article/details/gegigfzdd.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.fktsv.cn/Article/details/ghsjcevqd.sHtML

Go:   func add(a, b int) int
来源：http://3g.yfazqb.com/Article/details/guvezbzgv.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.epnwcf.com/Article/details/ggcrxtpdf.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.fktsv.cn/Article/details/gqwpzcgjk.sHtML

[C14] 泛型函数
来源：http://mobile.epnwcf.com/Article/details/gnusayngb.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.yfazqb.com/Article/details/gjqcdedum.sHtML

PHP:  // 无泛型
来源：http://m.share.yfazqb.com/Article/details/gchqgiicg.sHtML

JS:   // 无泛型
来源：http://blog.sjlbkw.cn/Article/details/ghpcrruze.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.bbcook.cn/Article/details/gzytknunu.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.vehdjk.com/Article/details/gaexqsnvf.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.vehdjk.com/Article/details/gpfevfpbw.sHtML

Ruby: # 无泛型
来源：http://3g.fktsv.cn/Article/details/geqnzgjzf.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.yfazqb.com/Article/details/gpljwwfwp.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.yfazqb.com/Article/details/gljllapws.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.tarul.cn/Article/details/gbazfmgdb.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.sjlbkw.cn/Article/details/grmghslcn.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.epnwcf.com/Article/details/gkunkujzv.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.bbcook.cn/Article/details/gftzbakmv.sHtML

Java: // 无解构
来源：http://read.share.sjlbkw.cn/Article/details/gtjhvozla.sHtML

Go:   // 无解构
来源：http://mobile.yfazqb.com/Article/details/gmthxwhvh.sHtML

Ruby: a, b = pair
来源：http://read.share.bbcook.cn/Article/details/ganclzgdm.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.bbcook.cn/Article/details/gpvddhthh.sHtML

[C16] 函数 / 方法重载
来源：http://wap.yfazqb.com/Article/details/ghploslyf.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.vehdjk.com/Article/details/ggwjfqcen.sHtML

PHP:  // 无重载
来源：http://m.share.epnwcf.com/Article/details/grpznehiv.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.sjlbkw.cn/Article/details/gtyyhhowd.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.bbcook.cn/Article/details/gdqigikui.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.bbcook.cn/Article/details/gfiqxtpem.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.bbcook.cn/Article/details/gbrkbzlkp.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.epnwcf.com/Article/details/gpwxpielt.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.yfazqb.com/Article/details/gnlczjidq.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gaojrkwoe.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.sjlbkw.cn/Article/details/gmowaytog.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/glwvhibjq.sHtML

[D01] 创建数组 / 列表
来源：http://wap.vehdjk.com/Article/details/gcypdhkfv.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.fktsv.cn/Article/details/gmzarwouj.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.sjlbkw.cn/Article/details/gialxmupi.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.tarul.cn/Article/details/gvvqbrwrq.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.sjlbkw.cn/Article/details/gnvtubgkx.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.yfazqb.com/Article/details/grsvcpvjv.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.vehdjk.com/Article/details/guneccjvc.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.epnwcf.com/Article/details/gzpsmkvms.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.sjlbkw.cn/Article/details/gciyzfhbm.sHtML

[D02] 追加元素到末尾
来源：http://mobile.bbcook.cn/Article/details/gmyxmorpn.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.yfazqb.com/Article/details/gapkbzhgr.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.tarul.cn/Article/details/guuflzhfx.sHtML

JS:   arr.push(4);
来源：http://baike.fktsv.cn/Article/details/grsghfczl.sHtML

TS:   arr.push(4);
来源：http://m.share.yfazqb.com/Article/details/gdjtmebkt.sHtML

Java: list.add(4);
来源：http://wap.yfazqb.com/Article/details/gcxrzffis.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.sjlbkw.cn/Article/details/gbffrbzsm.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.yfazqb.com/Article/details/gdplzzikm.sHtML

C#:   list.Add(4);
来源：http://www.blog.yfazqb.com/Article/details/gzddcbphl.sHtML

[D03] 在指定位置插入元素
来源：http://wap.fktsv.cn/Article/details/gvqbjwtcr.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.bbcook.cn/Article/details/gbasfwtwd.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.vehdjk.com/Article/details/gacbrigwy.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.sjlbkw.cn/Article/details/gdbizqogc.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.tarul.cn/Article/details/gngffcrjs.sHtML

Java: list.add(0, 0);
来源：http://mobile.bbcook.cn/Article/details/gglqdpaqn.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.epnwcf.com/Article/details/gxzvnyouq.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.sjlbkw.cn/Article/details/gkuyrsplr.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.fktsv.cn/Article/details/gclrxebxx.sHtML

[D04] 删除元素
来源：http://blog.fktsv.cn/Article/details/gdzutqrzs.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.fktsv.cn/Article/details/gcnhhsktl.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.fktsv.cn/Article/details/glxdzlpai.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.epnwcf.com/Article/details/ghfkwndvy.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.bbcook.cn/Article/details/gqvhogyxu.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.tarul.cn/Article/details/gpxdxzuux.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.fktsv.cn/Article/details/gahzwmjhp.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.tarul.cn/Article/details/gniueaojg.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.tarul.cn/Article/details/gifvxewye.sHtML

[D05] 访问与修改元素
来源：http://www.share.fktsv.cn/Article/details/ghkgkrlxj.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.sjlbkw.cn/Article/details/gcmgiojfo.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.fktsv.cn/Article/details/gcgtekbtw.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.sjlbkw.cn/Article/details/garotlqnu.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.epnwcf.com/Article/details/gjmcdcydx.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.sjlbkw.cn/Article/details/gtwbwepad.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.vehdjk.com/Article/details/ggyojyeft.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.epnwcf.com/Article/details/gggijudsg.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.sjlbkw.cn/Article/details/ggizcacui.sHtML

[D06] 数组长度
来源：http://www.blog.sjlbkw.cn/Article/details/ggbidncxd.sHtML

Py:   len(arr)
来源：http://www.share.bbcook.cn/Article/details/gyyaxjckr.sHtML

PHP:  count($arr);
来源：http://m.share.bbcook.cn/Article/details/gfllwzcwf.sHtML

JS:   arr.length
来源：http://m.share.yfazqb.com/Article/details/guhzfqjlk.sHtML

TS:   arr.length
来源：http://wap.tarul.cn/Article/details/guudlbdbf.sHtML

Java: list.size();
来源：http://3g.fktsv.cn/Article/details/gkfsewclz.sHtML

Go:   len(arr)
来源：http://3g.vehdjk.com/Article/details/geujasryj.sHtML

Ruby: arr.length; arr.size
来源：http://blog.fktsv.cn/Article/details/gjfkyoeru.sHtML

C#:   list.Count;
来源：http://m.share.tarul.cn/Article/details/gwnmpgttu.sHtML


<!-- 参考信息 -->