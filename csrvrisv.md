代发 wailian999

TS:   const square = (x: number): number => x * x;
来源：http://bgy.sysykeji.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://buk.aizwys.cn

Go:   sq := func(x int) int { return x * x }
来源：http://fkk.tarul.cn

Ruby: square = ->(x) { x * x }
来源：http://gzp.vehdjk.com

C#:   Func<int, int> square = x => x * x;
来源：http://crd.cheryme.top

[C07] 把函数作为参数传入
来源：http://xcq.xuetiantiany.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://jiu.tianlin.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://gxf.dashuyun.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://deh.sysykeji.top

TS:   arr.map(String)
来源：http://wug.tian-w.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ynk.shanyushiyangtech.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://cpm.ywan-chungtsiang.top

Ruby: arr.map(&:upcase)
来源：http://zzv.jinyuanbaomall.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://rut.yuxming.cn

[C08] 闭包
来源：http://tbm.yj20258888.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://egx.hysaishi.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ndq.sufxvd.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://avl.zdbjq.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://pju.guowangkeji.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://yxf.ydjk.org.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://rtu.ivvv.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hsc.sjlbkw.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://yde.havefunace.top

[C09] 递归
来源：http://vuq.jqgufenzy.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://djj.fzhhl.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://tfv.hesvh.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bxw.yj202588.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jsf.snrcjt.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://xmb.yanxiufei.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://zqr.ybcxt.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wjp.zhixingplan.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hmf.zhoulong.xyz

[C10] 变量作用域
来源：http://mpu.jianghu66.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://uix.smart0.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://toi.sysykeji.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://zmp.sxryk.cn

TS:   同 JS
来源：http://nbv.jinyuanbaomall.cn

Java: 方法内为块级作用域
来源：http://bij.meibo888.top

Go:   花括号块级作用域
来源：http://ltx.yuxming.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ljn.pycfn.com

C#:   块级作用域
来源：http://icg.jianghu66.top

[C11] 模块导入与导出
来源：http://goh.xuetiantiany.cn

Py:   from module import func
来源：http://iqz.yj202588.top

PHP:  require "file.php";  或 use App\Service;
来源：http://jqc.mhx1999.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://urq.daxiang520.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ioc.cheryme.top

Java: import java.util.List;
来源：http://afq.zdbjq.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://tvw.wangshuangyany.cn

Ruby: require "json"; require_relative "./util"
来源：http://yop.snrcjt.cn

C#:   using System.Text;
来源：http://ocj.fehbvm.com

[C12] 立即执行函数 IIFE
来源：http://hgk.c1oappe.top

Py:   (lambda: print("run"))()
来源：http://dfr.dashuyun.cn

PHP:  (function () { echo "run"; })();
来源：http://eru.ydjk.org.cn

JS:   (() => { console.log("run"); })();
来源：http://jgc.sweek.top

TS:   (() => { console.log("run"); })();
来源：http://doe.fengsongda.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jpr.0kj1m.cn

Go:   func() { fmt.Println("run") }()
来源：http://vub.chenlongwang.top

Ruby: -> { puts "run" }.call
来源：http://tgg.zdqjudy.top

C#:   // 无 IIFE：用静态构造函数
来源：http://hyr.hcnkem.com

[C13] 类型声明 / 类型注解
来源：http://xxg.jianghu66.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://yzw.yongpay.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://aed.hesvh.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hrl.pycfn.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dbp.aizwys.cn

Java: int add(int a, int b) { return a + b; }
来源：http://lpi.sxryk.cn

Go:   func add(a, b int) int
来源：http://yvj.haohaochexian.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://qyr.sufxvd.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ket.zdbjq.cn

[C14] 泛型函数
来源：http://exp.sxryk.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://pot.pycfn.com

PHP:  // 无泛型
来源：http://oly.zhiwuduotai.top

JS:   // 无泛型
来源：http://hhd.0kj1m.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://jss.shanyushiyangkeji.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://pjk.ctjpmb.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://vcq.sweek.top

Ruby: # 无泛型
来源：http://euk.zhaomingkeji.xyz

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ulg.sxryk.cn

[C15] 解构 / 展开参数
来源：http://ssa.jiagoushi.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://fuj.sjlbkw.cn

PHP:  [$a, $b] = $pair;
来源：http://skk.zhijiandao.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://gch.hfpthk.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://vtj.fanxiaobao.xyz

Java: // 无解构
来源：http://ywg.zycfv.cn

Go:   // 无解构
来源：http://bvg.ehwqpu.com

Ruby: a, b = pair
来源：http://uvg.chenlongwang.top

C#:   var (a, b) = pair;
来源：http://ukd.jinqigufen.top

[C16] 函数 / 方法重载
来源：http://ary.cheryme.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mrq.snrcjt.cn

PHP:  // 无重载
来源：http://zpt.zhoulong.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://zvy.jinqigfzy.top

TS:   // 用联合类型或重载签名声明
来源：http://dhj.aizwys.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://wds.sjlbkw.cn

Go:   // 无重载：用不同函数名
来源：http://nqd.ivvv.top

Ruby: # 无重载：靠动态参数
来源：http://kap.ywan-chungtsiang.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://aoe.yangfankeji.com

================================================================================
来源：http://noa.aibaodan.cn

D. 数组 / 列表 / 集合
来源：http://jnb.shanyushiyangtech.top

================================================================================
来源：http://tpm.meibo888.top

[D01] 创建数组 / 列表
来源：http://yel.dianchejie.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ktf.0kj1m.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://inw.hammf.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://oyk.zhaomingkeji.xyz

TS:   const arr: number[] = [1, 2, 3];
来源：http://wvt.chenlongwang.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://tpg.gaohongyu789.top

Go:   arr := []int{1, 2, 3}
来源：http://cqg.xylfe.cn

Ruby: arr = [1, 2, 3]
来源：http://ddy.yuanzhike.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://dtx.jlsjyb.cn

[D02] 追加元素到末尾
来源：http://cnr.ydjk.org.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://nwc.gaohongyu789.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://oxl.yonumen.top

JS:   arr.push(4);
来源：http://gww.redwolf501.top

TS:   arr.push(4);
来源：http://ojy.snrcjt.cn

Java: list.add(4);
来源：http://vah.jinqigfzy.top

Go:   arr = append(arr, 4)
来源：http://ztf.xziqi.cn

Ruby: arr << 4; arr.push(5)
来源：http://acj.shangyingyoupin.top

C#:   list.Add(4);
来源：http://lik.fzhhl.top

[D03] 在指定位置插入元素
来源：http://ltz.gogol.net.cn

Py:   arr.insert(0, 0)
来源：http://skc.ctjpmb.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mqh.bjfxy.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ozd.jiagoushi.top

TS:   arr.splice(0, 0, 0);
来源：http://dus.sjlbkw.cn

Java: list.add(0, 0);
来源：http://gup.zhiwuduotai.top

Go:   arr = append([]int{0}, arr...)
来源：http://osw.jianghu66.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hfv.ybcxt.top

C#:   list.Insert(0, 0);
来源：http://hbe.pengpengdd.cyou

[D04] 删除元素
来源：http://chx.xuanzx.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ehi.hesvh.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mph.hesvh.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://yyg.cashguo.top

TS:   arr.splice(0, 1);
来源：http://jgz.xingfuxueyuan.xyz

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://omk.tarul.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://npo.yvedp.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://qyb.sjlbkw.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://vre.quarkkingdee.top

[D05] 访问与修改元素
来源：http://xgt.haohaochexian.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ohy.tarul.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ayl.ybcxt.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ukt.jqgufenzy.top

TS:   arr[0]; arr.at(-1);
来源：http://hye.chenjidiqi.icu

Java: list.get(0); list.set(0, 9);
来源：http://lgk.shanyushiyangkeji.top

Go:   arr[0]; arr[0] = 9
来源：http://lou.gaohongyu789.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wha.zhongyouzk.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://oyr.daria6918.cn

[D06] 数组长度
来源：http://iiz.bbcook.cn

Py:   len(arr)
来源：http://sxk.yueranfly.top

PHP:  count($arr);
来源：http://xcz.cdnleiting.top

JS:   arr.length
来源：http://mcg.meibo888.top

TS:   arr.length
来源：http://iek.daxiang520.top

Java: list.size();
来源：http://nae.jqgufenzy.top

Go:   len(arr)
来源：http://smi.redwolf501.top

Ruby: arr.length; arr.size
来源：http://uuo.redwolf501.top

C#:   list.Count;
来源：http://mnr.pycfn.com

[D07] 切片 / 取子数组
来源：http://jbr.mhx1999.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://nyy.zhixingplan.top

PHP:  array_slice($arr, 1, 3);
来源：http://ywd.birdmap.top

JS:   arr.slice(1, 4);
来源：http://ygj.ctjpmb.com

TS:   arr.slice(1, 4);
来源：http://xei.hywenlv.cn

Java: list.subList(1, 4);
来源：http://ubn.shuidangran.top

Go:   arr[1:4]
来源：http://ozq.tian-w.cn

Ruby: arr[1, 3]
来源：http://stk.yanxiufei.cn

C#:   list.GetRange(1, 3);
来源：http://gqx.9152youxi.cn

[D08] 合并两个数组
来源：http://kfa.kuanghao11.cn

Py:   a + b;  a.extend(b)
来源：http://zif.chenzaomai.com

PHP:  array_merge($a, $b);
来源：http://tvx.gaohongyu789.top

JS:   [...a, ...b];  a.concat(b);
来源：http://bli.shanyushiyangtech.top

TS:   [...a, ...b];
来源：http://tbb.ivvv.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://dxn.pengpengdd.cyou

Go:   append(a, b...)
来源：http://wxd.aizwys.cn

Ruby: a + b;  a.concat(b)
来源：http://lqq.sufxvd.cn

C#:   a.Concat(b).ToList()
来源：http://xsj.shanyushiyangtech.top

[D09] 排序（升序）
来源：http://cjb.bjfxy.top

Py:   sorted(arr);  arr.sort()
来源：http://nxr.gogol.net.cn

PHP:  sort($arr);
来源：http://mge.yj20258.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ugz.0kj1m.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://eyi.ydzc1.top

Java: Collections.sort(list);  list.sort(null);
来源：http://ewh.yuxming.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ywo.dianchejie.cn

Ruby: arr.sort
来源：http://qeb.hnqzz.top

C#:   list.Sort();
来源：http://ucm.zhijiandao.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://btw.hysaishi.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://awm.smart0.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://txj.uphjek.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://zxu.havefunace.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://cbz.ppjwa.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://tcq.ehwqpu.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://btz.vehdjk.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://fxp.havefunace.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://afo.fengsongda.top

[D11] 反转数组
来源：http://bmr.dianchejie.cn

Py:   arr[::-1];  arr.reverse()
来源：http://wbq.nanxuanxn.top

PHP:  array_reverse($arr);
来源：http://tzi.ywan-chungtsiang.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://lkg.316326.xyz

TS:   [...arr].reverse();
来源：http://ayh.hesvh.cn

Java: Collections.reverse(list);
来源：http://ept.feifeiyinyue.top

Go:   slices.Reverse(arr)
来源：http://lon.zhiwuduotai.top

Ruby: arr.reverse
来源：http://qdz.jinghuilouyu.cn

C#:   list.Reverse();
来源：http://knl.hysaishi.cn

[D12] 查找元素下标
来源：http://eml.cashguo.top

Py:   arr.index(x);  x in arr
来源：http://cuf.ydjk.org.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://iyz.tarul.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ick.nanxinkj.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://daz.yvedp.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wou.zycfv.cn

Go:   slices.Index(arr, x)
来源：http://yfm.iojbl.cn

Ruby: arr.index(x)
来源：http://mzc.meibo888.top

C#:   list.IndexOf(x);
来源：http://mst.guowangkeji.top

[D13] 过滤（保留满足条件的）
来源：http://nfn.fanxiaobao.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ivt.xziqi.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://huq.jyoumei.cn

JS:   arr.filter(x => x > 3)
来源：http://kam.zhoulong.xyz

TS:   arr.filter(x => x > 3)
来源：http://ovk.xingfuxueyuan.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://glq.shanyushiyangkeji.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://nfy.jinyuanbaomall.cn

Ruby: arr.select { |x| x > 3 }
来源：http://asn.jinqigfzy.top

C#:   list.Where(x => x > 3).ToList()
来源：http://tlh.yanxiufei.cn

[D14] 映射转换（每个元素变形）
来源：http://ukl.havefunace.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://siq.daria6918.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://cwb.iojbl.cn

JS:   arr.map(x => x * 2)
来源：http://dmx.yj20258.top

TS:   arr.map(x => x * 2)
来源：http://rxp.yuanzhike.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://wzy.shanyushiyangkeji.top

Go:   // 手写循环
来源：http://hxm.hnqzz.top

Ruby: arr.map { |x| x * 2 }
来源：http://ijm.fanxiaobao.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://vmq.zhoulong.xyz

[D15] 去重
来源：http://vam.ivvv.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://zqr.sweek.top

PHP:  array_unique($arr);
来源：http://wpy.fzhhl.top

JS:   [...new Set(arr)]
来源：http://bwr.tanke756.top

TS:   [...new Set(arr)]
来源：http://iev.guannengcc.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://atb.gzhubu.top

Go:   // 用 map[T]struct{} 手写
来源：http://smp.ywan-chungtsiang.top

Ruby: arr.uniq
来源：http://ylm.haohaochexian.top

C#:   list.Distinct().ToList()
来源：http://yqg.316326.xyz

[D16] 求和与平均值
来源：http://mrx.cqqwz.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://vvp.xziqi.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://vjc.jianghu66.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://vtj.hfpthk.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hpy.9152youxi.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://uui.wangshuangyany.cn

Go:   // 手写循环累加
来源：http://poj.ydjk.org.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://dws.yangfankeji.com

C#:   list.Sum();  list.Average()
来源：http://ivz.pycfn.com

[D17] 最大值与最小值
来源：http://pxq.chenjidiqi.icu

Py:   max(arr);  min(arr)
来源：http://fzc.chenlongwang.top

PHP:  max($arr);  min($arr);
来源：http://gaj.gotoacloud.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mfa.pengpengdd.cyou

TS:   Math.max(...arr);
来源：http://ikh.fanxiaobao.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://kbj.yj202588.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://lug.bjfxy.top

Ruby: arr.max;  arr.min
来源：http://tlq.shangyingyoupin.top

C#:   list.Max();  list.Min()
来源：http://ths.vehdjk.com

[D18] 扁平化嵌套数组
来源：http://lpa.hywenlv.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://jtq.zdqjudy.top

PHP:  array_merge(...$nested);
来源：http://sbw.ybcxt.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://gtz.sufxvd.cn

TS:   nested.flat();
来源：http://piv.uphjek.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://bvz.tanke756.top

Go:   // 手写双层循环
来源：http://hzr.tian-w.cn

Ruby: nested.flatten
来源：http://jtx.hywenlv.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://kms.daria6918.cn

[D19] 按字段分组
来源：http://nrt.fanxiaobao.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://qub.tian-w.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://gye.vqdsnc.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://uoh.hnxiangtu.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://oky.zhengqikj.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hym.ivvv.top

Go:   // 手写 map[string][]T
来源：http://uxa.fzhhl.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://gzf.hnxiangtu.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ebo.tanke756.top

[D20] 统计每个元素出现次数
来源：http://cin.gotoacloud.top

Py:   Counter(arr)
来源：http://rum.yuxming.cn

PHP:  array_count_values($arr);
来源：http://mma.gaohongyu789.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bwj.xuetiantiany.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://iuz.9152youxi.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://lfl.jyoumei.cn

Go:   // 手写 map[T]int
来源：http://rlp.chenjidiqi.icu

Ruby: arr.tally
来源：http://lwd.tian-w.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ynv.cqqwz.cn

[D21] 判断是否包含某元素
来源：http://gao.redwolf501.top

Py:   x in arr
来源：http://xlm.chenjidiqi.icu

PHP:  in_array($x, $arr, true);
来源：http://qgi.yfazqb.com

JS:   arr.includes(x)
来源：http://osd.zdbjq.cn

TS:   arr.includes(x)
来源：http://zmz.hongshengwenyu.top

Java: list.contains(x)
来源：http://taj.hesvh.cn

Go:   slices.Contains(arr, x)
来源：http://oip.wangshuangyany.cn

Ruby: arr.include?(x)
来源：http://myx.zhixingplan.top

C#:   list.Contains(x)
来源：http://xzi.xinyue.icu

[D22] 复制数组（避免共享引用）
来源：http://bmi.52xcode.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://jwn.guowangkeji.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://myt.jinqigfzy.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mxt.cheryme.top

TS:   [...arr];
来源：http://jkv.svipenyu.cn

Java: new ArrayList<>(list);
来源：http://jqf.guowangkeji.top

Go:   copied := append([]int(nil), arr...)
来源：http://ohr.chenlongwang.top

Ruby: arr.dup;  arr.clone
来源：http://ssq.snrcjt.cn

C#:   new List<int>(list);
来源：http://tps.wangshuangyany.cn

[D23] reduce 累积计算
来源：http://jct.dashuyun.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ezb.sysykeji.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mbz.ywan-chungtsiang.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://eud.sxryk.cn


<!-- 参考信息 -->