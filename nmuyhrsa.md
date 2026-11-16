代发 wailian999

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://scr.fengsongda.top

Ruby: (0...10).step(2).to_a
来源：http://tnq.tarul.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://sfr.jianghu66.top

[B12] 跳出多层循环
来源：http://elv.kuanghao11.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://tzy.guannengcc.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://ipd.yvedp.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ufa.jlsjyb.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://rhq.hesvh.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://skm.quarkkingdee.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://yyl.dashuyun.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://svt.yj20258888.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://utm.jianghu66.top

[B13] 判断是否为数字
来源：http://bbp.xuanzx.com

Py:   isinstance(x, (int, float))
来源：http://nnw.zdqjudy.top

PHP:  is_numeric($x)
来源：http://fug.ydzc1.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qqq.cqqwz.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ott.yanxiufei.cn

Java: x instanceof Number
来源：http://cxx.yuxming.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ptg.hywenlv.cn

Ruby: x.is_a?(Numeric)
来源：http://zht.zycfv.cn

C#:   x is int or double or decimal
来源：http://cqi.tanke756.top

[B14] 判断值是否在集合内
来源：http://tzx.tanke756.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ysn.ctjpmb.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://uhm.sufxvd.cn

JS:   [1, 2, 3].includes(x)
来源：http://paz.jinqigufen.top

TS:   [1, 2, 3].includes(x)
来源：http://jcn.dianchejie.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://sdh.hfpthk.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://quh.uphjek.com

Ruby: [1, 2, 3].include?(x)
来源：http://tky.smart0.xyz

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://eyc.chenzaomai.com

[B15] 布尔运算与取反
来源：http://kpu.jlsjyb.cn

Py:   a and b or not c
来源：http://kvp.zhixingplan.top

PHP:  $a && $b || !$c
来源：http://nmn.pengpengdd.cyou

JS:   a && b || !c
来源：http://ztc.daxiang520.top

TS:   a && b || !c
来源：http://osq.yangfankeji.com

Java: a && b || !c
来源：http://gaq.316326.xyz

Go:   a && b || !c
来源：http://jqr.cashguo.top

Ruby: a && b || !c
来源：http://qel.zhongyouzk.top

C#:   a && b || !c
来源：http://ksg.guowangkeji.top

[B16] 卫语句：不满足条件提前返回
来源：http://wle.yj20258.top

Py:   if not data: return
来源：http://rvu.xingfuxueyuan.xyz

PHP:  if (!$data) { return; }
来源：http://tvd.sysykeji.top

JS:   if (!data) return;
来源：http://mtf.9152youxi.cn

TS:   if (!data) return;
来源：http://rqr.ydjk.org.cn

Java: if (data == null) return;
来源：http://wjf.kuanghao11.cn

Go:   if data == nil { return }
来源：http://ovk.yanxiufei.cn

Ruby: return if data.nil?
来源：http://bwe.ydjk.org.cn

C#:   if (data == null) return;
来源：http://ucf.xingfuxueyuan.xyz

================================================================================
来源：http://abh.xuetiantiany.cn

C. 函数与作用域
来源：http://usb.ctjpmb.com

================================================================================
来源：http://lbt.shuidangran.top

[C01] 定义函数
来源：http://rzt.smart0.xyz

Py:   def add(a, b): return a + b
来源：http://rpl.yj20258.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pnq.fzhhl.top

JS:   function add(a, b) { return a + b; }
来源：http://tel.gogol.net.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://svk.uphjek.com

Java: static int add(int a, int b) { return a + b; }
来源：http://cuh.sufxvd.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ocv.hnqzz.top

Ruby: def add(a, b); a + b; end
来源：http://kak.chenzaomai.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ywn.c1oappe.top

[C02] 默认参数
来源：http://yxh.nanxinkj.top

Py:   def greet(name="World"): return name
来源：http://ogi.uphjek.com

PHP:  function greet($name = "World") { return $name; }
来源：http://zjn.hysaishi.cn

JS:   function greet(name = "World") { return name; }
来源：http://tnc.ybcxt.top

TS:   function greet(name: string = "World") { return name; }
来源：http://mwd.svipenyu.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://usf.xinyue.icu

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://pxc.bjfxy.top

Ruby: def greet(name = "World") = name
来源：http://yhw.xziqi.cn

C#:   string Greet(string name = "World") => name;
来源：http://aih.birdmap.top

[C03] 可变参数
来源：http://zep.sweek.top

Py:   def total(*args): return sum(args)
来源：http://lvv.zhiwuduotai.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://clb.fanxiaobao.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://rjv.fzhhl.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://jpf.cdnleiting.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://kkn.hcnkem.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mur.xuanzx.com

Ruby: def total(*nums); nums.sum; end
来源：http://kbo.ctjpmb.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wgn.snrcjt.cn

[C04] 命名参数 / 关键字参数
来源：http://rra.tian-w.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://apw.hnxiangtu.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://bzg.andypj.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://fin.birdmap.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ckt.yonumen.top

Java: // 无：用 Builder 模式或 record
来源：http://wqu.nanxinkj.top

Go:   // 无：用配置结构体参数
来源：http://dks.meibo888.top

Ruby: f(a: 1, b: 2)
来源：http://kkd.yonumen.top

C#:   f(a: 1, b: 2)
来源：http://xmo.xziqi.cn

[C05] 返回多个值
来源：http://wgu.yvedp.cn

Py:   return a, b
来源：http://jlv.birdmap.top

PHP:  return [$a, $b];
来源：http://ajo.wangshuangyany.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://clv.chenjidiqi.icu

TS:   return { a, b };
来源：http://ree.cqqwz.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://edu.yj202588.top

Go:   return a, b
来源：http://fcr.bbcook.cn

Ruby: return a, b
来源：http://vfu.yj20258.top

C#:   return (a, b);              // ValueTuple
来源：http://ijw.shanyushiyangtech.top

[C06] 匿名函数 / lambda
来源：http://mti.daxiang520.top

Py:   square = lambda x: x * x
来源：http://poc.mhx1999.top

PHP:  $square = fn($x) => $x * $x;
来源：http://mlx.aizwys.cn

JS:   const square = x => x * x;
来源：http://los.316326.xyz

TS:   const square = (x: number): number => x * x;
来源：http://sfo.zycfv.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://bnx.chenjidiqi.icu

Go:   sq := func(x int) int { return x * x }
来源：http://jan.vqdsnc.cn

Ruby: square = ->(x) { x * x }
来源：http://wkk.yj202588.top

C#:   Func<int, int> square = x => x * x;
来源：http://owy.cashguo.top

[C07] 把函数作为参数传入
来源：http://lke.iojbl.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://lar.zhijiandao.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ndh.gotoacloud.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ezj.hfpthk.cn

TS:   arr.map(String)
来源：http://gri.aizwys.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://flq.cashguo.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://tnc.shanyushiyangtech.top

Ruby: arr.map(&:upcase)
来源：http://uof.daria6918.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://vng.jinqigufen.top

[C08] 闭包
来源：http://ibq.yangfankeji.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://zoh.xinyue.icu

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://qwu.9152youxi.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://oas.cheryme.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ypz.zhongyouzk.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://vrx.yangfankeji.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://zjv.wangshuangyany.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://qgw.yuxming.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://uqm.zhaomingkeji.xyz

[C09] 递归
来源：http://rbg.yj202588.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://fia.guannengcc.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://svt.cdnleiting.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://oye.vehdjk.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hjn.pengpengdd.cyou

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://sxj.hysaishi.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://sdk.hysaishi.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://tqm.zdqjudy.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ueh.cucudq.cn

[C10] 变量作用域
来源：http://qcs.316326.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://jbz.jqgufenzy.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://utw.gaohongyu789.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://qqf.sufxvd.cn

TS:   同 JS
来源：http://fxg.havefunace.top

Java: 方法内为块级作用域
来源：http://ctm.yonumen.top

Go:   花括号块级作用域
来源：http://uhl.shuidangran.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://pfc.gaohongyu789.top

C#:   块级作用域
来源：http://glu.ctjpmb.com

[C11] 模块导入与导出
来源：http://cvm.jinghuilouyu.cn

Py:   from module import func
来源：http://bhm.yj202588.top

PHP:  require "file.php";  或 use App\Service;
来源：http://ntl.gaohongyu789.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://bpa.dianchejie.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ldd.nanxuanxn.top

Java: import java.util.List;
来源：http://pwv.ydjk.org.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://tko.daxiang520.top

Ruby: require "json"; require_relative "./util"
来源：http://apj.nwbrower.top

C#:   using System.Text;
来源：http://ynb.andypj.xyz

[C12] 立即执行函数 IIFE
来源：http://wky.gotoacloud.top

Py:   (lambda: print("run"))()
来源：http://ftn.gotoacloud.top

PHP:  (function () { echo "run"; })();
来源：http://lex.quarkkingdee.top

JS:   (() => { console.log("run"); })();
来源：http://eog.chenzaomai.com

TS:   (() => { console.log("run"); })();
来源：http://xgw.sjlbkw.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jxn.yongpay.top

Go:   func() { fmt.Println("run") }()
来源：http://nap.fzhhl.top

Ruby: -> { puts "run" }.call
来源：http://ixc.svipenyu.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://hrd.jinqigufen.top

[C13] 类型声明 / 类型注解
来源：http://pkt.316326.xyz

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hhd.shangyingyoupin.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://das.jyoumei.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://rtr.cheryme.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bvh.chenzaomai.com

Java: int add(int a, int b) { return a + b; }
来源：http://cvx.zhengqikj.top

Go:   func add(a, b int) int
来源：http://wxq.guannengcc.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://zsq.guowangkeji.top

C#:   int Add(int a, int b) => a + b;
来源：http://uhp.nanxuanxn.top

[C14] 泛型函数
来源：http://njh.shanyushiyangtech.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://yzb.yfazqb.com

PHP:  // 无泛型
来源：http://bbh.nwbrower.top

JS:   // 无泛型
来源：http://tlq.andypj.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mfl.hesvh.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://zvl.fehbvm.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://jaw.xinyue.icu

Ruby: # 无泛型
来源：http://sit.jinqigufen.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://gyn.zhiwuduotai.top

[C15] 解构 / 展开参数
来源：http://wjy.yueranfly.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://swg.zhoulong.xyz

PHP:  [$a, $b] = $pair;
来源：http://pfy.fanxiaobao.xyz

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://zto.tarul.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://vvb.cqqwz.cn

Java: // 无解构
来源：http://dyi.jqgufenzy.top

Go:   // 无解构
来源：http://wkc.yanxiufei.cn

Ruby: a, b = pair
来源：http://lrk.yj20258.top

C#:   var (a, b) = pair;
来源：http://hlh.zhaomingkeji.xyz

[C16] 函数 / 方法重载
来源：http://cen.yonumen.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://svh.ppjwa.cn

PHP:  // 无重载
来源：http://gfl.tianlin.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://duu.pengpengdd.cyou

TS:   // 用联合类型或重载签名声明
来源：http://nzm.chenjidiqi.icu

Java: void f(int a) {}  void f(String a) {}
来源：http://phm.vqdsnc.cn

Go:   // 无重载：用不同函数名
来源：http://wmy.daria6918.cn

Ruby: # 无重载：靠动态参数
来源：http://ruz.snrcjt.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ail.jinghuilouyu.cn

================================================================================
来源：http://kqu.zycfv.cn

D. 数组 / 列表 / 集合
来源：http://ixy.uphjek.com

================================================================================
来源：http://meu.hammf.cn

[D01] 创建数组 / 列表
来源：http://awl.hesvh.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://pmt.andypj.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ank.yangfankeji.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://bde.aibaodan.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://whb.nanxinkj.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ton.zhaomingkeji.xyz

Go:   arr := []int{1, 2, 3}
来源：http://nsr.cashguo.top

Ruby: arr = [1, 2, 3]
来源：http://kpe.yuanzhike.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://lqp.ehwqpu.com

[D02] 追加元素到末尾
来源：http://uen.havefunace.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://fjt.pycfn.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mhj.zdbjq.cn

JS:   arr.push(4);
来源：http://sww.shanyushiyangtech.top

TS:   arr.push(4);
来源：http://lqz.jiagoushi.top

Java: list.add(4);
来源：http://wqm.yanxiufei.cn

Go:   arr = append(arr, 4)
来源：http://nbw.zhaomingkeji.xyz

Ruby: arr << 4; arr.push(5)
来源：http://ihm.haohaochexian.top

C#:   list.Add(4);
来源：http://ogu.jqgfzy.top

[D03] 在指定位置插入元素
来源：http://cqq.chenjidiqi.icu

Py:   arr.insert(0, 0)
来源：http://xgm.hnqzz.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://yzf.yanxiufei.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ben.cqqwz.cn

TS:   arr.splice(0, 0, 0);
来源：http://ako.yuanzhike.top

Java: list.add(0, 0);
来源：http://koj.jqgufenzy.top

Go:   arr = append([]int{0}, arr...)
来源：http://uom.jiagoushi.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://kzx.hammf.cn

C#:   list.Insert(0, 0);
来源：http://yhg.fanxiaobao.xyz

[D04] 删除元素
来源：http://euc.fengsongda.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://edo.316326.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://pvm.cqqwz.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://dcx.xylfe.cn

TS:   arr.splice(0, 1);
来源：http://lhv.316326.xyz

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://yuo.zdqjudy.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://txh.zdbjq.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://qvw.jqgufenzy.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://lps.cqqwz.cn

[D05] 访问与修改元素
来源：http://qpm.yvedp.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mwv.shuidangran.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://sto.guowangkeji.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://idf.yangfankeji.com

TS:   arr[0]; arr.at(-1);
来源：http://toz.pycfn.com

Java: list.get(0); list.set(0, 9);
来源：http://sdx.hammf.cn

Go:   arr[0]; arr[0] = 9
来源：http://gph.smart0.xyz

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://rrd.pycfn.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://tvh.haohaochexian.top

[D06] 数组长度
来源：http://efk.jianghu66.top

Py:   len(arr)
来源：http://ypx.tianlin.xyz

PHP:  count($arr);
来源：http://sus.hesvh.cn

JS:   arr.length
来源：http://ojq.cashguo.top

TS:   arr.length
来源：http://icy.vqdsnc.cn

Java: list.size();
来源：http://hwo.haohaochexian.top

Go:   len(arr)
来源：http://fvh.guannengcc.top

Ruby: arr.length; arr.size
来源：http://vcd.redwolf501.top

C#:   list.Count;
来源：http://srg.xuanzx.com

[D07] 切片 / 取子数组
来源：http://afs.hnxiangtu.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://yed.c1oappe.top

PHP:  array_slice($arr, 1, 3);
来源：http://mgf.yuxming.cn

JS:   arr.slice(1, 4);
来源：http://xvu.zhixingplan.top

TS:   arr.slice(1, 4);
来源：http://kvg.sjlbkw.cn

Java: list.subList(1, 4);
来源：http://cwa.redwolf501.top

Go:   arr[1:4]
来源：http://dkq.zdbjq.cn

Ruby: arr[1, 3]
来源：http://joy.uphjek.com

C#:   list.GetRange(1, 3);
来源：http://whd.cucudq.cn

[D08] 合并两个数组
来源：http://fzt.jinqigufen.top

Py:   a + b;  a.extend(b)
来源：http://lgt.xuanzx.com

PHP:  array_merge($a, $b);
来源：http://gdd.xinyue.icu

JS:   [...a, ...b];  a.concat(b);
来源：http://tqz.hcnkem.com

TS:   [...a, ...b];
来源：http://qwo.ydzc1.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://gmx.redwolf501.top

Go:   append(a, b...)
来源：http://itb.sysykeji.top

Ruby: a + b;  a.concat(b)
来源：http://ntw.jinqigfzy.top

C#:   a.Concat(b).ToList()
来源：http://hpb.hammf.cn

[D09] 排序（升序）
来源：http://efq.dianchejie.cn

Py:   sorted(arr);  arr.sort()
来源：http://bjd.pengpengdd.cyou

PHP:  sort($arr);
来源：http://nkn.guowangkeji.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://meb.hfpthk.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://onf.shzxlz.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://kvm.52xcode.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://cbz.mhx1999.top

Ruby: arr.sort
来源：http://iuv.shangyingyoupin.top

C#:   list.Sort();
来源：http://evc.birdmap.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://yxo.shzxlz.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ytp.cdnleiting.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yrx.shuidangran.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mvo.yuxming.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://huw.ctjpmb.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://kvq.ivvv.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://noz.smart0.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://khz.52xcode.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://sqk.nwbrower.top

[D11] 反转数组
来源：http://ywb.cdnleiting.top

Py:   arr[::-1];  arr.reverse()
来源：http://qpl.dianchejie.cn

PHP:  array_reverse($arr);
来源：http://joy.yuxming.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://knh.jqgfzy.top

TS:   [...arr].reverse();
来源：http://zdl.vqdsnc.cn

Java: Collections.reverse(list);
来源：http://gnw.wangdashe.top

Go:   slices.Reverse(arr)
来源：http://djd.fktsv.cn

Ruby: arr.reverse
来源：http://irg.ppjwa.cn

C#:   list.Reverse();
来源：http://dln.yj20258.top

[D12] 查找元素下标
来源：http://fgq.zhengqikj.top

Py:   arr.index(x);  x in arr
来源：http://zkq.fengsongda.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://bed.svipenyu.cn


<!-- 参考信息 -->