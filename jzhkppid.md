代发 wailian999

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jqs.zhongyouzk.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qnw.hysaishi.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ggx.wangshuangyany.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://kar.chenzaomai.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://dqk.aizwys.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pwh.chenlongwang.top

[B03] switch / match / case
来源：http://hyd.nanxuanxn.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://imp.jiagoushi.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://kji.hongshengwenyu.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rru.0kj1m.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wax.daxiang520.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://nrx.gaohongyu789.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://kpq.shanyushiyangkeji.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://loa.shangyingyoupin.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://fqr.sxryk.cn

[B04] for 计数循环
来源：http://zcs.hnqzz.top

Py:   for i in range(10): print(i)
来源：http://nxz.uphjek.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://klf.nanxuanxn.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jrp.aibaodan.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cgp.tanke756.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://tws.wangdashe.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://cmq.zhongyouzk.top

Ruby: 10.times { |i| puts i }
来源：http://ouk.vehdjk.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ypl.feifeiyinyue.top

[B05] 遍历数组 / 列表
来源：http://rts.havefunace.top

Py:   for item in arr: print(item)
来源：http://pfq.yangfankeji.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://tqu.wangdashe.top

JS:   for (const item of arr) { console.log(item); }
来源：http://lxm.zdqjudy.top

TS:   for (const item of arr) { console.log(item); }
来源：http://unh.yonumen.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://qdv.ybcxt.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://kon.cheryme.top

Ruby: arr.each { |item| puts item }
来源：http://djq.wangshuangyany.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://err.yj202588.top

[B06] 遍历字典 / 对象
来源：http://xim.wangshuangyany.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://pum.shzxlz.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://jum.dianchejie.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wyx.wangdashe.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://uew.redwolf501.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://poj.cheryme.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ihn.shuidangran.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://zfq.yvedp.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://pnw.yanxiufei.cn

[B07] while 循环
来源：http://uor.andypj.xyz

Py:   while i < 10: i += 1
来源：http://dpu.yfazqb.com

PHP:  while ($i < 10) { $i++; }
来源：http://rgd.ybcxt.top

JS:   while (i < 10) { i++; }
来源：http://zpb.hnxiangtu.top

TS:   while (i < 10) { i++; }
来源：http://cpg.yuxming.cn

Java: while (i < 10) { i++; }
来源：http://vib.birdmap.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ffs.tianlin.xyz

Ruby: while i < 10; i += 1; end
来源：http://cyw.ydjk.org.cn

C#:   while (i < 10) { i++; }
来源：http://teq.guannengcc.top

[B08] do-while（至少执行一次）
来源：http://nbz.jinyuanbaomall.cn

Py:   # 无 do-while：用 while True + break
来源：http://ylv.jyoumei.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://pke.yanxiufei.cn

JS:   do { i++; } while (i < 10);
来源：http://wmp.shzxlz.cn

TS:   do { i++; } while (i < 10);
来源：http://eal.svipenyu.cn

Java: do { i++; } while (i < 10);
来源：http://vrn.svipenyu.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://nmt.ydjk.org.cn

Ruby: begin; i += 1; end while i < 10
来源：http://wit.xuanzx.com

C#:   do { i++; } while (i < 10);
来源：http://tjd.zhixingplan.top

[B09] break 与 continue
来源：http://kyo.jianghu66.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://nfv.tian-w.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://tgy.pengpengdd.cyou

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qrr.shuidangran.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pya.pengpengdd.cyou

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://igb.smart0.xyz

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://zce.shzxlz.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://lcw.zhiwuduotai.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xgx.xingfuxueyuan.xyz

[B10] 遍历同时拿索引
来源：http://gim.wangdashe.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://rpg.aizwys.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://sug.epnwcf.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://tfd.yonumen.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://yer.zhongyouzk.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://vie.nwbrower.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mwz.wangdashe.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://lpa.jinghuilouyu.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://dbh.chenzaomai.com

[B11] 生成数字序列 / 区间
来源：http://fmb.cashguo.top

Py:   list(range(0, 10, 2))
来源：http://kmh.zdbjq.cn

PHP:  range(0, 10, 2);
来源：http://rqm.52xcode.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rqf.ivvv.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nkc.hesvh.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://kcf.fktsv.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://tbn.wangshuangyany.cn

Ruby: (0...10).step(2).to_a
来源：http://eyv.yvedp.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://brn.quarkkingdee.top

[B12] 跳出多层循环
来源：http://bmn.hammf.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://mvb.xuanzx.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://gfj.tianlin.xyz

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://zyp.meibo888.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://bmi.pengpengdd.cyou

Java: outer: for (...) { for (...) { break outer; } }
来源：http://onz.hywenlv.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://qbn.yj202588.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wvc.cashguo.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://krn.zhoulong.xyz

[B13] 判断是否为数字
来源：http://jxv.cdnleiting.top

Py:   isinstance(x, (int, float))
来源：http://ybz.9152youxi.cn

PHP:  is_numeric($x)
来源：http://mtj.meibo888.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vcb.gzhubu.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xkc.fanxiaobao.xyz

Java: x instanceof Number
来源：http://rfc.tianlin.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hxj.aizwys.cn

Ruby: x.is_a?(Numeric)
来源：http://pjc.chenlongwang.top

C#:   x is int or double or decimal
来源：http://dor.daxiang520.top

[B14] 判断值是否在集合内
来源：http://mqb.cqqwz.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ytl.tian-w.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ope.ydzc1.top

JS:   [1, 2, 3].includes(x)
来源：http://meh.jinghuilouyu.cn

TS:   [1, 2, 3].includes(x)
来源：http://lmb.zhiwuduotai.top

Java: List.of(1, 2, 3).contains(x)
来源：http://zgf.uphjek.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://nmi.yueranfly.top

Ruby: [1, 2, 3].include?(x)
来源：http://kvz.sufxvd.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://jkc.iojbl.cn

[B15] 布尔运算与取反
来源：http://mwt.epnwcf.com

Py:   a and b or not c
来源：http://qms.ctjpmb.com

PHP:  $a && $b || !$c
来源：http://wls.jinghuilouyu.cn

JS:   a && b || !c
来源：http://skm.ctjpmb.com

TS:   a && b || !c
来源：http://pwx.birdmap.top

Java: a && b || !c
来源：http://xgf.xziqi.cn

Go:   a && b || !c
来源：http://nzk.jinghuilouyu.cn

Ruby: a && b || !c
来源：http://zij.fktsv.cn

C#:   a && b || !c
来源：http://ojs.hnqzz.top

[B16] 卫语句：不满足条件提前返回
来源：http://xij.haohaochexian.top

Py:   if not data: return
来源：http://zyd.fktsv.cn

PHP:  if (!$data) { return; }
来源：http://hxk.jinyuanbaomall.cn

JS:   if (!data) return;
来源：http://rjh.yj20258.top

TS:   if (!data) return;
来源：http://zvk.ybcxt.top

Java: if (data == null) return;
来源：http://wcv.jyoumei.cn

Go:   if data == nil { return }
来源：http://scn.birdmap.top

Ruby: return if data.nil?
来源：http://qzw.jqgufenzy.top

C#:   if (data == null) return;
来源：http://nkx.feifeiyinyue.top

================================================================================
来源：http://pvr.jinqigfzy.top

C. 函数与作用域
来源：http://wee.gzhubu.top

================================================================================
来源：http://ctq.uphjek.com

[C01] 定义函数
来源：http://gkf.sjlbkw.cn

Py:   def add(a, b): return a + b
来源：http://qfj.fktsv.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jag.smart0.xyz

JS:   function add(a, b) { return a + b; }
来源：http://wvm.zhengqikj.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wxm.9152youxi.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://zqz.epnwcf.com

Go:   func add(a, b int) int { return a + b }
来源：http://pos.gogol.net.cn

Ruby: def add(a, b); a + b; end
来源：http://ehc.fengsongda.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ybb.yj202588.top

[C02] 默认参数
来源：http://nmr.zhengqikj.top

Py:   def greet(name="World"): return name
来源：http://udk.jinqigfzy.top

PHP:  function greet($name = "World") { return $name; }
来源：http://sxc.zhengqikj.top

JS:   function greet(name = "World") { return name; }
来源：http://rsf.yonumen.top

TS:   function greet(name: string = "World") { return name; }
来源：http://ijq.yuanzhike.top

Java: // 无默认参数：方法重载或 Optional
来源：http://hvm.zhiwuduotai.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ndv.sysykeji.top

Ruby: def greet(name = "World") = name
来源：http://czg.epnwcf.com

C#:   string Greet(string name = "World") => name;
来源：http://wvz.sysykeji.top

[C03] 可变参数
来源：http://ldw.aibaodan.cn

Py:   def total(*args): return sum(args)
来源：http://dep.sweek.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://pbn.shanyushiyangtech.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wxn.ydjk.org.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xyx.epnwcf.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://sjg.uphjek.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://jiy.jinyuanbaomall.cn

Ruby: def total(*nums); nums.sum; end
来源：http://xdd.ydjk.org.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://lls.pengpengdd.cyou

[C04] 命名参数 / 关键字参数
来源：http://bdx.gaohongyu789.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://vdu.zdbjq.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://sfp.hywenlv.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://vem.guowangkeji.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://svo.wangshuangyany.cn

Java: // 无：用 Builder 模式或 record
来源：http://qjb.tianlin.xyz

Go:   // 无：用配置结构体参数
来源：http://izn.ydzc1.top

Ruby: f(a: 1, b: 2)
来源：http://hct.0kj1m.cn

C#:   f(a: 1, b: 2)
来源：http://bpt.andypj.xyz

[C05] 返回多个值
来源：http://dmh.zhijiandao.cn

Py:   return a, b
来源：http://bpm.yanxiufei.cn

PHP:  return [$a, $b];
来源：http://sac.fktsv.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://pcs.chenzaomai.com

TS:   return { a, b };
来源：http://dib.kuanghao11.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://uee.hongshengwenyu.top

Go:   return a, b
来源：http://nrz.shanyushiyangtech.top

Ruby: return a, b
来源：http://lyc.tian-w.cn

C#:   return (a, b);              // ValueTuple
来源：http://gzr.52xcode.cn

[C06] 匿名函数 / lambda
来源：http://pfy.zhongyouzk.top

Py:   square = lambda x: x * x
来源：http://hma.jyoumei.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://cob.jqgufenzy.top

JS:   const square = x => x * x;
来源：http://zie.zhijiandao.cn

TS:   const square = (x: number): number => x * x;
来源：http://hjd.c1oappe.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://cwq.yuanzhike.top

Go:   sq := func(x int) int { return x * x }
来源：http://drz.mhx1999.top

Ruby: square = ->(x) { x * x }
来源：http://ugf.tian-w.cn

C#:   Func<int, int> square = x => x * x;
来源：http://pde.hnxiangtu.top

[C07] 把函数作为参数传入
来源：http://oyd.0kj1m.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mvh.yangfankeji.com

PHP:  array_map("strtoupper", $arr);
来源：http://cvx.xuanzx.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://gea.redwolf501.top

TS:   arr.map(String)
来源：http://fyd.ivvv.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://fym.smart0.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qhy.jianghu66.top

Ruby: arr.map(&:upcase)
来源：http://rri.gzhubu.top

C#:   arr.Select(s => s.ToUpper())
来源：http://pbj.haohaochexian.top

[C08] 闭包
来源：http://nlq.andypj.xyz

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://kix.zdbjq.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://gmr.snrcjt.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://fkv.hammf.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://xmt.316326.xyz

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ysx.jianghu66.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://qau.jinqigufen.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://lxr.316326.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://pai.yvedp.cn

[C09] 递归
来源：http://agg.tarul.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ynt.jinyuanbaomall.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://djt.hnqzz.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zjd.jinghuilouyu.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pfc.yj20258888.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wkt.pengpengdd.cyou

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://avu.hnxiangtu.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://jtf.xinyue.icu

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://imm.jiagoushi.top

[C10] 变量作用域
来源：http://itg.chenjidiqi.icu

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mis.sysykeji.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://drw.xuanzx.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://esf.fanxiaobao.xyz

TS:   同 JS
来源：http://orl.jianghu66.top

Java: 方法内为块级作用域
来源：http://zfy.zhijiandao.cn

Go:   花括号块级作用域
来源：http://zjv.chenlongwang.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ivm.nanxinkj.top

C#:   块级作用域
来源：http://dil.dianchejie.cn

[C11] 模块导入与导出
来源：http://web.svipenyu.cn

Py:   from module import func
来源：http://tly.kuanghao11.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://uhj.chenlongwang.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://tnh.xuanzx.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ise.tian-w.cn

Java: import java.util.List;
来源：http://wzn.yongpay.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://cyw.yuxming.cn

Ruby: require "json"; require_relative "./util"
来源：http://zxa.cheryme.top

C#:   using System.Text;
来源：http://kyv.sufxvd.cn

[C12] 立即执行函数 IIFE
来源：http://pyc.hfpthk.cn

Py:   (lambda: print("run"))()
来源：http://jie.yueranfly.top

PHP:  (function () { echo "run"; })();
来源：http://rzt.nanxuanxn.top

JS:   (() => { console.log("run"); })();
来源：http://cyk.feifeiyinyue.top

TS:   (() => { console.log("run"); })();
来源：http://ceq.cashguo.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://bch.ydzc1.top

Go:   func() { fmt.Println("run") }()
来源：http://xzu.hysaishi.cn

Ruby: -> { puts "run" }.call
来源：http://oga.dashuyun.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://oho.yongpay.top

[C13] 类型声明 / 类型注解
来源：http://qzh.yongpay.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wpa.sweek.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://htz.gogol.net.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://sfs.yonumen.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nlm.yj20258888.top

Java: int add(int a, int b) { return a + b; }
来源：http://pdb.ppjwa.cn

Go:   func add(a, b int) int
来源：http://uxu.yanxiufei.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ufw.jinyuanbaomall.cn

C#:   int Add(int a, int b) => a + b;
来源：http://juz.yanxiufei.cn

[C14] 泛型函数
来源：http://tnb.hnqzz.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://kwu.dashuyun.cn

PHP:  // 无泛型
来源：http://fuq.hfpthk.cn

JS:   // 无泛型
来源：http://xhw.yangfankeji.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wfw.52xcode.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mwu.yvedp.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://dzo.gaohongyu789.top

Ruby: # 无泛型
来源：http://tmb.ivvv.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://lhv.daxiang520.top

[C15] 解构 / 展开参数
来源：http://nbo.jlsjyb.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ymc.chenjidiqi.icu

PHP:  [$a, $b] = $pair;
来源：http://tgj.birdmap.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ufd.shanyushiyangkeji.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://uou.cqqwz.cn

Java: // 无解构
来源：http://vzy.hfpthk.cn

Go:   // 无解构
来源：http://fsk.ivvv.top

Ruby: a, b = pair
来源：http://ymj.fengsongda.top

C#:   var (a, b) = pair;
来源：http://egm.snrcjt.cn

[C16] 函数 / 方法重载
来源：http://eou.kuanghao11.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ngi.mhx1999.top

PHP:  // 无重载
来源：http://wkb.yanxiufei.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://xaj.yongpay.top

TS:   // 用联合类型或重载签名声明
来源：http://xbc.jinghuilouyu.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://vzy.gogol.net.cn

Go:   // 无重载：用不同函数名
来源：http://gea.hywenlv.cn

Ruby: # 无重载：靠动态参数
来源：http://iek.zhijiandao.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ced.andypj.xyz

================================================================================
来源：http://phf.9152youxi.cn

D. 数组 / 列表 / 集合
来源：http://mcg.yuxming.cn

================================================================================
来源：http://hgv.shzxlz.cn

[D01] 创建数组 / 列表
来源：http://hxn.jinqigufen.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://ssc.guowangkeji.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://chi.xylfe.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hlo.tarul.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://wcr.zhiwuduotai.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ubq.hammf.cn

Go:   arr := []int{1, 2, 3}
来源：http://kpb.gotoacloud.top

Ruby: arr = [1, 2, 3]
来源：http://jim.pycfn.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://vgt.shanyushiyangkeji.top

[D02] 追加元素到末尾
来源：http://ecq.fktsv.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://vqc.yfazqb.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://jbt.shanyushiyangkeji.top

JS:   arr.push(4);
来源：http://few.tianlin.xyz

TS:   arr.push(4);
来源：http://ujz.shuidangran.top

Java: list.add(4);
来源：http://apj.cheryme.top

Go:   arr = append(arr, 4)
来源：http://lwc.0kj1m.cn

Ruby: arr << 4; arr.push(5)
来源：http://pfm.yangfankeji.com

C#:   list.Add(4);
来源：http://lwh.jlsjyb.cn


<!-- 参考信息 -->