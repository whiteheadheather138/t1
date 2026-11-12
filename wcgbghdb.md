代发 wailian999

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://twd.yuanzhike.top

================================================================================
来源：http://tos.fktsv.cn

B. 流程控制
来源：http://gcd.snrcjt.cn

================================================================================
来源：http://cfu.fzhhl.top

[B01] 条件判断 if / else
来源：http://uij.316326.xyz

Py:   result = "正" if x > 0 else "非正"
来源：http://cdq.haohaochexian.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://gpl.wangshuangyany.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://msc.vehdjk.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://oic.nanxinkj.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://crw.jinghuilouyu.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://lkx.gogol.net.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ebh.zhixingplan.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://idg.ydzc1.top

[B02] 多分支 else if / elif
来源：http://hrw.yangfankeji.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://dfc.ydjk.org.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://uie.birdmap.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yoc.xinyue.icu

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lom.jyoumei.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ukv.hywenlv.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://eni.chenlongwang.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://jib.cashguo.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eqi.316326.xyz

[B03] switch / match / case
来源：http://yrm.zycfv.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://eul.hongshengwenyu.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://los.ctjpmb.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tre.snrcjt.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bhu.guowangkeji.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wnj.hywenlv.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://tig.cucudq.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://uyz.fktsv.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ggg.nwbrower.top

[B04] for 计数循环
来源：http://xxv.tanke756.top

Py:   for i in range(10): print(i)
来源：http://ezw.shangyingyoupin.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://kmk.cashguo.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zob.snrcjt.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ine.shangyingyoupin.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://stv.yj20258.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://kvu.xziqi.cn

Ruby: 10.times { |i| puts i }
来源：http://ptv.jinqigfzy.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://dbh.cucudq.cn

[B05] 遍历数组 / 列表
来源：http://jqh.yuxming.cn

Py:   for item in arr: print(item)
来源：http://xmw.zhixingplan.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://pfm.shanyushiyangtech.top

JS:   for (const item of arr) { console.log(item); }
来源：http://yqb.yueranfly.top

TS:   for (const item of arr) { console.log(item); }
来源：http://fmo.zhiwuduotai.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://dkk.jinqigufen.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://cmh.sysykeji.top

Ruby: arr.each { |item| puts item }
来源：http://sux.cdnleiting.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://haq.sufxvd.cn

[B06] 遍历字典 / 对象
来源：http://ufn.wangdashe.top

Py:   for k, v in d.items(): print(k, v)
来源：http://usx.hnqzz.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://izf.zhiwuduotai.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qve.xuetiantiany.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fce.fanxiaobao.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://eoy.ctjpmb.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://sgu.meibo888.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://znz.9152youxi.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://jxh.xylfe.cn

[B07] while 循环
来源：http://toy.yj20258888.top

Py:   while i < 10: i += 1
来源：http://nii.ivvv.top

PHP:  while ($i < 10) { $i++; }
来源：http://lys.shuidangran.top

JS:   while (i < 10) { i++; }
来源：http://rrg.tanke756.top

TS:   while (i < 10) { i++; }
来源：http://vin.zdqjudy.top

Java: while (i < 10) { i++; }
来源：http://mcr.vehdjk.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://dlz.fktsv.cn

Ruby: while i < 10; i += 1; end
来源：http://aji.sxryk.cn

C#:   while (i < 10) { i++; }
来源：http://qxj.yonumen.top

[B08] do-while（至少执行一次）
来源：http://syi.hnqzz.top

Py:   # 无 do-while：用 while True + break
来源：http://kmf.hywenlv.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://mqt.shuidangran.top

JS:   do { i++; } while (i < 10);
来源：http://ekb.bjfxy.top

TS:   do { i++; } while (i < 10);
来源：http://psy.316326.xyz

Java: do { i++; } while (i < 10);
来源：http://ngo.andypj.xyz

Go:   for { i++; if i >= 10 { break } }
来源：http://dxd.redwolf501.top

Ruby: begin; i += 1; end while i < 10
来源：http://fap.hnqzz.top

C#:   do { i++; } while (i < 10);
来源：http://xvv.shuidangran.top

[B09] break 与 continue
来源：http://nll.52xcode.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://iuq.zycfv.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ylo.jyoumei.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ffz.cucudq.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lac.yj202588.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mbb.c1oappe.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://byk.fengsongda.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://aag.vqdsnc.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ver.ywan-chungtsiang.top

[B10] 遍历同时拿索引
来源：http://lzq.ydzc1.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://fcq.tianlin.xyz

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://jvg.vqdsnc.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://nbz.52xcode.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wde.sweek.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://dkj.fzhhl.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://kgr.yuxming.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mng.yj202588.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ige.chenlongwang.top

[B11] 生成数字序列 / 区间
来源：http://tqh.tanke756.top

Py:   list(range(0, 10, 2))
来源：http://uoi.zdbjq.cn

PHP:  range(0, 10, 2);
来源：http://iro.jiagoushi.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://iml.jinqigfzy.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://aan.hysaishi.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://aui.feifeiyinyue.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://rrt.sxryk.cn

Ruby: (0...10).step(2).to_a
来源：http://mhx.52xcode.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://jky.gotoacloud.top

[B12] 跳出多层循环
来源：http://jux.havefunace.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://gih.cheryme.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://tjl.zhijiandao.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wgo.zdqjudy.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://qxv.wangshuangyany.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://fci.gaohongyu789.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://lou.316326.xyz

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://xbc.ybcxt.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://vjo.sjlbkw.cn

[B13] 判断是否为数字
来源：http://rkr.hammf.cn

Py:   isinstance(x, (int, float))
来源：http://xru.zhaomingkeji.xyz

PHP:  is_numeric($x)
来源：http://kcc.guannengcc.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gry.zhixingplan.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://umx.wangshuangyany.cn

Java: x instanceof Number
来源：http://daf.9152youxi.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://itl.mhx1999.top

Ruby: x.is_a?(Numeric)
来源：http://jxz.ehwqpu.com

C#:   x is int or double or decimal
来源：http://mon.zhixingplan.top

[B14] 判断值是否在集合内
来源：http://jih.hnqzz.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ydp.bjfxy.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://izg.snrcjt.cn

JS:   [1, 2, 3].includes(x)
来源：http://alk.ydzc1.top

TS:   [1, 2, 3].includes(x)
来源：http://muu.quarkkingdee.top

Java: List.of(1, 2, 3).contains(x)
来源：http://edc.jlsjyb.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ppj.zhijiandao.cn

Ruby: [1, 2, 3].include?(x)
来源：http://frg.havefunace.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://jvg.hcnkem.com

[B15] 布尔运算与取反
来源：http://ifl.svipenyu.cn

Py:   a and b or not c
来源：http://lel.ywan-chungtsiang.top

PHP:  $a && $b || !$c
来源：http://sjt.guowangkeji.top

JS:   a && b || !c
来源：http://hjn.feifeiyinyue.top

TS:   a && b || !c
来源：http://xhd.ehwqpu.com

Java: a && b || !c
来源：http://dqi.zhoulong.xyz

Go:   a && b || !c
来源：http://hjn.cqqwz.cn

Ruby: a && b || !c
来源：http://ila.havefunace.top

C#:   a && b || !c
来源：http://ipe.xziqi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://vtw.zhiwuduotai.top

Py:   if not data: return
来源：http://cdk.daria6918.cn

PHP:  if (!$data) { return; }
来源：http://vxu.vqdsnc.cn

JS:   if (!data) return;
来源：http://rqv.mhx1999.top

TS:   if (!data) return;
来源：http://pso.9152youxi.cn

Java: if (data == null) return;
来源：http://obj.xingfuxueyuan.xyz

Go:   if data == nil { return }
来源：http://fnk.fanxiaobao.xyz

Ruby: return if data.nil?
来源：http://koc.ivvv.top

C#:   if (data == null) return;
来源：http://kvj.cdnleiting.top

================================================================================
来源：http://tls.jyoumei.cn

C. 函数与作用域
来源：http://nio.tarul.cn

================================================================================
来源：http://lby.vqdsnc.cn

[C01] 定义函数
来源：http://ehp.mhx1999.top

Py:   def add(a, b): return a + b
来源：http://als.kuanghao11.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lsg.sxryk.cn

JS:   function add(a, b) { return a + b; }
来源：http://naw.fanxiaobao.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tld.aizwys.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://bhy.fanxiaobao.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://lic.aibaodan.cn

Ruby: def add(a, b); a + b; end
来源：http://qsr.hesvh.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://sih.haohaochexian.top

[C02] 默认参数
来源：http://pic.ppjwa.cn

Py:   def greet(name="World"): return name
来源：http://uwk.uphjek.com

PHP:  function greet($name = "World") { return $name; }
来源：http://owv.chenzaomai.com

JS:   function greet(name = "World") { return name; }
来源：http://tob.zycfv.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://bzm.yangfankeji.com

Java: // 无默认参数：方法重载或 Optional
来源：http://evg.jinqigfzy.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://com.ivvv.top

Ruby: def greet(name = "World") = name
来源：http://cnx.yuxming.cn

C#:   string Greet(string name = "World") => name;
来源：http://ken.havefunace.top

[C03] 可变参数
来源：http://bcx.pycfn.com

Py:   def total(*args): return sum(args)
来源：http://qux.zhijiandao.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://zba.ydzc1.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://rzd.haohaochexian.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hzl.birdmap.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://slb.xuetiantiany.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://toc.shuidangran.top

Ruby: def total(*nums); nums.sum; end
来源：http://pvx.cqqwz.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mvu.jqgfzy.top

[C04] 命名参数 / 关键字参数
来源：http://iri.yongpay.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://tol.sufxvd.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://egb.yanxiufei.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://owz.cheryme.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://anb.316326.xyz

Java: // 无：用 Builder 模式或 record
来源：http://qhw.sjlbkw.cn

Go:   // 无：用配置结构体参数
来源：http://qfe.tianlin.xyz

Ruby: f(a: 1, b: 2)
来源：http://cbp.hnqzz.top

C#:   f(a: 1, b: 2)
来源：http://ybi.xylfe.cn

[C05] 返回多个值
来源：http://yvf.gogol.net.cn

Py:   return a, b
来源：http://evs.sxryk.cn

PHP:  return [$a, $b];
来源：http://zlu.yuanzhike.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://fzo.jqgfzy.top

TS:   return { a, b };
来源：http://wec.shuidangran.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://sbx.gotoacloud.top

Go:   return a, b
来源：http://qon.meibo888.top

Ruby: return a, b
来源：http://mcc.zhaomingkeji.xyz

C#:   return (a, b);              // ValueTuple
来源：http://ydv.ydjk.org.cn

[C06] 匿名函数 / lambda
来源：http://jec.svipenyu.cn

Py:   square = lambda x: x * x
来源：http://mjo.iojbl.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://tsk.jlsjyb.cn

JS:   const square = x => x * x;
来源：http://mgj.cqqwz.cn

TS:   const square = (x: number): number => x * x;
来源：http://fhe.yvedp.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mqh.hammf.cn

Go:   sq := func(x int) int { return x * x }
来源：http://isc.zdbjq.cn

Ruby: square = ->(x) { x * x }
来源：http://kca.xinyue.icu

C#:   Func<int, int> square = x => x * x;
来源：http://gow.ehwqpu.com

[C07] 把函数作为参数传入
来源：http://sem.zhijiandao.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mqm.havefunace.top

PHP:  array_map("strtoupper", $arr);
来源：http://mdf.nwbrower.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://cjk.pengpengdd.cyou

TS:   arr.map(String)
来源：http://xxh.tianlin.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://myw.316326.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ixj.haohaochexian.top

Ruby: arr.map(&:upcase)
来源：http://fdc.pycfn.com

C#:   arr.Select(s => s.ToUpper())
来源：http://sxu.vqdsnc.cn

[C08] 闭包
来源：http://ncv.kuanghao11.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://vrq.chenlongwang.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ojc.ydjk.org.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wwr.yj20258.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://pso.cashguo.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://fcx.nwbrower.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ymi.meibo888.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://pyp.hammf.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://xok.meibo888.top

[C09] 递归
来源：http://rqo.sufxvd.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://xee.snrcjt.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://qlr.gzhubu.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://whr.hfpthk.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://smq.andypj.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://sgu.zhengqikj.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://nef.snrcjt.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hmz.dashuyun.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wkd.c1oappe.top

[C10] 变量作用域
来源：http://cts.redwolf501.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wok.zhiwuduotai.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://gip.zdbjq.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://zlj.cdnleiting.top

TS:   同 JS
来源：http://xja.shanyushiyangtech.top

Java: 方法内为块级作用域
来源：http://dld.guowangkeji.top

Go:   花括号块级作用域
来源：http://jle.jianghu66.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xko.shuidangran.top

C#:   块级作用域
来源：http://byh.316326.xyz

[C11] 模块导入与导出
来源：http://hjx.zhongyouzk.top

Py:   from module import func
来源：http://pfx.jinyuanbaomall.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ogd.aibaodan.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ban.zhengqikj.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://zls.yj20258.top

Java: import java.util.List;
来源：http://eya.yuxming.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://jod.smart0.xyz

Ruby: require "json"; require_relative "./util"
来源：http://zam.ybcxt.top

C#:   using System.Text;
来源：http://hup.ppjwa.cn

[C12] 立即执行函数 IIFE
来源：http://hpr.shanyushiyangkeji.top

Py:   (lambda: print("run"))()
来源：http://qzi.ydjk.org.cn

PHP:  (function () { echo "run"; })();
来源：http://ips.fzhhl.top

JS:   (() => { console.log("run"); })();
来源：http://pts.epnwcf.com

TS:   (() => { console.log("run"); })();
来源：http://dyb.jianghu66.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://avi.zhaomingkeji.xyz

Go:   func() { fmt.Println("run") }()
来源：http://gng.hcnkem.com

Ruby: -> { puts "run" }.call
来源：http://ezy.wangshuangyany.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ltb.kuanghao11.cn

[C13] 类型声明 / 类型注解
来源：http://lnf.svipenyu.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://zaq.fanxiaobao.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gtd.svipenyu.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ehk.nanxinkj.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://snd.yongpay.top

Java: int add(int a, int b) { return a + b; }
来源：http://mlm.hysaishi.cn

Go:   func add(a, b int) int
来源：http://qrr.dianchejie.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://fyz.shangyingyoupin.top

C#:   int Add(int a, int b) => a + b;
来源：http://fpq.jyoumei.cn

[C14] 泛型函数
来源：http://tab.0kj1m.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ntk.vqdsnc.cn

PHP:  // 无泛型
来源：http://iyr.xuanzx.com

JS:   // 无泛型
来源：http://bmg.nanxuanxn.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://kxg.daxiang520.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hdx.zhoulong.xyz

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ndv.hnqzz.top

Ruby: # 无泛型
来源：http://hia.ydjk.org.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://nec.chenjidiqi.icu

[C15] 解构 / 展开参数
来源：http://fma.kuanghao11.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://rrv.guannengcc.top

PHP:  [$a, $b] = $pair;
来源：http://fwn.ybcxt.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://izn.daria6918.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mts.shzxlz.cn

Java: // 无解构
来源：http://sfr.bjfxy.top

Go:   // 无解构
来源：http://hvk.zycfv.cn

Ruby: a, b = pair
来源：http://ftf.tarul.cn

C#:   var (a, b) = pair;
来源：http://uel.hfpthk.cn

[C16] 函数 / 方法重载
来源：http://jel.cheryme.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://bjg.cqqwz.cn

PHP:  // 无重载
来源：http://zyt.epnwcf.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://seq.bbcook.cn

TS:   // 用联合类型或重载签名声明
来源：http://waz.jinqigfzy.top

Java: void f(int a) {}  void f(String a) {}
来源：http://rge.dianchejie.cn

Go:   // 无重载：用不同函数名
来源：http://wus.c1oappe.top

Ruby: # 无重载：靠动态参数
来源：http://qls.cqqwz.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://oro.yvedp.cn

================================================================================
来源：http://ztc.tarul.cn

D. 数组 / 列表 / 集合
来源：http://iqh.nanxuanxn.top

================================================================================
来源：http://bqh.zhijiandao.cn

[D01] 创建数组 / 列表
来源：http://ndt.vqdsnc.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ftj.dashuyun.cn


<!-- 参考信息 -->