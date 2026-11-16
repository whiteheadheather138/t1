代发 wailian999

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hre.ppjwa.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://gsn.xziqi.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mfb.yonumen.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://fjy.zhoulong.xyz

C#:   var r = x > 0 ? "正" : "非正";
来源：http://xuj.yuxming.cn

[B02] 多分支 else if / elif
来源：http://xns.yvedp.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://jmf.sysykeji.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ayd.zdbjq.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://afv.hongshengwenyu.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://edq.cdnleiting.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://erq.xinyue.icu

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://lff.xuanzx.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://zuw.cashguo.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://aza.jinqigfzy.top

[B03] switch / match / case
来源：http://kcr.andypj.xyz

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://bqy.hfpthk.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://efz.ctjpmb.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qhl.yongpay.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bdy.yj20258888.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://jqs.wangdashe.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://vev.sxryk.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ejz.chenjidiqi.icu

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://qkf.jqgfzy.top

[B04] for 计数循环
来源：http://zaw.yuanzhike.top

Py:   for i in range(10): print(i)
来源：http://bsn.jyoumei.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://fcj.tanke756.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sir.pycfn.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jbc.yfazqb.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mvc.zycfv.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://nre.fehbvm.com

Ruby: 10.times { |i| puts i }
来源：http://nqh.daxiang520.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://gtr.fzhhl.top

[B05] 遍历数组 / 列表
来源：http://rdc.cqqwz.cn

Py:   for item in arr: print(item)
来源：http://gte.bbcook.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://rbc.havefunace.top

JS:   for (const item of arr) { console.log(item); }
来源：http://pjc.ybcxt.top

TS:   for (const item of arr) { console.log(item); }
来源：http://ycx.hesvh.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://vsr.quarkkingdee.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://vco.sysykeji.top

Ruby: arr.each { |item| puts item }
来源：http://pwf.jqgufenzy.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://epl.tian-w.cn

[B06] 遍历字典 / 对象
来源：http://jcn.iojbl.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://vpl.hywenlv.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://kzx.guowangkeji.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ctu.xingfuxueyuan.xyz

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://trf.xylfe.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://nir.bjfxy.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://kvw.gzhubu.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mug.fengsongda.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://qai.0kj1m.cn

[B07] while 循环
来源：http://xyp.ydjk.org.cn

Py:   while i < 10: i += 1
来源：http://gqb.yvedp.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ijl.vehdjk.com

JS:   while (i < 10) { i++; }
来源：http://dua.52xcode.cn

TS:   while (i < 10) { i++; }
来源：http://izw.kuanghao11.cn

Java: while (i < 10) { i++; }
来源：http://lsd.hysaishi.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://dbx.jinghuilouyu.cn

Ruby: while i < 10; i += 1; end
来源：http://sts.meibo888.top

C#:   while (i < 10) { i++; }
来源：http://wdb.yj20258888.top

[B08] do-while（至少执行一次）
来源：http://jnr.jinyuanbaomall.cn

Py:   # 无 do-while：用 while True + break
来源：http://alb.cdnleiting.top

PHP:  do { $i++; } while ($i < 10);
来源：http://zkj.jinqigufen.top

JS:   do { i++; } while (i < 10);
来源：http://pfc.ehwqpu.com

TS:   do { i++; } while (i < 10);
来源：http://lit.daxiang520.top

Java: do { i++; } while (i < 10);
来源：http://eut.hnxiangtu.top

Go:   for { i++; if i >= 10 { break } }
来源：http://aoo.gzhubu.top

Ruby: begin; i += 1; end while i < 10
来源：http://qfw.bjfxy.top

C#:   do { i++; } while (i < 10);
来源：http://syo.birdmap.top

[B09] break 与 continue
来源：http://vxf.epnwcf.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://esn.tianlin.xyz

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://gdl.tarul.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vvm.bjfxy.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lkg.sweek.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kpg.birdmap.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://xmo.jlsjyb.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xry.tarul.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tjg.bbcook.cn

[B10] 遍历同时拿索引
来源：http://rxd.316326.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hkn.jlsjyb.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://jwj.fanxiaobao.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://dwd.zhongyouzk.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://koe.316326.xyz

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wsb.yangfankeji.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://tev.hywenlv.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://snc.chenzaomai.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://bee.xinyue.icu

[B11] 生成数字序列 / 区间
来源：http://qow.ctjpmb.com

Py:   list(range(0, 10, 2))
来源：http://ikp.zycfv.cn

PHP:  range(0, 10, 2);
来源：http://nvu.xuanzx.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://oiz.yonumen.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xzd.zhixingplan.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://nla.daxiang520.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wxl.gaohongyu789.top

Ruby: (0...10).step(2).to_a
来源：http://qao.epnwcf.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://jbx.shzxlz.cn

[B12] 跳出多层循环
来源：http://riv.uphjek.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://hbi.svipenyu.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://wec.smart0.xyz

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://jbv.zhengqikj.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://won.yangfankeji.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://yuj.hongshengwenyu.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://uez.fehbvm.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ptl.gaohongyu789.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://vkq.zhoulong.xyz

[B13] 判断是否为数字
来源：http://oic.zhixingplan.top

Py:   isinstance(x, (int, float))
来源：http://quc.xingfuxueyuan.xyz

PHP:  is_numeric($x)
来源：http://xot.0kj1m.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wwf.nanxuanxn.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yek.dashuyun.cn

Java: x instanceof Number
来源：http://yra.snrcjt.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mzi.pycfn.com

Ruby: x.is_a?(Numeric)
来源：http://oby.ydzc1.top

C#:   x is int or double or decimal
来源：http://ffl.snrcjt.cn

[B14] 判断值是否在集合内
来源：http://ygq.nwbrower.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://uiz.svipenyu.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wjx.nanxinkj.top

JS:   [1, 2, 3].includes(x)
来源：http://dcb.havefunace.top

TS:   [1, 2, 3].includes(x)
来源：http://vws.birdmap.top

Java: List.of(1, 2, 3).contains(x)
来源：http://olo.jiagoushi.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://qzg.yvedp.cn

Ruby: [1, 2, 3].include?(x)
来源：http://jcx.52xcode.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://usx.bjfxy.top

[B15] 布尔运算与取反
来源：http://mgq.yuxming.cn

Py:   a and b or not c
来源：http://pry.fehbvm.com

PHP:  $a && $b || !$c
来源：http://vnb.cdnleiting.top

JS:   a && b || !c
来源：http://hgf.ywan-chungtsiang.top

TS:   a && b || !c
来源：http://uqw.xingfuxueyuan.xyz

Java: a && b || !c
来源：http://dhu.nanxinkj.top

Go:   a && b || !c
来源：http://ltj.yangfankeji.com

Ruby: a && b || !c
来源：http://mgh.hnxiangtu.top

C#:   a && b || !c
来源：http://ody.ppjwa.cn

[B16] 卫语句：不满足条件提前返回
来源：http://dhb.gzhubu.top

Py:   if not data: return
来源：http://olw.fanxiaobao.xyz

PHP:  if (!$data) { return; }
来源：http://vnd.wangshuangyany.cn

JS:   if (!data) return;
来源：http://ijp.yongpay.top

TS:   if (!data) return;
来源：http://xwv.smart0.xyz

Java: if (data == null) return;
来源：http://qog.zhoulong.xyz

Go:   if data == nil { return }
来源：http://ipy.havefunace.top

Ruby: return if data.nil?
来源：http://qda.cdnleiting.top

C#:   if (data == null) return;
来源：http://stv.ehwqpu.com

================================================================================
来源：http://iro.guannengcc.top

C. 函数与作用域
来源：http://too.tarul.cn

================================================================================
来源：http://ukp.jyoumei.cn

[C01] 定义函数
来源：http://ffp.aizwys.cn

Py:   def add(a, b): return a + b
来源：http://neu.yj20258888.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yzq.bjfxy.top

JS:   function add(a, b) { return a + b; }
来源：http://ymy.yanxiufei.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qrg.tianlin.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://jze.jinqigufen.top

Go:   func add(a, b int) int { return a + b }
来源：http://fmw.snrcjt.cn

Ruby: def add(a, b); a + b; end
来源：http://ldc.yuxming.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://khv.birdmap.top

[C02] 默认参数
来源：http://vbz.bjfxy.top

Py:   def greet(name="World"): return name
来源：http://lqj.9152youxi.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://cax.jqgufenzy.top

JS:   function greet(name = "World") { return name; }
来源：http://zur.sxryk.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ehi.jqgufenzy.top

Java: // 无默认参数：方法重载或 Optional
来源：http://bxa.zhengqikj.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://jxm.zycfv.cn

Ruby: def greet(name = "World") = name
来源：http://nco.shanyushiyangkeji.top

C#:   string Greet(string name = "World") => name;
来源：http://lop.yongpay.top

[C03] 可变参数
来源：http://ifl.pengpengdd.cyou

Py:   def total(*args): return sum(args)
来源：http://nub.tanke756.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://oyg.shanyushiyangtech.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ror.cheryme.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://uxr.aizwys.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vpo.fengsongda.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://kmg.gaohongyu789.top

Ruby: def total(*nums); nums.sum; end
来源：http://wcp.hnqzz.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ixg.nanxinkj.top

[C04] 命名参数 / 关键字参数
来源：http://ysr.xinyue.icu

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://heb.nanxinkj.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://opa.yueranfly.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://vfw.uphjek.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://fbn.sjlbkw.cn

Java: // 无：用 Builder 模式或 record
来源：http://upu.pycfn.com

Go:   // 无：用配置结构体参数
来源：http://fct.jinqigufen.top

Ruby: f(a: 1, b: 2)
来源：http://ycc.chenzaomai.com

C#:   f(a: 1, b: 2)
来源：http://gxr.hfpthk.cn

[C05] 返回多个值
来源：http://omo.jinqigfzy.top

Py:   return a, b
来源：http://uqf.chenlongwang.top

PHP:  return [$a, $b];
来源：http://xqx.ydzc1.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://agr.zhoulong.xyz

TS:   return { a, b };
来源：http://ipy.hnqzz.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://tqh.tarul.cn

Go:   return a, b
来源：http://kqo.aizwys.cn

Ruby: return a, b
来源：http://cgw.zhongyouzk.top

C#:   return (a, b);              // ValueTuple
来源：http://qbl.meibo888.top

[C06] 匿名函数 / lambda
来源：http://iva.c1oappe.top

Py:   square = lambda x: x * x
来源：http://dqg.vqdsnc.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://xox.havefunace.top

JS:   const square = x => x * x;
来源：http://aig.hcnkem.com

TS:   const square = (x: number): number => x * x;
来源：http://qhh.shangyingyoupin.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://atn.pycfn.com

Go:   sq := func(x int) int { return x * x }
来源：http://gbz.daxiang520.top

Ruby: square = ->(x) { x * x }
来源：http://aho.sysykeji.top

C#:   Func<int, int> square = x => x * x;
来源：http://upm.jqgufenzy.top

[C07] 把函数作为参数传入
来源：http://org.jlsjyb.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://sbr.316326.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://ugc.yangfankeji.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://zoc.fengsongda.top

TS:   arr.map(String)
来源：http://pwv.yj20258888.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mfd.yangfankeji.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://yjq.ybcxt.top

Ruby: arr.map(&:upcase)
来源：http://mbp.zhijiandao.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://wqi.ctjpmb.com

[C08] 闭包
来源：http://rvr.chenlongwang.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://kxl.gogol.net.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://izo.xziqi.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://cgu.jqgfzy.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://uvl.gogol.net.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://jcn.tianlin.xyz

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://xpi.hnxiangtu.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://lsy.wangdashe.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ssk.tanke756.top

[C09] 递归
来源：http://zds.tarul.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://uco.yuxming.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://xzn.jinghuilouyu.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jpj.jinyuanbaomall.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xkq.ydjk.org.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ziy.tarul.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://uhk.0kj1m.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://jsh.daria6918.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://tlo.cdnleiting.top

[C10] 变量作用域
来源：http://wra.yuanzhike.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://bdw.yangfankeji.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://rcd.zycfv.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://uko.fktsv.cn

TS:   同 JS
来源：http://xuz.andypj.xyz

Java: 方法内为块级作用域
来源：http://lhv.cdnleiting.top

Go:   花括号块级作用域
来源：http://whb.daria6918.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://qhq.andypj.xyz

C#:   块级作用域
来源：http://xos.jqgufenzy.top

[C11] 模块导入与导出
来源：http://syw.hfpthk.cn

Py:   from module import func
来源：http://byx.jinghuilouyu.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://xyn.sysykeji.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://wuf.fanxiaobao.xyz

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mpo.daria6918.cn

Java: import java.util.List;
来源：http://icw.nwbrower.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://zfl.ywan-chungtsiang.top

Ruby: require "json"; require_relative "./util"
来源：http://ilu.bbcook.cn

C#:   using System.Text;
来源：http://fbi.fktsv.cn

[C12] 立即执行函数 IIFE
来源：http://yax.hammf.cn

Py:   (lambda: print("run"))()
来源：http://cti.iojbl.cn

PHP:  (function () { echo "run"; })();
来源：http://dkl.bbcook.cn

JS:   (() => { console.log("run"); })();
来源：http://rin.shanyushiyangkeji.top

TS:   (() => { console.log("run"); })();
来源：http://tfg.zhixingplan.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jsb.cqqwz.cn

Go:   func() { fmt.Println("run") }()
来源：http://ucf.ydzc1.top

Ruby: -> { puts "run" }.call
来源：http://hxe.hnxiangtu.top

C#:   // 无 IIFE：用静态构造函数
来源：http://lfn.hcnkem.com

[C13] 类型声明 / 类型注解
来源：http://hev.nanxuanxn.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mtc.sjlbkw.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hoa.ehwqpu.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://fhl.fehbvm.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ymd.bbcook.cn

Java: int add(int a, int b) { return a + b; }
来源：http://siq.jyoumei.cn

Go:   func add(a, b int) int
来源：http://bpc.hongshengwenyu.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://sbs.yfazqb.com

C#:   int Add(int a, int b) => a + b;
来源：http://gvm.quarkkingdee.top

[C14] 泛型函数
来源：http://zez.zhaomingkeji.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://taz.hesvh.cn

PHP:  // 无泛型
来源：http://khd.ehwqpu.com

JS:   // 无泛型
来源：http://ecf.sufxvd.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://zso.pycfn.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://umq.redwolf501.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://lrk.c1oappe.top

Ruby: # 无泛型
来源：http://mqz.jlsjyb.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://nun.fanxiaobao.xyz

[C15] 解构 / 展开参数
来源：http://zdy.chenzaomai.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://iwz.nanxuanxn.top

PHP:  [$a, $b] = $pair;
来源：http://fkh.zdqjudy.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wqk.yuanzhike.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://jrg.cucudq.cn

Java: // 无解构
来源：http://ctc.316326.xyz

Go:   // 无解构
来源：http://pwm.dianchejie.cn

Ruby: a, b = pair
来源：http://wow.guannengcc.top

C#:   var (a, b) = pair;
来源：http://azm.hywenlv.cn

[C16] 函数 / 方法重载
来源：http://lqe.feifeiyinyue.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ltm.jinqigufen.top

PHP:  // 无重载
来源：http://cfv.gotoacloud.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://fuo.quarkkingdee.top

TS:   // 用联合类型或重载签名声明
来源：http://wde.hnxiangtu.top

Java: void f(int a) {}  void f(String a) {}
来源：http://rpb.xziqi.cn

Go:   // 无重载：用不同函数名
来源：http://rky.zhijiandao.cn

Ruby: # 无重载：靠动态参数
来源：http://ptd.sjlbkw.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://twa.jyoumei.cn

================================================================================
来源：http://hts.jqgfzy.top

D. 数组 / 列表 / 集合
来源：http://mul.gogol.net.cn

================================================================================
来源：http://hes.hammf.cn

[D01] 创建数组 / 列表
来源：http://gdv.xuetiantiany.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://smx.cdnleiting.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://nxa.hammf.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://fwa.hesvh.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://gjl.zdbjq.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://koq.ppjwa.cn

Go:   arr := []int{1, 2, 3}
来源：http://znz.316326.xyz

Ruby: arr = [1, 2, 3]
来源：http://ypf.aizwys.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://oag.svipenyu.cn

[D02] 追加元素到末尾
来源：http://aof.mhx1999.top


<!-- 参考信息 -->