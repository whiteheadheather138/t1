代发 wailian999

TS:   const r = x > 0 ? "正" : "非正";
来源：http://kqo.tanke756.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://hkq.xylfe.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://viv.zdqjudy.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://qvr.haohaochexian.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://xts.aizwys.cn

[B02] 多分支 else if / elif
来源：http://ebd.nwbrower.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://rgj.fehbvm.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://iej.ybcxt.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wty.shangyingyoupin.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rcm.zhaomingkeji.xyz

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qzd.gogol.net.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://lhz.jqgufenzy.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://fau.hesvh.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://czr.daria6918.cn

[B03] switch / match / case
来源：http://ymo.sysykeji.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://lhk.snrcjt.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://dmb.xylfe.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lvz.gogol.net.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fbu.hongshengwenyu.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://tsq.wangshuangyany.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://slu.ppjwa.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://sfy.bbcook.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wyu.nwbrower.top

[B04] for 计数循环
来源：http://gll.zycfv.cn

Py:   for i in range(10): print(i)
来源：http://msl.pycfn.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://tjd.fktsv.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://psl.yfazqb.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ugs.yueranfly.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://kre.havefunace.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hyd.snrcjt.cn

Ruby: 10.times { |i| puts i }
来源：http://plm.yuxming.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://elp.yj20258888.top

[B05] 遍历数组 / 列表
来源：http://oga.nanxuanxn.top

Py:   for item in arr: print(item)
来源：http://fcd.havefunace.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mlq.jqgfzy.top

JS:   for (const item of arr) { console.log(item); }
来源：http://sae.shanyushiyangtech.top

TS:   for (const item of arr) { console.log(item); }
来源：http://oxk.hcnkem.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://cey.smart0.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://snq.fktsv.cn

Ruby: arr.each { |item| puts item }
来源：http://tbs.xingfuxueyuan.xyz

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://fju.xuetiantiany.cn

[B06] 遍历字典 / 对象
来源：http://hsg.tianlin.xyz

Py:   for k, v in d.items(): print(k, v)
来源：http://uic.ehwqpu.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hbg.andypj.xyz

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ijo.havefunace.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://efv.hywenlv.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://rit.yuxming.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://lqr.zhoulong.xyz

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://jks.cdnleiting.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://dll.zhaomingkeji.xyz

[B07] while 循环
来源：http://pzz.nanxuanxn.top

Py:   while i < 10: i += 1
来源：http://uwq.c1oappe.top

PHP:  while ($i < 10) { $i++; }
来源：http://lnh.sysykeji.top

JS:   while (i < 10) { i++; }
来源：http://fjz.dianchejie.cn

TS:   while (i < 10) { i++; }
来源：http://lmx.yj20258888.top

Java: while (i < 10) { i++; }
来源：http://reu.hongshengwenyu.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://kxt.pycfn.com

Ruby: while i < 10; i += 1; end
来源：http://ovv.nanxinkj.top

C#:   while (i < 10) { i++; }
来源：http://umk.yj20258888.top

[B08] do-while（至少执行一次）
来源：http://wtx.hammf.cn

Py:   # 无 do-while：用 while True + break
来源：http://pnf.pengpengdd.cyou

PHP:  do { $i++; } while ($i < 10);
来源：http://jxp.zhixingplan.top

JS:   do { i++; } while (i < 10);
来源：http://tyf.pengpengdd.cyou

TS:   do { i++; } while (i < 10);
来源：http://pzn.vqdsnc.cn

Java: do { i++; } while (i < 10);
来源：http://pzl.quarkkingdee.top

Go:   for { i++; if i >= 10 { break } }
来源：http://ool.shanyushiyangtech.top

Ruby: begin; i += 1; end while i < 10
来源：http://wyd.bjfxy.top

C#:   do { i++; } while (i < 10);
来源：http://wzh.guannengcc.top

[B09] break 与 continue
来源：http://kjg.jinyuanbaomall.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://avb.yangfankeji.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://owp.daxiang520.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jkb.tanke756.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uns.gotoacloud.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jvn.yuxming.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://nwq.wangdashe.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://too.feifeiyinyue.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uyf.shanyushiyangtech.top

[B10] 遍历同时拿索引
来源：http://hie.vehdjk.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://vxl.guannengcc.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://qjf.havefunace.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://bwh.wangdashe.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ppr.jinghuilouyu.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://qrg.xinyue.icu

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ffx.hnxiangtu.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://bkx.cqqwz.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://dwa.gogol.net.cn

[B11] 生成数字序列 / 区间
来源：http://kjh.pengpengdd.cyou

Py:   list(range(0, 10, 2))
来源：http://qrh.ctjpmb.com

PHP:  range(0, 10, 2);
来源：http://tto.ctjpmb.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://amx.jinqigfzy.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tca.jqgufenzy.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://bse.cqqwz.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://irr.tanke756.top

Ruby: (0...10).step(2).to_a
来源：http://bap.yongpay.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://xmv.redwolf501.top

[B12] 跳出多层循环
来源：http://nwg.cqqwz.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://igj.svipenyu.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ton.wangshuangyany.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://fbk.hysaishi.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hjw.wangdashe.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://qff.yuxming.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://nbz.316326.xyz

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mqm.tian-w.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://elt.snrcjt.cn

[B13] 判断是否为数字
来源：http://azv.shangyingyoupin.top

Py:   isinstance(x, (int, float))
来源：http://lpg.sufxvd.cn

PHP:  is_numeric($x)
来源：http://vka.yueranfly.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bmm.zhaomingkeji.xyz

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qbz.hcnkem.com

Java: x instanceof Number
来源：http://nry.cdnleiting.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://lsg.andypj.xyz

Ruby: x.is_a?(Numeric)
来源：http://qnb.pycfn.com

C#:   x is int or double or decimal
来源：http://ndr.316326.xyz

[B14] 判断值是否在集合内
来源：http://wel.jqgufenzy.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://aye.shangyingyoupin.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://dgy.zhijiandao.cn

JS:   [1, 2, 3].includes(x)
来源：http://tyz.jiagoushi.top

TS:   [1, 2, 3].includes(x)
来源：http://liu.ywan-chungtsiang.top

Java: List.of(1, 2, 3).contains(x)
来源：http://rma.0kj1m.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://eot.jinqigfzy.top

Ruby: [1, 2, 3].include?(x)
来源：http://eqb.dashuyun.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://iwh.hfpthk.cn

[B15] 布尔运算与取反
来源：http://ueh.cdnleiting.top

Py:   a and b or not c
来源：http://wam.0kj1m.cn

PHP:  $a && $b || !$c
来源：http://btq.tian-w.cn

JS:   a && b || !c
来源：http://pyv.andypj.xyz

TS:   a && b || !c
来源：http://ksm.xingfuxueyuan.xyz

Java: a && b || !c
来源：http://vau.gaohongyu789.top

Go:   a && b || !c
来源：http://pel.dianchejie.cn

Ruby: a && b || !c
来源：http://uqf.gotoacloud.top

C#:   a && b || !c
来源：http://ekj.hnxiangtu.top

[B16] 卫语句：不满足条件提前返回
来源：http://mvz.xuanzx.com

Py:   if not data: return
来源：http://qli.yj202588.top

PHP:  if (!$data) { return; }
来源：http://gau.snrcjt.cn

JS:   if (!data) return;
来源：http://ioc.cqqwz.cn

TS:   if (!data) return;
来源：http://ymw.guowangkeji.top

Java: if (data == null) return;
来源：http://rso.daria6918.cn

Go:   if data == nil { return }
来源：http://bae.aizwys.cn

Ruby: return if data.nil?
来源：http://qqt.cucudq.cn

C#:   if (data == null) return;
来源：http://mss.dianchejie.cn

================================================================================
来源：http://tqj.nanxinkj.top

C. 函数与作用域
来源：http://awt.wangdashe.top

================================================================================
来源：http://fyw.jqgfzy.top

[C01] 定义函数
来源：http://hou.yanxiufei.cn

Py:   def add(a, b): return a + b
来源：http://afa.shanyushiyangkeji.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ckq.pengpengdd.cyou

JS:   function add(a, b) { return a + b; }
来源：http://jxj.sjlbkw.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jjx.fehbvm.com

Java: static int add(int a, int b) { return a + b; }
来源：http://lob.aizwys.cn

Go:   func add(a, b int) int { return a + b }
来源：http://yxb.yonumen.top

Ruby: def add(a, b); a + b; end
来源：http://sjm.hesvh.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://nlz.fktsv.cn

[C02] 默认参数
来源：http://mre.jlsjyb.cn

Py:   def greet(name="World"): return name
来源：http://sos.zhixingplan.top

PHP:  function greet($name = "World") { return $name; }
来源：http://bsy.hnxiangtu.top

JS:   function greet(name = "World") { return name; }
来源：http://vol.hnxiangtu.top

TS:   function greet(name: string = "World") { return name; }
来源：http://izv.andypj.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://yov.sweek.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://gtc.xuanzx.com

Ruby: def greet(name = "World") = name
来源：http://ovz.iojbl.cn

C#:   string Greet(string name = "World") => name;
来源：http://yfo.birdmap.top

[C03] 可变参数
来源：http://ndx.jianghu66.top

Py:   def total(*args): return sum(args)
来源：http://vqj.zhengqikj.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://lcv.jqgufenzy.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://web.vehdjk.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://jre.zhixingplan.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://xpc.jianghu66.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://eex.jlsjyb.cn

Ruby: def total(*nums); nums.sum; end
来源：http://yin.jiagoushi.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://egk.aibaodan.cn

[C04] 命名参数 / 关键字参数
来源：http://zsi.sweek.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://zuf.snrcjt.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xvw.yanxiufei.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://vjd.zhijiandao.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hmb.kuanghao11.cn

Java: // 无：用 Builder 模式或 record
来源：http://cqu.yj20258.top

Go:   // 无：用配置结构体参数
来源：http://hnw.redwolf501.top

Ruby: f(a: 1, b: 2)
来源：http://hor.hfpthk.cn

C#:   f(a: 1, b: 2)
来源：http://lng.jyoumei.cn

[C05] 返回多个值
来源：http://nln.gzhubu.top

Py:   return a, b
来源：http://pxa.dashuyun.cn

PHP:  return [$a, $b];
来源：http://oza.hcnkem.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://qel.xylfe.cn

TS:   return { a, b };
来源：http://oqp.hnxiangtu.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://dln.ydjk.org.cn

Go:   return a, b
来源：http://nqk.ydjk.org.cn

Ruby: return a, b
来源：http://nef.yanxiufei.cn

C#:   return (a, b);              // ValueTuple
来源：http://nck.yj20258888.top

[C06] 匿名函数 / lambda
来源：http://pni.ehwqpu.com

Py:   square = lambda x: x * x
来源：http://mdh.jianghu66.top

PHP:  $square = fn($x) => $x * $x;
来源：http://tmp.havefunace.top

JS:   const square = x => x * x;
来源：http://xfe.yvedp.cn

TS:   const square = (x: number): number => x * x;
来源：http://zqe.cashguo.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://vib.havefunace.top

Go:   sq := func(x int) int { return x * x }
来源：http://ixe.feifeiyinyue.top

Ruby: square = ->(x) { x * x }
来源：http://rqc.fehbvm.com

C#:   Func<int, int> square = x => x * x;
来源：http://ysb.chenzaomai.com

[C07] 把函数作为参数传入
来源：http://zxe.uphjek.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://zti.0kj1m.cn

PHP:  array_map("strtoupper", $arr);
来源：http://akd.hywenlv.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wnq.redwolf501.top

TS:   arr.map(String)
来源：http://rmf.zhijiandao.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://kru.hnxiangtu.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qga.yuanzhike.top

Ruby: arr.map(&:upcase)
来源：http://fvw.zhaomingkeji.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://hry.zycfv.cn

[C08] 闭包
来源：http://noj.wangshuangyany.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://tmm.zdqjudy.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://sjh.yj202588.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://cex.zdbjq.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://efv.chenzaomai.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://qxd.ydjk.org.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wlh.xingfuxueyuan.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://qgl.zhengqikj.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ecz.redwolf501.top

[C09] 递归
来源：http://nph.mhx1999.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://unu.hnxiangtu.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ewz.0kj1m.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kil.xziqi.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jtx.snrcjt.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://lde.ybcxt.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wpe.chenzaomai.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://oax.xuanzx.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wcj.nanxuanxn.top

[C10] 变量作用域
来源：http://kgj.fengsongda.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qla.snrcjt.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://zfw.guannengcc.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://gcm.nwbrower.top

TS:   同 JS
来源：http://yey.nanxuanxn.top

Java: 方法内为块级作用域
来源：http://hnj.gogol.net.cn

Go:   花括号块级作用域
来源：http://hwd.yj20258888.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://kvd.pengpengdd.cyou

C#:   块级作用域
来源：http://rqr.hcnkem.com

[C11] 模块导入与导出
来源：http://jnm.0kj1m.cn

Py:   from module import func
来源：http://vnr.yj20258.top

PHP:  require "file.php";  或 use App\Service;
来源：http://kjh.quarkkingdee.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://fgo.aizwys.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hzh.svipenyu.cn

Java: import java.util.List;
来源：http://rvl.hnqzz.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://obo.fzhhl.top

Ruby: require "json"; require_relative "./util"
来源：http://zru.hesvh.cn

C#:   using System.Text;
来源：http://nkh.gzhubu.top

[C12] 立即执行函数 IIFE
来源：http://tfp.sweek.top

Py:   (lambda: print("run"))()
来源：http://eyb.cqqwz.cn

PHP:  (function () { echo "run"; })();
来源：http://mng.ivvv.top

JS:   (() => { console.log("run"); })();
来源：http://umv.fzhhl.top

TS:   (() => { console.log("run"); })();
来源：http://zbb.aibaodan.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://tcj.52xcode.cn

Go:   func() { fmt.Println("run") }()
来源：http://tip.iojbl.cn

Ruby: -> { puts "run" }.call
来源：http://pso.yj20258888.top

C#:   // 无 IIFE：用静态构造函数
来源：http://lqz.hnqzz.top

[C13] 类型声明 / 类型注解
来源：http://wfu.yfazqb.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://kzf.gaohongyu789.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tao.andypj.xyz

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ijf.jlsjyb.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hcp.nwbrower.top

Java: int add(int a, int b) { return a + b; }
来源：http://hat.yuxming.cn

Go:   func add(a, b int) int
来源：http://fbe.sxryk.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://fgz.52xcode.cn

C#:   int Add(int a, int b) => a + b;
来源：http://zsb.cheryme.top

[C14] 泛型函数
来源：http://wmq.ybcxt.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://koa.fanxiaobao.xyz

PHP:  // 无泛型
来源：http://sln.nanxuanxn.top

JS:   // 无泛型
来源：http://tic.mhx1999.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wyp.aizwys.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ajq.xuanzx.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wgq.aibaodan.cn

Ruby: # 无泛型
来源：http://afg.xingfuxueyuan.xyz

C#:   static T First<T>(List<T> items) => items[0];
来源：http://byg.shzxlz.cn

[C15] 解构 / 展开参数
来源：http://ayg.meibo888.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wnh.iojbl.cn

PHP:  [$a, $b] = $pair;
来源：http://lux.0kj1m.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ynu.meibo888.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hlr.sweek.top

Java: // 无解构
来源：http://gux.9152youxi.cn

Go:   // 无解构
来源：http://hgw.tianlin.xyz

Ruby: a, b = pair
来源：http://sah.yanxiufei.cn

C#:   var (a, b) = pair;
来源：http://tld.dianchejie.cn

[C16] 函数 / 方法重载
来源：http://zkf.jinghuilouyu.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://kzp.yonumen.top

PHP:  // 无重载
来源：http://fqw.uphjek.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://don.epnwcf.com

TS:   // 用联合类型或重载签名声明
来源：http://qou.pengpengdd.cyou

Java: void f(int a) {}  void f(String a) {}
来源：http://squ.zdqjudy.top

Go:   // 无重载：用不同函数名
来源：http://afc.ydjk.org.cn

Ruby: # 无重载：靠动态参数
来源：http://zkx.vqdsnc.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://cjl.fengsongda.top

================================================================================
来源：http://ohc.jqgfzy.top

D. 数组 / 列表 / 集合
来源：http://pbq.hnqzz.top

================================================================================
来源：http://bwd.jinqigufen.top

[D01] 创建数组 / 列表
来源：http://acx.tian-w.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://kae.fengsongda.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://xrr.xylfe.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://yrw.shzxlz.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://lls.birdmap.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://qur.kuanghao11.cn

Go:   arr := []int{1, 2, 3}
来源：http://mej.yuanzhike.top

Ruby: arr = [1, 2, 3]
来源：http://gdt.dianchejie.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://abb.bjfxy.top

[D02] 追加元素到末尾
来源：http://nca.bjfxy.top


<!-- 参考信息 -->