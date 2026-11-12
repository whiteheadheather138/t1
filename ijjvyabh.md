代发 wailian999

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://lfq.iojbl.cn

Go:   return a, b
来源：http://kdj.wangshuangyany.cn

Ruby: return a, b
来源：http://obl.bbcook.cn

C#:   return (a, b);              // ValueTuple
来源：http://xki.zhiwuduotai.top

[C06] 匿名函数 / lambda
来源：http://fyx.haohaochexian.top

Py:   square = lambda x: x * x
来源：http://rnc.mhx1999.top

PHP:  $square = fn($x) => $x * $x;
来源：http://zft.zhoulong.xyz

JS:   const square = x => x * x;
来源：http://nto.ydjk.org.cn

TS:   const square = (x: number): number => x * x;
来源：http://ynr.cqqwz.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://gmr.svipenyu.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ozl.sxryk.cn

Ruby: square = ->(x) { x * x }
来源：http://kos.chenlongwang.top

C#:   Func<int, int> square = x => x * x;
来源：http://uis.ivvv.top

[C07] 把函数作为参数传入
来源：http://nyq.ctjpmb.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://cqa.gaohongyu789.top

PHP:  array_map("strtoupper", $arr);
来源：http://ydb.xuanzx.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://jyg.zdbjq.cn

TS:   arr.map(String)
来源：http://zly.yuanzhike.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://nrt.yj202588.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://oui.ehwqpu.com

Ruby: arr.map(&:upcase)
来源：http://kix.zycfv.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ndx.zhiwuduotai.top

[C08] 闭包
来源：http://ngy.uphjek.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://kyl.redwolf501.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://dqc.shuidangran.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ngz.jqgufenzy.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hht.ivvv.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://pso.wangshuangyany.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://aiu.fehbvm.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://uga.hnxiangtu.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://eae.yanxiufei.cn

[C09] 递归
来源：http://xph.shanyushiyangkeji.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://obf.chenzaomai.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://dci.hnqzz.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://oib.smart0.xyz

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ghm.bbcook.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ajw.nwbrower.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://dne.sjlbkw.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://jda.cucudq.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://cbb.vqdsnc.cn

[C10] 变量作用域
来源：http://iox.yueranfly.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://lix.meibo888.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://vul.feifeiyinyue.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://asc.xylfe.cn

TS:   同 JS
来源：http://aot.chenzaomai.com

Java: 方法内为块级作用域
来源：http://sai.redwolf501.top

Go:   花括号块级作用域
来源：http://rdb.wangdashe.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://urj.hnxiangtu.top

C#:   块级作用域
来源：http://qnw.havefunace.top

[C11] 模块导入与导出
来源：http://ubj.sysykeji.top

Py:   from module import func
来源：http://gha.havefunace.top

PHP:  require "file.php";  或 use App\Service;
来源：http://wwd.yangfankeji.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://eqm.feifeiyinyue.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://jzg.yonumen.top

Java: import java.util.List;
来源：http://ntq.ppjwa.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://xdr.yangfankeji.com

Ruby: require "json"; require_relative "./util"
来源：http://vyq.tianlin.xyz

C#:   using System.Text;
来源：http://yew.andypj.xyz

[C12] 立即执行函数 IIFE
来源：http://cwu.ywan-chungtsiang.top

Py:   (lambda: print("run"))()
来源：http://nog.haohaochexian.top

PHP:  (function () { echo "run"; })();
来源：http://epn.hammf.cn

JS:   (() => { console.log("run"); })();
来源：http://fbd.ehwqpu.com

TS:   (() => { console.log("run"); })();
来源：http://clc.shzxlz.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://gsx.nwbrower.top

Go:   func() { fmt.Println("run") }()
来源：http://mpv.haohaochexian.top

Ruby: -> { puts "run" }.call
来源：http://xqf.zycfv.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://njs.guannengcc.top

[C13] 类型声明 / 类型注解
来源：http://upz.smart0.xyz

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ggm.shanyushiyangkeji.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zfw.yongpay.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://pxs.shanyushiyangtech.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yha.jqgfzy.top

Java: int add(int a, int b) { return a + b; }
来源：http://iyr.tian-w.cn

Go:   func add(a, b int) int
来源：http://odn.xuetiantiany.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://gtb.zhongyouzk.top

C#:   int Add(int a, int b) => a + b;
来源：http://caq.smart0.xyz

[C14] 泛型函数
来源：http://ksm.daxiang520.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://bve.pycfn.com

PHP:  // 无泛型
来源：http://qje.snrcjt.cn

JS:   // 无泛型
来源：http://icm.aibaodan.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://dbh.sweek.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://lvk.jinqigufen.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://xov.yangfankeji.com

Ruby: # 无泛型
来源：http://rzk.cqqwz.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wlu.sxryk.cn

[C15] 解构 / 展开参数
来源：http://pok.zdbjq.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://jxh.zycfv.cn

PHP:  [$a, $b] = $pair;
来源：http://ulc.bbcook.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://leh.jiagoushi.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://xph.cqqwz.cn

Java: // 无解构
来源：http://lvr.ehwqpu.com

Go:   // 无解构
来源：http://zin.havefunace.top

Ruby: a, b = pair
来源：http://rtf.sweek.top

C#:   var (a, b) = pair;
来源：http://ajl.xylfe.cn

[C16] 函数 / 方法重载
来源：http://wmr.yangfankeji.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://jtz.feifeiyinyue.top

PHP:  // 无重载
来源：http://yqi.cdnleiting.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://luh.ybcxt.top

TS:   // 用联合类型或重载签名声明
来源：http://eet.gaohongyu789.top

Java: void f(int a) {}  void f(String a) {}
来源：http://bgy.fktsv.cn

Go:   // 无重载：用不同函数名
来源：http://odg.havefunace.top

Ruby: # 无重载：靠动态参数
来源：http://tww.wangdashe.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://fsy.zhongyouzk.top

================================================================================
来源：http://kux.tian-w.cn

D. 数组 / 列表 / 集合
来源：http://stb.meibo888.top

================================================================================
来源：http://gmu.guowangkeji.top

[D01] 创建数组 / 列表
来源：http://hem.jlsjyb.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://zzb.yuxming.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hul.jianghu66.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://vpe.gzhubu.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://nor.vqdsnc.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://bqg.shanyushiyangtech.top

Go:   arr := []int{1, 2, 3}
来源：http://mum.yuxming.cn

Ruby: arr = [1, 2, 3]
来源：http://rji.hesvh.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://bfg.hnxiangtu.top

[D02] 追加元素到末尾
来源：http://piy.fzhhl.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://sfr.smart0.xyz

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://vsh.jyoumei.cn

JS:   arr.push(4);
来源：http://pwn.c1oappe.top

TS:   arr.push(4);
来源：http://jft.daxiang520.top

Java: list.add(4);
来源：http://kvy.aibaodan.cn

Go:   arr = append(arr, 4)
来源：http://tgh.chenzaomai.com

Ruby: arr << 4; arr.push(5)
来源：http://eqg.shangyingyoupin.top

C#:   list.Add(4);
来源：http://isv.shuidangran.top

[D03] 在指定位置插入元素
来源：http://wxh.jinghuilouyu.cn

Py:   arr.insert(0, 0)
来源：http://dvk.shanyushiyangkeji.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://tzo.guannengcc.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ysx.shanyushiyangkeji.top

TS:   arr.splice(0, 0, 0);
来源：http://qxc.mhx1999.top

Java: list.add(0, 0);
来源：http://lhy.redwolf501.top

Go:   arr = append([]int{0}, arr...)
来源：http://eeb.jinghuilouyu.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://sqm.0kj1m.cn

C#:   list.Insert(0, 0);
来源：http://nok.hammf.cn

[D04] 删除元素
来源：http://ioi.zdbjq.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://csd.yueranfly.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ozq.zhiwuduotai.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://efc.nanxuanxn.top

TS:   arr.splice(0, 1);
来源：http://osx.ywan-chungtsiang.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://shk.shzxlz.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://jxr.mhx1999.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://bag.ppjwa.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://exa.yonumen.top

[D05] 访问与修改元素
来源：http://pga.pengpengdd.cyou

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://dqf.pengpengdd.cyou

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://iwe.aibaodan.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://zio.yj202588.top

TS:   arr[0]; arr.at(-1);
来源：http://nsf.chenlongwang.top

Java: list.get(0); list.set(0, 9);
来源：http://kca.sweek.top

Go:   arr[0]; arr[0] = 9
来源：http://wyi.jinqigufen.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://sac.bbcook.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://lhi.hnxiangtu.top

[D06] 数组长度
来源：http://kzo.daria6918.cn

Py:   len(arr)
来源：http://tqs.jlsjyb.cn

PHP:  count($arr);
来源：http://qvt.iojbl.cn

JS:   arr.length
来源：http://okh.svipenyu.cn

TS:   arr.length
来源：http://pzp.52xcode.cn

Java: list.size();
来源：http://jnw.fehbvm.com

Go:   len(arr)
来源：http://wwz.ydzc1.top

Ruby: arr.length; arr.size
来源：http://uty.dianchejie.cn

C#:   list.Count;
来源：http://ftr.hfpthk.cn

[D07] 切片 / 取子数组
来源：http://xkm.hesvh.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://jrj.hnxiangtu.top

PHP:  array_slice($arr, 1, 3);
来源：http://giv.zhengqikj.top

JS:   arr.slice(1, 4);
来源：http://fvd.zhongyouzk.top

TS:   arr.slice(1, 4);
来源：http://npx.ctjpmb.com

Java: list.subList(1, 4);
来源：http://mzk.zycfv.cn

Go:   arr[1:4]
来源：http://psq.zdqjudy.top

Ruby: arr[1, 3]
来源：http://lyq.ybcxt.top

C#:   list.GetRange(1, 3);
来源：http://gnq.zhixingplan.top

[D08] 合并两个数组
来源：http://too.svipenyu.cn

Py:   a + b;  a.extend(b)
来源：http://ihs.52xcode.cn

PHP:  array_merge($a, $b);
来源：http://kmd.hnxiangtu.top

JS:   [...a, ...b];  a.concat(b);
来源：http://dup.ehwqpu.com

TS:   [...a, ...b];
来源：http://gvd.c1oappe.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mih.bjfxy.top

Go:   append(a, b...)
来源：http://iij.ydzc1.top

Ruby: a + b;  a.concat(b)
来源：http://avg.bjfxy.top

C#:   a.Concat(b).ToList()
来源：http://bnl.cashguo.top

[D09] 排序（升序）
来源：http://sdq.jinyuanbaomall.cn

Py:   sorted(arr);  arr.sort()
来源：http://xid.jyoumei.cn

PHP:  sort($arr);
来源：http://hkn.shangyingyoupin.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ndn.nanxinkj.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://unh.vqdsnc.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://mdu.zhaomingkeji.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://eir.wangshuangyany.cn

Ruby: arr.sort
来源：http://zoq.guannengcc.top

C#:   list.Sort();
来源：http://epz.yj20258888.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://aug.cdnleiting.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ihl.c1oappe.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kmg.52xcode.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://meo.yuanzhike.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fii.yueranfly.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://rnb.9152youxi.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mdn.yanxiufei.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://kcd.cashguo.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://owc.hnxiangtu.top

[D11] 反转数组
来源：http://cwp.shanyushiyangtech.top

Py:   arr[::-1];  arr.reverse()
来源：http://iuw.guannengcc.top

PHP:  array_reverse($arr);
来源：http://kzs.sufxvd.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hmn.ehwqpu.com

TS:   [...arr].reverse();
来源：http://ucj.iojbl.cn

Java: Collections.reverse(list);
来源：http://psh.jinghuilouyu.cn

Go:   slices.Reverse(arr)
来源：http://uyu.vqdsnc.cn

Ruby: arr.reverse
来源：http://bhz.ybcxt.top

C#:   list.Reverse();
来源：http://kcn.zhengqikj.top

[D12] 查找元素下标
来源：http://her.c1oappe.top

Py:   arr.index(x);  x in arr
来源：http://sdy.xuanzx.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://acc.sweek.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://etx.tianlin.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://skt.andypj.xyz

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://glr.sufxvd.cn

Go:   slices.Index(arr, x)
来源：http://fmz.chenjidiqi.icu

Ruby: arr.index(x)
来源：http://gfy.yj202588.top

C#:   list.IndexOf(x);
来源：http://qih.shzxlz.cn

[D13] 过滤（保留满足条件的）
来源：http://jgj.havefunace.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://cqi.sxryk.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://opk.guowangkeji.top

JS:   arr.filter(x => x > 3)
来源：http://jlf.52xcode.cn

TS:   arr.filter(x => x > 3)
来源：http://hep.sweek.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://aoh.mhx1999.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://muf.tanke756.top

Ruby: arr.select { |x| x > 3 }
来源：http://nzx.hammf.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://nwu.guowangkeji.top

[D14] 映射转换（每个元素变形）
来源：http://vfz.guannengcc.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://gej.hcnkem.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://nzv.shuidangran.top

JS:   arr.map(x => x * 2)
来源：http://ggy.yanxiufei.cn

TS:   arr.map(x => x * 2)
来源：http://ndh.gogol.net.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://aba.shuidangran.top

Go:   // 手写循环
来源：http://nxo.yanxiufei.cn

Ruby: arr.map { |x| x * 2 }
来源：http://kgc.ywan-chungtsiang.top

C#:   list.Select(x => x * 2).ToList()
来源：http://znb.ydzc1.top

[D15] 去重
来源：http://zkz.xingfuxueyuan.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ybm.aizwys.cn

PHP:  array_unique($arr);
来源：http://vgn.hnxiangtu.top

JS:   [...new Set(arr)]
来源：http://wuo.jinghuilouyu.cn

TS:   [...new Set(arr)]
来源：http://tob.svipenyu.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://uvc.0kj1m.cn

Go:   // 用 map[T]struct{} 手写
来源：http://gvn.ppjwa.cn

Ruby: arr.uniq
来源：http://gdo.shuidangran.top

C#:   list.Distinct().ToList()
来源：http://wfo.cqqwz.cn

[D16] 求和与平均值
来源：http://hvx.sufxvd.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://tvm.sjlbkw.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://gsu.xuanzx.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://juq.xuanzx.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://fxv.yfazqb.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://sab.yanxiufei.cn

Go:   // 手写循环累加
来源：http://uuj.bbcook.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://jyl.snrcjt.cn

C#:   list.Sum();  list.Average()
来源：http://pwo.chenzaomai.com

[D17] 最大值与最小值
来源：http://mvq.cashguo.top

Py:   max(arr);  min(arr)
来源：http://cid.0kj1m.cn

PHP:  max($arr);  min($arr);
来源：http://jum.jinqigfzy.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://xda.zhiwuduotai.top

TS:   Math.max(...arr);
来源：http://emj.jiagoushi.top

Java: Collections.max(list);  Collections.min(list);
来源：http://gvi.jqgfzy.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://tiu.shzxlz.cn

Ruby: arr.max;  arr.min
来源：http://rzd.vehdjk.com

C#:   list.Max();  list.Min()
来源：http://ymo.sxryk.cn

[D18] 扁平化嵌套数组
来源：http://zhe.hcnkem.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ply.hysaishi.cn

PHP:  array_merge(...$nested);
来源：http://ezd.tian-w.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://kkb.fzhhl.top

TS:   nested.flat();
来源：http://bzm.hnqzz.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://qen.pycfn.com

Go:   // 手写双层循环
来源：http://wqc.jqgufenzy.top

Ruby: nested.flatten
来源：http://yib.zhengqikj.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://nhu.fanxiaobao.xyz

[D19] 按字段分组
来源：http://hsd.tarul.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hkc.fanxiaobao.xyz

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://jve.tian-w.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://rsg.xinyue.icu

TS:   Object.groupBy(arr, x => x.type)
来源：http://xvn.haohaochexian.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://arj.yangfankeji.com

Go:   // 手写 map[string][]T
来源：http://tjk.meibo888.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://aie.xuanzx.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://knj.dianchejie.cn

[D20] 统计每个元素出现次数
来源：http://lds.daria6918.cn

Py:   Counter(arr)
来源：http://lro.shangyingyoupin.top

PHP:  array_count_values($arr);
来源：http://jbm.sufxvd.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bpu.uphjek.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cni.sweek.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://oad.fktsv.cn

Go:   // 手写 map[T]int
来源：http://fax.fanxiaobao.xyz

Ruby: arr.tally
来源：http://rhj.vqdsnc.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://vpn.vqdsnc.cn

[D21] 判断是否包含某元素
来源：http://lgg.xuetiantiany.cn

Py:   x in arr
来源：http://amv.jiagoushi.top

PHP:  in_array($x, $arr, true);
来源：http://uzg.ehwqpu.com

JS:   arr.includes(x)
来源：http://nfd.hnqzz.top

TS:   arr.includes(x)
来源：http://rtz.fehbvm.com

Java: list.contains(x)
来源：http://hyj.vqdsnc.cn

Go:   slices.Contains(arr, x)
来源：http://mcz.hnxiangtu.top

Ruby: arr.include?(x)
来源：http://ybh.yj20258888.top

C#:   list.Contains(x)
来源：http://sqv.meibo888.top

[D22] 复制数组（避免共享引用）
来源：http://tpw.c1oappe.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mpj.gogol.net.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://iqd.ywan-chungtsiang.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hbn.ybcxt.top

TS:   [...arr];
来源：http://lpa.xingfuxueyuan.xyz


<!-- 参考信息 -->