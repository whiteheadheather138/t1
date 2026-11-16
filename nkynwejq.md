代发 wailian999

Java: do { i++; } while (i < 10);
来源：http://cvb.aizwys.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://wkk.daria6918.cn

Ruby: begin; i += 1; end while i < 10
来源：http://vhm.pycfn.com

C#:   do { i++; } while (i < 10);
来源：http://qcy.zhixingplan.top

[B09] break 与 continue
来源：http://afl.hywenlv.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://aid.sufxvd.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://uxb.pycfn.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://olp.vqdsnc.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bfe.hnxiangtu.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pbd.redwolf501.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ksp.haohaochexian.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ptx.guannengcc.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://coq.smart0.xyz

[B10] 遍历同时拿索引
来源：http://rkd.hammf.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://gox.dashuyun.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://yhi.xziqi.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://gil.cashguo.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://bre.uphjek.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hwz.wangshuangyany.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://nsv.zhaomingkeji.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ojn.ywan-chungtsiang.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://dml.yuanzhike.top

[B11] 生成数字序列 / 区间
来源：http://ijt.yueranfly.top

Py:   list(range(0, 10, 2))
来源：http://bsa.yj20258.top

PHP:  range(0, 10, 2);
来源：http://jnt.xingfuxueyuan.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bry.haohaochexian.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://uml.xuanzx.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://das.shanyushiyangkeji.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ybx.jiagoushi.top

Ruby: (0...10).step(2).to_a
来源：http://zli.cqqwz.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://yho.jyoumei.cn

[B12] 跳出多层循环
来源：http://kvn.cqqwz.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://cqm.xingfuxueyuan.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://zfe.zdqjudy.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://lyq.andypj.xyz

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://gof.tianlin.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://stb.jiagoushi.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://lfd.cucudq.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ajr.zdbjq.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://kpc.vehdjk.com

[B13] 判断是否为数字
来源：http://lwt.aizwys.cn

Py:   isinstance(x, (int, float))
来源：http://sbx.bbcook.cn

PHP:  is_numeric($x)
来源：http://wik.tian-w.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yju.zhijiandao.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xdk.ywan-chungtsiang.top

Java: x instanceof Number
来源：http://tlx.zhaomingkeji.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ifh.cucudq.cn

Ruby: x.is_a?(Numeric)
来源：http://xbe.fzhhl.top

C#:   x is int or double or decimal
来源：http://kek.shangyingyoupin.top

[B14] 判断值是否在集合内
来源：http://oci.ehwqpu.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://amt.sjlbkw.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://plx.yonumen.top

JS:   [1, 2, 3].includes(x)
来源：http://bwx.zhongyouzk.top

TS:   [1, 2, 3].includes(x)
来源：http://tuq.meibo888.top

Java: List.of(1, 2, 3).contains(x)
来源：http://nak.jyoumei.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://tue.sjlbkw.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ivb.jinqigfzy.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://lju.wangshuangyany.cn

[B15] 布尔运算与取反
来源：http://sxq.yanxiufei.cn

Py:   a and b or not c
来源：http://vbm.hammf.cn

PHP:  $a && $b || !$c
来源：http://vov.shanyushiyangkeji.top

JS:   a && b || !c
来源：http://sle.iojbl.cn

TS:   a && b || !c
来源：http://gcf.zhiwuduotai.top

Java: a && b || !c
来源：http://rlo.shangyingyoupin.top

Go:   a && b || !c
来源：http://arb.ydzc1.top

Ruby: a && b || !c
来源：http://hgo.yanxiufei.cn

C#:   a && b || !c
来源：http://fiu.zhijiandao.cn

[B16] 卫语句：不满足条件提前返回
来源：http://mja.haohaochexian.top

Py:   if not data: return
来源：http://eze.snrcjt.cn

PHP:  if (!$data) { return; }
来源：http://bnf.bbcook.cn

JS:   if (!data) return;
来源：http://ppk.daria6918.cn

TS:   if (!data) return;
来源：http://lbn.yueranfly.top

Java: if (data == null) return;
来源：http://sir.sysykeji.top

Go:   if data == nil { return }
来源：http://nxh.zhengqikj.top

Ruby: return if data.nil?
来源：http://crc.jinyuanbaomall.cn

C#:   if (data == null) return;
来源：http://fxf.hysaishi.cn

================================================================================
来源：http://xjy.cqqwz.cn

C. 函数与作用域
来源：http://ulh.jqgfzy.top

================================================================================
来源：http://omo.fzhhl.top

[C01] 定义函数
来源：http://lii.jianghu66.top

Py:   def add(a, b): return a + b
来源：http://smx.yongpay.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lxu.zhixingplan.top

JS:   function add(a, b) { return a + b; }
来源：http://krz.jiagoushi.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qwr.yj20258888.top

Java: static int add(int a, int b) { return a + b; }
来源：http://ext.hongshengwenyu.top

Go:   func add(a, b int) int { return a + b }
来源：http://ixr.dashuyun.cn

Ruby: def add(a, b); a + b; end
来源：http://fdy.ivvv.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://bup.ctjpmb.com

[C02] 默认参数
来源：http://set.gotoacloud.top

Py:   def greet(name="World"): return name
来源：http://lba.nanxuanxn.top

PHP:  function greet($name = "World") { return $name; }
来源：http://jzl.guannengcc.top

JS:   function greet(name = "World") { return name; }
来源：http://pfp.chenzaomai.com

TS:   function greet(name: string = "World") { return name; }
来源：http://bba.hcnkem.com

Java: // 无默认参数：方法重载或 Optional
来源：http://qjq.daxiang520.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://pml.shanyushiyangkeji.top

Ruby: def greet(name = "World") = name
来源：http://zpw.guowangkeji.top

C#:   string Greet(string name = "World") => name;
来源：http://jjb.jianghu66.top

[C03] 可变参数
来源：http://wlf.haohaochexian.top

Py:   def total(*args): return sum(args)
来源：http://wuv.sxryk.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://vnh.daria6918.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ndz.hesvh.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://rzk.shuidangran.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://iwh.yj202588.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://fss.tanke756.top

Ruby: def total(*nums); nums.sum; end
来源：http://utg.ydzc1.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://nis.cheryme.top

[C04] 命名参数 / 关键字参数
来源：http://amw.tianlin.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://xmd.jinqigufen.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://pon.jinqigfzy.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ddp.yueranfly.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://zbc.zhengqikj.top

Java: // 无：用 Builder 模式或 record
来源：http://bhh.quarkkingdee.top

Go:   // 无：用配置结构体参数
来源：http://yyx.0kj1m.cn

Ruby: f(a: 1, b: 2)
来源：http://myc.yangfankeji.com

C#:   f(a: 1, b: 2)
来源：http://lbf.shzxlz.cn

[C05] 返回多个值
来源：http://ihu.cashguo.top

Py:   return a, b
来源：http://toa.sysykeji.top

PHP:  return [$a, $b];
来源：http://myq.xziqi.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://izf.yj202588.top

TS:   return { a, b };
来源：http://flt.tarul.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ogh.c1oappe.top

Go:   return a, b
来源：http://mir.sufxvd.cn

Ruby: return a, b
来源：http://akk.hysaishi.cn

C#:   return (a, b);              // ValueTuple
来源：http://mof.ivvv.top

[C06] 匿名函数 / lambda
来源：http://hcy.jqgufenzy.top

Py:   square = lambda x: x * x
来源：http://rpo.nanxuanxn.top

PHP:  $square = fn($x) => $x * $x;
来源：http://fnj.fzhhl.top

JS:   const square = x => x * x;
来源：http://jrb.jinqigfzy.top

TS:   const square = (x: number): number => x * x;
来源：http://mov.shuidangran.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://euk.cheryme.top

Go:   sq := func(x int) int { return x * x }
来源：http://egm.sjlbkw.cn

Ruby: square = ->(x) { x * x }
来源：http://wgh.gogol.net.cn

C#:   Func<int, int> square = x => x * x;
来源：http://xvf.bbcook.cn

[C07] 把函数作为参数传入
来源：http://lxi.316326.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ukb.shzxlz.cn

PHP:  array_map("strtoupper", $arr);
来源：http://hzx.gogol.net.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://fku.cucudq.cn

TS:   arr.map(String)
来源：http://ksn.xylfe.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://kdw.svipenyu.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://lfx.hnxiangtu.top

Ruby: arr.map(&:upcase)
来源：http://kmk.jianghu66.top

C#:   arr.Select(s => s.ToUpper())
来源：http://sdg.shzxlz.cn

[C08] 闭包
来源：http://edu.shangyingyoupin.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ktr.cheryme.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://big.jlsjyb.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vwp.tanke756.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://loc.ydjk.org.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://gak.wangdashe.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mtm.zhaomingkeji.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://qam.pycfn.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://abl.yuanzhike.top

[C09] 递归
来源：http://qak.aizwys.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://nkl.chenzaomai.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://afy.ivvv.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kgf.ydzc1.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rkb.yj20258888.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://cgp.ybcxt.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://upa.yj202588.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://yft.pengpengdd.cyou

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://jlx.yuanzhike.top

[C10] 变量作用域
来源：http://oai.svipenyu.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://pht.shangyingyoupin.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ekt.daxiang520.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://kyn.aizwys.cn

TS:   同 JS
来源：http://dxy.ydzc1.top

Java: 方法内为块级作用域
来源：http://yoy.yj20258.top

Go:   花括号块级作用域
来源：http://yyl.pengpengdd.cyou

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mtn.yuanzhike.top

C#:   块级作用域
来源：http://pxk.shanyushiyangkeji.top

[C11] 模块导入与导出
来源：http://tee.hysaishi.cn

Py:   from module import func
来源：http://hgy.ivvv.top

PHP:  require "file.php";  或 use App\Service;
来源：http://oig.daxiang520.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://oca.gzhubu.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://jhr.shanyushiyangtech.top

Java: import java.util.List;
来源：http://lvg.birdmap.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://lqy.gaohongyu789.top

Ruby: require "json"; require_relative "./util"
来源：http://brj.meibo888.top

C#:   using System.Text;
来源：http://iyp.jinqigufen.top

[C12] 立即执行函数 IIFE
来源：http://gdb.epnwcf.com

Py:   (lambda: print("run"))()
来源：http://gxm.zhaomingkeji.xyz

PHP:  (function () { echo "run"; })();
来源：http://bew.cheryme.top

JS:   (() => { console.log("run"); })();
来源：http://vjx.quarkkingdee.top

TS:   (() => { console.log("run"); })();
来源：http://jsx.yj20258.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hxv.dianchejie.cn

Go:   func() { fmt.Println("run") }()
来源：http://xpr.yuxming.cn

Ruby: -> { puts "run" }.call
来源：http://sps.tarul.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://xdr.ydzc1.top

[C13] 类型声明 / 类型注解
来源：http://ood.ydzc1.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://cgf.ehwqpu.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://txd.birdmap.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://alx.jlsjyb.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jct.yonumen.top

Java: int add(int a, int b) { return a + b; }
来源：http://iag.jqgufenzy.top

Go:   func add(a, b int) int
来源：http://psp.havefunace.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mqa.pengpengdd.cyou

C#:   int Add(int a, int b) => a + b;
来源：http://mvd.hnxiangtu.top

[C14] 泛型函数
来源：http://xdy.c1oappe.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zrv.yfazqb.com

PHP:  // 无泛型
来源：http://cbs.tian-w.cn

JS:   // 无泛型
来源：http://nkn.pengpengdd.cyou

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://udp.gogol.net.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://fkp.zhengqikj.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://zuc.chenzaomai.com

Ruby: # 无泛型
来源：http://chz.dianchejie.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://kdq.9152youxi.cn

[C15] 解构 / 展开参数
来源：http://zuj.jinyuanbaomall.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hmf.sysykeji.top

PHP:  [$a, $b] = $pair;
来源：http://ala.tian-w.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://onb.sufxvd.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://vvc.ydjk.org.cn

Java: // 无解构
来源：http://trv.fanxiaobao.xyz

Go:   // 无解构
来源：http://dqa.ydzc1.top

Ruby: a, b = pair
来源：http://rdr.iojbl.cn

C#:   var (a, b) = pair;
来源：http://fhj.ybcxt.top

[C16] 函数 / 方法重载
来源：http://tiq.sysykeji.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://cym.sweek.top

PHP:  // 无重载
来源：http://jjf.zhongyouzk.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://jnv.nwbrower.top

TS:   // 用联合类型或重载签名声明
来源：http://xok.svipenyu.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://eer.0kj1m.cn

Go:   // 无重载：用不同函数名
来源：http://djm.fktsv.cn

Ruby: # 无重载：靠动态参数
来源：http://uxt.ybcxt.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://xtp.zhoulong.xyz

================================================================================
来源：http://tjk.jianghu66.top

D. 数组 / 列表 / 集合
来源：http://sqk.daxiang520.top

================================================================================
来源：http://mdo.svipenyu.cn

[D01] 创建数组 / 列表
来源：http://ezt.sweek.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://alx.snrcjt.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://his.hywenlv.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://gaa.fehbvm.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://oqj.daxiang520.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://cuq.iojbl.cn

Go:   arr := []int{1, 2, 3}
来源：http://olb.meibo888.top

Ruby: arr = [1, 2, 3]
来源：http://nmo.jinqigufen.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://nsq.ybcxt.top

[D02] 追加元素到末尾
来源：http://ifi.redwolf501.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mwi.nanxuanxn.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://kun.jqgfzy.top

JS:   arr.push(4);
来源：http://pjx.yj20258.top

TS:   arr.push(4);
来源：http://sae.ctjpmb.com

Java: list.add(4);
来源：http://sfw.hysaishi.cn

Go:   arr = append(arr, 4)
来源：http://fhe.haohaochexian.top

Ruby: arr << 4; arr.push(5)
来源：http://zpp.smart0.xyz

C#:   list.Add(4);
来源：http://etq.chenzaomai.com

[D03] 在指定位置插入元素
来源：http://hkr.chenzaomai.com

Py:   arr.insert(0, 0)
来源：http://ipn.jqgufenzy.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wsy.meibo888.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://eex.gogol.net.cn

TS:   arr.splice(0, 0, 0);
来源：http://ebl.vehdjk.com

Java: list.add(0, 0);
来源：http://jlw.smart0.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://wtj.yj20258.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://uub.guannengcc.top

C#:   list.Insert(0, 0);
来源：http://oyi.hfpthk.cn

[D04] 删除元素
来源：http://erq.aizwys.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://bil.cdnleiting.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://tvk.guannengcc.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xop.ydjk.org.cn

TS:   arr.splice(0, 1);
来源：http://sla.fzhhl.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ssj.andypj.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://vqy.svipenyu.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hto.yanxiufei.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://uuf.zycfv.cn

[D05] 访问与修改元素
来源：http://phj.tanke756.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://yda.yongpay.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://atu.ydjk.org.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://bps.ehwqpu.com

TS:   arr[0]; arr.at(-1);
来源：http://cqg.ydjk.org.cn

Java: list.get(0); list.set(0, 9);
来源：http://phe.cashguo.top

Go:   arr[0]; arr[0] = 9
来源：http://dzi.xuetiantiany.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://fzk.jinghuilouyu.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://uyi.xinyue.icu

[D06] 数组长度
来源：http://kio.svipenyu.cn

Py:   len(arr)
来源：http://sdv.hywenlv.cn

PHP:  count($arr);
来源：http://fur.zhoulong.xyz

JS:   arr.length
来源：http://ruy.xziqi.cn

TS:   arr.length
来源：http://smc.sufxvd.cn

Java: list.size();
来源：http://olo.hongshengwenyu.top

Go:   len(arr)
来源：http://agy.dashuyun.cn

Ruby: arr.length; arr.size
来源：http://uzu.sufxvd.cn

C#:   list.Count;
来源：http://cao.jinghuilouyu.cn

[D07] 切片 / 取子数组
来源：http://erz.yonumen.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ywf.fengsongda.top

PHP:  array_slice($arr, 1, 3);
来源：http://kee.yj20258.top

JS:   arr.slice(1, 4);
来源：http://ixr.zhixingplan.top

TS:   arr.slice(1, 4);
来源：http://wsh.chenzaomai.com

Java: list.subList(1, 4);
来源：http://wwt.wangshuangyany.cn

Go:   arr[1:4]
来源：http://qzd.xziqi.cn

Ruby: arr[1, 3]
来源：http://uao.ydjk.org.cn

C#:   list.GetRange(1, 3);
来源：http://qwb.yvedp.cn

[D08] 合并两个数组
来源：http://ysy.cashguo.top

Py:   a + b;  a.extend(b)
来源：http://rvo.gogol.net.cn

PHP:  array_merge($a, $b);
来源：http://jls.fanxiaobao.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://egw.aibaodan.cn

TS:   [...a, ...b];
来源：http://wwm.xinyue.icu

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://jxh.cqqwz.cn

Go:   append(a, b...)
来源：http://gzs.cqqwz.cn

Ruby: a + b;  a.concat(b)
来源：http://ift.zdbjq.cn

C#:   a.Concat(b).ToList()
来源：http://bpj.pengpengdd.cyou

[D09] 排序（升序）
来源：http://brg.daria6918.cn

Py:   sorted(arr);  arr.sort()
来源：http://bqt.yueranfly.top


<!-- 参考信息 -->