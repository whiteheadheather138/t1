代发 wailian999

TS:   const r = x > 0 ? "正" : "非正";
来源：http://xgi.nanxinkj.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://njv.hesvh.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://gtk.ppjwa.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://pmi.pengpengdd.cyou

C#:   var r = x > 0 ? "正" : "非正";
来源：http://kew.yj20258888.top

[B02] 多分支 else if / elif
来源：http://xyq.sufxvd.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://bcx.uphjek.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://tty.tian-w.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nfj.zhijiandao.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mjt.andypj.xyz

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uyj.zhiwuduotai.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ube.yj202588.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://jzd.hcnkem.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ggw.pycfn.com

[B03] switch / match / case
来源：http://nlt.dianchejie.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://won.ehwqpu.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://nwm.cdnleiting.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nbx.dashuyun.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://enx.zdqjudy.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://rav.dianchejie.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://bll.smart0.xyz

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://xcn.zhaomingkeji.xyz

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://dyi.svipenyu.cn

[B04] for 计数循环
来源：http://txe.0kj1m.cn

Py:   for i in range(10): print(i)
来源：http://uch.xziqi.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://kpq.316326.xyz

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nir.andypj.xyz

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yvx.chenlongwang.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://npf.pycfn.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://oww.yanxiufei.cn

Ruby: 10.times { |i| puts i }
来源：http://ssj.zhijiandao.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://stg.zhongyouzk.top

[B05] 遍历数组 / 列表
来源：http://cbp.havefunace.top

Py:   for item in arr: print(item)
来源：http://org.cheryme.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://rdh.yfazqb.com

JS:   for (const item of arr) { console.log(item); }
来源：http://opi.zdbjq.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://spc.xuetiantiany.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://bdz.c1oappe.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://bgr.fengsongda.top

Ruby: arr.each { |item| puts item }
来源：http://ydv.fktsv.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ajb.dianchejie.cn

[B06] 遍历字典 / 对象
来源：http://wqi.jinyuanbaomall.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://axp.xinyue.icu

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://uko.uphjek.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vsm.sufxvd.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lbj.nanxuanxn.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://fyb.jinyuanbaomall.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://oek.yj20258.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ofp.hywenlv.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ywc.nanxuanxn.top

[B07] while 循环
来源：http://jbk.chenlongwang.top

Py:   while i < 10: i += 1
来源：http://stj.chenzaomai.com

PHP:  while ($i < 10) { $i++; }
来源：http://inp.shanyushiyangtech.top

JS:   while (i < 10) { i++; }
来源：http://ibp.shangyingyoupin.top

TS:   while (i < 10) { i++; }
来源：http://bya.ywan-chungtsiang.top

Java: while (i < 10) { i++; }
来源：http://qmk.shanyushiyangtech.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mrc.hongshengwenyu.top

Ruby: while i < 10; i += 1; end
来源：http://lno.gaohongyu789.top

C#:   while (i < 10) { i++; }
来源：http://aor.haohaochexian.top

[B08] do-while（至少执行一次）
来源：http://jld.xingfuxueyuan.xyz

Py:   # 无 do-while：用 while True + break
来源：http://ezo.xingfuxueyuan.xyz

PHP:  do { $i++; } while ($i < 10);
来源：http://fdf.cucudq.cn

JS:   do { i++; } while (i < 10);
来源：http://mvi.yanxiufei.cn

TS:   do { i++; } while (i < 10);
来源：http://scz.quarkkingdee.top

Java: do { i++; } while (i < 10);
来源：http://uds.yj202588.top

Go:   for { i++; if i >= 10 { break } }
来源：http://ctd.zdbjq.cn

Ruby: begin; i += 1; end while i < 10
来源：http://drh.yonumen.top

C#:   do { i++; } while (i < 10);
来源：http://jaw.hysaishi.cn

[B09] break 与 continue
来源：http://qgm.xziqi.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ito.shangyingyoupin.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://uug.yongpay.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lro.cqqwz.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wyk.sxryk.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://iug.xuetiantiany.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://afu.bjfxy.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://dkn.gogol.net.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zsj.tarul.cn

[B10] 遍历同时拿索引
来源：http://iog.tanke756.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://jrg.shangyingyoupin.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://btk.vqdsnc.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://iwz.hysaishi.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://dsb.bjfxy.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://pga.zdbjq.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://jgv.andypj.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ekb.shuidangran.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://zhd.wangdashe.top

[B11] 生成数字序列 / 区间
来源：http://olj.nwbrower.top

Py:   list(range(0, 10, 2))
来源：http://zmo.havefunace.top

PHP:  range(0, 10, 2);
来源：http://ffy.shuidangran.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pin.fehbvm.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://njm.ywan-chungtsiang.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://fqx.zycfv.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://zua.jinqigufen.top

Ruby: (0...10).step(2).to_a
来源：http://sty.cucudq.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://gsp.9152youxi.cn

[B12] 跳出多层循环
来源：http://eiq.fehbvm.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://nhp.dashuyun.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://sfi.xuetiantiany.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://xtg.chenjidiqi.icu

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://urp.shangyingyoupin.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://qpx.shzxlz.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://uzw.andypj.xyz

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://oqx.sweek.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://fif.zycfv.cn

[B13] 判断是否为数字
来源：http://wgu.xziqi.cn

Py:   isinstance(x, (int, float))
来源：http://jwj.hnxiangtu.top

PHP:  is_numeric($x)
来源：http://hmf.hfpthk.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pdo.fktsv.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cbd.birdmap.top

Java: x instanceof Number
来源：http://yyi.nwbrower.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ght.ydzc1.top

Ruby: x.is_a?(Numeric)
来源：http://fmg.meibo888.top

C#:   x is int or double or decimal
来源：http://yny.ehwqpu.com

[B14] 判断值是否在集合内
来源：http://gvk.52xcode.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://acs.gogol.net.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://yoi.xingfuxueyuan.xyz

JS:   [1, 2, 3].includes(x)
来源：http://hvn.yuxming.cn

TS:   [1, 2, 3].includes(x)
来源：http://aau.jiagoushi.top

Java: List.of(1, 2, 3).contains(x)
来源：http://fpo.smart0.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://bmd.shanyushiyangtech.top

Ruby: [1, 2, 3].include?(x)
来源：http://mlw.zhixingplan.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://eyn.mhx1999.top

[B15] 布尔运算与取反
来源：http://yni.cqqwz.cn

Py:   a and b or not c
来源：http://mwj.mhx1999.top

PHP:  $a && $b || !$c
来源：http://tln.fehbvm.com

JS:   a && b || !c
来源：http://jsj.dianchejie.cn

TS:   a && b || !c
来源：http://xbj.snrcjt.cn

Java: a && b || !c
来源：http://yoi.yangfankeji.com

Go:   a && b || !c
来源：http://bxj.kuanghao11.cn

Ruby: a && b || !c
来源：http://yrt.pycfn.com

C#:   a && b || !c
来源：http://rxx.fehbvm.com

[B16] 卫语句：不满足条件提前返回
来源：http://rkg.xuetiantiany.cn

Py:   if not data: return
来源：http://fih.yueranfly.top

PHP:  if (!$data) { return; }
来源：http://tmu.xuetiantiany.cn

JS:   if (!data) return;
来源：http://elw.52xcode.cn

TS:   if (!data) return;
来源：http://ukr.bjfxy.top

Java: if (data == null) return;
来源：http://zgd.uphjek.com

Go:   if data == nil { return }
来源：http://vgd.jinqigfzy.top

Ruby: return if data.nil?
来源：http://gih.jiagoushi.top

C#:   if (data == null) return;
来源：http://fii.jinqigfzy.top

================================================================================
来源：http://gyq.ywan-chungtsiang.top

C. 函数与作用域
来源：http://fpo.hcnkem.com

================================================================================
来源：http://mjg.feifeiyinyue.top

[C01] 定义函数
来源：http://pwe.sxryk.cn

Py:   def add(a, b): return a + b
来源：http://rtr.jiagoushi.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blo.ywan-chungtsiang.top

JS:   function add(a, b) { return a + b; }
来源：http://xpi.xuanzx.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hio.yanxiufei.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://aoc.nanxinkj.top

Go:   func add(a, b int) int { return a + b }
来源：http://agt.cdnleiting.top

Ruby: def add(a, b); a + b; end
来源：http://vsz.shanyushiyangtech.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://dzd.daria6918.cn

[C02] 默认参数
来源：http://cqq.cdnleiting.top

Py:   def greet(name="World"): return name
来源：http://buz.c1oappe.top

PHP:  function greet($name = "World") { return $name; }
来源：http://jkr.tian-w.cn

JS:   function greet(name = "World") { return name; }
来源：http://hmb.gaohongyu789.top

TS:   function greet(name: string = "World") { return name; }
来源：http://jte.yfazqb.com

Java: // 无默认参数：方法重载或 Optional
来源：http://nwj.hysaishi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ner.tian-w.cn

Ruby: def greet(name = "World") = name
来源：http://dxl.guowangkeji.top

C#:   string Greet(string name = "World") => name;
来源：http://hum.chenlongwang.top

[C03] 可变参数
来源：http://oxa.jyoumei.cn

Py:   def total(*args): return sum(args)
来源：http://uwq.hywenlv.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://zdf.wangdashe.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://dnp.zhongyouzk.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://jlm.fzhhl.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://kgs.zhijiandao.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://xfj.yuxming.cn

Ruby: def total(*nums); nums.sum; end
来源：http://dow.yj20258888.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://qrj.jyoumei.cn

[C04] 命名参数 / 关键字参数
来源：http://uov.shzxlz.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://vwp.zhixingplan.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://naf.aizwys.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://jfk.yj20258888.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ojq.jinghuilouyu.cn

Java: // 无：用 Builder 模式或 record
来源：http://gfd.tanke756.top

Go:   // 无：用配置结构体参数
来源：http://oad.kuanghao11.cn

Ruby: f(a: 1, b: 2)
来源：http://beg.xuanzx.com

C#:   f(a: 1, b: 2)
来源：http://kzf.guannengcc.top

[C05] 返回多个值
来源：http://zdn.haohaochexian.top

Py:   return a, b
来源：http://lrt.zhaomingkeji.xyz

PHP:  return [$a, $b];
来源：http://czc.guannengcc.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://yiq.ywan-chungtsiang.top

TS:   return { a, b };
来源：http://lba.yfazqb.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://yud.svipenyu.cn

Go:   return a, b
来源：http://wmk.sjlbkw.cn

Ruby: return a, b
来源：http://rtj.jinghuilouyu.cn

C#:   return (a, b);              // ValueTuple
来源：http://rzk.jlsjyb.cn

[C06] 匿名函数 / lambda
来源：http://cna.feifeiyinyue.top

Py:   square = lambda x: x * x
来源：http://zva.yfazqb.com

PHP:  $square = fn($x) => $x * $x;
来源：http://uby.zhoulong.xyz

JS:   const square = x => x * x;
来源：http://mef.vqdsnc.cn

TS:   const square = (x: number): number => x * x;
来源：http://yqw.hysaishi.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://aly.wangdashe.top

Go:   sq := func(x int) int { return x * x }
来源：http://ysa.yvedp.cn

Ruby: square = ->(x) { x * x }
来源：http://yop.dianchejie.cn

C#:   Func<int, int> square = x => x * x;
来源：http://jvc.hesvh.cn

[C07] 把函数作为参数传入
来源：http://xwf.hfpthk.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://gpp.fktsv.cn

PHP:  array_map("strtoupper", $arr);
来源：http://wkg.shzxlz.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://dva.fktsv.cn

TS:   arr.map(String)
来源：http://tqc.vehdjk.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://bfm.yfazqb.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://bme.uphjek.com

Ruby: arr.map(&:upcase)
来源：http://trf.yj20258888.top

C#:   arr.Select(s => s.ToUpper())
来源：http://gdn.xylfe.cn

[C08] 闭包
来源：http://xhq.tian-w.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://bqt.redwolf501.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://jof.mhx1999.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://feb.yj202588.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://jtm.yuxming.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://nox.quarkkingdee.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://qsi.yvedp.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://cge.aizwys.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://etp.tian-w.cn

[C09] 递归
来源：http://vyn.dashuyun.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hmg.nanxuanxn.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://xen.ybcxt.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hrv.zdqjudy.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hxk.uphjek.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://glh.smart0.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mbm.ybcxt.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xcj.cashguo.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://nie.fengsongda.top

[C10] 变量作用域
来源：http://bvy.shanyushiyangtech.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ota.shanyushiyangkeji.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ilm.zhiwuduotai.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://lzh.cashguo.top

TS:   同 JS
来源：http://eqb.yfazqb.com

Java: 方法内为块级作用域
来源：http://rhp.sufxvd.cn

Go:   花括号块级作用域
来源：http://vma.yueranfly.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://unw.ehwqpu.com

C#:   块级作用域
来源：http://nxl.jqgfzy.top

[C11] 模块导入与导出
来源：http://ego.52xcode.cn

Py:   from module import func
来源：http://ehe.guannengcc.top

PHP:  require "file.php";  或 use App\Service;
来源：http://dcj.hcnkem.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://wgt.haohaochexian.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://sgl.fanxiaobao.xyz

Java: import java.util.List;
来源：http://gub.smart0.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://vfb.aizwys.cn

Ruby: require "json"; require_relative "./util"
来源：http://mrx.cashguo.top

C#:   using System.Text;
来源：http://kbk.feifeiyinyue.top

[C12] 立即执行函数 IIFE
来源：http://zxx.ctjpmb.com

Py:   (lambda: print("run"))()
来源：http://cdz.hywenlv.cn

PHP:  (function () { echo "run"; })();
来源：http://hnb.jinghuilouyu.cn

JS:   (() => { console.log("run"); })();
来源：http://kha.cqqwz.cn

TS:   (() => { console.log("run"); })();
来源：http://kur.jianghu66.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jwv.andypj.xyz

Go:   func() { fmt.Println("run") }()
来源：http://obm.cashguo.top

Ruby: -> { puts "run" }.call
来源：http://rya.hesvh.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://jdw.fzhhl.top

[C13] 类型声明 / 类型注解
来源：http://wyr.wangshuangyany.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://rfx.zhiwuduotai.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yss.hywenlv.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://pps.fengsongda.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ajx.cheryme.top

Java: int add(int a, int b) { return a + b; }
来源：http://juj.smart0.xyz

Go:   func add(a, b int) int
来源：http://knc.zhaomingkeji.xyz

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mks.jqgufenzy.top

C#:   int Add(int a, int b) => a + b;
来源：http://dwr.9152youxi.cn

[C14] 泛型函数
来源：http://cbw.wangdashe.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://nrc.jyoumei.cn

PHP:  // 无泛型
来源：http://gif.c1oappe.top

JS:   // 无泛型
来源：http://dzy.52xcode.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://nxu.chenjidiqi.icu

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wnt.gaohongyu789.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://euh.yfazqb.com

Ruby: # 无泛型
来源：http://bap.nwbrower.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://djw.fengsongda.top

[C15] 解构 / 展开参数
来源：http://jlw.jiagoushi.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://yia.jyoumei.cn

PHP:  [$a, $b] = $pair;
来源：http://czl.smart0.xyz

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://uol.wangdashe.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wer.fanxiaobao.xyz

Java: // 无解构
来源：http://gvx.316326.xyz

Go:   // 无解构
来源：http://krn.guowangkeji.top

Ruby: a, b = pair
来源：http://uuv.jianghu66.top

C#:   var (a, b) = pair;
来源：http://ufp.xuetiantiany.cn

[C16] 函数 / 方法重载
来源：http://qya.hesvh.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://rre.gaohongyu789.top

PHP:  // 无重载
来源：http://kvd.jqgfzy.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://fwy.zhijiandao.cn

TS:   // 用联合类型或重载签名声明
来源：http://xrk.fktsv.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://zjw.jlsjyb.cn

Go:   // 无重载：用不同函数名
来源：http://upd.shanyushiyangkeji.top

Ruby: # 无重载：靠动态参数
来源：http://ppe.fehbvm.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://mnk.iojbl.cn

================================================================================
来源：http://uez.xziqi.cn

D. 数组 / 列表 / 集合
来源：http://sdx.gogol.net.cn

================================================================================
来源：http://htc.quarkkingdee.top

[D01] 创建数组 / 列表
来源：http://stl.xylfe.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://sid.cdnleiting.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ndq.shanyushiyangkeji.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://gle.jlsjyb.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://fbc.quarkkingdee.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://yft.chenzaomai.com

Go:   arr := []int{1, 2, 3}
来源：http://kvv.wangshuangyany.cn

Ruby: arr = [1, 2, 3]
来源：http://yby.zhengqikj.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://jin.jqgfzy.top

[D02] 追加元素到末尾
来源：http://ghg.tanke756.top


<!-- 参考信息 -->