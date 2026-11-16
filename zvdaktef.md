代发 wailian999

C#:   string Greet(string name = "World") => name;
来源：http://ojj.gaohongyu789.top

[C03] 可变参数
来源：http://sko.zhaomingkeji.xyz

Py:   def total(*args): return sum(args)
来源：http://fhi.pycfn.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://gao.aibaodan.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mbm.ydzc1.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://oef.fzhhl.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://uqz.yanxiufei.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://dya.yuanzhike.top

Ruby: def total(*nums); nums.sum; end
来源：http://sxa.hysaishi.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://frm.yj20258888.top

[C04] 命名参数 / 关键字参数
来源：http://rht.yj20258.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://uuh.chenjidiqi.icu

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://neu.zdqjudy.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ktw.cucudq.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xeo.quarkkingdee.top

Java: // 无：用 Builder 模式或 record
来源：http://ssb.birdmap.top

Go:   // 无：用配置结构体参数
来源：http://qdv.fzhhl.top

Ruby: f(a: 1, b: 2)
来源：http://ftu.havefunace.top

C#:   f(a: 1, b: 2)
来源：http://ldy.epnwcf.com

[C05] 返回多个值
来源：http://rqs.vehdjk.com

Py:   return a, b
来源：http://mvm.shanyushiyangtech.top

PHP:  return [$a, $b];
来源：http://gkq.fehbvm.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://egp.cqqwz.cn

TS:   return { a, b };
来源：http://ybu.iojbl.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://cgx.jqgfzy.top

Go:   return a, b
来源：http://wgt.fktsv.cn

Ruby: return a, b
来源：http://uwh.yj202588.top

C#:   return (a, b);              // ValueTuple
来源：http://znq.kuanghao11.cn

[C06] 匿名函数 / lambda
来源：http://khj.shanyushiyangkeji.top

Py:   square = lambda x: x * x
来源：http://ago.fzhhl.top

PHP:  $square = fn($x) => $x * $x;
来源：http://lkt.birdmap.top

JS:   const square = x => x * x;
来源：http://imo.epnwcf.com

TS:   const square = (x: number): number => x * x;
来源：http://ric.hnxiangtu.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://icd.pengpengdd.cyou

Go:   sq := func(x int) int { return x * x }
来源：http://lyk.jianghu66.top

Ruby: square = ->(x) { x * x }
来源：http://aqo.gaohongyu789.top

C#:   Func<int, int> square = x => x * x;
来源：http://hfy.guannengcc.top

[C07] 把函数作为参数传入
来源：http://uqn.zhiwuduotai.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://fet.vehdjk.com

PHP:  array_map("strtoupper", $arr);
来源：http://gzg.nanxinkj.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://zyk.daxiang520.top

TS:   arr.map(String)
来源：http://rxj.dashuyun.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ana.pycfn.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hjm.bjfxy.top

Ruby: arr.map(&:upcase)
来源：http://vlj.svipenyu.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ogf.jqgufenzy.top

[C08] 闭包
来源：http://vng.ppjwa.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://tdp.tian-w.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://nyx.yj202588.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vlp.pengpengdd.cyou

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://buh.yangfankeji.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://dou.zdbjq.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://pzw.zhixingplan.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ktd.yonumen.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://rye.hnxiangtu.top

[C09] 递归
来源：http://lhq.meibo888.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://fvi.redwolf501.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ycg.shuidangran.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mub.shangyingyoupin.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zdh.ehwqpu.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://occ.xinyue.icu

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://nnh.shanyushiyangtech.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://cdw.jqgufenzy.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ugm.yvedp.cn

[C10] 变量作用域
来源：http://ljj.gogol.net.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://awy.dianchejie.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ajw.jiagoushi.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wry.guannengcc.top

TS:   同 JS
来源：http://cde.chenzaomai.com

Java: 方法内为块级作用域
来源：http://lje.snrcjt.cn

Go:   花括号块级作用域
来源：http://hcz.dashuyun.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wtj.tanke756.top

C#:   块级作用域
来源：http://zqe.nanxuanxn.top

[C11] 模块导入与导出
来源：http://jxh.yj20258.top

Py:   from module import func
来源：http://yre.zdbjq.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://klw.quarkkingdee.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://qzm.fengsongda.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://gsp.jinqigfzy.top

Java: import java.util.List;
来源：http://nmw.shuidangran.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://net.vehdjk.com

Ruby: require "json"; require_relative "./util"
来源：http://okw.xuetiantiany.cn

C#:   using System.Text;
来源：http://hqz.cucudq.cn

[C12] 立即执行函数 IIFE
来源：http://sgf.jiagoushi.top

Py:   (lambda: print("run"))()
来源：http://fmu.yuxming.cn

PHP:  (function () { echo "run"; })();
来源：http://fyl.ybcxt.top

JS:   (() => { console.log("run"); })();
来源：http://soc.hywenlv.cn

TS:   (() => { console.log("run"); })();
来源：http://jcl.jinyuanbaomall.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://aav.fzhhl.top

Go:   func() { fmt.Println("run") }()
来源：http://lqk.ppjwa.cn

Ruby: -> { puts "run" }.call
来源：http://mhl.jinqigfzy.top

C#:   // 无 IIFE：用静态构造函数
来源：http://amn.chenlongwang.top

[C13] 类型声明 / 类型注解
来源：http://vle.yanxiufei.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://zmn.zhongyouzk.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://uol.sysykeji.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://gac.xylfe.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mza.hesvh.cn

Java: int add(int a, int b) { return a + b; }
来源：http://tob.xuanzx.com

Go:   func add(a, b int) int
来源：http://vlt.zhengqikj.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://uxy.cashguo.top

C#:   int Add(int a, int b) => a + b;
来源：http://cit.yj20258.top

[C14] 泛型函数
来源：http://wta.zhijiandao.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zrr.cdnleiting.top

PHP:  // 无泛型
来源：http://ocd.havefunace.top

JS:   // 无泛型
来源：http://hca.fzhhl.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://tgf.cheryme.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://kyr.tarul.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ylv.xuetiantiany.cn

Ruby: # 无泛型
来源：http://swt.bjfxy.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://glx.gotoacloud.top

[C15] 解构 / 展开参数
来源：http://jxm.ybcxt.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://syk.xuetiantiany.cn

PHP:  [$a, $b] = $pair;
来源：http://mlh.chenzaomai.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://svs.ppjwa.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hsq.yueranfly.top

Java: // 无解构
来源：http://mle.aibaodan.cn

Go:   // 无解构
来源：http://jgz.smart0.xyz

Ruby: a, b = pair
来源：http://tgf.tarul.cn

C#:   var (a, b) = pair;
来源：http://qbk.316326.xyz

[C16] 函数 / 方法重载
来源：http://pbo.tarul.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ikr.jinqigufen.top

PHP:  // 无重载
来源：http://wqm.wangdashe.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://kug.guowangkeji.top

TS:   // 用联合类型或重载签名声明
来源：http://gbt.jyoumei.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://awy.svipenyu.cn

Go:   // 无重载：用不同函数名
来源：http://rbs.fzhhl.top

Ruby: # 无重载：靠动态参数
来源：http://ego.jinghuilouyu.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://hyf.mhx1999.top

================================================================================
来源：http://img.meibo888.top

D. 数组 / 列表 / 集合
来源：http://rpm.ydjk.org.cn

================================================================================
来源：http://osh.chenzaomai.com

[D01] 创建数组 / 列表
来源：http://bmr.yj20258.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://zpd.xinyue.icu

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://htj.cucudq.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ali.nanxuanxn.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://kzl.daxiang520.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://lvs.cashguo.top

Go:   arr := []int{1, 2, 3}
来源：http://lko.nwbrower.top

Ruby: arr = [1, 2, 3]
来源：http://zbk.daria6918.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hsg.xylfe.cn

[D02] 追加元素到末尾
来源：http://xva.bbcook.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ddn.ivvv.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hmn.redwolf501.top

JS:   arr.push(4);
来源：http://khb.tianlin.xyz

TS:   arr.push(4);
来源：http://vvm.chenjidiqi.icu

Java: list.add(4);
来源：http://vvi.snrcjt.cn

Go:   arr = append(arr, 4)
来源：http://xao.zhixingplan.top

Ruby: arr << 4; arr.push(5)
来源：http://ape.cucudq.cn

C#:   list.Add(4);
来源：http://puq.zhiwuduotai.top

[D03] 在指定位置插入元素
来源：http://ajo.aibaodan.cn

Py:   arr.insert(0, 0)
来源：http://xwx.yuanzhike.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://kpa.tianlin.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://iiv.daria6918.cn

TS:   arr.splice(0, 0, 0);
来源：http://mkm.smart0.xyz

Java: list.add(0, 0);
来源：http://dkm.svipenyu.cn

Go:   arr = append([]int{0}, arr...)
来源：http://miz.jyoumei.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://uzj.gogol.net.cn

C#:   list.Insert(0, 0);
来源：http://dzh.yangfankeji.com

[D04] 删除元素
来源：http://gln.xuanzx.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wzc.jinqigufen.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://njy.fanxiaobao.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://pgp.redwolf501.top

TS:   arr.splice(0, 1);
来源：http://ury.cdnleiting.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://nyk.jinghuilouyu.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://xaq.ehwqpu.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://nfh.jinghuilouyu.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xln.shanyushiyangtech.top

[D05] 访问与修改元素
来源：http://eft.fanxiaobao.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://nlo.9152youxi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://enl.shangyingyoupin.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://lnh.ydzc1.top

TS:   arr[0]; arr.at(-1);
来源：http://ive.tanke756.top

Java: list.get(0); list.set(0, 9);
来源：http://asb.cdnleiting.top

Go:   arr[0]; arr[0] = 9
来源：http://uiz.ctjpmb.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ugh.cqqwz.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://dca.hammf.cn

[D06] 数组长度
来源：http://vqr.jqgfzy.top

Py:   len(arr)
来源：http://izt.pycfn.com

PHP:  count($arr);
来源：http://red.gotoacloud.top

JS:   arr.length
来源：http://ojp.bjfxy.top

TS:   arr.length
来源：http://ejd.yj20258888.top

Java: list.size();
来源：http://reh.jinqigufen.top

Go:   len(arr)
来源：http://rpy.sufxvd.cn

Ruby: arr.length; arr.size
来源：http://kze.jlsjyb.cn

C#:   list.Count;
来源：http://ewk.shanyushiyangkeji.top

[D07] 切片 / 取子数组
来源：http://cfg.jyoumei.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://fgr.dashuyun.cn

PHP:  array_slice($arr, 1, 3);
来源：http://wko.cqqwz.cn

JS:   arr.slice(1, 4);
来源：http://snr.guannengcc.top

TS:   arr.slice(1, 4);
来源：http://hnq.cqqwz.cn

Java: list.subList(1, 4);
来源：http://nvp.zhoulong.xyz

Go:   arr[1:4]
来源：http://yqm.zdbjq.cn

Ruby: arr[1, 3]
来源：http://zpv.xingfuxueyuan.xyz

C#:   list.GetRange(1, 3);
来源：http://tgq.fengsongda.top

[D08] 合并两个数组
来源：http://swz.vqdsnc.cn

Py:   a + b;  a.extend(b)
来源：http://dyo.ybcxt.top

PHP:  array_merge($a, $b);
来源：http://rwm.316326.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://coh.hnxiangtu.top

TS:   [...a, ...b];
来源：http://gdp.c1oappe.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ikv.wangdashe.top

Go:   append(a, b...)
来源：http://mon.fengsongda.top

Ruby: a + b;  a.concat(b)
来源：http://vvu.jianghu66.top

C#:   a.Concat(b).ToList()
来源：http://aqn.jianghu66.top

[D09] 排序（升序）
来源：http://yfv.316326.xyz

Py:   sorted(arr);  arr.sort()
来源：http://ohi.ehwqpu.com

PHP:  sort($arr);
来源：http://hik.ybcxt.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://tuu.yvedp.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://tpl.jianghu66.top

Java: Collections.sort(list);  list.sort(null);
来源：http://ioe.sxryk.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wmp.ehwqpu.com

Ruby: arr.sort
来源：http://dzh.bbcook.cn

C#:   list.Sort();
来源：http://vns.bbcook.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://iov.xuanzx.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://fpw.yj20258.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://iss.hnxiangtu.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://gnq.cucudq.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wzs.fanxiaobao.xyz

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ikh.hywenlv.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://gol.hongshengwenyu.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://tec.daxiang520.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hok.ctjpmb.com

[D11] 反转数组
来源：http://dwl.hongshengwenyu.top

Py:   arr[::-1];  arr.reverse()
来源：http://oeo.daxiang520.top

PHP:  array_reverse($arr);
来源：http://hrw.xylfe.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://agi.zhijiandao.cn

TS:   [...arr].reverse();
来源：http://ogb.vqdsnc.cn

Java: Collections.reverse(list);
来源：http://zkl.316326.xyz

Go:   slices.Reverse(arr)
来源：http://spa.52xcode.cn

Ruby: arr.reverse
来源：http://jve.ybcxt.top

C#:   list.Reverse();
来源：http://pgi.guannengcc.top

[D12] 查找元素下标
来源：http://asj.quarkkingdee.top

Py:   arr.index(x);  x in arr
来源：http://asf.nanxuanxn.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://oek.zhaomingkeji.xyz

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qxd.daria6918.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kjy.xziqi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wok.hysaishi.cn

Go:   slices.Index(arr, x)
来源：http://jou.havefunace.top

Ruby: arr.index(x)
来源：http://ceu.iojbl.cn

C#:   list.IndexOf(x);
来源：http://tbc.fehbvm.com

[D13] 过滤（保留满足条件的）
来源：http://ahm.vehdjk.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://kxe.xylfe.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://znn.birdmap.top

JS:   arr.filter(x => x > 3)
来源：http://kap.hammf.cn

TS:   arr.filter(x => x > 3)
来源：http://nls.iojbl.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://tqn.0kj1m.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://fiq.snrcjt.cn

Ruby: arr.select { |x| x > 3 }
来源：http://bug.yanxiufei.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ldx.fengsongda.top

[D14] 映射转换（每个元素变形）
来源：http://rby.fzhhl.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://vja.birdmap.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vkz.ehwqpu.com

JS:   arr.map(x => x * 2)
来源：http://xst.gogol.net.cn

TS:   arr.map(x => x * 2)
来源：http://ivo.ydjk.org.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://itu.gaohongyu789.top

Go:   // 手写循环
来源：http://ovw.bbcook.cn

Ruby: arr.map { |x| x * 2 }
来源：http://hzk.fzhhl.top

C#:   list.Select(x => x * 2).ToList()
来源：http://qcr.wangdashe.top

[D15] 去重
来源：http://ufl.jqgufenzy.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://qih.cucudq.cn

PHP:  array_unique($arr);
来源：http://kce.hammf.cn

JS:   [...new Set(arr)]
来源：http://ipb.mhx1999.top

TS:   [...new Set(arr)]
来源：http://mfq.dianchejie.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://npa.0kj1m.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ufw.cheryme.top

Ruby: arr.uniq
来源：http://bwx.guannengcc.top

C#:   list.Distinct().ToList()
来源：http://ltn.sxryk.cn

[D16] 求和与平均值
来源：http://ovw.redwolf501.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qwv.snrcjt.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://gxy.tanke756.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://dqe.tian-w.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://rwi.cqqwz.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://lez.bjfxy.top

Go:   // 手写循环累加
来源：http://yic.yonumen.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ibw.hfpthk.cn

C#:   list.Sum();  list.Average()
来源：http://ouk.yanxiufei.cn

[D17] 最大值与最小值
来源：http://vic.jinqigufen.top

Py:   max(arr);  min(arr)
来源：http://wvr.cqqwz.cn

PHP:  max($arr);  min($arr);
来源：http://rxd.shangyingyoupin.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://lfr.316326.xyz

TS:   Math.max(...arr);
来源：http://qsn.yj202588.top

Java: Collections.max(list);  Collections.min(list);
来源：http://xms.yuanzhike.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://fub.pycfn.com

Ruby: arr.max;  arr.min
来源：http://lea.fktsv.cn

C#:   list.Max();  list.Min()
来源：http://zbq.hfpthk.cn

[D18] 扁平化嵌套数组
来源：http://nff.daxiang520.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ltn.xuetiantiany.cn

PHP:  array_merge(...$nested);
来源：http://uql.hywenlv.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://nbp.yuxming.cn

TS:   nested.flat();
来源：http://zhh.yvedp.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wav.svipenyu.cn

Go:   // 手写双层循环
来源：http://yzl.nanxuanxn.top

Ruby: nested.flatten
来源：http://xxv.cdnleiting.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://euq.yvedp.cn

[D19] 按字段分组
来源：http://dsz.hysaishi.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://bxn.jianghu66.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://bqc.chenjidiqi.icu

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://jiw.fengsongda.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://swx.yuxming.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://sfg.aizwys.cn

Go:   // 手写 map[string][]T
来源：http://xqd.jqgfzy.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://xak.smart0.xyz


<!-- 参考信息 -->