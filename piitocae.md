代发 wailian999

Go:   a && b || !c
来源：http://zni.yvedp.cn

Ruby: a && b || !c
来源：http://iad.birdmap.top

C#:   a && b || !c
来源：http://nfs.guannengcc.top

[B16] 卫语句：不满足条件提前返回
来源：http://nei.ctjpmb.com

Py:   if not data: return
来源：http://ynf.snrcjt.cn

PHP:  if (!$data) { return; }
来源：http://kxq.ivvv.top

JS:   if (!data) return;
来源：http://lah.cqqwz.cn

TS:   if (!data) return;
来源：http://wot.9152youxi.cn

Java: if (data == null) return;
来源：http://ocm.meibo888.top

Go:   if data == nil { return }
来源：http://bgk.shzxlz.cn

Ruby: return if data.nil?
来源：http://mpv.shanyushiyangkeji.top

C#:   if (data == null) return;
来源：http://nay.havefunace.top

================================================================================
来源：http://pad.shzxlz.cn

C. 函数与作用域
来源：http://bwt.0kj1m.cn

================================================================================
来源：http://bku.chenjidiqi.icu

[C01] 定义函数
来源：http://uza.vqdsnc.cn

Py:   def add(a, b): return a + b
来源：http://mwv.quarkkingdee.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zen.aibaodan.cn

JS:   function add(a, b) { return a + b; }
来源：http://rro.chenlongwang.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xus.iojbl.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://zpi.hnqzz.top

Go:   func add(a, b int) int { return a + b }
来源：http://pql.aizwys.cn

Ruby: def add(a, b); a + b; end
来源：http://ezr.andypj.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://oqa.jinghuilouyu.cn

[C02] 默认参数
来源：http://ntu.redwolf501.top

Py:   def greet(name="World"): return name
来源：http://czs.kuanghao11.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://thw.gogol.net.cn

JS:   function greet(name = "World") { return name; }
来源：http://vrv.yueranfly.top

TS:   function greet(name: string = "World") { return name; }
来源：http://ite.zhixingplan.top

Java: // 无默认参数：方法重载或 Optional
来源：http://vii.jqgufenzy.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ruo.hfpthk.cn

Ruby: def greet(name = "World") = name
来源：http://quc.yonumen.top

C#:   string Greet(string name = "World") => name;
来源：http://xxb.shzxlz.cn

[C03] 可变参数
来源：http://htp.zdbjq.cn

Py:   def total(*args): return sum(args)
来源：http://shh.aibaodan.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://zaw.kuanghao11.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ice.cdnleiting.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://qgn.yonumen.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mbv.shzxlz.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://egu.52xcode.cn

Ruby: def total(*nums); nums.sum; end
来源：http://xbk.ybcxt.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blc.hfpthk.cn

[C04] 命名参数 / 关键字参数
来源：http://ciw.daxiang520.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://odk.sjlbkw.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://pxf.sweek.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ydz.pengpengdd.cyou

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://onc.feifeiyinyue.top

Java: // 无：用 Builder 模式或 record
来源：http://zmm.snrcjt.cn

Go:   // 无：用配置结构体参数
来源：http://xls.kuanghao11.cn

Ruby: f(a: 1, b: 2)
来源：http://dez.xinyue.icu

C#:   f(a: 1, b: 2)
来源：http://itn.jinqigufen.top

[C05] 返回多个值
来源：http://nzt.vehdjk.com

Py:   return a, b
来源：http://rzf.snrcjt.cn

PHP:  return [$a, $b];
来源：http://azb.ywan-chungtsiang.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://lkr.jinghuilouyu.cn

TS:   return { a, b };
来源：http://apv.hywenlv.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://bgs.sysykeji.top

Go:   return a, b
来源：http://num.sjlbkw.cn

Ruby: return a, b
来源：http://lwj.meibo888.top

C#:   return (a, b);              // ValueTuple
来源：http://pwh.xylfe.cn

[C06] 匿名函数 / lambda
来源：http://swm.sufxvd.cn

Py:   square = lambda x: x * x
来源：http://jtw.sufxvd.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://pjg.zhixingplan.top

JS:   const square = x => x * x;
来源：http://fff.sweek.top

TS:   const square = (x: number): number => x * x;
来源：http://iix.sysykeji.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://nrw.wangdashe.top

Go:   sq := func(x int) int { return x * x }
来源：http://ato.xziqi.cn

Ruby: square = ->(x) { x * x }
来源：http://mjr.jianghu66.top

C#:   Func<int, int> square = x => x * x;
来源：http://gby.zhengqikj.top

[C07] 把函数作为参数传入
来源：http://mpl.sjlbkw.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://yts.cdnleiting.top

PHP:  array_map("strtoupper", $arr);
来源：http://vuy.daria6918.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ejc.nanxinkj.top

TS:   arr.map(String)
来源：http://tjs.jqgfzy.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://uzo.chenjidiqi.icu

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://csd.xziqi.cn

Ruby: arr.map(&:upcase)
来源：http://wsp.fktsv.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://kkn.yj202588.top

[C08] 闭包
来源：http://jlc.cucudq.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://aml.jinyuanbaomall.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://fvj.wangdashe.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://riw.xziqi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mib.gzhubu.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://zis.tianlin.xyz

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://nox.cheryme.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hvi.bjfxy.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://nho.jinqigufen.top

[C09] 递归
来源：http://xbv.sysykeji.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wcd.tian-w.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://lec.chenzaomai.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zjb.chenjidiqi.icu

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tgi.fehbvm.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://udx.zhengqikj.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://xmg.0kj1m.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://vev.nanxuanxn.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://gkt.vqdsnc.cn

[C10] 变量作用域
来源：http://kdt.xuetiantiany.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://tvm.sxryk.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ioo.sxryk.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://gui.ywan-chungtsiang.top

TS:   同 JS
来源：http://cvy.pycfn.com

Java: 方法内为块级作用域
来源：http://pxb.c1oappe.top

Go:   花括号块级作用域
来源：http://xvm.chenzaomai.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://int.hesvh.cn

C#:   块级作用域
来源：http://ikg.xinyue.icu

[C11] 模块导入与导出
来源：http://wme.uphjek.com

Py:   from module import func
来源：http://yct.wangdashe.top

PHP:  require "file.php";  或 use App\Service;
来源：http://roi.zhiwuduotai.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://qwl.cucudq.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ahw.ydjk.org.cn

Java: import java.util.List;
来源：http://aja.vqdsnc.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://xmj.zhengqikj.top

Ruby: require "json"; require_relative "./util"
来源：http://cgu.sxryk.cn

C#:   using System.Text;
来源：http://tud.hnqzz.top

[C12] 立即执行函数 IIFE
来源：http://jwn.jiagoushi.top

Py:   (lambda: print("run"))()
来源：http://hhy.fktsv.cn

PHP:  (function () { echo "run"; })();
来源：http://kgq.yonumen.top

JS:   (() => { console.log("run"); })();
来源：http://auy.wangdashe.top

TS:   (() => { console.log("run"); })();
来源：http://gru.xuanzx.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://juw.nanxinkj.top

Go:   func() { fmt.Println("run") }()
来源：http://yhd.ydzc1.top

Ruby: -> { puts "run" }.call
来源：http://fth.yangfankeji.com

C#:   // 无 IIFE：用静态构造函数
来源：http://rki.bjfxy.top

[C13] 类型声明 / 类型注解
来源：http://qhp.hfpthk.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://rne.xuetiantiany.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wmc.ctjpmb.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://lrp.hnxiangtu.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rqw.uphjek.com

Java: int add(int a, int b) { return a + b; }
来源：http://xfn.tianlin.xyz

Go:   func add(a, b int) int
来源：http://uao.zdbjq.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://sws.meibo888.top

C#:   int Add(int a, int b) => a + b;
来源：http://tcx.cucudq.cn

[C14] 泛型函数
来源：http://hle.hammf.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hax.chenzaomai.com

PHP:  // 无泛型
来源：http://umm.0kj1m.cn

JS:   // 无泛型
来源：http://ewx.cheryme.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wkb.fehbvm.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://poe.daxiang520.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://iug.daxiang520.top

Ruby: # 无泛型
来源：http://vog.52xcode.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://qpv.shanyushiyangkeji.top

[C15] 解构 / 展开参数
来源：http://qum.sysykeji.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://sfs.zhongyouzk.top

PHP:  [$a, $b] = $pair;
来源：http://ryp.smart0.xyz

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://tzv.bjfxy.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ubb.snrcjt.cn

Java: // 无解构
来源：http://gjp.hysaishi.cn

Go:   // 无解构
来源：http://jqq.sjlbkw.cn

Ruby: a, b = pair
来源：http://did.0kj1m.cn

C#:   var (a, b) = pair;
来源：http://ozz.zhixingplan.top

[C16] 函数 / 方法重载
来源：http://zwy.chenjidiqi.icu

Py:   # 无重载：用默认参数或 *args 变通
来源：http://qdt.ydzc1.top

PHP:  // 无重载
来源：http://akd.hongshengwenyu.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://kli.ydzc1.top

TS:   // 用联合类型或重载签名声明
来源：http://tid.gzhubu.top

Java: void f(int a) {}  void f(String a) {}
来源：http://iva.mhx1999.top

Go:   // 无重载：用不同函数名
来源：http://cqx.quarkkingdee.top

Ruby: # 无重载：靠动态参数
来源：http://chw.daxiang520.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://baw.yuxming.cn

================================================================================
来源：http://czw.smart0.xyz

D. 数组 / 列表 / 集合
来源：http://bie.zdqjudy.top

================================================================================
来源：http://xzd.hesvh.cn

[D01] 创建数组 / 列表
来源：http://qhg.snrcjt.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://max.9152youxi.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://isn.jinqigfzy.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://dhd.jinghuilouyu.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://hwn.ydzc1.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://kyp.ivvv.top

Go:   arr := []int{1, 2, 3}
来源：http://sxe.hongshengwenyu.top

Ruby: arr = [1, 2, 3]
来源：http://wwm.bbcook.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://jdq.feifeiyinyue.top

[D02] 追加元素到末尾
来源：http://bke.zycfv.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://pjt.chenlongwang.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://kve.zhiwuduotai.top

JS:   arr.push(4);
来源：http://huv.sxryk.cn

TS:   arr.push(4);
来源：http://zhv.zdbjq.cn

Java: list.add(4);
来源：http://dby.ydzc1.top

Go:   arr = append(arr, 4)
来源：http://ujw.cashguo.top

Ruby: arr << 4; arr.push(5)
来源：http://jyw.hnxiangtu.top

C#:   list.Add(4);
来源：http://tku.dashuyun.cn

[D03] 在指定位置插入元素
来源：http://hqb.zdbjq.cn

Py:   arr.insert(0, 0)
来源：http://xfe.feifeiyinyue.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ymn.birdmap.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://vdy.dianchejie.cn

TS:   arr.splice(0, 0, 0);
来源：http://eeh.uphjek.com

Java: list.add(0, 0);
来源：http://alb.daxiang520.top

Go:   arr = append([]int{0}, arr...)
来源：http://vue.jqgufenzy.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ypb.gaohongyu789.top

C#:   list.Insert(0, 0);
来源：http://ndf.feifeiyinyue.top

[D04] 删除元素
来源：http://ahr.yfazqb.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://irb.aibaodan.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://lfh.cucudq.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wcl.ehwqpu.com

TS:   arr.splice(0, 1);
来源：http://szj.dashuyun.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://owg.vehdjk.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://yna.wangshuangyany.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ccy.wangdashe.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wwk.9152youxi.cn

[D05] 访问与修改元素
来源：http://ltt.uphjek.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://eku.shuidangran.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://dgq.shzxlz.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://kvz.zdbjq.cn

TS:   arr[0]; arr.at(-1);
来源：http://agd.gogol.net.cn

Java: list.get(0); list.set(0, 9);
来源：http://syx.feifeiyinyue.top

Go:   arr[0]; arr[0] = 9
来源：http://eea.gogol.net.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://lph.vehdjk.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://anm.jiagoushi.top

[D06] 数组长度
来源：http://yhx.jqgufenzy.top

Py:   len(arr)
来源：http://mcl.jinghuilouyu.cn

PHP:  count($arr);
来源：http://rjg.ybcxt.top

JS:   arr.length
来源：http://laq.sweek.top

TS:   arr.length
来源：http://vsd.zhongyouzk.top

Java: list.size();
来源：http://nqw.gaohongyu789.top

Go:   len(arr)
来源：http://mri.daria6918.cn

Ruby: arr.length; arr.size
来源：http://jun.zhoulong.xyz

C#:   list.Count;
来源：http://bod.feifeiyinyue.top

[D07] 切片 / 取子数组
来源：http://zul.aibaodan.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://yjb.guowangkeji.top

PHP:  array_slice($arr, 1, 3);
来源：http://jte.ppjwa.cn

JS:   arr.slice(1, 4);
来源：http://vnt.bbcook.cn

TS:   arr.slice(1, 4);
来源：http://frj.9152youxi.cn

Java: list.subList(1, 4);
来源：http://cdn.feifeiyinyue.top

Go:   arr[1:4]
来源：http://ehg.xuanzx.com

Ruby: arr[1, 3]
来源：http://dop.svipenyu.cn

C#:   list.GetRange(1, 3);
来源：http://kmr.zdbjq.cn

[D08] 合并两个数组
来源：http://zeu.vehdjk.com

Py:   a + b;  a.extend(b)
来源：http://ijo.xylfe.cn

PHP:  array_merge($a, $b);
来源：http://dzm.fehbvm.com

JS:   [...a, ...b];  a.concat(b);
来源：http://cjq.jqgufenzy.top

TS:   [...a, ...b];
来源：http://hbw.guannengcc.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://tcw.hammf.cn

Go:   append(a, b...)
来源：http://mpw.ybcxt.top

Ruby: a + b;  a.concat(b)
来源：http://eqo.yueranfly.top

C#:   a.Concat(b).ToList()
来源：http://vfz.yuxming.cn

[D09] 排序（升序）
来源：http://bsq.fengsongda.top

Py:   sorted(arr);  arr.sort()
来源：http://imj.zycfv.cn

PHP:  sort($arr);
来源：http://arw.zhengqikj.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://vcl.gogol.net.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://frp.dianchejie.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://zqb.shuidangran.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://xup.sufxvd.cn

Ruby: arr.sort
来源：http://dzb.jinqigfzy.top

C#:   list.Sort();
来源：http://kgb.jiagoushi.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://ril.xuanzx.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qff.feifeiyinyue.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://elr.gogol.net.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://gtd.nanxuanxn.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://yfm.yuanzhike.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://xlf.nanxinkj.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://jsq.chenzaomai.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://tdz.yonumen.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://dgs.tarul.cn

[D11] 反转数组
来源：http://urb.quarkkingdee.top

Py:   arr[::-1];  arr.reverse()
来源：http://xin.xylfe.cn

PHP:  array_reverse($arr);
来源：http://kra.xziqi.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://iah.zhoulong.xyz

TS:   [...arr].reverse();
来源：http://wkp.ppjwa.cn

Java: Collections.reverse(list);
来源：http://gim.hongshengwenyu.top

Go:   slices.Reverse(arr)
来源：http://jqb.daxiang520.top

Ruby: arr.reverse
来源：http://uob.hongshengwenyu.top

C#:   list.Reverse();
来源：http://ubr.yonumen.top

[D12] 查找元素下标
来源：http://yba.yj20258.top

Py:   arr.index(x);  x in arr
来源：http://yws.jqgfzy.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://gfc.zdbjq.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mba.jqgufenzy.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ycm.yanxiufei.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://dck.zdqjudy.top

Go:   slices.Index(arr, x)
来源：http://xoh.chenlongwang.top

Ruby: arr.index(x)
来源：http://pdj.shuidangran.top

C#:   list.IndexOf(x);
来源：http://gss.jianghu66.top

[D13] 过滤（保留满足条件的）
来源：http://zye.haohaochexian.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wuj.xingfuxueyuan.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://emu.snrcjt.cn

JS:   arr.filter(x => x > 3)
来源：http://itf.hywenlv.cn

TS:   arr.filter(x => x > 3)
来源：http://qie.snrcjt.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://xig.sjlbkw.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://stf.cucudq.cn

Ruby: arr.select { |x| x > 3 }
来源：http://oig.hongshengwenyu.top

C#:   list.Where(x => x > 3).ToList()
来源：http://cvv.gogol.net.cn

[D14] 映射转换（每个元素变形）
来源：http://oup.xuetiantiany.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://vxo.yj202588.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hcj.epnwcf.com

JS:   arr.map(x => x * 2)
来源：http://kzy.ivvv.top

TS:   arr.map(x => x * 2)
来源：http://nkz.bbcook.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://nwx.316326.xyz

Go:   // 手写循环
来源：http://tfk.ydjk.org.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ejg.meibo888.top

C#:   list.Select(x => x * 2).ToList()
来源：http://bzd.jqgfzy.top

[D15] 去重
来源：http://cwi.gotoacloud.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://nvj.zdqjudy.top

PHP:  array_unique($arr);
来源：http://irp.zhijiandao.cn

JS:   [...new Set(arr)]
来源：http://ctg.chenjidiqi.icu

TS:   [...new Set(arr)]
来源：http://fml.yongpay.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://awb.zhijiandao.cn

Go:   // 用 map[T]struct{} 手写
来源：http://gis.redwolf501.top

Ruby: arr.uniq
来源：http://tlf.xuetiantiany.cn

C#:   list.Distinct().ToList()
来源：http://pzj.guannengcc.top

[D16] 求和与平均值
来源：http://clr.ybcxt.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://vkf.jqgfzy.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ekx.cqqwz.cn


<!-- 参考信息 -->