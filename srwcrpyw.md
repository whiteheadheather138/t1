代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://fhl.xziqi.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://hxc.andypj.xyz

JS:   do { i++; } while (i < 10);
来源：http://qoc.jqgufenzy.top

TS:   do { i++; } while (i < 10);
来源：http://krv.tianlin.xyz

Java: do { i++; } while (i < 10);
来源：http://acz.52xcode.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://iht.fktsv.cn

Ruby: begin; i += 1; end while i < 10
来源：http://gqd.snrcjt.cn

C#:   do { i++; } while (i < 10);
来源：http://jbn.sjlbkw.cn

[B09] break 与 continue
来源：http://emy.ivvv.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://dpp.tianlin.xyz

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://jnk.vqdsnc.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wkp.yvedp.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mkv.nanxuanxn.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eqd.sysykeji.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://coy.gotoacloud.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xyp.52xcode.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zov.epnwcf.com

[B10] 遍历同时拿索引
来源：http://qul.cashguo.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://cdm.hfpthk.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://egj.sweek.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://tye.hnxiangtu.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://iwr.jinqigufen.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://cob.hfpthk.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ftw.aibaodan.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://xou.c1oappe.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mzi.bbcook.cn

[B11] 生成数字序列 / 区间
来源：http://gvw.52xcode.cn

Py:   list(range(0, 10, 2))
来源：http://qhz.hcnkem.com

PHP:  range(0, 10, 2);
来源：http://bvo.redwolf501.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://raz.zhaomingkeji.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dmj.sufxvd.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mmx.gaohongyu789.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://lto.yanxiufei.cn

Ruby: (0...10).step(2).to_a
来源：http://eph.shzxlz.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zsr.tianlin.xyz

[B12] 跳出多层循环
来源：http://fci.epnwcf.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://mrb.ybcxt.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://krt.chenlongwang.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://lvr.xuanzx.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wce.hongshengwenyu.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://vxz.zhongyouzk.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://lgm.cheryme.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://orq.yuanzhike.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://yyq.epnwcf.com

[B13] 判断是否为数字
来源：http://ltu.hammf.cn

Py:   isinstance(x, (int, float))
来源：http://pmu.9152youxi.cn

PHP:  is_numeric($x)
来源：http://ixr.shanyushiyangtech.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wxc.hesvh.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vlr.quarkkingdee.top

Java: x instanceof Number
来源：http://rhi.ppjwa.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ywd.ehwqpu.com

Ruby: x.is_a?(Numeric)
来源：http://otp.yongpay.top

C#:   x is int or double or decimal
来源：http://fgw.bbcook.cn

[B14] 判断值是否在集合内
来源：http://fsq.ydzc1.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://gcv.nanxinkj.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ufa.yuxming.cn

JS:   [1, 2, 3].includes(x)
来源：http://yzs.guowangkeji.top

TS:   [1, 2, 3].includes(x)
来源：http://dgc.zhixingplan.top

Java: List.of(1, 2, 3).contains(x)
来源：http://cwt.epnwcf.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://pjo.ywan-chungtsiang.top

Ruby: [1, 2, 3].include?(x)
来源：http://xgj.tanke756.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mxl.wangdashe.top

[B15] 布尔运算与取反
来源：http://qex.cqqwz.cn

Py:   a and b or not c
来源：http://vpd.cqqwz.cn

PHP:  $a && $b || !$c
来源：http://mok.cdnleiting.top

JS:   a && b || !c
来源：http://opf.redwolf501.top

TS:   a && b || !c
来源：http://hms.yanxiufei.cn

Java: a && b || !c
来源：http://ynf.yvedp.cn

Go:   a && b || !c
来源：http://aex.zhixingplan.top

Ruby: a && b || !c
来源：http://xcd.zhengqikj.top

C#:   a && b || !c
来源：http://rtn.cdnleiting.top

[B16] 卫语句：不满足条件提前返回
来源：http://bdv.jinqigufen.top

Py:   if not data: return
来源：http://chh.xylfe.cn

PHP:  if (!$data) { return; }
来源：http://iso.jyoumei.cn

JS:   if (!data) return;
来源：http://pdr.cqqwz.cn

TS:   if (!data) return;
来源：http://jko.shzxlz.cn

Java: if (data == null) return;
来源：http://cbi.vqdsnc.cn

Go:   if data == nil { return }
来源：http://kkk.yuxming.cn

Ruby: return if data.nil?
来源：http://yxp.daria6918.cn

C#:   if (data == null) return;
来源：http://hdj.yvedp.cn

================================================================================
来源：http://hbn.bbcook.cn

C. 函数与作用域
来源：http://clm.316326.xyz

================================================================================
来源：http://boo.aibaodan.cn

[C01] 定义函数
来源：http://lst.haohaochexian.top

Py:   def add(a, b): return a + b
来源：http://cgk.ydjk.org.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mea.zhaomingkeji.xyz

JS:   function add(a, b) { return a + b; }
来源：http://vlp.hesvh.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lmx.nwbrower.top

Java: static int add(int a, int b) { return a + b; }
来源：http://fze.guannengcc.top

Go:   func add(a, b int) int { return a + b }
来源：http://vaz.nwbrower.top

Ruby: def add(a, b); a + b; end
来源：http://iov.316326.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://tip.fehbvm.com

[C02] 默认参数
来源：http://bbs.bbcook.cn

Py:   def greet(name="World"): return name
来源：http://kaz.meibo888.top

PHP:  function greet($name = "World") { return $name; }
来源：http://lpw.tarul.cn

JS:   function greet(name = "World") { return name; }
来源：http://iak.tian-w.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ivp.epnwcf.com

Java: // 无默认参数：方法重载或 Optional
来源：http://ljf.yj20258888.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://iwd.hammf.cn

Ruby: def greet(name = "World") = name
来源：http://tqx.zycfv.cn

C#:   string Greet(string name = "World") => name;
来源：http://fvz.yj202588.top

[C03] 可变参数
来源：http://hfi.guannengcc.top

Py:   def total(*args): return sum(args)
来源：http://pmg.guowangkeji.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://fde.jqgufenzy.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://gby.jinghuilouyu.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://kgm.tianlin.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://fsw.hcnkem.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://zat.ydjk.org.cn

Ruby: def total(*nums); nums.sum; end
来源：http://qwv.aizwys.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://vao.zhijiandao.cn

[C04] 命名参数 / 关键字参数
来源：http://ctm.guannengcc.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://cnh.tarul.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://qqt.sxryk.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://zuq.ydjk.org.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://uzr.andypj.xyz

Java: // 无：用 Builder 模式或 record
来源：http://sua.yvedp.cn

Go:   // 无：用配置结构体参数
来源：http://cvw.snrcjt.cn

Ruby: f(a: 1, b: 2)
来源：http://gki.daxiang520.top

C#:   f(a: 1, b: 2)
来源：http://obl.jinghuilouyu.cn

[C05] 返回多个值
来源：http://fsz.uphjek.com

Py:   return a, b
来源：http://xfv.fzhhl.top

PHP:  return [$a, $b];
来源：http://zip.smart0.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://cog.chenlongwang.top

TS:   return { a, b };
来源：http://fxz.jinghuilouyu.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://eua.hongshengwenyu.top

Go:   return a, b
来源：http://yhe.yj20258.top

Ruby: return a, b
来源：http://iok.feifeiyinyue.top

C#:   return (a, b);              // ValueTuple
来源：http://tls.yangfankeji.com

[C06] 匿名函数 / lambda
来源：http://zrn.fktsv.cn

Py:   square = lambda x: x * x
来源：http://rzs.zycfv.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://uaz.jiagoushi.top

JS:   const square = x => x * x;
来源：http://zfn.fktsv.cn

TS:   const square = (x: number): number => x * x;
来源：http://zsn.redwolf501.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://bfp.tian-w.cn

Go:   sq := func(x int) int { return x * x }
来源：http://kjq.jinqigufen.top

Ruby: square = ->(x) { x * x }
来源：http://uiz.birdmap.top

C#:   Func<int, int> square = x => x * x;
来源：http://gmf.feifeiyinyue.top

[C07] 把函数作为参数传入
来源：http://itz.gogol.net.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://fwo.xinyue.icu

PHP:  array_map("strtoupper", $arr);
来源：http://lxr.hongshengwenyu.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xhy.cheryme.top

TS:   arr.map(String)
来源：http://mxr.c1oappe.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://pbo.hnxiangtu.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qjp.hcnkem.com

Ruby: arr.map(&:upcase)
来源：http://pjz.hfpthk.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://set.svipenyu.cn

[C08] 闭包
来源：http://vnk.ppjwa.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://lfk.hesvh.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://cib.chenjidiqi.icu

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://dfn.xylfe.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://epc.fzhhl.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://eaa.cheryme.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://nhf.cashguo.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://dpp.jinghuilouyu.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://iib.birdmap.top

[C09] 递归
来源：http://gui.hywenlv.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://fbo.jlsjyb.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://dvr.hywenlv.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://oir.mhx1999.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ilg.pengpengdd.cyou

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://nel.guannengcc.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mjk.quarkkingdee.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://exg.tarul.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://rjn.tarul.cn

[C10] 变量作用域
来源：http://uuv.kuanghao11.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://tes.cucudq.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://qow.jiagoushi.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://dsp.yj20258888.top

TS:   同 JS
来源：http://xoz.nwbrower.top

Java: 方法内为块级作用域
来源：http://zyz.zhixingplan.top

Go:   花括号块级作用域
来源：http://pxz.ehwqpu.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://amu.yonumen.top

C#:   块级作用域
来源：http://zhi.jinqigufen.top

[C11] 模块导入与导出
来源：http://muy.sxryk.cn

Py:   from module import func
来源：http://uee.shzxlz.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://cbi.zhengqikj.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://xky.jinqigfzy.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://nct.shzxlz.cn

Java: import java.util.List;
来源：http://lpp.yj20258.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://qkd.zdqjudy.top

Ruby: require "json"; require_relative "./util"
来源：http://qyp.cheryme.top

C#:   using System.Text;
来源：http://cza.wangshuangyany.cn

[C12] 立即执行函数 IIFE
来源：http://cdv.cashguo.top

Py:   (lambda: print("run"))()
来源：http://lhx.yj20258888.top

PHP:  (function () { echo "run"; })();
来源：http://bzl.52xcode.cn

JS:   (() => { console.log("run"); })();
来源：http://vrj.bbcook.cn

TS:   (() => { console.log("run"); })();
来源：http://njv.pengpengdd.cyou

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://bly.52xcode.cn

Go:   func() { fmt.Println("run") }()
来源：http://sbr.shanyushiyangtech.top

Ruby: -> { puts "run" }.call
来源：http://iib.jinqigfzy.top

C#:   // 无 IIFE：用静态构造函数
来源：http://hsm.snrcjt.cn

[C13] 类型声明 / 类型注解
来源：http://ewt.jyoumei.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mdd.mhx1999.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zwl.ctjpmb.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://bzm.cashguo.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gjr.cheryme.top

Java: int add(int a, int b) { return a + b; }
来源：http://zji.ppjwa.cn

Go:   func add(a, b int) int
来源：http://oer.daria6918.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://luc.mhx1999.top

C#:   int Add(int a, int b) => a + b;
来源：http://vhn.yuxming.cn

[C14] 泛型函数
来源：http://rpn.hysaishi.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://pza.jqgufenzy.top

PHP:  // 无泛型
来源：http://pxg.yuanzhike.top

JS:   // 无泛型
来源：http://ggv.jinqigufen.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://guk.vehdjk.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://rrk.nanxuanxn.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://jcb.uphjek.com

Ruby: # 无泛型
来源：http://det.vehdjk.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://vpz.pengpengdd.cyou

[C15] 解构 / 展开参数
来源：http://gzi.xylfe.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://iwa.fktsv.cn

PHP:  [$a, $b] = $pair;
来源：http://qen.gaohongyu789.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://uwy.yonumen.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ooj.sufxvd.cn

Java: // 无解构
来源：http://les.jinghuilouyu.cn

Go:   // 无解构
来源：http://koc.bjfxy.top

Ruby: a, b = pair
来源：http://ohc.52xcode.cn

C#:   var (a, b) = pair;
来源：http://hlo.xuetiantiany.cn

[C16] 函数 / 方法重载
来源：http://iqr.yuanzhike.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vsy.jinyuanbaomall.cn

PHP:  // 无重载
来源：http://pzs.cucudq.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://xll.nanxuanxn.top

TS:   // 用联合类型或重载签名声明
来源：http://swm.bbcook.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://sqc.jlsjyb.cn

Go:   // 无重载：用不同函数名
来源：http://uqk.iojbl.cn

Ruby: # 无重载：靠动态参数
来源：http://dgy.yueranfly.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://xgd.52xcode.cn

================================================================================
来源：http://mpj.gzhubu.top

D. 数组 / 列表 / 集合
来源：http://qiv.0kj1m.cn

================================================================================
来源：http://ugx.yvedp.cn

[D01] 创建数组 / 列表
来源：http://kha.yj202588.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://acw.yonumen.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://vtp.jqgfzy.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://qud.daxiang520.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://lau.ivvv.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ocp.shanyushiyangtech.top

Go:   arr := []int{1, 2, 3}
来源：http://mgl.jinghuilouyu.cn

Ruby: arr = [1, 2, 3]
来源：http://mll.hammf.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://rsv.jiagoushi.top

[D02] 追加元素到末尾
来源：http://ibg.zhaomingkeji.xyz

Py:   arr.append(4); arr.extend([5, 6])
来源：http://tpo.cashguo.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://nus.chenlongwang.top

JS:   arr.push(4);
来源：http://rjt.aibaodan.cn

TS:   arr.push(4);
来源：http://gyj.ywan-chungtsiang.top

Java: list.add(4);
来源：http://uyf.tianlin.xyz

Go:   arr = append(arr, 4)
来源：http://ivi.xylfe.cn

Ruby: arr << 4; arr.push(5)
来源：http://tgs.hywenlv.cn

C#:   list.Add(4);
来源：http://fyj.yueranfly.top

[D03] 在指定位置插入元素
来源：http://pjx.cucudq.cn

Py:   arr.insert(0, 0)
来源：http://mph.ehwqpu.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://pzi.yuanzhike.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://taz.guannengcc.top

TS:   arr.splice(0, 0, 0);
来源：http://tnn.aibaodan.cn

Java: list.add(0, 0);
来源：http://rht.redwolf501.top

Go:   arr = append([]int{0}, arr...)
来源：http://iyj.hesvh.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://zro.hnxiangtu.top

C#:   list.Insert(0, 0);
来源：http://xsn.fanxiaobao.xyz

[D04] 删除元素
来源：http://hfl.shanyushiyangtech.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ahk.yongpay.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://nzp.yanxiufei.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://fpd.nanxinkj.top

TS:   arr.splice(0, 1);
来源：http://ciq.xinyue.icu

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://chg.hongshengwenyu.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://fli.uphjek.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://jeq.quarkkingdee.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://vcw.gzhubu.top

[D05] 访问与修改元素
来源：http://gqx.zhixingplan.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://rkr.zdqjudy.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://kal.jqgfzy.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wse.ppjwa.cn

TS:   arr[0]; arr.at(-1);
来源：http://xky.sufxvd.cn

Java: list.get(0); list.set(0, 9);
来源：http://vjj.pengpengdd.cyou

Go:   arr[0]; arr[0] = 9
来源：http://cqu.svipenyu.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://grr.wangdashe.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://sbq.ehwqpu.com

[D06] 数组长度
来源：http://upi.tarul.cn

Py:   len(arr)
来源：http://ygn.zhijiandao.cn

PHP:  count($arr);
来源：http://jvr.xinyue.icu

JS:   arr.length
来源：http://ueu.yfazqb.com

TS:   arr.length
来源：http://cza.jqgfzy.top

Java: list.size();
来源：http://sbq.hfpthk.cn

Go:   len(arr)
来源：http://cat.52xcode.cn

Ruby: arr.length; arr.size
来源：http://zja.yanxiufei.cn

C#:   list.Count;
来源：http://sbl.c1oappe.top

[D07] 切片 / 取子数组
来源：http://oqm.meibo888.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wvf.zdbjq.cn

PHP:  array_slice($arr, 1, 3);
来源：http://wjb.zhaomingkeji.xyz

JS:   arr.slice(1, 4);
来源：http://ips.ppjwa.cn

TS:   arr.slice(1, 4);
来源：http://ufd.sweek.top

Java: list.subList(1, 4);
来源：http://eys.chenjidiqi.icu

Go:   arr[1:4]
来源：http://udk.dashuyun.cn

Ruby: arr[1, 3]
来源：http://cgg.ppjwa.cn

C#:   list.GetRange(1, 3);
来源：http://fmf.hammf.cn

[D08] 合并两个数组
来源：http://udm.haohaochexian.top

Py:   a + b;  a.extend(b)
来源：http://plo.sufxvd.cn

PHP:  array_merge($a, $b);
来源：http://vfs.jinqigfzy.top

JS:   [...a, ...b];  a.concat(b);
来源：http://dol.jianghu66.top

TS:   [...a, ...b];
来源：http://dbp.aizwys.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ghp.gaohongyu789.top

Go:   append(a, b...)
来源：http://lko.hammf.cn


<!-- 参考信息 -->