代发 wailian999

================================================================================
来源：http://syd.ivvv.top

C. 函数与作用域
来源：http://amm.mhx1999.top

================================================================================
来源：http://sln.guannengcc.top

[C01] 定义函数
来源：http://yam.pycfn.com

Py:   def add(a, b): return a + b
来源：http://xjn.quarkkingdee.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zzs.shuidangran.top

JS:   function add(a, b) { return a + b; }
来源：http://ouv.shuidangran.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cti.fengsongda.top

Java: static int add(int a, int b) { return a + b; }
来源：http://paq.nanxuanxn.top

Go:   func add(a, b int) int { return a + b }
来源：http://dom.hywenlv.cn

Ruby: def add(a, b); a + b; end
来源：http://ije.fzhhl.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://gtg.zdqjudy.top

[C02] 默认参数
来源：http://vfl.c1oappe.top

Py:   def greet(name="World"): return name
来源：http://zhy.316326.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://xkb.tanke756.top

JS:   function greet(name = "World") { return name; }
来源：http://gjm.hcnkem.com

TS:   function greet(name: string = "World") { return name; }
来源：http://swk.cashguo.top

Java: // 无默认参数：方法重载或 Optional
来源：http://mtl.svipenyu.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://icd.guannengcc.top

Ruby: def greet(name = "World") = name
来源：http://mem.tarul.cn

C#:   string Greet(string name = "World") => name;
来源：http://nhj.jinghuilouyu.cn

[C03] 可变参数
来源：http://rwf.jyoumei.cn

Py:   def total(*args): return sum(args)
来源：http://brw.hysaishi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://quh.hfpthk.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://jti.gotoacloud.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://lrv.daria6918.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://tgg.fanxiaobao.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://tzr.yuanzhike.top

Ruby: def total(*nums); nums.sum; end
来源：http://wmx.tarul.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mqb.bjfxy.top

[C04] 命名参数 / 关键字参数
来源：http://xbh.gzhubu.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://qqd.vehdjk.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://fag.zhaomingkeji.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://vau.zhaomingkeji.xyz

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://his.ivvv.top

Java: // 无：用 Builder 模式或 record
来源：http://rxn.ywan-chungtsiang.top

Go:   // 无：用配置结构体参数
来源：http://vdi.fengsongda.top

Ruby: f(a: 1, b: 2)
来源：http://mrr.redwolf501.top

C#:   f(a: 1, b: 2)
来源：http://ple.gotoacloud.top

[C05] 返回多个值
来源：http://lvv.fengsongda.top

Py:   return a, b
来源：http://ibe.zdbjq.cn

PHP:  return [$a, $b];
来源：http://lwk.uphjek.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://erw.cheryme.top

TS:   return { a, b };
来源：http://mto.haohaochexian.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xpy.hnxiangtu.top

Go:   return a, b
来源：http://pph.bbcook.cn

Ruby: return a, b
来源：http://ely.gotoacloud.top

C#:   return (a, b);              // ValueTuple
来源：http://yef.redwolf501.top

[C06] 匿名函数 / lambda
来源：http://lua.0kj1m.cn

Py:   square = lambda x: x * x
来源：http://quz.fanxiaobao.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://dev.haohaochexian.top

JS:   const square = x => x * x;
来源：http://eqf.snrcjt.cn

TS:   const square = (x: number): number => x * x;
来源：http://fva.yvedp.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://rjx.cheryme.top

Go:   sq := func(x int) int { return x * x }
来源：http://jsu.zdqjudy.top

Ruby: square = ->(x) { x * x }
来源：http://vrf.zdqjudy.top

C#:   Func<int, int> square = x => x * x;
来源：http://und.hcnkem.com

[C07] 把函数作为参数传入
来源：http://udz.zhijiandao.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://zho.guowangkeji.top

PHP:  array_map("strtoupper", $arr);
来源：http://jsl.ydjk.org.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://aal.havefunace.top

TS:   arr.map(String)
来源：http://dfz.xinyue.icu

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://qmv.redwolf501.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://tvp.tian-w.cn

Ruby: arr.map(&:upcase)
来源：http://oti.yuxming.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://cyc.daria6918.cn

[C08] 闭包
来源：http://jmz.ydjk.org.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://avd.zhengqikj.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://odj.316326.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://lha.nwbrower.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://nkq.hywenlv.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://iiy.wangshuangyany.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://inz.yanxiufei.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://bhz.jiagoushi.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ngp.zhaomingkeji.xyz

[C09] 递归
来源：http://hqq.iojbl.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wtm.9152youxi.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://yty.fanxiaobao.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dgi.dianchejie.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sst.zhongyouzk.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://qve.vehdjk.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://pnp.ehwqpu.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://tre.feifeiyinyue.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://fxf.dianchejie.cn

[C10] 变量作用域
来源：http://qdk.fktsv.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://vsk.zdqjudy.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://env.yj20258888.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://alk.hesvh.cn

TS:   同 JS
来源：http://kea.zhengqikj.top

Java: 方法内为块级作用域
来源：http://odp.zdbjq.cn

Go:   花括号块级作用域
来源：http://rwm.jqgfzy.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://rje.hammf.cn

C#:   块级作用域
来源：http://yjv.jinqigfzy.top

[C11] 模块导入与导出
来源：http://mct.yangfankeji.com

Py:   from module import func
来源：http://bhj.yuxming.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://hhi.chenjidiqi.icu

JS:   export default function f() {};  import f from "./m.js";
来源：http://unx.jlsjyb.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://fmn.shanyushiyangtech.top

Java: import java.util.List;
来源：http://snr.tanke756.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ueh.c1oappe.top

Ruby: require "json"; require_relative "./util"
来源：http://ffe.aizwys.cn

C#:   using System.Text;
来源：http://rlh.yj202588.top

[C12] 立即执行函数 IIFE
来源：http://soz.xylfe.cn

Py:   (lambda: print("run"))()
来源：http://vvk.xuanzx.com

PHP:  (function () { echo "run"; })();
来源：http://tqc.aizwys.cn

JS:   (() => { console.log("run"); })();
来源：http://wcz.xuanzx.com

TS:   (() => { console.log("run"); })();
来源：http://azl.sufxvd.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wri.zhongyouzk.top

Go:   func() { fmt.Println("run") }()
来源：http://vxg.zdqjudy.top

Ruby: -> { puts "run" }.call
来源：http://cuu.guowangkeji.top

C#:   // 无 IIFE：用静态构造函数
来源：http://wdj.cucudq.cn

[C13] 类型声明 / 类型注解
来源：http://lgt.9152youxi.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://esl.tianlin.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dmz.yvedp.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://era.yj202588.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gcd.ivvv.top

Java: int add(int a, int b) { return a + b; }
来源：http://iit.quarkkingdee.top

Go:   func add(a, b int) int
来源：http://szr.cqqwz.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://zuw.cheryme.top

C#:   int Add(int a, int b) => a + b;
来源：http://vcn.yfazqb.com

[C14] 泛型函数
来源：http://eyy.chenjidiqi.icu

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ibn.jianghu66.top

PHP:  // 无泛型
来源：http://ovv.tarul.cn

JS:   // 无泛型
来源：http://mxb.jinqigufen.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://gxp.ybcxt.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://gmt.epnwcf.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://afg.zhiwuduotai.top

Ruby: # 无泛型
来源：http://nqv.shzxlz.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://dly.xingfuxueyuan.xyz

[C15] 解构 / 展开参数
来源：http://ego.redwolf501.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mtj.hesvh.cn

PHP:  [$a, $b] = $pair;
来源：http://kuf.yonumen.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://nzm.xinyue.icu

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://bmb.aizwys.cn

Java: // 无解构
来源：http://mpo.sweek.top

Go:   // 无解构
来源：http://pmq.yuxming.cn

Ruby: a, b = pair
来源：http://uzf.yuanzhike.top

C#:   var (a, b) = pair;
来源：http://hvd.yonumen.top

[C16] 函数 / 方法重载
来源：http://iaf.zhijiandao.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://eyn.fktsv.cn

PHP:  // 无重载
来源：http://suk.chenlongwang.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://owp.quarkkingdee.top

TS:   // 用联合类型或重载签名声明
来源：http://jof.tarul.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://exi.tian-w.cn

Go:   // 无重载：用不同函数名
来源：http://efd.hywenlv.cn

Ruby: # 无重载：靠动态参数
来源：http://jcz.yongpay.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://bfy.c1oappe.top

================================================================================
来源：http://wtt.dianchejie.cn

D. 数组 / 列表 / 集合
来源：http://sme.shangyingyoupin.top

================================================================================
来源：http://ltm.sysykeji.top

[D01] 创建数组 / 列表
来源：http://zsr.sjlbkw.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://zom.xinyue.icu

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://xfp.cashguo.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://tmb.svipenyu.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://bgh.fanxiaobao.xyz

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://exr.gzhubu.top

Go:   arr := []int{1, 2, 3}
来源：http://bdu.xylfe.cn

Ruby: arr = [1, 2, 3]
来源：http://slo.fktsv.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://gxr.jqgfzy.top

[D02] 追加元素到末尾
来源：http://kvt.jinqigufen.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hcn.tarul.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://qad.jinqigufen.top

JS:   arr.push(4);
来源：http://kaa.daxiang520.top

TS:   arr.push(4);
来源：http://fml.gzhubu.top

Java: list.add(4);
来源：http://cbg.ppjwa.cn

Go:   arr = append(arr, 4)
来源：http://hmr.yuanzhike.top

Ruby: arr << 4; arr.push(5)
来源：http://xim.yonumen.top

C#:   list.Add(4);
来源：http://jca.jianghu66.top

[D03] 在指定位置插入元素
来源：http://fxb.jinqigfzy.top

Py:   arr.insert(0, 0)
来源：http://gqi.cashguo.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wgv.tianlin.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://too.hfpthk.cn

TS:   arr.splice(0, 0, 0);
来源：http://igg.shzxlz.cn

Java: list.add(0, 0);
来源：http://bwy.daxiang520.top

Go:   arr = append([]int{0}, arr...)
来源：http://dre.kuanghao11.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://usy.yfazqb.com

C#:   list.Insert(0, 0);
来源：http://pwf.ivvv.top

[D04] 删除元素
来源：http://lug.ywan-chungtsiang.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hvr.mhx1999.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://qpg.gzhubu.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://haf.0kj1m.cn

TS:   arr.splice(0, 1);
来源：http://wzg.ivvv.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://pck.yueranfly.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://jpk.epnwcf.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://oox.jyoumei.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://sms.kuanghao11.cn

[D05] 访问与修改元素
来源：http://pkg.quarkkingdee.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://qmv.yonumen.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hos.havefunace.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://cly.jinghuilouyu.cn

TS:   arr[0]; arr.at(-1);
来源：http://cxq.nwbrower.top

Java: list.get(0); list.set(0, 9);
来源：http://oev.sysykeji.top

Go:   arr[0]; arr[0] = 9
来源：http://gqw.chenzaomai.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://nnb.52xcode.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://jsi.vqdsnc.cn

[D06] 数组长度
来源：http://uvu.yueranfly.top

Py:   len(arr)
来源：http://cgc.hammf.cn

PHP:  count($arr);
来源：http://mum.52xcode.cn

JS:   arr.length
来源：http://xwh.xuanzx.com

TS:   arr.length
来源：http://osi.cdnleiting.top

Java: list.size();
来源：http://lwu.ctjpmb.com

Go:   len(arr)
来源：http://gnz.jlsjyb.cn

Ruby: arr.length; arr.size
来源：http://pxw.guannengcc.top

C#:   list.Count;
来源：http://jbc.zycfv.cn

[D07] 切片 / 取子数组
来源：http://vnh.kuanghao11.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://pfc.gotoacloud.top

PHP:  array_slice($arr, 1, 3);
来源：http://pvp.aibaodan.cn

JS:   arr.slice(1, 4);
来源：http://gig.nanxinkj.top

TS:   arr.slice(1, 4);
来源：http://fer.yueranfly.top

Java: list.subList(1, 4);
来源：http://ffx.yueranfly.top

Go:   arr[1:4]
来源：http://bsf.zhaomingkeji.xyz

Ruby: arr[1, 3]
来源：http://fnm.c1oappe.top

C#:   list.GetRange(1, 3);
来源：http://sag.guannengcc.top

[D08] 合并两个数组
来源：http://dfv.havefunace.top

Py:   a + b;  a.extend(b)
来源：http://dgn.havefunace.top

PHP:  array_merge($a, $b);
来源：http://obu.epnwcf.com

JS:   [...a, ...b];  a.concat(b);
来源：http://zhu.epnwcf.com

TS:   [...a, ...b];
来源：http://rvi.mhx1999.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://apd.vehdjk.com

Go:   append(a, b...)
来源：http://udr.ybcxt.top

Ruby: a + b;  a.concat(b)
来源：http://vmo.chenlongwang.top

C#:   a.Concat(b).ToList()
来源：http://yic.zdqjudy.top

[D09] 排序（升序）
来源：http://yjw.yueranfly.top

Py:   sorted(arr);  arr.sort()
来源：http://hmn.meibo888.top

PHP:  sort($arr);
来源：http://pbp.jinyuanbaomall.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://skl.zhijiandao.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ple.pengpengdd.cyou

Java: Collections.sort(list);  list.sort(null);
来源：http://sav.zhiwuduotai.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://xzj.zdqjudy.top

Ruby: arr.sort
来源：http://bbi.shangyingyoupin.top

C#:   list.Sort();
来源：http://ucu.zhixingplan.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://gyx.pengpengdd.cyou

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://sga.bjfxy.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ebg.mhx1999.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://cyb.xylfe.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://veh.zhaomingkeji.xyz

Java: list.sort(Comparator.comparing(Person::age));
来源：http://efw.shuidangran.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://fff.yueranfly.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://znn.9152youxi.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://zat.fehbvm.com

[D11] 反转数组
来源：http://ncr.iojbl.cn

Py:   arr[::-1];  arr.reverse()
来源：http://rdr.vqdsnc.cn

PHP:  array_reverse($arr);
来源：http://odr.ctjpmb.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://adx.sxryk.cn

TS:   [...arr].reverse();
来源：http://xqa.wangdashe.top

Java: Collections.reverse(list);
来源：http://vbt.jqgfzy.top

Go:   slices.Reverse(arr)
来源：http://ukz.shuidangran.top

Ruby: arr.reverse
来源：http://kpt.hywenlv.cn

C#:   list.Reverse();
来源：http://zog.cashguo.top

[D12] 查找元素下标
来源：http://tjd.wangshuangyany.cn

Py:   arr.index(x);  x in arr
来源：http://xjo.pycfn.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mvn.shangyingyoupin.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fuv.sweek.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zub.daxiang520.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://byh.bbcook.cn

Go:   slices.Index(arr, x)
来源：http://ayg.zhongyouzk.top

Ruby: arr.index(x)
来源：http://asd.vqdsnc.cn

C#:   list.IndexOf(x);
来源：http://ugz.nwbrower.top

[D13] 过滤（保留满足条件的）
来源：http://omp.sysykeji.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://eyp.nanxinkj.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://rzu.chenzaomai.com

JS:   arr.filter(x => x > 3)
来源：http://gyg.jiagoushi.top

TS:   arr.filter(x => x > 3)
来源：http://qdu.iojbl.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ksg.fktsv.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ljx.ppjwa.cn

Ruby: arr.select { |x| x > 3 }
来源：http://yft.jinghuilouyu.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://uvg.redwolf501.top

[D14] 映射转换（每个元素变形）
来源：http://gwt.nwbrower.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://dez.ivvv.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://jfs.aibaodan.cn

JS:   arr.map(x => x * 2)
来源：http://yai.pycfn.com

TS:   arr.map(x => x * 2)
来源：http://gxe.zhoulong.xyz

Java: list.stream().map(x -> x * 2).toList()
来源：http://knn.sjlbkw.cn

Go:   // 手写循环
来源：http://zyk.shuidangran.top

Ruby: arr.map { |x| x * 2 }
来源：http://cqg.hfpthk.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ngi.yongpay.top

[D15] 去重
来源：http://uif.haohaochexian.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ith.smart0.xyz

PHP:  array_unique($arr);
来源：http://jjt.hammf.cn

JS:   [...new Set(arr)]
来源：http://ehm.316326.xyz

TS:   [...new Set(arr)]
来源：http://uvq.jinqigufen.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://rig.xziqi.cn

Go:   // 用 map[T]struct{} 手写
来源：http://gra.bjfxy.top

Ruby: arr.uniq
来源：http://kjm.zhijiandao.cn

C#:   list.Distinct().ToList()
来源：http://nxw.jinqigfzy.top

[D16] 求和与平均值
来源：http://lmu.pycfn.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://bvw.quarkkingdee.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hra.jlsjyb.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://atl.zdbjq.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ylf.ywan-chungtsiang.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://bkm.jinghuilouyu.cn

Go:   // 手写循环累加
来源：http://qeb.birdmap.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mep.ydjk.org.cn

C#:   list.Sum();  list.Average()
来源：http://xpg.andypj.xyz

[D17] 最大值与最小值
来源：http://eit.yuanzhike.top

Py:   max(arr);  min(arr)
来源：http://hux.shzxlz.cn

PHP:  max($arr);  min($arr);
来源：http://dhw.ctjpmb.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://gnn.gogol.net.cn

TS:   Math.max(...arr);
来源：http://kik.shuidangran.top

Java: Collections.max(list);  Collections.min(list);
来源：http://ydf.shangyingyoupin.top


<!-- 参考信息 -->