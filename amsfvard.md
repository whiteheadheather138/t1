代发 wailian999

[B01] 条件判断 if / else
来源：http://twi.bjfxy.top

Py:   result = "正" if x > 0 else "非正"
来源：http://fdc.yvedp.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://joc.nanxinkj.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://bwt.yueranfly.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://jkq.jlsjyb.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ksu.chenlongwang.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://rcg.yueranfly.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mlf.hcnkem.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://xhu.nwbrower.top

[B02] 多分支 else if / elif
来源：http://noa.yongpay.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://dif.pengpengdd.cyou

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://lva.aibaodan.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vkr.ctjpmb.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jyu.xinyue.icu

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gdo.ydjk.org.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://syn.hammf.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://kih.jinqigfzy.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ywe.ctjpmb.com

[B03] switch / match / case
来源：http://dwm.wangshuangyany.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://eyt.vqdsnc.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://dlt.52xcode.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pfu.dianchejie.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vpv.shzxlz.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://lzz.yangfankeji.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hdb.dashuyun.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://bpu.yj20258.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://gaq.fanxiaobao.xyz

[B04] for 计数循环
来源：http://scr.yj20258888.top

Py:   for i in range(10): print(i)
来源：http://zyb.shzxlz.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://byi.chenjidiqi.icu

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hgp.jinyuanbaomall.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://eoe.ivvv.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://rvs.ctjpmb.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mid.dashuyun.cn

Ruby: 10.times { |i| puts i }
来源：http://qma.snrcjt.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://fsp.hnxiangtu.top

[B05] 遍历数组 / 列表
来源：http://xqu.nanxinkj.top

Py:   for item in arr: print(item)
来源：http://cfd.aizwys.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://fdc.dianchejie.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://qic.jyoumei.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://bey.hywenlv.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://hlu.shanyushiyangtech.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://zuj.guannengcc.top

Ruby: arr.each { |item| puts item }
来源：http://dge.ehwqpu.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://cpi.wangdashe.top

[B06] 遍历字典 / 对象
来源：http://dip.shangyingyoupin.top

Py:   for k, v in d.items(): print(k, v)
来源：http://ccc.sufxvd.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://yik.bbcook.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://foa.9152youxi.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gzx.fktsv.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://dic.snrcjt.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://kty.cashguo.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://sge.cucudq.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://rqq.hcnkem.com

[B07] while 循环
来源：http://siv.ehwqpu.com

Py:   while i < 10: i += 1
来源：http://quy.zhixingplan.top

PHP:  while ($i < 10) { $i++; }
来源：http://bfq.kuanghao11.cn

JS:   while (i < 10) { i++; }
来源：http://jgm.quarkkingdee.top

TS:   while (i < 10) { i++; }
来源：http://kme.birdmap.top

Java: while (i < 10) { i++; }
来源：http://deo.jqgufenzy.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://klg.yuxming.cn

Ruby: while i < 10; i += 1; end
来源：http://urj.yvedp.cn

C#:   while (i < 10) { i++; }
来源：http://rcn.gzhubu.top

[B08] do-while（至少执行一次）
来源：http://gtz.aizwys.cn

Py:   # 无 do-while：用 while True + break
来源：http://xgi.bjfxy.top

PHP:  do { $i++; } while ($i < 10);
来源：http://zsc.jinghuilouyu.cn

JS:   do { i++; } while (i < 10);
来源：http://vqw.havefunace.top

TS:   do { i++; } while (i < 10);
来源：http://hbn.tian-w.cn

Java: do { i++; } while (i < 10);
来源：http://oyx.zdbjq.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ekk.hesvh.cn

Ruby: begin; i += 1; end while i < 10
来源：http://okn.tanke756.top

C#:   do { i++; } while (i < 10);
来源：http://tob.yanxiufei.cn

[B09] break 与 continue
来源：http://rjd.zhoulong.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://pux.ppjwa.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://jaj.gogol.net.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ovz.chenzaomai.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qdc.hcnkem.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jqp.yj20258888.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ppw.jinqigufen.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://qka.fktsv.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ghi.gzhubu.top

[B10] 遍历同时拿索引
来源：http://xmj.jqgufenzy.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ank.sxryk.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://gwp.yj202588.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://aeu.zhengqikj.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://xzs.jinqigfzy.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://pxe.xziqi.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ibf.hnxiangtu.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://frg.gogol.net.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://qwe.dianchejie.cn

[B11] 生成数字序列 / 区间
来源：http://qpe.dianchejie.cn

Py:   list(range(0, 10, 2))
来源：http://qjm.cdnleiting.top

PHP:  range(0, 10, 2);
来源：http://hjp.dashuyun.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qzg.fengsongda.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ceq.xinyue.icu

Java: IntStream.range(0, 10).boxed().toList()
来源：http://tlg.xylfe.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://tlp.chenlongwang.top

Ruby: (0...10).step(2).to_a
来源：http://gjy.zdbjq.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zwm.chenjidiqi.icu

[B12] 跳出多层循环
来源：http://tcx.tian-w.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://iws.gotoacloud.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://jch.sxryk.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mps.dianchejie.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://lnc.ybcxt.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://slr.sjlbkw.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://xdw.yj202588.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://rtb.iojbl.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://xrg.sweek.top

[B13] 判断是否为数字
来源：http://ymo.cheryme.top

Py:   isinstance(x, (int, float))
来源：http://xyl.yuxming.cn

PHP:  is_numeric($x)
来源：http://dix.hfpthk.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://utu.xuetiantiany.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tfm.nwbrower.top

Java: x instanceof Number
来源：http://sey.tian-w.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://rto.hysaishi.cn

Ruby: x.is_a?(Numeric)
来源：http://qlq.wangshuangyany.cn

C#:   x is int or double or decimal
来源：http://cbd.tianlin.xyz

[B14] 判断值是否在集合内
来源：http://rdv.fanxiaobao.xyz

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://oiu.dashuyun.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://iuv.pengpengdd.cyou

JS:   [1, 2, 3].includes(x)
来源：http://zri.fehbvm.com

TS:   [1, 2, 3].includes(x)
来源：http://pfr.birdmap.top

Java: List.of(1, 2, 3).contains(x)
来源：http://pds.zhongyouzk.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://lul.zhijiandao.cn

Ruby: [1, 2, 3].include?(x)
来源：http://bpg.kuanghao11.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://cyc.jqgufenzy.top

[B15] 布尔运算与取反
来源：http://cpk.epnwcf.com

Py:   a and b or not c
来源：http://nmb.kuanghao11.cn

PHP:  $a && $b || !$c
来源：http://sly.shanyushiyangtech.top

JS:   a && b || !c
来源：http://ydf.pycfn.com

TS:   a && b || !c
来源：http://srd.shzxlz.cn

Java: a && b || !c
来源：http://qzy.tian-w.cn

Go:   a && b || !c
来源：http://hri.cashguo.top

Ruby: a && b || !c
来源：http://ysw.quarkkingdee.top

C#:   a && b || !c
来源：http://gyb.316326.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://yhs.ehwqpu.com

Py:   if not data: return
来源：http://xae.zhijiandao.cn

PHP:  if (!$data) { return; }
来源：http://otq.nanxuanxn.top

JS:   if (!data) return;
来源：http://ala.aibaodan.cn

TS:   if (!data) return;
来源：http://efh.daria6918.cn

Java: if (data == null) return;
来源：http://awk.feifeiyinyue.top

Go:   if data == nil { return }
来源：http://tdg.zycfv.cn

Ruby: return if data.nil?
来源：http://qjb.xinyue.icu

C#:   if (data == null) return;
来源：http://wlh.jiagoushi.top

================================================================================
来源：http://otu.ybcxt.top

C. 函数与作用域
来源：http://evj.tarul.cn

================================================================================
来源：http://cbq.uphjek.com

[C01] 定义函数
来源：http://jks.redwolf501.top

Py:   def add(a, b): return a + b
来源：http://pbm.hesvh.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nph.fzhhl.top

JS:   function add(a, b) { return a + b; }
来源：http://nqs.chenjidiqi.icu

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gir.guowangkeji.top

Java: static int add(int a, int b) { return a + b; }
来源：http://abg.redwolf501.top

Go:   func add(a, b int) int { return a + b }
来源：http://eci.guannengcc.top

Ruby: def add(a, b); a + b; end
来源：http://gdu.yongpay.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://rjb.hammf.cn

[C02] 默认参数
来源：http://qgj.cqqwz.cn

Py:   def greet(name="World"): return name
来源：http://kuq.fengsongda.top

PHP:  function greet($name = "World") { return $name; }
来源：http://lvp.gotoacloud.top

JS:   function greet(name = "World") { return name; }
来源：http://luv.nanxuanxn.top

TS:   function greet(name: string = "World") { return name; }
来源：http://gxk.vqdsnc.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://tna.yfazqb.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hcj.tian-w.cn

Ruby: def greet(name = "World") = name
来源：http://fkc.hnxiangtu.top

C#:   string Greet(string name = "World") => name;
来源：http://tyc.svipenyu.cn

[C03] 可变参数
来源：http://ptn.0kj1m.cn

Py:   def total(*args): return sum(args)
来源：http://nhm.chenzaomai.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xbq.zdbjq.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://eai.chenjidiqi.icu

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ggf.ywan-chungtsiang.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://puo.tian-w.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ifr.xuanzx.com

Ruby: def total(*nums); nums.sum; end
来源：http://wgr.hywenlv.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://znx.pengpengdd.cyou

[C04] 命名参数 / 关键字参数
来源：http://crt.bjfxy.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://gtl.birdmap.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ahb.wangdashe.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ifr.tianlin.xyz

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mss.aibaodan.cn

Java: // 无：用 Builder 模式或 record
来源：http://hrz.bjfxy.top

Go:   // 无：用配置结构体参数
来源：http://rlr.fktsv.cn

Ruby: f(a: 1, b: 2)
来源：http://too.gaohongyu789.top

C#:   f(a: 1, b: 2)
来源：http://akh.redwolf501.top

[C05] 返回多个值
来源：http://ldf.zhoulong.xyz

Py:   return a, b
来源：http://nqs.uphjek.com

PHP:  return [$a, $b];
来源：http://ozx.bjfxy.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://rge.yuanzhike.top

TS:   return { a, b };
来源：http://juj.zdbjq.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mae.xylfe.cn

Go:   return a, b
来源：http://equ.uphjek.com

Ruby: return a, b
来源：http://rte.snrcjt.cn

C#:   return (a, b);              // ValueTuple
来源：http://dqn.ctjpmb.com

[C06] 匿名函数 / lambda
来源：http://avk.hongshengwenyu.top

Py:   square = lambda x: x * x
来源：http://ltf.daria6918.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://bro.ivvv.top

JS:   const square = x => x * x;
来源：http://bve.xylfe.cn

TS:   const square = (x: number): number => x * x;
来源：http://dic.gogol.net.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://gju.ydzc1.top

Go:   sq := func(x int) int { return x * x }
来源：http://bjy.zhoulong.xyz

Ruby: square = ->(x) { x * x }
来源：http://rzq.ywan-chungtsiang.top

C#:   Func<int, int> square = x => x * x;
来源：http://nej.snrcjt.cn

[C07] 把函数作为参数传入
来源：http://jka.uphjek.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://nji.ctjpmb.com

PHP:  array_map("strtoupper", $arr);
来源：http://evd.fanxiaobao.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://nor.52xcode.cn

TS:   arr.map(String)
来源：http://bga.jyoumei.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://sws.ydjk.org.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://cfe.chenjidiqi.icu

Ruby: arr.map(&:upcase)
来源：http://odl.hesvh.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://njl.svipenyu.cn

[C08] 闭包
来源：http://nrm.yangfankeji.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://fxg.xuanzx.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://azs.ywan-chungtsiang.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://uud.wangdashe.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://rym.uphjek.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://fyn.tanke756.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wfj.feifeiyinyue.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://fgm.iojbl.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://vhi.jinyuanbaomall.cn

[C09] 递归
来源：http://eaj.sysykeji.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://zgb.nanxinkj.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ukr.xingfuxueyuan.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vuo.fanxiaobao.xyz

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://noo.316326.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://yxs.jlsjyb.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://fkd.nwbrower.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://twh.daria6918.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://uvh.gotoacloud.top

[C10] 变量作用域
来源：http://pwj.cucudq.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wuh.gzhubu.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://twy.0kj1m.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hrn.sxryk.cn

TS:   同 JS
来源：http://aue.ehwqpu.com

Java: 方法内为块级作用域
来源：http://ccv.yj20258888.top

Go:   花括号块级作用域
来源：http://zay.bjfxy.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://nst.sysykeji.top

C#:   块级作用域
来源：http://dqr.yanxiufei.cn

[C11] 模块导入与导出
来源：http://deq.hfpthk.cn

Py:   from module import func
来源：http://tvx.cheryme.top

PHP:  require "file.php";  或 use App\Service;
来源：http://stu.9152youxi.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://cbp.hongshengwenyu.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ugb.gaohongyu789.top

Java: import java.util.List;
来源：http://cai.yonumen.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://fgo.hesvh.cn

Ruby: require "json"; require_relative "./util"
来源：http://hgx.yueranfly.top

C#:   using System.Text;
来源：http://bfm.quarkkingdee.top

[C12] 立即执行函数 IIFE
来源：http://nvk.iojbl.cn

Py:   (lambda: print("run"))()
来源：http://rak.tianlin.xyz

PHP:  (function () { echo "run"; })();
来源：http://qil.zhengqikj.top

JS:   (() => { console.log("run"); })();
来源：http://wyz.bjfxy.top

TS:   (() => { console.log("run"); })();
来源：http://csj.316326.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://vqt.haohaochexian.top

Go:   func() { fmt.Println("run") }()
来源：http://uvg.cashguo.top

Ruby: -> { puts "run" }.call
来源：http://sqc.jinqigfzy.top

C#:   // 无 IIFE：用静态构造函数
来源：http://jni.cheryme.top

[C13] 类型声明 / 类型注解
来源：http://bqb.sweek.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://jho.bbcook.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gpo.gaohongyu789.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://fjd.mhx1999.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fbv.quarkkingdee.top

Java: int add(int a, int b) { return a + b; }
来源：http://ixc.ivvv.top

Go:   func add(a, b int) int
来源：http://acs.chenlongwang.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://gqf.ppjwa.cn

C#:   int Add(int a, int b) => a + b;
来源：http://cyn.fanxiaobao.xyz

[C14] 泛型函数
来源：http://pls.jqgufenzy.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wdd.hnqzz.top

PHP:  // 无泛型
来源：http://tty.uphjek.com

JS:   // 无泛型
来源：http://wui.xuanzx.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://orf.daxiang520.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://sgt.xinyue.icu

Go:   func First[T any](items []T) T { return items[0] }
来源：http://lpg.hongshengwenyu.top

Ruby: # 无泛型
来源：http://qnx.chenjidiqi.icu

C#:   static T First<T>(List<T> items) => items[0];
来源：http://doz.hesvh.cn

[C15] 解构 / 展开参数
来源：http://rte.yangfankeji.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://obo.wangshuangyany.cn

PHP:  [$a, $b] = $pair;
来源：http://pyt.gotoacloud.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://fqb.sjlbkw.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://pfw.svipenyu.cn

Java: // 无解构
来源：http://iri.wangshuangyany.cn

Go:   // 无解构
来源：http://obo.nwbrower.top

Ruby: a, b = pair
来源：http://kuk.xuanzx.com

C#:   var (a, b) = pair;
来源：http://cuy.9152youxi.cn

[C16] 函数 / 方法重载
来源：http://fbp.shangyingyoupin.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://yop.yuxming.cn

PHP:  // 无重载
来源：http://kxu.quarkkingdee.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://kht.yueranfly.top

TS:   // 用联合类型或重载签名声明
来源：http://qfv.snrcjt.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://awb.hcnkem.com

Go:   // 无重载：用不同函数名
来源：http://yrb.snrcjt.cn

Ruby: # 无重载：靠动态参数
来源：http://pyf.zhongyouzk.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://lbb.ybcxt.top

================================================================================
来源：http://yus.gotoacloud.top

D. 数组 / 列表 / 集合
来源：http://nik.birdmap.top

================================================================================
来源：http://ard.jinyuanbaomall.cn

[D01] 创建数组 / 列表
来源：http://olh.iojbl.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://jsb.snrcjt.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wdh.fktsv.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://vny.tianlin.xyz

TS:   const arr: number[] = [1, 2, 3];
来源：http://ymy.kuanghao11.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://glx.zhixingplan.top


<!-- 参考信息 -->