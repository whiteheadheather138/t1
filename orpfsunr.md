代发 wailian999

================================================================================
来源：http://yvi.xuetiantiany.cn

C. 函数与作用域
来源：http://cje.yanxiufei.cn

================================================================================
来源：http://hod.ctjpmb.com

[C01] 定义函数
来源：http://sic.fanxiaobao.xyz

Py:   def add(a, b): return a + b
来源：http://vct.hongshengwenyu.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hdm.fehbvm.com

JS:   function add(a, b) { return a + b; }
来源：http://bhl.bbcook.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qjw.fengsongda.top

Java: static int add(int a, int b) { return a + b; }
来源：http://jqe.hcnkem.com

Go:   func add(a, b int) int { return a + b }
来源：http://xxt.gaohongyu789.top

Ruby: def add(a, b); a + b; end
来源：http://ngy.epnwcf.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wxb.yonumen.top

[C02] 默认参数
来源：http://tpv.xziqi.cn

Py:   def greet(name="World"): return name
来源：http://acv.zhiwuduotai.top

PHP:  function greet($name = "World") { return $name; }
来源：http://uxb.gogol.net.cn

JS:   function greet(name = "World") { return name; }
来源：http://tag.birdmap.top

TS:   function greet(name: string = "World") { return name; }
来源：http://ovg.havefunace.top

Java: // 无默认参数：方法重载或 Optional
来源：http://fvj.guowangkeji.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://igb.c1oappe.top

Ruby: def greet(name = "World") = name
来源：http://kgn.mhx1999.top

C#:   string Greet(string name = "World") => name;
来源：http://goa.dashuyun.cn

[C03] 可变参数
来源：http://fir.vehdjk.com

Py:   def total(*args): return sum(args)
来源：http://wkl.epnwcf.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://dab.yuanzhike.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ryj.gotoacloud.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wvu.pycfn.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://lwb.xuetiantiany.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://gqh.yueranfly.top

Ruby: def total(*nums); nums.sum; end
来源：http://moe.jinyuanbaomall.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://vhy.xinyue.icu

[C04] 命名参数 / 关键字参数
来源：http://yie.svipenyu.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://pfg.yangfankeji.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xvh.316326.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://dpa.ydzc1.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://sak.kuanghao11.cn

Java: // 无：用 Builder 模式或 record
来源：http://sab.hesvh.cn

Go:   // 无：用配置结构体参数
来源：http://roz.xuanzx.com

Ruby: f(a: 1, b: 2)
来源：http://pja.hongshengwenyu.top

C#:   f(a: 1, b: 2)
来源：http://aup.guannengcc.top

[C05] 返回多个值
来源：http://hbx.gaohongyu789.top

Py:   return a, b
来源：http://qog.sjlbkw.cn

PHP:  return [$a, $b];
来源：http://nhh.gaohongyu789.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://qta.svipenyu.cn

TS:   return { a, b };
来源：http://dlr.guannengcc.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://nvc.aizwys.cn

Go:   return a, b
来源：http://zmf.sysykeji.top

Ruby: return a, b
来源：http://joi.zycfv.cn

C#:   return (a, b);              // ValueTuple
来源：http://zsz.fehbvm.com

[C06] 匿名函数 / lambda
来源：http://xoe.kuanghao11.cn

Py:   square = lambda x: x * x
来源：http://xdi.shanyushiyangtech.top

PHP:  $square = fn($x) => $x * $x;
来源：http://wlq.hysaishi.cn

JS:   const square = x => x * x;
来源：http://ukx.zdqjudy.top

TS:   const square = (x: number): number => x * x;
来源：http://tvw.hammf.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://iyg.fzhhl.top

Go:   sq := func(x int) int { return x * x }
来源：http://jpq.chenjidiqi.icu

Ruby: square = ->(x) { x * x }
来源：http://ehs.ppjwa.cn

C#:   Func<int, int> square = x => x * x;
来源：http://qnt.yuanzhike.top

[C07] 把函数作为参数传入
来源：http://hyp.316326.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://muv.tian-w.cn

PHP:  array_map("strtoupper", $arr);
来源：http://dzg.yfazqb.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hqs.havefunace.top

TS:   arr.map(String)
来源：http://kre.tarul.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://tzb.shangyingyoupin.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ubw.aizwys.cn

Ruby: arr.map(&:upcase)
来源：http://elw.feifeiyinyue.top

C#:   arr.Select(s => s.ToUpper())
来源：http://dox.wangdashe.top

[C08] 闭包
来源：http://crz.yvedp.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://kac.smart0.xyz

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://tdw.ppjwa.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://urf.shanyushiyangkeji.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://rfn.zhixingplan.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://rna.sysykeji.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jht.9152youxi.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://jmt.jinqigufen.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://eng.hongshengwenyu.top

[C09] 递归
来源：http://miu.jyoumei.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mwc.ctjpmb.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://dve.hongshengwenyu.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ctw.fanxiaobao.xyz

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hsa.jiagoushi.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://bse.gotoacloud.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://uqg.bbcook.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://lon.yongpay.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://qmk.iojbl.cn

[C10] 变量作用域
来源：http://jyu.daxiang520.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://vjp.wangdashe.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wzd.andypj.xyz

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xhy.dashuyun.cn

TS:   同 JS
来源：http://tvn.52xcode.cn

Java: 方法内为块级作用域
来源：http://atk.jiagoushi.top

Go:   花括号块级作用域
来源：http://ngk.0kj1m.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://deb.jyoumei.cn

C#:   块级作用域
来源：http://ilt.yj202588.top

[C11] 模块导入与导出
来源：http://aaa.sweek.top

Py:   from module import func
来源：http://ind.svipenyu.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://jba.gaohongyu789.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://dsi.mhx1999.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ayh.zdqjudy.top

Java: import java.util.List;
来源：http://pre.zdbjq.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://thh.kuanghao11.cn

Ruby: require "json"; require_relative "./util"
来源：http://kbr.nanxinkj.top

C#:   using System.Text;
来源：http://ivb.kuanghao11.cn

[C12] 立即执行函数 IIFE
来源：http://bud.yanxiufei.cn

Py:   (lambda: print("run"))()
来源：http://laf.zhoulong.xyz

PHP:  (function () { echo "run"; })();
来源：http://exq.ydzc1.top

JS:   (() => { console.log("run"); })();
来源：http://wtw.quarkkingdee.top

TS:   (() => { console.log("run"); })();
来源：http://qjk.fehbvm.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://icw.yj202588.top

Go:   func() { fmt.Println("run") }()
来源：http://smx.yvedp.cn

Ruby: -> { puts "run" }.call
来源：http://wys.ctjpmb.com

C#:   // 无 IIFE：用静态构造函数
来源：http://kqz.xuetiantiany.cn

[C13] 类型声明 / 类型注解
来源：http://qrg.yonumen.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://zpm.fanxiaobao.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lpm.dashuyun.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://nfe.shangyingyoupin.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fmo.hnxiangtu.top

Java: int add(int a, int b) { return a + b; }
来源：http://ctd.xinyue.icu

Go:   func add(a, b int) int
来源：http://xjx.hongshengwenyu.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://cfq.yongpay.top

C#:   int Add(int a, int b) => a + b;
来源：http://fjh.hcnkem.com

[C14] 泛型函数
来源：http://nab.bjfxy.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://aqb.pengpengdd.cyou

PHP:  // 无泛型
来源：http://mvv.cashguo.top

JS:   // 无泛型
来源：http://ijk.mhx1999.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://dzs.tarul.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://khx.zhijiandao.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://jfe.xingfuxueyuan.xyz

Ruby: # 无泛型
来源：http://mro.aizwys.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://iym.gaohongyu789.top

[C15] 解构 / 展开参数
来源：http://cts.hcnkem.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://rgh.yj20258888.top

PHP:  [$a, $b] = $pair;
来源：http://dbf.quarkkingdee.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://atd.jinyuanbaomall.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://sro.sweek.top

Java: // 无解构
来源：http://cod.xylfe.cn

Go:   // 无解构
来源：http://kqk.shangyingyoupin.top

Ruby: a, b = pair
来源：http://mut.chenjidiqi.icu

C#:   var (a, b) = pair;
来源：http://zoq.nwbrower.top

[C16] 函数 / 方法重载
来源：http://rxo.smart0.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://aeg.xziqi.cn

PHP:  // 无重载
来源：http://tmt.pengpengdd.cyou

JS:   // 无重载：靠 arguments.length 分支
来源：http://xhb.shanyushiyangtech.top

TS:   // 用联合类型或重载签名声明
来源：http://gop.haohaochexian.top

Java: void f(int a) {}  void f(String a) {}
来源：http://dwq.chenlongwang.top

Go:   // 无重载：用不同函数名
来源：http://vfj.shanyushiyangkeji.top

Ruby: # 无重载：靠动态参数
来源：http://lcn.daria6918.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://uvw.pycfn.com

================================================================================
来源：http://nac.pengpengdd.cyou

D. 数组 / 列表 / 集合
来源：http://iwu.shangyingyoupin.top

================================================================================
来源：http://yvj.xziqi.cn

[D01] 创建数组 / 列表
来源：http://sjf.tanke756.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://ysj.9152youxi.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://pix.jlsjyb.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://xts.hfpthk.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://nji.ydzc1.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://bbv.jqgufenzy.top

Go:   arr := []int{1, 2, 3}
来源：http://zkl.dashuyun.cn

Ruby: arr = [1, 2, 3]
来源：http://sak.yonumen.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://skv.aibaodan.cn

[D02] 追加元素到末尾
来源：http://epu.jyoumei.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://qsd.cashguo.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://lwi.hammf.cn

JS:   arr.push(4);
来源：http://obt.tanke756.top

TS:   arr.push(4);
来源：http://sir.shanyushiyangtech.top

Java: list.add(4);
来源：http://zvi.gaohongyu789.top

Go:   arr = append(arr, 4)
来源：http://xvo.c1oappe.top

Ruby: arr << 4; arr.push(5)
来源：http://hah.havefunace.top

C#:   list.Add(4);
来源：http://wvn.birdmap.top

[D03] 在指定位置插入元素
来源：http://rid.uphjek.com

Py:   arr.insert(0, 0)
来源：http://xxv.hammf.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ptx.shuidangran.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://yuv.yuanzhike.top

TS:   arr.splice(0, 0, 0);
来源：http://oie.dashuyun.cn

Java: list.add(0, 0);
来源：http://qqr.0kj1m.cn

Go:   arr = append([]int{0}, arr...)
来源：http://icd.yangfankeji.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ydh.daxiang520.top

C#:   list.Insert(0, 0);
来源：http://kdx.zhoulong.xyz

[D04] 删除元素
来源：http://ine.9152youxi.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wpg.zhengqikj.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://jga.bbcook.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xgi.gzhubu.top

TS:   arr.splice(0, 1);
来源：http://lgo.kuanghao11.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ial.jinqigfzy.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://brw.hongshengwenyu.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://rrq.xuetiantiany.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://dfs.smart0.xyz

[D05] 访问与修改元素
来源：http://iro.sysykeji.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://iux.nanxinkj.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://xcg.yongpay.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://pys.nanxinkj.top

TS:   arr[0]; arr.at(-1);
来源：http://reu.jqgufenzy.top

Java: list.get(0); list.set(0, 9);
来源：http://bdz.gogol.net.cn

Go:   arr[0]; arr[0] = 9
来源：http://fgl.xuanzx.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://odg.zhengqikj.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ytv.hammf.cn

[D06] 数组长度
来源：http://oyt.hesvh.cn

Py:   len(arr)
来源：http://fzf.zhiwuduotai.top

PHP:  count($arr);
来源：http://laz.tian-w.cn

JS:   arr.length
来源：http://ekf.chenjidiqi.icu

TS:   arr.length
来源：http://hqc.shanyushiyangkeji.top

Java: list.size();
来源：http://jzm.xingfuxueyuan.xyz

Go:   len(arr)
来源：http://cxu.epnwcf.com

Ruby: arr.length; arr.size
来源：http://psv.aizwys.cn

C#:   list.Count;
来源：http://kpz.vehdjk.com

[D07] 切片 / 取子数组
来源：http://pay.hnxiangtu.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qce.jqgfzy.top

PHP:  array_slice($arr, 1, 3);
来源：http://pqx.yj202588.top

JS:   arr.slice(1, 4);
来源：http://zwg.ydjk.org.cn

TS:   arr.slice(1, 4);
来源：http://gfw.andypj.xyz

Java: list.subList(1, 4);
来源：http://paf.cqqwz.cn

Go:   arr[1:4]
来源：http://gdp.ybcxt.top

Ruby: arr[1, 3]
来源：http://lch.havefunace.top

C#:   list.GetRange(1, 3);
来源：http://qoc.shanyushiyangtech.top

[D08] 合并两个数组
来源：http://ypf.zhengqikj.top

Py:   a + b;  a.extend(b)
来源：http://mdp.ywan-chungtsiang.top

PHP:  array_merge($a, $b);
来源：http://gnp.shanyushiyangtech.top

JS:   [...a, ...b];  a.concat(b);
来源：http://khl.zhengqikj.top

TS:   [...a, ...b];
来源：http://lak.quarkkingdee.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://pfz.vehdjk.com

Go:   append(a, b...)
来源：http://dct.ivvv.top

Ruby: a + b;  a.concat(b)
来源：http://zuz.jyoumei.cn

C#:   a.Concat(b).ToList()
来源：http://iko.meibo888.top

[D09] 排序（升序）
来源：http://yeo.ehwqpu.com

Py:   sorted(arr);  arr.sort()
来源：http://zqo.zhixingplan.top

PHP:  sort($arr);
来源：http://vgm.shanyushiyangkeji.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://olk.yj20258888.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://jwt.hnqzz.top

Java: Collections.sort(list);  list.sort(null);
来源：http://jtq.uphjek.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://zjf.jyoumei.cn

Ruby: arr.sort
来源：http://tpz.yuanzhike.top

C#:   list.Sort();
来源：http://zgk.tianlin.xyz

[D10] 自定义排序（按字段 / 多条件）
来源：http://yuk.ppjwa.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://muo.gaohongyu789.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ird.xuanzx.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://yza.shanyushiyangkeji.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ejd.yonumen.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://tru.yangfankeji.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://lcx.jiagoushi.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://zkb.shuidangran.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://kns.xuetiantiany.cn

[D11] 反转数组
来源：http://bfq.wangshuangyany.cn

Py:   arr[::-1];  arr.reverse()
来源：http://gpj.jyoumei.cn

PHP:  array_reverse($arr);
来源：http://xfx.hammf.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ivt.xziqi.cn

TS:   [...arr].reverse();
来源：http://xmf.andypj.xyz

Java: Collections.reverse(list);
来源：http://prb.yj202588.top

Go:   slices.Reverse(arr)
来源：http://kzg.hesvh.cn

Ruby: arr.reverse
来源：http://zjr.uphjek.com

C#:   list.Reverse();
来源：http://qrq.yj20258888.top

[D12] 查找元素下标
来源：http://nxr.cdnleiting.top

Py:   arr.index(x);  x in arr
来源：http://icu.jinghuilouyu.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://gad.gogol.net.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nuk.cqqwz.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ipd.hywenlv.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://oqg.52xcode.cn

Go:   slices.Index(arr, x)
来源：http://uza.yueranfly.top

Ruby: arr.index(x)
来源：http://wfa.pengpengdd.cyou

C#:   list.IndexOf(x);
来源：http://pko.zhiwuduotai.top

[D13] 过滤（保留满足条件的）
来源：http://qlc.xylfe.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qhv.bbcook.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://bwh.gaohongyu789.top

JS:   arr.filter(x => x > 3)
来源：http://ukp.feifeiyinyue.top

TS:   arr.filter(x => x > 3)
来源：http://axp.svipenyu.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://gsw.yuanzhike.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://pib.fengsongda.top

Ruby: arr.select { |x| x > 3 }
来源：http://xjk.yangfankeji.com

C#:   list.Where(x => x > 3).ToList()
来源：http://cjq.xylfe.cn

[D14] 映射转换（每个元素变形）
来源：http://kbd.xinyue.icu

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xgb.tianlin.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ipp.aibaodan.cn

JS:   arr.map(x => x * 2)
来源：http://khj.yj20258.top

TS:   arr.map(x => x * 2)
来源：http://bui.cqqwz.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://umr.zhengqikj.top

Go:   // 手写循环
来源：http://ayg.jinyuanbaomall.cn

Ruby: arr.map { |x| x * 2 }
来源：http://nfi.sxryk.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://dfa.316326.xyz

[D15] 去重
来源：http://jam.cheryme.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://tpl.fktsv.cn

PHP:  array_unique($arr);
来源：http://oml.fengsongda.top

JS:   [...new Set(arr)]
来源：http://etp.shzxlz.cn

TS:   [...new Set(arr)]
来源：http://zhm.yangfankeji.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://tqv.jyoumei.cn

Go:   // 用 map[T]struct{} 手写
来源：http://zwn.chenlongwang.top

Ruby: arr.uniq
来源：http://pas.pengpengdd.cyou

C#:   list.Distinct().ToList()
来源：http://epl.meibo888.top

[D16] 求和与平均值
来源：http://vox.dianchejie.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://umd.nwbrower.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://sny.fktsv.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://zix.yuxming.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://sjx.havefunace.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://sna.ivvv.top

Go:   // 手写循环累加
来源：http://wuo.quarkkingdee.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ubp.yj20258.top

C#:   list.Sum();  list.Average()
来源：http://jsm.yj20258.top

[D17] 最大值与最小值
来源：http://bhc.svipenyu.cn

Py:   max(arr);  min(arr)
来源：http://eqk.andypj.xyz

PHP:  max($arr);  min($arr);
来源：http://hir.aizwys.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://pkx.c1oappe.top

TS:   Math.max(...arr);
来源：http://xbr.yuanzhike.top

Java: Collections.max(list);  Collections.min(list);
来源：http://jnz.hfpthk.cn


<!-- 参考信息 -->