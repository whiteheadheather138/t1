代发 wailian999

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://boc.zdqjudy.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lpd.gogol.net.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://aos.nanxinkj.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://iaj.9152youxi.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lxq.jqgufenzy.top

[B10] 遍历同时拿索引
来源：http://siv.yuxming.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ozb.cqqwz.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://llg.fengsongda.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://raa.svipenyu.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ghs.yonumen.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mqr.hysaishi.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://lyw.feifeiyinyue.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://nky.zhaomingkeji.xyz

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://reo.jqgufenzy.top

[B11] 生成数字序列 / 区间
来源：http://bac.quarkkingdee.top

Py:   list(range(0, 10, 2))
来源：http://rcr.ywan-chungtsiang.top

PHP:  range(0, 10, 2);
来源：http://gli.xylfe.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bsn.sysykeji.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mmv.yuxming.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://zqy.52xcode.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://cwk.hongshengwenyu.top

Ruby: (0...10).step(2).to_a
来源：http://zii.vqdsnc.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://vvf.zhijiandao.cn

[B12] 跳出多层循环
来源：http://vog.jqgfzy.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://fuq.xingfuxueyuan.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://zga.fengsongda.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://csc.sjlbkw.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://zhy.yonumen.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://dze.sxryk.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://bop.cheryme.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://lmj.sufxvd.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://qys.52xcode.cn

[B13] 判断是否为数字
来源：http://auk.cashguo.top

Py:   isinstance(x, (int, float))
来源：http://lyv.hesvh.cn

PHP:  is_numeric($x)
来源：http://vvs.epnwcf.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tue.birdmap.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rwq.xingfuxueyuan.xyz

Java: x instanceof Number
来源：http://vtk.xinyue.icu

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ssa.chenzaomai.com

Ruby: x.is_a?(Numeric)
来源：http://kjq.jinqigufen.top

C#:   x is int or double or decimal
来源：http://qrp.hnqzz.top

[B14] 判断值是否在集合内
来源：http://jqk.cashguo.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://kfh.cheryme.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ves.guowangkeji.top

JS:   [1, 2, 3].includes(x)
来源：http://vyg.quarkkingdee.top

TS:   [1, 2, 3].includes(x)
来源：http://bwb.pycfn.com

Java: List.of(1, 2, 3).contains(x)
来源：http://yhz.yangfankeji.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://vjp.xuanzx.com

Ruby: [1, 2, 3].include?(x)
来源：http://afp.shuidangran.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://zof.guannengcc.top

[B15] 布尔运算与取反
来源：http://dul.nanxinkj.top

Py:   a and b or not c
来源：http://skl.xylfe.cn

PHP:  $a && $b || !$c
来源：http://nlk.zhaomingkeji.xyz

JS:   a && b || !c
来源：http://yzn.tarul.cn

TS:   a && b || !c
来源：http://clp.jqgufenzy.top

Java: a && b || !c
来源：http://jvy.yuanzhike.top

Go:   a && b || !c
来源：http://zpi.ywan-chungtsiang.top

Ruby: a && b || !c
来源：http://sul.zdbjq.cn

C#:   a && b || !c
来源：http://wtb.epnwcf.com

[B16] 卫语句：不满足条件提前返回
来源：http://mlr.zhoulong.xyz

Py:   if not data: return
来源：http://vyk.shanyushiyangkeji.top

PHP:  if (!$data) { return; }
来源：http://vge.ivvv.top

JS:   if (!data) return;
来源：http://laf.yfazqb.com

TS:   if (!data) return;
来源：http://nwg.svipenyu.cn

Java: if (data == null) return;
来源：http://iei.jianghu66.top

Go:   if data == nil { return }
来源：http://qks.nanxinkj.top

Ruby: return if data.nil?
来源：http://nhx.tian-w.cn

C#:   if (data == null) return;
来源：http://byz.chenlongwang.top

================================================================================
来源：http://ygg.ydzc1.top

C. 函数与作用域
来源：http://ggl.yj202588.top

================================================================================
来源：http://vkw.sjlbkw.cn

[C01] 定义函数
来源：http://vae.jlsjyb.cn

Py:   def add(a, b): return a + b
来源：http://kco.xuetiantiany.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xhc.fengsongda.top

JS:   function add(a, b) { return a + b; }
来源：http://poa.fzhhl.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fto.fengsongda.top

Java: static int add(int a, int b) { return a + b; }
来源：http://sba.tian-w.cn

Go:   func add(a, b int) int { return a + b }
来源：http://cdx.feifeiyinyue.top

Ruby: def add(a, b); a + b; end
来源：http://yfx.zhixingplan.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://olb.hysaishi.cn

[C02] 默认参数
来源：http://bgq.xingfuxueyuan.xyz

Py:   def greet(name="World"): return name
来源：http://icz.jianghu66.top

PHP:  function greet($name = "World") { return $name; }
来源：http://skl.yuxming.cn

JS:   function greet(name = "World") { return name; }
来源：http://xqy.pengpengdd.cyou

TS:   function greet(name: string = "World") { return name; }
来源：http://vay.tianlin.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://njn.wangdashe.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ueb.gogol.net.cn

Ruby: def greet(name = "World") = name
来源：http://cdf.hcnkem.com

C#:   string Greet(string name = "World") => name;
来源：http://pri.fzhhl.top

[C03] 可变参数
来源：http://ppn.tianlin.xyz

Py:   def total(*args): return sum(args)
来源：http://eyz.tianlin.xyz

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://pnq.haohaochexian.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ujp.gotoacloud.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://jyj.daxiang520.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mhw.yueranfly.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://fcg.shzxlz.cn

Ruby: def total(*nums); nums.sum; end
来源：http://nch.zhengqikj.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://uzy.hesvh.cn

[C04] 命名参数 / 关键字参数
来源：http://vkj.cdnleiting.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://fyt.guowangkeji.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://zyu.ehwqpu.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mwd.mhx1999.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mgz.xingfuxueyuan.xyz

Java: // 无：用 Builder 模式或 record
来源：http://spo.iojbl.cn

Go:   // 无：用配置结构体参数
来源：http://jml.ywan-chungtsiang.top

Ruby: f(a: 1, b: 2)
来源：http://snr.zhixingplan.top

C#:   f(a: 1, b: 2)
来源：http://cmb.ctjpmb.com

[C05] 返回多个值
来源：http://seh.yongpay.top

Py:   return a, b
来源：http://ftr.bbcook.cn

PHP:  return [$a, $b];
来源：http://eaj.hcnkem.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://sam.sysykeji.top

TS:   return { a, b };
来源：http://cde.zhixingplan.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://lww.hnqzz.top

Go:   return a, b
来源：http://mlt.xuanzx.com

Ruby: return a, b
来源：http://vsb.redwolf501.top

C#:   return (a, b);              // ValueTuple
来源：http://iio.pengpengdd.cyou

[C06] 匿名函数 / lambda
来源：http://zmp.epnwcf.com

Py:   square = lambda x: x * x
来源：http://atv.yj202588.top

PHP:  $square = fn($x) => $x * $x;
来源：http://pdz.tarul.cn

JS:   const square = x => x * x;
来源：http://vvq.jiagoushi.top

TS:   const square = (x: number): number => x * x;
来源：http://jms.9152youxi.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://gws.quarkkingdee.top

Go:   sq := func(x int) int { return x * x }
来源：http://qlu.shangyingyoupin.top

Ruby: square = ->(x) { x * x }
来源：http://lvk.sxryk.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ohm.52xcode.cn

[C07] 把函数作为参数传入
来源：http://ywr.jlsjyb.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://uoc.nanxinkj.top

PHP:  array_map("strtoupper", $arr);
来源：http://bjl.chenjidiqi.icu

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://cyk.meibo888.top

TS:   arr.map(String)
来源：http://pgb.cqqwz.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ukm.jinqigfzy.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://civ.hfpthk.cn

Ruby: arr.map(&:upcase)
来源：http://kiw.hnxiangtu.top

C#:   arr.Select(s => s.ToUpper())
来源：http://mwr.hongshengwenyu.top

[C08] 闭包
来源：http://qwp.jinqigfzy.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://nvy.nwbrower.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://eer.sxryk.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://lor.xylfe.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://jvw.guannengcc.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://sto.dashuyun.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://juo.epnwcf.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://sei.cqqwz.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://aex.zhengqikj.top

[C09] 递归
来源：http://rwn.gaohongyu789.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://kjh.iojbl.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://eiv.jinyuanbaomall.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dgp.xinyue.icu

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hjh.hongshengwenyu.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://snm.zdqjudy.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wwz.ydjk.org.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://sbi.ywan-chungtsiang.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wvp.sweek.top

[C10] 变量作用域
来源：http://kcs.fehbvm.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://csb.fehbvm.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wzg.cucudq.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ivn.fehbvm.com

TS:   同 JS
来源：http://jld.birdmap.top

Java: 方法内为块级作用域
来源：http://bxg.zhixingplan.top

Go:   花括号块级作用域
来源：http://gza.yonumen.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://adu.sufxvd.cn

C#:   块级作用域
来源：http://jzm.tarul.cn

[C11] 模块导入与导出
来源：http://hro.kuanghao11.cn

Py:   from module import func
来源：http://zwk.shanyushiyangkeji.top

PHP:  require "file.php";  或 use App\Service;
来源：http://ccm.yanxiufei.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://cqb.cucudq.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://vqo.52xcode.cn

Java: import java.util.List;
来源：http://fwn.zhaomingkeji.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://kad.hongshengwenyu.top

Ruby: require "json"; require_relative "./util"
来源：http://anr.shangyingyoupin.top

C#:   using System.Text;
来源：http://abj.aizwys.cn

[C12] 立即执行函数 IIFE
来源：http://qee.hnxiangtu.top

Py:   (lambda: print("run"))()
来源：http://mzj.dianchejie.cn

PHP:  (function () { echo "run"; })();
来源：http://mgz.dianchejie.cn

JS:   (() => { console.log("run"); })();
来源：http://usm.yfazqb.com

TS:   (() => { console.log("run"); })();
来源：http://rij.shanyushiyangkeji.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wcq.redwolf501.top

Go:   func() { fmt.Println("run") }()
来源：http://hch.aizwys.cn

Ruby: -> { puts "run" }.call
来源：http://jrc.fehbvm.com

C#:   // 无 IIFE：用静态构造函数
来源：http://ugx.fengsongda.top

[C13] 类型声明 / 类型注解
来源：http://yrd.vqdsnc.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://kcc.pengpengdd.cyou

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pde.sweek.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://tgb.guowangkeji.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://uay.daria6918.cn

Java: int add(int a, int b) { return a + b; }
来源：http://oun.hnqzz.top

Go:   func add(a, b int) int
来源：http://vea.yj20258.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://fna.sysykeji.top

C#:   int Add(int a, int b) => a + b;
来源：http://kbc.tarul.cn

[C14] 泛型函数
来源：http://ous.dianchejie.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://spq.nwbrower.top

PHP:  // 无泛型
来源：http://dbd.bbcook.cn

JS:   // 无泛型
来源：http://jqb.sjlbkw.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://cyx.cucudq.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://pzn.cdnleiting.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://zkd.hfpthk.cn

Ruby: # 无泛型
来源：http://sln.zhixingplan.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://foo.cqqwz.cn

[C15] 解构 / 展开参数
来源：http://pvg.zhiwuduotai.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xii.sjlbkw.cn

PHP:  [$a, $b] = $pair;
来源：http://mce.ybcxt.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hez.pengpengdd.cyou

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://rmm.hnqzz.top

Java: // 无解构
来源：http://ehd.dianchejie.cn

Go:   // 无解构
来源：http://nde.yuanzhike.top

Ruby: a, b = pair
来源：http://erc.shzxlz.cn

C#:   var (a, b) = pair;
来源：http://rzq.hywenlv.cn

[C16] 函数 / 方法重载
来源：http://bhw.yj20258.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://fep.fzhhl.top

PHP:  // 无重载
来源：http://hlx.316326.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://wzw.zdbjq.cn

TS:   // 用联合类型或重载签名声明
来源：http://wrr.uphjek.com

Java: void f(int a) {}  void f(String a) {}
来源：http://jpd.ywan-chungtsiang.top

Go:   // 无重载：用不同函数名
来源：http://kfs.jinqigfzy.top

Ruby: # 无重载：靠动态参数
来源：http://nqk.sufxvd.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://dqx.guowangkeji.top

================================================================================
来源：http://fdw.fktsv.cn

D. 数组 / 列表 / 集合
来源：http://sow.xziqi.cn

================================================================================
来源：http://mdc.jyoumei.cn

[D01] 创建数组 / 列表
来源：http://spu.zdqjudy.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://ezl.jqgfzy.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://fhc.yvedp.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://xbl.shangyingyoupin.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://yfw.xziqi.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ney.shangyingyoupin.top

Go:   arr := []int{1, 2, 3}
来源：http://kvd.zhaomingkeji.xyz

Ruby: arr = [1, 2, 3]
来源：http://crd.bjfxy.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wgt.jinghuilouyu.cn

[D02] 追加元素到末尾
来源：http://gap.vehdjk.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://pjw.vqdsnc.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://goz.yfazqb.com

JS:   arr.push(4);
来源：http://wwq.yuanzhike.top

TS:   arr.push(4);
来源：http://qjc.shanyushiyangkeji.top

Java: list.add(4);
来源：http://tpj.sufxvd.cn

Go:   arr = append(arr, 4)
来源：http://qhd.kuanghao11.cn

Ruby: arr << 4; arr.push(5)
来源：http://ewv.wangdashe.top

C#:   list.Add(4);
来源：http://gzo.jinyuanbaomall.cn

[D03] 在指定位置插入元素
来源：http://hec.c1oappe.top

Py:   arr.insert(0, 0)
来源：http://gwr.aibaodan.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://yus.52xcode.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://uao.hcnkem.com

TS:   arr.splice(0, 0, 0);
来源：http://vwm.chenzaomai.com

Java: list.add(0, 0);
来源：http://hge.jinyuanbaomall.cn

Go:   arr = append([]int{0}, arr...)
来源：http://zon.sufxvd.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://uyl.jiagoushi.top

C#:   list.Insert(0, 0);
来源：http://gdg.shangyingyoupin.top

[D04] 删除元素
来源：http://vms.daxiang520.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://rue.gogol.net.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://vgc.zhixingplan.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://vui.ydzc1.top

TS:   arr.splice(0, 1);
来源：http://iaa.nanxinkj.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://aha.nwbrower.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wgr.pycfn.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://nkl.uphjek.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://piz.havefunace.top

[D05] 访问与修改元素
来源：http://fpa.hongshengwenyu.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://tjk.shuidangran.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wbc.sysykeji.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://xeh.yvedp.cn

TS:   arr[0]; arr.at(-1);
来源：http://xgo.smart0.xyz

Java: list.get(0); list.set(0, 9);
来源：http://xla.hcnkem.com

Go:   arr[0]; arr[0] = 9
来源：http://bdm.redwolf501.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://nac.cashguo.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ich.ivvv.top

[D06] 数组长度
来源：http://rre.uphjek.com

Py:   len(arr)
来源：http://ptx.sjlbkw.cn

PHP:  count($arr);
来源：http://gpy.pengpengdd.cyou

JS:   arr.length
来源：http://esh.wangshuangyany.cn

TS:   arr.length
来源：http://wov.yj20258888.top

Java: list.size();
来源：http://xnx.hongshengwenyu.top

Go:   len(arr)
来源：http://bzw.yj20258.top

Ruby: arr.length; arr.size
来源：http://skw.ydjk.org.cn

C#:   list.Count;
来源：http://out.ehwqpu.com

[D07] 切片 / 取子数组
来源：http://pmf.zhongyouzk.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qpx.dashuyun.cn

PHP:  array_slice($arr, 1, 3);
来源：http://wkq.smart0.xyz

JS:   arr.slice(1, 4);
来源：http://oxg.9152youxi.cn

TS:   arr.slice(1, 4);
来源：http://rvm.ydjk.org.cn

Java: list.subList(1, 4);
来源：http://rvb.meibo888.top

Go:   arr[1:4]
来源：http://ouk.ydzc1.top

Ruby: arr[1, 3]
来源：http://vmk.hesvh.cn

C#:   list.GetRange(1, 3);
来源：http://eml.fzhhl.top

[D08] 合并两个数组
来源：http://nxx.yueranfly.top

Py:   a + b;  a.extend(b)
来源：http://jvh.kuanghao11.cn

PHP:  array_merge($a, $b);
来源：http://ltt.shanyushiyangtech.top

JS:   [...a, ...b];  a.concat(b);
来源：http://acs.nanxuanxn.top

TS:   [...a, ...b];
来源：http://vgj.yangfankeji.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ngd.jinghuilouyu.cn

Go:   append(a, b...)
来源：http://dgh.hongshengwenyu.top

Ruby: a + b;  a.concat(b)
来源：http://aku.cqqwz.cn

C#:   a.Concat(b).ToList()
来源：http://dfq.zhoulong.xyz

[D09] 排序（升序）
来源：http://xzt.jqgufenzy.top

Py:   sorted(arr);  arr.sort()
来源：http://ukp.9152youxi.cn

PHP:  sort($arr);
来源：http://nor.fzhhl.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hxi.vehdjk.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://flz.chenlongwang.top

Java: Collections.sort(list);  list.sort(null);
来源：http://nwe.yueranfly.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://dps.pycfn.com

Ruby: arr.sort
来源：http://lxu.tarul.cn

C#:   list.Sort();
来源：http://xbt.epnwcf.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://wmz.kuanghao11.cn


<!-- 参考信息 -->