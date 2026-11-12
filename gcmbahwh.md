代发 wailian999

C#:   var r = x > 0 ? "正" : "非正";
来源：http://goe.yanxiufei.cn

[B02] 多分支 else if / elif
来源：http://uuy.hnxiangtu.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://usq.nanxinkj.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ppi.hnqzz.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cyl.sufxvd.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gor.hnxiangtu.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nxg.ctjpmb.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://moh.gaohongyu789.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://kxb.c1oappe.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lrn.smart0.xyz

[B03] switch / match / case
来源：http://gvv.quarkkingdee.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://pjt.svipenyu.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mdc.dianchejie.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kpv.aibaodan.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://sqa.gotoacloud.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://axt.bbcook.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ymk.kuanghao11.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://pmt.sxryk.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://rau.havefunace.top

[B04] for 计数循环
来源：http://vgt.gotoacloud.top

Py:   for i in range(10): print(i)
来源：http://guk.andypj.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://pdf.chenjidiqi.icu

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sdr.zdbjq.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vxo.zhoulong.xyz

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://non.aizwys.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://bdz.bbcook.cn

Ruby: 10.times { |i| puts i }
来源：http://fnf.cdnleiting.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://xfn.bjfxy.top

[B05] 遍历数组 / 列表
来源：http://pex.snrcjt.cn

Py:   for item in arr: print(item)
来源：http://sjt.guowangkeji.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ngm.zhiwuduotai.top

JS:   for (const item of arr) { console.log(item); }
来源：http://eub.iojbl.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://zee.guowangkeji.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://qqx.wangdashe.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://rsg.yuxming.cn

Ruby: arr.each { |item| puts item }
来源：http://gjg.chenzaomai.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://dbc.wangdashe.top

[B06] 遍历字典 / 对象
来源：http://vys.haohaochexian.top

Py:   for k, v in d.items(): print(k, v)
来源：http://tqe.meibo888.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ngo.zhaomingkeji.xyz

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pfi.tian-w.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tgc.andypj.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://lnk.jqgfzy.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hue.hnxiangtu.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://nqi.sxryk.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ilu.nanxinkj.top

[B07] while 循环
来源：http://qzk.birdmap.top

Py:   while i < 10: i += 1
来源：http://jsv.fzhhl.top

PHP:  while ($i < 10) { $i++; }
来源：http://qjg.mhx1999.top

JS:   while (i < 10) { i++; }
来源：http://wzo.hnqzz.top

TS:   while (i < 10) { i++; }
来源：http://loh.hesvh.cn

Java: while (i < 10) { i++; }
来源：http://wwk.wangdashe.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://fam.jlsjyb.cn

Ruby: while i < 10; i += 1; end
来源：http://dto.c1oappe.top

C#:   while (i < 10) { i++; }
来源：http://upr.fehbvm.com

[B08] do-while（至少执行一次）
来源：http://orq.jinqigfzy.top

Py:   # 无 do-while：用 while True + break
来源：http://vzu.hfpthk.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://mvr.cheryme.top

JS:   do { i++; } while (i < 10);
来源：http://nyv.daria6918.cn

TS:   do { i++; } while (i < 10);
来源：http://cjr.52xcode.cn

Java: do { i++; } while (i < 10);
来源：http://wag.zhongyouzk.top

Go:   for { i++; if i >= 10 { break } }
来源：http://rrx.cucudq.cn

Ruby: begin; i += 1; end while i < 10
来源：http://cjc.pengpengdd.cyou

C#:   do { i++; } while (i < 10);
来源：http://qcr.fanxiaobao.xyz

[B09] break 与 continue
来源：http://tpg.zdqjudy.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ydh.tarul.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hxs.ydzc1.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ywy.yfazqb.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://msm.nwbrower.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jtd.jinqigufen.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://fns.zhoulong.xyz

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://bbi.yongpay.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wnp.9152youxi.cn

[B10] 遍历同时拿索引
来源：http://lwl.hongshengwenyu.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://pwe.wangdashe.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://nir.svipenyu.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wmn.ppjwa.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://oty.jiagoushi.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://qcv.zhaomingkeji.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wwt.jqgfzy.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hld.svipenyu.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ahz.hnqzz.top

[B11] 生成数字序列 / 区间
来源：http://rvk.zdbjq.cn

Py:   list(range(0, 10, 2))
来源：http://pqp.meibo888.top

PHP:  range(0, 10, 2);
来源：http://ibl.sysykeji.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nai.jqgufenzy.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://auo.fehbvm.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://zfs.shzxlz.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ynx.zdqjudy.top

Ruby: (0...10).step(2).to_a
来源：http://fuj.quarkkingdee.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zbw.gogol.net.cn

[B12] 跳出多层循环
来源：http://mqc.jinqigufen.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://dlc.yanxiufei.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://cwj.feifeiyinyue.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hxx.xuetiantiany.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://dhg.quarkkingdee.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mgy.cdnleiting.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://jeu.hnqzz.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://kah.chenzaomai.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://dmy.jianghu66.top

[B13] 判断是否为数字
来源：http://udr.vehdjk.com

Py:   isinstance(x, (int, float))
来源：http://awr.mhx1999.top

PHP:  is_numeric($x)
来源：http://rlz.jlsjyb.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://emp.xuetiantiany.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dau.bjfxy.top

Java: x instanceof Number
来源：http://dct.chenjidiqi.icu

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://dbz.0kj1m.cn

Ruby: x.is_a?(Numeric)
来源：http://bjz.aizwys.cn

C#:   x is int or double or decimal
来源：http://dzf.zhengqikj.top

[B14] 判断值是否在集合内
来源：http://wye.ywan-chungtsiang.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://uvk.pycfn.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://pcv.meibo888.top

JS:   [1, 2, 3].includes(x)
来源：http://ppb.yanxiufei.cn

TS:   [1, 2, 3].includes(x)
来源：http://ipp.yj202588.top

Java: List.of(1, 2, 3).contains(x)
来源：http://ebw.jinqigfzy.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://atb.chenzaomai.com

Ruby: [1, 2, 3].include?(x)
来源：http://hai.hywenlv.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://dum.chenzaomai.com

[B15] 布尔运算与取反
来源：http://vxm.birdmap.top

Py:   a and b or not c
来源：http://ofv.yvedp.cn

PHP:  $a && $b || !$c
来源：http://bjs.pycfn.com

JS:   a && b || !c
来源：http://ucy.zycfv.cn

TS:   a && b || !c
来源：http://uiw.shzxlz.cn

Java: a && b || !c
来源：http://rok.sufxvd.cn

Go:   a && b || !c
来源：http://ais.zhiwuduotai.top

Ruby: a && b || !c
来源：http://pzc.zhengqikj.top

C#:   a && b || !c
来源：http://qbc.nwbrower.top

[B16] 卫语句：不满足条件提前返回
来源：http://rvh.vqdsnc.cn

Py:   if not data: return
来源：http://sxo.zycfv.cn

PHP:  if (!$data) { return; }
来源：http://sua.iojbl.cn

JS:   if (!data) return;
来源：http://vkd.nanxuanxn.top

TS:   if (!data) return;
来源：http://gpk.ctjpmb.com

Java: if (data == null) return;
来源：http://jmw.shanyushiyangkeji.top

Go:   if data == nil { return }
来源：http://bnn.vehdjk.com

Ruby: return if data.nil?
来源：http://jdw.zhijiandao.cn

C#:   if (data == null) return;
来源：http://fhd.wangdashe.top

================================================================================
来源：http://grc.hysaishi.cn

C. 函数与作用域
来源：http://omu.zhengqikj.top

================================================================================
来源：http://jlz.zycfv.cn

[C01] 定义函数
来源：http://xox.zhoulong.xyz

Py:   def add(a, b): return a + b
来源：http://fpv.zhiwuduotai.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sri.jianghu66.top

JS:   function add(a, b) { return a + b; }
来源：http://dau.sufxvd.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ake.hesvh.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://uis.hongshengwenyu.top

Go:   func add(a, b int) int { return a + b }
来源：http://dyo.sjlbkw.cn

Ruby: def add(a, b); a + b; end
来源：http://teo.kuanghao11.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wjo.sufxvd.cn

[C02] 默认参数
来源：http://bar.andypj.xyz

Py:   def greet(name="World"): return name
来源：http://dqr.chenjidiqi.icu

PHP:  function greet($name = "World") { return $name; }
来源：http://xow.fzhhl.top

JS:   function greet(name = "World") { return name; }
来源：http://zml.chenlongwang.top

TS:   function greet(name: string = "World") { return name; }
来源：http://ysv.zhijiandao.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://rle.yj202588.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://glu.ydzc1.top

Ruby: def greet(name = "World") = name
来源：http://uwh.kuanghao11.cn

C#:   string Greet(string name = "World") => name;
来源：http://xuz.jinqigufen.top

[C03] 可变参数
来源：http://wtu.tianlin.xyz

Py:   def total(*args): return sum(args)
来源：http://ggu.yj20258888.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://zke.kuanghao11.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hlw.pycfn.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://abe.cucudq.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://zqs.c1oappe.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://lkc.yfazqb.com

Ruby: def total(*nums); nums.sum; end
来源：http://msp.bbcook.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zvj.nanxinkj.top

[C04] 命名参数 / 关键字参数
来源：http://eou.jianghu66.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://eli.shangyingyoupin.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://sey.zdbjq.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hir.jinghuilouyu.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://lmw.svipenyu.cn

Java: // 无：用 Builder 模式或 record
来源：http://zpf.xylfe.cn

Go:   // 无：用配置结构体参数
来源：http://nwj.jinqigfzy.top

Ruby: f(a: 1, b: 2)
来源：http://kje.jinqigufen.top

C#:   f(a: 1, b: 2)
来源：http://fio.sysykeji.top

[C05] 返回多个值
来源：http://fpo.meibo888.top

Py:   return a, b
来源：http://lvc.mhx1999.top

PHP:  return [$a, $b];
来源：http://ouv.vqdsnc.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://mpp.jyoumei.cn

TS:   return { a, b };
来源：http://dez.52xcode.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://dab.jlsjyb.cn

Go:   return a, b
来源：http://dyt.yfazqb.com

Ruby: return a, b
来源：http://uif.yueranfly.top

C#:   return (a, b);              // ValueTuple
来源：http://cwt.feifeiyinyue.top

[C06] 匿名函数 / lambda
来源：http://typ.xingfuxueyuan.xyz

Py:   square = lambda x: x * x
来源：http://piw.c1oappe.top

PHP:  $square = fn($x) => $x * $x;
来源：http://kim.jianghu66.top

JS:   const square = x => x * x;
来源：http://usm.ctjpmb.com

TS:   const square = (x: number): number => x * x;
来源：http://pnx.smart0.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://eey.yanxiufei.cn

Go:   sq := func(x int) int { return x * x }
来源：http://kun.wangshuangyany.cn

Ruby: square = ->(x) { x * x }
来源：http://trf.zhijiandao.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ssf.cashguo.top

[C07] 把函数作为参数传入
来源：http://qkn.nanxinkj.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://bbg.yueranfly.top

PHP:  array_map("strtoupper", $arr);
来源：http://vry.havefunace.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xvp.sweek.top

TS:   arr.map(String)
来源：http://hzo.hcnkem.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://rfo.fanxiaobao.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://dbs.hysaishi.cn

Ruby: arr.map(&:upcase)
来源：http://psd.jlsjyb.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://cvw.nanxinkj.top

[C08] 闭包
来源：http://vab.havefunace.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://rud.hcnkem.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hzj.bjfxy.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://kdm.fehbvm.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://rux.xinyue.icu

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://qby.zhiwuduotai.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://alu.hesvh.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://zgi.ywan-chungtsiang.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://yha.hcnkem.com

[C09] 递归
来源：http://qvp.yj202588.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://nce.cashguo.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://qfb.hywenlv.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dyr.xziqi.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kzy.hfpthk.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://oex.ctjpmb.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://dya.yvedp.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://jnx.yfazqb.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ihg.gogol.net.cn

[C10] 变量作用域
来源：http://bzk.jinqigufen.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://opm.guannengcc.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://eaw.ybcxt.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://oza.vqdsnc.cn

TS:   同 JS
来源：http://hyi.gzhubu.top

Java: 方法内为块级作用域
来源：http://mei.jqgfzy.top

Go:   花括号块级作用域
来源：http://fui.yuxming.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://jqo.0kj1m.cn

C#:   块级作用域
来源：http://ymo.pengpengdd.cyou

[C11] 模块导入与导出
来源：http://tbp.tian-w.cn

Py:   from module import func
来源：http://pzt.pycfn.com

PHP:  require "file.php";  或 use App\Service;
来源：http://muc.gotoacloud.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://rva.zhengqikj.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://bui.ydzc1.top

Java: import java.util.List;
来源：http://dqz.bbcook.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://dxw.yj20258888.top

Ruby: require "json"; require_relative "./util"
来源：http://jdq.sysykeji.top

C#:   using System.Text;
来源：http://fae.yuanzhike.top

[C12] 立即执行函数 IIFE
来源：http://zxk.chenzaomai.com

Py:   (lambda: print("run"))()
来源：http://gdv.fzhhl.top

PHP:  (function () { echo "run"; })();
来源：http://nvx.sxryk.cn

JS:   (() => { console.log("run"); })();
来源：http://bfl.andypj.xyz

TS:   (() => { console.log("run"); })();
来源：http://cgc.gotoacloud.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://yvj.xylfe.cn

Go:   func() { fmt.Println("run") }()
来源：http://szd.ybcxt.top

Ruby: -> { puts "run" }.call
来源：http://blf.hcnkem.com

C#:   // 无 IIFE：用静态构造函数
来源：http://iuf.jinqigfzy.top

[C13] 类型声明 / 类型注解
来源：http://hkz.sjlbkw.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://xwz.zdqjudy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dkc.uphjek.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://enq.hywenlv.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cdq.vehdjk.com

Java: int add(int a, int b) { return a + b; }
来源：http://soz.daria6918.cn

Go:   func add(a, b int) int
来源：http://kps.yanxiufei.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://qql.aibaodan.cn

C#:   int Add(int a, int b) => a + b;
来源：http://fiz.havefunace.top

[C14] 泛型函数
来源：http://ahk.zhongyouzk.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wep.meibo888.top

PHP:  // 无泛型
来源：http://xzb.ywan-chungtsiang.top

JS:   // 无泛型
来源：http://wnp.shanyushiyangtech.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://fgd.hysaishi.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://llg.zdqjudy.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://qdb.fzhhl.top

Ruby: # 无泛型
来源：http://exr.uphjek.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://kdw.yj20258.top

[C15] 解构 / 展开参数
来源：http://jzf.shanyushiyangtech.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://qft.birdmap.top

PHP:  [$a, $b] = $pair;
来源：http://syx.jinqigufen.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ffl.kuanghao11.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hrk.andypj.xyz

Java: // 无解构
来源：http://agy.jyoumei.cn

Go:   // 无解构
来源：http://izq.pycfn.com

Ruby: a, b = pair
来源：http://kzz.fengsongda.top

C#:   var (a, b) = pair;
来源：http://byj.hywenlv.cn

[C16] 函数 / 方法重载
来源：http://qmr.haohaochexian.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://etg.iojbl.cn

PHP:  // 无重载
来源：http://ims.cdnleiting.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://ybs.havefunace.top

TS:   // 用联合类型或重载签名声明
来源：http://jwy.yanxiufei.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://fqh.hongshengwenyu.top

Go:   // 无重载：用不同函数名
来源：http://xpk.svipenyu.cn

Ruby: # 无重载：靠动态参数
来源：http://baz.ppjwa.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://qjn.xuanzx.com

================================================================================
来源：http://xvn.chenzaomai.com

D. 数组 / 列表 / 集合
来源：http://nnz.xuanzx.com

================================================================================
来源：http://vdh.jianghu66.top

[D01] 创建数组 / 列表
来源：http://uxx.feifeiyinyue.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://rvs.zhijiandao.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://vwt.xinyue.icu

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://fwx.hysaishi.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://fhz.vehdjk.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mky.chenjidiqi.icu

Go:   arr := []int{1, 2, 3}
来源：http://kuy.hnxiangtu.top

Ruby: arr = [1, 2, 3]
来源：http://xgr.iojbl.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hkf.ybcxt.top

[D02] 追加元素到末尾
来源：http://wnr.yangfankeji.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://vdo.mhx1999.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://bmr.jinqigufen.top

JS:   arr.push(4);
来源：http://scb.zhaomingkeji.xyz

TS:   arr.push(4);
来源：http://nks.sjlbkw.cn


<!-- 参考信息 -->