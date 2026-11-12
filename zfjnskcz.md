代发 wailian999

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mmb.ctjpmb.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://irm.haohaochexian.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://dew.chenlongwang.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://xny.fanxiaobao.xyz

C#:   var r = x > 0 ? "正" : "非正";
来源：http://stb.yueranfly.top

[B02] 多分支 else if / elif
来源：http://wqw.hywenlv.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ndy.havefunace.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://buo.zhaomingkeji.xyz

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yhc.9152youxi.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mdi.yfazqb.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sgb.yuxming.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://xba.zhoulong.xyz

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mrm.cashguo.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gzo.smart0.xyz

[B03] switch / match / case
来源：http://pee.zdqjudy.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://kfe.sysykeji.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://arr.zhaomingkeji.xyz

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://usn.yj202588.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://flx.hesvh.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://izi.tarul.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://azg.sweek.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ykl.haohaochexian.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://kyz.birdmap.top

[B04] for 计数循环
来源：http://rfm.shzxlz.cn

Py:   for i in range(10): print(i)
来源：http://lkf.sysykeji.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://cmd.cheryme.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rkt.ppjwa.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sbv.zhixingplan.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ktm.bbcook.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://abk.cdnleiting.top

Ruby: 10.times { |i| puts i }
来源：http://hlp.zdqjudy.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ndu.yongpay.top

[B05] 遍历数组 / 列表
来源：http://sum.iojbl.cn

Py:   for item in arr: print(item)
来源：http://gfv.bbcook.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://bow.aibaodan.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://hjk.jyoumei.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://bqa.svipenyu.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://byq.jlsjyb.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wbo.cqqwz.cn

Ruby: arr.each { |item| puts item }
来源：http://fkm.iojbl.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://yfs.meibo888.top

[B06] 遍历字典 / 对象
来源：http://ted.xingfuxueyuan.xyz

Py:   for k, v in d.items(): print(k, v)
来源：http://dyu.zhongyouzk.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://abx.xziqi.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ayv.jinghuilouyu.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://izb.gaohongyu789.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://azp.chenjidiqi.icu

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://sup.nwbrower.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://fgc.cucudq.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://rdd.yuxming.cn

[B07] while 循环
来源：http://fyr.hnxiangtu.top

Py:   while i < 10: i += 1
来源：http://axe.nwbrower.top

PHP:  while ($i < 10) { $i++; }
来源：http://ugf.xuanzx.com

JS:   while (i < 10) { i++; }
来源：http://nta.sxryk.cn

TS:   while (i < 10) { i++; }
来源：http://lwx.zhoulong.xyz

Java: while (i < 10) { i++; }
来源：http://jes.sxryk.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hou.daria6918.cn

Ruby: while i < 10; i += 1; end
来源：http://xjl.xylfe.cn

C#:   while (i < 10) { i++; }
来源：http://ytv.daxiang520.top

[B08] do-while（至少执行一次）
来源：http://apl.hywenlv.cn

Py:   # 无 do-while：用 while True + break
来源：http://yqj.vqdsnc.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://edb.hysaishi.cn

JS:   do { i++; } while (i < 10);
来源：http://lax.ppjwa.cn

TS:   do { i++; } while (i < 10);
来源：http://qus.yj202588.top

Java: do { i++; } while (i < 10);
来源：http://sau.sjlbkw.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://qza.svipenyu.cn

Ruby: begin; i += 1; end while i < 10
来源：http://mxa.bjfxy.top

C#:   do { i++; } while (i < 10);
来源：http://jqn.epnwcf.com

[B09] break 与 continue
来源：http://nka.hywenlv.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mpr.snrcjt.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://sez.ybcxt.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mir.andypj.xyz

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nzs.shuidangran.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ror.jlsjyb.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ejj.vqdsnc.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://emr.vehdjk.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lob.yj20258.top

[B10] 遍历同时拿索引
来源：http://qfg.jlsjyb.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://xgd.jianghu66.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://yza.zhixingplan.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mtj.shanyushiyangkeji.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://zoj.yuanzhike.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://abh.yongpay.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://jcy.wangshuangyany.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://vpj.mhx1999.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wuc.nanxuanxn.top

[B11] 生成数字序列 / 区间
来源：http://igt.meibo888.top

Py:   list(range(0, 10, 2))
来源：http://jwi.gogol.net.cn

PHP:  range(0, 10, 2);
来源：http://rpg.zhijiandao.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://drl.nanxinkj.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jbw.xuetiantiany.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ofo.jqgfzy.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mdj.cucudq.cn

Ruby: (0...10).step(2).to_a
来源：http://tyd.0kj1m.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://umx.yueranfly.top

[B12] 跳出多层循环
来源：http://ckb.cheryme.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://xqb.tianlin.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://zsi.mhx1999.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hpz.redwolf501.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://pzl.pycfn.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ddn.vehdjk.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ape.cucudq.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://rza.zhixingplan.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://htl.ybcxt.top

[B13] 判断是否为数字
来源：http://gfk.nanxuanxn.top

Py:   isinstance(x, (int, float))
来源：http://mra.feifeiyinyue.top

PHP:  is_numeric($x)
来源：http://bda.zhoulong.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lbo.yj20258888.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ljw.hfpthk.cn

Java: x instanceof Number
来源：http://kds.zdqjudy.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ztx.mhx1999.top

Ruby: x.is_a?(Numeric)
来源：http://ovr.xuanzx.com

C#:   x is int or double or decimal
来源：http://brw.gogol.net.cn

[B14] 判断值是否在集合内
来源：http://jrg.xinyue.icu

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://xnx.fktsv.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://nob.yfazqb.com

JS:   [1, 2, 3].includes(x)
来源：http://esx.snrcjt.cn

TS:   [1, 2, 3].includes(x)
来源：http://dwd.xuetiantiany.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://lxm.jiagoushi.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://fuo.xziqi.cn

Ruby: [1, 2, 3].include?(x)
来源：http://cui.wangdashe.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mot.chenjidiqi.icu

[B15] 布尔运算与取反
来源：http://lpg.yongpay.top

Py:   a and b or not c
来源：http://hdq.316326.xyz

PHP:  $a && $b || !$c
来源：http://hwb.jianghu66.top

JS:   a && b || !c
来源：http://aeg.bbcook.cn

TS:   a && b || !c
来源：http://ger.yj20258888.top

Java: a && b || !c
来源：http://rxi.zdqjudy.top

Go:   a && b || !c
来源：http://phg.chenzaomai.com

Ruby: a && b || !c
来源：http://sgr.uphjek.com

C#:   a && b || !c
来源：http://aen.tianlin.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://uzs.ivvv.top

Py:   if not data: return
来源：http://xfy.jinghuilouyu.cn

PHP:  if (!$data) { return; }
来源：http://bll.zhoulong.xyz

JS:   if (!data) return;
来源：http://scb.jinqigfzy.top

TS:   if (!data) return;
来源：http://ryk.hammf.cn

Java: if (data == null) return;
来源：http://pmn.havefunace.top

Go:   if data == nil { return }
来源：http://dkq.dashuyun.cn

Ruby: return if data.nil?
来源：http://evs.wangdashe.top

C#:   if (data == null) return;
来源：http://fqn.fehbvm.com

================================================================================
来源：http://paw.shuidangran.top

C. 函数与作用域
来源：http://tnr.andypj.xyz

================================================================================
来源：http://rma.zhoulong.xyz

[C01] 定义函数
来源：http://npt.ybcxt.top

Py:   def add(a, b): return a + b
来源：http://tsc.yj20258.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vrh.ppjwa.cn

JS:   function add(a, b) { return a + b; }
来源：http://yey.zhixingplan.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://auj.yj20258.top

Java: static int add(int a, int b) { return a + b; }
来源：http://obz.redwolf501.top

Go:   func add(a, b int) int { return a + b }
来源：http://wpm.ppjwa.cn

Ruby: def add(a, b); a + b; end
来源：http://ryl.sysykeji.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://eow.ppjwa.cn

[C02] 默认参数
来源：http://xlr.havefunace.top

Py:   def greet(name="World"): return name
来源：http://opl.ppjwa.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://uqf.ybcxt.top

JS:   function greet(name = "World") { return name; }
来源：http://nug.mhx1999.top

TS:   function greet(name: string = "World") { return name; }
来源：http://ogv.xingfuxueyuan.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://pzr.xylfe.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://xyx.gaohongyu789.top

Ruby: def greet(name = "World") = name
来源：http://mpb.havefunace.top

C#:   string Greet(string name = "World") => name;
来源：http://tnl.guowangkeji.top

[C03] 可变参数
来源：http://wps.xziqi.cn

Py:   def total(*args): return sum(args)
来源：http://nzq.dianchejie.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://gns.tianlin.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://xkm.yj20258888.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://yix.sxryk.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://erq.iojbl.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://pad.tarul.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ejx.316326.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ooc.yuanzhike.top

[C04] 命名参数 / 关键字参数
来源：http://qke.shanyushiyangtech.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://bic.bbcook.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://auc.hysaishi.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://scd.zhiwuduotai.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://uyr.hysaishi.cn

Java: // 无：用 Builder 模式或 record
来源：http://xti.guowangkeji.top

Go:   // 无：用配置结构体参数
来源：http://ciy.zycfv.cn

Ruby: f(a: 1, b: 2)
来源：http://zbb.yj20258888.top

C#:   f(a: 1, b: 2)
来源：http://kxg.aibaodan.cn

[C05] 返回多个值
来源：http://ido.mhx1999.top

Py:   return a, b
来源：http://owx.chenlongwang.top

PHP:  return [$a, $b];
来源：http://mxy.dianchejie.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://gnz.tianlin.xyz

TS:   return { a, b };
来源：http://ttf.c1oappe.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://yyd.dashuyun.cn

Go:   return a, b
来源：http://khw.hywenlv.cn

Ruby: return a, b
来源：http://ctl.feifeiyinyue.top

C#:   return (a, b);              // ValueTuple
来源：http://phb.tarul.cn

[C06] 匿名函数 / lambda
来源：http://kvt.daxiang520.top

Py:   square = lambda x: x * x
来源：http://kun.svipenyu.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://kib.nwbrower.top

JS:   const square = x => x * x;
来源：http://jxr.guannengcc.top

TS:   const square = (x: number): number => x * x;
来源：http://gut.meibo888.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hzq.mhx1999.top

Go:   sq := func(x int) int { return x * x }
来源：http://ury.fengsongda.top

Ruby: square = ->(x) { x * x }
来源：http://xbg.zhoulong.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://igh.hywenlv.cn

[C07] 把函数作为参数传入
来源：http://gua.yuanzhike.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ttg.hongshengwenyu.top

PHP:  array_map("strtoupper", $arr);
来源：http://jfl.iojbl.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://nsj.yfazqb.com

TS:   arr.map(String)
来源：http://ujb.zhiwuduotai.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://agb.jianghu66.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://gqe.ppjwa.cn

Ruby: arr.map(&:upcase)
来源：http://nqq.uphjek.com

C#:   arr.Select(s => s.ToUpper())
来源：http://fib.yj202588.top

[C08] 闭包
来源：http://cns.hnqzz.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://lnx.zhengqikj.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://nwr.9152youxi.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hrd.shuidangran.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://tnp.jqgfzy.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://azu.birdmap.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://fiz.chenjidiqi.icu

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://pgp.hongshengwenyu.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://sox.zhaomingkeji.xyz

[C09] 递归
来源：http://njl.fktsv.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://job.hesvh.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://uht.tanke756.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hqi.hammf.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lrk.yj20258.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://vlj.sysykeji.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ozn.sysykeji.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://jnf.vehdjk.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://jhv.birdmap.top

[C10] 变量作用域
来源：http://bjv.jinghuilouyu.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://izf.tianlin.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ruz.jianghu66.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ezx.jlsjyb.cn

TS:   同 JS
来源：http://qdu.yj20258.top

Java: 方法内为块级作用域
来源：http://xqg.iojbl.cn

Go:   花括号块级作用域
来源：http://sdl.ybcxt.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://iqq.yj20258.top

C#:   块级作用域
来源：http://wwy.daxiang520.top

[C11] 模块导入与导出
来源：http://lrn.c1oappe.top

Py:   from module import func
来源：http://ioo.hysaishi.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://eww.dianchejie.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://jen.chenzaomai.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://fjz.fktsv.cn

Java: import java.util.List;
来源：http://mqp.gogol.net.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://kku.jinghuilouyu.cn

Ruby: require "json"; require_relative "./util"
来源：http://mlz.hysaishi.cn

C#:   using System.Text;
来源：http://wuf.bbcook.cn

[C12] 立即执行函数 IIFE
来源：http://sps.xuetiantiany.cn

Py:   (lambda: print("run"))()
来源：http://bep.sweek.top

PHP:  (function () { echo "run"; })();
来源：http://bup.epnwcf.com

JS:   (() => { console.log("run"); })();
来源：http://pbv.ctjpmb.com

TS:   (() => { console.log("run"); })();
来源：http://jgf.yangfankeji.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://lcw.hysaishi.cn

Go:   func() { fmt.Println("run") }()
来源：http://yjp.yfazqb.com

Ruby: -> { puts "run" }.call
来源：http://xgn.nanxuanxn.top

C#:   // 无 IIFE：用静态构造函数
来源：http://mac.andypj.xyz

[C13] 类型声明 / 类型注解
来源：http://wyo.meibo888.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://qoi.zhaomingkeji.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://koq.xuetiantiany.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hiy.zhongyouzk.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://btd.jiagoushi.top

Java: int add(int a, int b) { return a + b; }
来源：http://iei.zdqjudy.top

Go:   func add(a, b int) int
来源：http://vve.cashguo.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://sxw.ivvv.top

C#:   int Add(int a, int b) => a + b;
来源：http://lid.gaohongyu789.top

[C14] 泛型函数
来源：http://sap.gzhubu.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://usb.andypj.xyz

PHP:  // 无泛型
来源：http://ejg.iojbl.cn

JS:   // 无泛型
来源：http://gtz.shanyushiyangtech.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ptn.cqqwz.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://dlk.wangdashe.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ees.sxryk.cn

Ruby: # 无泛型
来源：http://kdd.hnqzz.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://bar.chenjidiqi.icu

[C15] 解构 / 展开参数
来源：http://dhi.cashguo.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ztc.gaohongyu789.top

PHP:  [$a, $b] = $pair;
来源：http://blr.zhengqikj.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://pnw.yonumen.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://jpe.nanxinkj.top

Java: // 无解构
来源：http://nrh.tanke756.top

Go:   // 无解构
来源：http://gri.nanxuanxn.top

Ruby: a, b = pair
来源：http://fef.daxiang520.top

C#:   var (a, b) = pair;
来源：http://zot.hnxiangtu.top

[C16] 函数 / 方法重载
来源：http://uyd.smart0.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ovk.shzxlz.cn

PHP:  // 无重载
来源：http://qch.hesvh.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://mpw.shuidangran.top

TS:   // 用联合类型或重载签名声明
来源：http://sjv.pycfn.com

Java: void f(int a) {}  void f(String a) {}
来源：http://oyl.chenzaomai.com

Go:   // 无重载：用不同函数名
来源：http://egi.fehbvm.com

Ruby: # 无重载：靠动态参数
来源：http://tqg.cdnleiting.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://qlb.cheryme.top

================================================================================
来源：http://fat.wangdashe.top

D. 数组 / 列表 / 集合
来源：http://hig.gotoacloud.top

================================================================================
来源：http://wxl.sjlbkw.cn

[D01] 创建数组 / 列表
来源：http://ggh.cucudq.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://uhm.yvedp.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://cma.nanxuanxn.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ukg.cdnleiting.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://mdj.yangfankeji.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://dkq.meibo888.top

Go:   arr := []int{1, 2, 3}
来源：http://tep.ydjk.org.cn

Ruby: arr = [1, 2, 3]
来源：http://coj.xuetiantiany.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://lmq.havefunace.top

[D02] 追加元素到末尾
来源：http://ark.haohaochexian.top


<!-- 参考信息 -->