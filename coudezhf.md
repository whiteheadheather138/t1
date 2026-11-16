代发 wailian999

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ozq.jqgufenzy.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://xlf.aizwys.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://rpd.ybcxt.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ovz.tanke756.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://fzr.wangshuangyany.cn

[B02] 多分支 else if / elif
来源：http://pdk.vehdjk.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://bdx.xuetiantiany.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ztv.xuetiantiany.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hot.zdbjq.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yhc.meibo888.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://evu.cucudq.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://xvg.jinqigufen.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://xzu.quarkkingdee.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wmx.c1oappe.top

[B03] switch / match / case
来源：http://uda.ybcxt.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://qio.yuanzhike.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://srv.cdnleiting.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wtv.pengpengdd.cyou

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://iop.quarkkingdee.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ibq.316326.xyz

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://qfl.cashguo.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://txt.guannengcc.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://xbp.sysykeji.top

[B04] for 计数循环
来源：http://sqf.zdqjudy.top

Py:   for i in range(10): print(i)
来源：http://lty.shzxlz.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://bir.yvedp.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fwd.zhoulong.xyz

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wdq.xinyue.icu

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://eki.gzhubu.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://qlk.hysaishi.cn

Ruby: 10.times { |i| puts i }
来源：http://ojf.zycfv.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://pcp.iojbl.cn

[B05] 遍历数组 / 列表
来源：http://had.haohaochexian.top

Py:   for item in arr: print(item)
来源：http://jyc.daria6918.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://tom.sweek.top

JS:   for (const item of arr) { console.log(item); }
来源：http://mlb.jyoumei.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://bwl.svipenyu.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://jjh.yonumen.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://plz.haohaochexian.top

Ruby: arr.each { |item| puts item }
来源：http://tyn.gotoacloud.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://qwz.zhoulong.xyz

[B06] 遍历字典 / 对象
来源：http://ulw.wangshuangyany.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://acr.ctjpmb.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://oju.yuxming.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ouh.epnwcf.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ncc.xziqi.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://yrz.dashuyun.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://goz.hysaishi.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://zlr.redwolf501.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://rjn.zhengqikj.top

[B07] while 循环
来源：http://cya.zycfv.cn

Py:   while i < 10: i += 1
来源：http://pan.sysykeji.top

PHP:  while ($i < 10) { $i++; }
来源：http://zya.xziqi.cn

JS:   while (i < 10) { i++; }
来源：http://imy.gogol.net.cn

TS:   while (i < 10) { i++; }
来源：http://cqb.ctjpmb.com

Java: while (i < 10) { i++; }
来源：http://ugk.ydzc1.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://eol.pengpengdd.cyou

Ruby: while i < 10; i += 1; end
来源：http://jmn.kuanghao11.cn

C#:   while (i < 10) { i++; }
来源：http://swe.daria6918.cn

[B08] do-while（至少执行一次）
来源：http://euh.chenjidiqi.icu

Py:   # 无 do-while：用 while True + break
来源：http://ekm.haohaochexian.top

PHP:  do { $i++; } while ($i < 10);
来源：http://sec.fanxiaobao.xyz

JS:   do { i++; } while (i < 10);
来源：http://ipo.ydjk.org.cn

TS:   do { i++; } while (i < 10);
来源：http://prt.nwbrower.top

Java: do { i++; } while (i < 10);
来源：http://dee.pengpengdd.cyou

Go:   for { i++; if i >= 10 { break } }
来源：http://gau.zhijiandao.cn

Ruby: begin; i += 1; end while i < 10
来源：http://nsl.yuanzhike.top

C#:   do { i++; } while (i < 10);
来源：http://zmi.fehbvm.com

[B09] break 与 continue
来源：http://tmw.hnxiangtu.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://qhl.birdmap.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://kty.hnxiangtu.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dsy.xingfuxueyuan.xyz

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sqf.yj20258888.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fow.uphjek.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ayn.zdbjq.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://anu.daria6918.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://alb.xziqi.cn

[B10] 遍历同时拿索引
来源：http://uur.yj202588.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wgx.tanke756.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://fxs.jinqigfzy.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://frj.cdnleiting.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://zam.jinqigufen.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://oie.yangfankeji.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://rwz.yj20258.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://kfo.xziqi.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://emm.yj202588.top

[B11] 生成数字序列 / 区间
来源：http://jpb.feifeiyinyue.top

Py:   list(range(0, 10, 2))
来源：http://ywe.hcnkem.com

PHP:  range(0, 10, 2);
来源：http://uzk.cqqwz.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mgu.tian-w.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mvc.hcnkem.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://etp.daxiang520.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://nhy.sufxvd.cn

Ruby: (0...10).step(2).to_a
来源：http://kom.jinqigfzy.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hxt.bjfxy.top

[B12] 跳出多层循环
来源：http://zby.chenzaomai.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://oew.zhoulong.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://boz.hfpthk.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://unz.sjlbkw.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://rwn.zhoulong.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hks.yongpay.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://brx.hfpthk.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://fkl.feifeiyinyue.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://djn.jqgfzy.top

[B13] 判断是否为数字
来源：http://moo.fzhhl.top

Py:   isinstance(x, (int, float))
来源：http://lby.xingfuxueyuan.xyz

PHP:  is_numeric($x)
来源：http://rki.jinghuilouyu.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://adr.gogol.net.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://huk.smart0.xyz

Java: x instanceof Number
来源：http://pez.dashuyun.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://qyt.hnxiangtu.top

Ruby: x.is_a?(Numeric)
来源：http://cku.jinqigufen.top

C#:   x is int or double or decimal
来源：http://zpd.xinyue.icu

[B14] 判断值是否在集合内
来源：http://jbc.hnxiangtu.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://zys.gotoacloud.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://uwo.hammf.cn

JS:   [1, 2, 3].includes(x)
来源：http://gpi.ctjpmb.com

TS:   [1, 2, 3].includes(x)
来源：http://otn.xziqi.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://iib.xinyue.icu

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://szf.cqqwz.cn

Ruby: [1, 2, 3].include?(x)
来源：http://qql.sufxvd.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://pce.yongpay.top

[B15] 布尔运算与取反
来源：http://hts.yuxming.cn

Py:   a and b or not c
来源：http://igd.yongpay.top

PHP:  $a && $b || !$c
来源：http://lsy.cashguo.top

JS:   a && b || !c
来源：http://nlv.yangfankeji.com

TS:   a && b || !c
来源：http://fbr.zdqjudy.top

Java: a && b || !c
来源：http://onu.daxiang520.top

Go:   a && b || !c
来源：http://tqf.tian-w.cn

Ruby: a && b || !c
来源：http://ieu.chenzaomai.com

C#:   a && b || !c
来源：http://kmw.52xcode.cn

[B16] 卫语句：不满足条件提前返回
来源：http://gnr.shanyushiyangtech.top

Py:   if not data: return
来源：http://vmp.yonumen.top

PHP:  if (!$data) { return; }
来源：http://uoj.snrcjt.cn

JS:   if (!data) return;
来源：http://fgf.cqqwz.cn

TS:   if (!data) return;
来源：http://xan.jinyuanbaomall.cn

Java: if (data == null) return;
来源：http://nik.zhoulong.xyz

Go:   if data == nil { return }
来源：http://wrz.hysaishi.cn

Ruby: return if data.nil?
来源：http://tgi.pengpengdd.cyou

C#:   if (data == null) return;
来源：http://hlq.yangfankeji.com

================================================================================
来源：http://vgt.xuetiantiany.cn

C. 函数与作用域
来源：http://yff.yueranfly.top

================================================================================
来源：http://hqn.jinghuilouyu.cn

[C01] 定义函数
来源：http://ltg.kuanghao11.cn

Py:   def add(a, b): return a + b
来源：http://gdg.redwolf501.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://drw.ivvv.top

JS:   function add(a, b) { return a + b; }
来源：http://fpl.jinghuilouyu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ekl.hnxiangtu.top

Java: static int add(int a, int b) { return a + b; }
来源：http://ndx.jianghu66.top

Go:   func add(a, b int) int { return a + b }
来源：http://smq.zhiwuduotai.top

Ruby: def add(a, b); a + b; end
来源：http://gaa.0kj1m.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://nmo.wangdashe.top

[C02] 默认参数
来源：http://nte.daria6918.cn

Py:   def greet(name="World"): return name
来源：http://lgq.hnxiangtu.top

PHP:  function greet($name = "World") { return $name; }
来源：http://rkb.zhaomingkeji.xyz

JS:   function greet(name = "World") { return name; }
来源：http://tyc.fanxiaobao.xyz

TS:   function greet(name: string = "World") { return name; }
来源：http://uop.jinqigufen.top

Java: // 无默认参数：方法重载或 Optional
来源：http://tek.kuanghao11.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://vgi.nwbrower.top

Ruby: def greet(name = "World") = name
来源：http://nqx.cqqwz.cn

C#:   string Greet(string name = "World") => name;
来源：http://vdx.hnxiangtu.top

[C03] 可变参数
来源：http://bxj.316326.xyz

Py:   def total(*args): return sum(args)
来源：http://tqr.xuetiantiany.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://zmc.zhongyouzk.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://uza.zhijiandao.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://twi.yfazqb.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://xbw.shuidangran.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mxo.hcnkem.com

Ruby: def total(*nums); nums.sum; end
来源：http://eqb.ctjpmb.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://adg.hongshengwenyu.top

[C04] 命名参数 / 关键字参数
来源：http://gnw.ivvv.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://oqj.wangdashe.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://jig.pengpengdd.cyou

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://scw.yuanzhike.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://jzx.tianlin.xyz

Java: // 无：用 Builder 模式或 record
来源：http://jmq.birdmap.top

Go:   // 无：用配置结构体参数
来源：http://jky.zycfv.cn

Ruby: f(a: 1, b: 2)
来源：http://nxl.yj20258.top

C#:   f(a: 1, b: 2)
来源：http://aaj.yangfankeji.com

[C05] 返回多个值
来源：http://ymn.fengsongda.top

Py:   return a, b
来源：http://hvv.yanxiufei.cn

PHP:  return [$a, $b];
来源：http://nhx.ppjwa.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ujl.sweek.top

TS:   return { a, b };
来源：http://gkd.ywan-chungtsiang.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://vcj.yongpay.top

Go:   return a, b
来源：http://eqg.daxiang520.top

Ruby: return a, b
来源：http://oyf.quarkkingdee.top

C#:   return (a, b);              // ValueTuple
来源：http://rpz.nanxinkj.top

[C06] 匿名函数 / lambda
来源：http://emj.shanyushiyangkeji.top

Py:   square = lambda x: x * x
来源：http://rtg.yuanzhike.top

PHP:  $square = fn($x) => $x * $x;
来源：http://jlv.jlsjyb.cn

JS:   const square = x => x * x;
来源：http://ejm.hysaishi.cn

TS:   const square = (x: number): number => x * x;
来源：http://gok.meibo888.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ule.iojbl.cn

Go:   sq := func(x int) int { return x * x }
来源：http://qea.sysykeji.top

Ruby: square = ->(x) { x * x }
来源：http://hvv.c1oappe.top

C#:   Func<int, int> square = x => x * x;
来源：http://laz.guowangkeji.top

[C07] 把函数作为参数传入
来源：http://jgy.xuanzx.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://osn.jinyuanbaomall.cn

PHP:  array_map("strtoupper", $arr);
来源：http://cmg.yfazqb.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hsv.havefunace.top

TS:   arr.map(String)
来源：http://vpk.chenjidiqi.icu

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://cne.xziqi.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://oqr.uphjek.com

Ruby: arr.map(&:upcase)
来源：http://ois.chenjidiqi.icu

C#:   arr.Select(s => s.ToUpper())
来源：http://omk.guowangkeji.top

[C08] 闭包
来源：http://qsu.hammf.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wpd.gaohongyu789.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://xzz.sjlbkw.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qes.sysykeji.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://fnv.snrcjt.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://bsj.ivvv.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hqq.svipenyu.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://sps.dianchejie.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mpn.nanxuanxn.top

[C09] 递归
来源：http://ryk.yonumen.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://siw.daria6918.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ane.pycfn.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zyy.hesvh.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pjm.chenjidiqi.icu

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://trq.yanxiufei.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://fyu.iojbl.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://tmm.zhiwuduotai.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://pkp.yueranfly.top

[C10] 变量作用域
来源：http://pyx.ywan-chungtsiang.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://xju.zdqjudy.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://udf.sxryk.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://qmp.jqgufenzy.top

TS:   同 JS
来源：http://jtg.yj202588.top

Java: 方法内为块级作用域
来源：http://nfq.0kj1m.cn

Go:   花括号块级作用域
来源：http://acz.daria6918.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wwn.zhiwuduotai.top

C#:   块级作用域
来源：http://adt.aizwys.cn

[C11] 模块导入与导出
来源：http://rhh.cheryme.top

Py:   from module import func
来源：http://dwc.cqqwz.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://dkb.gaohongyu789.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://vct.guannengcc.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://sjn.jlsjyb.cn

Java: import java.util.List;
来源：http://syc.cucudq.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://fxr.hfpthk.cn

Ruby: require "json"; require_relative "./util"
来源：http://tkz.vehdjk.com

C#:   using System.Text;
来源：http://lww.havefunace.top

[C12] 立即执行函数 IIFE
来源：http://cxn.chenzaomai.com

Py:   (lambda: print("run"))()
来源：http://ikb.yanxiufei.cn

PHP:  (function () { echo "run"; })();
来源：http://pml.chenjidiqi.icu

JS:   (() => { console.log("run"); })();
来源：http://ejj.yuxming.cn

TS:   (() => { console.log("run"); })();
来源：http://rvt.fengsongda.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://yvk.hongshengwenyu.top

Go:   func() { fmt.Println("run") }()
来源：http://nse.wangdashe.top

Ruby: -> { puts "run" }.call
来源：http://gzq.yanxiufei.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://zvn.xziqi.cn

[C13] 类型声明 / 类型注解
来源：http://oeh.sxryk.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://srb.xziqi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://igg.dianchejie.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ivi.mhx1999.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qsn.jiagoushi.top

Java: int add(int a, int b) { return a + b; }
来源：http://pdg.haohaochexian.top

Go:   func add(a, b int) int
来源：http://ifi.hywenlv.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://gmj.uphjek.com

C#:   int Add(int a, int b) => a + b;
来源：http://mvi.shanyushiyangkeji.top

[C14] 泛型函数
来源：http://iid.fanxiaobao.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://nbd.vehdjk.com

PHP:  // 无泛型
来源：http://enm.ydzc1.top

JS:   // 无泛型
来源：http://obe.meibo888.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://qft.xuetiantiany.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://edi.xinyue.icu

Go:   func First[T any](items []T) T { return items[0] }
来源：http://zzb.jianghu66.top

Ruby: # 无泛型
来源：http://lhr.daxiang520.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://nse.chenjidiqi.icu

[C15] 解构 / 展开参数
来源：http://pvd.jyoumei.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://omr.guannengcc.top

PHP:  [$a, $b] = $pair;
来源：http://vpy.yj20258.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://kod.sysykeji.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://qvv.xingfuxueyuan.xyz

Java: // 无解构
来源：http://nvs.meibo888.top

Go:   // 无解构
来源：http://cfm.redwolf501.top

Ruby: a, b = pair
来源：http://cxk.cdnleiting.top

C#:   var (a, b) = pair;
来源：http://myu.jqgfzy.top

[C16] 函数 / 方法重载
来源：http://osv.jiagoushi.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://bow.jqgfzy.top

PHP:  // 无重载
来源：http://scp.ydzc1.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://mgl.hysaishi.cn

TS:   // 用联合类型或重载签名声明
来源：http://dop.tianlin.xyz

Java: void f(int a) {}  void f(String a) {}
来源：http://xoo.hnqzz.top

Go:   // 无重载：用不同函数名
来源：http://wdb.hnqzz.top

Ruby: # 无重载：靠动态参数
来源：http://pes.wangdashe.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://blm.xuanzx.com

================================================================================
来源：http://hyi.yj20258.top

D. 数组 / 列表 / 集合
来源：http://wpl.pycfn.com

================================================================================
来源：http://cpb.gaohongyu789.top

[D01] 创建数组 / 列表
来源：http://kzt.shanyushiyangtech.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://mqr.birdmap.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hrc.yonumen.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://bmo.svipenyu.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://vsq.aizwys.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://cdk.gotoacloud.top

Go:   arr := []int{1, 2, 3}
来源：http://vut.vqdsnc.cn

Ruby: arr = [1, 2, 3]
来源：http://vmk.fktsv.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://odd.shzxlz.cn

[D02] 追加元素到末尾
来源：http://dkb.ybcxt.top


<!-- 参考信息 -->