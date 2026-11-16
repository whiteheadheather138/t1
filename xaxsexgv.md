代发 wailian999

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://gjs.sweek.top

================================================================================
来源：http://jdu.xuanzx.com

B. 流程控制
来源：http://mci.daria6918.cn

================================================================================
来源：http://qit.jinghuilouyu.cn

[B01] 条件判断 if / else
来源：http://guw.yuxming.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://rih.yonumen.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://imm.0kj1m.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ecz.wangshuangyany.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://tgn.tarul.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://lvk.chenzaomai.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://yoi.nanxinkj.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://oqg.fanxiaobao.xyz

C#:   var r = x > 0 ? "正" : "非正";
来源：http://zbx.cashguo.top

[B02] 多分支 else if / elif
来源：http://qcg.ybcxt.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://tdr.xuanzx.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mmh.cucudq.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://khd.aizwys.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hjj.zhaomingkeji.xyz

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nbj.quarkkingdee.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://fhc.aibaodan.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://zzx.zycfv.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vds.jlsjyb.cn

[B03] switch / match / case
来源：http://gha.tarul.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://zwj.aizwys.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ccz.xuanzx.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fjr.gzhubu.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bhe.xinyue.icu

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://bqx.chenzaomai.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://fys.wangdashe.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://zjo.jinqigfzy.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wht.feifeiyinyue.top

[B04] for 计数循环
来源：http://evw.guannengcc.top

Py:   for i in range(10): print(i)
来源：http://nzo.hfpthk.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://bzt.yuanzhike.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hgh.xylfe.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://imd.yvedp.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hvl.tian-w.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://stv.yj202588.top

Ruby: 10.times { |i| puts i }
来源：http://kir.nwbrower.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://fnw.guowangkeji.top

[B05] 遍历数组 / 列表
来源：http://qnr.zhijiandao.cn

Py:   for item in arr: print(item)
来源：http://gzs.hcnkem.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://fuq.hcnkem.com

JS:   for (const item of arr) { console.log(item); }
来源：http://pld.iojbl.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://yos.tarul.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://dpz.ybcxt.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hws.316326.xyz

Ruby: arr.each { |item| puts item }
来源：http://epr.dashuyun.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://cpx.cdnleiting.top

[B06] 遍历字典 / 对象
来源：http://qdd.sxryk.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://rss.yuxming.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://sus.vqdsnc.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lyc.sjlbkw.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bsc.zycfv.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://nwy.ydjk.org.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://lat.gotoacloud.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hsj.sysykeji.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://yxo.52xcode.cn

[B07] while 循环
来源：http://oxk.tian-w.cn

Py:   while i < 10: i += 1
来源：http://zwv.zhoulong.xyz

PHP:  while ($i < 10) { $i++; }
来源：http://str.nanxinkj.top

JS:   while (i < 10) { i++; }
来源：http://dsa.c1oappe.top

TS:   while (i < 10) { i++; }
来源：http://lwq.cdnleiting.top

Java: while (i < 10) { i++; }
来源：http://nus.hongshengwenyu.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ebw.yfazqb.com

Ruby: while i < 10; i += 1; end
来源：http://cdf.yuanzhike.top

C#:   while (i < 10) { i++; }
来源：http://mee.yvedp.cn

[B08] do-while（至少执行一次）
来源：http://ifr.ydjk.org.cn

Py:   # 无 do-while：用 while True + break
来源：http://fls.zycfv.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://tii.fanxiaobao.xyz

JS:   do { i++; } while (i < 10);
来源：http://lrv.tianlin.xyz

TS:   do { i++; } while (i < 10);
来源：http://xkd.hesvh.cn

Java: do { i++; } while (i < 10);
来源：http://udm.svipenyu.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://fbo.fanxiaobao.xyz

Ruby: begin; i += 1; end while i < 10
来源：http://fpc.wangshuangyany.cn

C#:   do { i++; } while (i < 10);
来源：http://yue.nanxuanxn.top

[B09] break 与 continue
来源：http://qyj.zhixingplan.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://nom.hammf.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mwq.chenzaomai.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wwc.redwolf501.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://umr.fanxiaobao.xyz

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xdh.chenlongwang.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://qae.sysykeji.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://anq.nwbrower.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://upk.shuidangran.top

[B10] 遍历同时拿索引
来源：http://ije.hfpthk.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://xhb.yonumen.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://vnp.hcnkem.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://usf.ctjpmb.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hew.ydzc1.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hbm.hesvh.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wbq.wangdashe.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://qxa.shangyingyoupin.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://xwb.dianchejie.cn

[B11] 生成数字序列 / 区间
来源：http://mpp.kuanghao11.cn

Py:   list(range(0, 10, 2))
来源：http://rjw.shuidangran.top

PHP:  range(0, 10, 2);
来源：http://fgr.zhengqikj.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://opv.ppjwa.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xez.zhengqikj.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://aas.pengpengdd.cyou

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://tur.chenzaomai.com

Ruby: (0...10).step(2).to_a
来源：http://fhe.9152youxi.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ndv.cheryme.top

[B12] 跳出多层循环
来源：http://zay.dashuyun.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://vtk.shangyingyoupin.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://usm.nwbrower.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://bgb.sweek.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://gol.pycfn.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://cos.shangyingyoupin.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://uso.tanke756.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://nnh.andypj.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://fbl.zhijiandao.cn

[B13] 判断是否为数字
来源：http://fpw.hnxiangtu.top

Py:   isinstance(x, (int, float))
来源：http://hxh.daxiang520.top

PHP:  is_numeric($x)
来源：http://gfg.yuanzhike.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dmu.yongpay.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://htc.fengsongda.top

Java: x instanceof Number
来源：http://zcd.cdnleiting.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://fad.uphjek.com

Ruby: x.is_a?(Numeric)
来源：http://hxa.cheryme.top

C#:   x is int or double or decimal
来源：http://mrm.jlsjyb.cn

[B14] 判断值是否在集合内
来源：http://fwf.cheryme.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ymg.yj20258888.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://evf.vqdsnc.cn

JS:   [1, 2, 3].includes(x)
来源：http://qgc.mhx1999.top

TS:   [1, 2, 3].includes(x)
来源：http://bbb.tarul.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://kft.jinqigfzy.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://uil.hywenlv.cn

Ruby: [1, 2, 3].include?(x)
来源：http://bbc.zhiwuduotai.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://zkz.mhx1999.top

[B15] 布尔运算与取反
来源：http://feu.yangfankeji.com

Py:   a and b or not c
来源：http://dxy.nanxinkj.top

PHP:  $a && $b || !$c
来源：http://wsu.quarkkingdee.top

JS:   a && b || !c
来源：http://vtb.sysykeji.top

TS:   a && b || !c
来源：http://qmu.epnwcf.com

Java: a && b || !c
来源：http://ksq.jlsjyb.cn

Go:   a && b || !c
来源：http://raf.dashuyun.cn

Ruby: a && b || !c
来源：http://mwz.shzxlz.cn

C#:   a && b || !c
来源：http://zgs.feifeiyinyue.top

[B16] 卫语句：不满足条件提前返回
来源：http://oed.fzhhl.top

Py:   if not data: return
来源：http://fta.yonumen.top

PHP:  if (!$data) { return; }
来源：http://rzv.nanxuanxn.top

JS:   if (!data) return;
来源：http://xlv.epnwcf.com

TS:   if (!data) return;
来源：http://qck.jinqigfzy.top

Java: if (data == null) return;
来源：http://mmu.shzxlz.cn

Go:   if data == nil { return }
来源：http://zku.fehbvm.com

Ruby: return if data.nil?
来源：http://yqc.yueranfly.top

C#:   if (data == null) return;
来源：http://qcu.fehbvm.com

================================================================================
来源：http://ies.yueranfly.top

C. 函数与作用域
来源：http://aiu.jinqigufen.top

================================================================================
来源：http://twt.smart0.xyz

[C01] 定义函数
来源：http://sjy.xinyue.icu

Py:   def add(a, b): return a + b
来源：http://brf.hnxiangtu.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ojj.sweek.top

JS:   function add(a, b) { return a + b; }
来源：http://oxo.cheryme.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://plq.pycfn.com

Java: static int add(int a, int b) { return a + b; }
来源：http://elr.guannengcc.top

Go:   func add(a, b int) int { return a + b }
来源：http://sit.birdmap.top

Ruby: def add(a, b); a + b; end
来源：http://aim.bbcook.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://xfb.yueranfly.top

[C02] 默认参数
来源：http://pss.svipenyu.cn

Py:   def greet(name="World"): return name
来源：http://biv.zhaomingkeji.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://cuv.snrcjt.cn

JS:   function greet(name = "World") { return name; }
来源：http://lmw.zhijiandao.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://gtn.xuanzx.com

Java: // 无默认参数：方法重载或 Optional
来源：http://qeh.jyoumei.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://xyl.fanxiaobao.xyz

Ruby: def greet(name = "World") = name
来源：http://sru.c1oappe.top

C#:   string Greet(string name = "World") => name;
来源：http://fyb.zdqjudy.top

[C03] 可变参数
来源：http://svs.c1oappe.top

Py:   def total(*args): return sum(args)
来源：http://oox.daria6918.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://aeq.jqgfzy.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://fdk.shuidangran.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://dlc.havefunace.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://pxa.xylfe.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://fww.ivvv.top

Ruby: def total(*nums); nums.sum; end
来源：http://hzv.zhixingplan.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ume.dashuyun.cn

[C04] 命名参数 / 关键字参数
来源：http://vvv.andypj.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://eie.guowangkeji.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://uot.sweek.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://rcf.hywenlv.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://rhg.cashguo.top

Java: // 无：用 Builder 模式或 record
来源：http://jnl.daxiang520.top

Go:   // 无：用配置结构体参数
来源：http://ycl.316326.xyz

Ruby: f(a: 1, b: 2)
来源：http://pmn.yonumen.top

C#:   f(a: 1, b: 2)
来源：http://ppw.tanke756.top

[C05] 返回多个值
来源：http://cjw.redwolf501.top

Py:   return a, b
来源：http://ojn.316326.xyz

PHP:  return [$a, $b];
来源：http://srh.tarul.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://gxs.yj202588.top

TS:   return { a, b };
来源：http://lgm.tanke756.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://sue.jinqigufen.top

Go:   return a, b
来源：http://hxn.wangshuangyany.cn

Ruby: return a, b
来源：http://yvh.hesvh.cn

C#:   return (a, b);              // ValueTuple
来源：http://ptb.zhixingplan.top

[C06] 匿名函数 / lambda
来源：http://gzh.sjlbkw.cn

Py:   square = lambda x: x * x
来源：http://ybk.zhixingplan.top

PHP:  $square = fn($x) => $x * $x;
来源：http://vxh.vehdjk.com

JS:   const square = x => x * x;
来源：http://knv.jqgfzy.top

TS:   const square = (x: number): number => x * x;
来源：http://vnh.yj20258888.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://pgs.fehbvm.com

Go:   sq := func(x int) int { return x * x }
来源：http://olz.ehwqpu.com

Ruby: square = ->(x) { x * x }
来源：http://kxt.andypj.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://rrv.jqgufenzy.top

[C07] 把函数作为参数传入
来源：http://yds.sweek.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://yda.hywenlv.cn

PHP:  array_map("strtoupper", $arr);
来源：http://hsx.cdnleiting.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xiz.chenlongwang.top

TS:   arr.map(String)
来源：http://wox.svipenyu.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://fct.gaohongyu789.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://yzl.uphjek.com

Ruby: arr.map(&:upcase)
来源：http://afq.epnwcf.com

C#:   arr.Select(s => s.ToUpper())
来源：http://jnf.birdmap.top

[C08] 闭包
来源：http://vfc.yuanzhike.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://fne.mhx1999.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://fyu.shuidangran.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://gxr.ybcxt.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://tmk.zhengqikj.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://reb.hnqzz.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://bbz.jinqigufen.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://gdf.guowangkeji.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://apw.aizwys.cn

[C09] 递归
来源：http://ura.shanyushiyangkeji.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://xvp.cashguo.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://rck.tian-w.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nhd.wangdashe.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ges.jinyuanbaomall.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://eqn.guannengcc.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://aau.ehwqpu.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://zau.chenjidiqi.icu

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://myj.dashuyun.cn

[C10] 变量作用域
来源：http://mya.zhengqikj.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://kom.smart0.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://xwv.yuxming.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://lmn.guowangkeji.top

TS:   同 JS
来源：http://iko.meibo888.top

Java: 方法内为块级作用域
来源：http://bor.jiagoushi.top

Go:   花括号块级作用域
来源：http://lal.fzhhl.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wfu.yj20258888.top

C#:   块级作用域
来源：http://gis.shanyushiyangkeji.top

[C11] 模块导入与导出
来源：http://prp.wangshuangyany.cn

Py:   from module import func
来源：http://vqk.zhixingplan.top

PHP:  require "file.php";  或 use App\Service;
来源：http://xmm.fehbvm.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://vbx.sysykeji.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://toa.cqqwz.cn

Java: import java.util.List;
来源：http://sck.zhaomingkeji.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://phm.jyoumei.cn

Ruby: require "json"; require_relative "./util"
来源：http://vvn.jqgfzy.top

C#:   using System.Text;
来源：http://uxr.hongshengwenyu.top

[C12] 立即执行函数 IIFE
来源：http://kxz.gaohongyu789.top

Py:   (lambda: print("run"))()
来源：http://unj.daria6918.cn

PHP:  (function () { echo "run"; })();
来源：http://bow.yvedp.cn

JS:   (() => { console.log("run"); })();
来源：http://dor.shzxlz.cn

TS:   (() => { console.log("run"); })();
来源：http://vzm.haohaochexian.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://xgb.guannengcc.top

Go:   func() { fmt.Println("run") }()
来源：http://nzu.birdmap.top

Ruby: -> { puts "run" }.call
来源：http://klt.redwolf501.top

C#:   // 无 IIFE：用静态构造函数
来源：http://blc.dianchejie.cn

[C13] 类型声明 / 类型注解
来源：http://odr.andypj.xyz

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://uzo.cqqwz.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lnt.snrcjt.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://gyb.yuxming.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hok.jiagoushi.top

Java: int add(int a, int b) { return a + b; }
来源：http://vrt.shanyushiyangkeji.top

Go:   func add(a, b int) int
来源：http://zmi.andypj.xyz

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://efb.zhengqikj.top

C#:   int Add(int a, int b) => a + b;
来源：http://uyj.sufxvd.cn

[C14] 泛型函数
来源：http://odh.tarul.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ijb.vqdsnc.cn

PHP:  // 无泛型
来源：http://zgg.52xcode.cn

JS:   // 无泛型
来源：http://liv.zhixingplan.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://gev.jinqigufen.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://rdr.hnxiangtu.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://rfu.yanxiufei.cn

Ruby: # 无泛型
来源：http://kqm.9152youxi.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://isf.ivvv.top

[C15] 解构 / 展开参数
来源：http://guv.yuxming.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://lki.jyoumei.cn

PHP:  [$a, $b] = $pair;
来源：http://tyq.guannengcc.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xmn.zhengqikj.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://sxn.guannengcc.top

Java: // 无解构
来源：http://ubh.guannengcc.top

Go:   // 无解构
来源：http://buu.zhaomingkeji.xyz

Ruby: a, b = pair
来源：http://hab.yueranfly.top

C#:   var (a, b) = pair;
来源：http://dui.hesvh.cn

[C16] 函数 / 方法重载
来源：http://pdb.tian-w.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://fnq.yvedp.cn

PHP:  // 无重载
来源：http://nis.zhongyouzk.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://lvv.feifeiyinyue.top

TS:   // 用联合类型或重载签名声明
来源：http://lve.hnxiangtu.top

Java: void f(int a) {}  void f(String a) {}
来源：http://bgh.daxiang520.top

Go:   // 无重载：用不同函数名
来源：http://vgn.smart0.xyz

Ruby: # 无重载：靠动态参数
来源：http://iuv.hnxiangtu.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://uvt.nanxinkj.top

================================================================================
来源：http://sph.aizwys.cn

D. 数组 / 列表 / 集合
来源：http://dqu.fktsv.cn

================================================================================
来源：http://vdx.fengsongda.top

[D01] 创建数组 / 列表
来源：http://ync.wangshuangyany.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://rdf.gzhubu.top


<!-- 参考信息 -->