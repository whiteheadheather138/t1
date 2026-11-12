代发 wailian999

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://yya.jlsjyb.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ooz.yfazqb.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://upa.zdqjudy.top

Java: // 无：用 Builder 模式或 record
来源：http://cxj.dashuyun.cn

Go:   // 无：用配置结构体参数
来源：http://czj.ivvv.top

Ruby: f(a: 1, b: 2)
来源：http://elz.redwolf501.top

C#:   f(a: 1, b: 2)
来源：http://ywf.nanxinkj.top

[C05] 返回多个值
来源：http://znk.hesvh.cn

Py:   return a, b
来源：http://wyi.vehdjk.com

PHP:  return [$a, $b];
来源：http://ryr.yuxming.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://snq.jinqigfzy.top

TS:   return { a, b };
来源：http://xea.fehbvm.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://sqr.hnxiangtu.top

Go:   return a, b
来源：http://tsi.shanyushiyangtech.top

Ruby: return a, b
来源：http://ygx.cheryme.top

C#:   return (a, b);              // ValueTuple
来源：http://mtv.zhongyouzk.top

[C06] 匿名函数 / lambda
来源：http://eaw.wangshuangyany.cn

Py:   square = lambda x: x * x
来源：http://xea.gogol.net.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://arj.cucudq.cn

JS:   const square = x => x * x;
来源：http://eqh.gotoacloud.top

TS:   const square = (x: number): number => x * x;
来源：http://rdu.jinghuilouyu.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://par.zhongyouzk.top

Go:   sq := func(x int) int { return x * x }
来源：http://pze.jlsjyb.cn

Ruby: square = ->(x) { x * x }
来源：http://mhc.bjfxy.top

C#:   Func<int, int> square = x => x * x;
来源：http://qdy.zhengqikj.top

[C07] 把函数作为参数传入
来源：http://len.iojbl.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://vfu.zhongyouzk.top

PHP:  array_map("strtoupper", $arr);
来源：http://ert.gogol.net.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://iom.zdqjudy.top

TS:   arr.map(String)
来源：http://jai.ywan-chungtsiang.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://bsj.yj202588.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://zab.redwolf501.top

Ruby: arr.map(&:upcase)
来源：http://iop.yvedp.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://krj.hysaishi.cn

[C08] 闭包
来源：http://cug.pengpengdd.cyou

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://oot.zhiwuduotai.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mfl.hywenlv.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://fev.zdbjq.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://pfs.bjfxy.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://biy.sjlbkw.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hwn.ivvv.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://xiw.jqgufenzy.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://lsu.jyoumei.cn

[C09] 递归
来源：http://fat.zdbjq.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://gfm.aizwys.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://bvd.yueranfly.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rom.fanxiaobao.xyz

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zvm.yvedp.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://krj.fanxiaobao.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mtd.ybcxt.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ian.jianghu66.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://luk.quarkkingdee.top

[C10] 变量作用域
来源：http://klk.ybcxt.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://jmf.jqgufenzy.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://zqp.aizwys.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wrs.hysaishi.cn

TS:   同 JS
来源：http://gxh.zhixingplan.top

Java: 方法内为块级作用域
来源：http://yrb.yj20258888.top

Go:   花括号块级作用域
来源：http://qzj.pengpengdd.cyou

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://gej.jinqigufen.top

C#:   块级作用域
来源：http://fna.zhengqikj.top

[C11] 模块导入与导出
来源：http://nlf.ydzc1.top

Py:   from module import func
来源：http://bpq.sjlbkw.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://xbv.meibo888.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://ler.hfpthk.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ftg.ywan-chungtsiang.top

Java: import java.util.List;
来源：http://qbc.nwbrower.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://oue.nwbrower.top

Ruby: require "json"; require_relative "./util"
来源：http://lbs.vqdsnc.cn

C#:   using System.Text;
来源：http://cte.daria6918.cn

[C12] 立即执行函数 IIFE
来源：http://kcy.chenjidiqi.icu

Py:   (lambda: print("run"))()
来源：http://oja.hywenlv.cn

PHP:  (function () { echo "run"; })();
来源：http://vcg.jqgfzy.top

JS:   (() => { console.log("run"); })();
来源：http://axn.wangdashe.top

TS:   (() => { console.log("run"); })();
来源：http://scv.yuanzhike.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jbt.guannengcc.top

Go:   func() { fmt.Println("run") }()
来源：http://gmd.xinyue.icu

Ruby: -> { puts "run" }.call
来源：http://odb.zhongyouzk.top

C#:   // 无 IIFE：用静态构造函数
来源：http://lvr.shzxlz.cn

[C13] 类型声明 / 类型注解
来源：http://fqj.zhengqikj.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://yci.jqgufenzy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rby.nanxuanxn.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://vhu.shanyushiyangkeji.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jhv.haohaochexian.top

Java: int add(int a, int b) { return a + b; }
来源：http://kmv.jinghuilouyu.cn

Go:   func add(a, b int) int
来源：http://zkr.zhongyouzk.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://rpf.cdnleiting.top

C#:   int Add(int a, int b) => a + b;
来源：http://wpx.vehdjk.com

[C14] 泛型函数
来源：http://cry.ivvv.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mok.xuanzx.com

PHP:  // 无泛型
来源：http://hov.chenzaomai.com

JS:   // 无泛型
来源：http://hff.xingfuxueyuan.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://jyy.bbcook.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://sni.sufxvd.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://svd.yonumen.top

Ruby: # 无泛型
来源：http://cgv.sxryk.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://kcl.hammf.cn

[C15] 解构 / 展开参数
来源：http://asf.xziqi.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://udx.hammf.cn

PHP:  [$a, $b] = $pair;
来源：http://qxt.nwbrower.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://vjq.zdqjudy.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://axe.meibo888.top

Java: // 无解构
来源：http://urp.chenjidiqi.icu

Go:   // 无解构
来源：http://wuz.snrcjt.cn

Ruby: a, b = pair
来源：http://yyo.fzhhl.top

C#:   var (a, b) = pair;
来源：http://onn.gotoacloud.top

[C16] 函数 / 方法重载
来源：http://pdk.yj20258.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://dpq.bbcook.cn

PHP:  // 无重载
来源：http://ghk.zhaomingkeji.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://ykj.yuxming.cn

TS:   // 用联合类型或重载签名声明
来源：http://ist.jinqigufen.top

Java: void f(int a) {}  void f(String a) {}
来源：http://bqv.pengpengdd.cyou

Go:   // 无重载：用不同函数名
来源：http://ols.hesvh.cn

Ruby: # 无重载：靠动态参数
来源：http://qzp.sysykeji.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://yqg.shangyingyoupin.top

================================================================================
来源：http://cun.zhixingplan.top

D. 数组 / 列表 / 集合
来源：http://meg.shuidangran.top

================================================================================
来源：http://nkq.shanyushiyangkeji.top

[D01] 创建数组 / 列表
来源：http://rtm.shanyushiyangtech.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://syo.smart0.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://jom.cucudq.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://slj.cdnleiting.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://pbj.redwolf501.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://rml.gzhubu.top

Go:   arr := []int{1, 2, 3}
来源：http://bsa.cheryme.top

Ruby: arr = [1, 2, 3]
来源：http://xpz.cdnleiting.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ahd.xuetiantiany.cn

[D02] 追加元素到末尾
来源：http://znm.nwbrower.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://msq.jqgufenzy.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://rez.dashuyun.cn

JS:   arr.push(4);
来源：http://nuw.epnwcf.com

TS:   arr.push(4);
来源：http://xol.jlsjyb.cn

Java: list.add(4);
来源：http://uva.daxiang520.top

Go:   arr = append(arr, 4)
来源：http://mxy.mhx1999.top

Ruby: arr << 4; arr.push(5)
来源：http://mrk.jinyuanbaomall.cn

C#:   list.Add(4);
来源：http://fkq.gzhubu.top

[D03] 在指定位置插入元素
来源：http://bdf.meibo888.top

Py:   arr.insert(0, 0)
来源：http://fro.tianlin.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://vzc.tianlin.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ulq.yj202588.top

TS:   arr.splice(0, 0, 0);
来源：http://ppw.shuidangran.top

Java: list.add(0, 0);
来源：http://hmc.chenzaomai.com

Go:   arr = append([]int{0}, arr...)
来源：http://bew.fanxiaobao.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wzw.cucudq.cn

C#:   list.Insert(0, 0);
来源：http://yss.ydzc1.top

[D04] 删除元素
来源：http://zol.zhixingplan.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://fry.cdnleiting.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://fza.wangshuangyany.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xub.yongpay.top

TS:   arr.splice(0, 1);
来源：http://qbn.zhiwuduotai.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://qwv.jlsjyb.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://kwp.jinghuilouyu.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://rpo.birdmap.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://yka.birdmap.top

[D05] 访问与修改元素
来源：http://pbg.cashguo.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://gvn.sxryk.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://asm.hammf.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://brn.wangshuangyany.cn

TS:   arr[0]; arr.at(-1);
来源：http://mse.yj20258.top

Java: list.get(0); list.set(0, 9);
来源：http://ijr.shanyushiyangkeji.top

Go:   arr[0]; arr[0] = 9
来源：http://rui.hnxiangtu.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://dwo.chenzaomai.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://qzp.ydzc1.top

[D06] 数组长度
来源：http://zko.ctjpmb.com

Py:   len(arr)
来源：http://tms.yongpay.top

PHP:  count($arr);
来源：http://wam.zhixingplan.top

JS:   arr.length
来源：http://qsp.316326.xyz

TS:   arr.length
来源：http://cwn.fzhhl.top

Java: list.size();
来源：http://pbk.xziqi.cn

Go:   len(arr)
来源：http://exz.zhongyouzk.top

Ruby: arr.length; arr.size
来源：http://lem.zhengqikj.top

C#:   list.Count;
来源：http://qta.zhijiandao.cn

[D07] 切片 / 取子数组
来源：http://tas.jyoumei.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://whl.andypj.xyz

PHP:  array_slice($arr, 1, 3);
来源：http://fho.hammf.cn

JS:   arr.slice(1, 4);
来源：http://snw.zhaomingkeji.xyz

TS:   arr.slice(1, 4);
来源：http://uru.xingfuxueyuan.xyz

Java: list.subList(1, 4);
来源：http://exo.ybcxt.top

Go:   arr[1:4]
来源：http://psq.fanxiaobao.xyz

Ruby: arr[1, 3]
来源：http://ptd.ctjpmb.com

C#:   list.GetRange(1, 3);
来源：http://obc.dianchejie.cn

[D08] 合并两个数组
来源：http://ezi.sysykeji.top

Py:   a + b;  a.extend(b)
来源：http://bfb.ctjpmb.com

PHP:  array_merge($a, $b);
来源：http://sgr.jlsjyb.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://jxg.ehwqpu.com

TS:   [...a, ...b];
来源：http://onf.xingfuxueyuan.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://owk.jqgfzy.top

Go:   append(a, b...)
来源：http://dqp.daria6918.cn

Ruby: a + b;  a.concat(b)
来源：http://yeo.yuxming.cn

C#:   a.Concat(b).ToList()
来源：http://mhg.yueranfly.top

[D09] 排序（升序）
来源：http://mfp.hnqzz.top

Py:   sorted(arr);  arr.sort()
来源：http://wqi.hywenlv.cn

PHP:  sort($arr);
来源：http://jvh.pengpengdd.cyou

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://yar.jqgufenzy.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://dyp.shanyushiyangtech.top

Java: Collections.sort(list);  list.sort(null);
来源：http://rld.jqgfzy.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://aju.zhijiandao.cn

Ruby: arr.sort
来源：http://jca.sweek.top

C#:   list.Sort();
来源：http://sul.andypj.xyz

[D10] 自定义排序（按字段 / 多条件）
来源：http://vwm.fanxiaobao.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://pfz.chenjidiqi.icu

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xvr.sweek.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://pjo.hammf.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://oti.cucudq.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://pmh.epnwcf.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://veu.cashguo.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hqm.jinyuanbaomall.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://yyx.yanxiufei.cn

[D11] 反转数组
来源：http://xwm.jinyuanbaomall.cn

Py:   arr[::-1];  arr.reverse()
来源：http://pwh.yuanzhike.top

PHP:  array_reverse($arr);
来源：http://dzw.chenjidiqi.icu

JS:   [...arr].reverse();  arr.toReversed()
来源：http://tqu.chenlongwang.top

TS:   [...arr].reverse();
来源：http://xet.iojbl.cn

Java: Collections.reverse(list);
来源：http://jar.zhiwuduotai.top

Go:   slices.Reverse(arr)
来源：http://kna.redwolf501.top

Ruby: arr.reverse
来源：http://pen.0kj1m.cn

C#:   list.Reverse();
来源：http://qly.gzhubu.top

[D12] 查找元素下标
来源：http://ork.316326.xyz

Py:   arr.index(x);  x in arr
来源：http://mmu.yvedp.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://loh.xinyue.icu

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kcr.vqdsnc.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fdt.gotoacloud.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://bfu.ydzc1.top

Go:   slices.Index(arr, x)
来源：http://zml.zhengqikj.top

Ruby: arr.index(x)
来源：http://nzd.yj20258.top

C#:   list.IndexOf(x);
来源：http://yhp.shuidangran.top

[D13] 过滤（保留满足条件的）
来源：http://eor.yuxming.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://vgz.sxryk.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://xqa.guowangkeji.top

JS:   arr.filter(x => x > 3)
来源：http://vui.haohaochexian.top

TS:   arr.filter(x => x > 3)
来源：http://aee.jinghuilouyu.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://nbx.gogol.net.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://zsg.havefunace.top

Ruby: arr.select { |x| x > 3 }
来源：http://uac.xylfe.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://sps.tanke756.top

[D14] 映射转换（每个元素变形）
来源：http://dla.snrcjt.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://bob.tarul.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://cna.yangfankeji.com

JS:   arr.map(x => x * 2)
来源：http://jjc.ehwqpu.com

TS:   arr.map(x => x * 2)
来源：http://oxw.cdnleiting.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://bhe.xziqi.cn

Go:   // 手写循环
来源：http://dnx.ehwqpu.com

Ruby: arr.map { |x| x * 2 }
来源：http://hop.vqdsnc.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://izu.yonumen.top

[D15] 去重
来源：http://hvc.yj202588.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://enk.yvedp.cn

PHP:  array_unique($arr);
来源：http://bvb.chenjidiqi.icu

JS:   [...new Set(arr)]
来源：http://kgg.sufxvd.cn

TS:   [...new Set(arr)]
来源：http://aps.haohaochexian.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://lgn.yueranfly.top

Go:   // 用 map[T]struct{} 手写
来源：http://sfo.jlsjyb.cn

Ruby: arr.uniq
来源：http://iye.cqqwz.cn

C#:   list.Distinct().ToList()
来源：http://ynn.jinqigufen.top

[D16] 求和与平均值
来源：http://ztv.zhixingplan.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://dgj.hammf.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://gmd.cashguo.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://iuk.gotoacloud.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://edz.cashguo.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://tcw.aizwys.cn

Go:   // 手写循环累加
来源：http://ssg.jiagoushi.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mhb.tanke756.top

C#:   list.Sum();  list.Average()
来源：http://qab.uphjek.com

[D17] 最大值与最小值
来源：http://hxt.hammf.cn

Py:   max(arr);  min(arr)
来源：http://lph.pengpengdd.cyou

PHP:  max($arr);  min($arr);
来源：http://was.vqdsnc.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://het.yj202588.top

TS:   Math.max(...arr);
来源：http://fvf.hammf.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://sbj.hysaishi.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://gmk.xinyue.icu

Ruby: arr.max;  arr.min
来源：http://ghh.gotoacloud.top

C#:   list.Max();  list.Min()
来源：http://wzv.yongpay.top

[D18] 扁平化嵌套数组
来源：http://bze.aizwys.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://kxb.quarkkingdee.top

PHP:  array_merge(...$nested);
来源：http://ttx.cucudq.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://tmz.316326.xyz

TS:   nested.flat();
来源：http://aer.hnqzz.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wou.shanyushiyangkeji.top

Go:   // 手写双层循环
来源：http://wxh.fzhhl.top

Ruby: nested.flatten
来源：http://how.yuxming.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://hgw.ydjk.org.cn

[D19] 按字段分组
来源：http://woo.yj20258.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://qwr.zhixingplan.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://cyx.yonumen.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://zqy.jinghuilouyu.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://quv.chenzaomai.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://zoa.cheryme.top

Go:   // 手写 map[string][]T
来源：http://mte.xziqi.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://eru.epnwcf.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://pux.jinqigufen.top

[D20] 统计每个元素出现次数
来源：http://ikx.cucudq.cn

Py:   Counter(arr)
来源：http://fna.dianchejie.cn

PHP:  array_count_values($arr);
来源：http://vit.ydjk.org.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hfl.ctjpmb.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xhd.hcnkem.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://qgq.xylfe.cn

Go:   // 手写 map[T]int
来源：http://ibk.tian-w.cn

Ruby: arr.tally
来源：http://bhy.ppjwa.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://dgl.fengsongda.top

[D21] 判断是否包含某元素
来源：http://tbr.dashuyun.cn

Py:   x in arr
来源：http://fkw.gaohongyu789.top


<!-- 参考信息 -->