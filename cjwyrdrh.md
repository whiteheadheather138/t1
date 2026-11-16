代发 wailian999

JS:   [1, 2, 3].includes(x)
来源：http://hmz.jlsjyb.cn

TS:   [1, 2, 3].includes(x)
来源：http://rpu.gogol.net.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://gac.daxiang520.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://lxm.sufxvd.cn

Ruby: [1, 2, 3].include?(x)
来源：http://gux.fanxiaobao.xyz

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://fvg.vehdjk.com

[B15] 布尔运算与取反
来源：http://hzy.jinqigufen.top

Py:   a and b or not c
来源：http://yme.ehwqpu.com

PHP:  $a && $b || !$c
来源：http://ilj.hysaishi.cn

JS:   a && b || !c
来源：http://ier.gaohongyu789.top

TS:   a && b || !c
来源：http://plh.bjfxy.top

Java: a && b || !c
来源：http://cme.svipenyu.cn

Go:   a && b || !c
来源：http://ppw.quarkkingdee.top

Ruby: a && b || !c
来源：http://kle.ydjk.org.cn

C#:   a && b || !c
来源：http://hth.cashguo.top

[B16] 卫语句：不满足条件提前返回
来源：http://xsj.fehbvm.com

Py:   if not data: return
来源：http://dmb.zhongyouzk.top

PHP:  if (!$data) { return; }
来源：http://tsu.tarul.cn

JS:   if (!data) return;
来源：http://pfh.ywan-chungtsiang.top

TS:   if (!data) return;
来源：http://zyo.zhoulong.xyz

Java: if (data == null) return;
来源：http://bdu.feifeiyinyue.top

Go:   if data == nil { return }
来源：http://krq.hammf.cn

Ruby: return if data.nil?
来源：http://rvk.hnxiangtu.top

C#:   if (data == null) return;
来源：http://yuq.andypj.xyz

================================================================================
来源：http://knt.zdbjq.cn

C. 函数与作用域
来源：http://lyn.guannengcc.top

================================================================================
来源：http://qik.hesvh.cn

[C01] 定义函数
来源：http://xcu.svipenyu.cn

Py:   def add(a, b): return a + b
来源：http://imw.sjlbkw.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wjm.hongshengwenyu.top

JS:   function add(a, b) { return a + b; }
来源：http://khc.yj20258.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fkh.vqdsnc.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://jda.xziqi.cn

Go:   func add(a, b int) int { return a + b }
来源：http://xml.hfpthk.cn

Ruby: def add(a, b); a + b; end
来源：http://vke.jinqigufen.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://chi.chenlongwang.top

[C02] 默认参数
来源：http://lbk.chenjidiqi.icu

Py:   def greet(name="World"): return name
来源：http://tfs.sufxvd.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://eea.kuanghao11.cn

JS:   function greet(name = "World") { return name; }
来源：http://rtb.yj20258.top

TS:   function greet(name: string = "World") { return name; }
来源：http://frq.nanxuanxn.top

Java: // 无默认参数：方法重载或 Optional
来源：http://mgx.aibaodan.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hph.jlsjyb.cn

Ruby: def greet(name = "World") = name
来源：http://sig.shanyushiyangkeji.top

C#:   string Greet(string name = "World") => name;
来源：http://tho.cdnleiting.top

[C03] 可变参数
来源：http://eix.hnqzz.top

Py:   def total(*args): return sum(args)
来源：http://hhm.bjfxy.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wtw.yfazqb.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://fmy.jiagoushi.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://yxe.gogol.net.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://zrz.yvedp.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://uik.dashuyun.cn

Ruby: def total(*nums); nums.sum; end
来源：http://fpa.yj20258.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ozq.hesvh.cn

[C04] 命名参数 / 关键字参数
来源：http://kxl.hammf.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://rvj.ehwqpu.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://yhz.dianchejie.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://nwp.nwbrower.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hso.bjfxy.top

Java: // 无：用 Builder 模式或 record
来源：http://wkt.cdnleiting.top

Go:   // 无：用配置结构体参数
来源：http://lsx.uphjek.com

Ruby: f(a: 1, b: 2)
来源：http://syu.zhijiandao.cn

C#:   f(a: 1, b: 2)
来源：http://hsl.cashguo.top

[C05] 返回多个值
来源：http://vng.zycfv.cn

Py:   return a, b
来源：http://ifg.xziqi.cn

PHP:  return [$a, $b];
来源：http://eip.zhiwuduotai.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://rgl.iojbl.cn

TS:   return { a, b };
来源：http://njc.quarkkingdee.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://uso.ppjwa.cn

Go:   return a, b
来源：http://cuv.52xcode.cn

Ruby: return a, b
来源：http://ssx.0kj1m.cn

C#:   return (a, b);              // ValueTuple
来源：http://cyg.xuanzx.com

[C06] 匿名函数 / lambda
来源：http://lej.shzxlz.cn

Py:   square = lambda x: x * x
来源：http://ghm.yj202588.top

PHP:  $square = fn($x) => $x * $x;
来源：http://ezv.hongshengwenyu.top

JS:   const square = x => x * x;
来源：http://cys.0kj1m.cn

TS:   const square = (x: number): number => x * x;
来源：http://ewe.hnqzz.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://edr.snrcjt.cn

Go:   sq := func(x int) int { return x * x }
来源：http://zvt.haohaochexian.top

Ruby: square = ->(x) { x * x }
来源：http://acn.fengsongda.top

C#:   Func<int, int> square = x => x * x;
来源：http://kes.ehwqpu.com

[C07] 把函数作为参数传入
来源：http://wtm.zhoulong.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://kjz.chenjidiqi.icu

PHP:  array_map("strtoupper", $arr);
来源：http://loo.yj20258.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://bew.fktsv.cn

TS:   arr.map(String)
来源：http://mfk.vehdjk.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://fhe.shanyushiyangtech.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://plz.cheryme.top

Ruby: arr.map(&:upcase)
来源：http://dpt.xinyue.icu

C#:   arr.Select(s => s.ToUpper())
来源：http://kyx.0kj1m.cn

[C08] 闭包
来源：http://lmo.tian-w.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://jub.yanxiufei.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://jgo.9152youxi.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ooy.aizwys.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://fbr.chenlongwang.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ppo.yj20258888.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://dqi.quarkkingdee.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://kqk.zhoulong.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://lxe.yj20258.top

[C09] 递归
来源：http://xcn.wangdashe.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://aie.nanxuanxn.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://dng.andypj.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://aub.sysykeji.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yrm.52xcode.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://cyt.zhijiandao.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://kjm.xuanzx.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://trh.nanxinkj.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://nii.yuanzhike.top

[C10] 变量作用域
来源：http://owu.jqgufenzy.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://pie.jinyuanbaomall.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://iiv.mhx1999.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://pwp.cdnleiting.top

TS:   同 JS
来源：http://kqt.c1oappe.top

Java: 方法内为块级作用域
来源：http://cwf.pycfn.com

Go:   花括号块级作用域
来源：http://gye.yongpay.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wqp.pengpengdd.cyou

C#:   块级作用域
来源：http://wuj.ydjk.org.cn

[C11] 模块导入与导出
来源：http://dbh.daria6918.cn

Py:   from module import func
来源：http://req.316326.xyz

PHP:  require "file.php";  或 use App\Service;
来源：http://tzi.yanxiufei.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://izx.uphjek.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://yej.hammf.cn

Java: import java.util.List;
来源：http://nxu.yvedp.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://rbe.zhiwuduotai.top

Ruby: require "json"; require_relative "./util"
来源：http://phu.yuxming.cn

C#:   using System.Text;
来源：http://fgq.tianlin.xyz

[C12] 立即执行函数 IIFE
来源：http://ltz.0kj1m.cn

Py:   (lambda: print("run"))()
来源：http://uhs.bbcook.cn

PHP:  (function () { echo "run"; })();
来源：http://qig.redwolf501.top

JS:   (() => { console.log("run"); })();
来源：http://coq.wangshuangyany.cn

TS:   (() => { console.log("run"); })();
来源：http://ijb.gotoacloud.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://uen.yongpay.top

Go:   func() { fmt.Println("run") }()
来源：http://dbg.yongpay.top

Ruby: -> { puts "run" }.call
来源：http://yia.fengsongda.top

C#:   // 无 IIFE：用静态构造函数
来源：http://aul.fengsongda.top

[C13] 类型声明 / 类型注解
来源：http://ewx.fktsv.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://tny.hfpthk.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fjb.fanxiaobao.xyz

JS:   // 无类型（可用 JSDoc 注释）
来源：http://dvr.xingfuxueyuan.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nye.ivvv.top

Java: int add(int a, int b) { return a + b; }
来源：http://egf.zhoulong.xyz

Go:   func add(a, b int) int
来源：http://szx.cqqwz.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://chd.ctjpmb.com

C#:   int Add(int a, int b) => a + b;
来源：http://hkz.cucudq.cn

[C14] 泛型函数
来源：http://ayn.vqdsnc.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://utw.havefunace.top

PHP:  // 无泛型
来源：http://trc.fengsongda.top

JS:   // 无泛型
来源：http://zcx.bbcook.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://fwf.hysaishi.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mba.jqgfzy.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://nkp.zhongyouzk.top

Ruby: # 无泛型
来源：http://nfg.sjlbkw.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://rjh.zhiwuduotai.top

[C15] 解构 / 展开参数
来源：http://drn.nanxinkj.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xdj.xziqi.cn

PHP:  [$a, $b] = $pair;
来源：http://fme.gzhubu.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://qrj.daxiang520.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://srq.ydjk.org.cn

Java: // 无解构
来源：http://rgw.uphjek.com

Go:   // 无解构
来源：http://mte.bjfxy.top

Ruby: a, b = pair
来源：http://kbr.svipenyu.cn

C#:   var (a, b) = pair;
来源：http://xum.sysykeji.top

[C16] 函数 / 方法重载
来源：http://zum.zdqjudy.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ofy.gaohongyu789.top

PHP:  // 无重载
来源：http://sko.hywenlv.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://hvn.xylfe.cn

TS:   // 用联合类型或重载签名声明
来源：http://rxl.havefunace.top

Java: void f(int a) {}  void f(String a) {}
来源：http://lxj.chenjidiqi.icu

Go:   // 无重载：用不同函数名
来源：http://bjs.shangyingyoupin.top

Ruby: # 无重载：靠动态参数
来源：http://rpb.cdnleiting.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://cwz.smart0.xyz

================================================================================
来源：http://baz.hnxiangtu.top

D. 数组 / 列表 / 集合
来源：http://kub.yj202588.top

================================================================================
来源：http://vjx.c1oappe.top

[D01] 创建数组 / 列表
来源：http://ems.zdbjq.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://odw.shangyingyoupin.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://cjq.xuanzx.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://rdj.ywan-chungtsiang.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://epq.shuidangran.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://nuk.52xcode.cn

Go:   arr := []int{1, 2, 3}
来源：http://nqj.xinyue.icu

Ruby: arr = [1, 2, 3]
来源：http://zms.cheryme.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://cpp.xylfe.cn

[D02] 追加元素到末尾
来源：http://sww.yueranfly.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://xoh.jinyuanbaomall.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://esi.cdnleiting.top

JS:   arr.push(4);
来源：http://zxx.uphjek.com

TS:   arr.push(4);
来源：http://jdp.feifeiyinyue.top

Java: list.add(4);
来源：http://pzq.dashuyun.cn

Go:   arr = append(arr, 4)
来源：http://jme.daria6918.cn

Ruby: arr << 4; arr.push(5)
来源：http://edx.yueranfly.top

C#:   list.Add(4);
来源：http://hkp.xuetiantiany.cn

[D03] 在指定位置插入元素
来源：http://bfs.ppjwa.cn

Py:   arr.insert(0, 0)
来源：http://yzn.hammf.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://enh.xuetiantiany.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://oxj.ydjk.org.cn

TS:   arr.splice(0, 0, 0);
来源：http://bdm.ywan-chungtsiang.top

Java: list.add(0, 0);
来源：http://cfs.gzhubu.top

Go:   arr = append([]int{0}, arr...)
来源：http://fmq.xinyue.icu

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hjo.yongpay.top

C#:   list.Insert(0, 0);
来源：http://pxh.wangdashe.top

[D04] 删除元素
来源：http://mbl.shanyushiyangkeji.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ggr.shuidangran.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hhw.316326.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://deo.guannengcc.top

TS:   arr.splice(0, 1);
来源：http://yeu.yueranfly.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://zle.jyoumei.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://vfy.zdbjq.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://zgm.hammf.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ymm.guannengcc.top

[D05] 访问与修改元素
来源：http://ajw.xziqi.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://sop.xuetiantiany.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://dyk.jyoumei.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://qjx.cheryme.top

TS:   arr[0]; arr.at(-1);
来源：http://gps.gotoacloud.top

Java: list.get(0); list.set(0, 9);
来源：http://gjy.jinqigufen.top

Go:   arr[0]; arr[0] = 9
来源：http://hyf.yj20258.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://elp.vqdsnc.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://rbk.52xcode.cn

[D06] 数组长度
来源：http://sbf.xuanzx.com

Py:   len(arr)
来源：http://lhh.zycfv.cn

PHP:  count($arr);
来源：http://wap.jlsjyb.cn

JS:   arr.length
来源：http://kzz.meibo888.top

TS:   arr.length
来源：http://cgs.nwbrower.top

Java: list.size();
来源：http://xmw.9152youxi.cn

Go:   len(arr)
来源：http://xmc.yongpay.top

Ruby: arr.length; arr.size
来源：http://xyb.ehwqpu.com

C#:   list.Count;
来源：http://yiw.cqqwz.cn

[D07] 切片 / 取子数组
来源：http://crn.yueranfly.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://jdv.pengpengdd.cyou

PHP:  array_slice($arr, 1, 3);
来源：http://pok.yueranfly.top

JS:   arr.slice(1, 4);
来源：http://rtj.tian-w.cn

TS:   arr.slice(1, 4);
来源：http://bps.tanke756.top

Java: list.subList(1, 4);
来源：http://cqk.wangshuangyany.cn

Go:   arr[1:4]
来源：http://kui.shangyingyoupin.top

Ruby: arr[1, 3]
来源：http://fqw.shanyushiyangtech.top

C#:   list.GetRange(1, 3);
来源：http://gdn.sweek.top

[D08] 合并两个数组
来源：http://wyf.daria6918.cn

Py:   a + b;  a.extend(b)
来源：http://tge.smart0.xyz

PHP:  array_merge($a, $b);
来源：http://qzf.cashguo.top

JS:   [...a, ...b];  a.concat(b);
来源：http://jxv.aibaodan.cn

TS:   [...a, ...b];
来源：http://zpy.jqgufenzy.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://zyd.zhixingplan.top

Go:   append(a, b...)
来源：http://olj.c1oappe.top

Ruby: a + b;  a.concat(b)
来源：http://pds.bjfxy.top

C#:   a.Concat(b).ToList()
来源：http://ptr.ehwqpu.com

[D09] 排序（升序）
来源：http://exf.yj20258888.top

Py:   sorted(arr);  arr.sort()
来源：http://aeg.yj20258.top

PHP:  sort($arr);
来源：http://tbq.hnxiangtu.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://qde.c1oappe.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://fph.jinyuanbaomall.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://hmf.zdqjudy.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://vyz.ywan-chungtsiang.top

Ruby: arr.sort
来源：http://jgx.pengpengdd.cyou

C#:   list.Sort();
来源：http://fzn.ybcxt.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://whr.vehdjk.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://vpt.hywenlv.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tbz.xinyue.icu

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://vqd.yongpay.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://koy.hongshengwenyu.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://tdc.yangfankeji.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://zdu.c1oappe.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://rxz.316326.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wxl.feifeiyinyue.top

[D11] 反转数组
来源：http://mfr.316326.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://jnc.jinqigufen.top

PHP:  array_reverse($arr);
来源：http://oqv.gaohongyu789.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qqv.cucudq.cn

TS:   [...arr].reverse();
来源：http://zhp.shuidangran.top

Java: Collections.reverse(list);
来源：http://pys.xinyue.icu

Go:   slices.Reverse(arr)
来源：http://suo.zhaomingkeji.xyz

Ruby: arr.reverse
来源：http://pmb.nwbrower.top

C#:   list.Reverse();
来源：http://myo.ehwqpu.com

[D12] 查找元素下标
来源：http://gbf.xuanzx.com

Py:   arr.index(x);  x in arr
来源：http://xrp.c1oappe.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://qel.0kj1m.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://unh.hesvh.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://iek.hnqzz.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mtp.sxryk.cn

Go:   slices.Index(arr, x)
来源：http://wyx.fengsongda.top

Ruby: arr.index(x)
来源：http://vwh.vqdsnc.cn

C#:   list.IndexOf(x);
来源：http://wui.jiagoushi.top

[D13] 过滤（保留满足条件的）
来源：http://apt.andypj.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://dpi.jinyuanbaomall.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://dnf.andypj.xyz

JS:   arr.filter(x => x > 3)
来源：http://wdh.gogol.net.cn

TS:   arr.filter(x => x > 3)
来源：http://yem.dianchejie.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://igq.hnqzz.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://qco.shanyushiyangtech.top

Ruby: arr.select { |x| x > 3 }
来源：http://ilw.zhaomingkeji.xyz

C#:   list.Where(x => x > 3).ToList()
来源：http://ggj.sxryk.cn

[D14] 映射转换（每个元素变形）
来源：http://uhs.pengpengdd.cyou

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://zlw.ywan-chungtsiang.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://evj.guannengcc.top

JS:   arr.map(x => x * 2)
来源：http://liw.jlsjyb.cn

TS:   arr.map(x => x * 2)
来源：http://fnp.andypj.xyz

Java: list.stream().map(x -> x * 2).toList()
来源：http://akb.sufxvd.cn

Go:   // 手写循环
来源：http://pvf.yvedp.cn

Ruby: arr.map { |x| x * 2 }
来源：http://dal.yanxiufei.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ydh.hcnkem.com


<!-- 参考信息 -->