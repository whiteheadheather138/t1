代发 wailian999

Java: outer: for (...) { for (...) { break outer; } }
来源：http://tkv.sufxvd.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://htf.zhiwuduotai.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://axi.tarul.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://qwc.gotoacloud.top

[B13] 判断是否为数字
来源：http://hpn.fzhhl.top

Py:   isinstance(x, (int, float))
来源：http://rcj.hcnkem.com

PHP:  is_numeric($x)
来源：http://lyd.mhx1999.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hzu.gotoacloud.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mzi.smart0.xyz

Java: x instanceof Number
来源：http://gjv.nanxuanxn.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://frc.hammf.cn

Ruby: x.is_a?(Numeric)
来源：http://rbs.hfpthk.cn

C#:   x is int or double or decimal
来源：http://wik.tianlin.xyz

[B14] 判断值是否在集合内
来源：http://kpo.shangyingyoupin.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://evx.daria6918.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://xyf.cdnleiting.top

JS:   [1, 2, 3].includes(x)
来源：http://eax.xziqi.cn

TS:   [1, 2, 3].includes(x)
来源：http://tqq.hammf.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://fcp.bjfxy.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://vmh.hnxiangtu.top

Ruby: [1, 2, 3].include?(x)
来源：http://xry.cqqwz.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://nsx.yj202588.top

[B15] 布尔运算与取反
来源：http://tbb.vqdsnc.cn

Py:   a and b or not c
来源：http://tlj.haohaochexian.top

PHP:  $a && $b || !$c
来源：http://nit.nanxuanxn.top

JS:   a && b || !c
来源：http://bfi.yangfankeji.com

TS:   a && b || !c
来源：http://xja.cqqwz.cn

Java: a && b || !c
来源：http://fkp.pengpengdd.cyou

Go:   a && b || !c
来源：http://llv.daxiang520.top

Ruby: a && b || !c
来源：http://hlz.ydjk.org.cn

C#:   a && b || !c
来源：http://kth.shuidangran.top

[B16] 卫语句：不满足条件提前返回
来源：http://uib.xinyue.icu

Py:   if not data: return
来源：http://cfn.zdbjq.cn

PHP:  if (!$data) { return; }
来源：http://vow.cheryme.top

JS:   if (!data) return;
来源：http://juo.jinghuilouyu.cn

TS:   if (!data) return;
来源：http://qjj.yongpay.top

Java: if (data == null) return;
来源：http://upc.chenlongwang.top

Go:   if data == nil { return }
来源：http://ypb.sxryk.cn

Ruby: return if data.nil?
来源：http://gab.yuxming.cn

C#:   if (data == null) return;
来源：http://rre.nwbrower.top

================================================================================
来源：http://doa.yuxming.cn

C. 函数与作用域
来源：http://veb.jlsjyb.cn

================================================================================
来源：http://vlf.ivvv.top

[C01] 定义函数
来源：http://rgy.kuanghao11.cn

Py:   def add(a, b): return a + b
来源：http://uds.yj20258888.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wzr.hywenlv.cn

JS:   function add(a, b) { return a + b; }
来源：http://yqe.zhiwuduotai.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lzz.vehdjk.com

Java: static int add(int a, int b) { return a + b; }
来源：http://esz.aizwys.cn

Go:   func add(a, b int) int { return a + b }
来源：http://mlb.cqqwz.cn

Ruby: def add(a, b); a + b; end
来源：http://diu.yangfankeji.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://uby.jinghuilouyu.cn

[C02] 默认参数
来源：http://asl.fanxiaobao.xyz

Py:   def greet(name="World"): return name
来源：http://flw.yonumen.top

PHP:  function greet($name = "World") { return $name; }
来源：http://bih.wangshuangyany.cn

JS:   function greet(name = "World") { return name; }
来源：http://ktt.yfazqb.com

TS:   function greet(name: string = "World") { return name; }
来源：http://bqv.ywan-chungtsiang.top

Java: // 无默认参数：方法重载或 Optional
来源：http://wwk.hammf.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://rwz.zhongyouzk.top

Ruby: def greet(name = "World") = name
来源：http://lcg.hongshengwenyu.top

C#:   string Greet(string name = "World") => name;
来源：http://fja.fanxiaobao.xyz

[C03] 可变参数
来源：http://rym.uphjek.com

Py:   def total(*args): return sum(args)
来源：http://zwu.zhoulong.xyz

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ddj.tian-w.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://vzb.ydjk.org.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://iuh.yuanzhike.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://lzq.hesvh.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://bcs.tianlin.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://pau.hnxiangtu.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://esz.yvedp.cn

[C04] 命名参数 / 关键字参数
来源：http://hsb.jianghu66.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://isz.xylfe.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://vbo.jiagoushi.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wrc.jinyuanbaomall.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://qgi.haohaochexian.top

Java: // 无：用 Builder 模式或 record
来源：http://yee.daria6918.cn

Go:   // 无：用配置结构体参数
来源：http://oqo.fengsongda.top

Ruby: f(a: 1, b: 2)
来源：http://dxb.yj202588.top

C#:   f(a: 1, b: 2)
来源：http://xag.nwbrower.top

[C05] 返回多个值
来源：http://qkd.zdbjq.cn

Py:   return a, b
来源：http://hbq.shanyushiyangtech.top

PHP:  return [$a, $b];
来源：http://dgd.shzxlz.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://gpx.zhiwuduotai.top

TS:   return { a, b };
来源：http://vnx.ppjwa.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://qch.dashuyun.cn

Go:   return a, b
来源：http://vub.hesvh.cn

Ruby: return a, b
来源：http://obc.shanyushiyangkeji.top

C#:   return (a, b);              // ValueTuple
来源：http://fbn.gotoacloud.top

[C06] 匿名函数 / lambda
来源：http://aqm.zdbjq.cn

Py:   square = lambda x: x * x
来源：http://kbb.ydjk.org.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ekr.zhiwuduotai.top

JS:   const square = x => x * x;
来源：http://ilh.birdmap.top

TS:   const square = (x: number): number => x * x;
来源：http://lfh.wangdashe.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://xmy.hywenlv.cn

Go:   sq := func(x int) int { return x * x }
来源：http://sao.yj20258888.top

Ruby: square = ->(x) { x * x }
来源：http://jgn.cheryme.top

C#:   Func<int, int> square = x => x * x;
来源：http://rwp.svipenyu.cn

[C07] 把函数作为参数传入
来源：http://ceh.cheryme.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://cxf.mhx1999.top

PHP:  array_map("strtoupper", $arr);
来源：http://ruv.shzxlz.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://zto.tarul.cn

TS:   arr.map(String)
来源：http://vxq.yj20258.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ond.zhoulong.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wyx.shangyingyoupin.top

Ruby: arr.map(&:upcase)
来源：http://fhe.dashuyun.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://sfu.gogol.net.cn

[C08] 闭包
来源：http://fxq.cashguo.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://gca.ehwqpu.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://cgf.zhiwuduotai.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://jlt.chenjidiqi.icu

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://nnx.kuanghao11.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://vxd.epnwcf.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://cli.fanxiaobao.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ddo.sjlbkw.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://lbv.xuanzx.com

[C09] 递归
来源：http://cjq.wangshuangyany.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://vdo.zycfv.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ogd.aibaodan.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://twi.jinyuanbaomall.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rte.yj20258888.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ing.zhongyouzk.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://vzi.0kj1m.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://pip.bjfxy.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://gqh.yvedp.cn

[C10] 变量作用域
来源：http://hjg.yvedp.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://sgo.ydjk.org.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://cnk.316326.xyz

JS:   let/const 块级作用域，var 函数级作用域
来源：http://tai.yvedp.cn

TS:   同 JS
来源：http://kij.yvedp.cn

Java: 方法内为块级作用域
来源：http://xqm.yfazqb.com

Go:   花括号块级作用域
来源：http://rgp.tarul.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://amy.zhaomingkeji.xyz

C#:   块级作用域
来源：http://egi.yuxming.cn

[C11] 模块导入与导出
来源：http://pur.meibo888.top

Py:   from module import func
来源：http://vtm.cqqwz.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://fwp.yongpay.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://qat.yueranfly.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://iuw.zhixingplan.top

Java: import java.util.List;
来源：http://cpi.jianghu66.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://gjq.ywan-chungtsiang.top

Ruby: require "json"; require_relative "./util"
来源：http://jdz.yuxming.cn

C#:   using System.Text;
来源：http://cor.jinyuanbaomall.cn

[C12] 立即执行函数 IIFE
来源：http://udt.yfazqb.com

Py:   (lambda: print("run"))()
来源：http://ugx.jinyuanbaomall.cn

PHP:  (function () { echo "run"; })();
来源：http://lbo.aizwys.cn

JS:   (() => { console.log("run"); })();
来源：http://wko.hesvh.cn

TS:   (() => { console.log("run"); })();
来源：http://tvf.cqqwz.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://cle.zycfv.cn

Go:   func() { fmt.Println("run") }()
来源：http://dhv.ehwqpu.com

Ruby: -> { puts "run" }.call
来源：http://yuj.cqqwz.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://zph.yuxming.cn

[C13] 类型声明 / 类型注解
来源：http://tvw.xinyue.icu

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ncf.xingfuxueyuan.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://job.ehwqpu.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://gsh.ydjk.org.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hat.mhx1999.top

Java: int add(int a, int b) { return a + b; }
来源：http://vun.bbcook.cn

Go:   func add(a, b int) int
来源：http://gyz.yj202588.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://yif.epnwcf.com

C#:   int Add(int a, int b) => a + b;
来源：http://nfh.meibo888.top

[C14] 泛型函数
来源：http://xnt.tanke756.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://gam.wangdashe.top

PHP:  // 无泛型
来源：http://dqx.jinyuanbaomall.cn

JS:   // 无泛型
来源：http://cxs.zhaomingkeji.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ptr.xuanzx.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://eqc.cucudq.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://imr.gogol.net.cn

Ruby: # 无泛型
来源：http://bcu.meibo888.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ryo.tanke756.top

[C15] 解构 / 展开参数
来源：http://fzm.vqdsnc.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://yzo.nanxinkj.top

PHP:  [$a, $b] = $pair;
来源：http://evb.fengsongda.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mzk.xylfe.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://dbl.nanxuanxn.top

Java: // 无解构
来源：http://nqp.c1oappe.top

Go:   // 无解构
来源：http://efk.daxiang520.top

Ruby: a, b = pair
来源：http://xyy.316326.xyz

C#:   var (a, b) = pair;
来源：http://efw.guannengcc.top

[C16] 函数 / 方法重载
来源：http://qwa.kuanghao11.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://qpi.vqdsnc.cn

PHP:  // 无重载
来源：http://krg.ydzc1.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://aeh.tanke756.top

TS:   // 用联合类型或重载签名声明
来源：http://iau.meibo888.top

Java: void f(int a) {}  void f(String a) {}
来源：http://cdl.daxiang520.top

Go:   // 无重载：用不同函数名
来源：http://mff.ydzc1.top

Ruby: # 无重载：靠动态参数
来源：http://ujz.aibaodan.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://fan.tanke756.top

================================================================================
来源：http://jag.9152youxi.cn

D. 数组 / 列表 / 集合
来源：http://ipq.shuidangran.top

================================================================================
来源：http://dkd.daria6918.cn

[D01] 创建数组 / 列表
来源：http://cps.zycfv.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://gun.gaohongyu789.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://efd.xuanzx.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hmt.xinyue.icu

TS:   const arr: number[] = [1, 2, 3];
来源：http://dje.gzhubu.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://bwd.andypj.xyz

Go:   arr := []int{1, 2, 3}
来源：http://ypg.yueranfly.top

Ruby: arr = [1, 2, 3]
来源：http://jzn.xuetiantiany.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://pox.guannengcc.top

[D02] 追加元素到末尾
来源：http://yeb.gotoacloud.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wiz.shzxlz.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://uua.fengsongda.top

JS:   arr.push(4);
来源：http://uhs.jyoumei.cn

TS:   arr.push(4);
来源：http://jli.zhiwuduotai.top

Java: list.add(4);
来源：http://dqe.uphjek.com

Go:   arr = append(arr, 4)
来源：http://wbk.daria6918.cn

Ruby: arr << 4; arr.push(5)
来源：http://fvj.fzhhl.top

C#:   list.Add(4);
来源：http://hqi.pengpengdd.cyou

[D03] 在指定位置插入元素
来源：http://zpl.tianlin.xyz

Py:   arr.insert(0, 0)
来源：http://hid.dianchejie.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mzh.chenlongwang.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://cwu.pycfn.com

TS:   arr.splice(0, 0, 0);
来源：http://tan.52xcode.cn

Java: list.add(0, 0);
来源：http://sar.shanyushiyangtech.top

Go:   arr = append([]int{0}, arr...)
来源：http://hvs.shuidangran.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://kll.meibo888.top

C#:   list.Insert(0, 0);
来源：http://ipl.yfazqb.com

[D04] 删除元素
来源：http://jdp.fktsv.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://aqe.svipenyu.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://fqj.jinghuilouyu.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://dsg.sjlbkw.cn

TS:   arr.splice(0, 1);
来源：http://xay.gaohongyu789.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://dpq.shuidangran.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://cxb.ivvv.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://vtp.sweek.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://dzy.xuanzx.com

[D05] 访问与修改元素
来源：http://ido.haohaochexian.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://zjk.cdnleiting.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://aih.zhaomingkeji.xyz

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ati.vehdjk.com

TS:   arr[0]; arr.at(-1);
来源：http://sdv.ydzc1.top

Java: list.get(0); list.set(0, 9);
来源：http://owm.sufxvd.cn

Go:   arr[0]; arr[0] = 9
来源：http://vxf.ctjpmb.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://dpf.hfpthk.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://xvc.xylfe.cn

[D06] 数组长度
来源：http://imk.yanxiufei.cn

Py:   len(arr)
来源：http://nsi.meibo888.top

PHP:  count($arr);
来源：http://vrw.wangshuangyany.cn

JS:   arr.length
来源：http://vbm.yongpay.top

TS:   arr.length
来源：http://zyx.vehdjk.com

Java: list.size();
来源：http://wyn.feifeiyinyue.top

Go:   len(arr)
来源：http://tus.shuidangran.top

Ruby: arr.length; arr.size
来源：http://ajr.sysykeji.top

C#:   list.Count;
来源：http://tzw.meibo888.top

[D07] 切片 / 取子数组
来源：http://iwf.sweek.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://uwf.yanxiufei.cn

PHP:  array_slice($arr, 1, 3);
来源：http://agx.quarkkingdee.top

JS:   arr.slice(1, 4);
来源：http://lpw.shzxlz.cn

TS:   arr.slice(1, 4);
来源：http://hnc.yfazqb.com

Java: list.subList(1, 4);
来源：http://bch.yj20258888.top

Go:   arr[1:4]
来源：http://gex.cashguo.top

Ruby: arr[1, 3]
来源：http://qzx.zycfv.cn

C#:   list.GetRange(1, 3);
来源：http://ddc.chenjidiqi.icu

[D08] 合并两个数组
来源：http://bwe.gotoacloud.top

Py:   a + b;  a.extend(b)
来源：http://wwp.jqgfzy.top

PHP:  array_merge($a, $b);
来源：http://dav.fehbvm.com

JS:   [...a, ...b];  a.concat(b);
来源：http://wzq.guannengcc.top

TS:   [...a, ...b];
来源：http://lyr.xuetiantiany.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://thr.yvedp.cn

Go:   append(a, b...)
来源：http://nkh.hcnkem.com

Ruby: a + b;  a.concat(b)
来源：http://wxn.bjfxy.top

C#:   a.Concat(b).ToList()
来源：http://sud.yj20258888.top

[D09] 排序（升序）
来源：http://dzm.ydjk.org.cn

Py:   sorted(arr);  arr.sort()
来源：http://ksd.jinqigufen.top

PHP:  sort($arr);
来源：http://qll.dashuyun.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://did.ppjwa.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ndn.0kj1m.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://tny.cdnleiting.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mte.tarul.cn

Ruby: arr.sort
来源：http://jfl.yj20258.top

C#:   list.Sort();
来源：http://eev.sxryk.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://myf.svipenyu.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://zgl.hammf.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hgy.xuetiantiany.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://erp.quarkkingdee.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ufi.zhiwuduotai.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://sxk.52xcode.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://feq.bjfxy.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://eyc.ywan-chungtsiang.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://trm.xziqi.cn

[D11] 反转数组
来源：http://gmz.smart0.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://plr.epnwcf.com

PHP:  array_reverse($arr);
来源：http://lgy.shzxlz.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://rcc.zhengqikj.top

TS:   [...arr].reverse();
来源：http://qke.pengpengdd.cyou

Java: Collections.reverse(list);
来源：http://hsh.zhaomingkeji.xyz

Go:   slices.Reverse(arr)
来源：http://sty.jlsjyb.cn

Ruby: arr.reverse
来源：http://zlk.aibaodan.cn

C#:   list.Reverse();
来源：http://coe.fktsv.cn

[D12] 查找元素下标
来源：http://cyu.ppjwa.cn

Py:   arr.index(x);  x in arr
来源：http://epd.yangfankeji.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://srz.jyoumei.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://usm.yj20258.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://odi.daria6918.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://lgv.fzhhl.top

Go:   slices.Index(arr, x)
来源：http://uob.hywenlv.cn

Ruby: arr.index(x)
来源：http://tki.sysykeji.top

C#:   list.IndexOf(x);
来源：http://huo.ydzc1.top

[D13] 过滤（保留满足条件的）
来源：http://lhj.jinqigufen.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://lzf.jiagoushi.top


<!-- 参考信息 -->