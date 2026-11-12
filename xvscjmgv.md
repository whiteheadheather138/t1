代发 wailian999

[B01] 条件判断 if / else
来源：http://rhy.hcnkem.com

Py:   result = "正" if x > 0 else "非正"
来源：http://evj.gaohongyu789.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mxx.tarul.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ztp.cucudq.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://qba.iojbl.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ihp.nwbrower.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://zxg.xylfe.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wun.xinyue.icu

C#:   var r = x > 0 ? "正" : "非正";
来源：http://jrj.pycfn.com

[B02] 多分支 else if / elif
来源：http://jyf.birdmap.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://htd.ydjk.org.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://jqx.guowangkeji.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://onz.zdqjudy.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ndx.cheryme.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rmw.jqgfzy.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://plj.epnwcf.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ept.fzhhl.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bnl.xinyue.icu

[B03] switch / match / case
来源：http://rkf.zhongyouzk.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ebb.hnxiangtu.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://jmb.52xcode.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://llm.nwbrower.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lxd.jinghuilouyu.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://xlp.ppjwa.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://qgb.yangfankeji.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://jpn.smart0.xyz

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://tzs.gogol.net.cn

[B04] for 计数循环
来源：http://vii.svipenyu.cn

Py:   for i in range(10): print(i)
来源：http://hwg.zhaomingkeji.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://dzt.cqqwz.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xjz.mhx1999.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lwx.zhongyouzk.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wzt.zhaomingkeji.xyz

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://eij.dashuyun.cn

Ruby: 10.times { |i| puts i }
来源：http://lju.jinyuanbaomall.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://zmf.ehwqpu.com

[B05] 遍历数组 / 列表
来源：http://wbo.jinqigufen.top

Py:   for item in arr: print(item)
来源：http://ovx.hywenlv.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://gxs.yuanzhike.top

JS:   for (const item of arr) { console.log(item); }
来源：http://bxo.uphjek.com

TS:   for (const item of arr) { console.log(item); }
来源：http://bgs.ppjwa.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://gwp.zdqjudy.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wnx.yj20258.top

Ruby: arr.each { |item| puts item }
来源：http://fxe.sweek.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://vha.nanxuanxn.top

[B06] 遍历字典 / 对象
来源：http://fcr.tarul.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://sme.9152youxi.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://qja.pycfn.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ice.yj202588.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fsu.fktsv.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ell.ppjwa.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://otw.yuxming.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ayu.yfazqb.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://fcj.mhx1999.top

[B07] while 循环
来源：http://iar.redwolf501.top

Py:   while i < 10: i += 1
来源：http://jul.xziqi.cn

PHP:  while ($i < 10) { $i++; }
来源：http://cfu.fengsongda.top

JS:   while (i < 10) { i++; }
来源：http://oxz.zdqjudy.top

TS:   while (i < 10) { i++; }
来源：http://rxi.jyoumei.cn

Java: while (i < 10) { i++; }
来源：http://iyt.epnwcf.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://qpi.jiagoushi.top

Ruby: while i < 10; i += 1; end
来源：http://ons.zdbjq.cn

C#:   while (i < 10) { i++; }
来源：http://qep.fzhhl.top

[B08] do-while（至少执行一次）
来源：http://dst.aizwys.cn

Py:   # 无 do-while：用 while True + break
来源：http://rva.cheryme.top

PHP:  do { $i++; } while ($i < 10);
来源：http://zbe.yj20258.top

JS:   do { i++; } while (i < 10);
来源：http://xjn.pycfn.com

TS:   do { i++; } while (i < 10);
来源：http://his.c1oappe.top

Java: do { i++; } while (i < 10);
来源：http://hck.daria6918.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://iyf.xylfe.cn

Ruby: begin; i += 1; end while i < 10
来源：http://kch.shzxlz.cn

C#:   do { i++; } while (i < 10);
来源：http://aae.gzhubu.top

[B09] break 与 continue
来源：http://qht.tianlin.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://llx.jinqigufen.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://kvm.zdbjq.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ukn.pycfn.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qce.yfazqb.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kpd.zhoulong.xyz

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://bvw.ywan-chungtsiang.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://fwo.zhoulong.xyz

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wns.smart0.xyz

[B10] 遍历同时拿索引
来源：http://ryj.meibo888.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://zlb.sysykeji.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://pcb.gogol.net.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wzx.fengsongda.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://pfw.jinqigufen.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://gcu.epnwcf.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ada.9152youxi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://nyn.tian-w.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://qql.yanxiufei.cn

[B11] 生成数字序列 / 区间
来源：http://wmm.shanyushiyangkeji.top

Py:   list(range(0, 10, 2))
来源：http://ddj.fzhhl.top

PHP:  range(0, 10, 2);
来源：http://sny.andypj.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lbw.shangyingyoupin.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://aji.52xcode.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://vce.jianghu66.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://tzm.wangdashe.top

Ruby: (0...10).step(2).to_a
来源：http://viv.guowangkeji.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://jdo.hcnkem.com

[B12] 跳出多层循环
来源：http://vef.52xcode.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://hti.yangfankeji.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://dqb.redwolf501.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://rdy.mhx1999.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://kla.jinqigufen.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://quu.sufxvd.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://cfm.cashguo.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ocz.zhengqikj.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://vmj.meibo888.top

[B13] 判断是否为数字
来源：http://gtw.0kj1m.cn

Py:   isinstance(x, (int, float))
来源：http://ysu.fanxiaobao.xyz

PHP:  is_numeric($x)
来源：http://bhm.zhongyouzk.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ayi.jianghu66.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jge.yj20258.top

Java: x instanceof Number
来源：http://gcq.jianghu66.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://rzw.tianlin.xyz

Ruby: x.is_a?(Numeric)
来源：http://umo.cashguo.top

C#:   x is int or double or decimal
来源：http://gej.guannengcc.top

[B14] 判断值是否在集合内
来源：http://gwj.sjlbkw.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jza.jyoumei.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ehk.daria6918.cn

JS:   [1, 2, 3].includes(x)
来源：http://otn.feifeiyinyue.top

TS:   [1, 2, 3].includes(x)
来源：http://vfv.zhoulong.xyz

Java: List.of(1, 2, 3).contains(x)
来源：http://vzx.sjlbkw.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://jbm.havefunace.top

Ruby: [1, 2, 3].include?(x)
来源：http://she.chenzaomai.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://zar.ctjpmb.com

[B15] 布尔运算与取反
来源：http://aay.feifeiyinyue.top

Py:   a and b or not c
来源：http://jzv.cqqwz.cn

PHP:  $a && $b || !$c
来源：http://xdr.tianlin.xyz

JS:   a && b || !c
来源：http://fod.jyoumei.cn

TS:   a && b || !c
来源：http://ptz.52xcode.cn

Java: a && b || !c
来源：http://mzo.bbcook.cn

Go:   a && b || !c
来源：http://sfo.kuanghao11.cn

Ruby: a && b || !c
来源：http://dyn.gzhubu.top

C#:   a && b || !c
来源：http://ajf.chenjidiqi.icu

[B16] 卫语句：不满足条件提前返回
来源：http://dju.yongpay.top

Py:   if not data: return
来源：http://ltq.cheryme.top

PHP:  if (!$data) { return; }
来源：http://fob.sysykeji.top

JS:   if (!data) return;
来源：http://nve.tarul.cn

TS:   if (!data) return;
来源：http://ewj.epnwcf.com

Java: if (data == null) return;
来源：http://uhp.9152youxi.cn

Go:   if data == nil { return }
来源：http://pvk.kuanghao11.cn

Ruby: return if data.nil?
来源：http://aqs.yueranfly.top

C#:   if (data == null) return;
来源：http://unc.yj20258.top

================================================================================
来源：http://sne.jyoumei.cn

C. 函数与作用域
来源：http://fdj.316326.xyz

================================================================================
来源：http://nxi.epnwcf.com

[C01] 定义函数
来源：http://rlf.cashguo.top

Py:   def add(a, b): return a + b
来源：http://wss.zdqjudy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://eht.shanyushiyangkeji.top

JS:   function add(a, b) { return a + b; }
来源：http://ovm.smart0.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tgq.tanke756.top

Java: static int add(int a, int b) { return a + b; }
来源：http://wsn.daria6918.cn

Go:   func add(a, b int) int { return a + b }
来源：http://jrx.jqgfzy.top

Ruby: def add(a, b); a + b; end
来源：http://xad.fzhhl.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hbp.yangfankeji.com

[C02] 默认参数
来源：http://oaj.xingfuxueyuan.xyz

Py:   def greet(name="World"): return name
来源：http://zpm.chenlongwang.top

PHP:  function greet($name = "World") { return $name; }
来源：http://wlg.xuanzx.com

JS:   function greet(name = "World") { return name; }
来源：http://dwv.zhongyouzk.top

TS:   function greet(name: string = "World") { return name; }
来源：http://aoy.fehbvm.com

Java: // 无默认参数：方法重载或 Optional
来源：http://mjv.chenzaomai.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ddp.cdnleiting.top

Ruby: def greet(name = "World") = name
来源：http://miz.yuanzhike.top

C#:   string Greet(string name = "World") => name;
来源：http://ufc.jinghuilouyu.cn

[C03] 可变参数
来源：http://glj.zdqjudy.top

Py:   def total(*args): return sum(args)
来源：http://hcc.yfazqb.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://oka.shanyushiyangkeji.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://jgz.yangfankeji.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://bmv.xuanzx.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://zde.gotoacloud.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://avt.tarul.cn

Ruby: def total(*nums); nums.sum; end
来源：http://xmr.yangfankeji.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://sdf.hongshengwenyu.top

[C04] 命名参数 / 关键字参数
来源：http://jxc.bbcook.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://drk.nanxuanxn.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://gru.52xcode.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://yea.mhx1999.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://oux.nwbrower.top

Java: // 无：用 Builder 模式或 record
来源：http://qca.jinqigfzy.top

Go:   // 无：用配置结构体参数
来源：http://ycr.dashuyun.cn

Ruby: f(a: 1, b: 2)
来源：http://zsj.zhaomingkeji.xyz

C#:   f(a: 1, b: 2)
来源：http://gmr.jlsjyb.cn

[C05] 返回多个值
来源：http://mpq.xingfuxueyuan.xyz

Py:   return a, b
来源：http://kfz.fengsongda.top

PHP:  return [$a, $b];
来源：http://dnl.yfazqb.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://mmb.iojbl.cn

TS:   return { a, b };
来源：http://jip.pengpengdd.cyou

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xav.ppjwa.cn

Go:   return a, b
来源：http://wet.zhongyouzk.top

Ruby: return a, b
来源：http://cyu.haohaochexian.top

C#:   return (a, b);              // ValueTuple
来源：http://qgm.epnwcf.com

[C06] 匿名函数 / lambda
来源：http://mnd.dianchejie.cn

Py:   square = lambda x: x * x
来源：http://laq.sxryk.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://kep.tanke756.top

JS:   const square = x => x * x;
来源：http://vsm.gotoacloud.top

TS:   const square = (x: number): number => x * x;
来源：http://akj.zhongyouzk.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://myr.tian-w.cn

Go:   sq := func(x int) int { return x * x }
来源：http://dsx.dianchejie.cn

Ruby: square = ->(x) { x * x }
来源：http://hep.fengsongda.top

C#:   Func<int, int> square = x => x * x;
来源：http://dvn.zdqjudy.top

[C07] 把函数作为参数传入
来源：http://cku.hammf.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://kje.hywenlv.cn

PHP:  array_map("strtoupper", $arr);
来源：http://jlh.nanxuanxn.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ikl.wangdashe.top

TS:   arr.map(String)
来源：http://uoa.cdnleiting.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hhr.hongshengwenyu.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://sur.zycfv.cn

Ruby: arr.map(&:upcase)
来源：http://odh.smart0.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://kqu.gaohongyu789.top

[C08] 闭包
来源：http://wwt.sweek.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://cwb.yongpay.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://xbk.aizwys.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://utl.hnxiangtu.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://kdd.jinqigfzy.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mms.daxiang520.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://uxe.fktsv.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://orb.pycfn.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hbv.iojbl.cn

[C09] 递归
来源：http://whj.chenlongwang.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://vbg.hfpthk.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ykl.cheryme.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mfk.fengsongda.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zkk.fehbvm.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://bah.xziqi.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://cgq.havefunace.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://frg.fktsv.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://nyp.yongpay.top

[C10] 变量作用域
来源：http://xtg.epnwcf.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qtk.shangyingyoupin.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://qcs.zycfv.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ijz.gaohongyu789.top

TS:   同 JS
来源：http://pml.zdbjq.cn

Java: 方法内为块级作用域
来源：http://brj.hywenlv.cn

Go:   花括号块级作用域
来源：http://uev.yanxiufei.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://uol.shanyushiyangtech.top

C#:   块级作用域
来源：http://ovb.yvedp.cn

[C11] 模块导入与导出
来源：http://rog.gaohongyu789.top

Py:   from module import func
来源：http://wgz.iojbl.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://xpy.kuanghao11.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://dmg.hfpthk.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://igp.bjfxy.top

Java: import java.util.List;
来源：http://fra.hysaishi.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://rfc.jianghu66.top

Ruby: require "json"; require_relative "./util"
来源：http://ycb.zhengqikj.top

C#:   using System.Text;
来源：http://pus.ydjk.org.cn

[C12] 立即执行函数 IIFE
来源：http://pza.yanxiufei.cn

Py:   (lambda: print("run"))()
来源：http://mdo.fengsongda.top

PHP:  (function () { echo "run"; })();
来源：http://fkx.fzhhl.top

JS:   (() => { console.log("run"); })();
来源：http://xfw.sweek.top

TS:   (() => { console.log("run"); })();
来源：http://hvq.sysykeji.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://eik.vehdjk.com

Go:   func() { fmt.Println("run") }()
来源：http://pko.ywan-chungtsiang.top

Ruby: -> { puts "run" }.call
来源：http://uxx.hfpthk.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ktf.cheryme.top

[C13] 类型声明 / 类型注解
来源：http://pko.yuanzhike.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ogs.feifeiyinyue.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rtq.shangyingyoupin.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://msl.svipenyu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yif.ctjpmb.com

Java: int add(int a, int b) { return a + b; }
来源：http://ome.uphjek.com

Go:   func add(a, b int) int
来源：http://bib.ydjk.org.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://azh.shuidangran.top

C#:   int Add(int a, int b) => a + b;
来源：http://lra.redwolf501.top

[C14] 泛型函数
来源：http://pdg.quarkkingdee.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://nyl.svipenyu.cn

PHP:  // 无泛型
来源：http://nve.chenjidiqi.icu

JS:   // 无泛型
来源：http://cmd.hnqzz.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://nie.52xcode.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://cvc.pycfn.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hbe.nanxinkj.top

Ruby: # 无泛型
来源：http://til.zhengqikj.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://vxe.shanyushiyangkeji.top

[C15] 解构 / 展开参数
来源：http://kxw.xingfuxueyuan.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://aas.9152youxi.cn

PHP:  [$a, $b] = $pair;
来源：http://xku.hnxiangtu.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://nzn.kuanghao11.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ziz.xylfe.cn

Java: // 无解构
来源：http://jzf.chenjidiqi.icu

Go:   // 无解构
来源：http://vzh.daxiang520.top

Ruby: a, b = pair
来源：http://djp.jqgufenzy.top

C#:   var (a, b) = pair;
来源：http://utd.xylfe.cn

[C16] 函数 / 方法重载
来源：http://udd.nanxuanxn.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ccb.ppjwa.cn

PHP:  // 无重载
来源：http://cxo.fzhhl.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://pmj.svipenyu.cn

TS:   // 用联合类型或重载签名声明
来源：http://lvn.yvedp.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://qwe.yvedp.cn

Go:   // 无重载：用不同函数名
来源：http://hdi.yj202588.top

Ruby: # 无重载：靠动态参数
来源：http://dwe.yonumen.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://qfz.zhixingplan.top

================================================================================
来源：http://grm.yanxiufei.cn

D. 数组 / 列表 / 集合
来源：http://whb.zdbjq.cn

================================================================================
来源：http://vmo.daria6918.cn

[D01] 创建数组 / 列表
来源：http://ilp.aizwys.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://yzu.pycfn.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://glx.uphjek.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ioa.xylfe.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://efg.shangyingyoupin.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://smr.zhengqikj.top


<!-- 参考信息 -->