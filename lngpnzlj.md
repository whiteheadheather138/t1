代发 wailian999

[B05] 遍历数组 / 列表
来源：http://xsz.sxryk.cn

Py:   for item in arr: print(item)
来源：http://byp.mhx1999.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://zkl.svipenyu.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://yfm.jianghu66.top

TS:   for (const item of arr) { console.log(item); }
来源：http://sim.shanyushiyangtech.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://epp.jyoumei.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://bxd.quarkkingdee.top

Ruby: arr.each { |item| puts item }
来源：http://per.hysaishi.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://egf.kuanghao11.cn

[B06] 遍历字典 / 对象
来源：http://pby.yfazqb.com

Py:   for k, v in d.items(): print(k, v)
来源：http://faz.0kj1m.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mbh.yangfankeji.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dwr.meibo888.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wxj.sufxvd.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://gha.yuxming.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://beb.shanyushiyangtech.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://avb.yanxiufei.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ujf.yuxming.cn

[B07] while 循环
来源：http://xrq.xuetiantiany.cn

Py:   while i < 10: i += 1
来源：http://bup.chenjidiqi.icu

PHP:  while ($i < 10) { $i++; }
来源：http://kni.yj202588.top

JS:   while (i < 10) { i++; }
来源：http://rbx.cashguo.top

TS:   while (i < 10) { i++; }
来源：http://jrb.aizwys.cn

Java: while (i < 10) { i++; }
来源：http://xmc.316326.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://tzo.yueranfly.top

Ruby: while i < 10; i += 1; end
来源：http://xzm.zhiwuduotai.top

C#:   while (i < 10) { i++; }
来源：http://qky.zhoulong.xyz

[B08] do-while（至少执行一次）
来源：http://sya.jiagoushi.top

Py:   # 无 do-while：用 while True + break
来源：http://hoq.zhoulong.xyz

PHP:  do { $i++; } while ($i < 10);
来源：http://psg.smart0.xyz

JS:   do { i++; } while (i < 10);
来源：http://ezp.aibaodan.cn

TS:   do { i++; } while (i < 10);
来源：http://lfj.snrcjt.cn

Java: do { i++; } while (i < 10);
来源：http://bgo.jinyuanbaomall.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://jzm.yuxming.cn

Ruby: begin; i += 1; end while i < 10
来源：http://glw.havefunace.top

C#:   do { i++; } while (i < 10);
来源：http://geq.yanxiufei.cn

[B09] break 与 continue
来源：http://ned.bbcook.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://dgf.sxryk.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://lfp.ppjwa.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wod.0kj1m.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mib.hnxiangtu.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rki.birdmap.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://elj.bjfxy.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://orl.mhx1999.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://flk.hfpthk.cn

[B10] 遍历同时拿索引
来源：http://qpm.zhaomingkeji.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ukk.cqqwz.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://pmt.chenjidiqi.icu

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://tkg.cashguo.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://bod.ppjwa.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://zii.iojbl.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://fui.vqdsnc.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://tsu.cqqwz.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://zoo.hysaishi.cn

[B11] 生成数字序列 / 区间
来源：http://sys.yj202588.top

Py:   list(range(0, 10, 2))
来源：http://nnn.guannengcc.top

PHP:  range(0, 10, 2);
来源：http://qfi.smart0.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nus.iojbl.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://arf.yvedp.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://uft.jinghuilouyu.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://gnp.iojbl.cn

Ruby: (0...10).step(2).to_a
来源：http://fae.sweek.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ezs.sufxvd.cn

[B12] 跳出多层循环
来源：http://qja.sysykeji.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://bwz.fehbvm.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://nfx.hongshengwenyu.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://yfp.pycfn.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://gra.fanxiaobao.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://egh.jiagoushi.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://xcg.shanyushiyangkeji.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://jmr.haohaochexian.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://jdy.yuxming.cn

[B13] 判断是否为数字
来源：http://unx.nwbrower.top

Py:   isinstance(x, (int, float))
来源：http://oyn.zhaomingkeji.xyz

PHP:  is_numeric($x)
来源：http://bjp.hywenlv.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vqu.andypj.xyz

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dgw.ywan-chungtsiang.top

Java: x instanceof Number
来源：http://eze.quarkkingdee.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://zeo.nanxinkj.top

Ruby: x.is_a?(Numeric)
来源：http://tae.tanke756.top

C#:   x is int or double or decimal
来源：http://sdi.jyoumei.cn

[B14] 判断值是否在集合内
来源：http://ovo.fanxiaobao.xyz

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wwt.redwolf501.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://luq.sweek.top

JS:   [1, 2, 3].includes(x)
来源：http://ixc.yongpay.top

TS:   [1, 2, 3].includes(x)
来源：http://yms.jinqigfzy.top

Java: List.of(1, 2, 3).contains(x)
来源：http://mep.9152youxi.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mao.smart0.xyz

Ruby: [1, 2, 3].include?(x)
来源：http://sqb.shzxlz.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wat.kuanghao11.cn

[B15] 布尔运算与取反
来源：http://mxc.jinghuilouyu.cn

Py:   a and b or not c
来源：http://nrf.cheryme.top

PHP:  $a && $b || !$c
来源：http://swz.bbcook.cn

JS:   a && b || !c
来源：http://xqt.haohaochexian.top

TS:   a && b || !c
来源：http://opf.pengpengdd.cyou

Java: a && b || !c
来源：http://ldn.jinyuanbaomall.cn

Go:   a && b || !c
来源：http://kkh.fzhhl.top

Ruby: a && b || !c
来源：http://qnt.tarul.cn

C#:   a && b || !c
来源：http://xgi.tanke756.top

[B16] 卫语句：不满足条件提前返回
来源：http://kvy.sjlbkw.cn

Py:   if not data: return
来源：http://xxy.tian-w.cn

PHP:  if (!$data) { return; }
来源：http://aia.vehdjk.com

JS:   if (!data) return;
来源：http://wvp.andypj.xyz

TS:   if (!data) return;
来源：http://mvm.ivvv.top

Java: if (data == null) return;
来源：http://rxr.xuanzx.com

Go:   if data == nil { return }
来源：http://apn.pengpengdd.cyou

Ruby: return if data.nil?
来源：http://esw.9152youxi.cn

C#:   if (data == null) return;
来源：http://hkx.xinyue.icu

================================================================================
来源：http://sru.smart0.xyz

C. 函数与作用域
来源：http://nht.hywenlv.cn

================================================================================
来源：http://rqg.ydzc1.top

[C01] 定义函数
来源：http://xli.dianchejie.cn

Py:   def add(a, b): return a + b
来源：http://zni.jinqigfzy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lrl.fanxiaobao.xyz

JS:   function add(a, b) { return a + b; }
来源：http://qnx.shzxlz.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rbd.chenjidiqi.icu

Java: static int add(int a, int b) { return a + b; }
来源：http://ods.gaohongyu789.top

Go:   func add(a, b int) int { return a + b }
来源：http://zlf.havefunace.top

Ruby: def add(a, b); a + b; end
来源：http://ubn.haohaochexian.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://pwl.bbcook.cn

[C02] 默认参数
来源：http://yhv.fehbvm.com

Py:   def greet(name="World"): return name
来源：http://iua.zhongyouzk.top

PHP:  function greet($name = "World") { return $name; }
来源：http://aoe.xinyue.icu

JS:   function greet(name = "World") { return name; }
来源：http://mpq.daria6918.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://fvx.ydzc1.top

Java: // 无默认参数：方法重载或 Optional
来源：http://iws.jqgufenzy.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://zga.zhiwuduotai.top

Ruby: def greet(name = "World") = name
来源：http://qfo.0kj1m.cn

C#:   string Greet(string name = "World") => name;
来源：http://xrw.sxryk.cn

[C03] 可变参数
来源：http://fcm.xziqi.cn

Py:   def total(*args): return sum(args)
来源：http://hwb.fehbvm.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://qwr.hnxiangtu.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ukl.gotoacloud.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://nua.gzhubu.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://bux.ywan-chungtsiang.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ecy.jqgfzy.top

Ruby: def total(*nums); nums.sum; end
来源：http://kwy.yongpay.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://bwk.sjlbkw.cn

[C04] 命名参数 / 关键字参数
来源：http://bmi.hesvh.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://vui.0kj1m.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://gmc.ybcxt.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://vqi.wangshuangyany.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://kdc.snrcjt.cn

Java: // 无：用 Builder 模式或 record
来源：http://vco.nanxinkj.top

Go:   // 无：用配置结构体参数
来源：http://mxl.havefunace.top

Ruby: f(a: 1, b: 2)
来源：http://qee.shanyushiyangkeji.top

C#:   f(a: 1, b: 2)
来源：http://rwj.hammf.cn

[C05] 返回多个值
来源：http://ijb.ctjpmb.com

Py:   return a, b
来源：http://wuo.cucudq.cn

PHP:  return [$a, $b];
来源：http://osk.sweek.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://tvf.quarkkingdee.top

TS:   return { a, b };
来源：http://ntm.fengsongda.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://aid.yanxiufei.cn

Go:   return a, b
来源：http://vzu.xziqi.cn

Ruby: return a, b
来源：http://gxo.yuxming.cn

C#:   return (a, b);              // ValueTuple
来源：http://sti.hnqzz.top

[C06] 匿名函数 / lambda
来源：http://rwh.xylfe.cn

Py:   square = lambda x: x * x
来源：http://nsv.zdbjq.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://yny.yanxiufei.cn

JS:   const square = x => x * x;
来源：http://xml.birdmap.top

TS:   const square = (x: number): number => x * x;
来源：http://wnc.tanke756.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://bmy.hongshengwenyu.top

Go:   sq := func(x int) int { return x * x }
来源：http://acd.yangfankeji.com

Ruby: square = ->(x) { x * x }
来源：http://nve.sysykeji.top

C#:   Func<int, int> square = x => x * x;
来源：http://hpt.dashuyun.cn

[C07] 把函数作为参数传入
来源：http://xhm.fktsv.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://vuj.sufxvd.cn

PHP:  array_map("strtoupper", $arr);
来源：http://wzy.tarul.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://rwy.daria6918.cn

TS:   arr.map(String)
来源：http://zwr.dashuyun.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hhp.ppjwa.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://kfr.hysaishi.cn

Ruby: arr.map(&:upcase)
来源：http://nto.xinyue.icu

C#:   arr.Select(s => s.ToUpper())
来源：http://txn.shanyushiyangtech.top

[C08] 闭包
来源：http://qpq.0kj1m.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://eyr.yj20258.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://lvn.kuanghao11.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qrl.zhaomingkeji.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://yvj.feifeiyinyue.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ywh.c1oappe.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ubv.hongshengwenyu.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://fgv.ehwqpu.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hrh.zdqjudy.top

[C09] 递归
来源：http://juc.yuxming.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://cjh.redwolf501.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://qhi.tarul.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bwx.tianlin.xyz

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xhy.bjfxy.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ilj.sweek.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://gmc.quarkkingdee.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://aqs.haohaochexian.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://thr.shanyushiyangtech.top

[C10] 变量作用域
来源：http://wsh.jinyuanbaomall.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://omy.yj202588.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://yju.nwbrower.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ipn.smart0.xyz

TS:   同 JS
来源：http://ktb.svipenyu.cn

Java: 方法内为块级作用域
来源：http://rmn.ydzc1.top

Go:   花括号块级作用域
来源：http://ijy.gzhubu.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://pgh.xylfe.cn

C#:   块级作用域
来源：http://wve.52xcode.cn

[C11] 模块导入与导出
来源：http://wsp.yfazqb.com

Py:   from module import func
来源：http://uiy.zhiwuduotai.top

PHP:  require "file.php";  或 use App\Service;
来源：http://tlp.epnwcf.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://mpv.uphjek.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://nyp.meibo888.top

Java: import java.util.List;
来源：http://rxo.hnqzz.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://iik.tanke756.top

Ruby: require "json"; require_relative "./util"
来源：http://xov.yuanzhike.top

C#:   using System.Text;
来源：http://nim.c1oappe.top

[C12] 立即执行函数 IIFE
来源：http://hba.nanxuanxn.top

Py:   (lambda: print("run"))()
来源：http://usc.sysykeji.top

PHP:  (function () { echo "run"; })();
来源：http://okd.cashguo.top

JS:   (() => { console.log("run"); })();
来源：http://mfh.daria6918.cn

TS:   (() => { console.log("run"); })();
来源：http://mhi.yongpay.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://xjo.zhixingplan.top

Go:   func() { fmt.Println("run") }()
来源：http://kiv.hnqzz.top

Ruby: -> { puts "run" }.call
来源：http://doa.shangyingyoupin.top

C#:   // 无 IIFE：用静态构造函数
来源：http://qzg.yuxming.cn

[C13] 类型声明 / 类型注解
来源：http://ijo.mhx1999.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://jlo.nanxinkj.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://goz.wangshuangyany.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://oxv.chenlongwang.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://stn.yuanzhike.top

Java: int add(int a, int b) { return a + b; }
来源：http://bed.jinyuanbaomall.cn

Go:   func add(a, b int) int
来源：http://wlp.cucudq.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://pwz.wangdashe.top

C#:   int Add(int a, int b) => a + b;
来源：http://fmb.wangshuangyany.cn

[C14] 泛型函数
来源：http://doc.yuanzhike.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://rrr.jinqigfzy.top

PHP:  // 无泛型
来源：http://dem.ppjwa.cn

JS:   // 无泛型
来源：http://xys.feifeiyinyue.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://gtl.birdmap.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://jun.chenzaomai.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://asr.daxiang520.top

Ruby: # 无泛型
来源：http://jji.mhx1999.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://iig.fengsongda.top

[C15] 解构 / 展开参数
来源：http://von.shangyingyoupin.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://jyb.hnqzz.top

PHP:  [$a, $b] = $pair;
来源：http://ema.hfpthk.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://iug.nanxinkj.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://khh.havefunace.top

Java: // 无解构
来源：http://med.jqgufenzy.top

Go:   // 无解构
来源：http://izf.tarul.cn

Ruby: a, b = pair
来源：http://mkz.guannengcc.top

C#:   var (a, b) = pair;
来源：http://izf.yj202588.top

[C16] 函数 / 方法重载
来源：http://cdq.zhengqikj.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://tzv.hfpthk.cn

PHP:  // 无重载
来源：http://vxc.jyoumei.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://asa.yfazqb.com

TS:   // 用联合类型或重载签名声明
来源：http://ikb.xinyue.icu

Java: void f(int a) {}  void f(String a) {}
来源：http://gmg.hfpthk.cn

Go:   // 无重载：用不同函数名
来源：http://pvx.jiagoushi.top

Ruby: # 无重载：靠动态参数
来源：http://hbo.sysykeji.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://eup.yueranfly.top

================================================================================
来源：http://wzh.zhengqikj.top

D. 数组 / 列表 / 集合
来源：http://xou.hesvh.cn

================================================================================
来源：http://qjm.316326.xyz

[D01] 创建数组 / 列表
来源：http://viu.uphjek.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://nir.sjlbkw.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hpu.cheryme.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ukf.yj20258.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://nrm.9152youxi.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://dnq.gzhubu.top

Go:   arr := []int{1, 2, 3}
来源：http://rmi.iojbl.cn

Ruby: arr = [1, 2, 3]
来源：http://ulz.yonumen.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://sur.vehdjk.com

[D02] 追加元素到末尾
来源：http://hfv.haohaochexian.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://gfi.yuanzhike.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://gkw.sjlbkw.cn

JS:   arr.push(4);
来源：http://apw.hesvh.cn

TS:   arr.push(4);
来源：http://qbo.yuxming.cn

Java: list.add(4);
来源：http://zfw.ppjwa.cn

Go:   arr = append(arr, 4)
来源：http://qpz.cheryme.top

Ruby: arr << 4; arr.push(5)
来源：http://fin.hysaishi.cn

C#:   list.Add(4);
来源：http://vtg.ehwqpu.com

[D03] 在指定位置插入元素
来源：http://jpw.fengsongda.top

Py:   arr.insert(0, 0)
来源：http://rma.vehdjk.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://kxd.jiagoushi.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://vvx.feifeiyinyue.top

TS:   arr.splice(0, 0, 0);
来源：http://rkn.bjfxy.top

Java: list.add(0, 0);
来源：http://rzt.zhaomingkeji.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://hhh.andypj.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mcc.vqdsnc.cn

C#:   list.Insert(0, 0);
来源：http://wgb.uphjek.com

[D04] 删除元素
来源：http://jxq.bjfxy.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://xjn.svipenyu.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://all.wangdashe.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://zod.wangdashe.top

TS:   arr.splice(0, 1);
来源：http://tah.jqgfzy.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hgl.iojbl.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://rhx.tianlin.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ulw.meibo888.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://tmb.316326.xyz

[D05] 访问与修改元素
来源：http://wtu.ehwqpu.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://xbo.yuxming.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://osq.hysaishi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://anq.sweek.top

TS:   arr[0]; arr.at(-1);
来源：http://rif.ywan-chungtsiang.top

Java: list.get(0); list.set(0, 9);
来源：http://bnf.zhaomingkeji.xyz


<!-- 参考信息 -->