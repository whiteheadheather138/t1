代发 wailian999

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://htm.jinyuanbaomall.cn

Java: x instanceof Number
来源：http://edg.kuanghao11.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://pwd.hnqzz.top

Ruby: x.is_a?(Numeric)
来源：http://zrj.yuxming.cn

C#:   x is int or double or decimal
来源：http://aor.hfpthk.cn

[B14] 判断值是否在集合内
来源：http://dsk.kuanghao11.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://gak.gogol.net.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://dqs.sjlbkw.cn

JS:   [1, 2, 3].includes(x)
来源：http://uaf.9152youxi.cn

TS:   [1, 2, 3].includes(x)
来源：http://zxa.sysykeji.top

Java: List.of(1, 2, 3).contains(x)
来源：http://omn.jinqigufen.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://zsw.xinyue.icu

Ruby: [1, 2, 3].include?(x)
来源：http://fyf.tian-w.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://cou.shanyushiyangkeji.top

[B15] 布尔运算与取反
来源：http://glw.yueranfly.top

Py:   a and b or not c
来源：http://ouj.kuanghao11.cn

PHP:  $a && $b || !$c
来源：http://vrh.redwolf501.top

JS:   a && b || !c
来源：http://qmv.jqgfzy.top

TS:   a && b || !c
来源：http://esa.fktsv.cn

Java: a && b || !c
来源：http://xau.zycfv.cn

Go:   a && b || !c
来源：http://nie.yuanzhike.top

Ruby: a && b || !c
来源：http://kqh.daria6918.cn

C#:   a && b || !c
来源：http://xwv.chenlongwang.top

[B16] 卫语句：不满足条件提前返回
来源：http://iyk.tarul.cn

Py:   if not data: return
来源：http://qfu.shzxlz.cn

PHP:  if (!$data) { return; }
来源：http://tou.zhijiandao.cn

JS:   if (!data) return;
来源：http://ncw.jlsjyb.cn

TS:   if (!data) return;
来源：http://tfl.hfpthk.cn

Java: if (data == null) return;
来源：http://fqf.hcnkem.com

Go:   if data == nil { return }
来源：http://hdb.vehdjk.com

Ruby: return if data.nil?
来源：http://kzj.yanxiufei.cn

C#:   if (data == null) return;
来源：http://ypt.sweek.top

================================================================================
来源：http://oqi.gogol.net.cn

C. 函数与作用域
来源：http://wsv.hysaishi.cn

================================================================================
来源：http://frw.cqqwz.cn

[C01] 定义函数
来源：http://kjk.fengsongda.top

Py:   def add(a, b): return a + b
来源：http://xax.jiagoushi.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hct.yj202588.top

JS:   function add(a, b) { return a + b; }
来源：http://qcd.hesvh.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mwk.jiagoushi.top

Java: static int add(int a, int b) { return a + b; }
来源：http://vix.wangdashe.top

Go:   func add(a, b int) int { return a + b }
来源：http://wdc.xuanzx.com

Ruby: def add(a, b); a + b; end
来源：http://lku.yfazqb.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://vlf.ctjpmb.com

[C02] 默认参数
来源：http://zrw.daxiang520.top

Py:   def greet(name="World"): return name
来源：http://pmk.316326.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://dqt.mhx1999.top

JS:   function greet(name = "World") { return name; }
来源：http://lkh.yueranfly.top

TS:   function greet(name: string = "World") { return name; }
来源：http://pby.vehdjk.com

Java: // 无默认参数：方法重载或 Optional
来源：http://mzc.pycfn.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://uuv.hfpthk.cn

Ruby: def greet(name = "World") = name
来源：http://lsj.aizwys.cn

C#:   string Greet(string name = "World") => name;
来源：http://zlv.hywenlv.cn

[C03] 可变参数
来源：http://iqg.tianlin.xyz

Py:   def total(*args): return sum(args)
来源：http://qlz.chenjidiqi.icu

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://plv.zycfv.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://fxa.haohaochexian.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://qre.yangfankeji.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://zaz.hongshengwenyu.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://tzq.316326.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://mhz.tanke756.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://gii.hesvh.cn

[C04] 命名参数 / 关键字参数
来源：http://msa.andypj.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://kvj.pycfn.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://vxw.wangdashe.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://sme.zhijiandao.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://kkj.yongpay.top

Java: // 无：用 Builder 模式或 record
来源：http://ikp.shanyushiyangkeji.top

Go:   // 无：用配置结构体参数
来源：http://fjg.pycfn.com

Ruby: f(a: 1, b: 2)
来源：http://pbj.smart0.xyz

C#:   f(a: 1, b: 2)
来源：http://xoi.feifeiyinyue.top

[C05] 返回多个值
来源：http://lob.shangyingyoupin.top

Py:   return a, b
来源：http://mks.hnxiangtu.top

PHP:  return [$a, $b];
来源：http://elj.tarul.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://jdq.yvedp.cn

TS:   return { a, b };
来源：http://jkd.zdbjq.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://imh.iojbl.cn

Go:   return a, b
来源：http://thj.ctjpmb.com

Ruby: return a, b
来源：http://oeo.ydzc1.top

C#:   return (a, b);              // ValueTuple
来源：http://gxo.cheryme.top

[C06] 匿名函数 / lambda
来源：http://pnq.zhijiandao.cn

Py:   square = lambda x: x * x
来源：http://mnq.svipenyu.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://dsl.ydzc1.top

JS:   const square = x => x * x;
来源：http://nzx.daria6918.cn

TS:   const square = (x: number): number => x * x;
来源：http://dcw.zhiwuduotai.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://zni.ydjk.org.cn

Go:   sq := func(x int) int { return x * x }
来源：http://gcr.yvedp.cn

Ruby: square = ->(x) { x * x }
来源：http://hjv.gaohongyu789.top

C#:   Func<int, int> square = x => x * x;
来源：http://jcs.nanxuanxn.top

[C07] 把函数作为参数传入
来源：http://aet.cucudq.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mrv.haohaochexian.top

PHP:  array_map("strtoupper", $arr);
来源：http://pok.aizwys.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ltg.yvedp.cn

TS:   arr.map(String)
来源：http://aku.fzhhl.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://och.vehdjk.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://vlj.zhengqikj.top

Ruby: arr.map(&:upcase)
来源：http://tdj.chenlongwang.top

C#:   arr.Select(s => s.ToUpper())
来源：http://wqs.xylfe.cn

[C08] 闭包
来源：http://vjp.ivvv.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://dip.andypj.xyz

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://dmv.aibaodan.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://djw.hesvh.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://zak.wangshuangyany.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://vsw.bjfxy.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://rch.ywan-chungtsiang.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://xfc.xuanzx.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://psi.iojbl.cn

[C09] 递归
来源：http://jar.tian-w.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://dgj.yanxiufei.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://tyg.havefunace.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vuj.guannengcc.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://svi.guannengcc.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://bux.yj202588.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://nxi.pengpengdd.cyou

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://byi.havefunace.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ony.jiagoushi.top

[C10] 变量作用域
来源：http://nzt.svipenyu.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hya.yangfankeji.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://kmh.sjlbkw.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://brv.nwbrower.top

TS:   同 JS
来源：http://trr.birdmap.top

Java: 方法内为块级作用域
来源：http://irr.0kj1m.cn

Go:   花括号块级作用域
来源：http://uux.yongpay.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://cdr.epnwcf.com

C#:   块级作用域
来源：http://jtk.ybcxt.top

[C11] 模块导入与导出
来源：http://jgl.sjlbkw.cn

Py:   from module import func
来源：http://dls.ydzc1.top

PHP:  require "file.php";  或 use App\Service;
来源：http://oqj.xuetiantiany.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://obe.cqqwz.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ozo.tian-w.cn

Java: import java.util.List;
来源：http://lpo.meibo888.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ucl.hcnkem.com

Ruby: require "json"; require_relative "./util"
来源：http://qbp.shanyushiyangtech.top

C#:   using System.Text;
来源：http://fhd.jqgufenzy.top

[C12] 立即执行函数 IIFE
来源：http://slo.tian-w.cn

Py:   (lambda: print("run"))()
来源：http://wqv.gzhubu.top

PHP:  (function () { echo "run"; })();
来源：http://feq.ydjk.org.cn

JS:   (() => { console.log("run"); })();
来源：http://vzf.hesvh.cn

TS:   (() => { console.log("run"); })();
来源：http://whb.zhengqikj.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://vof.ctjpmb.com

Go:   func() { fmt.Println("run") }()
来源：http://iff.aizwys.cn

Ruby: -> { puts "run" }.call
来源：http://cbq.zhiwuduotai.top

C#:   // 无 IIFE：用静态构造函数
来源：http://xws.tian-w.cn

[C13] 类型声明 / 类型注解
来源：http://vfy.ivvv.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://nop.xuetiantiany.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mnh.yj20258888.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ysb.chenlongwang.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ptx.ybcxt.top

Java: int add(int a, int b) { return a + b; }
来源：http://hse.hfpthk.cn

Go:   func add(a, b int) int
来源：http://ori.ywan-chungtsiang.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://pzr.hysaishi.cn

C#:   int Add(int a, int b) => a + b;
来源：http://tof.andypj.xyz

[C14] 泛型函数
来源：http://jor.jiagoushi.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wso.daxiang520.top

PHP:  // 无泛型
来源：http://ueg.ivvv.top

JS:   // 无泛型
来源：http://hfq.ppjwa.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://czr.shangyingyoupin.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://fuz.wangdashe.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://isp.yueranfly.top

Ruby: # 无泛型
来源：http://uii.jqgfzy.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://tro.yj20258.top

[C15] 解构 / 展开参数
来源：http://ztk.9152youxi.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://cci.yueranfly.top

PHP:  [$a, $b] = $pair;
来源：http://tgl.aibaodan.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ysq.haohaochexian.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ffc.0kj1m.cn

Java: // 无解构
来源：http://jdf.snrcjt.cn

Go:   // 无解构
来源：http://lsb.nanxuanxn.top

Ruby: a, b = pair
来源：http://xgu.yanxiufei.cn

C#:   var (a, b) = pair;
来源：http://ifo.fehbvm.com

[C16] 函数 / 方法重载
来源：http://brm.jianghu66.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mho.yuxming.cn

PHP:  // 无重载
来源：http://erb.daria6918.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://fnc.hammf.cn

TS:   // 用联合类型或重载签名声明
来源：http://mke.yuanzhike.top

Java: void f(int a) {}  void f(String a) {}
来源：http://ioh.cdnleiting.top

Go:   // 无重载：用不同函数名
来源：http://oio.yonumen.top

Ruby: # 无重载：靠动态参数
来源：http://joa.daxiang520.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://lpq.cucudq.cn

================================================================================
来源：http://xkj.zdqjudy.top

D. 数组 / 列表 / 集合
来源：http://ddp.zhoulong.xyz

================================================================================
来源：http://awv.nanxinkj.top

[D01] 创建数组 / 列表
来源：http://wkg.mhx1999.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://jil.shanyushiyangkeji.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://zjy.zdqjudy.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://dzh.havefunace.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://fjy.52xcode.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hmp.hnqzz.top

Go:   arr := []int{1, 2, 3}
来源：http://gas.snrcjt.cn

Ruby: arr = [1, 2, 3]
来源：http://nho.ydzc1.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://tpy.pengpengdd.cyou

[D02] 追加元素到末尾
来源：http://xrw.cqqwz.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://bfx.sjlbkw.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://bzw.xuanzx.com

JS:   arr.push(4);
来源：http://ask.yuanzhike.top

TS:   arr.push(4);
来源：http://vjj.kuanghao11.cn

Java: list.add(4);
来源：http://kks.snrcjt.cn

Go:   arr = append(arr, 4)
来源：http://fwe.meibo888.top

Ruby: arr << 4; arr.push(5)
来源：http://pds.ydjk.org.cn

C#:   list.Add(4);
来源：http://nrp.ehwqpu.com

[D03] 在指定位置插入元素
来源：http://prc.ydzc1.top

Py:   arr.insert(0, 0)
来源：http://gkt.birdmap.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://tle.pycfn.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://zhp.jlsjyb.cn

TS:   arr.splice(0, 0, 0);
来源：http://rhl.jiagoushi.top

Java: list.add(0, 0);
来源：http://gvw.haohaochexian.top

Go:   arr = append([]int{0}, arr...)
来源：http://gze.0kj1m.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://qrr.ivvv.top

C#:   list.Insert(0, 0);
来源：http://pzz.fzhhl.top

[D04] 删除元素
来源：http://wfo.shanyushiyangkeji.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://tqi.nanxinkj.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://dtt.kuanghao11.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://gwe.daria6918.cn

TS:   arr.splice(0, 1);
来源：http://mjd.xuetiantiany.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://jck.wangshuangyany.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://xbc.yj202588.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://iau.shanyushiyangkeji.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wwf.jyoumei.cn

[D05] 访问与修改元素
来源：http://wgc.zhoulong.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://nro.yangfankeji.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://pju.sjlbkw.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://vyl.yfazqb.com

TS:   arr[0]; arr.at(-1);
来源：http://mls.uphjek.com

Java: list.get(0); list.set(0, 9);
来源：http://flq.jyoumei.cn

Go:   arr[0]; arr[0] = 9
来源：http://ein.gaohongyu789.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://zoa.uphjek.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://jjf.tanke756.top

[D06] 数组长度
来源：http://kwp.cqqwz.cn

Py:   len(arr)
来源：http://sgq.aizwys.cn

PHP:  count($arr);
来源：http://bkc.shuidangran.top

JS:   arr.length
来源：http://pun.xinyue.icu

TS:   arr.length
来源：http://pla.bbcook.cn

Java: list.size();
来源：http://hkr.shanyushiyangtech.top

Go:   len(arr)
来源：http://xes.aizwys.cn

Ruby: arr.length; arr.size
来源：http://yit.snrcjt.cn

C#:   list.Count;
来源：http://gby.pycfn.com

[D07] 切片 / 取子数组
来源：http://xoi.yvedp.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://zyr.shzxlz.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ycg.nanxinkj.top

JS:   arr.slice(1, 4);
来源：http://hvx.shangyingyoupin.top

TS:   arr.slice(1, 4);
来源：http://qwm.hammf.cn

Java: list.subList(1, 4);
来源：http://jos.zycfv.cn

Go:   arr[1:4]
来源：http://pub.sysykeji.top

Ruby: arr[1, 3]
来源：http://tne.chenjidiqi.icu

C#:   list.GetRange(1, 3);
来源：http://rlb.hongshengwenyu.top

[D08] 合并两个数组
来源：http://gqs.havefunace.top

Py:   a + b;  a.extend(b)
来源：http://gxt.fzhhl.top

PHP:  array_merge($a, $b);
来源：http://rhm.zhijiandao.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://glp.yj20258888.top

TS:   [...a, ...b];
来源：http://oma.yfazqb.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ywl.kuanghao11.cn

Go:   append(a, b...)
来源：http://ngd.gzhubu.top

Ruby: a + b;  a.concat(b)
来源：http://anv.ydzc1.top

C#:   a.Concat(b).ToList()
来源：http://nln.birdmap.top

[D09] 排序（升序）
来源：http://neu.jlsjyb.cn

Py:   sorted(arr);  arr.sort()
来源：http://gte.jinyuanbaomall.cn

PHP:  sort($arr);
来源：http://nkn.zdqjudy.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://fxw.shzxlz.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ybq.wangshuangyany.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://cge.tianlin.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://lde.jqgufenzy.top

Ruby: arr.sort
来源：http://whb.birdmap.top

C#:   list.Sort();
来源：http://jwk.jinqigufen.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://vjz.zdbjq.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://zuf.tianlin.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zzb.cheryme.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://kkp.sxryk.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://qyt.fehbvm.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://jqq.chenzaomai.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://beu.wangdashe.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://vzl.epnwcf.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://klc.xuetiantiany.cn

[D11] 反转数组
来源：http://dvk.yuanzhike.top

Py:   arr[::-1];  arr.reverse()
来源：http://ofl.nanxinkj.top

PHP:  array_reverse($arr);
来源：http://qnc.xuanzx.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hmj.xuanzx.com

TS:   [...arr].reverse();
来源：http://kxu.yvedp.cn

Java: Collections.reverse(list);
来源：http://zcu.ydzc1.top

Go:   slices.Reverse(arr)
来源：http://vxr.pycfn.com

Ruby: arr.reverse
来源：http://jyn.fehbvm.com

C#:   list.Reverse();
来源：http://isu.sweek.top

[D12] 查找元素下标
来源：http://dab.jlsjyb.cn

Py:   arr.index(x);  x in arr
来源：http://azg.hfpthk.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://vts.yj202588.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://utd.yj20258888.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ybi.hysaishi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://gcc.daria6918.cn

Go:   slices.Index(arr, x)
来源：http://tsg.dashuyun.cn

Ruby: arr.index(x)
来源：http://ops.fehbvm.com

C#:   list.IndexOf(x);
来源：http://sxs.yongpay.top

[D13] 过滤（保留满足条件的）
来源：http://lql.ydzc1.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://zsn.xuanzx.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://lzu.zhengqikj.top

JS:   arr.filter(x => x > 3)
来源：http://wop.ydzc1.top

TS:   arr.filter(x => x > 3)
来源：http://mfz.aibaodan.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zbi.yueranfly.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://cvj.uphjek.com

Ruby: arr.select { |x| x > 3 }
来源：http://wue.quarkkingdee.top

C#:   list.Where(x => x > 3).ToList()
来源：http://tkb.zhixingplan.top

[D14] 映射转换（每个元素变形）
来源：http://ysf.hnqzz.top


<!-- 参考信息 -->