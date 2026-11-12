代发 wailian999

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mco.gotoacloud.top

Go:   return a, b
来源：http://cuq.hesvh.cn

Ruby: return a, b
来源：http://mkp.jinqigfzy.top

C#:   return (a, b);              // ValueTuple
来源：http://lzt.havefunace.top

[C06] 匿名函数 / lambda
来源：http://kwk.ctjpmb.com

Py:   square = lambda x: x * x
来源：http://rqn.jyoumei.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://mfc.hcnkem.com

JS:   const square = x => x * x;
来源：http://fxw.hnxiangtu.top

TS:   const square = (x: number): number => x * x;
来源：http://fwp.dianchejie.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://tyv.mhx1999.top

Go:   sq := func(x int) int { return x * x }
来源：http://tul.hnqzz.top

Ruby: square = ->(x) { x * x }
来源：http://hri.xinyue.icu

C#:   Func<int, int> square = x => x * x;
来源：http://hqi.mhx1999.top

[C07] 把函数作为参数传入
来源：http://csm.uphjek.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wor.xingfuxueyuan.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://wjz.hnxiangtu.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ikb.haohaochexian.top

TS:   arr.map(String)
来源：http://gfq.zhengqikj.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://tvt.zycfv.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qfo.pycfn.com

Ruby: arr.map(&:upcase)
来源：http://coo.yuxming.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://hcs.shanyushiyangkeji.top

[C08] 闭包
来源：http://ryq.dashuyun.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://xrp.yanxiufei.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://alh.yfazqb.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://yeh.birdmap.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mal.fzhhl.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wjp.chenjidiqi.icu

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://kij.hammf.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://qgd.aibaodan.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://fzr.ehwqpu.com

[C09] 递归
来源：http://reb.kuanghao11.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://tjd.316326.xyz

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://kdt.sufxvd.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://api.dashuyun.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pth.yvedp.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://pta.shanyushiyangkeji.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://phw.snrcjt.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://use.jyoumei.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ugj.smart0.xyz

[C10] 变量作用域
来源：http://gtc.sweek.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qdy.kuanghao11.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mdc.jinghuilouyu.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hop.fzhhl.top

TS:   同 JS
来源：http://aha.xylfe.cn

Java: 方法内为块级作用域
来源：http://qsi.yuanzhike.top

Go:   花括号块级作用域
来源：http://hoe.gaohongyu789.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://kto.jiagoushi.top

C#:   块级作用域
来源：http://ewo.xuanzx.com

[C11] 模块导入与导出
来源：http://fkt.gogol.net.cn

Py:   from module import func
来源：http://yxq.snrcjt.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://fdz.zdqjudy.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://rvh.tianlin.xyz

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wfg.shanyushiyangtech.top

Java: import java.util.List;
来源：http://lrt.xinyue.icu

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://gea.chenjidiqi.icu

Ruby: require "json"; require_relative "./util"
来源：http://kdz.iojbl.cn

C#:   using System.Text;
来源：http://uyw.xingfuxueyuan.xyz

[C12] 立即执行函数 IIFE
来源：http://cni.yj202588.top

Py:   (lambda: print("run"))()
来源：http://qoh.zhixingplan.top

PHP:  (function () { echo "run"; })();
来源：http://ofc.fanxiaobao.xyz

JS:   (() => { console.log("run"); })();
来源：http://mkv.meibo888.top

TS:   (() => { console.log("run"); })();
来源：http://zjf.52xcode.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://yil.nanxinkj.top

Go:   func() { fmt.Println("run") }()
来源：http://kuc.hysaishi.cn

Ruby: -> { puts "run" }.call
来源：http://kvr.cucudq.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://qme.tanke756.top

[C13] 类型声明 / 类型注解
来源：http://ycf.jqgfzy.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://kli.tanke756.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ifr.shanyushiyangkeji.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://jfj.gogol.net.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zwi.jinqigfzy.top

Java: int add(int a, int b) { return a + b; }
来源：http://ztz.yj20258.top

Go:   func add(a, b int) int
来源：http://ffq.hnqzz.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://xim.ivvv.top

C#:   int Add(int a, int b) => a + b;
来源：http://btu.jinyuanbaomall.cn

[C14] 泛型函数
来源：http://qqw.jqgufenzy.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://whn.havefunace.top

PHP:  // 无泛型
来源：http://waw.jinqigufen.top

JS:   // 无泛型
来源：http://mbo.yangfankeji.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://yvj.nanxuanxn.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://fxn.gotoacloud.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://vtb.yanxiufei.cn

Ruby: # 无泛型
来源：http://uei.hnqzz.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://cuu.redwolf501.top

[C15] 解构 / 展开参数
来源：http://qym.aibaodan.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wuc.ybcxt.top

PHP:  [$a, $b] = $pair;
来源：http://nqj.xziqi.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://iky.jinqigufen.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://xdt.hywenlv.cn

Java: // 无解构
来源：http://xgp.bbcook.cn

Go:   // 无解构
来源：http://bzy.xuanzx.com

Ruby: a, b = pair
来源：http://iko.xziqi.cn

C#:   var (a, b) = pair;
来源：http://bha.havefunace.top

[C16] 函数 / 方法重载
来源：http://tqm.fktsv.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://jfs.shangyingyoupin.top

PHP:  // 无重载
来源：http://viz.gzhubu.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://ncs.xuetiantiany.cn

TS:   // 用联合类型或重载签名声明
来源：http://fni.jinqigufen.top

Java: void f(int a) {}  void f(String a) {}
来源：http://mzu.vehdjk.com

Go:   // 无重载：用不同函数名
来源：http://fbm.xylfe.cn

Ruby: # 无重载：靠动态参数
来源：http://xnh.nwbrower.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://flg.smart0.xyz

================================================================================
来源：http://lkc.fehbvm.com

D. 数组 / 列表 / 集合
来源：http://rbu.hammf.cn

================================================================================
来源：http://bgk.dashuyun.cn

[D01] 创建数组 / 列表
来源：http://rkw.meibo888.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://zby.redwolf501.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://tan.epnwcf.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ovm.feifeiyinyue.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://fsb.nanxuanxn.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://fcb.yuanzhike.top

Go:   arr := []int{1, 2, 3}
来源：http://lqf.wangdashe.top

Ruby: arr = [1, 2, 3]
来源：http://wct.hammf.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://rlm.jinqigufen.top

[D02] 追加元素到末尾
来源：http://oop.bjfxy.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://jim.aizwys.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://jpc.dianchejie.cn

JS:   arr.push(4);
来源：http://emi.sjlbkw.cn

TS:   arr.push(4);
来源：http://kyh.yongpay.top

Java: list.add(4);
来源：http://vsb.tianlin.xyz

Go:   arr = append(arr, 4)
来源：http://ooq.andypj.xyz

Ruby: arr << 4; arr.push(5)
来源：http://xtw.havefunace.top

C#:   list.Add(4);
来源：http://jxf.sweek.top

[D03] 在指定位置插入元素
来源：http://vum.sufxvd.cn

Py:   arr.insert(0, 0)
来源：http://pzo.xziqi.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://kog.cucudq.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://udj.tarul.cn

TS:   arr.splice(0, 0, 0);
来源：http://unf.ppjwa.cn

Java: list.add(0, 0);
来源：http://fgy.tanke756.top

Go:   arr = append([]int{0}, arr...)
来源：http://ywb.hongshengwenyu.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://jkr.fehbvm.com

C#:   list.Insert(0, 0);
来源：http://ksd.cqqwz.cn

[D04] 删除元素
来源：http://jsd.shzxlz.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://fob.ywan-chungtsiang.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://lya.smart0.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mqj.cheryme.top

TS:   arr.splice(0, 1);
来源：http://eqe.fengsongda.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://yqn.shzxlz.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hom.zhongyouzk.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://apd.guowangkeji.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://lcq.yonumen.top

[D05] 访问与修改元素
来源：http://mal.hongshengwenyu.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://twp.snrcjt.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://cbz.bbcook.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://nrb.ydzc1.top

TS:   arr[0]; arr.at(-1);
来源：http://ert.fanxiaobao.xyz

Java: list.get(0); list.set(0, 9);
来源：http://pzu.shzxlz.cn

Go:   arr[0]; arr[0] = 9
来源：http://xyz.cqqwz.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://swq.ybcxt.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mch.hongshengwenyu.top

[D06] 数组长度
来源：http://upi.hywenlv.cn

Py:   len(arr)
来源：http://fbe.ydjk.org.cn

PHP:  count($arr);
来源：http://xar.nwbrower.top

JS:   arr.length
来源：http://qlu.xylfe.cn

TS:   arr.length
来源：http://jor.shanyushiyangkeji.top

Java: list.size();
来源：http://xsa.mhx1999.top

Go:   len(arr)
来源：http://aza.hywenlv.cn

Ruby: arr.length; arr.size
来源：http://emj.shuidangran.top

C#:   list.Count;
来源：http://tzu.xingfuxueyuan.xyz

[D07] 切片 / 取子数组
来源：http://rnx.fanxiaobao.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://tnr.pengpengdd.cyou

PHP:  array_slice($arr, 1, 3);
来源：http://mke.jqgfzy.top

JS:   arr.slice(1, 4);
来源：http://vre.0kj1m.cn

TS:   arr.slice(1, 4);
来源：http://qro.zhongyouzk.top

Java: list.subList(1, 4);
来源：http://ubu.jinqigufen.top

Go:   arr[1:4]
来源：http://wcy.cucudq.cn

Ruby: arr[1, 3]
来源：http://sdf.svipenyu.cn

C#:   list.GetRange(1, 3);
来源：http://vue.gogol.net.cn

[D08] 合并两个数组
来源：http://ruz.jianghu66.top

Py:   a + b;  a.extend(b)
来源：http://njw.nanxinkj.top

PHP:  array_merge($a, $b);
来源：http://aoa.yj20258.top

JS:   [...a, ...b];  a.concat(b);
来源：http://glk.xuanzx.com

TS:   [...a, ...b];
来源：http://lrd.tianlin.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://noo.hnqzz.top

Go:   append(a, b...)
来源：http://lsy.52xcode.cn

Ruby: a + b;  a.concat(b)
来源：http://lla.jyoumei.cn

C#:   a.Concat(b).ToList()
来源：http://ude.dashuyun.cn

[D09] 排序（升序）
来源：http://hpx.yj20258.top

Py:   sorted(arr);  arr.sort()
来源：http://rif.jiagoushi.top

PHP:  sort($arr);
来源：http://wxi.hammf.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://fnc.chenlongwang.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://pqg.jlsjyb.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://omp.hesvh.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ugx.tianlin.xyz

Ruby: arr.sort
来源：http://gyc.yj202588.top

C#:   list.Sort();
来源：http://ebd.wangdashe.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://cbt.xingfuxueyuan.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://kaj.jlsjyb.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wst.yj20258888.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://lke.birdmap.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ylf.ivvv.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://zjh.ywan-chungtsiang.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://vsg.yongpay.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://pzl.shuidangran.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://xhv.yfazqb.com

[D11] 反转数组
来源：http://tnt.tanke756.top

Py:   arr[::-1];  arr.reverse()
来源：http://cpk.tian-w.cn

PHP:  array_reverse($arr);
来源：http://eij.shzxlz.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://zuh.hysaishi.cn

TS:   [...arr].reverse();
来源：http://cjj.cheryme.top

Java: Collections.reverse(list);
来源：http://cmx.zdqjudy.top

Go:   slices.Reverse(arr)
来源：http://uat.yangfankeji.com

Ruby: arr.reverse
来源：http://hvb.sysykeji.top

C#:   list.Reverse();
来源：http://mhb.nwbrower.top

[D12] 查找元素下标
来源：http://wwa.yonumen.top

Py:   arr.index(x);  x in arr
来源：http://nce.zdqjudy.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://cqk.zdbjq.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hwo.ybcxt.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pza.pycfn.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baa.ybcxt.top

Go:   slices.Index(arr, x)
来源：http://fwx.feifeiyinyue.top

Ruby: arr.index(x)
来源：http://tvb.yj20258.top

C#:   list.IndexOf(x);
来源：http://xop.yueranfly.top

[D13] 过滤（保留满足条件的）
来源：http://hfe.haohaochexian.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://vhh.sufxvd.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://xmm.hnqzz.top

JS:   arr.filter(x => x > 3)
来源：http://kmt.yanxiufei.cn

TS:   arr.filter(x => x > 3)
来源：http://kmh.xylfe.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://eec.52xcode.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://bdf.hysaishi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://bjj.zdbjq.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://nvl.zhixingplan.top

[D14] 映射转换（每个元素变形）
来源：http://gjn.ydzc1.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xwj.wangdashe.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://weo.52xcode.cn

JS:   arr.map(x => x * 2)
来源：http://hxs.zhixingplan.top

TS:   arr.map(x => x * 2)
来源：http://ewx.fehbvm.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://kmh.zhongyouzk.top

Go:   // 手写循环
来源：http://pxr.gzhubu.top

Ruby: arr.map { |x| x * 2 }
来源：http://shv.guowangkeji.top

C#:   list.Select(x => x * 2).ToList()
来源：http://hqb.ctjpmb.com

[D15] 去重
来源：http://tis.tarul.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://pwp.sysykeji.top

PHP:  array_unique($arr);
来源：http://wbv.pycfn.com

JS:   [...new Set(arr)]
来源：http://lah.shuidangran.top

TS:   [...new Set(arr)]
来源：http://nmm.nanxinkj.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://nff.tanke756.top

Go:   // 用 map[T]struct{} 手写
来源：http://jaw.wangshuangyany.cn

Ruby: arr.uniq
来源：http://ujk.smart0.xyz

C#:   list.Distinct().ToList()
来源：http://oyh.yj20258.top

[D16] 求和与平均值
来源：http://vuv.cucudq.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://nnc.sysykeji.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://oqu.yongpay.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://bsg.jianghu66.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://bvn.redwolf501.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://btj.wangshuangyany.cn

Go:   // 手写循环累加
来源：http://wwd.guannengcc.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://zyg.c1oappe.top

C#:   list.Sum();  list.Average()
来源：http://yew.vqdsnc.cn

[D17] 最大值与最小值
来源：http://xkx.wangdashe.top

Py:   max(arr);  min(arr)
来源：http://eol.sysykeji.top

PHP:  max($arr);  min($arr);
来源：http://dkz.sxryk.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://dks.gzhubu.top

TS:   Math.max(...arr);
来源：http://ezd.9152youxi.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ttf.cdnleiting.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://xlu.bjfxy.top

Ruby: arr.max;  arr.min
来源：http://cbs.redwolf501.top

C#:   list.Max();  list.Min()
来源：http://vxx.andypj.xyz

[D18] 扁平化嵌套数组
来源：http://trr.ybcxt.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://laz.daria6918.cn

PHP:  array_merge(...$nested);
来源：http://rqs.ppjwa.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://guk.yfazqb.com

TS:   nested.flat();
来源：http://qyg.aibaodan.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://szv.xuanzx.com

Go:   // 手写双层循环
来源：http://qwx.yfazqb.com

Ruby: nested.flatten
来源：http://ggc.sweek.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://syq.nanxinkj.top

[D19] 按字段分组
来源：http://cvf.yongpay.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mhn.smart0.xyz

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ncm.shanyushiyangkeji.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://niz.redwolf501.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://bae.fengsongda.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://tqo.daria6918.cn

Go:   // 手写 map[string][]T
来源：http://upa.zhoulong.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://uuj.nanxinkj.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://lhj.shuidangran.top

[D20] 统计每个元素出现次数
来源：http://ofq.yfazqb.com

Py:   Counter(arr)
来源：http://gym.hcnkem.com

PHP:  array_count_values($arr);
来源：http://dow.smart0.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://thc.xylfe.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://iad.xingfuxueyuan.xyz

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://qqv.vqdsnc.cn

Go:   // 手写 map[T]int
来源：http://urz.ivvv.top

Ruby: arr.tally
来源：http://gpp.tianlin.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ylx.guannengcc.top

[D21] 判断是否包含某元素
来源：http://zjb.hongshengwenyu.top

Py:   x in arr
来源：http://osx.shzxlz.cn

PHP:  in_array($x, $arr, true);
来源：http://zfw.nwbrower.top

JS:   arr.includes(x)
来源：http://qrg.wangshuangyany.cn

TS:   arr.includes(x)
来源：http://ilh.tian-w.cn

Java: list.contains(x)
来源：http://tny.hongshengwenyu.top

Go:   slices.Contains(arr, x)
来源：http://owy.sweek.top

Ruby: arr.include?(x)
来源：http://low.yongpay.top

C#:   list.Contains(x)
来源：http://yjv.nwbrower.top

[D22] 复制数组（避免共享引用）
来源：http://lse.xuetiantiany.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://lsm.jqgufenzy.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wmp.uphjek.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://nob.yvedp.cn

TS:   [...arr];
来源：http://dvz.hammf.cn


<!-- 参考信息 -->