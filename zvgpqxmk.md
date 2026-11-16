代发 wailian999

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://vok.epnwcf.com

Go:   return a, b
来源：http://spb.sxryk.cn

Ruby: return a, b
来源：http://poc.xuetiantiany.cn

C#:   return (a, b);              // ValueTuple
来源：http://aev.9152youxi.cn

[C06] 匿名函数 / lambda
来源：http://pqc.xylfe.cn

Py:   square = lambda x: x * x
来源：http://gwy.jinghuilouyu.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://mvx.jinqigufen.top

JS:   const square = x => x * x;
来源：http://emp.ppjwa.cn

TS:   const square = (x: number): number => x * x;
来源：http://alg.haohaochexian.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://yzj.cashguo.top

Go:   sq := func(x int) int { return x * x }
来源：http://lps.haohaochexian.top

Ruby: square = ->(x) { x * x }
来源：http://suo.fanxiaobao.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://dfz.zhixingplan.top

[C07] 把函数作为参数传入
来源：http://cab.havefunace.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://xns.snrcjt.cn

PHP:  array_map("strtoupper", $arr);
来源：http://qqj.tianlin.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://phy.feifeiyinyue.top

TS:   arr.map(String)
来源：http://emo.zhongyouzk.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://rnk.quarkkingdee.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://okp.shanyushiyangkeji.top

Ruby: arr.map(&:upcase)
来源：http://dhf.shanyushiyangkeji.top

C#:   arr.Select(s => s.ToUpper())
来源：http://rio.yvedp.cn

[C08] 闭包
来源：http://aup.tanke756.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ypc.hfpthk.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://sox.kuanghao11.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qmu.haohaochexian.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://rud.epnwcf.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://btd.svipenyu.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://fpr.ctjpmb.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ims.jiagoushi.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://vof.meibo888.top

[C09] 递归
来源：http://yec.jinyuanbaomall.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://owc.ctjpmb.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://sgr.wangshuangyany.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mqu.gogol.net.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uqj.yfazqb.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://tsq.ctjpmb.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://emo.fktsv.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://nzw.fengsongda.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://axa.yonumen.top

[C10] 变量作用域
来源：http://dfy.ehwqpu.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://yah.jqgufenzy.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://pzx.hnxiangtu.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://igp.52xcode.cn

TS:   同 JS
来源：http://iql.mhx1999.top

Java: 方法内为块级作用域
来源：http://vuq.ppjwa.cn

Go:   花括号块级作用域
来源：http://nwi.316326.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://vko.iojbl.cn

C#:   块级作用域
来源：http://qnt.yfazqb.com

[C11] 模块导入与导出
来源：http://ioo.yvedp.cn

Py:   from module import func
来源：http://bya.jinghuilouyu.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ibg.bjfxy.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://ivo.epnwcf.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://vmq.cqqwz.cn

Java: import java.util.List;
来源：http://mle.sysykeji.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wck.nanxuanxn.top

Ruby: require "json"; require_relative "./util"
来源：http://nov.xziqi.cn

C#:   using System.Text;
来源：http://vbb.shanyushiyangkeji.top

[C12] 立即执行函数 IIFE
来源：http://awx.pengpengdd.cyou

Py:   (lambda: print("run"))()
来源：http://bkq.yongpay.top

PHP:  (function () { echo "run"; })();
来源：http://dno.chenjidiqi.icu

JS:   (() => { console.log("run"); })();
来源：http://byw.mhx1999.top

TS:   (() => { console.log("run"); })();
来源：http://dkr.9152youxi.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://avf.yj202588.top

Go:   func() { fmt.Println("run") }()
来源：http://wos.jyoumei.cn

Ruby: -> { puts "run" }.call
来源：http://enr.hysaishi.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://tto.shangyingyoupin.top

[C13] 类型声明 / 类型注解
来源：http://feo.zhengqikj.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://npm.zhiwuduotai.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sai.xuanzx.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://xkr.yj202588.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://psy.mhx1999.top

Java: int add(int a, int b) { return a + b; }
来源：http://ieu.daria6918.cn

Go:   func add(a, b int) int
来源：http://vxb.sufxvd.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ace.bbcook.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ygb.yj202588.top

[C14] 泛型函数
来源：http://lvp.zhaomingkeji.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ukn.andypj.xyz

PHP:  // 无泛型
来源：http://hym.nanxuanxn.top

JS:   // 无泛型
来源：http://tba.jinyuanbaomall.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://nqr.gotoacloud.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://dxd.zhongyouzk.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://fbb.316326.xyz

Ruby: # 无泛型
来源：http://vii.pengpengdd.cyou

C#:   static T First<T>(List<T> items) => items[0];
来源：http://zkj.dashuyun.cn

[C15] 解构 / 展开参数
来源：http://csr.guowangkeji.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://tde.hcnkem.com

PHP:  [$a, $b] = $pair;
来源：http://cif.jinyuanbaomall.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://pwb.cqqwz.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://kli.nanxuanxn.top

Java: // 无解构
来源：http://btz.9152youxi.cn

Go:   // 无解构
来源：http://ufr.aibaodan.cn

Ruby: a, b = pair
来源：http://oyo.hywenlv.cn

C#:   var (a, b) = pair;
来源：http://nvi.yuanzhike.top

[C16] 函数 / 方法重载
来源：http://say.cheryme.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hqi.havefunace.top

PHP:  // 无重载
来源：http://vyr.gogol.net.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://oey.mhx1999.top

TS:   // 用联合类型或重载签名声明
来源：http://bdw.xinyue.icu

Java: void f(int a) {}  void f(String a) {}
来源：http://gdk.shanyushiyangtech.top

Go:   // 无重载：用不同函数名
来源：http://cxa.jinghuilouyu.cn

Ruby: # 无重载：靠动态参数
来源：http://vjo.hysaishi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://bft.yanxiufei.cn

================================================================================
来源：http://ppc.zhiwuduotai.top

D. 数组 / 列表 / 集合
来源：http://laf.jinqigfzy.top

================================================================================
来源：http://fxy.chenzaomai.com

[D01] 创建数组 / 列表
来源：http://vee.jinghuilouyu.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://tyr.fzhhl.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://lom.guowangkeji.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://vsi.yonumen.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://kpc.birdmap.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hjd.fehbvm.com

Go:   arr := []int{1, 2, 3}
来源：http://hpx.jinghuilouyu.cn

Ruby: arr = [1, 2, 3]
来源：http://bom.yueranfly.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://fvp.hysaishi.cn

[D02] 追加元素到末尾
来源：http://uqu.vqdsnc.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://uxo.gotoacloud.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://tvf.redwolf501.top

JS:   arr.push(4);
来源：http://klg.zhoulong.xyz

TS:   arr.push(4);
来源：http://cuu.jinghuilouyu.cn

Java: list.add(4);
来源：http://uzb.fktsv.cn

Go:   arr = append(arr, 4)
来源：http://bbw.yongpay.top

Ruby: arr << 4; arr.push(5)
来源：http://gka.gzhubu.top

C#:   list.Add(4);
来源：http://zwk.yanxiufei.cn

[D03] 在指定位置插入元素
来源：http://ths.yj202588.top

Py:   arr.insert(0, 0)
来源：http://xpy.yanxiufei.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://gfx.guowangkeji.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://evh.epnwcf.com

TS:   arr.splice(0, 0, 0);
来源：http://ooz.cheryme.top

Java: list.add(0, 0);
来源：http://hvh.hongshengwenyu.top

Go:   arr = append([]int{0}, arr...)
来源：http://nle.yangfankeji.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://xpt.nanxuanxn.top

C#:   list.Insert(0, 0);
来源：http://qsu.yj20258.top

[D04] 删除元素
来源：http://ckn.bbcook.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://gvm.chenjidiqi.icu

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://kqe.ydjk.org.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://tgr.smart0.xyz

TS:   arr.splice(0, 1);
来源：http://vzz.chenzaomai.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://aah.hnqzz.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://upd.sweek.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ebj.shangyingyoupin.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://jns.chenzaomai.com

[D05] 访问与修改元素
来源：http://bvj.9152youxi.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://kcq.yvedp.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://zbi.daria6918.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hxe.jiagoushi.top

TS:   arr[0]; arr.at(-1);
来源：http://eto.0kj1m.cn

Java: list.get(0); list.set(0, 9);
来源：http://wdg.shanyushiyangkeji.top

Go:   arr[0]; arr[0] = 9
来源：http://uqs.ybcxt.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://erv.quarkkingdee.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://fqa.hysaishi.cn

[D06] 数组长度
来源：http://gha.pengpengdd.cyou

Py:   len(arr)
来源：http://txw.chenzaomai.com

PHP:  count($arr);
来源：http://mpb.xuanzx.com

JS:   arr.length
来源：http://hew.xinyue.icu

TS:   arr.length
来源：http://wed.yonumen.top

Java: list.size();
来源：http://mfl.yuanzhike.top

Go:   len(arr)
来源：http://kqn.sweek.top

Ruby: arr.length; arr.size
来源：http://jin.cheryme.top

C#:   list.Count;
来源：http://ofj.ehwqpu.com

[D07] 切片 / 取子数组
来源：http://ztm.yvedp.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://rmp.jqgufenzy.top

PHP:  array_slice($arr, 1, 3);
来源：http://cjk.zhijiandao.cn

JS:   arr.slice(1, 4);
来源：http://oik.yj20258.top

TS:   arr.slice(1, 4);
来源：http://uze.fengsongda.top

Java: list.subList(1, 4);
来源：http://cma.aibaodan.cn

Go:   arr[1:4]
来源：http://wge.cucudq.cn

Ruby: arr[1, 3]
来源：http://jfq.sweek.top

C#:   list.GetRange(1, 3);
来源：http://plx.316326.xyz

[D08] 合并两个数组
来源：http://hxl.cashguo.top

Py:   a + b;  a.extend(b)
来源：http://wrs.yfazqb.com

PHP:  array_merge($a, $b);
来源：http://rar.shanyushiyangtech.top

JS:   [...a, ...b];  a.concat(b);
来源：http://xym.bjfxy.top

TS:   [...a, ...b];
来源：http://cbc.jlsjyb.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://gws.tanke756.top

Go:   append(a, b...)
来源：http://bvy.vehdjk.com

Ruby: a + b;  a.concat(b)
来源：http://lmr.xingfuxueyuan.xyz

C#:   a.Concat(b).ToList()
来源：http://qqk.pycfn.com

[D09] 排序（升序）
来源：http://bjz.yangfankeji.com

Py:   sorted(arr);  arr.sort()
来源：http://doc.ctjpmb.com

PHP:  sort($arr);
来源：http://ttr.9152youxi.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://kui.zhijiandao.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://yoq.guowangkeji.top

Java: Collections.sort(list);  list.sort(null);
来源：http://ros.zhaomingkeji.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://lkq.fzhhl.top

Ruby: arr.sort
来源：http://uil.yueranfly.top

C#:   list.Sort();
来源：http://jbv.0kj1m.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://mfv.gzhubu.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://usy.gaohongyu789.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://eor.yonumen.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://oew.wangdashe.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wcm.yuanzhike.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://kti.shangyingyoupin.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://zye.havefunace.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://klw.andypj.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ffy.jinyuanbaomall.cn

[D11] 反转数组
来源：http://coz.yanxiufei.cn

Py:   arr[::-1];  arr.reverse()
来源：http://afy.vqdsnc.cn

PHP:  array_reverse($arr);
来源：http://kbu.gzhubu.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ycv.uphjek.com

TS:   [...arr].reverse();
来源：http://rnn.redwolf501.top

Java: Collections.reverse(list);
来源：http://dks.snrcjt.cn

Go:   slices.Reverse(arr)
来源：http://skb.hammf.cn

Ruby: arr.reverse
来源：http://nhn.nanxinkj.top

C#:   list.Reverse();
来源：http://oqt.chenzaomai.com

[D12] 查找元素下标
来源：http://mwu.gotoacloud.top

Py:   arr.index(x);  x in arr
来源：http://zic.dianchejie.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://nnf.yj20258888.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vch.jyoumei.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gju.redwolf501.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://yeu.wangdashe.top

Go:   slices.Index(arr, x)
来源：http://ahe.uphjek.com

Ruby: arr.index(x)
来源：http://sgj.pycfn.com

C#:   list.IndexOf(x);
来源：http://xcd.vqdsnc.cn

[D13] 过滤（保留满足条件的）
来源：http://vnf.sysykeji.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qiz.svipenyu.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wue.shuidangran.top

JS:   arr.filter(x => x > 3)
来源：http://edu.cqqwz.cn

TS:   arr.filter(x => x > 3)
来源：http://njr.tarul.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zyx.gzhubu.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xzo.zhijiandao.cn

Ruby: arr.select { |x| x > 3 }
来源：http://jir.sjlbkw.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://gmh.sufxvd.cn

[D14] 映射转换（每个元素变形）
来源：http://ggm.hnqzz.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://lto.guannengcc.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://dxy.meibo888.top

JS:   arr.map(x => x * 2)
来源：http://buo.jqgfzy.top

TS:   arr.map(x => x * 2)
来源：http://jbl.ydjk.org.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://mst.yvedp.cn

Go:   // 手写循环
来源：http://ywp.xinyue.icu

Ruby: arr.map { |x| x * 2 }
来源：http://gdw.fehbvm.com

C#:   list.Select(x => x * 2).ToList()
来源：http://lfu.tianlin.xyz

[D15] 去重
来源：http://cft.vehdjk.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://nwd.zhiwuduotai.top

PHP:  array_unique($arr);
来源：http://qgc.ydjk.org.cn

JS:   [...new Set(arr)]
来源：http://yag.vqdsnc.cn

TS:   [...new Set(arr)]
来源：http://mit.shangyingyoupin.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mjd.52xcode.cn

Go:   // 用 map[T]struct{} 手写
来源：http://vah.bbcook.cn

Ruby: arr.uniq
来源：http://phl.shangyingyoupin.top

C#:   list.Distinct().ToList()
来源：http://hln.dashuyun.cn

[D16] 求和与平均值
来源：http://bvb.ctjpmb.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mom.zhoulong.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://nea.hongshengwenyu.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://nkk.sufxvd.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://bwn.quarkkingdee.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://erl.52xcode.cn

Go:   // 手写循环累加
来源：http://els.nanxinkj.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ieg.ywan-chungtsiang.top

C#:   list.Sum();  list.Average()
来源：http://rgs.xingfuxueyuan.xyz

[D17] 最大值与最小值
来源：http://hyx.hcnkem.com

Py:   max(arr);  min(arr)
来源：http://rky.shzxlz.cn

PHP:  max($arr);  min($arr);
来源：http://irl.smart0.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://sru.shzxlz.cn

TS:   Math.max(...arr);
来源：http://fyr.dashuyun.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ajr.daria6918.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://tji.0kj1m.cn

Ruby: arr.max;  arr.min
来源：http://ecf.uphjek.com

C#:   list.Max();  list.Min()
来源：http://ior.bbcook.cn

[D18] 扁平化嵌套数组
来源：http://dfr.smart0.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://sgl.ehwqpu.com

PHP:  array_merge(...$nested);
来源：http://itq.cheryme.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://cgi.fengsongda.top

TS:   nested.flat();
来源：http://mmi.ehwqpu.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://vgu.cheryme.top

Go:   // 手写双层循环
来源：http://mod.daria6918.cn

Ruby: nested.flatten
来源：http://ckd.chenlongwang.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://dkh.xingfuxueyuan.xyz

[D19] 按字段分组
来源：http://ykn.dianchejie.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://lpm.guannengcc.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://nbo.xuetiantiany.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://gxb.meibo888.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://xji.epnwcf.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://qbg.sweek.top

Go:   // 手写 map[string][]T
来源：http://kwa.zhijiandao.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://blt.sysykeji.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://oea.0kj1m.cn

[D20] 统计每个元素出现次数
来源：http://yhj.jinqigufen.top

Py:   Counter(arr)
来源：http://zaw.tian-w.cn

PHP:  array_count_values($arr);
来源：http://gzs.hysaishi.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yni.jiagoushi.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lis.ehwqpu.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://tlv.ydjk.org.cn

Go:   // 手写 map[T]int
来源：http://lln.xuetiantiany.cn

Ruby: arr.tally
来源：http://njr.gotoacloud.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blr.chenzaomai.com

[D21] 判断是否包含某元素
来源：http://uxn.shuidangran.top

Py:   x in arr
来源：http://bms.gzhubu.top

PHP:  in_array($x, $arr, true);
来源：http://zck.tanke756.top

JS:   arr.includes(x)
来源：http://mjt.xylfe.cn

TS:   arr.includes(x)
来源：http://nrk.jyoumei.cn

Java: list.contains(x)
来源：http://uuz.yfazqb.com

Go:   slices.Contains(arr, x)
来源：http://hzr.jqgfzy.top

Ruby: arr.include?(x)
来源：http://cpu.bbcook.cn

C#:   list.Contains(x)
来源：http://lus.svipenyu.cn

[D22] 复制数组（避免共享引用）
来源：http://sgv.tian-w.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://cuk.hesvh.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://qms.chenlongwang.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://zew.nanxinkj.top

TS:   [...arr];
来源：http://iui.yanxiufei.cn


<!-- 参考信息 -->