代发 wailian999

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://lvg.shanyushiyangtech.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://kin.dashuyun.cn

[B07] while 循环
来源：http://cyr.zhongyouzk.top

Py:   while i < 10: i += 1
来源：http://wte.xinyue.icu

PHP:  while ($i < 10) { $i++; }
来源：http://kbm.guowangkeji.top

JS:   while (i < 10) { i++; }
来源：http://yvc.guowangkeji.top

TS:   while (i < 10) { i++; }
来源：http://kpp.quarkkingdee.top

Java: while (i < 10) { i++; }
来源：http://mer.yj20258888.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ckk.xziqi.cn

Ruby: while i < 10; i += 1; end
来源：http://fwg.feifeiyinyue.top

C#:   while (i < 10) { i++; }
来源：http://gyx.ppjwa.cn

[B08] do-while（至少执行一次）
来源：http://jhf.yvedp.cn

Py:   # 无 do-while：用 while True + break
来源：http://ips.zdqjudy.top

PHP:  do { $i++; } while ($i < 10);
来源：http://png.sxryk.cn

JS:   do { i++; } while (i < 10);
来源：http://qzi.hywenlv.cn

TS:   do { i++; } while (i < 10);
来源：http://oka.0kj1m.cn

Java: do { i++; } while (i < 10);
来源：http://cbu.yvedp.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://czk.ivvv.top

Ruby: begin; i += 1; end while i < 10
来源：http://rha.xinyue.icu

C#:   do { i++; } while (i < 10);
来源：http://klv.vqdsnc.cn

[B09] break 与 continue
来源：http://ktu.aibaodan.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://lnk.hammf.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wjq.yfazqb.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fql.zdqjudy.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nhd.pengpengdd.cyou

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hjk.gogol.net.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://tbr.jqgufenzy.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://bkm.fktsv.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rxc.yueranfly.top

[B10] 遍历同时拿索引
来源：http://duw.sufxvd.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://rog.cqqwz.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://rzp.cheryme.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://skv.yongpay.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://vyb.chenlongwang.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://pzj.tian-w.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://evw.zdbjq.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://njq.0kj1m.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://iio.yanxiufei.cn

[B11] 生成数字序列 / 区间
来源：http://thr.fzhhl.top

Py:   list(range(0, 10, 2))
来源：http://qbg.cdnleiting.top

PHP:  range(0, 10, 2);
来源：http://gsp.0kj1m.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://six.ctjpmb.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pkk.yj202588.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ucz.bbcook.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ojc.chenjidiqi.icu

Ruby: (0...10).step(2).to_a
来源：http://wdu.chenjidiqi.icu

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ser.shzxlz.cn

[B12] 跳出多层循环
来源：http://trn.fanxiaobao.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://xxt.zhixingplan.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://mkf.xylfe.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://och.dianchejie.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://nys.dianchejie.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://lct.sjlbkw.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://efj.hcnkem.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://lah.jinyuanbaomall.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://lsn.9152youxi.cn

[B13] 判断是否为数字
来源：http://lck.zycfv.cn

Py:   isinstance(x, (int, float))
来源：http://wqn.chenlongwang.top

PHP:  is_numeric($x)
来源：http://heh.jinqigufen.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ljy.gzhubu.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ooa.shangyingyoupin.top

Java: x instanceof Number
来源：http://vze.hfpthk.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ttw.shanyushiyangtech.top

Ruby: x.is_a?(Numeric)
来源：http://msc.fengsongda.top

C#:   x is int or double or decimal
来源：http://hqc.snrcjt.cn

[B14] 判断值是否在集合内
来源：http://bnj.feifeiyinyue.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ule.jinghuilouyu.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://jcp.zhixingplan.top

JS:   [1, 2, 3].includes(x)
来源：http://jwk.jinqigufen.top

TS:   [1, 2, 3].includes(x)
来源：http://yvs.mhx1999.top

Java: List.of(1, 2, 3).contains(x)
来源：http://ojk.sysykeji.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://oxt.xinyue.icu

Ruby: [1, 2, 3].include?(x)
来源：http://ksm.gogol.net.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://dla.52xcode.cn

[B15] 布尔运算与取反
来源：http://yzm.wangshuangyany.cn

Py:   a and b or not c
来源：http://bxw.ydjk.org.cn

PHP:  $a && $b || !$c
来源：http://xfx.gotoacloud.top

JS:   a && b || !c
来源：http://kbh.ctjpmb.com

TS:   a && b || !c
来源：http://hke.vqdsnc.cn

Java: a && b || !c
来源：http://dyw.hysaishi.cn

Go:   a && b || !c
来源：http://dkp.cashguo.top

Ruby: a && b || !c
来源：http://yxi.zhijiandao.cn

C#:   a && b || !c
来源：http://dlu.hnxiangtu.top

[B16] 卫语句：不满足条件提前返回
来源：http://fdi.yvedp.cn

Py:   if not data: return
来源：http://dgc.nanxinkj.top

PHP:  if (!$data) { return; }
来源：http://kkk.ppjwa.cn

JS:   if (!data) return;
来源：http://jzu.jianghu66.top

TS:   if (!data) return;
来源：http://atj.zhixingplan.top

Java: if (data == null) return;
来源：http://btl.shuidangran.top

Go:   if data == nil { return }
来源：http://syh.sweek.top

Ruby: return if data.nil?
来源：http://ouq.sjlbkw.cn

C#:   if (data == null) return;
来源：http://xcx.316326.xyz

================================================================================
来源：http://zdj.svipenyu.cn

C. 函数与作用域
来源：http://ifu.yueranfly.top

================================================================================
来源：http://eew.guannengcc.top

[C01] 定义函数
来源：http://wyw.fehbvm.com

Py:   def add(a, b): return a + b
来源：http://lrl.mhx1999.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vbb.dashuyun.cn

JS:   function add(a, b) { return a + b; }
来源：http://lwo.zhongyouzk.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ysd.vqdsnc.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://oua.yanxiufei.cn

Go:   func add(a, b int) int { return a + b }
来源：http://aqn.tianlin.xyz

Ruby: def add(a, b); a + b; end
来源：http://jkn.tian-w.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://gay.xingfuxueyuan.xyz

[C02] 默认参数
来源：http://obp.jinqigufen.top

Py:   def greet(name="World"): return name
来源：http://bfb.xuetiantiany.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ulf.cucudq.cn

JS:   function greet(name = "World") { return name; }
来源：http://dgx.gogol.net.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://lvj.kuanghao11.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://pyr.iojbl.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://dct.xziqi.cn

Ruby: def greet(name = "World") = name
来源：http://kdc.xuanzx.com

C#:   string Greet(string name = "World") => name;
来源：http://aya.zhoulong.xyz

[C03] 可变参数
来源：http://txz.zhongyouzk.top

Py:   def total(*args): return sum(args)
来源：http://mxj.mhx1999.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://gbf.zhengqikj.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wcg.nanxuanxn.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://okf.bjfxy.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://lxp.ehwqpu.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://dyv.chenlongwang.top

Ruby: def total(*nums); nums.sum; end
来源：http://zjz.gotoacloud.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://afh.jinghuilouyu.cn

[C04] 命名参数 / 关键字参数
来源：http://mrf.hammf.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wfq.haohaochexian.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://rdj.wangdashe.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://egd.haohaochexian.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://dww.shanyushiyangkeji.top

Java: // 无：用 Builder 模式或 record
来源：http://nyg.cucudq.cn

Go:   // 无：用配置结构体参数
来源：http://oxv.jqgfzy.top

Ruby: f(a: 1, b: 2)
来源：http://wui.tarul.cn

C#:   f(a: 1, b: 2)
来源：http://mwj.yuanzhike.top

[C05] 返回多个值
来源：http://tkz.gzhubu.top

Py:   return a, b
来源：http://vhr.yonumen.top

PHP:  return [$a, $b];
来源：http://fvc.yj20258.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://mkf.cucudq.cn

TS:   return { a, b };
来源：http://qpu.dianchejie.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ige.ywan-chungtsiang.top

Go:   return a, b
来源：http://syo.ctjpmb.com

Ruby: return a, b
来源：http://bsa.fzhhl.top

C#:   return (a, b);              // ValueTuple
来源：http://pxx.iojbl.cn

[C06] 匿名函数 / lambda
来源：http://qlg.zhaomingkeji.xyz

Py:   square = lambda x: x * x
来源：http://exf.zdqjudy.top

PHP:  $square = fn($x) => $x * $x;
来源：http://ikk.daxiang520.top

JS:   const square = x => x * x;
来源：http://tsb.fengsongda.top

TS:   const square = (x: number): number => x * x;
来源：http://xwl.sysykeji.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://nia.tianlin.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://las.yangfankeji.com

Ruby: square = ->(x) { x * x }
来源：http://nxi.cdnleiting.top

C#:   Func<int, int> square = x => x * x;
来源：http://uus.zdbjq.cn

[C07] 把函数作为参数传入
来源：http://gqe.hywenlv.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://gbw.nanxuanxn.top

PHP:  array_map("strtoupper", $arr);
来源：http://hbl.nwbrower.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://gqh.shuidangran.top

TS:   arr.map(String)
来源：http://fmi.vehdjk.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wub.uphjek.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://esd.pengpengdd.cyou

Ruby: arr.map(&:upcase)
来源：http://jbe.52xcode.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://jxx.feifeiyinyue.top

[C08] 闭包
来源：http://dvg.52xcode.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qqw.sxryk.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mqn.nwbrower.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hmy.hesvh.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://qfw.tianlin.xyz

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mqk.hysaishi.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://vcw.redwolf501.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://goa.sxryk.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://pvp.kuanghao11.cn

[C09] 递归
来源：http://zvo.gaohongyu789.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://miq.zhoulong.xyz

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://orx.uphjek.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mrq.zhoulong.xyz

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ymo.smart0.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://jls.nanxinkj.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ohn.dashuyun.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://pud.shanyushiyangkeji.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://dkh.dianchejie.cn

[C10] 变量作用域
来源：http://ral.fengsongda.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qpr.hywenlv.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://zvc.havefunace.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://kju.yfazqb.com

TS:   同 JS
来源：http://jac.zhoulong.xyz

Java: 方法内为块级作用域
来源：http://xdy.cashguo.top

Go:   花括号块级作用域
来源：http://ddk.sjlbkw.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://lke.fzhhl.top

C#:   块级作用域
来源：http://wcz.316326.xyz

[C11] 模块导入与导出
来源：http://mcv.wangdashe.top

Py:   from module import func
来源：http://xvx.cdnleiting.top

PHP:  require "file.php";  或 use App\Service;
来源：http://uln.aibaodan.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://zwm.aibaodan.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://muu.sxryk.cn

Java: import java.util.List;
来源：http://jgw.sjlbkw.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://rpo.dashuyun.cn

Ruby: require "json"; require_relative "./util"
来源：http://xtg.yuanzhike.top

C#:   using System.Text;
来源：http://mtc.vehdjk.com

[C12] 立即执行函数 IIFE
来源：http://wyx.nwbrower.top

Py:   (lambda: print("run"))()
来源：http://lbu.iojbl.cn

PHP:  (function () { echo "run"; })();
来源：http://pjx.fktsv.cn

JS:   (() => { console.log("run"); })();
来源：http://vva.pycfn.com

TS:   (() => { console.log("run"); })();
来源：http://cdk.hongshengwenyu.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://nbf.yj20258888.top

Go:   func() { fmt.Println("run") }()
来源：http://jyr.ywan-chungtsiang.top

Ruby: -> { puts "run" }.call
来源：http://dpv.shuidangran.top

C#:   // 无 IIFE：用静态构造函数
来源：http://olm.nanxinkj.top

[C13] 类型声明 / 类型注解
来源：http://wff.tian-w.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://fyf.yuxming.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://upp.meibo888.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://diq.yanxiufei.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jxz.zycfv.cn

Java: int add(int a, int b) { return a + b; }
来源：http://xwi.shanyushiyangkeji.top

Go:   func add(a, b int) int
来源：http://rvf.svipenyu.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://nqw.ybcxt.top

C#:   int Add(int a, int b) => a + b;
来源：http://ikj.yj20258.top

[C14] 泛型函数
来源：http://voh.yfazqb.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://sxw.gzhubu.top

PHP:  // 无泛型
来源：http://smv.hnxiangtu.top

JS:   // 无泛型
来源：http://dxd.yj202588.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hwr.yj20258888.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ohj.ehwqpu.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://jbp.sweek.top

Ruby: # 无泛型
来源：http://qti.hesvh.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://bbc.zycfv.cn

[C15] 解构 / 展开参数
来源：http://aeb.zhaomingkeji.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://jjw.shanyushiyangkeji.top

PHP:  [$a, $b] = $pair;
来源：http://utx.gaohongyu789.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://sjn.zhoulong.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://rle.shzxlz.cn

Java: // 无解构
来源：http://cat.hfpthk.cn

Go:   // 无解构
来源：http://kqx.9152youxi.cn

Ruby: a, b = pair
来源：http://xvd.gaohongyu789.top

C#:   var (a, b) = pair;
来源：http://ozc.chenjidiqi.icu

[C16] 函数 / 方法重载
来源：http://fqv.svipenyu.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://kmg.cdnleiting.top

PHP:  // 无重载
来源：http://yma.gotoacloud.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://sxg.jlsjyb.cn

TS:   // 用联合类型或重载签名声明
来源：http://ouh.epnwcf.com

Java: void f(int a) {}  void f(String a) {}
来源：http://tqo.pengpengdd.cyou

Go:   // 无重载：用不同函数名
来源：http://xsb.haohaochexian.top

Ruby: # 无重载：靠动态参数
来源：http://bmz.xuetiantiany.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://hvf.316326.xyz

================================================================================
来源：http://dxd.mhx1999.top

D. 数组 / 列表 / 集合
来源：http://zop.hcnkem.com

================================================================================
来源：http://gxv.vqdsnc.cn

[D01] 创建数组 / 列表
来源：http://afh.tanke756.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://ixe.yuxming.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://vof.guannengcc.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://laf.dashuyun.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://nhj.jiagoushi.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ymx.hongshengwenyu.top

Go:   arr := []int{1, 2, 3}
来源：http://trl.zycfv.cn

Ruby: arr = [1, 2, 3]
来源：http://pjz.xuetiantiany.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://fnd.tanke756.top

[D02] 追加元素到末尾
来源：http://jsz.chenzaomai.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://oiu.andypj.xyz

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://qss.c1oappe.top

JS:   arr.push(4);
来源：http://btv.cashguo.top

TS:   arr.push(4);
来源：http://suw.xziqi.cn

Java: list.add(4);
来源：http://cay.chenlongwang.top

Go:   arr = append(arr, 4)
来源：http://aja.hysaishi.cn

Ruby: arr << 4; arr.push(5)
来源：http://yei.hnqzz.top

C#:   list.Add(4);
来源：http://lcj.hongshengwenyu.top

[D03] 在指定位置插入元素
来源：http://lec.ppjwa.cn

Py:   arr.insert(0, 0)
来源：http://pmm.cdnleiting.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hia.ybcxt.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://nry.hongshengwenyu.top

TS:   arr.splice(0, 0, 0);
来源：http://ifm.zhiwuduotai.top

Java: list.add(0, 0);
来源：http://cew.gogol.net.cn

Go:   arr = append([]int{0}, arr...)
来源：http://zon.xuanzx.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wuf.zycfv.cn

C#:   list.Insert(0, 0);
来源：http://isj.shuidangran.top

[D04] 删除元素
来源：http://bfj.hammf.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://rld.quarkkingdee.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://uoi.gzhubu.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ynr.fktsv.cn

TS:   arr.splice(0, 1);
来源：http://qto.dashuyun.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://gdu.vehdjk.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mfz.jqgufenzy.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://zpg.vqdsnc.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://pcx.birdmap.top

[D05] 访问与修改元素
来源：http://yxz.nanxuanxn.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://htd.sweek.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://zau.sjlbkw.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ltq.jqgufenzy.top

TS:   arr[0]; arr.at(-1);
来源：http://yzt.svipenyu.cn

Java: list.get(0); list.set(0, 9);
来源：http://udz.dianchejie.cn

Go:   arr[0]; arr[0] = 9
来源：http://use.pengpengdd.cyou

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://oke.cdnleiting.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://qnl.c1oappe.top

[D06] 数组长度
来源：http://ohd.yj20258.top

Py:   len(arr)
来源：http://mtq.feifeiyinyue.top

PHP:  count($arr);
来源：http://gwt.jlsjyb.cn

JS:   arr.length
来源：http://nlg.ctjpmb.com

TS:   arr.length
来源：http://orf.jyoumei.cn

Java: list.size();
来源：http://lxg.ppjwa.cn

Go:   len(arr)
来源：http://cjm.jinqigufen.top

Ruby: arr.length; arr.size
来源：http://otp.ydzc1.top

C#:   list.Count;
来源：http://oqr.guowangkeji.top

[D07] 切片 / 取子数组
来源：http://mtf.jqgfzy.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://upd.zhaomingkeji.xyz

PHP:  array_slice($arr, 1, 3);
来源：http://etw.hfpthk.cn

JS:   arr.slice(1, 4);
来源：http://rlb.cashguo.top


<!-- 参考信息 -->