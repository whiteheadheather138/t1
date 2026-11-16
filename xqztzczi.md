代发 wailian999

Java: static int add(int a, int b) { return a + b; }
来源：http://xlb.ybcxt.top

Go:   func add(a, b int) int { return a + b }
来源：http://vyb.guowangkeji.top

Ruby: def add(a, b); a + b; end
来源：http://opi.sysykeji.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://shu.cdnleiting.top

[C02] 默认参数
来源：http://izi.yueranfly.top

Py:   def greet(name="World"): return name
来源：http://fiz.yuanzhike.top

PHP:  function greet($name = "World") { return $name; }
来源：http://gfm.iojbl.cn

JS:   function greet(name = "World") { return name; }
来源：http://qbq.wangshuangyany.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://qse.vehdjk.com

Java: // 无默认参数：方法重载或 Optional
来源：http://jdh.gotoacloud.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://nqm.yvedp.cn

Ruby: def greet(name = "World") = name
来源：http://eds.hywenlv.cn

C#:   string Greet(string name = "World") => name;
来源：http://zmc.fktsv.cn

[C03] 可变参数
来源：http://aah.sjlbkw.cn

Py:   def total(*args): return sum(args)
来源：http://ikz.tarul.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://vyh.sysykeji.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://anb.mhx1999.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://szn.bjfxy.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://rvx.snrcjt.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://sdr.gogol.net.cn

Ruby: def total(*nums); nums.sum; end
来源：http://vok.vehdjk.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://fqo.xziqi.cn

[C04] 命名参数 / 关键字参数
来源：http://yds.snrcjt.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://lns.zhaomingkeji.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://aeb.smart0.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://zbt.jqgufenzy.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://chd.hnqzz.top

Java: // 无：用 Builder 模式或 record
来源：http://iyl.yuxming.cn

Go:   // 无：用配置结构体参数
来源：http://twx.daria6918.cn

Ruby: f(a: 1, b: 2)
来源：http://fuj.jianghu66.top

C#:   f(a: 1, b: 2)
来源：http://rve.vqdsnc.cn

[C05] 返回多个值
来源：http://klw.nwbrower.top

Py:   return a, b
来源：http://rgm.tarul.cn

PHP:  return [$a, $b];
来源：http://cbm.fehbvm.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://tgb.bbcook.cn

TS:   return { a, b };
来源：http://fkl.sweek.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://qll.guowangkeji.top

Go:   return a, b
来源：http://ggy.ehwqpu.com

Ruby: return a, b
来源：http://kqg.daxiang520.top

C#:   return (a, b);              // ValueTuple
来源：http://ivg.snrcjt.cn

[C06] 匿名函数 / lambda
来源：http://fas.sufxvd.cn

Py:   square = lambda x: x * x
来源：http://nln.nwbrower.top

PHP:  $square = fn($x) => $x * $x;
来源：http://vhr.zycfv.cn

JS:   const square = x => x * x;
来源：http://pjw.chenzaomai.com

TS:   const square = (x: number): number => x * x;
来源：http://asb.jinqigfzy.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ros.fanxiaobao.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://yqo.daria6918.cn

Ruby: square = ->(x) { x * x }
来源：http://ijo.jianghu66.top

C#:   Func<int, int> square = x => x * x;
来源：http://tfs.wangdashe.top

[C07] 把函数作为参数传入
来源：http://bsb.vqdsnc.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://gyi.chenzaomai.com

PHP:  array_map("strtoupper", $arr);
来源：http://bac.gzhubu.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wfr.gogol.net.cn

TS:   arr.map(String)
来源：http://lby.hnqzz.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://snx.yj20258888.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qvr.hfpthk.cn

Ruby: arr.map(&:upcase)
来源：http://xix.bbcook.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://juq.gogol.net.cn

[C08] 闭包
来源：http://hxg.hcnkem.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mfg.ydjk.org.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://vjc.hammf.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://smf.jinqigufen.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://whw.pengpengdd.cyou

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ajv.mhx1999.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://vzx.zhongyouzk.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://rbi.daxiang520.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://rio.yfazqb.com

[C09] 递归
来源：http://nth.cucudq.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ued.haohaochexian.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://kxl.dianchejie.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qna.gzhubu.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pxq.cqqwz.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://yty.sxryk.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://bdd.zhoulong.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://cdw.chenzaomai.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ldi.xuanzx.com

[C10] 变量作用域
来源：http://gtw.guowangkeji.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qlx.andypj.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://fzq.cheryme.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wzm.chenzaomai.com

TS:   同 JS
来源：http://rmu.daxiang520.top

Java: 方法内为块级作用域
来源：http://jab.vqdsnc.cn

Go:   花括号块级作用域
来源：http://qtn.daxiang520.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://fan.gogol.net.cn

C#:   块级作用域
来源：http://ehi.chenzaomai.com

[C11] 模块导入与导出
来源：http://qkb.shanyushiyangtech.top

Py:   from module import func
来源：http://vaw.vqdsnc.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://uvp.zhixingplan.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://rnq.meibo888.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://tvg.pycfn.com

Java: import java.util.List;
来源：http://zoy.daria6918.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://fvp.chenlongwang.top

Ruby: require "json"; require_relative "./util"
来源：http://chc.sweek.top

C#:   using System.Text;
来源：http://fmp.snrcjt.cn

[C12] 立即执行函数 IIFE
来源：http://fwk.zdbjq.cn

Py:   (lambda: print("run"))()
来源：http://uvv.daxiang520.top

PHP:  (function () { echo "run"; })();
来源：http://thf.nanxinkj.top

JS:   (() => { console.log("run"); })();
来源：http://kde.yonumen.top

TS:   (() => { console.log("run"); })();
来源：http://tzb.sufxvd.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://xkz.jinqigufen.top

Go:   func() { fmt.Println("run") }()
来源：http://nvz.9152youxi.cn

Ruby: -> { puts "run" }.call
来源：http://pye.iojbl.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://qvc.jqgufenzy.top

[C13] 类型声明 / 类型注解
来源：http://biv.gogol.net.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://pio.c1oappe.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zzh.hongshengwenyu.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://xmm.316326.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fbi.feifeiyinyue.top

Java: int add(int a, int b) { return a + b; }
来源：http://pxs.redwolf501.top

Go:   func add(a, b int) int
来源：http://ncd.hammf.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://snm.xziqi.cn

C#:   int Add(int a, int b) => a + b;
来源：http://asu.guowangkeji.top

[C14] 泛型函数
来源：http://fll.ppjwa.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zyz.xylfe.cn

PHP:  // 无泛型
来源：http://ogk.yonumen.top

JS:   // 无泛型
来源：http://brz.epnwcf.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://gve.tianlin.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ukx.guannengcc.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://goz.vqdsnc.cn

Ruby: # 无泛型
来源：http://lrb.zhengqikj.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://gat.epnwcf.com

[C15] 解构 / 展开参数
来源：http://kft.jiagoushi.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mex.fzhhl.top

PHP:  [$a, $b] = $pair;
来源：http://umc.yfazqb.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://uvf.zhengqikj.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wuh.sxryk.cn

Java: // 无解构
来源：http://mwl.0kj1m.cn

Go:   // 无解构
来源：http://mex.cdnleiting.top

Ruby: a, b = pair
来源：http://jwa.quarkkingdee.top

C#:   var (a, b) = pair;
来源：http://ccc.cdnleiting.top

[C16] 函数 / 方法重载
来源：http://uij.yueranfly.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://bcb.zhixingplan.top

PHP:  // 无重载
来源：http://vju.sweek.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://gye.bjfxy.top

TS:   // 用联合类型或重载签名声明
来源：http://mgz.mhx1999.top

Java: void f(int a) {}  void f(String a) {}
来源：http://rfa.quarkkingdee.top

Go:   // 无重载：用不同函数名
来源：http://lyl.fktsv.cn

Ruby: # 无重载：靠动态参数
来源：http://lxd.mhx1999.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://ydv.uphjek.com

================================================================================
来源：http://ltq.hongshengwenyu.top

D. 数组 / 列表 / 集合
来源：http://ilq.tianlin.xyz

================================================================================
来源：http://mmy.dianchejie.cn

[D01] 创建数组 / 列表
来源：http://uac.gzhubu.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://zju.fzhhl.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://xqa.daxiang520.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://klk.yuanzhike.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://wdn.meibo888.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://vkt.yuanzhike.top

Go:   arr := []int{1, 2, 3}
来源：http://ygz.fzhhl.top

Ruby: arr = [1, 2, 3]
来源：http://bpq.hcnkem.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wgu.jiagoushi.top

[D02] 追加元素到末尾
来源：http://lti.gotoacloud.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mep.cdnleiting.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://pmc.epnwcf.com

JS:   arr.push(4);
来源：http://oto.daria6918.cn

TS:   arr.push(4);
来源：http://laq.xingfuxueyuan.xyz

Java: list.add(4);
来源：http://mnl.jqgfzy.top

Go:   arr = append(arr, 4)
来源：http://nxu.jqgfzy.top

Ruby: arr << 4; arr.push(5)
来源：http://uaq.xinyue.icu

C#:   list.Add(4);
来源：http://par.gogol.net.cn

[D03] 在指定位置插入元素
来源：http://qrk.shzxlz.cn

Py:   arr.insert(0, 0)
来源：http://wwl.xuetiantiany.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://set.gzhubu.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://pvb.bjfxy.top

TS:   arr.splice(0, 0, 0);
来源：http://qyt.shanyushiyangtech.top

Java: list.add(0, 0);
来源：http://yat.fzhhl.top

Go:   arr = append([]int{0}, arr...)
来源：http://tbi.sjlbkw.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://etr.guannengcc.top

C#:   list.Insert(0, 0);
来源：http://pow.smart0.xyz

[D04] 删除元素
来源：http://mcg.guannengcc.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://yyv.xylfe.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://yyf.ctjpmb.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xae.ehwqpu.com

TS:   arr.splice(0, 1);
来源：http://foq.yonumen.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://voc.bjfxy.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://pbq.jyoumei.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://xph.fanxiaobao.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://lzu.fehbvm.com

[D05] 访问与修改元素
来源：http://spq.andypj.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hqq.fengsongda.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://cvs.cdnleiting.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://lvj.sjlbkw.cn

TS:   arr[0]; arr.at(-1);
来源：http://dvk.redwolf501.top

Java: list.get(0); list.set(0, 9);
来源：http://eba.epnwcf.com

Go:   arr[0]; arr[0] = 9
来源：http://cog.sweek.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://qbj.haohaochexian.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hpi.shzxlz.cn

[D06] 数组长度
来源：http://uoq.jiagoushi.top

Py:   len(arr)
来源：http://gml.uphjek.com

PHP:  count($arr);
来源：http://oyl.hnqzz.top

JS:   arr.length
来源：http://efx.zdqjudy.top

TS:   arr.length
来源：http://gew.redwolf501.top

Java: list.size();
来源：http://sdb.daria6918.cn

Go:   len(arr)
来源：http://dhh.yuxming.cn

Ruby: arr.length; arr.size
来源：http://xhz.jiagoushi.top

C#:   list.Count;
来源：http://hsr.hammf.cn

[D07] 切片 / 取子数组
来源：http://yxy.yfazqb.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://lcg.feifeiyinyue.top

PHP:  array_slice($arr, 1, 3);
来源：http://cho.yueranfly.top

JS:   arr.slice(1, 4);
来源：http://lkg.yj202588.top

TS:   arr.slice(1, 4);
来源：http://xto.havefunace.top

Java: list.subList(1, 4);
来源：http://pud.haohaochexian.top

Go:   arr[1:4]
来源：http://snz.haohaochexian.top

Ruby: arr[1, 3]
来源：http://ofq.hesvh.cn

C#:   list.GetRange(1, 3);
来源：http://ctt.ctjpmb.com

[D08] 合并两个数组
来源：http://duw.chenzaomai.com

Py:   a + b;  a.extend(b)
来源：http://crd.gotoacloud.top

PHP:  array_merge($a, $b);
来源：http://rrm.shangyingyoupin.top

JS:   [...a, ...b];  a.concat(b);
来源：http://wsj.hnxiangtu.top

TS:   [...a, ...b];
来源：http://gic.hysaishi.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://drl.xinyue.icu

Go:   append(a, b...)
来源：http://ktl.hysaishi.cn

Ruby: a + b;  a.concat(b)
来源：http://rvs.hongshengwenyu.top

C#:   a.Concat(b).ToList()
来源：http://gur.feifeiyinyue.top

[D09] 排序（升序）
来源：http://cnk.zhongyouzk.top

Py:   sorted(arr);  arr.sort()
来源：http://ypp.haohaochexian.top

PHP:  sort($arr);
来源：http://oet.xylfe.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://otl.jyoumei.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ltf.guannengcc.top

Java: Collections.sort(list);  list.sort(null);
来源：http://yqy.fehbvm.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://usq.ydzc1.top

Ruby: arr.sort
来源：http://vle.chenzaomai.com

C#:   list.Sort();
来源：http://plq.yvedp.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://eno.shuidangran.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://yey.c1oappe.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://sxz.ctjpmb.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://tpq.fktsv.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hhb.vehdjk.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://spb.hywenlv.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://rlp.cashguo.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://aby.zhoulong.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qdw.shuidangran.top

[D11] 反转数组
来源：http://crr.havefunace.top

Py:   arr[::-1];  arr.reverse()
来源：http://tkv.zhongyouzk.top

PHP:  array_reverse($arr);
来源：http://hvz.tanke756.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://yuw.chenzaomai.com

TS:   [...arr].reverse();
来源：http://jjj.c1oappe.top

Java: Collections.reverse(list);
来源：http://ubp.52xcode.cn

Go:   slices.Reverse(arr)
来源：http://nul.sxryk.cn

Ruby: arr.reverse
来源：http://zzb.zdqjudy.top

C#:   list.Reverse();
来源：http://bje.cheryme.top

[D12] 查找元素下标
来源：http://mpy.shanyushiyangtech.top

Py:   arr.index(x);  x in arr
来源：http://vhh.aibaodan.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://bwh.snrcjt.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ahp.svipenyu.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://klw.yj202588.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://qiy.cqqwz.cn

Go:   slices.Index(arr, x)
来源：http://nhi.yj20258.top

Ruby: arr.index(x)
来源：http://cpu.hongshengwenyu.top

C#:   list.IndexOf(x);
来源：http://dsp.zhongyouzk.top

[D13] 过滤（保留满足条件的）
来源：http://trg.hywenlv.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://foz.guowangkeji.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://vga.sxryk.cn

JS:   arr.filter(x => x > 3)
来源：http://grb.yongpay.top

TS:   arr.filter(x => x > 3)
来源：http://qeg.gotoacloud.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ilh.xingfuxueyuan.xyz

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://bmv.zycfv.cn

Ruby: arr.select { |x| x > 3 }
来源：http://hls.nanxuanxn.top

C#:   list.Where(x => x > 3).ToList()
来源：http://afv.zhiwuduotai.top

[D14] 映射转换（每个元素变形）
来源：http://qhg.zdbjq.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://klr.yangfankeji.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://rep.svipenyu.cn

JS:   arr.map(x => x * 2)
来源：http://cel.zhengqikj.top

TS:   arr.map(x => x * 2)
来源：http://tzd.hongshengwenyu.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://djn.jqgufenzy.top

Go:   // 手写循环
来源：http://cpt.hnqzz.top

Ruby: arr.map { |x| x * 2 }
来源：http://oxn.chenjidiqi.icu

C#:   list.Select(x => x * 2).ToList()
来源：http://lgq.yj202588.top

[D15] 去重
来源：http://ocq.zycfv.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://xnz.epnwcf.com

PHP:  array_unique($arr);
来源：http://iow.wangshuangyany.cn

JS:   [...new Set(arr)]
来源：http://qbi.nwbrower.top

TS:   [...new Set(arr)]
来源：http://deh.cqqwz.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://cwf.cdnleiting.top

Go:   // 用 map[T]struct{} 手写
来源：http://hqj.shanyushiyangtech.top

Ruby: arr.uniq
来源：http://hfh.yj202588.top

C#:   list.Distinct().ToList()
来源：http://uob.haohaochexian.top

[D16] 求和与平均值
来源：http://tez.aibaodan.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://znd.yangfankeji.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://enc.chenzaomai.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://lbh.fanxiaobao.xyz

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://auh.0kj1m.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://iix.ywan-chungtsiang.top

Go:   // 手写循环累加
来源：http://ctw.zycfv.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://fya.guowangkeji.top

C#:   list.Sum();  list.Average()
来源：http://oej.xingfuxueyuan.xyz

[D17] 最大值与最小值
来源：http://eit.meibo888.top

Py:   max(arr);  min(arr)
来源：http://qpp.zhijiandao.cn

PHP:  max($arr);  min($arr);
来源：http://rap.jqgufenzy.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://xek.jyoumei.cn

TS:   Math.max(...arr);
来源：http://akt.wangdashe.top

Java: Collections.max(list);  Collections.min(list);
来源：http://tcf.cdnleiting.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://lsn.ydzc1.top

Ruby: arr.max;  arr.min
来源：http://azd.gzhubu.top

C#:   list.Max();  list.Min()
来源：http://lhz.fengsongda.top

[D18] 扁平化嵌套数组
来源：http://ykl.zhixingplan.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://vce.zhoulong.xyz

PHP:  array_merge(...$nested);
来源：http://npi.aibaodan.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://xgn.jiagoushi.top

TS:   nested.flat();
来源：http://mrq.xingfuxueyuan.xyz


<!-- 参考信息 -->