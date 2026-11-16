代发 wailian999

Java: static int add(int a, int b) { return a + b; }
来源：http://kcc.pengpengdd.cyou

Go:   func add(a, b int) int { return a + b }
来源：http://vfe.yuanzhike.top

Ruby: def add(a, b); a + b; end
来源：http://vec.smart0.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://tod.tarul.cn

[C02] 默认参数
来源：http://sbk.wangshuangyany.cn

Py:   def greet(name="World"): return name
来源：http://hum.dianchejie.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://obt.kuanghao11.cn

JS:   function greet(name = "World") { return name; }
来源：http://ypn.jqgfzy.top

TS:   function greet(name: string = "World") { return name; }
来源：http://vzb.jqgufenzy.top

Java: // 无默认参数：方法重载或 Optional
来源：http://ttq.yonumen.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://fns.tian-w.cn

Ruby: def greet(name = "World") = name
来源：http://sdg.ybcxt.top

C#:   string Greet(string name = "World") => name;
来源：http://kve.gzhubu.top

[C03] 可变参数
来源：http://bbj.shanyushiyangtech.top

Py:   def total(*args): return sum(args)
来源：http://rcj.dashuyun.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://urp.vqdsnc.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://qnx.shanyushiyangkeji.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://epu.daria6918.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://rxm.jlsjyb.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://jzp.wangdashe.top

Ruby: def total(*nums); nums.sum; end
来源：http://xgr.shanyushiyangtech.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://dvm.shzxlz.cn

[C04] 命名参数 / 关键字参数
来源：http://rxl.quarkkingdee.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://vws.cucudq.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wvx.dianchejie.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://nyi.yvedp.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://jed.svipenyu.cn

Java: // 无：用 Builder 模式或 record
来源：http://kvy.ydzc1.top

Go:   // 无：用配置结构体参数
来源：http://ofu.tanke756.top

Ruby: f(a: 1, b: 2)
来源：http://tpx.birdmap.top

C#:   f(a: 1, b: 2)
来源：http://vki.cqqwz.cn

[C05] 返回多个值
来源：http://mit.yanxiufei.cn

Py:   return a, b
来源：http://haq.tian-w.cn

PHP:  return [$a, $b];
来源：http://qet.yonumen.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://baq.epnwcf.com

TS:   return { a, b };
来源：http://shr.chenlongwang.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://lbs.sysykeji.top

Go:   return a, b
来源：http://map.hammf.cn

Ruby: return a, b
来源：http://czk.fanxiaobao.xyz

C#:   return (a, b);              // ValueTuple
来源：http://pid.zhengqikj.top

[C06] 匿名函数 / lambda
来源：http://eri.ivvv.top

Py:   square = lambda x: x * x
来源：http://fde.epnwcf.com

PHP:  $square = fn($x) => $x * $x;
来源：http://obi.jinqigufen.top

JS:   const square = x => x * x;
来源：http://ekw.yfazqb.com

TS:   const square = (x: number): number => x * x;
来源：http://mfz.shuidangran.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ekd.xylfe.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ade.uphjek.com

Ruby: square = ->(x) { x * x }
来源：http://lao.ivvv.top

C#:   Func<int, int> square = x => x * x;
来源：http://skc.svipenyu.cn

[C07] 把函数作为参数传入
来源：http://irn.yangfankeji.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mpg.tian-w.cn

PHP:  array_map("strtoupper", $arr);
来源：http://osh.xuanzx.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://dsv.aibaodan.cn

TS:   arr.map(String)
来源：http://tuy.quarkkingdee.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://zkc.yongpay.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://xgw.haohaochexian.top

Ruby: arr.map(&:upcase)
来源：http://zcq.yj20258.top

C#:   arr.Select(s => s.ToUpper())
来源：http://ixh.sjlbkw.cn

[C08] 闭包
来源：http://lam.hnxiangtu.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://njb.vqdsnc.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://vly.zdbjq.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://umn.jiagoushi.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://fcc.iojbl.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wzh.shangyingyoupin.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://aug.chenzaomai.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://uie.hammf.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://etg.hongshengwenyu.top

[C09] 递归
来源：http://agf.shuidangran.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://nev.uphjek.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://rpb.zhoulong.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xxf.zhixingplan.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fbx.gotoacloud.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://vfq.yuanzhike.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://nij.xylfe.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://jct.vehdjk.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://gqb.meibo888.top

[C10] 变量作用域
来源：http://pfw.tianlin.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://yfj.zhijiandao.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mpv.zycfv.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://vin.gzhubu.top

TS:   同 JS
来源：http://iyq.hongshengwenyu.top

Java: 方法内为块级作用域
来源：http://veo.nanxinkj.top

Go:   花括号块级作用域
来源：http://whw.uphjek.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://shs.yfazqb.com

C#:   块级作用域
来源：http://mvz.xylfe.cn

[C11] 模块导入与导出
来源：http://rzi.zdqjudy.top

Py:   from module import func
来源：http://zco.zhixingplan.top

PHP:  require "file.php";  或 use App\Service;
来源：http://chp.zdbjq.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ijr.havefunace.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://znc.ivvv.top

Java: import java.util.List;
来源：http://cqz.shanyushiyangtech.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://srm.yfazqb.com

Ruby: require "json"; require_relative "./util"
来源：http://zfe.wangshuangyany.cn

C#:   using System.Text;
来源：http://inf.ydzc1.top

[C12] 立即执行函数 IIFE
来源：http://nov.jinghuilouyu.cn

Py:   (lambda: print("run"))()
来源：http://iju.dianchejie.cn

PHP:  (function () { echo "run"; })();
来源：http://wgr.jqgfzy.top

JS:   (() => { console.log("run"); })();
来源：http://skl.sweek.top

TS:   (() => { console.log("run"); })();
来源：http://klu.xuanzx.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://tya.jqgufenzy.top

Go:   func() { fmt.Println("run") }()
来源：http://dgi.jqgfzy.top

Ruby: -> { puts "run" }.call
来源：http://hfp.nanxinkj.top

C#:   // 无 IIFE：用静态构造函数
来源：http://fmq.jinqigufen.top

[C13] 类型声明 / 类型注解
来源：http://iyr.tian-w.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ovc.sysykeji.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hne.smart0.xyz

JS:   // 无类型（可用 JSDoc 注释）
来源：http://qto.vqdsnc.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ebp.yanxiufei.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ufy.mhx1999.top

Go:   func add(a, b int) int
来源：http://hoh.jyoumei.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ddr.wangdashe.top

C#:   int Add(int a, int b) => a + b;
来源：http://joj.mhx1999.top

[C14] 泛型函数
来源：http://gjw.hammf.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://umf.jinqigufen.top

PHP:  // 无泛型
来源：http://fzb.cqqwz.cn

JS:   // 无泛型
来源：http://alm.nanxinkj.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://qbc.xinyue.icu

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mzx.52xcode.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://kmf.52xcode.cn

Ruby: # 无泛型
来源：http://acv.yj202588.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ilh.tian-w.cn

[C15] 解构 / 展开参数
来源：http://baj.ybcxt.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://fir.haohaochexian.top

PHP:  [$a, $b] = $pair;
来源：http://wnl.yonumen.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://vzv.zhaomingkeji.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mmt.chenjidiqi.icu

Java: // 无解构
来源：http://kto.ivvv.top

Go:   // 无解构
来源：http://hje.shuidangran.top

Ruby: a, b = pair
来源：http://dzo.fehbvm.com

C#:   var (a, b) = pair;
来源：http://ugc.sweek.top

[C16] 函数 / 方法重载
来源：http://ktr.daria6918.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://nra.sysykeji.top

PHP:  // 无重载
来源：http://xbt.wangdashe.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://zcl.feifeiyinyue.top

TS:   // 用联合类型或重载签名声明
来源：http://jjn.xinyue.icu

Java: void f(int a) {}  void f(String a) {}
来源：http://jfy.havefunace.top

Go:   // 无重载：用不同函数名
来源：http://anq.bbcook.cn

Ruby: # 无重载：靠动态参数
来源：http://dro.jlsjyb.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://gvw.guannengcc.top

================================================================================
来源：http://jmi.yvedp.cn

D. 数组 / 列表 / 集合
来源：http://sdn.yfazqb.com

================================================================================
来源：http://lcb.shuidangran.top

[D01] 创建数组 / 列表
来源：http://awr.zhijiandao.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://tcu.zhoulong.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://lae.9152youxi.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://xpm.hesvh.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://whw.yuanzhike.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://gcx.xingfuxueyuan.xyz

Go:   arr := []int{1, 2, 3}
来源：http://prz.pycfn.com

Ruby: arr = [1, 2, 3]
来源：http://xxe.zhongyouzk.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://crf.cashguo.top

[D02] 追加元素到末尾
来源：http://ufw.dianchejie.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://yty.xingfuxueyuan.xyz

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://rcu.yangfankeji.com

JS:   arr.push(4);
来源：http://vml.hnqzz.top

TS:   arr.push(4);
来源：http://xsp.chenjidiqi.icu

Java: list.add(4);
来源：http://sne.xinyue.icu

Go:   arr = append(arr, 4)
来源：http://vpd.jinghuilouyu.cn

Ruby: arr << 4; arr.push(5)
来源：http://dur.wangshuangyany.cn

C#:   list.Add(4);
来源：http://lew.yj20258.top

[D03] 在指定位置插入元素
来源：http://frc.shanyushiyangkeji.top

Py:   arr.insert(0, 0)
来源：http://pcx.yanxiufei.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://isz.xuanzx.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://vbr.316326.xyz

TS:   arr.splice(0, 0, 0);
来源：http://ihf.tarul.cn

Java: list.add(0, 0);
来源：http://tzv.zhoulong.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://njr.sysykeji.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ntd.cqqwz.cn

C#:   list.Insert(0, 0);
来源：http://shm.fktsv.cn

[D04] 删除元素
来源：http://vww.ywan-chungtsiang.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://xry.kuanghao11.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://nub.zdqjudy.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ejn.ydjk.org.cn

TS:   arr.splice(0, 1);
来源：http://srb.jlsjyb.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://eko.birdmap.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://idl.meibo888.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://uzf.shanyushiyangkeji.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xzq.xingfuxueyuan.xyz

[D05] 访问与修改元素
来源：http://abw.shanyushiyangtech.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://sfa.gotoacloud.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://aee.smart0.xyz

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://kqx.jiagoushi.top

TS:   arr[0]; arr.at(-1);
来源：http://cul.wangdashe.top

Java: list.get(0); list.set(0, 9);
来源：http://cfr.hcnkem.com

Go:   arr[0]; arr[0] = 9
来源：http://slt.ctjpmb.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mor.dashuyun.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ukb.zycfv.cn

[D06] 数组长度
来源：http://bzb.cucudq.cn

Py:   len(arr)
来源：http://ivs.c1oappe.top

PHP:  count($arr);
来源：http://lkg.yueranfly.top

JS:   arr.length
来源：http://buy.daxiang520.top

TS:   arr.length
来源：http://qlg.hcnkem.com

Java: list.size();
来源：http://ssh.yuxming.cn

Go:   len(arr)
来源：http://kpp.fanxiaobao.xyz

Ruby: arr.length; arr.size
来源：http://eal.shzxlz.cn

C#:   list.Count;
来源：http://gdm.xuanzx.com

[D07] 切片 / 取子数组
来源：http://dde.gotoacloud.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://lxv.hnqzz.top

PHP:  array_slice($arr, 1, 3);
来源：http://zwi.andypj.xyz

JS:   arr.slice(1, 4);
来源：http://rph.zdbjq.cn

TS:   arr.slice(1, 4);
来源：http://mmz.tianlin.xyz

Java: list.subList(1, 4);
来源：http://yjy.chenzaomai.com

Go:   arr[1:4]
来源：http://uxn.tianlin.xyz

Ruby: arr[1, 3]
来源：http://ccx.shanyushiyangtech.top

C#:   list.GetRange(1, 3);
来源：http://hxc.hysaishi.cn

[D08] 合并两个数组
来源：http://exi.redwolf501.top

Py:   a + b;  a.extend(b)
来源：http://ucy.smart0.xyz

PHP:  array_merge($a, $b);
来源：http://bif.iojbl.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://cqb.zdbjq.cn

TS:   [...a, ...b];
来源：http://bic.zhiwuduotai.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ntj.yangfankeji.com

Go:   append(a, b...)
来源：http://sbv.smart0.xyz

Ruby: a + b;  a.concat(b)
来源：http://kwc.ivvv.top

C#:   a.Concat(b).ToList()
来源：http://qgx.yuanzhike.top

[D09] 排序（升序）
来源：http://noq.jinghuilouyu.cn

Py:   sorted(arr);  arr.sort()
来源：http://sfy.ydzc1.top

PHP:  sort($arr);
来源：http://ljg.yanxiufei.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://iqa.hysaishi.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://kbl.xuetiantiany.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ybb.gaohongyu789.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ode.mhx1999.top

Ruby: arr.sort
来源：http://ecr.xingfuxueyuan.xyz

C#:   list.Sort();
来源：http://olc.jinghuilouyu.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://vgg.ctjpmb.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://odq.hywenlv.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bgk.cqqwz.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://rfa.yj20258888.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://gip.sufxvd.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://rcd.yuanzhike.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://dps.yuanzhike.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://xos.xuanzx.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://llm.bbcook.cn

[D11] 反转数组
来源：http://mbs.aibaodan.cn

Py:   arr[::-1];  arr.reverse()
来源：http://nmv.tanke756.top

PHP:  array_reverse($arr);
来源：http://gxu.xuanzx.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wwg.jianghu66.top

TS:   [...arr].reverse();
来源：http://eyr.jlsjyb.cn

Java: Collections.reverse(list);
来源：http://anx.uphjek.com

Go:   slices.Reverse(arr)
来源：http://wty.wangshuangyany.cn

Ruby: arr.reverse
来源：http://tyw.shanyushiyangtech.top

C#:   list.Reverse();
来源：http://dwp.wangdashe.top

[D12] 查找元素下标
来源：http://gxs.chenzaomai.com

Py:   arr.index(x);  x in arr
来源：http://xgy.nwbrower.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mts.xziqi.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mxh.zdbjq.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bll.nwbrower.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://iog.fktsv.cn

Go:   slices.Index(arr, x)
来源：http://std.jianghu66.top

Ruby: arr.index(x)
来源：http://ulk.aizwys.cn

C#:   list.IndexOf(x);
来源：http://aci.yanxiufei.cn

[D13] 过滤（保留满足条件的）
来源：http://fjd.zhiwuduotai.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ohl.316326.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mxq.yueranfly.top

JS:   arr.filter(x => x > 3)
来源：http://wzt.wangshuangyany.cn

TS:   arr.filter(x => x > 3)
来源：http://qlf.sweek.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://xgh.jyoumei.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://vhv.yonumen.top

Ruby: arr.select { |x| x > 3 }
来源：http://egm.bbcook.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://sdp.nanxuanxn.top

[D14] 映射转换（每个元素变形）
来源：http://fij.hnqzz.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://gve.yanxiufei.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://kmo.zhijiandao.cn

JS:   arr.map(x => x * 2)
来源：http://qns.hesvh.cn

TS:   arr.map(x => x * 2)
来源：http://tfx.xuanzx.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://vhz.hammf.cn

Go:   // 手写循环
来源：http://rfo.kuanghao11.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ovy.yonumen.top

C#:   list.Select(x => x * 2).ToList()
来源：http://qid.kuanghao11.cn

[D15] 去重
来源：http://ljj.hfpthk.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ujc.hywenlv.cn

PHP:  array_unique($arr);
来源：http://lrd.dashuyun.cn

JS:   [...new Set(arr)]
来源：http://mat.zhoulong.xyz

TS:   [...new Set(arr)]
来源：http://gxa.andypj.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wid.smart0.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://rlc.hongshengwenyu.top

Ruby: arr.uniq
来源：http://nct.yj202588.top

C#:   list.Distinct().ToList()
来源：http://nkz.ybcxt.top

[D16] 求和与平均值
来源：http://jua.jiagoushi.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://jcf.shanyushiyangkeji.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://dmw.yueranfly.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://anl.hysaishi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://xyk.tanke756.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://csk.sufxvd.cn

Go:   // 手写循环累加
来源：http://mis.yanxiufei.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://fps.birdmap.top

C#:   list.Sum();  list.Average()
来源：http://ohx.yj20258888.top

[D17] 最大值与最小值
来源：http://svw.snrcjt.cn

Py:   max(arr);  min(arr)
来源：http://vts.ydjk.org.cn

PHP:  max($arr);  min($arr);
来源：http://xdd.jinyuanbaomall.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://lqo.feifeiyinyue.top

TS:   Math.max(...arr);
来源：http://ebm.wangshuangyany.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ofp.wangshuangyany.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ifv.shanyushiyangtech.top

Ruby: arr.max;  arr.min
来源：http://osd.0kj1m.cn

C#:   list.Max();  list.Min()
来源：http://mtq.sysykeji.top

[D18] 扁平化嵌套数组
来源：http://onx.hywenlv.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://nki.ehwqpu.com

PHP:  array_merge(...$nested);
来源：http://rsx.daxiang520.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://vjw.yj20258.top

TS:   nested.flat();
来源：http://tev.ydzc1.top


<!-- 参考信息 -->