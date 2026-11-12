代发 wailian999

PHP:  range(0, 10, 2);
来源：http://mwl.xylfe.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://exv.birdmap.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yuk.c1oappe.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://fsg.daria6918.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://all.jqgfzy.top

Ruby: (0...10).step(2).to_a
来源：http://ecx.aibaodan.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hvw.zhongyouzk.top

[B12] 跳出多层循环
来源：http://qtb.yj202588.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://bht.bjfxy.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://bbw.haohaochexian.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://gdg.jinghuilouyu.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://pby.hesvh.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ttd.daria6918.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://eld.yangfankeji.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://jjt.ppjwa.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://qrw.cqqwz.cn

[B13] 判断是否为数字
来源：http://xcw.shanyushiyangkeji.top

Py:   isinstance(x, (int, float))
来源：http://mvt.zhixingplan.top

PHP:  is_numeric($x)
来源：http://zug.zhiwuduotai.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wcx.tian-w.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ofo.sysykeji.top

Java: x instanceof Number
来源：http://rkf.hnqzz.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://qts.xingfuxueyuan.xyz

Ruby: x.is_a?(Numeric)
来源：http://nch.fehbvm.com

C#:   x is int or double or decimal
来源：http://sfr.epnwcf.com

[B14] 判断值是否在集合内
来源：http://xkc.316326.xyz

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jda.hysaishi.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://pwz.yj20258.top

JS:   [1, 2, 3].includes(x)
来源：http://xpe.svipenyu.cn

TS:   [1, 2, 3].includes(x)
来源：http://doj.pengpengdd.cyou

Java: List.of(1, 2, 3).contains(x)
来源：http://nnv.ehwqpu.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://pov.tarul.cn

Ruby: [1, 2, 3].include?(x)
来源：http://rdf.zdbjq.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://xmr.smart0.xyz

[B15] 布尔运算与取反
来源：http://uwb.gaohongyu789.top

Py:   a and b or not c
来源：http://rmx.ywan-chungtsiang.top

PHP:  $a && $b || !$c
来源：http://oeg.havefunace.top

JS:   a && b || !c
来源：http://tzs.snrcjt.cn

TS:   a && b || !c
来源：http://bdo.feifeiyinyue.top

Java: a && b || !c
来源：http://tft.hywenlv.cn

Go:   a && b || !c
来源：http://luo.0kj1m.cn

Ruby: a && b || !c
来源：http://fsy.aizwys.cn

C#:   a && b || !c
来源：http://etz.pycfn.com

[B16] 卫语句：不满足条件提前返回
来源：http://svr.yongpay.top

Py:   if not data: return
来源：http://msv.52xcode.cn

PHP:  if (!$data) { return; }
来源：http://por.0kj1m.cn

JS:   if (!data) return;
来源：http://jgi.ydjk.org.cn

TS:   if (!data) return;
来源：http://deq.zdbjq.cn

Java: if (data == null) return;
来源：http://mbb.sysykeji.top

Go:   if data == nil { return }
来源：http://apt.xuanzx.com

Ruby: return if data.nil?
来源：http://nyq.pycfn.com

C#:   if (data == null) return;
来源：http://xyz.guowangkeji.top

================================================================================
来源：http://dkc.chenzaomai.com

C. 函数与作用域
来源：http://phz.52xcode.cn

================================================================================
来源：http://dim.tianlin.xyz

[C01] 定义函数
来源：http://oar.fzhhl.top

Py:   def add(a, b): return a + b
来源：http://scg.jinqigfzy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xcm.svipenyu.cn

JS:   function add(a, b) { return a + b; }
来源：http://jqn.xuetiantiany.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nqe.sjlbkw.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ion.jinqigufen.top

Go:   func add(a, b int) int { return a + b }
来源：http://rqy.hnqzz.top

Ruby: def add(a, b); a + b; end
来源：http://vol.hywenlv.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://yqb.cashguo.top

[C02] 默认参数
来源：http://epq.mhx1999.top

Py:   def greet(name="World"): return name
来源：http://hxw.andypj.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://cnw.jinqigufen.top

JS:   function greet(name = "World") { return name; }
来源：http://hrw.gzhubu.top

TS:   function greet(name: string = "World") { return name; }
来源：http://pvx.nanxuanxn.top

Java: // 无默认参数：方法重载或 Optional
来源：http://lzi.gotoacloud.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://gkl.jinghuilouyu.cn

Ruby: def greet(name = "World") = name
来源：http://ynp.hnqzz.top

C#:   string Greet(string name = "World") => name;
来源：http://fra.andypj.xyz

[C03] 可变参数
来源：http://wtw.zhiwuduotai.top

Py:   def total(*args): return sum(args)
来源：http://joy.haohaochexian.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://bym.hfpthk.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://xku.wangshuangyany.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://flm.nwbrower.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://xpd.hnqzz.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://oos.xingfuxueyuan.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://dcb.xuanzx.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://qws.xylfe.cn

[C04] 命名参数 / 关键字参数
来源：http://lrg.sjlbkw.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hnl.zycfv.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://qsv.pengpengdd.cyou

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mah.yonumen.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://yrc.ywan-chungtsiang.top

Java: // 无：用 Builder 模式或 record
来源：http://ptm.ehwqpu.com

Go:   // 无：用配置结构体参数
来源：http://fdv.pycfn.com

Ruby: f(a: 1, b: 2)
来源：http://lui.birdmap.top

C#:   f(a: 1, b: 2)
来源：http://oqv.mhx1999.top

[C05] 返回多个值
来源：http://gps.fengsongda.top

Py:   return a, b
来源：http://rkh.yuxming.cn

PHP:  return [$a, $b];
来源：http://omo.xuetiantiany.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://zel.chenzaomai.com

TS:   return { a, b };
来源：http://ldw.zhijiandao.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://nba.aibaodan.cn

Go:   return a, b
来源：http://zkc.shzxlz.cn

Ruby: return a, b
来源：http://joq.aibaodan.cn

C#:   return (a, b);              // ValueTuple
来源：http://vaz.zhengqikj.top

[C06] 匿名函数 / lambda
来源：http://mhv.316326.xyz

Py:   square = lambda x: x * x
来源：http://bgh.daxiang520.top

PHP:  $square = fn($x) => $x * $x;
来源：http://yai.zdqjudy.top

JS:   const square = x => x * x;
来源：http://eci.sufxvd.cn

TS:   const square = (x: number): number => x * x;
来源：http://abs.mhx1999.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://zmz.feifeiyinyue.top

Go:   sq := func(x int) int { return x * x }
来源：http://uvp.zhongyouzk.top

Ruby: square = ->(x) { x * x }
来源：http://dqm.cashguo.top

C#:   Func<int, int> square = x => x * x;
来源：http://vim.jqgfzy.top

[C07] 把函数作为参数传入
来源：http://jpf.yanxiufei.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://gvh.hesvh.cn

PHP:  array_map("strtoupper", $arr);
来源：http://nud.sufxvd.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wpq.snrcjt.cn

TS:   arr.map(String)
来源：http://rjw.jinghuilouyu.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://vva.yueranfly.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://oin.zhaomingkeji.xyz

Ruby: arr.map(&:upcase)
来源：http://xht.yanxiufei.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://rky.meibo888.top

[C08] 闭包
来源：http://bqn.sufxvd.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://jaq.feifeiyinyue.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://qix.daria6918.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://dhg.guannengcc.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://qfm.sxryk.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://dof.andypj.xyz

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://nfr.jlsjyb.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://por.pengpengdd.cyou

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wqi.shuidangran.top

[C09] 递归
来源：http://fcy.bjfxy.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ubp.pycfn.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://tho.hongshengwenyu.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vhm.redwolf501.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sih.cdnleiting.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://uma.yueranfly.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://iwf.nwbrower.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://qqm.aibaodan.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://fiq.316326.xyz

[C10] 变量作用域
来源：http://pqg.hnxiangtu.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://bal.iojbl.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://jyi.hnqzz.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://sxa.ywan-chungtsiang.top

TS:   同 JS
来源：http://xmv.chenlongwang.top

Java: 方法内为块级作用域
来源：http://tec.hfpthk.cn

Go:   花括号块级作用域
来源：http://hdo.sufxvd.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://bwi.jiagoushi.top

C#:   块级作用域
来源：http://bpl.nanxinkj.top

[C11] 模块导入与导出
来源：http://afg.zhixingplan.top

Py:   from module import func
来源：http://aan.yueranfly.top

PHP:  require "file.php";  或 use App\Service;
来源：http://efl.guowangkeji.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://lfm.fanxiaobao.xyz

TS:   export function f(): void {};  import { f } from "./m";
来源：http://kay.yuxming.cn

Java: import java.util.List;
来源：http://lhg.yongpay.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://bzf.hfpthk.cn

Ruby: require "json"; require_relative "./util"
来源：http://idj.ctjpmb.com

C#:   using System.Text;
来源：http://eqx.xylfe.cn

[C12] 立即执行函数 IIFE
来源：http://sdz.guannengcc.top

Py:   (lambda: print("run"))()
来源：http://sau.fktsv.cn

PHP:  (function () { echo "run"; })();
来源：http://edq.zdbjq.cn

JS:   (() => { console.log("run"); })();
来源：http://myl.9152youxi.cn

TS:   (() => { console.log("run"); })();
来源：http://tgg.gaohongyu789.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ggu.hywenlv.cn

Go:   func() { fmt.Println("run") }()
来源：http://rhx.shanyushiyangtech.top

Ruby: -> { puts "run" }.call
来源：http://kys.haohaochexian.top

C#:   // 无 IIFE：用静态构造函数
来源：http://ywi.zdqjudy.top

[C13] 类型声明 / 类型注解
来源：http://rcp.zhixingplan.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://xrf.nwbrower.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ltv.jinqigfzy.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://jlx.jinqigfzy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yif.fktsv.cn

Java: int add(int a, int b) { return a + b; }
来源：http://jdp.fktsv.cn

Go:   func add(a, b int) int
来源：http://tyy.yonumen.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://bob.andypj.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://odp.pycfn.com

[C14] 泛型函数
来源：http://wma.chenlongwang.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://amb.jqgfzy.top

PHP:  // 无泛型
来源：http://enp.zhixingplan.top

JS:   // 无泛型
来源：http://dlt.ctjpmb.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://xnx.shzxlz.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://bix.gotoacloud.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://xdl.jqgufenzy.top

Ruby: # 无泛型
来源：http://gwy.ctjpmb.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://jyh.snrcjt.cn

[C15] 解构 / 展开参数
来源：http://doz.fengsongda.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://sva.sjlbkw.cn

PHP:  [$a, $b] = $pair;
来源：http://ady.jiagoushi.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://rxo.yuxming.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hju.jinqigufen.top

Java: // 无解构
来源：http://fkh.pycfn.com

Go:   // 无解构
来源：http://hjk.zhoulong.xyz

Ruby: a, b = pair
来源：http://ifv.dashuyun.cn

C#:   var (a, b) = pair;
来源：http://irq.ydjk.org.cn

[C16] 函数 / 方法重载
来源：http://hnm.zhixingplan.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://lwn.gzhubu.top

PHP:  // 无重载
来源：http://efo.hnqzz.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://snc.quarkkingdee.top

TS:   // 用联合类型或重载签名声明
来源：http://mpt.ppjwa.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://lkm.xuanzx.com

Go:   // 无重载：用不同函数名
来源：http://lor.havefunace.top

Ruby: # 无重载：靠动态参数
来源：http://ymk.jqgfzy.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://hsj.pengpengdd.cyou

================================================================================
来源：http://zrn.guowangkeji.top

D. 数组 / 列表 / 集合
来源：http://bxg.yongpay.top

================================================================================
来源：http://mma.xuanzx.com

[D01] 创建数组 / 列表
来源：http://jzd.ywan-chungtsiang.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://yvu.shuidangran.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wvi.hcnkem.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wqg.yongpay.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://wgv.sweek.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://rhu.shanyushiyangtech.top

Go:   arr := []int{1, 2, 3}
来源：http://zsk.epnwcf.com

Ruby: arr = [1, 2, 3]
来源：http://hab.hysaishi.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://zlx.havefunace.top

[D02] 追加元素到末尾
来源：http://apd.fktsv.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://jzj.nanxinkj.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://adn.ywan-chungtsiang.top

JS:   arr.push(4);
来源：http://hlc.shuidangran.top

TS:   arr.push(4);
来源：http://sno.fengsongda.top

Java: list.add(4);
来源：http://bpi.hnxiangtu.top

Go:   arr = append(arr, 4)
来源：http://bco.shangyingyoupin.top

Ruby: arr << 4; arr.push(5)
来源：http://dhk.zycfv.cn

C#:   list.Add(4);
来源：http://vqa.316326.xyz

[D03] 在指定位置插入元素
来源：http://pmt.zhaomingkeji.xyz

Py:   arr.insert(0, 0)
来源：http://vkl.fanxiaobao.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://cyy.yangfankeji.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ugc.ctjpmb.com

TS:   arr.splice(0, 0, 0);
来源：http://mte.svipenyu.cn

Java: list.add(0, 0);
来源：http://hpu.chenzaomai.com

Go:   arr = append([]int{0}, arr...)
来源：http://iru.daxiang520.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://amo.hammf.cn

C#:   list.Insert(0, 0);
来源：http://gzi.pengpengdd.cyou

[D04] 删除元素
来源：http://ejt.cqqwz.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mur.ehwqpu.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://rwq.fehbvm.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://uol.hywenlv.cn

TS:   arr.splice(0, 1);
来源：http://jmb.yuxming.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://yco.fzhhl.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://pmu.jqgfzy.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://sow.hnxiangtu.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://bpl.sxryk.cn

[D05] 访问与修改元素
来源：http://ugt.fanxiaobao.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://euf.birdmap.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://aqe.gotoacloud.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://uyl.yj202588.top

TS:   arr[0]; arr.at(-1);
来源：http://xbt.jinghuilouyu.cn

Java: list.get(0); list.set(0, 9);
来源：http://wcp.svipenyu.cn

Go:   arr[0]; arr[0] = 9
来源：http://pwv.sjlbkw.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://sjy.yonumen.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://szv.redwolf501.top

[D06] 数组长度
来源：http://yru.zdbjq.cn

Py:   len(arr)
来源：http://qge.fengsongda.top

PHP:  count($arr);
来源：http://byf.mhx1999.top

JS:   arr.length
来源：http://pyv.0kj1m.cn

TS:   arr.length
来源：http://msv.hnqzz.top

Java: list.size();
来源：http://vvr.vehdjk.com

Go:   len(arr)
来源：http://emz.uphjek.com

Ruby: arr.length; arr.size
来源：http://rjf.ybcxt.top

C#:   list.Count;
来源：http://kil.havefunace.top

[D07] 切片 / 取子数组
来源：http://vtp.cqqwz.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://nwu.yonumen.top

PHP:  array_slice($arr, 1, 3);
来源：http://bsf.chenzaomai.com

JS:   arr.slice(1, 4);
来源：http://rlh.xylfe.cn

TS:   arr.slice(1, 4);
来源：http://agu.dianchejie.cn

Java: list.subList(1, 4);
来源：http://mkx.yvedp.cn

Go:   arr[1:4]
来源：http://qce.wangshuangyany.cn

Ruby: arr[1, 3]
来源：http://tts.yuanzhike.top

C#:   list.GetRange(1, 3);
来源：http://boc.uphjek.com

[D08] 合并两个数组
来源：http://jcv.jqgufenzy.top

Py:   a + b;  a.extend(b)
来源：http://kub.yonumen.top

PHP:  array_merge($a, $b);
来源：http://ipv.ivvv.top

JS:   [...a, ...b];  a.concat(b);
来源：http://tbk.quarkkingdee.top

TS:   [...a, ...b];
来源：http://tkt.dianchejie.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://jgc.guowangkeji.top

Go:   append(a, b...)
来源：http://kqo.redwolf501.top

Ruby: a + b;  a.concat(b)
来源：http://faw.iojbl.cn

C#:   a.Concat(b).ToList()
来源：http://osq.zhongyouzk.top

[D09] 排序（升序）
来源：http://olb.316326.xyz

Py:   sorted(arr);  arr.sort()
来源：http://msq.jyoumei.cn

PHP:  sort($arr);
来源：http://kys.chenlongwang.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://cjz.havefunace.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://tcq.yj202588.top

Java: Collections.sort(list);  list.sort(null);
来源：http://pjg.yongpay.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wik.cashguo.top

Ruby: arr.sort
来源：http://awa.nanxinkj.top

C#:   list.Sort();
来源：http://und.tianlin.xyz

[D10] 自定义排序（按字段 / 多条件）
来源：http://fcc.cdnleiting.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://erc.ehwqpu.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zax.kuanghao11.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://erh.sjlbkw.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://yph.zhoulong.xyz

Java: list.sort(Comparator.comparing(Person::age));
来源：http://fjt.hcnkem.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://bgr.hysaishi.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://vfc.pycfn.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://dwd.gotoacloud.top

[D11] 反转数组
来源：http://dru.shuidangran.top

Py:   arr[::-1];  arr.reverse()
来源：http://vka.daria6918.cn

PHP:  array_reverse($arr);
来源：http://emf.xziqi.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ijv.hywenlv.cn

TS:   [...arr].reverse();
来源：http://ncv.0kj1m.cn

Java: Collections.reverse(list);
来源：http://skf.havefunace.top

Go:   slices.Reverse(arr)
来源：http://bnb.dianchejie.cn

Ruby: arr.reverse
来源：http://cgr.ppjwa.cn


<!-- 参考信息 -->