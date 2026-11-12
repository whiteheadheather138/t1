代发 wailian999

Go:   a && b || !c
来源：http://ogc.zhongyouzk.top

Ruby: a && b || !c
来源：http://wvc.chenlongwang.top

C#:   a && b || !c
来源：http://szr.wangshuangyany.cn

[B16] 卫语句：不满足条件提前返回
来源：http://lnv.vqdsnc.cn

Py:   if not data: return
来源：http://ilx.guowangkeji.top

PHP:  if (!$data) { return; }
来源：http://ktu.quarkkingdee.top

JS:   if (!data) return;
来源：http://kjo.tarul.cn

TS:   if (!data) return;
来源：http://iwa.cheryme.top

Java: if (data == null) return;
来源：http://dls.cdnleiting.top

Go:   if data == nil { return }
来源：http://jyw.yueranfly.top

Ruby: return if data.nil?
来源：http://tad.chenlongwang.top

C#:   if (data == null) return;
来源：http://lhp.tian-w.cn

================================================================================
来源：http://hcy.shanyushiyangtech.top

C. 函数与作用域
来源：http://box.ydzc1.top

================================================================================
来源：http://lsd.vehdjk.com

[C01] 定义函数
来源：http://kwo.yanxiufei.cn

Py:   def add(a, b): return a + b
来源：http://aka.zhijiandao.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fqw.xylfe.cn

JS:   function add(a, b) { return a + b; }
来源：http://qet.xingfuxueyuan.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sen.fengsongda.top

Java: static int add(int a, int b) { return a + b; }
来源：http://hee.316326.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://kvl.zhaomingkeji.xyz

Ruby: def add(a, b); a + b; end
来源：http://gxc.bbcook.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ylw.jqgfzy.top

[C02] 默认参数
来源：http://rkb.dashuyun.cn

Py:   def greet(name="World"): return name
来源：http://aqm.havefunace.top

PHP:  function greet($name = "World") { return $name; }
来源：http://vxr.gzhubu.top

JS:   function greet(name = "World") { return name; }
来源：http://aaf.zdqjudy.top

TS:   function greet(name: string = "World") { return name; }
来源：http://nle.jianghu66.top

Java: // 无默认参数：方法重载或 Optional
来源：http://kxz.yueranfly.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wsk.fzhhl.top

Ruby: def greet(name = "World") = name
来源：http://izs.yanxiufei.cn

C#:   string Greet(string name = "World") => name;
来源：http://hdo.chenlongwang.top

[C03] 可变参数
来源：http://cgw.fehbvm.com

Py:   def total(*args): return sum(args)
来源：http://rmy.hywenlv.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hlj.hywenlv.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://owz.ivvv.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://kkn.gzhubu.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://xaq.andypj.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://kya.tanke756.top

Ruby: def total(*nums); nums.sum; end
来源：http://xuw.zhengqikj.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://cxn.yueranfly.top

[C04] 命名参数 / 关键字参数
来源：http://gco.jinghuilouyu.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mvz.gotoacloud.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://rth.wangshuangyany.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://dxn.pycfn.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://vqo.xylfe.cn

Java: // 无：用 Builder 模式或 record
来源：http://ral.0kj1m.cn

Go:   // 无：用配置结构体参数
来源：http://gpb.daria6918.cn

Ruby: f(a: 1, b: 2)
来源：http://med.zhijiandao.cn

C#:   f(a: 1, b: 2)
来源：http://zac.wangdashe.top

[C05] 返回多个值
来源：http://bso.shuidangran.top

Py:   return a, b
来源：http://lbx.yuanzhike.top

PHP:  return [$a, $b];
来源：http://szl.yangfankeji.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://jgr.wangdashe.top

TS:   return { a, b };
来源：http://kah.quarkkingdee.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://iny.mhx1999.top

Go:   return a, b
来源：http://ftq.nwbrower.top

Ruby: return a, b
来源：http://knd.xuanzx.com

C#:   return (a, b);              // ValueTuple
来源：http://dsi.yvedp.cn

[C06] 匿名函数 / lambda
来源：http://yac.andypj.xyz

Py:   square = lambda x: x * x
来源：http://wyz.jinqigufen.top

PHP:  $square = fn($x) => $x * $x;
来源：http://hwv.vehdjk.com

JS:   const square = x => x * x;
来源：http://zoc.zhaomingkeji.xyz

TS:   const square = (x: number): number => x * x;
来源：http://ljf.jinqigfzy.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://cxa.tarul.cn

Go:   sq := func(x int) int { return x * x }
来源：http://qeh.sjlbkw.cn

Ruby: square = ->(x) { x * x }
来源：http://vne.yvedp.cn

C#:   Func<int, int> square = x => x * x;
来源：http://awj.xuetiantiany.cn

[C07] 把函数作为参数传入
来源：http://dtg.ydzc1.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wls.zdqjudy.top

PHP:  array_map("strtoupper", $arr);
来源：http://yuq.yj20258.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://sxw.hammf.cn

TS:   arr.map(String)
来源：http://gdv.ydzc1.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://yzy.tian-w.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ykb.hesvh.cn

Ruby: arr.map(&:upcase)
来源：http://oru.hesvh.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://zwc.fehbvm.com

[C08] 闭包
来源：http://gfp.fktsv.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://fwf.yvedp.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://uow.birdmap.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vsx.vehdjk.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://vxk.smart0.xyz

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://run.daria6918.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://bva.uphjek.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://uqo.jiagoushi.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ydp.sysykeji.top

[C09] 递归
来源：http://eyd.xingfuxueyuan.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://izf.guowangkeji.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://qzw.fehbvm.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://acb.cheryme.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mtm.andypj.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://yrq.chenjidiqi.icu

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://gdy.c1oappe.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://txb.smart0.xyz

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hwt.chenjidiqi.icu

[C10] 变量作用域
来源：http://mlk.daria6918.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://kqv.gogol.net.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://nzd.fzhhl.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://qog.tianlin.xyz

TS:   同 JS
来源：http://dpl.sxryk.cn

Java: 方法内为块级作用域
来源：http://gtv.daria6918.cn

Go:   花括号块级作用域
来源：http://nbf.yfazqb.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://zjr.guannengcc.top

C#:   块级作用域
来源：http://wva.zdqjudy.top

[C11] 模块导入与导出
来源：http://bqi.epnwcf.com

Py:   from module import func
来源：http://bzw.cdnleiting.top

PHP:  require "file.php";  或 use App\Service;
来源：http://kle.gzhubu.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://owb.snrcjt.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://snx.jianghu66.top

Java: import java.util.List;
来源：http://nqk.feifeiyinyue.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://bwq.sjlbkw.cn

Ruby: require "json"; require_relative "./util"
来源：http://cer.shanyushiyangtech.top

C#:   using System.Text;
来源：http://zjf.quarkkingdee.top

[C12] 立即执行函数 IIFE
来源：http://thf.yuxming.cn

Py:   (lambda: print("run"))()
来源：http://pvv.yuanzhike.top

PHP:  (function () { echo "run"; })();
来源：http://ndi.zhaomingkeji.xyz

JS:   (() => { console.log("run"); })();
来源：http://uhc.chenjidiqi.icu

TS:   (() => { console.log("run"); })();
来源：http://hze.sufxvd.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wyx.gogol.net.cn

Go:   func() { fmt.Println("run") }()
来源：http://qzt.xylfe.cn

Ruby: -> { puts "run" }.call
来源：http://xgg.cqqwz.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://fgo.316326.xyz

[C13] 类型声明 / 类型注解
来源：http://foq.yongpay.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://nvf.jinyuanbaomall.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://swm.nwbrower.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://eoo.epnwcf.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lix.jinghuilouyu.cn

Java: int add(int a, int b) { return a + b; }
来源：http://xun.andypj.xyz

Go:   func add(a, b int) int
来源：http://tmv.hammf.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://xek.chenjidiqi.icu

C#:   int Add(int a, int b) => a + b;
来源：http://imc.hongshengwenyu.top

[C14] 泛型函数
来源：http://brf.yfazqb.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hgh.cashguo.top

PHP:  // 无泛型
来源：http://lkh.9152youxi.cn

JS:   // 无泛型
来源：http://cep.shuidangran.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://nlr.havefunace.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://qxp.andypj.xyz

Go:   func First[T any](items []T) T { return items[0] }
来源：http://izp.chenzaomai.com

Ruby: # 无泛型
来源：http://jqt.zycfv.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://bev.quarkkingdee.top

[C15] 解构 / 展开参数
来源：http://xqv.gaohongyu789.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://zwd.chenlongwang.top

PHP:  [$a, $b] = $pair;
来源：http://bod.jinyuanbaomall.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://qoe.yuxming.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://kef.0kj1m.cn

Java: // 无解构
来源：http://pwf.fanxiaobao.xyz

Go:   // 无解构
来源：http://xow.dianchejie.cn

Ruby: a, b = pair
来源：http://ann.cdnleiting.top

C#:   var (a, b) = pair;
来源：http://ocp.tanke756.top

[C16] 函数 / 方法重载
来源：http://whw.havefunace.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wlr.ctjpmb.com

PHP:  // 无重载
来源：http://kcp.snrcjt.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://jrr.zhaomingkeji.xyz

TS:   // 用联合类型或重载签名声明
来源：http://aid.hongshengwenyu.top

Java: void f(int a) {}  void f(String a) {}
来源：http://yrx.mhx1999.top

Go:   // 无重载：用不同函数名
来源：http://ikn.yvedp.cn

Ruby: # 无重载：靠动态参数
来源：http://avk.zdqjudy.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://fxp.svipenyu.cn

================================================================================
来源：http://zem.jlsjyb.cn

D. 数组 / 列表 / 集合
来源：http://ezp.cucudq.cn

================================================================================
来源：http://lxg.pycfn.com

[D01] 创建数组 / 列表
来源：http://xfp.andypj.xyz

Py:   arr = [1, 2, 3];  empty = []
来源：http://ope.yueranfly.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://bza.aibaodan.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://met.jqgfzy.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://ypl.gotoacloud.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://yan.guannengcc.top

Go:   arr := []int{1, 2, 3}
来源：http://tgx.xingfuxueyuan.xyz

Ruby: arr = [1, 2, 3]
来源：http://okg.bjfxy.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hmm.yvedp.cn

[D02] 追加元素到末尾
来源：http://don.cucudq.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://inz.chenjidiqi.icu

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ogc.jianghu66.top

JS:   arr.push(4);
来源：http://dkn.yj20258.top

TS:   arr.push(4);
来源：http://enj.daria6918.cn

Java: list.add(4);
来源：http://eif.jqgfzy.top

Go:   arr = append(arr, 4)
来源：http://iuq.fehbvm.com

Ruby: arr << 4; arr.push(5)
来源：http://vqt.jqgfzy.top

C#:   list.Add(4);
来源：http://rrp.wangshuangyany.cn

[D03] 在指定位置插入元素
来源：http://vgv.hfpthk.cn

Py:   arr.insert(0, 0)
来源：http://aui.hfpthk.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://fnt.ydzc1.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://jnq.hysaishi.cn

TS:   arr.splice(0, 0, 0);
来源：http://lnx.tianlin.xyz

Java: list.add(0, 0);
来源：http://yqs.gzhubu.top

Go:   arr = append([]int{0}, arr...)
来源：http://eay.iojbl.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hhx.havefunace.top

C#:   list.Insert(0, 0);
来源：http://wpi.zhixingplan.top

[D04] 删除元素
来源：http://oec.zhiwuduotai.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ghf.aibaodan.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://kmo.hnxiangtu.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xcd.fehbvm.com

TS:   arr.splice(0, 1);
来源：http://gus.tarul.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://tpv.yvedp.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://tsq.bbcook.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://cpx.hnxiangtu.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://yss.jinqigufen.top

[D05] 访问与修改元素
来源：http://nib.xingfuxueyuan.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://lds.birdmap.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://pja.yj20258888.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://lao.yfazqb.com

TS:   arr[0]; arr.at(-1);
来源：http://wli.cashguo.top

Java: list.get(0); list.set(0, 9);
来源：http://apo.hammf.cn

Go:   arr[0]; arr[0] = 9
来源：http://kis.yongpay.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://kqk.zdbjq.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://qar.0kj1m.cn

[D06] 数组长度
来源：http://bdv.hfpthk.cn

Py:   len(arr)
来源：http://jls.yuanzhike.top

PHP:  count($arr);
来源：http://ems.cheryme.top

JS:   arr.length
来源：http://idy.yj20258.top

TS:   arr.length
来源：http://fop.aibaodan.cn

Java: list.size();
来源：http://otr.zhijiandao.cn

Go:   len(arr)
来源：http://gnx.yonumen.top

Ruby: arr.length; arr.size
来源：http://hnq.chenjidiqi.icu

C#:   list.Count;
来源：http://dpp.nanxinkj.top

[D07] 切片 / 取子数组
来源：http://kbn.jlsjyb.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wjy.yonumen.top

PHP:  array_slice($arr, 1, 3);
来源：http://rmn.jiagoushi.top

JS:   arr.slice(1, 4);
来源：http://ueg.yj20258.top

TS:   arr.slice(1, 4);
来源：http://zbo.nwbrower.top

Java: list.subList(1, 4);
来源：http://upy.sxryk.cn

Go:   arr[1:4]
来源：http://hwn.jqgufenzy.top

Ruby: arr[1, 3]
来源：http://jec.xinyue.icu

C#:   list.GetRange(1, 3);
来源：http://vzd.tian-w.cn

[D08] 合并两个数组
来源：http://nyt.aibaodan.cn

Py:   a + b;  a.extend(b)
来源：http://brt.jyoumei.cn

PHP:  array_merge($a, $b);
来源：http://wnx.fktsv.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://nlt.xinyue.icu

TS:   [...a, ...b];
来源：http://jjc.tianlin.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://jer.guannengcc.top

Go:   append(a, b...)
来源：http://lze.gogol.net.cn

Ruby: a + b;  a.concat(b)
来源：http://nsp.sxryk.cn

C#:   a.Concat(b).ToList()
来源：http://rym.nanxuanxn.top

[D09] 排序（升序）
来源：http://xel.xziqi.cn

Py:   sorted(arr);  arr.sort()
来源：http://tap.ydzc1.top

PHP:  sort($arr);
来源：http://vsu.ppjwa.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hfc.yj20258.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://zsi.ydjk.org.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://xrp.bjfxy.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wxe.bjfxy.top

Ruby: arr.sort
来源：http://iif.shuidangran.top

C#:   list.Sort();
来源：http://okt.gaohongyu789.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://mow.xinyue.icu

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qul.havefunace.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bts.jiagoushi.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://dry.shangyingyoupin.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://txt.zhongyouzk.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://zcs.dashuyun.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ppj.hnqzz.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://txe.yongpay.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://chg.0kj1m.cn

[D11] 反转数组
来源：http://aqv.ctjpmb.com

Py:   arr[::-1];  arr.reverse()
来源：http://xfr.zhiwuduotai.top

PHP:  array_reverse($arr);
来源：http://fkq.daxiang520.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://awm.chenlongwang.top

TS:   [...arr].reverse();
来源：http://mxb.yvedp.cn

Java: Collections.reverse(list);
来源：http://sof.c1oappe.top

Go:   slices.Reverse(arr)
来源：http://kdh.smart0.xyz

Ruby: arr.reverse
来源：http://lqz.nanxinkj.top

C#:   list.Reverse();
来源：http://naa.yanxiufei.cn

[D12] 查找元素下标
来源：http://wad.jqgufenzy.top

Py:   arr.index(x);  x in arr
来源：http://aea.sweek.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://huq.redwolf501.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://isu.zhengqikj.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qmu.gaohongyu789.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mxa.ppjwa.cn

Go:   slices.Index(arr, x)
来源：http://qfp.aizwys.cn

Ruby: arr.index(x)
来源：http://xtr.bbcook.cn

C#:   list.IndexOf(x);
来源：http://nse.iojbl.cn

[D13] 过滤（保留满足条件的）
来源：http://plv.yvedp.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ajm.hnxiangtu.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://oyd.zhiwuduotai.top

JS:   arr.filter(x => x > 3)
来源：http://eux.yuanzhike.top

TS:   arr.filter(x => x > 3)
来源：http://zbc.kuanghao11.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://int.jinqigfzy.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://vrx.vqdsnc.cn

Ruby: arr.select { |x| x > 3 }
来源：http://xfi.52xcode.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://fyl.tianlin.xyz

[D14] 映射转换（每个元素变形）
来源：http://aoi.zhongyouzk.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://enx.mhx1999.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://fou.yuxming.cn

JS:   arr.map(x => x * 2)
来源：http://kdg.yuanzhike.top

TS:   arr.map(x => x * 2)
来源：http://ncl.ctjpmb.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://zfq.xuanzx.com

Go:   // 手写循环
来源：http://glb.daxiang520.top

Ruby: arr.map { |x| x * 2 }
来源：http://rwz.xinyue.icu

C#:   list.Select(x => x * 2).ToList()
来源：http://wlp.yj202588.top

[D15] 去重
来源：http://hfg.ppjwa.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://bpc.zhaomingkeji.xyz

PHP:  array_unique($arr);
来源：http://xwy.xinyue.icu

JS:   [...new Set(arr)]
来源：http://qlb.fengsongda.top

TS:   [...new Set(arr)]
来源：http://oma.cdnleiting.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://kds.jinqigufen.top

Go:   // 用 map[T]struct{} 手写
来源：http://qfp.zycfv.cn

Ruby: arr.uniq
来源：http://qsl.tian-w.cn

C#:   list.Distinct().ToList()
来源：http://rzf.guowangkeji.top

[D16] 求和与平均值
来源：http://dnd.jinqigufen.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://thy.vehdjk.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://tpw.fktsv.cn


<!-- 参考信息 -->