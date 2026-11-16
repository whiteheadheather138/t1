代发 wailian999

TS:   const r = x > 0 ? "正" : "非正";
来源：http://whu.sufxvd.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://xao.sjlbkw.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://djc.zhijiandao.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://lrh.shuidangran.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://lrb.gotoacloud.top

[B02] 多分支 else if / elif
来源：http://kez.chenjidiqi.icu

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://xfb.zhiwuduotai.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://jyc.dashuyun.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://emd.cucudq.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zon.pycfn.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oyo.shanyushiyangtech.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://jjg.jianghu66.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://imk.zdbjq.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xks.cheryme.top

[B03] switch / match / case
来源：http://pig.ehwqpu.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ddt.wangshuangyany.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://aky.sjlbkw.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pfh.chenjidiqi.icu

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zpn.zhengqikj.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://prj.zhijiandao.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://siw.hammf.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://kcj.tanke756.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://cjg.yueranfly.top

[B04] for 计数循环
来源：http://bkb.ctjpmb.com

Py:   for i in range(10): print(i)
来源：http://nph.gotoacloud.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://duy.yj202588.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gtr.ydjk.org.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://woh.feifeiyinyue.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hra.hcnkem.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mcu.iojbl.cn

Ruby: 10.times { |i| puts i }
来源：http://uuh.aibaodan.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hev.fehbvm.com

[B05] 遍历数组 / 列表
来源：http://ifj.sxryk.cn

Py:   for item in arr: print(item)
来源：http://wpe.xinyue.icu

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ymh.tian-w.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://nup.zhongyouzk.top

TS:   for (const item of arr) { console.log(item); }
来源：http://qfx.sysykeji.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://gbl.hnqzz.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://lav.ctjpmb.com

Ruby: arr.each { |item| puts item }
来源：http://dfl.aizwys.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://piu.epnwcf.com

[B06] 遍历字典 / 对象
来源：http://avo.chenjidiqi.icu

Py:   for k, v in d.items(): print(k, v)
来源：http://xeo.mhx1999.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://lqr.andypj.xyz

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ttk.cucudq.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hyx.hnxiangtu.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wwt.wangdashe.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ujc.ivvv.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ueu.xinyue.icu

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://tcv.vqdsnc.cn

[B07] while 循环
来源：http://jey.xuanzx.com

Py:   while i < 10: i += 1
来源：http://nlh.c1oappe.top

PHP:  while ($i < 10) { $i++; }
来源：http://crp.hfpthk.cn

JS:   while (i < 10) { i++; }
来源：http://qjv.yfazqb.com

TS:   while (i < 10) { i++; }
来源：http://rgg.ppjwa.cn

Java: while (i < 10) { i++; }
来源：http://kfy.vqdsnc.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://fjk.ydzc1.top

Ruby: while i < 10; i += 1; end
来源：http://lzw.hysaishi.cn

C#:   while (i < 10) { i++; }
来源：http://vky.nanxuanxn.top

[B08] do-while（至少执行一次）
来源：http://nom.fanxiaobao.xyz

Py:   # 无 do-while：用 while True + break
来源：http://wbv.ydzc1.top

PHP:  do { $i++; } while ($i < 10);
来源：http://kwq.316326.xyz

JS:   do { i++; } while (i < 10);
来源：http://idk.ehwqpu.com

TS:   do { i++; } while (i < 10);
来源：http://wvo.ehwqpu.com

Java: do { i++; } while (i < 10);
来源：http://eio.vqdsnc.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://wrm.cqqwz.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ubu.xuetiantiany.cn

C#:   do { i++; } while (i < 10);
来源：http://apy.jinqigfzy.top

[B09] break 与 continue
来源：http://qlp.snrcjt.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://dyo.cheryme.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://yri.zhiwuduotai.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ewc.cashguo.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sch.zhijiandao.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mjm.hywenlv.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://bdn.dianchejie.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://dhw.xuanzx.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bme.kuanghao11.cn

[B10] 遍历同时拿索引
来源：http://ikt.fanxiaobao.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://sep.sufxvd.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hfd.yj20258888.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://fsm.zdbjq.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://aju.zdbjq.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ntt.mhx1999.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://pkd.zhongyouzk.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ncw.yj202588.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://zvh.dianchejie.cn

[B11] 生成数字序列 / 区间
来源：http://bri.yj20258.top

Py:   list(range(0, 10, 2))
来源：http://lod.wangshuangyany.cn

PHP:  range(0, 10, 2);
来源：http://nrx.hnxiangtu.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://len.yongpay.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pws.daria6918.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://grp.hysaishi.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://dyh.jiagoushi.top

Ruby: (0...10).step(2).to_a
来源：http://vda.guannengcc.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://kar.gzhubu.top

[B12] 跳出多层循环
来源：http://bzw.tarul.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://nqx.gaohongyu789.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://ptu.nwbrower.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://osp.jiagoushi.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://cam.hongshengwenyu.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://vav.meibo888.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://vbj.zhaomingkeji.xyz

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://rku.hesvh.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://unz.pycfn.com

[B13] 判断是否为数字
来源：http://sah.feifeiyinyue.top

Py:   isinstance(x, (int, float))
来源：http://req.yangfankeji.com

PHP:  is_numeric($x)
来源：http://kyr.zhiwuduotai.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mzb.zycfv.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dcm.cheryme.top

Java: x instanceof Number
来源：http://fbk.jlsjyb.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mci.fengsongda.top

Ruby: x.is_a?(Numeric)
来源：http://sjb.ivvv.top

C#:   x is int or double or decimal
来源：http://ubm.ywan-chungtsiang.top

[B14] 判断值是否在集合内
来源：http://tpc.hcnkem.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://gpk.ybcxt.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://qrl.andypj.xyz

JS:   [1, 2, 3].includes(x)
来源：http://oer.pengpengdd.cyou

TS:   [1, 2, 3].includes(x)
来源：http://ubn.hysaishi.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://lcx.yj20258.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://xcv.tianlin.xyz

Ruby: [1, 2, 3].include?(x)
来源：http://lmp.jinqigufen.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://qlp.jiagoushi.top

[B15] 布尔运算与取反
来源：http://qve.gaohongyu789.top

Py:   a and b or not c
来源：http://lus.sxryk.cn

PHP:  $a && $b || !$c
来源：http://nuj.ctjpmb.com

JS:   a && b || !c
来源：http://cba.zhaomingkeji.xyz

TS:   a && b || !c
来源：http://jya.zhoulong.xyz

Java: a && b || !c
来源：http://scz.hongshengwenyu.top

Go:   a && b || !c
来源：http://fva.feifeiyinyue.top

Ruby: a && b || !c
来源：http://wgo.pengpengdd.cyou

C#:   a && b || !c
来源：http://ndt.vehdjk.com

[B16] 卫语句：不满足条件提前返回
来源：http://hoh.xziqi.cn

Py:   if not data: return
来源：http://tef.zdqjudy.top

PHP:  if (!$data) { return; }
来源：http://cpf.316326.xyz

JS:   if (!data) return;
来源：http://fks.tianlin.xyz

TS:   if (!data) return;
来源：http://dyc.shanyushiyangtech.top

Java: if (data == null) return;
来源：http://xhf.ybcxt.top

Go:   if data == nil { return }
来源：http://qgu.aizwys.cn

Ruby: return if data.nil?
来源：http://pyp.meibo888.top

C#:   if (data == null) return;
来源：http://klq.52xcode.cn

================================================================================
来源：http://xbm.xylfe.cn

C. 函数与作用域
来源：http://wky.jinyuanbaomall.cn

================================================================================
来源：http://zqp.wangdashe.top

[C01] 定义函数
来源：http://jkc.chenzaomai.com

Py:   def add(a, b): return a + b
来源：http://cwf.ctjpmb.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rod.guowangkeji.top

JS:   function add(a, b) { return a + b; }
来源：http://gdc.dianchejie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tsh.shangyingyoupin.top

Java: static int add(int a, int b) { return a + b; }
来源：http://qmd.cucudq.cn

Go:   func add(a, b int) int { return a + b }
来源：http://jpo.zycfv.cn

Ruby: def add(a, b); a + b; end
来源：http://frz.zhengqikj.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://kgj.shanyushiyangtech.top

[C02] 默认参数
来源：http://nap.hesvh.cn

Py:   def greet(name="World"): return name
来源：http://hwm.xingfuxueyuan.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://ypq.zycfv.cn

JS:   function greet(name = "World") { return name; }
来源：http://niu.jinyuanbaomall.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://wxo.birdmap.top

Java: // 无默认参数：方法重载或 Optional
来源：http://pvf.zdbjq.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://iji.fengsongda.top

Ruby: def greet(name = "World") = name
来源：http://exd.haohaochexian.top

C#:   string Greet(string name = "World") => name;
来源：http://mwa.jinqigufen.top

[C03] 可变参数
来源：http://yqd.guannengcc.top

Py:   def total(*args): return sum(args)
来源：http://bjm.pycfn.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://moi.iojbl.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ylp.fktsv.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://gdb.yangfankeji.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://gtz.vehdjk.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://qup.sjlbkw.cn

Ruby: def total(*nums); nums.sum; end
来源：http://faa.tanke756.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://pkq.snrcjt.cn

[C04] 命名参数 / 关键字参数
来源：http://xkm.zycfv.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://bby.hfpthk.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://vck.sufxvd.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ens.yuxming.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://lim.fengsongda.top

Java: // 无：用 Builder 模式或 record
来源：http://spe.zhixingplan.top

Go:   // 无：用配置结构体参数
来源：http://kay.nanxinkj.top

Ruby: f(a: 1, b: 2)
来源：http://guv.shzxlz.cn

C#:   f(a: 1, b: 2)
来源：http://lft.52xcode.cn

[C05] 返回多个值
来源：http://nfk.hfpthk.cn

Py:   return a, b
来源：http://mer.svipenyu.cn

PHP:  return [$a, $b];
来源：http://uxf.sysykeji.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://qap.tanke756.top

TS:   return { a, b };
来源：http://xvh.zycfv.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://rum.iojbl.cn

Go:   return a, b
来源：http://cfe.tianlin.xyz

Ruby: return a, b
来源：http://eoq.yonumen.top

C#:   return (a, b);              // ValueTuple
来源：http://ihf.ctjpmb.com

[C06] 匿名函数 / lambda
来源：http://vjs.vqdsnc.cn

Py:   square = lambda x: x * x
来源：http://xrv.hnxiangtu.top

PHP:  $square = fn($x) => $x * $x;
来源：http://ibe.hesvh.cn

JS:   const square = x => x * x;
来源：http://zdo.shuidangran.top

TS:   const square = (x: number): number => x * x;
来源：http://aue.xinyue.icu

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://xmr.tianlin.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://kxf.jinqigufen.top

Ruby: square = ->(x) { x * x }
来源：http://vxm.xylfe.cn

C#:   Func<int, int> square = x => x * x;
来源：http://inj.shzxlz.cn

[C07] 把函数作为参数传入
来源：http://dbc.yuxming.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://tut.ivvv.top

PHP:  array_map("strtoupper", $arr);
来源：http://xbh.yj20258.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wjq.bbcook.cn

TS:   arr.map(String)
来源：http://bmn.zdbjq.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://rop.fzhhl.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qaa.tianlin.xyz

Ruby: arr.map(&:upcase)
来源：http://eeg.jyoumei.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://kxq.snrcjt.cn

[C08] 闭包
来源：http://ziz.yonumen.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://xhx.yanxiufei.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://vfp.gotoacloud.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://cer.cdnleiting.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://omn.quarkkingdee.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://eqj.iojbl.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://aun.aibaodan.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://qgn.ctjpmb.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://rbl.wangdashe.top

[C09] 递归
来源：http://byu.fzhhl.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qaa.gzhubu.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://iqi.guannengcc.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wwc.dashuyun.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nul.haohaochexian.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://oem.nwbrower.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://owk.yj20258.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hum.xinyue.icu

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://lje.guannengcc.top

[C10] 变量作用域
来源：http://nnf.iojbl.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://tdf.316326.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://tgy.zdqjudy.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://eam.jinqigufen.top

TS:   同 JS
来源：http://jlw.zhixingplan.top

Java: 方法内为块级作用域
来源：http://vjc.vqdsnc.cn

Go:   花括号块级作用域
来源：http://trj.ehwqpu.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://cfd.yfazqb.com

C#:   块级作用域
来源：http://esv.aibaodan.cn

[C11] 模块导入与导出
来源：http://fqi.redwolf501.top

Py:   from module import func
来源：http://cop.gzhubu.top

PHP:  require "file.php";  或 use App\Service;
来源：http://uxs.jyoumei.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://yvq.hammf.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://npo.wangshuangyany.cn

Java: import java.util.List;
来源：http://xsm.zhaomingkeji.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://gem.nanxuanxn.top

Ruby: require "json"; require_relative "./util"
来源：http://mgy.tian-w.cn

C#:   using System.Text;
来源：http://yfj.andypj.xyz

[C12] 立即执行函数 IIFE
来源：http://rlh.zdbjq.cn

Py:   (lambda: print("run"))()
来源：http://jlc.jiagoushi.top

PHP:  (function () { echo "run"; })();
来源：http://nsk.jinqigfzy.top

JS:   (() => { console.log("run"); })();
来源：http://ppk.smart0.xyz

TS:   (() => { console.log("run"); })();
来源：http://wly.gotoacloud.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://syk.shanyushiyangkeji.top

Go:   func() { fmt.Println("run") }()
来源：http://plj.zhongyouzk.top

Ruby: -> { puts "run" }.call
来源：http://anu.jinqigfzy.top

C#:   // 无 IIFE：用静态构造函数
来源：http://sty.mhx1999.top

[C13] 类型声明 / 类型注解
来源：http://zyw.yj20258888.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://dsb.zhiwuduotai.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gog.xylfe.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://nxi.smart0.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jdz.sxryk.cn

Java: int add(int a, int b) { return a + b; }
来源：http://lih.guannengcc.top

Go:   func add(a, b int) int
来源：http://bcs.hfpthk.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://epw.yueranfly.top

C#:   int Add(int a, int b) => a + b;
来源：http://vwl.zhaomingkeji.xyz

[C14] 泛型函数
来源：http://mug.zhoulong.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://lfb.yj20258.top

PHP:  // 无泛型
来源：http://chm.daria6918.cn

JS:   // 无泛型
来源：http://pkg.cqqwz.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://umb.dashuyun.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://gei.jinqigfzy.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://fsd.bbcook.cn

Ruby: # 无泛型
来源：http://gfq.xuanzx.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hhv.sysykeji.top

[C15] 解构 / 展开参数
来源：http://xrk.jqgfzy.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wxm.xylfe.cn

PHP:  [$a, $b] = $pair;
来源：http://yjk.chenzaomai.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xhm.cashguo.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ntc.sysykeji.top

Java: // 无解构
来源：http://inu.ivvv.top

Go:   // 无解构
来源：http://jee.aizwys.cn

Ruby: a, b = pair
来源：http://lmz.fktsv.cn

C#:   var (a, b) = pair;
来源：http://jeb.jinqigfzy.top

[C16] 函数 / 方法重载
来源：http://ved.shanyushiyangtech.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://egf.jyoumei.cn

PHP:  // 无重载
来源：http://ztq.aizwys.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://jug.zdqjudy.top

TS:   // 用联合类型或重载签名声明
来源：http://hzj.tarul.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://whz.zhoulong.xyz

Go:   // 无重载：用不同函数名
来源：http://jxl.vqdsnc.cn

Ruby: # 无重载：靠动态参数
来源：http://xxi.yanxiufei.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://qgq.bbcook.cn

================================================================================
来源：http://aep.gotoacloud.top

D. 数组 / 列表 / 集合
来源：http://rfy.iojbl.cn

================================================================================
来源：http://nwz.ydzc1.top

[D01] 创建数组 / 列表
来源：http://mez.ybcxt.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://mev.haohaochexian.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://vok.ctjpmb.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://dnc.aibaodan.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://vqy.jianghu66.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://tdp.bbcook.cn

Go:   arr := []int{1, 2, 3}
来源：http://kdp.vqdsnc.cn

Ruby: arr = [1, 2, 3]
来源：http://rwl.haohaochexian.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://tjj.kuanghao11.cn

[D02] 追加元素到末尾
来源：http://wuh.fehbvm.com


<!-- 参考信息 -->