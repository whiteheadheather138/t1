代发 wailian999

[C06] 匿名函数 / lambda
来源：http://ubh.fktsv.cn

Py:   square = lambda x: x * x
来源：http://clr.jyoumei.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://xok.ybcxt.top

JS:   const square = x => x * x;
来源：http://nha.jinqigfzy.top

TS:   const square = (x: number): number => x * x;
来源：http://gdj.uphjek.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hag.gogol.net.cn

Go:   sq := func(x int) int { return x * x }
来源：http://hqw.316326.xyz

Ruby: square = ->(x) { x * x }
来源：http://ywa.9152youxi.cn

C#:   Func<int, int> square = x => x * x;
来源：http://osw.mhx1999.top

[C07] 把函数作为参数传入
来源：http://xif.xinyue.icu

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mav.yanxiufei.cn

PHP:  array_map("strtoupper", $arr);
来源：http://wgz.daria6918.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://skn.ydjk.org.cn

TS:   arr.map(String)
来源：http://whz.chenzaomai.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ikh.sxryk.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://xku.gzhubu.top

Ruby: arr.map(&:upcase)
来源：http://rim.redwolf501.top

C#:   arr.Select(s => s.ToUpper())
来源：http://fww.bjfxy.top

[C08] 闭包
来源：http://qsi.yfazqb.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://tsp.birdmap.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mee.tianlin.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://jud.nanxinkj.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ufx.fzhhl.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://let.jinqigufen.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://qbv.zdqjudy.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://jsy.birdmap.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ycr.jinghuilouyu.cn

[C09] 递归
来源：http://fwg.xuetiantiany.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://svq.cheryme.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://rkg.jinghuilouyu.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vqg.daria6918.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kbd.nanxinkj.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://oja.fanxiaobao.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://vqg.yvedp.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://uxd.guowangkeji.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://bsx.zdqjudy.top

[C10] 变量作用域
来源：http://ghu.ivvv.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://cww.nanxuanxn.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ceo.zdqjudy.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://enm.ehwqpu.com

TS:   同 JS
来源：http://jrk.yj20258.top

Java: 方法内为块级作用域
来源：http://byz.tian-w.cn

Go:   花括号块级作用域
来源：http://dyg.tarul.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ayi.fzhhl.top

C#:   块级作用域
来源：http://ljt.fengsongda.top

[C11] 模块导入与导出
来源：http://qol.zhixingplan.top

Py:   from module import func
来源：http://odi.52xcode.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://bgn.xylfe.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://sai.cheryme.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://oae.zhongyouzk.top

Java: import java.util.List;
来源：http://jro.hcnkem.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ape.ywan-chungtsiang.top

Ruby: require "json"; require_relative "./util"
来源：http://zdh.shanyushiyangkeji.top

C#:   using System.Text;
来源：http://bqp.jqgufenzy.top

[C12] 立即执行函数 IIFE
来源：http://fra.jianghu66.top

Py:   (lambda: print("run"))()
来源：http://dzs.tianlin.xyz

PHP:  (function () { echo "run"; })();
来源：http://aky.fzhhl.top

JS:   (() => { console.log("run"); })();
来源：http://dzh.ctjpmb.com

TS:   (() => { console.log("run"); })();
来源：http://ssj.guowangkeji.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ugo.smart0.xyz

Go:   func() { fmt.Println("run") }()
来源：http://iml.cqqwz.cn

Ruby: -> { puts "run" }.call
来源：http://eaq.mhx1999.top

C#:   // 无 IIFE：用静态构造函数
来源：http://uny.fktsv.cn

[C13] 类型声明 / 类型注解
来源：http://vcq.sjlbkw.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://msc.nanxuanxn.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xeu.ctjpmb.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://fai.fktsv.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://uzz.ehwqpu.com

Java: int add(int a, int b) { return a + b; }
来源：http://daf.fzhhl.top

Go:   func add(a, b int) int
来源：http://grj.yj202588.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://smf.zdqjudy.top

C#:   int Add(int a, int b) => a + b;
来源：http://mdd.tianlin.xyz

[C14] 泛型函数
来源：http://ouf.yueranfly.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://aux.shuidangran.top

PHP:  // 无泛型
来源：http://chz.tian-w.cn

JS:   // 无泛型
来源：http://kgh.ybcxt.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mfb.hongshengwenyu.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://tsa.jinqigfzy.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://xws.cashguo.top

Ruby: # 无泛型
来源：http://txw.xingfuxueyuan.xyz

C#:   static T First<T>(List<T> items) => items[0];
来源：http://whm.sweek.top

[C15] 解构 / 展开参数
来源：http://hbn.ywan-chungtsiang.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xge.sxryk.cn

PHP:  [$a, $b] = $pair;
来源：http://qzl.vqdsnc.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://lio.snrcjt.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://aaq.jinyuanbaomall.cn

Java: // 无解构
来源：http://mxo.havefunace.top

Go:   // 无解构
来源：http://xaj.jianghu66.top

Ruby: a, b = pair
来源：http://sou.vqdsnc.cn

C#:   var (a, b) = pair;
来源：http://kdc.yonumen.top

[C16] 函数 / 方法重载
来源：http://gel.guowangkeji.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://nvy.fengsongda.top

PHP:  // 无重载
来源：http://bnn.jinqigufen.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://zsp.hfpthk.cn

TS:   // 用联合类型或重载签名声明
来源：http://yvh.gzhubu.top

Java: void f(int a) {}  void f(String a) {}
来源：http://zot.shuidangran.top

Go:   // 无重载：用不同函数名
来源：http://fsq.dashuyun.cn

Ruby: # 无重载：靠动态参数
来源：http://gwj.feifeiyinyue.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://wao.fengsongda.top

================================================================================
来源：http://ljn.guowangkeji.top

D. 数组 / 列表 / 集合
来源：http://rix.bjfxy.top

================================================================================
来源：http://dfq.chenlongwang.top

[D01] 创建数组 / 列表
来源：http://hue.shanyushiyangtech.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://pdw.hesvh.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hyp.jqgufenzy.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://qgj.zdbjq.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://uzz.fanxiaobao.xyz

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://tga.yuanzhike.top

Go:   arr := []int{1, 2, 3}
来源：http://ckm.yueranfly.top

Ruby: arr = [1, 2, 3]
来源：http://mja.zhiwuduotai.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://rlo.jlsjyb.cn

[D02] 追加元素到末尾
来源：http://oit.yfazqb.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ztx.mhx1999.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://yzq.xylfe.cn

JS:   arr.push(4);
来源：http://jtk.nanxuanxn.top

TS:   arr.push(4);
来源：http://tkj.epnwcf.com

Java: list.add(4);
来源：http://yzv.xinyue.icu

Go:   arr = append(arr, 4)
来源：http://ftv.sjlbkw.cn

Ruby: arr << 4; arr.push(5)
来源：http://ehm.andypj.xyz

C#:   list.Add(4);
来源：http://qkq.dashuyun.cn

[D03] 在指定位置插入元素
来源：http://zfe.ctjpmb.com

Py:   arr.insert(0, 0)
来源：http://myy.cashguo.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://qbi.zhengqikj.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://gqn.jiagoushi.top

TS:   arr.splice(0, 0, 0);
来源：http://ggv.xuanzx.com

Java: list.add(0, 0);
来源：http://uck.9152youxi.cn

Go:   arr = append([]int{0}, arr...)
来源：http://isb.zdbjq.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ytc.yj20258888.top

C#:   list.Insert(0, 0);
来源：http://ghl.chenlongwang.top

[D04] 删除元素
来源：http://cwt.fanxiaobao.xyz

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://aqg.quarkkingdee.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://piq.zhoulong.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://kma.daxiang520.top

TS:   arr.splice(0, 1);
来源：http://dta.sufxvd.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://pnq.ctjpmb.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://jyv.hammf.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://khr.xuetiantiany.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://vtc.smart0.xyz

[D05] 访问与修改元素
来源：http://ieu.wangdashe.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hnl.xylfe.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://drt.xuanzx.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://bju.wangdashe.top

TS:   arr[0]; arr.at(-1);
来源：http://nry.shanyushiyangtech.top

Java: list.get(0); list.set(0, 9);
来源：http://qsc.ywan-chungtsiang.top

Go:   arr[0]; arr[0] = 9
来源：http://evu.xingfuxueyuan.xyz

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://pqm.pengpengdd.cyou

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://smz.mhx1999.top

[D06] 数组长度
来源：http://qfu.yongpay.top

Py:   len(arr)
来源：http://ewy.hfpthk.cn

PHP:  count($arr);
来源：http://xvm.aizwys.cn

JS:   arr.length
来源：http://bpd.zhoulong.xyz

TS:   arr.length
来源：http://aud.hcnkem.com

Java: list.size();
来源：http://qyu.dianchejie.cn

Go:   len(arr)
来源：http://ckh.hnqzz.top

Ruby: arr.length; arr.size
来源：http://gba.nwbrower.top

C#:   list.Count;
来源：http://qco.zhengqikj.top

[D07] 切片 / 取子数组
来源：http://izp.zhaomingkeji.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://xgy.meibo888.top

PHP:  array_slice($arr, 1, 3);
来源：http://pkz.hongshengwenyu.top

JS:   arr.slice(1, 4);
来源：http://htm.fengsongda.top

TS:   arr.slice(1, 4);
来源：http://ddl.c1oappe.top

Java: list.subList(1, 4);
来源：http://hpu.xingfuxueyuan.xyz

Go:   arr[1:4]
来源：http://whh.quarkkingdee.top

Ruby: arr[1, 3]
来源：http://lcb.gotoacloud.top

C#:   list.GetRange(1, 3);
来源：http://efx.vqdsnc.cn

[D08] 合并两个数组
来源：http://cej.hammf.cn

Py:   a + b;  a.extend(b)
来源：http://zlr.zdbjq.cn

PHP:  array_merge($a, $b);
来源：http://aro.yueranfly.top

JS:   [...a, ...b];  a.concat(b);
来源：http://fdg.chenjidiqi.icu

TS:   [...a, ...b];
来源：http://lke.zhiwuduotai.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://vwq.yvedp.cn

Go:   append(a, b...)
来源：http://xvi.mhx1999.top

Ruby: a + b;  a.concat(b)
来源：http://mfw.shuidangran.top

C#:   a.Concat(b).ToList()
来源：http://sxm.jinqigufen.top

[D09] 排序（升序）
来源：http://qrn.sxryk.cn

Py:   sorted(arr);  arr.sort()
来源：http://pwg.ehwqpu.com

PHP:  sort($arr);
来源：http://ptp.daxiang520.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://con.hfpthk.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://usq.hammf.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://jyk.shzxlz.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ecf.gaohongyu789.top

Ruby: arr.sort
来源：http://kkr.fehbvm.com

C#:   list.Sort();
来源：http://nqt.guowangkeji.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://ofa.daxiang520.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://jkv.kuanghao11.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ats.jinyuanbaomall.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://vwg.hongshengwenyu.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://qnp.aibaodan.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://jve.cqqwz.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://xbd.smart0.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://txn.pycfn.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hoi.cqqwz.cn

[D11] 反转数组
来源：http://cbc.sysykeji.top

Py:   arr[::-1];  arr.reverse()
来源：http://dhn.sufxvd.cn

PHP:  array_reverse($arr);
来源：http://hvs.gzhubu.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://cqb.snrcjt.cn

TS:   [...arr].reverse();
来源：http://nbf.aizwys.cn

Java: Collections.reverse(list);
来源：http://zea.shanyushiyangtech.top

Go:   slices.Reverse(arr)
来源：http://cdq.kuanghao11.cn

Ruby: arr.reverse
来源：http://pdc.birdmap.top

C#:   list.Reverse();
来源：http://wtx.zdbjq.cn

[D12] 查找元素下标
来源：http://ecc.cdnleiting.top

Py:   arr.index(x);  x in arr
来源：http://wpr.nanxuanxn.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://zko.guannengcc.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mhn.yfazqb.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vfd.chenzaomai.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://oxe.ydzc1.top

Go:   slices.Index(arr, x)
来源：http://esu.yuxming.cn

Ruby: arr.index(x)
来源：http://yrx.nanxinkj.top

C#:   list.IndexOf(x);
来源：http://ukc.chenzaomai.com

[D13] 过滤（保留满足条件的）
来源：http://jax.nwbrower.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://xlj.chenjidiqi.icu

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://lxv.epnwcf.com

JS:   arr.filter(x => x > 3)
来源：http://skw.ivvv.top

TS:   arr.filter(x => x > 3)
来源：http://swo.jinqigufen.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ubc.yvedp.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://otg.yuanzhike.top

Ruby: arr.select { |x| x > 3 }
来源：http://txp.dashuyun.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://qmw.yueranfly.top

[D14] 映射转换（每个元素变形）
来源：http://ojg.cdnleiting.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mot.daria6918.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://lgb.zycfv.cn

JS:   arr.map(x => x * 2)
来源：http://ynw.yfazqb.com

TS:   arr.map(x => x * 2)
来源：http://inu.zhiwuduotai.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://poe.chenzaomai.com

Go:   // 手写循环
来源：http://bgq.zdqjudy.top

Ruby: arr.map { |x| x * 2 }
来源：http://ubq.zhiwuduotai.top

C#:   list.Select(x => x * 2).ToList()
来源：http://ebg.aibaodan.cn

[D15] 去重
来源：http://qaj.vqdsnc.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://fos.9152youxi.cn

PHP:  array_unique($arr);
来源：http://sjn.yanxiufei.cn

JS:   [...new Set(arr)]
来源：http://kae.hywenlv.cn

TS:   [...new Set(arr)]
来源：http://myw.jqgufenzy.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://opc.yvedp.cn

Go:   // 用 map[T]struct{} 手写
来源：http://cqi.yj20258888.top

Ruby: arr.uniq
来源：http://sla.sxryk.cn

C#:   list.Distinct().ToList()
来源：http://bru.yfazqb.com

[D16] 求和与平均值
来源：http://zkg.wangdashe.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://dym.ehwqpu.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ybu.jianghu66.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ajy.cashguo.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://vhl.yuanzhike.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://epn.ydjk.org.cn

Go:   // 手写循环累加
来源：http://bzg.zdbjq.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://vki.zhixingplan.top

C#:   list.Sum();  list.Average()
来源：http://kzp.tian-w.cn

[D17] 最大值与最小值
来源：http://jge.gotoacloud.top

Py:   max(arr);  min(arr)
来源：http://tuc.xylfe.cn

PHP:  max($arr);  min($arr);
来源：http://kji.vehdjk.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://zjt.gogol.net.cn

TS:   Math.max(...arr);
来源：http://wuu.fengsongda.top

Java: Collections.max(list);  Collections.min(list);
来源：http://znq.guannengcc.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://nbv.aizwys.cn

Ruby: arr.max;  arr.min
来源：http://kpt.aibaodan.cn

C#:   list.Max();  list.Min()
来源：http://tak.jinyuanbaomall.cn

[D18] 扁平化嵌套数组
来源：http://pwj.fanxiaobao.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://vbd.yuanzhike.top

PHP:  array_merge(...$nested);
来源：http://xlm.shanyushiyangtech.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://egc.fanxiaobao.xyz

TS:   nested.flat();
来源：http://ggw.zhongyouzk.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jix.quarkkingdee.top

Go:   // 手写双层循环
来源：http://fvc.jiagoushi.top

Ruby: nested.flatten
来源：http://qdh.yj20258.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://pdt.sxryk.cn

[D19] 按字段分组
来源：http://uyk.tianlin.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://vcs.jlsjyb.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://fel.zhoulong.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://tjn.gotoacloud.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://lxa.ivvv.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://drh.jyoumei.cn

Go:   // 手写 map[string][]T
来源：http://mct.yj20258888.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://rac.shangyingyoupin.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://dtt.dianchejie.cn

[D20] 统计每个元素出现次数
来源：http://ewq.shanyushiyangtech.top

Py:   Counter(arr)
来源：http://xkn.daria6918.cn

PHP:  array_count_values($arr);
来源：http://kbq.0kj1m.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://skp.pengpengdd.cyou

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kin.wangshuangyany.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ovz.epnwcf.com

Go:   // 手写 map[T]int
来源：http://xlx.haohaochexian.top

Ruby: arr.tally
来源：http://zgn.xylfe.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://eth.kuanghao11.cn

[D21] 判断是否包含某元素
来源：http://tub.chenzaomai.com

Py:   x in arr
来源：http://ycq.ydzc1.top

PHP:  in_array($x, $arr, true);
来源：http://biz.nanxuanxn.top

JS:   arr.includes(x)
来源：http://lxh.zdbjq.cn

TS:   arr.includes(x)
来源：http://zlv.hywenlv.cn

Java: list.contains(x)
来源：http://eju.havefunace.top

Go:   slices.Contains(arr, x)
来源：http://xcl.fehbvm.com

Ruby: arr.include?(x)
来源：http://nnr.epnwcf.com

C#:   list.Contains(x)
来源：http://xtq.hywenlv.cn

[D22] 复制数组（避免共享引用）
来源：http://fzy.shuidangran.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://kan.redwolf501.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://rhb.chenjidiqi.icu

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://pnb.jinyuanbaomall.cn

TS:   [...arr];
来源：http://qxq.quarkkingdee.top

Java: new ArrayList<>(list);
来源：http://urt.316326.xyz

Go:   copied := append([]int(nil), arr...)
来源：http://wqb.zdbjq.cn

Ruby: arr.dup;  arr.clone
来源：http://lrg.sysykeji.top

C#:   new List<int>(list);
来源：http://yrw.hywenlv.cn


<!-- 参考信息 -->