代发 wailian999

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ktq.andypj.xyz

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://brr.hnqzz.top

[B07] while 循环
来源：http://syc.xylfe.cn

Py:   while i < 10: i += 1
来源：http://mng.aizwys.cn

PHP:  while ($i < 10) { $i++; }
来源：http://yyv.quarkkingdee.top

JS:   while (i < 10) { i++; }
来源：http://kzz.svipenyu.cn

TS:   while (i < 10) { i++; }
来源：http://ffc.bbcook.cn

Java: while (i < 10) { i++; }
来源：http://ddj.andypj.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://iev.chenlongwang.top

Ruby: while i < 10; i += 1; end
来源：http://mft.hnxiangtu.top

C#:   while (i < 10) { i++; }
来源：http://xue.ctjpmb.com

[B08] do-while（至少执行一次）
来源：http://hzi.xinyue.icu

Py:   # 无 do-while：用 while True + break
来源：http://gvh.tianlin.xyz

PHP:  do { $i++; } while ($i < 10);
来源：http://xoj.guowangkeji.top

JS:   do { i++; } while (i < 10);
来源：http://kbn.gogol.net.cn

TS:   do { i++; } while (i < 10);
来源：http://vsl.sufxvd.cn

Java: do { i++; } while (i < 10);
来源：http://crd.gzhubu.top

Go:   for { i++; if i >= 10 { break } }
来源：http://ymt.zhoulong.xyz

Ruby: begin; i += 1; end while i < 10
来源：http://zec.zhiwuduotai.top

C#:   do { i++; } while (i < 10);
来源：http://yfd.c1oappe.top

[B09] break 与 continue
来源：http://zjt.uphjek.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ikq.zhoulong.xyz

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://zsv.c1oappe.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bcl.hnqzz.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qoo.ydjk.org.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gsa.epnwcf.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://frt.gzhubu.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xkt.jinqigufen.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bsx.ybcxt.top

[B10] 遍历同时拿索引
来源：http://hsx.xingfuxueyuan.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://syi.havefunace.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://zkx.zhijiandao.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://opi.epnwcf.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ilk.xziqi.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://uxc.fanxiaobao.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://pqu.aibaodan.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hri.fanxiaobao.xyz

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://htv.hnqzz.top

[B11] 生成数字序列 / 区间
来源：http://rmx.snrcjt.cn

Py:   list(range(0, 10, 2))
来源：http://yrk.shanyushiyangtech.top

PHP:  range(0, 10, 2);
来源：http://ava.fehbvm.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nsm.tianlin.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://omx.shzxlz.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://nji.jiagoushi.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://eae.jyoumei.cn

Ruby: (0...10).step(2).to_a
来源：http://nyi.hywenlv.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://nmo.jianghu66.top

[B12] 跳出多层循环
来源：http://rzs.jyoumei.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ylx.hnqzz.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://nga.andypj.xyz

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://jit.zhijiandao.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://uhd.chenzaomai.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://xxe.hnxiangtu.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://bdv.tianlin.xyz

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://vsd.nwbrower.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://tbt.jyoumei.cn

[B13] 判断是否为数字
来源：http://gom.cashguo.top

Py:   isinstance(x, (int, float))
来源：http://ljv.jiagoushi.top

PHP:  is_numeric($x)
来源：http://pwn.tanke756.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jjp.shanyushiyangkeji.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wfs.redwolf501.top

Java: x instanceof Number
来源：http://inq.zdbjq.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ybr.vehdjk.com

Ruby: x.is_a?(Numeric)
来源：http://ddz.yonumen.top

C#:   x is int or double or decimal
来源：http://qof.daria6918.cn

[B14] 判断值是否在集合内
来源：http://dli.tanke756.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://iog.316326.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://gas.chenzaomai.com

JS:   [1, 2, 3].includes(x)
来源：http://uyv.ivvv.top

TS:   [1, 2, 3].includes(x)
来源：http://wsf.kuanghao11.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://kip.epnwcf.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://zhd.iojbl.cn

Ruby: [1, 2, 3].include?(x)
来源：http://iiq.feifeiyinyue.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://xwq.0kj1m.cn

[B15] 布尔运算与取反
来源：http://jwr.cashguo.top

Py:   a and b or not c
来源：http://vkd.yj202588.top

PHP:  $a && $b || !$c
来源：http://luj.yvedp.cn

JS:   a && b || !c
来源：http://rbp.zhixingplan.top

TS:   a && b || !c
来源：http://xoe.fehbvm.com

Java: a && b || !c
来源：http://hfq.andypj.xyz

Go:   a && b || !c
来源：http://mof.nanxuanxn.top

Ruby: a && b || !c
来源：http://ztn.nwbrower.top

C#:   a && b || !c
来源：http://fef.zhixingplan.top

[B16] 卫语句：不满足条件提前返回
来源：http://zcy.0kj1m.cn

Py:   if not data: return
来源：http://fpr.sufxvd.cn

PHP:  if (!$data) { return; }
来源：http://hag.jinqigfzy.top

JS:   if (!data) return;
来源：http://ajs.quarkkingdee.top

TS:   if (!data) return;
来源：http://dyx.fengsongda.top

Java: if (data == null) return;
来源：http://jut.tian-w.cn

Go:   if data == nil { return }
来源：http://ice.316326.xyz

Ruby: return if data.nil?
来源：http://wgj.gotoacloud.top

C#:   if (data == null) return;
来源：http://nex.cqqwz.cn

================================================================================
来源：http://wqf.shangyingyoupin.top

C. 函数与作用域
来源：http://zex.andypj.xyz

================================================================================
来源：http://bff.havefunace.top

[C01] 定义函数
来源：http://zui.dashuyun.cn

Py:   def add(a, b): return a + b
来源：http://yaz.yj202588.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ywj.daxiang520.top

JS:   function add(a, b) { return a + b; }
来源：http://azx.birdmap.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ppt.havefunace.top

Java: static int add(int a, int b) { return a + b; }
来源：http://sqr.zhijiandao.cn

Go:   func add(a, b int) int { return a + b }
来源：http://pfd.c1oappe.top

Ruby: def add(a, b); a + b; end
来源：http://sbs.zdqjudy.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://tgb.shuidangran.top

[C02] 默认参数
来源：http://frg.yj20258.top

Py:   def greet(name="World"): return name
来源：http://rcz.52xcode.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://oqt.kuanghao11.cn

JS:   function greet(name = "World") { return name; }
来源：http://yyc.yvedp.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://jbh.jinghuilouyu.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://rto.cqqwz.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://cal.zhoulong.xyz

Ruby: def greet(name = "World") = name
来源：http://mat.yfazqb.com

C#:   string Greet(string name = "World") => name;
来源：http://xvv.sxryk.cn

[C03] 可变参数
来源：http://iyq.feifeiyinyue.top

Py:   def total(*args): return sum(args)
来源：http://axe.fengsongda.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xrd.xingfuxueyuan.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://zjx.meibo888.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://aap.tarul.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ziv.xylfe.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://xuh.pengpengdd.cyou

Ruby: def total(*nums); nums.sum; end
来源：http://lqv.zhoulong.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://nyu.redwolf501.top

[C04] 命名参数 / 关键字参数
来源：http://dlj.hywenlv.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://sne.chenzaomai.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://lsx.hcnkem.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://zld.hywenlv.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://inb.jqgufenzy.top

Java: // 无：用 Builder 模式或 record
来源：http://lpc.shuidangran.top

Go:   // 无：用配置结构体参数
来源：http://nxe.ybcxt.top

Ruby: f(a: 1, b: 2)
来源：http://zrm.yanxiufei.cn

C#:   f(a: 1, b: 2)
来源：http://amy.nwbrower.top

[C05] 返回多个值
来源：http://kiw.ywan-chungtsiang.top

Py:   return a, b
来源：http://xmq.pycfn.com

PHP:  return [$a, $b];
来源：http://rbe.aizwys.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://rsh.wangshuangyany.cn

TS:   return { a, b };
来源：http://nll.zhijiandao.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://jig.chenjidiqi.icu

Go:   return a, b
来源：http://yhu.sufxvd.cn

Ruby: return a, b
来源：http://mqc.ywan-chungtsiang.top

C#:   return (a, b);              // ValueTuple
来源：http://zna.c1oappe.top

[C06] 匿名函数 / lambda
来源：http://svm.havefunace.top

Py:   square = lambda x: x * x
来源：http://wdj.wangdashe.top

PHP:  $square = fn($x) => $x * $x;
来源：http://xlm.xingfuxueyuan.xyz

JS:   const square = x => x * x;
来源：http://wrz.havefunace.top

TS:   const square = (x: number): number => x * x;
来源：http://nws.shanyushiyangtech.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ijo.sxryk.cn

Go:   sq := func(x int) int { return x * x }
来源：http://dqa.tian-w.cn

Ruby: square = ->(x) { x * x }
来源：http://val.zhengqikj.top

C#:   Func<int, int> square = x => x * x;
来源：http://jfk.ctjpmb.com

[C07] 把函数作为参数传入
来源：http://gpx.fzhhl.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://vrd.daxiang520.top

PHP:  array_map("strtoupper", $arr);
来源：http://jwj.jqgfzy.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://vwo.jqgfzy.top

TS:   arr.map(String)
来源：http://xwo.jlsjyb.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://fhy.shzxlz.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qhg.daxiang520.top

Ruby: arr.map(&:upcase)
来源：http://tmc.cheryme.top

C#:   arr.Select(s => s.ToUpper())
来源：http://fnz.guowangkeji.top

[C08] 闭包
来源：http://dnw.ydjk.org.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://pdt.ydzc1.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://udw.bjfxy.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://fsw.daxiang520.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://itj.zhaomingkeji.xyz

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mff.jiagoushi.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://dmy.xylfe.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://gxi.hnqzz.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://llo.hesvh.cn

[C09] 递归
来源：http://vyh.wangshuangyany.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://gls.fzhhl.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://vvw.ydjk.org.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fdt.jinghuilouyu.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vvm.fehbvm.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://sra.tanke756.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://qlb.cqqwz.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://stl.jinghuilouyu.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://kod.jinqigufen.top

[C10] 变量作用域
来源：http://aeo.zycfv.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mdg.dianchejie.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://dqn.shanyushiyangtech.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ktq.jinqigufen.top

TS:   同 JS
来源：http://lav.ywan-chungtsiang.top

Java: 方法内为块级作用域
来源：http://ebr.nanxuanxn.top

Go:   花括号块级作用域
来源：http://mxu.kuanghao11.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://kbt.sysykeji.top

C#:   块级作用域
来源：http://yke.zdbjq.cn

[C11] 模块导入与导出
来源：http://xdv.wangshuangyany.cn

Py:   from module import func
来源：http://xbv.zhiwuduotai.top

PHP:  require "file.php";  或 use App\Service;
来源：http://phv.gzhubu.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://rov.zdqjudy.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ycf.hnqzz.top

Java: import java.util.List;
来源：http://omf.gotoacloud.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mqu.jiagoushi.top

Ruby: require "json"; require_relative "./util"
来源：http://ora.yfazqb.com

C#:   using System.Text;
来源：http://jlz.zdqjudy.top

[C12] 立即执行函数 IIFE
来源：http://fsy.iojbl.cn

Py:   (lambda: print("run"))()
来源：http://gfc.zhijiandao.cn

PHP:  (function () { echo "run"; })();
来源：http://mdh.quarkkingdee.top

JS:   (() => { console.log("run"); })();
来源：http://qed.shanyushiyangkeji.top

TS:   (() => { console.log("run"); })();
来源：http://tds.tarul.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ifm.fehbvm.com

Go:   func() { fmt.Println("run") }()
来源：http://fih.jinyuanbaomall.cn

Ruby: -> { puts "run" }.call
来源：http://nwe.ydzc1.top

C#:   // 无 IIFE：用静态构造函数
来源：http://dkj.guowangkeji.top

[C13] 类型声明 / 类型注解
来源：http://hgp.gzhubu.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mqm.chenjidiqi.icu

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://aby.nwbrower.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://kvy.jinghuilouyu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lqw.yangfankeji.com

Java: int add(int a, int b) { return a + b; }
来源：http://fzr.jinyuanbaomall.cn

Go:   func add(a, b int) int
来源：http://rdc.uphjek.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://maz.aizwys.cn

C#:   int Add(int a, int b) => a + b;
来源：http://nqw.sxryk.cn

[C14] 泛型函数
来源：http://otl.shanyushiyangtech.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://vii.smart0.xyz

PHP:  // 无泛型
来源：http://cti.nanxinkj.top

JS:   // 无泛型
来源：http://eui.sufxvd.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://qpj.shzxlz.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://vti.tarul.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mxi.52xcode.cn

Ruby: # 无泛型
来源：http://ghe.daxiang520.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://jsr.wangshuangyany.cn

[C15] 解构 / 展开参数
来源：http://jpd.guowangkeji.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://yci.feifeiyinyue.top

PHP:  [$a, $b] = $pair;
来源：http://rjl.ybcxt.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mao.tarul.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wec.jlsjyb.cn

Java: // 无解构
来源：http://ctz.wangshuangyany.cn

Go:   // 无解构
来源：http://uvy.smart0.xyz

Ruby: a, b = pair
来源：http://cxi.jinqigfzy.top

C#:   var (a, b) = pair;
来源：http://lhx.fktsv.cn

[C16] 函数 / 方法重载
来源：http://sol.zhengqikj.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mdt.smart0.xyz

PHP:  // 无重载
来源：http://lsf.shangyingyoupin.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://rwl.xylfe.cn

TS:   // 用联合类型或重载签名声明
来源：http://mua.yuanzhike.top

Java: void f(int a) {}  void f(String a) {}
来源：http://dpe.chenjidiqi.icu

Go:   // 无重载：用不同函数名
来源：http://zbm.cqqwz.cn

Ruby: # 无重载：靠动态参数
来源：http://kld.yj202588.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://jxh.cucudq.cn

================================================================================
来源：http://fvu.gotoacloud.top

D. 数组 / 列表 / 集合
来源：http://pln.xuanzx.com

================================================================================
来源：http://xyk.hysaishi.cn

[D01] 创建数组 / 列表
来源：http://hjx.zdbjq.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://yqw.ivvv.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://xhj.jinyuanbaomall.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://bzj.quarkkingdee.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://qnd.tianlin.xyz

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ulo.pengpengdd.cyou

Go:   arr := []int{1, 2, 3}
来源：http://zep.yonumen.top

Ruby: arr = [1, 2, 3]
来源：http://woy.chenlongwang.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://tdi.daxiang520.top

[D02] 追加元素到末尾
来源：http://qqk.ppjwa.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://cmd.hesvh.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://quf.jinqigfzy.top

JS:   arr.push(4);
来源：http://zih.sweek.top

TS:   arr.push(4);
来源：http://rlb.yj20258.top

Java: list.add(4);
来源：http://cao.hnqzz.top

Go:   arr = append(arr, 4)
来源：http://yiw.cdnleiting.top

Ruby: arr << 4; arr.push(5)
来源：http://jxo.tianlin.xyz

C#:   list.Add(4);
来源：http://fbw.yfazqb.com

[D03] 在指定位置插入元素
来源：http://rbe.shangyingyoupin.top

Py:   arr.insert(0, 0)
来源：http://ghc.andypj.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://juh.uphjek.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://qsv.xylfe.cn

TS:   arr.splice(0, 0, 0);
来源：http://gjq.jinyuanbaomall.cn

Java: list.add(0, 0);
来源：http://zve.cdnleiting.top

Go:   arr = append([]int{0}, arr...)
来源：http://wsl.ydzc1.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://nwc.xylfe.cn

C#:   list.Insert(0, 0);
来源：http://lip.jyoumei.cn

[D04] 删除元素
来源：http://wti.pengpengdd.cyou

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ptm.yongpay.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://pzh.xingfuxueyuan.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://fca.shanyushiyangkeji.top

TS:   arr.splice(0, 1);
来源：http://olr.52xcode.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ogg.redwolf501.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://eam.nanxuanxn.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://cui.hesvh.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ckm.jinqigufen.top

[D05] 访问与修改元素
来源：http://ram.yueranfly.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ygc.haohaochexian.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://iih.cashguo.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://dpi.jiagoushi.top

TS:   arr[0]; arr.at(-1);
来源：http://jzb.cashguo.top

Java: list.get(0); list.set(0, 9);
来源：http://cqd.zdbjq.cn

Go:   arr[0]; arr[0] = 9
来源：http://pdi.yj20258888.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hcc.xziqi.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://tir.jinqigfzy.top

[D06] 数组长度
来源：http://mih.jinghuilouyu.cn

Py:   len(arr)
来源：http://gjn.pycfn.com

PHP:  count($arr);
来源：http://vey.zhiwuduotai.top

JS:   arr.length
来源：http://msv.tanke756.top

TS:   arr.length
来源：http://ckh.jqgufenzy.top

Java: list.size();
来源：http://vxs.zhijiandao.cn

Go:   len(arr)
来源：http://ubr.yfazqb.com

Ruby: arr.length; arr.size
来源：http://tia.hnqzz.top

C#:   list.Count;
来源：http://pxu.xinyue.icu

[D07] 切片 / 取子数组
来源：http://jcj.gzhubu.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qlr.jinqigufen.top

PHP:  array_slice($arr, 1, 3);
来源：http://hmo.yuxming.cn

JS:   arr.slice(1, 4);
来源：http://qkj.ctjpmb.com


<!-- 参考信息 -->