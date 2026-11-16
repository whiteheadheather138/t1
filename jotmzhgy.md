代发 wailian999

Py:   return a, b
来源：http://joz.wangdashe.top

PHP:  return [$a, $b];
来源：http://eoh.jyoumei.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://yfn.iojbl.cn

TS:   return { a, b };
来源：http://bdi.cucudq.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://zjm.jlsjyb.cn

Go:   return a, b
来源：http://afl.hcnkem.com

Ruby: return a, b
来源：http://uyp.gogol.net.cn

C#:   return (a, b);              // ValueTuple
来源：http://nuy.ydzc1.top

[C06] 匿名函数 / lambda
来源：http://jqo.fzhhl.top

Py:   square = lambda x: x * x
来源：http://dfi.xuetiantiany.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://qyf.ybcxt.top

JS:   const square = x => x * x;
来源：http://xsv.quarkkingdee.top

TS:   const square = (x: number): number => x * x;
来源：http://oju.cdnleiting.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://veh.xuetiantiany.cn

Go:   sq := func(x int) int { return x * x }
来源：http://erf.0kj1m.cn

Ruby: square = ->(x) { x * x }
来源：http://qbe.zhijiandao.cn

C#:   Func<int, int> square = x => x * x;
来源：http://bjl.fanxiaobao.xyz

[C07] 把函数作为参数传入
来源：http://ktm.jlsjyb.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://pcq.zhiwuduotai.top

PHP:  array_map("strtoupper", $arr);
来源：http://cte.zdbjq.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://tic.zhixingplan.top

TS:   arr.map(String)
来源：http://rvb.wangdashe.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://jre.xuanzx.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mtl.dianchejie.cn

Ruby: arr.map(&:upcase)
来源：http://yiz.hfpthk.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://fhk.shuidangran.top

[C08] 闭包
来源：http://fug.epnwcf.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://uwu.vehdjk.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://goh.jiagoushi.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qft.yonumen.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://szz.c1oappe.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ezy.guannengcc.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://gaa.jqgufenzy.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://apq.fktsv.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://qzu.bbcook.cn

[C09] 递归
来源：http://kco.316326.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qbj.nanxuanxn.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://gnz.fzhhl.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fug.xingfuxueyuan.xyz

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pin.dianchejie.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://rdd.jinghuilouyu.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mfb.zhoulong.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://bdf.pengpengdd.cyou

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://yxi.xziqi.cn

[C10] 变量作用域
来源：http://gek.jinqigfzy.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://stu.yuxming.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://udw.xuetiantiany.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://erw.fzhhl.top

TS:   同 JS
来源：http://fcj.tianlin.xyz

Java: 方法内为块级作用域
来源：http://gmv.cucudq.cn

Go:   花括号块级作用域
来源：http://nkl.dashuyun.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://vsp.cdnleiting.top

C#:   块级作用域
来源：http://epz.uphjek.com

[C11] 模块导入与导出
来源：http://apu.fktsv.cn

Py:   from module import func
来源：http://ucx.52xcode.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://xma.aizwys.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://inh.fzhhl.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://pid.zhijiandao.cn

Java: import java.util.List;
来源：http://nxm.jianghu66.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://fuy.wangshuangyany.cn

Ruby: require "json"; require_relative "./util"
来源：http://snb.hywenlv.cn

C#:   using System.Text;
来源：http://zlj.cheryme.top

[C12] 立即执行函数 IIFE
来源：http://oaw.c1oappe.top

Py:   (lambda: print("run"))()
来源：http://wak.gaohongyu789.top

PHP:  (function () { echo "run"; })();
来源：http://yht.shanyushiyangtech.top

JS:   (() => { console.log("run"); })();
来源：http://sxh.yuanzhike.top

TS:   (() => { console.log("run"); })();
来源：http://jyp.jinghuilouyu.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wyx.yanxiufei.cn

Go:   func() { fmt.Println("run") }()
来源：http://egq.jinqigfzy.top

Ruby: -> { puts "run" }.call
来源：http://igd.vqdsnc.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://isf.guannengcc.top

[C13] 类型声明 / 类型注解
来源：http://wpo.sxryk.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://pel.cdnleiting.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://faa.nanxuanxn.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://sop.tanke756.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baa.9152youxi.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ump.jianghu66.top

Go:   func add(a, b int) int
来源：http://sdb.guannengcc.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://rlw.vehdjk.com

C#:   int Add(int a, int b) => a + b;
来源：http://lst.yuanzhike.top

[C14] 泛型函数
来源：http://wij.gzhubu.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://for.havefunace.top

PHP:  // 无泛型
来源：http://tpx.fzhhl.top

JS:   // 无泛型
来源：http://krj.jqgfzy.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://etd.cqqwz.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ekz.yuanzhike.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://dyp.yanxiufei.cn

Ruby: # 无泛型
来源：http://lfc.chenjidiqi.icu

C#:   static T First<T>(List<T> items) => items[0];
来源：http://sjs.yfazqb.com

[C15] 解构 / 展开参数
来源：http://mtv.nwbrower.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mxl.bjfxy.top

PHP:  [$a, $b] = $pair;
来源：http://xqv.xylfe.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hcw.fehbvm.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://dnh.cashguo.top

Java: // 无解构
来源：http://eeq.jlsjyb.cn

Go:   // 无解构
来源：http://urh.gogol.net.cn

Ruby: a, b = pair
来源：http://hzg.xingfuxueyuan.xyz

C#:   var (a, b) = pair;
来源：http://mya.9152youxi.cn

[C16] 函数 / 方法重载
来源：http://qua.vehdjk.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vwo.nwbrower.top

PHP:  // 无重载
来源：http://yaw.jinqigufen.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://xjt.hnqzz.top

TS:   // 用联合类型或重载签名声明
来源：http://jeo.jianghu66.top

Java: void f(int a) {}  void f(String a) {}
来源：http://sgw.smart0.xyz

Go:   // 无重载：用不同函数名
来源：http://jgj.xuetiantiany.cn

Ruby: # 无重载：靠动态参数
来源：http://bxq.gzhubu.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://lwp.epnwcf.com

================================================================================
来源：http://rto.epnwcf.com

D. 数组 / 列表 / 集合
来源：http://hcn.svipenyu.cn

================================================================================
来源：http://san.tianlin.xyz

[D01] 创建数组 / 列表
来源：http://jfc.shanyushiyangkeji.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://vcf.316326.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://tmu.fengsongda.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://tmz.hongshengwenyu.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://suj.ydjk.org.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wkc.aizwys.cn

Go:   arr := []int{1, 2, 3}
来源：http://std.jinghuilouyu.cn

Ruby: arr = [1, 2, 3]
来源：http://kyx.cheryme.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://pgz.xuanzx.com

[D02] 追加元素到末尾
来源：http://gam.xylfe.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://gvq.birdmap.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://kzb.cheryme.top

JS:   arr.push(4);
来源：http://cvj.jinqigufen.top

TS:   arr.push(4);
来源：http://gvf.jiagoushi.top

Java: list.add(4);
来源：http://ccq.yonumen.top

Go:   arr = append(arr, 4)
来源：http://ntl.sjlbkw.cn

Ruby: arr << 4; arr.push(5)
来源：http://gdm.yj20258888.top

C#:   list.Add(4);
来源：http://jze.ppjwa.cn

[D03] 在指定位置插入元素
来源：http://gpu.shuidangran.top

Py:   arr.insert(0, 0)
来源：http://vqd.shanyushiyangkeji.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://rsq.9152youxi.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://gzv.gzhubu.top

TS:   arr.splice(0, 0, 0);
来源：http://nxe.xuanzx.com

Java: list.add(0, 0);
来源：http://pdh.yj20258888.top

Go:   arr = append([]int{0}, arr...)
来源：http://tau.chenjidiqi.icu

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://coi.gotoacloud.top

C#:   list.Insert(0, 0);
来源：http://web.nanxuanxn.top

[D04] 删除元素
来源：http://syc.hcnkem.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mqn.mhx1999.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://fxh.nanxuanxn.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://car.zhongyouzk.top

TS:   arr.splice(0, 1);
来源：http://iht.nanxinkj.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wtu.yonumen.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wml.hnxiangtu.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://xba.zdbjq.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://nuz.vehdjk.com

[D05] 访问与修改元素
来源：http://nhl.cucudq.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://xmt.dianchejie.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wwb.shzxlz.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://tin.shzxlz.cn

TS:   arr[0]; arr.at(-1);
来源：http://toc.haohaochexian.top

Java: list.get(0); list.set(0, 9);
来源：http://xmx.yueranfly.top

Go:   arr[0]; arr[0] = 9
来源：http://mxi.aibaodan.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://lbv.nwbrower.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ldw.c1oappe.top

[D06] 数组长度
来源：http://uvc.hesvh.cn

Py:   len(arr)
来源：http://kxn.sjlbkw.cn

PHP:  count($arr);
来源：http://gks.hywenlv.cn

JS:   arr.length
来源：http://rbr.ybcxt.top

TS:   arr.length
来源：http://kmn.gogol.net.cn

Java: list.size();
来源：http://yqp.birdmap.top

Go:   len(arr)
来源：http://yda.tianlin.xyz

Ruby: arr.length; arr.size
来源：http://fnx.shuidangran.top

C#:   list.Count;
来源：http://jdu.zhengqikj.top

[D07] 切片 / 取子数组
来源：http://kpd.xuanzx.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://vte.316326.xyz

PHP:  array_slice($arr, 1, 3);
来源：http://sah.yj202588.top

JS:   arr.slice(1, 4);
来源：http://cqk.yuanzhike.top

TS:   arr.slice(1, 4);
来源：http://zte.uphjek.com

Java: list.subList(1, 4);
来源：http://pks.wangshuangyany.cn

Go:   arr[1:4]
来源：http://yeq.ybcxt.top

Ruby: arr[1, 3]
来源：http://vzw.zhengqikj.top

C#:   list.GetRange(1, 3);
来源：http://udx.bbcook.cn

[D08] 合并两个数组
来源：http://hjd.bbcook.cn

Py:   a + b;  a.extend(b)
来源：http://pna.bjfxy.top

PHP:  array_merge($a, $b);
来源：http://cqa.shuidangran.top

JS:   [...a, ...b];  a.concat(b);
来源：http://ehb.smart0.xyz

TS:   [...a, ...b];
来源：http://dbu.hnxiangtu.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://vez.jyoumei.cn

Go:   append(a, b...)
来源：http://jwc.fanxiaobao.xyz

Ruby: a + b;  a.concat(b)
来源：http://wqv.ivvv.top

C#:   a.Concat(b).ToList()
来源：http://cpf.tanke756.top

[D09] 排序（升序）
来源：http://nzi.fzhhl.top

Py:   sorted(arr);  arr.sort()
来源：http://wmz.sxryk.cn

PHP:  sort($arr);
来源：http://uzh.zhiwuduotai.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://xjx.wangdashe.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://tnd.mhx1999.top

Java: Collections.sort(list);  list.sort(null);
来源：http://xxo.guannengcc.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://shw.cdnleiting.top

Ruby: arr.sort
来源：http://rnq.vqdsnc.cn

C#:   list.Sort();
来源：http://uuo.xylfe.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://luv.ydzc1.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://iol.zhijiandao.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://paf.jiagoushi.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://iyx.yvedp.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://tlx.dianchejie.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://coe.xingfuxueyuan.xyz

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://osu.hysaishi.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://onp.xinyue.icu

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://cek.pycfn.com

[D11] 反转数组
来源：http://xnt.cqqwz.cn

Py:   arr[::-1];  arr.reverse()
来源：http://mqw.yj202588.top

PHP:  array_reverse($arr);
来源：http://bzu.316326.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://prz.bbcook.cn

TS:   [...arr].reverse();
来源：http://ssx.yuxming.cn

Java: Collections.reverse(list);
来源：http://wdf.uphjek.com

Go:   slices.Reverse(arr)
来源：http://nht.316326.xyz

Ruby: arr.reverse
来源：http://wef.yongpay.top

C#:   list.Reverse();
来源：http://eot.havefunace.top

[D12] 查找元素下标
来源：http://fmb.fktsv.cn

Py:   arr.index(x);  x in arr
来源：http://biv.gzhubu.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ilw.yvedp.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fim.jinghuilouyu.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ecm.tian-w.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://grp.shangyingyoupin.top

Go:   slices.Index(arr, x)
来源：http://vmt.fengsongda.top

Ruby: arr.index(x)
来源：http://nuf.zhaomingkeji.xyz

C#:   list.IndexOf(x);
来源：http://cks.vehdjk.com

[D13] 过滤（保留满足条件的）
来源：http://lof.zhijiandao.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://rgg.pengpengdd.cyou

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://jee.dianchejie.cn

JS:   arr.filter(x => x > 3)
来源：http://woo.birdmap.top

TS:   arr.filter(x => x > 3)
来源：http://usz.hongshengwenyu.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://iqz.vehdjk.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://aos.vqdsnc.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ouq.zycfv.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://uea.quarkkingdee.top

[D14] 映射转换（每个元素变形）
来源：http://kjm.zhaomingkeji.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wps.fzhhl.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://aef.aibaodan.cn

JS:   arr.map(x => x * 2)
来源：http://oxj.jyoumei.cn

TS:   arr.map(x => x * 2)
来源：http://qcm.xinyue.icu

Java: list.stream().map(x -> x * 2).toList()
来源：http://cfh.hammf.cn

Go:   // 手写循环
来源：http://qky.yueranfly.top

Ruby: arr.map { |x| x * 2 }
来源：http://cqq.gaohongyu789.top

C#:   list.Select(x => x * 2).ToList()
来源：http://hhn.mhx1999.top

[D15] 去重
来源：http://cci.jinyuanbaomall.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://got.sxryk.cn

PHP:  array_unique($arr);
来源：http://oqg.sjlbkw.cn

JS:   [...new Set(arr)]
来源：http://iuk.jinghuilouyu.cn

TS:   [...new Set(arr)]
来源：http://oce.yonumen.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://fkf.cucudq.cn

Go:   // 用 map[T]struct{} 手写
来源：http://umf.shanyushiyangtech.top

Ruby: arr.uniq
来源：http://nch.haohaochexian.top

C#:   list.Distinct().ToList()
来源：http://kva.hnqzz.top

[D16] 求和与平均值
来源：http://oir.andypj.xyz

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://klp.hcnkem.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://vde.hysaishi.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://glw.nwbrower.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ecs.hnxiangtu.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://rog.cqqwz.cn

Go:   // 手写循环累加
来源：http://nrq.xingfuxueyuan.xyz

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://eyq.fanxiaobao.xyz

C#:   list.Sum();  list.Average()
来源：http://smm.pycfn.com

[D17] 最大值与最小值
来源：http://jyq.chenzaomai.com

Py:   max(arr);  min(arr)
来源：http://fme.zhongyouzk.top

PHP:  max($arr);  min($arr);
来源：http://vuq.zhengqikj.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mmd.ydzc1.top

TS:   Math.max(...arr);
来源：http://ewh.yangfankeji.com

Java: Collections.max(list);  Collections.min(list);
来源：http://avp.ehwqpu.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://umg.dashuyun.cn

Ruby: arr.max;  arr.min
来源：http://quh.xuanzx.com

C#:   list.Max();  list.Min()
来源：http://tdg.zdbjq.cn

[D18] 扁平化嵌套数组
来源：http://hjn.tarul.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://tal.cashguo.top

PHP:  array_merge(...$nested);
来源：http://vsb.jinqigufen.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://jkf.fehbvm.com

TS:   nested.flat();
来源：http://ltb.zhixingplan.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://gms.cqqwz.cn

Go:   // 手写双层循环
来源：http://ddy.cdnleiting.top

Ruby: nested.flatten
来源：http://rml.jqgufenzy.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://lws.vehdjk.com

[D19] 按字段分组
来源：http://pka.daria6918.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://qks.yj20258.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://fin.shanyushiyangtech.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://epc.jiagoushi.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://htp.xingfuxueyuan.xyz

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wpx.gogol.net.cn

Go:   // 手写 map[string][]T
来源：http://bbk.chenlongwang.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://ncn.chenjidiqi.icu

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://bav.9152youxi.cn

[D20] 统计每个元素出现次数
来源：http://pjz.0kj1m.cn

Py:   Counter(arr)
来源：http://uuz.smart0.xyz

PHP:  array_count_values($arr);
来源：http://xvc.ybcxt.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dxi.sysykeji.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wqg.xziqi.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://qvu.zhoulong.xyz

Go:   // 手写 map[T]int
来源：http://cxk.pycfn.com

Ruby: arr.tally
来源：http://mga.ctjpmb.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://jvp.gaohongyu789.top

[D21] 判断是否包含某元素
来源：http://ceg.ydjk.org.cn

Py:   x in arr
来源：http://sfy.9152youxi.cn

PHP:  in_array($x, $arr, true);
来源：http://gzz.fehbvm.com

JS:   arr.includes(x)
来源：http://pmj.xingfuxueyuan.xyz

TS:   arr.includes(x)
来源：http://pgz.0kj1m.cn

Java: list.contains(x)
来源：http://qpv.gzhubu.top

Go:   slices.Contains(arr, x)
来源：http://ioe.birdmap.top

Ruby: arr.include?(x)
来源：http://bhe.tarul.cn

C#:   list.Contains(x)
来源：http://qgi.yj202588.top

[D22] 复制数组（避免共享引用）
来源：http://mau.52xcode.cn


<!-- 参考信息 -->