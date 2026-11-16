代发 wailian999

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://fzb.nanxuanxn.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://cgj.jiagoushi.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://rdz.zhaomingkeji.xyz

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://xbv.hfpthk.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://qnm.tanke756.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ohw.yangfankeji.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://fjn.zhixingplan.top

[C09] 递归
来源：http://hvj.quarkkingdee.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ski.daxiang520.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://egf.jinyuanbaomall.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://iag.cashguo.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fpr.sxryk.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://rlk.yongpay.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mdv.feifeiyinyue.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://jjr.yangfankeji.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://nxg.cdnleiting.top

[C10] 变量作用域
来源：http://ril.sweek.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://dyp.guannengcc.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mkj.wangshuangyany.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://tmj.zycfv.cn

TS:   同 JS
来源：http://psn.zdbjq.cn

Java: 方法内为块级作用域
来源：http://fyc.xinyue.icu

Go:   花括号块级作用域
来源：http://gjo.birdmap.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://eej.uphjek.com

C#:   块级作用域
来源：http://qzw.jinqigfzy.top

[C11] 模块导入与导出
来源：http://ibz.chenlongwang.top

Py:   from module import func
来源：http://hgq.nanxinkj.top

PHP:  require "file.php";  或 use App\Service;
来源：http://ikk.daxiang520.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://wkc.yongpay.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://yhm.fzhhl.top

Java: import java.util.List;
来源：http://rpn.shzxlz.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://uwh.daria6918.cn

Ruby: require "json"; require_relative "./util"
来源：http://hul.0kj1m.cn

C#:   using System.Text;
来源：http://nmz.sufxvd.cn

[C12] 立即执行函数 IIFE
来源：http://uhm.yj20258.top

Py:   (lambda: print("run"))()
来源：http://jrd.gotoacloud.top

PHP:  (function () { echo "run"; })();
来源：http://qwb.haohaochexian.top

JS:   (() => { console.log("run"); })();
来源：http://dbm.cdnleiting.top

TS:   (() => { console.log("run"); })();
来源：http://bdq.yongpay.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://zlj.ivvv.top

Go:   func() { fmt.Println("run") }()
来源：http://keq.gaohongyu789.top

Ruby: -> { puts "run" }.call
来源：http://nlt.uphjek.com

C#:   // 无 IIFE：用静态构造函数
来源：http://ukd.xingfuxueyuan.xyz

[C13] 类型声明 / 类型注解
来源：http://yyr.aibaodan.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://emy.jiagoushi.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tuv.yj20258888.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://vuq.quarkkingdee.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://duw.yueranfly.top

Java: int add(int a, int b) { return a + b; }
来源：http://wim.fanxiaobao.xyz

Go:   func add(a, b int) int
来源：http://vll.gzhubu.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://kzy.aizwys.cn

C#:   int Add(int a, int b) => a + b;
来源：http://xlf.shanyushiyangkeji.top

[C14] 泛型函数
来源：http://ipn.redwolf501.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://shq.fktsv.cn

PHP:  // 无泛型
来源：http://bio.zdbjq.cn

JS:   // 无泛型
来源：http://btw.zhoulong.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ayu.shuidangran.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://edb.bbcook.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://bcr.haohaochexian.top

Ruby: # 无泛型
来源：http://euq.yanxiufei.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://vwq.shangyingyoupin.top

[C15] 解构 / 展开参数
来源：http://qmp.bbcook.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://fjv.jinqigufen.top

PHP:  [$a, $b] = $pair;
来源：http://mgf.c1oappe.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://pss.fanxiaobao.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://kys.haohaochexian.top

Java: // 无解构
来源：http://few.52xcode.cn

Go:   // 无解构
来源：http://zxl.fzhhl.top

Ruby: a, b = pair
来源：http://wti.0kj1m.cn

C#:   var (a, b) = pair;
来源：http://dpy.snrcjt.cn

[C16] 函数 / 方法重载
来源：http://fyq.xinyue.icu

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ike.nanxinkj.top

PHP:  // 无重载
来源：http://sje.guannengcc.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://zrj.gotoacloud.top

TS:   // 用联合类型或重载签名声明
来源：http://uvp.yonumen.top

Java: void f(int a) {}  void f(String a) {}
来源：http://zdp.hnqzz.top

Go:   // 无重载：用不同函数名
来源：http://itl.sufxvd.cn

Ruby: # 无重载：靠动态参数
来源：http://eed.mhx1999.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://tqw.hongshengwenyu.top

================================================================================
来源：http://hfz.tian-w.cn

D. 数组 / 列表 / 集合
来源：http://set.cashguo.top

================================================================================
来源：http://wqc.jlsjyb.cn

[D01] 创建数组 / 列表
来源：http://jlz.cheryme.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://gvm.ywan-chungtsiang.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://xxz.haohaochexian.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://idy.52xcode.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://xhs.ivvv.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://gea.mhx1999.top

Go:   arr := []int{1, 2, 3}
来源：http://hor.yanxiufei.cn

Ruby: arr = [1, 2, 3]
来源：http://cxy.tian-w.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://sfb.chenzaomai.com

[D02] 追加元素到末尾
来源：http://zlh.birdmap.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mcc.xziqi.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://lpg.shuidangran.top

JS:   arr.push(4);
来源：http://muj.redwolf501.top

TS:   arr.push(4);
来源：http://aww.sysykeji.top

Java: list.add(4);
来源：http://wpi.jinqigufen.top

Go:   arr = append(arr, 4)
来源：http://fhz.tianlin.xyz

Ruby: arr << 4; arr.push(5)
来源：http://muy.yj20258888.top

C#:   list.Add(4);
来源：http://lqi.epnwcf.com

[D03] 在指定位置插入元素
来源：http://gyv.wangdashe.top

Py:   arr.insert(0, 0)
来源：http://msx.dianchejie.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://xey.ydzc1.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wmp.cdnleiting.top

TS:   arr.splice(0, 0, 0);
来源：http://gbq.c1oappe.top

Java: list.add(0, 0);
来源：http://iap.bbcook.cn

Go:   arr = append([]int{0}, arr...)
来源：http://zfu.vehdjk.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://qkz.yuanzhike.top

C#:   list.Insert(0, 0);
来源：http://zqo.tanke756.top

[D04] 删除元素
来源：http://oqe.daxiang520.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://xnj.shanyushiyangkeji.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://vdw.sjlbkw.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mmb.pycfn.com

TS:   arr.splice(0, 1);
来源：http://flj.c1oappe.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://rep.yj20258.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://nlw.bjfxy.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mqe.cqqwz.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://byl.xingfuxueyuan.xyz

[D05] 访问与修改元素
来源：http://tmh.yonumen.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wbu.yvedp.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mjw.yj20258888.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://fph.yj20258.top

TS:   arr[0]; arr.at(-1);
来源：http://aew.hysaishi.cn

Java: list.get(0); list.set(0, 9);
来源：http://ngp.yuxming.cn

Go:   arr[0]; arr[0] = 9
来源：http://yjq.hnxiangtu.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://xxl.sjlbkw.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://nvb.jqgfzy.top

[D06] 数组长度
来源：http://nmh.vehdjk.com

Py:   len(arr)
来源：http://lit.0kj1m.cn

PHP:  count($arr);
来源：http://ulf.zdqjudy.top

JS:   arr.length
来源：http://cqg.zhijiandao.cn

TS:   arr.length
来源：http://yxj.shanyushiyangkeji.top

Java: list.size();
来源：http://utk.fktsv.cn

Go:   len(arr)
来源：http://clf.jinqigufen.top

Ruby: arr.length; arr.size
来源：http://qge.sysykeji.top

C#:   list.Count;
来源：http://ayo.hesvh.cn

[D07] 切片 / 取子数组
来源：http://ojz.0kj1m.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://dtm.sweek.top

PHP:  array_slice($arr, 1, 3);
来源：http://fsn.52xcode.cn

JS:   arr.slice(1, 4);
来源：http://njp.sysykeji.top

TS:   arr.slice(1, 4);
来源：http://iut.smart0.xyz

Java: list.subList(1, 4);
来源：http://kvl.chenjidiqi.icu

Go:   arr[1:4]
来源：http://uwf.havefunace.top

Ruby: arr[1, 3]
来源：http://kes.9152youxi.cn

C#:   list.GetRange(1, 3);
来源：http://dqb.jinghuilouyu.cn

[D08] 合并两个数组
来源：http://nks.ppjwa.cn

Py:   a + b;  a.extend(b)
来源：http://gwg.shuidangran.top

PHP:  array_merge($a, $b);
来源：http://hyx.jinqigufen.top

JS:   [...a, ...b];  a.concat(b);
来源：http://kiz.jinqigfzy.top

TS:   [...a, ...b];
来源：http://xer.jiagoushi.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hus.jianghu66.top

Go:   append(a, b...)
来源：http://kqw.c1oappe.top

Ruby: a + b;  a.concat(b)
来源：http://cdp.fzhhl.top

C#:   a.Concat(b).ToList()
来源：http://owj.yanxiufei.cn

[D09] 排序（升序）
来源：http://nwh.jiagoushi.top

Py:   sorted(arr);  arr.sort()
来源：http://prj.dianchejie.cn

PHP:  sort($arr);
来源：http://lxh.shanyushiyangkeji.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://puw.hongshengwenyu.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://ngw.cashguo.top

Java: Collections.sort(list);  list.sort(null);
来源：http://gbo.haohaochexian.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://oeg.redwolf501.top

Ruby: arr.sort
来源：http://oyu.ppjwa.cn

C#:   list.Sort();
来源：http://txu.daxiang520.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://pnd.bjfxy.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://lmn.hfpthk.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dej.ywan-chungtsiang.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://seb.xuetiantiany.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://lat.zhiwuduotai.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://iry.sxryk.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://vue.316326.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hja.vqdsnc.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qmi.wangshuangyany.cn

[D11] 反转数组
来源：http://dyn.zhengqikj.top

Py:   arr[::-1];  arr.reverse()
来源：http://wpi.sxryk.cn

PHP:  array_reverse($arr);
来源：http://bij.yj20258888.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://meb.havefunace.top

TS:   [...arr].reverse();
来源：http://qhl.yj20258.top

Java: Collections.reverse(list);
来源：http://vvz.zhoulong.xyz

Go:   slices.Reverse(arr)
来源：http://ddz.yfazqb.com

Ruby: arr.reverse
来源：http://hlm.hnqzz.top

C#:   list.Reverse();
来源：http://tww.ybcxt.top

[D12] 查找元素下标
来源：http://sbj.nanxuanxn.top

Py:   arr.index(x);  x in arr
来源：http://nph.jqgufenzy.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ujx.daria6918.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rpf.gzhubu.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dhc.yonumen.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://fsx.xylfe.cn

Go:   slices.Index(arr, x)
来源：http://qki.cashguo.top

Ruby: arr.index(x)
来源：http://ivu.sysykeji.top

C#:   list.IndexOf(x);
来源：http://xpl.yanxiufei.cn

[D13] 过滤（保留满足条件的）
来源：http://bzb.zhoulong.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://irf.jianghu66.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ewo.0kj1m.cn

JS:   arr.filter(x => x > 3)
来源：http://wli.hcnkem.com

TS:   arr.filter(x => x > 3)
来源：http://iwe.tanke756.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://fyw.yj20258.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ddj.cqqwz.cn

Ruby: arr.select { |x| x > 3 }
来源：http://vev.zhijiandao.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://rza.chenlongwang.top

[D14] 映射转换（每个元素变形）
来源：http://dfl.sjlbkw.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://gdg.jianghu66.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://kzn.daxiang520.top

JS:   arr.map(x => x * 2)
来源：http://ocb.sweek.top

TS:   arr.map(x => x * 2)
来源：http://pze.shzxlz.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://zfu.vqdsnc.cn

Go:   // 手写循环
来源：http://gyo.epnwcf.com

Ruby: arr.map { |x| x * 2 }
来源：http://xwi.guannengcc.top

C#:   list.Select(x => x * 2).ToList()
来源：http://bjw.guowangkeji.top

[D15] 去重
来源：http://ozm.fengsongda.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://jvt.zhiwuduotai.top

PHP:  array_unique($arr);
来源：http://yfq.hcnkem.com

JS:   [...new Set(arr)]
来源：http://zke.jqgfzy.top

TS:   [...new Set(arr)]
来源：http://wnv.yj202588.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://dex.hfpthk.cn

Go:   // 用 map[T]struct{} 手写
来源：http://wgt.tarul.cn

Ruby: arr.uniq
来源：http://sxa.ydjk.org.cn

C#:   list.Distinct().ToList()
来源：http://jyn.52xcode.cn

[D16] 求和与平均值
来源：http://rfu.hongshengwenyu.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://zta.52xcode.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://aid.yonumen.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://tyz.jinyuanbaomall.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://fan.zhijiandao.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ixo.jinghuilouyu.cn

Go:   // 手写循环累加
来源：http://rmr.yanxiufei.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://lzc.ehwqpu.com

C#:   list.Sum();  list.Average()
来源：http://upq.aibaodan.cn

[D17] 最大值与最小值
来源：http://yqg.hongshengwenyu.top

Py:   max(arr);  min(arr)
来源：http://bgk.fanxiaobao.xyz

PHP:  max($arr);  min($arr);
来源：http://nyk.sweek.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://pzi.jinqigfzy.top

TS:   Math.max(...arr);
来源：http://tot.ppjwa.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://mwq.bjfxy.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ask.shzxlz.cn

Ruby: arr.max;  arr.min
来源：http://fiy.gaohongyu789.top

C#:   list.Max();  list.Min()
来源：http://rfi.pengpengdd.cyou

[D18] 扁平化嵌套数组
来源：http://qhe.xuetiantiany.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ddy.yj20258.top

PHP:  array_merge(...$nested);
来源：http://xwp.cdnleiting.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ecm.nanxinkj.top

TS:   nested.flat();
来源：http://pbx.xuanzx.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://lbt.pycfn.com

Go:   // 手写双层循环
来源：http://yor.feifeiyinyue.top

Ruby: nested.flatten
来源：http://juv.aibaodan.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://mwz.feifeiyinyue.top

[D19] 按字段分组
来源：http://mas.xingfuxueyuan.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://owg.sxryk.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qsi.daxiang520.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://iam.xylfe.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://hxz.aizwys.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://pdj.zycfv.cn

Go:   // 手写 map[string][]T
来源：http://zvx.shzxlz.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://vpn.redwolf501.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://pwr.sufxvd.cn

[D20] 统计每个元素出现次数
来源：http://utl.jinqigufen.top

Py:   Counter(arr)
来源：http://qca.9152youxi.cn

PHP:  array_count_values($arr);
来源：http://bzl.hnqzz.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wph.hnxiangtu.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://npg.gotoacloud.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://yxa.yj20258.top

Go:   // 手写 map[T]int
来源：http://ohh.jianghu66.top

Ruby: arr.tally
来源：http://ivx.iojbl.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://zmz.nwbrower.top

[D21] 判断是否包含某元素
来源：http://wft.daxiang520.top

Py:   x in arr
来源：http://hqq.hammf.cn

PHP:  in_array($x, $arr, true);
来源：http://wgo.tian-w.cn

JS:   arr.includes(x)
来源：http://kmg.mhx1999.top

TS:   arr.includes(x)
来源：http://hwb.zycfv.cn

Java: list.contains(x)
来源：http://foj.xinyue.icu

Go:   slices.Contains(arr, x)
来源：http://xqn.jinqigufen.top

Ruby: arr.include?(x)
来源：http://cnk.cheryme.top

C#:   list.Contains(x)
来源：http://xzt.shanyushiyangkeji.top

[D22] 复制数组（避免共享引用）
来源：http://chf.hnxiangtu.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ced.jinqigfzy.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://atr.yfazqb.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://lmi.smart0.xyz

TS:   [...arr];
来源：http://ypt.jianghu66.top

Java: new ArrayList<>(list);
来源：http://ntk.feifeiyinyue.top

Go:   copied := append([]int(nil), arr...)
来源：http://hgm.aizwys.cn

Ruby: arr.dup;  arr.clone
来源：http://tkv.yueranfly.top

C#:   new List<int>(list);
来源：http://ubf.sweek.top

[D23] reduce 累积计算
来源：http://dud.wangdashe.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hkl.xinyue.icu

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://yqx.svipenyu.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lwb.zdbjq.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bdn.feifeiyinyue.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://wck.9152youxi.cn

Go:   // 手写循环
来源：http://wnw.iojbl.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://jhr.wangdashe.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://zkp.hongshengwenyu.top

[D24] 字典 / Map 基本操作
来源：http://rac.epnwcf.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://kbz.fehbvm.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://zcx.9152youxi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://kdr.jinghuilouyu.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://owl.bjfxy.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ead.feifeiyinyue.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://rwz.cdnleiting.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://vvy.sysykeji.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://pru.ydzc1.top

[D25] Set 集合去重与交并差
来源：http://yis.pengpengdd.cyou

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wnk.snrcjt.cn


<!-- 参考信息 -->