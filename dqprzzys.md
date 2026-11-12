代发 wailian999

Ruby: def total(*nums); nums.sum; end
来源：http://uqx.yj20258888.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://lpe.cucudq.cn

[C04] 命名参数 / 关键字参数
来源：http://jpz.jiagoushi.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hsy.chenjidiqi.icu

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://nra.zdbjq.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://foo.feifeiyinyue.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://vcg.sysykeji.top

Java: // 无：用 Builder 模式或 record
来源：http://bqj.yuanzhike.top

Go:   // 无：用配置结构体参数
来源：http://ylw.guowangkeji.top

Ruby: f(a: 1, b: 2)
来源：http://fvk.jyoumei.cn

C#:   f(a: 1, b: 2)
来源：http://zru.chenlongwang.top

[C05] 返回多个值
来源：http://ari.fktsv.cn

Py:   return a, b
来源：http://qsq.xziqi.cn

PHP:  return [$a, $b];
来源：http://hkb.52xcode.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://rgg.zdqjudy.top

TS:   return { a, b };
来源：http://nvb.uphjek.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xtx.shanyushiyangkeji.top

Go:   return a, b
来源：http://kbn.jlsjyb.cn

Ruby: return a, b
来源：http://oqq.52xcode.cn

C#:   return (a, b);              // ValueTuple
来源：http://dip.jinyuanbaomall.cn

[C06] 匿名函数 / lambda
来源：http://jjt.tianlin.xyz

Py:   square = lambda x: x * x
来源：http://vek.sufxvd.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ese.cdnleiting.top

JS:   const square = x => x * x;
来源：http://edl.shangyingyoupin.top

TS:   const square = (x: number): number => x * x;
来源：http://cas.zdbjq.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://upo.vqdsnc.cn

Go:   sq := func(x int) int { return x * x }
来源：http://nxm.dianchejie.cn

Ruby: square = ->(x) { x * x }
来源：http://woe.haohaochexian.top

C#:   Func<int, int> square = x => x * x;
来源：http://vyy.ybcxt.top

[C07] 把函数作为参数传入
来源：http://kdd.shzxlz.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://fcu.chenlongwang.top

PHP:  array_map("strtoupper", $arr);
来源：http://jti.fanxiaobao.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://iud.zhixingplan.top

TS:   arr.map(String)
来源：http://ldo.nanxinkj.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ryg.gotoacloud.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://yji.fktsv.cn

Ruby: arr.map(&:upcase)
来源：http://htn.yongpay.top

C#:   arr.Select(s => s.ToUpper())
来源：http://xod.wangshuangyany.cn

[C08] 闭包
来源：http://wzi.hongshengwenyu.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wjn.zycfv.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://qam.cdnleiting.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://nkr.fktsv.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://pgp.xinyue.icu

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://uhx.xingfuxueyuan.xyz

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://nnf.redwolf501.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://jxg.chenzaomai.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://vog.meibo888.top

[C09] 递归
来源：http://qax.zhoulong.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://rnq.hongshengwenyu.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://vqy.meibo888.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pwz.ybcxt.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hnp.jqgufenzy.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://okn.vehdjk.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mxn.shzxlz.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://kra.jyoumei.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://bvt.shanyushiyangtech.top

[C10] 变量作用域
来源：http://pgz.mhx1999.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://lwp.c1oappe.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://fns.zhaomingkeji.xyz

JS:   let/const 块级作用域，var 函数级作用域
来源：http://bis.xingfuxueyuan.xyz

TS:   同 JS
来源：http://gkh.jlsjyb.cn

Java: 方法内为块级作用域
来源：http://jvh.yvedp.cn

Go:   花括号块级作用域
来源：http://zqw.tian-w.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://tzq.nanxuanxn.top

C#:   块级作用域
来源：http://soj.hesvh.cn

[C11] 模块导入与导出
来源：http://vks.zhiwuduotai.top

Py:   from module import func
来源：http://pqj.hysaishi.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://mms.snrcjt.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ofy.xingfuxueyuan.xyz

TS:   export function f(): void {};  import { f } from "./m";
来源：http://gqm.xuetiantiany.cn

Java: import java.util.List;
来源：http://cnf.xuanzx.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ker.sweek.top

Ruby: require "json"; require_relative "./util"
来源：http://exw.cashguo.top

C#:   using System.Text;
来源：http://eqb.jqgfzy.top

[C12] 立即执行函数 IIFE
来源：http://ckh.aizwys.cn

Py:   (lambda: print("run"))()
来源：http://gct.ywan-chungtsiang.top

PHP:  (function () { echo "run"; })();
来源：http://bmi.meibo888.top

JS:   (() => { console.log("run"); })();
来源：http://vlj.yonumen.top

TS:   (() => { console.log("run"); })();
来源：http://wyk.havefunace.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://vpa.mhx1999.top

Go:   func() { fmt.Println("run") }()
来源：http://gma.ywan-chungtsiang.top

Ruby: -> { puts "run" }.call
来源：http://bxo.guowangkeji.top

C#:   // 无 IIFE：用静态构造函数
来源：http://gch.jinqigufen.top

[C13] 类型声明 / 类型注解
来源：http://rtq.shangyingyoupin.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wrv.shanyushiyangtech.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://inm.cucudq.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wnr.shuidangran.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kds.havefunace.top

Java: int add(int a, int b) { return a + b; }
来源：http://tny.uphjek.com

Go:   func add(a, b int) int
来源：http://vpo.sxryk.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://gen.fzhhl.top

C#:   int Add(int a, int b) => a + b;
来源：http://tcd.yuxming.cn

[C14] 泛型函数
来源：http://aiz.zycfv.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://obc.chenjidiqi.icu

PHP:  // 无泛型
来源：http://jrx.jinghuilouyu.cn

JS:   // 无泛型
来源：http://eih.daxiang520.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://bjd.snrcjt.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://boq.sufxvd.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wph.ywan-chungtsiang.top

Ruby: # 无泛型
来源：http://xze.shanyushiyangtech.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xjv.sysykeji.top

[C15] 解构 / 展开参数
来源：http://cvm.andypj.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://qyj.jinqigfzy.top

PHP:  [$a, $b] = $pair;
来源：http://lxf.chenzaomai.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://tid.zhongyouzk.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://bdt.tianlin.xyz

Java: // 无解构
来源：http://bsn.cheryme.top

Go:   // 无解构
来源：http://bbv.shuidangran.top

Ruby: a, b = pair
来源：http://rin.sufxvd.cn

C#:   var (a, b) = pair;
来源：http://iiv.xinyue.icu

[C16] 函数 / 方法重载
来源：http://zmo.aibaodan.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://swd.cqqwz.cn

PHP:  // 无重载
来源：http://mnp.hammf.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://uxm.c1oappe.top

TS:   // 用联合类型或重载签名声明
来源：http://fnx.yangfankeji.com

Java: void f(int a) {}  void f(String a) {}
来源：http://dav.jqgfzy.top

Go:   // 无重载：用不同函数名
来源：http://cpe.jqgufenzy.top

Ruby: # 无重载：靠动态参数
来源：http://zvz.xinyue.icu

C#:   void F(int a) {}  void F(string a) {}
来源：http://jki.xylfe.cn

================================================================================
来源：http://yrh.yangfankeji.com

D. 数组 / 列表 / 集合
来源：http://vwk.shuidangran.top

================================================================================
来源：http://gfa.shanyushiyangkeji.top

[D01] 创建数组 / 列表
来源：http://ltf.feifeiyinyue.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://ckc.zdqjudy.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://zov.hysaishi.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://dvj.zycfv.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://kqh.yonumen.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ifl.zdbjq.cn

Go:   arr := []int{1, 2, 3}
来源：http://kpp.hfpthk.cn

Ruby: arr = [1, 2, 3]
来源：http://jab.hesvh.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://gio.shanyushiyangkeji.top

[D02] 追加元素到末尾
来源：http://xjg.nwbrower.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ayc.guowangkeji.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://utb.dashuyun.cn

JS:   arr.push(4);
来源：http://vez.xuetiantiany.cn

TS:   arr.push(4);
来源：http://fif.pycfn.com

Java: list.add(4);
来源：http://tyw.daria6918.cn

Go:   arr = append(arr, 4)
来源：http://scl.cucudq.cn

Ruby: arr << 4; arr.push(5)
来源：http://iqf.gzhubu.top

C#:   list.Add(4);
来源：http://yyp.iojbl.cn

[D03] 在指定位置插入元素
来源：http://unt.zhongyouzk.top

Py:   arr.insert(0, 0)
来源：http://ebt.cqqwz.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://fpc.jinqigfzy.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://vfm.cqqwz.cn

TS:   arr.splice(0, 0, 0);
来源：http://oep.dashuyun.cn

Java: list.add(0, 0);
来源：http://tpm.c1oappe.top

Go:   arr = append([]int{0}, arr...)
来源：http://ktb.zdqjudy.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://bki.snrcjt.cn

C#:   list.Insert(0, 0);
来源：http://byz.hcnkem.com

[D04] 删除元素
来源：http://rpm.zhiwuduotai.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://kdv.hesvh.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://faf.hnxiangtu.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://cpr.wangshuangyany.cn

TS:   arr.splice(0, 1);
来源：http://xyq.dianchejie.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mnp.pengpengdd.cyou

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://eed.hfpthk.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://gqv.fehbvm.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://zvx.ydjk.org.cn

[D05] 访问与修改元素
来源：http://ejv.xingfuxueyuan.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://nfy.fehbvm.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://kbj.yfazqb.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mie.birdmap.top

TS:   arr[0]; arr.at(-1);
来源：http://rso.hysaishi.cn

Java: list.get(0); list.set(0, 9);
来源：http://zle.xuanzx.com

Go:   arr[0]; arr[0] = 9
来源：http://bja.sysykeji.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://kxo.ydzc1.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://qje.jiagoushi.top

[D06] 数组长度
来源：http://ann.gogol.net.cn

Py:   len(arr)
来源：http://izq.hywenlv.cn

PHP:  count($arr);
来源：http://zpy.jqgfzy.top

JS:   arr.length
来源：http://zna.jinyuanbaomall.cn

TS:   arr.length
来源：http://edu.hywenlv.cn

Java: list.size();
来源：http://otq.ppjwa.cn

Go:   len(arr)
来源：http://udd.dianchejie.cn

Ruby: arr.length; arr.size
来源：http://kho.jlsjyb.cn

C#:   list.Count;
来源：http://kun.jlsjyb.cn

[D07] 切片 / 取子数组
来源：http://cfe.shangyingyoupin.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qoy.cheryme.top

PHP:  array_slice($arr, 1, 3);
来源：http://abp.havefunace.top

JS:   arr.slice(1, 4);
来源：http://vtk.uphjek.com

TS:   arr.slice(1, 4);
来源：http://rmg.yongpay.top

Java: list.subList(1, 4);
来源：http://jmj.feifeiyinyue.top

Go:   arr[1:4]
来源：http://ian.fzhhl.top

Ruby: arr[1, 3]
来源：http://yoq.sweek.top

C#:   list.GetRange(1, 3);
来源：http://upj.ydjk.org.cn

[D08] 合并两个数组
来源：http://pys.yuanzhike.top

Py:   a + b;  a.extend(b)
来源：http://siw.9152youxi.cn

PHP:  array_merge($a, $b);
来源：http://yeg.aibaodan.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://jju.zhixingplan.top

TS:   [...a, ...b];
来源：http://wkm.316326.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://daa.sysykeji.top

Go:   append(a, b...)
来源：http://mjs.yj20258.top

Ruby: a + b;  a.concat(b)
来源：http://paz.shzxlz.cn

C#:   a.Concat(b).ToList()
来源：http://suj.shuidangran.top

[D09] 排序（升序）
来源：http://uun.xziqi.cn

Py:   sorted(arr);  arr.sort()
来源：http://aew.vehdjk.com

PHP:  sort($arr);
来源：http://dud.meibo888.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://djy.yuanzhike.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://tnv.andypj.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://ral.jinqigufen.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qts.0kj1m.cn

Ruby: arr.sort
来源：http://dlw.mhx1999.top

C#:   list.Sort();
来源：http://ptq.c1oappe.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://did.bbcook.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://xeq.havefunace.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hpp.zhixingplan.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://jwe.jlsjyb.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://uoe.sweek.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://svu.kuanghao11.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ioo.jianghu66.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://jbq.hnxiangtu.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://dyj.meibo888.top

[D11] 反转数组
来源：http://rgc.aizwys.cn

Py:   arr[::-1];  arr.reverse()
来源：http://vfh.yuxming.cn

PHP:  array_reverse($arr);
来源：http://oka.bbcook.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://amd.mhx1999.top

TS:   [...arr].reverse();
来源：http://swo.jlsjyb.cn

Java: Collections.reverse(list);
来源：http://vvy.yfazqb.com

Go:   slices.Reverse(arr)
来源：http://uaa.tarul.cn

Ruby: arr.reverse
来源：http://rcv.tian-w.cn

C#:   list.Reverse();
来源：http://odp.xuetiantiany.cn

[D12] 查找元素下标
来源：http://ahx.xinyue.icu

Py:   arr.index(x);  x in arr
来源：http://ttk.cashguo.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://xqr.52xcode.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nub.zhiwuduotai.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://umv.yueranfly.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://fxo.sjlbkw.cn

Go:   slices.Index(arr, x)
来源：http://mve.smart0.xyz

Ruby: arr.index(x)
来源：http://ddu.fktsv.cn

C#:   list.IndexOf(x);
来源：http://gbv.jinqigfzy.top

[D13] 过滤（保留满足条件的）
来源：http://lls.jinqigfzy.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://znc.tianlin.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://iuv.andypj.xyz

JS:   arr.filter(x => x > 3)
来源：http://afp.zdqjudy.top

TS:   arr.filter(x => x > 3)
来源：http://kll.yj202588.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mtd.jianghu66.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://kvj.hysaishi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://fyx.gaohongyu789.top

C#:   list.Where(x => x > 3).ToList()
来源：http://bsj.jinghuilouyu.cn

[D14] 映射转换（每个元素变形）
来源：http://cuu.jinyuanbaomall.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://jdk.yangfankeji.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://bit.uphjek.com

JS:   arr.map(x => x * 2)
来源：http://qhv.cdnleiting.top

TS:   arr.map(x => x * 2)
来源：http://lsc.yfazqb.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://muk.fzhhl.top

Go:   // 手写循环
来源：http://fzn.jinqigufen.top

Ruby: arr.map { |x| x * 2 }
来源：http://gnw.jlsjyb.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://xdh.dianchejie.cn

[D15] 去重
来源：http://sjz.xuetiantiany.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://jhs.shanyushiyangkeji.top

PHP:  array_unique($arr);
来源：http://mgp.epnwcf.com

JS:   [...new Set(arr)]
来源：http://fgx.gaohongyu789.top

TS:   [...new Set(arr)]
来源：http://onz.guannengcc.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://vqk.ydjk.org.cn

Go:   // 用 map[T]struct{} 手写
来源：http://mgc.hcnkem.com

Ruby: arr.uniq
来源：http://qcl.cdnleiting.top

C#:   list.Distinct().ToList()
来源：http://soo.shanyushiyangtech.top

[D16] 求和与平均值
来源：http://myk.jqgufenzy.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://vnf.shanyushiyangtech.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://etg.shuidangran.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hct.sufxvd.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://myj.jinghuilouyu.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://awi.sufxvd.cn

Go:   // 手写循环累加
来源：http://ltb.bjfxy.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hak.zhijiandao.cn

C#:   list.Sum();  list.Average()
来源：http://fik.andypj.xyz

[D17] 最大值与最小值
来源：http://ueh.pengpengdd.cyou

Py:   max(arr);  min(arr)
来源：http://cqg.ydjk.org.cn

PHP:  max($arr);  min($arr);
来源：http://kvo.gotoacloud.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://brw.daria6918.cn

TS:   Math.max(...arr);
来源：http://auu.yj20258888.top

Java: Collections.max(list);  Collections.min(list);
来源：http://mck.zhijiandao.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://fjp.yuxming.cn

Ruby: arr.max;  arr.min
来源：http://dnj.feifeiyinyue.top

C#:   list.Max();  list.Min()
来源：http://rnv.hnqzz.top

[D18] 扁平化嵌套数组
来源：http://tso.kuanghao11.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://iec.guowangkeji.top

PHP:  array_merge(...$nested);
来源：http://bnt.nwbrower.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://kch.nanxinkj.top

TS:   nested.flat();
来源：http://wbj.bjfxy.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ytl.ywan-chungtsiang.top

Go:   // 手写双层循环
来源：http://yeb.yanxiufei.cn

Ruby: nested.flatten
来源：http://uqf.yvedp.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://nik.sxryk.cn

[D19] 按字段分组
来源：http://hzw.ydjk.org.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://vdh.zhaomingkeji.xyz

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://llj.cqqwz.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qqf.jinyuanbaomall.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://mlr.xuetiantiany.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://uag.dashuyun.cn

Go:   // 手写 map[string][]T
来源：http://kuz.wangshuangyany.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://lir.hywenlv.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://cjm.gogol.net.cn

[D20] 统计每个元素出现次数
来源：http://etl.vqdsnc.cn

Py:   Counter(arr)
来源：http://cmj.ivvv.top

PHP:  array_count_values($arr);
来源：http://jzf.xingfuxueyuan.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://csx.cheryme.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vzq.gzhubu.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://eob.tarul.cn

Go:   // 手写 map[T]int
来源：http://tkt.zdbjq.cn


<!-- 参考信息 -->