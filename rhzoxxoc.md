代发 wailian999

C#:   var r = x > 0 ? "正" : "非正";
来源：http://awh.gogol.net.cn

[B02] 多分支 else if / elif
来源：http://svm.sweek.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://fqc.hammf.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://vmn.ctjpmb.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vig.c1oappe.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zuh.aizwys.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://agy.chenzaomai.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://zbs.xylfe.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://vma.52xcode.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wwh.hammf.cn

[B03] switch / match / case
来源：http://peh.316326.xyz

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://aot.tarul.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://nbd.shangyingyoupin.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://amj.cqqwz.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wdv.snrcjt.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://epn.nanxuanxn.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hqw.chenzaomai.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://oqd.yj20258.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://seq.hywenlv.cn

[B04] for 计数循环
来源：http://iop.tian-w.cn

Py:   for i in range(10): print(i)
来源：http://zec.jinqigfzy.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://yqz.yvedp.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mcg.kuanghao11.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cba.redwolf501.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://tmv.aizwys.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://jbt.zhongyouzk.top

Ruby: 10.times { |i| puts i }
来源：http://uly.hysaishi.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://top.9152youxi.cn

[B05] 遍历数组 / 列表
来源：http://cgi.hammf.cn

Py:   for item in arr: print(item)
来源：http://dqx.tarul.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://nzz.cheryme.top

JS:   for (const item of arr) { console.log(item); }
来源：http://ruj.fanxiaobao.xyz

TS:   for (const item of arr) { console.log(item); }
来源：http://bnb.sweek.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://uyb.tarul.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wyw.xuanzx.com

Ruby: arr.each { |item| puts item }
来源：http://beu.hnxiangtu.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wps.yj20258888.top

[B06] 遍历字典 / 对象
来源：http://elk.yuxming.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://tdx.epnwcf.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://pso.shanyushiyangtech.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bpn.xuanzx.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qxo.cqqwz.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ndv.cdnleiting.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://vpe.redwolf501.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://agp.svipenyu.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://lly.zhixingplan.top

[B07] while 循环
来源：http://olx.shuidangran.top

Py:   while i < 10: i += 1
来源：http://xil.jlsjyb.cn

PHP:  while ($i < 10) { $i++; }
来源：http://iwz.sxryk.cn

JS:   while (i < 10) { i++; }
来源：http://uio.hysaishi.cn

TS:   while (i < 10) { i++; }
来源：http://szd.gaohongyu789.top

Java: while (i < 10) { i++; }
来源：http://sxt.cqqwz.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://llb.xziqi.cn

Ruby: while i < 10; i += 1; end
来源：http://urd.haohaochexian.top

C#:   while (i < 10) { i++; }
来源：http://ose.hywenlv.cn

[B08] do-while（至少执行一次）
来源：http://wsz.jqgufenzy.top

Py:   # 无 do-while：用 while True + break
来源：http://snz.fengsongda.top

PHP:  do { $i++; } while ($i < 10);
来源：http://zrq.ywan-chungtsiang.top

JS:   do { i++; } while (i < 10);
来源：http://hux.hammf.cn

TS:   do { i++; } while (i < 10);
来源：http://gbt.fehbvm.com

Java: do { i++; } while (i < 10);
来源：http://gig.zdbjq.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://mue.52xcode.cn

Ruby: begin; i += 1; end while i < 10
来源：http://heu.zycfv.cn

C#:   do { i++; } while (i < 10);
来源：http://nmq.zhongyouzk.top

[B09] break 与 continue
来源：http://xqd.yuxming.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://rdj.pycfn.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://oys.xuetiantiany.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tsg.9152youxi.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tpj.xingfuxueyuan.xyz

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dlr.chenjidiqi.icu

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://vbb.chenlongwang.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://pmd.cdnleiting.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eeg.ehwqpu.com

[B10] 遍历同时拿索引
来源：http://jog.ywan-chungtsiang.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://dgb.wangdashe.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ozh.zhongyouzk.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://fwb.jqgufenzy.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://eiq.meibo888.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://rnt.nwbrower.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://xzm.zhongyouzk.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ewx.hnqzz.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://swb.tianlin.xyz

[B11] 生成数字序列 / 区间
来源：http://elv.quarkkingdee.top

Py:   list(range(0, 10, 2))
来源：http://rqr.nanxuanxn.top

PHP:  range(0, 10, 2);
来源：http://ngf.jyoumei.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gik.yonumen.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://twj.tianlin.xyz

Java: IntStream.range(0, 10).boxed().toList()
来源：http://yrt.havefunace.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mly.vqdsnc.cn

Ruby: (0...10).step(2).to_a
来源：http://xcw.yuxming.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wsf.yj202588.top

[B12] 跳出多层循环
来源：http://ccw.andypj.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://nty.mhx1999.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://gbd.yonumen.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://bgl.meibo888.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ebq.yuxming.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://lnw.fktsv.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://nsg.hfpthk.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ztu.dianchejie.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://aum.ywan-chungtsiang.top

[B13] 判断是否为数字
来源：http://hmv.jinqigfzy.top

Py:   isinstance(x, (int, float))
来源：http://uqp.tian-w.cn

PHP:  is_numeric($x)
来源：http://xbm.0kj1m.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nwj.ydzc1.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://alr.ppjwa.cn

Java: x instanceof Number
来源：http://kng.sweek.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mdu.zycfv.cn

Ruby: x.is_a?(Numeric)
来源：http://vuk.wangdashe.top

C#:   x is int or double or decimal
来源：http://baz.fzhhl.top

[B14] 判断值是否在集合内
来源：http://zyu.jinqigufen.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://yio.daxiang520.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://yhy.yongpay.top

JS:   [1, 2, 3].includes(x)
来源：http://yax.zhiwuduotai.top

TS:   [1, 2, 3].includes(x)
来源：http://gzv.daria6918.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://iad.sweek.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://xwm.nanxinkj.top

Ruby: [1, 2, 3].include?(x)
来源：http://tiz.hcnkem.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://rju.9152youxi.cn

[B15] 布尔运算与取反
来源：http://xba.bbcook.cn

Py:   a and b or not c
来源：http://jej.c1oappe.top

PHP:  $a && $b || !$c
来源：http://mbv.jqgfzy.top

JS:   a && b || !c
来源：http://iyp.hammf.cn

TS:   a && b || !c
来源：http://byr.ybcxt.top

Java: a && b || !c
来源：http://xim.haohaochexian.top

Go:   a && b || !c
来源：http://jed.shanyushiyangtech.top

Ruby: a && b || !c
来源：http://bqk.jiagoushi.top

C#:   a && b || !c
来源：http://kik.zdqjudy.top

[B16] 卫语句：不满足条件提前返回
来源：http://kbi.wangdashe.top

Py:   if not data: return
来源：http://oti.yuxming.cn

PHP:  if (!$data) { return; }
来源：http://ojc.yangfankeji.com

JS:   if (!data) return;
来源：http://dxg.ydjk.org.cn

TS:   if (!data) return;
来源：http://bik.zycfv.cn

Java: if (data == null) return;
来源：http://aqi.birdmap.top

Go:   if data == nil { return }
来源：http://ewb.aibaodan.cn

Ruby: return if data.nil?
来源：http://vtd.xingfuxueyuan.xyz

C#:   if (data == null) return;
来源：http://uhb.yvedp.cn

================================================================================
来源：http://ykc.quarkkingdee.top

C. 函数与作用域
来源：http://gbo.yuanzhike.top

================================================================================
来源：http://lat.haohaochexian.top

[C01] 定义函数
来源：http://nki.wangdashe.top

Py:   def add(a, b): return a + b
来源：http://qkd.zhixingplan.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xqb.ybcxt.top

JS:   function add(a, b) { return a + b; }
来源：http://dwt.gogol.net.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ktv.gotoacloud.top

Java: static int add(int a, int b) { return a + b; }
来源：http://cyo.tarul.cn

Go:   func add(a, b int) int { return a + b }
来源：http://sph.sxryk.cn

Ruby: def add(a, b); a + b; end
来源：http://hkb.gaohongyu789.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://gei.vqdsnc.cn

[C02] 默认参数
来源：http://rzy.xingfuxueyuan.xyz

Py:   def greet(name="World"): return name
来源：http://qbt.0kj1m.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ytw.fehbvm.com

JS:   function greet(name = "World") { return name; }
来源：http://kic.gotoacloud.top

TS:   function greet(name: string = "World") { return name; }
来源：http://vlt.xuetiantiany.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://vwh.zhongyouzk.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://pxk.birdmap.top

Ruby: def greet(name = "World") = name
来源：http://tza.pengpengdd.cyou

C#:   string Greet(string name = "World") => name;
来源：http://ajw.vehdjk.com

[C03] 可变参数
来源：http://syx.ydzc1.top

Py:   def total(*args): return sum(args)
来源：http://qne.gotoacloud.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ivt.sufxvd.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://toe.jinqigufen.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ixg.aizwys.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://yes.daria6918.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hxf.kuanghao11.cn

Ruby: def total(*nums); nums.sum; end
来源：http://dnz.birdmap.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://sgx.cheryme.top

[C04] 命名参数 / 关键字参数
来源：http://rif.yj20258888.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://cib.yangfankeji.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ajh.vehdjk.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xvi.jinqigfzy.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://dtt.hywenlv.cn

Java: // 无：用 Builder 模式或 record
来源：http://xyo.yj202588.top

Go:   // 无：用配置结构体参数
来源：http://ogl.yfazqb.com

Ruby: f(a: 1, b: 2)
来源：http://unj.mhx1999.top

C#:   f(a: 1, b: 2)
来源：http://ztj.yj20258.top

[C05] 返回多个值
来源：http://vic.bjfxy.top

Py:   return a, b
来源：http://qgr.vehdjk.com

PHP:  return [$a, $b];
来源：http://zqj.yanxiufei.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://eas.hysaishi.cn

TS:   return { a, b };
来源：http://ysd.xuanzx.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://tri.cucudq.cn

Go:   return a, b
来源：http://qks.jinghuilouyu.cn

Ruby: return a, b
来源：http://xuc.cqqwz.cn

C#:   return (a, b);              // ValueTuple
来源：http://kya.ppjwa.cn

[C06] 匿名函数 / lambda
来源：http://gfg.wangdashe.top

Py:   square = lambda x: x * x
来源：http://byf.shanyushiyangkeji.top

PHP:  $square = fn($x) => $x * $x;
来源：http://swr.wangshuangyany.cn

JS:   const square = x => x * x;
来源：http://fcn.feifeiyinyue.top

TS:   const square = (x: number): number => x * x;
来源：http://znw.shanyushiyangtech.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mgn.meibo888.top

Go:   sq := func(x int) int { return x * x }
来源：http://qwc.vehdjk.com

Ruby: square = ->(x) { x * x }
来源：http://jgu.svipenyu.cn

C#:   Func<int, int> square = x => x * x;
来源：http://dlq.jlsjyb.cn

[C07] 把函数作为参数传入
来源：http://nkc.hnqzz.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://zqd.aibaodan.cn

PHP:  array_map("strtoupper", $arr);
来源：http://bql.fzhhl.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://fid.sysykeji.top

TS:   arr.map(String)
来源：http://efk.jqgfzy.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://tqw.tarul.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ejl.fehbvm.com

Ruby: arr.map(&:upcase)
来源：http://gjj.zhoulong.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://dfw.cheryme.top

[C08] 闭包
来源：http://qwr.fengsongda.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://tha.jinghuilouyu.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://bac.zdqjudy.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://dyz.hywenlv.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://def.yuanzhike.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://bef.zdqjudy.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://vtw.bbcook.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wrq.ydjk.org.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://est.iojbl.cn

[C09] 递归
来源：http://ssd.xylfe.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://sjm.feifeiyinyue.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://fcc.xinyue.icu

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gtb.guannengcc.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ykj.dashuyun.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://uuy.xuetiantiany.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hcc.sjlbkw.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xik.shangyingyoupin.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://kkv.fengsongda.top

[C10] 变量作用域
来源：http://cft.hongshengwenyu.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ebj.cashguo.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://heg.vehdjk.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://zoy.yuanzhike.top

TS:   同 JS
来源：http://khq.epnwcf.com

Java: 方法内为块级作用域
来源：http://daa.yangfankeji.com

Go:   花括号块级作用域
来源：http://ajg.hammf.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://fgq.zhongyouzk.top

C#:   块级作用域
来源：http://inw.epnwcf.com

[C11] 模块导入与导出
来源：http://svs.ivvv.top

Py:   from module import func
来源：http://euz.zdbjq.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://mnx.zhoulong.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://nkf.quarkkingdee.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ijs.0kj1m.cn

Java: import java.util.List;
来源：http://wxm.tian-w.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://azy.iojbl.cn

Ruby: require "json"; require_relative "./util"
来源：http://eeh.tanke756.top

C#:   using System.Text;
来源：http://nge.jinyuanbaomall.cn

[C12] 立即执行函数 IIFE
来源：http://isx.chenzaomai.com

Py:   (lambda: print("run"))()
来源：http://qei.yongpay.top

PHP:  (function () { echo "run"; })();
来源：http://caq.pengpengdd.cyou

JS:   (() => { console.log("run"); })();
来源：http://hyr.mhx1999.top

TS:   (() => { console.log("run"); })();
来源：http://wmj.jiagoushi.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://eqn.sxryk.cn

Go:   func() { fmt.Println("run") }()
来源：http://zab.aibaodan.cn

Ruby: -> { puts "run" }.call
来源：http://roj.fanxiaobao.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://oyf.vehdjk.com

[C13] 类型声明 / 类型注解
来源：http://laz.gotoacloud.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://evu.jyoumei.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bqx.smart0.xyz

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ozs.hywenlv.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xar.hongshengwenyu.top

Java: int add(int a, int b) { return a + b; }
来源：http://vve.tarul.cn

Go:   func add(a, b int) int
来源：http://amv.zycfv.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wuz.c1oappe.top

C#:   int Add(int a, int b) => a + b;
来源：http://way.xinyue.icu

[C14] 泛型函数
来源：http://ynm.nwbrower.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mgb.yanxiufei.cn

PHP:  // 无泛型
来源：http://xas.shanyushiyangtech.top

JS:   // 无泛型
来源：http://jvt.gaohongyu789.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://uyn.vehdjk.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://buk.yueranfly.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://obg.shangyingyoupin.top

Ruby: # 无泛型
来源：http://jqm.sjlbkw.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xbs.vehdjk.com

[C15] 解构 / 展开参数
来源：http://mbk.fengsongda.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://bsx.fzhhl.top

PHP:  [$a, $b] = $pair;
来源：http://vbb.yuanzhike.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://gsc.andypj.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wke.aizwys.cn

Java: // 无解构
来源：http://lor.ehwqpu.com

Go:   // 无解构
来源：http://dcb.yuxming.cn

Ruby: a, b = pair
来源：http://pnt.haohaochexian.top

C#:   var (a, b) = pair;
来源：http://zhh.tianlin.xyz

[C16] 函数 / 方法重载
来源：http://dtf.xuetiantiany.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ubj.xylfe.cn

PHP:  // 无重载
来源：http://pes.zhongyouzk.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://dpe.hnxiangtu.top

TS:   // 用联合类型或重载签名声明
来源：http://ksr.shanyushiyangtech.top

Java: void f(int a) {}  void f(String a) {}
来源：http://kvy.ydzc1.top

Go:   // 无重载：用不同函数名
来源：http://mwt.dianchejie.cn

Ruby: # 无重载：靠动态参数
来源：http://etm.svipenyu.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://mpk.yuanzhike.top

================================================================================
来源：http://bav.jyoumei.cn

D. 数组 / 列表 / 集合
来源：http://iiu.9152youxi.cn

================================================================================
来源：http://rze.zhijiandao.cn

[D01] 创建数组 / 列表
来源：http://dnn.hongshengwenyu.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://wrr.zhiwuduotai.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://vnc.hnxiangtu.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://jgu.uphjek.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://ibh.yonumen.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hnb.sweek.top

Go:   arr := []int{1, 2, 3}
来源：http://skr.xylfe.cn

Ruby: arr = [1, 2, 3]
来源：http://zss.tian-w.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://agw.wangshuangyany.cn

[D02] 追加元素到末尾
来源：http://sll.vqdsnc.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://gmh.ydzc1.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mcp.vqdsnc.cn

JS:   arr.push(4);
来源：http://vgd.feifeiyinyue.top

TS:   arr.push(4);
来源：http://pjx.yuxming.cn


<!-- 参考信息 -->