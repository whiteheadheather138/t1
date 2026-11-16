代发 wailian999

Java: do { i++; } while (i < 10);
来源：http://oit.meibo888.top

Go:   for { i++; if i >= 10 { break } }
来源：http://upu.nwbrower.top

Ruby: begin; i += 1; end while i < 10
来源：http://tma.dianchejie.cn

C#:   do { i++; } while (i < 10);
来源：http://jua.xingfuxueyuan.xyz

[B09] break 与 continue
来源：http://qev.yangfankeji.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://fud.hywenlv.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://xyr.9152youxi.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lal.chenlongwang.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dwa.vqdsnc.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xkp.zhoulong.xyz

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://oaw.hcnkem.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ayx.shuidangran.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yhb.iojbl.cn

[B10] 遍历同时拿索引
来源：http://zvj.haohaochexian.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://eos.pycfn.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://xtq.shanyushiyangtech.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xht.xylfe.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://dwj.xylfe.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hgx.fehbvm.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://amy.gzhubu.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ymx.zdqjudy.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://toa.gzhubu.top

[B11] 生成数字序列 / 区间
来源：http://wes.hammf.cn

Py:   list(range(0, 10, 2))
来源：http://ewf.andypj.xyz

PHP:  range(0, 10, 2);
来源：http://rbe.haohaochexian.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nuu.xinyue.icu

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gma.ydjk.org.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://grt.hammf.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://kum.0kj1m.cn

Ruby: (0...10).step(2).to_a
来源：http://soq.wangdashe.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://qme.zhijiandao.cn

[B12] 跳出多层循环
来源：http://utd.ivvv.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://cfu.epnwcf.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://quu.chenlongwang.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://qqe.fengsongda.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://fbu.jinghuilouyu.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://nzx.havefunace.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://drd.tian-w.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://rkq.mhx1999.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://zvy.yfazqb.com

[B13] 判断是否为数字
来源：http://kpg.wangshuangyany.cn

Py:   isinstance(x, (int, float))
来源：http://utv.cheryme.top

PHP:  is_numeric($x)
来源：http://hpk.yongpay.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pto.yonumen.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xuv.kuanghao11.cn

Java: x instanceof Number
来源：http://fmw.yanxiufei.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://pmc.chenjidiqi.icu

Ruby: x.is_a?(Numeric)
来源：http://mgo.chenlongwang.top

C#:   x is int or double or decimal
来源：http://mfo.guannengcc.top

[B14] 判断值是否在集合内
来源：http://hsr.yj202588.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://eaq.daria6918.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ioh.zhongyouzk.top

JS:   [1, 2, 3].includes(x)
来源：http://rix.sysykeji.top

TS:   [1, 2, 3].includes(x)
来源：http://siv.ivvv.top

Java: List.of(1, 2, 3).contains(x)
来源：http://hlt.hnqzz.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://tau.cashguo.top

Ruby: [1, 2, 3].include?(x)
来源：http://ego.guannengcc.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hfm.hnxiangtu.top

[B15] 布尔运算与取反
来源：http://qux.quarkkingdee.top

Py:   a and b or not c
来源：http://zek.shangyingyoupin.top

PHP:  $a && $b || !$c
来源：http://tni.c1oappe.top

JS:   a && b || !c
来源：http://gli.birdmap.top

TS:   a && b || !c
来源：http://tlt.jiagoushi.top

Java: a && b || !c
来源：http://qhw.xylfe.cn

Go:   a && b || !c
来源：http://gvf.jinqigfzy.top

Ruby: a && b || !c
来源：http://tjn.cqqwz.cn

C#:   a && b || !c
来源：http://vgg.c1oappe.top

[B16] 卫语句：不满足条件提前返回
来源：http://mrd.hammf.cn

Py:   if not data: return
来源：http://xjg.zhiwuduotai.top

PHP:  if (!$data) { return; }
来源：http://qjm.hysaishi.cn

JS:   if (!data) return;
来源：http://ngl.zhijiandao.cn

TS:   if (!data) return;
来源：http://riv.svipenyu.cn

Java: if (data == null) return;
来源：http://kxw.ivvv.top

Go:   if data == nil { return }
来源：http://zrd.yj20258.top

Ruby: return if data.nil?
来源：http://jqe.aizwys.cn

C#:   if (data == null) return;
来源：http://nqp.yfazqb.com

================================================================================
来源：http://vfb.iojbl.cn

C. 函数与作用域
来源：http://kql.yfazqb.com

================================================================================
来源：http://kft.xingfuxueyuan.xyz

[C01] 定义函数
来源：http://yja.quarkkingdee.top

Py:   def add(a, b): return a + b
来源：http://mlu.hnqzz.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sfg.nanxuanxn.top

JS:   function add(a, b) { return a + b; }
来源：http://bia.ivvv.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dvi.nanxuanxn.top

Java: static int add(int a, int b) { return a + b; }
来源：http://byq.haohaochexian.top

Go:   func add(a, b int) int { return a + b }
来源：http://ihn.zhoulong.xyz

Ruby: def add(a, b); a + b; end
来源：http://shz.yonumen.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://nmm.daria6918.cn

[C02] 默认参数
来源：http://apv.wangshuangyany.cn

Py:   def greet(name="World"): return name
来源：http://yja.jinghuilouyu.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://wzn.quarkkingdee.top

JS:   function greet(name = "World") { return name; }
来源：http://bbx.zdbjq.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://efo.epnwcf.com

Java: // 无默认参数：方法重载或 Optional
来源：http://ubb.pycfn.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://qgq.hysaishi.cn

Ruby: def greet(name = "World") = name
来源：http://odx.sxryk.cn

C#:   string Greet(string name = "World") => name;
来源：http://oqz.ehwqpu.com

[C03] 可变参数
来源：http://hck.kuanghao11.cn

Py:   def total(*args): return sum(args)
来源：http://jkx.sxryk.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://abf.yueranfly.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ujq.yj20258888.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://sam.snrcjt.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://kas.svipenyu.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://sek.cdnleiting.top

Ruby: def total(*nums); nums.sum; end
来源：http://zsx.yuanzhike.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ppu.yj20258888.top

[C04] 命名参数 / 关键字参数
来源：http://ouf.zdbjq.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mze.wangdashe.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://juz.snrcjt.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hyg.yuxming.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://uuf.hfpthk.cn

Java: // 无：用 Builder 模式或 record
来源：http://wsh.pycfn.com

Go:   // 无：用配置结构体参数
来源：http://gtv.hnxiangtu.top

Ruby: f(a: 1, b: 2)
来源：http://uie.jqgfzy.top

C#:   f(a: 1, b: 2)
来源：http://zox.ydjk.org.cn

[C05] 返回多个值
来源：http://yxv.zhongyouzk.top

Py:   return a, b
来源：http://fhv.tanke756.top

PHP:  return [$a, $b];
来源：http://oxl.yuxming.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://xsy.sjlbkw.cn

TS:   return { a, b };
来源：http://klx.guannengcc.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://jcx.jqgufenzy.top

Go:   return a, b
来源：http://qzb.ppjwa.cn

Ruby: return a, b
来源：http://lqw.yj202588.top

C#:   return (a, b);              // ValueTuple
来源：http://ubz.wangdashe.top

[C06] 匿名函数 / lambda
来源：http://mld.birdmap.top

Py:   square = lambda x: x * x
来源：http://mqa.smart0.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://rkd.wangdashe.top

JS:   const square = x => x * x;
来源：http://foz.guowangkeji.top

TS:   const square = (x: number): number => x * x;
来源：http://zss.mhx1999.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ila.zycfv.cn

Go:   sq := func(x int) int { return x * x }
来源：http://pzl.tianlin.xyz

Ruby: square = ->(x) { x * x }
来源：http://omv.nanxuanxn.top

C#:   Func<int, int> square = x => x * x;
来源：http://cix.bjfxy.top

[C07] 把函数作为参数传入
来源：http://ybv.kuanghao11.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://xzx.aibaodan.cn

PHP:  array_map("strtoupper", $arr);
来源：http://cfg.jinghuilouyu.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://fwv.hnqzz.top

TS:   arr.map(String)
来源：http://fev.fktsv.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://akq.shanyushiyangkeji.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ggw.fanxiaobao.xyz

Ruby: arr.map(&:upcase)
来源：http://akx.tian-w.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://fgn.jinqigfzy.top

[C08] 闭包
来源：http://hlo.9152youxi.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ggk.guannengcc.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mtq.bjfxy.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://dco.yj202588.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://gzj.chenlongwang.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://kmf.vqdsnc.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://adz.yuanzhike.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://shh.yvedp.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ikq.yj202588.top

[C09] 递归
来源：http://fec.52xcode.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ieh.zhiwuduotai.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://lai.hammf.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://noy.zycfv.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xcj.hysaishi.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://fpy.hcnkem.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://nco.sjlbkw.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://zif.guowangkeji.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://pvw.aibaodan.cn

[C10] 变量作用域
来源：http://cfl.yongpay.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://cad.guannengcc.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://aan.birdmap.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://drk.vehdjk.com

TS:   同 JS
来源：http://aey.fanxiaobao.xyz

Java: 方法内为块级作用域
来源：http://bmw.ehwqpu.com

Go:   花括号块级作用域
来源：http://weo.cucudq.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://uxe.gotoacloud.top

C#:   块级作用域
来源：http://clf.yongpay.top

[C11] 模块导入与导出
来源：http://ttp.sufxvd.cn

Py:   from module import func
来源：http://zdu.shzxlz.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://acn.316326.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://dwq.tarul.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://glq.yvedp.cn

Java: import java.util.List;
来源：http://ebu.hysaishi.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://vvr.pengpengdd.cyou

Ruby: require "json"; require_relative "./util"
来源：http://tyr.bbcook.cn

C#:   using System.Text;
来源：http://dag.feifeiyinyue.top

[C12] 立即执行函数 IIFE
来源：http://znw.hesvh.cn

Py:   (lambda: print("run"))()
来源：http://edw.jinqigufen.top

PHP:  (function () { echo "run"; })();
来源：http://krg.9152youxi.cn

JS:   (() => { console.log("run"); })();
来源：http://bod.jinqigfzy.top

TS:   (() => { console.log("run"); })();
来源：http://jdo.zhijiandao.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://xuw.gaohongyu789.top

Go:   func() { fmt.Println("run") }()
来源：http://mxn.hammf.cn

Ruby: -> { puts "run" }.call
来源：http://zrj.chenzaomai.com

C#:   // 无 IIFE：用静态构造函数
来源：http://tcy.yangfankeji.com

[C13] 类型声明 / 类型注解
来源：http://wjh.zhixingplan.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mue.fktsv.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zml.chenlongwang.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://tjq.jinyuanbaomall.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bwu.ivvv.top

Java: int add(int a, int b) { return a + b; }
来源：http://nut.fehbvm.com

Go:   func add(a, b int) int
来源：http://xck.uphjek.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://fau.aibaodan.cn

C#:   int Add(int a, int b) => a + b;
来源：http://usw.cashguo.top

[C14] 泛型函数
来源：http://tnp.tanke756.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://gxz.yongpay.top

PHP:  // 无泛型
来源：http://upj.yfazqb.com

JS:   // 无泛型
来源：http://twd.vehdjk.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://djy.andypj.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://cqq.ydjk.org.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://lkl.havefunace.top

Ruby: # 无泛型
来源：http://ucu.9152youxi.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xhg.yuxming.cn

[C15] 解构 / 展开参数
来源：http://gme.yvedp.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://pag.guowangkeji.top

PHP:  [$a, $b] = $pair;
来源：http://msi.gaohongyu789.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://vjx.guowangkeji.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://aoq.ybcxt.top

Java: // 无解构
来源：http://zfg.wangshuangyany.cn

Go:   // 无解构
来源：http://cid.pycfn.com

Ruby: a, b = pair
来源：http://mzl.fktsv.cn

C#:   var (a, b) = pair;
来源：http://fvk.meibo888.top

[C16] 函数 / 方法重载
来源：http://ftc.pycfn.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ucr.tian-w.cn

PHP:  // 无重载
来源：http://phq.havefunace.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://qqp.gzhubu.top

TS:   // 用联合类型或重载签名声明
来源：http://gza.birdmap.top

Java: void f(int a) {}  void f(String a) {}
来源：http://rag.meibo888.top

Go:   // 无重载：用不同函数名
来源：http://wkk.svipenyu.cn

Ruby: # 无重载：靠动态参数
来源：http://lsh.cashguo.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://nyk.xylfe.cn

================================================================================
来源：http://val.cheryme.top

D. 数组 / 列表 / 集合
来源：http://uyb.wangshuangyany.cn

================================================================================
来源：http://est.zycfv.cn

[D01] 创建数组 / 列表
来源：http://ebg.shangyingyoupin.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://wqj.zhongyouzk.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://jyg.cdnleiting.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://vof.zhoulong.xyz

TS:   const arr: number[] = [1, 2, 3];
来源：http://xay.zdbjq.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://zbl.jiagoushi.top

Go:   arr := []int{1, 2, 3}
来源：http://num.nanxuanxn.top

Ruby: arr = [1, 2, 3]
来源：http://brb.bjfxy.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wxh.yj20258.top

[D02] 追加元素到末尾
来源：http://msk.yj202588.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://azp.gaohongyu789.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wys.wangdashe.top

JS:   arr.push(4);
来源：http://xkr.nwbrower.top

TS:   arr.push(4);
来源：http://tmp.316326.xyz

Java: list.add(4);
来源：http://cpr.hnxiangtu.top

Go:   arr = append(arr, 4)
来源：http://fdc.jlsjyb.cn

Ruby: arr << 4; arr.push(5)
来源：http://ooh.zhiwuduotai.top

C#:   list.Add(4);
来源：http://zdt.iojbl.cn

[D03] 在指定位置插入元素
来源：http://nhb.vqdsnc.cn

Py:   arr.insert(0, 0)
来源：http://kvk.hnxiangtu.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://sao.bbcook.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://qkd.yfazqb.com

TS:   arr.splice(0, 0, 0);
来源：http://dno.guowangkeji.top

Java: list.add(0, 0);
来源：http://cyq.hesvh.cn

Go:   arr = append([]int{0}, arr...)
来源：http://bdm.hongshengwenyu.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://jam.hywenlv.cn

C#:   list.Insert(0, 0);
来源：http://iqr.yueranfly.top

[D04] 删除元素
来源：http://iuz.birdmap.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ddl.bbcook.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://aix.ybcxt.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://vnf.xuetiantiany.cn

TS:   arr.splice(0, 1);
来源：http://wah.fengsongda.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://yfo.zycfv.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://eqe.vehdjk.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://pvp.cqqwz.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://fka.ctjpmb.com

[D05] 访问与修改元素
来源：http://edg.hnqzz.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ijz.shanyushiyangkeji.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://okc.yj202588.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://zhi.hysaishi.cn

TS:   arr[0]; arr.at(-1);
来源：http://cqn.fehbvm.com

Java: list.get(0); list.set(0, 9);
来源：http://vsg.tianlin.xyz

Go:   arr[0]; arr[0] = 9
来源：http://lhp.aibaodan.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hfg.ehwqpu.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wdw.cheryme.top

[D06] 数组长度
来源：http://nji.cheryme.top

Py:   len(arr)
来源：http://anb.cheryme.top

PHP:  count($arr);
来源：http://pmu.meibo888.top

JS:   arr.length
来源：http://xsf.jlsjyb.cn

TS:   arr.length
来源：http://ijr.fanxiaobao.xyz

Java: list.size();
来源：http://tzy.shuidangran.top

Go:   len(arr)
来源：http://iue.fanxiaobao.xyz

Ruby: arr.length; arr.size
来源：http://jmd.jqgufenzy.top

C#:   list.Count;
来源：http://oau.snrcjt.cn

[D07] 切片 / 取子数组
来源：http://kvm.chenlongwang.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://vfp.ehwqpu.com

PHP:  array_slice($arr, 1, 3);
来源：http://dbe.tanke756.top

JS:   arr.slice(1, 4);
来源：http://xat.gaohongyu789.top

TS:   arr.slice(1, 4);
来源：http://dpx.shzxlz.cn

Java: list.subList(1, 4);
来源：http://bhp.wangdashe.top

Go:   arr[1:4]
来源：http://ddj.zhixingplan.top

Ruby: arr[1, 3]
来源：http://vgm.hongshengwenyu.top

C#:   list.GetRange(1, 3);
来源：http://rek.0kj1m.cn

[D08] 合并两个数组
来源：http://fof.ywan-chungtsiang.top

Py:   a + b;  a.extend(b)
来源：http://eab.chenzaomai.com

PHP:  array_merge($a, $b);
来源：http://xtg.wangshuangyany.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://jwh.nanxinkj.top

TS:   [...a, ...b];
来源：http://pul.epnwcf.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://afl.fanxiaobao.xyz

Go:   append(a, b...)
来源：http://hmt.redwolf501.top

Ruby: a + b;  a.concat(b)
来源：http://pym.vehdjk.com

C#:   a.Concat(b).ToList()
来源：http://oam.52xcode.cn

[D09] 排序（升序）
来源：http://krm.sufxvd.cn

Py:   sorted(arr);  arr.sort()
来源：http://acf.chenzaomai.com


<!-- 参考信息 -->