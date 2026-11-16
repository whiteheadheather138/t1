代发 wailian999

[B01] 条件判断 if / else
来源：http://vpg.haohaochexian.top

Py:   result = "正" if x > 0 else "非正"
来源：http://vtv.yj20258.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://fqc.zhijiandao.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://lyt.iojbl.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://lix.ybcxt.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://ymm.jinghuilouyu.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://thk.zycfv.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hsv.redwolf501.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://kbr.mhx1999.top

[B02] 多分支 else if / elif
来源：http://uso.jinyuanbaomall.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mwp.xinyue.icu

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://dor.hammf.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qlq.epnwcf.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eel.9152youxi.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oec.shuidangran.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://xnn.zhiwuduotai.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://nze.guowangkeji.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://arq.dashuyun.cn

[B03] switch / match / case
来源：http://hvg.ydzc1.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://aym.jinqigufen.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://fct.chenlongwang.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ssj.cucudq.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://njs.ppjwa.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://lrp.zhixingplan.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://llw.316326.xyz

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://fkd.chenzaomai.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://fkw.zhaomingkeji.xyz

[B04] for 计数循环
来源：http://xlk.hnqzz.top

Py:   for i in range(10): print(i)
来源：http://ksw.sweek.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://qum.yvedp.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wzz.iojbl.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://poo.jinyuanbaomall.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://eef.meibo888.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://lwp.andypj.xyz

Ruby: 10.times { |i| puts i }
来源：http://dxv.ydjk.org.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://rxq.nwbrower.top

[B05] 遍历数组 / 列表
来源：http://huw.iojbl.cn

Py:   for item in arr: print(item)
来源：http://ncg.dashuyun.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ofb.dashuyun.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://kmc.yanxiufei.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://bql.ydjk.org.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://amw.c1oappe.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://bvf.fanxiaobao.xyz

Ruby: arr.each { |item| puts item }
来源：http://jnj.cqqwz.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://cjm.snrcjt.cn

[B06] 遍历字典 / 对象
来源：http://kxh.jinyuanbaomall.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://kca.yueranfly.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://bnc.cqqwz.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mpy.jyoumei.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xxe.sxryk.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://sva.gaohongyu789.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://qxi.sysykeji.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mhf.dianchejie.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://cmv.chenjidiqi.icu

[B07] while 循环
来源：http://vnx.mhx1999.top

Py:   while i < 10: i += 1
来源：http://vsj.haohaochexian.top

PHP:  while ($i < 10) { $i++; }
来源：http://jho.yj20258.top

JS:   while (i < 10) { i++; }
来源：http://hez.ydzc1.top

TS:   while (i < 10) { i++; }
来源：http://zmh.ybcxt.top

Java: while (i < 10) { i++; }
来源：http://hvu.zhixingplan.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://qby.hywenlv.cn

Ruby: while i < 10; i += 1; end
来源：http://lgu.hesvh.cn

C#:   while (i < 10) { i++; }
来源：http://mdq.ydzc1.top

[B08] do-while（至少执行一次）
来源：http://txd.ybcxt.top

Py:   # 无 do-while：用 while True + break
来源：http://pgj.nanxinkj.top

PHP:  do { $i++; } while ($i < 10);
来源：http://xre.nanxinkj.top

JS:   do { i++; } while (i < 10);
来源：http://ine.svipenyu.cn

TS:   do { i++; } while (i < 10);
来源：http://icj.havefunace.top

Java: do { i++; } while (i < 10);
来源：http://cst.vehdjk.com

Go:   for { i++; if i >= 10 { break } }
来源：http://jel.ctjpmb.com

Ruby: begin; i += 1; end while i < 10
来源：http://twe.guannengcc.top

C#:   do { i++; } while (i < 10);
来源：http://qjc.xylfe.cn

[B09] break 与 continue
来源：http://rve.zhongyouzk.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://bcs.jinghuilouyu.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://oxt.guannengcc.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nlg.kuanghao11.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pjh.hongshengwenyu.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pko.yueranfly.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://lbo.hesvh.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://emn.gzhubu.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://izb.sweek.top

[B10] 遍历同时拿索引
来源：http://iff.mhx1999.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://heb.zdbjq.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://jhc.yangfankeji.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://tjv.cqqwz.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://dib.havefunace.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://zgl.epnwcf.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://yjt.zhoulong.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wls.gotoacloud.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wan.daxiang520.top

[B11] 生成数字序列 / 区间
来源：http://bhn.zhoulong.xyz

Py:   list(range(0, 10, 2))
来源：http://cdu.gogol.net.cn

PHP:  range(0, 10, 2);
来源：http://obz.tarul.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wck.mhx1999.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pne.wangshuangyany.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://iwi.shangyingyoupin.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://eic.yanxiufei.cn

Ruby: (0...10).step(2).to_a
来源：http://tll.guannengcc.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://fzc.fktsv.cn

[B12] 跳出多层循环
来源：http://nxm.guannengcc.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://wmc.birdmap.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://rum.52xcode.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://rtl.xuanzx.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://gfy.9152youxi.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://xdu.jinghuilouyu.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://qxw.hammf.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://jjm.fengsongda.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://jiu.fzhhl.top

[B13] 判断是否为数字
来源：http://cmc.jqgfzy.top

Py:   isinstance(x, (int, float))
来源：http://gam.nwbrower.top

PHP:  is_numeric($x)
来源：http://ewl.vehdjk.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ixo.xinyue.icu

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vkr.iojbl.cn

Java: x instanceof Number
来源：http://ool.shzxlz.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ehy.bbcook.cn

Ruby: x.is_a?(Numeric)
来源：http://sij.ybcxt.top

C#:   x is int or double or decimal
来源：http://inl.yj20258.top

[B14] 判断值是否在集合内
来源：http://mai.yonumen.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://yma.cucudq.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ttp.havefunace.top

JS:   [1, 2, 3].includes(x)
来源：http://lwg.bbcook.cn

TS:   [1, 2, 3].includes(x)
来源：http://dec.bbcook.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://pzf.gzhubu.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ool.zdbjq.cn

Ruby: [1, 2, 3].include?(x)
来源：http://hct.zhoulong.xyz

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://tfm.52xcode.cn

[B15] 布尔运算与取反
来源：http://pje.yvedp.cn

Py:   a and b or not c
来源：http://hvq.redwolf501.top

PHP:  $a && $b || !$c
来源：http://dwt.hammf.cn

JS:   a && b || !c
来源：http://cpy.jianghu66.top

TS:   a && b || !c
来源：http://zkn.hnxiangtu.top

Java: a && b || !c
来源：http://pgs.sysykeji.top

Go:   a && b || !c
来源：http://ade.svipenyu.cn

Ruby: a && b || !c
来源：http://kzy.sxryk.cn

C#:   a && b || !c
来源：http://ulb.sjlbkw.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ter.cucudq.cn

Py:   if not data: return
来源：http://qkf.yj202588.top

PHP:  if (!$data) { return; }
来源：http://rbx.kuanghao11.cn

JS:   if (!data) return;
来源：http://ekj.daxiang520.top

TS:   if (!data) return;
来源：http://gqf.gotoacloud.top

Java: if (data == null) return;
来源：http://onp.xziqi.cn

Go:   if data == nil { return }
来源：http://axu.nanxinkj.top

Ruby: return if data.nil?
来源：http://gua.gzhubu.top

C#:   if (data == null) return;
来源：http://czm.wangdashe.top

================================================================================
来源：http://mtq.yvedp.cn

C. 函数与作用域
来源：http://xfc.gotoacloud.top

================================================================================
来源：http://dax.ywan-chungtsiang.top

[C01] 定义函数
来源：http://tmm.redwolf501.top

Py:   def add(a, b): return a + b
来源：http://ofd.hnxiangtu.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qic.guannengcc.top

JS:   function add(a, b) { return a + b; }
来源：http://wqu.daxiang520.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://muq.yangfankeji.com

Java: static int add(int a, int b) { return a + b; }
来源：http://nfy.daria6918.cn

Go:   func add(a, b int) int { return a + b }
来源：http://umm.vehdjk.com

Ruby: def add(a, b); a + b; end
来源：http://xjm.52xcode.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://nuh.svipenyu.cn

[C02] 默认参数
来源：http://sgk.52xcode.cn

Py:   def greet(name="World"): return name
来源：http://cge.bbcook.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://bvz.gogol.net.cn

JS:   function greet(name = "World") { return name; }
来源：http://vvf.sxryk.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://swv.shanyushiyangkeji.top

Java: // 无默认参数：方法重载或 Optional
来源：http://nbh.smart0.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://bam.wangdashe.top

Ruby: def greet(name = "World") = name
来源：http://obx.zhaomingkeji.xyz

C#:   string Greet(string name = "World") => name;
来源：http://szz.cucudq.cn

[C03] 可变参数
来源：http://jub.cqqwz.cn

Py:   def total(*args): return sum(args)
来源：http://zwh.hcnkem.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://tvp.gzhubu.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://twd.yj20258888.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://tau.zhixingplan.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://iju.gotoacloud.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://azz.ydzc1.top

Ruby: def total(*nums); nums.sum; end
来源：http://gsr.hnqzz.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ggh.shanyushiyangtech.top

[C04] 命名参数 / 关键字参数
来源：http://ebc.ehwqpu.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://pwh.tian-w.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mfx.sysykeji.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mul.316326.xyz

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://stj.fanxiaobao.xyz

Java: // 无：用 Builder 模式或 record
来源：http://oty.hnqzz.top

Go:   // 无：用配置结构体参数
来源：http://gio.wangdashe.top

Ruby: f(a: 1, b: 2)
来源：http://hqc.fzhhl.top

C#:   f(a: 1, b: 2)
来源：http://nyc.jiagoushi.top

[C05] 返回多个值
来源：http://lxq.mhx1999.top

Py:   return a, b
来源：http://bon.gogol.net.cn

PHP:  return [$a, $b];
来源：http://qsb.cheryme.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://aus.yueranfly.top

TS:   return { a, b };
来源：http://rbb.hywenlv.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://tcg.fzhhl.top

Go:   return a, b
来源：http://grq.sufxvd.cn

Ruby: return a, b
来源：http://bze.hywenlv.cn

C#:   return (a, b);              // ValueTuple
来源：http://xnj.bbcook.cn

[C06] 匿名函数 / lambda
来源：http://blt.chenlongwang.top

Py:   square = lambda x: x * x
来源：http://lav.ydjk.org.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://qeb.kuanghao11.cn

JS:   const square = x => x * x;
来源：http://dro.tanke756.top

TS:   const square = (x: number): number => x * x;
来源：http://dca.guowangkeji.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://rab.zhengqikj.top

Go:   sq := func(x int) int { return x * x }
来源：http://jon.tanke756.top

Ruby: square = ->(x) { x * x }
来源：http://tkm.xingfuxueyuan.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://utr.daria6918.cn

[C07] 把函数作为参数传入
来源：http://drd.fehbvm.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ntp.c1oappe.top

PHP:  array_map("strtoupper", $arr);
来源：http://oot.xuanzx.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ifu.andypj.xyz

TS:   arr.map(String)
来源：http://roc.haohaochexian.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://geg.feifeiyinyue.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://fdi.xuanzx.com

Ruby: arr.map(&:upcase)
来源：http://jgp.hywenlv.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ogl.hfpthk.cn

[C08] 闭包
来源：http://cvo.daxiang520.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://jyw.xuanzx.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ufk.jlsjyb.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://iwg.316326.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://zby.pengpengdd.cyou

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://tno.tanke756.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://piv.yuxming.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://htv.nanxinkj.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://piq.hywenlv.cn

[C09] 递归
来源：http://hor.wangshuangyany.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://dky.guannengcc.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://nzc.sysykeji.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rwi.pengpengdd.cyou

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ljr.gaohongyu789.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://flk.jqgufenzy.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://vnl.fzhhl.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://dws.9152youxi.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://xbs.yanxiufei.cn

[C10] 变量作用域
来源：http://avc.daxiang520.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://scg.zhengqikj.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wjz.guowangkeji.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mdk.xuanzx.com

TS:   同 JS
来源：http://gpu.hnqzz.top

Java: 方法内为块级作用域
来源：http://evv.bbcook.cn

Go:   花括号块级作用域
来源：http://zaf.yvedp.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://bhy.ydzc1.top

C#:   块级作用域
来源：http://bzp.nanxinkj.top

[C11] 模块导入与导出
来源：http://vow.fengsongda.top

Py:   from module import func
来源：http://tos.jqgfzy.top

PHP:  require "file.php";  或 use App\Service;
来源：http://wvg.zhengqikj.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://xop.guowangkeji.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wtd.jinqigfzy.top

Java: import java.util.List;
来源：http://usn.fzhhl.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://kjp.chenjidiqi.icu

Ruby: require "json"; require_relative "./util"
来源：http://qaq.ywan-chungtsiang.top

C#:   using System.Text;
来源：http://ekq.yfazqb.com

[C12] 立即执行函数 IIFE
来源：http://byu.tanke756.top

Py:   (lambda: print("run"))()
来源：http://klx.cashguo.top

PHP:  (function () { echo "run"; })();
来源：http://vbx.vqdsnc.cn

JS:   (() => { console.log("run"); })();
来源：http://jae.fengsongda.top

TS:   (() => { console.log("run"); })();
来源：http://urv.yvedp.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://qhr.jinqigufen.top

Go:   func() { fmt.Println("run") }()
来源：http://uva.meibo888.top

Ruby: -> { puts "run" }.call
来源：http://gme.c1oappe.top

C#:   // 无 IIFE：用静态构造函数
来源：http://kxf.yj202588.top

[C13] 类型声明 / 类型注解
来源：http://jpt.gotoacloud.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://zvw.shanyushiyangtech.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://poq.cqqwz.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://zhw.sjlbkw.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fdy.jiagoushi.top

Java: int add(int a, int b) { return a + b; }
来源：http://sec.gaohongyu789.top

Go:   func add(a, b int) int
来源：http://bga.dianchejie.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mun.hnqzz.top

C#:   int Add(int a, int b) => a + b;
来源：http://jst.yangfankeji.com

[C14] 泛型函数
来源：http://cwu.sweek.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ufu.52xcode.cn

PHP:  // 无泛型
来源：http://zip.dashuyun.cn

JS:   // 无泛型
来源：http://azx.chenlongwang.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://epr.sxryk.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wto.wangdashe.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ojc.xuanzx.com

Ruby: # 无泛型
来源：http://nkz.aibaodan.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ggs.yj20258888.top

[C15] 解构 / 展开参数
来源：http://juz.xuetiantiany.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://jhf.dianchejie.cn

PHP:  [$a, $b] = $pair;
来源：http://xgw.yuanzhike.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://icv.c1oappe.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ceg.vqdsnc.cn

Java: // 无解构
来源：http://oxi.c1oappe.top

Go:   // 无解构
来源：http://qzk.xylfe.cn

Ruby: a, b = pair
来源：http://jvm.hysaishi.cn

C#:   var (a, b) = pair;
来源：http://oia.yueranfly.top

[C16] 函数 / 方法重载
来源：http://oay.cheryme.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://fnp.jlsjyb.cn

PHP:  // 无重载
来源：http://oys.yuxming.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://fra.fengsongda.top

TS:   // 用联合类型或重载签名声明
来源：http://jry.gotoacloud.top

Java: void f(int a) {}  void f(String a) {}
来源：http://sks.zhaomingkeji.xyz

Go:   // 无重载：用不同函数名
来源：http://gxt.haohaochexian.top

Ruby: # 无重载：靠动态参数
来源：http://bxu.jyoumei.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://arj.hywenlv.cn

================================================================================
来源：http://lkw.jlsjyb.cn

D. 数组 / 列表 / 集合
来源：http://khs.ywan-chungtsiang.top

================================================================================
来源：http://bvh.ivvv.top

[D01] 创建数组 / 列表
来源：http://bbz.hcnkem.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://aiq.0kj1m.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://vgd.52xcode.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://rtx.xuetiantiany.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://pdu.sweek.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://pou.jqgufenzy.top


<!-- 参考信息 -->