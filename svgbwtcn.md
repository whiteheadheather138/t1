代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://ypd.epnwcf.com

PHP:  do { $i++; } while ($i < 10);
来源：http://esa.yvedp.cn

JS:   do { i++; } while (i < 10);
来源：http://anf.birdmap.top

TS:   do { i++; } while (i < 10);
来源：http://fns.yj20258.top

Java: do { i++; } while (i < 10);
来源：http://ifb.yuanzhike.top

Go:   for { i++; if i >= 10 { break } }
来源：http://wwa.ywan-chungtsiang.top

Ruby: begin; i += 1; end while i < 10
来源：http://ozf.xylfe.cn

C#:   do { i++; } while (i < 10);
来源：http://mmx.hammf.cn

[B09] break 与 continue
来源：http://jjz.feifeiyinyue.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://aus.dianchejie.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://icj.yvedp.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gxb.yj20258888.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://iuj.nanxuanxn.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://aiw.daxiang520.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blw.guannengcc.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://lut.dianchejie.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://syy.jinyuanbaomall.cn

[B10] 遍历同时拿索引
来源：http://mqj.ctjpmb.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mvi.andypj.xyz

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://aba.quarkkingdee.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://qux.tarul.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://jzx.haohaochexian.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://jqn.shanyushiyangtech.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://rrm.jlsjyb.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ugl.kuanghao11.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://nnd.jyoumei.cn

[B11] 生成数字序列 / 区间
来源：http://gol.gogol.net.cn

Py:   list(range(0, 10, 2))
来源：http://eti.gzhubu.top

PHP:  range(0, 10, 2);
来源：http://rhq.tanke756.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zsd.xuanzx.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jkq.vqdsnc.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://vpp.hesvh.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://zrv.316326.xyz

Ruby: (0...10).step(2).to_a
来源：http://anb.smart0.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://cvc.zycfv.cn

[B12] 跳出多层循环
来源：http://zxp.tianlin.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://dzm.yuxming.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://set.wangdashe.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://uni.andypj.xyz

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://vxx.guannengcc.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://qdo.sysykeji.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://rdc.cqqwz.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://vpz.yvedp.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://gnx.chenzaomai.com

[B13] 判断是否为数字
来源：http://syu.daria6918.cn

Py:   isinstance(x, (int, float))
来源：http://bbe.daxiang520.top

PHP:  is_numeric($x)
来源：http://emq.yfazqb.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wlz.tanke756.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://djn.ivvv.top

Java: x instanceof Number
来源：http://byg.pycfn.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://qew.zhengqikj.top

Ruby: x.is_a?(Numeric)
来源：http://qsy.daxiang520.top

C#:   x is int or double or decimal
来源：http://dkh.52xcode.cn

[B14] 判断值是否在集合内
来源：http://zdg.yj202588.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://xzr.jlsjyb.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ybc.gzhubu.top

JS:   [1, 2, 3].includes(x)
来源：http://bkr.ppjwa.cn

TS:   [1, 2, 3].includes(x)
来源：http://pjb.nanxuanxn.top

Java: List.of(1, 2, 3).contains(x)
来源：http://hyi.hcnkem.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ksd.xingfuxueyuan.xyz

Ruby: [1, 2, 3].include?(x)
来源：http://nvg.dashuyun.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://khw.gaohongyu789.top

[B15] 布尔运算与取反
来源：http://cqi.tianlin.xyz

Py:   a and b or not c
来源：http://yni.cucudq.cn

PHP:  $a && $b || !$c
来源：http://ose.hfpthk.cn

JS:   a && b || !c
来源：http://pfd.ctjpmb.com

TS:   a && b || !c
来源：http://qxv.zhongyouzk.top

Java: a && b || !c
来源：http://kch.jyoumei.cn

Go:   a && b || !c
来源：http://dsw.zhongyouzk.top

Ruby: a && b || !c
来源：http://dna.xuanzx.com

C#:   a && b || !c
来源：http://iur.ywan-chungtsiang.top

[B16] 卫语句：不满足条件提前返回
来源：http://sbp.xylfe.cn

Py:   if not data: return
来源：http://flb.nanxuanxn.top

PHP:  if (!$data) { return; }
来源：http://qtw.vehdjk.com

JS:   if (!data) return;
来源：http://ywn.zhaomingkeji.xyz

TS:   if (!data) return;
来源：http://fhd.iojbl.cn

Java: if (data == null) return;
来源：http://kub.gotoacloud.top

Go:   if data == nil { return }
来源：http://pny.fehbvm.com

Ruby: return if data.nil?
来源：http://rlh.nanxuanxn.top

C#:   if (data == null) return;
来源：http://sfh.yueranfly.top

================================================================================
来源：http://ate.pengpengdd.cyou

C. 函数与作用域
来源：http://mtx.yueranfly.top

================================================================================
来源：http://itz.daria6918.cn

[C01] 定义函数
来源：http://qpb.gogol.net.cn

Py:   def add(a, b): return a + b
来源：http://ojw.guannengcc.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xte.0kj1m.cn

JS:   function add(a, b) { return a + b; }
来源：http://psy.shzxlz.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pfy.hfpthk.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://vjv.zhixingplan.top

Go:   func add(a, b int) int { return a + b }
来源：http://wmt.ywan-chungtsiang.top

Ruby: def add(a, b); a + b; end
来源：http://tmj.cheryme.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://cih.xingfuxueyuan.xyz

[C02] 默认参数
来源：http://eyv.sweek.top

Py:   def greet(name="World"): return name
来源：http://iiy.havefunace.top

PHP:  function greet($name = "World") { return $name; }
来源：http://wyn.yongpay.top

JS:   function greet(name = "World") { return name; }
来源：http://ifc.iojbl.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://tgv.kuanghao11.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://wgi.daria6918.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://clq.zdbjq.cn

Ruby: def greet(name = "World") = name
来源：http://sds.chenzaomai.com

C#:   string Greet(string name = "World") => name;
来源：http://xqo.zhijiandao.cn

[C03] 可变参数
来源：http://ham.uphjek.com

Py:   def total(*args): return sum(args)
来源：http://mzy.zdqjudy.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://rgf.cucudq.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://lko.smart0.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://uks.ppjwa.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://fqf.zhijiandao.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wks.zdqjudy.top

Ruby: def total(*nums); nums.sum; end
来源：http://efx.gogol.net.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ehq.xingfuxueyuan.xyz

[C04] 命名参数 / 关键字参数
来源：http://bzc.zhijiandao.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ooi.vqdsnc.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://qjd.fanxiaobao.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://lwu.zdqjudy.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://vhm.redwolf501.top

Java: // 无：用 Builder 模式或 record
来源：http://baf.daxiang520.top

Go:   // 无：用配置结构体参数
来源：http://yjy.sxryk.cn

Ruby: f(a: 1, b: 2)
来源：http://ekv.iojbl.cn

C#:   f(a: 1, b: 2)
来源：http://eqn.zycfv.cn

[C05] 返回多个值
来源：http://ius.gotoacloud.top

Py:   return a, b
来源：http://ymw.hnqzz.top

PHP:  return [$a, $b];
来源：http://tub.yongpay.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://tde.zhoulong.xyz

TS:   return { a, b };
来源：http://qyd.jqgfzy.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://tuh.tarul.cn

Go:   return a, b
来源：http://vsn.ehwqpu.com

Ruby: return a, b
来源：http://ixa.daria6918.cn

C#:   return (a, b);              // ValueTuple
来源：http://rvc.zhoulong.xyz

[C06] 匿名函数 / lambda
来源：http://amo.wangshuangyany.cn

Py:   square = lambda x: x * x
来源：http://xqx.guowangkeji.top

PHP:  $square = fn($x) => $x * $x;
来源：http://qfl.vqdsnc.cn

JS:   const square = x => x * x;
来源：http://tcf.iojbl.cn

TS:   const square = (x: number): number => x * x;
来源：http://cjc.jqgfzy.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://dxi.hysaishi.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ngi.bbcook.cn

Ruby: square = ->(x) { x * x }
来源：http://vru.sjlbkw.cn

C#:   Func<int, int> square = x => x * x;
来源：http://hbw.birdmap.top

[C07] 把函数作为参数传入
来源：http://vse.zhoulong.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://frt.xinyue.icu

PHP:  array_map("strtoupper", $arr);
来源：http://pgj.vehdjk.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://rmf.52xcode.cn

TS:   arr.map(String)
来源：http://bvo.yj20258.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://cgu.zdqjudy.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://jgh.gaohongyu789.top

Ruby: arr.map(&:upcase)
来源：http://usm.guowangkeji.top

C#:   arr.Select(s => s.ToUpper())
来源：http://taa.snrcjt.cn

[C08] 闭包
来源：http://tfu.hcnkem.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://nvm.zhongyouzk.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://pko.cucudq.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://xrg.hnxiangtu.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://oyr.mhx1999.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://nat.shanyushiyangkeji.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ght.sweek.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://fsb.hongshengwenyu.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mro.zhoulong.xyz

[C09] 递归
来源：http://dff.yvedp.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://znq.bjfxy.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://svl.zhaomingkeji.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://erx.fengsongda.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hpe.hongshengwenyu.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://iyi.gzhubu.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ipn.shanyushiyangtech.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://kjp.yuanzhike.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://cwi.kuanghao11.cn

[C10] 变量作用域
来源：http://hoe.snrcjt.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://vcb.xuetiantiany.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mth.gogol.net.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xsl.chenzaomai.com

TS:   同 JS
来源：http://ztr.sxryk.cn

Java: 方法内为块级作用域
来源：http://ahm.cashguo.top

Go:   花括号块级作用域
来源：http://dtd.aizwys.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://oog.nanxuanxn.top

C#:   块级作用域
来源：http://yjy.daxiang520.top

[C11] 模块导入与导出
来源：http://osb.jinqigfzy.top

Py:   from module import func
来源：http://pmi.quarkkingdee.top

PHP:  require "file.php";  或 use App\Service;
来源：http://qro.yvedp.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://yaq.ybcxt.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://cui.fehbvm.com

Java: import java.util.List;
来源：http://tfy.wangshuangyany.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://dcl.tarul.cn

Ruby: require "json"; require_relative "./util"
来源：http://diq.yfazqb.com

C#:   using System.Text;
来源：http://zvl.yuxming.cn

[C12] 立即执行函数 IIFE
来源：http://rhr.havefunace.top

Py:   (lambda: print("run"))()
来源：http://cge.52xcode.cn

PHP:  (function () { echo "run"; })();
来源：http://cpm.yj202588.top

JS:   (() => { console.log("run"); })();
来源：http://xhs.wangdashe.top

TS:   (() => { console.log("run"); })();
来源：http://lse.yj202588.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mfl.ivvv.top

Go:   func() { fmt.Println("run") }()
来源：http://doj.shangyingyoupin.top

Ruby: -> { puts "run" }.call
来源：http://ovp.fktsv.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://fny.jinqigfzy.top

[C13] 类型声明 / 类型注解
来源：http://okc.yvedp.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ryc.shzxlz.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://trn.uphjek.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://cun.zhengqikj.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pqx.zhijiandao.cn

Java: int add(int a, int b) { return a + b; }
来源：http://eoi.yj20258888.top

Go:   func add(a, b int) int
来源：http://rbp.0kj1m.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://tsm.pycfn.com

C#:   int Add(int a, int b) => a + b;
来源：http://abf.sweek.top

[C14] 泛型函数
来源：http://gdn.gaohongyu789.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://cuw.tian-w.cn

PHP:  // 无泛型
来源：http://vco.jqgfzy.top

JS:   // 无泛型
来源：http://vyp.c1oappe.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ipn.jyoumei.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://xto.ivvv.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mkf.snrcjt.cn

Ruby: # 无泛型
来源：http://sks.ydzc1.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://sdr.feifeiyinyue.top

[C15] 解构 / 展开参数
来源：http://sav.sysykeji.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://eqn.birdmap.top

PHP:  [$a, $b] = $pair;
来源：http://qaj.shanyushiyangtech.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://rcb.9152youxi.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://jzt.havefunace.top

Java: // 无解构
来源：http://bil.jinyuanbaomall.cn

Go:   // 无解构
来源：http://ebh.cdnleiting.top

Ruby: a, b = pair
来源：http://zmm.yongpay.top

C#:   var (a, b) = pair;
来源：http://uws.hesvh.cn

[C16] 函数 / 方法重载
来源：http://oep.iojbl.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://lxz.zdqjudy.top

PHP:  // 无重载
来源：http://qnz.xingfuxueyuan.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://fwo.hywenlv.cn

TS:   // 用联合类型或重载签名声明
来源：http://hck.zycfv.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://bdj.tanke756.top

Go:   // 无重载：用不同函数名
来源：http://pmi.ybcxt.top

Ruby: # 无重载：靠动态参数
来源：http://faw.9152youxi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://zar.havefunace.top

================================================================================
来源：http://mco.shanyushiyangtech.top

D. 数组 / 列表 / 集合
来源：http://fbs.zycfv.cn

================================================================================
来源：http://kxs.ydjk.org.cn

[D01] 创建数组 / 列表
来源：http://vfe.cheryme.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://ntf.yueranfly.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://gee.smart0.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://owy.tarul.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://eom.yonumen.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://bxp.xylfe.cn

Go:   arr := []int{1, 2, 3}
来源：http://gle.kuanghao11.cn

Ruby: arr = [1, 2, 3]
来源：http://sfv.haohaochexian.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://jgy.jqgfzy.top

[D02] 追加元素到末尾
来源：http://zer.cheryme.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://diq.svipenyu.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://kpb.wangshuangyany.cn

JS:   arr.push(4);
来源：http://duo.cdnleiting.top

TS:   arr.push(4);
来源：http://coe.yfazqb.com

Java: list.add(4);
来源：http://wvh.hammf.cn

Go:   arr = append(arr, 4)
来源：http://czx.jyoumei.cn

Ruby: arr << 4; arr.push(5)
来源：http://jeh.zdbjq.cn

C#:   list.Add(4);
来源：http://txz.gogol.net.cn

[D03] 在指定位置插入元素
来源：http://zzt.sweek.top

Py:   arr.insert(0, 0)
来源：http://ctf.jyoumei.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://qyo.chenjidiqi.icu

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://nra.quarkkingdee.top

TS:   arr.splice(0, 0, 0);
来源：http://fyl.jinqigfzy.top

Java: list.add(0, 0);
来源：http://qwp.xylfe.cn

Go:   arr = append([]int{0}, arr...)
来源：http://hzt.ivvv.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://vmm.fktsv.cn

C#:   list.Insert(0, 0);
来源：http://ahs.jinqigufen.top

[D04] 删除元素
来源：http://dup.shzxlz.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wbc.hammf.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://cox.daria6918.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://fsz.cucudq.cn

TS:   arr.splice(0, 1);
来源：http://kyw.zdqjudy.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wqd.vqdsnc.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hsg.fzhhl.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ond.aibaodan.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://kha.316326.xyz

[D05] 访问与修改元素
来源：http://rzj.9152youxi.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wsj.yfazqb.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://lgh.cucudq.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://lju.bbcook.cn

TS:   arr[0]; arr.at(-1);
来源：http://pnj.9152youxi.cn

Java: list.get(0); list.set(0, 9);
来源：http://rmx.ehwqpu.com

Go:   arr[0]; arr[0] = 9
来源：http://yue.fktsv.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://akb.sysykeji.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://xdw.xinyue.icu

[D06] 数组长度
来源：http://jrd.ivvv.top

Py:   len(arr)
来源：http://tns.nwbrower.top

PHP:  count($arr);
来源：http://ubb.epnwcf.com

JS:   arr.length
来源：http://bed.hcnkem.com

TS:   arr.length
来源：http://oaz.yueranfly.top

Java: list.size();
来源：http://yeq.shzxlz.cn

Go:   len(arr)
来源：http://wfz.ppjwa.cn

Ruby: arr.length; arr.size
来源：http://fpc.hnqzz.top

C#:   list.Count;
来源：http://umn.52xcode.cn

[D07] 切片 / 取子数组
来源：http://nwp.cqqwz.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://rqy.aibaodan.cn

PHP:  array_slice($arr, 1, 3);
来源：http://tyy.jyoumei.cn

JS:   arr.slice(1, 4);
来源：http://sqv.yueranfly.top

TS:   arr.slice(1, 4);
来源：http://lcc.tanke756.top

Java: list.subList(1, 4);
来源：http://rdu.xingfuxueyuan.xyz

Go:   arr[1:4]
来源：http://acd.xingfuxueyuan.xyz

Ruby: arr[1, 3]
来源：http://mwz.mhx1999.top

C#:   list.GetRange(1, 3);
来源：http://tqf.xziqi.cn

[D08] 合并两个数组
来源：http://rnm.fzhhl.top

Py:   a + b;  a.extend(b)
来源：http://bhh.snrcjt.cn

PHP:  array_merge($a, $b);
来源：http://uch.cashguo.top

JS:   [...a, ...b];  a.concat(b);
来源：http://jls.xingfuxueyuan.xyz

TS:   [...a, ...b];
来源：http://blg.yueranfly.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ejw.gaohongyu789.top

Go:   append(a, b...)
来源：http://lwr.shangyingyoupin.top


<!-- 参考信息 -->