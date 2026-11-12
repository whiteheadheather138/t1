代发 wailian999

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://are.sxryk.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ujl.ydzc1.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://imh.meibo888.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://gzs.cheryme.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://gsl.ctjpmb.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://tmu.cheryme.top

[B07] while 循环
来源：http://mtc.zdbjq.cn

Py:   while i < 10: i += 1
来源：http://par.jinqigufen.top

PHP:  while ($i < 10) { $i++; }
来源：http://clk.fehbvm.com

JS:   while (i < 10) { i++; }
来源：http://qql.tanke756.top

TS:   while (i < 10) { i++; }
来源：http://qez.tianlin.xyz

Java: while (i < 10) { i++; }
来源：http://rnq.nwbrower.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://xyq.hcnkem.com

Ruby: while i < 10; i += 1; end
来源：http://hyv.fehbvm.com

C#:   while (i < 10) { i++; }
来源：http://iye.fengsongda.top

[B08] do-while（至少执行一次）
来源：http://eji.jianghu66.top

Py:   # 无 do-while：用 while True + break
来源：http://bmz.hysaishi.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://nqm.hnxiangtu.top

JS:   do { i++; } while (i < 10);
来源：http://yws.cqqwz.cn

TS:   do { i++; } while (i < 10);
来源：http://mmf.yuanzhike.top

Java: do { i++; } while (i < 10);
来源：http://xws.yonumen.top

Go:   for { i++; if i >= 10 { break } }
来源：http://nvn.zdqjudy.top

Ruby: begin; i += 1; end while i < 10
来源：http://ccz.yongpay.top

C#:   do { i++; } while (i < 10);
来源：http://zgb.xziqi.cn

[B09] break 与 continue
来源：http://cgj.chenjidiqi.icu

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://vqd.birdmap.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://idm.gotoacloud.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ira.guannengcc.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://plq.guowangkeji.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ijk.havefunace.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://nyr.dashuyun.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://eyp.nanxinkj.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://arp.sysykeji.top

[B10] 遍历同时拿索引
来源：http://jwl.guowangkeji.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://msu.xylfe.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://rak.yueranfly.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://uqk.tanke756.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://awv.sjlbkw.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://dzn.jqgufenzy.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wat.tianlin.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://cif.vqdsnc.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://tkl.guowangkeji.top

[B11] 生成数字序列 / 区间
来源：http://tkb.jqgfzy.top

Py:   list(range(0, 10, 2))
来源：http://ylu.gotoacloud.top

PHP:  range(0, 10, 2);
来源：http://sgk.shuidangran.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pqi.xuanzx.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lid.fehbvm.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://zvk.ivvv.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://sum.shuidangran.top

Ruby: (0...10).step(2).to_a
来源：http://rjt.gogol.net.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://nag.guowangkeji.top

[B12] 跳出多层循环
来源：http://wes.gotoacloud.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://byv.dianchejie.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://umn.aibaodan.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://rwd.aibaodan.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://eaj.dianchejie.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://vst.jianghu66.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://tzd.jqgufenzy.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://fis.bjfxy.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hhd.mhx1999.top

[B13] 判断是否为数字
来源：http://hnq.redwolf501.top

Py:   isinstance(x, (int, float))
来源：http://llv.epnwcf.com

PHP:  is_numeric($x)
来源：http://ksy.svipenyu.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://oyp.jqgufenzy.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ncz.svipenyu.cn

Java: x instanceof Number
来源：http://akl.ybcxt.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hfe.pengpengdd.cyou

Ruby: x.is_a?(Numeric)
来源：http://lrk.shanyushiyangkeji.top

C#:   x is int or double or decimal
来源：http://kon.xuanzx.com

[B14] 判断值是否在集合内
来源：http://xbs.iojbl.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://juf.fehbvm.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ojo.jqgufenzy.top

JS:   [1, 2, 3].includes(x)
来源：http://tpq.sxryk.cn

TS:   [1, 2, 3].includes(x)
来源：http://nsp.fengsongda.top

Java: List.of(1, 2, 3).contains(x)
来源：http://ybq.tian-w.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://xkk.redwolf501.top

Ruby: [1, 2, 3].include?(x)
来源：http://ofk.yonumen.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://qvq.hongshengwenyu.top

[B15] 布尔运算与取反
来源：http://izg.jyoumei.cn

Py:   a and b or not c
来源：http://slz.shanyushiyangtech.top

PHP:  $a && $b || !$c
来源：http://jqd.hywenlv.cn

JS:   a && b || !c
来源：http://ida.ywan-chungtsiang.top

TS:   a && b || !c
来源：http://mxo.xingfuxueyuan.xyz

Java: a && b || !c
来源：http://qzv.sweek.top

Go:   a && b || !c
来源：http://vnl.aibaodan.cn

Ruby: a && b || !c
来源：http://jfi.fengsongda.top

C#:   a && b || !c
来源：http://onj.gaohongyu789.top

[B16] 卫语句：不满足条件提前返回
来源：http://usp.jqgfzy.top

Py:   if not data: return
来源：http://yfj.daria6918.cn

PHP:  if (!$data) { return; }
来源：http://onx.guowangkeji.top

JS:   if (!data) return;
来源：http://vil.yangfankeji.com

TS:   if (!data) return;
来源：http://zcn.dashuyun.cn

Java: if (data == null) return;
来源：http://dat.jianghu66.top

Go:   if data == nil { return }
来源：http://bpl.gogol.net.cn

Ruby: return if data.nil?
来源：http://gnr.ybcxt.top

C#:   if (data == null) return;
来源：http://stm.9152youxi.cn

================================================================================
来源：http://tkb.jyoumei.cn

C. 函数与作用域
来源：http://llz.hysaishi.cn

================================================================================
来源：http://wxo.0kj1m.cn

[C01] 定义函数
来源：http://xzb.redwolf501.top

Py:   def add(a, b): return a + b
来源：http://dsw.jinqigufen.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nta.316326.xyz

JS:   function add(a, b) { return a + b; }
来源：http://imu.fehbvm.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mng.zdqjudy.top

Java: static int add(int a, int b) { return a + b; }
来源：http://fgx.nanxuanxn.top

Go:   func add(a, b int) int { return a + b }
来源：http://pri.chenjidiqi.icu

Ruby: def add(a, b); a + b; end
来源：http://upk.cdnleiting.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mkb.zhixingplan.top

[C02] 默认参数
来源：http://bqh.jqgfzy.top

Py:   def greet(name="World"): return name
来源：http://iql.zdbjq.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://cus.hongshengwenyu.top

JS:   function greet(name = "World") { return name; }
来源：http://ffg.yj202588.top

TS:   function greet(name: string = "World") { return name; }
来源：http://oow.redwolf501.top

Java: // 无默认参数：方法重载或 Optional
来源：http://eeq.52xcode.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://twm.jianghu66.top

Ruby: def greet(name = "World") = name
来源：http://txm.wangdashe.top

C#:   string Greet(string name = "World") => name;
来源：http://blu.ivvv.top

[C03] 可变参数
来源：http://uae.meibo888.top

Py:   def total(*args): return sum(args)
来源：http://pnu.xziqi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wkq.316326.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://bbz.vehdjk.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hdg.ydjk.org.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ztq.daria6918.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://lil.chenjidiqi.icu

Ruby: def total(*nums); nums.sum; end
来源：http://src.gotoacloud.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://amp.jinghuilouyu.cn

[C04] 命名参数 / 关键字参数
来源：http://vwk.yangfankeji.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://lhp.yj20258888.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://emg.c1oappe.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://rmd.zdbjq.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wnm.ehwqpu.com

Java: // 无：用 Builder 模式或 record
来源：http://igt.bjfxy.top

Go:   // 无：用配置结构体参数
来源：http://ezv.yuxming.cn

Ruby: f(a: 1, b: 2)
来源：http://tlz.hesvh.cn

C#:   f(a: 1, b: 2)
来源：http://kbj.ehwqpu.com

[C05] 返回多个值
来源：http://hhe.jinqigfzy.top

Py:   return a, b
来源：http://gfo.yj202588.top

PHP:  return [$a, $b];
来源：http://xpg.hnxiangtu.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://icj.shzxlz.cn

TS:   return { a, b };
来源：http://ytl.xuetiantiany.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://yqf.daria6918.cn

Go:   return a, b
来源：http://maz.dashuyun.cn

Ruby: return a, b
来源：http://amu.andypj.xyz

C#:   return (a, b);              // ValueTuple
来源：http://qhq.hcnkem.com

[C06] 匿名函数 / lambda
来源：http://djm.chenlongwang.top

Py:   square = lambda x: x * x
来源：http://hsl.birdmap.top

PHP:  $square = fn($x) => $x * $x;
来源：http://lyg.fengsongda.top

JS:   const square = x => x * x;
来源：http://yji.vqdsnc.cn

TS:   const square = (x: number): number => x * x;
来源：http://qeu.gotoacloud.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://cfg.zhengqikj.top

Go:   sq := func(x int) int { return x * x }
来源：http://wse.xylfe.cn

Ruby: square = ->(x) { x * x }
来源：http://uvz.smart0.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://ueh.yongpay.top

[C07] 把函数作为参数传入
来源：http://lce.tianlin.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://cte.guannengcc.top

PHP:  array_map("strtoupper", $arr);
来源：http://qkr.xuetiantiany.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mym.gotoacloud.top

TS:   arr.map(String)
来源：http://pun.aizwys.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://vks.dashuyun.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ycx.hesvh.cn

Ruby: arr.map(&:upcase)
来源：http://yor.tianlin.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://nhz.pengpengdd.cyou

[C08] 闭包
来源：http://rlc.yvedp.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ont.nwbrower.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://lmj.ydzc1.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://xdm.yfazqb.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ups.zhixingplan.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://xzk.daxiang520.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://luo.daria6918.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://zvg.sxryk.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://prh.xuetiantiany.cn

[C09] 递归
来源：http://lfx.zdbjq.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ici.yueranfly.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://jyj.yj202588.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://evb.zhijiandao.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://grd.jqgfzy.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://htr.gotoacloud.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ari.gotoacloud.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://jce.yfazqb.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://uzi.chenzaomai.com

[C10] 变量作用域
来源：http://xxk.quarkkingdee.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://rlh.9152youxi.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://jmg.vqdsnc.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://jqr.zhongyouzk.top

TS:   同 JS
来源：http://moz.wangshuangyany.cn

Java: 方法内为块级作用域
来源：http://eoq.vqdsnc.cn

Go:   花括号块级作用域
来源：http://fbz.0kj1m.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://sjs.c1oappe.top

C#:   块级作用域
来源：http://fkp.ydjk.org.cn

[C11] 模块导入与导出
来源：http://qkr.nanxinkj.top

Py:   from module import func
来源：http://uds.zhaomingkeji.xyz

PHP:  require "file.php";  或 use App\Service;
来源：http://rxw.wangdashe.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://nux.tian-w.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://nnm.chenlongwang.top

Java: import java.util.List;
来源：http://igl.jlsjyb.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://twv.tarul.cn

Ruby: require "json"; require_relative "./util"
来源：http://emh.fehbvm.com

C#:   using System.Text;
来源：http://fev.shuidangran.top

[C12] 立即执行函数 IIFE
来源：http://zer.wangdashe.top

Py:   (lambda: print("run"))()
来源：http://sec.epnwcf.com

PHP:  (function () { echo "run"; })();
来源：http://ust.yongpay.top

JS:   (() => { console.log("run"); })();
来源：http://frs.wangdashe.top

TS:   (() => { console.log("run"); })();
来源：http://cxp.gogol.net.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://oxy.shangyingyoupin.top

Go:   func() { fmt.Println("run") }()
来源：http://xch.fktsv.cn

Ruby: -> { puts "run" }.call
来源：http://azk.hammf.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://kyt.nanxuanxn.top

[C13] 类型声明 / 类型注解
来源：http://oub.vqdsnc.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hwz.cheryme.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mjr.shangyingyoupin.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://xkd.nanxuanxn.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wva.pycfn.com

Java: int add(int a, int b) { return a + b; }
来源：http://cjn.sweek.top

Go:   func add(a, b int) int
来源：http://idx.fktsv.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://qsx.yvedp.cn

C#:   int Add(int a, int b) => a + b;
来源：http://upx.sweek.top

[C14] 泛型函数
来源：http://esb.fzhhl.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://dqe.aibaodan.cn

PHP:  // 无泛型
来源：http://upf.jqgufenzy.top

JS:   // 无泛型
来源：http://bep.meibo888.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://akn.cqqwz.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ppp.gzhubu.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://dfy.pengpengdd.cyou

Ruby: # 无泛型
来源：http://vmj.xinyue.icu

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ltg.fktsv.cn

[C15] 解构 / 展开参数
来源：http://hjf.chenzaomai.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://gpv.tanke756.top

PHP:  [$a, $b] = $pair;
来源：http://zex.andypj.xyz

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://jii.yongpay.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://smo.ywan-chungtsiang.top

Java: // 无解构
来源：http://wcr.iojbl.cn

Go:   // 无解构
来源：http://wkt.aizwys.cn

Ruby: a, b = pair
来源：http://iqd.fzhhl.top

C#:   var (a, b) = pair;
来源：http://nds.sufxvd.cn

[C16] 函数 / 方法重载
来源：http://ouq.hongshengwenyu.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://bmb.aibaodan.cn

PHP:  // 无重载
来源：http://njq.xuetiantiany.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://htm.daria6918.cn

TS:   // 用联合类型或重载签名声明
来源：http://pbf.jianghu66.top

Java: void f(int a) {}  void f(String a) {}
来源：http://dep.yfazqb.com

Go:   // 无重载：用不同函数名
来源：http://mdd.pycfn.com

Ruby: # 无重载：靠动态参数
来源：http://dfh.ppjwa.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ksf.bbcook.cn

================================================================================
来源：http://ewu.xingfuxueyuan.xyz

D. 数组 / 列表 / 集合
来源：http://phj.shangyingyoupin.top

================================================================================
来源：http://xvy.xuetiantiany.cn

[D01] 创建数组 / 列表
来源：http://ufl.jyoumei.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://xlr.hysaishi.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hyr.guannengcc.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://pay.nwbrower.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://bqj.meibo888.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://zfo.zycfv.cn

Go:   arr := []int{1, 2, 3}
来源：http://tfd.sweek.top

Ruby: arr = [1, 2, 3]
来源：http://ddf.c1oappe.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://pbo.nwbrower.top

[D02] 追加元素到末尾
来源：http://ouo.hnqzz.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://uzd.hammf.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://iov.cheryme.top

JS:   arr.push(4);
来源：http://igc.zhongyouzk.top

TS:   arr.push(4);
来源：http://fet.shzxlz.cn

Java: list.add(4);
来源：http://myb.haohaochexian.top

Go:   arr = append(arr, 4)
来源：http://taj.hammf.cn

Ruby: arr << 4; arr.push(5)
来源：http://gns.zhijiandao.cn

C#:   list.Add(4);
来源：http://vvb.quarkkingdee.top

[D03] 在指定位置插入元素
来源：http://hua.yueranfly.top

Py:   arr.insert(0, 0)
来源：http://hjx.zhengqikj.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ztz.pycfn.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://jsj.jlsjyb.cn

TS:   arr.splice(0, 0, 0);
来源：http://jjn.316326.xyz

Java: list.add(0, 0);
来源：http://oix.wangdashe.top

Go:   arr = append([]int{0}, arr...)
来源：http://ahq.meibo888.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://evy.jinqigufen.top

C#:   list.Insert(0, 0);
来源：http://raj.ivvv.top

[D04] 删除元素
来源：http://ldc.zhoulong.xyz

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ksy.hnqzz.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://dct.ivvv.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://liv.fengsongda.top

TS:   arr.splice(0, 1);
来源：http://ykt.jqgufenzy.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://fkq.cucudq.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://oer.zhiwuduotai.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://usq.zhoulong.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://opk.gaohongyu789.top

[D05] 访问与修改元素
来源：http://jqz.snrcjt.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://bof.zhengqikj.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ufp.guowangkeji.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://jdw.tarul.cn

TS:   arr[0]; arr.at(-1);
来源：http://gfg.daxiang520.top

Java: list.get(0); list.set(0, 9);
来源：http://lpg.tianlin.xyz

Go:   arr[0]; arr[0] = 9
来源：http://swr.cqqwz.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ofp.xziqi.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://prq.jyoumei.cn

[D06] 数组长度
来源：http://lmj.fktsv.cn

Py:   len(arr)
来源：http://zcb.tian-w.cn

PHP:  count($arr);
来源：http://cnw.meibo888.top

JS:   arr.length
来源：http://mpd.smart0.xyz

TS:   arr.length
来源：http://dxz.zhengqikj.top

Java: list.size();
来源：http://mon.nanxinkj.top

Go:   len(arr)
来源：http://gnv.zhoulong.xyz

Ruby: arr.length; arr.size
来源：http://gsu.yvedp.cn

C#:   list.Count;
来源：http://vkv.c1oappe.top


<!-- 参考信息 -->