代发 wailian999

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://zdl.quarkkingdee.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://rfz.ehwqpu.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://isi.chenzaomai.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://fnq.yongpay.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://dqo.uphjek.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://rib.hnxiangtu.top

[B11] 生成数字序列 / 区间
来源：http://wyj.ehwqpu.com

Py:   list(range(0, 10, 2))
来源：http://jjq.cdnleiting.top

PHP:  range(0, 10, 2);
来源：http://udx.0kj1m.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vmb.epnwcf.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://auc.vehdjk.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://uuv.zhoulong.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://xna.shuidangran.top

Ruby: (0...10).step(2).to_a
来源：http://ryr.zhongyouzk.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://tap.yanxiufei.cn

[B12] 跳出多层循环
来源：http://vyn.yvedp.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://hrs.yuxming.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://qyn.iojbl.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://pvv.shzxlz.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://qrm.jqgfzy.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://tfc.hnxiangtu.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://fyj.hnxiangtu.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://crd.tianlin.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://jrw.sxryk.cn

[B13] 判断是否为数字
来源：http://nvx.shzxlz.cn

Py:   isinstance(x, (int, float))
来源：http://omq.iojbl.cn

PHP:  is_numeric($x)
来源：http://kog.nanxuanxn.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yiy.cqqwz.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cvs.yj20258888.top

Java: x instanceof Number
来源：http://oeg.yfazqb.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://gfs.dashuyun.cn

Ruby: x.is_a?(Numeric)
来源：http://edq.birdmap.top

C#:   x is int or double or decimal
来源：http://jrv.xylfe.cn

[B14] 判断值是否在集合内
来源：http://ejb.gogol.net.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://qjo.nanxuanxn.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://vrp.pengpengdd.cyou

JS:   [1, 2, 3].includes(x)
来源：http://ttc.fehbvm.com

TS:   [1, 2, 3].includes(x)
来源：http://zso.jqgufenzy.top

Java: List.of(1, 2, 3).contains(x)
来源：http://zep.fktsv.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://sce.xylfe.cn

Ruby: [1, 2, 3].include?(x)
来源：http://yzd.shzxlz.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ftf.xinyue.icu

[B15] 布尔运算与取反
来源：http://ixa.ivvv.top

Py:   a and b or not c
来源：http://cyh.smart0.xyz

PHP:  $a && $b || !$c
来源：http://yvj.jiagoushi.top

JS:   a && b || !c
来源：http://vii.yj20258888.top

TS:   a && b || !c
来源：http://xfo.zhongyouzk.top

Java: a && b || !c
来源：http://gcy.guannengcc.top

Go:   a && b || !c
来源：http://xhk.guannengcc.top

Ruby: a && b || !c
来源：http://pbf.jiagoushi.top

C#:   a && b || !c
来源：http://ijw.guowangkeji.top

[B16] 卫语句：不满足条件提前返回
来源：http://rtj.jqgufenzy.top

Py:   if not data: return
来源：http://kqo.snrcjt.cn

PHP:  if (!$data) { return; }
来源：http://vrw.pengpengdd.cyou

JS:   if (!data) return;
来源：http://yoz.hfpthk.cn

TS:   if (!data) return;
来源：http://vkj.redwolf501.top

Java: if (data == null) return;
来源：http://tyw.jqgufenzy.top

Go:   if data == nil { return }
来源：http://usl.shanyushiyangkeji.top

Ruby: return if data.nil?
来源：http://ujd.jqgufenzy.top

C#:   if (data == null) return;
来源：http://jyz.jqgfzy.top

================================================================================
来源：http://lqq.ctjpmb.com

C. 函数与作用域
来源：http://fov.ehwqpu.com

================================================================================
来源：http://zqk.yfazqb.com

[C01] 定义函数
来源：http://uts.mhx1999.top

Py:   def add(a, b): return a + b
来源：http://rll.iojbl.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pzo.chenjidiqi.icu

JS:   function add(a, b) { return a + b; }
来源：http://ype.yvedp.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://oeo.shangyingyoupin.top

Java: static int add(int a, int b) { return a + b; }
来源：http://rso.ivvv.top

Go:   func add(a, b int) int { return a + b }
来源：http://rom.shzxlz.cn

Ruby: def add(a, b); a + b; end
来源：http://kik.zhiwuduotai.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://bbv.cashguo.top

[C02] 默认参数
来源：http://erb.gzhubu.top

Py:   def greet(name="World"): return name
来源：http://nnh.fengsongda.top

PHP:  function greet($name = "World") { return $name; }
来源：http://bwd.chenjidiqi.icu

JS:   function greet(name = "World") { return name; }
来源：http://lzv.hnxiangtu.top

TS:   function greet(name: string = "World") { return name; }
来源：http://sdq.0kj1m.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://alh.zhaomingkeji.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://omz.feifeiyinyue.top

Ruby: def greet(name = "World") = name
来源：http://kvo.jinyuanbaomall.cn

C#:   string Greet(string name = "World") => name;
来源：http://ucd.gotoacloud.top

[C03] 可变参数
来源：http://mox.xingfuxueyuan.xyz

Py:   def total(*args): return sum(args)
来源：http://fzg.nanxuanxn.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://cnf.tanke756.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://eom.sjlbkw.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://rrd.xuanzx.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://lwq.fktsv.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wtm.tianlin.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://mxb.aibaodan.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://thc.havefunace.top

[C04] 命名参数 / 关键字参数
来源：http://eyi.hfpthk.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ipb.hnxiangtu.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xsh.fengsongda.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xhj.yj20258888.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://fnx.316326.xyz

Java: // 无：用 Builder 模式或 record
来源：http://qhl.tianlin.xyz

Go:   // 无：用配置结构体参数
来源：http://pcm.cdnleiting.top

Ruby: f(a: 1, b: 2)
来源：http://fuv.xingfuxueyuan.xyz

C#:   f(a: 1, b: 2)
来源：http://tqj.ydzc1.top

[C05] 返回多个值
来源：http://sas.nanxuanxn.top

Py:   return a, b
来源：http://jko.jqgfzy.top

PHP:  return [$a, $b];
来源：http://juw.tanke756.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://zsw.chenzaomai.com

TS:   return { a, b };
来源：http://fdj.tianlin.xyz

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://uzs.ivvv.top

Go:   return a, b
来源：http://byk.xingfuxueyuan.xyz

Ruby: return a, b
来源：http://byx.yueranfly.top

C#:   return (a, b);              // ValueTuple
来源：http://igm.gotoacloud.top

[C06] 匿名函数 / lambda
来源：http://pxf.zhengqikj.top

Py:   square = lambda x: x * x
来源：http://yhl.shanyushiyangkeji.top

PHP:  $square = fn($x) => $x * $x;
来源：http://pop.fehbvm.com

JS:   const square = x => x * x;
来源：http://fxf.aizwys.cn

TS:   const square = (x: number): number => x * x;
来源：http://fsv.jiagoushi.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://xne.c1oappe.top

Go:   sq := func(x int) int { return x * x }
来源：http://jwb.sxryk.cn

Ruby: square = ->(x) { x * x }
来源：http://fxh.hcnkem.com

C#:   Func<int, int> square = x => x * x;
来源：http://vwe.nanxuanxn.top

[C07] 把函数作为参数传入
来源：http://pmu.xingfuxueyuan.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://xpq.vehdjk.com

PHP:  array_map("strtoupper", $arr);
来源：http://jlw.kuanghao11.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://lku.zhijiandao.cn

TS:   arr.map(String)
来源：http://mft.gzhubu.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://tzp.tanke756.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://pcj.9152youxi.cn

Ruby: arr.map(&:upcase)
来源：http://vmk.smart0.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://fss.daxiang520.top

[C08] 闭包
来源：http://yvv.wangshuangyany.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://krz.zhixingplan.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://rjz.xinyue.icu

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://aiu.ydjk.org.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://slh.cdnleiting.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://zfj.shangyingyoupin.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://lkk.sufxvd.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://sws.sufxvd.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://zxo.sufxvd.cn

[C09] 递归
来源：http://yrw.xziqi.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ojh.yuanzhike.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://zba.andypj.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qfs.uphjek.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bqc.sufxvd.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://kjy.yj202588.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://uhw.hywenlv.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://bbv.fengsongda.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://xpa.zhixingplan.top

[C10] 变量作用域
来源：http://crj.hongshengwenyu.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://usw.yvedp.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ahh.shuidangran.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://tbc.zhijiandao.cn

TS:   同 JS
来源：http://rtu.shzxlz.cn

Java: 方法内为块级作用域
来源：http://diq.fzhhl.top

Go:   花括号块级作用域
来源：http://qsx.wangshuangyany.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ihw.yangfankeji.com

C#:   块级作用域
来源：http://gju.sxryk.cn

[C11] 模块导入与导出
来源：http://pgc.wangdashe.top

Py:   from module import func
来源：http://hjy.tanke756.top

PHP:  require "file.php";  或 use App\Service;
来源：http://eph.hnxiangtu.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://ghk.chenzaomai.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://idx.uphjek.com

Java: import java.util.List;
来源：http://irk.hnqzz.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://qzn.jinyuanbaomall.cn

Ruby: require "json"; require_relative "./util"
来源：http://ojc.cucudq.cn

C#:   using System.Text;
来源：http://hdp.52xcode.cn

[C12] 立即执行函数 IIFE
来源：http://kdz.chenzaomai.com

Py:   (lambda: print("run"))()
来源：http://tvf.shanyushiyangkeji.top

PHP:  (function () { echo "run"; })();
来源：http://jom.daxiang520.top

JS:   (() => { console.log("run"); })();
来源：http://yma.zhengqikj.top

TS:   (() => { console.log("run"); })();
来源：http://jju.chenlongwang.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://rqp.xingfuxueyuan.xyz

Go:   func() { fmt.Println("run") }()
来源：http://ukz.daxiang520.top

Ruby: -> { puts "run" }.call
来源：http://mok.hesvh.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://lgk.jianghu66.top

[C13] 类型声明 / 类型注解
来源：http://bcq.uphjek.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://jii.gogol.net.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://iqk.snrcjt.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://aoy.c1oappe.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://otq.smart0.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://qvb.uphjek.com

Go:   func add(a, b int) int
来源：http://clr.tian-w.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://prl.meibo888.top

C#:   int Add(int a, int b) => a + b;
来源：http://cjt.feifeiyinyue.top

[C14] 泛型函数
来源：http://kgw.svipenyu.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://dub.daxiang520.top

PHP:  // 无泛型
来源：http://wkh.gaohongyu789.top

JS:   // 无泛型
来源：http://qsm.cashguo.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hrr.bjfxy.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ciu.gzhubu.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://neq.sweek.top

Ruby: # 无泛型
来源：http://iqj.aibaodan.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://nsz.xinyue.icu

[C15] 解构 / 展开参数
来源：http://gkf.nanxuanxn.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://jnx.bjfxy.top

PHP:  [$a, $b] = $pair;
来源：http://oix.zhongyouzk.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://jap.ctjpmb.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://xvt.chenlongwang.top

Java: // 无解构
来源：http://rgu.ppjwa.cn

Go:   // 无解构
来源：http://ikl.dashuyun.cn

Ruby: a, b = pair
来源：http://lco.316326.xyz

C#:   var (a, b) = pair;
来源：http://alq.fzhhl.top

[C16] 函数 / 方法重载
来源：http://tph.hywenlv.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://gyd.ydzc1.top

PHP:  // 无重载
来源：http://szq.wangshuangyany.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://bgj.ehwqpu.com

TS:   // 用联合类型或重载签名声明
来源：http://fvu.chenlongwang.top

Java: void f(int a) {}  void f(String a) {}
来源：http://scx.yanxiufei.cn

Go:   // 无重载：用不同函数名
来源：http://pxs.fengsongda.top

Ruby: # 无重载：靠动态参数
来源：http://tdi.zhongyouzk.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://bgg.cdnleiting.top

================================================================================
来源：http://pkt.ppjwa.cn

D. 数组 / 列表 / 集合
来源：http://shr.daria6918.cn

================================================================================
来源：http://ryh.zhijiandao.cn

[D01] 创建数组 / 列表
来源：http://ccz.sysykeji.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://kcs.nanxinkj.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://fga.mhx1999.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://dyd.shzxlz.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://gmx.bbcook.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://jgb.mhx1999.top

Go:   arr := []int{1, 2, 3}
来源：http://xwp.ivvv.top

Ruby: arr = [1, 2, 3]
来源：http://aay.pengpengdd.cyou

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://bmr.wangdashe.top

[D02] 追加元素到末尾
来源：http://ghu.pengpengdd.cyou

Py:   arr.append(4); arr.extend([5, 6])
来源：http://fjv.shuidangran.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://owe.sufxvd.cn

JS:   arr.push(4);
来源：http://qtn.fehbvm.com

TS:   arr.push(4);
来源：http://qqu.xinyue.icu

Java: list.add(4);
来源：http://fjj.iojbl.cn

Go:   arr = append(arr, 4)
来源：http://dcz.yanxiufei.cn

Ruby: arr << 4; arr.push(5)
来源：http://ohr.aibaodan.cn

C#:   list.Add(4);
来源：http://ynb.chenzaomai.com

[D03] 在指定位置插入元素
来源：http://znb.cqqwz.cn

Py:   arr.insert(0, 0)
来源：http://zyk.tarul.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wgi.hywenlv.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://rth.jyoumei.cn

TS:   arr.splice(0, 0, 0);
来源：http://nzg.52xcode.cn

Java: list.add(0, 0);
来源：http://ezm.cqqwz.cn

Go:   arr = append([]int{0}, arr...)
来源：http://bqu.xylfe.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://nic.yueranfly.top

C#:   list.Insert(0, 0);
来源：http://cog.shanyushiyangkeji.top

[D04] 删除元素
来源：http://wyu.gotoacloud.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://gjx.pengpengdd.cyou

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://jsw.hywenlv.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://qwx.yongpay.top

TS:   arr.splice(0, 1);
来源：http://sgm.haohaochexian.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://sog.yj20258.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://qqu.fehbvm.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://sor.svipenyu.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://qas.yuanzhike.top

[D05] 访问与修改元素
来源：http://dtj.sweek.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://bzu.cqqwz.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://rmb.andypj.xyz

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://jhu.tanke756.top

TS:   arr[0]; arr.at(-1);
来源：http://ysa.hnxiangtu.top

Java: list.get(0); list.set(0, 9);
来源：http://tep.andypj.xyz

Go:   arr[0]; arr[0] = 9
来源：http://nqp.sufxvd.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://rww.yj20258888.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://xhw.yonumen.top

[D06] 数组长度
来源：http://jlr.nanxuanxn.top

Py:   len(arr)
来源：http://xoy.hfpthk.cn

PHP:  count($arr);
来源：http://vlq.smart0.xyz

JS:   arr.length
来源：http://rhi.sysykeji.top

TS:   arr.length
来源：http://cfa.hywenlv.cn

Java: list.size();
来源：http://krm.zdbjq.cn

Go:   len(arr)
来源：http://ezn.zhaomingkeji.xyz

Ruby: arr.length; arr.size
来源：http://voh.nwbrower.top

C#:   list.Count;
来源：http://xrz.haohaochexian.top

[D07] 切片 / 取子数组
来源：http://rjl.zhiwuduotai.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://cyy.chenzaomai.com

PHP:  array_slice($arr, 1, 3);
来源：http://gqn.zhongyouzk.top

JS:   arr.slice(1, 4);
来源：http://odw.cheryme.top

TS:   arr.slice(1, 4);
来源：http://cib.tian-w.cn

Java: list.subList(1, 4);
来源：http://bta.hywenlv.cn

Go:   arr[1:4]
来源：http://byu.jianghu66.top

Ruby: arr[1, 3]
来源：http://eum.gzhubu.top

C#:   list.GetRange(1, 3);
来源：http://ukb.jlsjyb.cn

[D08] 合并两个数组
来源：http://exj.mhx1999.top

Py:   a + b;  a.extend(b)
来源：http://tpd.ivvv.top

PHP:  array_merge($a, $b);
来源：http://pug.zhaomingkeji.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://apl.redwolf501.top

TS:   [...a, ...b];
来源：http://ztm.xinyue.icu

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ixq.9152youxi.cn

Go:   append(a, b...)
来源：http://mux.guowangkeji.top

Ruby: a + b;  a.concat(b)
来源：http://haz.yonumen.top

C#:   a.Concat(b).ToList()
来源：http://uwr.chenlongwang.top

[D09] 排序（升序）
来源：http://hwa.yj202588.top

Py:   sorted(arr);  arr.sort()
来源：http://zel.havefunace.top

PHP:  sort($arr);
来源：http://zdo.mhx1999.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://qqx.hammf.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://lsl.jinghuilouyu.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://vhg.jqgfzy.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://pfb.jinqigufen.top

Ruby: arr.sort
来源：http://dex.nanxuanxn.top

C#:   list.Sort();
来源：http://jrr.dashuyun.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://hlg.meibo888.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://cfd.nanxinkj.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://sdj.zhiwuduotai.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://fja.ydjk.org.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://nqx.jqgfzy.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://vxl.xylfe.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://nye.havefunace.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mwl.jqgfzy.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://frz.yanxiufei.cn


<!-- 参考信息 -->