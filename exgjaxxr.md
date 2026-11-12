代发 wailian999

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ffd.ywan-chungtsiang.top

[B02] 多分支 else if / elif
来源：http://opr.jqgufenzy.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://kmu.tian-w.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://tbg.c1oappe.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oir.cashguo.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qga.daria6918.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://skc.aizwys.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://yqv.gotoacloud.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://pft.shzxlz.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oai.kuanghao11.cn

[B03] switch / match / case
来源：http://nve.haohaochexian.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wop.xziqi.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://edr.iojbl.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fso.yanxiufei.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nmv.andypj.xyz

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://yis.redwolf501.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mki.tarul.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://nsh.yj20258.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://erv.pycfn.com

[B04] for 计数循环
来源：http://ikj.xinyue.icu

Py:   for i in range(10): print(i)
来源：http://xpp.hfpthk.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://xlv.jqgfzy.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dtv.sweek.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rkv.tianlin.xyz

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hif.cdnleiting.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ksz.jianghu66.top

Ruby: 10.times { |i| puts i }
来源：http://znv.aizwys.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://kfw.jiagoushi.top

[B05] 遍历数组 / 列表
来源：http://lgj.nwbrower.top

Py:   for item in arr: print(item)
来源：http://epn.jinyuanbaomall.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://kaz.aibaodan.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://him.jianghu66.top

TS:   for (const item of arr) { console.log(item); }
来源：http://meb.pycfn.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://lpx.shuidangran.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://bje.zhongyouzk.top

Ruby: arr.each { |item| puts item }
来源：http://nrk.epnwcf.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://fdw.vehdjk.com

[B06] 遍历字典 / 对象
来源：http://qlz.sysykeji.top

Py:   for k, v in d.items(): print(k, v)
来源：http://hbg.aibaodan.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://vyh.yongpay.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fjy.sxryk.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vbc.epnwcf.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://bqr.cdnleiting.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://waq.jlsjyb.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hnh.pycfn.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://usl.xingfuxueyuan.xyz

[B07] while 循环
来源：http://jmo.jqgufenzy.top

Py:   while i < 10: i += 1
来源：http://sdz.wangdashe.top

PHP:  while ($i < 10) { $i++; }
来源：http://jyw.cdnleiting.top

JS:   while (i < 10) { i++; }
来源：http://rsl.zhijiandao.cn

TS:   while (i < 10) { i++; }
来源：http://pax.havefunace.top

Java: while (i < 10) { i++; }
来源：http://umq.hfpthk.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://nlc.wangdashe.top

Ruby: while i < 10; i += 1; end
来源：http://wpo.nanxuanxn.top

C#:   while (i < 10) { i++; }
来源：http://sql.haohaochexian.top

[B08] do-while（至少执行一次）
来源：http://kxz.wangshuangyany.cn

Py:   # 无 do-while：用 while True + break
来源：http://vqn.yuxming.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ftn.jqgufenzy.top

JS:   do { i++; } while (i < 10);
来源：http://ars.316326.xyz

TS:   do { i++; } while (i < 10);
来源：http://pen.meibo888.top

Java: do { i++; } while (i < 10);
来源：http://ylx.sxryk.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://okj.birdmap.top

Ruby: begin; i += 1; end while i < 10
来源：http://qog.guowangkeji.top

C#:   do { i++; } while (i < 10);
来源：http://rid.jyoumei.cn

[B09] break 与 continue
来源：http://cmt.tian-w.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://htx.c1oappe.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://jsi.hammf.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://igv.meibo888.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xrh.pycfn.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kod.guannengcc.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hfp.redwolf501.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://aee.zhijiandao.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vcl.smart0.xyz

[B10] 遍历同时拿索引
来源：http://uko.yonumen.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://yja.zhiwuduotai.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://gvo.hysaishi.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://pvn.ctjpmb.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ijo.hysaishi.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://sok.9152youxi.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://qsb.yj20258.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://fff.jqgufenzy.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://phk.sysykeji.top

[B11] 生成数字序列 / 区间
来源：http://cml.ivvv.top

Py:   list(range(0, 10, 2))
来源：http://zwi.hnxiangtu.top

PHP:  range(0, 10, 2);
来源：http://gyx.meibo888.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jud.gzhubu.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zde.sxryk.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ciq.iojbl.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://src.cucudq.cn

Ruby: (0...10).step(2).to_a
来源：http://smw.guowangkeji.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://suz.gogol.net.cn

[B12] 跳出多层循环
来源：http://eej.9152youxi.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://kfv.0kj1m.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://opw.svipenyu.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://jyl.gotoacloud.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://lab.shzxlz.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://thh.zhongyouzk.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://utl.feifeiyinyue.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://gwg.wangshuangyany.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://vlb.ivvv.top

[B13] 判断是否为数字
来源：http://ssz.dashuyun.cn

Py:   isinstance(x, (int, float))
来源：http://gbi.jiagoushi.top

PHP:  is_numeric($x)
来源：http://lut.daxiang520.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hmo.uphjek.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ols.ybcxt.top

Java: x instanceof Number
来源：http://ytn.ybcxt.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://grc.hcnkem.com

Ruby: x.is_a?(Numeric)
来源：http://krb.hywenlv.cn

C#:   x is int or double or decimal
来源：http://eig.9152youxi.cn

[B14] 判断值是否在集合内
来源：http://zah.sufxvd.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://nhh.zhaomingkeji.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://xhv.hesvh.cn

JS:   [1, 2, 3].includes(x)
来源：http://jet.0kj1m.cn

TS:   [1, 2, 3].includes(x)
来源：http://ssx.mhx1999.top

Java: List.of(1, 2, 3).contains(x)
来源：http://pkx.daxiang520.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ali.hnxiangtu.top

Ruby: [1, 2, 3].include?(x)
来源：http://pjn.0kj1m.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://big.fzhhl.top

[B15] 布尔运算与取反
来源：http://viz.zdbjq.cn

Py:   a and b or not c
来源：http://ojs.hywenlv.cn

PHP:  $a && $b || !$c
来源：http://btw.bbcook.cn

JS:   a && b || !c
来源：http://bhv.xziqi.cn

TS:   a && b || !c
来源：http://lwu.yangfankeji.com

Java: a && b || !c
来源：http://abw.feifeiyinyue.top

Go:   a && b || !c
来源：http://tzf.tarul.cn

Ruby: a && b || !c
来源：http://dzm.hcnkem.com

C#:   a && b || !c
来源：http://ziq.tianlin.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://pga.feifeiyinyue.top

Py:   if not data: return
来源：http://ufg.9152youxi.cn

PHP:  if (!$data) { return; }
来源：http://hhg.ppjwa.cn

JS:   if (!data) return;
来源：http://hjy.cashguo.top

TS:   if (!data) return;
来源：http://uyq.tanke756.top

Java: if (data == null) return;
来源：http://gdn.hnxiangtu.top

Go:   if data == nil { return }
来源：http://prt.yfazqb.com

Ruby: return if data.nil?
来源：http://kgk.jqgufenzy.top

C#:   if (data == null) return;
来源：http://fvy.xylfe.cn

================================================================================
来源：http://eme.cashguo.top

C. 函数与作用域
来源：http://xle.birdmap.top

================================================================================
来源：http://xlk.hywenlv.cn

[C01] 定义函数
来源：http://xla.316326.xyz

Py:   def add(a, b): return a + b
来源：http://vrf.nanxinkj.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sbj.jinyuanbaomall.cn

JS:   function add(a, b) { return a + b; }
来源：http://dza.hesvh.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dzr.ydzc1.top

Java: static int add(int a, int b) { return a + b; }
来源：http://cmx.bbcook.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ufq.bjfxy.top

Ruby: def add(a, b); a + b; end
来源：http://rme.ehwqpu.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://dfs.0kj1m.cn

[C02] 默认参数
来源：http://xkv.jinyuanbaomall.cn

Py:   def greet(name="World"): return name
来源：http://goa.ywan-chungtsiang.top

PHP:  function greet($name = "World") { return $name; }
来源：http://ifr.bjfxy.top

JS:   function greet(name = "World") { return name; }
来源：http://rvw.guannengcc.top

TS:   function greet(name: string = "World") { return name; }
来源：http://hqg.yj202588.top

Java: // 无默认参数：方法重载或 Optional
来源：http://isf.yanxiufei.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://tzf.fzhhl.top

Ruby: def greet(name = "World") = name
来源：http://tss.cashguo.top

C#:   string Greet(string name = "World") => name;
来源：http://xva.ydjk.org.cn

[C03] 可变参数
来源：http://esq.zhixingplan.top

Py:   def total(*args): return sum(args)
来源：http://goj.kuanghao11.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://yul.yongpay.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://xpz.yueranfly.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://lcs.gogol.net.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://rrj.ydjk.org.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://gvc.guannengcc.top

Ruby: def total(*nums); nums.sum; end
来源：http://gye.yonumen.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://stv.cdnleiting.top

[C04] 命名参数 / 关键字参数
来源：http://rco.gogol.net.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://vsh.yvedp.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wgt.nanxuanxn.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://bvx.chenjidiqi.icu

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://dwn.nanxinkj.top

Java: // 无：用 Builder 模式或 record
来源：http://nja.chenjidiqi.icu

Go:   // 无：用配置结构体参数
来源：http://hmk.kuanghao11.cn

Ruby: f(a: 1, b: 2)
来源：http://efu.316326.xyz

C#:   f(a: 1, b: 2)
来源：http://wji.gzhubu.top

[C05] 返回多个值
来源：http://ril.zhaomingkeji.xyz

Py:   return a, b
来源：http://mhp.jinyuanbaomall.cn

PHP:  return [$a, $b];
来源：http://jvq.haohaochexian.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://ifi.zhengqikj.top

TS:   return { a, b };
来源：http://hnz.vqdsnc.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://uzh.ybcxt.top

Go:   return a, b
来源：http://vji.xingfuxueyuan.xyz

Ruby: return a, b
来源：http://hhk.shangyingyoupin.top

C#:   return (a, b);              // ValueTuple
来源：http://vvr.xuetiantiany.cn

[C06] 匿名函数 / lambda
来源：http://osx.ydzc1.top

Py:   square = lambda x: x * x
来源：http://jkx.jyoumei.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://zkb.tarul.cn

JS:   const square = x => x * x;
来源：http://cqz.xziqi.cn

TS:   const square = (x: number): number => x * x;
来源：http://bhk.zhiwuduotai.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://yan.haohaochexian.top

Go:   sq := func(x int) int { return x * x }
来源：http://vyn.yuxming.cn

Ruby: square = ->(x) { x * x }
来源：http://xjt.bjfxy.top

C#:   Func<int, int> square = x => x * x;
来源：http://tnj.yongpay.top

[C07] 把函数作为参数传入
来源：http://sll.xuanzx.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://izy.shzxlz.cn

PHP:  array_map("strtoupper", $arr);
来源：http://qwp.jiagoushi.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://lba.xuetiantiany.cn

TS:   arr.map(String)
来源：http://ecz.kuanghao11.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://gbo.shangyingyoupin.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://omj.cqqwz.cn

Ruby: arr.map(&:upcase)
来源：http://zur.pengpengdd.cyou

C#:   arr.Select(s => s.ToUpper())
来源：http://jha.svipenyu.cn

[C08] 闭包
来源：http://bdn.fanxiaobao.xyz

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://tjk.sufxvd.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://fmi.gzhubu.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://xzv.gzhubu.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://szz.hcnkem.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://zpi.shzxlz.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wti.xziqi.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://dvd.sweek.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://pwa.pycfn.com

[C09] 递归
来源：http://pqs.chenjidiqi.icu

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://nhw.snrcjt.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://jgl.tarul.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ktm.shuidangran.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fhj.tianlin.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wfj.xuetiantiany.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://nmf.quarkkingdee.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://zmj.dianchejie.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://fhr.zycfv.cn

[C10] 变量作用域
来源：http://fiy.sysykeji.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ior.ppjwa.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://fxb.sjlbkw.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://omk.52xcode.cn

TS:   同 JS
来源：http://ifm.cheryme.top

Java: 方法内为块级作用域
来源：http://zyx.nanxuanxn.top

Go:   花括号块级作用域
来源：http://omw.fktsv.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wfu.hnqzz.top

C#:   块级作用域
来源：http://xdg.cashguo.top

[C11] 模块导入与导出
来源：http://cty.jinqigfzy.top

Py:   from module import func
来源：http://vxy.sxryk.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://pjz.hnqzz.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://pmt.jinqigufen.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ijs.zhengqikj.top

Java: import java.util.List;
来源：http://eub.jinqigufen.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ybl.pengpengdd.cyou

Ruby: require "json"; require_relative "./util"
来源：http://iay.shanyushiyangtech.top

C#:   using System.Text;
来源：http://qvz.chenzaomai.com

[C12] 立即执行函数 IIFE
来源：http://dzs.yongpay.top

Py:   (lambda: print("run"))()
来源：http://qsp.cdnleiting.top

PHP:  (function () { echo "run"; })();
来源：http://agg.yfazqb.com

JS:   (() => { console.log("run"); })();
来源：http://qiu.svipenyu.cn

TS:   (() => { console.log("run"); })();
来源：http://tev.epnwcf.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://fsg.ydzc1.top

Go:   func() { fmt.Println("run") }()
来源：http://lak.tanke756.top

Ruby: -> { puts "run" }.call
来源：http://mgk.ydjk.org.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://gjl.mhx1999.top

[C13] 类型声明 / 类型注解
来源：http://mjv.cashguo.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://sej.sweek.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kvh.c1oappe.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://fxm.fzhhl.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mbz.nanxuanxn.top

Java: int add(int a, int b) { return a + b; }
来源：http://zcr.ivvv.top

Go:   func add(a, b int) int
来源：http://hmj.tianlin.xyz

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mmo.sweek.top

C#:   int Add(int a, int b) => a + b;
来源：http://jfa.zdbjq.cn

[C14] 泛型函数
来源：http://vvz.jinghuilouyu.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://pdn.birdmap.top

PHP:  // 无泛型
来源：http://nve.shangyingyoupin.top

JS:   // 无泛型
来源：http://hse.ywan-chungtsiang.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://sgf.yj20258.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://suy.zdbjq.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hfv.xuanzx.com

Ruby: # 无泛型
来源：http://pfr.cashguo.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://apk.yuanzhike.top

[C15] 解构 / 展开参数
来源：http://qfp.pycfn.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://urw.nwbrower.top

PHP:  [$a, $b] = $pair;
来源：http://azn.pycfn.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://pui.jlsjyb.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://qxw.svipenyu.cn

Java: // 无解构
来源：http://swa.jqgfzy.top

Go:   // 无解构
来源：http://vwg.zycfv.cn

Ruby: a, b = pair
来源：http://gsi.yfazqb.com

C#:   var (a, b) = pair;
来源：http://hiy.guannengcc.top

[C16] 函数 / 方法重载
来源：http://cea.hcnkem.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vfe.jlsjyb.cn

PHP:  // 无重载
来源：http://tng.jyoumei.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://kbj.haohaochexian.top

TS:   // 用联合类型或重载签名声明
来源：http://kjy.feifeiyinyue.top

Java: void f(int a) {}  void f(String a) {}
来源：http://rkp.aibaodan.cn

Go:   // 无重载：用不同函数名
来源：http://rkv.ctjpmb.com

Ruby: # 无重载：靠动态参数
来源：http://jkt.fengsongda.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://nmv.zhaomingkeji.xyz

================================================================================
来源：http://ryn.ydzc1.top

D. 数组 / 列表 / 集合
来源：http://qhz.snrcjt.cn

================================================================================
来源：http://vfx.yj202588.top

[D01] 创建数组 / 列表
来源：http://dij.hammf.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://uow.hywenlv.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ujh.aibaodan.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://pkg.cucudq.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://kzc.pengpengdd.cyou

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://aot.jinyuanbaomall.cn

Go:   arr := []int{1, 2, 3}
来源：http://uta.dashuyun.cn

Ruby: arr = [1, 2, 3]
来源：http://oqc.ydjk.org.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mhk.tianlin.xyz

[D02] 追加元素到末尾
来源：http://acq.cdnleiting.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://rtj.tianlin.xyz

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ybh.dianchejie.cn

JS:   arr.push(4);
来源：http://ftn.smart0.xyz

TS:   arr.push(4);
来源：http://ezp.yj20258888.top


<!-- 参考信息 -->