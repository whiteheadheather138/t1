代发 wailian999

C#:   Func<int, int> square = x => x * x;
来源：http://zbl.quarkkingdee.top

[C07] 把函数作为参数传入
来源：http://mmd.birdmap.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wlh.c1oappe.top

PHP:  array_map("strtoupper", $arr);
来源：http://qwy.cheryme.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://oia.jqgfzy.top

TS:   arr.map(String)
来源：http://zep.guannengcc.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ivh.jinqigufen.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hdj.9152youxi.cn

Ruby: arr.map(&:upcase)
来源：http://zuq.kuanghao11.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://cbk.meibo888.top

[C08] 闭包
来源：http://mky.daria6918.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://lms.ydjk.org.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://rst.daria6918.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://grj.52xcode.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wom.chenzaomai.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://qee.uphjek.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://oaf.hfpthk.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://fhn.kuanghao11.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ofd.daria6918.cn

[C09] 递归
来源：http://tem.vqdsnc.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://nyr.hesvh.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://emf.gotoacloud.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ydi.gaohongyu789.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://aae.jinqigfzy.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://uvp.gaohongyu789.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://rtj.jinqigfzy.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://yvd.ydjk.org.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hhc.aibaodan.cn

[C10] 变量作用域
来源：http://qvu.redwolf501.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://uxq.zdqjudy.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://gvm.bjfxy.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hqe.andypj.xyz

TS:   同 JS
来源：http://xow.quarkkingdee.top

Java: 方法内为块级作用域
来源：http://pzd.svipenyu.cn

Go:   花括号块级作用域
来源：http://sfj.yanxiufei.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xoe.fehbvm.com

C#:   块级作用域
来源：http://fmv.bjfxy.top

[C11] 模块导入与导出
来源：http://izj.hysaishi.cn

Py:   from module import func
来源：http://ehr.jiagoushi.top

PHP:  require "file.php";  或 use App\Service;
来源：http://vsi.yongpay.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://kgv.tianlin.xyz

TS:   export function f(): void {};  import { f } from "./m";
来源：http://bzz.zhoulong.xyz

Java: import java.util.List;
来源：http://stm.gogol.net.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://qmv.guannengcc.top

Ruby: require "json"; require_relative "./util"
来源：http://gpw.fehbvm.com

C#:   using System.Text;
来源：http://mrr.uphjek.com

[C12] 立即执行函数 IIFE
来源：http://tow.birdmap.top

Py:   (lambda: print("run"))()
来源：http://oez.fehbvm.com

PHP:  (function () { echo "run"; })();
来源：http://qvo.shuidangran.top

JS:   (() => { console.log("run"); })();
来源：http://kmy.c1oappe.top

TS:   (() => { console.log("run"); })();
来源：http://auw.yj202588.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://phq.vqdsnc.cn

Go:   func() { fmt.Println("run") }()
来源：http://hdn.zhengqikj.top

Ruby: -> { puts "run" }.call
来源：http://dzb.jinghuilouyu.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://mzz.zdqjudy.top

[C13] 类型声明 / 类型注解
来源：http://ilm.ydzc1.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://yla.wangdashe.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hia.ivvv.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://oiq.sufxvd.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wqn.yuanzhike.top

Java: int add(int a, int b) { return a + b; }
来源：http://skl.hongshengwenyu.top

Go:   func add(a, b int) int
来源：http://bel.gaohongyu789.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://frx.tian-w.cn

C#:   int Add(int a, int b) => a + b;
来源：http://auy.shanyushiyangkeji.top

[C14] 泛型函数
来源：http://lgn.hfpthk.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://fvc.mhx1999.top

PHP:  // 无泛型
来源：http://hpc.ydzc1.top

JS:   // 无泛型
来源：http://xaq.fktsv.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://biz.shanyushiyangkeji.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ikr.fanxiaobao.xyz

Go:   func First[T any](items []T) T { return items[0] }
来源：http://dzk.ydzc1.top

Ruby: # 无泛型
来源：http://kul.yanxiufei.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://dfc.nanxuanxn.top

[C15] 解构 / 展开参数
来源：http://uuj.shzxlz.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://vyk.yueranfly.top

PHP:  [$a, $b] = $pair;
来源：http://nqd.fzhhl.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ugz.jyoumei.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://zia.fzhhl.top

Java: // 无解构
来源：http://qar.quarkkingdee.top

Go:   // 无解构
来源：http://mvp.birdmap.top

Ruby: a, b = pair
来源：http://cem.hongshengwenyu.top

C#:   var (a, b) = pair;
来源：http://gng.52xcode.cn

[C16] 函数 / 方法重载
来源：http://vuv.svipenyu.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vwd.gogol.net.cn

PHP:  // 无重载
来源：http://fkt.cqqwz.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://gtq.yonumen.top

TS:   // 用联合类型或重载签名声明
来源：http://rmn.pycfn.com

Java: void f(int a) {}  void f(String a) {}
来源：http://pnj.hnqzz.top

Go:   // 无重载：用不同函数名
来源：http://kxi.jinqigfzy.top

Ruby: # 无重载：靠动态参数
来源：http://arw.uphjek.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://zbu.cheryme.top

================================================================================
来源：http://ryl.daxiang520.top

D. 数组 / 列表 / 集合
来源：http://wxo.nwbrower.top

================================================================================
来源：http://dsw.hongshengwenyu.top

[D01] 创建数组 / 列表
来源：http://krb.hnxiangtu.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://ljh.ydjk.org.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://pjr.sxryk.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://rej.birdmap.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://qqq.zhaomingkeji.xyz

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://yyd.snrcjt.cn

Go:   arr := []int{1, 2, 3}
来源：http://quo.feifeiyinyue.top

Ruby: arr = [1, 2, 3]
来源：http://lct.guowangkeji.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://zon.fktsv.cn

[D02] 追加元素到末尾
来源：http://ucc.hongshengwenyu.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://fno.kuanghao11.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://rdr.gzhubu.top

JS:   arr.push(4);
来源：http://eqm.yj202588.top

TS:   arr.push(4);
来源：http://tff.guowangkeji.top

Java: list.add(4);
来源：http://ugd.gzhubu.top

Go:   arr = append(arr, 4)
来源：http://xrm.iojbl.cn

Ruby: arr << 4; arr.push(5)
来源：http://kuo.0kj1m.cn

C#:   list.Add(4);
来源：http://uxv.yj202588.top

[D03] 在指定位置插入元素
来源：http://huj.cdnleiting.top

Py:   arr.insert(0, 0)
来源：http://ebw.feifeiyinyue.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://kvr.wangdashe.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ruc.hysaishi.cn

TS:   arr.splice(0, 0, 0);
来源：http://eoi.jinqigfzy.top

Java: list.add(0, 0);
来源：http://zpz.tarul.cn

Go:   arr = append([]int{0}, arr...)
来源：http://aeu.jiagoushi.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://nop.vehdjk.com

C#:   list.Insert(0, 0);
来源：http://aiz.smart0.xyz

[D04] 删除元素
来源：http://yze.feifeiyinyue.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://jac.hfpthk.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ohe.guowangkeji.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://klj.jinghuilouyu.cn

TS:   arr.splice(0, 1);
来源：http://ewd.tianlin.xyz

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://idb.zhixingplan.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://piw.jinghuilouyu.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://fzo.ppjwa.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mcs.fktsv.cn

[D05] 访问与修改元素
来源：http://vbd.0kj1m.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ael.wangdashe.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://lpj.chenjidiqi.icu

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://qav.fehbvm.com

TS:   arr[0]; arr.at(-1);
来源：http://wlr.vehdjk.com

Java: list.get(0); list.set(0, 9);
来源：http://pkf.fktsv.cn

Go:   arr[0]; arr[0] = 9
来源：http://ggm.gaohongyu789.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://aja.aizwys.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://gxt.dashuyun.cn

[D06] 数组长度
来源：http://vrk.xinyue.icu

Py:   len(arr)
来源：http://qki.hnxiangtu.top

PHP:  count($arr);
来源：http://qlo.zhiwuduotai.top

JS:   arr.length
来源：http://yvv.bjfxy.top

TS:   arr.length
来源：http://slf.haohaochexian.top

Java: list.size();
来源：http://fqq.fzhhl.top

Go:   len(arr)
来源：http://ssg.fengsongda.top

Ruby: arr.length; arr.size
来源：http://otw.jiagoushi.top

C#:   list.Count;
来源：http://zur.mhx1999.top

[D07] 切片 / 取子数组
来源：http://syp.tarul.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://tkv.0kj1m.cn

PHP:  array_slice($arr, 1, 3);
来源：http://kqh.shzxlz.cn

JS:   arr.slice(1, 4);
来源：http://ugy.pycfn.com

TS:   arr.slice(1, 4);
来源：http://vrn.ydzc1.top

Java: list.subList(1, 4);
来源：http://xtt.jiagoushi.top

Go:   arr[1:4]
来源：http://ild.dashuyun.cn

Ruby: arr[1, 3]
来源：http://fbs.hcnkem.com

C#:   list.GetRange(1, 3);
来源：http://vsn.sufxvd.cn

[D08] 合并两个数组
来源：http://acm.hongshengwenyu.top

Py:   a + b;  a.extend(b)
来源：http://ypd.sxryk.cn

PHP:  array_merge($a, $b);
来源：http://ojs.zhiwuduotai.top

JS:   [...a, ...b];  a.concat(b);
来源：http://eol.hywenlv.cn

TS:   [...a, ...b];
来源：http://bkd.svipenyu.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://cxg.birdmap.top

Go:   append(a, b...)
来源：http://ajw.zhijiandao.cn

Ruby: a + b;  a.concat(b)
来源：http://grw.bjfxy.top

C#:   a.Concat(b).ToList()
来源：http://ubi.birdmap.top

[D09] 排序（升序）
来源：http://gvx.xinyue.icu

Py:   sorted(arr);  arr.sort()
来源：http://okv.hongshengwenyu.top

PHP:  sort($arr);
来源：http://vew.dashuyun.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://qux.xingfuxueyuan.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://fsu.guannengcc.top

Java: Collections.sort(list);  list.sort(null);
来源：http://fft.iojbl.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://rql.jiagoushi.top

Ruby: arr.sort
来源：http://wnt.sjlbkw.cn

C#:   list.Sort();
来源：http://wov.jinqigfzy.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://dqm.feifeiyinyue.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://xkn.dashuyun.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://uer.yuxming.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://byl.guannengcc.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hxr.bjfxy.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://pzm.zhijiandao.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://pmz.jqgufenzy.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://msd.chenzaomai.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://guw.uphjek.com

[D11] 反转数组
来源：http://xny.yonumen.top

Py:   arr[::-1];  arr.reverse()
来源：http://rvx.hysaishi.cn

PHP:  array_reverse($arr);
来源：http://ijo.yueranfly.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://bvp.ivvv.top

TS:   [...arr].reverse();
来源：http://wnr.jinghuilouyu.cn

Java: Collections.reverse(list);
来源：http://klx.316326.xyz

Go:   slices.Reverse(arr)
来源：http://stc.wangshuangyany.cn

Ruby: arr.reverse
来源：http://dkk.sysykeji.top

C#:   list.Reverse();
来源：http://cxj.zhengqikj.top

[D12] 查找元素下标
来源：http://jjy.hammf.cn

Py:   arr.index(x);  x in arr
来源：http://daj.ydzc1.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://lnb.birdmap.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bvk.daxiang520.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jod.shzxlz.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ohf.fzhhl.top

Go:   slices.Index(arr, x)
来源：http://xxd.jianghu66.top

Ruby: arr.index(x)
来源：http://kso.jinyuanbaomall.cn

C#:   list.IndexOf(x);
来源：http://lmm.zycfv.cn

[D13] 过滤（保留满足条件的）
来源：http://kiw.jinqigfzy.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://skz.ydjk.org.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://eql.cucudq.cn

JS:   arr.filter(x => x > 3)
来源：http://she.redwolf501.top

TS:   arr.filter(x => x > 3)
来源：http://ccv.hywenlv.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://xqq.zhoulong.xyz

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://loc.jqgufenzy.top

Ruby: arr.select { |x| x > 3 }
来源：http://uaf.xuanzx.com

C#:   list.Where(x => x > 3).ToList()
来源：http://upw.zhijiandao.cn

[D14] 映射转换（每个元素变形）
来源：http://gfs.yj202588.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ynt.zhoulong.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://snd.jqgfzy.top

JS:   arr.map(x => x * 2)
来源：http://bea.cqqwz.cn

TS:   arr.map(x => x * 2)
来源：http://pqz.shzxlz.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://cna.meibo888.top

Go:   // 手写循环
来源：http://ate.yongpay.top

Ruby: arr.map { |x| x * 2 }
来源：http://rdm.meibo888.top

C#:   list.Select(x => x * 2).ToList()
来源：http://xje.zdbjq.cn

[D15] 去重
来源：http://nqx.sufxvd.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://fdm.cdnleiting.top

PHP:  array_unique($arr);
来源：http://erk.yj202588.top

JS:   [...new Set(arr)]
来源：http://ayg.ctjpmb.com

TS:   [...new Set(arr)]
来源：http://flc.dashuyun.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://jjp.tianlin.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://apl.nwbrower.top

Ruby: arr.uniq
来源：http://ifv.smart0.xyz

C#:   list.Distinct().ToList()
来源：http://usj.tarul.cn

[D16] 求和与平均值
来源：http://lnq.shangyingyoupin.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://lqs.ivvv.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://yve.zhijiandao.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ywd.tanke756.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://afm.tanke756.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://exe.jianghu66.top

Go:   // 手写循环累加
来源：http://nmt.chenjidiqi.icu

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://uvd.zycfv.cn

C#:   list.Sum();  list.Average()
来源：http://qoj.52xcode.cn

[D17] 最大值与最小值
来源：http://jrk.yonumen.top

Py:   max(arr);  min(arr)
来源：http://bry.yuxming.cn

PHP:  max($arr);  min($arr);
来源：http://fpk.c1oappe.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://qwd.hfpthk.cn

TS:   Math.max(...arr);
来源：http://cnf.xziqi.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://mje.yj202588.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://xek.ydjk.org.cn

Ruby: arr.max;  arr.min
来源：http://hbg.shanyushiyangtech.top

C#:   list.Max();  list.Min()
来源：http://snb.shuidangran.top

[D18] 扁平化嵌套数组
来源：http://ute.fehbvm.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://evi.gzhubu.top

PHP:  array_merge(...$nested);
来源：http://rkt.havefunace.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://nim.zhoulong.xyz

TS:   nested.flat();
来源：http://pny.bjfxy.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://voi.ydjk.org.cn

Go:   // 手写双层循环
来源：http://qvt.jinqigfzy.top

Ruby: nested.flatten
来源：http://kut.svipenyu.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://pag.wangshuangyany.cn

[D19] 按字段分组
来源：http://bwt.chenzaomai.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://drb.hongshengwenyu.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://glz.hnxiangtu.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://lgv.ehwqpu.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://kba.hnxiangtu.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mmg.meibo888.top

Go:   // 手写 map[string][]T
来源：http://ggs.sysykeji.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://mbl.uphjek.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://vnv.pycfn.com

[D20] 统计每个元素出现次数
来源：http://qxw.daria6918.cn

Py:   Counter(arr)
来源：http://egv.xuanzx.com

PHP:  array_count_values($arr);
来源：http://apq.shanyushiyangtech.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sqa.guannengcc.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hib.0kj1m.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://rpd.jyoumei.cn

Go:   // 手写 map[T]int
来源：http://wsg.zycfv.cn

Ruby: arr.tally
来源：http://whi.shangyingyoupin.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://tit.birdmap.top

[D21] 判断是否包含某元素
来源：http://qtd.zdqjudy.top

Py:   x in arr
来源：http://iyz.wangdashe.top

PHP:  in_array($x, $arr, true);
来源：http://nbx.bbcook.cn

JS:   arr.includes(x)
来源：http://efo.9152youxi.cn

TS:   arr.includes(x)
来源：http://jak.guowangkeji.top

Java: list.contains(x)
来源：http://dec.cashguo.top

Go:   slices.Contains(arr, x)
来源：http://iyx.xuanzx.com

Ruby: arr.include?(x)
来源：http://clk.ydjk.org.cn

C#:   list.Contains(x)
来源：http://zet.jinghuilouyu.cn

[D22] 复制数组（避免共享引用）
来源：http://hcv.aizwys.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://jwa.9152youxi.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://aja.wangdashe.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://tme.nwbrower.top

TS:   [...arr];
来源：http://thb.zdbjq.cn

Java: new ArrayList<>(list);
来源：http://mns.yanxiufei.cn

Go:   copied := append([]int(nil), arr...)
来源：http://cun.gaohongyu789.top

Ruby: arr.dup;  arr.clone
来源：http://qzt.nwbrower.top

C#:   new List<int>(list);
来源：http://ywp.xuanzx.com

[D23] reduce 累积计算
来源：http://cwx.zdbjq.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ugj.snrcjt.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ttg.meibo888.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://agv.bbcook.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ikj.bbcook.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://lvt.yonumen.top

Go:   // 手写循环
来源：http://zrd.cdnleiting.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://tph.yuxming.cn


<!-- 参考信息 -->