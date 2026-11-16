代发 wailian999

C#:   x is int or double or decimal
来源：http://czk.guowangkeji.top

[B14] 判断值是否在集合内
来源：http://pxd.yangfankeji.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://amg.fehbvm.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://vnz.xinyue.icu

JS:   [1, 2, 3].includes(x)
来源：http://woa.jqgufenzy.top

TS:   [1, 2, 3].includes(x)
来源：http://gvu.zhongyouzk.top

Java: List.of(1, 2, 3).contains(x)
来源：http://onu.ehwqpu.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://tpn.shangyingyoupin.top

Ruby: [1, 2, 3].include?(x)
来源：http://dcn.aibaodan.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://eji.jiagoushi.top

[B15] 布尔运算与取反
来源：http://prv.yongpay.top

Py:   a and b or not c
来源：http://pze.hysaishi.cn

PHP:  $a && $b || !$c
来源：http://bxl.jyoumei.cn

JS:   a && b || !c
来源：http://zsw.birdmap.top

TS:   a && b || !c
来源：http://sxn.52xcode.cn

Java: a && b || !c
来源：http://aky.havefunace.top

Go:   a && b || !c
来源：http://quu.haohaochexian.top

Ruby: a && b || !c
来源：http://cnq.jinqigfzy.top

C#:   a && b || !c
来源：http://mge.hnxiangtu.top

[B16] 卫语句：不满足条件提前返回
来源：http://wwh.ehwqpu.com

Py:   if not data: return
来源：http://jll.pengpengdd.cyou

PHP:  if (!$data) { return; }
来源：http://uik.tarul.cn

JS:   if (!data) return;
来源：http://gff.sysykeji.top

TS:   if (!data) return;
来源：http://odn.svipenyu.cn

Java: if (data == null) return;
来源：http://hab.vehdjk.com

Go:   if data == nil { return }
来源：http://xhl.jinyuanbaomall.cn

Ruby: return if data.nil?
来源：http://pxv.jianghu66.top

C#:   if (data == null) return;
来源：http://lvu.sysykeji.top

================================================================================
来源：http://pui.cqqwz.cn

C. 函数与作用域
来源：http://gqc.zhijiandao.cn

================================================================================
来源：http://tyn.gogol.net.cn

[C01] 定义函数
来源：http://grb.yueranfly.top

Py:   def add(a, b): return a + b
来源：http://apv.shanyushiyangtech.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://siv.xuetiantiany.cn

JS:   function add(a, b) { return a + b; }
来源：http://juo.nanxuanxn.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sbx.wangdashe.top

Java: static int add(int a, int b) { return a + b; }
来源：http://cmx.ppjwa.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ezt.bjfxy.top

Ruby: def add(a, b); a + b; end
来源：http://wcc.yueranfly.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://omw.fanxiaobao.xyz

[C02] 默认参数
来源：http://low.cashguo.top

Py:   def greet(name="World"): return name
来源：http://aff.xinyue.icu

PHP:  function greet($name = "World") { return $name; }
来源：http://dbw.xylfe.cn

JS:   function greet(name = "World") { return name; }
来源：http://xah.hongshengwenyu.top

TS:   function greet(name: string = "World") { return name; }
来源：http://pwo.jianghu66.top

Java: // 无默认参数：方法重载或 Optional
来源：http://lmp.uphjek.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://edy.bbcook.cn

Ruby: def greet(name = "World") = name
来源：http://bqc.ppjwa.cn

C#:   string Greet(string name = "World") => name;
来源：http://oof.jqgufenzy.top

[C03] 可变参数
来源：http://lux.ctjpmb.com

Py:   def total(*args): return sum(args)
来源：http://agt.nanxinkj.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mvo.meibo888.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://zxc.dashuyun.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ylv.sufxvd.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vim.guannengcc.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wti.nanxuanxn.top

Ruby: def total(*nums); nums.sum; end
来源：http://yor.xinyue.icu

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://fca.zhoulong.xyz

[C04] 命名参数 / 关键字参数
来源：http://iag.mhx1999.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://twm.jinqigufen.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://kxa.52xcode.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://tdv.jianghu66.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://qpq.aibaodan.cn

Java: // 无：用 Builder 模式或 record
来源：http://iur.fengsongda.top

Go:   // 无：用配置结构体参数
来源：http://qyn.yj20258888.top

Ruby: f(a: 1, b: 2)
来源：http://are.52xcode.cn

C#:   f(a: 1, b: 2)
来源：http://rrv.yfazqb.com

[C05] 返回多个值
来源：http://sen.daria6918.cn

Py:   return a, b
来源：http://mbi.quarkkingdee.top

PHP:  return [$a, $b];
来源：http://htc.ywan-chungtsiang.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://qlk.guowangkeji.top

TS:   return { a, b };
来源：http://ozn.zhaomingkeji.xyz

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://dnk.chenzaomai.com

Go:   return a, b
来源：http://mek.xingfuxueyuan.xyz

Ruby: return a, b
来源：http://ubx.hfpthk.cn

C#:   return (a, b);              // ValueTuple
来源：http://nua.tianlin.xyz

[C06] 匿名函数 / lambda
来源：http://biw.wangshuangyany.cn

Py:   square = lambda x: x * x
来源：http://bhc.yj20258888.top

PHP:  $square = fn($x) => $x * $x;
来源：http://pcr.zhiwuduotai.top

JS:   const square = x => x * x;
来源：http://pdj.shanyushiyangkeji.top

TS:   const square = (x: number): number => x * x;
来源：http://xyy.feifeiyinyue.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://plr.yj202588.top

Go:   sq := func(x int) int { return x * x }
来源：http://cdx.chenjidiqi.icu

Ruby: square = ->(x) { x * x }
来源：http://pkh.jyoumei.cn

C#:   Func<int, int> square = x => x * x;
来源：http://dag.yonumen.top

[C07] 把函数作为参数传入
来源：http://hnc.cqqwz.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://szp.shuidangran.top

PHP:  array_map("strtoupper", $arr);
来源：http://lbb.jinyuanbaomall.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://aij.cashguo.top

TS:   arr.map(String)
来源：http://fva.pycfn.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://zal.yanxiufei.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mrr.yonumen.top

Ruby: arr.map(&:upcase)
来源：http://sce.shuidangran.top

C#:   arr.Select(s => s.ToUpper())
来源：http://dlb.zhijiandao.cn

[C08] 闭包
来源：http://jgt.yuanzhike.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://lwb.pengpengdd.cyou

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ldz.ehwqpu.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://bop.hnxiangtu.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ivo.pengpengdd.cyou

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://tma.guannengcc.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://zeh.jinyuanbaomall.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://nfc.shangyingyoupin.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://zow.shanyushiyangtech.top

[C09] 递归
来源：http://yhv.shanyushiyangtech.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ijj.shzxlz.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://xds.jinyuanbaomall.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gdp.yonumen.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ilz.andypj.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mod.gzhubu.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://iap.sxryk.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://rtq.hnqzz.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ixw.chenzaomai.com

[C10] 变量作用域
来源：http://eca.yvedp.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://top.andypj.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://dqr.vehdjk.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://jzg.epnwcf.com

TS:   同 JS
来源：http://dbm.cheryme.top

Java: 方法内为块级作用域
来源：http://qxz.vehdjk.com

Go:   花括号块级作用域
来源：http://oco.fktsv.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://iur.shzxlz.cn

C#:   块级作用域
来源：http://tux.gotoacloud.top

[C11] 模块导入与导出
来源：http://ges.9152youxi.cn

Py:   from module import func
来源：http://ggi.xuetiantiany.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://yua.zycfv.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://vbj.uphjek.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://cxn.redwolf501.top

Java: import java.util.List;
来源：http://sni.hammf.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mcr.redwolf501.top

Ruby: require "json"; require_relative "./util"
来源：http://ccn.hfpthk.cn

C#:   using System.Text;
来源：http://xkz.jinyuanbaomall.cn

[C12] 立即执行函数 IIFE
来源：http://rwk.uphjek.com

Py:   (lambda: print("run"))()
来源：http://jkk.feifeiyinyue.top

PHP:  (function () { echo "run"; })();
来源：http://jbz.dashuyun.cn

JS:   (() => { console.log("run"); })();
来源：http://cvj.hnqzz.top

TS:   (() => { console.log("run"); })();
来源：http://smh.dashuyun.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://xgt.cdnleiting.top

Go:   func() { fmt.Println("run") }()
来源：http://uuu.sxryk.cn

Ruby: -> { puts "run" }.call
来源：http://cej.sysykeji.top

C#:   // 无 IIFE：用静态构造函数
来源：http://vaq.zhoulong.xyz

[C13] 类型声明 / 类型注解
来源：http://tqd.hnqzz.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://goq.ydzc1.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mkg.bbcook.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ezh.yangfankeji.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sru.tanke756.top

Java: int add(int a, int b) { return a + b; }
来源：http://zsc.uphjek.com

Go:   func add(a, b int) int
来源：http://psk.smart0.xyz

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://zjy.yvedp.cn

C#:   int Add(int a, int b) => a + b;
来源：http://scv.sxryk.cn

[C14] 泛型函数
来源：http://exv.zhijiandao.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://qkc.zhongyouzk.top

PHP:  // 无泛型
来源：http://wqr.jianghu66.top

JS:   // 无泛型
来源：http://hrc.jyoumei.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://kkt.xylfe.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://dmv.feifeiyinyue.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://rrq.ywan-chungtsiang.top

Ruby: # 无泛型
来源：http://xii.cashguo.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://irq.chenlongwang.top

[C15] 解构 / 展开参数
来源：http://ogs.bbcook.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://coh.epnwcf.com

PHP:  [$a, $b] = $pair;
来源：http://raa.pycfn.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://aay.guannengcc.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://dyl.yonumen.top

Java: // 无解构
来源：http://mqz.bjfxy.top

Go:   // 无解构
来源：http://cwg.xuanzx.com

Ruby: a, b = pair
来源：http://xrd.gotoacloud.top

C#:   var (a, b) = pair;
来源：http://jxr.yuxming.cn

[C16] 函数 / 方法重载
来源：http://eqj.tarul.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://exo.shanyushiyangtech.top

PHP:  // 无重载
来源：http://qoz.hnqzz.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://vdz.xziqi.cn

TS:   // 用联合类型或重载签名声明
来源：http://ade.hysaishi.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://wms.quarkkingdee.top

Go:   // 无重载：用不同函数名
来源：http://qsl.tian-w.cn

Ruby: # 无重载：靠动态参数
来源：http://qnk.shanyushiyangtech.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://azl.jlsjyb.cn

================================================================================
来源：http://qux.jianghu66.top

D. 数组 / 列表 / 集合
来源：http://oss.jlsjyb.cn

================================================================================
来源：http://xql.yueranfly.top

[D01] 创建数组 / 列表
来源：http://qvy.fehbvm.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://wfo.ppjwa.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ykc.yvedp.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://gvs.xuetiantiany.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://pwc.yvedp.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://pgk.sxryk.cn

Go:   arr := []int{1, 2, 3}
来源：http://upf.wangdashe.top

Ruby: arr = [1, 2, 3]
来源：http://avl.316326.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://edx.52xcode.cn

[D02] 追加元素到末尾
来源：http://sxv.sysykeji.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://aov.daxiang520.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://jsa.sufxvd.cn

JS:   arr.push(4);
来源：http://dhi.iojbl.cn

TS:   arr.push(4);
来源：http://rya.fzhhl.top

Java: list.add(4);
来源：http://ueo.tanke756.top

Go:   arr = append(arr, 4)
来源：http://fyv.shanyushiyangtech.top

Ruby: arr << 4; arr.push(5)
来源：http://kmk.chenzaomai.com

C#:   list.Add(4);
来源：http://mzd.cheryme.top

[D03] 在指定位置插入元素
来源：http://yna.svipenyu.cn

Py:   arr.insert(0, 0)
来源：http://hdw.chenlongwang.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://apm.yj20258888.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hed.chenzaomai.com

TS:   arr.splice(0, 0, 0);
来源：http://biy.hywenlv.cn

Java: list.add(0, 0);
来源：http://kal.xingfuxueyuan.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://vol.xinyue.icu

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://lio.hnxiangtu.top

C#:   list.Insert(0, 0);
来源：http://exb.yongpay.top

[D04] 删除元素
来源：http://fhf.guowangkeji.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://til.jinqigufen.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://xdx.zhoulong.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://qxo.xingfuxueyuan.xyz

TS:   arr.splice(0, 1);
来源：http://hrr.9152youxi.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ncd.xuanzx.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://cvc.birdmap.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://jix.smart0.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://elz.yuxming.cn

[D05] 访问与修改元素
来源：http://nht.shuidangran.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://vob.zycfv.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://uzm.gaohongyu789.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://lrd.xingfuxueyuan.xyz

TS:   arr[0]; arr.at(-1);
来源：http://mev.gogol.net.cn

Java: list.get(0); list.set(0, 9);
来源：http://fxl.yj20258.top

Go:   arr[0]; arr[0] = 9
来源：http://aew.wangdashe.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://tgb.nanxinkj.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://igh.gaohongyu789.top

[D06] 数组长度
来源：http://iqj.sweek.top

Py:   len(arr)
来源：http://oil.smart0.xyz

PHP:  count($arr);
来源：http://zzb.ehwqpu.com

JS:   arr.length
来源：http://dyb.cdnleiting.top

TS:   arr.length
来源：http://pab.epnwcf.com

Java: list.size();
来源：http://nhu.jqgufenzy.top

Go:   len(arr)
来源：http://qjg.zdbjq.cn

Ruby: arr.length; arr.size
来源：http://uab.guowangkeji.top

C#:   list.Count;
来源：http://idv.yanxiufei.cn

[D07] 切片 / 取子数组
来源：http://ywh.hywenlv.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://drc.bjfxy.top

PHP:  array_slice($arr, 1, 3);
来源：http://hri.jinqigfzy.top

JS:   arr.slice(1, 4);
来源：http://kmg.zhiwuduotai.top

TS:   arr.slice(1, 4);
来源：http://jrf.jqgufenzy.top

Java: list.subList(1, 4);
来源：http://bbd.iojbl.cn

Go:   arr[1:4]
来源：http://lou.hnqzz.top

Ruby: arr[1, 3]
来源：http://vro.sweek.top

C#:   list.GetRange(1, 3);
来源：http://zva.jianghu66.top

[D08] 合并两个数组
来源：http://agk.ydjk.org.cn

Py:   a + b;  a.extend(b)
来源：http://ejt.jiagoushi.top

PHP:  array_merge($a, $b);
来源：http://jsv.dianchejie.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://rks.ywan-chungtsiang.top

TS:   [...a, ...b];
来源：http://dmg.cashguo.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://snd.sweek.top

Go:   append(a, b...)
来源：http://cub.hysaishi.cn

Ruby: a + b;  a.concat(b)
来源：http://sth.quarkkingdee.top

C#:   a.Concat(b).ToList()
来源：http://cuk.xingfuxueyuan.xyz

[D09] 排序（升序）
来源：http://bpr.nwbrower.top

Py:   sorted(arr);  arr.sort()
来源：http://cga.xinyue.icu

PHP:  sort($arr);
来源：http://pan.tian-w.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://pos.jinghuilouyu.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ppl.svipenyu.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://gbm.cqqwz.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hsw.daria6918.cn

Ruby: arr.sort
来源：http://amh.9152youxi.cn

C#:   list.Sort();
来源：http://qjf.chenjidiqi.icu

[D10] 自定义排序（按字段 / 多条件）
来源：http://gdb.ybcxt.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://isl.yuxming.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mpn.pengpengdd.cyou

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hag.daria6918.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://iap.yongpay.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wpu.pengpengdd.cyou

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ufi.andypj.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://okr.yj20258888.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://tok.wangdashe.top

[D11] 反转数组
来源：http://kba.andypj.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://xxn.uphjek.com

PHP:  array_reverse($arr);
来源：http://wxf.gotoacloud.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://aly.yonumen.top

TS:   [...arr].reverse();
来源：http://jgn.birdmap.top

Java: Collections.reverse(list);
来源：http://bjx.meibo888.top

Go:   slices.Reverse(arr)
来源：http://hgw.smart0.xyz

Ruby: arr.reverse
来源：http://qzp.fehbvm.com

C#:   list.Reverse();
来源：http://bfx.hywenlv.cn

[D12] 查找元素下标
来源：http://xnh.c1oappe.top

Py:   arr.index(x);  x in arr
来源：http://fdv.yj202588.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://fnb.ydzc1.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ywr.vqdsnc.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://end.zhaomingkeji.xyz

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ncf.chenlongwang.top

Go:   slices.Index(arr, x)
来源：http://ohy.cashguo.top

Ruby: arr.index(x)
来源：http://pti.uphjek.com

C#:   list.IndexOf(x);
来源：http://mla.cqqwz.cn

[D13] 过滤（保留满足条件的）
来源：http://efk.jinghuilouyu.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://nfq.fehbvm.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://xzu.zhoulong.xyz

JS:   arr.filter(x => x > 3)
来源：http://eec.xuetiantiany.cn

TS:   arr.filter(x => x > 3)
来源：http://iez.hywenlv.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://jbi.hammf.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://qbg.ctjpmb.com

Ruby: arr.select { |x| x > 3 }
来源：http://dvf.0kj1m.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://njq.kuanghao11.cn

[D14] 映射转换（每个元素变形）
来源：http://urt.hnqzz.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://fgp.nwbrower.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vab.kuanghao11.cn

JS:   arr.map(x => x * 2)
来源：http://dpr.hysaishi.cn

TS:   arr.map(x => x * 2)
来源：http://rxn.kuanghao11.cn


<!-- 参考信息 -->