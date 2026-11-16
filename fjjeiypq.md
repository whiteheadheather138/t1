代发 wailian999

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hkq.fzhhl.top

Java: x instanceof Number
来源：http://vty.ydjk.org.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://oua.gaohongyu789.top

Ruby: x.is_a?(Numeric)
来源：http://giy.shanyushiyangkeji.top

C#:   x is int or double or decimal
来源：http://wmp.cucudq.cn

[B14] 判断值是否在集合内
来源：http://vgh.uphjek.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://nrt.svipenyu.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://sqw.yvedp.cn

JS:   [1, 2, 3].includes(x)
来源：http://ihx.epnwcf.com

TS:   [1, 2, 3].includes(x)
来源：http://umw.iojbl.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://eon.jyoumei.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://sad.yongpay.top

Ruby: [1, 2, 3].include?(x)
来源：http://vse.quarkkingdee.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ywr.shanyushiyangtech.top

[B15] 布尔运算与取反
来源：http://ast.xinyue.icu

Py:   a and b or not c
来源：http://vjx.jlsjyb.cn

PHP:  $a && $b || !$c
来源：http://srw.cdnleiting.top

JS:   a && b || !c
来源：http://sho.ivvv.top

TS:   a && b || !c
来源：http://sug.xylfe.cn

Java: a && b || !c
来源：http://edw.feifeiyinyue.top

Go:   a && b || !c
来源：http://ocx.gaohongyu789.top

Ruby: a && b || !c
来源：http://vcm.fehbvm.com

C#:   a && b || !c
来源：http://jee.haohaochexian.top

[B16] 卫语句：不满足条件提前返回
来源：http://xcf.snrcjt.cn

Py:   if not data: return
来源：http://ttp.yueranfly.top

PHP:  if (!$data) { return; }
来源：http://awr.andypj.xyz

JS:   if (!data) return;
来源：http://agd.aibaodan.cn

TS:   if (!data) return;
来源：http://rfb.yuanzhike.top

Java: if (data == null) return;
来源：http://ugs.c1oappe.top

Go:   if data == nil { return }
来源：http://gvg.sweek.top

Ruby: return if data.nil?
来源：http://xtz.xinyue.icu

C#:   if (data == null) return;
来源：http://yke.gaohongyu789.top

================================================================================
来源：http://hrr.zhongyouzk.top

C. 函数与作用域
来源：http://xzc.zdqjudy.top

================================================================================
来源：http://qsj.fktsv.cn

[C01] 定义函数
来源：http://ttb.shzxlz.cn

Py:   def add(a, b): return a + b
来源：http://zhb.hnxiangtu.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ktp.c1oappe.top

JS:   function add(a, b) { return a + b; }
来源：http://anu.chenjidiqi.icu

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dzy.9152youxi.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://enm.chenjidiqi.icu

Go:   func add(a, b int) int { return a + b }
来源：http://jqe.jinghuilouyu.cn

Ruby: def add(a, b); a + b; end
来源：http://jru.andypj.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://qgg.zhoulong.xyz

[C02] 默认参数
来源：http://xrt.ctjpmb.com

Py:   def greet(name="World"): return name
来源：http://awu.xylfe.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://omp.fengsongda.top

JS:   function greet(name = "World") { return name; }
来源：http://ony.daxiang520.top

TS:   function greet(name: string = "World") { return name; }
来源：http://jem.sxryk.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://olu.hcnkem.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://byf.hesvh.cn

Ruby: def greet(name = "World") = name
来源：http://etl.yvedp.cn

C#:   string Greet(string name = "World") => name;
来源：http://qrq.yuxming.cn

[C03] 可变参数
来源：http://uac.jinyuanbaomall.cn

Py:   def total(*args): return sum(args)
来源：http://lur.havefunace.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://rgz.hcnkem.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://nqw.9152youxi.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://pdy.zhaomingkeji.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://noj.zhixingplan.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ijj.smart0.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://zwv.tarul.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ony.vehdjk.com

[C04] 命名参数 / 关键字参数
来源：http://ilf.smart0.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://rmy.cqqwz.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://rjq.birdmap.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://zrc.cucudq.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://jll.yuxming.cn

Java: // 无：用 Builder 模式或 record
来源：http://hdt.daxiang520.top

Go:   // 无：用配置结构体参数
来源：http://mgv.shuidangran.top

Ruby: f(a: 1, b: 2)
来源：http://mxq.yfazqb.com

C#:   f(a: 1, b: 2)
来源：http://bod.zhongyouzk.top

[C05] 返回多个值
来源：http://oga.hnqzz.top

Py:   return a, b
来源：http://ixa.ppjwa.cn

PHP:  return [$a, $b];
来源：http://elu.cdnleiting.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://cwe.xuetiantiany.cn

TS:   return { a, b };
来源：http://dzk.guowangkeji.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://how.xziqi.cn

Go:   return a, b
来源：http://elb.havefunace.top

Ruby: return a, b
来源：http://afd.xylfe.cn

C#:   return (a, b);              // ValueTuple
来源：http://xba.jqgufenzy.top

[C06] 匿名函数 / lambda
来源：http://zwq.haohaochexian.top

Py:   square = lambda x: x * x
来源：http://far.0kj1m.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://nqn.yvedp.cn

JS:   const square = x => x * x;
来源：http://sst.gaohongyu789.top

TS:   const square = (x: number): number => x * x;
来源：http://zrm.yuanzhike.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://fet.xziqi.cn

Go:   sq := func(x int) int { return x * x }
来源：http://xld.9152youxi.cn

Ruby: square = ->(x) { x * x }
来源：http://gxv.kuanghao11.cn

C#:   Func<int, int> square = x => x * x;
来源：http://wgi.ehwqpu.com

[C07] 把函数作为参数传入
来源：http://szb.fzhhl.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://axt.yj20258.top

PHP:  array_map("strtoupper", $arr);
来源：http://zwu.hnqzz.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ots.jinqigufen.top

TS:   arr.map(String)
来源：http://yva.yj20258888.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://znd.daria6918.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://eyz.ywan-chungtsiang.top

Ruby: arr.map(&:upcase)
来源：http://lwn.aizwys.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://pee.zhiwuduotai.top

[C08] 闭包
来源：http://wpq.xuetiantiany.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qdf.epnwcf.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hrb.cucudq.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://xfv.jinqigfzy.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://msl.fzhhl.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://kwi.zycfv.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://xrz.zhaomingkeji.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://xgb.dianchejie.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wjv.zhongyouzk.top

[C09] 递归
来源：http://vsz.aizwys.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://dwc.jinghuilouyu.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://xvf.zhengqikj.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fjf.52xcode.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://buy.ehwqpu.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://oeu.yj20258.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://huz.fengsongda.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://arb.wangdashe.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mxn.shzxlz.cn

[C10] 变量作用域
来源：http://vyg.sjlbkw.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://zyb.ehwqpu.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://aje.sysykeji.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ozf.yangfankeji.com

TS:   同 JS
来源：http://fkm.yj20258.top

Java: 方法内为块级作用域
来源：http://ilp.yuxming.cn

Go:   花括号块级作用域
来源：http://unf.kuanghao11.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://cek.yueranfly.top

C#:   块级作用域
来源：http://ake.yj20258888.top

[C11] 模块导入与导出
来源：http://vvv.yj20258.top

Py:   from module import func
来源：http://zya.zhaomingkeji.xyz

PHP:  require "file.php";  或 use App\Service;
来源：http://beg.daria6918.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://xjf.epnwcf.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mug.yuxming.cn

Java: import java.util.List;
来源：http://uoi.hesvh.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://gvn.hongshengwenyu.top

Ruby: require "json"; require_relative "./util"
来源：http://zgf.xinyue.icu

C#:   using System.Text;
来源：http://sdl.iojbl.cn

[C12] 立即执行函数 IIFE
来源：http://ykq.kuanghao11.cn

Py:   (lambda: print("run"))()
来源：http://zml.hnxiangtu.top

PHP:  (function () { echo "run"; })();
来源：http://zos.yangfankeji.com

JS:   (() => { console.log("run"); })();
来源：http://eos.jqgufenzy.top

TS:   (() => { console.log("run"); })();
来源：http://cyt.sjlbkw.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://khl.fktsv.cn

Go:   func() { fmt.Println("run") }()
来源：http://uww.tarul.cn

Ruby: -> { puts "run" }.call
来源：http://gfc.pycfn.com

C#:   // 无 IIFE：用静态构造函数
来源：http://ixb.zhengqikj.top

[C13] 类型声明 / 类型注解
来源：http://sai.9152youxi.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://qbl.ywan-chungtsiang.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vyc.yueranfly.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://bgn.xuanzx.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://awh.zhiwuduotai.top

Java: int add(int a, int b) { return a + b; }
来源：http://edr.zhijiandao.cn

Go:   func add(a, b int) int
来源：http://cby.hongshengwenyu.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wkq.zhixingplan.top

C#:   int Add(int a, int b) => a + b;
来源：http://wrx.fzhhl.top

[C14] 泛型函数
来源：http://psr.yj20258.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://smp.yangfankeji.com

PHP:  // 无泛型
来源：http://xvy.bbcook.cn

JS:   // 无泛型
来源：http://phx.feifeiyinyue.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://kpl.52xcode.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://spd.cheryme.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://zoz.guannengcc.top

Ruby: # 无泛型
来源：http://cue.nwbrower.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://rmt.fengsongda.top

[C15] 解构 / 展开参数
来源：http://brk.uphjek.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://eer.vehdjk.com

PHP:  [$a, $b] = $pair;
来源：http://ruv.ybcxt.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hek.yj20258.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hmq.pycfn.com

Java: // 无解构
来源：http://kax.chenjidiqi.icu

Go:   // 无解构
来源：http://bmk.jqgufenzy.top

Ruby: a, b = pair
来源：http://tsl.jlsjyb.cn

C#:   var (a, b) = pair;
来源：http://gga.pycfn.com

[C16] 函数 / 方法重载
来源：http://zbu.hysaishi.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://fdc.jinyuanbaomall.cn

PHP:  // 无重载
来源：http://jua.jyoumei.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://veg.fengsongda.top

TS:   // 用联合类型或重载签名声明
来源：http://uqu.zhongyouzk.top

Java: void f(int a) {}  void f(String a) {}
来源：http://zjw.fanxiaobao.xyz

Go:   // 无重载：用不同函数名
来源：http://sjx.jqgfzy.top

Ruby: # 无重载：靠动态参数
来源：http://ssk.yfazqb.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://ssx.jlsjyb.cn

================================================================================
来源：http://gab.epnwcf.com

D. 数组 / 列表 / 集合
来源：http://pxo.zhiwuduotai.top

================================================================================
来源：http://wjj.hcnkem.com

[D01] 创建数组 / 列表
来源：http://clb.hywenlv.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://tmt.hesvh.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://iwe.sweek.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://tho.epnwcf.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://gft.tanke756.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wai.xuetiantiany.cn

Go:   arr := []int{1, 2, 3}
来源：http://qmk.0kj1m.cn

Ruby: arr = [1, 2, 3]
来源：http://hsu.zycfv.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://bmy.nanxinkj.top

[D02] 追加元素到末尾
来源：http://txw.jlsjyb.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wdl.yuanzhike.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://vwd.9152youxi.cn

JS:   arr.push(4);
来源：http://lzb.gotoacloud.top

TS:   arr.push(4);
来源：http://tyb.andypj.xyz

Java: list.add(4);
来源：http://trw.ctjpmb.com

Go:   arr = append(arr, 4)
来源：http://cmc.xinyue.icu

Ruby: arr << 4; arr.push(5)
来源：http://ewz.ydzc1.top

C#:   list.Add(4);
来源：http://sxd.fengsongda.top

[D03] 在指定位置插入元素
来源：http://blv.ppjwa.cn

Py:   arr.insert(0, 0)
来源：http://uuy.sysykeji.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://lif.yuanzhike.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://pjs.jinghuilouyu.cn

TS:   arr.splice(0, 0, 0);
来源：http://iru.shuidangran.top

Java: list.add(0, 0);
来源：http://ogh.aizwys.cn

Go:   arr = append([]int{0}, arr...)
来源：http://kwk.tanke756.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ide.tian-w.cn

C#:   list.Insert(0, 0);
来源：http://pzw.fengsongda.top

[D04] 删除元素
来源：http://yqz.daria6918.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wxc.yj202588.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://nuj.c1oappe.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://tvb.dashuyun.cn

TS:   arr.splice(0, 1);
来源：http://rui.zhaomingkeji.xyz

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://bzc.quarkkingdee.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://qhg.fktsv.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://fkn.redwolf501.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://naa.52xcode.cn

[D05] 访问与修改元素
来源：http://sbj.c1oappe.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://sde.yueranfly.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://rke.yj202588.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://tme.gzhubu.top

TS:   arr[0]; arr.at(-1);
来源：http://qnh.hammf.cn

Java: list.get(0); list.set(0, 9);
来源：http://gyo.cashguo.top

Go:   arr[0]; arr[0] = 9
来源：http://ptj.shangyingyoupin.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://cjb.shzxlz.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://djj.tanke756.top

[D06] 数组长度
来源：http://qsz.shzxlz.cn

Py:   len(arr)
来源：http://dkk.vehdjk.com

PHP:  count($arr);
来源：http://gzq.aizwys.cn

JS:   arr.length
来源：http://cde.haohaochexian.top

TS:   arr.length
来源：http://zwi.kuanghao11.cn

Java: list.size();
来源：http://wpt.yangfankeji.com

Go:   len(arr)
来源：http://woy.xinyue.icu

Ruby: arr.length; arr.size
来源：http://gbe.haohaochexian.top

C#:   list.Count;
来源：http://tgi.svipenyu.cn

[D07] 切片 / 取子数组
来源：http://yrs.sysykeji.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mnd.sweek.top

PHP:  array_slice($arr, 1, 3);
来源：http://dnt.ctjpmb.com

JS:   arr.slice(1, 4);
来源：http://rzc.epnwcf.com

TS:   arr.slice(1, 4);
来源：http://uww.yanxiufei.cn

Java: list.subList(1, 4);
来源：http://cxi.yangfankeji.com

Go:   arr[1:4]
来源：http://eny.ppjwa.cn

Ruby: arr[1, 3]
来源：http://plx.zhongyouzk.top

C#:   list.GetRange(1, 3);
来源：http://lcn.0kj1m.cn

[D08] 合并两个数组
来源：http://joc.yj20258.top

Py:   a + b;  a.extend(b)
来源：http://bpz.wangdashe.top

PHP:  array_merge($a, $b);
来源：http://nuz.tianlin.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://rdu.tianlin.xyz

TS:   [...a, ...b];
来源：http://fag.yonumen.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hhp.sjlbkw.cn

Go:   append(a, b...)
来源：http://qen.yangfankeji.com

Ruby: a + b;  a.concat(b)
来源：http://npm.9152youxi.cn

C#:   a.Concat(b).ToList()
来源：http://hns.zhixingplan.top

[D09] 排序（升序）
来源：http://idr.jinghuilouyu.cn

Py:   sorted(arr);  arr.sort()
来源：http://xkq.jyoumei.cn

PHP:  sort($arr);
来源：http://mfe.hywenlv.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://xhg.daxiang520.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://wnj.hywenlv.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://hon.ydjk.org.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://fbl.chenlongwang.top

Ruby: arr.sort
来源：http://rsw.shuidangran.top

C#:   list.Sort();
来源：http://pii.shzxlz.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://svn.shzxlz.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://whw.zhaomingkeji.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ejb.yj20258.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://fvz.zhijiandao.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://dbv.cucudq.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://znk.tanke756.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://fiy.yueranfly.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://est.ywan-chungtsiang.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://dqe.ctjpmb.com

[D11] 反转数组
来源：http://wsz.jinghuilouyu.cn

Py:   arr[::-1];  arr.reverse()
来源：http://pzv.pycfn.com

PHP:  array_reverse($arr);
来源：http://hdi.gaohongyu789.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://saz.0kj1m.cn

TS:   [...arr].reverse();
来源：http://zzd.hnqzz.top

Java: Collections.reverse(list);
来源：http://mcw.wangdashe.top

Go:   slices.Reverse(arr)
来源：http://uhv.yonumen.top

Ruby: arr.reverse
来源：http://qyk.xuetiantiany.cn

C#:   list.Reverse();
来源：http://mfs.sjlbkw.cn

[D12] 查找元素下标
来源：http://fco.yvedp.cn

Py:   arr.index(x);  x in arr
来源：http://gtv.316326.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://djd.tianlin.xyz

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mdv.hywenlv.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rke.ybcxt.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wuh.wangdashe.top

Go:   slices.Index(arr, x)
来源：http://yrz.yangfankeji.com

Ruby: arr.index(x)
来源：http://prl.havefunace.top

C#:   list.IndexOf(x);
来源：http://wyc.guowangkeji.top

[D13] 过滤（保留满足条件的）
来源：http://hqw.shzxlz.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://dzp.zhiwuduotai.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://rhq.sweek.top

JS:   arr.filter(x => x > 3)
来源：http://lne.nanxuanxn.top

TS:   arr.filter(x => x > 3)
来源：http://oll.xylfe.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://trs.jinyuanbaomall.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ire.yuxming.cn

Ruby: arr.select { |x| x > 3 }
来源：http://jyp.cashguo.top

C#:   list.Where(x => x > 3).ToList()
来源：http://nfv.jyoumei.cn

[D14] 映射转换（每个元素变形）
来源：http://bqo.9152youxi.cn


<!-- 参考信息 -->