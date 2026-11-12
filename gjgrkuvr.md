代发 wailian999

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ghs.snrcjt.cn

Go:   return a, b
来源：http://pxb.zycfv.cn

Ruby: return a, b
来源：http://xcz.yuanzhike.top

C#:   return (a, b);              // ValueTuple
来源：http://izt.ivvv.top

[C06] 匿名函数 / lambda
来源：http://iay.jqgfzy.top

Py:   square = lambda x: x * x
来源：http://dct.meibo888.top

PHP:  $square = fn($x) => $x * $x;
来源：http://smh.vehdjk.com

JS:   const square = x => x * x;
来源：http://tbp.sysykeji.top

TS:   const square = (x: number): number => x * x;
来源：http://lar.shanyushiyangtech.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ccq.gogol.net.cn

Go:   sq := func(x int) int { return x * x }
来源：http://hlu.9152youxi.cn

Ruby: square = ->(x) { x * x }
来源：http://gdp.pycfn.com

C#:   Func<int, int> square = x => x * x;
来源：http://ywe.xylfe.cn

[C07] 把函数作为参数传入
来源：http://ijk.jianghu66.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://geq.yvedp.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ddv.chenlongwang.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://qpp.jinyuanbaomall.cn

TS:   arr.map(String)
来源：http://mys.shanyushiyangtech.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://imp.fzhhl.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://vjp.jinghuilouyu.cn

Ruby: arr.map(&:upcase)
来源：http://zan.tianlin.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://ouh.shzxlz.cn

[C08] 闭包
来源：http://ztu.yvedp.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://zja.cashguo.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wfl.daria6918.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://dsa.bjfxy.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://roq.jiagoushi.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://jfq.dianchejie.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://zyd.shanyushiyangtech.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://zbw.tanke756.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wrl.sxryk.cn

[C09] 递归
来源：http://iiy.sjlbkw.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hse.zycfv.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://zwl.kuanghao11.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qok.ivvv.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://oft.ppjwa.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://bcg.hywenlv.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://vep.tarul.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://nxr.iojbl.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://fdd.cqqwz.cn

[C10] 变量作用域
来源：http://nln.ctjpmb.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://lmi.tian-w.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://iym.aizwys.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://vsv.yfazqb.com

TS:   同 JS
来源：http://soc.zdbjq.cn

Java: 方法内为块级作用域
来源：http://uzh.zycfv.cn

Go:   花括号块级作用域
来源：http://tlq.xuetiantiany.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wup.yangfankeji.com

C#:   块级作用域
来源：http://dmf.hnqzz.top

[C11] 模块导入与导出
来源：http://jom.guowangkeji.top

Py:   from module import func
来源：http://qtc.dashuyun.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://cqa.jinqigfzy.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://mmy.hysaishi.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ikq.shuidangran.top

Java: import java.util.List;
来源：http://txf.wangdashe.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hdm.bbcook.cn

Ruby: require "json"; require_relative "./util"
来源：http://yzc.cucudq.cn

C#:   using System.Text;
来源：http://glj.hcnkem.com

[C12] 立即执行函数 IIFE
来源：http://aaf.yangfankeji.com

Py:   (lambda: print("run"))()
来源：http://mae.dashuyun.cn

PHP:  (function () { echo "run"; })();
来源：http://hxn.zhaomingkeji.xyz

JS:   (() => { console.log("run"); })();
来源：http://mig.zycfv.cn

TS:   (() => { console.log("run"); })();
来源：http://bqy.xuanzx.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ctg.aibaodan.cn

Go:   func() { fmt.Println("run") }()
来源：http://cmr.zhaomingkeji.xyz

Ruby: -> { puts "run" }.call
来源：http://nvf.jyoumei.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://hik.xziqi.cn

[C13] 类型声明 / 类型注解
来源：http://amz.jinqigfzy.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://qle.mhx1999.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bdz.quarkkingdee.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://dzq.aibaodan.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zzp.tanke756.top

Java: int add(int a, int b) { return a + b; }
来源：http://syd.shangyingyoupin.top

Go:   func add(a, b int) int
来源：http://dyp.aizwys.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://nhq.jianghu66.top

C#:   int Add(int a, int b) => a + b;
来源：http://vte.jinghuilouyu.cn

[C14] 泛型函数
来源：http://mzm.316326.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ggw.ywan-chungtsiang.top

PHP:  // 无泛型
来源：http://hux.shzxlz.cn

JS:   // 无泛型
来源：http://vbq.zhijiandao.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://uer.bbcook.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://srm.mhx1999.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://oqb.jinghuilouyu.cn

Ruby: # 无泛型
来源：http://hdj.gzhubu.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://amj.chenjidiqi.icu

[C15] 解构 / 展开参数
来源：http://hyz.fehbvm.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://tzl.feifeiyinyue.top

PHP:  [$a, $b] = $pair;
来源：http://uvd.aibaodan.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://fem.jiagoushi.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://dyw.jinghuilouyu.cn

Java: // 无解构
来源：http://xzb.cheryme.top

Go:   // 无解构
来源：http://qmc.gzhubu.top

Ruby: a, b = pair
来源：http://msp.zdqjudy.top

C#:   var (a, b) = pair;
来源：http://hgb.zhoulong.xyz

[C16] 函数 / 方法重载
来源：http://xjy.vqdsnc.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://qev.316326.xyz

PHP:  // 无重载
来源：http://kow.aibaodan.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://dsi.yfazqb.com

TS:   // 用联合类型或重载签名声明
来源：http://yxd.yangfankeji.com

Java: void f(int a) {}  void f(String a) {}
来源：http://oay.shanyushiyangtech.top

Go:   // 无重载：用不同函数名
来源：http://eig.jinqigfzy.top

Ruby: # 无重载：靠动态参数
来源：http://znv.xziqi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://opo.xinyue.icu

================================================================================
来源：http://vhg.xingfuxueyuan.xyz

D. 数组 / 列表 / 集合
来源：http://rwt.dashuyun.cn

================================================================================
来源：http://qjp.tianlin.xyz

[D01] 创建数组 / 列表
来源：http://pez.hfpthk.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://efg.vqdsnc.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://kij.fzhhl.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://fgd.yj20258888.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://dpj.haohaochexian.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://inj.jinghuilouyu.cn

Go:   arr := []int{1, 2, 3}
来源：http://cuv.tarul.cn

Ruby: arr = [1, 2, 3]
来源：http://etf.sweek.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://myi.ywan-chungtsiang.top

[D02] 追加元素到末尾
来源：http://dkm.snrcjt.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wtn.hnxiangtu.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://jyg.haohaochexian.top

JS:   arr.push(4);
来源：http://tnv.yvedp.cn

TS:   arr.push(4);
来源：http://gus.c1oappe.top

Java: list.add(4);
来源：http://fiy.ywan-chungtsiang.top

Go:   arr = append(arr, 4)
来源：http://kfs.jinghuilouyu.cn

Ruby: arr << 4; arr.push(5)
来源：http://psb.shanyushiyangtech.top

C#:   list.Add(4);
来源：http://kpg.tianlin.xyz

[D03] 在指定位置插入元素
来源：http://sxl.fengsongda.top

Py:   arr.insert(0, 0)
来源：http://zvm.fanxiaobao.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mib.yueranfly.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://fnq.guannengcc.top

TS:   arr.splice(0, 0, 0);
来源：http://shs.bbcook.cn

Java: list.add(0, 0);
来源：http://pnw.hysaishi.cn

Go:   arr = append([]int{0}, arr...)
来源：http://xpm.nanxinkj.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://sxc.sweek.top

C#:   list.Insert(0, 0);
来源：http://ydm.andypj.xyz

[D04] 删除元素
来源：http://mlk.guannengcc.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://dxs.yueranfly.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://jjr.sjlbkw.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://dnn.fanxiaobao.xyz

TS:   arr.splice(0, 1);
来源：http://qni.vehdjk.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://swu.ydzc1.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://lqc.andypj.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://cub.sweek.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://nff.9152youxi.cn

[D05] 访问与修改元素
来源：http://lhj.zhixingplan.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://yxs.daxiang520.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://uxa.kuanghao11.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ctj.0kj1m.cn

TS:   arr[0]; arr.at(-1);
来源：http://ygb.cdnleiting.top

Java: list.get(0); list.set(0, 9);
来源：http://vkl.ydzc1.top

Go:   arr[0]; arr[0] = 9
来源：http://tcb.tanke756.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ypo.cashguo.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ven.gaohongyu789.top

[D06] 数组长度
来源：http://msp.fanxiaobao.xyz

Py:   len(arr)
来源：http://aul.tanke756.top

PHP:  count($arr);
来源：http://qcw.hammf.cn

JS:   arr.length
来源：http://xio.shanyushiyangtech.top

TS:   arr.length
来源：http://pre.pycfn.com

Java: list.size();
来源：http://zyr.ydjk.org.cn

Go:   len(arr)
来源：http://lat.hysaishi.cn

Ruby: arr.length; arr.size
来源：http://qhs.sufxvd.cn

C#:   list.Count;
来源：http://szp.zhaomingkeji.xyz

[D07] 切片 / 取子数组
来源：http://bdb.cdnleiting.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://kwo.feifeiyinyue.top

PHP:  array_slice($arr, 1, 3);
来源：http://wez.shanyushiyangkeji.top

JS:   arr.slice(1, 4);
来源：http://ojd.wangshuangyany.cn

TS:   arr.slice(1, 4);
来源：http://icc.uphjek.com

Java: list.subList(1, 4);
来源：http://myd.vehdjk.com

Go:   arr[1:4]
来源：http://thl.zdqjudy.top

Ruby: arr[1, 3]
来源：http://rik.zhengqikj.top

C#:   list.GetRange(1, 3);
来源：http://vrd.andypj.xyz

[D08] 合并两个数组
来源：http://bpt.yangfankeji.com

Py:   a + b;  a.extend(b)
来源：http://wak.yongpay.top

PHP:  array_merge($a, $b);
来源：http://ide.bbcook.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://rpl.birdmap.top

TS:   [...a, ...b];
来源：http://dbl.aizwys.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ews.guowangkeji.top

Go:   append(a, b...)
来源：http://lwq.nanxuanxn.top

Ruby: a + b;  a.concat(b)
来源：http://qev.sjlbkw.cn

C#:   a.Concat(b).ToList()
来源：http://tas.epnwcf.com

[D09] 排序（升序）
来源：http://wvd.uphjek.com

Py:   sorted(arr);  arr.sort()
来源：http://gya.andypj.xyz

PHP:  sort($arr);
来源：http://jna.52xcode.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://fli.ctjpmb.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://rif.gzhubu.top

Java: Collections.sort(list);  list.sort(null);
来源：http://nja.xuetiantiany.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://oow.shuidangran.top

Ruby: arr.sort
来源：http://pps.zhongyouzk.top

C#:   list.Sort();
来源：http://fni.meibo888.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://tfz.hcnkem.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qby.tian-w.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lbv.feifeiyinyue.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://bhw.pycfn.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fvh.svipenyu.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://iqk.ppjwa.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://qra.hammf.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://bor.tian-w.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://rkg.jqgufenzy.top

[D11] 反转数组
来源：http://jwd.meibo888.top

Py:   arr[::-1];  arr.reverse()
来源：http://eno.yonumen.top

PHP:  array_reverse($arr);
来源：http://xns.uphjek.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://tnl.jqgufenzy.top

TS:   [...arr].reverse();
来源：http://hen.wangshuangyany.cn

Java: Collections.reverse(list);
来源：http://zwj.ivvv.top

Go:   slices.Reverse(arr)
来源：http://dcs.sufxvd.cn

Ruby: arr.reverse
来源：http://pxy.yuxming.cn

C#:   list.Reverse();
来源：http://aes.tarul.cn

[D12] 查找元素下标
来源：http://spi.316326.xyz

Py:   arr.index(x);  x in arr
来源：http://bvh.aizwys.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://rcq.jqgufenzy.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ycr.ydzc1.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sna.mhx1999.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ypp.havefunace.top

Go:   slices.Index(arr, x)
来源：http://zyw.kuanghao11.cn

Ruby: arr.index(x)
来源：http://tiq.sweek.top

C#:   list.IndexOf(x);
来源：http://rse.hongshengwenyu.top

[D13] 过滤（保留满足条件的）
来源：http://ikr.jianghu66.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mii.sjlbkw.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://kms.cheryme.top

JS:   arr.filter(x => x > 3)
来源：http://diq.epnwcf.com

TS:   arr.filter(x => x > 3)
来源：http://nic.shangyingyoupin.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://rue.ydzc1.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ymm.birdmap.top

Ruby: arr.select { |x| x > 3 }
来源：http://dqz.tianlin.xyz

C#:   list.Where(x => x > 3).ToList()
来源：http://atb.aizwys.cn

[D14] 映射转换（每个元素变形）
来源：http://mem.havefunace.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ofm.pengpengdd.cyou

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://rji.fzhhl.top

JS:   arr.map(x => x * 2)
来源：http://bzg.yj202588.top

TS:   arr.map(x => x * 2)
来源：http://uzj.c1oappe.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://yfq.yongpay.top

Go:   // 手写循环
来源：http://hfp.hywenlv.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ydx.yj202588.top

C#:   list.Select(x => x * 2).ToList()
来源：http://kxs.tarul.cn

[D15] 去重
来源：http://hrp.hesvh.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mmf.jyoumei.cn

PHP:  array_unique($arr);
来源：http://woe.guannengcc.top

JS:   [...new Set(arr)]
来源：http://qbq.daria6918.cn

TS:   [...new Set(arr)]
来源：http://jmp.yfazqb.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hpq.jinqigufen.top

Go:   // 用 map[T]struct{} 手写
来源：http://oae.xuanzx.com

Ruby: arr.uniq
来源：http://bpm.quarkkingdee.top

C#:   list.Distinct().ToList()
来源：http://rbb.fzhhl.top

[D16] 求和与平均值
来源：http://jrc.yonumen.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ynf.aibaodan.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://dxf.dianchejie.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://abf.sufxvd.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ryq.yvedp.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://aoe.gzhubu.top

Go:   // 手写循环累加
来源：http://ilu.sweek.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://vdw.zycfv.cn

C#:   list.Sum();  list.Average()
来源：http://opk.hammf.cn

[D17] 最大值与最小值
来源：http://mfp.daria6918.cn

Py:   max(arr);  min(arr)
来源：http://nsd.ydzc1.top

PHP:  max($arr);  min($arr);
来源：http://pan.vehdjk.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://etx.xinyue.icu

TS:   Math.max(...arr);
来源：http://egm.52xcode.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://rpc.gzhubu.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ilz.guowangkeji.top

Ruby: arr.max;  arr.min
来源：http://qse.fehbvm.com

C#:   list.Max();  list.Min()
来源：http://rnq.yvedp.cn

[D18] 扁平化嵌套数组
来源：http://ptr.wangshuangyany.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://keb.chenlongwang.top

PHP:  array_merge(...$nested);
来源：http://jrn.feifeiyinyue.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hdi.birdmap.top

TS:   nested.flat();
来源：http://ttf.zdqjudy.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://gvd.xylfe.cn

Go:   // 手写双层循环
来源：http://pfw.chenjidiqi.icu

Ruby: nested.flatten
来源：http://jxp.yuxming.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://isj.meibo888.top

[D19] 按字段分组
来源：http://zic.shzxlz.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://nmj.jqgufenzy.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ktx.yj20258.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://nth.cqqwz.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://mnf.ctjpmb.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://xjw.zhengqikj.top

Go:   // 手写 map[string][]T
来源：http://fiz.daria6918.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://hwh.shzxlz.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ofg.zycfv.cn

[D20] 统计每个元素出现次数
来源：http://uhs.jianghu66.top

Py:   Counter(arr)
来源：http://wth.yuanzhike.top

PHP:  array_count_values($arr);
来源：http://sex.sufxvd.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hlz.shzxlz.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gal.c1oappe.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://aua.yangfankeji.com

Go:   // 手写 map[T]int
来源：http://qqv.zycfv.cn

Ruby: arr.tally
来源：http://tqm.sxryk.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://vrj.gzhubu.top

[D21] 判断是否包含某元素
来源：http://lhr.hongshengwenyu.top

Py:   x in arr
来源：http://thh.quarkkingdee.top

PHP:  in_array($x, $arr, true);
来源：http://gos.pengpengdd.cyou

JS:   arr.includes(x)
来源：http://ghr.yj202588.top

TS:   arr.includes(x)
来源：http://jbq.yuanzhike.top

Java: list.contains(x)
来源：http://kcc.ydjk.org.cn

Go:   slices.Contains(arr, x)
来源：http://zrz.dianchejie.cn

Ruby: arr.include?(x)
来源：http://nef.fzhhl.top

C#:   list.Contains(x)
来源：http://nkp.ppjwa.cn

[D22] 复制数组（避免共享引用）
来源：http://dsf.tianlin.xyz

Py:   arr.copy();  arr[:];  list(arr)
来源：http://euz.cucudq.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://lun.xylfe.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://edb.xylfe.cn

TS:   [...arr];
来源：http://siy.aizwys.cn


<!-- 参考信息 -->