代发 wailian999

C#:   string Greet(string name = "World") => name;
来源：http://pnr.sufxvd.cn

[C03] 可变参数
来源：http://ezj.birdmap.top

Py:   def total(*args): return sum(args)
来源：http://gik.hcnkem.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://tsr.gzhubu.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://una.jinqigfzy.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://poh.yj202588.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ztx.aizwys.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://xhn.xingfuxueyuan.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://vnd.hammf.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wcs.andypj.xyz

[C04] 命名参数 / 关键字参数
来源：http://obk.uphjek.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://usm.uphjek.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://yrf.dianchejie.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://lbo.nanxinkj.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://bmg.0kj1m.cn

Java: // 无：用 Builder 模式或 record
来源：http://btr.fzhhl.top

Go:   // 无：用配置结构体参数
来源：http://kkv.zhixingplan.top

Ruby: f(a: 1, b: 2)
来源：http://dzw.jinghuilouyu.cn

C#:   f(a: 1, b: 2)
来源：http://bua.tarul.cn

[C05] 返回多个值
来源：http://npo.hongshengwenyu.top

Py:   return a, b
来源：http://rmr.shuidangran.top

PHP:  return [$a, $b];
来源：http://xmn.iojbl.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://zog.fengsongda.top

TS:   return { a, b };
来源：http://pdf.tian-w.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://grw.gaohongyu789.top

Go:   return a, b
来源：http://wgt.hfpthk.cn

Ruby: return a, b
来源：http://jbl.fzhhl.top

C#:   return (a, b);              // ValueTuple
来源：http://ozp.tianlin.xyz

[C06] 匿名函数 / lambda
来源：http://khp.hnqzz.top

Py:   square = lambda x: x * x
来源：http://smv.redwolf501.top

PHP:  $square = fn($x) => $x * $x;
来源：http://tag.cashguo.top

JS:   const square = x => x * x;
来源：http://jnu.nanxuanxn.top

TS:   const square = (x: number): number => x * x;
来源：http://eif.hcnkem.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://tdy.chenjidiqi.icu

Go:   sq := func(x int) int { return x * x }
来源：http://anu.hammf.cn

Ruby: square = ->(x) { x * x }
来源：http://lys.uphjek.com

C#:   Func<int, int> square = x => x * x;
来源：http://rkb.feifeiyinyue.top

[C07] 把函数作为参数传入
来源：http://wvd.shangyingyoupin.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://vwf.zdbjq.cn

PHP:  array_map("strtoupper", $arr);
来源：http://veo.0kj1m.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://bfn.316326.xyz

TS:   arr.map(String)
来源：http://hab.vehdjk.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://qap.jyoumei.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wvh.yj202588.top

Ruby: arr.map(&:upcase)
来源：http://vrc.zhiwuduotai.top

C#:   arr.Select(s => s.ToUpper())
来源：http://aqw.yj20258.top

[C08] 闭包
来源：http://rlv.ehwqpu.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://rnq.shanyushiyangkeji.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://gow.gotoacloud.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://iok.uphjek.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://aha.hcnkem.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://fyt.sxryk.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://xzf.sysykeji.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://vyb.jqgfzy.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ujl.xziqi.cn

[C09] 递归
来源：http://wyo.hywenlv.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://gmp.jyoumei.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://zub.jianghu66.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://imc.kuanghao11.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ouw.ywan-chungtsiang.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://tmj.ivvv.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://gtb.pycfn.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://otz.ybcxt.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://uub.yvedp.cn

[C10] 变量作用域
来源：http://jel.jianghu66.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wmb.yonumen.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://bfq.epnwcf.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://phq.bbcook.cn

TS:   同 JS
来源：http://mzl.xuanzx.com

Java: 方法内为块级作用域
来源：http://asl.birdmap.top

Go:   花括号块级作用域
来源：http://kca.yuanzhike.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://exu.pengpengdd.cyou

C#:   块级作用域
来源：http://npt.fzhhl.top

[C11] 模块导入与导出
来源：http://ori.daxiang520.top

Py:   from module import func
来源：http://opo.ydzc1.top

PHP:  require "file.php";  或 use App\Service;
来源：http://eex.shanyushiyangtech.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://lqt.zhongyouzk.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://pbj.52xcode.cn

Java: import java.util.List;
来源：http://byu.yanxiufei.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://zyp.ybcxt.top

Ruby: require "json"; require_relative "./util"
来源：http://roa.cqqwz.cn

C#:   using System.Text;
来源：http://ake.fanxiaobao.xyz

[C12] 立即执行函数 IIFE
来源：http://mur.hongshengwenyu.top

Py:   (lambda: print("run"))()
来源：http://skg.zhixingplan.top

PHP:  (function () { echo "run"; })();
来源：http://xkz.fehbvm.com

JS:   (() => { console.log("run"); })();
来源：http://zcg.hfpthk.cn

TS:   (() => { console.log("run"); })();
来源：http://rji.svipenyu.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://lem.316326.xyz

Go:   func() { fmt.Println("run") }()
来源：http://abp.hongshengwenyu.top

Ruby: -> { puts "run" }.call
来源：http://dbq.52xcode.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://hvf.pycfn.com

[C13] 类型声明 / 类型注解
来源：http://bhl.xylfe.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wde.zhengqikj.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jyb.xinyue.icu

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ntw.shanyushiyangtech.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dvy.tianlin.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://avt.sxryk.cn

Go:   func add(a, b int) int
来源：http://ahs.yongpay.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hom.vehdjk.com

C#:   int Add(int a, int b) => a + b;
来源：http://ozr.hongshengwenyu.top

[C14] 泛型函数
来源：http://cgi.nanxinkj.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://dtg.fktsv.cn

PHP:  // 无泛型
来源：http://ilw.sweek.top

JS:   // 无泛型
来源：http://apl.xinyue.icu

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://zez.bjfxy.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://gni.daria6918.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://pls.cdnleiting.top

Ruby: # 无泛型
来源：http://edd.gaohongyu789.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://uct.jianghu66.top

[C15] 解构 / 展开参数
来源：http://ecc.redwolf501.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://zqp.ehwqpu.com

PHP:  [$a, $b] = $pair;
来源：http://ufe.birdmap.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xhs.nwbrower.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://coq.ehwqpu.com

Java: // 无解构
来源：http://xuw.zdbjq.cn

Go:   // 无解构
来源：http://iux.smart0.xyz

Ruby: a, b = pair
来源：http://xiv.vehdjk.com

C#:   var (a, b) = pair;
来源：http://xxd.shanyushiyangkeji.top

[C16] 函数 / 方法重载
来源：http://ojm.jinghuilouyu.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://cxt.ivvv.top

PHP:  // 无重载
来源：http://znj.fehbvm.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://aih.nanxinkj.top

TS:   // 用联合类型或重载签名声明
来源：http://txu.sufxvd.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://fzu.zhoulong.xyz

Go:   // 无重载：用不同函数名
来源：http://csu.ctjpmb.com

Ruby: # 无重载：靠动态参数
来源：http://ufw.yfazqb.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://uol.yueranfly.top

================================================================================
来源：http://xpy.zhaomingkeji.xyz

D. 数组 / 列表 / 集合
来源：http://iyw.xylfe.cn

================================================================================
来源：http://mjo.shanyushiyangtech.top

[D01] 创建数组 / 列表
来源：http://jfe.jinyuanbaomall.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://aww.jiagoushi.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://zaq.pycfn.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://zgk.shangyingyoupin.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://ngv.smart0.xyz

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://xcq.zdqjudy.top

Go:   arr := []int{1, 2, 3}
来源：http://esh.yfazqb.com

Ruby: arr = [1, 2, 3]
来源：http://vpc.zhijiandao.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://xqo.hysaishi.cn

[D02] 追加元素到末尾
来源：http://bbr.iojbl.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://vtt.shzxlz.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://nhm.jlsjyb.cn

JS:   arr.push(4);
来源：http://ubm.yonumen.top

TS:   arr.push(4);
来源：http://wli.fzhhl.top

Java: list.add(4);
来源：http://ein.sweek.top

Go:   arr = append(arr, 4)
来源：http://edu.xziqi.cn

Ruby: arr << 4; arr.push(5)
来源：http://kmd.yueranfly.top

C#:   list.Add(4);
来源：http://lia.zhongyouzk.top

[D03] 在指定位置插入元素
来源：http://lwg.guowangkeji.top

Py:   arr.insert(0, 0)
来源：http://xoi.ehwqpu.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://tvz.fzhhl.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://dsn.yuanzhike.top

TS:   arr.splice(0, 0, 0);
来源：http://gdw.kuanghao11.cn

Java: list.add(0, 0);
来源：http://wvr.hfpthk.cn

Go:   arr = append([]int{0}, arr...)
来源：http://sur.jyoumei.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://sod.xuanzx.com

C#:   list.Insert(0, 0);
来源：http://obb.ehwqpu.com

[D04] 删除元素
来源：http://wgr.meibo888.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://kpi.hfpthk.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ssz.hnqzz.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://jaf.fktsv.cn

TS:   arr.splice(0, 1);
来源：http://zhz.wangdashe.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ejf.fengsongda.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://gby.zdbjq.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://kiw.gaohongyu789.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://bsk.haohaochexian.top

[D05] 访问与修改元素
来源：http://qeq.yangfankeji.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://rkn.ctjpmb.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://lvd.gaohongyu789.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://fpa.gogol.net.cn

TS:   arr[0]; arr.at(-1);
来源：http://kxm.shangyingyoupin.top

Java: list.get(0); list.set(0, 9);
来源：http://ujc.cucudq.cn

Go:   arr[0]; arr[0] = 9
来源：http://hgu.ctjpmb.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://raa.ivvv.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ftu.9152youxi.cn

[D06] 数组长度
来源：http://dhe.cdnleiting.top

Py:   len(arr)
来源：http://pko.shangyingyoupin.top

PHP:  count($arr);
来源：http://vsr.jiagoushi.top

JS:   arr.length
来源：http://dsl.ybcxt.top

TS:   arr.length
来源：http://odz.hammf.cn

Java: list.size();
来源：http://xea.zycfv.cn

Go:   len(arr)
来源：http://oaj.jinqigufen.top

Ruby: arr.length; arr.size
来源：http://wlo.yj20258.top

C#:   list.Count;
来源：http://iep.sweek.top

[D07] 切片 / 取子数组
来源：http://oif.zhiwuduotai.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://pbc.vqdsnc.cn

PHP:  array_slice($arr, 1, 3);
来源：http://jgy.fanxiaobao.xyz

JS:   arr.slice(1, 4);
来源：http://vsl.chenjidiqi.icu

TS:   arr.slice(1, 4);
来源：http://grr.xinyue.icu

Java: list.subList(1, 4);
来源：http://dlw.xuanzx.com

Go:   arr[1:4]
来源：http://lin.zhaomingkeji.xyz

Ruby: arr[1, 3]
来源：http://ppx.hnxiangtu.top

C#:   list.GetRange(1, 3);
来源：http://zif.yj20258888.top

[D08] 合并两个数组
来源：http://olj.ehwqpu.com

Py:   a + b;  a.extend(b)
来源：http://nhn.tianlin.xyz

PHP:  array_merge($a, $b);
来源：http://got.dianchejie.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://sxy.gotoacloud.top

TS:   [...a, ...b];
来源：http://ezd.yuxming.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://xdj.fengsongda.top

Go:   append(a, b...)
来源：http://ruq.yj202588.top

Ruby: a + b;  a.concat(b)
来源：http://jwv.haohaochexian.top

C#:   a.Concat(b).ToList()
来源：http://fzq.chenzaomai.com

[D09] 排序（升序）
来源：http://kox.shzxlz.cn

Py:   sorted(arr);  arr.sort()
来源：http://znu.snrcjt.cn

PHP:  sort($arr);
来源：http://gul.xuetiantiany.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://lum.hnxiangtu.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://ddk.pengpengdd.cyou

Java: Collections.sort(list);  list.sort(null);
来源：http://ruf.gogol.net.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ysp.xinyue.icu

Ruby: arr.sort
来源：http://dwl.sxryk.cn

C#:   list.Sort();
来源：http://zwd.feifeiyinyue.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://vjc.yuanzhike.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wun.gaohongyu789.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nnw.meibo888.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://vih.wangshuangyany.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fvx.sweek.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://etn.jinqigfzy.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://spt.hywenlv.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://uir.fzhhl.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wzv.redwolf501.top

[D11] 反转数组
来源：http://ebl.yanxiufei.cn

Py:   arr[::-1];  arr.reverse()
来源：http://pqd.jqgfzy.top

PHP:  array_reverse($arr);
来源：http://tdf.ivvv.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://yhj.jqgfzy.top

TS:   [...arr].reverse();
来源：http://zbq.gzhubu.top

Java: Collections.reverse(list);
来源：http://rlw.hfpthk.cn

Go:   slices.Reverse(arr)
来源：http://pey.mhx1999.top

Ruby: arr.reverse
来源：http://xhn.wangshuangyany.cn

C#:   list.Reverse();
来源：http://ujf.bbcook.cn

[D12] 查找元素下标
来源：http://ekz.jianghu66.top

Py:   arr.index(x);  x in arr
来源：http://iaz.aibaodan.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://txv.yj20258.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wqz.cheryme.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xdc.hysaishi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mlh.fengsongda.top

Go:   slices.Index(arr, x)
来源：http://zzr.haohaochexian.top

Ruby: arr.index(x)
来源：http://rse.zycfv.cn

C#:   list.IndexOf(x);
来源：http://mlu.tarul.cn

[D13] 过滤（保留满足条件的）
来源：http://xql.zhixingplan.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ihf.hnxiangtu.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://tdn.52xcode.cn

JS:   arr.filter(x => x > 3)
来源：http://dde.ctjpmb.com

TS:   arr.filter(x => x > 3)
来源：http://dsv.c1oappe.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://jxi.gogol.net.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://kql.jinqigfzy.top

Ruby: arr.select { |x| x > 3 }
来源：http://xxo.feifeiyinyue.top

C#:   list.Where(x => x > 3).ToList()
来源：http://mnk.zhongyouzk.top

[D14] 映射转换（每个元素变形）
来源：http://pak.xziqi.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://rpc.daxiang520.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://tkz.zhoulong.xyz

JS:   arr.map(x => x * 2)
来源：http://piz.andypj.xyz

TS:   arr.map(x => x * 2)
来源：http://qmz.xuetiantiany.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://uqi.tianlin.xyz

Go:   // 手写循环
来源：http://dvz.jinqigufen.top

Ruby: arr.map { |x| x * 2 }
来源：http://des.ywan-chungtsiang.top

C#:   list.Select(x => x * 2).ToList()
来源：http://rry.zhijiandao.cn

[D15] 去重
来源：http://yyl.pengpengdd.cyou

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://kot.jinqigfzy.top

PHP:  array_unique($arr);
来源：http://aak.yueranfly.top

JS:   [...new Set(arr)]
来源：http://vzo.hesvh.cn

TS:   [...new Set(arr)]
来源：http://prc.ppjwa.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://sdv.jinqigfzy.top

Go:   // 用 map[T]struct{} 手写
来源：http://yfs.cheryme.top

Ruby: arr.uniq
来源：http://bnz.quarkkingdee.top

C#:   list.Distinct().ToList()
来源：http://plw.cucudq.cn

[D16] 求和与平均值
来源：http://kgd.guannengcc.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wxj.mhx1999.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://elz.xziqi.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://khf.bbcook.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://cvw.cashguo.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://jju.nanxinkj.top

Go:   // 手写循环累加
来源：http://qeo.hfpthk.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://pfn.jlsjyb.cn

C#:   list.Sum();  list.Average()
来源：http://lbq.vqdsnc.cn

[D17] 最大值与最小值
来源：http://jic.zhiwuduotai.top

Py:   max(arr);  min(arr)
来源：http://qve.pengpengdd.cyou

PHP:  max($arr);  min($arr);
来源：http://twb.ydzc1.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://cqm.jqgufenzy.top

TS:   Math.max(...arr);
来源：http://shl.zhiwuduotai.top

Java: Collections.max(list);  Collections.min(list);
来源：http://skk.yvedp.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://btn.aizwys.cn

Ruby: arr.max;  arr.min
来源：http://rpq.nanxuanxn.top

C#:   list.Max();  list.Min()
来源：http://tin.cucudq.cn

[D18] 扁平化嵌套数组
来源：http://izp.andypj.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ofx.mhx1999.top

PHP:  array_merge(...$nested);
来源：http://gwv.ppjwa.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://vqk.hnxiangtu.top

TS:   nested.flat();
来源：http://wyi.zhoulong.xyz

Java: nested.stream().flatMap(List::stream).toList()
来源：http://nox.wangdashe.top

Go:   // 手写双层循环
来源：http://ghp.zhoulong.xyz

Ruby: nested.flatten
来源：http://wzs.gaohongyu789.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://lsh.bjfxy.top

[D19] 按字段分组
来源：http://xko.dashuyun.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://tjd.hesvh.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://cjz.shanyushiyangtech.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hjo.yj20258.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://vxq.daxiang520.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://fbj.zycfv.cn

Go:   // 手写 map[string][]T
来源：http://fkt.ywan-chungtsiang.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://yze.xingfuxueyuan.xyz


<!-- 参考信息 -->