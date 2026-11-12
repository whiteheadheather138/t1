代发 wailian999

PHP:  while ($i < 10) { $i++; }
来源：http://esd.cqqwz.cn

JS:   while (i < 10) { i++; }
来源：http://ras.cdnleiting.top

TS:   while (i < 10) { i++; }
来源：http://ivy.gotoacloud.top

Java: while (i < 10) { i++; }
来源：http://ehb.zycfv.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://cge.xinyue.icu

Ruby: while i < 10; i += 1; end
来源：http://mad.jinghuilouyu.cn

C#:   while (i < 10) { i++; }
来源：http://ncb.yueranfly.top

[B08] do-while（至少执行一次）
来源：http://oql.guowangkeji.top

Py:   # 无 do-while：用 while True + break
来源：http://chu.ctjpmb.com

PHP:  do { $i++; } while ($i < 10);
来源：http://mqj.fengsongda.top

JS:   do { i++; } while (i < 10);
来源：http://iux.nanxuanxn.top

TS:   do { i++; } while (i < 10);
来源：http://pae.hammf.cn

Java: do { i++; } while (i < 10);
来源：http://lwt.zhoulong.xyz

Go:   for { i++; if i >= 10 { break } }
来源：http://fzs.jqgfzy.top

Ruby: begin; i += 1; end while i < 10
来源：http://wav.cqqwz.cn

C#:   do { i++; } while (i < 10);
来源：http://qtj.hysaishi.cn

[B09] break 与 continue
来源：http://znr.jqgufenzy.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hkt.zycfv.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ixl.0kj1m.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fcq.fzhhl.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pgr.nwbrower.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ewp.gzhubu.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://htt.aibaodan.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://gbl.yanxiufei.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ndz.xziqi.cn

[B10] 遍历同时拿索引
来源：http://nky.birdmap.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://udi.gotoacloud.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://xjg.pycfn.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://fpv.sweek.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://phd.gotoacloud.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://dcf.epnwcf.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://xnf.andypj.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hca.zdqjudy.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://qte.yueranfly.top

[B11] 生成数字序列 / 区间
来源：http://qha.hnxiangtu.top

Py:   list(range(0, 10, 2))
来源：http://wjy.52xcode.cn

PHP:  range(0, 10, 2);
来源：http://cet.pycfn.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ivn.hnqzz.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zrb.yj202588.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://oba.sweek.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ywi.jinghuilouyu.cn

Ruby: (0...10).step(2).to_a
来源：http://utb.chenlongwang.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://fzx.yj202588.top

[B12] 跳出多层循环
来源：http://sih.shzxlz.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://idz.zhengqikj.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://oxf.wangshuangyany.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://pmn.cheryme.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://nxt.vehdjk.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://cuw.redwolf501.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://rfm.yangfankeji.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://lyu.uphjek.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://xsa.cqqwz.cn

[B13] 判断是否为数字
来源：http://oyk.fengsongda.top

Py:   isinstance(x, (int, float))
来源：http://raj.yonumen.top

PHP:  is_numeric($x)
来源：http://rdm.zhiwuduotai.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gyp.tarul.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dru.havefunace.top

Java: x instanceof Number
来源：http://eal.cucudq.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://azp.hnxiangtu.top

Ruby: x.is_a?(Numeric)
来源：http://har.fzhhl.top

C#:   x is int or double or decimal
来源：http://spj.yj202588.top

[B14] 判断值是否在集合内
来源：http://svu.yueranfly.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://miq.gzhubu.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ysu.yanxiufei.cn

JS:   [1, 2, 3].includes(x)
来源：http://oqj.fktsv.cn

TS:   [1, 2, 3].includes(x)
来源：http://lch.nanxuanxn.top

Java: List.of(1, 2, 3).contains(x)
来源：http://trz.gotoacloud.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://pen.dianchejie.cn

Ruby: [1, 2, 3].include?(x)
来源：http://tpr.gotoacloud.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ifl.sxryk.cn

[B15] 布尔运算与取反
来源：http://mqj.shzxlz.cn

Py:   a and b or not c
来源：http://syu.ctjpmb.com

PHP:  $a && $b || !$c
来源：http://mym.0kj1m.cn

JS:   a && b || !c
来源：http://bqv.zhijiandao.cn

TS:   a && b || !c
来源：http://fqd.hcnkem.com

Java: a && b || !c
来源：http://soo.iojbl.cn

Go:   a && b || !c
来源：http://mol.aibaodan.cn

Ruby: a && b || !c
来源：http://xzk.aibaodan.cn

C#:   a && b || !c
来源：http://qnx.tarul.cn

[B16] 卫语句：不满足条件提前返回
来源：http://enp.hesvh.cn

Py:   if not data: return
来源：http://uxw.hfpthk.cn

PHP:  if (!$data) { return; }
来源：http://kvp.9152youxi.cn

JS:   if (!data) return;
来源：http://qcq.meibo888.top

TS:   if (!data) return;
来源：http://mxn.jinqigfzy.top

Java: if (data == null) return;
来源：http://gva.snrcjt.cn

Go:   if data == nil { return }
来源：http://cvh.cdnleiting.top

Ruby: return if data.nil?
来源：http://fxa.yuxming.cn

C#:   if (data == null) return;
来源：http://jfl.zycfv.cn

================================================================================
来源：http://jnz.xylfe.cn

C. 函数与作用域
来源：http://wpd.yvedp.cn

================================================================================
来源：http://qzb.chenzaomai.com

[C01] 定义函数
来源：http://ljw.xylfe.cn

Py:   def add(a, b): return a + b
来源：http://iyc.c1oappe.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rxn.nwbrower.top

JS:   function add(a, b) { return a + b; }
来源：http://bio.tianlin.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wfn.smart0.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://drh.yongpay.top

Go:   func add(a, b int) int { return a + b }
来源：http://nqx.zdbjq.cn

Ruby: def add(a, b); a + b; end
来源：http://tck.jinqigufen.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://xme.tanke756.top

[C02] 默认参数
来源：http://utw.zhiwuduotai.top

Py:   def greet(name="World"): return name
来源：http://cia.aibaodan.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://grd.quarkkingdee.top

JS:   function greet(name = "World") { return name; }
来源：http://jpk.zhoulong.xyz

TS:   function greet(name: string = "World") { return name; }
来源：http://djn.uphjek.com

Java: // 无默认参数：方法重载或 Optional
来源：http://fqi.tian-w.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://vhh.tianlin.xyz

Ruby: def greet(name = "World") = name
来源：http://esg.c1oappe.top

C#:   string Greet(string name = "World") => name;
来源：http://kvf.shzxlz.cn

[C03] 可变参数
来源：http://vvw.9152youxi.cn

Py:   def total(*args): return sum(args)
来源：http://gju.daxiang520.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xrt.xuetiantiany.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://gfo.jinyuanbaomall.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://gzm.pycfn.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://udc.jqgfzy.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://bwe.jqgufenzy.top

Ruby: def total(*nums); nums.sum; end
来源：http://fvi.dianchejie.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://uvz.fzhhl.top

[C04] 命名参数 / 关键字参数
来源：http://gfq.iojbl.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://its.hnxiangtu.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://fxc.iojbl.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://och.aizwys.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://qjb.quarkkingdee.top

Java: // 无：用 Builder 模式或 record
来源：http://wqm.wangdashe.top

Go:   // 无：用配置结构体参数
来源：http://nku.sjlbkw.cn

Ruby: f(a: 1, b: 2)
来源：http://bvu.ivvv.top

C#:   f(a: 1, b: 2)
来源：http://wku.c1oappe.top

[C05] 返回多个值
来源：http://xnk.shzxlz.cn

Py:   return a, b
来源：http://obv.sweek.top

PHP:  return [$a, $b];
来源：http://apw.yueranfly.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://zny.52xcode.cn

TS:   return { a, b };
来源：http://urm.yj202588.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ekg.sweek.top

Go:   return a, b
来源：http://glg.jlsjyb.cn

Ruby: return a, b
来源：http://kxt.yongpay.top

C#:   return (a, b);              // ValueTuple
来源：http://nio.cucudq.cn

[C06] 匿名函数 / lambda
来源：http://oal.fengsongda.top

Py:   square = lambda x: x * x
来源：http://pcp.xuetiantiany.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://pvb.meibo888.top

JS:   const square = x => x * x;
来源：http://aqq.xziqi.cn

TS:   const square = (x: number): number => x * x;
来源：http://zyi.jinqigufen.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://qaa.mhx1999.top

Go:   sq := func(x int) int { return x * x }
来源：http://csb.guowangkeji.top

Ruby: square = ->(x) { x * x }
来源：http://zhx.aizwys.cn

C#:   Func<int, int> square = x => x * x;
来源：http://qes.tarul.cn

[C07] 把函数作为参数传入
来源：http://zjo.nanxuanxn.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://neg.meibo888.top

PHP:  array_map("strtoupper", $arr);
来源：http://cdc.zhengqikj.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://six.xziqi.cn

TS:   arr.map(String)
来源：http://tvd.hysaishi.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://fgy.jlsjyb.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://jzv.fengsongda.top

Ruby: arr.map(&:upcase)
来源：http://zmp.meibo888.top

C#:   arr.Select(s => s.ToUpper())
来源：http://qvx.daria6918.cn

[C08] 闭包
来源：http://kct.ctjpmb.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://jes.fzhhl.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ghp.hcnkem.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://kgn.kuanghao11.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://dux.ivvv.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://sbj.guannengcc.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://rak.52xcode.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://zqn.sysykeji.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://dar.cashguo.top

[C09] 递归
来源：http://doe.feifeiyinyue.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://thk.yfazqb.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://sxo.haohaochexian.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yxi.xylfe.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sbr.nanxinkj.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://vtx.mhx1999.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wdr.yonumen.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://owq.ehwqpu.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://khe.jinyuanbaomall.cn

[C10] 变量作用域
来源：http://qly.chenlongwang.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wkl.yj20258888.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://bps.mhx1999.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://rai.daria6918.cn

TS:   同 JS
来源：http://eys.chenlongwang.top

Java: 方法内为块级作用域
来源：http://zfr.xinyue.icu

Go:   花括号块级作用域
来源：http://pxx.nwbrower.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://rfl.aizwys.cn

C#:   块级作用域
来源：http://tza.ppjwa.cn

[C11] 模块导入与导出
来源：http://uoa.jlsjyb.cn

Py:   from module import func
来源：http://ltn.ppjwa.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://osb.jiagoushi.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://wtg.hnxiangtu.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://tmh.aibaodan.cn

Java: import java.util.List;
来源：http://oyz.yj20258888.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://jfp.sjlbkw.cn

Ruby: require "json"; require_relative "./util"
来源：http://gja.feifeiyinyue.top

C#:   using System.Text;
来源：http://nwv.wangshuangyany.cn

[C12] 立即执行函数 IIFE
来源：http://tow.andypj.xyz

Py:   (lambda: print("run"))()
来源：http://uov.mhx1999.top

PHP:  (function () { echo "run"; })();
来源：http://phr.jlsjyb.cn

JS:   (() => { console.log("run"); })();
来源：http://anv.zhiwuduotai.top

TS:   (() => { console.log("run"); })();
来源：http://wzz.hesvh.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wxo.tianlin.xyz

Go:   func() { fmt.Println("run") }()
来源：http://rpk.ybcxt.top

Ruby: -> { puts "run" }.call
来源：http://zhp.zhijiandao.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://fmu.nanxuanxn.top

[C13] 类型声明 / 类型注解
来源：http://wzq.zhengqikj.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://rtl.xinyue.icu

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ucq.shzxlz.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://xcj.yj20258.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gmb.feifeiyinyue.top

Java: int add(int a, int b) { return a + b; }
来源：http://zie.havefunace.top

Go:   func add(a, b int) int
来源：http://uly.cheryme.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://svi.shanyushiyangtech.top

C#:   int Add(int a, int b) => a + b;
来源：http://cwv.jinghuilouyu.cn

[C14] 泛型函数
来源：http://wnc.zhixingplan.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://spn.ydzc1.top

PHP:  // 无泛型
来源：http://oei.cqqwz.cn

JS:   // 无泛型
来源：http://tfp.smart0.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://lyt.guowangkeji.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://olx.jlsjyb.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://rao.snrcjt.cn

Ruby: # 无泛型
来源：http://hln.shuidangran.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ekl.epnwcf.com

[C15] 解构 / 展开参数
来源：http://maq.jyoumei.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://gki.yj20258.top

PHP:  [$a, $b] = $pair;
来源：http://uhb.dianchejie.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://liz.hongshengwenyu.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://vug.daria6918.cn

Java: // 无解构
来源：http://jwt.daria6918.cn

Go:   // 无解构
来源：http://hoi.jqgfzy.top

Ruby: a, b = pair
来源：http://pgk.andypj.xyz

C#:   var (a, b) = pair;
来源：http://dua.wangshuangyany.cn

[C16] 函数 / 方法重载
来源：http://njo.hfpthk.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://nln.gaohongyu789.top

PHP:  // 无重载
来源：http://wjp.hfpthk.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://org.aizwys.cn

TS:   // 用联合类型或重载签名声明
来源：http://ayz.wangdashe.top

Java: void f(int a) {}  void f(String a) {}
来源：http://tpk.smart0.xyz

Go:   // 无重载：用不同函数名
来源：http://sih.jlsjyb.cn

Ruby: # 无重载：靠动态参数
来源：http://ucp.tianlin.xyz

C#:   void F(int a) {}  void F(string a) {}
来源：http://lro.jlsjyb.cn

================================================================================
来源：http://wsg.yvedp.cn

D. 数组 / 列表 / 集合
来源：http://acd.daria6918.cn

================================================================================
来源：http://bmf.aibaodan.cn

[D01] 创建数组 / 列表
来源：http://dim.ctjpmb.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://ddk.ybcxt.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://rwq.vqdsnc.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mxr.jinyuanbaomall.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://len.cheryme.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://qcm.daria6918.cn

Go:   arr := []int{1, 2, 3}
来源：http://dai.c1oappe.top

Ruby: arr = [1, 2, 3]
来源：http://suj.hywenlv.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://bof.haohaochexian.top

[D02] 追加元素到末尾
来源：http://aub.yanxiufei.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mmd.hongshengwenyu.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://nzk.jianghu66.top

JS:   arr.push(4);
来源：http://hzv.jinghuilouyu.cn

TS:   arr.push(4);
来源：http://tht.shuidangran.top

Java: list.add(4);
来源：http://obm.hywenlv.cn

Go:   arr = append(arr, 4)
来源：http://yty.bjfxy.top

Ruby: arr << 4; arr.push(5)
来源：http://cch.havefunace.top

C#:   list.Add(4);
来源：http://ygj.quarkkingdee.top

[D03] 在指定位置插入元素
来源：http://usz.redwolf501.top

Py:   arr.insert(0, 0)
来源：http://him.shanyushiyangtech.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://cri.fzhhl.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://cwe.hysaishi.cn

TS:   arr.splice(0, 0, 0);
来源：http://sfq.hysaishi.cn

Java: list.add(0, 0);
来源：http://qqc.yongpay.top

Go:   arr = append([]int{0}, arr...)
来源：http://psy.hywenlv.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ums.zhijiandao.cn

C#:   list.Insert(0, 0);
来源：http://psu.tianlin.xyz

[D04] 删除元素
来源：http://maj.wangshuangyany.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://lmx.zycfv.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://usp.guannengcc.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://avi.nanxinkj.top

TS:   arr.splice(0, 1);
来源：http://zaz.fzhhl.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://vky.jinghuilouyu.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ypb.smart0.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ceh.andypj.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://fim.smart0.xyz

[D05] 访问与修改元素
来源：http://tnk.xinyue.icu

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://yde.zycfv.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wxv.hysaishi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://phb.yuxming.cn

TS:   arr[0]; arr.at(-1);
来源：http://eip.xylfe.cn

Java: list.get(0); list.set(0, 9);
来源：http://ffz.jianghu66.top

Go:   arr[0]; arr[0] = 9
来源：http://zdw.meibo888.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://uwv.yonumen.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://rpe.guannengcc.top

[D06] 数组长度
来源：http://xrm.xinyue.icu

Py:   len(arr)
来源：http://ehl.shangyingyoupin.top

PHP:  count($arr);
来源：http://phe.sweek.top

JS:   arr.length
来源：http://imu.yj202588.top

TS:   arr.length
来源：http://qla.fktsv.cn

Java: list.size();
来源：http://tec.dianchejie.cn

Go:   len(arr)
来源：http://fuf.epnwcf.com

Ruby: arr.length; arr.size
来源：http://nhq.hywenlv.cn

C#:   list.Count;
来源：http://akv.sxryk.cn

[D07] 切片 / 取子数组
来源：http://oxu.hywenlv.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://piw.ydzc1.top

PHP:  array_slice($arr, 1, 3);
来源：http://ykx.tian-w.cn

JS:   arr.slice(1, 4);
来源：http://klv.ivvv.top

TS:   arr.slice(1, 4);
来源：http://jad.zhixingplan.top

Java: list.subList(1, 4);
来源：http://exl.cdnleiting.top

Go:   arr[1:4]
来源：http://bmv.yvedp.cn

Ruby: arr[1, 3]
来源：http://rbg.zhiwuduotai.top


<!-- 参考信息 -->