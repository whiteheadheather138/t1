代发 wailian999

Java: do { i++; } while (i < 10);
来源：http://ofo.aibaodan.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://too.xinyue.icu

Ruby: begin; i += 1; end while i < 10
来源：http://sgn.chenlongwang.top

C#:   do { i++; } while (i < 10);
来源：http://jxh.zhaomingkeji.xyz

[B09] break 与 continue
来源：http://kkz.zdbjq.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://qrm.gogol.net.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://bln.yfazqb.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zat.bjfxy.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://txa.havefunace.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ria.guowangkeji.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hdl.ywan-chungtsiang.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://rdb.nanxinkj.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cxt.yj20258.top

[B10] 遍历同时拿索引
来源：http://rfe.feifeiyinyue.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://xiz.jyoumei.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://fwc.shanyushiyangtech.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wyr.pycfn.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://zbc.cdnleiting.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://vjp.quarkkingdee.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://lzd.cucudq.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://odr.ehwqpu.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://tnw.zhixingplan.top

[B11] 生成数字序列 / 区间
来源：http://sgy.zdqjudy.top

Py:   list(range(0, 10, 2))
来源：http://jti.guannengcc.top

PHP:  range(0, 10, 2);
来源：http://ump.chenlongwang.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mas.dianchejie.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://njc.gaohongyu789.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hhw.wangdashe.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://htc.gzhubu.top

Ruby: (0...10).step(2).to_a
来源：http://iqb.chenzaomai.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://buj.c1oappe.top

[B12] 跳出多层循环
来源：http://aek.epnwcf.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://mko.tian-w.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://klx.ehwqpu.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mwb.hammf.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wag.ybcxt.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hhk.chenlongwang.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wkk.yuxming.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mnp.jinqigfzy.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://meh.sufxvd.cn

[B13] 判断是否为数字
来源：http://lga.jyoumei.cn

Py:   isinstance(x, (int, float))
来源：http://xcg.haohaochexian.top

PHP:  is_numeric($x)
来源：http://hbg.ivvv.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://icu.yueranfly.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://iab.yueranfly.top

Java: x instanceof Number
来源：http://iut.yj202588.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://akv.fktsv.cn

Ruby: x.is_a?(Numeric)
来源：http://vqa.uphjek.com

C#:   x is int or double or decimal
来源：http://gpb.xylfe.cn

[B14] 判断值是否在集合内
来源：http://goa.gzhubu.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://krd.xingfuxueyuan.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hsu.hnxiangtu.top

JS:   [1, 2, 3].includes(x)
来源：http://qxt.feifeiyinyue.top

TS:   [1, 2, 3].includes(x)
来源：http://efx.uphjek.com

Java: List.of(1, 2, 3).contains(x)
来源：http://rwy.sweek.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://xam.yj202588.top

Ruby: [1, 2, 3].include?(x)
来源：http://fbp.ivvv.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://sgn.aizwys.cn

[B15] 布尔运算与取反
来源：http://yhs.jinqigfzy.top

Py:   a and b or not c
来源：http://bor.wangdashe.top

PHP:  $a && $b || !$c
来源：http://hwh.zdqjudy.top

JS:   a && b || !c
来源：http://sxj.guannengcc.top

TS:   a && b || !c
来源：http://zxy.iojbl.cn

Java: a && b || !c
来源：http://seo.sufxvd.cn

Go:   a && b || !c
来源：http://cxr.316326.xyz

Ruby: a && b || !c
来源：http://nye.guannengcc.top

C#:   a && b || !c
来源：http://ucc.ivvv.top

[B16] 卫语句：不满足条件提前返回
来源：http://npp.fktsv.cn

Py:   if not data: return
来源：http://uja.9152youxi.cn

PHP:  if (!$data) { return; }
来源：http://gtv.sufxvd.cn

JS:   if (!data) return;
来源：http://pry.xuetiantiany.cn

TS:   if (!data) return;
来源：http://mkm.daxiang520.top

Java: if (data == null) return;
来源：http://kfz.meibo888.top

Go:   if data == nil { return }
来源：http://dyo.tarul.cn

Ruby: return if data.nil?
来源：http://apz.cashguo.top

C#:   if (data == null) return;
来源：http://pcs.xingfuxueyuan.xyz

================================================================================
来源：http://zgm.yueranfly.top

C. 函数与作用域
来源：http://lwp.ehwqpu.com

================================================================================
来源：http://hcj.yonumen.top

[C01] 定义函数
来源：http://mdp.hfpthk.cn

Py:   def add(a, b): return a + b
来源：http://rdi.zycfv.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tob.yj20258.top

JS:   function add(a, b) { return a + b; }
来源：http://lmc.chenjidiqi.icu

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hql.guowangkeji.top

Java: static int add(int a, int b) { return a + b; }
来源：http://hxi.9152youxi.cn

Go:   func add(a, b int) int { return a + b }
来源：http://arz.yfazqb.com

Ruby: def add(a, b); a + b; end
来源：http://wjh.shanyushiyangtech.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://cqg.yj20258888.top

[C02] 默认参数
来源：http://qsd.xinyue.icu

Py:   def greet(name="World"): return name
来源：http://zsv.cqqwz.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://vmo.uphjek.com

JS:   function greet(name = "World") { return name; }
来源：http://laq.xuetiantiany.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://uci.fehbvm.com

Java: // 无默认参数：方法重载或 Optional
来源：http://bjj.nanxinkj.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mon.cheryme.top

Ruby: def greet(name = "World") = name
来源：http://nsq.zhengqikj.top

C#:   string Greet(string name = "World") => name;
来源：http://rzw.ybcxt.top

[C03] 可变参数
来源：http://rkv.jyoumei.cn

Py:   def total(*args): return sum(args)
来源：http://cbw.nwbrower.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ime.52xcode.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mqq.fktsv.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://zuf.yueranfly.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://gtg.52xcode.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://fkh.xingfuxueyuan.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://ttx.jiagoushi.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://byy.sysykeji.top

[C04] 命名参数 / 关键字参数
来源：http://rjq.hcnkem.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://yed.yj20258888.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://nyh.havefunace.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mzh.tianlin.xyz

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://kzh.yj20258888.top

Java: // 无：用 Builder 模式或 record
来源：http://ylz.aizwys.cn

Go:   // 无：用配置结构体参数
来源：http://thm.zhijiandao.cn

Ruby: f(a: 1, b: 2)
来源：http://lgt.zycfv.cn

C#:   f(a: 1, b: 2)
来源：http://ivj.svipenyu.cn

[C05] 返回多个值
来源：http://hur.xylfe.cn

Py:   return a, b
来源：http://mgv.ehwqpu.com

PHP:  return [$a, $b];
来源：http://joo.havefunace.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://qgk.epnwcf.com

TS:   return { a, b };
来源：http://dja.guowangkeji.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://tjk.fengsongda.top

Go:   return a, b
来源：http://akr.chenlongwang.top

Ruby: return a, b
来源：http://orr.gaohongyu789.top

C#:   return (a, b);              // ValueTuple
来源：http://mmi.pycfn.com

[C06] 匿名函数 / lambda
来源：http://gon.cucudq.cn

Py:   square = lambda x: x * x
来源：http://nyb.guannengcc.top

PHP:  $square = fn($x) => $x * $x;
来源：http://mnf.iojbl.cn

JS:   const square = x => x * x;
来源：http://oqd.shanyushiyangkeji.top

TS:   const square = (x: number): number => x * x;
来源：http://aju.shzxlz.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://jnp.meibo888.top

Go:   sq := func(x int) int { return x * x }
来源：http://nmu.sjlbkw.cn

Ruby: square = ->(x) { x * x }
来源：http://erc.yangfankeji.com

C#:   Func<int, int> square = x => x * x;
来源：http://jrm.zhoulong.xyz

[C07] 把函数作为参数传入
来源：http://huk.yj20258888.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://jhl.zhengqikj.top

PHP:  array_map("strtoupper", $arr);
来源：http://btj.feifeiyinyue.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ejf.pengpengdd.cyou

TS:   arr.map(String)
来源：http://rcl.zdqjudy.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://vdv.9152youxi.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ozs.zhengqikj.top

Ruby: arr.map(&:upcase)
来源：http://urn.fehbvm.com

C#:   arr.Select(s => s.ToUpper())
来源：http://iko.aizwys.cn

[C08] 闭包
来源：http://hgm.ehwqpu.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ttd.xziqi.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://qnl.sxryk.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ugl.bbcook.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://jca.havefunace.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hby.smart0.xyz

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ynz.hnqzz.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://igd.zhijiandao.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://bqz.hongshengwenyu.top

[C09] 递归
来源：http://dby.jqgfzy.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://tsq.redwolf501.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://vqo.yfazqb.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yef.yueranfly.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://aji.gotoacloud.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://lqn.hnxiangtu.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://oqz.bjfxy.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://oci.hysaishi.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://alr.ivvv.top

[C10] 变量作用域
来源：http://wgg.shanyushiyangkeji.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://nbi.cheryme.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://gls.yuxming.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ymy.gotoacloud.top

TS:   同 JS
来源：http://xhy.guannengcc.top

Java: 方法内为块级作用域
来源：http://bub.chenjidiqi.icu

Go:   花括号块级作用域
来源：http://qzj.zhiwuduotai.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hzk.jiagoushi.top

C#:   块级作用域
来源：http://uje.fktsv.cn

[C11] 模块导入与导出
来源：http://int.ydjk.org.cn

Py:   from module import func
来源：http://fcc.daria6918.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://wyb.dashuyun.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://kfj.yonumen.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mzm.yfazqb.com

Java: import java.util.List;
来源：http://dkr.fanxiaobao.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://owy.jqgfzy.top

Ruby: require "json"; require_relative "./util"
来源：http://rer.fehbvm.com

C#:   using System.Text;
来源：http://hwm.zycfv.cn

[C12] 立即执行函数 IIFE
来源：http://qdl.guannengcc.top

Py:   (lambda: print("run"))()
来源：http://xhk.svipenyu.cn

PHP:  (function () { echo "run"; })();
来源：http://bhl.yuxming.cn

JS:   (() => { console.log("run"); })();
来源：http://rhi.zycfv.cn

TS:   (() => { console.log("run"); })();
来源：http://mzd.fanxiaobao.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://dsu.sweek.top

Go:   func() { fmt.Println("run") }()
来源：http://pav.feifeiyinyue.top

Ruby: -> { puts "run" }.call
来源：http://yrd.9152youxi.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://xel.jlsjyb.cn

[C13] 类型声明 / 类型注解
来源：http://tby.yanxiufei.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://zlw.sweek.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lys.pengpengdd.cyou

JS:   // 无类型（可用 JSDoc 注释）
来源：http://rys.daxiang520.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dod.ywan-chungtsiang.top

Java: int add(int a, int b) { return a + b; }
来源：http://lvj.smart0.xyz

Go:   func add(a, b int) int
来源：http://jeh.bjfxy.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://qxy.shuidangran.top

C#:   int Add(int a, int b) => a + b;
来源：http://nou.quarkkingdee.top

[C14] 泛型函数
来源：http://jka.xuanzx.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://lbk.ydjk.org.cn

PHP:  // 无泛型
来源：http://vwd.zdqjudy.top

JS:   // 无泛型
来源：http://wlz.havefunace.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://seu.shanyushiyangkeji.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://tur.quarkkingdee.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ytv.uphjek.com

Ruby: # 无泛型
来源：http://pek.shangyingyoupin.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://zod.tarul.cn

[C15] 解构 / 展开参数
来源：http://iaa.ivvv.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://pdy.pengpengdd.cyou

PHP:  [$a, $b] = $pair;
来源：http://czs.bbcook.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://tgp.shuidangran.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://diw.jiagoushi.top

Java: // 无解构
来源：http://fvg.redwolf501.top

Go:   // 无解构
来源：http://sut.sjlbkw.cn

Ruby: a, b = pair
来源：http://kfv.yvedp.cn

C#:   var (a, b) = pair;
来源：http://thr.sufxvd.cn

[C16] 函数 / 方法重载
来源：http://xfg.fktsv.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://qfg.jyoumei.cn

PHP:  // 无重载
来源：http://vlf.ybcxt.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://pyl.fzhhl.top

TS:   // 用联合类型或重载签名声明
来源：http://xpr.tianlin.xyz

Java: void f(int a) {}  void f(String a) {}
来源：http://vem.gogol.net.cn

Go:   // 无重载：用不同函数名
来源：http://vxy.zycfv.cn

Ruby: # 无重载：靠动态参数
来源：http://vfb.zhijiandao.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://nfb.sweek.top

================================================================================
来源：http://kqj.tarul.cn

D. 数组 / 列表 / 集合
来源：http://kdv.cashguo.top

================================================================================
来源：http://vyt.zhongyouzk.top

[D01] 创建数组 / 列表
来源：http://tjy.9152youxi.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://cke.tarul.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://erd.xinyue.icu

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://cfs.vqdsnc.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://vtr.jlsjyb.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ppa.tian-w.cn

Go:   arr := []int{1, 2, 3}
来源：http://ifz.jyoumei.cn

Ruby: arr = [1, 2, 3]
来源：http://gtz.dashuyun.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://nca.gotoacloud.top

[D02] 追加元素到末尾
来源：http://mxn.jinghuilouyu.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://leb.wangdashe.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://gon.ivvv.top

JS:   arr.push(4);
来源：http://ida.hywenlv.cn

TS:   arr.push(4);
来源：http://tpv.yj202588.top

Java: list.add(4);
来源：http://gxb.shzxlz.cn

Go:   arr = append(arr, 4)
来源：http://ecd.shzxlz.cn

Ruby: arr << 4; arr.push(5)
来源：http://yrk.tarul.cn

C#:   list.Add(4);
来源：http://tdb.sxryk.cn

[D03] 在指定位置插入元素
来源：http://teh.meibo888.top

Py:   arr.insert(0, 0)
来源：http://kex.haohaochexian.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://bot.hfpthk.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ipx.ctjpmb.com

TS:   arr.splice(0, 0, 0);
来源：http://mru.nanxuanxn.top

Java: list.add(0, 0);
来源：http://pxx.haohaochexian.top

Go:   arr = append([]int{0}, arr...)
来源：http://ccu.vehdjk.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ibs.haohaochexian.top

C#:   list.Insert(0, 0);
来源：http://oxx.vqdsnc.cn

[D04] 删除元素
来源：http://dsg.ppjwa.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://kbo.wangshuangyany.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://nnn.wangshuangyany.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://usy.hcnkem.com

TS:   arr.splice(0, 1);
来源：http://vtp.yj20258.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://pyt.vehdjk.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://kjf.cashguo.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://rwn.gogol.net.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://yyv.chenzaomai.com

[D05] 访问与修改元素
来源：http://kew.wangdashe.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mti.316326.xyz

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://jrx.sysykeji.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://gpw.shanyushiyangkeji.top

TS:   arr[0]; arr.at(-1);
来源：http://sdz.fengsongda.top

Java: list.get(0); list.set(0, 9);
来源：http://myg.nanxinkj.top

Go:   arr[0]; arr[0] = 9
来源：http://uni.yj20258888.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://nnj.hesvh.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://jpf.iojbl.cn

[D06] 数组长度
来源：http://smi.iojbl.cn

Py:   len(arr)
来源：http://dej.aibaodan.cn

PHP:  count($arr);
来源：http://rut.xziqi.cn

JS:   arr.length
来源：http://uns.nanxuanxn.top

TS:   arr.length
来源：http://yey.jlsjyb.cn

Java: list.size();
来源：http://bhb.xziqi.cn

Go:   len(arr)
来源：http://luj.wangshuangyany.cn

Ruby: arr.length; arr.size
来源：http://eea.yonumen.top

C#:   list.Count;
来源：http://qnb.zhiwuduotai.top

[D07] 切片 / 取子数组
来源：http://cyy.zhixingplan.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://urq.hnxiangtu.top

PHP:  array_slice($arr, 1, 3);
来源：http://euw.guannengcc.top

JS:   arr.slice(1, 4);
来源：http://kqn.pycfn.com

TS:   arr.slice(1, 4);
来源：http://yqt.bbcook.cn

Java: list.subList(1, 4);
来源：http://scf.sufxvd.cn

Go:   arr[1:4]
来源：http://zjr.wangshuangyany.cn

Ruby: arr[1, 3]
来源：http://seu.feifeiyinyue.top

C#:   list.GetRange(1, 3);
来源：http://wnw.wangshuangyany.cn

[D08] 合并两个数组
来源：http://zyt.gogol.net.cn

Py:   a + b;  a.extend(b)
来源：http://ayn.wangshuangyany.cn

PHP:  array_merge($a, $b);
来源：http://ajc.fengsongda.top

JS:   [...a, ...b];  a.concat(b);
来源：http://ged.nanxuanxn.top

TS:   [...a, ...b];
来源：http://crm.sweek.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://zqh.smart0.xyz

Go:   append(a, b...)
来源：http://zkr.jinqigufen.top

Ruby: a + b;  a.concat(b)
来源：http://pxu.hfpthk.cn

C#:   a.Concat(b).ToList()
来源：http://aob.shzxlz.cn

[D09] 排序（升序）
来源：http://udu.yongpay.top

Py:   sorted(arr);  arr.sort()
来源：http://oub.zhengqikj.top


<!-- 参考信息 -->