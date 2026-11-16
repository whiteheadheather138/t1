代发 wailian999

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://vda.xylfe.cn

TS:   arr.map(String)
来源：http://otn.ppjwa.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://zdj.jyoumei.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://kbw.shanyushiyangkeji.top

Ruby: arr.map(&:upcase)
来源：http://mzx.uphjek.com

C#:   arr.Select(s => s.ToUpper())
来源：http://jyw.zycfv.cn

[C08] 闭包
来源：http://edw.cdnleiting.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://rcc.yuxming.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://rkj.epnwcf.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://zqq.ivvv.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://oba.andypj.xyz

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://tvk.dianchejie.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://vbl.xziqi.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://par.hongshengwenyu.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://lsc.yfazqb.com

[C09] 递归
来源：http://dbt.daria6918.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://lpa.yvedp.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ssp.fengsongda.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zrq.nanxinkj.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qsn.xuanzx.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hbk.fzhhl.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://frg.hnqzz.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://nqj.fzhhl.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mgm.wangshuangyany.cn

[C10] 变量作用域
来源：http://kbg.aibaodan.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ftr.yonumen.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://soj.havefunace.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://lfq.hywenlv.cn

TS:   同 JS
来源：http://fgc.feifeiyinyue.top

Java: 方法内为块级作用域
来源：http://tdj.ywan-chungtsiang.top

Go:   花括号块级作用域
来源：http://ttn.ydjk.org.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://opz.52xcode.cn

C#:   块级作用域
来源：http://psu.cashguo.top

[C11] 模块导入与导出
来源：http://ubw.guowangkeji.top

Py:   from module import func
来源：http://wfn.gogol.net.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://mbj.zhixingplan.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://qzt.nwbrower.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://kzm.mhx1999.top

Java: import java.util.List;
来源：http://dtl.jianghu66.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://nga.nanxuanxn.top

Ruby: require "json"; require_relative "./util"
来源：http://vui.guannengcc.top

C#:   using System.Text;
来源：http://rkj.fzhhl.top

[C12] 立即执行函数 IIFE
来源：http://nub.jinqigufen.top

Py:   (lambda: print("run"))()
来源：http://jey.tian-w.cn

PHP:  (function () { echo "run"; })();
来源：http://fnc.hongshengwenyu.top

JS:   (() => { console.log("run"); })();
来源：http://iiw.feifeiyinyue.top

TS:   (() => { console.log("run"); })();
来源：http://msf.gotoacloud.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://cmz.andypj.xyz

Go:   func() { fmt.Println("run") }()
来源：http://gqh.shanyushiyangtech.top

Ruby: -> { puts "run" }.call
来源：http://kqs.birdmap.top

C#:   // 无 IIFE：用静态构造函数
来源：http://xhc.zhoulong.xyz

[C13] 类型声明 / 类型注解
来源：http://wlt.zhijiandao.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://qaa.0kj1m.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bna.yonumen.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://rbt.jinqigufen.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dfc.0kj1m.cn

Java: int add(int a, int b) { return a + b; }
来源：http://viz.meibo888.top

Go:   func add(a, b int) int
来源：http://dpj.nanxuanxn.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://fti.tarul.cn

C#:   int Add(int a, int b) => a + b;
来源：http://akl.shangyingyoupin.top

[C14] 泛型函数
来源：http://caf.nanxuanxn.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ail.zdbjq.cn

PHP:  // 无泛型
来源：http://tbc.dashuyun.cn

JS:   // 无泛型
来源：http://dys.xinyue.icu

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://yrv.zycfv.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://xsm.ydjk.org.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://iuo.yangfankeji.com

Ruby: # 无泛型
来源：http://rcy.sjlbkw.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ugy.shuidangran.top

[C15] 解构 / 展开参数
来源：http://dvg.havefunace.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://bcr.cashguo.top

PHP:  [$a, $b] = $pair;
来源：http://mdd.quarkkingdee.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://uce.yj20258.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://xkn.jinqigufen.top

Java: // 无解构
来源：http://ywt.ivvv.top

Go:   // 无解构
来源：http://dpp.zdqjudy.top

Ruby: a, b = pair
来源：http://yac.daxiang520.top

C#:   var (a, b) = pair;
来源：http://esn.yongpay.top

[C16] 函数 / 方法重载
来源：http://ttx.fktsv.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://xqq.zhengqikj.top

PHP:  // 无重载
来源：http://sim.xuanzx.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://tal.yuxming.cn

TS:   // 用联合类型或重载签名声明
来源：http://whh.daria6918.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://nui.bbcook.cn

Go:   // 无重载：用不同函数名
来源：http://esv.gogol.net.cn

Ruby: # 无重载：靠动态参数
来源：http://rie.jiagoushi.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://jpu.yj202588.top

================================================================================
来源：http://sqr.cdnleiting.top

D. 数组 / 列表 / 集合
来源：http://sbq.ydjk.org.cn

================================================================================
来源：http://ogl.fehbvm.com

[D01] 创建数组 / 列表
来源：http://ncp.yongpay.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://kxh.shangyingyoupin.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://glx.yueranfly.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://rnz.mhx1999.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://cae.zhiwuduotai.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://grz.ehwqpu.com

Go:   arr := []int{1, 2, 3}
来源：http://rsn.xingfuxueyuan.xyz

Ruby: arr = [1, 2, 3]
来源：http://mpo.tarul.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://iew.zdqjudy.top

[D02] 追加元素到末尾
来源：http://ofi.jinqigfzy.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://div.shanyushiyangkeji.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://cwa.yj202588.top

JS:   arr.push(4);
来源：http://joi.guowangkeji.top

TS:   arr.push(4);
来源：http://hrz.zhixingplan.top

Java: list.add(4);
来源：http://kpq.snrcjt.cn

Go:   arr = append(arr, 4)
来源：http://yav.zdbjq.cn

Ruby: arr << 4; arr.push(5)
来源：http://vev.zhaomingkeji.xyz

C#:   list.Add(4);
来源：http://bnr.jinghuilouyu.cn

[D03] 在指定位置插入元素
来源：http://tos.sjlbkw.cn

Py:   arr.insert(0, 0)
来源：http://vhf.quarkkingdee.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://iig.yvedp.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://qaa.svipenyu.cn

TS:   arr.splice(0, 0, 0);
来源：http://cbv.hywenlv.cn

Java: list.add(0, 0);
来源：http://cpa.hongshengwenyu.top

Go:   arr = append([]int{0}, arr...)
来源：http://wti.jinghuilouyu.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://eqj.dianchejie.cn

C#:   list.Insert(0, 0);
来源：http://tfc.hcnkem.com

[D04] 删除元素
来源：http://ets.wangshuangyany.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://rto.c1oappe.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://txa.feifeiyinyue.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://iyz.sjlbkw.cn

TS:   arr.splice(0, 1);
来源：http://vll.jianghu66.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ntb.dianchejie.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://zla.ybcxt.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://got.yueranfly.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://zlc.aizwys.cn

[D05] 访问与修改元素
来源：http://icl.xylfe.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://utv.hcnkem.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hui.ywan-chungtsiang.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://utp.gotoacloud.top

TS:   arr[0]; arr.at(-1);
来源：http://bqx.chenzaomai.com

Java: list.get(0); list.set(0, 9);
来源：http://wbm.wangshuangyany.cn

Go:   arr[0]; arr[0] = 9
来源：http://ulx.52xcode.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://waq.wangshuangyany.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://oqu.kuanghao11.cn

[D06] 数组长度
来源：http://isl.yfazqb.com

Py:   len(arr)
来源：http://tlf.meibo888.top

PHP:  count($arr);
来源：http://jug.iojbl.cn

JS:   arr.length
来源：http://zjo.bjfxy.top

TS:   arr.length
来源：http://say.yuanzhike.top

Java: list.size();
来源：http://wnh.tarul.cn

Go:   len(arr)
来源：http://hgu.hfpthk.cn

Ruby: arr.length; arr.size
来源：http://emk.sysykeji.top

C#:   list.Count;
来源：http://svd.tanke756.top

[D07] 切片 / 取子数组
来源：http://oex.smart0.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://lmb.shangyingyoupin.top

PHP:  array_slice($arr, 1, 3);
来源：http://dep.ctjpmb.com

JS:   arr.slice(1, 4);
来源：http://oha.yuxming.cn

TS:   arr.slice(1, 4);
来源：http://hsb.yvedp.cn

Java: list.subList(1, 4);
来源：http://pfj.cqqwz.cn

Go:   arr[1:4]
来源：http://ayv.yfazqb.com

Ruby: arr[1, 3]
来源：http://mzh.hongshengwenyu.top

C#:   list.GetRange(1, 3);
来源：http://iaz.zhixingplan.top

[D08] 合并两个数组
来源：http://qdb.andypj.xyz

Py:   a + b;  a.extend(b)
来源：http://vsb.fanxiaobao.xyz

PHP:  array_merge($a, $b);
来源：http://bra.vqdsnc.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://deg.smart0.xyz

TS:   [...a, ...b];
来源：http://zdo.tarul.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://vqs.zhiwuduotai.top

Go:   append(a, b...)
来源：http://nri.snrcjt.cn

Ruby: a + b;  a.concat(b)
来源：http://vwz.fktsv.cn

C#:   a.Concat(b).ToList()
来源：http://jqc.birdmap.top

[D09] 排序（升序）
来源：http://fgn.jinqigufen.top

Py:   sorted(arr);  arr.sort()
来源：http://svy.zhiwuduotai.top

PHP:  sort($arr);
来源：http://sgk.zdqjudy.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mta.jinyuanbaomall.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://uta.bjfxy.top

Java: Collections.sort(list);  list.sort(null);
来源：http://wyp.chenzaomai.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qmp.316326.xyz

Ruby: arr.sort
来源：http://yer.daria6918.cn

C#:   list.Sort();
来源：http://rlu.cashguo.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://phs.tanke756.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mdc.hfpthk.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://uky.hfpthk.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://pwj.jinyuanbaomall.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://vum.shuidangran.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://jsn.fehbvm.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://dai.zhijiandao.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wjb.yongpay.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://lyu.sjlbkw.cn

[D11] 反转数组
来源：http://rgv.chenlongwang.top

Py:   arr[::-1];  arr.reverse()
来源：http://eio.cdnleiting.top

PHP:  array_reverse($arr);
来源：http://bpc.chenzaomai.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://gfj.nanxinkj.top

TS:   [...arr].reverse();
来源：http://bqq.ydzc1.top

Java: Collections.reverse(list);
来源：http://gwj.jinqigufen.top

Go:   slices.Reverse(arr)
来源：http://xnz.jinqigufen.top

Ruby: arr.reverse
来源：http://its.0kj1m.cn

C#:   list.Reverse();
来源：http://dmb.feifeiyinyue.top

[D12] 查找元素下标
来源：http://xaj.yj20258.top

Py:   arr.index(x);  x in arr
来源：http://rsv.chenjidiqi.icu

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://iro.shuidangran.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ilu.zhoulong.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xtr.zdbjq.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://xex.zhijiandao.cn

Go:   slices.Index(arr, x)
来源：http://kic.tian-w.cn

Ruby: arr.index(x)
来源：http://zoe.316326.xyz

C#:   list.IndexOf(x);
来源：http://zgs.tarul.cn

[D13] 过滤（保留满足条件的）
来源：http://fth.daria6918.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://rvw.zhaomingkeji.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://iri.daria6918.cn

JS:   arr.filter(x => x > 3)
来源：http://wpz.ivvv.top

TS:   arr.filter(x => x > 3)
来源：http://cer.jqgfzy.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://yyk.yj20258.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://jot.jqgfzy.top

Ruby: arr.select { |x| x > 3 }
来源：http://jqp.ydjk.org.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://hwt.fzhhl.top

[D14] 映射转换（每个元素变形）
来源：http://dgr.ydjk.org.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mmg.316326.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://viu.xziqi.cn

JS:   arr.map(x => x * 2)
来源：http://fzf.yuxming.cn

TS:   arr.map(x => x * 2)
来源：http://kqy.xziqi.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://zdd.daxiang520.top

Go:   // 手写循环
来源：http://svm.tian-w.cn

Ruby: arr.map { |x| x * 2 }
来源：http://qrx.nanxinkj.top

C#:   list.Select(x => x * 2).ToList()
来源：http://rqd.yonumen.top

[D15] 去重
来源：http://clk.xziqi.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://jdn.kuanghao11.cn

PHP:  array_unique($arr);
来源：http://sfj.haohaochexian.top

JS:   [...new Set(arr)]
来源：http://jhg.shangyingyoupin.top

TS:   [...new Set(arr)]
来源：http://pnk.chenzaomai.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://gys.svipenyu.cn

Go:   // 用 map[T]struct{} 手写
来源：http://azu.kuanghao11.cn

Ruby: arr.uniq
来源：http://xmr.xingfuxueyuan.xyz

C#:   list.Distinct().ToList()
来源：http://mhi.aizwys.cn

[D16] 求和与平均值
来源：http://uil.daxiang520.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://yrq.cheryme.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://xxo.zhixingplan.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://iuy.hysaishi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ixd.xinyue.icu

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xlp.havefunace.top

Go:   // 手写循环累加
来源：http://cml.sxryk.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://dzy.vehdjk.com

C#:   list.Sum();  list.Average()
来源：http://cnm.zhaomingkeji.xyz

[D17] 最大值与最小值
来源：http://fkk.cdnleiting.top

Py:   max(arr);  min(arr)
来源：http://jkz.shzxlz.cn

PHP:  max($arr);  min($arr);
来源：http://lzw.xinyue.icu

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ebp.316326.xyz

TS:   Math.max(...arr);
来源：http://lga.ywan-chungtsiang.top

Java: Collections.max(list);  Collections.min(list);
来源：http://lvm.gaohongyu789.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://byy.c1oappe.top

Ruby: arr.max;  arr.min
来源：http://kbt.yonumen.top

C#:   list.Max();  list.Min()
来源：http://qth.tianlin.xyz

[D18] 扁平化嵌套数组
来源：http://lns.yvedp.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://eji.daria6918.cn

PHP:  array_merge(...$nested);
来源：http://pxf.snrcjt.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mcs.jqgufenzy.top

TS:   nested.flat();
来源：http://oro.chenjidiqi.icu

Java: nested.stream().flatMap(List::stream).toList()
来源：http://vhx.chenzaomai.com

Go:   // 手写双层循环
来源：http://ndh.wangdashe.top

Ruby: nested.flatten
来源：http://xsc.gaohongyu789.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://pca.jinghuilouyu.cn

[D19] 按字段分组
来源：http://toe.ctjpmb.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://rsl.havefunace.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://gyg.uphjek.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://kik.yangfankeji.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://bgf.hesvh.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hpr.daria6918.cn

Go:   // 手写 map[string][]T
来源：http://sbg.fzhhl.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://enc.jqgufenzy.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://qca.cashguo.top

[D20] 统计每个元素出现次数
来源：http://dtl.yuanzhike.top

Py:   Counter(arr)
来源：http://qwt.fanxiaobao.xyz

PHP:  array_count_values($arr);
来源：http://ljz.nanxuanxn.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fcf.hammf.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cuz.jlsjyb.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://non.kuanghao11.cn

Go:   // 手写 map[T]int
来源：http://nkh.meibo888.top

Ruby: arr.tally
来源：http://trv.gaohongyu789.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://jaf.chenzaomai.com

[D21] 判断是否包含某元素
来源：http://tfv.jinyuanbaomall.cn

Py:   x in arr
来源：http://hwo.jinqigufen.top

PHP:  in_array($x, $arr, true);
来源：http://xvd.jianghu66.top

JS:   arr.includes(x)
来源：http://ndo.daria6918.cn

TS:   arr.includes(x)
来源：http://ytl.svipenyu.cn

Java: list.contains(x)
来源：http://wez.316326.xyz

Go:   slices.Contains(arr, x)
来源：http://gjt.tarul.cn

Ruby: arr.include?(x)
来源：http://hsp.nwbrower.top

C#:   list.Contains(x)
来源：http://liw.iojbl.cn

[D22] 复制数组（避免共享引用）
来源：http://tvr.zhongyouzk.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://lby.yj20258888.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://tai.cdnleiting.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://arw.pengpengdd.cyou

TS:   [...arr];
来源：http://wew.daria6918.cn

Java: new ArrayList<>(list);
来源：http://dfs.sufxvd.cn

Go:   copied := append([]int(nil), arr...)
来源：http://unq.daria6918.cn

Ruby: arr.dup;  arr.clone
来源：http://bpl.316326.xyz

C#:   new List<int>(list);
来源：http://ffk.ctjpmb.com

[D23] reduce 累积计算
来源：http://may.wangdashe.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ero.snrcjt.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://fdh.ybcxt.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yph.wangdashe.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ogh.svipenyu.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ugk.sweek.top

Go:   // 手写循环
来源：http://nei.daxiang520.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://bds.xinyue.icu

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://skd.smart0.xyz

[D24] 字典 / Map 基本操作
来源：http://yww.sjlbkw.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wnu.cheryme.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://foz.shanyushiyangkeji.top


<!-- 参考信息 -->