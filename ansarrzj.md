代发 wailian999

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ryb.hammf.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://anm.gogol.net.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ygp.hammf.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://brl.0kj1m.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://emx.cashguo.top

[B02] 多分支 else if / elif
来源：http://iae.xinyue.icu

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://iyw.shanyushiyangkeji.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://uqs.zdqjudy.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ymz.hnqzz.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://grx.yanxiufei.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cwy.andypj.xyz

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wkg.tanke756.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://nqb.mhx1999.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://paz.tanke756.top

[B03] switch / match / case
来源：http://yei.fzhhl.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wlj.gogol.net.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ydk.yfazqb.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jmg.hnqzz.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nle.yangfankeji.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://rfl.svipenyu.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://pmy.tanke756.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://lid.redwolf501.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://gjb.jinqigfzy.top

[B04] for 计数循环
来源：http://num.hammf.cn

Py:   for i in range(10): print(i)
来源：http://nlv.zhengqikj.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wzg.vehdjk.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://uqo.yj202588.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rlx.yueranfly.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://jfm.ehwqpu.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://urw.zycfv.cn

Ruby: 10.times { |i| puts i }
来源：http://frq.yongpay.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://oym.aizwys.cn

[B05] 遍历数组 / 列表
来源：http://pne.hysaishi.cn

Py:   for item in arr: print(item)
来源：http://kby.aizwys.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ocw.pengpengdd.cyou

JS:   for (const item of arr) { console.log(item); }
来源：http://vwr.nanxinkj.top

TS:   for (const item of arr) { console.log(item); }
来源：http://sex.yueranfly.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://wpy.jianghu66.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://sfu.xingfuxueyuan.xyz

Ruby: arr.each { |item| puts item }
来源：http://eqq.aizwys.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://acm.yangfankeji.com

[B06] 遍历字典 / 对象
来源：http://tnj.ctjpmb.com

Py:   for k, v in d.items(): print(k, v)
来源：http://gda.guowangkeji.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://zyi.fengsongda.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xad.jlsjyb.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tqk.sjlbkw.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://pqj.pengpengdd.cyou

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://lut.xinyue.icu

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://pkx.ywan-chungtsiang.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mgg.c1oappe.top

[B07] while 循环
来源：http://ncf.zycfv.cn

Py:   while i < 10: i += 1
来源：http://flt.hnqzz.top

PHP:  while ($i < 10) { $i++; }
来源：http://ghn.snrcjt.cn

JS:   while (i < 10) { i++; }
来源：http://dxt.fengsongda.top

TS:   while (i < 10) { i++; }
来源：http://asv.nwbrower.top

Java: while (i < 10) { i++; }
来源：http://ydm.cdnleiting.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://eau.xziqi.cn

Ruby: while i < 10; i += 1; end
来源：http://hpd.yuxming.cn

C#:   while (i < 10) { i++; }
来源：http://xxa.jinyuanbaomall.cn

[B08] do-while（至少执行一次）
来源：http://nex.fanxiaobao.xyz

Py:   # 无 do-while：用 while True + break
来源：http://vbc.redwolf501.top

PHP:  do { $i++; } while ($i < 10);
来源：http://mtm.aizwys.cn

JS:   do { i++; } while (i < 10);
来源：http://vua.andypj.xyz

TS:   do { i++; } while (i < 10);
来源：http://kvb.jqgufenzy.top

Java: do { i++; } while (i < 10);
来源：http://noo.jqgfzy.top

Go:   for { i++; if i >= 10 { break } }
来源：http://aig.gzhubu.top

Ruby: begin; i += 1; end while i < 10
来源：http://axf.shzxlz.cn

C#:   do { i++; } while (i < 10);
来源：http://jna.meibo888.top

[B09] break 与 continue
来源：http://arl.hysaishi.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wur.yongpay.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://pfu.cucudq.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xpt.ydjk.org.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tle.jinqigfzy.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mnf.cashguo.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://bbc.jlsjyb.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://swl.hammf.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cnl.hfpthk.cn

[B10] 遍历同时拿索引
来源：http://mcd.jqgufenzy.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hew.chenjidiqi.icu

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://vzr.dashuyun.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://yly.dianchejie.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ftx.fktsv.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://aer.cucudq.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://zkh.dashuyun.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ivr.zhaomingkeji.xyz

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wrk.jianghu66.top

[B11] 生成数字序列 / 区间
来源：http://gaa.bjfxy.top

Py:   list(range(0, 10, 2))
来源：http://qix.fanxiaobao.xyz

PHP:  range(0, 10, 2);
来源：http://qww.yj202588.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bdh.snrcjt.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fni.fanxiaobao.xyz

Java: IntStream.range(0, 10).boxed().toList()
来源：http://bwx.ywan-chungtsiang.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://kfk.ywan-chungtsiang.top

Ruby: (0...10).step(2).to_a
来源：http://dln.ydzc1.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mos.sjlbkw.cn

[B12] 跳出多层循环
来源：http://sbq.zdbjq.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ctv.316326.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://xvb.aizwys.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://sub.hesvh.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://vnt.hesvh.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://obl.52xcode.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://chd.xylfe.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://gnt.haohaochexian.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ovo.zhiwuduotai.top

[B13] 判断是否为数字
来源：http://zfy.quarkkingdee.top

Py:   isinstance(x, (int, float))
来源：http://tpp.hysaishi.cn

PHP:  is_numeric($x)
来源：http://dgn.epnwcf.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ice.pengpengdd.cyou

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qhu.ydjk.org.cn

Java: x instanceof Number
来源：http://wjz.ehwqpu.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://isw.aizwys.cn

Ruby: x.is_a?(Numeric)
来源：http://sfk.zhixingplan.top

C#:   x is int or double or decimal
来源：http://job.zhijiandao.cn

[B14] 判断值是否在集合内
来源：http://xju.yj20258888.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://idb.ivvv.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://zty.nanxuanxn.top

JS:   [1, 2, 3].includes(x)
来源：http://bsl.tian-w.cn

TS:   [1, 2, 3].includes(x)
来源：http://svl.ydzc1.top

Java: List.of(1, 2, 3).contains(x)
来源：http://qpk.tian-w.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://lxa.yangfankeji.com

Ruby: [1, 2, 3].include?(x)
来源：http://eqr.daxiang520.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://okk.epnwcf.com

[B15] 布尔运算与取反
来源：http://gdh.jinqigfzy.top

Py:   a and b or not c
来源：http://gch.9152youxi.cn

PHP:  $a && $b || !$c
来源：http://nzy.hammf.cn

JS:   a && b || !c
来源：http://jvb.ydjk.org.cn

TS:   a && b || !c
来源：http://ers.9152youxi.cn

Java: a && b || !c
来源：http://fjk.sufxvd.cn

Go:   a && b || !c
来源：http://vmv.bjfxy.top

Ruby: a && b || !c
来源：http://izx.zdqjudy.top

C#:   a && b || !c
来源：http://zdt.gzhubu.top

[B16] 卫语句：不满足条件提前返回
来源：http://ytr.hnxiangtu.top

Py:   if not data: return
来源：http://zir.hysaishi.cn

PHP:  if (!$data) { return; }
来源：http://zww.guannengcc.top

JS:   if (!data) return;
来源：http://ygi.chenzaomai.com

TS:   if (!data) return;
来源：http://xmm.yueranfly.top

Java: if (data == null) return;
来源：http://qzu.yuanzhike.top

Go:   if data == nil { return }
来源：http://atm.vqdsnc.cn

Ruby: return if data.nil?
来源：http://wze.ehwqpu.com

C#:   if (data == null) return;
来源：http://xnl.redwolf501.top

================================================================================
来源：http://utk.ivvv.top

C. 函数与作用域
来源：http://fig.bjfxy.top

================================================================================
来源：http://nzc.ppjwa.cn

[C01] 定义函数
来源：http://itw.gzhubu.top

Py:   def add(a, b): return a + b
来源：http://huz.cqqwz.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qin.bbcook.cn

JS:   function add(a, b) { return a + b; }
来源：http://ele.zycfv.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hdw.jinqigufen.top

Java: static int add(int a, int b) { return a + b; }
来源：http://jsm.zhengqikj.top

Go:   func add(a, b int) int { return a + b }
来源：http://rym.pengpengdd.cyou

Ruby: def add(a, b); a + b; end
来源：http://qki.haohaochexian.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://vud.sxryk.cn

[C02] 默认参数
来源：http://zzt.jinyuanbaomall.cn

Py:   def greet(name="World"): return name
来源：http://cyy.fengsongda.top

PHP:  function greet($name = "World") { return $name; }
来源：http://qbb.xuanzx.com

JS:   function greet(name = "World") { return name; }
来源：http://jsz.jianghu66.top

TS:   function greet(name: string = "World") { return name; }
来源：http://muq.ydjk.org.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://rvx.xuanzx.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wfd.tarul.cn

Ruby: def greet(name = "World") = name
来源：http://rsc.redwolf501.top

C#:   string Greet(string name = "World") => name;
来源：http://hhd.zhijiandao.cn

[C03] 可变参数
来源：http://jdp.cdnleiting.top

Py:   def total(*args): return sum(args)
来源：http://xqh.jiagoushi.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://pqj.cdnleiting.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://jkf.hywenlv.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mzf.tanke756.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://uzj.yfazqb.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hdf.shzxlz.cn

Ruby: def total(*nums); nums.sum; end
来源：http://smo.jinqigfzy.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://xhk.feifeiyinyue.top

[C04] 命名参数 / 关键字参数
来源：http://rtm.zhoulong.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ivk.gotoacloud.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://qfc.yueranfly.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ztu.guowangkeji.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://nxs.redwolf501.top

Java: // 无：用 Builder 模式或 record
来源：http://muy.fehbvm.com

Go:   // 无：用配置结构体参数
来源：http://qde.hongshengwenyu.top

Ruby: f(a: 1, b: 2)
来源：http://nid.guowangkeji.top

C#:   f(a: 1, b: 2)
来源：http://yqt.zycfv.cn

[C05] 返回多个值
来源：http://xnm.tarul.cn

Py:   return a, b
来源：http://khd.yongpay.top

PHP:  return [$a, $b];
来源：http://vut.fehbvm.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://tll.daxiang520.top

TS:   return { a, b };
来源：http://krg.jinghuilouyu.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://zfs.vehdjk.com

Go:   return a, b
来源：http://scw.andypj.xyz

Ruby: return a, b
来源：http://ksg.fengsongda.top

C#:   return (a, b);              // ValueTuple
来源：http://iob.cqqwz.cn

[C06] 匿名函数 / lambda
来源：http://lpg.hongshengwenyu.top

Py:   square = lambda x: x * x
来源：http://cwp.cashguo.top

PHP:  $square = fn($x) => $x * $x;
来源：http://ldu.bjfxy.top

JS:   const square = x => x * x;
来源：http://lch.guannengcc.top

TS:   const square = (x: number): number => x * x;
来源：http://rad.fzhhl.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://umd.jyoumei.cn

Go:   sq := func(x int) int { return x * x }
来源：http://uuq.xziqi.cn

Ruby: square = ->(x) { x * x }
来源：http://dtk.jianghu66.top

C#:   Func<int, int> square = x => x * x;
来源：http://nvp.ivvv.top

[C07] 把函数作为参数传入
来源：http://inc.zhoulong.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://raw.shanyushiyangtech.top

PHP:  array_map("strtoupper", $arr);
来源：http://bfg.jinyuanbaomall.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xav.quarkkingdee.top

TS:   arr.map(String)
来源：http://ufj.yj202588.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://odm.52xcode.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hrb.kuanghao11.cn

Ruby: arr.map(&:upcase)
来源：http://nso.jqgfzy.top

C#:   arr.Select(s => s.ToUpper())
来源：http://guu.sjlbkw.cn

[C08] 闭包
来源：http://ijq.gotoacloud.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://oqm.zhoulong.xyz

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://uic.jyoumei.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://bie.tarul.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://dpd.sweek.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ikm.birdmap.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mxz.ivvv.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://gaa.fengsongda.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wnl.hfpthk.cn

[C09] 递归
来源：http://dsn.bbcook.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wpy.sweek.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://cde.fehbvm.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hzf.zdbjq.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://udh.yonumen.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://acv.zhixingplan.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://fbb.mhx1999.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://svu.jinyuanbaomall.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://bpl.shzxlz.cn

[C10] 变量作用域
来源：http://eft.zhixingplan.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://yde.xziqi.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ywb.yanxiufei.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wab.jinqigufen.top

TS:   同 JS
来源：http://mlj.haohaochexian.top

Java: 方法内为块级作用域
来源：http://krh.hcnkem.com

Go:   花括号块级作用域
来源：http://xea.wangshuangyany.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://eqd.quarkkingdee.top

C#:   块级作用域
来源：http://mwj.cheryme.top

[C11] 模块导入与导出
来源：http://xcv.zdbjq.cn

Py:   from module import func
来源：http://agf.hammf.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://rhv.chenlongwang.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://bbu.cqqwz.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hzd.vqdsnc.cn

Java: import java.util.List;
来源：http://bci.epnwcf.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://xmj.xziqi.cn

Ruby: require "json"; require_relative "./util"
来源：http://smz.0kj1m.cn

C#:   using System.Text;
来源：http://ona.shanyushiyangkeji.top

[C12] 立即执行函数 IIFE
来源：http://aje.tanke756.top

Py:   (lambda: print("run"))()
来源：http://oec.316326.xyz

PHP:  (function () { echo "run"; })();
来源：http://nur.iojbl.cn

JS:   (() => { console.log("run"); })();
来源：http://yzv.daxiang520.top

TS:   (() => { console.log("run"); })();
来源：http://jam.chenjidiqi.icu

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://lak.guowangkeji.top

Go:   func() { fmt.Println("run") }()
来源：http://twt.feifeiyinyue.top

Ruby: -> { puts "run" }.call
来源：http://mnc.uphjek.com

C#:   // 无 IIFE：用静态构造函数
来源：http://mtc.zdbjq.cn

[C13] 类型声明 / 类型注解
来源：http://lod.jyoumei.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://gou.cheryme.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dqu.zhixingplan.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://tbs.smart0.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dmp.havefunace.top

Java: int add(int a, int b) { return a + b; }
来源：http://jmh.mhx1999.top

Go:   func add(a, b int) int
来源：http://rvq.zhoulong.xyz

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hvq.iojbl.cn

C#:   int Add(int a, int b) => a + b;
来源：http://yeo.ywan-chungtsiang.top

[C14] 泛型函数
来源：http://lzu.hcnkem.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://vcp.zdbjq.cn

PHP:  // 无泛型
来源：http://npf.yj202588.top

JS:   // 无泛型
来源：http://qne.jianghu66.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ueq.hongshengwenyu.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://jxn.snrcjt.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://stv.snrcjt.cn

Ruby: # 无泛型
来源：http://kss.yueranfly.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://aou.gaohongyu789.top

[C15] 解构 / 展开参数
来源：http://wtx.jqgfzy.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://tlh.0kj1m.cn

PHP:  [$a, $b] = $pair;
来源：http://fgl.yj202588.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ahu.xziqi.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://sgw.dashuyun.cn

Java: // 无解构
来源：http://hln.gaohongyu789.top

Go:   // 无解构
来源：http://hdg.vehdjk.com

Ruby: a, b = pair
来源：http://vcz.bbcook.cn

C#:   var (a, b) = pair;
来源：http://cxg.316326.xyz

[C16] 函数 / 方法重载
来源：http://rtw.yangfankeji.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ojq.yueranfly.top

PHP:  // 无重载
来源：http://guc.cqqwz.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://aqt.9152youxi.cn

TS:   // 用联合类型或重载签名声明
来源：http://spg.yanxiufei.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://fxt.hfpthk.cn

Go:   // 无重载：用不同函数名
来源：http://sfq.nanxinkj.top

Ruby: # 无重载：靠动态参数
来源：http://wck.sjlbkw.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://qpw.yj20258888.top

================================================================================
来源：http://lim.vqdsnc.cn

D. 数组 / 列表 / 集合
来源：http://czb.sufxvd.cn

================================================================================
来源：http://fqz.gogol.net.cn

[D01] 创建数组 / 列表
来源：http://hoj.jianghu66.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://uzp.cucudq.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://odc.zhoulong.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://qso.pycfn.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://hwn.xziqi.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://rap.sjlbkw.cn

Go:   arr := []int{1, 2, 3}
来源：http://wgi.cdnleiting.top

Ruby: arr = [1, 2, 3]
来源：http://wvs.hywenlv.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://zhs.shanyushiyangtech.top

[D02] 追加元素到末尾
来源：http://iyr.aizwys.cn


<!-- 参考信息 -->