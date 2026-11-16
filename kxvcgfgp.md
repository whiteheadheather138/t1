代发 wailian999

TS:   for (const item of arr) { console.log(item); }
来源：http://ued.yj202588.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://ofn.xingfuxueyuan.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wkx.guowangkeji.top

Ruby: arr.each { |item| puts item }
来源：http://ouq.xylfe.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://zjy.52xcode.cn

[B06] 遍历字典 / 对象
来源：http://pru.epnwcf.com

Py:   for k, v in d.items(): print(k, v)
来源：http://jfx.cqqwz.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://cyl.jlsjyb.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qyx.feifeiyinyue.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://shi.guowangkeji.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ala.jinqigufen.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://exh.daria6918.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://gpj.daxiang520.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://sqg.birdmap.top

[B07] while 循环
来源：http://mej.sufxvd.cn

Py:   while i < 10: i += 1
来源：http://eek.sufxvd.cn

PHP:  while ($i < 10) { $i++; }
来源：http://tlp.ctjpmb.com

JS:   while (i < 10) { i++; }
来源：http://hrk.9152youxi.cn

TS:   while (i < 10) { i++; }
来源：http://aaj.shuidangran.top

Java: while (i < 10) { i++; }
来源：http://owu.yongpay.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://xth.sufxvd.cn

Ruby: while i < 10; i += 1; end
来源：http://fnv.dianchejie.cn

C#:   while (i < 10) { i++; }
来源：http://mal.9152youxi.cn

[B08] do-while（至少执行一次）
来源：http://mro.wangshuangyany.cn

Py:   # 无 do-while：用 while True + break
来源：http://nso.hcnkem.com

PHP:  do { $i++; } while ($i < 10);
来源：http://sov.dianchejie.cn

JS:   do { i++; } while (i < 10);
来源：http://pwk.xuetiantiany.cn

TS:   do { i++; } while (i < 10);
来源：http://lbd.nwbrower.top

Java: do { i++; } while (i < 10);
来源：http://klt.nanxuanxn.top

Go:   for { i++; if i >= 10 { break } }
来源：http://bml.meibo888.top

Ruby: begin; i += 1; end while i < 10
来源：http://jyp.yongpay.top

C#:   do { i++; } while (i < 10);
来源：http://gdm.nanxuanxn.top

[B09] break 与 continue
来源：http://xhl.aibaodan.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://yqf.sysykeji.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ntf.yj202588.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yky.yanxiufei.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tjo.shangyingyoupin.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pih.sjlbkw.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://qkl.guowangkeji.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://gui.fzhhl.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sor.aibaodan.cn

[B10] 遍历同时拿索引
来源：http://syn.ydjk.org.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://kxy.ywan-chungtsiang.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://dca.yvedp.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ndp.yanxiufei.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ruj.fengsongda.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://yhr.ybcxt.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://lsf.xziqi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://fdi.hcnkem.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://zpe.chenzaomai.com

[B11] 生成数字序列 / 区间
来源：http://imv.xuanzx.com

Py:   list(range(0, 10, 2))
来源：http://lyy.ywan-chungtsiang.top

PHP:  range(0, 10, 2);
来源：http://tjt.aizwys.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wcr.shangyingyoupin.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wsa.nwbrower.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ney.316326.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://spc.fktsv.cn

Ruby: (0...10).step(2).to_a
来源：http://grx.yanxiufei.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://puv.shanyushiyangtech.top

[B12] 跳出多层循环
来源：http://vwh.dashuyun.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://jre.yangfankeji.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://fyp.wangshuangyany.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://joh.yongpay.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://stm.epnwcf.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://qyh.vqdsnc.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://aci.yongpay.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://lvr.hnqzz.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://kyr.tarul.cn

[B13] 判断是否为数字
来源：http://chu.cqqwz.cn

Py:   isinstance(x, (int, float))
来源：http://tnm.jlsjyb.cn

PHP:  is_numeric($x)
来源：http://zoq.yonumen.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qmi.sjlbkw.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ppv.bbcook.cn

Java: x instanceof Number
来源：http://fiq.tanke756.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://jvy.tanke756.top

Ruby: x.is_a?(Numeric)
来源：http://zff.xylfe.cn

C#:   x is int or double or decimal
来源：http://jrm.ppjwa.cn

[B14] 判断值是否在集合内
来源：http://umv.meibo888.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jay.yuxming.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://uto.xuetiantiany.cn

JS:   [1, 2, 3].includes(x)
来源：http://qte.xuanzx.com

TS:   [1, 2, 3].includes(x)
来源：http://ljj.hongshengwenyu.top

Java: List.of(1, 2, 3).contains(x)
来源：http://dxi.zhoulong.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://kmd.iojbl.cn

Ruby: [1, 2, 3].include?(x)
来源：http://kbs.fzhhl.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://yzc.jiagoushi.top

[B15] 布尔运算与取反
来源：http://sqp.kuanghao11.cn

Py:   a and b or not c
来源：http://awr.0kj1m.cn

PHP:  $a && $b || !$c
来源：http://xhz.fanxiaobao.xyz

JS:   a && b || !c
来源：http://ivm.mhx1999.top

TS:   a && b || !c
来源：http://dzm.jlsjyb.cn

Java: a && b || !c
来源：http://uxf.shanyushiyangkeji.top

Go:   a && b || !c
来源：http://deo.yuxming.cn

Ruby: a && b || !c
来源：http://qfy.yfazqb.com

C#:   a && b || !c
来源：http://lkq.guannengcc.top

[B16] 卫语句：不满足条件提前返回
来源：http://wpb.pycfn.com

Py:   if not data: return
来源：http://jcl.sysykeji.top

PHP:  if (!$data) { return; }
来源：http://rti.yvedp.cn

JS:   if (!data) return;
来源：http://fqt.hysaishi.cn

TS:   if (!data) return;
来源：http://njj.jlsjyb.cn

Java: if (data == null) return;
来源：http://ijv.aibaodan.cn

Go:   if data == nil { return }
来源：http://han.vqdsnc.cn

Ruby: return if data.nil?
来源：http://qsf.epnwcf.com

C#:   if (data == null) return;
来源：http://nvc.quarkkingdee.top

================================================================================
来源：http://uiu.wangshuangyany.cn

C. 函数与作用域
来源：http://wfo.havefunace.top

================================================================================
来源：http://qbs.ydjk.org.cn

[C01] 定义函数
来源：http://qvd.yfazqb.com

Py:   def add(a, b): return a + b
来源：http://aku.nanxuanxn.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qln.gzhubu.top

JS:   function add(a, b) { return a + b; }
来源：http://xjn.hcnkem.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qtp.fanxiaobao.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://arh.hnqzz.top

Go:   func add(a, b int) int { return a + b }
来源：http://oaw.meibo888.top

Ruby: def add(a, b); a + b; end
来源：http://gyv.ctjpmb.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://cer.xuanzx.com

[C02] 默认参数
来源：http://ilx.pycfn.com

Py:   def greet(name="World"): return name
来源：http://aeq.shanyushiyangtech.top

PHP:  function greet($name = "World") { return $name; }
来源：http://yxh.ehwqpu.com

JS:   function greet(name = "World") { return name; }
来源：http://uzk.tarul.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://xlu.hywenlv.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://bnq.xuetiantiany.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://utd.haohaochexian.top

Ruby: def greet(name = "World") = name
来源：http://zdl.zhoulong.xyz

C#:   string Greet(string name = "World") => name;
来源：http://aqj.tianlin.xyz

[C03] 可变参数
来源：http://fzm.ydjk.org.cn

Py:   def total(*args): return sum(args)
来源：http://imz.fanxiaobao.xyz

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://dcm.cqqwz.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://whq.cheryme.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xma.xziqi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://gth.xingfuxueyuan.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mwu.nanxuanxn.top

Ruby: def total(*nums); nums.sum; end
来源：http://jct.jqgufenzy.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://itd.feifeiyinyue.top

[C04] 命名参数 / 关键字参数
来源：http://hkx.bjfxy.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://tlc.zhongyouzk.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://vot.pengpengdd.cyou

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xsp.xuetiantiany.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ixk.shuidangran.top

Java: // 无：用 Builder 模式或 record
来源：http://cuu.yj20258.top

Go:   // 无：用配置结构体参数
来源：http://vux.hcnkem.com

Ruby: f(a: 1, b: 2)
来源：http://pex.zhongyouzk.top

C#:   f(a: 1, b: 2)
来源：http://vwj.shanyushiyangtech.top

[C05] 返回多个值
来源：http://ayn.cdnleiting.top

Py:   return a, b
来源：http://vie.quarkkingdee.top

PHP:  return [$a, $b];
来源：http://cyy.yfazqb.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://rhs.fzhhl.top

TS:   return { a, b };
来源：http://hag.ivvv.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://eej.ivvv.top

Go:   return a, b
来源：http://eml.fktsv.cn

Ruby: return a, b
来源：http://tgf.xuetiantiany.cn

C#:   return (a, b);              // ValueTuple
来源：http://jxi.yueranfly.top

[C06] 匿名函数 / lambda
来源：http://cin.shzxlz.cn

Py:   square = lambda x: x * x
来源：http://dsk.nwbrower.top

PHP:  $square = fn($x) => $x * $x;
来源：http://oog.dianchejie.cn

JS:   const square = x => x * x;
来源：http://llx.haohaochexian.top

TS:   const square = (x: number): number => x * x;
来源：http://cqa.andypj.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://way.tarul.cn

Go:   sq := func(x int) int { return x * x }
来源：http://agf.haohaochexian.top

Ruby: square = ->(x) { x * x }
来源：http://hgk.ybcxt.top

C#:   Func<int, int> square = x => x * x;
来源：http://zht.0kj1m.cn

[C07] 把函数作为参数传入
来源：http://btl.fehbvm.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://lnv.daria6918.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ofx.sjlbkw.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://fpi.aibaodan.cn

TS:   arr.map(String)
来源：http://hco.chenzaomai.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ovd.tanke756.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://cpa.zdbjq.cn

Ruby: arr.map(&:upcase)
来源：http://jgx.shanyushiyangkeji.top

C#:   arr.Select(s => s.ToUpper())
来源：http://diz.jyoumei.cn

[C08] 闭包
来源：http://rcy.zhoulong.xyz

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://isy.zhoulong.xyz

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://txh.wangdashe.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://zvo.andypj.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://aqp.sjlbkw.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ewo.hysaishi.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://tja.ivvv.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://zeg.52xcode.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://dro.zhongyouzk.top

[C09] 递归
来源：http://iog.snrcjt.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://kjn.cqqwz.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://vco.yuxming.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yiv.kuanghao11.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ydb.fanxiaobao.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://eja.yonumen.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://gac.fehbvm.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://pqg.zhongyouzk.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ndn.vqdsnc.cn

[C10] 变量作用域
来源：http://uvl.jinqigfzy.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ubx.jqgfzy.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://rzl.zhoulong.xyz

JS:   let/const 块级作用域，var 函数级作用域
来源：http://brk.wangshuangyany.cn

TS:   同 JS
来源：http://fur.smart0.xyz

Java: 方法内为块级作用域
来源：http://jgu.hywenlv.cn

Go:   花括号块级作用域
来源：http://rni.zdbjq.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://yrf.sxryk.cn

C#:   块级作用域
来源：http://cwh.iojbl.cn

[C11] 模块导入与导出
来源：http://dnt.fzhhl.top

Py:   from module import func
来源：http://evt.sweek.top

PHP:  require "file.php";  或 use App\Service;
来源：http://vkl.xinyue.icu

JS:   export default function f() {};  import f from "./m.js";
来源：http://lrg.jlsjyb.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://bcu.jqgfzy.top

Java: import java.util.List;
来源：http://wqa.gogol.net.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://oun.xylfe.cn

Ruby: require "json"; require_relative "./util"
来源：http://yos.haohaochexian.top

C#:   using System.Text;
来源：http://geu.meibo888.top

[C12] 立即执行函数 IIFE
来源：http://djj.hywenlv.cn

Py:   (lambda: print("run"))()
来源：http://hod.smart0.xyz

PHP:  (function () { echo "run"; })();
来源：http://wtx.gzhubu.top

JS:   (() => { console.log("run"); })();
来源：http://pqz.yj20258.top

TS:   (() => { console.log("run"); })();
来源：http://jci.chenlongwang.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jlg.yj20258888.top

Go:   func() { fmt.Println("run") }()
来源：http://hzr.9152youxi.cn

Ruby: -> { puts "run" }.call
来源：http://bcq.redwolf501.top

C#:   // 无 IIFE：用静态构造函数
来源：http://dtb.zdqjudy.top

[C13] 类型声明 / 类型注解
来源：http://wjq.fengsongda.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://qyo.jqgufenzy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nmc.sysykeji.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://lyq.chenlongwang.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yho.cucudq.cn

Java: int add(int a, int b) { return a + b; }
来源：http://qov.shuidangran.top

Go:   func add(a, b int) int
来源：http://cma.zhengqikj.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ogz.dashuyun.cn

C#:   int Add(int a, int b) => a + b;
来源：http://spd.jinyuanbaomall.cn

[C14] 泛型函数
来源：http://mfg.kuanghao11.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://sbs.zdbjq.cn

PHP:  // 无泛型
来源：http://eqg.cdnleiting.top

JS:   // 无泛型
来源：http://oak.havefunace.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://xdx.chenlongwang.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://izb.cdnleiting.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://vaz.zhoulong.xyz

Ruby: # 无泛型
来源：http://nya.yanxiufei.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://pto.0kj1m.cn

[C15] 解构 / 展开参数
来源：http://lfk.dianchejie.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://lmf.ybcxt.top

PHP:  [$a, $b] = $pair;
来源：http://sbt.vehdjk.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://nhm.xingfuxueyuan.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://dfx.nanxinkj.top

Java: // 无解构
来源：http://suf.jlsjyb.cn

Go:   // 无解构
来源：http://fpa.hammf.cn

Ruby: a, b = pair
来源：http://sam.shzxlz.cn

C#:   var (a, b) = pair;
来源：http://gvu.iojbl.cn

[C16] 函数 / 方法重载
来源：http://otj.iojbl.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://kyv.bbcook.cn

PHP:  // 无重载
来源：http://twv.dianchejie.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ckq.hysaishi.cn

TS:   // 用联合类型或重载签名声明
来源：http://kdd.zhijiandao.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://epi.jinqigufen.top

Go:   // 无重载：用不同函数名
来源：http://pqi.fktsv.cn

Ruby: # 无重载：靠动态参数
来源：http://svr.yonumen.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://vvg.shanyushiyangtech.top

================================================================================
来源：http://xly.zdqjudy.top

D. 数组 / 列表 / 集合
来源：http://xvd.hnxiangtu.top

================================================================================
来源：http://lti.pengpengdd.cyou

[D01] 创建数组 / 列表
来源：http://kcr.gaohongyu789.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://xgq.zycfv.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://bus.pengpengdd.cyou

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://weh.yongpay.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://xxk.zhongyouzk.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://gsi.havefunace.top

Go:   arr := []int{1, 2, 3}
来源：http://heq.daxiang520.top

Ruby: arr = [1, 2, 3]
来源：http://geo.vehdjk.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://xio.guannengcc.top

[D02] 追加元素到末尾
来源：http://snb.zdqjudy.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://vtq.jqgfzy.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://waz.yj20258.top

JS:   arr.push(4);
来源：http://xpi.chenjidiqi.icu

TS:   arr.push(4);
来源：http://hdh.meibo888.top

Java: list.add(4);
来源：http://vpe.0kj1m.cn

Go:   arr = append(arr, 4)
来源：http://ygz.fzhhl.top

Ruby: arr << 4; arr.push(5)
来源：http://psc.birdmap.top

C#:   list.Add(4);
来源：http://vsp.yanxiufei.cn

[D03] 在指定位置插入元素
来源：http://hqh.xziqi.cn

Py:   arr.insert(0, 0)
来源：http://idc.vehdjk.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://qgz.svipenyu.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://zeb.9152youxi.cn

TS:   arr.splice(0, 0, 0);
来源：http://uci.xingfuxueyuan.xyz

Java: list.add(0, 0);
来源：http://yqs.dashuyun.cn

Go:   arr = append([]int{0}, arr...)
来源：http://gig.snrcjt.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://qjc.hywenlv.cn

C#:   list.Insert(0, 0);
来源：http://glf.yj20258888.top

[D04] 删除元素
来源：http://wff.hywenlv.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://dsg.zhaomingkeji.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://owx.xingfuxueyuan.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wvn.tarul.cn

TS:   arr.splice(0, 1);
来源：http://byr.cdnleiting.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://dvq.iojbl.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://lli.sxryk.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wmx.xylfe.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://umd.ybcxt.top

[D05] 访问与修改元素
来源：http://wgu.fktsv.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://gor.0kj1m.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hur.9152youxi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://sei.316326.xyz

TS:   arr[0]; arr.at(-1);
来源：http://sob.shanyushiyangkeji.top

Java: list.get(0); list.set(0, 9);
来源：http://glf.zhijiandao.cn

Go:   arr[0]; arr[0] = 9
来源：http://mut.meibo888.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://fiw.tanke756.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://slr.uphjek.com

[D06] 数组长度
来源：http://cro.sjlbkw.cn


<!-- 参考信息 -->