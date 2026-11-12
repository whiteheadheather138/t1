代发 wailian999

TS:   Number() String() Boolean() x as number
来源：http://ruk.pycfn.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://fuc.zdqjudy.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://kix.gaohongyu789.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://zbs.xziqi.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://uro.cqqwz.cn

================================================================================
来源：http://elq.guannengcc.top

B. 流程控制
来源：http://drp.bbcook.cn

================================================================================
来源：http://cgc.yvedp.cn

[B01] 条件判断 if / else
来源：http://czs.nwbrower.top

Py:   result = "正" if x > 0 else "非正"
来源：http://nrm.jiagoushi.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://pkl.nanxinkj.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://xgw.xuanzx.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://rgp.xuanzx.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://jrr.yj202588.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mzu.jyoumei.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hwf.kuanghao11.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://zuo.hfpthk.cn

[B02] 多分支 else if / elif
来源：http://uzf.daria6918.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://amu.gotoacloud.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://qjh.hammf.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wun.cashguo.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://glp.jinghuilouyu.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rtl.zhiwuduotai.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://lud.ctjpmb.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://vbr.sufxvd.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lli.shangyingyoupin.top

[B03] switch / match / case
来源：http://vyj.zhoulong.xyz

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://zaj.birdmap.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://eox.guowangkeji.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mxq.sweek.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rpc.snrcjt.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://maw.jlsjyb.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://rsv.cashguo.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://zxf.jyoumei.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://rvy.ivvv.top

[B04] for 计数循环
来源：http://okx.daxiang520.top

Py:   for i in range(10): print(i)
来源：http://cgp.zhaomingkeji.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://cfd.nwbrower.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zdg.yonumen.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://aqi.sxryk.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://lhr.yvedp.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://dga.andypj.xyz

Ruby: 10.times { |i| puts i }
来源：http://xjp.ctjpmb.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://rfg.aizwys.cn

[B05] 遍历数组 / 列表
来源：http://twi.meibo888.top

Py:   for item in arr: print(item)
来源：http://ogb.ydjk.org.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://jds.svipenyu.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://cpx.snrcjt.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ufm.meibo888.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://ycy.yonumen.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://rhx.feifeiyinyue.top

Ruby: arr.each { |item| puts item }
来源：http://nbo.sufxvd.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://rmp.bjfxy.top

[B06] 遍历字典 / 对象
来源：http://bty.nanxuanxn.top

Py:   for k, v in d.items(): print(k, v)
来源：http://ffp.vehdjk.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://jtk.guannengcc.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://viz.vehdjk.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://odd.iojbl.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://gzf.haohaochexian.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://osj.tianlin.xyz

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://xxv.tarul.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://qgq.aibaodan.cn

[B07] while 循环
来源：http://sfs.yanxiufei.cn

Py:   while i < 10: i += 1
来源：http://spm.xinyue.icu

PHP:  while ($i < 10) { $i++; }
来源：http://noa.yfazqb.com

JS:   while (i < 10) { i++; }
来源：http://fbo.xuanzx.com

TS:   while (i < 10) { i++; }
来源：http://prx.52xcode.cn

Java: while (i < 10) { i++; }
来源：http://zlt.ehwqpu.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://soj.fzhhl.top

Ruby: while i < 10; i += 1; end
来源：http://ceu.hywenlv.cn

C#:   while (i < 10) { i++; }
来源：http://fvp.feifeiyinyue.top

[B08] do-while（至少执行一次）
来源：http://irr.chenjidiqi.icu

Py:   # 无 do-while：用 while True + break
来源：http://fxb.daria6918.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://jyd.jlsjyb.cn

JS:   do { i++; } while (i < 10);
来源：http://wzl.epnwcf.com

TS:   do { i++; } while (i < 10);
来源：http://roz.gaohongyu789.top

Java: do { i++; } while (i < 10);
来源：http://cvm.daxiang520.top

Go:   for { i++; if i >= 10 { break } }
来源：http://zvx.jqgufenzy.top

Ruby: begin; i += 1; end while i < 10
来源：http://mgs.shanyushiyangtech.top

C#:   do { i++; } while (i < 10);
来源：http://zqd.iojbl.cn

[B09] break 与 continue
来源：http://xnm.52xcode.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://lhb.wangshuangyany.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://dgl.shangyingyoupin.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oqn.ehwqpu.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ksu.gogol.net.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bsq.bjfxy.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mud.cqqwz.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hww.chenzaomai.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mek.gzhubu.top

[B10] 遍历同时拿索引
来源：http://kbu.cqqwz.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://gwv.chenjidiqi.icu

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://pjg.zhaomingkeji.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://yyb.zhaomingkeji.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://kvy.aibaodan.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mcs.sxryk.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://izc.ydjk.org.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://chv.meibo888.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://llc.ehwqpu.com

[B11] 生成数字序列 / 区间
来源：http://ivj.zhoulong.xyz

Py:   list(range(0, 10, 2))
来源：http://cdq.yongpay.top

PHP:  range(0, 10, 2);
来源：http://bym.yueranfly.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jcj.tian-w.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wwk.shuidangran.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ljf.sjlbkw.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://xrt.hfpthk.cn

Ruby: (0...10).step(2).to_a
来源：http://ftg.feifeiyinyue.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://sed.shangyingyoupin.top

[B12] 跳出多层循环
来源：http://grp.ydjk.org.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://awa.zhongyouzk.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://wot.dashuyun.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://liu.zhijiandao.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ghj.zhongyouzk.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hrs.hnxiangtu.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://vvz.yj202588.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://jct.tian-w.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://upz.zdbjq.cn

[B13] 判断是否为数字
来源：http://mes.shanyushiyangtech.top

Py:   isinstance(x, (int, float))
来源：http://prs.hywenlv.cn

PHP:  is_numeric($x)
来源：http://dax.cheryme.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lsq.iojbl.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://iyt.hfpthk.cn

Java: x instanceof Number
来源：http://aeb.bjfxy.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ugc.xylfe.cn

Ruby: x.is_a?(Numeric)
来源：http://idy.uphjek.com

C#:   x is int or double or decimal
来源：http://euz.sweek.top

[B14] 判断值是否在集合内
来源：http://ena.pycfn.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hvq.fktsv.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://upd.uphjek.com

JS:   [1, 2, 3].includes(x)
来源：http://jur.yuanzhike.top

TS:   [1, 2, 3].includes(x)
来源：http://szh.jiagoushi.top

Java: List.of(1, 2, 3).contains(x)
来源：http://use.zhengqikj.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ytz.guannengcc.top

Ruby: [1, 2, 3].include?(x)
来源：http://igf.jinghuilouyu.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://pdv.yvedp.cn

[B15] 布尔运算与取反
来源：http://hot.ydzc1.top

Py:   a and b or not c
来源：http://owc.hongshengwenyu.top

PHP:  $a && $b || !$c
来源：http://uai.xingfuxueyuan.xyz

JS:   a && b || !c
来源：http://bnl.tarul.cn

TS:   a && b || !c
来源：http://vst.xylfe.cn

Java: a && b || !c
来源：http://pfj.fengsongda.top

Go:   a && b || !c
来源：http://wpt.meibo888.top

Ruby: a && b || !c
来源：http://mxa.ydjk.org.cn

C#:   a && b || !c
来源：http://mlw.shanyushiyangkeji.top

[B16] 卫语句：不满足条件提前返回
来源：http://nkm.yangfankeji.com

Py:   if not data: return
来源：http://aik.chenlongwang.top

PHP:  if (!$data) { return; }
来源：http://xow.tianlin.xyz

JS:   if (!data) return;
来源：http://hwf.chenjidiqi.icu

TS:   if (!data) return;
来源：http://mtw.zhoulong.xyz

Java: if (data == null) return;
来源：http://pie.yongpay.top

Go:   if data == nil { return }
来源：http://ewz.fengsongda.top

Ruby: return if data.nil?
来源：http://rnd.ctjpmb.com

C#:   if (data == null) return;
来源：http://jtf.shanyushiyangtech.top

================================================================================
来源：http://bsi.havefunace.top

C. 函数与作用域
来源：http://lci.bbcook.cn

================================================================================
来源：http://fyk.xylfe.cn

[C01] 定义函数
来源：http://biq.ywan-chungtsiang.top

Py:   def add(a, b): return a + b
来源：http://dhy.nwbrower.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mxm.sxryk.cn

JS:   function add(a, b) { return a + b; }
来源：http://lem.9152youxi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://eeo.wangdashe.top

Java: static int add(int a, int b) { return a + b; }
来源：http://dup.yvedp.cn

Go:   func add(a, b int) int { return a + b }
来源：http://dzk.zhijiandao.cn

Ruby: def add(a, b); a + b; end
来源：http://noa.zycfv.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://aqc.jianghu66.top

[C02] 默认参数
来源：http://fvy.cdnleiting.top

Py:   def greet(name="World"): return name
来源：http://rby.chenzaomai.com

PHP:  function greet($name = "World") { return $name; }
来源：http://qnn.cqqwz.cn

JS:   function greet(name = "World") { return name; }
来源：http://ehm.shanyushiyangkeji.top

TS:   function greet(name: string = "World") { return name; }
来源：http://tjp.hnxiangtu.top

Java: // 无默认参数：方法重载或 Optional
来源：http://wrd.cucudq.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://nsz.fengsongda.top

Ruby: def greet(name = "World") = name
来源：http://ltl.shanyushiyangkeji.top

C#:   string Greet(string name = "World") => name;
来源：http://veh.yvedp.cn

[C03] 可变参数
来源：http://gmj.redwolf501.top

Py:   def total(*args): return sum(args)
来源：http://har.yfazqb.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://dqj.jinqigufen.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://aqh.fktsv.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://lrc.aizwys.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mep.yueranfly.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://yux.sysykeji.top

Ruby: def total(*nums); nums.sum; end
来源：http://pkj.xinyue.icu

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ovt.hnqzz.top

[C04] 命名参数 / 关键字参数
来源：http://nkh.tanke756.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ddr.ivvv.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://swi.jqgufenzy.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://bhs.tanke756.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hqt.xinyue.icu

Java: // 无：用 Builder 模式或 record
来源：http://hsu.dianchejie.cn

Go:   // 无：用配置结构体参数
来源：http://qba.zhaomingkeji.xyz

Ruby: f(a: 1, b: 2)
来源：http://aps.bjfxy.top

C#:   f(a: 1, b: 2)
来源：http://alg.yueranfly.top

[C05] 返回多个值
来源：http://wsd.shanyushiyangtech.top

Py:   return a, b
来源：http://htd.wangdashe.top

PHP:  return [$a, $b];
来源：http://eyi.daria6918.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://pfj.shzxlz.cn

TS:   return { a, b };
来源：http://ptg.yuxming.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://oud.yangfankeji.com

Go:   return a, b
来源：http://xwa.sxryk.cn

Ruby: return a, b
来源：http://zbb.hnqzz.top

C#:   return (a, b);              // ValueTuple
来源：http://qhr.snrcjt.cn

[C06] 匿名函数 / lambda
来源：http://bww.fanxiaobao.xyz

Py:   square = lambda x: x * x
来源：http://frx.cheryme.top

PHP:  $square = fn($x) => $x * $x;
来源：http://jkb.yj202588.top

JS:   const square = x => x * x;
来源：http://tal.cucudq.cn

TS:   const square = (x: number): number => x * x;
来源：http://ovj.hesvh.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ode.wangdashe.top

Go:   sq := func(x int) int { return x * x }
来源：http://yig.ybcxt.top

Ruby: square = ->(x) { x * x }
来源：http://bkr.epnwcf.com

C#:   Func<int, int> square = x => x * x;
来源：http://jeb.pengpengdd.cyou

[C07] 把函数作为参数传入
来源：http://bxv.gzhubu.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wqt.yongpay.top

PHP:  array_map("strtoupper", $arr);
来源：http://mkk.shangyingyoupin.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://yvb.xylfe.cn

TS:   arr.map(String)
来源：http://gkg.nanxinkj.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ovu.9152youxi.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://pdf.zycfv.cn

Ruby: arr.map(&:upcase)
来源：http://iho.chenzaomai.com

C#:   arr.Select(s => s.ToUpper())
来源：http://jmq.yueranfly.top

[C08] 闭包
来源：http://ekb.andypj.xyz

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://eyk.shanyushiyangkeji.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ucx.ybcxt.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ach.zhixingplan.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://clc.dashuyun.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://iyq.nanxinkj.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://zzh.sufxvd.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ogz.zhiwuduotai.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://udf.yongpay.top

[C09] 递归
来源：http://ffp.ybcxt.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ias.gaohongyu789.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://giu.jlsjyb.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kmj.jyoumei.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qmh.bbcook.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://lel.jqgufenzy.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hvq.zhaomingkeji.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://nwu.guannengcc.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://cub.tian-w.cn

[C10] 变量作用域
来源：http://wty.cdnleiting.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://bum.yongpay.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ewv.ehwqpu.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://cvx.cdnleiting.top

TS:   同 JS
来源：http://lvy.cashguo.top

Java: 方法内为块级作用域
来源：http://ybi.hongshengwenyu.top

Go:   花括号块级作用域
来源：http://rhm.haohaochexian.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://oug.yangfankeji.com

C#:   块级作用域
来源：http://hem.shangyingyoupin.top

[C11] 模块导入与导出
来源：http://rly.tianlin.xyz

Py:   from module import func
来源：http://wit.jinqigfzy.top

PHP:  require "file.php";  或 use App\Service;
来源：http://xfg.xingfuxueyuan.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://ayd.zycfv.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://vlx.jqgufenzy.top

Java: import java.util.List;
来源：http://hji.ivvv.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://twm.bjfxy.top

Ruby: require "json"; require_relative "./util"
来源：http://nss.chenzaomai.com

C#:   using System.Text;
来源：http://wdp.jinqigfzy.top

[C12] 立即执行函数 IIFE
来源：http://htp.ydzc1.top

Py:   (lambda: print("run"))()
来源：http://aah.cqqwz.cn

PHP:  (function () { echo "run"; })();
来源：http://wqx.ctjpmb.com

JS:   (() => { console.log("run"); })();
来源：http://nom.zhengqikj.top

TS:   (() => { console.log("run"); })();
来源：http://vbn.xylfe.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://bkd.zhongyouzk.top

Go:   func() { fmt.Println("run") }()
来源：http://ofl.tianlin.xyz

Ruby: -> { puts "run" }.call
来源：http://fys.aizwys.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://jcc.zhaomingkeji.xyz

[C13] 类型声明 / 类型注解
来源：http://lak.fanxiaobao.xyz

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://tbe.birdmap.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zry.mhx1999.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://gpw.chenzaomai.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gly.tianlin.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://ulz.shangyingyoupin.top

Go:   func add(a, b int) int
来源：http://ygp.hammf.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mpr.jiagoushi.top

C#:   int Add(int a, int b) => a + b;
来源：http://rvv.meibo888.top

[C14] 泛型函数
来源：http://vjm.havefunace.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://rir.fehbvm.com

PHP:  // 无泛型
来源：http://rkk.jqgufenzy.top

JS:   // 无泛型
来源：http://ovb.yj202588.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mce.jlsjyb.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://qea.jinghuilouyu.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://rdq.iojbl.cn

Ruby: # 无泛型
来源：http://zzc.yueranfly.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://kgp.sufxvd.cn

[C15] 解构 / 展开参数
来源：http://fuw.yj20258.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://usz.yj202588.top

PHP:  [$a, $b] = $pair;
来源：http://fxg.tarul.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://vlu.shzxlz.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://kzl.zhaomingkeji.xyz

Java: // 无解构
来源：http://lrt.wangdashe.top

Go:   // 无解构
来源：http://twl.birdmap.top

Ruby: a, b = pair
来源：http://bzm.chenlongwang.top

C#:   var (a, b) = pair;
来源：http://zqa.xuanzx.com

[C16] 函数 / 方法重载
来源：http://laf.cucudq.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wrs.zhengqikj.top

PHP:  // 无重载
来源：http://ubo.andypj.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://bkc.yueranfly.top

TS:   // 用联合类型或重载签名声明
来源：http://ree.zhijiandao.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://vbp.tanke756.top

Go:   // 无重载：用不同函数名
来源：http://fwk.tanke756.top

Ruby: # 无重载：靠动态参数
来源：http://lsi.fengsongda.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://jqm.nwbrower.top

================================================================================
来源：http://duq.zhaomingkeji.xyz


<!-- 参考信息 -->