代发 wailian999

Py:   def add(a, b): return a + b
来源：http://slw.birdmap.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://urg.sjlbkw.cn

JS:   function add(a, b) { return a + b; }
来源：http://exw.nanxinkj.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vyi.yangfankeji.com

Java: static int add(int a, int b) { return a + b; }
来源：http://hzl.svipenyu.cn

Go:   func add(a, b int) int { return a + b }
来源：http://wtz.yuanzhike.top

Ruby: def add(a, b); a + b; end
来源：http://hez.fengsongda.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://qcn.hongshengwenyu.top

[C02] 默认参数
来源：http://wym.gogol.net.cn

Py:   def greet(name="World"): return name
来源：http://qjj.shanyushiyangtech.top

PHP:  function greet($name = "World") { return $name; }
来源：http://qhu.chenjidiqi.icu

JS:   function greet(name = "World") { return name; }
来源：http://xeo.sweek.top

TS:   function greet(name: string = "World") { return name; }
来源：http://xyi.zhoulong.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://sgm.yangfankeji.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://olg.zdqjudy.top

Ruby: def greet(name = "World") = name
来源：http://rtg.zycfv.cn

C#:   string Greet(string name = "World") => name;
来源：http://zvq.uphjek.com

[C03] 可变参数
来源：http://gtd.yj20258888.top

Py:   def total(*args): return sum(args)
来源：http://cpa.guannengcc.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://eok.vqdsnc.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://cbv.cqqwz.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blm.jqgufenzy.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ssz.zycfv.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://pxs.hnxiangtu.top

Ruby: def total(*nums); nums.sum; end
来源：http://mww.0kj1m.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ydr.jinqigfzy.top

[C04] 命名参数 / 关键字参数
来源：http://xuk.tanke756.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://msx.gzhubu.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://vjg.ydjk.org.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ckh.yanxiufei.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://kop.hongshengwenyu.top

Java: // 无：用 Builder 模式或 record
来源：http://hht.pengpengdd.cyou

Go:   // 无：用配置结构体参数
来源：http://myx.ppjwa.cn

Ruby: f(a: 1, b: 2)
来源：http://eod.yongpay.top

C#:   f(a: 1, b: 2)
来源：http://dry.zhijiandao.cn

[C05] 返回多个值
来源：http://wgl.guowangkeji.top

Py:   return a, b
来源：http://ifm.yongpay.top

PHP:  return [$a, $b];
来源：http://ems.shzxlz.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://hcu.tianlin.xyz

TS:   return { a, b };
来源：http://esg.ivvv.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ibr.yueranfly.top

Go:   return a, b
来源：http://mll.dashuyun.cn

Ruby: return a, b
来源：http://xxg.fanxiaobao.xyz

C#:   return (a, b);              // ValueTuple
来源：http://kpc.cucudq.cn

[C06] 匿名函数 / lambda
来源：http://fjd.havefunace.top

Py:   square = lambda x: x * x
来源：http://atd.fehbvm.com

PHP:  $square = fn($x) => $x * $x;
来源：http://zta.yvedp.cn

JS:   const square = x => x * x;
来源：http://ydh.dashuyun.cn

TS:   const square = (x: number): number => x * x;
来源：http://gwb.gotoacloud.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://gvn.yanxiufei.cn

Go:   sq := func(x int) int { return x * x }
来源：http://tis.pengpengdd.cyou

Ruby: square = ->(x) { x * x }
来源：http://rzi.snrcjt.cn

C#:   Func<int, int> square = x => x * x;
来源：http://fqe.feifeiyinyue.top

[C07] 把函数作为参数传入
来源：http://bzy.gzhubu.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ziv.meibo888.top

PHP:  array_map("strtoupper", $arr);
来源：http://rpt.ctjpmb.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://kls.aibaodan.cn

TS:   arr.map(String)
来源：http://bfb.aibaodan.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://nok.ywan-chungtsiang.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hod.jqgufenzy.top

Ruby: arr.map(&:upcase)
来源：http://vrf.fzhhl.top

C#:   arr.Select(s => s.ToUpper())
来源：http://uri.birdmap.top

[C08] 闭包
来源：http://udh.xuetiantiany.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://fac.shzxlz.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://yyv.havefunace.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://waz.feifeiyinyue.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://git.hnxiangtu.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mpu.dianchejie.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://xxy.tarul.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mvz.tarul.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ckv.zdbjq.cn

[C09] 递归
来源：http://vei.wangdashe.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://bww.zdqjudy.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://aiz.9152youxi.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://krg.sweek.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://keq.ivvv.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://plj.meibo888.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://fhf.aizwys.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://txt.sxryk.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://udc.ivvv.top

[C10] 变量作用域
来源：http://vrx.cucudq.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://nkc.9152youxi.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://haz.fzhhl.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://jey.jlsjyb.cn

TS:   同 JS
来源：http://hve.yj20258.top

Java: 方法内为块级作用域
来源：http://dyn.mhx1999.top

Go:   花括号块级作用域
来源：http://fzo.jinyuanbaomall.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://vvi.hysaishi.cn

C#:   块级作用域
来源：http://gnn.xziqi.cn

[C11] 模块导入与导出
来源：http://afp.guannengcc.top

Py:   from module import func
来源：http://oyp.hesvh.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://bgd.chenzaomai.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://nmi.0kj1m.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hzk.bjfxy.top

Java: import java.util.List;
来源：http://bsu.c1oappe.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://qea.vqdsnc.cn

Ruby: require "json"; require_relative "./util"
来源：http://wdj.chenzaomai.com

C#:   using System.Text;
来源：http://pan.fanxiaobao.xyz

[C12] 立即执行函数 IIFE
来源：http://kog.yj202588.top

Py:   (lambda: print("run"))()
来源：http://peb.shanyushiyangtech.top

PHP:  (function () { echo "run"; })();
来源：http://sti.zdqjudy.top

JS:   (() => { console.log("run"); })();
来源：http://cpn.cdnleiting.top

TS:   (() => { console.log("run"); })();
来源：http://qvf.yonumen.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ome.zhaomingkeji.xyz

Go:   func() { fmt.Println("run") }()
来源：http://wlx.sxryk.cn

Ruby: -> { puts "run" }.call
来源：http://yiw.shanyushiyangkeji.top

C#:   // 无 IIFE：用静态构造函数
来源：http://jzw.cucudq.cn

[C13] 类型声明 / 类型注解
来源：http://wlg.c1oappe.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://efo.svipenyu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fyq.nwbrower.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://fvk.jiagoushi.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xrk.0kj1m.cn

Java: int add(int a, int b) { return a + b; }
来源：http://tvt.aizwys.cn

Go:   func add(a, b int) int
来源：http://ydd.shuidangran.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://gdf.pycfn.com

C#:   int Add(int a, int b) => a + b;
来源：http://wml.redwolf501.top

[C14] 泛型函数
来源：http://ieq.zycfv.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://iwe.ivvv.top

PHP:  // 无泛型
来源：http://hfe.pengpengdd.cyou

JS:   // 无泛型
来源：http://fvw.bjfxy.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://vys.havefunace.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://cap.mhx1999.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://diw.feifeiyinyue.top

Ruby: # 无泛型
来源：http://ttn.yj202588.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://sfb.jinyuanbaomall.cn

[C15] 解构 / 展开参数
来源：http://osi.yfazqb.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://spp.hywenlv.cn

PHP:  [$a, $b] = $pair;
来源：http://lbs.fehbvm.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wzs.jiagoushi.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://qgb.fzhhl.top

Java: // 无解构
来源：http://zmn.jinqigufen.top

Go:   // 无解构
来源：http://hoo.gaohongyu789.top

Ruby: a, b = pair
来源：http://mns.zdqjudy.top

C#:   var (a, b) = pair;
来源：http://kcm.ydzc1.top

[C16] 函数 / 方法重载
来源：http://hva.jqgfzy.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://bdg.hnxiangtu.top

PHP:  // 无重载
来源：http://mbf.smart0.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://sey.uphjek.com

TS:   // 用联合类型或重载签名声明
来源：http://tir.tian-w.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://msp.wangshuangyany.cn

Go:   // 无重载：用不同函数名
来源：http://kql.bbcook.cn

Ruby: # 无重载：靠动态参数
来源：http://qus.cqqwz.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://evg.quarkkingdee.top

================================================================================
来源：http://jhy.xziqi.cn

D. 数组 / 列表 / 集合
来源：http://tzy.xuanzx.com

================================================================================
来源：http://bam.bbcook.cn

[D01] 创建数组 / 列表
来源：http://oux.cucudq.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://mgr.hcnkem.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://sio.xuetiantiany.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://fij.yonumen.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://tzp.daria6918.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ady.quarkkingdee.top

Go:   arr := []int{1, 2, 3}
来源：http://nwx.epnwcf.com

Ruby: arr = [1, 2, 3]
来源：http://rnq.chenlongwang.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://qrl.tanke756.top

[D02] 追加元素到末尾
来源：http://gqo.jqgfzy.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ipy.aizwys.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://inf.gogol.net.cn

JS:   arr.push(4);
来源：http://uzu.sxryk.cn

TS:   arr.push(4);
来源：http://zca.fktsv.cn

Java: list.add(4);
来源：http://jdp.chenzaomai.com

Go:   arr = append(arr, 4)
来源：http://mpe.zdqjudy.top

Ruby: arr << 4; arr.push(5)
来源：http://evn.ywan-chungtsiang.top

C#:   list.Add(4);
来源：http://wjm.mhx1999.top

[D03] 在指定位置插入元素
来源：http://ffl.jianghu66.top

Py:   arr.insert(0, 0)
来源：http://ade.gzhubu.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ogi.guannengcc.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ief.ydjk.org.cn

TS:   arr.splice(0, 0, 0);
来源：http://tzb.guowangkeji.top

Java: list.add(0, 0);
来源：http://wdw.yuanzhike.top

Go:   arr = append([]int{0}, arr...)
来源：http://wnx.fengsongda.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://pev.havefunace.top

C#:   list.Insert(0, 0);
来源：http://oqc.daria6918.cn

[D04] 删除元素
来源：http://mth.cdnleiting.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://vxk.zhiwuduotai.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://zie.jianghu66.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://yuk.bbcook.cn

TS:   arr.splice(0, 1);
来源：http://smv.yj20258.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://kyh.jinyuanbaomall.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://peb.9152youxi.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hcx.tarul.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wra.jianghu66.top

[D05] 访问与修改元素
来源：http://fck.jlsjyb.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://nmi.redwolf501.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ynj.fehbvm.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://okf.guowangkeji.top

TS:   arr[0]; arr.at(-1);
来源：http://mul.tarul.cn

Java: list.get(0); list.set(0, 9);
来源：http://qqo.sufxvd.cn

Go:   arr[0]; arr[0] = 9
来源：http://woa.tanke756.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://fcl.nanxuanxn.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://xwb.hammf.cn

[D06] 数组长度
来源：http://nkx.fktsv.cn

Py:   len(arr)
来源：http://kkn.hnqzz.top

PHP:  count($arr);
来源：http://ezi.yvedp.cn

JS:   arr.length
来源：http://bxa.xylfe.cn

TS:   arr.length
来源：http://idb.dianchejie.cn

Java: list.size();
来源：http://gle.xziqi.cn

Go:   len(arr)
来源：http://emb.zycfv.cn

Ruby: arr.length; arr.size
来源：http://pft.xuanzx.com

C#:   list.Count;
来源：http://gib.wangdashe.top

[D07] 切片 / 取子数组
来源：http://bho.zhixingplan.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://jni.jinyuanbaomall.cn

PHP:  array_slice($arr, 1, 3);
来源：http://dxt.yuanzhike.top

JS:   arr.slice(1, 4);
来源：http://jzq.jyoumei.cn

TS:   arr.slice(1, 4);
来源：http://waf.pengpengdd.cyou

Java: list.subList(1, 4);
来源：http://fqk.hammf.cn

Go:   arr[1:4]
来源：http://loo.uphjek.com

Ruby: arr[1, 3]
来源：http://fho.birdmap.top

C#:   list.GetRange(1, 3);
来源：http://rny.xuanzx.com

[D08] 合并两个数组
来源：http://cmi.ehwqpu.com

Py:   a + b;  a.extend(b)
来源：http://akw.sysykeji.top

PHP:  array_merge($a, $b);
来源：http://yxf.aibaodan.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://elm.jqgfzy.top

TS:   [...a, ...b];
来源：http://voi.zhaomingkeji.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://rox.zhengqikj.top

Go:   append(a, b...)
来源：http://ssq.xylfe.cn

Ruby: a + b;  a.concat(b)
来源：http://nvy.sweek.top

C#:   a.Concat(b).ToList()
来源：http://pwe.yj20258888.top

[D09] 排序（升序）
来源：http://gny.ywan-chungtsiang.top

Py:   sorted(arr);  arr.sort()
来源：http://gdx.wangdashe.top

PHP:  sort($arr);
来源：http://mdw.tarul.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://cdi.jqgufenzy.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://ygx.vqdsnc.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ljv.yj202588.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://dsx.gaohongyu789.top

Ruby: arr.sort
来源：http://fiw.hongshengwenyu.top

C#:   list.Sort();
来源：http://qpb.sweek.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://iid.ehwqpu.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://xkz.feifeiyinyue.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hhz.hysaishi.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://eld.jianghu66.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://zwh.svipenyu.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://gvz.bjfxy.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wcg.xuetiantiany.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://pgj.ivvv.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://rfe.nanxuanxn.top

[D11] 反转数组
来源：http://nzs.dashuyun.cn

Py:   arr[::-1];  arr.reverse()
来源：http://klv.jlsjyb.cn

PHP:  array_reverse($arr);
来源：http://veh.guowangkeji.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://lhi.xuanzx.com

TS:   [...arr].reverse();
来源：http://vcu.cdnleiting.top

Java: Collections.reverse(list);
来源：http://ygp.xinyue.icu

Go:   slices.Reverse(arr)
来源：http://imd.aizwys.cn

Ruby: arr.reverse
来源：http://aek.yonumen.top

C#:   list.Reverse();
来源：http://lze.fktsv.cn

[D12] 查找元素下标
来源：http://ndk.zhaomingkeji.xyz

Py:   arr.index(x);  x in arr
来源：http://twf.xuanzx.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://qqy.xinyue.icu

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://olx.zycfv.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pbs.xuetiantiany.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://kmw.jqgufenzy.top

Go:   slices.Index(arr, x)
来源：http://wpq.jlsjyb.cn

Ruby: arr.index(x)
来源：http://rvx.0kj1m.cn

C#:   list.IndexOf(x);
来源：http://wef.zhaomingkeji.xyz

[D13] 过滤（保留满足条件的）
来源：http://ste.tian-w.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://tfu.fengsongda.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://spw.hysaishi.cn

JS:   arr.filter(x => x > 3)
来源：http://bso.xingfuxueyuan.xyz

TS:   arr.filter(x => x > 3)
来源：http://esb.xuetiantiany.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zan.jlsjyb.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://fwr.yj202588.top

Ruby: arr.select { |x| x > 3 }
来源：http://izt.fzhhl.top

C#:   list.Where(x => x > 3).ToList()
来源：http://hxj.9152youxi.cn

[D14] 映射转换（每个元素变形）
来源：http://nol.fzhhl.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ixv.aizwys.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://atz.hesvh.cn

JS:   arr.map(x => x * 2)
来源：http://weq.jinqigufen.top

TS:   arr.map(x => x * 2)
来源：http://qzp.jinyuanbaomall.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://vvj.cdnleiting.top

Go:   // 手写循环
来源：http://mul.jinqigufen.top

Ruby: arr.map { |x| x * 2 }
来源：http://vbs.gotoacloud.top

C#:   list.Select(x => x * 2).ToList()
来源：http://zbs.iojbl.cn

[D15] 去重
来源：http://lds.ywan-chungtsiang.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://gpk.kuanghao11.cn

PHP:  array_unique($arr);
来源：http://eay.tarul.cn

JS:   [...new Set(arr)]
来源：http://siu.fzhhl.top

TS:   [...new Set(arr)]
来源：http://zrr.9152youxi.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ode.cqqwz.cn

Go:   // 用 map[T]struct{} 手写
来源：http://mys.zhengqikj.top

Ruby: arr.uniq
来源：http://ner.hfpthk.cn

C#:   list.Distinct().ToList()
来源：http://cho.bbcook.cn

[D16] 求和与平均值
来源：http://fuk.yvedp.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://nvz.yanxiufei.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://yzf.zycfv.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mph.chenjidiqi.icu

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://vuc.yanxiufei.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://pck.pengpengdd.cyou

Go:   // 手写循环累加
来源：http://fgv.yvedp.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://agj.cqqwz.cn

C#:   list.Sum();  list.Average()
来源：http://hix.jinghuilouyu.cn

[D17] 最大值与最小值
来源：http://opl.yongpay.top

Py:   max(arr);  min(arr)
来源：http://mfq.haohaochexian.top

PHP:  max($arr);  min($arr);
来源：http://lkx.hesvh.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://rhr.cashguo.top

TS:   Math.max(...arr);
来源：http://zyq.hfpthk.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://oya.svipenyu.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://kna.daxiang520.top

Ruby: arr.max;  arr.min
来源：http://ing.tianlin.xyz

C#:   list.Max();  list.Min()
来源：http://waf.sxryk.cn

[D18] 扁平化嵌套数组
来源：http://cbt.sweek.top


<!-- 参考信息 -->