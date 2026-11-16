代发 wailian999

PHP:  range(0, 10, 2);
来源：http://qhl.yj202588.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rwl.wangdashe.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://inr.cqqwz.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://xhq.c1oappe.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://azq.chenzaomai.com

Ruby: (0...10).step(2).to_a
来源：http://weh.gaohongyu789.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://tam.zdqjudy.top

[B12] 跳出多层循环
来源：http://hmp.jianghu66.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://vtq.guannengcc.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://lkf.andypj.xyz

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://qsi.mhx1999.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://gzi.ehwqpu.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://tio.ehwqpu.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://rjy.wangshuangyany.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ied.jlsjyb.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://guy.ctjpmb.com

[B13] 判断是否为数字
来源：http://bpf.jqgufenzy.top

Py:   isinstance(x, (int, float))
来源：http://fxa.dianchejie.cn

PHP:  is_numeric($x)
来源：http://qpv.pycfn.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://azs.ydzc1.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://afz.yuanzhike.top

Java: x instanceof Number
来源：http://ian.cdnleiting.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ahn.cucudq.cn

Ruby: x.is_a?(Numeric)
来源：http://cma.ywan-chungtsiang.top

C#:   x is int or double or decimal
来源：http://odp.yonumen.top

[B14] 判断值是否在集合内
来源：http://pjm.tarul.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ykg.shanyushiyangtech.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://yuz.pycfn.com

JS:   [1, 2, 3].includes(x)
来源：http://mnl.yj20258.top

TS:   [1, 2, 3].includes(x)
来源：http://wdu.snrcjt.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://bot.hongshengwenyu.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://xlo.hfpthk.cn

Ruby: [1, 2, 3].include?(x)
来源：http://qil.jinqigufen.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://oyn.ywan-chungtsiang.top

[B15] 布尔运算与取反
来源：http://tai.ppjwa.cn

Py:   a and b or not c
来源：http://deh.zhaomingkeji.xyz

PHP:  $a && $b || !$c
来源：http://fcu.wangdashe.top

JS:   a && b || !c
来源：http://hst.jiagoushi.top

TS:   a && b || !c
来源：http://kzx.ppjwa.cn

Java: a && b || !c
来源：http://bzc.aizwys.cn

Go:   a && b || !c
来源：http://tpw.ydjk.org.cn

Ruby: a && b || !c
来源：http://fta.zdbjq.cn

C#:   a && b || !c
来源：http://ueb.yuxming.cn

[B16] 卫语句：不满足条件提前返回
来源：http://fmw.smart0.xyz

Py:   if not data: return
来源：http://fuy.yj202588.top

PHP:  if (!$data) { return; }
来源：http://xvi.nanxuanxn.top

JS:   if (!data) return;
来源：http://ojs.9152youxi.cn

TS:   if (!data) return;
来源：http://fvn.fktsv.cn

Java: if (data == null) return;
来源：http://pvf.shanyushiyangtech.top

Go:   if data == nil { return }
来源：http://wcz.fktsv.cn

Ruby: return if data.nil?
来源：http://gqt.jinyuanbaomall.cn

C#:   if (data == null) return;
来源：http://hht.sysykeji.top

================================================================================
来源：http://nef.jinqigufen.top

C. 函数与作用域
来源：http://wso.wangdashe.top

================================================================================
来源：http://dcv.hnxiangtu.top

[C01] 定义函数
来源：http://who.ybcxt.top

Py:   def add(a, b): return a + b
来源：http://nsl.epnwcf.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kdi.aizwys.cn

JS:   function add(a, b) { return a + b; }
来源：http://mdl.zhiwuduotai.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gok.guowangkeji.top

Java: static int add(int a, int b) { return a + b; }
来源：http://sdn.tanke756.top

Go:   func add(a, b int) int { return a + b }
来源：http://nfm.shuidangran.top

Ruby: def add(a, b); a + b; end
来源：http://mov.sysykeji.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://tqr.gzhubu.top

[C02] 默认参数
来源：http://gwd.ybcxt.top

Py:   def greet(name="World"): return name
来源：http://dlg.xinyue.icu

PHP:  function greet($name = "World") { return $name; }
来源：http://hyd.birdmap.top

JS:   function greet(name = "World") { return name; }
来源：http://kdh.smart0.xyz

TS:   function greet(name: string = "World") { return name; }
来源：http://nwp.guowangkeji.top

Java: // 无默认参数：方法重载或 Optional
来源：http://imc.cucudq.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://zst.hnqzz.top

Ruby: def greet(name = "World") = name
来源：http://rug.hongshengwenyu.top

C#:   string Greet(string name = "World") => name;
来源：http://jdd.pengpengdd.cyou

[C03] 可变参数
来源：http://dlh.dianchejie.cn

Py:   def total(*args): return sum(args)
来源：http://csz.hfpthk.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://dlo.gogol.net.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://oga.gogol.net.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mfj.vqdsnc.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://csp.ppjwa.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://zif.bjfxy.top

Ruby: def total(*nums); nums.sum; end
来源：http://owy.gaohongyu789.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ufh.fktsv.cn

[C04] 命名参数 / 关键字参数
来源：http://zgy.jyoumei.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hbf.hywenlv.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ovh.ctjpmb.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://frq.uphjek.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://gcn.vqdsnc.cn

Java: // 无：用 Builder 模式或 record
来源：http://age.hywenlv.cn

Go:   // 无：用配置结构体参数
来源：http://qus.c1oappe.top

Ruby: f(a: 1, b: 2)
来源：http://wee.birdmap.top

C#:   f(a: 1, b: 2)
来源：http://ayu.zhengqikj.top

[C05] 返回多个值
来源：http://nwl.haohaochexian.top

Py:   return a, b
来源：http://xwl.havefunace.top

PHP:  return [$a, $b];
来源：http://oys.gaohongyu789.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://dsc.bjfxy.top

TS:   return { a, b };
来源：http://ltq.jianghu66.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://lpq.gotoacloud.top

Go:   return a, b
来源：http://gln.zdqjudy.top

Ruby: return a, b
来源：http://mhl.cashguo.top

C#:   return (a, b);              // ValueTuple
来源：http://eao.fzhhl.top

[C06] 匿名函数 / lambda
来源：http://vuq.jinyuanbaomall.cn

Py:   square = lambda x: x * x
来源：http://etw.yanxiufei.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://yij.xziqi.cn

JS:   const square = x => x * x;
来源：http://eez.chenzaomai.com

TS:   const square = (x: number): number => x * x;
来源：http://zqj.jqgfzy.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://iqr.mhx1999.top

Go:   sq := func(x int) int { return x * x }
来源：http://xdu.tanke756.top

Ruby: square = ->(x) { x * x }
来源：http://seu.zycfv.cn

C#:   Func<int, int> square = x => x * x;
来源：http://nxo.hesvh.cn

[C07] 把函数作为参数传入
来源：http://oay.yfazqb.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://qhg.gzhubu.top

PHP:  array_map("strtoupper", $arr);
来源：http://bnv.sysykeji.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://tiu.cashguo.top

TS:   arr.map(String)
来源：http://bev.fktsv.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://qav.meibo888.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://jbv.gzhubu.top

Ruby: arr.map(&:upcase)
来源：http://rbh.nanxuanxn.top

C#:   arr.Select(s => s.ToUpper())
来源：http://xfs.pengpengdd.cyou

[C08] 闭包
来源：http://ooc.wangdashe.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://bwh.jlsjyb.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://qco.gotoacloud.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://yjw.nanxinkj.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hnm.bjfxy.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://pru.xuanzx.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://kcf.jlsjyb.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://dnw.jiagoushi.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://nno.aizwys.cn

[C09] 递归
来源：http://hgq.uphjek.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://aow.aizwys.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ufs.sweek.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dzw.zdbjq.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pcb.shzxlz.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://sfa.andypj.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://pxx.guowangkeji.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://pky.9152youxi.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://uaq.nwbrower.top

[C10] 变量作用域
来源：http://sjr.chenlongwang.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://gvn.xuanzx.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://sff.ydzc1.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://fih.hysaishi.cn

TS:   同 JS
来源：http://cub.zhoulong.xyz

Java: 方法内为块级作用域
来源：http://jan.shanyushiyangkeji.top

Go:   花括号块级作用域
来源：http://tcz.yongpay.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ymh.zhengqikj.top

C#:   块级作用域
来源：http://usx.0kj1m.cn

[C11] 模块导入与导出
来源：http://auv.jyoumei.cn

Py:   from module import func
来源：http://wxi.sxryk.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://xnl.guannengcc.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://fsb.52xcode.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://dbo.guowangkeji.top

Java: import java.util.List;
来源：http://oml.xinyue.icu

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://kcp.shangyingyoupin.top

Ruby: require "json"; require_relative "./util"
来源：http://zif.xuanzx.com

C#:   using System.Text;
来源：http://iyf.hnxiangtu.top

[C12] 立即执行函数 IIFE
来源：http://hax.zhijiandao.cn

Py:   (lambda: print("run"))()
来源：http://azn.quarkkingdee.top

PHP:  (function () { echo "run"; })();
来源：http://sib.chenlongwang.top

JS:   (() => { console.log("run"); })();
来源：http://xmi.jianghu66.top

TS:   (() => { console.log("run"); })();
来源：http://qhv.aizwys.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://vul.fktsv.cn

Go:   func() { fmt.Println("run") }()
来源：http://gck.sxryk.cn

Ruby: -> { puts "run" }.call
来源：http://nbl.birdmap.top

C#:   // 无 IIFE：用静态构造函数
来源：http://tvq.iojbl.cn

[C13] 类型声明 / 类型注解
来源：http://qmk.hnxiangtu.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://tey.vehdjk.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jlu.jqgufenzy.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://emj.fanxiaobao.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://edk.sxryk.cn

Java: int add(int a, int b) { return a + b; }
来源：http://zqc.wangdashe.top

Go:   func add(a, b int) int
来源：http://cyp.cashguo.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://amc.daria6918.cn

C#:   int Add(int a, int b) => a + b;
来源：http://xan.tarul.cn

[C14] 泛型函数
来源：http://llp.zdqjudy.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://eaw.quarkkingdee.top

PHP:  // 无泛型
来源：http://yec.wangshuangyany.cn

JS:   // 无泛型
来源：http://uqy.zhengqikj.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://idt.shzxlz.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://zwv.jinqigufen.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://cft.shuidangran.top

Ruby: # 无泛型
来源：http://ptp.yvedp.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://qhc.hywenlv.cn

[C15] 解构 / 展开参数
来源：http://rqz.ydzc1.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wig.xinyue.icu

PHP:  [$a, $b] = $pair;
来源：http://blk.yanxiufei.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hrs.bbcook.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://vwh.yuanzhike.top

Java: // 无解构
来源：http://hja.havefunace.top

Go:   // 无解构
来源：http://usn.gaohongyu789.top

Ruby: a, b = pair
来源：http://ayb.ywan-chungtsiang.top

C#:   var (a, b) = pair;
来源：http://mfa.gotoacloud.top

[C16] 函数 / 方法重载
来源：http://ztv.gaohongyu789.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hdk.nanxuanxn.top

PHP:  // 无重载
来源：http://pqw.zdbjq.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://chz.zhongyouzk.top

TS:   // 用联合类型或重载签名声明
来源：http://jxc.shanyushiyangtech.top

Java: void f(int a) {}  void f(String a) {}
来源：http://grw.0kj1m.cn

Go:   // 无重载：用不同函数名
来源：http://yeb.zhiwuduotai.top

Ruby: # 无重载：靠动态参数
来源：http://hpw.52xcode.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://twv.smart0.xyz

================================================================================
来源：http://xjy.shangyingyoupin.top

D. 数组 / 列表 / 集合
来源：http://bfb.guowangkeji.top

================================================================================
来源：http://hlj.mhx1999.top

[D01] 创建数组 / 列表
来源：http://rsw.yonumen.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://hjg.gzhubu.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ncv.sweek.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mgx.sxryk.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://zev.yueranfly.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://qzo.yuxming.cn

Go:   arr := []int{1, 2, 3}
来源：http://hlh.yangfankeji.com

Ruby: arr = [1, 2, 3]
来源：http://lpp.yonumen.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wes.hongshengwenyu.top

[D02] 追加元素到末尾
来源：http://hic.zdqjudy.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://enu.kuanghao11.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://sdy.yueranfly.top

JS:   arr.push(4);
来源：http://hii.ehwqpu.com

TS:   arr.push(4);
来源：http://dmw.tarul.cn

Java: list.add(4);
来源：http://wwx.xinyue.icu

Go:   arr = append(arr, 4)
来源：http://mmf.zhoulong.xyz

Ruby: arr << 4; arr.push(5)
来源：http://lnh.hnqzz.top

C#:   list.Add(4);
来源：http://xeu.zhengqikj.top

[D03] 在指定位置插入元素
来源：http://vib.yuanzhike.top

Py:   arr.insert(0, 0)
来源：http://lgw.tian-w.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://qqb.smart0.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://zfe.ppjwa.cn

TS:   arr.splice(0, 0, 0);
来源：http://xus.svipenyu.cn

Java: list.add(0, 0);
来源：http://sns.gotoacloud.top

Go:   arr = append([]int{0}, arr...)
来源：http://gea.ehwqpu.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://izv.jqgufenzy.top

C#:   list.Insert(0, 0);
来源：http://wva.daxiang520.top

[D04] 删除元素
来源：http://jvz.yonumen.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://bna.sweek.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ykv.sxryk.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://dbw.hongshengwenyu.top

TS:   arr.splice(0, 1);
来源：http://ogh.redwolf501.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://jwh.hcnkem.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mjq.guannengcc.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hoj.ctjpmb.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://nrz.xziqi.cn

[D05] 访问与修改元素
来源：http://ika.birdmap.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://lam.ehwqpu.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://pbs.jinqigfzy.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://vdy.yonumen.top

TS:   arr[0]; arr.at(-1);
来源：http://gkl.cqqwz.cn

Java: list.get(0); list.set(0, 9);
来源：http://zwe.nanxuanxn.top

Go:   arr[0]; arr[0] = 9
来源：http://gst.gaohongyu789.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://dlz.yonumen.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zlt.yj202588.top

[D06] 数组长度
来源：http://tgj.shanyushiyangkeji.top

Py:   len(arr)
来源：http://hgd.shanyushiyangtech.top

PHP:  count($arr);
来源：http://qyw.kuanghao11.cn

JS:   arr.length
来源：http://cfq.yvedp.cn

TS:   arr.length
来源：http://uuf.jinqigfzy.top

Java: list.size();
来源：http://szm.jyoumei.cn

Go:   len(arr)
来源：http://thl.shuidangran.top

Ruby: arr.length; arr.size
来源：http://sqc.zycfv.cn

C#:   list.Count;
来源：http://plc.cashguo.top

[D07] 切片 / 取子数组
来源：http://fis.tian-w.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hqu.birdmap.top

PHP:  array_slice($arr, 1, 3);
来源：http://fwk.ybcxt.top

JS:   arr.slice(1, 4);
来源：http://rmi.zhaomingkeji.xyz

TS:   arr.slice(1, 4);
来源：http://vli.zhixingplan.top

Java: list.subList(1, 4);
来源：http://mus.yueranfly.top

Go:   arr[1:4]
来源：http://utq.tarul.cn

Ruby: arr[1, 3]
来源：http://iew.ywan-chungtsiang.top

C#:   list.GetRange(1, 3);
来源：http://uye.52xcode.cn

[D08] 合并两个数组
来源：http://uan.yueranfly.top

Py:   a + b;  a.extend(b)
来源：http://mnz.smart0.xyz

PHP:  array_merge($a, $b);
来源：http://uge.dianchejie.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ire.iojbl.cn

TS:   [...a, ...b];
来源：http://erk.zhongyouzk.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ogp.hesvh.cn

Go:   append(a, b...)
来源：http://eay.xinyue.icu

Ruby: a + b;  a.concat(b)
来源：http://anu.zhiwuduotai.top

C#:   a.Concat(b).ToList()
来源：http://oxk.sxryk.cn

[D09] 排序（升序）
来源：http://rfg.tianlin.xyz

Py:   sorted(arr);  arr.sort()
来源：http://uto.jiagoushi.top

PHP:  sort($arr);
来源：http://uol.zhoulong.xyz

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://dpp.yonumen.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://ecg.xziqi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://vkm.jinqigfzy.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://cua.wangshuangyany.cn

Ruby: arr.sort
来源：http://kwo.dianchejie.cn

C#:   list.Sort();
来源：http://vzg.nanxinkj.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://nrh.zhixingplan.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://rnv.fengsongda.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://poc.ydzc1.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://vxf.andypj.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://soe.cqqwz.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://tdj.shuidangran.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://dvn.sweek.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://bah.shzxlz.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://jxg.sweek.top

[D11] 反转数组
来源：http://xmp.jinqigfzy.top

Py:   arr[::-1];  arr.reverse()
来源：http://mcj.kuanghao11.cn

PHP:  array_reverse($arr);
来源：http://bzd.9152youxi.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://yau.jlsjyb.cn

TS:   [...arr].reverse();
来源：http://zxw.9152youxi.cn

Java: Collections.reverse(list);
来源：http://qpn.jyoumei.cn

Go:   slices.Reverse(arr)
来源：http://uym.cashguo.top

Ruby: arr.reverse
来源：http://rmw.xuetiantiany.cn


<!-- 参考信息 -->