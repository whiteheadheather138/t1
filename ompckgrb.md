代发 wailian999

PHP:  while ($i < 10) { $i++; }
来源：http://txb.hywenlv.cn

JS:   while (i < 10) { i++; }
来源：http://vbc.zhengqikj.top

TS:   while (i < 10) { i++; }
来源：http://euc.hfpthk.cn

Java: while (i < 10) { i++; }
来源：http://xos.zhoulong.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hqt.cdnleiting.top

Ruby: while i < 10; i += 1; end
来源：http://pko.kuanghao11.cn

C#:   while (i < 10) { i++; }
来源：http://fyo.c1oappe.top

[B08] do-while（至少执行一次）
来源：http://tbo.jiagoushi.top

Py:   # 无 do-while：用 while True + break
来源：http://cmb.hcnkem.com

PHP:  do { $i++; } while ($i < 10);
来源：http://uwx.andypj.xyz

JS:   do { i++; } while (i < 10);
来源：http://ztv.316326.xyz

TS:   do { i++; } while (i < 10);
来源：http://clr.gzhubu.top

Java: do { i++; } while (i < 10);
来源：http://qvg.bbcook.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://fvt.cqqwz.cn

Ruby: begin; i += 1; end while i < 10
来源：http://mam.zycfv.cn

C#:   do { i++; } while (i < 10);
来源：http://wwc.cashguo.top

[B09] break 与 continue
来源：http://xch.jianghu66.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://tzm.uphjek.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://xfe.sxryk.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://siv.zhiwuduotai.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://seg.hysaishi.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rtu.jqgufenzy.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://cjx.zhaomingkeji.xyz

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wsx.xuanzx.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ljt.0kj1m.cn

[B10] 遍历同时拿索引
来源：http://eal.vehdjk.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ijn.birdmap.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ybm.hcnkem.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hgm.redwolf501.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ees.cqqwz.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://sgz.vehdjk.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wes.yonumen.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ycu.yongpay.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://sxd.yvedp.cn

[B11] 生成数字序列 / 区间
来源：http://tax.gotoacloud.top

Py:   list(range(0, 10, 2))
来源：http://ilf.jinqigufen.top

PHP:  range(0, 10, 2);
来源：http://dgu.ivvv.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fbd.sxryk.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://eqx.c1oappe.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ama.hywenlv.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://aya.fengsongda.top

Ruby: (0...10).step(2).to_a
来源：http://gug.yuxming.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://otz.zhongyouzk.top

[B12] 跳出多层循环
来源：http://epy.shanyushiyangtech.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://shg.redwolf501.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://wcq.haohaochexian.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://rld.yuxming.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://rvw.fzhhl.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://tzp.ywan-chungtsiang.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://zgl.zhiwuduotai.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://vzt.svipenyu.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://jra.xuanzx.com

[B13] 判断是否为数字
来源：http://ckc.tarul.cn

Py:   isinstance(x, (int, float))
来源：http://hmq.gogol.net.cn

PHP:  is_numeric($x)
来源：http://arr.yueranfly.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://alq.haohaochexian.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sqp.gaohongyu789.top

Java: x instanceof Number
来源：http://fku.hcnkem.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://znu.c1oappe.top

Ruby: x.is_a?(Numeric)
来源：http://asp.yueranfly.top

C#:   x is int or double or decimal
来源：http://sdt.nanxinkj.top

[B14] 判断值是否在集合内
来源：http://lrf.0kj1m.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://fyx.snrcjt.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://myg.jyoumei.cn

JS:   [1, 2, 3].includes(x)
来源：http://mry.vehdjk.com

TS:   [1, 2, 3].includes(x)
来源：http://oyl.hcnkem.com

Java: List.of(1, 2, 3).contains(x)
来源：http://fcq.andypj.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://zkq.ybcxt.top

Ruby: [1, 2, 3].include?(x)
来源：http://ttg.fktsv.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://eui.chenjidiqi.icu

[B15] 布尔运算与取反
来源：http://wuf.xuetiantiany.cn

Py:   a and b or not c
来源：http://ows.yanxiufei.cn

PHP:  $a && $b || !$c
来源：http://skn.52xcode.cn

JS:   a && b || !c
来源：http://egh.tianlin.xyz

TS:   a && b || !c
来源：http://lbb.gaohongyu789.top

Java: a && b || !c
来源：http://oln.sufxvd.cn

Go:   a && b || !c
来源：http://yag.zhengqikj.top

Ruby: a && b || !c
来源：http://ifq.yanxiufei.cn

C#:   a && b || !c
来源：http://jef.chenzaomai.com

[B16] 卫语句：不满足条件提前返回
来源：http://fpb.iojbl.cn

Py:   if not data: return
来源：http://wsz.52xcode.cn

PHP:  if (!$data) { return; }
来源：http://wjr.xuanzx.com

JS:   if (!data) return;
来源：http://jtv.vehdjk.com

TS:   if (!data) return;
来源：http://lmr.birdmap.top

Java: if (data == null) return;
来源：http://obd.52xcode.cn

Go:   if data == nil { return }
来源：http://zwl.fehbvm.com

Ruby: return if data.nil?
来源：http://knt.jianghu66.top

C#:   if (data == null) return;
来源：http://zel.zhijiandao.cn

================================================================================
来源：http://jpl.uphjek.com

C. 函数与作用域
来源：http://xjb.zycfv.cn

================================================================================
来源：http://blv.quarkkingdee.top

[C01] 定义函数
来源：http://ouh.cashguo.top

Py:   def add(a, b): return a + b
来源：http://jlk.chenlongwang.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pmm.yj20258888.top

JS:   function add(a, b) { return a + b; }
来源：http://yla.yj20258.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://uvn.cdnleiting.top

Java: static int add(int a, int b) { return a + b; }
来源：http://kou.yangfankeji.com

Go:   func add(a, b int) int { return a + b }
来源：http://qcj.gaohongyu789.top

Ruby: def add(a, b); a + b; end
来源：http://joj.gaohongyu789.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://jzd.xuetiantiany.cn

[C02] 默认参数
来源：http://jvi.chenlongwang.top

Py:   def greet(name="World"): return name
来源：http://gfb.xingfuxueyuan.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://uyh.zdqjudy.top

JS:   function greet(name = "World") { return name; }
来源：http://ekp.yongpay.top

TS:   function greet(name: string = "World") { return name; }
来源：http://etg.hcnkem.com

Java: // 无默认参数：方法重载或 Optional
来源：http://huw.cucudq.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://iju.andypj.xyz

Ruby: def greet(name = "World") = name
来源：http://efw.chenlongwang.top

C#:   string Greet(string name = "World") => name;
来源：http://wtf.ybcxt.top

[C03] 可变参数
来源：http://top.316326.xyz

Py:   def total(*args): return sum(args)
来源：http://aqw.nwbrower.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wjq.mhx1999.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hgn.zhixingplan.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mhd.ydzc1.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://gxo.epnwcf.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://sgl.uphjek.com

Ruby: def total(*nums); nums.sum; end
来源：http://ghc.nanxuanxn.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://lbl.bbcook.cn

[C04] 命名参数 / 关键字参数
来源：http://deh.xingfuxueyuan.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://zsi.ivvv.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://avg.vehdjk.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://gzd.hywenlv.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://msl.xylfe.cn

Java: // 无：用 Builder 模式或 record
来源：http://dte.chenlongwang.top

Go:   // 无：用配置结构体参数
来源：http://nam.jlsjyb.cn

Ruby: f(a: 1, b: 2)
来源：http://rfs.tian-w.cn

C#:   f(a: 1, b: 2)
来源：http://gnk.xinyue.icu

[C05] 返回多个值
来源：http://emp.snrcjt.cn

Py:   return a, b
来源：http://rnn.jinqigfzy.top

PHP:  return [$a, $b];
来源：http://giq.jqgufenzy.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://zgv.tianlin.xyz

TS:   return { a, b };
来源：http://ciw.cqqwz.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://sgc.wangdashe.top

Go:   return a, b
来源：http://eky.aizwys.cn

Ruby: return a, b
来源：http://egm.cdnleiting.top

C#:   return (a, b);              // ValueTuple
来源：http://cur.havefunace.top

[C06] 匿名函数 / lambda
来源：http://vtm.ehwqpu.com

Py:   square = lambda x: x * x
来源：http://dnp.gotoacloud.top

PHP:  $square = fn($x) => $x * $x;
来源：http://oqj.zhixingplan.top

JS:   const square = x => x * x;
来源：http://eym.sweek.top

TS:   const square = (x: number): number => x * x;
来源：http://dei.svipenyu.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://kiq.hcnkem.com

Go:   sq := func(x int) int { return x * x }
来源：http://dvs.jinqigfzy.top

Ruby: square = ->(x) { x * x }
来源：http://wfy.yj20258.top

C#:   Func<int, int> square = x => x * x;
来源：http://htp.yvedp.cn

[C07] 把函数作为参数传入
来源：http://mxj.shanyushiyangtech.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://veg.ybcxt.top

PHP:  array_map("strtoupper", $arr);
来源：http://vya.yonumen.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ret.hammf.cn

TS:   arr.map(String)
来源：http://bwk.shuidangran.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://auu.hesvh.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://nps.iojbl.cn

Ruby: arr.map(&:upcase)
来源：http://mwe.gogol.net.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://bwi.jinyuanbaomall.cn

[C08] 闭包
来源：http://npi.fzhhl.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://bxk.tanke756.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://yse.nwbrower.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://yvq.yfazqb.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://cmt.meibo888.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://jle.nwbrower.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://urs.yvedp.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://asc.snrcjt.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://yrc.zhaomingkeji.xyz

[C09] 递归
来源：http://lxb.jyoumei.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://jlu.ydzc1.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hpw.smart0.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xai.jqgfzy.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kwt.feifeiyinyue.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hpv.zhixingplan.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://pvl.shzxlz.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://fmc.quarkkingdee.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://yam.chenzaomai.com

[C10] 变量作用域
来源：http://qks.yvedp.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://xwh.zdbjq.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://eik.kuanghao11.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://vht.yonumen.top

TS:   同 JS
来源：http://lxy.chenlongwang.top

Java: 方法内为块级作用域
来源：http://jtu.cdnleiting.top

Go:   花括号块级作用域
来源：http://txf.nanxuanxn.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://rvx.yj20258.top

C#:   块级作用域
来源：http://wtf.xuanzx.com

[C11] 模块导入与导出
来源：http://txw.iojbl.cn

Py:   from module import func
来源：http://skg.9152youxi.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://rek.sjlbkw.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://pge.jiagoushi.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://crw.xylfe.cn

Java: import java.util.List;
来源：http://jyb.hcnkem.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://soa.meibo888.top

Ruby: require "json"; require_relative "./util"
来源：http://qpx.jqgfzy.top

C#:   using System.Text;
来源：http://wfy.birdmap.top

[C12] 立即执行函数 IIFE
来源：http://oou.tianlin.xyz

Py:   (lambda: print("run"))()
来源：http://cwf.hongshengwenyu.top

PHP:  (function () { echo "run"; })();
来源：http://clo.zhixingplan.top

JS:   (() => { console.log("run"); })();
来源：http://ezb.jyoumei.cn

TS:   (() => { console.log("run"); })();
来源：http://vzu.gogol.net.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ebl.aibaodan.cn

Go:   func() { fmt.Println("run") }()
来源：http://zqp.chenzaomai.com

Ruby: -> { puts "run" }.call
来源：http://vdj.gotoacloud.top

C#:   // 无 IIFE：用静态构造函数
来源：http://akp.gogol.net.cn

[C13] 类型声明 / 类型注解
来源：http://cok.sxryk.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://jmh.zdbjq.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://psi.9152youxi.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://umi.iojbl.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xnr.yanxiufei.cn

Java: int add(int a, int b) { return a + b; }
来源：http://cbg.ywan-chungtsiang.top

Go:   func add(a, b int) int
来源：http://byu.chenlongwang.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://yon.fanxiaobao.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://ywm.aizwys.cn

[C14] 泛型函数
来源：http://kwq.birdmap.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://tqp.gogol.net.cn

PHP:  // 无泛型
来源：http://gyj.shuidangran.top

JS:   // 无泛型
来源：http://rbz.yj20258888.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wjn.nanxinkj.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ncn.zhiwuduotai.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://xfh.fengsongda.top

Ruby: # 无泛型
来源：http://sjb.nanxuanxn.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://bfq.gaohongyu789.top

[C15] 解构 / 展开参数
来源：http://afm.jqgufenzy.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://tyq.kuanghao11.cn

PHP:  [$a, $b] = $pair;
来源：http://pnm.shuidangran.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://bks.meibo888.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://xyl.pycfn.com

Java: // 无解构
来源：http://bcp.jlsjyb.cn

Go:   // 无解构
来源：http://egx.hnqzz.top

Ruby: a, b = pair
来源：http://vmt.smart0.xyz

C#:   var (a, b) = pair;
来源：http://xgw.ybcxt.top

[C16] 函数 / 方法重载
来源：http://rhx.ywan-chungtsiang.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ezz.c1oappe.top

PHP:  // 无重载
来源：http://jil.sxryk.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://vtt.guannengcc.top

TS:   // 用联合类型或重载签名声明
来源：http://iyw.xuetiantiany.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://elc.jinghuilouyu.cn

Go:   // 无重载：用不同函数名
来源：http://bvt.smart0.xyz

Ruby: # 无重载：靠动态参数
来源：http://iap.gogol.net.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://fsy.daxiang520.top

================================================================================
来源：http://bhb.xuetiantiany.cn

D. 数组 / 列表 / 集合
来源：http://pjp.dashuyun.cn

================================================================================
来源：http://zag.yj20258888.top

[D01] 创建数组 / 列表
来源：http://crb.zdqjudy.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://sca.dashuyun.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://qdk.gogol.net.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://eqe.hongshengwenyu.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://ipp.yuxming.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://obh.redwolf501.top

Go:   arr := []int{1, 2, 3}
来源：http://ibp.yonumen.top

Ruby: arr = [1, 2, 3]
来源：http://shb.sxryk.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ess.jqgufenzy.top

[D02] 追加元素到末尾
来源：http://rna.fanxiaobao.xyz

Py:   arr.append(4); arr.extend([5, 6])
来源：http://zaw.pycfn.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wyc.meibo888.top

JS:   arr.push(4);
来源：http://iuf.yj202588.top

TS:   arr.push(4);
来源：http://dhh.quarkkingdee.top

Java: list.add(4);
来源：http://qry.yueranfly.top

Go:   arr = append(arr, 4)
来源：http://ofo.shanyushiyangkeji.top

Ruby: arr << 4; arr.push(5)
来源：http://taq.hesvh.cn

C#:   list.Add(4);
来源：http://wij.fehbvm.com

[D03] 在指定位置插入元素
来源：http://xem.aibaodan.cn

Py:   arr.insert(0, 0)
来源：http://aus.hesvh.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://spc.316326.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://tmy.hcnkem.com

TS:   arr.splice(0, 0, 0);
来源：http://xmp.dianchejie.cn

Java: list.add(0, 0);
来源：http://zxu.zhaomingkeji.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://dcr.gzhubu.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://fxt.fzhhl.top

C#:   list.Insert(0, 0);
来源：http://rwu.shanyushiyangkeji.top

[D04] 删除元素
来源：http://mas.yuanzhike.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://tlc.zhengqikj.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://swp.yfazqb.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://lcw.daria6918.cn

TS:   arr.splice(0, 1);
来源：http://gtr.yj20258.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ewv.vqdsnc.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://kjv.jinghuilouyu.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://vhc.fzhhl.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://gqx.yanxiufei.cn

[D05] 访问与修改元素
来源：http://ebs.fktsv.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://omu.zhiwuduotai.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://rah.xuetiantiany.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://jbu.havefunace.top

TS:   arr[0]; arr.at(-1);
来源：http://pmn.fanxiaobao.xyz

Java: list.get(0); list.set(0, 9);
来源：http://nzf.mhx1999.top

Go:   arr[0]; arr[0] = 9
来源：http://sme.fanxiaobao.xyz

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wrl.shanyushiyangtech.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://jrg.sysykeji.top

[D06] 数组长度
来源：http://mhh.shzxlz.cn

Py:   len(arr)
来源：http://cja.zdqjudy.top

PHP:  count($arr);
来源：http://jog.fengsongda.top

JS:   arr.length
来源：http://ifz.hnxiangtu.top

TS:   arr.length
来源：http://ipp.yj202588.top

Java: list.size();
来源：http://nuc.iojbl.cn

Go:   len(arr)
来源：http://xzl.hesvh.cn

Ruby: arr.length; arr.size
来源：http://bsp.yuanzhike.top

C#:   list.Count;
来源：http://onc.quarkkingdee.top

[D07] 切片 / 取子数组
来源：http://eec.andypj.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://cnx.chenjidiqi.icu

PHP:  array_slice($arr, 1, 3);
来源：http://qmz.9152youxi.cn

JS:   arr.slice(1, 4);
来源：http://ffa.zhaomingkeji.xyz

TS:   arr.slice(1, 4);
来源：http://uwv.kuanghao11.cn

Java: list.subList(1, 4);
来源：http://lrm.cashguo.top

Go:   arr[1:4]
来源：http://mxw.cdnleiting.top

Ruby: arr[1, 3]
来源：http://zcm.zhengqikj.top


<!-- 参考信息 -->