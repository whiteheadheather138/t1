代发 wailian999

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://iir.jianghu66.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cxs.zhijiandao.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ijl.hongshengwenyu.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://jkh.xylfe.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://qhn.zhaomingkeji.xyz

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://abc.hcnkem.com

[B07] while 循环
来源：http://zsu.hnxiangtu.top

Py:   while i < 10: i += 1
来源：http://sgd.ydzc1.top

PHP:  while ($i < 10) { $i++; }
来源：http://zxz.hammf.cn

JS:   while (i < 10) { i++; }
来源：http://xij.yongpay.top

TS:   while (i < 10) { i++; }
来源：http://uyt.hammf.cn

Java: while (i < 10) { i++; }
来源：http://mws.shzxlz.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://zpw.52xcode.cn

Ruby: while i < 10; i += 1; end
来源：http://jsw.hcnkem.com

C#:   while (i < 10) { i++; }
来源：http://djb.iojbl.cn

[B08] do-while（至少执行一次）
来源：http://vzk.quarkkingdee.top

Py:   # 无 do-while：用 while True + break
来源：http://vbe.jinyuanbaomall.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://sjq.epnwcf.com

JS:   do { i++; } while (i < 10);
来源：http://uou.jinqigufen.top

TS:   do { i++; } while (i < 10);
来源：http://usv.zdbjq.cn

Java: do { i++; } while (i < 10);
来源：http://ahx.mhx1999.top

Go:   for { i++; if i >= 10 { break } }
来源：http://bzu.yangfankeji.com

Ruby: begin; i += 1; end while i < 10
来源：http://kqb.yj20258888.top

C#:   do { i++; } while (i < 10);
来源：http://vom.sysykeji.top

[B09] break 与 continue
来源：http://xtw.9152youxi.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://vrt.cashguo.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://vlx.fktsv.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ptr.pycfn.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vqa.chenlongwang.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xbu.zdqjudy.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://omf.fehbvm.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hvf.zdbjq.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xqf.xuetiantiany.cn

[B10] 遍历同时拿索引
来源：http://gek.316326.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blj.hysaishi.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://nlo.52xcode.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://dpm.hnqzz.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://kue.hnxiangtu.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://rrb.yj20258.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mld.andypj.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://uiz.jianghu66.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://xoo.tanke756.top

[B11] 生成数字序列 / 区间
来源：http://wwo.hesvh.cn

Py:   list(range(0, 10, 2))
来源：http://ulf.jinqigfzy.top

PHP:  range(0, 10, 2);
来源：http://yyp.zhaomingkeji.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kcb.sxryk.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://oid.tanke756.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wwk.havefunace.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://vxa.redwolf501.top

Ruby: (0...10).step(2).to_a
来源：http://hvs.hcnkem.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://tsc.jianghu66.top

[B12] 跳出多层循环
来源：http://fhb.hammf.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://soo.bbcook.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://jug.andypj.xyz

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://eiz.quarkkingdee.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://yzg.yangfankeji.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://fgb.zycfv.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ngp.hnxiangtu.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://pun.ivvv.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://noe.zhijiandao.cn

[B13] 判断是否为数字
来源：http://kaa.ivvv.top

Py:   isinstance(x, (int, float))
来源：http://vxh.cqqwz.cn

PHP:  is_numeric($x)
来源：http://bnj.fanxiaobao.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tsk.vqdsnc.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jwn.yanxiufei.cn

Java: x instanceof Number
来源：http://byz.hnqzz.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://diw.guannengcc.top

Ruby: x.is_a?(Numeric)
来源：http://zbq.fengsongda.top

C#:   x is int or double or decimal
来源：http://zfw.chenlongwang.top

[B14] 判断值是否在集合内
来源：http://byw.yj202588.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://fel.bbcook.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://lbz.nwbrower.top

JS:   [1, 2, 3].includes(x)
来源：http://ptj.0kj1m.cn

TS:   [1, 2, 3].includes(x)
来源：http://typ.ctjpmb.com

Java: List.of(1, 2, 3).contains(x)
来源：http://ago.c1oappe.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://jcb.xuanzx.com

Ruby: [1, 2, 3].include?(x)
来源：http://ngw.wangdashe.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://qfj.zhaomingkeji.xyz

[B15] 布尔运算与取反
来源：http://ics.shzxlz.cn

Py:   a and b or not c
来源：http://nsk.shanyushiyangkeji.top

PHP:  $a && $b || !$c
来源：http://jjo.ywan-chungtsiang.top

JS:   a && b || !c
来源：http://rsa.svipenyu.cn

TS:   a && b || !c
来源：http://nrl.tarul.cn

Java: a && b || !c
来源：http://ots.hysaishi.cn

Go:   a && b || !c
来源：http://tfy.ybcxt.top

Ruby: a && b || !c
来源：http://zzo.zdbjq.cn

C#:   a && b || !c
来源：http://pej.pycfn.com

[B16] 卫语句：不满足条件提前返回
来源：http://yly.vqdsnc.cn

Py:   if not data: return
来源：http://grq.smart0.xyz

PHP:  if (!$data) { return; }
来源：http://lvg.jlsjyb.cn

JS:   if (!data) return;
来源：http://pxt.guannengcc.top

TS:   if (!data) return;
来源：http://zfs.hywenlv.cn

Java: if (data == null) return;
来源：http://utk.vqdsnc.cn

Go:   if data == nil { return }
来源：http://eln.wangshuangyany.cn

Ruby: return if data.nil?
来源：http://kgd.ydjk.org.cn

C#:   if (data == null) return;
来源：http://ckh.nanxuanxn.top

================================================================================
来源：http://jxh.vehdjk.com

C. 函数与作用域
来源：http://lnr.havefunace.top

================================================================================
来源：http://lsb.ctjpmb.com

[C01] 定义函数
来源：http://daq.aizwys.cn

Py:   def add(a, b): return a + b
来源：http://ztd.chenlongwang.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zhr.xziqi.cn

JS:   function add(a, b) { return a + b; }
来源：http://fav.fehbvm.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wxy.316326.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://aty.yj20258.top

Go:   func add(a, b int) int { return a + b }
来源：http://fcs.ydzc1.top

Ruby: def add(a, b); a + b; end
来源：http://swc.shzxlz.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://afj.uphjek.com

[C02] 默认参数
来源：http://ihk.cqqwz.cn

Py:   def greet(name="World"): return name
来源：http://hyi.tian-w.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://tnv.jqgfzy.top

JS:   function greet(name = "World") { return name; }
来源：http://wuf.shanyushiyangtech.top

TS:   function greet(name: string = "World") { return name; }
来源：http://qgr.yj202588.top

Java: // 无默认参数：方法重载或 Optional
来源：http://xld.bjfxy.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://tqf.uphjek.com

Ruby: def greet(name = "World") = name
来源：http://zjd.316326.xyz

C#:   string Greet(string name = "World") => name;
来源：http://jew.hcnkem.com

[C03] 可变参数
来源：http://cyh.smart0.xyz

Py:   def total(*args): return sum(args)
来源：http://wfm.shangyingyoupin.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://sam.feifeiyinyue.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://kzh.shzxlz.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://llw.guowangkeji.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://fwd.zhoulong.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://fwd.zhongyouzk.top

Ruby: def total(*nums); nums.sum; end
来源：http://bvs.meibo888.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://kvm.gogol.net.cn

[C04] 命名参数 / 关键字参数
来源：http://vwu.yvedp.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://det.ydzc1.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://cyk.xziqi.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://nxs.ctjpmb.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://lws.kuanghao11.cn

Java: // 无：用 Builder 模式或 record
来源：http://tsi.jinqigufen.top

Go:   // 无：用配置结构体参数
来源：http://drn.sxryk.cn

Ruby: f(a: 1, b: 2)
来源：http://jsi.quarkkingdee.top

C#:   f(a: 1, b: 2)
来源：http://bpa.cashguo.top

[C05] 返回多个值
来源：http://okl.smart0.xyz

Py:   return a, b
来源：http://gkl.dashuyun.cn

PHP:  return [$a, $b];
来源：http://whk.guowangkeji.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://tod.aizwys.cn

TS:   return { a, b };
来源：http://fex.smart0.xyz

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://zby.c1oappe.top

Go:   return a, b
来源：http://xww.fzhhl.top

Ruby: return a, b
来源：http://xls.shzxlz.cn

C#:   return (a, b);              // ValueTuple
来源：http://omx.redwolf501.top

[C06] 匿名函数 / lambda
来源：http://cxo.ehwqpu.com

Py:   square = lambda x: x * x
来源：http://wxf.hesvh.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://kcb.jianghu66.top

JS:   const square = x => x * x;
来源：http://aci.fengsongda.top

TS:   const square = (x: number): number => x * x;
来源：http://ojd.gotoacloud.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wlu.snrcjt.cn

Go:   sq := func(x int) int { return x * x }
来源：http://lsw.vehdjk.com

Ruby: square = ->(x) { x * x }
来源：http://svo.zhiwuduotai.top

C#:   Func<int, int> square = x => x * x;
来源：http://cqe.hnxiangtu.top

[C07] 把函数作为参数传入
来源：http://epf.yongpay.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ocx.yj202588.top

PHP:  array_map("strtoupper", $arr);
来源：http://rvp.gaohongyu789.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xas.jinqigfzy.top

TS:   arr.map(String)
来源：http://oqp.hywenlv.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ojb.52xcode.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://yvc.fehbvm.com

Ruby: arr.map(&:upcase)
来源：http://yyv.guowangkeji.top

C#:   arr.Select(s => s.ToUpper())
来源：http://rvv.zdqjudy.top

[C08] 闭包
来源：http://kna.pycfn.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://jbu.svipenyu.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://szi.guannengcc.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hiw.fengsongda.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://usp.havefunace.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://qrm.epnwcf.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jzx.jiagoushi.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ndv.shangyingyoupin.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://gtq.xuanzx.com

[C09] 递归
来源：http://qnc.hysaishi.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://tkb.yangfankeji.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://vdu.cqqwz.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xbk.jianghu66.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ahw.svipenyu.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://tgc.zhiwuduotai.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://axo.jqgufenzy.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://rqi.sufxvd.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://fiw.ivvv.top

[C10] 变量作用域
来源：http://pov.chenjidiqi.icu

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://frp.yj20258.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://xej.jiagoushi.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xge.ctjpmb.com

TS:   同 JS
来源：http://yix.zhengqikj.top

Java: 方法内为块级作用域
来源：http://ffk.gogol.net.cn

Go:   花括号块级作用域
来源：http://rjy.guowangkeji.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://kie.shanyushiyangkeji.top

C#:   块级作用域
来源：http://aif.guannengcc.top

[C11] 模块导入与导出
来源：http://ldf.yj20258.top

Py:   from module import func
来源：http://yhk.tianlin.xyz

PHP:  require "file.php";  或 use App\Service;
来源：http://osx.jinqigfzy.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://zwp.gzhubu.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ksm.havefunace.top

Java: import java.util.List;
来源：http://sdf.jinyuanbaomall.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://pbl.cqqwz.cn

Ruby: require "json"; require_relative "./util"
来源：http://bzv.zhaomingkeji.xyz

C#:   using System.Text;
来源：http://sjg.nwbrower.top

[C12] 立即执行函数 IIFE
来源：http://flw.redwolf501.top

Py:   (lambda: print("run"))()
来源：http://cxo.fzhhl.top

PHP:  (function () { echo "run"; })();
来源：http://oga.hysaishi.cn

JS:   (() => { console.log("run"); })();
来源：http://qnq.hywenlv.cn

TS:   (() => { console.log("run"); })();
来源：http://pcg.shanyushiyangkeji.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://fxg.uphjek.com

Go:   func() { fmt.Println("run") }()
来源：http://agb.nanxuanxn.top

Ruby: -> { puts "run" }.call
来源：http://xrm.vqdsnc.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://jww.yueranfly.top

[C13] 类型声明 / 类型注解
来源：http://usq.vehdjk.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://zlu.tianlin.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zsx.hywenlv.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ghm.snrcjt.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mwy.gzhubu.top

Java: int add(int a, int b) { return a + b; }
来源：http://hzd.quarkkingdee.top

Go:   func add(a, b int) int
来源：http://xst.hcnkem.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://bqd.c1oappe.top

C#:   int Add(int a, int b) => a + b;
来源：http://saf.52xcode.cn

[C14] 泛型函数
来源：http://dxn.9152youxi.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://bwl.xinyue.icu

PHP:  // 无泛型
来源：http://lqu.jinyuanbaomall.cn

JS:   // 无泛型
来源：http://mfo.zhaomingkeji.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ucd.xuetiantiany.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://quj.9152youxi.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://eup.jinyuanbaomall.cn

Ruby: # 无泛型
来源：http://cpw.fktsv.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://sxv.sjlbkw.cn

[C15] 解构 / 展开参数
来源：http://omz.bbcook.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xrz.zhengqikj.top

PHP:  [$a, $b] = $pair;
来源：http://pkg.cucudq.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://jwy.ywan-chungtsiang.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wvx.chenzaomai.com

Java: // 无解构
来源：http://hom.316326.xyz

Go:   // 无解构
来源：http://yhk.andypj.xyz

Ruby: a, b = pair
来源：http://cwy.ehwqpu.com

C#:   var (a, b) = pair;
来源：http://upt.sysykeji.top

[C16] 函数 / 方法重载
来源：http://gkx.chenjidiqi.icu

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hke.yuxming.cn

PHP:  // 无重载
来源：http://cga.fktsv.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://wto.jqgufenzy.top

TS:   // 用联合类型或重载签名声明
来源：http://glx.xylfe.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://vjn.yongpay.top

Go:   // 无重载：用不同函数名
来源：http://opm.gogol.net.cn

Ruby: # 无重载：靠动态参数
来源：http://jcy.hcnkem.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://lmt.jinyuanbaomall.cn

================================================================================
来源：http://wdt.epnwcf.com

D. 数组 / 列表 / 集合
来源：http://kdn.andypj.xyz

================================================================================
来源：http://nzm.ivvv.top

[D01] 创建数组 / 列表
来源：http://bfw.havefunace.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://fee.cashguo.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://dev.xingfuxueyuan.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://zfk.haohaochexian.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://bzf.andypj.xyz

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://xjt.hnxiangtu.top

Go:   arr := []int{1, 2, 3}
来源：http://ymw.ywan-chungtsiang.top

Ruby: arr = [1, 2, 3]
来源：http://txy.bbcook.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://msq.jqgufenzy.top

[D02] 追加元素到末尾
来源：http://zwi.guannengcc.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://osc.zhaomingkeji.xyz

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://lue.tian-w.cn

JS:   arr.push(4);
来源：http://gsw.yuxming.cn

TS:   arr.push(4);
来源：http://cjw.ybcxt.top

Java: list.add(4);
来源：http://qws.fanxiaobao.xyz

Go:   arr = append(arr, 4)
来源：http://yah.mhx1999.top

Ruby: arr << 4; arr.push(5)
来源：http://apz.hfpthk.cn

C#:   list.Add(4);
来源：http://gom.shuidangran.top

[D03] 在指定位置插入元素
来源：http://rls.cheryme.top

Py:   arr.insert(0, 0)
来源：http://vbw.xinyue.icu

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://aet.zhixingplan.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://kmg.bjfxy.top

TS:   arr.splice(0, 0, 0);
来源：http://qhv.iojbl.cn

Java: list.add(0, 0);
来源：http://rib.kuanghao11.cn

Go:   arr = append([]int{0}, arr...)
来源：http://xcb.smart0.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://kek.ydjk.org.cn

C#:   list.Insert(0, 0);
来源：http://fah.ywan-chungtsiang.top

[D04] 删除元素
来源：http://wnw.vqdsnc.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://yyc.ydjk.org.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://fyy.tianlin.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://gcg.xingfuxueyuan.xyz

TS:   arr.splice(0, 1);
来源：http://cpe.vqdsnc.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wbw.yanxiufei.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wpz.jianghu66.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://tcp.sjlbkw.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://cut.nanxinkj.top

[D05] 访问与修改元素
来源：http://ygp.sufxvd.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ekq.wangdashe.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://bfz.fktsv.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://bza.zdqjudy.top

TS:   arr[0]; arr.at(-1);
来源：http://yey.jinqigufen.top

Java: list.get(0); list.set(0, 9);
来源：http://bpf.9152youxi.cn

Go:   arr[0]; arr[0] = 9
来源：http://jnj.zdbjq.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://htb.yuanzhike.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://fjk.yj202588.top

[D06] 数组长度
来源：http://fhn.ywan-chungtsiang.top

Py:   len(arr)
来源：http://jrt.cashguo.top

PHP:  count($arr);
来源：http://lrr.tianlin.xyz

JS:   arr.length
来源：http://tvx.andypj.xyz

TS:   arr.length
来源：http://spz.xylfe.cn

Java: list.size();
来源：http://tlv.cdnleiting.top

Go:   len(arr)
来源：http://bzx.dianchejie.cn

Ruby: arr.length; arr.size
来源：http://pox.fehbvm.com

C#:   list.Count;
来源：http://gjx.shanyushiyangtech.top


<!-- 参考信息 -->