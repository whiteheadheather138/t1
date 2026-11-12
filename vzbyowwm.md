代发 wailian999

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lps.wangdashe.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ikv.sjlbkw.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://rdu.hnqzz.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://jqk.jinyuanbaomall.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://kmy.guowangkeji.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mor.tarul.cn

[B07] while 循环
来源：http://ail.xinyue.icu

Py:   while i < 10: i += 1
来源：http://dws.jyoumei.cn

PHP:  while ($i < 10) { $i++; }
来源：http://gaf.shanyushiyangtech.top

JS:   while (i < 10) { i++; }
来源：http://xjt.shanyushiyangtech.top

TS:   while (i < 10) { i++; }
来源：http://wba.zhijiandao.cn

Java: while (i < 10) { i++; }
来源：http://til.hnqzz.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://brq.vehdjk.com

Ruby: while i < 10; i += 1; end
来源：http://ibf.yj202588.top

C#:   while (i < 10) { i++; }
来源：http://pnh.hnxiangtu.top

[B08] do-while（至少执行一次）
来源：http://ngo.aizwys.cn

Py:   # 无 do-while：用 while True + break
来源：http://swl.zhongyouzk.top

PHP:  do { $i++; } while ($i < 10);
来源：http://kjr.hfpthk.cn

JS:   do { i++; } while (i < 10);
来源：http://hfj.gotoacloud.top

TS:   do { i++; } while (i < 10);
来源：http://njr.haohaochexian.top

Java: do { i++; } while (i < 10);
来源：http://wqr.xingfuxueyuan.xyz

Go:   for { i++; if i >= 10 { break } }
来源：http://adm.sjlbkw.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ybi.sufxvd.cn

C#:   do { i++; } while (i < 10);
来源：http://enc.shanyushiyangtech.top

[B09] break 与 continue
来源：http://wwu.uphjek.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ojw.guannengcc.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://yba.ydjk.org.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://stu.zhixingplan.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ujr.jinghuilouyu.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cat.yueranfly.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://dne.0kj1m.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hbt.hesvh.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gwy.gaohongyu789.top

[B10] 遍历同时拿索引
来源：http://bjs.zhijiandao.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://sbj.hywenlv.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://tga.bbcook.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://meb.ybcxt.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://pzv.shzxlz.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ply.ctjpmb.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mko.ydjk.org.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://rac.xziqi.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://vwz.yueranfly.top

[B11] 生成数字序列 / 区间
来源：http://xaw.chenzaomai.com

Py:   list(range(0, 10, 2))
来源：http://lkh.cucudq.cn

PHP:  range(0, 10, 2);
来源：http://syo.nwbrower.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://caf.xziqi.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ysw.guannengcc.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://eui.xinyue.icu

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ado.ydzc1.top

Ruby: (0...10).step(2).to_a
来源：http://ocx.0kj1m.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zgc.c1oappe.top

[B12] 跳出多层循环
来源：http://nbh.jinghuilouyu.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ruz.daria6918.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ind.chenjidiqi.icu

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://uoa.fengsongda.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://eno.gzhubu.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ekr.hysaishi.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://vot.ybcxt.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mwq.cheryme.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://bgk.jinqigfzy.top

[B13] 判断是否为数字
来源：http://otf.yongpay.top

Py:   isinstance(x, (int, float))
来源：http://vrd.cashguo.top

PHP:  is_numeric($x)
来源：http://ahj.hesvh.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lrb.hnxiangtu.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ynf.zycfv.cn

Java: x instanceof Number
来源：http://ond.xuanzx.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://rhe.jinghuilouyu.cn

Ruby: x.is_a?(Numeric)
来源：http://whf.jianghu66.top

C#:   x is int or double or decimal
来源：http://bcf.hnxiangtu.top

[B14] 判断值是否在集合内
来源：http://vvj.jqgfzy.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://qwu.mhx1999.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ihi.zycfv.cn

JS:   [1, 2, 3].includes(x)
来源：http://cox.yangfankeji.com

TS:   [1, 2, 3].includes(x)
来源：http://aum.kuanghao11.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://vkw.mhx1999.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://qsy.hesvh.cn

Ruby: [1, 2, 3].include?(x)
来源：http://mzu.aibaodan.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://nqv.cashguo.top

[B15] 布尔运算与取反
来源：http://uva.zdbjq.cn

Py:   a and b or not c
来源：http://rpl.shzxlz.cn

PHP:  $a && $b || !$c
来源：http://wgu.snrcjt.cn

JS:   a && b || !c
来源：http://lij.shuidangran.top

TS:   a && b || !c
来源：http://qao.52xcode.cn

Java: a && b || !c
来源：http://fua.tian-w.cn

Go:   a && b || !c
来源：http://oeg.zycfv.cn

Ruby: a && b || !c
来源：http://adq.hfpthk.cn

C#:   a && b || !c
来源：http://bah.ctjpmb.com

[B16] 卫语句：不满足条件提前返回
来源：http://tme.gaohongyu789.top

Py:   if not data: return
来源：http://qyi.pengpengdd.cyou

PHP:  if (!$data) { return; }
来源：http://xbx.bjfxy.top

JS:   if (!data) return;
来源：http://xld.quarkkingdee.top

TS:   if (!data) return;
来源：http://fax.yj20258888.top

Java: if (data == null) return;
来源：http://feh.vehdjk.com

Go:   if data == nil { return }
来源：http://svp.bjfxy.top

Ruby: return if data.nil?
来源：http://vzi.sjlbkw.cn

C#:   if (data == null) return;
来源：http://eym.shangyingyoupin.top

================================================================================
来源：http://sbo.xingfuxueyuan.xyz

C. 函数与作用域
来源：http://wve.sweek.top

================================================================================
来源：http://bkt.ywan-chungtsiang.top

[C01] 定义函数
来源：http://wyi.meibo888.top

Py:   def add(a, b): return a + b
来源：http://jbo.gotoacloud.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gis.jyoumei.cn

JS:   function add(a, b) { return a + b; }
来源：http://srg.shzxlz.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dwd.ywan-chungtsiang.top

Java: static int add(int a, int b) { return a + b; }
来源：http://zlq.jianghu66.top

Go:   func add(a, b int) int { return a + b }
来源：http://fpy.mhx1999.top

Ruby: def add(a, b); a + b; end
来源：http://jqp.yj20258.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://pfq.uphjek.com

[C02] 默认参数
来源：http://edd.zdqjudy.top

Py:   def greet(name="World"): return name
来源：http://chv.nanxinkj.top

PHP:  function greet($name = "World") { return $name; }
来源：http://daz.pengpengdd.cyou

JS:   function greet(name = "World") { return name; }
来源：http://dke.jlsjyb.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://now.jinyuanbaomall.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://lyx.havefunace.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://spf.tarul.cn

Ruby: def greet(name = "World") = name
来源：http://jxr.cashguo.top

C#:   string Greet(string name = "World") => name;
来源：http://qim.cheryme.top

[C03] 可变参数
来源：http://lkx.hongshengwenyu.top

Py:   def total(*args): return sum(args)
来源：http://xgm.yfazqb.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://rvp.ydzc1.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://osr.dianchejie.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://swo.yj202588.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://lfz.vehdjk.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://dhq.gogol.net.cn

Ruby: def total(*nums); nums.sum; end
来源：http://pkw.gotoacloud.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wwe.bbcook.cn

[C04] 命名参数 / 关键字参数
来源：http://qkw.tarul.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://kej.xuanzx.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://rqg.bbcook.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://dkl.andypj.xyz

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://tsf.jyoumei.cn

Java: // 无：用 Builder 模式或 record
来源：http://qli.jinghuilouyu.cn

Go:   // 无：用配置结构体参数
来源：http://yfz.ydjk.org.cn

Ruby: f(a: 1, b: 2)
来源：http://asm.bjfxy.top

C#:   f(a: 1, b: 2)
来源：http://mvb.sjlbkw.cn

[C05] 返回多个值
来源：http://zvl.tianlin.xyz

Py:   return a, b
来源：http://qyf.ehwqpu.com

PHP:  return [$a, $b];
来源：http://xtl.birdmap.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://nma.cucudq.cn

TS:   return { a, b };
来源：http://jbt.aibaodan.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xnf.wangdashe.top

Go:   return a, b
来源：http://jge.zdbjq.cn

Ruby: return a, b
来源：http://xal.xuetiantiany.cn

C#:   return (a, b);              // ValueTuple
来源：http://lpx.fehbvm.com

[C06] 匿名函数 / lambda
来源：http://hmf.meibo888.top

Py:   square = lambda x: x * x
来源：http://lyr.sjlbkw.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://enq.xinyue.icu

JS:   const square = x => x * x;
来源：http://owf.havefunace.top

TS:   const square = (x: number): number => x * x;
来源：http://qwq.tian-w.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://erd.ppjwa.cn

Go:   sq := func(x int) int { return x * x }
来源：http://olz.guowangkeji.top

Ruby: square = ->(x) { x * x }
来源：http://kmj.yanxiufei.cn

C#:   Func<int, int> square = x => x * x;
来源：http://hhi.zycfv.cn

[C07] 把函数作为参数传入
来源：http://jly.jqgufenzy.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://dew.aibaodan.cn

PHP:  array_map("strtoupper", $arr);
来源：http://rrq.yuanzhike.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://fxz.dianchejie.cn

TS:   arr.map(String)
来源：http://inn.yfazqb.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://nha.cheryme.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://inw.ppjwa.cn

Ruby: arr.map(&:upcase)
来源：http://ezu.zycfv.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://pvm.zhengqikj.top

[C08] 闭包
来源：http://swx.aizwys.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://drq.52xcode.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mvw.redwolf501.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://yvi.fzhhl.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ltz.jlsjyb.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://kaa.xziqi.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://nqp.chenzaomai.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wzy.zhiwuduotai.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://jnu.jinqigfzy.top

[C09] 递归
来源：http://qpi.andypj.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://xsk.0kj1m.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://xcp.yongpay.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qum.sweek.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qmw.fengsongda.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://orl.fzhhl.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://gco.mhx1999.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hiy.yj20258.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://jtv.hnqzz.top

[C10] 变量作用域
来源：http://oqe.svipenyu.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mhf.hysaishi.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://qap.yfazqb.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wbm.havefunace.top

TS:   同 JS
来源：http://hrq.hnxiangtu.top

Java: 方法内为块级作用域
来源：http://rmj.shanyushiyangtech.top

Go:   花括号块级作用域
来源：http://vvm.cheryme.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://dbs.yj20258888.top

C#:   块级作用域
来源：http://ojq.quarkkingdee.top

[C11] 模块导入与导出
来源：http://skk.jiagoushi.top

Py:   from module import func
来源：http://nxe.gzhubu.top

PHP:  require "file.php";  或 use App\Service;
来源：http://axk.jinghuilouyu.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://gnk.chenzaomai.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xzg.hammf.cn

Java: import java.util.List;
来源：http://hyd.yanxiufei.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://fuy.0kj1m.cn

Ruby: require "json"; require_relative "./util"
来源：http://knx.jiagoushi.top

C#:   using System.Text;
来源：http://qrj.yonumen.top

[C12] 立即执行函数 IIFE
来源：http://ojr.wangdashe.top

Py:   (lambda: print("run"))()
来源：http://kml.pycfn.com

PHP:  (function () { echo "run"; })();
来源：http://tdl.yj202588.top

JS:   (() => { console.log("run"); })();
来源：http://yal.yuanzhike.top

TS:   (() => { console.log("run"); })();
来源：http://fxq.ydzc1.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hln.nwbrower.top

Go:   func() { fmt.Println("run") }()
来源：http://rvp.xziqi.cn

Ruby: -> { puts "run" }.call
来源：http://hrq.svipenyu.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://bhi.sysykeji.top

[C13] 类型声明 / 类型注解
来源：http://fxj.fengsongda.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://kyv.jinqigufen.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://foz.sufxvd.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://cow.zhoulong.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jvg.nanxinkj.top

Java: int add(int a, int b) { return a + b; }
来源：http://prg.jqgufenzy.top

Go:   func add(a, b int) int
来源：http://onl.yfazqb.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ysf.fanxiaobao.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://hza.jiagoushi.top

[C14] 泛型函数
来源：http://shj.zhoulong.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://drc.hammf.cn

PHP:  // 无泛型
来源：http://fgh.gaohongyu789.top

JS:   // 无泛型
来源：http://unm.guowangkeji.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://sow.ywan-chungtsiang.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://jty.wangdashe.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://cuu.zhixingplan.top

Ruby: # 无泛型
来源：http://vkm.zhixingplan.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://lsv.cdnleiting.top

[C15] 解构 / 展开参数
来源：http://cvr.yueranfly.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wmz.mhx1999.top

PHP:  [$a, $b] = $pair;
来源：http://buy.hysaishi.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://azt.bjfxy.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://jwo.gaohongyu789.top

Java: // 无解构
来源：http://fgs.sweek.top

Go:   // 无解构
来源：http://drl.jiagoushi.top

Ruby: a, b = pair
来源：http://muu.bbcook.cn

C#:   var (a, b) = pair;
来源：http://gwp.jqgufenzy.top

[C16] 函数 / 方法重载
来源：http://yrd.yvedp.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://prl.fktsv.cn

PHP:  // 无重载
来源：http://jzf.ivvv.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://ecx.yvedp.cn

TS:   // 用联合类型或重载签名声明
来源：http://zbq.xinyue.icu

Java: void f(int a) {}  void f(String a) {}
来源：http://pke.ivvv.top

Go:   // 无重载：用不同函数名
来源：http://ehh.jinghuilouyu.cn

Ruby: # 无重载：靠动态参数
来源：http://yyd.nanxuanxn.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://qjf.jyoumei.cn

================================================================================
来源：http://tbq.tarul.cn

D. 数组 / 列表 / 集合
来源：http://wom.hfpthk.cn

================================================================================
来源：http://opv.ppjwa.cn

[D01] 创建数组 / 列表
来源：http://esx.ctjpmb.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://yyk.9152youxi.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://nqd.daria6918.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://vmf.tarul.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://puj.zhongyouzk.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://niy.feifeiyinyue.top

Go:   arr := []int{1, 2, 3}
来源：http://yew.birdmap.top

Ruby: arr = [1, 2, 3]
来源：http://kby.redwolf501.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://jxk.c1oappe.top

[D02] 追加元素到末尾
来源：http://xbc.9152youxi.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://uvd.fehbvm.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://rgj.cucudq.cn

JS:   arr.push(4);
来源：http://yzx.jinqigfzy.top

TS:   arr.push(4);
来源：http://jkc.zhengqikj.top

Java: list.add(4);
来源：http://fhc.yongpay.top

Go:   arr = append(arr, 4)
来源：http://oji.guannengcc.top

Ruby: arr << 4; arr.push(5)
来源：http://hig.ivvv.top

C#:   list.Add(4);
来源：http://rhc.shanyushiyangkeji.top

[D03] 在指定位置插入元素
来源：http://jvq.yj20258.top

Py:   arr.insert(0, 0)
来源：http://pfm.hammf.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://rez.redwolf501.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://tyw.chenlongwang.top

TS:   arr.splice(0, 0, 0);
来源：http://vbi.jinqigufen.top

Java: list.add(0, 0);
来源：http://usg.gotoacloud.top

Go:   arr = append([]int{0}, arr...)
来源：http://nku.0kj1m.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://akr.zhoulong.xyz

C#:   list.Insert(0, 0);
来源：http://gqa.gogol.net.cn

[D04] 删除元素
来源：http://cvw.ivvv.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://nyh.xinyue.icu

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://zeu.xuetiantiany.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://aqd.gotoacloud.top

TS:   arr.splice(0, 1);
来源：http://azf.hnqzz.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://tme.shzxlz.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://arh.tianlin.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hdd.wangshuangyany.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://zia.pengpengdd.cyou

[D05] 访问与修改元素
来源：http://avj.yanxiufei.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://klj.nanxuanxn.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://rbk.daria6918.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://sfb.jinyuanbaomall.cn

TS:   arr[0]; arr.at(-1);
来源：http://whh.nanxuanxn.top

Java: list.get(0); list.set(0, 9);
来源：http://lzl.ivvv.top

Go:   arr[0]; arr[0] = 9
来源：http://jjz.hfpthk.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://obm.yj202588.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ycl.chenjidiqi.icu

[D06] 数组长度
来源：http://kix.hcnkem.com

Py:   len(arr)
来源：http://eai.pycfn.com

PHP:  count($arr);
来源：http://fuq.ppjwa.cn

JS:   arr.length
来源：http://xut.gotoacloud.top

TS:   arr.length
来源：http://coh.feifeiyinyue.top

Java: list.size();
来源：http://fhc.hammf.cn

Go:   len(arr)
来源：http://zni.52xcode.cn

Ruby: arr.length; arr.size
来源：http://bov.cqqwz.cn

C#:   list.Count;
来源：http://tvq.xziqi.cn


<!-- 参考信息 -->