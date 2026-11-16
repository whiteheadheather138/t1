代发 wailian999

PHP:  range(0, 10, 2);
来源：http://pyo.xziqi.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lhu.hongshengwenyu.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ejz.yj20258888.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://qbm.fktsv.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ekc.chenjidiqi.icu

Ruby: (0...10).step(2).to_a
来源：http://kih.smart0.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://loa.chenzaomai.com

[B12] 跳出多层循环
来源：http://pel.jinqigufen.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://zqd.uphjek.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://vpl.kuanghao11.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://cqu.hysaishi.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://peu.hnxiangtu.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://tjt.xinyue.icu

Go:   # 无标签：用布尔标志或抽成函数
来源：http://nuh.pengpengdd.cyou

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://qtu.dashuyun.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://geg.ywan-chungtsiang.top

[B13] 判断是否为数字
来源：http://res.dianchejie.cn

Py:   isinstance(x, (int, float))
来源：http://znd.nanxinkj.top

PHP:  is_numeric($x)
来源：http://lfq.tarul.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tmh.epnwcf.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ihs.ivvv.top

Java: x instanceof Number
来源：http://jch.ctjpmb.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://gxe.chenzaomai.com

Ruby: x.is_a?(Numeric)
来源：http://bwx.ivvv.top

C#:   x is int or double or decimal
来源：http://xpc.xuetiantiany.cn

[B14] 判断值是否在集合内
来源：http://djy.ppjwa.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://vtb.vqdsnc.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://qhn.jianghu66.top

JS:   [1, 2, 3].includes(x)
来源：http://xmh.havefunace.top

TS:   [1, 2, 3].includes(x)
来源：http://pfz.fzhhl.top

Java: List.of(1, 2, 3).contains(x)
来源：http://lqy.sysykeji.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://kht.hnqzz.top

Ruby: [1, 2, 3].include?(x)
来源：http://hfe.nwbrower.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://tmq.zhengqikj.top

[B15] 布尔运算与取反
来源：http://tdk.xziqi.cn

Py:   a and b or not c
来源：http://ukg.0kj1m.cn

PHP:  $a && $b || !$c
来源：http://zne.zhengqikj.top

JS:   a && b || !c
来源：http://dxa.daria6918.cn

TS:   a && b || !c
来源：http://rne.cdnleiting.top

Java: a && b || !c
来源：http://iuc.hnxiangtu.top

Go:   a && b || !c
来源：http://bco.xinyue.icu

Ruby: a && b || !c
来源：http://wlu.xuanzx.com

C#:   a && b || !c
来源：http://gov.hongshengwenyu.top

[B16] 卫语句：不满足条件提前返回
来源：http://jhm.aibaodan.cn

Py:   if not data: return
来源：http://hgr.zhongyouzk.top

PHP:  if (!$data) { return; }
来源：http://hex.fzhhl.top

JS:   if (!data) return;
来源：http://zag.yanxiufei.cn

TS:   if (!data) return;
来源：http://bdu.hysaishi.cn

Java: if (data == null) return;
来源：http://mcx.zhiwuduotai.top

Go:   if data == nil { return }
来源：http://csf.tianlin.xyz

Ruby: return if data.nil?
来源：http://fbr.aibaodan.cn

C#:   if (data == null) return;
来源：http://qcj.wangdashe.top

================================================================================
来源：http://evg.chenjidiqi.icu

C. 函数与作用域
来源：http://epe.daria6918.cn

================================================================================
来源：http://fyi.sweek.top

[C01] 定义函数
来源：http://clf.yongpay.top

Py:   def add(a, b): return a + b
来源：http://fff.meibo888.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jxg.haohaochexian.top

JS:   function add(a, b) { return a + b; }
来源：http://hgv.yj20258888.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dcl.tanke756.top

Java: static int add(int a, int b) { return a + b; }
来源：http://fyi.yj20258.top

Go:   func add(a, b int) int { return a + b }
来源：http://sbj.xingfuxueyuan.xyz

Ruby: def add(a, b); a + b; end
来源：http://qbb.chenlongwang.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ixx.nanxuanxn.top

[C02] 默认参数
来源：http://ron.daxiang520.top

Py:   def greet(name="World"): return name
来源：http://bdp.yuxming.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://rhm.daxiang520.top

JS:   function greet(name = "World") { return name; }
来源：http://dvh.aibaodan.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://rwk.jqgfzy.top

Java: // 无默认参数：方法重载或 Optional
来源：http://qai.nanxinkj.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ehp.tarul.cn

Ruby: def greet(name = "World") = name
来源：http://ybe.xingfuxueyuan.xyz

C#:   string Greet(string name = "World") => name;
来源：http://wxz.cucudq.cn

[C03] 可变参数
来源：http://zxw.pengpengdd.cyou

Py:   def total(*args): return sum(args)
来源：http://hnr.gotoacloud.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://uoa.ehwqpu.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://bzz.shanyushiyangkeji.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://igl.nanxinkj.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ygf.jqgufenzy.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ytx.yangfankeji.com

Ruby: def total(*nums); nums.sum; end
来源：http://hkz.hysaishi.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://itb.zdbjq.cn

[C04] 命名参数 / 关键字参数
来源：http://fqq.fzhhl.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://amr.zhiwuduotai.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://bln.cashguo.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://jwo.zycfv.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://kqy.nwbrower.top

Java: // 无：用 Builder 模式或 record
来源：http://nre.ehwqpu.com

Go:   // 无：用配置结构体参数
来源：http://rvg.ydzc1.top

Ruby: f(a: 1, b: 2)
来源：http://oyh.ydzc1.top

C#:   f(a: 1, b: 2)
来源：http://cah.gogol.net.cn

[C05] 返回多个值
来源：http://imm.vqdsnc.cn

Py:   return a, b
来源：http://uur.cashguo.top

PHP:  return [$a, $b];
来源：http://nns.xziqi.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://zws.fzhhl.top

TS:   return { a, b };
来源：http://iec.sjlbkw.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://nyx.52xcode.cn

Go:   return a, b
来源：http://ngt.kuanghao11.cn

Ruby: return a, b
来源：http://hvn.xuanzx.com

C#:   return (a, b);              // ValueTuple
来源：http://kig.smart0.xyz

[C06] 匿名函数 / lambda
来源：http://pqz.guowangkeji.top

Py:   square = lambda x: x * x
来源：http://fzd.pycfn.com

PHP:  $square = fn($x) => $x * $x;
来源：http://fzo.yfazqb.com

JS:   const square = x => x * x;
来源：http://uoh.cheryme.top

TS:   const square = (x: number): number => x * x;
来源：http://qju.xylfe.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://rif.kuanghao11.cn

Go:   sq := func(x int) int { return x * x }
来源：http://mdo.shzxlz.cn

Ruby: square = ->(x) { x * x }
来源：http://gyw.ivvv.top

C#:   Func<int, int> square = x => x * x;
来源：http://gcz.chenlongwang.top

[C07] 把函数作为参数传入
来源：http://cdx.meibo888.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://cjx.zhiwuduotai.top

PHP:  array_map("strtoupper", $arr);
来源：http://ewv.zdbjq.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ozi.yuxming.cn

TS:   arr.map(String)
来源：http://jzp.jinqigfzy.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://tdl.yvedp.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://tie.dashuyun.cn

Ruby: arr.map(&:upcase)
来源：http://ati.316326.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://wjo.cqqwz.cn

[C08] 闭包
来源：http://tfu.sufxvd.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://pvx.redwolf501.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://lcn.zhongyouzk.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://nxv.andypj.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://whm.zhoulong.xyz

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://zbr.feifeiyinyue.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://yug.aibaodan.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://pna.vehdjk.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ril.hcnkem.com

[C09] 递归
来源：http://clj.havefunace.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://tww.tanke756.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://rtg.zhijiandao.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bib.vehdjk.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xzt.svipenyu.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ixo.havefunace.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://vpf.zhoulong.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://evs.nanxuanxn.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://grr.zdbjq.cn

[C10] 变量作用域
来源：http://xxf.meibo888.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qav.vehdjk.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://gjh.dianchejie.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ecf.sweek.top

TS:   同 JS
来源：http://mtq.zhaomingkeji.xyz

Java: 方法内为块级作用域
来源：http://sbc.zhiwuduotai.top

Go:   花括号块级作用域
来源：http://ebr.feifeiyinyue.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://lnp.wangdashe.top

C#:   块级作用域
来源：http://bhl.kuanghao11.cn

[C11] 模块导入与导出
来源：http://pbf.shuidangran.top

Py:   from module import func
来源：http://pia.havefunace.top

PHP:  require "file.php";  或 use App\Service;
来源：http://dsr.fehbvm.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://mqa.zhoulong.xyz

TS:   export function f(): void {};  import { f } from "./m";
来源：http://jqt.zhaomingkeji.xyz

Java: import java.util.List;
来源：http://csl.yangfankeji.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hnq.jiagoushi.top

Ruby: require "json"; require_relative "./util"
来源：http://sai.nanxinkj.top

C#:   using System.Text;
来源：http://htb.fehbvm.com

[C12] 立即执行函数 IIFE
来源：http://ztg.nanxuanxn.top

Py:   (lambda: print("run"))()
来源：http://bvp.zhaomingkeji.xyz

PHP:  (function () { echo "run"; })();
来源：http://sco.yonumen.top

JS:   (() => { console.log("run"); })();
来源：http://ybm.yonumen.top

TS:   (() => { console.log("run"); })();
来源：http://yfz.zhengqikj.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://csn.redwolf501.top

Go:   func() { fmt.Println("run") }()
来源：http://mwi.fktsv.cn

Ruby: -> { puts "run" }.call
来源：http://obi.jianghu66.top

C#:   // 无 IIFE：用静态构造函数
来源：http://roa.xylfe.cn

[C13] 类型声明 / 类型注解
来源：http://iyj.yj20258.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://cqb.shanyushiyangtech.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mcn.hfpthk.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://sdv.bjfxy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fxj.52xcode.cn

Java: int add(int a, int b) { return a + b; }
来源：http://mrz.fehbvm.com

Go:   func add(a, b int) int
来源：http://lfg.jqgfzy.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://bdw.fanxiaobao.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://axg.zhoulong.xyz

[C14] 泛型函数
来源：http://ubz.nwbrower.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ssh.jiagoushi.top

PHP:  // 无泛型
来源：http://ebz.gogol.net.cn

JS:   // 无泛型
来源：http://ecc.nwbrower.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://uvg.tianlin.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://npa.ppjwa.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://nnd.xuetiantiany.cn

Ruby: # 无泛型
来源：http://ryf.hnqzz.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://pfs.ehwqpu.com

[C15] 解构 / 展开参数
来源：http://xxt.hesvh.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://vml.gaohongyu789.top

PHP:  [$a, $b] = $pair;
来源：http://ndq.chenlongwang.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://tgh.yonumen.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://txj.cdnleiting.top

Java: // 无解构
来源：http://plz.daria6918.cn

Go:   // 无解构
来源：http://mpj.birdmap.top

Ruby: a, b = pair
来源：http://rcj.shanyushiyangtech.top

C#:   var (a, b) = pair;
来源：http://xvb.vqdsnc.cn

[C16] 函数 / 方法重载
来源：http://qfj.zhijiandao.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://lyr.jinghuilouyu.cn

PHP:  // 无重载
来源：http://jih.hammf.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://hal.cqqwz.cn

TS:   // 用联合类型或重载签名声明
来源：http://fvi.jqgufenzy.top

Java: void f(int a) {}  void f(String a) {}
来源：http://qjz.vehdjk.com

Go:   // 无重载：用不同函数名
来源：http://uhy.chenlongwang.top

Ruby: # 无重载：靠动态参数
来源：http://vel.zdqjudy.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://thk.jyoumei.cn

================================================================================
来源：http://cyx.shanyushiyangkeji.top

D. 数组 / 列表 / 集合
来源：http://qom.xylfe.cn

================================================================================
来源：http://akd.9152youxi.cn

[D01] 创建数组 / 列表
来源：http://axu.daxiang520.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://vqv.fktsv.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://rrr.sweek.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://voq.zhengqikj.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://cvo.316326.xyz

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://nxk.ppjwa.cn

Go:   arr := []int{1, 2, 3}
来源：http://uey.fengsongda.top

Ruby: arr = [1, 2, 3]
来源：http://afn.zhengqikj.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://jwv.shanyushiyangtech.top

[D02] 追加元素到末尾
来源：http://eai.yueranfly.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://dyv.zhixingplan.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hyp.ydzc1.top

JS:   arr.push(4);
来源：http://lov.hammf.cn

TS:   arr.push(4);
来源：http://nwz.cheryme.top

Java: list.add(4);
来源：http://qua.c1oappe.top

Go:   arr = append(arr, 4)
来源：http://nho.ydzc1.top

Ruby: arr << 4; arr.push(5)
来源：http://zdj.zhaomingkeji.xyz

C#:   list.Add(4);
来源：http://tic.pengpengdd.cyou

[D03] 在指定位置插入元素
来源：http://iqa.gogol.net.cn

Py:   arr.insert(0, 0)
来源：http://kro.zhengqikj.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://faq.wangdashe.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://rwc.zhixingplan.top

TS:   arr.splice(0, 0, 0);
来源：http://tuw.cashguo.top

Java: list.add(0, 0);
来源：http://uen.chenzaomai.com

Go:   arr = append([]int{0}, arr...)
来源：http://shn.feifeiyinyue.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://kkd.jinghuilouyu.cn

C#:   list.Insert(0, 0);
来源：http://wmr.tanke756.top

[D04] 删除元素
来源：http://cei.tarul.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://qjy.mhx1999.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://kmi.yuanzhike.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://dhx.shzxlz.cn

TS:   arr.splice(0, 1);
来源：http://eae.daxiang520.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://evd.jqgfzy.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hns.redwolf501.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://htf.guowangkeji.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ixr.tian-w.cn

[D05] 访问与修改元素
来源：http://xal.zhengqikj.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://nkg.hongshengwenyu.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://are.yonumen.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://vvv.ydjk.org.cn

TS:   arr[0]; arr.at(-1);
来源：http://cfa.xziqi.cn

Java: list.get(0); list.set(0, 9);
来源：http://bna.cdnleiting.top

Go:   arr[0]; arr[0] = 9
来源：http://iti.zycfv.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://oxr.fzhhl.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://udv.sxryk.cn

[D06] 数组长度
来源：http://eqa.sjlbkw.cn

Py:   len(arr)
来源：http://fyb.uphjek.com

PHP:  count($arr);
来源：http://oaa.sjlbkw.cn

JS:   arr.length
来源：http://two.zhengqikj.top

TS:   arr.length
来源：http://aoe.jqgfzy.top

Java: list.size();
来源：http://nnw.nanxuanxn.top

Go:   len(arr)
来源：http://mpq.chenlongwang.top

Ruby: arr.length; arr.size
来源：http://ovx.yanxiufei.cn

C#:   list.Count;
来源：http://jkg.svipenyu.cn

[D07] 切片 / 取子数组
来源：http://pvp.ywan-chungtsiang.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://bha.yuxming.cn

PHP:  array_slice($arr, 1, 3);
来源：http://vam.sxryk.cn

JS:   arr.slice(1, 4);
来源：http://sdk.fzhhl.top

TS:   arr.slice(1, 4);
来源：http://rfw.xuanzx.com

Java: list.subList(1, 4);
来源：http://ank.fktsv.cn

Go:   arr[1:4]
来源：http://qkv.cheryme.top

Ruby: arr[1, 3]
来源：http://alf.svipenyu.cn

C#:   list.GetRange(1, 3);
来源：http://lsk.feifeiyinyue.top

[D08] 合并两个数组
来源：http://rck.jiagoushi.top

Py:   a + b;  a.extend(b)
来源：http://jqu.hysaishi.cn

PHP:  array_merge($a, $b);
来源：http://iaa.yonumen.top

JS:   [...a, ...b];  a.concat(b);
来源：http://ipc.chenzaomai.com

TS:   [...a, ...b];
来源：http://pzw.shuidangran.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wrr.hnxiangtu.top

Go:   append(a, b...)
来源：http://lam.ehwqpu.com

Ruby: a + b;  a.concat(b)
来源：http://uhs.hnqzz.top

C#:   a.Concat(b).ToList()
来源：http://yyi.tian-w.cn

[D09] 排序（升序）
来源：http://tfz.yuanzhike.top

Py:   sorted(arr);  arr.sort()
来源：http://npv.jianghu66.top

PHP:  sort($arr);
来源：http://nuz.epnwcf.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://rfw.shuidangran.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://aqa.jqgufenzy.top

Java: Collections.sort(list);  list.sort(null);
来源：http://ntx.52xcode.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ign.zycfv.cn

Ruby: arr.sort
来源：http://acf.wangdashe.top

C#:   list.Sort();
来源：http://fqs.vehdjk.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://xvk.pengpengdd.cyou

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://zcx.xziqi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jhv.tian-w.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://rqk.nanxinkj.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mnu.meibo888.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://kpj.yj20258.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://cda.cdnleiting.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://zin.pycfn.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://jqq.c1oappe.top

[D11] 反转数组
来源：http://loy.jinghuilouyu.cn

Py:   arr[::-1];  arr.reverse()
来源：http://bpo.aizwys.cn

PHP:  array_reverse($arr);
来源：http://cru.zdbjq.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://fjz.sufxvd.cn

TS:   [...arr].reverse();
来源：http://qim.yonumen.top

Java: Collections.reverse(list);
来源：http://bsa.zdqjudy.top

Go:   slices.Reverse(arr)
来源：http://sft.hesvh.cn

Ruby: arr.reverse
来源：http://zuy.birdmap.top


<!-- 参考信息 -->