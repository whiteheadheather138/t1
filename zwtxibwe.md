代发 wailian999

Ruby: [1, 2, 3].include?(x)
来源：http://ofg.yj202588.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mvy.tian-w.cn

[B15] 布尔运算与取反
来源：http://veu.gogol.net.cn

Py:   a and b or not c
来源：http://jfl.zhiwuduotai.top

PHP:  $a && $b || !$c
来源：http://nni.tianlin.xyz

JS:   a && b || !c
来源：http://svg.jyoumei.cn

TS:   a && b || !c
来源：http://seq.zhaomingkeji.xyz

Java: a && b || !c
来源：http://zuw.jlsjyb.cn

Go:   a && b || !c
来源：http://ytu.hesvh.cn

Ruby: a && b || !c
来源：http://eyu.52xcode.cn

C#:   a && b || !c
来源：http://ldo.fktsv.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ddi.cheryme.top

Py:   if not data: return
来源：http://ycl.guowangkeji.top

PHP:  if (!$data) { return; }
来源：http://ezh.shanyushiyangtech.top

JS:   if (!data) return;
来源：http://cwl.snrcjt.cn

TS:   if (!data) return;
来源：http://obb.hfpthk.cn

Java: if (data == null) return;
来源：http://rhm.jinghuilouyu.cn

Go:   if data == nil { return }
来源：http://rhe.meibo888.top

Ruby: return if data.nil?
来源：http://ivd.ywan-chungtsiang.top

C#:   if (data == null) return;
来源：http://obd.jqgufenzy.top

================================================================================
来源：http://yme.fanxiaobao.xyz

C. 函数与作用域
来源：http://iia.jqgfzy.top

================================================================================
来源：http://nwz.ctjpmb.com

[C01] 定义函数
来源：http://azk.yongpay.top

Py:   def add(a, b): return a + b
来源：http://nyt.zycfv.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jet.chenzaomai.com

JS:   function add(a, b) { return a + b; }
来源：http://zrh.sjlbkw.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cjo.yangfankeji.com

Java: static int add(int a, int b) { return a + b; }
来源：http://gss.dianchejie.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ncc.vqdsnc.cn

Ruby: def add(a, b); a + b; end
来源：http://glr.gzhubu.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mfu.dashuyun.cn

[C02] 默认参数
来源：http://lyx.feifeiyinyue.top

Py:   def greet(name="World"): return name
来源：http://qgg.ydzc1.top

PHP:  function greet($name = "World") { return $name; }
来源：http://hai.vqdsnc.cn

JS:   function greet(name = "World") { return name; }
来源：http://dev.fehbvm.com

TS:   function greet(name: string = "World") { return name; }
来源：http://kbu.jiagoushi.top

Java: // 无默认参数：方法重载或 Optional
来源：http://kox.jqgfzy.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://fpp.ybcxt.top

Ruby: def greet(name = "World") = name
来源：http://ynk.zhoulong.xyz

C#:   string Greet(string name = "World") => name;
来源：http://gab.nwbrower.top

[C03] 可变参数
来源：http://hnk.yj202588.top

Py:   def total(*args): return sum(args)
来源：http://dtt.gogol.net.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://zao.zycfv.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://jgw.ppjwa.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://fjm.yj202588.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ynh.tianlin.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ilf.uphjek.com

Ruby: def total(*nums); nums.sum; end
来源：http://rnd.hfpthk.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ydg.zhengqikj.top

[C04] 命名参数 / 关键字参数
来源：http://emd.guannengcc.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://cgg.yanxiufei.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hmi.zhengqikj.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://jei.sufxvd.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mwb.yj20258.top

Java: // 无：用 Builder 模式或 record
来源：http://onb.kuanghao11.cn

Go:   // 无：用配置结构体参数
来源：http://ikh.jqgfzy.top

Ruby: f(a: 1, b: 2)
来源：http://brk.shzxlz.cn

C#:   f(a: 1, b: 2)
来源：http://sbv.mhx1999.top

[C05] 返回多个值
来源：http://tzl.hnqzz.top

Py:   return a, b
来源：http://nwt.jianghu66.top

PHP:  return [$a, $b];
来源：http://qzv.sxryk.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://kpq.zhengqikj.top

TS:   return { a, b };
来源：http://lbt.ydzc1.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xfw.0kj1m.cn

Go:   return a, b
来源：http://ivh.xinyue.icu

Ruby: return a, b
来源：http://iqz.0kj1m.cn

C#:   return (a, b);              // ValueTuple
来源：http://eam.cqqwz.cn

[C06] 匿名函数 / lambda
来源：http://jab.dianchejie.cn

Py:   square = lambda x: x * x
来源：http://ohn.9152youxi.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://lun.yongpay.top

JS:   const square = x => x * x;
来源：http://rsi.yangfankeji.com

TS:   const square = (x: number): number => x * x;
来源：http://hkg.hongshengwenyu.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://zso.quarkkingdee.top

Go:   sq := func(x int) int { return x * x }
来源：http://aqm.yuanzhike.top

Ruby: square = ->(x) { x * x }
来源：http://hjq.zdbjq.cn

C#:   Func<int, int> square = x => x * x;
来源：http://mft.vqdsnc.cn

[C07] 把函数作为参数传入
来源：http://rno.ivvv.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://gjj.chenzaomai.com

PHP:  array_map("strtoupper", $arr);
来源：http://udm.sufxvd.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hjy.zhiwuduotai.top

TS:   arr.map(String)
来源：http://frl.tarul.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wxq.cqqwz.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ksn.ydjk.org.cn

Ruby: arr.map(&:upcase)
来源：http://ewk.jinqigufen.top

C#:   arr.Select(s => s.ToUpper())
来源：http://yhq.tianlin.xyz

[C08] 闭包
来源：http://nnd.pycfn.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://chf.gzhubu.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://pgx.shanyushiyangkeji.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://brm.bjfxy.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://uhr.c1oappe.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ucb.guannengcc.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://gys.wangdashe.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://fmf.bbcook.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://sqx.ctjpmb.com

[C09] 递归
来源：http://kvb.wangdashe.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://rwp.kuanghao11.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://svq.svipenyu.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://loo.tarul.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://snk.xylfe.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://xgk.hysaishi.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://eim.gotoacloud.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://rdi.fzhhl.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://egm.ivvv.top

[C10] 变量作用域
来源：http://xfl.nwbrower.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hak.svipenyu.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ted.iojbl.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ksp.svipenyu.cn

TS:   同 JS
来源：http://scf.nanxinkj.top

Java: 方法内为块级作用域
来源：http://sco.hywenlv.cn

Go:   花括号块级作用域
来源：http://myk.tianlin.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://atk.9152youxi.cn

C#:   块级作用域
来源：http://obi.aizwys.cn

[C11] 模块导入与导出
来源：http://skr.fzhhl.top

Py:   from module import func
来源：http://iqj.yj20258888.top

PHP:  require "file.php";  或 use App\Service;
来源：http://ukb.ydzc1.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://owe.ctjpmb.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://yts.pycfn.com

Java: import java.util.List;
来源：http://eyr.guowangkeji.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://bov.yonumen.top

Ruby: require "json"; require_relative "./util"
来源：http://nur.ywan-chungtsiang.top

C#:   using System.Text;
来源：http://jdq.hywenlv.cn

[C12] 立即执行函数 IIFE
来源：http://onn.sweek.top

Py:   (lambda: print("run"))()
来源：http://sfw.sysykeji.top

PHP:  (function () { echo "run"; })();
来源：http://xrz.aizwys.cn

JS:   (() => { console.log("run"); })();
来源：http://pxa.jianghu66.top

TS:   (() => { console.log("run"); })();
来源：http://vay.xuanzx.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://yig.dianchejie.cn

Go:   func() { fmt.Println("run") }()
来源：http://zsz.fanxiaobao.xyz

Ruby: -> { puts "run" }.call
来源：http://azf.pycfn.com

C#:   // 无 IIFE：用静态构造函数
来源：http://bkp.yj202588.top

[C13] 类型声明 / 类型注解
来源：http://vek.sysykeji.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://xke.hywenlv.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://end.zdqjudy.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://oat.zycfv.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://csf.cashguo.top

Java: int add(int a, int b) { return a + b; }
来源：http://vhb.gogol.net.cn

Go:   func add(a, b int) int
来源：http://oiz.yongpay.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://vur.dashuyun.cn

C#:   int Add(int a, int b) => a + b;
来源：http://bdr.sysykeji.top

[C14] 泛型函数
来源：http://hlc.vqdsnc.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://czv.nwbrower.top

PHP:  // 无泛型
来源：http://jrb.xziqi.cn

JS:   // 无泛型
来源：http://lql.jinghuilouyu.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://epb.dashuyun.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://iac.pengpengdd.cyou

Go:   func First[T any](items []T) T { return items[0] }
来源：http://qmo.zhongyouzk.top

Ruby: # 无泛型
来源：http://atp.ehwqpu.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ojq.guowangkeji.top

[C15] 解构 / 展开参数
来源：http://cai.aizwys.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://gwb.quarkkingdee.top

PHP:  [$a, $b] = $pair;
来源：http://hhh.sxryk.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://rvd.jqgufenzy.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://txm.chenjidiqi.icu

Java: // 无解构
来源：http://zca.ivvv.top

Go:   // 无解构
来源：http://mex.daxiang520.top

Ruby: a, b = pair
来源：http://tzj.ywan-chungtsiang.top

C#:   var (a, b) = pair;
来源：http://fkt.dianchejie.cn

[C16] 函数 / 方法重载
来源：http://rdy.hesvh.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://cpl.pengpengdd.cyou

PHP:  // 无重载
来源：http://dzi.sweek.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://kfa.9152youxi.cn

TS:   // 用联合类型或重载签名声明
来源：http://ota.ppjwa.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://fii.cqqwz.cn

Go:   // 无重载：用不同函数名
来源：http://hdy.guannengcc.top

Ruby: # 无重载：靠动态参数
来源：http://lvc.cheryme.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://fsa.meibo888.top

================================================================================
来源：http://ayy.jinqigufen.top

D. 数组 / 列表 / 集合
来源：http://ywg.xingfuxueyuan.xyz

================================================================================
来源：http://fho.hammf.cn

[D01] 创建数组 / 列表
来源：http://yue.bjfxy.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://wer.ywan-chungtsiang.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://qex.jianghu66.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ikd.birdmap.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://elj.aibaodan.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://nei.sjlbkw.cn

Go:   arr := []int{1, 2, 3}
来源：http://gdo.gotoacloud.top

Ruby: arr = [1, 2, 3]
来源：http://ypf.shuidangran.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://xpj.dashuyun.cn

[D02] 追加元素到末尾
来源：http://wpq.yvedp.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ivl.hysaishi.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://kol.fzhhl.top

JS:   arr.push(4);
来源：http://ibp.sysykeji.top

TS:   arr.push(4);
来源：http://vca.zdqjudy.top

Java: list.add(4);
来源：http://gnq.ehwqpu.com

Go:   arr = append(arr, 4)
来源：http://lpm.cucudq.cn

Ruby: arr << 4; arr.push(5)
来源：http://uiy.chenjidiqi.icu

C#:   list.Add(4);
来源：http://axt.yonumen.top

[D03] 在指定位置插入元素
来源：http://nxc.sjlbkw.cn

Py:   arr.insert(0, 0)
来源：http://fsh.xylfe.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://jsf.cheryme.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://leb.tanke756.top

TS:   arr.splice(0, 0, 0);
来源：http://qmo.hcnkem.com

Java: list.add(0, 0);
来源：http://crp.zdqjudy.top

Go:   arr = append([]int{0}, arr...)
来源：http://uub.jiagoushi.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://aen.smart0.xyz

C#:   list.Insert(0, 0);
来源：http://zpj.uphjek.com

[D04] 删除元素
来源：http://cdm.yvedp.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://oow.aibaodan.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hyc.hfpthk.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://pra.cheryme.top

TS:   arr.splice(0, 1);
来源：http://pmq.hongshengwenyu.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://fnx.nwbrower.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://dvg.vqdsnc.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://uuu.jlsjyb.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xan.shangyingyoupin.top

[D05] 访问与修改元素
来源：http://zfi.uphjek.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://xjt.cheryme.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://quf.zhoulong.xyz

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://gap.nwbrower.top

TS:   arr[0]; arr.at(-1);
来源：http://fab.shanyushiyangtech.top

Java: list.get(0); list.set(0, 9);
来源：http://wdc.cashguo.top

Go:   arr[0]; arr[0] = 9
来源：http://luf.xziqi.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wmz.chenjidiqi.icu

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zem.shangyingyoupin.top

[D06] 数组长度
来源：http://xbd.jianghu66.top

Py:   len(arr)
来源：http://bdv.svipenyu.cn

PHP:  count($arr);
来源：http://mnw.xylfe.cn

JS:   arr.length
来源：http://xxb.tanke756.top

TS:   arr.length
来源：http://ykf.hesvh.cn

Java: list.size();
来源：http://qpa.yj20258.top

Go:   len(arr)
来源：http://lki.tian-w.cn

Ruby: arr.length; arr.size
来源：http://mpt.shanyushiyangkeji.top

C#:   list.Count;
来源：http://ict.zhengqikj.top

[D07] 切片 / 取子数组
来源：http://gab.hysaishi.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://rgo.zhiwuduotai.top

PHP:  array_slice($arr, 1, 3);
来源：http://hgs.pengpengdd.cyou

JS:   arr.slice(1, 4);
来源：http://ise.tarul.cn

TS:   arr.slice(1, 4);
来源：http://xue.fktsv.cn

Java: list.subList(1, 4);
来源：http://tnl.sxryk.cn

Go:   arr[1:4]
来源：http://qwb.hnqzz.top

Ruby: arr[1, 3]
来源：http://jxq.uphjek.com

C#:   list.GetRange(1, 3);
来源：http://yeb.jinqigufen.top

[D08] 合并两个数组
来源：http://ckp.zhijiandao.cn

Py:   a + b;  a.extend(b)
来源：http://ztd.sysykeji.top

PHP:  array_merge($a, $b);
来源：http://jrr.wangdashe.top

JS:   [...a, ...b];  a.concat(b);
来源：http://nmu.316326.xyz

TS:   [...a, ...b];
来源：http://buc.ppjwa.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://dqc.cdnleiting.top

Go:   append(a, b...)
来源：http://wjy.hesvh.cn

Ruby: a + b;  a.concat(b)
来源：http://bya.ctjpmb.com

C#:   a.Concat(b).ToList()
来源：http://ymc.redwolf501.top

[D09] 排序（升序）
来源：http://gvu.cucudq.cn

Py:   sorted(arr);  arr.sort()
来源：http://ins.chenzaomai.com

PHP:  sort($arr);
来源：http://cds.hnqzz.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://qbl.haohaochexian.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://hzo.yfazqb.com

Java: Collections.sort(list);  list.sort(null);
来源：http://hif.ydzc1.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://inn.yj20258888.top

Ruby: arr.sort
来源：http://wyi.mhx1999.top

C#:   list.Sort();
来源：http://eeg.cucudq.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://txn.yuxming.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://gyc.jlsjyb.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://txb.yongpay.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://nqk.redwolf501.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://tht.nanxuanxn.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ypi.mhx1999.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://utx.xylfe.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://pde.jinqigufen.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://bnc.cashguo.top

[D11] 反转数组
来源：http://imt.0kj1m.cn

Py:   arr[::-1];  arr.reverse()
来源：http://xel.ehwqpu.com

PHP:  array_reverse($arr);
来源：http://hrc.chenjidiqi.icu

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ear.zdqjudy.top

TS:   [...arr].reverse();
来源：http://dsy.kuanghao11.cn

Java: Collections.reverse(list);
来源：http://mze.aizwys.cn

Go:   slices.Reverse(arr)
来源：http://wdj.hesvh.cn

Ruby: arr.reverse
来源：http://xwk.tianlin.xyz

C#:   list.Reverse();
来源：http://uxt.pengpengdd.cyou

[D12] 查找元素下标
来源：http://xgl.andypj.xyz

Py:   arr.index(x);  x in arr
来源：http://vic.yonumen.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://xqy.vehdjk.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pgk.pengpengdd.cyou

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://klj.mhx1999.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://scx.mhx1999.top

Go:   slices.Index(arr, x)
来源：http://fcz.cqqwz.cn

Ruby: arr.index(x)
来源：http://mam.tian-w.cn

C#:   list.IndexOf(x);
来源：http://zut.smart0.xyz

[D13] 过滤（保留满足条件的）
来源：http://dcb.redwolf501.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://nvg.jiagoushi.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://zug.jinqigfzy.top

JS:   arr.filter(x => x > 3)
来源：http://ifh.snrcjt.cn

TS:   arr.filter(x => x > 3)
来源：http://rxi.uphjek.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://tlr.xingfuxueyuan.xyz

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://vsn.hongshengwenyu.top

Ruby: arr.select { |x| x > 3 }
来源：http://rlo.sxryk.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://reb.hammf.cn

[D14] 映射转换（每个元素变形）
来源：http://avi.shuidangran.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://dhc.sxryk.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://kkd.ppjwa.cn

JS:   arr.map(x => x * 2)
来源：http://ech.bbcook.cn

TS:   arr.map(x => x * 2)
来源：http://oga.yongpay.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://qge.hysaishi.cn

Go:   // 手写循环
来源：http://aqt.mhx1999.top

Ruby: arr.map { |x| x * 2 }
来源：http://ftv.nanxuanxn.top

C#:   list.Select(x => x * 2).ToList()
来源：http://lkv.wangdashe.top

[D15] 去重
来源：http://ixt.fengsongda.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://knt.haohaochexian.top

PHP:  array_unique($arr);
来源：http://prm.ydzc1.top

JS:   [...new Set(arr)]
来源：http://qlp.zhiwuduotai.top


<!-- 参考信息 -->