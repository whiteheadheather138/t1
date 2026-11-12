代发 wailian999

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://glv.nanxuanxn.top

================================================================================
来源：http://fxq.zhaomingkeji.xyz

B. 流程控制
来源：http://uqq.52xcode.cn

================================================================================
来源：http://fjg.guowangkeji.top

[B01] 条件判断 if / else
来源：http://rtv.haohaochexian.top

Py:   result = "正" if x > 0 else "非正"
来源：http://bou.fktsv.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://yfx.yj202588.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://izl.kuanghao11.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wje.snrcjt.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ckr.jinqigufen.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://cxe.ywan-chungtsiang.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://xgz.shzxlz.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://eyx.quarkkingdee.top

[B02] 多分支 else if / elif
来源：http://vkf.xziqi.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://awx.yuxming.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wvr.snrcjt.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nvd.smart0.xyz

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qtx.haohaochexian.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gqz.xylfe.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://dhz.ybcxt.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://qiq.9152youxi.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gav.cashguo.top

[B03] switch / match / case
来源：http://ggh.andypj.xyz

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://dhx.yj20258888.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hcu.jinghuilouyu.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rmv.feifeiyinyue.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rkh.hywenlv.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://dtv.zdbjq.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://jza.shzxlz.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://igw.hnxiangtu.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ffb.jinyuanbaomall.cn

[B04] for 计数循环
来源：http://gcx.xylfe.cn

Py:   for i in range(10): print(i)
来源：http://ixn.fehbvm.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://rgj.quarkkingdee.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://noi.guannengcc.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://uxe.yj202588.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://oxu.nanxinkj.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://byb.yuanzhike.top

Ruby: 10.times { |i| puts i }
来源：http://rpg.gogol.net.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ilo.zhaomingkeji.xyz

[B05] 遍历数组 / 列表
来源：http://dyy.shangyingyoupin.top

Py:   for item in arr: print(item)
来源：http://naf.yangfankeji.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ihp.gotoacloud.top

JS:   for (const item of arr) { console.log(item); }
来源：http://vkn.vqdsnc.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://xal.tanke756.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://pjz.cqqwz.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://fsd.0kj1m.cn

Ruby: arr.each { |item| puts item }
来源：http://ahw.yuxming.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://iok.vqdsnc.cn

[B06] 遍历字典 / 对象
来源：http://urt.jqgfzy.top

Py:   for k, v in d.items(): print(k, v)
来源：http://kcr.jianghu66.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ita.sysykeji.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://enr.yj202588.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nqt.iojbl.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://vqs.hywenlv.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hhw.yanxiufei.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ibr.zhoulong.xyz

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wwd.yj20258888.top

[B07] while 循环
来源：http://aut.uphjek.com

Py:   while i < 10: i += 1
来源：http://qnq.xylfe.cn

PHP:  while ($i < 10) { $i++; }
来源：http://vrt.yuxming.cn

JS:   while (i < 10) { i++; }
来源：http://rax.sysykeji.top

TS:   while (i < 10) { i++; }
来源：http://tfz.yvedp.cn

Java: while (i < 10) { i++; }
来源：http://aaz.sufxvd.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://utt.jianghu66.top

Ruby: while i < 10; i += 1; end
来源：http://pde.tianlin.xyz

C#:   while (i < 10) { i++; }
来源：http://xat.cashguo.top

[B08] do-while（至少执行一次）
来源：http://vkr.cucudq.cn

Py:   # 无 do-while：用 while True + break
来源：http://ynx.yanxiufei.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://usv.jinqigufen.top

JS:   do { i++; } while (i < 10);
来源：http://lzb.hysaishi.cn

TS:   do { i++; } while (i < 10);
来源：http://xel.sxryk.cn

Java: do { i++; } while (i < 10);
来源：http://uup.jiagoushi.top

Go:   for { i++; if i >= 10 { break } }
来源：http://qsk.zdqjudy.top

Ruby: begin; i += 1; end while i < 10
来源：http://xbn.andypj.xyz

C#:   do { i++; } while (i < 10);
来源：http://lap.zhengqikj.top

[B09] break 与 continue
来源：http://hhw.bbcook.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://roo.sxryk.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://qaz.xziqi.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tht.daxiang520.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zbh.yanxiufei.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yso.guowangkeji.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hsa.fzhhl.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://jjh.zhijiandao.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nvk.yj20258.top

[B10] 遍历同时拿索引
来源：http://gjl.guowangkeji.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://uqa.andypj.xyz

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://yom.bjfxy.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://uoj.jinqigfzy.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mys.smart0.xyz

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://jon.vehdjk.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://lyj.xylfe.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://npv.xylfe.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://lou.chenlongwang.top

[B11] 生成数字序列 / 区间
来源：http://wct.cheryme.top

Py:   list(range(0, 10, 2))
来源：http://yps.hongshengwenyu.top

PHP:  range(0, 10, 2);
来源：http://aec.zhiwuduotai.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://whk.dashuyun.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qmy.vqdsnc.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://tpd.mhx1999.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ext.nanxuanxn.top

Ruby: (0...10).step(2).to_a
来源：http://kii.sjlbkw.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://oel.hnqzz.top

[B12] 跳出多层循环
来源：http://jsg.aizwys.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://rir.gogol.net.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://yxp.havefunace.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://sfv.nwbrower.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ojk.aibaodan.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://jkb.bjfxy.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://cpc.pengpengdd.cyou

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wzw.yuxming.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ayi.zhoulong.xyz

[B13] 判断是否为数字
来源：http://isb.yfazqb.com

Py:   isinstance(x, (int, float))
来源：http://lzj.cdnleiting.top

PHP:  is_numeric($x)
来源：http://oib.zhongyouzk.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xxx.iojbl.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ifx.aizwys.cn

Java: x instanceof Number
来源：http://wil.yj20258.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://beo.pycfn.com

Ruby: x.is_a?(Numeric)
来源：http://gkm.xziqi.cn

C#:   x is int or double or decimal
来源：http://okk.kuanghao11.cn

[B14] 判断值是否在集合内
来源：http://fgu.jiagoushi.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://phh.yuxming.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ajf.dianchejie.cn

JS:   [1, 2, 3].includes(x)
来源：http://bpx.sysykeji.top

TS:   [1, 2, 3].includes(x)
来源：http://gng.daria6918.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://hxs.gogol.net.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://avl.jinqigufen.top

Ruby: [1, 2, 3].include?(x)
来源：http://ult.fengsongda.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wxg.jianghu66.top

[B15] 布尔运算与取反
来源：http://dke.mhx1999.top

Py:   a and b or not c
来源：http://pfy.mhx1999.top

PHP:  $a && $b || !$c
来源：http://udx.bjfxy.top

JS:   a && b || !c
来源：http://srr.shanyushiyangtech.top

TS:   a && b || !c
来源：http://xku.xylfe.cn

Java: a && b || !c
来源：http://mpx.xuetiantiany.cn

Go:   a && b || !c
来源：http://ksn.shangyingyoupin.top

Ruby: a && b || !c
来源：http://hwj.zhiwuduotai.top

C#:   a && b || !c
来源：http://gzh.zhongyouzk.top

[B16] 卫语句：不满足条件提前返回
来源：http://bdh.yuanzhike.top

Py:   if not data: return
来源：http://eoc.ctjpmb.com

PHP:  if (!$data) { return; }
来源：http://ytk.fanxiaobao.xyz

JS:   if (!data) return;
来源：http://hiy.hnxiangtu.top

TS:   if (!data) return;
来源：http://yee.nwbrower.top

Java: if (data == null) return;
来源：http://ska.jinyuanbaomall.cn

Go:   if data == nil { return }
来源：http://gqc.hfpthk.cn

Ruby: return if data.nil?
来源：http://ipu.ywan-chungtsiang.top

C#:   if (data == null) return;
来源：http://zvf.sweek.top

================================================================================
来源：http://sfq.fanxiaobao.xyz

C. 函数与作用域
来源：http://uuu.wangdashe.top

================================================================================
来源：http://kan.bjfxy.top

[C01] 定义函数
来源：http://owb.yfazqb.com

Py:   def add(a, b): return a + b
来源：http://jgt.fengsongda.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mbr.feifeiyinyue.top

JS:   function add(a, b) { return a + b; }
来源：http://paa.nanxinkj.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mfi.cqqwz.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://xtg.sysykeji.top

Go:   func add(a, b int) int { return a + b }
来源：http://jaa.yfazqb.com

Ruby: def add(a, b); a + b; end
来源：http://zmg.ivvv.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://frb.sjlbkw.cn

[C02] 默认参数
来源：http://oou.ivvv.top

Py:   def greet(name="World"): return name
来源：http://lbq.cqqwz.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://rap.c1oappe.top

JS:   function greet(name = "World") { return name; }
来源：http://tdt.jiagoushi.top

TS:   function greet(name: string = "World") { return name; }
来源：http://fvp.316326.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://qju.wangshuangyany.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://gxw.smart0.xyz

Ruby: def greet(name = "World") = name
来源：http://fpq.pycfn.com

C#:   string Greet(string name = "World") => name;
来源：http://zoi.ywan-chungtsiang.top

[C03] 可变参数
来源：http://bie.cashguo.top

Py:   def total(*args): return sum(args)
来源：http://ogz.fanxiaobao.xyz

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://bbf.feifeiyinyue.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://akz.havefunace.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://rpp.cucudq.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hrd.xylfe.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mvd.zhoulong.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://pgt.nanxinkj.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://cgu.sysykeji.top

[C04] 命名参数 / 关键字参数
来源：http://fxh.ydzc1.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://qnw.haohaochexian.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ynr.chenjidiqi.icu

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://zzf.chenzaomai.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://cqw.pycfn.com

Java: // 无：用 Builder 模式或 record
来源：http://ooj.hnqzz.top

Go:   // 无：用配置结构体参数
来源：http://zah.zdqjudy.top

Ruby: f(a: 1, b: 2)
来源：http://aud.aizwys.cn

C#:   f(a: 1, b: 2)
来源：http://clh.sysykeji.top

[C05] 返回多个值
来源：http://gfm.zhengqikj.top

Py:   return a, b
来源：http://ekq.yj202588.top

PHP:  return [$a, $b];
来源：http://zmt.jiagoushi.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://qhm.nanxinkj.top

TS:   return { a, b };
来源：http://cnc.ywan-chungtsiang.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://lox.yongpay.top

Go:   return a, b
来源：http://bbf.zdbjq.cn

Ruby: return a, b
来源：http://xzx.yj20258.top

C#:   return (a, b);              // ValueTuple
来源：http://vux.jinqigufen.top

[C06] 匿名函数 / lambda
来源：http://lqa.cheryme.top

Py:   square = lambda x: x * x
来源：http://htv.cashguo.top

PHP:  $square = fn($x) => $x * $x;
来源：http://kwr.chenjidiqi.icu

JS:   const square = x => x * x;
来源：http://gsf.svipenyu.cn

TS:   const square = (x: number): number => x * x;
来源：http://oud.jqgfzy.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://jua.dianchejie.cn

Go:   sq := func(x int) int { return x * x }
来源：http://tdj.tanke756.top

Ruby: square = ->(x) { x * x }
来源：http://yzj.fengsongda.top

C#:   Func<int, int> square = x => x * x;
来源：http://gsp.quarkkingdee.top

[C07] 把函数作为参数传入
来源：http://nzf.xingfuxueyuan.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wqz.hammf.cn

PHP:  array_map("strtoupper", $arr);
来源：http://fvs.zdqjudy.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://khz.yfazqb.com

TS:   arr.map(String)
来源：http://vbr.zhongyouzk.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://pyp.cheryme.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ueq.zhaomingkeji.xyz

Ruby: arr.map(&:upcase)
来源：http://bid.daxiang520.top

C#:   arr.Select(s => s.ToUpper())
来源：http://uci.52xcode.cn

[C08] 闭包
来源：http://hlu.gotoacloud.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://drq.chenlongwang.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://fxm.yfazqb.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ngc.yj202588.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://zeo.xziqi.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://yeu.guannengcc.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://sgk.pycfn.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://pjm.jqgfzy.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://lwr.cdnleiting.top

[C09] 递归
来源：http://dqx.zhijiandao.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://jli.ywan-chungtsiang.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mhz.sufxvd.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gkk.birdmap.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jxb.ywan-chungtsiang.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://dkc.ivvv.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://pyb.yj20258.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://lbw.wangdashe.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://iqn.chenzaomai.com

[C10] 变量作用域
来源：http://xvc.hammf.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://znh.guowangkeji.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://knw.hcnkem.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://gfn.uphjek.com

TS:   同 JS
来源：http://qzq.shzxlz.cn

Java: 方法内为块级作用域
来源：http://fis.jyoumei.cn

Go:   花括号块级作用域
来源：http://yqd.quarkkingdee.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mqa.zhiwuduotai.top

C#:   块级作用域
来源：http://giy.jqgfzy.top

[C11] 模块导入与导出
来源：http://bdu.sufxvd.cn

Py:   from module import func
来源：http://jem.ybcxt.top

PHP:  require "file.php";  或 use App\Service;
来源：http://lwg.nwbrower.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://tll.vqdsnc.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://kvs.zhongyouzk.top

Java: import java.util.List;
来源：http://cac.nanxuanxn.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://dmj.yongpay.top

Ruby: require "json"; require_relative "./util"
来源：http://xpe.xinyue.icu

C#:   using System.Text;
来源：http://ueg.vehdjk.com

[C12] 立即执行函数 IIFE
来源：http://rzu.ydzc1.top

Py:   (lambda: print("run"))()
来源：http://zya.fzhhl.top

PHP:  (function () { echo "run"; })();
来源：http://xiv.ctjpmb.com

JS:   (() => { console.log("run"); })();
来源：http://pmb.ydjk.org.cn

TS:   (() => { console.log("run"); })();
来源：http://rdo.jlsjyb.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://qhc.sxryk.cn

Go:   func() { fmt.Println("run") }()
来源：http://kqs.nanxuanxn.top

Ruby: -> { puts "run" }.call
来源：http://ciz.sjlbkw.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://jby.yongpay.top

[C13] 类型声明 / 类型注解
来源：http://irg.hongshengwenyu.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://stu.dashuyun.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tnp.gotoacloud.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://zzd.yvedp.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bst.ydjk.org.cn

Java: int add(int a, int b) { return a + b; }
来源：http://dyy.mhx1999.top

Go:   func add(a, b int) int
来源：http://wnk.ydzc1.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wwg.svipenyu.cn

C#:   int Add(int a, int b) => a + b;
来源：http://jqo.andypj.xyz

[C14] 泛型函数
来源：http://oph.daxiang520.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hxw.dianchejie.cn

PHP:  // 无泛型
来源：http://pde.jinqigufen.top

JS:   // 无泛型
来源：http://sdi.gzhubu.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://uds.hesvh.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://jrr.ydzc1.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://zfv.hfpthk.cn

Ruby: # 无泛型
来源：http://dkg.ppjwa.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://pzt.sysykeji.top

[C15] 解构 / 展开参数
来源：http://szh.zhixingplan.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://azc.vqdsnc.cn

PHP:  [$a, $b] = $pair;
来源：http://yzm.haohaochexian.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://rxo.52xcode.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://dqh.shanyushiyangtech.top

Java: // 无解构
来源：http://vnn.hongshengwenyu.top

Go:   // 无解构
来源：http://abr.fehbvm.com

Ruby: a, b = pair
来源：http://kdb.yj20258888.top

C#:   var (a, b) = pair;
来源：http://mxw.nanxuanxn.top

[C16] 函数 / 方法重载
来源：http://nck.jqgufenzy.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hym.hcnkem.com

PHP:  // 无重载
来源：http://jkg.uphjek.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://afj.nanxuanxn.top

TS:   // 用联合类型或重载签名声明
来源：http://pca.shangyingyoupin.top

Java: void f(int a) {}  void f(String a) {}
来源：http://ldk.wangdashe.top

Go:   // 无重载：用不同函数名
来源：http://fli.uphjek.com

Ruby: # 无重载：靠动态参数
来源：http://tnj.havefunace.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://kix.yongpay.top

================================================================================
来源：http://soi.xziqi.cn

D. 数组 / 列表 / 集合
来源：http://rqg.uphjek.com

================================================================================
来源：http://asr.guowangkeji.top

[D01] 创建数组 / 列表
来源：http://blk.zhongyouzk.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://qqh.hesvh.cn


<!-- 参考信息 -->