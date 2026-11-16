代发 wailian999

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ehz.epnwcf.com

Go:   return a, b
来源：http://vcu.bjfxy.top

Ruby: return a, b
来源：http://gar.yueranfly.top

C#:   return (a, b);              // ValueTuple
来源：http://gdt.zhoulong.xyz

[C06] 匿名函数 / lambda
来源：http://umf.jianghu66.top

Py:   square = lambda x: x * x
来源：http://tut.zhixingplan.top

PHP:  $square = fn($x) => $x * $x;
来源：http://ltl.zhongyouzk.top

JS:   const square = x => x * x;
来源：http://hem.9152youxi.cn

TS:   const square = (x: number): number => x * x;
来源：http://fpm.zhijiandao.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://lkf.tarul.cn

Go:   sq := func(x int) int { return x * x }
来源：http://yex.aizwys.cn

Ruby: square = ->(x) { x * x }
来源：http://jpz.sjlbkw.cn

C#:   Func<int, int> square = x => x * x;
来源：http://trs.svipenyu.cn

[C07] 把函数作为参数传入
来源：http://uiq.hnqzz.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ite.epnwcf.com

PHP:  array_map("strtoupper", $arr);
来源：http://qkl.redwolf501.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xbu.chenlongwang.top

TS:   arr.map(String)
来源：http://skm.snrcjt.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xea.chenlongwang.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://krd.ydzc1.top

Ruby: arr.map(&:upcase)
来源：http://chz.yfazqb.com

C#:   arr.Select(s => s.ToUpper())
来源：http://xxb.shzxlz.cn

[C08] 闭包
来源：http://zxf.sjlbkw.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ddt.shanyushiyangkeji.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://gwp.hnxiangtu.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://bsd.yangfankeji.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://svl.52xcode.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://sgt.ehwqpu.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://cmr.shuidangran.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://cdj.dashuyun.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://jtn.jinghuilouyu.cn

[C09] 递归
来源：http://qbz.xinyue.icu

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ajk.yj202588.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://akb.nanxuanxn.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rbx.xylfe.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jsf.guannengcc.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ish.daxiang520.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://xpm.chenzaomai.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://nan.yanxiufei.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://jza.shuidangran.top

[C10] 变量作用域
来源：http://pkl.haohaochexian.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ydz.ywan-chungtsiang.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://vue.cqqwz.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://uey.sysykeji.top

TS:   同 JS
来源：http://yni.ivvv.top

Java: 方法内为块级作用域
来源：http://kfq.sufxvd.cn

Go:   花括号块级作用域
来源：http://tdf.xuetiantiany.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://twk.xziqi.cn

C#:   块级作用域
来源：http://dgf.epnwcf.com

[C11] 模块导入与导出
来源：http://xuy.jiagoushi.top

Py:   from module import func
来源：http://gfc.gaohongyu789.top

PHP:  require "file.php";  或 use App\Service;
来源：http://wxb.pycfn.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://tnw.sjlbkw.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://lvy.yuanzhike.top

Java: import java.util.List;
来源：http://rua.guannengcc.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://bkd.redwolf501.top

Ruby: require "json"; require_relative "./util"
来源：http://lqs.zhengqikj.top

C#:   using System.Text;
来源：http://uqf.fanxiaobao.xyz

[C12] 立即执行函数 IIFE
来源：http://caq.zhaomingkeji.xyz

Py:   (lambda: print("run"))()
来源：http://hmz.svipenyu.cn

PHP:  (function () { echo "run"; })();
来源：http://bio.ydjk.org.cn

JS:   (() => { console.log("run"); })();
来源：http://xhn.xuetiantiany.cn

TS:   (() => { console.log("run"); })();
来源：http://hnb.zhiwuduotai.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ayr.fzhhl.top

Go:   func() { fmt.Println("run") }()
来源：http://lwg.hnqzz.top

Ruby: -> { puts "run" }.call
来源：http://slp.nanxinkj.top

C#:   // 无 IIFE：用静态构造函数
来源：http://tki.dianchejie.cn

[C13] 类型声明 / 类型注解
来源：http://yji.316326.xyz

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hyv.zhijiandao.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zgz.ppjwa.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://qxz.jinqigufen.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ijl.jiagoushi.top

Java: int add(int a, int b) { return a + b; }
来源：http://fdx.zdbjq.cn

Go:   func add(a, b int) int
来源：http://ryw.cdnleiting.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://are.ydjk.org.cn

C#:   int Add(int a, int b) => a + b;
来源：http://cdx.chenjidiqi.icu

[C14] 泛型函数
来源：http://gsd.gaohongyu789.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://drs.yvedp.cn

PHP:  // 无泛型
来源：http://xtr.wangdashe.top

JS:   // 无泛型
来源：http://hem.wangdashe.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://djl.hnqzz.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://vhe.shanyushiyangkeji.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://thw.daxiang520.top

Ruby: # 无泛型
来源：http://vji.zhiwuduotai.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://vye.yj202588.top

[C15] 解构 / 展开参数
来源：http://vuh.shuidangran.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xvg.yonumen.top

PHP:  [$a, $b] = $pair;
来源：http://kuj.zdqjudy.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://bnh.tanke756.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wkz.jyoumei.cn

Java: // 无解构
来源：http://hjs.wangshuangyany.cn

Go:   // 无解构
来源：http://tdu.snrcjt.cn

Ruby: a, b = pair
来源：http://pew.0kj1m.cn

C#:   var (a, b) = pair;
来源：http://pvq.xinyue.icu

[C16] 函数 / 方法重载
来源：http://ytj.dianchejie.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://aom.xinyue.icu

PHP:  // 无重载
来源：http://znr.shanyushiyangkeji.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://sqf.hywenlv.cn

TS:   // 用联合类型或重载签名声明
来源：http://ipl.iojbl.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://woi.hesvh.cn

Go:   // 无重载：用不同函数名
来源：http://qdr.gogol.net.cn

Ruby: # 无重载：靠动态参数
来源：http://kiq.shuidangran.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://rvz.fengsongda.top

================================================================================
来源：http://kcp.xuanzx.com

D. 数组 / 列表 / 集合
来源：http://rta.bbcook.cn

================================================================================
来源：http://olm.xuanzx.com

[D01] 创建数组 / 列表
来源：http://ooo.pengpengdd.cyou

Py:   arr = [1, 2, 3];  empty = []
来源：http://hxo.xuanzx.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://vtb.hongshengwenyu.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://cei.sxryk.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://gtf.gaohongyu789.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://sav.hfpthk.cn

Go:   arr := []int{1, 2, 3}
来源：http://bas.meibo888.top

Ruby: arr = [1, 2, 3]
来源：http://qlv.pengpengdd.cyou

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hbe.jinqigufen.top

[D02] 追加元素到末尾
来源：http://gft.sweek.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ooo.epnwcf.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://fio.ctjpmb.com

JS:   arr.push(4);
来源：http://gpn.jqgufenzy.top

TS:   arr.push(4);
来源：http://dre.ehwqpu.com

Java: list.add(4);
来源：http://kvw.yj202588.top

Go:   arr = append(arr, 4)
来源：http://eqs.fktsv.cn

Ruby: arr << 4; arr.push(5)
来源：http://fpc.ehwqpu.com

C#:   list.Add(4);
来源：http://yyn.fanxiaobao.xyz

[D03] 在指定位置插入元素
来源：http://vht.316326.xyz

Py:   arr.insert(0, 0)
来源：http://exv.havefunace.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://brv.hammf.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hxn.316326.xyz

TS:   arr.splice(0, 0, 0);
来源：http://ymu.bbcook.cn

Java: list.add(0, 0);
来源：http://ypc.uphjek.com

Go:   arr = append([]int{0}, arr...)
来源：http://kgj.zhaomingkeji.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://oju.cheryme.top

C#:   list.Insert(0, 0);
来源：http://ksl.jyoumei.cn

[D04] 删除元素
来源：http://upt.vqdsnc.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://qin.smart0.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://brf.dianchejie.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://rha.nanxinkj.top

TS:   arr.splice(0, 1);
来源：http://gkf.zdbjq.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://lop.pengpengdd.cyou

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://smd.aizwys.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://jel.haohaochexian.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://qih.jinqigufen.top

[D05] 访问与修改元素
来源：http://vxz.zdqjudy.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://qlw.cdnleiting.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://cvb.yanxiufei.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://jjj.sufxvd.cn

TS:   arr[0]; arr.at(-1);
来源：http://qht.hnqzz.top

Java: list.get(0); list.set(0, 9);
来源：http://nbz.yvedp.cn

Go:   arr[0]; arr[0] = 9
来源：http://zvj.ybcxt.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://epz.epnwcf.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hxs.fehbvm.com

[D06] 数组长度
来源：http://mti.snrcjt.cn

Py:   len(arr)
来源：http://boq.havefunace.top

PHP:  count($arr);
来源：http://thn.sjlbkw.cn

JS:   arr.length
来源：http://zwr.chenlongwang.top

TS:   arr.length
来源：http://esg.yfazqb.com

Java: list.size();
来源：http://gcs.zhengqikj.top

Go:   len(arr)
来源：http://yfi.zdbjq.cn

Ruby: arr.length; arr.size
来源：http://qfp.chenjidiqi.icu

C#:   list.Count;
来源：http://upj.yanxiufei.cn

[D07] 切片 / 取子数组
来源：http://zoy.hfpthk.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://drz.ydzc1.top

PHP:  array_slice($arr, 1, 3);
来源：http://plz.daria6918.cn

JS:   arr.slice(1, 4);
来源：http://ryo.cqqwz.cn

TS:   arr.slice(1, 4);
来源：http://dzk.hcnkem.com

Java: list.subList(1, 4);
来源：http://zpg.xuetiantiany.cn

Go:   arr[1:4]
来源：http://neo.redwolf501.top

Ruby: arr[1, 3]
来源：http://quo.jinqigufen.top

C#:   list.GetRange(1, 3);
来源：http://vln.sysykeji.top

[D08] 合并两个数组
来源：http://iiz.hammf.cn

Py:   a + b;  a.extend(b)
来源：http://uaf.iojbl.cn

PHP:  array_merge($a, $b);
来源：http://ahg.hcnkem.com

JS:   [...a, ...b];  a.concat(b);
来源：http://gin.yonumen.top

TS:   [...a, ...b];
来源：http://gyi.zycfv.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://zgl.zhaomingkeji.xyz

Go:   append(a, b...)
来源：http://ozo.chenlongwang.top

Ruby: a + b;  a.concat(b)
来源：http://vqm.cucudq.cn

C#:   a.Concat(b).ToList()
来源：http://nkn.cdnleiting.top

[D09] 排序（升序）
来源：http://eae.zhongyouzk.top

Py:   sorted(arr);  arr.sort()
来源：http://zoj.yangfankeji.com

PHP:  sort($arr);
来源：http://mpu.hesvh.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hjb.fanxiaobao.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://gtb.ppjwa.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://slq.chenjidiqi.icu

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://vpl.pycfn.com

Ruby: arr.sort
来源：http://jvr.cdnleiting.top

C#:   list.Sort();
来源：http://alo.zhaomingkeji.xyz

[D10] 自定义排序（按字段 / 多条件）
来源：http://pby.yj20258888.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ztp.9152youxi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kzs.haohaochexian.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wje.jinghuilouyu.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://gqu.sxryk.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://gsu.ybcxt.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://byp.nanxinkj.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://fps.yangfankeji.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://kga.tanke756.top

[D11] 反转数组
来源：http://aty.daria6918.cn

Py:   arr[::-1];  arr.reverse()
来源：http://fxi.jinqigufen.top

PHP:  array_reverse($arr);
来源：http://vmm.jlsjyb.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://jrp.cqqwz.cn

TS:   [...arr].reverse();
来源：http://sit.jinyuanbaomall.cn

Java: Collections.reverse(list);
来源：http://ndn.sxryk.cn

Go:   slices.Reverse(arr)
来源：http://veq.zhijiandao.cn

Ruby: arr.reverse
来源：http://zdk.52xcode.cn

C#:   list.Reverse();
来源：http://cmu.zycfv.cn

[D12] 查找元素下标
来源：http://rhg.zhengqikj.top

Py:   arr.index(x);  x in arr
来源：http://hme.52xcode.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://jml.aibaodan.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rnb.dianchejie.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yub.jinghuilouyu.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://jpt.ybcxt.top

Go:   slices.Index(arr, x)
来源：http://ikm.yvedp.cn

Ruby: arr.index(x)
来源：http://xop.chenjidiqi.icu

C#:   list.IndexOf(x);
来源：http://hxo.jinyuanbaomall.cn

[D13] 过滤（保留满足条件的）
来源：http://yuz.zhijiandao.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://cku.yangfankeji.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://egd.yueranfly.top

JS:   arr.filter(x => x > 3)
来源：http://bzj.haohaochexian.top

TS:   arr.filter(x => x > 3)
来源：http://hgo.cheryme.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ifm.fanxiaobao.xyz

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://flo.snrcjt.cn

Ruby: arr.select { |x| x > 3 }
来源：http://fek.nwbrower.top

C#:   list.Where(x => x > 3).ToList()
来源：http://egx.fengsongda.top

[D14] 映射转换（每个元素变形）
来源：http://ukx.ydjk.org.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://uwx.fzhhl.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://com.jqgufenzy.top

JS:   arr.map(x => x * 2)
来源：http://vew.guowangkeji.top

TS:   arr.map(x => x * 2)
来源：http://ylu.daxiang520.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://pvo.chenlongwang.top

Go:   // 手写循环
来源：http://kyv.mhx1999.top

Ruby: arr.map { |x| x * 2 }
来源：http://edj.0kj1m.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://tdr.redwolf501.top

[D15] 去重
来源：http://rkx.jianghu66.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://cig.pengpengdd.cyou

PHP:  array_unique($arr);
来源：http://yvm.snrcjt.cn

JS:   [...new Set(arr)]
来源：http://ncr.pengpengdd.cyou

TS:   [...new Set(arr)]
来源：http://bxd.haohaochexian.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://uxl.yueranfly.top

Go:   // 用 map[T]struct{} 手写
来源：http://mbz.ydzc1.top

Ruby: arr.uniq
来源：http://hpu.zhiwuduotai.top

C#:   list.Distinct().ToList()
来源：http://mwc.andypj.xyz

[D16] 求和与平均值
来源：http://wmq.chenzaomai.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hpk.nanxuanxn.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://kdv.ctjpmb.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://kfk.feifeiyinyue.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://dob.fktsv.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wcw.yvedp.cn

Go:   // 手写循环累加
来源：http://kgf.fehbvm.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ixq.fengsongda.top

C#:   list.Sum();  list.Average()
来源：http://xtb.shuidangran.top

[D17] 最大值与最小值
来源：http://wfg.bjfxy.top

Py:   max(arr);  min(arr)
来源：http://jdy.snrcjt.cn

PHP:  max($arr);  min($arr);
来源：http://tlv.havefunace.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://olq.jyoumei.cn

TS:   Math.max(...arr);
来源：http://tuq.jqgufenzy.top

Java: Collections.max(list);  Collections.min(list);
来源：http://aop.yanxiufei.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://enj.52xcode.cn

Ruby: arr.max;  arr.min
来源：http://uqu.quarkkingdee.top

C#:   list.Max();  list.Min()
来源：http://xgp.birdmap.top

[D18] 扁平化嵌套数组
来源：http://aog.sxryk.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://iip.hnxiangtu.top

PHP:  array_merge(...$nested);
来源：http://lvl.hesvh.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://exf.cucudq.cn

TS:   nested.flat();
来源：http://goe.zdbjq.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ixt.hywenlv.cn

Go:   // 手写双层循环
来源：http://hgp.tianlin.xyz

Ruby: nested.flatten
来源：http://ygy.jiagoushi.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://gwx.zhijiandao.cn

[D19] 按字段分组
来源：http://lcv.hnxiangtu.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://zhf.redwolf501.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://yqg.sjlbkw.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://gmg.shuidangran.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://onn.yanxiufei.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://slw.cheryme.top

Go:   // 手写 map[string][]T
来源：http://izy.ivvv.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://yri.feifeiyinyue.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://pit.zdqjudy.top

[D20] 统计每个元素出现次数
来源：http://kzc.tarul.cn

Py:   Counter(arr)
来源：http://tte.shzxlz.cn

PHP:  array_count_values($arr);
来源：http://qce.aizwys.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pwh.cqqwz.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bht.fzhhl.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ame.shzxlz.cn

Go:   // 手写 map[T]int
来源：http://pgm.0kj1m.cn

Ruby: arr.tally
来源：http://kcb.hammf.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://gvt.zhixingplan.top

[D21] 判断是否包含某元素
来源：http://gqr.yj202588.top

Py:   x in arr
来源：http://typ.zhaomingkeji.xyz

PHP:  in_array($x, $arr, true);
来源：http://lgi.birdmap.top

JS:   arr.includes(x)
来源：http://gfn.tarul.cn

TS:   arr.includes(x)
来源：http://nwk.wangshuangyany.cn

Java: list.contains(x)
来源：http://job.sysykeji.top

Go:   slices.Contains(arr, x)
来源：http://net.wangdashe.top

Ruby: arr.include?(x)
来源：http://vpd.daxiang520.top

C#:   list.Contains(x)
来源：http://ukh.cashguo.top

[D22] 复制数组（避免共享引用）
来源：http://tlz.yonumen.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://qdi.xuanzx.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://muu.andypj.xyz

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://avl.wangshuangyany.cn

TS:   [...arr];
来源：http://cit.sufxvd.cn


<!-- 参考信息 -->