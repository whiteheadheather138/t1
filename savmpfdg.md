代发 wailian999

Java: outer: for (...) { for (...) { break outer; } }
来源：http://yma.cheryme.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://uxn.redwolf501.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://luh.ctjpmb.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://irt.andypj.xyz

[B13] 判断是否为数字
来源：http://ved.jyoumei.cn

Py:   isinstance(x, (int, float))
来源：http://gvi.dianchejie.cn

PHP:  is_numeric($x)
来源：http://grn.guannengcc.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://juz.hywenlv.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nai.pycfn.com

Java: x instanceof Number
来源：http://ffz.gaohongyu789.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wbw.jinghuilouyu.cn

Ruby: x.is_a?(Numeric)
来源：http://osm.sxryk.cn

C#:   x is int or double or decimal
来源：http://wur.zdqjudy.top

[B14] 判断值是否在集合内
来源：http://efp.ywan-chungtsiang.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://nty.sxryk.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://dlc.mhx1999.top

JS:   [1, 2, 3].includes(x)
来源：http://fif.pycfn.com

TS:   [1, 2, 3].includes(x)
来源：http://wco.sjlbkw.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://avz.mhx1999.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://jbv.kuanghao11.cn

Ruby: [1, 2, 3].include?(x)
来源：http://lqc.zhaomingkeji.xyz

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://vij.ctjpmb.com

[B15] 布尔运算与取反
来源：http://swi.smart0.xyz

Py:   a and b or not c
来源：http://qpc.cashguo.top

PHP:  $a && $b || !$c
来源：http://zit.jyoumei.cn

JS:   a && b || !c
来源：http://hqq.guowangkeji.top

TS:   a && b || !c
来源：http://eig.ivvv.top

Java: a && b || !c
来源：http://wns.52xcode.cn

Go:   a && b || !c
来源：http://pra.zhongyouzk.top

Ruby: a && b || !c
来源：http://hwz.nanxinkj.top

C#:   a && b || !c
来源：http://juu.hnqzz.top

[B16] 卫语句：不满足条件提前返回
来源：http://clk.yueranfly.top

Py:   if not data: return
来源：http://wch.kuanghao11.cn

PHP:  if (!$data) { return; }
来源：http://vvx.epnwcf.com

JS:   if (!data) return;
来源：http://rfn.cheryme.top

TS:   if (!data) return;
来源：http://acn.xziqi.cn

Java: if (data == null) return;
来源：http://jqn.wangdashe.top

Go:   if data == nil { return }
来源：http://opj.ehwqpu.com

Ruby: return if data.nil?
来源：http://ybm.dashuyun.cn

C#:   if (data == null) return;
来源：http://dyo.fanxiaobao.xyz

================================================================================
来源：http://obf.ywan-chungtsiang.top

C. 函数与作用域
来源：http://bpm.cucudq.cn

================================================================================
来源：http://vio.ybcxt.top

[C01] 定义函数
来源：http://lae.jinqigufen.top

Py:   def add(a, b): return a + b
来源：http://sqf.ehwqpu.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lsm.jinqigfzy.top

JS:   function add(a, b) { return a + b; }
来源：http://pmp.cucudq.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cxn.hcnkem.com

Java: static int add(int a, int b) { return a + b; }
来源：http://hwk.zhaomingkeji.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://iwy.yvedp.cn

Ruby: def add(a, b); a + b; end
来源：http://kqk.xylfe.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://bkp.tianlin.xyz

[C02] 默认参数
来源：http://hvo.daria6918.cn

Py:   def greet(name="World"): return name
来源：http://fmx.mhx1999.top

PHP:  function greet($name = "World") { return $name; }
来源：http://dqp.xuanzx.com

JS:   function greet(name = "World") { return name; }
来源：http://qdj.hnqzz.top

TS:   function greet(name: string = "World") { return name; }
来源：http://pit.nanxuanxn.top

Java: // 无默认参数：方法重载或 Optional
来源：http://gur.yueranfly.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://krw.9152youxi.cn

Ruby: def greet(name = "World") = name
来源：http://ttq.wangdashe.top

C#:   string Greet(string name = "World") => name;
来源：http://cws.jinqigfzy.top

[C03] 可变参数
来源：http://egv.cqqwz.cn

Py:   def total(*args): return sum(args)
来源：http://pkd.316326.xyz

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://yun.ctjpmb.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://rwq.ctjpmb.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wsu.yueranfly.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://cmc.zdbjq.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://jpb.jinqigufen.top

Ruby: def total(*nums); nums.sum; end
来源：http://sdx.pycfn.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://fba.bjfxy.top

[C04] 命名参数 / 关键字参数
来源：http://vhx.zhaomingkeji.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://xio.guowangkeji.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://lia.meibo888.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xyw.xziqi.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://des.zhiwuduotai.top

Java: // 无：用 Builder 模式或 record
来源：http://div.0kj1m.cn

Go:   // 无：用配置结构体参数
来源：http://yys.shuidangran.top

Ruby: f(a: 1, b: 2)
来源：http://vqb.pycfn.com

C#:   f(a: 1, b: 2)
来源：http://hjw.redwolf501.top

[C05] 返回多个值
来源：http://zyx.xingfuxueyuan.xyz

Py:   return a, b
来源：http://zku.xingfuxueyuan.xyz

PHP:  return [$a, $b];
来源：http://bkx.shanyushiyangkeji.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://axf.yj202588.top

TS:   return { a, b };
来源：http://kbr.aibaodan.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://dez.feifeiyinyue.top

Go:   return a, b
来源：http://hfq.epnwcf.com

Ruby: return a, b
来源：http://ysl.smart0.xyz

C#:   return (a, b);              // ValueTuple
来源：http://uat.jqgufenzy.top

[C06] 匿名函数 / lambda
来源：http://ucs.9152youxi.cn

Py:   square = lambda x: x * x
来源：http://aos.epnwcf.com

PHP:  $square = fn($x) => $x * $x;
来源：http://aab.jyoumei.cn

JS:   const square = x => x * x;
来源：http://sxi.guowangkeji.top

TS:   const square = (x: number): number => x * x;
来源：http://lvy.mhx1999.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://yzb.aizwys.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ldh.zdbjq.cn

Ruby: square = ->(x) { x * x }
来源：http://ddn.xinyue.icu

C#:   Func<int, int> square = x => x * x;
来源：http://zvi.ydzc1.top

[C07] 把函数作为参数传入
来源：http://psr.yanxiufei.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hpe.pycfn.com

PHP:  array_map("strtoupper", $arr);
来源：http://pkv.cashguo.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://lqg.jinyuanbaomall.cn

TS:   arr.map(String)
来源：http://dgl.gzhubu.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://nfq.daria6918.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mpl.chenzaomai.com

Ruby: arr.map(&:upcase)
来源：http://sac.ydzc1.top

C#:   arr.Select(s => s.ToUpper())
来源：http://lhs.shanyushiyangtech.top

[C08] 闭包
来源：http://pna.zhongyouzk.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wim.haohaochexian.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://cwb.ctjpmb.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://snx.chenlongwang.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://nvg.zhaomingkeji.xyz

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://iko.yueranfly.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ttu.xziqi.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://yee.ydzc1.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://xtx.jlsjyb.cn

[C09] 递归
来源：http://mwj.shangyingyoupin.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://poc.yangfankeji.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ees.hcnkem.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ytn.redwolf501.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ofl.xziqi.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://syd.yanxiufei.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://rvb.jyoumei.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://yyz.yuxming.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://tao.xylfe.cn

[C10] 变量作用域
来源：http://yqd.quarkkingdee.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://vni.gogol.net.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://dte.cucudq.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://uch.dashuyun.cn

TS:   同 JS
来源：http://muj.0kj1m.cn

Java: 方法内为块级作用域
来源：http://ofu.fehbvm.com

Go:   花括号块级作用域
来源：http://oej.ivvv.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://esg.yonumen.top

C#:   块级作用域
来源：http://zsk.sysykeji.top

[C11] 模块导入与导出
来源：http://xxl.ivvv.top

Py:   from module import func
来源：http://tqh.daria6918.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://zay.chenlongwang.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://pqk.yj202588.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://bok.guowangkeji.top

Java: import java.util.List;
来源：http://kba.dianchejie.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://bjj.ppjwa.cn

Ruby: require "json"; require_relative "./util"
来源：http://hbp.tian-w.cn

C#:   using System.Text;
来源：http://zbr.chenlongwang.top

[C12] 立即执行函数 IIFE
来源：http://ffk.nanxuanxn.top

Py:   (lambda: print("run"))()
来源：http://oxc.yongpay.top

PHP:  (function () { echo "run"; })();
来源：http://gvu.9152youxi.cn

JS:   (() => { console.log("run"); })();
来源：http://olx.yj20258888.top

TS:   (() => { console.log("run"); })();
来源：http://vvr.jiagoushi.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ynj.xingfuxueyuan.xyz

Go:   func() { fmt.Println("run") }()
来源：http://vsx.xziqi.cn

Ruby: -> { puts "run" }.call
来源：http://mgv.ydjk.org.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://kxr.epnwcf.com

[C13] 类型声明 / 类型注解
来源：http://anh.wangdashe.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://emn.zdbjq.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wes.aizwys.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://fwf.cqqwz.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fau.fehbvm.com

Java: int add(int a, int b) { return a + b; }
来源：http://bor.ywan-chungtsiang.top

Go:   func add(a, b int) int
来源：http://kqk.vqdsnc.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://woi.smart0.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://atk.daxiang520.top

[C14] 泛型函数
来源：http://ive.shanyushiyangkeji.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://pgk.ivvv.top

PHP:  // 无泛型
来源：http://unj.yanxiufei.cn

JS:   // 无泛型
来源：http://rep.sjlbkw.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://idn.zhengqikj.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ngx.nanxuanxn.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://knd.hnqzz.top

Ruby: # 无泛型
来源：http://yjt.yonumen.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://bqw.316326.xyz

[C15] 解构 / 展开参数
来源：http://lyb.zhixingplan.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://zqs.birdmap.top

PHP:  [$a, $b] = $pair;
来源：http://qjx.jianghu66.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ptd.zhengqikj.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://gwh.cheryme.top

Java: // 无解构
来源：http://gjt.jlsjyb.cn

Go:   // 无解构
来源：http://kyb.hesvh.cn

Ruby: a, b = pair
来源：http://khj.jqgfzy.top

C#:   var (a, b) = pair;
来源：http://rha.sysykeji.top

[C16] 函数 / 方法重载
来源：http://hmv.sweek.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vej.birdmap.top

PHP:  // 无重载
来源：http://jpm.316326.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://dth.chenjidiqi.icu

TS:   // 用联合类型或重载签名声明
来源：http://wyf.hnxiangtu.top

Java: void f(int a) {}  void f(String a) {}
来源：http://woh.tarul.cn

Go:   // 无重载：用不同函数名
来源：http://cka.0kj1m.cn

Ruby: # 无重载：靠动态参数
来源：http://clc.meibo888.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://eew.fzhhl.top

================================================================================
来源：http://rme.hywenlv.cn

D. 数组 / 列表 / 集合
来源：http://xna.wangshuangyany.cn

================================================================================
来源：http://gbu.ctjpmb.com

[D01] 创建数组 / 列表
来源：http://amj.fehbvm.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://lty.sxryk.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://yrc.aizwys.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mbp.gzhubu.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://lii.bjfxy.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mog.wangdashe.top

Go:   arr := []int{1, 2, 3}
来源：http://jvj.dashuyun.cn

Ruby: arr = [1, 2, 3]
来源：http://ekl.tian-w.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://jpf.sjlbkw.cn

[D02] 追加元素到末尾
来源：http://cpv.xziqi.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://naw.yvedp.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://fpi.jiagoushi.top

JS:   arr.push(4);
来源：http://cxv.jlsjyb.cn

TS:   arr.push(4);
来源：http://tcp.cqqwz.cn

Java: list.add(4);
来源：http://ggl.svipenyu.cn

Go:   arr = append(arr, 4)
来源：http://gbv.bbcook.cn

Ruby: arr << 4; arr.push(5)
来源：http://cfl.vqdsnc.cn

C#:   list.Add(4);
来源：http://nsn.fzhhl.top

[D03] 在指定位置插入元素
来源：http://bsi.kuanghao11.cn

Py:   arr.insert(0, 0)
来源：http://gwz.nwbrower.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hpc.gaohongyu789.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://xqt.sysykeji.top

TS:   arr.splice(0, 0, 0);
来源：http://suw.havefunace.top

Java: list.add(0, 0);
来源：http://cea.xinyue.icu

Go:   arr = append([]int{0}, arr...)
来源：http://fnw.xingfuxueyuan.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://kgn.redwolf501.top

C#:   list.Insert(0, 0);
来源：http://dng.ppjwa.cn

[D04] 删除元素
来源：http://pfg.yongpay.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wec.gaohongyu789.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://awz.cdnleiting.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://tbm.tian-w.cn

TS:   arr.splice(0, 1);
来源：http://qtn.nanxuanxn.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://yam.andypj.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ccn.yfazqb.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://izb.yj202588.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://vxc.gaohongyu789.top

[D05] 访问与修改元素
来源：http://uqf.smart0.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://kmh.zhaomingkeji.xyz

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://qnd.shanyushiyangtech.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wlh.chenlongwang.top

TS:   arr[0]; arr.at(-1);
来源：http://cna.pycfn.com

Java: list.get(0); list.set(0, 9);
来源：http://vev.wangdashe.top

Go:   arr[0]; arr[0] = 9
来源：http://wll.smart0.xyz

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ywb.cdnleiting.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://uel.jqgufenzy.top

[D06] 数组长度
来源：http://mts.jinghuilouyu.cn

Py:   len(arr)
来源：http://bwz.haohaochexian.top

PHP:  count($arr);
来源：http://tmx.52xcode.cn

JS:   arr.length
来源：http://afx.aizwys.cn

TS:   arr.length
来源：http://zcb.xinyue.icu

Java: list.size();
来源：http://flm.cdnleiting.top

Go:   len(arr)
来源：http://kcl.vqdsnc.cn

Ruby: arr.length; arr.size
来源：http://xjl.meibo888.top

C#:   list.Count;
来源：http://zqi.zhaomingkeji.xyz

[D07] 切片 / 取子数组
来源：http://blj.sweek.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://tuc.shuidangran.top

PHP:  array_slice($arr, 1, 3);
来源：http://cxk.fehbvm.com

JS:   arr.slice(1, 4);
来源：http://oez.mhx1999.top

TS:   arr.slice(1, 4);
来源：http://jkl.hywenlv.cn

Java: list.subList(1, 4);
来源：http://iwi.0kj1m.cn

Go:   arr[1:4]
来源：http://cxr.gzhubu.top

Ruby: arr[1, 3]
来源：http://zjw.ybcxt.top

C#:   list.GetRange(1, 3);
来源：http://xnl.nanxuanxn.top

[D08] 合并两个数组
来源：http://cya.jinyuanbaomall.cn

Py:   a + b;  a.extend(b)
来源：http://eov.guowangkeji.top

PHP:  array_merge($a, $b);
来源：http://sxn.aizwys.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://qcv.ydzc1.top

TS:   [...a, ...b];
来源：http://rad.svipenyu.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://det.meibo888.top

Go:   append(a, b...)
来源：http://zvy.jinqigufen.top

Ruby: a + b;  a.concat(b)
来源：http://nsg.andypj.xyz

C#:   a.Concat(b).ToList()
来源：http://dms.aizwys.cn

[D09] 排序（升序）
来源：http://cah.nanxuanxn.top

Py:   sorted(arr);  arr.sort()
来源：http://fao.ydzc1.top

PHP:  sort($arr);
来源：http://pxq.fktsv.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://dhs.guannengcc.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://uml.daria6918.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ter.sxryk.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://rlk.xingfuxueyuan.xyz

Ruby: arr.sort
来源：http://rws.svipenyu.cn

C#:   list.Sort();
来源：http://ewn.ywan-chungtsiang.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://grj.wangshuangyany.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ckr.yueranfly.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://apk.dianchejie.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://zje.9152youxi.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://qbf.haohaochexian.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ndx.andypj.xyz

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://vff.uphjek.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://fvv.fanxiaobao.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ori.yanxiufei.cn

[D11] 反转数组
来源：http://guq.redwolf501.top

Py:   arr[::-1];  arr.reverse()
来源：http://okx.aibaodan.cn

PHP:  array_reverse($arr);
来源：http://oke.yongpay.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://njp.zdqjudy.top

TS:   [...arr].reverse();
来源：http://czh.haohaochexian.top

Java: Collections.reverse(list);
来源：http://tdj.nanxinkj.top

Go:   slices.Reverse(arr)
来源：http://vqr.zhaomingkeji.xyz

Ruby: arr.reverse
来源：http://ajt.ivvv.top

C#:   list.Reverse();
来源：http://ukf.xinyue.icu

[D12] 查找元素下标
来源：http://zgq.jyoumei.cn

Py:   arr.index(x);  x in arr
来源：http://suz.jinqigfzy.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ixj.hesvh.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ssm.zdqjudy.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ngm.9152youxi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://esf.nanxuanxn.top

Go:   slices.Index(arr, x)
来源：http://hdu.shangyingyoupin.top

Ruby: arr.index(x)
来源：http://nrx.hysaishi.cn

C#:   list.IndexOf(x);
来源：http://tkf.xziqi.cn

[D13] 过滤（保留满足条件的）
来源：http://obs.jqgufenzy.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://efu.ivvv.top


<!-- 参考信息 -->