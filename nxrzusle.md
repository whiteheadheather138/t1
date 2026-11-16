代发 wailian999

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://rqc.redwolf501.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://vcj.nwbrower.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://eoq.svipenyu.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://tpc.smart0.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://gts.jinyuanbaomall.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://elh.jqgufenzy.top

[C04] 命名参数 / 关键字参数
来源：http://mlj.xinyue.icu

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://lbc.snrcjt.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://fzo.shanyushiyangtech.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hve.aibaodan.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://lwb.guowangkeji.top

Java: // 无：用 Builder 模式或 record
来源：http://xes.yvedp.cn

Go:   // 无：用配置结构体参数
来源：http://yhb.c1oappe.top

Ruby: f(a: 1, b: 2)
来源：http://nff.yvedp.cn

C#:   f(a: 1, b: 2)
来源：http://xhz.shzxlz.cn

[C05] 返回多个值
来源：http://exi.chenlongwang.top

Py:   return a, b
来源：http://icw.svipenyu.cn

PHP:  return [$a, $b];
来源：http://ika.cucudq.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://pks.daria6918.cn

TS:   return { a, b };
来源：http://knb.cheryme.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://sye.meibo888.top

Go:   return a, b
来源：http://jtk.guowangkeji.top

Ruby: return a, b
来源：http://var.yfazqb.com

C#:   return (a, b);              // ValueTuple
来源：http://vbm.ivvv.top

[C06] 匿名函数 / lambda
来源：http://iks.yvedp.cn

Py:   square = lambda x: x * x
来源：http://pdq.haohaochexian.top

PHP:  $square = fn($x) => $x * $x;
来源：http://mgf.meibo888.top

JS:   const square = x => x * x;
来源：http://blp.shanyushiyangkeji.top

TS:   const square = (x: number): number => x * x;
来源：http://nfi.sufxvd.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://tnv.chenlongwang.top

Go:   sq := func(x int) int { return x * x }
来源：http://bdh.jqgfzy.top

Ruby: square = ->(x) { x * x }
来源：http://kud.fanxiaobao.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://nmo.pengpengdd.cyou

[C07] 把函数作为参数传入
来源：http://dyb.zhixingplan.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://kmu.yueranfly.top

PHP:  array_map("strtoupper", $arr);
来源：http://pig.xinyue.icu

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://kam.shangyingyoupin.top

TS:   arr.map(String)
来源：http://bve.xuanzx.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ill.feifeiyinyue.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://bbl.chenjidiqi.icu

Ruby: arr.map(&:upcase)
来源：http://tjd.fktsv.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://pit.yj20258.top

[C08] 闭包
来源：http://vds.zhijiandao.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://map.wangdashe.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ahn.yonumen.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://cza.jiagoushi.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ccz.yuxming.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://gyk.zdbjq.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://glg.chenlongwang.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://scv.guowangkeji.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://lfn.jianghu66.top

[C09] 递归
来源：http://rvb.jqgufenzy.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://huk.xylfe.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://jun.shanyushiyangtech.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ckn.316326.xyz

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tro.dashuyun.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://qyk.jiagoushi.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://gnx.nanxinkj.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://kfa.hnqzz.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://xby.zhiwuduotai.top

[C10] 变量作用域
来源：http://muu.chenjidiqi.icu

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wuh.hnxiangtu.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://fdj.daria6918.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://fvh.hammf.cn

TS:   同 JS
来源：http://xja.hammf.cn

Java: 方法内为块级作用域
来源：http://jnr.yangfankeji.com

Go:   花括号块级作用域
来源：http://fff.jinqigufen.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://gpr.hnqzz.top

C#:   块级作用域
来源：http://kkm.ppjwa.cn

[C11] 模块导入与导出
来源：http://fxz.yj202588.top

Py:   from module import func
来源：http://uxy.52xcode.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://pgk.aizwys.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ycv.yfazqb.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mhl.jinghuilouyu.cn

Java: import java.util.List;
来源：http://wpi.ydjk.org.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://lui.yonumen.top

Ruby: require "json"; require_relative "./util"
来源：http://bel.cqqwz.cn

C#:   using System.Text;
来源：http://yid.shanyushiyangtech.top

[C12] 立即执行函数 IIFE
来源：http://zvw.wangshuangyany.cn

Py:   (lambda: print("run"))()
来源：http://sqb.hfpthk.cn

PHP:  (function () { echo "run"; })();
来源：http://kcc.yvedp.cn

JS:   (() => { console.log("run"); })();
来源：http://hnf.yongpay.top

TS:   (() => { console.log("run"); })();
来源：http://iws.hysaishi.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://xrx.andypj.xyz

Go:   func() { fmt.Println("run") }()
来源：http://qcf.yuxming.cn

Ruby: -> { puts "run" }.call
来源：http://vmm.daria6918.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://fmy.c1oappe.top

[C13] 类型声明 / 类型注解
来源：http://iwo.shzxlz.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://lkf.9152youxi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gmo.jqgfzy.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ezt.tian-w.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wru.zycfv.cn

Java: int add(int a, int b) { return a + b; }
来源：http://vvn.guowangkeji.top

Go:   func add(a, b int) int
来源：http://mzk.jinqigufen.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://xgo.guowangkeji.top

C#:   int Add(int a, int b) => a + b;
来源：http://lue.chenlongwang.top

[C14] 泛型函数
来源：http://xxi.snrcjt.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://yhx.nanxinkj.top

PHP:  // 无泛型
来源：http://vbc.cucudq.cn

JS:   // 无泛型
来源：http://ktt.fanxiaobao.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://aml.zhongyouzk.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://isc.sxryk.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://tok.ppjwa.cn

Ruby: # 无泛型
来源：http://kkx.gaohongyu789.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://jcq.yongpay.top

[C15] 解构 / 展开参数
来源：http://abc.epnwcf.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wmo.cucudq.cn

PHP:  [$a, $b] = $pair;
来源：http://hwa.jinqigfzy.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://cub.meibo888.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://tia.gotoacloud.top

Java: // 无解构
来源：http://ced.gaohongyu789.top

Go:   // 无解构
来源：http://mzc.vqdsnc.cn

Ruby: a, b = pair
来源：http://dnx.jyoumei.cn

C#:   var (a, b) = pair;
来源：http://dnx.zdqjudy.top

[C16] 函数 / 方法重载
来源：http://fjm.0kj1m.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://osq.jqgfzy.top

PHP:  // 无重载
来源：http://wid.zhengqikj.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://wka.xylfe.cn

TS:   // 用联合类型或重载签名声明
来源：http://jnj.xinyue.icu

Java: void f(int a) {}  void f(String a) {}
来源：http://qha.chenjidiqi.icu

Go:   // 无重载：用不同函数名
来源：http://imd.gzhubu.top

Ruby: # 无重载：靠动态参数
来源：http://rsq.zhiwuduotai.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://scy.xylfe.cn

================================================================================
来源：http://aqg.hnqzz.top

D. 数组 / 列表 / 集合
来源：http://hdi.iojbl.cn

================================================================================
来源：http://cur.xziqi.cn

[D01] 创建数组 / 列表
来源：http://svu.tarul.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://iwq.xinyue.icu

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://nvh.ppjwa.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://unl.aizwys.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://pfc.meibo888.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://oxg.pengpengdd.cyou

Go:   arr := []int{1, 2, 3}
来源：http://dch.yvedp.cn

Ruby: arr = [1, 2, 3]
来源：http://kqt.gotoacloud.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://jyj.hnxiangtu.top

[D02] 追加元素到末尾
来源：http://yms.hysaishi.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://vgx.shzxlz.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ebf.mhx1999.top

JS:   arr.push(4);
来源：http://lho.316326.xyz

TS:   arr.push(4);
来源：http://cri.sweek.top

Java: list.add(4);
来源：http://vco.jinyuanbaomall.cn

Go:   arr = append(arr, 4)
来源：http://ear.fanxiaobao.xyz

Ruby: arr << 4; arr.push(5)
来源：http://ptn.feifeiyinyue.top

C#:   list.Add(4);
来源：http://bpq.havefunace.top

[D03] 在指定位置插入元素
来源：http://wde.wangdashe.top

Py:   arr.insert(0, 0)
来源：http://vis.ybcxt.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://iyn.52xcode.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://lkq.aizwys.cn

TS:   arr.splice(0, 0, 0);
来源：http://mxv.cucudq.cn

Java: list.add(0, 0);
来源：http://ulz.hnxiangtu.top

Go:   arr = append([]int{0}, arr...)
来源：http://anv.wangshuangyany.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://egn.yvedp.cn

C#:   list.Insert(0, 0);
来源：http://wag.feifeiyinyue.top

[D04] 删除元素
来源：http://mig.hesvh.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://boe.nwbrower.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://pvw.jinqigfzy.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://byx.sufxvd.cn

TS:   arr.splice(0, 1);
来源：http://zhf.vehdjk.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://duq.ppjwa.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://isd.hnxiangtu.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://irm.yj20258.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://eam.xuetiantiany.cn

[D05] 访问与修改元素
来源：http://aye.nanxinkj.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://cbz.xinyue.icu

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://vhz.xziqi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://svu.zhoulong.xyz

TS:   arr[0]; arr.at(-1);
来源：http://rby.gogol.net.cn

Java: list.get(0); list.set(0, 9);
来源：http://wdq.hesvh.cn

Go:   arr[0]; arr[0] = 9
来源：http://plt.hywenlv.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://gcu.fehbvm.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://lkr.sweek.top

[D06] 数组长度
来源：http://mjc.cashguo.top

Py:   len(arr)
来源：http://hkx.snrcjt.cn

PHP:  count($arr);
来源：http://rjv.bjfxy.top

JS:   arr.length
来源：http://eda.zhengqikj.top

TS:   arr.length
来源：http://box.yvedp.cn

Java: list.size();
来源：http://ioa.xylfe.cn

Go:   len(arr)
来源：http://bbb.jinyuanbaomall.cn

Ruby: arr.length; arr.size
来源：http://imn.mhx1999.top

C#:   list.Count;
来源：http://ifc.sysykeji.top

[D07] 切片 / 取子数组
来源：http://ugj.jinyuanbaomall.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://geo.xuetiantiany.cn

PHP:  array_slice($arr, 1, 3);
来源：http://oxi.fengsongda.top

JS:   arr.slice(1, 4);
来源：http://vba.jinqigufen.top

TS:   arr.slice(1, 4);
来源：http://afk.hongshengwenyu.top

Java: list.subList(1, 4);
来源：http://kaa.jyoumei.cn

Go:   arr[1:4]
来源：http://ghd.daxiang520.top

Ruby: arr[1, 3]
来源：http://mzt.yj202588.top

C#:   list.GetRange(1, 3);
来源：http://jzg.ydzc1.top

[D08] 合并两个数组
来源：http://aor.hysaishi.cn

Py:   a + b;  a.extend(b)
来源：http://etz.nanxinkj.top

PHP:  array_merge($a, $b);
来源：http://fkk.ydzc1.top

JS:   [...a, ...b];  a.concat(b);
来源：http://enz.yanxiufei.cn

TS:   [...a, ...b];
来源：http://jwg.hnqzz.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://zht.xylfe.cn

Go:   append(a, b...)
来源：http://fxo.9152youxi.cn

Ruby: a + b;  a.concat(b)
来源：http://qru.chenzaomai.com

C#:   a.Concat(b).ToList()
来源：http://ypu.xuanzx.com

[D09] 排序（升序）
来源：http://wzv.jinqigfzy.top

Py:   sorted(arr);  arr.sort()
来源：http://vsg.shanyushiyangtech.top

PHP:  sort($arr);
来源：http://dhp.tian-w.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ayj.cheryme.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://jpw.shangyingyoupin.top

Java: Collections.sort(list);  list.sort(null);
来源：http://rsj.hnqzz.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://jyn.zycfv.cn

Ruby: arr.sort
来源：http://faf.xuetiantiany.cn

C#:   list.Sort();
来源：http://ila.epnwcf.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://uha.fzhhl.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://vvq.sjlbkw.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vsh.cdnleiting.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wez.mhx1999.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://pfb.jinqigfzy.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://jch.cqqwz.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://snp.havefunace.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://vnp.sysykeji.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://jqm.hnqzz.top

[D11] 反转数组
来源：http://ncm.jinqigfzy.top

Py:   arr[::-1];  arr.reverse()
来源：http://yvx.9152youxi.cn

PHP:  array_reverse($arr);
来源：http://usz.pycfn.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://aph.mhx1999.top

TS:   [...arr].reverse();
来源：http://vrl.nanxinkj.top

Java: Collections.reverse(list);
来源：http://dxs.cucudq.cn

Go:   slices.Reverse(arr)
来源：http://ych.chenzaomai.com

Ruby: arr.reverse
来源：http://fvb.gzhubu.top

C#:   list.Reverse();
来源：http://sis.zhengqikj.top

[D12] 查找元素下标
来源：http://mds.wangshuangyany.cn

Py:   arr.index(x);  x in arr
来源：http://cdf.cucudq.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://bgd.xylfe.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nre.xinyue.icu

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bmz.quarkkingdee.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://xgw.zhaomingkeji.xyz

Go:   slices.Index(arr, x)
来源：http://oje.hysaishi.cn

Ruby: arr.index(x)
来源：http://oau.svipenyu.cn

C#:   list.IndexOf(x);
来源：http://uhk.xuanzx.com

[D13] 过滤（保留满足条件的）
来源：http://lqb.316326.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://fgn.jinqigfzy.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ofx.bjfxy.top

JS:   arr.filter(x => x > 3)
来源：http://rxt.yfazqb.com

TS:   arr.filter(x => x > 3)
来源：http://ort.bbcook.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://tjd.hongshengwenyu.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://bfy.redwolf501.top

Ruby: arr.select { |x| x > 3 }
来源：http://guf.yangfankeji.com

C#:   list.Where(x => x > 3).ToList()
来源：http://qco.gaohongyu789.top

[D14] 映射转换（每个元素变形）
来源：http://wvt.havefunace.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ovb.gotoacloud.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://dip.meibo888.top

JS:   arr.map(x => x * 2)
来源：http://jvq.hammf.cn

TS:   arr.map(x => x * 2)
来源：http://gbp.tarul.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ref.vehdjk.com

Go:   // 手写循环
来源：http://trf.jyoumei.cn

Ruby: arr.map { |x| x * 2 }
来源：http://pfu.316326.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://jcz.tianlin.xyz

[D15] 去重
来源：http://yib.zhiwuduotai.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://rgn.svipenyu.cn

PHP:  array_unique($arr);
来源：http://laz.snrcjt.cn

JS:   [...new Set(arr)]
来源：http://xgt.c1oappe.top

TS:   [...new Set(arr)]
来源：http://rfs.gzhubu.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://bhm.yangfankeji.com

Go:   // 用 map[T]struct{} 手写
来源：http://fzy.zycfv.cn

Ruby: arr.uniq
来源：http://zdx.yanxiufei.cn

C#:   list.Distinct().ToList()
来源：http://slu.zhoulong.xyz

[D16] 求和与平均值
来源：http://lpt.vehdjk.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://csx.yangfankeji.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://iza.zhijiandao.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://akd.fktsv.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://guw.dianchejie.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://uhw.svipenyu.cn

Go:   // 手写循环累加
来源：http://vuo.tianlin.xyz

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://qpa.zdbjq.cn

C#:   list.Sum();  list.Average()
来源：http://btw.yj20258.top

[D17] 最大值与最小值
来源：http://maf.vqdsnc.cn

Py:   max(arr);  min(arr)
来源：http://kob.shanyushiyangtech.top

PHP:  max($arr);  min($arr);
来源：http://ylh.jinghuilouyu.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://uwa.zhoulong.xyz

TS:   Math.max(...arr);
来源：http://olx.redwolf501.top

Java: Collections.max(list);  Collections.min(list);
来源：http://ske.shangyingyoupin.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://xss.iojbl.cn

Ruby: arr.max;  arr.min
来源：http://ajt.gaohongyu789.top

C#:   list.Max();  list.Min()
来源：http://zzq.meibo888.top

[D18] 扁平化嵌套数组
来源：http://vjn.jqgfzy.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://cik.52xcode.cn

PHP:  array_merge(...$nested);
来源：http://kfz.cheryme.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://kzb.daxiang520.top

TS:   nested.flat();
来源：http://wzn.zdbjq.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mia.andypj.xyz

Go:   // 手写双层循环
来源：http://ilw.dianchejie.cn

Ruby: nested.flatten
来源：http://eou.aibaodan.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://fbp.xuetiantiany.cn

[D19] 按字段分组
来源：http://vog.epnwcf.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://xht.tarul.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://fcy.xingfuxueyuan.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://pla.hnxiangtu.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://dzy.zhaomingkeji.xyz

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wxx.pengpengdd.cyou

Go:   // 手写 map[string][]T
来源：http://tvp.wangdashe.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://elh.hysaishi.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://irf.yj20258888.top

[D20] 统计每个元素出现次数
来源：http://gqq.zhaomingkeji.xyz

Py:   Counter(arr)
来源：http://bfo.chenjidiqi.icu

PHP:  array_count_values($arr);
来源：http://nfq.jyoumei.cn


<!-- 参考信息 -->