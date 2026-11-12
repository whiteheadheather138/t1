代发 wailian999

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://rdo.wangshuangyany.cn

Ruby: (0...10).step(2).to_a
来源：http://vll.cqqwz.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://dwz.shzxlz.cn

[B12] 跳出多层循环
来源：http://ggu.redwolf501.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://elm.xylfe.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://bdv.aizwys.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://pil.chenzaomai.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://alf.ehwqpu.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://lbg.iojbl.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://yyv.fanxiaobao.xyz

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://fnn.tarul.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://vrg.meibo888.top

[B13] 判断是否为数字
来源：http://yhm.fehbvm.com

Py:   isinstance(x, (int, float))
来源：http://ogr.fanxiaobao.xyz

PHP:  is_numeric($x)
来源：http://duv.xuanzx.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qyb.fktsv.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jms.sxryk.cn

Java: x instanceof Number
来源：http://jgs.jianghu66.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://pyc.hnxiangtu.top

Ruby: x.is_a?(Numeric)
来源：http://pfd.pycfn.com

C#:   x is int or double or decimal
来源：http://pkd.ctjpmb.com

[B14] 判断值是否在集合内
来源：http://uas.yanxiufei.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ekg.sjlbkw.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wku.gaohongyu789.top

JS:   [1, 2, 3].includes(x)
来源：http://jth.andypj.xyz

TS:   [1, 2, 3].includes(x)
来源：http://bbo.c1oappe.top

Java: List.of(1, 2, 3).contains(x)
来源：http://lpb.pycfn.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://amw.dianchejie.cn

Ruby: [1, 2, 3].include?(x)
来源：http://anm.redwolf501.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://xrk.sjlbkw.cn

[B15] 布尔运算与取反
来源：http://bnu.shuidangran.top

Py:   a and b or not c
来源：http://dgs.guannengcc.top

PHP:  $a && $b || !$c
来源：http://fyg.jinghuilouyu.cn

JS:   a && b || !c
来源：http://eiq.redwolf501.top

TS:   a && b || !c
来源：http://oad.hammf.cn

Java: a && b || !c
来源：http://cdp.ctjpmb.com

Go:   a && b || !c
来源：http://czn.jinqigufen.top

Ruby: a && b || !c
来源：http://qyz.chenzaomai.com

C#:   a && b || !c
来源：http://hze.jianghu66.top

[B16] 卫语句：不满足条件提前返回
来源：http://wiw.hongshengwenyu.top

Py:   if not data: return
来源：http://ufy.yonumen.top

PHP:  if (!$data) { return; }
来源：http://tff.shanyushiyangtech.top

JS:   if (!data) return;
来源：http://pyh.shanyushiyangtech.top

TS:   if (!data) return;
来源：http://atg.sysykeji.top

Java: if (data == null) return;
来源：http://nlm.zhongyouzk.top

Go:   if data == nil { return }
来源：http://wcz.chenlongwang.top

Ruby: return if data.nil?
来源：http://ewm.zhiwuduotai.top

C#:   if (data == null) return;
来源：http://vcu.shzxlz.cn

================================================================================
来源：http://lua.nanxinkj.top

C. 函数与作用域
来源：http://ucf.fengsongda.top

================================================================================
来源：http://kho.tian-w.cn

[C01] 定义函数
来源：http://ahr.guowangkeji.top

Py:   def add(a, b): return a + b
来源：http://jzi.yanxiufei.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://saz.wangshuangyany.cn

JS:   function add(a, b) { return a + b; }
来源：http://aaz.zhaomingkeji.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dsq.cdnleiting.top

Java: static int add(int a, int b) { return a + b; }
来源：http://mcs.0kj1m.cn

Go:   func add(a, b int) int { return a + b }
来源：http://qtz.hesvh.cn

Ruby: def add(a, b); a + b; end
来源：http://oci.mhx1999.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://smz.nwbrower.top

[C02] 默认参数
来源：http://zyx.nanxuanxn.top

Py:   def greet(name="World"): return name
来源：http://mcj.yj20258.top

PHP:  function greet($name = "World") { return $name; }
来源：http://xrf.cashguo.top

JS:   function greet(name = "World") { return name; }
来源：http://rei.cashguo.top

TS:   function greet(name: string = "World") { return name; }
来源：http://esh.uphjek.com

Java: // 无默认参数：方法重载或 Optional
来源：http://wyt.yj20258.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hma.vqdsnc.cn

Ruby: def greet(name = "World") = name
来源：http://oxr.yanxiufei.cn

C#:   string Greet(string name = "World") => name;
来源：http://dgt.bbcook.cn

[C03] 可变参数
来源：http://cxk.ywan-chungtsiang.top

Py:   def total(*args): return sum(args)
来源：http://kzh.hammf.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://fbe.tianlin.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://xyp.shuidangran.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ktc.yangfankeji.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://tux.yangfankeji.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ryz.9152youxi.cn

Ruby: def total(*nums); nums.sum; end
来源：http://uqx.52xcode.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://qkc.sufxvd.cn

[C04] 命名参数 / 关键字参数
来源：http://pxn.ppjwa.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://loz.ywan-chungtsiang.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://jpf.zhengqikj.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xba.guannengcc.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://bof.guowangkeji.top

Java: // 无：用 Builder 模式或 record
来源：http://nyn.zdbjq.cn

Go:   // 无：用配置结构体参数
来源：http://fwj.yangfankeji.com

Ruby: f(a: 1, b: 2)
来源：http://mfb.aibaodan.cn

C#:   f(a: 1, b: 2)
来源：http://kix.sweek.top

[C05] 返回多个值
来源：http://ccu.jiagoushi.top

Py:   return a, b
来源：http://jox.yonumen.top

PHP:  return [$a, $b];
来源：http://kxi.cdnleiting.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://pir.yj202588.top

TS:   return { a, b };
来源：http://syg.cheryme.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://upt.hongshengwenyu.top

Go:   return a, b
来源：http://aoe.zhaomingkeji.xyz

Ruby: return a, b
来源：http://oom.ydjk.org.cn

C#:   return (a, b);              // ValueTuple
来源：http://qdq.smart0.xyz

[C06] 匿名函数 / lambda
来源：http://wqj.jinghuilouyu.cn

Py:   square = lambda x: x * x
来源：http://cix.shuidangran.top

PHP:  $square = fn($x) => $x * $x;
来源：http://oim.andypj.xyz

JS:   const square = x => x * x;
来源：http://qkx.vehdjk.com

TS:   const square = (x: number): number => x * x;
来源：http://hbl.daria6918.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://puj.guowangkeji.top

Go:   sq := func(x int) int { return x * x }
来源：http://tku.sweek.top

Ruby: square = ->(x) { x * x }
来源：http://dty.gogol.net.cn

C#:   Func<int, int> square = x => x * x;
来源：http://qnd.cdnleiting.top

[C07] 把函数作为参数传入
来源：http://jpp.ybcxt.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://dtr.jinyuanbaomall.cn

PHP:  array_map("strtoupper", $arr);
来源：http://rrb.jinqigufen.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://sfi.0kj1m.cn

TS:   arr.map(String)
来源：http://iha.nwbrower.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://gqd.hfpthk.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ooo.hongshengwenyu.top

Ruby: arr.map(&:upcase)
来源：http://vjt.52xcode.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://jex.pengpengdd.cyou

[C08] 闭包
来源：http://rlw.yuxming.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://cfk.nwbrower.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://eel.iojbl.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://rgm.cucudq.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ldj.hcnkem.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://dnb.yfazqb.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://qsf.cdnleiting.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://efu.yj20258888.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://cmd.shuidangran.top

[C09] 递归
来源：http://avy.cdnleiting.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hjt.ydzc1.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wlz.guannengcc.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zaw.ehwqpu.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://whu.tianlin.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wvu.yvedp.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://msp.yueranfly.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://soc.redwolf501.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ivo.redwolf501.top

[C10] 变量作用域
来源：http://hvl.hammf.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://teg.0kj1m.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ejo.yonumen.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://rjz.pycfn.com

TS:   同 JS
来源：http://ogc.jinghuilouyu.cn

Java: 方法内为块级作用域
来源：http://bcd.yuanzhike.top

Go:   花括号块级作用域
来源：http://qrc.nwbrower.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://tip.hesvh.cn

C#:   块级作用域
来源：http://cnp.ybcxt.top

[C11] 模块导入与导出
来源：http://dac.vqdsnc.cn

Py:   from module import func
来源：http://apo.jinghuilouyu.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://qqb.chenlongwang.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://pvx.svipenyu.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wym.shangyingyoupin.top

Java: import java.util.List;
来源：http://zga.pycfn.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://eec.fengsongda.top

Ruby: require "json"; require_relative "./util"
来源：http://vxo.yongpay.top

C#:   using System.Text;
来源：http://trg.yuanzhike.top

[C12] 立即执行函数 IIFE
来源：http://yup.zhongyouzk.top

Py:   (lambda: print("run"))()
来源：http://sgl.vehdjk.com

PHP:  (function () { echo "run"; })();
来源：http://trx.xuanzx.com

JS:   (() => { console.log("run"); })();
来源：http://xbd.sysykeji.top

TS:   (() => { console.log("run"); })();
来源：http://trp.tian-w.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://avf.gaohongyu789.top

Go:   func() { fmt.Println("run") }()
来源：http://gvl.dashuyun.cn

Ruby: -> { puts "run" }.call
来源：http://aqa.pengpengdd.cyou

C#:   // 无 IIFE：用静态构造函数
来源：http://fjy.nanxuanxn.top

[C13] 类型声明 / 类型注解
来源：http://evz.mhx1999.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hsz.snrcjt.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zox.cqqwz.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://frz.yanxiufei.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xqx.vehdjk.com

Java: int add(int a, int b) { return a + b; }
来源：http://liq.fengsongda.top

Go:   func add(a, b int) int
来源：http://uut.0kj1m.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://dwm.xuetiantiany.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ljt.ybcxt.top

[C14] 泛型函数
来源：http://pky.ppjwa.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://yqz.yfazqb.com

PHP:  // 无泛型
来源：http://tfw.sysykeji.top

JS:   // 无泛型
来源：http://tvh.daxiang520.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://dge.cheryme.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ezd.zdqjudy.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://vji.dashuyun.cn

Ruby: # 无泛型
来源：http://ekr.havefunace.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://nfb.aizwys.cn

[C15] 解构 / 展开参数
来源：http://rpj.dianchejie.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wkb.xziqi.cn

PHP:  [$a, $b] = $pair;
来源：http://hum.vehdjk.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://lrq.shanyushiyangkeji.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://jqq.xinyue.icu

Java: // 无解构
来源：http://kex.ywan-chungtsiang.top

Go:   // 无解构
来源：http://kmq.yuxming.cn

Ruby: a, b = pair
来源：http://jjh.jinqigfzy.top

C#:   var (a, b) = pair;
来源：http://mry.9152youxi.cn

[C16] 函数 / 方法重载
来源：http://lab.yueranfly.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://zhu.wangshuangyany.cn

PHP:  // 无重载
来源：http://ysv.hammf.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://bsx.zdbjq.cn

TS:   // 用联合类型或重载签名声明
来源：http://gbe.shangyingyoupin.top

Java: void f(int a) {}  void f(String a) {}
来源：http://aay.ydjk.org.cn

Go:   // 无重载：用不同函数名
来源：http://oba.vqdsnc.cn

Ruby: # 无重载：靠动态参数
来源：http://jtq.zdqjudy.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://yff.chenzaomai.com

================================================================================
来源：http://bfy.guannengcc.top

D. 数组 / 列表 / 集合
来源：http://cby.nanxuanxn.top

================================================================================
来源：http://vol.jianghu66.top

[D01] 创建数组 / 列表
来源：http://mke.aizwys.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://zjz.9152youxi.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ejl.gotoacloud.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://erg.sxryk.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://lqx.cqqwz.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://xhq.kuanghao11.cn

Go:   arr := []int{1, 2, 3}
来源：http://rhx.yvedp.cn

Ruby: arr = [1, 2, 3]
来源：http://por.ehwqpu.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://xrl.zhongyouzk.top

[D02] 追加元素到末尾
来源：http://kwg.yj20258888.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://lpc.redwolf501.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://kuj.vqdsnc.cn

JS:   arr.push(4);
来源：http://apm.gzhubu.top

TS:   arr.push(4);
来源：http://kpk.yj20258888.top

Java: list.add(4);
来源：http://zgx.ydjk.org.cn

Go:   arr = append(arr, 4)
来源：http://iyh.vehdjk.com

Ruby: arr << 4; arr.push(5)
来源：http://ltt.gaohongyu789.top

C#:   list.Add(4);
来源：http://qpp.feifeiyinyue.top

[D03] 在指定位置插入元素
来源：http://eve.shanyushiyangtech.top

Py:   arr.insert(0, 0)
来源：http://rpr.yvedp.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://bqm.yj20258.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://cfj.jinqigfzy.top

TS:   arr.splice(0, 0, 0);
来源：http://yws.svipenyu.cn

Java: list.add(0, 0);
来源：http://lgo.zhijiandao.cn

Go:   arr = append([]int{0}, arr...)
来源：http://gln.yfazqb.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://jez.jinqigfzy.top

C#:   list.Insert(0, 0);
来源：http://oxl.fanxiaobao.xyz

[D04] 删除元素
来源：http://sym.sxryk.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://zgs.sxryk.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://vrt.xylfe.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://gbc.tian-w.cn

TS:   arr.splice(0, 1);
来源：http://gzd.ywan-chungtsiang.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://tfd.jinghuilouyu.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mqr.bjfxy.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wgi.sjlbkw.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://nvu.feifeiyinyue.top

[D05] 访问与修改元素
来源：http://til.xuetiantiany.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://lda.jianghu66.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://qdb.ydjk.org.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://qug.gzhubu.top

TS:   arr[0]; arr.at(-1);
来源：http://vhh.hysaishi.cn

Java: list.get(0); list.set(0, 9);
来源：http://vks.cucudq.cn

Go:   arr[0]; arr[0] = 9
来源：http://xob.xuetiantiany.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ite.guannengcc.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://nnk.gotoacloud.top

[D06] 数组长度
来源：http://xrl.cucudq.cn

Py:   len(arr)
来源：http://ppe.zhongyouzk.top

PHP:  count($arr);
来源：http://fle.birdmap.top

JS:   arr.length
来源：http://vit.aizwys.cn

TS:   arr.length
来源：http://vjn.aizwys.cn

Java: list.size();
来源：http://kpw.dashuyun.cn

Go:   len(arr)
来源：http://gia.zhixingplan.top

Ruby: arr.length; arr.size
来源：http://eqs.zhijiandao.cn

C#:   list.Count;
来源：http://naq.jinqigfzy.top

[D07] 切片 / 取子数组
来源：http://hiv.jinqigufen.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://tht.aibaodan.cn

PHP:  array_slice($arr, 1, 3);
来源：http://egd.shuidangran.top

JS:   arr.slice(1, 4);
来源：http://qvw.daria6918.cn

TS:   arr.slice(1, 4);
来源：http://dyv.jqgufenzy.top

Java: list.subList(1, 4);
来源：http://olh.zdbjq.cn

Go:   arr[1:4]
来源：http://zjn.chenjidiqi.icu

Ruby: arr[1, 3]
来源：http://agg.yuanzhike.top

C#:   list.GetRange(1, 3);
来源：http://jnh.yuanzhike.top

[D08] 合并两个数组
来源：http://rot.chenjidiqi.icu

Py:   a + b;  a.extend(b)
来源：http://hdr.shuidangran.top

PHP:  array_merge($a, $b);
来源：http://uws.xylfe.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://jbv.daxiang520.top

TS:   [...a, ...b];
来源：http://bym.hnqzz.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://aph.fanxiaobao.xyz

Go:   append(a, b...)
来源：http://mrj.ybcxt.top

Ruby: a + b;  a.concat(b)
来源：http://ukh.tarul.cn

C#:   a.Concat(b).ToList()
来源：http://fwj.316326.xyz

[D09] 排序（升序）
来源：http://dmw.yj20258888.top

Py:   sorted(arr);  arr.sort()
来源：http://gcv.zdqjudy.top

PHP:  sort($arr);
来源：http://geq.jqgufenzy.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://eeb.yj20258.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://gfg.gotoacloud.top

Java: Collections.sort(list);  list.sort(null);
来源：http://bmi.jyoumei.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ite.zdqjudy.top

Ruby: arr.sort
来源：http://jxy.shuidangran.top

C#:   list.Sort();
来源：http://blf.hywenlv.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://gwx.jlsjyb.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://azg.iojbl.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qky.zhaomingkeji.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://jvp.shuidangran.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://yjw.c1oappe.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ybl.ywan-chungtsiang.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://apz.yj20258888.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ohn.yangfankeji.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://kvf.zhoulong.xyz

[D11] 反转数组
来源：http://tey.bjfxy.top

Py:   arr[::-1];  arr.reverse()
来源：http://tyt.zhaomingkeji.xyz

PHP:  array_reverse($arr);
来源：http://ify.gzhubu.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://tyv.shangyingyoupin.top

TS:   [...arr].reverse();
来源：http://ekj.ctjpmb.com

Java: Collections.reverse(list);
来源：http://dfx.xuetiantiany.cn

Go:   slices.Reverse(arr)
来源：http://olc.fengsongda.top

Ruby: arr.reverse
来源：http://grv.yangfankeji.com

C#:   list.Reverse();
来源：http://kov.dashuyun.cn

[D12] 查找元素下标
来源：http://mep.chenzaomai.com

Py:   arr.index(x);  x in arr
来源：http://ylx.gzhubu.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://qbo.sufxvd.cn


<!-- 参考信息 -->