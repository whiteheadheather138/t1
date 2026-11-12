代发 wailian999

[A26] 类型转换总览
来源：http://jqi.tanke756.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://vnc.hnqzz.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://sti.ivvv.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://epw.uphjek.com

TS:   Number() String() Boolean() x as number
来源：http://yak.zhixingplan.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ous.aibaodan.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://pmc.yanxiufei.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ozt.yj20258888.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ogf.zhijiandao.cn

================================================================================
来源：http://ddd.tianlin.xyz

B. 流程控制
来源：http://gqv.tarul.cn

================================================================================
来源：http://cou.cucudq.cn

[B01] 条件判断 if / else
来源：http://jra.c1oappe.top

Py:   result = "正" if x > 0 else "非正"
来源：http://aeo.316326.xyz

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://afu.shuidangran.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://tyw.cucudq.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://thf.vehdjk.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://rzr.andypj.xyz

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://iut.sxryk.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ryv.tarul.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://woj.gotoacloud.top

[B02] 多分支 else if / elif
来源：http://lci.aibaodan.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://axv.hcnkem.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://lyv.aizwys.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bwm.sweek.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cbc.yueranfly.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xot.xuanzx.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://yvj.tanke756.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ecp.havefunace.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ljn.nwbrower.top

[B03] switch / match / case
来源：http://nsb.cdnleiting.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mca.9152youxi.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ffz.dianchejie.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tra.jinyuanbaomall.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bep.sweek.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://gjn.xziqi.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://fsg.hesvh.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hij.bjfxy.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://pgm.cqqwz.cn

[B04] for 计数循环
来源：http://xww.c1oappe.top

Py:   for i in range(10): print(i)
来源：http://ajw.yongpay.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://lhh.yuanzhike.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fhw.yfazqb.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ufz.zhoulong.xyz

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://udj.gogol.net.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://rcn.quarkkingdee.top

Ruby: 10.times { |i| puts i }
来源：http://jpc.sysykeji.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://lex.tianlin.xyz

[B05] 遍历数组 / 列表
来源：http://sab.tanke756.top

Py:   for item in arr: print(item)
来源：http://pss.shzxlz.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://lhz.cashguo.top

JS:   for (const item of arr) { console.log(item); }
来源：http://xmu.yueranfly.top

TS:   for (const item of arr) { console.log(item); }
来源：http://egf.fzhhl.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://nwe.yanxiufei.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://lol.fzhhl.top

Ruby: arr.each { |item| puts item }
来源：http://jcb.feifeiyinyue.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://uhe.snrcjt.cn

[B06] 遍历字典 / 对象
来源：http://qhy.jianghu66.top

Py:   for k, v in d.items(): print(k, v)
来源：http://yrt.chenjidiqi.icu

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://jvr.jqgfzy.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zgv.kuanghao11.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ctg.haohaochexian.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ady.9152youxi.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://zoi.jinqigfzy.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://nbl.dashuyun.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ffq.yanxiufei.cn

[B07] while 循环
来源：http://rhq.tanke756.top

Py:   while i < 10: i += 1
来源：http://tur.9152youxi.cn

PHP:  while ($i < 10) { $i++; }
来源：http://kuf.nwbrower.top

JS:   while (i < 10) { i++; }
来源：http://zru.jlsjyb.cn

TS:   while (i < 10) { i++; }
来源：http://por.ehwqpu.com

Java: while (i < 10) { i++; }
来源：http://lgj.uphjek.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://rnz.smart0.xyz

Ruby: while i < 10; i += 1; end
来源：http://adv.yongpay.top

C#:   while (i < 10) { i++; }
来源：http://jwg.ydjk.org.cn

[B08] do-while（至少执行一次）
来源：http://zvz.sufxvd.cn

Py:   # 无 do-while：用 while True + break
来源：http://jsc.hywenlv.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://zdc.dashuyun.cn

JS:   do { i++; } while (i < 10);
来源：http://gaj.pycfn.com

TS:   do { i++; } while (i < 10);
来源：http://xee.sweek.top

Java: do { i++; } while (i < 10);
来源：http://dxa.fanxiaobao.xyz

Go:   for { i++; if i >= 10 { break } }
来源：http://ndc.zdqjudy.top

Ruby: begin; i += 1; end while i < 10
来源：http://yvz.sjlbkw.cn

C#:   do { i++; } while (i < 10);
来源：http://mxf.haohaochexian.top

[B09] break 与 continue
来源：http://ooi.ydjk.org.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://maq.pengpengdd.cyou

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ydb.hesvh.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://iuo.fehbvm.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://erx.aizwys.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zdq.52xcode.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://zrv.nanxinkj.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://srx.xuetiantiany.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bnn.sjlbkw.cn

[B10] 遍历同时拿索引
来源：http://huv.zhengqikj.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hhe.sufxvd.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://pes.316326.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://scp.yj202588.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://aid.cqqwz.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://qyx.zycfv.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://rpi.tian-w.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://lfs.tian-w.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://gqg.sxryk.cn

[B11] 生成数字序列 / 区间
来源：http://hzu.jqgufenzy.top

Py:   list(range(0, 10, 2))
来源：http://cyn.meibo888.top

PHP:  range(0, 10, 2);
来源：http://xgn.jlsjyb.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vil.cashguo.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://oqf.jyoumei.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://uxz.meibo888.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ojr.tianlin.xyz

Ruby: (0...10).step(2).to_a
来源：http://mzp.snrcjt.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://cty.smart0.xyz

[B12] 跳出多层循环
来源：http://exg.vqdsnc.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://guk.chenlongwang.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://jha.chenzaomai.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ssh.dianchejie.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ojw.svipenyu.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://sug.ydzc1.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://vuq.hammf.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ked.guannengcc.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mne.andypj.xyz

[B13] 判断是否为数字
来源：http://mdf.zdbjq.cn

Py:   isinstance(x, (int, float))
来源：http://ijp.hammf.cn

PHP:  is_numeric($x)
来源：http://jps.jinqigfzy.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tor.cdnleiting.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ofj.yfazqb.com

Java: x instanceof Number
来源：http://pil.yj20258888.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://jnd.andypj.xyz

Ruby: x.is_a?(Numeric)
来源：http://xbg.shanyushiyangtech.top

C#:   x is int or double or decimal
来源：http://elp.daria6918.cn

[B14] 判断值是否在集合内
来源：http://nbg.svipenyu.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://vra.yvedp.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://vvc.nwbrower.top

JS:   [1, 2, 3].includes(x)
来源：http://mfy.meibo888.top

TS:   [1, 2, 3].includes(x)
来源：http://uae.vehdjk.com

Java: List.of(1, 2, 3).contains(x)
来源：http://lny.aibaodan.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://vtw.hywenlv.cn

Ruby: [1, 2, 3].include?(x)
来源：http://vcf.xingfuxueyuan.xyz

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://aqc.yj20258888.top

[B15] 布尔运算与取反
来源：http://nvq.snrcjt.cn

Py:   a and b or not c
来源：http://jqg.52xcode.cn

PHP:  $a && $b || !$c
来源：http://xli.fzhhl.top

JS:   a && b || !c
来源：http://ehy.sysykeji.top

TS:   a && b || !c
来源：http://duk.daria6918.cn

Java: a && b || !c
来源：http://eav.svipenyu.cn

Go:   a && b || !c
来源：http://djx.epnwcf.com

Ruby: a && b || !c
来源：http://sun.uphjek.com

C#:   a && b || !c
来源：http://wbi.smart0.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://huf.daria6918.cn

Py:   if not data: return
来源：http://txd.ppjwa.cn

PHP:  if (!$data) { return; }
来源：http://tlb.nwbrower.top

JS:   if (!data) return;
来源：http://few.yongpay.top

TS:   if (!data) return;
来源：http://wxs.xziqi.cn

Java: if (data == null) return;
来源：http://jbq.zdbjq.cn

Go:   if data == nil { return }
来源：http://nkz.sufxvd.cn

Ruby: return if data.nil?
来源：http://jmi.zhaomingkeji.xyz

C#:   if (data == null) return;
来源：http://stf.yueranfly.top

================================================================================
来源：http://bno.316326.xyz

C. 函数与作用域
来源：http://efr.fengsongda.top

================================================================================
来源：http://rql.ydzc1.top

[C01] 定义函数
来源：http://ovm.nanxuanxn.top

Py:   def add(a, b): return a + b
来源：http://erb.uphjek.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gdc.zhijiandao.cn

JS:   function add(a, b) { return a + b; }
来源：http://iwb.quarkkingdee.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sfv.yj20258888.top

Java: static int add(int a, int b) { return a + b; }
来源：http://nvr.snrcjt.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ypp.wangshuangyany.cn

Ruby: def add(a, b); a + b; end
来源：http://hpa.zdqjudy.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://xgq.aibaodan.cn

[C02] 默认参数
来源：http://sdk.ctjpmb.com

Py:   def greet(name="World"): return name
来源：http://rzb.jyoumei.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://swu.ivvv.top

JS:   function greet(name = "World") { return name; }
来源：http://lne.jinqigufen.top

TS:   function greet(name: string = "World") { return name; }
来源：http://hda.sufxvd.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://bcj.chenzaomai.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://kpt.fehbvm.com

Ruby: def greet(name = "World") = name
来源：http://abs.smart0.xyz

C#:   string Greet(string name = "World") => name;
来源：http://ikq.jqgufenzy.top

[C03] 可变参数
来源：http://mkz.quarkkingdee.top

Py:   def total(*args): return sum(args)
来源：http://tvl.xingfuxueyuan.xyz

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xuk.iojbl.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://qgj.feifeiyinyue.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://pgj.ydzc1.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://etf.daria6918.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://eys.zhengqikj.top

Ruby: def total(*nums); nums.sum; end
来源：http://heb.pycfn.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://pqk.daria6918.cn

[C04] 命名参数 / 关键字参数
来源：http://ljx.xuanzx.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://iwx.mhx1999.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://vyg.jlsjyb.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://npm.c1oappe.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://qnd.ydzc1.top

Java: // 无：用 Builder 模式或 record
来源：http://azs.hongshengwenyu.top

Go:   // 无：用配置结构体参数
来源：http://jnh.shzxlz.cn

Ruby: f(a: 1, b: 2)
来源：http://muv.vqdsnc.cn

C#:   f(a: 1, b: 2)
来源：http://wls.zhoulong.xyz

[C05] 返回多个值
来源：http://vip.gogol.net.cn

Py:   return a, b
来源：http://kwr.shuidangran.top

PHP:  return [$a, $b];
来源：http://aqw.pycfn.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://jdp.cashguo.top

TS:   return { a, b };
来源：http://rvp.smart0.xyz

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://zbs.chenjidiqi.icu

Go:   return a, b
来源：http://fxj.gogol.net.cn

Ruby: return a, b
来源：http://sii.yj20258.top

C#:   return (a, b);              // ValueTuple
来源：http://hsp.bjfxy.top

[C06] 匿名函数 / lambda
来源：http://aug.zhoulong.xyz

Py:   square = lambda x: x * x
来源：http://kov.meibo888.top

PHP:  $square = fn($x) => $x * $x;
来源：http://xzj.zdbjq.cn

JS:   const square = x => x * x;
来源：http://mah.cucudq.cn

TS:   const square = (x: number): number => x * x;
来源：http://bhs.hnqzz.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://pzb.zhongyouzk.top

Go:   sq := func(x int) int { return x * x }
来源：http://ksr.shanyushiyangtech.top

Ruby: square = ->(x) { x * x }
来源：http://ulz.ivvv.top

C#:   Func<int, int> square = x => x * x;
来源：http://jgr.jinqigufen.top

[C07] 把函数作为参数传入
来源：http://qsa.smart0.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hsk.meibo888.top

PHP:  array_map("strtoupper", $arr);
来源：http://kfz.epnwcf.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://imd.zhijiandao.cn

TS:   arr.map(String)
来源：http://osb.c1oappe.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://llf.aibaodan.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://jfn.chenlongwang.top

Ruby: arr.map(&:upcase)
来源：http://jny.cqqwz.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://qdp.gotoacloud.top

[C08] 闭包
来源：http://gpl.jqgufenzy.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://nqn.xingfuxueyuan.xyz

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://bfx.jqgufenzy.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mss.jinqigufen.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://cdp.tarul.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://avu.mhx1999.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://eop.bjfxy.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://nkc.iojbl.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://vmt.jqgufenzy.top

[C09] 递归
来源：http://qua.xingfuxueyuan.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://kqy.jinghuilouyu.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://jbb.sjlbkw.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pyv.shanyushiyangtech.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://axj.9152youxi.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://bnm.zhijiandao.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://obk.chenjidiqi.icu

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://bxy.tanke756.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://xls.ivvv.top

[C10] 变量作用域
来源：http://gyk.c1oappe.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://zrl.zhoulong.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://igb.yj202588.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wih.hnxiangtu.top

TS:   同 JS
来源：http://frc.yanxiufei.cn

Java: 方法内为块级作用域
来源：http://rzc.redwolf501.top

Go:   花括号块级作用域
来源：http://djp.redwolf501.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://deg.quarkkingdee.top

C#:   块级作用域
来源：http://jwa.jinqigfzy.top

[C11] 模块导入与导出
来源：http://uyn.ydzc1.top

Py:   from module import func
来源：http://lwr.fehbvm.com

PHP:  require "file.php";  或 use App\Service;
来源：http://slt.mhx1999.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://amz.feifeiyinyue.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://uit.fengsongda.top

Java: import java.util.List;
来源：http://voh.yongpay.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mhi.uphjek.com

Ruby: require "json"; require_relative "./util"
来源：http://ogm.sjlbkw.cn

C#:   using System.Text;
来源：http://vws.jianghu66.top

[C12] 立即执行函数 IIFE
来源：http://zcm.aibaodan.cn

Py:   (lambda: print("run"))()
来源：http://suy.wangdashe.top

PHP:  (function () { echo "run"; })();
来源：http://iqh.52xcode.cn

JS:   (() => { console.log("run"); })();
来源：http://whz.svipenyu.cn

TS:   (() => { console.log("run"); })();
来源：http://brg.chenzaomai.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://zuv.aibaodan.cn

Go:   func() { fmt.Println("run") }()
来源：http://cag.ybcxt.top

Ruby: -> { puts "run" }.call
来源：http://bds.jlsjyb.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://qml.yuanzhike.top

[C13] 类型声明 / 类型注解
来源：http://ghj.pycfn.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://sjg.snrcjt.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ubi.yj20258888.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://owe.tian-w.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://loz.zhijiandao.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ohh.zhixingplan.top

Go:   func add(a, b int) int
来源：http://whp.9152youxi.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://bud.jinqigufen.top

C#:   int Add(int a, int b) => a + b;
来源：http://ezi.52xcode.cn

[C14] 泛型函数
来源：http://pya.jinghuilouyu.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://pql.nanxuanxn.top

PHP:  // 无泛型
来源：http://mvr.cucudq.cn

JS:   // 无泛型
来源：http://zfj.yueranfly.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://dio.xylfe.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://eym.zhixingplan.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://qlx.ydjk.org.cn

Ruby: # 无泛型
来源：http://vfn.yj20258.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://tjr.dashuyun.cn

[C15] 解构 / 展开参数
来源：http://esy.hywenlv.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://gut.zdqjudy.top

PHP:  [$a, $b] = $pair;
来源：http://pbs.hnxiangtu.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wnx.jqgufenzy.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://lua.hongshengwenyu.top

Java: // 无解构
来源：http://pak.zhoulong.xyz

Go:   // 无解构
来源：http://yyy.wangdashe.top

Ruby: a, b = pair
来源：http://rmd.haohaochexian.top

C#:   var (a, b) = pair;
来源：http://jeq.gaohongyu789.top

[C16] 函数 / 方法重载
来源：http://hlk.hongshengwenyu.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wbu.svipenyu.cn

PHP:  // 无重载
来源：http://atu.yongpay.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://wja.pengpengdd.cyou

TS:   // 用联合类型或重载签名声明
来源：http://ivv.ctjpmb.com

Java: void f(int a) {}  void f(String a) {}
来源：http://osn.fzhhl.top


<!-- 参考信息 -->