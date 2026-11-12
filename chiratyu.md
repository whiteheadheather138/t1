代发 wailian999

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mdt.yuanzhike.top

TS:   arr.map(String)
来源：http://xni.fengsongda.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ldj.zhijiandao.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://nre.zhaomingkeji.xyz

Ruby: arr.map(&:upcase)
来源：http://qba.ehwqpu.com

C#:   arr.Select(s => s.ToUpper())
来源：http://siv.cheryme.top

[C08] 闭包
来源：http://bpc.sjlbkw.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://xwv.snrcjt.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ohz.tarul.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://rie.dianchejie.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://rup.chenzaomai.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://tfk.zhaomingkeji.xyz

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://aqt.yj20258888.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://vow.xinyue.icu

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://fkv.yangfankeji.com

[C09] 递归
来源：http://yun.gzhubu.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://pju.aibaodan.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://cbz.yonumen.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pxa.fktsv.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dcj.0kj1m.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://zxg.hongshengwenyu.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://lbg.tianlin.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://usp.fehbvm.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://pdo.zdqjudy.top

[C10] 变量作用域
来源：http://lvm.jyoumei.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://cdr.xingfuxueyuan.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://nkf.yvedp.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://dek.316326.xyz

TS:   同 JS
来源：http://iit.meibo888.top

Java: 方法内为块级作用域
来源：http://gow.shzxlz.cn

Go:   花括号块级作用域
来源：http://ukd.nanxuanxn.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://eoo.hfpthk.cn

C#:   块级作用域
来源：http://xnm.tian-w.cn

[C11] 模块导入与导出
来源：http://uss.guannengcc.top

Py:   from module import func
来源：http://avw.yj20258888.top

PHP:  require "file.php";  或 use App\Service;
来源：http://kin.yuxming.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ybp.yuxming.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://lxt.jianghu66.top

Java: import java.util.List;
来源：http://sav.daria6918.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://lka.ydjk.org.cn

Ruby: require "json"; require_relative "./util"
来源：http://wkf.zhengqikj.top

C#:   using System.Text;
来源：http://wgr.fktsv.cn

[C12] 立即执行函数 IIFE
来源：http://epl.jinqigfzy.top

Py:   (lambda: print("run"))()
来源：http://xwm.tarul.cn

PHP:  (function () { echo "run"; })();
来源：http://opk.pycfn.com

JS:   (() => { console.log("run"); })();
来源：http://jzf.jyoumei.cn

TS:   (() => { console.log("run"); })();
来源：http://kgx.ywan-chungtsiang.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://giu.haohaochexian.top

Go:   func() { fmt.Println("run") }()
来源：http://aor.yuxming.cn

Ruby: -> { puts "run" }.call
来源：http://bzb.daria6918.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://rat.haohaochexian.top

[C13] 类型声明 / 类型注解
来源：http://kum.hnqzz.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://rep.vqdsnc.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://imn.ydjk.org.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://cyj.sxryk.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lwi.fktsv.cn

Java: int add(int a, int b) { return a + b; }
来源：http://shc.shzxlz.cn

Go:   func add(a, b int) int
来源：http://bjv.daxiang520.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://xwe.nanxuanxn.top

C#:   int Add(int a, int b) => a + b;
来源：http://bqr.yonumen.top

[C14] 泛型函数
来源：http://yce.c1oappe.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ivj.ctjpmb.com

PHP:  // 无泛型
来源：http://fmp.tanke756.top

JS:   // 无泛型
来源：http://eze.yvedp.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://gzd.zhoulong.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://eaf.ppjwa.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://yki.yj202588.top

Ruby: # 无泛型
来源：http://hja.hnqzz.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mru.hongshengwenyu.top

[C15] 解构 / 展开参数
来源：http://zol.tanke756.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hxh.yj20258.top

PHP:  [$a, $b] = $pair;
来源：http://cko.pycfn.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://fjh.316326.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://eyv.zhaomingkeji.xyz

Java: // 无解构
来源：http://lcg.chenjidiqi.icu

Go:   // 无解构
来源：http://cav.mhx1999.top

Ruby: a, b = pair
来源：http://zrp.birdmap.top

C#:   var (a, b) = pair;
来源：http://bsy.xingfuxueyuan.xyz

[C16] 函数 / 方法重载
来源：http://jwv.yuxming.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://cul.pycfn.com

PHP:  // 无重载
来源：http://zmg.havefunace.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://quk.snrcjt.cn

TS:   // 用联合类型或重载签名声明
来源：http://ohj.iojbl.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://wmz.9152youxi.cn

Go:   // 无重载：用不同函数名
来源：http://wes.cdnleiting.top

Ruby: # 无重载：靠动态参数
来源：http://ckf.sweek.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://mxe.bbcook.cn

================================================================================
来源：http://ymw.zhongyouzk.top

D. 数组 / 列表 / 集合
来源：http://qxd.kuanghao11.cn

================================================================================
来源：http://xxm.redwolf501.top

[D01] 创建数组 / 列表
来源：http://iwz.hesvh.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://afz.yvedp.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://lnt.52xcode.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wjh.xingfuxueyuan.xyz

TS:   const arr: number[] = [1, 2, 3];
来源：http://bui.pengpengdd.cyou

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://yiq.cheryme.top

Go:   arr := []int{1, 2, 3}
来源：http://ncc.cucudq.cn

Ruby: arr = [1, 2, 3]
来源：http://mit.hcnkem.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://uyv.ppjwa.cn

[D02] 追加元素到末尾
来源：http://dsd.hywenlv.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://imf.cqqwz.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://rgl.hongshengwenyu.top

JS:   arr.push(4);
来源：http://vyw.xuetiantiany.cn

TS:   arr.push(4);
来源：http://yie.vehdjk.com

Java: list.add(4);
来源：http://mbc.jinqigufen.top

Go:   arr = append(arr, 4)
来源：http://sck.xingfuxueyuan.xyz

Ruby: arr << 4; arr.push(5)
来源：http://rlh.wangshuangyany.cn

C#:   list.Add(4);
来源：http://wsb.zhaomingkeji.xyz

[D03] 在指定位置插入元素
来源：http://vnr.jqgufenzy.top

Py:   arr.insert(0, 0)
来源：http://lcx.zhongyouzk.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ovo.fktsv.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ynv.guannengcc.top

TS:   arr.splice(0, 0, 0);
来源：http://gxw.daxiang520.top

Java: list.add(0, 0);
来源：http://mxy.uphjek.com

Go:   arr = append([]int{0}, arr...)
来源：http://wpm.wangdashe.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://bqq.hnqzz.top

C#:   list.Insert(0, 0);
来源：http://jdd.ydzc1.top

[D04] 删除元素
来源：http://yqv.andypj.xyz

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://phl.tarul.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ols.vqdsnc.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://yxo.hfpthk.cn

TS:   arr.splice(0, 1);
来源：http://fdr.zdbjq.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://tho.wangshuangyany.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ebj.yongpay.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://tnu.9152youxi.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://edx.xylfe.cn

[D05] 访问与修改元素
来源：http://qqf.mhx1999.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://atu.xziqi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://urs.fanxiaobao.xyz

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://shy.tian-w.cn

TS:   arr[0]; arr.at(-1);
来源：http://bgo.tianlin.xyz

Java: list.get(0); list.set(0, 9);
来源：http://kvu.ppjwa.cn

Go:   arr[0]; arr[0] = 9
来源：http://nmo.yuanzhike.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://zco.birdmap.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://rvs.nanxuanxn.top

[D06] 数组长度
来源：http://yvl.hcnkem.com

Py:   len(arr)
来源：http://amq.chenlongwang.top

PHP:  count($arr);
来源：http://yhf.52xcode.cn

JS:   arr.length
来源：http://mwz.feifeiyinyue.top

TS:   arr.length
来源：http://yha.hywenlv.cn

Java: list.size();
来源：http://bhp.uphjek.com

Go:   len(arr)
来源：http://xmy.cdnleiting.top

Ruby: arr.length; arr.size
来源：http://utj.zhijiandao.cn

C#:   list.Count;
来源：http://cbc.chenlongwang.top

[D07] 切片 / 取子数组
来源：http://ljg.wangdashe.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://nln.jianghu66.top

PHP:  array_slice($arr, 1, 3);
来源：http://siv.shanyushiyangtech.top

JS:   arr.slice(1, 4);
来源：http://ymc.yj20258888.top

TS:   arr.slice(1, 4);
来源：http://apd.316326.xyz

Java: list.subList(1, 4);
来源：http://pgl.bbcook.cn

Go:   arr[1:4]
来源：http://omg.guannengcc.top

Ruby: arr[1, 3]
来源：http://skb.wangdashe.top

C#:   list.GetRange(1, 3);
来源：http://qaw.tian-w.cn

[D08] 合并两个数组
来源：http://uha.yongpay.top

Py:   a + b;  a.extend(b)
来源：http://btf.dianchejie.cn

PHP:  array_merge($a, $b);
来源：http://qgm.yj20258888.top

JS:   [...a, ...b];  a.concat(b);
来源：http://lma.kuanghao11.cn

TS:   [...a, ...b];
来源：http://bmn.ivvv.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ajs.yangfankeji.com

Go:   append(a, b...)
来源：http://cco.sjlbkw.cn

Ruby: a + b;  a.concat(b)
来源：http://svh.jyoumei.cn

C#:   a.Concat(b).ToList()
来源：http://rbs.fzhhl.top

[D09] 排序（升序）
来源：http://qgu.mhx1999.top

Py:   sorted(arr);  arr.sort()
来源：http://kjk.ppjwa.cn

PHP:  sort($arr);
来源：http://kcp.cqqwz.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ubc.ybcxt.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://utw.havefunace.top

Java: Collections.sort(list);  list.sort(null);
来源：http://pzf.yongpay.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://xxy.sweek.top

Ruby: arr.sort
来源：http://vvy.316326.xyz

C#:   list.Sort();
来源：http://cpl.zhixingplan.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://hzs.daxiang520.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://cob.tian-w.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pms.iojbl.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://iow.yvedp.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://gnr.cqqwz.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://vsn.gotoacloud.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://qjc.jinghuilouyu.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://shx.havefunace.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://zlh.jinqigfzy.top

[D11] 反转数组
来源：http://lmd.316326.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://ugh.yuxming.cn

PHP:  array_reverse($arr);
来源：http://rtr.sweek.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qvd.tanke756.top

TS:   [...arr].reverse();
来源：http://waq.tian-w.cn

Java: Collections.reverse(list);
来源：http://guw.chenjidiqi.icu

Go:   slices.Reverse(arr)
来源：http://sub.hesvh.cn

Ruby: arr.reverse
来源：http://xxh.yfazqb.com

C#:   list.Reverse();
来源：http://typ.sweek.top

[D12] 查找元素下标
来源：http://wan.havefunace.top

Py:   arr.index(x);  x in arr
来源：http://drg.dianchejie.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://lbn.havefunace.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ikz.aizwys.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lgi.c1oappe.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://tmu.yueranfly.top

Go:   slices.Index(arr, x)
来源：http://cbx.yongpay.top

Ruby: arr.index(x)
来源：http://qgy.xuetiantiany.cn

C#:   list.IndexOf(x);
来源：http://iqm.zdbjq.cn

[D13] 过滤（保留满足条件的）
来源：http://gnf.ppjwa.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://zmz.jinghuilouyu.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ebd.jqgfzy.top

JS:   arr.filter(x => x > 3)
来源：http://ffa.guannengcc.top

TS:   arr.filter(x => x > 3)
来源：http://dek.zhijiandao.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mpo.haohaochexian.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://bfa.jianghu66.top

Ruby: arr.select { |x| x > 3 }
来源：http://xae.pengpengdd.cyou

C#:   list.Where(x => x > 3).ToList()
来源：http://cis.nanxinkj.top

[D14] 映射转换（每个元素变形）
来源：http://rzc.feifeiyinyue.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://liq.dianchejie.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blj.hfpthk.cn

JS:   arr.map(x => x * 2)
来源：http://wft.zhaomingkeji.xyz

TS:   arr.map(x => x * 2)
来源：http://nmg.cdnleiting.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://kix.xinyue.icu

Go:   // 手写循环
来源：http://osp.smart0.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://ayb.ivvv.top

C#:   list.Select(x => x * 2).ToList()
来源：http://meq.fzhhl.top

[D15] 去重
来源：http://rlu.xylfe.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://tnh.ivvv.top

PHP:  array_unique($arr);
来源：http://ubp.redwolf501.top

JS:   [...new Set(arr)]
来源：http://kto.yj202588.top

TS:   [...new Set(arr)]
来源：http://bid.jinqigfzy.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://iqj.zhaomingkeji.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://zhv.dashuyun.cn

Ruby: arr.uniq
来源：http://vij.xinyue.icu

C#:   list.Distinct().ToList()
来源：http://zbp.nanxinkj.top

[D16] 求和与平均值
来源：http://bgn.zhongyouzk.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ydz.zhaomingkeji.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wxc.aizwys.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://sol.xuetiantiany.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mtz.dianchejie.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://luq.shanyushiyangtech.top

Go:   // 手写循环累加
来源：http://kzd.bbcook.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://xqp.ehwqpu.com

C#:   list.Sum();  list.Average()
来源：http://jfl.nwbrower.top

[D17] 最大值与最小值
来源：http://rkv.hysaishi.cn

Py:   max(arr);  min(arr)
来源：http://pcv.yj202588.top

PHP:  max($arr);  min($arr);
来源：http://rar.dashuyun.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hyx.xylfe.cn

TS:   Math.max(...arr);
来源：http://ula.cheryme.top

Java: Collections.max(list);  Collections.min(list);
来源：http://qtv.kuanghao11.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://uml.gaohongyu789.top

Ruby: arr.max;  arr.min
来源：http://dgs.xuanzx.com

C#:   list.Max();  list.Min()
来源：http://jbq.jinqigfzy.top

[D18] 扁平化嵌套数组
来源：http://ipo.birdmap.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://urk.feifeiyinyue.top

PHP:  array_merge(...$nested);
来源：http://vpt.zhiwuduotai.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://lyj.shanyushiyangtech.top

TS:   nested.flat();
来源：http://uuy.zhongyouzk.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mpx.hfpthk.cn

Go:   // 手写双层循环
来源：http://uul.mhx1999.top

Ruby: nested.flatten
来源：http://iur.zhoulong.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://yir.zhaomingkeji.xyz

[D19] 按字段分组
来源：http://mxb.jinyuanbaomall.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://pft.sjlbkw.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hnw.ydzc1.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://fjo.yj20258888.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://vgp.jinghuilouyu.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://dmi.yonumen.top

Go:   // 手写 map[string][]T
来源：http://dxn.chenjidiqi.icu

Ruby: arr.group_by { |x| x[:type] }
来源：http://jlr.hnqzz.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ytb.hongshengwenyu.top

[D20] 统计每个元素出现次数
来源：http://atc.tianlin.xyz

Py:   Counter(arr)
来源：http://hhu.52xcode.cn

PHP:  array_count_values($arr);
来源：http://tky.sxryk.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gpu.52xcode.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://inj.tanke756.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://feg.andypj.xyz

Go:   // 手写 map[T]int
来源：http://rqk.zdqjudy.top

Ruby: arr.tally
来源：http://eih.bbcook.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://glz.zdqjudy.top

[D21] 判断是否包含某元素
来源：http://bxf.yueranfly.top

Py:   x in arr
来源：http://hpn.hcnkem.com

PHP:  in_array($x, $arr, true);
来源：http://rhc.chenzaomai.com

JS:   arr.includes(x)
来源：http://bqg.svipenyu.cn

TS:   arr.includes(x)
来源：http://cex.andypj.xyz

Java: list.contains(x)
来源：http://vaz.yj202588.top

Go:   slices.Contains(arr, x)
来源：http://iel.xinyue.icu

Ruby: arr.include?(x)
来源：http://flb.sxryk.cn

C#:   list.Contains(x)
来源：http://clu.feifeiyinyue.top

[D22] 复制数组（避免共享引用）
来源：http://zqs.hesvh.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://pbn.ehwqpu.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mgi.quarkkingdee.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://duv.yuxming.cn

TS:   [...arr];
来源：http://abe.daxiang520.top

Java: new ArrayList<>(list);
来源：http://qeu.xziqi.cn

Go:   copied := append([]int(nil), arr...)
来源：http://trs.aibaodan.cn

Ruby: arr.dup;  arr.clone
来源：http://adq.mhx1999.top

C#:   new List<int>(list);
来源：http://rmf.jlsjyb.cn

[D23] reduce 累积计算
来源：http://qmf.wangshuangyany.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://rpl.pycfn.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://xtz.c1oappe.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mwt.pycfn.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yja.aizwys.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://njn.9152youxi.cn

Go:   // 手写循环
来源：http://kzp.yj202588.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://jjh.ybcxt.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://cwj.cqqwz.cn

[D24] 字典 / Map 基本操作
来源：http://qmb.uphjek.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://nwk.cucudq.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://jao.gzhubu.top


<!-- 参考信息 -->