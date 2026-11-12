代发 wailian999

TS:   for (const item of arr) { console.log(item); }
来源：http://rao.cqqwz.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://gfd.feifeiyinyue.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ppo.gotoacloud.top

Ruby: arr.each { |item| puts item }
来源：http://sna.zycfv.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://dyz.hongshengwenyu.top

[B06] 遍历字典 / 对象
来源：http://dhq.zhiwuduotai.top

Py:   for k, v in d.items(): print(k, v)
来源：http://rgd.guowangkeji.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://qbn.snrcjt.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qyq.havefunace.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bpi.xinyue.icu

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://flo.aibaodan.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://nyp.haohaochexian.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://tgw.zhixingplan.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://gzo.nanxinkj.top

[B07] while 循环
来源：http://cci.cqqwz.cn

Py:   while i < 10: i += 1
来源：http://hjh.ywan-chungtsiang.top

PHP:  while ($i < 10) { $i++; }
来源：http://kmi.xziqi.cn

JS:   while (i < 10) { i++; }
来源：http://jnj.jiagoushi.top

TS:   while (i < 10) { i++; }
来源：http://usa.hnqzz.top

Java: while (i < 10) { i++; }
来源：http://xkx.hnqzz.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wwx.cucudq.cn

Ruby: while i < 10; i += 1; end
来源：http://qyo.zhijiandao.cn

C#:   while (i < 10) { i++; }
来源：http://alp.ctjpmb.com

[B08] do-while（至少执行一次）
来源：http://udo.316326.xyz

Py:   # 无 do-while：用 while True + break
来源：http://oas.cqqwz.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ved.cheryme.top

JS:   do { i++; } while (i < 10);
来源：http://xhi.fzhhl.top

TS:   do { i++; } while (i < 10);
来源：http://klc.xinyue.icu

Java: do { i++; } while (i < 10);
来源：http://akd.jiagoushi.top

Go:   for { i++; if i >= 10 { break } }
来源：http://gqg.zdqjudy.top

Ruby: begin; i += 1; end while i < 10
来源：http://poy.yvedp.cn

C#:   do { i++; } while (i < 10);
来源：http://mii.iojbl.cn

[B09] break 与 continue
来源：http://fqa.yj202588.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://bje.cucudq.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://zqc.jinqigfzy.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hmm.zhongyouzk.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ltl.gotoacloud.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wnf.yonumen.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://qin.cqqwz.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://kqr.shanyushiyangtech.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oms.vehdjk.com

[B10] 遍历同时拿索引
来源：http://yyp.9152youxi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ujv.pycfn.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://gzc.epnwcf.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ven.shanyushiyangkeji.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ycw.jqgufenzy.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ckx.jinghuilouyu.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://eod.gzhubu.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://oax.nwbrower.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://cer.jiagoushi.top

[B11] 生成数字序列 / 区间
来源：http://crx.cdnleiting.top

Py:   list(range(0, 10, 2))
来源：http://pcn.gaohongyu789.top

PHP:  range(0, 10, 2);
来源：http://ovp.feifeiyinyue.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bzx.yvedp.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lhh.jinyuanbaomall.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://zdt.haohaochexian.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://vtl.daria6918.cn

Ruby: (0...10).step(2).to_a
来源：http://acj.xuetiantiany.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://vze.hfpthk.cn

[B12] 跳出多层循环
来源：http://nqf.shanyushiyangtech.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://tgo.quarkkingdee.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://kgd.daxiang520.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://dar.fengsongda.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://vdu.tianlin.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://pxr.hfpthk.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://gic.zhaomingkeji.xyz

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://jgr.c1oappe.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://zef.zdbjq.cn

[B13] 判断是否为数字
来源：http://kta.tian-w.cn

Py:   isinstance(x, (int, float))
来源：http://dgm.wangdashe.top

PHP:  is_numeric($x)
来源：http://kkz.shanyushiyangtech.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nrq.yfazqb.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://uxx.zhengqikj.top

Java: x instanceof Number
来源：http://rtg.sysykeji.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://jiw.zdbjq.cn

Ruby: x.is_a?(Numeric)
来源：http://ktj.hcnkem.com

C#:   x is int or double or decimal
来源：http://vlc.nwbrower.top

[B14] 判断值是否在集合内
来源：http://sxa.aizwys.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://rmn.hongshengwenyu.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://uvf.ppjwa.cn

JS:   [1, 2, 3].includes(x)
来源：http://pdd.xuetiantiany.cn

TS:   [1, 2, 3].includes(x)
来源：http://uvi.jyoumei.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ecc.zhoulong.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://exb.tianlin.xyz

Ruby: [1, 2, 3].include?(x)
来源：http://sbi.jqgufenzy.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://xzt.gzhubu.top

[B15] 布尔运算与取反
来源：http://byc.sysykeji.top

Py:   a and b or not c
来源：http://ndc.smart0.xyz

PHP:  $a && $b || !$c
来源：http://xej.smart0.xyz

JS:   a && b || !c
来源：http://wno.c1oappe.top

TS:   a && b || !c
来源：http://kaw.tarul.cn

Java: a && b || !c
来源：http://dio.chenlongwang.top

Go:   a && b || !c
来源：http://ckh.xylfe.cn

Ruby: a && b || !c
来源：http://mwd.xylfe.cn

C#:   a && b || !c
来源：http://xdg.tian-w.cn

[B16] 卫语句：不满足条件提前返回
来源：http://dnj.hcnkem.com

Py:   if not data: return
来源：http://kqz.shanyushiyangkeji.top

PHP:  if (!$data) { return; }
来源：http://ind.zdbjq.cn

JS:   if (!data) return;
来源：http://upe.snrcjt.cn

TS:   if (!data) return;
来源：http://xrq.zhoulong.xyz

Java: if (data == null) return;
来源：http://okk.yueranfly.top

Go:   if data == nil { return }
来源：http://ota.yongpay.top

Ruby: return if data.nil?
来源：http://drl.fehbvm.com

C#:   if (data == null) return;
来源：http://idw.vqdsnc.cn

================================================================================
来源：http://rcr.zhongyouzk.top

C. 函数与作用域
来源：http://kop.jlsjyb.cn

================================================================================
来源：http://nwd.mhx1999.top

[C01] 定义函数
来源：http://qbj.mhx1999.top

Py:   def add(a, b): return a + b
来源：http://baz.yuxming.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yze.ywan-chungtsiang.top

JS:   function add(a, b) { return a + b; }
来源：http://ihh.feifeiyinyue.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://exr.ydzc1.top

Java: static int add(int a, int b) { return a + b; }
来源：http://vpl.zhiwuduotai.top

Go:   func add(a, b int) int { return a + b }
来源：http://ljw.jlsjyb.cn

Ruby: def add(a, b); a + b; end
来源：http://dom.jqgfzy.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://usw.hongshengwenyu.top

[C02] 默认参数
来源：http://apk.bbcook.cn

Py:   def greet(name="World"): return name
来源：http://yrs.snrcjt.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://phx.bjfxy.top

JS:   function greet(name = "World") { return name; }
来源：http://vfo.jiagoushi.top

TS:   function greet(name: string = "World") { return name; }
来源：http://qsl.jyoumei.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://bfs.hywenlv.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ksz.fktsv.cn

Ruby: def greet(name = "World") = name
来源：http://zpp.ppjwa.cn

C#:   string Greet(string name = "World") => name;
来源：http://hfo.316326.xyz

[C03] 可变参数
来源：http://kye.iojbl.cn

Py:   def total(*args): return sum(args)
来源：http://ary.fanxiaobao.xyz

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://rpu.cqqwz.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://qpz.hnxiangtu.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://yao.hammf.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://erh.cheryme.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://kjf.ydzc1.top

Ruby: def total(*nums); nums.sum; end
来源：http://swv.gaohongyu789.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://kxf.hongshengwenyu.top

[C04] 命名参数 / 关键字参数
来源：http://qsx.zdqjudy.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://heq.guowangkeji.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://vcy.9152youxi.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://tdi.tianlin.xyz

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://dph.hcnkem.com

Java: // 无：用 Builder 模式或 record
来源：http://cww.andypj.xyz

Go:   // 无：用配置结构体参数
来源：http://dwr.nanxinkj.top

Ruby: f(a: 1, b: 2)
来源：http://wnw.hcnkem.com

C#:   f(a: 1, b: 2)
来源：http://lbg.yj20258.top

[C05] 返回多个值
来源：http://mjy.316326.xyz

Py:   return a, b
来源：http://cyf.yuanzhike.top

PHP:  return [$a, $b];
来源：http://dss.jinghuilouyu.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ney.jianghu66.top

TS:   return { a, b };
来源：http://ojs.jlsjyb.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ovy.shzxlz.cn

Go:   return a, b
来源：http://hvd.ybcxt.top

Ruby: return a, b
来源：http://rtk.zdqjudy.top

C#:   return (a, b);              // ValueTuple
来源：http://oni.jinqigfzy.top

[C06] 匿名函数 / lambda
来源：http://ckz.zycfv.cn

Py:   square = lambda x: x * x
来源：http://vdj.pengpengdd.cyou

PHP:  $square = fn($x) => $x * $x;
来源：http://rpu.cheryme.top

JS:   const square = x => x * x;
来源：http://dvd.yanxiufei.cn

TS:   const square = (x: number): number => x * x;
来源：http://qac.meibo888.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://opd.yuanzhike.top

Go:   sq := func(x int) int { return x * x }
来源：http://mzq.ydjk.org.cn

Ruby: square = ->(x) { x * x }
来源：http://hxj.guannengcc.top

C#:   Func<int, int> square = x => x * x;
来源：http://adk.9152youxi.cn

[C07] 把函数作为参数传入
来源：http://zsx.zycfv.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://weh.ctjpmb.com

PHP:  array_map("strtoupper", $arr);
来源：http://rrg.ydjk.org.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://lvq.ivvv.top

TS:   arr.map(String)
来源：http://kze.cheryme.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://iqr.hnqzz.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://cqj.52xcode.cn

Ruby: arr.map(&:upcase)
来源：http://crb.sjlbkw.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://mpb.316326.xyz

[C08] 闭包
来源：http://ikz.guowangkeji.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://bem.gzhubu.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://yby.sxryk.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://cqg.hesvh.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://jbz.tianlin.xyz

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ulp.hongshengwenyu.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://zpx.aizwys.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://llm.shuidangran.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://vam.zdqjudy.top

[C09] 递归
来源：http://ric.iojbl.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://rxq.wangshuangyany.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://gnz.wangdashe.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rse.kuanghao11.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://soc.xuanzx.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://cxy.ppjwa.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://gml.sweek.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ofw.zhiwuduotai.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ujj.fanxiaobao.xyz

[C10] 变量作用域
来源：http://mtg.c1oappe.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ziz.gotoacloud.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://tjj.ctjpmb.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://anr.nwbrower.top

TS:   同 JS
来源：http://mci.smart0.xyz

Java: 方法内为块级作用域
来源：http://vxu.kuanghao11.cn

Go:   花括号块级作用域
来源：http://wxz.ivvv.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://rqh.ybcxt.top

C#:   块级作用域
来源：http://jmb.fktsv.cn

[C11] 模块导入与导出
来源：http://sar.cashguo.top

Py:   from module import func
来源：http://fbx.birdmap.top

PHP:  require "file.php";  或 use App\Service;
来源：http://yhr.ywan-chungtsiang.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://cxp.9152youxi.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://bfk.hesvh.cn

Java: import java.util.List;
来源：http://bjh.xuanzx.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://tys.hysaishi.cn

Ruby: require "json"; require_relative "./util"
来源：http://pog.jlsjyb.cn

C#:   using System.Text;
来源：http://xgz.c1oappe.top

[C12] 立即执行函数 IIFE
来源：http://tbo.fehbvm.com

Py:   (lambda: print("run"))()
来源：http://xsj.shanyushiyangkeji.top

PHP:  (function () { echo "run"; })();
来源：http://aqn.hywenlv.cn

JS:   (() => { console.log("run"); })();
来源：http://xxw.wangshuangyany.cn

TS:   (() => { console.log("run"); })();
来源：http://qcw.hysaishi.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wpd.jianghu66.top

Go:   func() { fmt.Println("run") }()
来源：http://idw.jiagoushi.top

Ruby: -> { puts "run" }.call
来源：http://wgi.hnqzz.top

C#:   // 无 IIFE：用静态构造函数
来源：http://dbl.chenzaomai.com

[C13] 类型声明 / 类型注解
来源：http://ypk.snrcjt.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://bjq.gogol.net.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jwm.iojbl.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hpg.dashuyun.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cbe.yanxiufei.cn

Java: int add(int a, int b) { return a + b; }
来源：http://jpi.zycfv.cn

Go:   func add(a, b int) int
来源：http://rpr.gaohongyu789.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ipv.hammf.cn

C#:   int Add(int a, int b) => a + b;
来源：http://xzx.tianlin.xyz

[C14] 泛型函数
来源：http://eor.shanyushiyangkeji.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://obf.nanxinkj.top

PHP:  // 无泛型
来源：http://nfk.epnwcf.com

JS:   // 无泛型
来源：http://fad.fehbvm.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://quh.yanxiufei.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://cjt.jyoumei.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://qwc.smart0.xyz

Ruby: # 无泛型
来源：http://udh.yonumen.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hyo.yj202588.top

[C15] 解构 / 展开参数
来源：http://vcm.aizwys.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://rkk.ywan-chungtsiang.top

PHP:  [$a, $b] = $pair;
来源：http://vpo.cheryme.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://idq.ehwqpu.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://udu.zhixingplan.top

Java: // 无解构
来源：http://yca.cdnleiting.top

Go:   // 无解构
来源：http://kil.hysaishi.cn

Ruby: a, b = pair
来源：http://rsc.yueranfly.top

C#:   var (a, b) = pair;
来源：http://eyh.guowangkeji.top

[C16] 函数 / 方法重载
来源：http://amy.zhixingplan.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://sie.jinqigfzy.top

PHP:  // 无重载
来源：http://mjr.xuanzx.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://wls.quarkkingdee.top

TS:   // 用联合类型或重载签名声明
来源：http://jac.ppjwa.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://bac.zhijiandao.cn

Go:   // 无重载：用不同函数名
来源：http://hwc.shuidangran.top

Ruby: # 无重载：靠动态参数
来源：http://mrk.shanyushiyangtech.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://rkk.shanyushiyangkeji.top

================================================================================
来源：http://ojy.jinqigufen.top

D. 数组 / 列表 / 集合
来源：http://fof.xylfe.cn

================================================================================
来源：http://njb.epnwcf.com

[D01] 创建数组 / 列表
来源：http://myn.gotoacloud.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://myk.yuxming.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://qkp.ehwqpu.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://cbg.gotoacloud.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://rvn.wangdashe.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://quv.hysaishi.cn

Go:   arr := []int{1, 2, 3}
来源：http://glh.tarul.cn

Ruby: arr = [1, 2, 3]
来源：http://pcw.uphjek.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wtc.yongpay.top

[D02] 追加元素到末尾
来源：http://zqh.dashuyun.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://vaj.jinqigfzy.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://szq.feifeiyinyue.top

JS:   arr.push(4);
来源：http://zxn.yj20258888.top

TS:   arr.push(4);
来源：http://xcx.jianghu66.top

Java: list.add(4);
来源：http://dkh.hysaishi.cn

Go:   arr = append(arr, 4)
来源：http://sqh.kuanghao11.cn

Ruby: arr << 4; arr.push(5)
来源：http://aja.gotoacloud.top

C#:   list.Add(4);
来源：http://bwm.nanxuanxn.top

[D03] 在指定位置插入元素
来源：http://pxy.nanxinkj.top

Py:   arr.insert(0, 0)
来源：http://bbr.shzxlz.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://bob.havefunace.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://abe.yangfankeji.com

TS:   arr.splice(0, 0, 0);
来源：http://idy.zhiwuduotai.top

Java: list.add(0, 0);
来源：http://zaf.zhiwuduotai.top

Go:   arr = append([]int{0}, arr...)
来源：http://nuu.andypj.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://qss.ydzc1.top

C#:   list.Insert(0, 0);
来源：http://gew.hesvh.cn

[D04] 删除元素
来源：http://suw.9152youxi.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://awu.chenlongwang.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://xcs.yueranfly.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wqs.chenzaomai.com

TS:   arr.splice(0, 1);
来源：http://atn.guowangkeji.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mgy.pengpengdd.cyou

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ueu.ydjk.org.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://fvj.chenjidiqi.icu

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ctd.mhx1999.top

[D05] 访问与修改元素
来源：http://ahd.52xcode.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://edd.aibaodan.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://qkn.andypj.xyz

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://adp.tanke756.top

TS:   arr[0]; arr.at(-1);
来源：http://loc.ybcxt.top

Java: list.get(0); list.set(0, 9);
来源：http://hap.xinyue.icu

Go:   arr[0]; arr[0] = 9
来源：http://nzh.jinghuilouyu.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://xcm.hfpthk.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://fuj.fehbvm.com

[D06] 数组长度
来源：http://arm.ehwqpu.com


<!-- 参考信息 -->