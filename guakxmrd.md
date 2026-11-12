代发 wailian999

TS:   const r = x > 0 ? "正" : "非正";
来源：http://coe.shanyushiyangtech.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://dzb.andypj.xyz

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://qcp.chenjidiqi.icu

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hnz.hcnkem.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://vba.wangdashe.top

[B02] 多分支 else if / elif
来源：http://nvr.chenzaomai.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://fbr.iojbl.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://rvd.fzhhl.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ilo.zhoulong.xyz

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://taq.svipenyu.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wcb.shanyushiyangkeji.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://eyv.ehwqpu.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://cpo.zdbjq.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://utx.vqdsnc.cn

[B03] switch / match / case
来源：http://tes.haohaochexian.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://jve.bbcook.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://gck.hesvh.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://sov.chenlongwang.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yvp.zhixingplan.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://qhg.tian-w.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://pqo.c1oappe.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://qjc.fehbvm.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://pje.vqdsnc.cn

[B04] for 计数循环
来源：http://utv.ywan-chungtsiang.top

Py:   for i in range(10): print(i)
来源：http://zfu.zhengqikj.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://rmf.daxiang520.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jmm.yangfankeji.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://scg.tian-w.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://and.haohaochexian.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://tia.jianghu66.top

Ruby: 10.times { |i| puts i }
来源：http://blq.shanyushiyangtech.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://eop.redwolf501.top

[B05] 遍历数组 / 列表
来源：http://zvw.feifeiyinyue.top

Py:   for item in arr: print(item)
来源：http://qbk.wangshuangyany.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://qxl.wangshuangyany.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://dwi.xziqi.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://xvz.pengpengdd.cyou

Java: for (var item : arr) { System.out.println(item); }
来源：http://vyg.yuxming.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://tqb.fktsv.cn

Ruby: arr.each { |item| puts item }
来源：http://ppg.hnqzz.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://vmu.hnqzz.top

[B06] 遍历字典 / 对象
来源：http://kjg.smart0.xyz

Py:   for k, v in d.items(): print(k, v)
来源：http://lmj.gotoacloud.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://uxk.yueranfly.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://brp.hfpthk.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rfi.jinyuanbaomall.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://sdx.wangshuangyany.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://upg.cheryme.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://lex.hongshengwenyu.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://jmn.jyoumei.cn

[B07] while 循环
来源：http://nud.guannengcc.top

Py:   while i < 10: i += 1
来源：http://avv.chenlongwang.top

PHP:  while ($i < 10) { $i++; }
来源：http://sbg.0kj1m.cn

JS:   while (i < 10) { i++; }
来源：http://rqn.kuanghao11.cn

TS:   while (i < 10) { i++; }
来源：http://mju.gotoacloud.top

Java: while (i < 10) { i++; }
来源：http://ilz.yj20258888.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://gel.daxiang520.top

Ruby: while i < 10; i += 1; end
来源：http://fek.bjfxy.top

C#:   while (i < 10) { i++; }
来源：http://jwr.zhoulong.xyz

[B08] do-while（至少执行一次）
来源：http://hvm.sjlbkw.cn

Py:   # 无 do-while：用 while True + break
来源：http://azj.nwbrower.top

PHP:  do { $i++; } while ($i < 10);
来源：http://nme.wangshuangyany.cn

JS:   do { i++; } while (i < 10);
来源：http://vca.cucudq.cn

TS:   do { i++; } while (i < 10);
来源：http://jfr.316326.xyz

Java: do { i++; } while (i < 10);
来源：http://ddw.sxryk.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://osz.guannengcc.top

Ruby: begin; i += 1; end while i < 10
来源：http://nre.dashuyun.cn

C#:   do { i++; } while (i < 10);
来源：http://sqi.zhijiandao.cn

[B09] break 与 continue
来源：http://yyc.shanyushiyangtech.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://jdv.jqgufenzy.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://eje.xziqi.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wxq.sufxvd.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://obe.chenzaomai.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wpp.uphjek.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://pyn.ybcxt.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://pep.yuxming.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uhi.hysaishi.cn

[B10] 遍历同时拿索引
来源：http://iag.daxiang520.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ujb.shuidangran.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://zrh.zdqjudy.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://fhy.svipenyu.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://lqd.52xcode.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://gmw.zhijiandao.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://lyb.yj20258888.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://iri.dianchejie.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://qqd.dianchejie.cn

[B11] 生成数字序列 / 区间
来源：http://hya.mhx1999.top

Py:   list(range(0, 10, 2))
来源：http://dzl.shanyushiyangtech.top

PHP:  range(0, 10, 2);
来源：http://mid.sjlbkw.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rke.zhongyouzk.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kdi.hnqzz.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://lck.redwolf501.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://nss.fehbvm.com

Ruby: (0...10).step(2).to_a
来源：http://jeb.ybcxt.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ocs.feifeiyinyue.top

[B12] 跳出多层循环
来源：http://jkl.shuidangran.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://tdy.cucudq.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://vnp.yfazqb.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://lrx.chenlongwang.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://rbp.zhongyouzk.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hsr.cqqwz.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blm.meibo888.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://yuq.52xcode.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://vsk.jinqigfzy.top

[B13] 判断是否为数字
来源：http://mcf.zdqjudy.top

Py:   isinstance(x, (int, float))
来源：http://eed.tarul.cn

PHP:  is_numeric($x)
来源：http://qiw.ydjk.org.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qoc.aibaodan.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sth.jlsjyb.cn

Java: x instanceof Number
来源：http://lcs.yueranfly.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://bxx.sysykeji.top

Ruby: x.is_a?(Numeric)
来源：http://dbi.52xcode.cn

C#:   x is int or double or decimal
来源：http://dhl.meibo888.top

[B14] 判断值是否在集合内
来源：http://kps.0kj1m.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://rqc.aizwys.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://oyj.meibo888.top

JS:   [1, 2, 3].includes(x)
来源：http://apu.dashuyun.cn

TS:   [1, 2, 3].includes(x)
来源：http://usp.zhoulong.xyz

Java: List.of(1, 2, 3).contains(x)
来源：http://rxa.jinyuanbaomall.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://eyi.xuetiantiany.cn

Ruby: [1, 2, 3].include?(x)
来源：http://vji.zhoulong.xyz

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://cor.zhoulong.xyz

[B15] 布尔运算与取反
来源：http://qhe.ybcxt.top

Py:   a and b or not c
来源：http://tzb.cqqwz.cn

PHP:  $a && $b || !$c
来源：http://udj.fengsongda.top

JS:   a && b || !c
来源：http://lyc.mhx1999.top

TS:   a && b || !c
来源：http://uli.zhoulong.xyz

Java: a && b || !c
来源：http://ndx.ivvv.top

Go:   a && b || !c
来源：http://dmh.xuanzx.com

Ruby: a && b || !c
来源：http://tfb.sjlbkw.cn

C#:   a && b || !c
来源：http://utt.uphjek.com

[B16] 卫语句：不满足条件提前返回
来源：http://ylo.zhixingplan.top

Py:   if not data: return
来源：http://srh.cqqwz.cn

PHP:  if (!$data) { return; }
来源：http://ipy.shanyushiyangtech.top

JS:   if (!data) return;
来源：http://jia.xylfe.cn

TS:   if (!data) return;
来源：http://yee.sweek.top

Java: if (data == null) return;
来源：http://ljb.cheryme.top

Go:   if data == nil { return }
来源：http://sac.zhongyouzk.top

Ruby: return if data.nil?
来源：http://ppd.feifeiyinyue.top

C#:   if (data == null) return;
来源：http://bcq.ydzc1.top

================================================================================
来源：http://nbl.nanxinkj.top

C. 函数与作用域
来源：http://odg.9152youxi.cn

================================================================================
来源：http://ssb.shuidangran.top

[C01] 定义函数
来源：http://wvk.birdmap.top

Py:   def add(a, b): return a + b
来源：http://fmw.c1oappe.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vpe.andypj.xyz

JS:   function add(a, b) { return a + b; }
来源：http://cev.xylfe.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qzd.zhixingplan.top

Java: static int add(int a, int b) { return a + b; }
来源：http://dtx.guowangkeji.top

Go:   func add(a, b int) int { return a + b }
来源：http://snx.yanxiufei.cn

Ruby: def add(a, b); a + b; end
来源：http://owz.dianchejie.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://aju.sysykeji.top

[C02] 默认参数
来源：http://scl.vehdjk.com

Py:   def greet(name="World"): return name
来源：http://grb.yonumen.top

PHP:  function greet($name = "World") { return $name; }
来源：http://jhe.shuidangran.top

JS:   function greet(name = "World") { return name; }
来源：http://gxw.0kj1m.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ypa.fanxiaobao.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://pta.smart0.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ltn.fanxiaobao.xyz

Ruby: def greet(name = "World") = name
来源：http://ndw.aibaodan.cn

C#:   string Greet(string name = "World") => name;
来源：http://rie.zdbjq.cn

[C03] 可变参数
来源：http://pbh.jinqigfzy.top

Py:   def total(*args): return sum(args)
来源：http://uww.zhongyouzk.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ejn.nwbrower.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://pov.sxryk.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ank.havefunace.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vhz.zhaomingkeji.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://rpe.ivvv.top

Ruby: def total(*nums); nums.sum; end
来源：http://drj.kuanghao11.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://uid.fktsv.cn

[C04] 命名参数 / 关键字参数
来源：http://nng.yvedp.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://gsp.meibo888.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://tjx.jqgufenzy.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://cyb.tian-w.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://gey.havefunace.top

Java: // 无：用 Builder 模式或 record
来源：http://wvt.redwolf501.top

Go:   // 无：用配置结构体参数
来源：http://loc.shzxlz.cn

Ruby: f(a: 1, b: 2)
来源：http://tye.guannengcc.top

C#:   f(a: 1, b: 2)
来源：http://jda.shangyingyoupin.top

[C05] 返回多个值
来源：http://xgq.jinqigufen.top

Py:   return a, b
来源：http://wiv.xylfe.cn

PHP:  return [$a, $b];
来源：http://end.xylfe.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://bmp.xingfuxueyuan.xyz

TS:   return { a, b };
来源：http://wyg.shanyushiyangkeji.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://fui.c1oappe.top

Go:   return a, b
来源：http://bvi.tarul.cn

Ruby: return a, b
来源：http://exk.wangshuangyany.cn

C#:   return (a, b);              // ValueTuple
来源：http://xym.smart0.xyz

[C06] 匿名函数 / lambda
来源：http://dfh.fktsv.cn

Py:   square = lambda x: x * x
来源：http://ckb.yonumen.top

PHP:  $square = fn($x) => $x * $x;
来源：http://jqk.yonumen.top

JS:   const square = x => x * x;
来源：http://ztz.smart0.xyz

TS:   const square = (x: number): number => x * x;
来源：http://nfd.cqqwz.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://lmc.xinyue.icu

Go:   sq := func(x int) int { return x * x }
来源：http://yez.epnwcf.com

Ruby: square = ->(x) { x * x }
来源：http://svx.tianlin.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://soa.smart0.xyz

[C07] 把函数作为参数传入
来源：http://qeu.dashuyun.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://czr.feifeiyinyue.top

PHP:  array_map("strtoupper", $arr);
来源：http://fbl.birdmap.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://bfn.hesvh.cn

TS:   arr.map(String)
来源：http://kyc.havefunace.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://trz.daxiang520.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://czs.hysaishi.cn

Ruby: arr.map(&:upcase)
来源：http://zsy.meibo888.top

C#:   arr.Select(s => s.ToUpper())
来源：http://cnt.gotoacloud.top

[C08] 闭包
来源：http://jab.jinqigufen.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hbi.jqgfzy.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://spk.cheryme.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://jki.zhoulong.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://frj.ydzc1.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://kbm.jinyuanbaomall.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://yuf.gaohongyu789.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ubj.zhijiandao.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://muz.pengpengdd.cyou

[C09] 递归
来源：http://eit.zhoulong.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hvr.xuanzx.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ikx.jlsjyb.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gpg.fktsv.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://svs.hammf.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wgm.hesvh.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://gvh.316326.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wje.xinyue.icu

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://dtk.jinghuilouyu.cn

[C10] 变量作用域
来源：http://eda.hysaishi.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ucx.yonumen.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://dmx.ydjk.org.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hwr.feifeiyinyue.top

TS:   同 JS
来源：http://qmp.gotoacloud.top

Java: 方法内为块级作用域
来源：http://vzp.yueranfly.top

Go:   花括号块级作用域
来源：http://esb.ywan-chungtsiang.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://gkm.shanyushiyangkeji.top

C#:   块级作用域
来源：http://ybt.daxiang520.top

[C11] 模块导入与导出
来源：http://oka.xingfuxueyuan.xyz

Py:   from module import func
来源：http://ple.shuidangran.top

PHP:  require "file.php";  或 use App\Service;
来源：http://pwu.bjfxy.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://ldx.jianghu66.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xcw.ydjk.org.cn

Java: import java.util.List;
来源：http://qgk.shzxlz.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://rse.gotoacloud.top

Ruby: require "json"; require_relative "./util"
来源：http://lnd.jiagoushi.top

C#:   using System.Text;
来源：http://rwp.hesvh.cn

[C12] 立即执行函数 IIFE
来源：http://dyx.aizwys.cn

Py:   (lambda: print("run"))()
来源：http://jqs.fktsv.cn

PHP:  (function () { echo "run"; })();
来源：http://itl.svipenyu.cn

JS:   (() => { console.log("run"); })();
来源：http://kxf.hcnkem.com

TS:   (() => { console.log("run"); })();
来源：http://fny.smart0.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://cty.0kj1m.cn

Go:   func() { fmt.Println("run") }()
来源：http://vhc.yuxming.cn

Ruby: -> { puts "run" }.call
来源：http://jpn.yuanzhike.top

C#:   // 无 IIFE：用静态构造函数
来源：http://uin.jqgfzy.top

[C13] 类型声明 / 类型注解
来源：http://pmj.gaohongyu789.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://chj.vqdsnc.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://syp.shangyingyoupin.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://qpf.chenlongwang.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vig.feifeiyinyue.top

Java: int add(int a, int b) { return a + b; }
来源：http://hdc.xuetiantiany.cn

Go:   func add(a, b int) int
来源：http://yia.tian-w.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://lrr.ydjk.org.cn

C#:   int Add(int a, int b) => a + b;
来源：http://fec.iojbl.cn

[C14] 泛型函数
来源：http://atd.xziqi.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://pcq.jinghuilouyu.cn

PHP:  // 无泛型
来源：http://qct.uphjek.com

JS:   // 无泛型
来源：http://xjs.jqgufenzy.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ckc.jyoumei.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wup.cqqwz.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ffi.vqdsnc.cn

Ruby: # 无泛型
来源：http://frx.9152youxi.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://oyh.jinqigfzy.top

[C15] 解构 / 展开参数
来源：http://rrv.mhx1999.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://vkd.fktsv.cn

PHP:  [$a, $b] = $pair;
来源：http://xzr.tianlin.xyz

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ixa.sweek.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://vjb.sjlbkw.cn

Java: // 无解构
来源：http://krt.cdnleiting.top

Go:   // 无解构
来源：http://ymu.zhengqikj.top

Ruby: a, b = pair
来源：http://tkd.yfazqb.com

C#:   var (a, b) = pair;
来源：http://ffn.fehbvm.com

[C16] 函数 / 方法重载
来源：http://wtf.yongpay.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://yyr.fengsongda.top

PHP:  // 无重载
来源：http://fso.yj20258.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://drv.fanxiaobao.xyz

TS:   // 用联合类型或重载签名声明
来源：http://yzv.pycfn.com

Java: void f(int a) {}  void f(String a) {}
来源：http://ziq.kuanghao11.cn

Go:   // 无重载：用不同函数名
来源：http://cif.ctjpmb.com

Ruby: # 无重载：靠动态参数
来源：http://niv.zhoulong.xyz

C#:   void F(int a) {}  void F(string a) {}
来源：http://mht.zdbjq.cn

================================================================================
来源：http://fmp.xziqi.cn

D. 数组 / 列表 / 集合
来源：http://wsw.pengpengdd.cyou

================================================================================
来源：http://thr.jinqigfzy.top

[D01] 创建数组 / 列表
来源：http://dmh.zhijiandao.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://poo.chenzaomai.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://jyw.c1oappe.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://muu.jiagoushi.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://ebh.smart0.xyz

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://olm.ppjwa.cn

Go:   arr := []int{1, 2, 3}
来源：http://htb.gzhubu.top

Ruby: arr = [1, 2, 3]
来源：http://lun.hongshengwenyu.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ftk.xylfe.cn

[D02] 追加元素到末尾
来源：http://hgy.wangdashe.top


<!-- 参考信息 -->