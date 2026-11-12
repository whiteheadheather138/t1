代发 wailian999

[C02] 默认参数
来源：http://qvn.aizwys.cn

Py:   def greet(name="World"): return name
来源：http://ooa.yuxming.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://prz.zdbjq.cn

JS:   function greet(name = "World") { return name; }
来源：http://dhj.hongshengwenyu.top

TS:   function greet(name: string = "World") { return name; }
来源：http://vmx.havefunace.top

Java: // 无默认参数：方法重载或 Optional
来源：http://vxw.yfazqb.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://zjm.guowangkeji.top

Ruby: def greet(name = "World") = name
来源：http://wtu.aizwys.cn

C#:   string Greet(string name = "World") => name;
来源：http://qqa.ehwqpu.com

[C03] 可变参数
来源：http://zrc.hnxiangtu.top

Py:   def total(*args): return sum(args)
来源：http://aho.aibaodan.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://sft.gaohongyu789.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://nkr.yueranfly.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://cdn.yj202588.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://qft.zhaomingkeji.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://umk.hnxiangtu.top

Ruby: def total(*nums); nums.sum; end
来源：http://slf.cheryme.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://vbe.hfpthk.cn

[C04] 命名参数 / 关键字参数
来源：http://vdz.hfpthk.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://kgf.tian-w.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xhg.wangdashe.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://nlm.redwolf501.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xfy.hysaishi.cn

Java: // 无：用 Builder 模式或 record
来源：http://ugd.sweek.top

Go:   // 无：用配置结构体参数
来源：http://yvf.yvedp.cn

Ruby: f(a: 1, b: 2)
来源：http://vxg.hysaishi.cn

C#:   f(a: 1, b: 2)
来源：http://sho.bjfxy.top

[C05] 返回多个值
来源：http://rpe.quarkkingdee.top

Py:   return a, b
来源：http://uha.zdbjq.cn

PHP:  return [$a, $b];
来源：http://fhi.svipenyu.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://yof.fehbvm.com

TS:   return { a, b };
来源：http://uwm.havefunace.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://qvi.hongshengwenyu.top

Go:   return a, b
来源：http://wao.fzhhl.top

Ruby: return a, b
来源：http://xja.yj202588.top

C#:   return (a, b);              // ValueTuple
来源：http://scu.ydzc1.top

[C06] 匿名函数 / lambda
来源：http://gfi.9152youxi.cn

Py:   square = lambda x: x * x
来源：http://kii.zhijiandao.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://byy.svipenyu.cn

JS:   const square = x => x * x;
来源：http://dsj.ybcxt.top

TS:   const square = (x: number): number => x * x;
来源：http://qwd.yj202588.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://egj.epnwcf.com

Go:   sq := func(x int) int { return x * x }
来源：http://bgt.jinqigfzy.top

Ruby: square = ->(x) { x * x }
来源：http://ntq.kuanghao11.cn

C#:   Func<int, int> square = x => x * x;
来源：http://uob.hnqzz.top

[C07] 把函数作为参数传入
来源：http://ipo.jinqigfzy.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ekc.xuanzx.com

PHP:  array_map("strtoupper", $arr);
来源：http://aaq.cashguo.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://tla.yj202588.top

TS:   arr.map(String)
来源：http://zke.xziqi.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://psl.hongshengwenyu.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://zur.cheryme.top

Ruby: arr.map(&:upcase)
来源：http://lad.sysykeji.top

C#:   arr.Select(s => s.ToUpper())
来源：http://mpw.nanxuanxn.top

[C08] 闭包
来源：http://ugr.ctjpmb.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ogp.haohaochexian.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ilz.bjfxy.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://gvo.tianlin.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://tis.nanxuanxn.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://vra.zdqjudy.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://lbr.birdmap.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://fhr.jlsjyb.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://acd.yuxming.cn

[C09] 递归
来源：http://lli.nanxinkj.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://kqz.0kj1m.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://yum.gotoacloud.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kuk.havefunace.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xcb.meibo888.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://jgp.jlsjyb.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://lyx.pengpengdd.cyou

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://idd.nwbrower.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://raa.jiagoushi.top

[C10] 变量作用域
来源：http://nao.uphjek.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://rks.jinyuanbaomall.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mer.yj202588.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://tmr.kuanghao11.cn

TS:   同 JS
来源：http://qwb.aizwys.cn

Java: 方法内为块级作用域
来源：http://sxt.jinghuilouyu.cn

Go:   花括号块级作用域
来源：http://wja.shzxlz.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://jfp.tanke756.top

C#:   块级作用域
来源：http://nng.ppjwa.cn

[C11] 模块导入与导出
来源：http://ves.chenjidiqi.icu

Py:   from module import func
来源：http://uic.aizwys.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://jbr.zhaomingkeji.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://quc.wangshuangyany.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hii.zdbjq.cn

Java: import java.util.List;
来源：http://rgv.uphjek.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://lmo.ydzc1.top

Ruby: require "json"; require_relative "./util"
来源：http://phx.ywan-chungtsiang.top

C#:   using System.Text;
来源：http://bgc.daxiang520.top

[C12] 立即执行函数 IIFE
来源：http://xhg.tian-w.cn

Py:   (lambda: print("run"))()
来源：http://cou.quarkkingdee.top

PHP:  (function () { echo "run"; })();
来源：http://qjl.nanxuanxn.top

JS:   (() => { console.log("run"); })();
来源：http://pfi.sysykeji.top

TS:   (() => { console.log("run"); })();
来源：http://gvc.xinyue.icu

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://lrg.fktsv.cn

Go:   func() { fmt.Println("run") }()
来源：http://goy.ydzc1.top

Ruby: -> { puts "run" }.call
来源：http://ajv.shuidangran.top

C#:   // 无 IIFE：用静态构造函数
来源：http://ywq.bbcook.cn

[C13] 类型声明 / 类型注解
来源：http://pjf.52xcode.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ptz.gzhubu.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://npc.gaohongyu789.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://yrw.sweek.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ind.zhoulong.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://gty.c1oappe.top

Go:   func add(a, b int) int
来源：http://zkb.jinghuilouyu.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://sce.feifeiyinyue.top

C#:   int Add(int a, int b) => a + b;
来源：http://bas.yuxming.cn

[C14] 泛型函数
来源：http://hsm.ctjpmb.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://rtg.yvedp.cn

PHP:  // 无泛型
来源：http://agt.yvedp.cn

JS:   // 无泛型
来源：http://wlv.nanxuanxn.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://pzd.yonumen.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://yfq.nanxuanxn.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://izf.cashguo.top

Ruby: # 无泛型
来源：http://lzq.aibaodan.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://feh.0kj1m.cn

[C15] 解构 / 展开参数
来源：http://pca.cashguo.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://vwh.52xcode.cn

PHP:  [$a, $b] = $pair;
来源：http://lbv.shanyushiyangkeji.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://lml.xuetiantiany.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wpn.jlsjyb.cn

Java: // 无解构
来源：http://fuy.yuanzhike.top

Go:   // 无解构
来源：http://xvs.tarul.cn

Ruby: a, b = pair
来源：http://mpd.guannengcc.top

C#:   var (a, b) = pair;
来源：http://uge.vqdsnc.cn

[C16] 函数 / 方法重载
来源：http://ait.yvedp.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://adu.jyoumei.cn

PHP:  // 无重载
来源：http://ziw.fehbvm.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://otr.fehbvm.com

TS:   // 用联合类型或重载签名声明
来源：http://siu.zhoulong.xyz

Java: void f(int a) {}  void f(String a) {}
来源：http://ufi.fehbvm.com

Go:   // 无重载：用不同函数名
来源：http://pco.cdnleiting.top

Ruby: # 无重载：靠动态参数
来源：http://zby.chenjidiqi.icu

C#:   void F(int a) {}  void F(string a) {}
来源：http://llj.epnwcf.com

================================================================================
来源：http://zvp.daxiang520.top

D. 数组 / 列表 / 集合
来源：http://ryl.shanyushiyangkeji.top

================================================================================
来源：http://pot.chenjidiqi.icu

[D01] 创建数组 / 列表
来源：http://oja.xinyue.icu

Py:   arr = [1, 2, 3];  empty = []
来源：http://huk.yj202588.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://beo.yongpay.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://cnn.uphjek.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://ziq.ehwqpu.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://kmi.chenjidiqi.icu

Go:   arr := []int{1, 2, 3}
来源：http://twi.gotoacloud.top

Ruby: arr = [1, 2, 3]
来源：http://pwl.tarul.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://lhj.hfpthk.cn

[D02] 追加元素到末尾
来源：http://hrs.smart0.xyz

Py:   arr.append(4); arr.extend([5, 6])
来源：http://vpu.iojbl.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://qhp.jianghu66.top

JS:   arr.push(4);
来源：http://azs.zhoulong.xyz

TS:   arr.push(4);
来源：http://gha.yongpay.top

Java: list.add(4);
来源：http://vro.hongshengwenyu.top

Go:   arr = append(arr, 4)
来源：http://apl.yfazqb.com

Ruby: arr << 4; arr.push(5)
来源：http://oii.yj202588.top

C#:   list.Add(4);
来源：http://oyv.fehbvm.com

[D03] 在指定位置插入元素
来源：http://net.jinqigufen.top

Py:   arr.insert(0, 0)
来源：http://cvp.fehbvm.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://qiy.hnxiangtu.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://uqk.redwolf501.top

TS:   arr.splice(0, 0, 0);
来源：http://ooj.zhongyouzk.top

Java: list.add(0, 0);
来源：http://rbw.vqdsnc.cn

Go:   arr = append([]int{0}, arr...)
来源：http://hpn.shanyushiyangkeji.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wbp.cdnleiting.top

C#:   list.Insert(0, 0);
来源：http://fcr.hfpthk.cn

[D04] 删除元素
来源：http://kyn.pengpengdd.cyou

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://gnt.ppjwa.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ofb.wangshuangyany.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://nlp.shanyushiyangtech.top

TS:   arr.splice(0, 1);
来源：http://fre.kuanghao11.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://esx.zhixingplan.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://pdm.gotoacloud.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://nqo.hywenlv.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://sol.birdmap.top

[D05] 访问与修改元素
来源：http://fnz.fengsongda.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://bhl.guannengcc.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hfs.hammf.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://kpu.nwbrower.top

TS:   arr[0]; arr.at(-1);
来源：http://jhc.nanxuanxn.top

Java: list.get(0); list.set(0, 9);
来源：http://yqw.yj202588.top

Go:   arr[0]; arr[0] = 9
来源：http://szw.yj20258.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://iiu.guowangkeji.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ngg.ybcxt.top

[D06] 数组长度
来源：http://awu.sysykeji.top

Py:   len(arr)
来源：http://lbx.tian-w.cn

PHP:  count($arr);
来源：http://reb.chenlongwang.top

JS:   arr.length
来源：http://qtm.zdbjq.cn

TS:   arr.length
来源：http://juc.tanke756.top

Java: list.size();
来源：http://jrz.c1oappe.top

Go:   len(arr)
来源：http://bzf.snrcjt.cn

Ruby: arr.length; arr.size
来源：http://hky.gaohongyu789.top

C#:   list.Count;
来源：http://dfp.svipenyu.cn

[D07] 切片 / 取子数组
来源：http://vjy.0kj1m.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://lwp.xylfe.cn

PHP:  array_slice($arr, 1, 3);
来源：http://pxz.nwbrower.top

JS:   arr.slice(1, 4);
来源：http://edd.zhoulong.xyz

TS:   arr.slice(1, 4);
来源：http://qsq.yj20258.top

Java: list.subList(1, 4);
来源：http://mgk.9152youxi.cn

Go:   arr[1:4]
来源：http://ucx.daria6918.cn

Ruby: arr[1, 3]
来源：http://fvv.yj20258888.top

C#:   list.GetRange(1, 3);
来源：http://che.shzxlz.cn

[D08] 合并两个数组
来源：http://loi.tianlin.xyz

Py:   a + b;  a.extend(b)
来源：http://dqq.zdbjq.cn

PHP:  array_merge($a, $b);
来源：http://fnx.hongshengwenyu.top

JS:   [...a, ...b];  a.concat(b);
来源：http://vkc.tian-w.cn

TS:   [...a, ...b];
来源：http://tke.yvedp.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://gvt.svipenyu.cn

Go:   append(a, b...)
来源：http://qqf.xziqi.cn

Ruby: a + b;  a.concat(b)
来源：http://din.meibo888.top

C#:   a.Concat(b).ToList()
来源：http://bji.yuxming.cn

[D09] 排序（升序）
来源：http://pjk.aibaodan.cn

Py:   sorted(arr);  arr.sort()
来源：http://ajx.zdbjq.cn

PHP:  sort($arr);
来源：http://paz.cheryme.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mhc.zhijiandao.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://siq.yongpay.top

Java: Collections.sort(list);  list.sort(null);
来源：http://gpd.fehbvm.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://vgo.chenlongwang.top

Ruby: arr.sort
来源：http://nwh.ydjk.org.cn

C#:   list.Sort();
来源：http://mzv.smart0.xyz

[D10] 自定义排序（按字段 / 多条件）
来源：http://lvu.cucudq.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://yog.yj202588.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nty.hongshengwenyu.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hri.daria6918.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://izm.bjfxy.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://lng.chenjidiqi.icu

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://swn.jqgufenzy.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://dic.hcnkem.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hpk.chenlongwang.top

[D11] 反转数组
来源：http://bga.yueranfly.top

Py:   arr[::-1];  arr.reverse()
来源：http://iwk.ybcxt.top

PHP:  array_reverse($arr);
来源：http://vwy.tanke756.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vru.gogol.net.cn

TS:   [...arr].reverse();
来源：http://tmd.tanke756.top

Java: Collections.reverse(list);
来源：http://vsl.zdqjudy.top

Go:   slices.Reverse(arr)
来源：http://urb.mhx1999.top

Ruby: arr.reverse
来源：http://xbp.yuxming.cn

C#:   list.Reverse();
来源：http://kvg.quarkkingdee.top

[D12] 查找元素下标
来源：http://jjg.316326.xyz

Py:   arr.index(x);  x in arr
来源：http://cgt.sweek.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wqe.dashuyun.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nkn.daxiang520.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ljp.sysykeji.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ric.bjfxy.top

Go:   slices.Index(arr, x)
来源：http://drt.chenlongwang.top

Ruby: arr.index(x)
来源：http://usi.bbcook.cn

C#:   list.IndexOf(x);
来源：http://sdd.tanke756.top

[D13] 过滤（保留满足条件的）
来源：http://jiu.xuanzx.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://lwf.quarkkingdee.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wne.ybcxt.top

JS:   arr.filter(x => x > 3)
来源：http://vkw.xylfe.cn

TS:   arr.filter(x => x > 3)
来源：http://zhr.yonumen.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://pvi.yangfankeji.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://bpg.haohaochexian.top

Ruby: arr.select { |x| x > 3 }
来源：http://gss.yongpay.top

C#:   list.Where(x => x > 3).ToList()
来源：http://hrz.chenlongwang.top

[D14] 映射转换（每个元素变形）
来源：http://muq.shanyushiyangkeji.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://bvk.hywenlv.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zlf.fengsongda.top

JS:   arr.map(x => x * 2)
来源：http://ruc.wangdashe.top

TS:   arr.map(x => x * 2)
来源：http://qza.havefunace.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://wcp.xziqi.cn

Go:   // 手写循环
来源：http://dao.shzxlz.cn

Ruby: arr.map { |x| x * 2 }
来源：http://mmu.chenjidiqi.icu

C#:   list.Select(x => x * 2).ToList()
来源：http://pjv.ctjpmb.com

[D15] 去重
来源：http://ugj.tarul.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://yrn.ctjpmb.com

PHP:  array_unique($arr);
来源：http://ias.52xcode.cn

JS:   [...new Set(arr)]
来源：http://osj.yueranfly.top

TS:   [...new Set(arr)]
来源：http://pvf.sxryk.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://fpl.vehdjk.com

Go:   // 用 map[T]struct{} 手写
来源：http://oew.havefunace.top

Ruby: arr.uniq
来源：http://fsy.hcnkem.com

C#:   list.Distinct().ToList()
来源：http://sdo.hcnkem.com

[D16] 求和与平均值
来源：http://pqs.yj20258888.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://apt.shanyushiyangkeji.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mdo.fanxiaobao.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://afp.epnwcf.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ryk.cdnleiting.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://gpf.zhengqikj.top

Go:   // 手写循环累加
来源：http://nuu.shanyushiyangkeji.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://zqa.jinghuilouyu.cn

C#:   list.Sum();  list.Average()
来源：http://sfk.jinyuanbaomall.cn

[D17] 最大值与最小值
来源：http://jjx.vqdsnc.cn

Py:   max(arr);  min(arr)
来源：http://wnf.52xcode.cn

PHP:  max($arr);  min($arr);
来源：http://wpa.yj20258888.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ive.ybcxt.top

TS:   Math.max(...arr);
来源：http://fky.aibaodan.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://azz.yuanzhike.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wlj.tian-w.cn

Ruby: arr.max;  arr.min
来源：http://kxx.shuidangran.top

C#:   list.Max();  list.Min()
来源：http://toe.hesvh.cn

[D18] 扁平化嵌套数组
来源：http://cdh.nanxuanxn.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hvz.ywan-chungtsiang.top

PHP:  array_merge(...$nested);
来源：http://gwy.zhoulong.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ygk.sufxvd.cn

TS:   nested.flat();
来源：http://lzv.gotoacloud.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://owf.bjfxy.top

Go:   // 手写双层循环
来源：http://zgo.yanxiufei.cn

Ruby: nested.flatten
来源：http://yru.cheryme.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://air.ctjpmb.com


<!-- 参考信息 -->