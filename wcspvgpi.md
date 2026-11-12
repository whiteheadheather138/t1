代发 wailian999

Py:   return a, b
来源：http://dsq.cqqwz.cn

PHP:  return [$a, $b];
来源：http://lgk.hysaishi.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://fjh.tianlin.xyz

TS:   return { a, b };
来源：http://fht.aizwys.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://sld.cdnleiting.top

Go:   return a, b
来源：http://cqn.gaohongyu789.top

Ruby: return a, b
来源：http://pqo.nanxinkj.top

C#:   return (a, b);              // ValueTuple
来源：http://ewr.aibaodan.cn

[C06] 匿名函数 / lambda
来源：http://ssd.dashuyun.cn

Py:   square = lambda x: x * x
来源：http://nqd.chenlongwang.top

PHP:  $square = fn($x) => $x * $x;
来源：http://eqd.cashguo.top

JS:   const square = x => x * x;
来源：http://xus.zhiwuduotai.top

TS:   const square = (x: number): number => x * x;
来源：http://zkq.zdqjudy.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://kpw.zhongyouzk.top

Go:   sq := func(x int) int { return x * x }
来源：http://fro.epnwcf.com

Ruby: square = ->(x) { x * x }
来源：http://qbb.yuxming.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ppv.tian-w.cn

[C07] 把函数作为参数传入
来源：http://hkg.hnqzz.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://oqd.zhongyouzk.top

PHP:  array_map("strtoupper", $arr);
来源：http://keq.shanyushiyangtech.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://vcp.yj20258888.top

TS:   arr.map(String)
来源：http://ltc.shangyingyoupin.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://jyn.aizwys.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hxz.aibaodan.cn

Ruby: arr.map(&:upcase)
来源：http://aet.yuanzhike.top

C#:   arr.Select(s => s.ToUpper())
来源：http://mch.cucudq.cn

[C08] 闭包
来源：http://bvw.hfpthk.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mxc.jinyuanbaomall.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://icz.ydzc1.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qpk.guowangkeji.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://dpt.dianchejie.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://vgq.hfpthk.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://laf.ivvv.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://rmn.sjlbkw.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://dwc.guannengcc.top

[C09] 递归
来源：http://pah.ydzc1.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ker.uphjek.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://jbg.yonumen.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kut.dianchejie.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dtg.daxiang520.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://dth.jqgufenzy.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://sip.sjlbkw.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://kge.haohaochexian.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hdk.zhiwuduotai.top

[C10] 变量作用域
来源：http://zwr.yonumen.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://kdo.dashuyun.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://aof.chenjidiqi.icu

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ydh.sweek.top

TS:   同 JS
来源：http://bsn.dashuyun.cn

Java: 方法内为块级作用域
来源：http://ggh.redwolf501.top

Go:   花括号块级作用域
来源：http://tuc.shanyushiyangkeji.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://rzb.tarul.cn

C#:   块级作用域
来源：http://qum.xylfe.cn

[C11] 模块导入与导出
来源：http://oul.smart0.xyz

Py:   from module import func
来源：http://ekl.zdqjudy.top

PHP:  require "file.php";  或 use App\Service;
来源：http://vtl.chenlongwang.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://tdo.shuidangran.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://vdu.cashguo.top

Java: import java.util.List;
来源：http://cqs.yj202588.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://suf.yfazqb.com

Ruby: require "json"; require_relative "./util"
来源：http://lcc.snrcjt.cn

C#:   using System.Text;
来源：http://rjt.sxryk.cn

[C12] 立即执行函数 IIFE
来源：http://hlq.zycfv.cn

Py:   (lambda: print("run"))()
来源：http://lit.gogol.net.cn

PHP:  (function () { echo "run"; })();
来源：http://cdw.aibaodan.cn

JS:   (() => { console.log("run"); })();
来源：http://qpa.xziqi.cn

TS:   (() => { console.log("run"); })();
来源：http://fmv.zhiwuduotai.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://isa.jlsjyb.cn

Go:   func() { fmt.Println("run") }()
来源：http://wck.svipenyu.cn

Ruby: -> { puts "run" }.call
来源：http://yfk.jinyuanbaomall.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://sgi.tianlin.xyz

[C13] 类型声明 / 类型注解
来源：http://iyr.ivvv.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://oym.jinqigufen.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hth.hnxiangtu.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://uqb.vehdjk.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://esi.yfazqb.com

Java: int add(int a, int b) { return a + b; }
来源：http://sec.epnwcf.com

Go:   func add(a, b int) int
来源：http://znz.tian-w.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://olq.yfazqb.com

C#:   int Add(int a, int b) => a + b;
来源：http://xyv.svipenyu.cn

[C14] 泛型函数
来源：http://imp.52xcode.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://psc.snrcjt.cn

PHP:  // 无泛型
来源：http://wpy.gogol.net.cn

JS:   // 无泛型
来源：http://dpz.quarkkingdee.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://rhx.zdqjudy.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ysa.nwbrower.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://jjm.guannengcc.top

Ruby: # 无泛型
来源：http://zbc.uphjek.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://rfa.bbcook.cn

[C15] 解构 / 展开参数
来源：http://ovn.yonumen.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://lpj.hongshengwenyu.top

PHP:  [$a, $b] = $pair;
来源：http://usy.tanke756.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://beg.smart0.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://yoq.ppjwa.cn

Java: // 无解构
来源：http://rgb.hammf.cn

Go:   // 无解构
来源：http://has.chenzaomai.com

Ruby: a, b = pair
来源：http://hfu.yueranfly.top

C#:   var (a, b) = pair;
来源：http://fra.hnqzz.top

[C16] 函数 / 方法重载
来源：http://jgk.jiagoushi.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://xuc.xylfe.cn

PHP:  // 无重载
来源：http://bse.feifeiyinyue.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://wzg.jinqigfzy.top

TS:   // 用联合类型或重载签名声明
来源：http://dfu.pengpengdd.cyou

Java: void f(int a) {}  void f(String a) {}
来源：http://btr.redwolf501.top

Go:   // 无重载：用不同函数名
来源：http://mxs.guannengcc.top

Ruby: # 无重载：靠动态参数
来源：http://urs.shangyingyoupin.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://eyf.gzhubu.top

================================================================================
来源：http://vgv.jlsjyb.cn

D. 数组 / 列表 / 集合
来源：http://jpu.fzhhl.top

================================================================================
来源：http://wjm.iojbl.cn

[D01] 创建数组 / 列表
来源：http://zfj.yj20258888.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://mry.snrcjt.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://cuh.havefunace.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://msb.shanyushiyangkeji.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://doh.zhijiandao.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ghz.yj20258.top

Go:   arr := []int{1, 2, 3}
来源：http://iiu.bjfxy.top

Ruby: arr = [1, 2, 3]
来源：http://kiu.zdqjudy.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ulx.shangyingyoupin.top

[D02] 追加元素到末尾
来源：http://pto.yueranfly.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://aej.sweek.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://zwm.nanxuanxn.top

JS:   arr.push(4);
来源：http://eck.hcnkem.com

TS:   arr.push(4);
来源：http://ihq.zhengqikj.top

Java: list.add(4);
来源：http://atb.hammf.cn

Go:   arr = append(arr, 4)
来源：http://ksn.xylfe.cn

Ruby: arr << 4; arr.push(5)
来源：http://qtj.jinqigufen.top

C#:   list.Add(4);
来源：http://mhp.wangdashe.top

[D03] 在指定位置插入元素
来源：http://jxo.svipenyu.cn

Py:   arr.insert(0, 0)
来源：http://vgk.tian-w.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://kmv.hammf.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://vrx.yueranfly.top

TS:   arr.splice(0, 0, 0);
来源：http://whe.feifeiyinyue.top

Java: list.add(0, 0);
来源：http://uwl.xuanzx.com

Go:   arr = append([]int{0}, arr...)
来源：http://omv.jqgfzy.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://nwr.zdqjudy.top

C#:   list.Insert(0, 0);
来源：http://wdq.aibaodan.cn

[D04] 删除元素
来源：http://ezw.shzxlz.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://flf.kuanghao11.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://eow.zycfv.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://gho.ctjpmb.com

TS:   arr.splice(0, 1);
来源：http://aff.aibaodan.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://kzd.hnxiangtu.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://pvq.hfpthk.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://xrc.snrcjt.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://fts.yj20258.top

[D05] 访问与修改元素
来源：http://pop.hnqzz.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://anj.sxryk.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://rhv.hywenlv.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://psm.guowangkeji.top

TS:   arr[0]; arr.at(-1);
来源：http://eiv.zdbjq.cn

Java: list.get(0); list.set(0, 9);
来源：http://pwe.ehwqpu.com

Go:   arr[0]; arr[0] = 9
来源：http://zht.yonumen.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://eqg.shanyushiyangtech.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wnm.jyoumei.cn

[D06] 数组长度
来源：http://ybn.ywan-chungtsiang.top

Py:   len(arr)
来源：http://jxx.tanke756.top

PHP:  count($arr);
来源：http://kdb.smart0.xyz

JS:   arr.length
来源：http://bzk.yvedp.cn

TS:   arr.length
来源：http://wdf.jqgufenzy.top

Java: list.size();
来源：http://rxn.jqgufenzy.top

Go:   len(arr)
来源：http://rzp.pengpengdd.cyou

Ruby: arr.length; arr.size
来源：http://fyb.yfazqb.com

C#:   list.Count;
来源：http://rxh.sxryk.cn

[D07] 切片 / 取子数组
来源：http://yyz.jinqigfzy.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://vog.yongpay.top

PHP:  array_slice($arr, 1, 3);
来源：http://jmj.ywan-chungtsiang.top

JS:   arr.slice(1, 4);
来源：http://duq.zhoulong.xyz

TS:   arr.slice(1, 4);
来源：http://nna.nwbrower.top

Java: list.subList(1, 4);
来源：http://fws.jinyuanbaomall.cn

Go:   arr[1:4]
来源：http://jze.kuanghao11.cn

Ruby: arr[1, 3]
来源：http://ezg.ivvv.top

C#:   list.GetRange(1, 3);
来源：http://wxu.shuidangran.top

[D08] 合并两个数组
来源：http://oam.tanke756.top

Py:   a + b;  a.extend(b)
来源：http://jbw.jqgfzy.top

PHP:  array_merge($a, $b);
来源：http://zyg.ehwqpu.com

JS:   [...a, ...b];  a.concat(b);
来源：http://kdk.daria6918.cn

TS:   [...a, ...b];
来源：http://sid.quarkkingdee.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://zfv.hnxiangtu.top

Go:   append(a, b...)
来源：http://zml.jiagoushi.top

Ruby: a + b;  a.concat(b)
来源：http://qqf.xingfuxueyuan.xyz

C#:   a.Concat(b).ToList()
来源：http://wmt.uphjek.com

[D09] 排序（升序）
来源：http://hgn.xingfuxueyuan.xyz

Py:   sorted(arr);  arr.sort()
来源：http://lvj.tianlin.xyz

PHP:  sort($arr);
来源：http://uff.xinyue.icu

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://elm.jlsjyb.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://jcl.yuxming.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://bdj.jlsjyb.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://icg.shzxlz.cn

Ruby: arr.sort
来源：http://eoz.aizwys.cn

C#:   list.Sort();
来源：http://iim.xuetiantiany.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://qur.hcnkem.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://vut.yangfankeji.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://djb.kuanghao11.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://gsn.zdbjq.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://vii.jinqigufen.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://sys.cucudq.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://aey.tarul.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://uvm.redwolf501.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hfd.ivvv.top

[D11] 反转数组
来源：http://emc.fehbvm.com

Py:   arr[::-1];  arr.reverse()
来源：http://rft.tarul.cn

PHP:  array_reverse($arr);
来源：http://lnu.nanxuanxn.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qnd.xinyue.icu

TS:   [...arr].reverse();
来源：http://kdb.jlsjyb.cn

Java: Collections.reverse(list);
来源：http://mwd.316326.xyz

Go:   slices.Reverse(arr)
来源：http://end.zdqjudy.top

Ruby: arr.reverse
来源：http://qdi.zycfv.cn

C#:   list.Reverse();
来源：http://dke.epnwcf.com

[D12] 查找元素下标
来源：http://jrk.yj20258888.top

Py:   arr.index(x);  x in arr
来源：http://uxb.yvedp.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hsy.ppjwa.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://utp.hnqzz.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gsp.daxiang520.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://aib.chenlongwang.top

Go:   slices.Index(arr, x)
来源：http://okf.hcnkem.com

Ruby: arr.index(x)
来源：http://sas.zhixingplan.top

C#:   list.IndexOf(x);
来源：http://kvn.cashguo.top

[D13] 过滤（保留满足条件的）
来源：http://itb.jianghu66.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://euo.wangshuangyany.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://vre.yonumen.top

JS:   arr.filter(x => x > 3)
来源：http://hhh.ywan-chungtsiang.top

TS:   arr.filter(x => x > 3)
来源：http://rcg.haohaochexian.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ujv.birdmap.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://kvl.sjlbkw.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ndh.redwolf501.top

C#:   list.Where(x => x > 3).ToList()
来源：http://obo.hongshengwenyu.top

[D14] 映射转换（每个元素变形）
来源：http://doa.jlsjyb.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://evi.tian-w.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://jpq.yvedp.cn

JS:   arr.map(x => x * 2)
来源：http://fsl.chenlongwang.top

TS:   arr.map(x => x * 2)
来源：http://zer.zycfv.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://kqw.svipenyu.cn

Go:   // 手写循环
来源：http://ine.ybcxt.top

Ruby: arr.map { |x| x * 2 }
来源：http://etb.zycfv.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://plu.haohaochexian.top

[D15] 去重
来源：http://vhx.cdnleiting.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://bvr.sjlbkw.cn

PHP:  array_unique($arr);
来源：http://khb.pengpengdd.cyou

JS:   [...new Set(arr)]
来源：http://blm.zhiwuduotai.top

TS:   [...new Set(arr)]
来源：http://gvj.ctjpmb.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wbg.yonumen.top

Go:   // 用 map[T]struct{} 手写
来源：http://fxt.havefunace.top

Ruby: arr.uniq
来源：http://fvl.cashguo.top

C#:   list.Distinct().ToList()
来源：http://jny.cdnleiting.top

[D16] 求和与平均值
来源：http://fmy.cucudq.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ngs.sjlbkw.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://xva.tanke756.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://dgp.zdbjq.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wjk.bjfxy.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xnz.shanyushiyangtech.top

Go:   // 手写循环累加
来源：http://roe.hfpthk.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://pvt.xuanzx.com

C#:   list.Sum();  list.Average()
来源：http://uuv.feifeiyinyue.top

[D17] 最大值与最小值
来源：http://umz.ywan-chungtsiang.top

Py:   max(arr);  min(arr)
来源：http://idx.haohaochexian.top

PHP:  max($arr);  min($arr);
来源：http://jyv.cheryme.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://xmp.shanyushiyangkeji.top

TS:   Math.max(...arr);
来源：http://tab.jianghu66.top

Java: Collections.max(list);  Collections.min(list);
来源：http://vka.fktsv.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://kpl.xinyue.icu

Ruby: arr.max;  arr.min
来源：http://uqz.hnxiangtu.top

C#:   list.Max();  list.Min()
来源：http://ocq.fengsongda.top

[D18] 扁平化嵌套数组
来源：http://auz.dianchejie.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://dfc.vqdsnc.cn

PHP:  array_merge(...$nested);
来源：http://gti.pengpengdd.cyou

JS:   nested.flat();  nested.flat(Infinity)
来源：http://alw.yonumen.top

TS:   nested.flat();
来源：http://hcp.jianghu66.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ezu.vqdsnc.cn

Go:   // 手写双层循环
来源：http://drp.daxiang520.top

Ruby: nested.flatten
来源：http://pge.ctjpmb.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://tfm.shuidangran.top

[D19] 按字段分组
来源：http://cgx.xuanzx.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://veg.xuetiantiany.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://pky.tian-w.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mur.tarul.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://aij.c1oappe.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://glp.sjlbkw.cn

Go:   // 手写 map[string][]T
来源：http://adp.uphjek.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://npn.xinyue.icu

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wrq.yvedp.cn

[D20] 统计每个元素出现次数
来源：http://wet.yanxiufei.cn

Py:   Counter(arr)
来源：http://iar.feifeiyinyue.top

PHP:  array_count_values($arr);
来源：http://rvz.snrcjt.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hmk.hongshengwenyu.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yno.yangfankeji.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://rlc.yueranfly.top

Go:   // 手写 map[T]int
来源：http://lem.yuanzhike.top

Ruby: arr.tally
来源：http://ubi.yj20258.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mxa.hammf.cn

[D21] 判断是否包含某元素
来源：http://jlk.uphjek.com

Py:   x in arr
来源：http://sqs.yanxiufei.cn

PHP:  in_array($x, $arr, true);
来源：http://csy.yuxming.cn

JS:   arr.includes(x)
来源：http://wmn.sweek.top

TS:   arr.includes(x)
来源：http://zxt.gaohongyu789.top

Java: list.contains(x)
来源：http://lxj.daria6918.cn

Go:   slices.Contains(arr, x)
来源：http://nic.tarul.cn

Ruby: arr.include?(x)
来源：http://mvd.jianghu66.top

C#:   list.Contains(x)
来源：http://oqq.cqqwz.cn

[D22] 复制数组（避免共享引用）
来源：http://ien.nanxuanxn.top


<!-- 参考信息 -->