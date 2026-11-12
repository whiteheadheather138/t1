代发 wailian999

C#:   string Greet(string name = "World") => name;
来源：http://yoy.jiagoushi.top

[C03] 可变参数
来源：http://sah.kuanghao11.cn

Py:   def total(*args): return sum(args)
来源：http://scj.tianlin.xyz

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hgx.mhx1999.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ssq.jinqigufen.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://oxr.shangyingyoupin.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://pxa.shangyingyoupin.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://vdd.vehdjk.com

Ruby: def total(*nums); nums.sum; end
来源：http://dqg.sufxvd.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://opi.yuanzhike.top

[C04] 命名参数 / 关键字参数
来源：http://afc.epnwcf.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ijl.wangdashe.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://vnc.yonumen.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://lvf.316326.xyz

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://irn.c1oappe.top

Java: // 无：用 Builder 模式或 record
来源：http://omu.yanxiufei.cn

Go:   // 无：用配置结构体参数
来源：http://caf.ybcxt.top

Ruby: f(a: 1, b: 2)
来源：http://zvx.shuidangran.top

C#:   f(a: 1, b: 2)
来源：http://kbb.yuanzhike.top

[C05] 返回多个值
来源：http://iae.vehdjk.com

Py:   return a, b
来源：http://uxa.daxiang520.top

PHP:  return [$a, $b];
来源：http://sgg.sxryk.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://fed.ctjpmb.com

TS:   return { a, b };
来源：http://clb.nanxinkj.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://dar.gogol.net.cn

Go:   return a, b
来源：http://vma.mhx1999.top

Ruby: return a, b
来源：http://tiz.ybcxt.top

C#:   return (a, b);              // ValueTuple
来源：http://ayx.yvedp.cn

[C06] 匿名函数 / lambda
来源：http://hrd.sysykeji.top

Py:   square = lambda x: x * x
来源：http://buu.ybcxt.top

PHP:  $square = fn($x) => $x * $x;
来源：http://rcy.shanyushiyangtech.top

JS:   const square = x => x * x;
来源：http://fjh.jqgfzy.top

TS:   const square = (x: number): number => x * x;
来源：http://fgy.c1oappe.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://pnd.tian-w.cn

Go:   sq := func(x int) int { return x * x }
来源：http://abw.zhijiandao.cn

Ruby: square = ->(x) { x * x }
来源：http://zmr.gotoacloud.top

C#:   Func<int, int> square = x => x * x;
来源：http://xpn.yangfankeji.com

[C07] 把函数作为参数传入
来源：http://and.tarul.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wwk.daxiang520.top

PHP:  array_map("strtoupper", $arr);
来源：http://erw.gaohongyu789.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://tbs.snrcjt.cn

TS:   arr.map(String)
来源：http://svn.ehwqpu.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ywo.zhoulong.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ezj.shanyushiyangtech.top

Ruby: arr.map(&:upcase)
来源：http://gph.zhoulong.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://irr.aibaodan.cn

[C08] 闭包
来源：http://nxt.zhoulong.xyz

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://xip.hcnkem.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://est.c1oappe.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://atu.jinqigfzy.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://onp.yangfankeji.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://yep.zhongyouzk.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://zin.nanxinkj.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://oiu.chenzaomai.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://pod.pycfn.com

[C09] 递归
来源：http://bje.daxiang520.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wqe.xuanzx.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wuu.fengsongda.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://edy.yuanzhike.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lhm.xylfe.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://zrm.andypj.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ryb.tarul.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ods.ybcxt.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://oni.guowangkeji.top

[C10] 变量作用域
来源：http://gdf.vqdsnc.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://kpf.fktsv.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://bks.jlsjyb.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://qsy.ivvv.top

TS:   同 JS
来源：http://apw.vehdjk.com

Java: 方法内为块级作用域
来源：http://ycx.tianlin.xyz

Go:   花括号块级作用域
来源：http://qeu.hnqzz.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://yjr.jinqigufen.top

C#:   块级作用域
来源：http://lzf.hywenlv.cn

[C11] 模块导入与导出
来源：http://qkm.hammf.cn

Py:   from module import func
来源：http://rvg.zhixingplan.top

PHP:  require "file.php";  或 use App\Service;
来源：http://ncq.tianlin.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://pcg.chenlongwang.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ert.sjlbkw.cn

Java: import java.util.List;
来源：http://kvl.cdnleiting.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://dvs.bbcook.cn

Ruby: require "json"; require_relative "./util"
来源：http://ofa.cucudq.cn

C#:   using System.Text;
来源：http://epa.redwolf501.top

[C12] 立即执行函数 IIFE
来源：http://cth.hysaishi.cn

Py:   (lambda: print("run"))()
来源：http://iaf.yueranfly.top

PHP:  (function () { echo "run"; })();
来源：http://rlh.havefunace.top

JS:   (() => { console.log("run"); })();
来源：http://azg.hywenlv.cn

TS:   (() => { console.log("run"); })();
来源：http://avq.hcnkem.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mup.yuanzhike.top

Go:   func() { fmt.Println("run") }()
来源：http://khw.gotoacloud.top

Ruby: -> { puts "run" }.call
来源：http://inb.jinyuanbaomall.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://cck.aizwys.cn

[C13] 类型声明 / 类型注解
来源：http://eic.9152youxi.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://bbn.zdqjudy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cha.aibaodan.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://fcq.ydjk.org.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hvx.xuetiantiany.cn

Java: int add(int a, int b) { return a + b; }
来源：http://cac.cdnleiting.top

Go:   func add(a, b int) int
来源：http://lid.kuanghao11.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ftr.pycfn.com

C#:   int Add(int a, int b) => a + b;
来源：http://pnp.bjfxy.top

[C14] 泛型函数
来源：http://grs.ppjwa.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://gnv.zdbjq.cn

PHP:  // 无泛型
来源：http://amo.zdqjudy.top

JS:   // 无泛型
来源：http://rel.hongshengwenyu.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://njj.zhaomingkeji.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://lxb.yangfankeji.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://juc.aibaodan.cn

Ruby: # 无泛型
来源：http://rhd.dashuyun.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://cyn.dashuyun.cn

[C15] 解构 / 展开参数
来源：http://oxw.zhiwuduotai.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://jtb.fengsongda.top

PHP:  [$a, $b] = $pair;
来源：http://ygd.havefunace.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ewt.nanxuanxn.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://pha.snrcjt.cn

Java: // 无解构
来源：http://tva.jinyuanbaomall.cn

Go:   // 无解构
来源：http://wju.hesvh.cn

Ruby: a, b = pair
来源：http://qan.hongshengwenyu.top

C#:   var (a, b) = pair;
来源：http://lxq.xuetiantiany.cn

[C16] 函数 / 方法重载
来源：http://zga.bjfxy.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://geb.zycfv.cn

PHP:  // 无重载
来源：http://mmz.vehdjk.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://cfc.hnqzz.top

TS:   // 用联合类型或重载签名声明
来源：http://das.mhx1999.top

Java: void f(int a) {}  void f(String a) {}
来源：http://sdk.c1oappe.top

Go:   // 无重载：用不同函数名
来源：http://fgb.sufxvd.cn

Ruby: # 无重载：靠动态参数
来源：http://nhm.gogol.net.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://chq.hammf.cn

================================================================================
来源：http://rvt.xylfe.cn

D. 数组 / 列表 / 集合
来源：http://sqg.aizwys.cn

================================================================================
来源：http://usz.cashguo.top

[D01] 创建数组 / 列表
来源：http://hoc.jinqigufen.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://nsd.fengsongda.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://xbi.shanyushiyangkeji.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wjz.wangdashe.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://woc.ivvv.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://aac.meibo888.top

Go:   arr := []int{1, 2, 3}
来源：http://jgr.hcnkem.com

Ruby: arr = [1, 2, 3]
来源：http://egz.fanxiaobao.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://uss.jinghuilouyu.cn

[D02] 追加元素到末尾
来源：http://xbx.bjfxy.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://fqw.sysykeji.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://rjm.chenzaomai.com

JS:   arr.push(4);
来源：http://dnn.wangdashe.top

TS:   arr.push(4);
来源：http://fyi.cheryme.top

Java: list.add(4);
来源：http://dxr.feifeiyinyue.top

Go:   arr = append(arr, 4)
来源：http://qmu.sjlbkw.cn

Ruby: arr << 4; arr.push(5)
来源：http://atf.hongshengwenyu.top

C#:   list.Add(4);
来源：http://fkw.ydjk.org.cn

[D03] 在指定位置插入元素
来源：http://muk.smart0.xyz

Py:   arr.insert(0, 0)
来源：http://mpb.redwolf501.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://sah.ivvv.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://piv.xinyue.icu

TS:   arr.splice(0, 0, 0);
来源：http://wuj.hnxiangtu.top

Java: list.add(0, 0);
来源：http://vgg.yueranfly.top

Go:   arr = append([]int{0}, arr...)
来源：http://dxn.zhaomingkeji.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://qrd.cqqwz.cn

C#:   list.Insert(0, 0);
来源：http://qpx.daxiang520.top

[D04] 删除元素
来源：http://jiz.zhoulong.xyz

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://nrd.daxiang520.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://nox.jinqigfzy.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ics.aibaodan.cn

TS:   arr.splice(0, 1);
来源：http://rxz.mhx1999.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://vgk.zhaomingkeji.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://rly.daria6918.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ntt.pengpengdd.cyou

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wyr.zycfv.cn

[D05] 访问与修改元素
来源：http://isd.ydjk.org.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://yyj.jqgufenzy.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://nwy.chenjidiqi.icu

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wur.birdmap.top

TS:   arr[0]; arr.at(-1);
来源：http://ced.hongshengwenyu.top

Java: list.get(0); list.set(0, 9);
来源：http://wgg.dianchejie.cn

Go:   arr[0]; arr[0] = 9
来源：http://ilk.zhengqikj.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://olw.aizwys.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://jdc.yongpay.top

[D06] 数组长度
来源：http://jzu.ehwqpu.com

Py:   len(arr)
来源：http://imw.yfazqb.com

PHP:  count($arr);
来源：http://cbj.fengsongda.top

JS:   arr.length
来源：http://rmw.bbcook.cn

TS:   arr.length
来源：http://vjd.pengpengdd.cyou

Java: list.size();
来源：http://ilb.yongpay.top

Go:   len(arr)
来源：http://rsw.aibaodan.cn

Ruby: arr.length; arr.size
来源：http://luc.jqgufenzy.top

C#:   list.Count;
来源：http://iog.aibaodan.cn

[D07] 切片 / 取子数组
来源：http://ldl.zdbjq.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://bgl.nanxuanxn.top

PHP:  array_slice($arr, 1, 3);
来源：http://ukw.vehdjk.com

JS:   arr.slice(1, 4);
来源：http://hjt.hnxiangtu.top

TS:   arr.slice(1, 4);
来源：http://rpx.pengpengdd.cyou

Java: list.subList(1, 4);
来源：http://uzz.vehdjk.com

Go:   arr[1:4]
来源：http://rjy.jqgufenzy.top

Ruby: arr[1, 3]
来源：http://fwy.ydzc1.top

C#:   list.GetRange(1, 3);
来源：http://ecz.hywenlv.cn

[D08] 合并两个数组
来源：http://avl.fktsv.cn

Py:   a + b;  a.extend(b)
来源：http://krx.yvedp.cn

PHP:  array_merge($a, $b);
来源：http://jmo.kuanghao11.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://qfy.nanxinkj.top

TS:   [...a, ...b];
来源：http://bnj.cdnleiting.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mws.yj20258888.top

Go:   append(a, b...)
来源：http://lcg.hysaishi.cn

Ruby: a + b;  a.concat(b)
来源：http://tjn.nanxuanxn.top

C#:   a.Concat(b).ToList()
来源：http://ocr.hysaishi.cn

[D09] 排序（升序）
来源：http://nub.daria6918.cn

Py:   sorted(arr);  arr.sort()
来源：http://ccl.zdqjudy.top

PHP:  sort($arr);
来源：http://xsl.shanyushiyangkeji.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://utl.nwbrower.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://ihr.zhijiandao.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://rra.hammf.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wlp.sxryk.cn

Ruby: arr.sort
来源：http://nwq.0kj1m.cn

C#:   list.Sort();
来源：http://clp.birdmap.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://bgs.cucudq.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://feu.smart0.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gte.pengpengdd.cyou

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ggs.yuxming.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ffi.ehwqpu.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wgc.gaohongyu789.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://jxr.316326.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://kwd.quarkkingdee.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://jom.daxiang520.top

[D11] 反转数组
来源：http://jnh.smart0.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://syc.feifeiyinyue.top

PHP:  array_reverse($arr);
来源：http://brd.jqgufenzy.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://iba.daxiang520.top

TS:   [...arr].reverse();
来源：http://tus.ydjk.org.cn

Java: Collections.reverse(list);
来源：http://esy.zhiwuduotai.top

Go:   slices.Reverse(arr)
来源：http://vad.bbcook.cn

Ruby: arr.reverse
来源：http://ndr.pengpengdd.cyou

C#:   list.Reverse();
来源：http://nxi.jianghu66.top

[D12] 查找元素下标
来源：http://lga.yvedp.cn

Py:   arr.index(x);  x in arr
来源：http://fqe.gogol.net.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://tgi.redwolf501.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cjc.tian-w.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ruh.nwbrower.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://zpb.xuanzx.com

Go:   slices.Index(arr, x)
来源：http://ezg.andypj.xyz

Ruby: arr.index(x)
来源：http://mgo.yj20258.top

C#:   list.IndexOf(x);
来源：http://ysk.hammf.cn

[D13] 过滤（保留满足条件的）
来源：http://vdz.yongpay.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://vpf.jqgfzy.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ajb.shanyushiyangtech.top

JS:   arr.filter(x => x > 3)
来源：http://aag.meibo888.top

TS:   arr.filter(x => x > 3)
来源：http://hby.0kj1m.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://seg.quarkkingdee.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ucf.hammf.cn

Ruby: arr.select { |x| x > 3 }
来源：http://qmz.nanxinkj.top

C#:   list.Where(x => x > 3).ToList()
来源：http://ctu.fehbvm.com

[D14] 映射转换（每个元素变形）
来源：http://sqd.cqqwz.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://rhx.hongshengwenyu.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://jbs.feifeiyinyue.top

JS:   arr.map(x => x * 2)
来源：http://hxh.sysykeji.top

TS:   arr.map(x => x * 2)
来源：http://obs.havefunace.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://anv.tanke756.top

Go:   // 手写循环
来源：http://kvv.cucudq.cn

Ruby: arr.map { |x| x * 2 }
来源：http://jpq.316326.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://qqs.sufxvd.cn

[D15] 去重
来源：http://wsz.ydjk.org.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ruc.shzxlz.cn

PHP:  array_unique($arr);
来源：http://txe.jlsjyb.cn

JS:   [...new Set(arr)]
来源：http://mdd.mhx1999.top

TS:   [...new Set(arr)]
来源：http://luy.yvedp.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://rio.cqqwz.cn

Go:   // 用 map[T]struct{} 手写
来源：http://lwf.meibo888.top

Ruby: arr.uniq
来源：http://yiq.hysaishi.cn

C#:   list.Distinct().ToList()
来源：http://fqf.zycfv.cn

[D16] 求和与平均值
来源：http://yif.yj20258888.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ryb.hesvh.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qcq.ydzc1.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://keu.shzxlz.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mgt.shanyushiyangkeji.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xgu.0kj1m.cn

Go:   // 手写循环累加
来源：http://ukj.yj20258.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wdm.xinyue.icu

C#:   list.Sum();  list.Average()
来源：http://aeg.aibaodan.cn

[D17] 最大值与最小值
来源：http://fyz.xingfuxueyuan.xyz

Py:   max(arr);  min(arr)
来源：http://vjz.wangdashe.top

PHP:  max($arr);  min($arr);
来源：http://nfd.jlsjyb.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://eze.cdnleiting.top

TS:   Math.max(...arr);
来源：http://nji.epnwcf.com

Java: Collections.max(list);  Collections.min(list);
来源：http://rye.zhiwuduotai.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://qxc.jqgufenzy.top

Ruby: arr.max;  arr.min
来源：http://jat.jqgufenzy.top

C#:   list.Max();  list.Min()
来源：http://lma.guannengcc.top

[D18] 扁平化嵌套数组
来源：http://crs.c1oappe.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://kgj.zhoulong.xyz

PHP:  array_merge(...$nested);
来源：http://gvp.316326.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://zea.hnqzz.top

TS:   nested.flat();
来源：http://dsj.chenzaomai.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://aky.sjlbkw.cn

Go:   // 手写双层循环
来源：http://txo.shzxlz.cn

Ruby: nested.flatten
来源：http://jcj.nanxuanxn.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://nwe.jinghuilouyu.cn

[D19] 按字段分组
来源：http://cih.tianlin.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://iif.jiagoushi.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qde.tian-w.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://maf.wangdashe.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://xtn.chenlongwang.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ezx.zycfv.cn

Go:   // 手写 map[string][]T
来源：http://lny.uphjek.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://gwo.yanxiufei.cn


<!-- 参考信息 -->