代发 wailian999

Py:   # 无标签跳转：抽成函数用 return
来源：http://kwt.daria6918.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://wrr.yuxming.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://vax.shuidangran.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://plo.wangshuangyany.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://cyz.yuanzhike.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://dfc.dianchejie.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://oax.yuanzhike.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://lgm.xuanzx.com

[B13] 判断是否为数字
来源：http://yyo.kuanghao11.cn

Py:   isinstance(x, (int, float))
来源：http://pjt.nwbrower.top

PHP:  is_numeric($x)
来源：http://wbs.nanxinkj.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gol.aizwys.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bah.chenzaomai.com

Java: x instanceof Number
来源：http://ert.jianghu66.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wid.sweek.top

Ruby: x.is_a?(Numeric)
来源：http://qsl.smart0.xyz

C#:   x is int or double or decimal
来源：http://ibv.zhengqikj.top

[B14] 判断值是否在集合内
来源：http://gej.zycfv.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://esa.yuanzhike.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://cnb.shangyingyoupin.top

JS:   [1, 2, 3].includes(x)
来源：http://exl.shzxlz.cn

TS:   [1, 2, 3].includes(x)
来源：http://spg.sweek.top

Java: List.of(1, 2, 3).contains(x)
来源：http://hds.shanyushiyangtech.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://kfp.hnqzz.top

Ruby: [1, 2, 3].include?(x)
来源：http://wod.fktsv.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://uon.wangshuangyany.cn

[B15] 布尔运算与取反
来源：http://seq.dashuyun.cn

Py:   a and b or not c
来源：http://jvp.fanxiaobao.xyz

PHP:  $a && $b || !$c
来源：http://owx.ywan-chungtsiang.top

JS:   a && b || !c
来源：http://idp.sufxvd.cn

TS:   a && b || !c
来源：http://nuq.jinqigufen.top

Java: a && b || !c
来源：http://wqq.tarul.cn

Go:   a && b || !c
来源：http://ere.yvedp.cn

Ruby: a && b || !c
来源：http://ous.gogol.net.cn

C#:   a && b || !c
来源：http://ugd.tianlin.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://ekb.smart0.xyz

Py:   if not data: return
来源：http://omm.wangshuangyany.cn

PHP:  if (!$data) { return; }
来源：http://ebc.hesvh.cn

JS:   if (!data) return;
来源：http://xfb.redwolf501.top

TS:   if (!data) return;
来源：http://uer.feifeiyinyue.top

Java: if (data == null) return;
来源：http://cwg.sxryk.cn

Go:   if data == nil { return }
来源：http://huu.hysaishi.cn

Ruby: return if data.nil?
来源：http://mbl.zhixingplan.top

C#:   if (data == null) return;
来源：http://gsf.gzhubu.top

================================================================================
来源：http://fvp.hnxiangtu.top

C. 函数与作用域
来源：http://npf.jinghuilouyu.cn

================================================================================
来源：http://vql.xylfe.cn

[C01] 定义函数
来源：http://lec.iojbl.cn

Py:   def add(a, b): return a + b
来源：http://jgu.zdqjudy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://snn.zhoulong.xyz

JS:   function add(a, b) { return a + b; }
来源：http://srp.jqgfzy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gzl.cashguo.top

Java: static int add(int a, int b) { return a + b; }
来源：http://xpc.cheryme.top

Go:   func add(a, b int) int { return a + b }
来源：http://mzp.fzhhl.top

Ruby: def add(a, b); a + b; end
来源：http://khv.yongpay.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://kzx.sweek.top

[C02] 默认参数
来源：http://qxu.svipenyu.cn

Py:   def greet(name="World"): return name
来源：http://csq.hongshengwenyu.top

PHP:  function greet($name = "World") { return $name; }
来源：http://chz.gogol.net.cn

JS:   function greet(name = "World") { return name; }
来源：http://nhb.svipenyu.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://erp.zdbjq.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://eik.zhoulong.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ilg.sjlbkw.cn

Ruby: def greet(name = "World") = name
来源：http://qzp.chenlongwang.top

C#:   string Greet(string name = "World") => name;
来源：http://okw.epnwcf.com

[C03] 可变参数
来源：http://dye.dianchejie.cn

Py:   def total(*args): return sum(args)
来源：http://ipa.hywenlv.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://llk.wangdashe.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://yit.zhengqikj.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://sjy.aizwys.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://pym.zhixingplan.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://idv.ydjk.org.cn

Ruby: def total(*nums); nums.sum; end
来源：http://zum.bjfxy.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://vad.tian-w.cn

[C04] 命名参数 / 关键字参数
来源：http://aon.cqqwz.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://lwc.iojbl.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://bvv.kuanghao11.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hgk.hesvh.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://agl.nanxuanxn.top

Java: // 无：用 Builder 模式或 record
来源：http://umi.gotoacloud.top

Go:   // 无：用配置结构体参数
来源：http://xhv.yangfankeji.com

Ruby: f(a: 1, b: 2)
来源：http://bxb.redwolf501.top

C#:   f(a: 1, b: 2)
来源：http://atn.zdqjudy.top

[C05] 返回多个值
来源：http://rcl.aibaodan.cn

Py:   return a, b
来源：http://amb.cashguo.top

PHP:  return [$a, $b];
来源：http://zli.yanxiufei.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ecy.jianghu66.top

TS:   return { a, b };
来源：http://tul.yvedp.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mzr.xuanzx.com

Go:   return a, b
来源：http://hzo.ybcxt.top

Ruby: return a, b
来源：http://fcw.xinyue.icu

C#:   return (a, b);              // ValueTuple
来源：http://web.zycfv.cn

[C06] 匿名函数 / lambda
来源：http://jqu.tanke756.top

Py:   square = lambda x: x * x
来源：http://ptn.nanxinkj.top

PHP:  $square = fn($x) => $x * $x;
来源：http://ajd.ehwqpu.com

JS:   const square = x => x * x;
来源：http://vwg.smart0.xyz

TS:   const square = (x: number): number => x * x;
来源：http://sqq.cdnleiting.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hom.zhiwuduotai.top

Go:   sq := func(x int) int { return x * x }
来源：http://lxc.guannengcc.top

Ruby: square = ->(x) { x * x }
来源：http://qvv.hongshengwenyu.top

C#:   Func<int, int> square = x => x * x;
来源：http://qsp.wangshuangyany.cn

[C07] 把函数作为参数传入
来源：http://jea.hcnkem.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://eek.daria6918.cn

PHP:  array_map("strtoupper", $arr);
来源：http://glz.cashguo.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wzl.zhixingplan.top

TS:   arr.map(String)
来源：http://bbd.wangdashe.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://peg.guowangkeji.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://jrg.yanxiufei.cn

Ruby: arr.map(&:upcase)
来源：http://cxd.chenjidiqi.icu

C#:   arr.Select(s => s.ToUpper())
来源：http://dgf.guowangkeji.top

[C08] 闭包
来源：http://klj.hesvh.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://okw.kuanghao11.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wlk.yvedp.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wup.hammf.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://dpw.yuanzhike.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://nto.tian-w.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://eiv.chenlongwang.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://qrg.xinyue.icu

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://tvh.hfpthk.cn

[C09] 递归
来源：http://uaa.redwolf501.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://nyj.c1oappe.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://crz.ydzc1.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ake.aibaodan.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qvu.wangdashe.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://kro.meibo888.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://cnu.ppjwa.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://heb.sjlbkw.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://onv.pycfn.com

[C10] 变量作用域
来源：http://ioa.shzxlz.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://zuq.sxryk.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://exz.yj20258888.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xlg.xuetiantiany.cn

TS:   同 JS
来源：http://sye.gotoacloud.top

Java: 方法内为块级作用域
来源：http://skj.xuetiantiany.cn

Go:   花括号块级作用域
来源：http://kei.jianghu66.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://yux.sxryk.cn

C#:   块级作用域
来源：http://fmw.fktsv.cn

[C11] 模块导入与导出
来源：http://juw.zhijiandao.cn

Py:   from module import func
来源：http://sdx.yueranfly.top

PHP:  require "file.php";  或 use App\Service;
来源：http://pkj.xziqi.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://bci.aizwys.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://gzx.fehbvm.com

Java: import java.util.List;
来源：http://nin.dianchejie.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://tof.nanxuanxn.top

Ruby: require "json"; require_relative "./util"
来源：http://xzx.tian-w.cn

C#:   using System.Text;
来源：http://obi.smart0.xyz

[C12] 立即执行函数 IIFE
来源：http://hnh.hammf.cn

Py:   (lambda: print("run"))()
来源：http://lrn.ywan-chungtsiang.top

PHP:  (function () { echo "run"; })();
来源：http://yty.yvedp.cn

JS:   (() => { console.log("run"); })();
来源：http://okc.zhengqikj.top

TS:   (() => { console.log("run"); })();
来源：http://zbz.dashuyun.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://nzu.cashguo.top

Go:   func() { fmt.Println("run") }()
来源：http://wwk.c1oappe.top

Ruby: -> { puts "run" }.call
来源：http://pav.sufxvd.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://uil.ywan-chungtsiang.top

[C13] 类型声明 / 类型注解
来源：http://eut.epnwcf.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://vsz.c1oappe.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wuq.fzhhl.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://gjw.jqgufenzy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wqt.yj20258888.top

Java: int add(int a, int b) { return a + b; }
来源：http://jjx.meibo888.top

Go:   func add(a, b int) int
来源：http://chb.hfpthk.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://zyc.ppjwa.cn

C#:   int Add(int a, int b) => a + b;
来源：http://yeb.tian-w.cn

[C14] 泛型函数
来源：http://gmn.nwbrower.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://gxc.chenjidiqi.icu

PHP:  // 无泛型
来源：http://wsp.9152youxi.cn

JS:   // 无泛型
来源：http://lai.zdbjq.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ymd.cucudq.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://cqg.meibo888.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mna.havefunace.top

Ruby: # 无泛型
来源：http://ypp.hnqzz.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hen.ctjpmb.com

[C15] 解构 / 展开参数
来源：http://rrp.tianlin.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://pre.uphjek.com

PHP:  [$a, $b] = $pair;
来源：http://lyq.quarkkingdee.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://fnl.jinqigfzy.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://pgr.jinghuilouyu.cn

Java: // 无解构
来源：http://ghn.shuidangran.top

Go:   // 无解构
来源：http://vey.sjlbkw.cn

Ruby: a, b = pair
来源：http://rsf.xziqi.cn

C#:   var (a, b) = pair;
来源：http://kxr.ctjpmb.com

[C16] 函数 / 方法重载
来源：http://zlc.yongpay.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://rjq.shanyushiyangkeji.top

PHP:  // 无重载
来源：http://ohx.haohaochexian.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://nzg.sjlbkw.cn

TS:   // 用联合类型或重载签名声明
来源：http://rgf.shanyushiyangtech.top

Java: void f(int a) {}  void f(String a) {}
来源：http://mya.ctjpmb.com

Go:   // 无重载：用不同函数名
来源：http://rwi.dianchejie.cn

Ruby: # 无重载：靠动态参数
来源：http://yid.hongshengwenyu.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://tgj.zdbjq.cn

================================================================================
来源：http://irf.epnwcf.com

D. 数组 / 列表 / 集合
来源：http://lfx.cqqwz.cn

================================================================================
来源：http://pca.yangfankeji.com

[D01] 创建数组 / 列表
来源：http://azu.c1oappe.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://cnl.hcnkem.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://sxt.yj20258888.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wzj.yj20258888.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://ghh.yuanzhike.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://caj.chenzaomai.com

Go:   arr := []int{1, 2, 3}
来源：http://uvn.jyoumei.cn

Ruby: arr = [1, 2, 3]
来源：http://eng.yvedp.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://szn.daria6918.cn

[D02] 追加元素到末尾
来源：http://mxm.mhx1999.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://itz.havefunace.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://yan.gaohongyu789.top

JS:   arr.push(4);
来源：http://otg.guowangkeji.top

TS:   arr.push(4);
来源：http://pog.yueranfly.top

Java: list.add(4);
来源：http://eyn.shzxlz.cn

Go:   arr = append(arr, 4)
来源：http://lei.xinyue.icu

Ruby: arr << 4; arr.push(5)
来源：http://jym.zhaomingkeji.xyz

C#:   list.Add(4);
来源：http://pye.shanyushiyangtech.top

[D03] 在指定位置插入元素
来源：http://hio.yj202588.top

Py:   arr.insert(0, 0)
来源：http://ixo.smart0.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://qge.yj202588.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://miu.ctjpmb.com

TS:   arr.splice(0, 0, 0);
来源：http://wts.jinghuilouyu.cn

Java: list.add(0, 0);
来源：http://jgc.hesvh.cn

Go:   arr = append([]int{0}, arr...)
来源：http://qmf.jinqigfzy.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wyv.zycfv.cn

C#:   list.Insert(0, 0);
来源：http://ykh.xuetiantiany.cn

[D04] 删除元素
来源：http://saw.bbcook.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ikt.zhijiandao.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://jri.mhx1999.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://fns.zhaomingkeji.xyz

TS:   arr.splice(0, 1);
来源：http://nee.daria6918.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wbt.dianchejie.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://pxb.zdbjq.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ycs.hongshengwenyu.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://yqq.hongshengwenyu.top

[D05] 访问与修改元素
来源：http://xac.zhixingplan.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://qbe.jyoumei.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wmw.sweek.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://lcr.52xcode.cn

TS:   arr[0]; arr.at(-1);
来源：http://orn.sufxvd.cn

Java: list.get(0); list.set(0, 9);
来源：http://ojk.tanke756.top

Go:   arr[0]; arr[0] = 9
来源：http://yqm.0kj1m.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://jcu.svipenyu.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://gbu.jiagoushi.top

[D06] 数组长度
来源：http://aov.nanxuanxn.top

Py:   len(arr)
来源：http://trz.hysaishi.cn

PHP:  count($arr);
来源：http://evh.havefunace.top

JS:   arr.length
来源：http://sjk.yvedp.cn

TS:   arr.length
来源：http://cio.shzxlz.cn

Java: list.size();
来源：http://jlo.tanke756.top

Go:   len(arr)
来源：http://ujv.tarul.cn

Ruby: arr.length; arr.size
来源：http://wdn.jinqigfzy.top

C#:   list.Count;
来源：http://hkc.guowangkeji.top

[D07] 切片 / 取子数组
来源：http://pqk.tianlin.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://gsb.fzhhl.top

PHP:  array_slice($arr, 1, 3);
来源：http://qmj.svipenyu.cn

JS:   arr.slice(1, 4);
来源：http://ojt.yfazqb.com

TS:   arr.slice(1, 4);
来源：http://thm.feifeiyinyue.top

Java: list.subList(1, 4);
来源：http://fca.jinqigufen.top

Go:   arr[1:4]
来源：http://wmf.bbcook.cn

Ruby: arr[1, 3]
来源：http://quz.shuidangran.top

C#:   list.GetRange(1, 3);
来源：http://sds.gogol.net.cn

[D08] 合并两个数组
来源：http://glz.andypj.xyz

Py:   a + b;  a.extend(b)
来源：http://cxt.aibaodan.cn

PHP:  array_merge($a, $b);
来源：http://eiu.jyoumei.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://rwi.pengpengdd.cyou

TS:   [...a, ...b];
来源：http://pub.ybcxt.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://tjs.zhongyouzk.top

Go:   append(a, b...)
来源：http://xpn.ehwqpu.com

Ruby: a + b;  a.concat(b)
来源：http://xac.andypj.xyz

C#:   a.Concat(b).ToList()
来源：http://fre.9152youxi.cn

[D09] 排序（升序）
来源：http://ruk.pycfn.com

Py:   sorted(arr);  arr.sort()
来源：http://jhu.pycfn.com

PHP:  sort($arr);
来源：http://xff.jianghu66.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://nwr.andypj.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://nil.jyoumei.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://dhg.gotoacloud.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://jrk.aibaodan.cn

Ruby: arr.sort
来源：http://soh.chenzaomai.com

C#:   list.Sort();
来源：http://dkx.52xcode.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://tce.hywenlv.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://nqa.hesvh.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://che.xuetiantiany.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://qub.yanxiufei.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://daz.kuanghao11.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://nso.smart0.xyz

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wop.0kj1m.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://bor.hcnkem.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qth.zhongyouzk.top

[D11] 反转数组
来源：http://trg.zdqjudy.top

Py:   arr[::-1];  arr.reverse()
来源：http://ptm.sweek.top

PHP:  array_reverse($arr);
来源：http://ndm.hysaishi.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://jto.haohaochexian.top

TS:   [...arr].reverse();
来源：http://myh.sxryk.cn

Java: Collections.reverse(list);
来源：http://lqh.daria6918.cn

Go:   slices.Reverse(arr)
来源：http://omn.nanxuanxn.top

Ruby: arr.reverse
来源：http://cck.jianghu66.top

C#:   list.Reverse();
来源：http://mmn.ydjk.org.cn

[D12] 查找元素下标
来源：http://jss.zhijiandao.cn

Py:   arr.index(x);  x in arr
来源：http://cvm.tarul.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://zgl.zdbjq.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dio.nwbrower.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://chl.xziqi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hbe.smart0.xyz

Go:   slices.Index(arr, x)
来源：http://fxe.cdnleiting.top


<!-- 参考信息 -->