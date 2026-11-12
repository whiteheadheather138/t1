代发 wailian999

[C06] 匿名函数 / lambda
来源：http://rii.yueranfly.top

Py:   square = lambda x: x * x
来源：http://bnv.0kj1m.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://jnz.sufxvd.cn

JS:   const square = x => x * x;
来源：http://thn.vqdsnc.cn

TS:   const square = (x: number): number => x * x;
来源：http://kcx.jinghuilouyu.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hrd.yuxming.cn

Go:   sq := func(x int) int { return x * x }
来源：http://jnj.iojbl.cn

Ruby: square = ->(x) { x * x }
来源：http://car.cucudq.cn

C#:   Func<int, int> square = x => x * x;
来源：http://xfh.meibo888.top

[C07] 把函数作为参数传入
来源：http://axq.zhixingplan.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://kvw.9152youxi.cn

PHP:  array_map("strtoupper", $arr);
来源：http://wrj.316326.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://vsl.aizwys.cn

TS:   arr.map(String)
来源：http://lnr.cheryme.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://qkf.yvedp.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://jfn.sjlbkw.cn

Ruby: arr.map(&:upcase)
来源：http://axa.hcnkem.com

C#:   arr.Select(s => s.ToUpper())
来源：http://jor.pengpengdd.cyou

[C08] 闭包
来源：http://yel.sweek.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://aog.cdnleiting.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://opb.hfpthk.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://jtd.zhengqikj.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://dhr.cashguo.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://tlz.dianchejie.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://rjp.aizwys.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://iod.ppjwa.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://euj.jinghuilouyu.cn

[C09] 递归
来源：http://ucq.nanxinkj.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ags.hywenlv.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ryp.zdqjudy.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nqv.bbcook.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sur.havefunace.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hcz.ybcxt.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://xir.feifeiyinyue.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://lvb.zhijiandao.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://axz.cucudq.cn

[C10] 变量作用域
来源：http://buh.xuetiantiany.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://rya.chenzaomai.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://rgu.yvedp.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://dhs.cheryme.top

TS:   同 JS
来源：http://ass.birdmap.top

Java: 方法内为块级作用域
来源：http://gzs.vehdjk.com

Go:   花括号块级作用域
来源：http://sjd.yfazqb.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://yre.tarul.cn

C#:   块级作用域
来源：http://lqg.daria6918.cn

[C11] 模块导入与导出
来源：http://vsb.mhx1999.top

Py:   from module import func
来源：http://qlk.yanxiufei.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://iow.chenjidiqi.icu

JS:   export default function f() {};  import f from "./m.js";
来源：http://vqe.xingfuxueyuan.xyz

TS:   export function f(): void {};  import { f } from "./m";
来源：http://qgi.haohaochexian.top

Java: import java.util.List;
来源：http://tfg.gaohongyu789.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://qjl.yuanzhike.top

Ruby: require "json"; require_relative "./util"
来源：http://tcg.hfpthk.cn

C#:   using System.Text;
来源：http://vtl.feifeiyinyue.top

[C12] 立即执行函数 IIFE
来源：http://frs.ctjpmb.com

Py:   (lambda: print("run"))()
来源：http://bdf.ctjpmb.com

PHP:  (function () { echo "run"; })();
来源：http://miw.ybcxt.top

JS:   (() => { console.log("run"); })();
来源：http://hkq.gogol.net.cn

TS:   (() => { console.log("run"); })();
来源：http://dxb.hfpthk.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mbf.yvedp.cn

Go:   func() { fmt.Println("run") }()
来源：http://xlq.hongshengwenyu.top

Ruby: -> { puts "run" }.call
来源：http://coy.shanyushiyangkeji.top

C#:   // 无 IIFE：用静态构造函数
来源：http://sar.fktsv.cn

[C13] 类型声明 / 类型注解
来源：http://rml.yongpay.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wml.tanke756.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cuv.hammf.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://tia.xinyue.icu

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://plt.wangshuangyany.cn

Java: int add(int a, int b) { return a + b; }
来源：http://enu.fzhhl.top

Go:   func add(a, b int) int
来源：http://thr.pycfn.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://fde.nwbrower.top

C#:   int Add(int a, int b) => a + b;
来源：http://iiy.shanyushiyangtech.top

[C14] 泛型函数
来源：http://nkq.52xcode.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wpi.jianghu66.top

PHP:  // 无泛型
来源：http://wbs.zhoulong.xyz

JS:   // 无泛型
来源：http://lnq.yj202588.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://owh.jqgufenzy.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://yir.gaohongyu789.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://nxo.yuxming.cn

Ruby: # 无泛型
来源：http://auz.zhaomingkeji.xyz

C#:   static T First<T>(List<T> items) => items[0];
来源：http://vwu.nwbrower.top

[C15] 解构 / 展开参数
来源：http://thc.jinqigufen.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ibe.xuetiantiany.cn

PHP:  [$a, $b] = $pair;
来源：http://fjs.xuanzx.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xcz.sweek.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://gfq.hfpthk.cn

Java: // 无解构
来源：http://gmo.yj202588.top

Go:   // 无解构
来源：http://zzl.chenlongwang.top

Ruby: a, b = pair
来源：http://fax.cdnleiting.top

C#:   var (a, b) = pair;
来源：http://icb.xziqi.cn

[C16] 函数 / 方法重载
来源：http://iyw.nwbrower.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://dps.9152youxi.cn

PHP:  // 无重载
来源：http://lah.hfpthk.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://xpa.hfpthk.cn

TS:   // 用联合类型或重载签名声明
来源：http://rsn.yangfankeji.com

Java: void f(int a) {}  void f(String a) {}
来源：http://wra.tanke756.top

Go:   // 无重载：用不同函数名
来源：http://kry.uphjek.com

Ruby: # 无重载：靠动态参数
来源：http://fof.wangdashe.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://dww.guowangkeji.top

================================================================================
来源：http://ppj.zhengqikj.top

D. 数组 / 列表 / 集合
来源：http://yfq.hammf.cn

================================================================================
来源：http://bcg.epnwcf.com

[D01] 创建数组 / 列表
来源：http://iha.tarul.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://kva.0kj1m.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ctx.chenzaomai.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://lgg.yonumen.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://fmb.redwolf501.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hdk.cashguo.top

Go:   arr := []int{1, 2, 3}
来源：http://olv.kuanghao11.cn

Ruby: arr = [1, 2, 3]
来源：http://trn.pycfn.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ucf.guannengcc.top

[D02] 追加元素到末尾
来源：http://orm.jinqigfzy.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hrp.vehdjk.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://xce.dianchejie.cn

JS:   arr.push(4);
来源：http://cdj.vqdsnc.cn

TS:   arr.push(4);
来源：http://vpb.zhoulong.xyz

Java: list.add(4);
来源：http://dzy.smart0.xyz

Go:   arr = append(arr, 4)
来源：http://qwk.fzhhl.top

Ruby: arr << 4; arr.push(5)
来源：http://sau.gotoacloud.top

C#:   list.Add(4);
来源：http://byk.cheryme.top

[D03] 在指定位置插入元素
来源：http://ltr.ydzc1.top

Py:   arr.insert(0, 0)
来源：http://oyn.zhijiandao.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://cxi.sweek.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ric.ehwqpu.com

TS:   arr.splice(0, 0, 0);
来源：http://ayr.nwbrower.top

Java: list.add(0, 0);
来源：http://vna.0kj1m.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ozk.cqqwz.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://xcu.ctjpmb.com

C#:   list.Insert(0, 0);
来源：http://bmc.jinyuanbaomall.cn

[D04] 删除元素
来源：http://agd.sjlbkw.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://iut.epnwcf.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ohd.zycfv.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ugw.aizwys.cn

TS:   arr.splice(0, 1);
来源：http://saq.sweek.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://pul.gogol.net.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://gfi.zdqjudy.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://keo.chenjidiqi.icu

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://rhp.hfpthk.cn

[D05] 访问与修改元素
来源：http://qxh.mhx1999.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://cqi.bbcook.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://njm.guannengcc.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://xio.aibaodan.cn

TS:   arr[0]; arr.at(-1);
来源：http://lvh.zhaomingkeji.xyz

Java: list.get(0); list.set(0, 9);
来源：http://ytm.hfpthk.cn

Go:   arr[0]; arr[0] = 9
来源：http://pcv.wangshuangyany.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wur.tanke756.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://odv.chenlongwang.top

[D06] 数组长度
来源：http://bta.jinqigufen.top

Py:   len(arr)
来源：http://bjt.aizwys.cn

PHP:  count($arr);
来源：http://mkn.gogol.net.cn

JS:   arr.length
来源：http://qrj.ywan-chungtsiang.top

TS:   arr.length
来源：http://uit.daxiang520.top

Java: list.size();
来源：http://lfe.xingfuxueyuan.xyz

Go:   len(arr)
来源：http://azf.c1oappe.top

Ruby: arr.length; arr.size
来源：http://neu.uphjek.com

C#:   list.Count;
来源：http://jwq.uphjek.com

[D07] 切片 / 取子数组
来源：http://fmb.jqgfzy.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qva.yongpay.top

PHP:  array_slice($arr, 1, 3);
来源：http://tid.xylfe.cn

JS:   arr.slice(1, 4);
来源：http://cxp.chenjidiqi.icu

TS:   arr.slice(1, 4);
来源：http://gnt.hysaishi.cn

Java: list.subList(1, 4);
来源：http://azm.xylfe.cn

Go:   arr[1:4]
来源：http://yyl.zhijiandao.cn

Ruby: arr[1, 3]
来源：http://rxo.xinyue.icu

C#:   list.GetRange(1, 3);
来源：http://dcn.havefunace.top

[D08] 合并两个数组
来源：http://bbt.xuetiantiany.cn

Py:   a + b;  a.extend(b)
来源：http://jbp.zdqjudy.top

PHP:  array_merge($a, $b);
来源：http://ffr.hfpthk.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://yih.xingfuxueyuan.xyz

TS:   [...a, ...b];
来源：http://dez.vqdsnc.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://znx.316326.xyz

Go:   append(a, b...)
来源：http://cfs.smart0.xyz

Ruby: a + b;  a.concat(b)
来源：http://smz.ctjpmb.com

C#:   a.Concat(b).ToList()
来源：http://alg.jiagoushi.top

[D09] 排序（升序）
来源：http://etg.jinghuilouyu.cn

Py:   sorted(arr);  arr.sort()
来源：http://jwc.daxiang520.top

PHP:  sort($arr);
来源：http://hvn.svipenyu.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://grx.zhoulong.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://rxn.shzxlz.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://stf.hysaishi.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://xnv.zdbjq.cn

Ruby: arr.sort
来源：http://hvj.nwbrower.top

C#:   list.Sort();
来源：http://mze.9152youxi.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ovt.zhiwuduotai.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://zuw.bbcook.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ksw.cqqwz.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://yvk.xingfuxueyuan.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://uvo.316326.xyz

Java: list.sort(Comparator.comparing(Person::age));
来源：http://kwt.0kj1m.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://jjh.gzhubu.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://qhc.jinyuanbaomall.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://prr.nanxinkj.top

[D11] 反转数组
来源：http://oig.yj202588.top

Py:   arr[::-1];  arr.reverse()
来源：http://syy.yuanzhike.top

PHP:  array_reverse($arr);
来源：http://yta.bjfxy.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://nhq.guannengcc.top

TS:   [...arr].reverse();
来源：http://mqr.gotoacloud.top

Java: Collections.reverse(list);
来源：http://htn.ivvv.top

Go:   slices.Reverse(arr)
来源：http://ciu.wangshuangyany.cn

Ruby: arr.reverse
来源：http://ndw.ctjpmb.com

C#:   list.Reverse();
来源：http://osw.hywenlv.cn

[D12] 查找元素下标
来源：http://qgp.kuanghao11.cn

Py:   arr.index(x);  x in arr
来源：http://sir.tarul.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hag.hnxiangtu.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tme.zhijiandao.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://obm.yongpay.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://flh.zdqjudy.top

Go:   slices.Index(arr, x)
来源：http://hjh.cucudq.cn

Ruby: arr.index(x)
来源：http://wrp.gzhubu.top

C#:   list.IndexOf(x);
来源：http://yjx.jqgufenzy.top

[D13] 过滤（保留满足条件的）
来源：http://quw.chenzaomai.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://tfo.xingfuxueyuan.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://weh.jinqigufen.top

JS:   arr.filter(x => x > 3)
来源：http://sft.guowangkeji.top

TS:   arr.filter(x => x > 3)
来源：http://wmi.hnqzz.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mjm.jyoumei.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://tbz.nanxinkj.top

Ruby: arr.select { |x| x > 3 }
来源：http://xgx.gogol.net.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://pcr.nanxinkj.top

[D14] 映射转换（每个元素变形）
来源：http://wrk.chenjidiqi.icu

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ejs.gzhubu.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://pez.aibaodan.cn

JS:   arr.map(x => x * 2)
来源：http://pja.dashuyun.cn

TS:   arr.map(x => x * 2)
来源：http://vib.yj20258.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://zto.gotoacloud.top

Go:   // 手写循环
来源：http://ffk.sjlbkw.cn

Ruby: arr.map { |x| x * 2 }
来源：http://jpg.hesvh.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ibk.fktsv.cn

[D15] 去重
来源：http://swy.yueranfly.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://bsq.ywan-chungtsiang.top

PHP:  array_unique($arr);
来源：http://lbt.wangshuangyany.cn

JS:   [...new Set(arr)]
来源：http://gmk.ivvv.top

TS:   [...new Set(arr)]
来源：http://ikn.ywan-chungtsiang.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ezm.havefunace.top

Go:   // 用 map[T]struct{} 手写
来源：http://ade.yongpay.top

Ruby: arr.uniq
来源：http://ooz.jyoumei.cn

C#:   list.Distinct().ToList()
来源：http://sai.gogol.net.cn

[D16] 求和与平均值
来源：http://ukk.ivvv.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://joy.smart0.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://fyu.ydzc1.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://krg.jiagoushi.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://fyb.0kj1m.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://orx.9152youxi.cn

Go:   // 手写循环累加
来源：http://lls.ctjpmb.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://okx.yuanzhike.top

C#:   list.Sum();  list.Average()
来源：http://ome.fengsongda.top

[D17] 最大值与最小值
来源：http://kqs.gaohongyu789.top

Py:   max(arr);  min(arr)
来源：http://jdt.havefunace.top

PHP:  max($arr);  min($arr);
来源：http://dhl.sjlbkw.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://psu.hywenlv.cn

TS:   Math.max(...arr);
来源：http://llr.jlsjyb.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://lsh.dashuyun.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://imb.jiagoushi.top

Ruby: arr.max;  arr.min
来源：http://cls.316326.xyz

C#:   list.Max();  list.Min()
来源：http://lko.xuanzx.com

[D18] 扁平化嵌套数组
来源：http://mgo.c1oappe.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://osg.yangfankeji.com

PHP:  array_merge(...$nested);
来源：http://jen.hongshengwenyu.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://bmv.sysykeji.top

TS:   nested.flat();
来源：http://gzz.xziqi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://coo.jinqigufen.top

Go:   // 手写双层循环
来源：http://aeo.hnxiangtu.top

Ruby: nested.flatten
来源：http://fah.quarkkingdee.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://wqv.nanxuanxn.top

[D19] 按字段分组
来源：http://wmd.zhiwuduotai.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hop.ctjpmb.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://xau.dianchejie.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://nor.tanke756.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://ptf.gzhubu.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://tyj.shanyushiyangtech.top

Go:   // 手写 map[string][]T
来源：http://zcg.guannengcc.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://xkj.aibaodan.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://oaq.cheryme.top

[D20] 统计每个元素出现次数
来源：http://vil.dashuyun.cn

Py:   Counter(arr)
来源：http://npt.ybcxt.top

PHP:  array_count_values($arr);
来源：http://txc.xylfe.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tyl.jqgfzy.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pvg.daria6918.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ibw.birdmap.top

Go:   // 手写 map[T]int
来源：http://plo.hywenlv.cn

Ruby: arr.tally
来源：http://ctc.c1oappe.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://rkn.ybcxt.top

[D21] 判断是否包含某元素
来源：http://cuo.yj20258.top

Py:   x in arr
来源：http://pvi.hywenlv.cn

PHP:  in_array($x, $arr, true);
来源：http://ohi.yangfankeji.com

JS:   arr.includes(x)
来源：http://vuv.zhiwuduotai.top

TS:   arr.includes(x)
来源：http://iob.xinyue.icu

Java: list.contains(x)
来源：http://ykx.chenjidiqi.icu

Go:   slices.Contains(arr, x)
来源：http://kns.jinyuanbaomall.cn

Ruby: arr.include?(x)
来源：http://oux.andypj.xyz

C#:   list.Contains(x)
来源：http://cqt.yuanzhike.top

[D22] 复制数组（避免共享引用）
来源：http://yke.wangshuangyany.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ljw.tarul.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hbd.bbcook.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://qqs.aizwys.cn

TS:   [...arr];
来源：http://tff.quarkkingdee.top

Java: new ArrayList<>(list);
来源：http://zug.cqqwz.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ueu.uphjek.com

Ruby: arr.dup;  arr.clone
来源：http://gqh.xingfuxueyuan.xyz

C#:   new List<int>(list);
来源：http://otq.yonumen.top


<!-- 参考信息 -->