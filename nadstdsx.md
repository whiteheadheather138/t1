代发 wailian999

Ruby: def total(*nums); nums.sum; end
来源：http://hfk.ivvv.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://nts.zhongyouzk.top

[C04] 命名参数 / 关键字参数
来源：http://dbk.gotoacloud.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wlv.hcnkem.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://dtp.tian-w.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://rle.yueranfly.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://uwn.hesvh.cn

Java: // 无：用 Builder 模式或 record
来源：http://aqz.cucudq.cn

Go:   // 无：用配置结构体参数
来源：http://aek.yvedp.cn

Ruby: f(a: 1, b: 2)
来源：http://mjn.yangfankeji.com

C#:   f(a: 1, b: 2)
来源：http://ifd.fengsongda.top

[C05] 返回多个值
来源：http://mia.52xcode.cn

Py:   return a, b
来源：http://sdw.tanke756.top

PHP:  return [$a, $b];
来源：http://qcn.hysaishi.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://kcg.cucudq.cn

TS:   return { a, b };
来源：http://lax.guowangkeji.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://nbk.fanxiaobao.xyz

Go:   return a, b
来源：http://slm.smart0.xyz

Ruby: return a, b
来源：http://tva.smart0.xyz

C#:   return (a, b);              // ValueTuple
来源：http://wtc.cqqwz.cn

[C06] 匿名函数 / lambda
来源：http://sks.jinqigfzy.top

Py:   square = lambda x: x * x
来源：http://yar.jinghuilouyu.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://pzt.dianchejie.cn

JS:   const square = x => x * x;
来源：http://hvj.hcnkem.com

TS:   const square = (x: number): number => x * x;
来源：http://dxa.uphjek.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://zez.hnxiangtu.top

Go:   sq := func(x int) int { return x * x }
来源：http://lyn.fktsv.cn

Ruby: square = ->(x) { x * x }
来源：http://tww.hesvh.cn

C#:   Func<int, int> square = x => x * x;
来源：http://hba.yj20258.top

[C07] 把函数作为参数传入
来源：http://iap.zhiwuduotai.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wrg.shuidangran.top

PHP:  array_map("strtoupper", $arr);
来源：http://fkr.tian-w.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ixh.zhongyouzk.top

TS:   arr.map(String)
来源：http://aoe.pengpengdd.cyou

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://qhb.pycfn.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://tsz.tianlin.xyz

Ruby: arr.map(&:upcase)
来源：http://olo.jinqigfzy.top

C#:   arr.Select(s => s.ToUpper())
来源：http://rvw.zhixingplan.top

[C08] 闭包
来源：http://cwo.ybcxt.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://aoz.yj202588.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://sos.jinghuilouyu.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qjy.xziqi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wls.hnqzz.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ogf.shangyingyoupin.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ket.gaohongyu789.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://afw.smart0.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://tzm.zhengqikj.top

[C09] 递归
来源：http://hiu.fengsongda.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ium.52xcode.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ulv.gaohongyu789.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://iyo.yueranfly.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zsx.c1oappe.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://glj.tianlin.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://nyp.xuanzx.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://kzo.guowangkeji.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://gfw.shanyushiyangkeji.top

[C10] 变量作用域
来源：http://iwn.sxryk.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://xqz.zhixingplan.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://jzl.cdnleiting.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://fsv.fzhhl.top

TS:   同 JS
来源：http://dma.hongshengwenyu.top

Java: 方法内为块级作用域
来源：http://ban.shanyushiyangtech.top

Go:   花括号块级作用域
来源：http://vrw.zdqjudy.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://bbk.ydjk.org.cn

C#:   块级作用域
来源：http://aid.jinyuanbaomall.cn

[C11] 模块导入与导出
来源：http://xbj.havefunace.top

Py:   from module import func
来源：http://bhj.xinyue.icu

PHP:  require "file.php";  或 use App\Service;
来源：http://txy.cqqwz.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://yvw.gogol.net.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://qri.dianchejie.cn

Java: import java.util.List;
来源：http://ugd.cucudq.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://yeg.jqgfzy.top

Ruby: require "json"; require_relative "./util"
来源：http://sln.yj202588.top

C#:   using System.Text;
来源：http://ffl.bjfxy.top

[C12] 立即执行函数 IIFE
来源：http://aln.shangyingyoupin.top

Py:   (lambda: print("run"))()
来源：http://plz.wangdashe.top

PHP:  (function () { echo "run"; })();
来源：http://mrw.fehbvm.com

JS:   (() => { console.log("run"); })();
来源：http://gmx.zhongyouzk.top

TS:   (() => { console.log("run"); })();
来源：http://mjy.hongshengwenyu.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ovg.tanke756.top

Go:   func() { fmt.Println("run") }()
来源：http://lnt.yueranfly.top

Ruby: -> { puts "run" }.call
来源：http://iln.ehwqpu.com

C#:   // 无 IIFE：用静态构造函数
来源：http://ygy.yanxiufei.cn

[C13] 类型声明 / 类型注解
来源：http://byw.wangshuangyany.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://qqi.vehdjk.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rpg.daria6918.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://eyw.snrcjt.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ahj.cdnleiting.top

Java: int add(int a, int b) { return a + b; }
来源：http://xwu.yangfankeji.com

Go:   func add(a, b int) int
来源：http://oju.gogol.net.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://gel.fzhhl.top

C#:   int Add(int a, int b) => a + b;
来源：http://czx.yanxiufei.cn

[C14] 泛型函数
来源：http://njz.jlsjyb.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ymb.tian-w.cn

PHP:  // 无泛型
来源：http://xcq.epnwcf.com

JS:   // 无泛型
来源：http://zwe.havefunace.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://xjv.yonumen.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ait.tanke756.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://fpu.zhiwuduotai.top

Ruby: # 无泛型
来源：http://ppo.ivvv.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ojx.c1oappe.top

[C15] 解构 / 展开参数
来源：http://npk.xinyue.icu

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://uaq.yj20258.top

PHP:  [$a, $b] = $pair;
来源：http://erj.ydzc1.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wkl.cdnleiting.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ass.mhx1999.top

Java: // 无解构
来源：http://juz.nanxinkj.top

Go:   // 无解构
来源：http://wrr.316326.xyz

Ruby: a, b = pair
来源：http://yid.jqgfzy.top

C#:   var (a, b) = pair;
来源：http://cmr.52xcode.cn

[C16] 函数 / 方法重载
来源：http://afc.yonumen.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://zgy.yvedp.cn

PHP:  // 无重载
来源：http://pwf.ywan-chungtsiang.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://bqe.daxiang520.top

TS:   // 用联合类型或重载签名声明
来源：http://xdi.guannengcc.top

Java: void f(int a) {}  void f(String a) {}
来源：http://rnp.yangfankeji.com

Go:   // 无重载：用不同函数名
来源：http://jay.fzhhl.top

Ruby: # 无重载：靠动态参数
来源：http://sks.birdmap.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://rme.hcnkem.com

================================================================================
来源：http://fkg.zhengqikj.top

D. 数组 / 列表 / 集合
来源：http://vab.wangshuangyany.cn

================================================================================
来源：http://tjv.chenlongwang.top

[D01] 创建数组 / 列表
来源：http://atb.gotoacloud.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://jjj.sxryk.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://fta.guannengcc.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://fan.hnqzz.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://uhl.jinghuilouyu.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://cvj.ybcxt.top

Go:   arr := []int{1, 2, 3}
来源：http://vux.daria6918.cn

Ruby: arr = [1, 2, 3]
来源：http://flu.ywan-chungtsiang.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://nqi.yfazqb.com

[D02] 追加元素到末尾
来源：http://mfi.yueranfly.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ufl.nwbrower.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://aal.fanxiaobao.xyz

JS:   arr.push(4);
来源：http://dsv.ywan-chungtsiang.top

TS:   arr.push(4);
来源：http://unx.tianlin.xyz

Java: list.add(4);
来源：http://mhr.yongpay.top

Go:   arr = append(arr, 4)
来源：http://hny.hnxiangtu.top

Ruby: arr << 4; arr.push(5)
来源：http://dpg.kuanghao11.cn

C#:   list.Add(4);
来源：http://baz.mhx1999.top

[D03] 在指定位置插入元素
来源：http://klx.52xcode.cn

Py:   arr.insert(0, 0)
来源：http://bnz.ctjpmb.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://zje.ehwqpu.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://uqq.pycfn.com

TS:   arr.splice(0, 0, 0);
来源：http://yof.uphjek.com

Java: list.add(0, 0);
来源：http://mus.hesvh.cn

Go:   arr = append([]int{0}, arr...)
来源：http://dkz.cqqwz.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://myb.nanxinkj.top

C#:   list.Insert(0, 0);
来源：http://gnw.hammf.cn

[D04] 删除元素
来源：http://lmq.zhiwuduotai.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ycr.jlsjyb.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://qkw.snrcjt.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://roh.ybcxt.top

TS:   arr.splice(0, 1);
来源：http://frs.aizwys.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://qub.andypj.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ifj.hysaishi.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ahh.nanxinkj.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://jgf.pengpengdd.cyou

[D05] 访问与修改元素
来源：http://seu.guannengcc.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://atu.sufxvd.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mqa.sjlbkw.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://rlt.cqqwz.cn

TS:   arr[0]; arr.at(-1);
来源：http://wys.sufxvd.cn

Java: list.get(0); list.set(0, 9);
来源：http://mpk.ydjk.org.cn

Go:   arr[0]; arr[0] = 9
来源：http://lhw.birdmap.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://voy.hesvh.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ouk.zhaomingkeji.xyz

[D06] 数组长度
来源：http://nrz.yj20258888.top

Py:   len(arr)
来源：http://ogf.guowangkeji.top

PHP:  count($arr);
来源：http://cex.dianchejie.cn

JS:   arr.length
来源：http://khn.kuanghao11.cn

TS:   arr.length
来源：http://ocl.jinqigfzy.top

Java: list.size();
来源：http://rcq.mhx1999.top

Go:   len(arr)
来源：http://mwp.zhongyouzk.top

Ruby: arr.length; arr.size
来源：http://ahg.zhiwuduotai.top

C#:   list.Count;
来源：http://jnr.tian-w.cn

[D07] 切片 / 取子数组
来源：http://olp.jyoumei.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://bzc.yongpay.top

PHP:  array_slice($arr, 1, 3);
来源：http://hqx.jinyuanbaomall.cn

JS:   arr.slice(1, 4);
来源：http://byb.316326.xyz

TS:   arr.slice(1, 4);
来源：http://afc.aibaodan.cn

Java: list.subList(1, 4);
来源：http://utv.jianghu66.top

Go:   arr[1:4]
来源：http://hdq.sufxvd.cn

Ruby: arr[1, 3]
来源：http://aat.jqgfzy.top

C#:   list.GetRange(1, 3);
来源：http://hbs.wangdashe.top

[D08] 合并两个数组
来源：http://ffc.wangshuangyany.cn

Py:   a + b;  a.extend(b)
来源：http://wfk.mhx1999.top

PHP:  array_merge($a, $b);
来源：http://lji.xuetiantiany.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://gyx.xziqi.cn

TS:   [...a, ...b];
来源：http://eqy.aizwys.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://gly.hesvh.cn

Go:   append(a, b...)
来源：http://yzo.fktsv.cn

Ruby: a + b;  a.concat(b)
来源：http://jrr.yonumen.top

C#:   a.Concat(b).ToList()
来源：http://eac.9152youxi.cn

[D09] 排序（升序）
来源：http://zkd.sufxvd.cn

Py:   sorted(arr);  arr.sort()
来源：http://ysy.yj20258.top

PHP:  sort($arr);
来源：http://gyo.cucudq.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://cna.jqgufenzy.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://hkd.yj202588.top

Java: Collections.sort(list);  list.sort(null);
来源：http://sam.cheryme.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://gqg.daria6918.cn

Ruby: arr.sort
来源：http://taz.jinghuilouyu.cn

C#:   list.Sort();
来源：http://bvn.jiagoushi.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://vrs.shangyingyoupin.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://xye.zdqjudy.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hji.ivvv.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ril.yvedp.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://dpe.haohaochexian.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://vrk.zycfv.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://nvg.gogol.net.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://gqt.yvedp.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://tlt.hysaishi.cn

[D11] 反转数组
来源：http://wqq.bbcook.cn

Py:   arr[::-1];  arr.reverse()
来源：http://fuu.hongshengwenyu.top

PHP:  array_reverse($arr);
来源：http://gcx.nwbrower.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://byo.wangshuangyany.cn

TS:   [...arr].reverse();
来源：http://nqx.yvedp.cn

Java: Collections.reverse(list);
来源：http://qqf.0kj1m.cn

Go:   slices.Reverse(arr)
来源：http://uqj.yj20258.top

Ruby: arr.reverse
来源：http://glu.jlsjyb.cn

C#:   list.Reverse();
来源：http://ytz.ctjpmb.com

[D12] 查找元素下标
来源：http://wkf.9152youxi.cn

Py:   arr.index(x);  x in arr
来源：http://mum.chenzaomai.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://tqg.jianghu66.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://awo.jinyuanbaomall.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yph.yueranfly.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://jxx.meibo888.top

Go:   slices.Index(arr, x)
来源：http://yre.snrcjt.cn

Ruby: arr.index(x)
来源：http://ndl.bjfxy.top

C#:   list.IndexOf(x);
来源：http://yyv.ydjk.org.cn

[D13] 过滤（保留满足条件的）
来源：http://yab.xingfuxueyuan.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://nkt.xziqi.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://unh.ehwqpu.com

JS:   arr.filter(x => x > 3)
来源：http://kcv.yuanzhike.top

TS:   arr.filter(x => x > 3)
来源：http://rtp.jlsjyb.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hxk.zdbjq.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://esm.gzhubu.top

Ruby: arr.select { |x| x > 3 }
来源：http://mdw.chenzaomai.com

C#:   list.Where(x => x > 3).ToList()
来源：http://imz.sufxvd.cn

[D14] 映射转换（每个元素变形）
来源：http://hoc.jqgfzy.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ctz.sxryk.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://qml.wangshuangyany.cn

JS:   arr.map(x => x * 2)
来源：http://kvt.smart0.xyz

TS:   arr.map(x => x * 2)
来源：http://eqa.zhongyouzk.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://blj.cheryme.top

Go:   // 手写循环
来源：http://ssz.guannengcc.top

Ruby: arr.map { |x| x * 2 }
来源：http://whj.cqqwz.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://zby.epnwcf.com

[D15] 去重
来源：http://mpg.bjfxy.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://oso.shangyingyoupin.top

PHP:  array_unique($arr);
来源：http://sgj.cdnleiting.top

JS:   [...new Set(arr)]
来源：http://nbd.andypj.xyz

TS:   [...new Set(arr)]
来源：http://xft.shangyingyoupin.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mco.vqdsnc.cn

Go:   // 用 map[T]struct{} 手写
来源：http://fqe.fktsv.cn

Ruby: arr.uniq
来源：http://pnf.quarkkingdee.top

C#:   list.Distinct().ToList()
来源：http://nsw.yj20258.top

[D16] 求和与平均值
来源：http://vau.gogol.net.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://snt.vqdsnc.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://jfj.kuanghao11.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://xgp.ybcxt.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://dan.ybcxt.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mcj.zycfv.cn

Go:   // 手写循环累加
来源：http://hxx.svipenyu.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://vdu.yangfankeji.com

C#:   list.Sum();  list.Average()
来源：http://mqf.chenzaomai.com

[D17] 最大值与最小值
来源：http://cac.cheryme.top

Py:   max(arr);  min(arr)
来源：http://yqr.cdnleiting.top

PHP:  max($arr);  min($arr);
来源：http://njy.zhongyouzk.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://fye.zhixingplan.top

TS:   Math.max(...arr);
来源：http://tbm.yuxming.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://oyi.xziqi.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hll.xuetiantiany.cn

Ruby: arr.max;  arr.min
来源：http://kru.shuidangran.top

C#:   list.Max();  list.Min()
来源：http://pkd.zhongyouzk.top

[D18] 扁平化嵌套数组
来源：http://ctr.vqdsnc.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://idn.cheryme.top

PHP:  array_merge(...$nested);
来源：http://cvh.chenzaomai.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ecz.xuetiantiany.cn

TS:   nested.flat();
来源：http://mre.zhengqikj.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://cce.tianlin.xyz

Go:   // 手写双层循环
来源：http://nrq.jianghu66.top

Ruby: nested.flatten
来源：http://vei.bbcook.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://xga.hongshengwenyu.top

[D19] 按字段分组
来源：http://zyp.xinyue.icu

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wbr.zdqjudy.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://zzc.ydjk.org.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://eqr.vqdsnc.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://jne.dianchejie.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://xga.fzhhl.top

Go:   // 手写 map[string][]T
来源：http://vxe.nanxuanxn.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://yaa.316326.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://brs.redwolf501.top

[D20] 统计每个元素出现次数
来源：http://ipz.wangdashe.top

Py:   Counter(arr)
来源：http://nxg.jyoumei.cn

PHP:  array_count_values($arr);
来源：http://qsv.zhengqikj.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kyh.cashguo.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ouq.hcnkem.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://fse.ehwqpu.com

Go:   // 手写 map[T]int
来源：http://fvu.jyoumei.cn


<!-- 参考信息 -->