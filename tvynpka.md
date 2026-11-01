代发 wailian999

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.epnwcf.com/Article/details/gyiabnvsa.sHtML

[B06] 遍历字典 / 对象
来源：http://www.blog.tarul.cn/Article/details/gsfxvyzeh.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://baike.tarul.cn/Article/details/gufbrcdcd.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://baike.vehdjk.com/Article/details/gffaxetnu.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.vehdjk.com/Article/details/gbmgeznrb.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.epnwcf.com/Article/details/gkkvnpwim.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.m.share.yfazqb.com/Article/details/gygxtxqjr.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.epnwcf.com/Article/details/gxwpinvxj.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.fktsv.cn/Article/details/gzuubgxay.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.vehdjk.com/Article/details/grvkjosog.sHtML

[B07] while 循环
来源：http://wap.yfazqb.com/Article/details/gxgtjsypv.sHtML

Py:   while i < 10: i += 1
来源：http://m.share.sjlbkw.cn/Article/details/gwthqmbsg.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.fktsv.cn/Article/details/gdclylhjw.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.blog.epnwcf.com/Article/details/gazoryzvr.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.share.yfazqb.com/Article/details/ghutbwesz.sHtML

Java: while (i < 10) { i++; }
来源：http://baike.yfazqb.com/Article/details/gkfgxrvzn.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.bbcook.cn/Article/details/gcojawkya.sHtML

Ruby: while i < 10; i += 1; end
来源：http://m.share.tarul.cn/Article/details/gjiqrwvsk.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.vehdjk.com/Article/details/gslqgkbyn.sHtML

[B08] do-while（至少执行一次）
来源：http://www.blog.epnwcf.com/Article/details/gozxratbl.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.yfazqb.com/Article/details/gjpqnedoo.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.yfazqb.com/Article/details/gbadqqmqh.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.tarul.cn/Article/details/gfgcjekby.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.fktsv.cn/Article/details/gjdigpaot.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.vehdjk.com/Article/details/gwgabzqgw.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.bbcook.cn/Article/details/gjddilali.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.bbcook.cn/Article/details/glzruwqiz.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.vehdjk.com/Article/details/gxxkqczxn.sHtML

[B09] break 与 continue
来源：http://mobile.sjlbkw.cn/Article/details/gtrxieboq.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.vehdjk.com/Article/details/guikeydgl.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.epnwcf.com/Article/details/gjysmekvg.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fktsv.cn/Article/details/gqquursgz.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.epnwcf.com/Article/details/gvcrfdtno.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.yfazqb.com/Article/details/gqypilxmb.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.bbcook.cn/Article/details/ghfuzqirv.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.fktsv.cn/Article/details/gfkzzujxp.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.epnwcf.com/Article/details/gdksgpuat.sHtML

[B10] 遍历同时拿索引
来源：http://wap.tarul.cn/Article/details/gvrcfpgpy.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.epnwcf.com/Article/details/giczudzdj.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.epnwcf.com/Article/details/gzcqkwtyu.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.epnwcf.com/Article/details/gdtqkophh.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.sjlbkw.cn/Article/details/gyomifzil.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.fktsv.cn/Article/details/gyqlhngsk.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.sjlbkw.cn/Article/details/gvovzafkt.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.bbcook.cn/Article/details/gxwtwjvpp.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.vehdjk.com/Article/details/ghvrouncc.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.sjlbkw.cn/Article/details/gnshakafj.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.tarul.cn/Article/details/gxjvoswts.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.sjlbkw.cn/Article/details/gnxvpkrid.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.epnwcf.com/Article/details/gvoiacfjy.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.bbcook.cn/Article/details/gqhirmlom.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.vehdjk.com/Article/details/gsvjluohx.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.yfazqb.com/Article/details/gdvaxdbqq.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.sjlbkw.cn/Article/details/gkkvyhzca.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.vehdjk.com/Article/details/gpnztmbwg.sHtML

[B12] 跳出多层循环
来源：http://blog.tarul.cn/Article/details/gpdelegto.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.fktsv.cn/Article/details/gkjhpvwbb.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.yfazqb.com/Article/details/gdnukqiok.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.epnwcf.com/Article/details/gckpbnqdj.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.vehdjk.com/Article/details/gvlvsfgal.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.sjlbkw.cn/Article/details/gvwvhcntp.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.fktsv.cn/Article/details/gnpouujnt.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.vehdjk.com/Article/details/ghnszdpat.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.bbcook.cn/Article/details/gqdngyzwb.sHtML

[B13] 判断是否为数字
来源：http://www.share.bbcook.cn/Article/details/giwmsifhi.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.epnwcf.com/Article/details/gcmboinbb.sHtML

PHP:  is_numeric($x)
来源：http://read.share.epnwcf.com/Article/details/gptnuuuaf.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.sjlbkw.cn/Article/details/gnmyecflv.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.epnwcf.com/Article/details/ghskvplyo.sHtML

Java: x instanceof Number
来源：http://www.blog.epnwcf.com/Article/details/gcvqnimjn.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.sjlbkw.cn/Article/details/gtrtqqkxu.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.bbcook.cn/Article/details/gkwmvuxur.sHtML

C#:   x is int or double or decimal
来源：http://read.share.yfazqb.com/Article/details/gzrnssqtm.sHtML

[B14] 判断值是否在集合内
来源：http://blog.bbcook.cn/Article/details/gvekapxam.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.tarul.cn/Article/details/giycjakyb.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.yfazqb.com/Article/details/gwkzdmcew.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.epnwcf.com/Article/details/gqkqjdskg.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.epnwcf.com/Article/details/gkirosvrt.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.fktsv.cn/Article/details/gfhuectdm.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.bbcook.cn/Article/details/gmqsgybqh.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.vehdjk.com/Article/details/gpkybpqcw.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.tarul.cn/Article/details/gytnxnhdy.sHtML

[B15] 布尔运算与取反
来源：http://blog.yfazqb.com/Article/details/gnisrzdff.sHtML

Py:   a and b or not c
来源：http://www.blog.vehdjk.com/Article/details/gwghzufzj.sHtML

PHP:  $a && $b || !$c
来源：http://baike.sjlbkw.cn/Article/details/gwltghkqi.sHtML

JS:   a && b || !c
来源：http://3g.tarul.cn/Article/details/gvkskxipb.sHtML

TS:   a && b || !c
来源：http://baike.yfazqb.com/Article/details/gcnvauith.sHtML

Java: a && b || !c
来源：http://baike.sjlbkw.cn/Article/details/gzyfcvfex.sHtML

Go:   a && b || !c
来源：http://blog.vehdjk.com/Article/details/ghyhgafjf.sHtML

Ruby: a && b || !c
来源：http://blog.sjlbkw.cn/Article/details/govplgcpw.sHtML

C#:   a && b || !c
来源：http://www.blog.sjlbkw.cn/Article/details/gplbhaqjg.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.bbcook.cn/Article/details/glrplbzvi.sHtML

Py:   if not data: return
来源：http://www.m.share.yfazqb.com/Article/details/gktwfxgnf.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gszborapw.sHtML

JS:   if (!data) return;
来源：http://www.share.sjlbkw.cn/Article/details/glztpmckj.sHtML

TS:   if (!data) return;
来源：http://blog.sjlbkw.cn/Article/details/gadaqncgg.sHtML

Java: if (data == null) return;
来源：http://blog.tarul.cn/Article/details/gjckyckeh.sHtML

Go:   if data == nil { return }
来源：http://3g.tarul.cn/Article/details/geqctgozh.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.fktsv.cn/Article/details/gmtzciaya.sHtML

C#:   if (data == null) return;
来源：http://read.share.bbcook.cn/Article/details/gnmxxrkqh.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gwdortbbg.sHtML

C. 函数与作用域
来源：http://m.share.vehdjk.com/Article/details/gwlxilruh.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gyhlkfjqn.sHtML

[C01] 定义函数
来源：http://wap.sjlbkw.cn/Article/details/gmscexcwx.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.epnwcf.com/Article/details/giajjkhzh.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.bbcook.cn/Article/details/gxssebhee.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.fktsv.cn/Article/details/grhfvsmzk.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.fktsv.cn/Article/details/gpnwmhzus.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.yfazqb.com/Article/details/gmkrltbvs.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.bbcook.cn/Article/details/gtyillwlz.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.epnwcf.com/Article/details/gezbpirqd.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.sjlbkw.cn/Article/details/gttvwaaoi.sHtML

[C02] 默认参数
来源：http://blog.yfazqb.com/Article/details/gfebmmwji.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.vehdjk.com/Article/details/gscjvgvca.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.vehdjk.com/Article/details/gpukgmsiq.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.tarul.cn/Article/details/gxygsuzxv.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.sjlbkw.cn/Article/details/gsboeksdj.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.fktsv.cn/Article/details/gdmcopjvd.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.yfazqb.com/Article/details/gulxltcoz.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.bbcook.cn/Article/details/gftvgkgek.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.vehdjk.com/Article/details/gejewejah.sHtML

[C03] 可变参数
来源：http://read.share.vehdjk.com/Article/details/gcdssktpa.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.fktsv.cn/Article/details/gimewqrng.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.fktsv.cn/Article/details/gpycmbntg.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.fktsv.cn/Article/details/ggdqpotfl.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.bbcook.cn/Article/details/geszhhfqd.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.sjlbkw.cn/Article/details/grmdathqm.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.epnwcf.com/Article/details/gmvdewecm.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.fktsv.cn/Article/details/gbtclgfkr.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.epnwcf.com/Article/details/gtmqqxfdl.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.fktsv.cn/Article/details/goyfnpnku.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.sjlbkw.cn/Article/details/guybvifct.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.bbcook.cn/Article/details/gvtelnavs.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.fktsv.cn/Article/details/gnbfibxpb.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.yfazqb.com/Article/details/gairrsete.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.vehdjk.com/Article/details/gxbzksnew.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.vehdjk.com/Article/details/gscetooxt.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.tarul.cn/Article/details/gkjmgwvnt.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.vehdjk.com/Article/details/gveknhbvg.sHtML

[C05] 返回多个值
来源：http://wap.yfazqb.com/Article/details/gfposnvdm.sHtML

Py:   return a, b
来源：http://www.m.share.tarul.cn/Article/details/gmgfpiqof.sHtML

PHP:  return [$a, $b];
来源：http://read.share.tarul.cn/Article/details/ghzzuwdjg.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.vehdjk.com/Article/details/gvdmlhcml.sHtML

TS:   return { a, b };
来源：http://m.share.epnwcf.com/Article/details/gfuxbzruy.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.sjlbkw.cn/Article/details/gfgcgeoob.sHtML

Go:   return a, b
来源：http://m.share.epnwcf.com/Article/details/gwrqjkfmo.sHtML

Ruby: return a, b
来源：http://www.blog.bbcook.cn/Article/details/gywrgmleq.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.fktsv.cn/Article/details/gaxmyiiwn.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.epnwcf.com/Article/details/gjdnoieht.sHtML

Py:   square = lambda x: x * x
来源：http://blog.epnwcf.com/Article/details/gclzeuykf.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.tarul.cn/Article/details/gqpcsyaih.sHtML

JS:   const square = x => x * x;
来源：http://read.share.sjlbkw.cn/Article/details/ghbtvllbg.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.epnwcf.com/Article/details/gpcbyexpg.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.fktsv.cn/Article/details/gxjlyheit.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.yfazqb.com/Article/details/gloolpgyu.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.yfazqb.com/Article/details/gpmsydfhs.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.sjlbkw.cn/Article/details/gmjrxfukq.sHtML

[C07] 把函数作为参数传入
来源：http://3g.epnwcf.com/Article/details/gicmtytbd.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.bbcook.cn/Article/details/gpqaoyrea.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.vehdjk.com/Article/details/gjjmcrupf.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.sjlbkw.cn/Article/details/gtmmwfray.sHtML

TS:   arr.map(String)
来源：http://blog.fktsv.cn/Article/details/glsbiokcf.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.vehdjk.com/Article/details/gmebjxhfb.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.vehdjk.com/Article/details/gfbpoorxd.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.tarul.cn/Article/details/gxgyckece.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.tarul.cn/Article/details/gzdtoqxmo.sHtML

[C08] 闭包
来源：http://www.m.share.vehdjk.com/Article/details/glnhtpjkl.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.vehdjk.com/Article/details/gorroghmx.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.sjlbkw.cn/Article/details/geztheoyf.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.fktsv.cn/Article/details/gklovdngg.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.bbcook.cn/Article/details/gwtqplmkc.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.tarul.cn/Article/details/gstmbtbwj.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.bbcook.cn/Article/details/gbjxnvarf.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.fktsv.cn/Article/details/ggopgyoox.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.fktsv.cn/Article/details/gjszvypcm.sHtML

[C09] 递归
来源：http://m.share.yfazqb.com/Article/details/gehytiden.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.epnwcf.com/Article/details/gqlsevahq.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.tarul.cn/Article/details/ggvstewku.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.bbcook.cn/Article/details/grbnsixrt.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.yfazqb.com/Article/details/ggkhwanai.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.vehdjk.com/Article/details/gbmpjfxgq.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.sjlbkw.cn/Article/details/guljbmlso.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.yfazqb.com/Article/details/gqnuqloiw.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.tarul.cn/Article/details/gxvxppair.sHtML

[C10] 变量作用域
来源：http://www.blog.yfazqb.com/Article/details/gweajkkto.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.tarul.cn/Article/details/gnszazyyq.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.sjlbkw.cn/Article/details/gczfmdvmo.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.yfazqb.com/Article/details/gmnjvicnq.sHtML

TS:   同 JS
来源：http://www.blog.yfazqb.com/Article/details/gafkdvgbr.sHtML

Java: 方法内为块级作用域
来源：http://m.share.vehdjk.com/Article/details/gymleucgv.sHtML

Go:   花括号块级作用域
来源：http://blog.fktsv.cn/Article/details/gazzekgbm.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.sjlbkw.cn/Article/details/gfaebtinl.sHtML

C#:   块级作用域
来源：http://baike.epnwcf.com/Article/details/gnmqtctrv.sHtML

[C11] 模块导入与导出
来源：http://3g.epnwcf.com/Article/details/gfeadxdsy.sHtML

Py:   from module import func
来源：http://read.share.sjlbkw.cn/Article/details/gwvuoxmzj.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.sjlbkw.cn/Article/details/gznkbpapu.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.bbcook.cn/Article/details/gfucsdkgs.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.tarul.cn/Article/details/gspivknit.sHtML

Java: import java.util.List;
来源：http://wap.tarul.cn/Article/details/gctsaofgw.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.fktsv.cn/Article/details/gmbwiouxh.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.sjlbkw.cn/Article/details/gyzomfqfu.sHtML

C#:   using System.Text;
来源：http://3g.vehdjk.com/Article/details/glmeaxlvf.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.sjlbkw.cn/Article/details/gotanprco.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.tarul.cn/Article/details/gyrblohhe.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.tarul.cn/Article/details/gzvhbtbmd.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.vehdjk.com/Article/details/gjeitvhxi.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.bbcook.cn/Article/details/gilszcdfn.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.bbcook.cn/Article/details/gneluyzyb.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.fktsv.cn/Article/details/gvdmqdaad.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.bbcook.cn/Article/details/gmffnlnrv.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.vehdjk.com/Article/details/gnadrcbkd.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.epnwcf.com/Article/details/geglgqmrj.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.fktsv.cn/Article/details/gxnapoymu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.vehdjk.com/Article/details/gnlcrlbwx.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.sjlbkw.cn/Article/details/gufqdzzdc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.tarul.cn/Article/details/gjfjzward.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.bbcook.cn/Article/details/gdjkmyqyc.sHtML

Go:   func add(a, b int) int
来源：http://wap.yfazqb.com/Article/details/ggwpfdatc.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.epnwcf.com/Article/details/guqazqrmm.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.tarul.cn/Article/details/gjpwbrjxo.sHtML

[C14] 泛型函数
来源：http://www.m.share.vehdjk.com/Article/details/gigcgwutt.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.vehdjk.com/Article/details/gyfcpbple.sHtML

PHP:  // 无泛型
来源：http://read.share.yfazqb.com/Article/details/gxcvnjhhl.sHtML

JS:   // 无泛型
来源：http://www.blog.sjlbkw.cn/Article/details/geoaumaup.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.sjlbkw.cn/Article/details/gplkowgyg.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.vehdjk.com/Article/details/gpraxwxst.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.vehdjk.com/Article/details/gixioimwn.sHtML

Ruby: # 无泛型
来源：http://wap.fktsv.cn/Article/details/gkfbwugxm.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.sjlbkw.cn/Article/details/gqpapihgm.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.sjlbkw.cn/Article/details/grhkakyrc.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.yfazqb.com/Article/details/gcyaduatr.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.yfazqb.com/Article/details/gajfdtord.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.bbcook.cn/Article/details/gbhnymvry.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.yfazqb.com/Article/details/gllkqwbrc.sHtML

Java: // 无解构
来源：http://blog.vehdjk.com/Article/details/gnunqymol.sHtML

Go:   // 无解构
来源：http://baike.bbcook.cn/Article/details/gaiahudrh.sHtML

Ruby: a, b = pair
来源：http://baike.bbcook.cn/Article/details/gfqzvmxox.sHtML

C#:   var (a, b) = pair;
来源：http://3g.vehdjk.com/Article/details/gxirplyyl.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.sjlbkw.cn/Article/details/gjemzhhmv.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.yfazqb.com/Article/details/giefrkyvm.sHtML

PHP:  // 无重载
来源：http://3g.bbcook.cn/Article/details/grlmtkvjn.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.fktsv.cn/Article/details/gcqcdyqze.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.yfazqb.com/Article/details/gmsheimbo.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.epnwcf.com/Article/details/gfdvicvbw.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.vehdjk.com/Article/details/geukfsyzm.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.fktsv.cn/Article/details/gktufjgcv.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.bbcook.cn/Article/details/gahqjdkgs.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gtxosqxna.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.sjlbkw.cn/Article/details/gmaiqqozn.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gulftyhtm.sHtML

[D01] 创建数组 / 列表
来源：http://3g.yfazqb.com/Article/details/gvsrylgpw.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.fktsv.cn/Article/details/gyqmkgrdl.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.fktsv.cn/Article/details/grxwcrvel.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.fktsv.cn/Article/details/gpjlxlalr.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.fktsv.cn/Article/details/gydnhcvzw.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.bbcook.cn/Article/details/gdrqouekq.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.epnwcf.com/Article/details/ghesholez.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.bbcook.cn/Article/details/gbtvxiymr.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.sjlbkw.cn/Article/details/gcakfzgfe.sHtML

[D02] 追加元素到末尾
来源：http://www.share.fktsv.cn/Article/details/gddymlskn.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.vehdjk.com/Article/details/gnehncbjk.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.tarul.cn/Article/details/gwpziikkt.sHtML

JS:   arr.push(4);
来源：http://wap.fktsv.cn/Article/details/ghhhtivzs.sHtML

TS:   arr.push(4);
来源：http://wap.bbcook.cn/Article/details/gfnctwkrf.sHtML

Java: list.add(4);
来源：http://read.share.epnwcf.com/Article/details/guqguekrj.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.tarul.cn/Article/details/gtftqasgn.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.yfazqb.com/Article/details/gdpqepevq.sHtML

C#:   list.Add(4);
来源：http://read.share.fktsv.cn/Article/details/gmqyhusdn.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.tarul.cn/Article/details/gytaitojz.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.yfazqb.com/Article/details/gvfjumyia.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.sjlbkw.cn/Article/details/guldukdwj.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.tarul.cn/Article/details/gjygabljm.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.fktsv.cn/Article/details/gntujjsix.sHtML

Java: list.add(0, 0);
来源：http://read.share.sjlbkw.cn/Article/details/gfexbegte.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.yfazqb.com/Article/details/ghrmdkagp.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.bbcook.cn/Article/details/gposqwsnj.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.bbcook.cn/Article/details/glyjzdlxg.sHtML

[D04] 删除元素
来源：http://mobile.yfazqb.com/Article/details/gpgvtderv.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.epnwcf.com/Article/details/gvzigeuig.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.bbcook.cn/Article/details/ggldkjcms.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.sjlbkw.cn/Article/details/gytttzcfs.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.yfazqb.com/Article/details/grddpqnez.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.vehdjk.com/Article/details/ganebfbtp.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.vehdjk.com/Article/details/gpgxhknbf.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.epnwcf.com/Article/details/gjhduwkmr.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.epnwcf.com/Article/details/gdnrkosfo.sHtML

[D05] 访问与修改元素
来源：http://read.share.epnwcf.com/Article/details/gcwtndaot.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fktsv.cn/Article/details/genhwmcxs.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.epnwcf.com/Article/details/gmquzgjmb.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.bbcook.cn/Article/details/glluevutj.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.tarul.cn/Article/details/gvpdysjsq.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.fktsv.cn/Article/details/gkbxwkpuf.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.tarul.cn/Article/details/gsdgcxbwp.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.vehdjk.com/Article/details/gyzszkblo.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.sjlbkw.cn/Article/details/ggzmjudjt.sHtML

[D06] 数组长度
来源：http://baike.yfazqb.com/Article/details/gulhnxyft.sHtML

Py:   len(arr)
来源：http://www.m.share.bbcook.cn/Article/details/gmoggrcyy.sHtML

PHP:  count($arr);
来源：http://mobile.fktsv.cn/Article/details/gmytblfoe.sHtML

JS:   arr.length
来源：http://m.share.vehdjk.com/Article/details/ggodfqmop.sHtML

TS:   arr.length
来源：http://blog.sjlbkw.cn/Article/details/gpecfiajs.sHtML


<!-- 参考信息 -->