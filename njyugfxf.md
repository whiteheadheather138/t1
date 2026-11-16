代发 wailian999

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zoi.zhijiandao.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ecb.jyoumei.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://gfz.hammf.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://bfy.guannengcc.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://daw.yuxming.cn

[B10] 遍历同时拿索引
来源：http://kju.yfazqb.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://bfg.gaohongyu789.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://vjk.sysykeji.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xua.hywenlv.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hgy.nwbrower.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://icu.snrcjt.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://gnw.shanyushiyangkeji.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://vyk.sweek.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://tpg.shzxlz.cn

[B11] 生成数字序列 / 区间
来源：http://jkf.haohaochexian.top

Py:   list(range(0, 10, 2))
来源：http://ldo.quarkkingdee.top

PHP:  range(0, 10, 2);
来源：http://phl.yuanzhike.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://iks.316326.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tdf.sxryk.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://dlo.zhijiandao.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hay.yuxming.cn

Ruby: (0...10).step(2).to_a
来源：http://ikl.shanyushiyangtech.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://jin.fzhhl.top

[B12] 跳出多层循环
来源：http://pfk.andypj.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://oav.0kj1m.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ezr.fktsv.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wgs.yuxming.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://rqm.zhaomingkeji.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://vnv.jiagoushi.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://pzf.zycfv.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mxl.jiagoushi.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://qur.ybcxt.top

[B13] 判断是否为数字
来源：http://xdq.yonumen.top

Py:   isinstance(x, (int, float))
来源：http://ecb.fehbvm.com

PHP:  is_numeric($x)
来源：http://hup.hywenlv.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pvs.daria6918.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xfn.jinqigufen.top

Java: x instanceof Number
来源：http://ivm.jianghu66.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://stl.cashguo.top

Ruby: x.is_a?(Numeric)
来源：http://tfn.fktsv.cn

C#:   x is int or double or decimal
来源：http://erx.cucudq.cn

[B14] 判断值是否在集合内
来源：http://okt.ctjpmb.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://pfh.haohaochexian.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://fhv.dianchejie.cn

JS:   [1, 2, 3].includes(x)
来源：http://hif.fanxiaobao.xyz

TS:   [1, 2, 3].includes(x)
来源：http://nkq.quarkkingdee.top

Java: List.of(1, 2, 3).contains(x)
来源：http://pad.tianlin.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wdi.bjfxy.top

Ruby: [1, 2, 3].include?(x)
来源：http://lbx.sysykeji.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://vjj.316326.xyz

[B15] 布尔运算与取反
来源：http://uil.redwolf501.top

Py:   a and b or not c
来源：http://zoo.c1oappe.top

PHP:  $a && $b || !$c
来源：http://fgf.jqgufenzy.top

JS:   a && b || !c
来源：http://url.jinqigfzy.top

TS:   a && b || !c
来源：http://gvm.zhiwuduotai.top

Java: a && b || !c
来源：http://plh.fengsongda.top

Go:   a && b || !c
来源：http://won.hammf.cn

Ruby: a && b || !c
来源：http://ody.nwbrower.top

C#:   a && b || !c
来源：http://tvb.ydzc1.top

[B16] 卫语句：不满足条件提前返回
来源：http://hkz.yangfankeji.com

Py:   if not data: return
来源：http://kez.cqqwz.cn

PHP:  if (!$data) { return; }
来源：http://cho.ydzc1.top

JS:   if (!data) return;
来源：http://nzc.vqdsnc.cn

TS:   if (!data) return;
来源：http://mis.yvedp.cn

Java: if (data == null) return;
来源：http://nju.tarul.cn

Go:   if data == nil { return }
来源：http://wts.bjfxy.top

Ruby: return if data.nil?
来源：http://rrn.yanxiufei.cn

C#:   if (data == null) return;
来源：http://ynz.ehwqpu.com

================================================================================
来源：http://ejt.iojbl.cn

C. 函数与作用域
来源：http://mta.epnwcf.com

================================================================================
来源：http://tyz.hnxiangtu.top

[C01] 定义函数
来源：http://kdu.yuxming.cn

Py:   def add(a, b): return a + b
来源：http://ogq.zhijiandao.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nhu.yj20258888.top

JS:   function add(a, b) { return a + b; }
来源：http://kji.andypj.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://owv.fzhhl.top

Java: static int add(int a, int b) { return a + b; }
来源：http://zfm.kuanghao11.cn

Go:   func add(a, b int) int { return a + b }
来源：http://zgv.zhengqikj.top

Ruby: def add(a, b); a + b; end
来源：http://uta.yongpay.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mlo.xziqi.cn

[C02] 默认参数
来源：http://ujf.gotoacloud.top

Py:   def greet(name="World"): return name
来源：http://hcx.yj20258.top

PHP:  function greet($name = "World") { return $name; }
来源：http://hxs.jinqigfzy.top

JS:   function greet(name = "World") { return name; }
来源：http://spn.hongshengwenyu.top

TS:   function greet(name: string = "World") { return name; }
来源：http://kqr.fktsv.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://fsu.xziqi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://myr.guowangkeji.top

Ruby: def greet(name = "World") = name
来源：http://bfd.fehbvm.com

C#:   string Greet(string name = "World") => name;
来源：http://apg.tarul.cn

[C03] 可变参数
来源：http://ddt.gaohongyu789.top

Py:   def total(*args): return sum(args)
来源：http://dwj.hcnkem.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wbu.hnqzz.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ykd.yangfankeji.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://tnr.52xcode.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://zfp.snrcjt.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://zhp.xuanzx.com

Ruby: def total(*nums); nums.sum; end
来源：http://fdt.guowangkeji.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://vpm.yangfankeji.com

[C04] 命名参数 / 关键字参数
来源：http://lbs.ivvv.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ppq.jqgfzy.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mdx.shzxlz.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://fwc.guannengcc.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://bpw.hfpthk.cn

Java: // 无：用 Builder 模式或 record
来源：http://xvv.aizwys.cn

Go:   // 无：用配置结构体参数
来源：http://nfx.gzhubu.top

Ruby: f(a: 1, b: 2)
来源：http://apc.aibaodan.cn

C#:   f(a: 1, b: 2)
来源：http://qsl.quarkkingdee.top

[C05] 返回多个值
来源：http://zmu.nanxuanxn.top

Py:   return a, b
来源：http://anr.zhongyouzk.top

PHP:  return [$a, $b];
来源：http://xbc.hesvh.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://buv.zdqjudy.top

TS:   return { a, b };
来源：http://xjf.hongshengwenyu.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://nto.yongpay.top

Go:   return a, b
来源：http://vyc.hammf.cn

Ruby: return a, b
来源：http://jqq.chenjidiqi.icu

C#:   return (a, b);              // ValueTuple
来源：http://nkd.xuetiantiany.cn

[C06] 匿名函数 / lambda
来源：http://pvt.shanyushiyangkeji.top

Py:   square = lambda x: x * x
来源：http://puw.gzhubu.top

PHP:  $square = fn($x) => $x * $x;
来源：http://nyb.yuxming.cn

JS:   const square = x => x * x;
来源：http://szc.ybcxt.top

TS:   const square = (x: number): number => x * x;
来源：http://amu.gzhubu.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://odu.cashguo.top

Go:   sq := func(x int) int { return x * x }
来源：http://deq.hysaishi.cn

Ruby: square = ->(x) { x * x }
来源：http://vgi.ydjk.org.cn

C#:   Func<int, int> square = x => x * x;
来源：http://gji.iojbl.cn

[C07] 把函数作为参数传入
来源：http://mnt.fanxiaobao.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://yfq.zdbjq.cn

PHP:  array_map("strtoupper", $arr);
来源：http://dfg.sweek.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://oar.hnqzz.top

TS:   arr.map(String)
来源：http://scg.guannengcc.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://jcl.pengpengdd.cyou

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://trb.jiagoushi.top

Ruby: arr.map(&:upcase)
来源：http://qjx.ydjk.org.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://pbt.zycfv.cn

[C08] 闭包
来源：http://ymg.nanxuanxn.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://omw.gaohongyu789.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://rzp.redwolf501.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://zbe.xylfe.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://cyk.jlsjyb.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://nvj.gzhubu.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://yod.feifeiyinyue.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://amt.hnxiangtu.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://gcq.pengpengdd.cyou

[C09] 递归
来源：http://hqh.yonumen.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://fwh.jqgfzy.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://czb.hnxiangtu.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cnj.gotoacloud.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://asi.hfpthk.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://dve.gaohongyu789.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ont.hysaishi.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wku.sysykeji.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wgv.nanxinkj.top

[C10] 变量作用域
来源：http://mzj.sjlbkw.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://etp.cdnleiting.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://zyk.sxryk.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ksl.52xcode.cn

TS:   同 JS
来源：http://vwe.fehbvm.com

Java: 方法内为块级作用域
来源：http://pvo.aizwys.cn

Go:   花括号块级作用域
来源：http://gpi.jiagoushi.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://yab.0kj1m.cn

C#:   块级作用域
来源：http://ddh.cqqwz.cn

[C11] 模块导入与导出
来源：http://zsc.hesvh.cn

Py:   from module import func
来源：http://vdv.fanxiaobao.xyz

PHP:  require "file.php";  或 use App\Service;
来源：http://rwt.iojbl.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://rap.jlsjyb.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mdh.fanxiaobao.xyz

Java: import java.util.List;
来源：http://ewu.yuanzhike.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://zho.chenjidiqi.icu

Ruby: require "json"; require_relative "./util"
来源：http://yro.aizwys.cn

C#:   using System.Text;
来源：http://kqa.jinqigufen.top

[C12] 立即执行函数 IIFE
来源：http://ssc.yj20258.top

Py:   (lambda: print("run"))()
来源：http://bfy.cqqwz.cn

PHP:  (function () { echo "run"; })();
来源：http://mmg.yj202588.top

JS:   (() => { console.log("run"); })();
来源：http://kvh.shzxlz.cn

TS:   (() => { console.log("run"); })();
来源：http://ykc.jlsjyb.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mir.havefunace.top

Go:   func() { fmt.Println("run") }()
来源：http://whh.sweek.top

Ruby: -> { puts "run" }.call
来源：http://xbg.hywenlv.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://laa.ehwqpu.com

[C13] 类型声明 / 类型注解
来源：http://yub.guowangkeji.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://vbc.fktsv.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ehh.iojbl.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://vyv.jqgfzy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wgu.kuanghao11.cn

Java: int add(int a, int b) { return a + b; }
来源：http://qxy.vqdsnc.cn

Go:   func add(a, b int) int
来源：http://acj.316326.xyz

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ler.yanxiufei.cn

C#:   int Add(int a, int b) => a + b;
来源：http://uvl.daxiang520.top

[C14] 泛型函数
来源：http://wdn.ydjk.org.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://snz.guannengcc.top

PHP:  // 无泛型
来源：http://utg.hcnkem.com

JS:   // 无泛型
来源：http://uce.fktsv.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wsf.yj202588.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://kuy.hcnkem.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://yyh.ivvv.top

Ruby: # 无泛型
来源：http://qju.tian-w.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://pwf.sufxvd.cn

[C15] 解构 / 展开参数
来源：http://oki.yuanzhike.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://jua.zdqjudy.top

PHP:  [$a, $b] = $pair;
来源：http://mvd.feifeiyinyue.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://yqu.shangyingyoupin.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mnw.bbcook.cn

Java: // 无解构
来源：http://rwc.mhx1999.top

Go:   // 无解构
来源：http://ulx.vehdjk.com

Ruby: a, b = pair
来源：http://kmt.mhx1999.top

C#:   var (a, b) = pair;
来源：http://lmx.yuanzhike.top

[C16] 函数 / 方法重载
来源：http://chd.tanke756.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://lwd.sufxvd.cn

PHP:  // 无重载
来源：http://dor.vehdjk.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://lvj.svipenyu.cn

TS:   // 用联合类型或重载签名声明
来源：http://pgh.daria6918.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://tzd.yonumen.top

Go:   // 无重载：用不同函数名
来源：http://kqo.iojbl.cn

Ruby: # 无重载：靠动态参数
来源：http://rnb.xziqi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://qph.pycfn.com

================================================================================
来源：http://tol.nanxinkj.top

D. 数组 / 列表 / 集合
来源：http://fnt.yongpay.top

================================================================================
来源：http://kvr.yueranfly.top

[D01] 创建数组 / 列表
来源：http://wjd.andypj.xyz

Py:   arr = [1, 2, 3];  empty = []
来源：http://cxh.jqgfzy.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://qhw.tianlin.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://gxq.nwbrower.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://uux.zhijiandao.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://xli.chenlongwang.top

Go:   arr := []int{1, 2, 3}
来源：http://ksq.yj202588.top

Ruby: arr = [1, 2, 3]
来源：http://hgn.ehwqpu.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wru.hammf.cn

[D02] 追加元素到末尾
来源：http://nim.yueranfly.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://cnj.gogol.net.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://uji.jinyuanbaomall.cn

JS:   arr.push(4);
来源：http://uot.meibo888.top

TS:   arr.push(4);
来源：http://gsz.yueranfly.top

Java: list.add(4);
来源：http://fvj.iojbl.cn

Go:   arr = append(arr, 4)
来源：http://ejo.c1oappe.top

Ruby: arr << 4; arr.push(5)
来源：http://vmm.smart0.xyz

C#:   list.Add(4);
来源：http://ing.zdbjq.cn

[D03] 在指定位置插入元素
来源：http://nun.zhoulong.xyz

Py:   arr.insert(0, 0)
来源：http://yor.52xcode.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://kya.andypj.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://jsg.fktsv.cn

TS:   arr.splice(0, 0, 0);
来源：http://jta.shuidangran.top

Java: list.add(0, 0);
来源：http://jls.ywan-chungtsiang.top

Go:   arr = append([]int{0}, arr...)
来源：http://hkz.shangyingyoupin.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://yuz.zycfv.cn

C#:   list.Insert(0, 0);
来源：http://uhe.vqdsnc.cn

[D04] 删除元素
来源：http://lbk.hfpthk.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://tzj.wangdashe.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ane.zdbjq.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://jcp.jinghuilouyu.cn

TS:   arr.splice(0, 1);
来源：http://jin.nanxuanxn.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://jom.yuxming.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ddt.yongpay.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://one.ctjpmb.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://yhb.hcnkem.com

[D05] 访问与修改元素
来源：http://dye.9152youxi.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://cvh.cqqwz.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://pch.xuetiantiany.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://yhc.jinghuilouyu.cn

TS:   arr[0]; arr.at(-1);
来源：http://ocw.fzhhl.top

Java: list.get(0); list.set(0, 9);
来源：http://ncz.snrcjt.cn

Go:   arr[0]; arr[0] = 9
来源：http://rao.cdnleiting.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://lys.zdbjq.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://upj.cucudq.cn

[D06] 数组长度
来源：http://tfj.gotoacloud.top

Py:   len(arr)
来源：http://zwb.yfazqb.com

PHP:  count($arr);
来源：http://sgb.snrcjt.cn

JS:   arr.length
来源：http://gov.redwolf501.top

TS:   arr.length
来源：http://boo.hysaishi.cn

Java: list.size();
来源：http://hjt.haohaochexian.top

Go:   len(arr)
来源：http://hbj.gotoacloud.top

Ruby: arr.length; arr.size
来源：http://ilw.316326.xyz

C#:   list.Count;
来源：http://dbq.xingfuxueyuan.xyz

[D07] 切片 / 取子数组
来源：http://ewb.cqqwz.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://apy.hcnkem.com

PHP:  array_slice($arr, 1, 3);
来源：http://pwa.chenlongwang.top

JS:   arr.slice(1, 4);
来源：http://fec.gzhubu.top

TS:   arr.slice(1, 4);
来源：http://chz.yueranfly.top

Java: list.subList(1, 4);
来源：http://bqo.cdnleiting.top

Go:   arr[1:4]
来源：http://sph.kuanghao11.cn

Ruby: arr[1, 3]
来源：http://pvn.yj20258888.top

C#:   list.GetRange(1, 3);
来源：http://svi.hysaishi.cn

[D08] 合并两个数组
来源：http://yzv.chenjidiqi.icu

Py:   a + b;  a.extend(b)
来源：http://srn.jinyuanbaomall.cn

PHP:  array_merge($a, $b);
来源：http://wwb.cqqwz.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ohd.zhengqikj.top

TS:   [...a, ...b];
来源：http://bqf.xuanzx.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mub.chenzaomai.com

Go:   append(a, b...)
来源：http://phd.nanxinkj.top

Ruby: a + b;  a.concat(b)
来源：http://dcp.yuxming.cn

C#:   a.Concat(b).ToList()
来源：http://orx.dashuyun.cn

[D09] 排序（升序）
来源：http://tpw.cqqwz.cn

Py:   sorted(arr);  arr.sort()
来源：http://tpz.hnxiangtu.top

PHP:  sort($arr);
来源：http://nbs.jqgufenzy.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://yrf.mhx1999.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://icg.nwbrower.top

Java: Collections.sort(list);  list.sort(null);
来源：http://wdr.smart0.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://whi.cheryme.top

Ruby: arr.sort
来源：http://ibs.feifeiyinyue.top

C#:   list.Sort();
来源：http://ihz.ehwqpu.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://vrf.ybcxt.top


<!-- 参考信息 -->