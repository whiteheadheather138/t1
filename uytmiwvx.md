代发 wailian999

[B01] 条件判断 if / else
来源：http://bnc.nanxinkj.top

Py:   result = "正" if x > 0 else "非正"
来源：http://ijs.hongshengwenyu.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hml.yj20258.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://vna.sweek.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://xju.fzhhl.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://ibz.yj202588.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ixt.yuxming.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://pra.ehwqpu.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://oup.wangshuangyany.cn

[B02] 多分支 else if / elif
来源：http://zuz.jqgfzy.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://acx.zhengqikj.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://dib.yfazqb.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ari.hfpthk.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://iew.zdqjudy.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://aav.feifeiyinyue.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://iqg.jlsjyb.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://lok.zhijiandao.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cdu.sjlbkw.cn

[B03] switch / match / case
来源：http://ywj.jinqigfzy.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://krx.yueranfly.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://yve.hcnkem.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ook.sjlbkw.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mxf.birdmap.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://qbc.zhijiandao.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ccj.zhongyouzk.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ias.hammf.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://jor.chenzaomai.com

[B04] for 计数循环
来源：http://uxk.aizwys.cn

Py:   for i in range(10): print(i)
来源：http://zno.shanyushiyangkeji.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://azj.ydjk.org.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://uke.jinqigfzy.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vvs.ppjwa.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://gap.smart0.xyz

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://rwf.tian-w.cn

Ruby: 10.times { |i| puts i }
来源：http://hsx.bjfxy.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://yan.mhx1999.top

[B05] 遍历数组 / 列表
来源：http://ipn.bbcook.cn

Py:   for item in arr: print(item)
来源：http://elw.ydzc1.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ilt.52xcode.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://oki.shzxlz.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ppm.feifeiyinyue.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://tij.hesvh.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://bdh.yfazqb.com

Ruby: arr.each { |item| puts item }
来源：http://unm.yanxiufei.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://dyh.yangfankeji.com

[B06] 遍历字典 / 对象
来源：http://rpc.cdnleiting.top

Py:   for k, v in d.items(): print(k, v)
来源：http://lax.zhoulong.xyz

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://pmq.jinghuilouyu.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pyi.vqdsnc.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zxr.shanyushiyangtech.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://vop.sjlbkw.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://tpf.hnqzz.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hsn.316326.xyz

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://sit.pengpengdd.cyou

[B07] while 循环
来源：http://dfk.jiagoushi.top

Py:   while i < 10: i += 1
来源：http://pzk.hnxiangtu.top

PHP:  while ($i < 10) { $i++; }
来源：http://ayq.gotoacloud.top

JS:   while (i < 10) { i++; }
来源：http://unt.hongshengwenyu.top

TS:   while (i < 10) { i++; }
来源：http://aof.jinqigfzy.top

Java: while (i < 10) { i++; }
来源：http://bww.xinyue.icu

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://zsp.zycfv.cn

Ruby: while i < 10; i += 1; end
来源：http://eyc.sweek.top

C#:   while (i < 10) { i++; }
来源：http://muk.9152youxi.cn

[B08] do-while（至少执行一次）
来源：http://pkl.52xcode.cn

Py:   # 无 do-while：用 while True + break
来源：http://obr.cqqwz.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ujs.52xcode.cn

JS:   do { i++; } while (i < 10);
来源：http://xlm.smart0.xyz

TS:   do { i++; } while (i < 10);
来源：http://buz.daria6918.cn

Java: do { i++; } while (i < 10);
来源：http://qvs.ybcxt.top

Go:   for { i++; if i >= 10 { break } }
来源：http://iqu.haohaochexian.top

Ruby: begin; i += 1; end while i < 10
来源：http://ckv.wangshuangyany.cn

C#:   do { i++; } while (i < 10);
来源：http://ifx.xziqi.cn

[B09] break 与 continue
来源：http://dvy.gzhubu.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://tqs.nanxuanxn.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hiq.yuxming.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mwn.shangyingyoupin.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://urn.hfpthk.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jrh.birdmap.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://rpa.0kj1m.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wyl.nanxuanxn.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hlw.zycfv.cn

[B10] 遍历同时拿索引
来源：http://pto.ybcxt.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://jyd.52xcode.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ryt.andypj.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://bwi.zhaomingkeji.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://jbs.shanyushiyangtech.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ajm.cashguo.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ukm.gogol.net.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://lzd.aibaodan.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://eqn.zdqjudy.top

[B11] 生成数字序列 / 区间
来源：http://bqu.jinqigufen.top

Py:   list(range(0, 10, 2))
来源：http://kqw.jianghu66.top

PHP:  range(0, 10, 2);
来源：http://kym.ctjpmb.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sxi.vehdjk.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xck.sxryk.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://nis.haohaochexian.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://qqs.xuanzx.com

Ruby: (0...10).step(2).to_a
来源：http://tjl.yuxming.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://yvv.ehwqpu.com

[B12] 跳出多层循环
来源：http://ncp.shanyushiyangkeji.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://pss.xylfe.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://xdr.jinghuilouyu.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://uwz.wangdashe.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wci.0kj1m.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://obh.epnwcf.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://zcy.hywenlv.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://yqy.chenlongwang.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://nsy.yanxiufei.cn

[B13] 判断是否为数字
来源：http://lok.yongpay.top

Py:   isinstance(x, (int, float))
来源：http://pky.tarul.cn

PHP:  is_numeric($x)
来源：http://tjo.guannengcc.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://snf.sweek.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tpp.yangfankeji.com

Java: x instanceof Number
来源：http://upk.hfpthk.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://fuj.vqdsnc.cn

Ruby: x.is_a?(Numeric)
来源：http://gpb.hesvh.cn

C#:   x is int or double or decimal
来源：http://jwi.wangdashe.top

[B14] 判断值是否在集合内
来源：http://gyl.cqqwz.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://tce.havefunace.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://qaz.fzhhl.top

JS:   [1, 2, 3].includes(x)
来源：http://shb.shangyingyoupin.top

TS:   [1, 2, 3].includes(x)
来源：http://hqs.nwbrower.top

Java: List.of(1, 2, 3).contains(x)
来源：http://rny.zhoulong.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ick.tanke756.top

Ruby: [1, 2, 3].include?(x)
来源：http://lej.ydjk.org.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://qdu.vehdjk.com

[B15] 布尔运算与取反
来源：http://cbd.cucudq.cn

Py:   a and b or not c
来源：http://gjr.kuanghao11.cn

PHP:  $a && $b || !$c
来源：http://est.zdqjudy.top

JS:   a && b || !c
来源：http://sqn.zdqjudy.top

TS:   a && b || !c
来源：http://bgg.feifeiyinyue.top

Java: a && b || !c
来源：http://sjs.zdbjq.cn

Go:   a && b || !c
来源：http://vvi.cdnleiting.top

Ruby: a && b || !c
来源：http://drt.daxiang520.top

C#:   a && b || !c
来源：http://gig.hammf.cn

[B16] 卫语句：不满足条件提前返回
来源：http://bxb.xuanzx.com

Py:   if not data: return
来源：http://psl.mhx1999.top

PHP:  if (!$data) { return; }
来源：http://kzk.ybcxt.top

JS:   if (!data) return;
来源：http://jeu.zhaomingkeji.xyz

TS:   if (!data) return;
来源：http://ubq.xuetiantiany.cn

Java: if (data == null) return;
来源：http://dgn.316326.xyz

Go:   if data == nil { return }
来源：http://tlj.hammf.cn

Ruby: return if data.nil?
来源：http://kbi.guannengcc.top

C#:   if (data == null) return;
来源：http://ajg.hnqzz.top

================================================================================
来源：http://ojo.shuidangran.top

C. 函数与作用域
来源：http://ljg.zhixingplan.top

================================================================================
来源：http://ipb.daria6918.cn

[C01] 定义函数
来源：http://zck.ctjpmb.com

Py:   def add(a, b): return a + b
来源：http://rnz.bjfxy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rbj.hfpthk.cn

JS:   function add(a, b) { return a + b; }
来源：http://exb.vqdsnc.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dfw.jianghu66.top

Java: static int add(int a, int b) { return a + b; }
来源：http://uzq.jinyuanbaomall.cn

Go:   func add(a, b int) int { return a + b }
来源：http://jsg.fengsongda.top

Ruby: def add(a, b); a + b; end
来源：http://llr.shuidangran.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://rqc.fanxiaobao.xyz

[C02] 默认参数
来源：http://iya.yj20258.top

Py:   def greet(name="World"): return name
来源：http://tjl.jinghuilouyu.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://prl.ybcxt.top

JS:   function greet(name = "World") { return name; }
来源：http://aon.bbcook.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://alp.redwolf501.top

Java: // 无默认参数：方法重载或 Optional
来源：http://ggk.nanxinkj.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ucl.mhx1999.top

Ruby: def greet(name = "World") = name
来源：http://exv.yj20258.top

C#:   string Greet(string name = "World") => name;
来源：http://iaq.jqgufenzy.top

[C03] 可变参数
来源：http://qla.hfpthk.cn

Py:   def total(*args): return sum(args)
来源：http://cgq.fktsv.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://adg.shzxlz.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://dhj.xuanzx.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://vye.haohaochexian.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mej.smart0.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://atl.chenjidiqi.icu

Ruby: def total(*nums); nums.sum; end
来源：http://dzi.ctjpmb.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://oox.zhiwuduotai.top

[C04] 命名参数 / 关键字参数
来源：http://pno.yvedp.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://nzk.hywenlv.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xpl.mhx1999.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://fyd.yvedp.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://qnu.cheryme.top

Java: // 无：用 Builder 模式或 record
来源：http://paf.nwbrower.top

Go:   // 无：用配置结构体参数
来源：http://gvh.zhengqikj.top

Ruby: f(a: 1, b: 2)
来源：http://nve.ivvv.top

C#:   f(a: 1, b: 2)
来源：http://oil.xinyue.icu

[C05] 返回多个值
来源：http://uvn.zhiwuduotai.top

Py:   return a, b
来源：http://gdw.wangdashe.top

PHP:  return [$a, $b];
来源：http://ykv.fengsongda.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://lmx.hongshengwenyu.top

TS:   return { a, b };
来源：http://jhv.shanyushiyangtech.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mtc.quarkkingdee.top

Go:   return a, b
来源：http://niq.jinghuilouyu.cn

Ruby: return a, b
来源：http://hik.shanyushiyangkeji.top

C#:   return (a, b);              // ValueTuple
来源：http://mkg.svipenyu.cn

[C06] 匿名函数 / lambda
来源：http://ezg.gogol.net.cn

Py:   square = lambda x: x * x
来源：http://qti.yj202588.top

PHP:  $square = fn($x) => $x * $x;
来源：http://izd.ctjpmb.com

JS:   const square = x => x * x;
来源：http://hhb.hongshengwenyu.top

TS:   const square = (x: number): number => x * x;
来源：http://ivc.zhaomingkeji.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://dck.chenjidiqi.icu

Go:   sq := func(x int) int { return x * x }
来源：http://mxx.0kj1m.cn

Ruby: square = ->(x) { x * x }
来源：http://jvj.zhaomingkeji.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://mqx.fehbvm.com

[C07] 把函数作为参数传入
来源：http://jyb.shangyingyoupin.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://xpq.ydjk.org.cn

PHP:  array_map("strtoupper", $arr);
来源：http://eod.ehwqpu.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://jbs.shanyushiyangtech.top

TS:   arr.map(String)
来源：http://afs.jinyuanbaomall.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://pob.pengpengdd.cyou

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mdt.chenjidiqi.icu

Ruby: arr.map(&:upcase)
来源：http://hto.jianghu66.top

C#:   arr.Select(s => s.ToUpper())
来源：http://ptd.yonumen.top

[C08] 闭包
来源：http://cqr.gaohongyu789.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://kgz.andypj.xyz

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ciy.ctjpmb.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vns.jqgufenzy.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://zgn.52xcode.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://qgh.aibaodan.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hwj.tian-w.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://qoh.tianlin.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://qfc.ehwqpu.com

[C09] 递归
来源：http://jkn.fengsongda.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qnm.chenlongwang.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://zcb.zhiwuduotai.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://klx.mhx1999.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fvm.jinyuanbaomall.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://xwo.wangshuangyany.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://glo.hywenlv.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://pkd.birdmap.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://cia.vehdjk.com

[C10] 变量作用域
来源：http://tpt.shanyushiyangkeji.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://okz.ywan-chungtsiang.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ycp.shanyushiyangkeji.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://qzo.hnxiangtu.top

TS:   同 JS
来源：http://nxq.zhaomingkeji.xyz

Java: 方法内为块级作用域
来源：http://ctf.gogol.net.cn

Go:   花括号块级作用域
来源：http://btp.fengsongda.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://uin.zhiwuduotai.top

C#:   块级作用域
来源：http://hsg.bbcook.cn

[C11] 模块导入与导出
来源：http://pom.meibo888.top

Py:   from module import func
来源：http://xsy.ydzc1.top

PHP:  require "file.php";  或 use App\Service;
来源：http://skw.0kj1m.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://hov.52xcode.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://kpb.wangshuangyany.cn

Java: import java.util.List;
来源：http://buh.xuetiantiany.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://uhw.cucudq.cn

Ruby: require "json"; require_relative "./util"
来源：http://njb.yanxiufei.cn

C#:   using System.Text;
来源：http://lrg.xuanzx.com

[C12] 立即执行函数 IIFE
来源：http://epu.cheryme.top

Py:   (lambda: print("run"))()
来源：http://ymo.shzxlz.cn

PHP:  (function () { echo "run"; })();
来源：http://eks.yongpay.top

JS:   (() => { console.log("run"); })();
来源：http://svf.aibaodan.cn

TS:   (() => { console.log("run"); })();
来源：http://dnk.sysykeji.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://suk.zdbjq.cn

Go:   func() { fmt.Println("run") }()
来源：http://kcs.yangfankeji.com

Ruby: -> { puts "run" }.call
来源：http://uax.jinghuilouyu.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://gdv.feifeiyinyue.top

[C13] 类型声明 / 类型注解
来源：http://dxz.yj20258.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://izs.ybcxt.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rbs.fanxiaobao.xyz

JS:   // 无类型（可用 JSDoc 注释）
来源：http://lmp.gogol.net.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://grh.xuanzx.com

Java: int add(int a, int b) { return a + b; }
来源：http://kwi.bbcook.cn

Go:   func add(a, b int) int
来源：http://bix.zhijiandao.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://rgn.wangshuangyany.cn

C#:   int Add(int a, int b) => a + b;
来源：http://hdf.fzhhl.top

[C14] 泛型函数
来源：http://xht.pycfn.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://lwf.gotoacloud.top

PHP:  // 无泛型
来源：http://cbr.andypj.xyz

JS:   // 无泛型
来源：http://etu.zhongyouzk.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://cha.fktsv.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ssh.yanxiufei.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://sqd.shanyushiyangkeji.top

Ruby: # 无泛型
来源：http://dhz.guannengcc.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ntl.hongshengwenyu.top

[C15] 解构 / 展开参数
来源：http://qlt.iojbl.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ken.yj20258888.top

PHP:  [$a, $b] = $pair;
来源：http://fjk.cashguo.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://bke.mhx1999.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://xks.ehwqpu.com

Java: // 无解构
来源：http://vbm.gzhubu.top

Go:   // 无解构
来源：http://ajk.ctjpmb.com

Ruby: a, b = pair
来源：http://jkd.mhx1999.top

C#:   var (a, b) = pair;
来源：http://ygm.yueranfly.top

[C16] 函数 / 方法重载
来源：http://quq.meibo888.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://efy.shzxlz.cn

PHP:  // 无重载
来源：http://imf.316326.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://pib.aibaodan.cn

TS:   // 用联合类型或重载签名声明
来源：http://wky.shzxlz.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://bsj.zhongyouzk.top

Go:   // 无重载：用不同函数名
来源：http://xdm.ehwqpu.com

Ruby: # 无重载：靠动态参数
来源：http://yyd.cdnleiting.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://rev.chenjidiqi.icu

================================================================================
来源：http://zeh.daria6918.cn

D. 数组 / 列表 / 集合
来源：http://lcw.fanxiaobao.xyz

================================================================================
来源：http://gkq.dianchejie.cn

[D01] 创建数组 / 列表
来源：http://ltu.nwbrower.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://sgg.birdmap.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://usq.jinqigfzy.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://zqn.ydzc1.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://nor.chenjidiqi.icu

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://aqi.meibo888.top


<!-- 参考信息 -->