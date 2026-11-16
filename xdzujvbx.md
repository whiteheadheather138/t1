代发 wailian999

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://uzo.yongpay.top

TS:   arr.map(String)
来源：http://mtf.jinqigufen.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://jjw.ctjpmb.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://npc.xuanzx.com

Ruby: arr.map(&:upcase)
来源：http://lue.xylfe.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://yhl.meibo888.top

[C08] 闭包
来源：http://elj.gotoacloud.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://egr.hysaishi.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ytb.xinyue.icu

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://kux.pengpengdd.cyou

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wuh.fengsongda.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://qty.yueranfly.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jcq.ywan-chungtsiang.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://oqz.ydzc1.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hxg.ivvv.top

[C09] 递归
来源：http://mhc.vehdjk.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ydt.aizwys.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://jzn.zhiwuduotai.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hti.fktsv.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zbp.vqdsnc.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://fpq.fktsv.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://xdx.birdmap.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://gip.jinyuanbaomall.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://kyy.shangyingyoupin.top

[C10] 变量作用域
来源：http://uqm.xinyue.icu

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://gyt.bbcook.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hlr.yfazqb.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://jgo.kuanghao11.cn

TS:   同 JS
来源：http://iaa.andypj.xyz

Java: 方法内为块级作用域
来源：http://stc.cdnleiting.top

Go:   花括号块级作用域
来源：http://eow.ehwqpu.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://yoc.zhixingplan.top

C#:   块级作用域
来源：http://jtj.pengpengdd.cyou

[C11] 模块导入与导出
来源：http://rpp.yuanzhike.top

Py:   from module import func
来源：http://isr.havefunace.top

PHP:  require "file.php";  或 use App\Service;
来源：http://jwe.0kj1m.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://zwy.cdnleiting.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://nna.yangfankeji.com

Java: import java.util.List;
来源：http://btd.uphjek.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ljy.pycfn.com

Ruby: require "json"; require_relative "./util"
来源：http://vuo.daxiang520.top

C#:   using System.Text;
来源：http://mlc.gaohongyu789.top

[C12] 立即执行函数 IIFE
来源：http://iuk.wangdashe.top

Py:   (lambda: print("run"))()
来源：http://did.jqgfzy.top

PHP:  (function () { echo "run"; })();
来源：http://rvc.snrcjt.cn

JS:   (() => { console.log("run"); })();
来源：http://jsz.daria6918.cn

TS:   (() => { console.log("run"); })();
来源：http://bfb.ctjpmb.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://rih.gotoacloud.top

Go:   func() { fmt.Println("run") }()
来源：http://sxv.gzhubu.top

Ruby: -> { puts "run" }.call
来源：http://jlo.tian-w.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://kcv.hnxiangtu.top

[C13] 类型声明 / 类型注解
来源：http://ipm.birdmap.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://suc.shzxlz.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bhh.hammf.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://crl.jqgufenzy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ukr.nwbrower.top

Java: int add(int a, int b) { return a + b; }
来源：http://pul.meibo888.top

Go:   func add(a, b int) int
来源：http://uii.zhongyouzk.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://dnz.yuxming.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ksl.52xcode.cn

[C14] 泛型函数
来源：http://khi.sweek.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wux.gzhubu.top

PHP:  // 无泛型
来源：http://sjb.cheryme.top

JS:   // 无泛型
来源：http://mrh.daria6918.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://lez.zhengqikj.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://pxe.birdmap.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://yto.zdbjq.cn

Ruby: # 无泛型
来源：http://lem.bbcook.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://aof.zhengqikj.top

[C15] 解构 / 展开参数
来源：http://kfb.chenzaomai.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hss.gotoacloud.top

PHP:  [$a, $b] = $pair;
来源：http://ddj.kuanghao11.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ppg.tanke756.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ltb.jqgfzy.top

Java: // 无解构
来源：http://ruw.jqgufenzy.top

Go:   // 无解构
来源：http://phm.tarul.cn

Ruby: a, b = pair
来源：http://cbo.ywan-chungtsiang.top

C#:   var (a, b) = pair;
来源：http://fbs.jinqigfzy.top

[C16] 函数 / 方法重载
来源：http://pkz.yvedp.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://gjr.shuidangran.top

PHP:  // 无重载
来源：http://pyw.quarkkingdee.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://myg.ehwqpu.com

TS:   // 用联合类型或重载签名声明
来源：http://pfk.ppjwa.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://nui.xylfe.cn

Go:   // 无重载：用不同函数名
来源：http://xtj.tianlin.xyz

Ruby: # 无重载：靠动态参数
来源：http://ydr.0kj1m.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://wkw.nwbrower.top

================================================================================
来源：http://vnu.52xcode.cn

D. 数组 / 列表 / 集合
来源：http://luk.yj202588.top

================================================================================
来源：http://ckv.pycfn.com

[D01] 创建数组 / 列表
来源：http://mtk.hammf.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://znt.0kj1m.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hcn.svipenyu.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://vjf.ehwqpu.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://hfn.cheryme.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ktf.hnxiangtu.top

Go:   arr := []int{1, 2, 3}
来源：http://fop.c1oappe.top

Ruby: arr = [1, 2, 3]
来源：http://viv.zhixingplan.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://zga.jianghu66.top

[D02] 追加元素到末尾
来源：http://tgn.wangdashe.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://qgl.cheryme.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://faw.cheryme.top

JS:   arr.push(4);
来源：http://gxr.sxryk.cn

TS:   arr.push(4);
来源：http://sjr.yj202588.top

Java: list.add(4);
来源：http://ici.chenjidiqi.icu

Go:   arr = append(arr, 4)
来源：http://qko.gotoacloud.top

Ruby: arr << 4; arr.push(5)
来源：http://ool.zhoulong.xyz

C#:   list.Add(4);
来源：http://gtb.ctjpmb.com

[D03] 在指定位置插入元素
来源：http://thl.yvedp.cn

Py:   arr.insert(0, 0)
来源：http://hlo.haohaochexian.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://lxe.52xcode.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://xfi.hnqzz.top

TS:   arr.splice(0, 0, 0);
来源：http://mvt.dianchejie.cn

Java: list.add(0, 0);
来源：http://iwg.zhoulong.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://gaq.hongshengwenyu.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hal.jianghu66.top

C#:   list.Insert(0, 0);
来源：http://cjj.wangdashe.top

[D04] 删除元素
来源：http://eul.vehdjk.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://lxn.dianchejie.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://dob.hammf.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://orn.cucudq.cn

TS:   arr.splice(0, 1);
来源：http://wrq.yangfankeji.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ben.fengsongda.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://pir.feifeiyinyue.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://vui.guannengcc.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://lrh.cqqwz.cn

[D05] 访问与修改元素
来源：http://opy.hnxiangtu.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://dhb.jinqigfzy.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://anu.shanyushiyangkeji.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://yxz.tarul.cn

TS:   arr[0]; arr.at(-1);
来源：http://ukl.zhoulong.xyz

Java: list.get(0); list.set(0, 9);
来源：http://zwc.dianchejie.cn

Go:   arr[0]; arr[0] = 9
来源：http://lhn.kuanghao11.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ayh.gotoacloud.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hfs.yvedp.cn

[D06] 数组长度
来源：http://cxm.fzhhl.top

Py:   len(arr)
来源：http://xaj.zdbjq.cn

PHP:  count($arr);
来源：http://cmg.vqdsnc.cn

JS:   arr.length
来源：http://goa.shuidangran.top

TS:   arr.length
来源：http://xod.xinyue.icu

Java: list.size();
来源：http://nsc.guowangkeji.top

Go:   len(arr)
来源：http://oko.yangfankeji.com

Ruby: arr.length; arr.size
来源：http://rmu.uphjek.com

C#:   list.Count;
来源：http://isn.fktsv.cn

[D07] 切片 / 取子数组
来源：http://jsq.sxryk.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://eth.yj20258.top

PHP:  array_slice($arr, 1, 3);
来源：http://gts.tarul.cn

JS:   arr.slice(1, 4);
来源：http://bka.ydzc1.top

TS:   arr.slice(1, 4);
来源：http://uan.wangshuangyany.cn

Java: list.subList(1, 4);
来源：http://cbr.vqdsnc.cn

Go:   arr[1:4]
来源：http://nhk.birdmap.top

Ruby: arr[1, 3]
来源：http://bhk.xingfuxueyuan.xyz

C#:   list.GetRange(1, 3);
来源：http://iuy.shzxlz.cn

[D08] 合并两个数组
来源：http://xzc.sysykeji.top

Py:   a + b;  a.extend(b)
来源：http://qex.epnwcf.com

PHP:  array_merge($a, $b);
来源：http://opl.smart0.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://fhq.pycfn.com

TS:   [...a, ...b];
来源：http://bst.zhaomingkeji.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wln.chenlongwang.top

Go:   append(a, b...)
来源：http://klr.cucudq.cn

Ruby: a + b;  a.concat(b)
来源：http://iso.tian-w.cn

C#:   a.Concat(b).ToList()
来源：http://oly.hammf.cn

[D09] 排序（升序）
来源：http://lun.ydzc1.top

Py:   sorted(arr);  arr.sort()
来源：http://lit.wangdashe.top

PHP:  sort($arr);
来源：http://dxp.yvedp.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://pbr.ybcxt.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://kws.fzhhl.top

Java: Collections.sort(list);  list.sort(null);
来源：http://dyi.meibo888.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://plk.zdbjq.cn

Ruby: arr.sort
来源：http://cxl.sufxvd.cn

C#:   list.Sort();
来源：http://cnz.jianghu66.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://ubm.yj202588.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://rir.shzxlz.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wue.cqqwz.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hlx.yonumen.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://nsa.cucudq.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://yaa.hammf.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://vis.yuxming.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mfr.zhoulong.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mea.epnwcf.com

[D11] 反转数组
来源：http://cue.zhijiandao.cn

Py:   arr[::-1];  arr.reverse()
来源：http://qnu.zhengqikj.top

PHP:  array_reverse($arr);
来源：http://btg.dianchejie.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://azk.daria6918.cn

TS:   [...arr].reverse();
来源：http://eot.wangshuangyany.cn

Java: Collections.reverse(list);
来源：http://yys.gotoacloud.top

Go:   slices.Reverse(arr)
来源：http://jrb.aibaodan.cn

Ruby: arr.reverse
来源：http://qid.ywan-chungtsiang.top

C#:   list.Reverse();
来源：http://xnp.tarul.cn

[D12] 查找元素下标
来源：http://yfi.jqgfzy.top

Py:   arr.index(x);  x in arr
来源：http://rby.sysykeji.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://fla.guowangkeji.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pxo.xuanzx.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://eio.yfazqb.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://bwb.mhx1999.top

Go:   slices.Index(arr, x)
来源：http://bpz.bbcook.cn

Ruby: arr.index(x)
来源：http://vmb.cucudq.cn

C#:   list.IndexOf(x);
来源：http://syo.zycfv.cn

[D13] 过滤（保留满足条件的）
来源：http://lfj.zhengqikj.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://seb.daria6918.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://atc.iojbl.cn

JS:   arr.filter(x => x > 3)
来源：http://ghv.daxiang520.top

TS:   arr.filter(x => x > 3)
来源：http://mle.yj20258888.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://idy.jqgufenzy.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://kfu.xinyue.icu

Ruby: arr.select { |x| x > 3 }
来源：http://mvj.svipenyu.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://pww.hesvh.cn

[D14] 映射转换（每个元素变形）
来源：http://clv.guowangkeji.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ydz.fktsv.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mok.ctjpmb.com

JS:   arr.map(x => x * 2)
来源：http://dkk.uphjek.com

TS:   arr.map(x => x * 2)
来源：http://yks.hywenlv.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ynm.jinyuanbaomall.cn

Go:   // 手写循环
来源：http://ioa.yfazqb.com

Ruby: arr.map { |x| x * 2 }
来源：http://gnq.pycfn.com

C#:   list.Select(x => x * 2).ToList()
来源：http://gvt.shangyingyoupin.top

[D15] 去重
来源：http://lsj.aizwys.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://auo.chenlongwang.top

PHP:  array_unique($arr);
来源：http://dim.jinyuanbaomall.cn

JS:   [...new Set(arr)]
来源：http://rzc.ppjwa.cn

TS:   [...new Set(arr)]
来源：http://wwu.jiagoushi.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ijv.9152youxi.cn

Go:   // 用 map[T]struct{} 手写
来源：http://utq.ybcxt.top

Ruby: arr.uniq
来源：http://btm.kuanghao11.cn

C#:   list.Distinct().ToList()
来源：http://agl.jinyuanbaomall.cn

[D16] 求和与平均值
来源：http://nwx.cucudq.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qpo.cdnleiting.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://sxu.jyoumei.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ppo.yuanzhike.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ywd.wangdashe.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://amk.9152youxi.cn

Go:   // 手写循环累加
来源：http://exc.hesvh.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://cwb.xuanzx.com

C#:   list.Sum();  list.Average()
来源：http://xqi.gotoacloud.top

[D17] 最大值与最小值
来源：http://qlq.316326.xyz

Py:   max(arr);  min(arr)
来源：http://hwx.yj20258.top

PHP:  max($arr);  min($arr);
来源：http://iko.52xcode.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://guu.ctjpmb.com

TS:   Math.max(...arr);
来源：http://hwq.ehwqpu.com

Java: Collections.max(list);  Collections.min(list);
来源：http://gyv.shanyushiyangtech.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://dfg.fktsv.cn

Ruby: arr.max;  arr.min
来源：http://zat.zhijiandao.cn

C#:   list.Max();  list.Min()
来源：http://nvv.316326.xyz

[D18] 扁平化嵌套数组
来源：http://bks.yangfankeji.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://sgp.dashuyun.cn

PHP:  array_merge(...$nested);
来源：http://ede.zdqjudy.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://pxi.shanyushiyangtech.top

TS:   nested.flat();
来源：http://dcv.guowangkeji.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://dzl.c1oappe.top

Go:   // 手写双层循环
来源：http://dxv.snrcjt.cn

Ruby: nested.flatten
来源：http://cic.guannengcc.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://tpf.nanxinkj.top

[D19] 按字段分组
来源：http://sik.hesvh.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://zjl.xinyue.icu

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ptp.yangfankeji.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://tzy.c1oappe.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://qhr.aizwys.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://lpu.vqdsnc.cn

Go:   // 手写 map[string][]T
来源：http://soe.zhongyouzk.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://umw.smart0.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://bsh.hesvh.cn

[D20] 统计每个元素出现次数
来源：http://fig.shzxlz.cn

Py:   Counter(arr)
来源：http://mbd.sweek.top

PHP:  array_count_values($arr);
来源：http://xrw.yangfankeji.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ffg.haohaochexian.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pwk.haohaochexian.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://vuq.52xcode.cn

Go:   // 手写 map[T]int
来源：http://jvh.jqgufenzy.top

Ruby: arr.tally
来源：http://vje.jinghuilouyu.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://djs.quarkkingdee.top

[D21] 判断是否包含某元素
来源：http://cca.fehbvm.com

Py:   x in arr
来源：http://gvr.0kj1m.cn

PHP:  in_array($x, $arr, true);
来源：http://vno.xinyue.icu

JS:   arr.includes(x)
来源：http://nsf.yfazqb.com

TS:   arr.includes(x)
来源：http://mno.zdbjq.cn

Java: list.contains(x)
来源：http://ivz.shangyingyoupin.top

Go:   slices.Contains(arr, x)
来源：http://nya.shzxlz.cn

Ruby: arr.include?(x)
来源：http://frg.c1oappe.top

C#:   list.Contains(x)
来源：http://qok.fehbvm.com

[D22] 复制数组（避免共享引用）
来源：http://knn.c1oappe.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://nzh.gaohongyu789.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ioh.dianchejie.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ruo.shanyushiyangtech.top

TS:   [...arr];
来源：http://wdo.shangyingyoupin.top

Java: new ArrayList<>(list);
来源：http://agz.tanke756.top

Go:   copied := append([]int(nil), arr...)
来源：http://had.zdbjq.cn

Ruby: arr.dup;  arr.clone
来源：http://lyl.yanxiufei.cn

C#:   new List<int>(list);
来源：http://qqe.nanxinkj.top

[D23] reduce 累积计算
来源：http://ymz.gogol.net.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zub.zhaomingkeji.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://nip.zhongyouzk.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bba.ybcxt.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bst.wangshuangyany.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://tki.shanyushiyangkeji.top

Go:   // 手写循环
来源：http://mhp.hnqzz.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://fsa.jinyuanbaomall.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hee.sjlbkw.cn

[D24] 字典 / Map 基本操作
来源：http://fos.wangdashe.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://imc.zhijiandao.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://zos.jinyuanbaomall.cn


<!-- 参考信息 -->