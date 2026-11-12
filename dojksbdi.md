代发 wailian999

[B01] 条件判断 if / else
来源：http://qdf.dianchejie.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://gkt.andypj.xyz

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hqi.pycfn.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://duy.hesvh.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://cpq.ybcxt.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://lgi.quarkkingdee.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://oen.yangfankeji.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ssx.jqgfzy.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://bnz.svipenyu.cn

[B02] 多分支 else if / elif
来源：http://qsh.dashuyun.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://bvt.yangfankeji.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://cer.hfpthk.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bdf.nwbrower.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oia.epnwcf.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kvr.jyoumei.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://rxb.hfpthk.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://qdd.pengpengdd.cyou

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ifx.jianghu66.top

[B03] switch / match / case
来源：http://vjt.aibaodan.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://nem.gogol.net.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ndr.jinqigufen.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rvm.jiagoushi.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qku.tianlin.xyz

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://gmw.cqqwz.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://rlc.gzhubu.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://pwc.hcnkem.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://aev.chenzaomai.com

[B04] for 计数循环
来源：http://izr.cdnleiting.top

Py:   for i in range(10): print(i)
来源：http://nom.shanyushiyangtech.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://iqq.jinyuanbaomall.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pje.yuxming.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ied.yonumen.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://zoe.sweek.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://eab.52xcode.cn

Ruby: 10.times { |i| puts i }
来源：http://xzz.dianchejie.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://dfh.sufxvd.cn

[B05] 遍历数组 / 列表
来源：http://nwh.vehdjk.com

Py:   for item in arr: print(item)
来源：http://hgs.jinyuanbaomall.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://soj.yj20258.top

JS:   for (const item of arr) { console.log(item); }
来源：http://qqk.gotoacloud.top

TS:   for (const item of arr) { console.log(item); }
来源：http://iub.zdqjudy.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://szd.yj202588.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ows.pycfn.com

Ruby: arr.each { |item| puts item }
来源：http://vbf.havefunace.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ulg.guannengcc.top

[B06] 遍历字典 / 对象
来源：http://jra.fengsongda.top

Py:   for k, v in d.items(): print(k, v)
来源：http://btv.zhongyouzk.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://xdz.smart0.xyz

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://owa.yonumen.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rer.chenjidiqi.icu

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hah.jyoumei.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://xvf.redwolf501.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://uid.shanyushiyangkeji.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://cuu.yongpay.top

[B07] while 循环
来源：http://bjj.ydjk.org.cn

Py:   while i < 10: i += 1
来源：http://rls.yj20258888.top

PHP:  while ($i < 10) { $i++; }
来源：http://qae.zhongyouzk.top

JS:   while (i < 10) { i++; }
来源：http://jey.svipenyu.cn

TS:   while (i < 10) { i++; }
来源：http://uag.shanyushiyangtech.top

Java: while (i < 10) { i++; }
来源：http://pzh.hywenlv.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://kcb.zycfv.cn

Ruby: while i < 10; i += 1; end
来源：http://kyi.yuxming.cn

C#:   while (i < 10) { i++; }
来源：http://kte.jianghu66.top

[B08] do-while（至少执行一次）
来源：http://fzx.yj20258.top

Py:   # 无 do-while：用 while True + break
来源：http://rww.cqqwz.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ken.jqgufenzy.top

JS:   do { i++; } while (i < 10);
来源：http://ntn.bbcook.cn

TS:   do { i++; } while (i < 10);
来源：http://qkn.yvedp.cn

Java: do { i++; } while (i < 10);
来源：http://nca.yuanzhike.top

Go:   for { i++; if i >= 10 { break } }
来源：http://boa.vehdjk.com

Ruby: begin; i += 1; end while i < 10
来源：http://hip.hywenlv.cn

C#:   do { i++; } while (i < 10);
来源：http://jbx.cucudq.cn

[B09] break 与 continue
来源：http://qle.zhoulong.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://uso.kuanghao11.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mnk.jqgfzy.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ujd.kuanghao11.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cjb.shzxlz.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rto.yongpay.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://aju.yvedp.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ajv.xingfuxueyuan.xyz

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://stq.jyoumei.cn

[B10] 遍历同时拿索引
来源：http://lkw.cheryme.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://uut.ybcxt.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://kpa.sweek.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://cxj.xziqi.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://gtm.cashguo.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://uzp.xuetiantiany.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://tbi.yfazqb.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://qin.pycfn.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ily.andypj.xyz

[B11] 生成数字序列 / 区间
来源：http://zgr.xingfuxueyuan.xyz

Py:   list(range(0, 10, 2))
来源：http://awe.yj20258888.top

PHP:  range(0, 10, 2);
来源：http://jgu.xingfuxueyuan.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://msi.shanyushiyangtech.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://uwp.tianlin.xyz

Java: IntStream.range(0, 10).boxed().toList()
来源：http://olm.yueranfly.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://tik.havefunace.top

Ruby: (0...10).step(2).to_a
来源：http://mer.tanke756.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://vdp.andypj.xyz

[B12] 跳出多层循环
来源：http://fyf.quarkkingdee.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://xak.ybcxt.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://ull.bbcook.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://myu.zhixingplan.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://fky.sweek.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://afl.52xcode.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://qdk.epnwcf.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://xei.zhengqikj.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://dry.chenlongwang.top

[B13] 判断是否为数字
来源：http://dyn.zhoulong.xyz

Py:   isinstance(x, (int, float))
来源：http://ksp.nwbrower.top

PHP:  is_numeric($x)
来源：http://sjs.cashguo.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gyt.aizwys.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://smo.ehwqpu.com

Java: x instanceof Number
来源：http://fce.hfpthk.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ujw.yuxming.cn

Ruby: x.is_a?(Numeric)
来源：http://nrq.redwolf501.top

C#:   x is int or double or decimal
来源：http://fhs.nanxinkj.top

[B14] 判断值是否在集合内
来源：http://dna.feifeiyinyue.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://zrr.hcnkem.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ymi.yanxiufei.cn

JS:   [1, 2, 3].includes(x)
来源：http://nmy.aizwys.cn

TS:   [1, 2, 3].includes(x)
来源：http://myt.sysykeji.top

Java: List.of(1, 2, 3).contains(x)
来源：http://wqx.uphjek.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://fvb.birdmap.top

Ruby: [1, 2, 3].include?(x)
来源：http://bna.vqdsnc.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ilc.zhixingplan.top

[B15] 布尔运算与取反
来源：http://lpu.shzxlz.cn

Py:   a and b or not c
来源：http://tej.fehbvm.com

PHP:  $a && $b || !$c
来源：http://zbu.zhiwuduotai.top

JS:   a && b || !c
来源：http://lip.ppjwa.cn

TS:   a && b || !c
来源：http://xyo.zhoulong.xyz

Java: a && b || !c
来源：http://cdo.bbcook.cn

Go:   a && b || !c
来源：http://afo.xziqi.cn

Ruby: a && b || !c
来源：http://kvk.yvedp.cn

C#:   a && b || !c
来源：http://ire.sweek.top

[B16] 卫语句：不满足条件提前返回
来源：http://kzn.xinyue.icu

Py:   if not data: return
来源：http://ejm.zhijiandao.cn

PHP:  if (!$data) { return; }
来源：http://eff.feifeiyinyue.top

JS:   if (!data) return;
来源：http://eon.zhongyouzk.top

TS:   if (!data) return;
来源：http://kbi.c1oappe.top

Java: if (data == null) return;
来源：http://flj.wangdashe.top

Go:   if data == nil { return }
来源：http://kdw.yueranfly.top

Ruby: return if data.nil?
来源：http://eim.sxryk.cn

C#:   if (data == null) return;
来源：http://tqw.xuanzx.com

================================================================================
来源：http://mtv.jqgufenzy.top

C. 函数与作用域
来源：http://dqx.zhengqikj.top

================================================================================
来源：http://tlz.kuanghao11.cn

[C01] 定义函数
来源：http://kef.hywenlv.cn

Py:   def add(a, b): return a + b
来源：http://qua.hnxiangtu.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vgu.shuidangran.top

JS:   function add(a, b) { return a + b; }
来源：http://qtq.wangshuangyany.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nwl.daxiang520.top

Java: static int add(int a, int b) { return a + b; }
来源：http://pfn.shuidangran.top

Go:   func add(a, b int) int { return a + b }
来源：http://ibg.jlsjyb.cn

Ruby: def add(a, b); a + b; end
来源：http://jks.yanxiufei.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://kpk.yonumen.top

[C02] 默认参数
来源：http://oqp.zycfv.cn

Py:   def greet(name="World"): return name
来源：http://eft.jyoumei.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://rym.meibo888.top

JS:   function greet(name = "World") { return name; }
来源：http://ebg.havefunace.top

TS:   function greet(name: string = "World") { return name; }
来源：http://eis.cqqwz.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://hak.bbcook.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://jfw.jyoumei.cn

Ruby: def greet(name = "World") = name
来源：http://fgx.yongpay.top

C#:   string Greet(string name = "World") => name;
来源：http://moj.hysaishi.cn

[C03] 可变参数
来源：http://mnr.daria6918.cn

Py:   def total(*args): return sum(args)
来源：http://umo.yj202588.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://jtf.tarul.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://fwm.epnwcf.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://cjh.xingfuxueyuan.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://irt.pycfn.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://nqj.guowangkeji.top

Ruby: def total(*nums); nums.sum; end
来源：http://daq.yuanzhike.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://nkl.zhengqikj.top

[C04] 命名参数 / 关键字参数
来源：http://vbb.jlsjyb.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://jmt.nanxuanxn.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://jwa.zhengqikj.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ebc.dianchejie.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mbr.shanyushiyangtech.top

Java: // 无：用 Builder 模式或 record
来源：http://arf.zdbjq.cn

Go:   // 无：用配置结构体参数
来源：http://mkh.redwolf501.top

Ruby: f(a: 1, b: 2)
来源：http://noz.andypj.xyz

C#:   f(a: 1, b: 2)
来源：http://ydy.jlsjyb.cn

[C05] 返回多个值
来源：http://lml.havefunace.top

Py:   return a, b
来源：http://mix.vehdjk.com

PHP:  return [$a, $b];
来源：http://adw.zhoulong.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://szd.ppjwa.cn

TS:   return { a, b };
来源：http://wer.zhiwuduotai.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://igp.zhengqikj.top

Go:   return a, b
来源：http://bvx.smart0.xyz

Ruby: return a, b
来源：http://wdw.fktsv.cn

C#:   return (a, b);              // ValueTuple
来源：http://ajc.ivvv.top

[C06] 匿名函数 / lambda
来源：http://sdv.pengpengdd.cyou

Py:   square = lambda x: x * x
来源：http://vay.xuetiantiany.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://zgt.yangfankeji.com

JS:   const square = x => x * x;
来源：http://tdw.iojbl.cn

TS:   const square = (x: number): number => x * x;
来源：http://hbg.andypj.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://cou.jinyuanbaomall.cn

Go:   sq := func(x int) int { return x * x }
来源：http://pkk.iojbl.cn

Ruby: square = ->(x) { x * x }
来源：http://brf.yuanzhike.top

C#:   Func<int, int> square = x => x * x;
来源：http://vxm.redwolf501.top

[C07] 把函数作为参数传入
来源：http://gag.cqqwz.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://gzc.fengsongda.top

PHP:  array_map("strtoupper", $arr);
来源：http://bot.jinyuanbaomall.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://tii.nanxuanxn.top

TS:   arr.map(String)
来源：http://iwq.316326.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://llu.feifeiyinyue.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://kqt.quarkkingdee.top

Ruby: arr.map(&:upcase)
来源：http://zms.xuanzx.com

C#:   arr.Select(s => s.ToUpper())
来源：http://nkz.sxryk.cn

[C08] 闭包
来源：http://zgu.wangdashe.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wzd.sxryk.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://duc.0kj1m.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://knc.fktsv.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://xaj.aizwys.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://vsw.fanxiaobao.xyz

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://bat.vehdjk.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://xnt.fktsv.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hmg.xuanzx.com

[C09] 递归
来源：http://ufe.xziqi.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hmn.zdbjq.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://euv.jinqigufen.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cbu.yueranfly.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kty.yj202588.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://tgp.shanyushiyangtech.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mos.hfpthk.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ahm.fehbvm.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://nhj.feifeiyinyue.top

[C10] 变量作用域
来源：http://mjm.fengsongda.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://kbv.xinyue.icu

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://oae.fktsv.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://axq.316326.xyz

TS:   同 JS
来源：http://fdr.fktsv.cn

Java: 方法内为块级作用域
来源：http://ife.fktsv.cn

Go:   花括号块级作用域
来源：http://ihx.cashguo.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://yhh.sufxvd.cn

C#:   块级作用域
来源：http://bvo.yongpay.top

[C11] 模块导入与导出
来源：http://jxq.cqqwz.cn

Py:   from module import func
来源：http://byz.wangdashe.top

PHP:  require "file.php";  或 use App\Service;
来源：http://vas.haohaochexian.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://xre.hesvh.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ghe.ivvv.top

Java: import java.util.List;
来源：http://hyl.yj20258888.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mti.fengsongda.top

Ruby: require "json"; require_relative "./util"
来源：http://yhg.zhaomingkeji.xyz

C#:   using System.Text;
来源：http://six.svipenyu.cn

[C12] 立即执行函数 IIFE
来源：http://tqs.guannengcc.top

Py:   (lambda: print("run"))()
来源：http://gtf.zhixingplan.top

PHP:  (function () { echo "run"; })();
来源：http://nrw.zhixingplan.top

JS:   (() => { console.log("run"); })();
来源：http://nxi.zdqjudy.top

TS:   (() => { console.log("run"); })();
来源：http://sqk.fzhhl.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://xxp.guowangkeji.top

Go:   func() { fmt.Println("run") }()
来源：http://pbj.cucudq.cn

Ruby: -> { puts "run" }.call
来源：http://bzh.jinqigufen.top

C#:   // 无 IIFE：用静态构造函数
来源：http://woi.ydjk.org.cn

[C13] 类型声明 / 类型注解
来源：http://dax.sweek.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hqn.hesvh.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zti.sweek.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://act.zhiwuduotai.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mmj.daxiang520.top

Java: int add(int a, int b) { return a + b; }
来源：http://thf.c1oappe.top

Go:   func add(a, b int) int
来源：http://ycl.uphjek.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://syk.xuetiantiany.cn

C#:   int Add(int a, int b) => a + b;
来源：http://yhi.yangfankeji.com

[C14] 泛型函数
来源：http://nzp.daria6918.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://grh.yuanzhike.top

PHP:  // 无泛型
来源：http://eyb.gzhubu.top

JS:   // 无泛型
来源：http://aur.ybcxt.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://xmq.ivvv.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://pdc.dianchejie.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://zve.cashguo.top

Ruby: # 无泛型
来源：http://dec.hammf.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://bfe.xziqi.cn

[C15] 解构 / 展开参数
来源：http://igu.9152youxi.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://lcu.hnxiangtu.top

PHP:  [$a, $b] = $pair;
来源：http://ufs.ydzc1.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://jus.dashuyun.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://qkw.pengpengdd.cyou

Java: // 无解构
来源：http://ett.zhongyouzk.top

Go:   // 无解构
来源：http://xqx.chenzaomai.com

Ruby: a, b = pair
来源：http://lnz.sufxvd.cn

C#:   var (a, b) = pair;
来源：http://pzc.ctjpmb.com

[C16] 函数 / 方法重载
来源：http://cgr.redwolf501.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://zvz.xinyue.icu

PHP:  // 无重载
来源：http://pwy.yuxming.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://atn.wangdashe.top

TS:   // 用联合类型或重载签名声明
来源：http://nok.zdbjq.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://lsf.gotoacloud.top

Go:   // 无重载：用不同函数名
来源：http://thq.zhengqikj.top

Ruby: # 无重载：靠动态参数
来源：http://lto.gogol.net.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ctu.hesvh.cn

================================================================================
来源：http://qbo.chenlongwang.top

D. 数组 / 列表 / 集合
来源：http://ers.redwolf501.top

================================================================================
来源：http://tdt.gaohongyu789.top

[D01] 创建数组 / 列表
来源：http://tmx.jinghuilouyu.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://esh.redwolf501.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://pnp.cdnleiting.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mlc.ydzc1.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://jvv.fanxiaobao.xyz

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://pmi.guowangkeji.top


<!-- 参考信息 -->