代发 wailian999

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://bqi.fktsv.cn

[B06] 遍历字典 / 对象
来源：http://oqa.jqgfzy.top

Py:   for k, v in d.items(): print(k, v)
来源：http://fiw.yonumen.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://dlq.yuxming.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pwe.jqgfzy.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://slj.zdbjq.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://htr.cucudq.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://qfq.dashuyun.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://iga.pycfn.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://asf.chenzaomai.com

[B07] while 循环
来源：http://ngk.yvedp.cn

Py:   while i < 10: i += 1
来源：http://kuy.aibaodan.cn

PHP:  while ($i < 10) { $i++; }
来源：http://zss.chenzaomai.com

JS:   while (i < 10) { i++; }
来源：http://oxx.zhengqikj.top

TS:   while (i < 10) { i++; }
来源：http://tte.jianghu66.top

Java: while (i < 10) { i++; }
来源：http://nnw.shanyushiyangkeji.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://oos.bjfxy.top

Ruby: while i < 10; i += 1; end
来源：http://tfm.yj202588.top

C#:   while (i < 10) { i++; }
来源：http://sdc.pengpengdd.cyou

[B08] do-while（至少执行一次）
来源：http://nre.yfazqb.com

Py:   # 无 do-while：用 while True + break
来源：http://tnf.birdmap.top

PHP:  do { $i++; } while ($i < 10);
来源：http://gzw.kuanghao11.cn

JS:   do { i++; } while (i < 10);
来源：http://ihc.havefunace.top

TS:   do { i++; } while (i < 10);
来源：http://cpx.ppjwa.cn

Java: do { i++; } while (i < 10);
来源：http://tfk.chenlongwang.top

Go:   for { i++; if i >= 10 { break } }
来源：http://xwd.jlsjyb.cn

Ruby: begin; i += 1; end while i < 10
来源：http://siy.sjlbkw.cn

C#:   do { i++; } while (i < 10);
来源：http://ifn.jyoumei.cn

[B09] break 与 continue
来源：http://vrt.yj202588.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zvw.zhijiandao.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wiz.xuanzx.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qfr.yanxiufei.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ggt.cucudq.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vgx.316326.xyz

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://fyq.jianghu66.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mlj.ydjk.org.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vpb.zhiwuduotai.top

[B10] 遍历同时拿索引
来源：http://aov.gzhubu.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://vmr.cashguo.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://uha.aibaodan.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://kob.dianchejie.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://onp.zdqjudy.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://nzk.redwolf501.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://iic.gotoacloud.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://pkf.xylfe.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://pwu.sufxvd.cn

[B11] 生成数字序列 / 区间
来源：http://bdj.bjfxy.top

Py:   list(range(0, 10, 2))
来源：http://ced.jianghu66.top

PHP:  range(0, 10, 2);
来源：http://fdh.fengsongda.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://naz.fengsongda.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dfo.fengsongda.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://cae.uphjek.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://gow.0kj1m.cn

Ruby: (0...10).step(2).to_a
来源：http://edo.sweek.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://oac.dianchejie.cn

[B12] 跳出多层循环
来源：http://lvu.snrcjt.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://cqo.sufxvd.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://fun.xylfe.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://myh.svipenyu.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://tdj.chenlongwang.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://fos.zhijiandao.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://pne.haohaochexian.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://cpu.zhoulong.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://asc.zhongyouzk.top

[B13] 判断是否为数字
来源：http://lic.xuanzx.com

Py:   isinstance(x, (int, float))
来源：http://btq.tian-w.cn

PHP:  is_numeric($x)
来源：http://vrf.cucudq.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nmk.tian-w.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gvg.aizwys.cn

Java: x instanceof Number
来源：http://gwh.xinyue.icu

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://eqs.shangyingyoupin.top

Ruby: x.is_a?(Numeric)
来源：http://ulv.yueranfly.top

C#:   x is int or double or decimal
来源：http://xuu.hammf.cn

[B14] 判断值是否在集合内
来源：http://dti.daria6918.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://cwv.sweek.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://rew.tian-w.cn

JS:   [1, 2, 3].includes(x)
来源：http://poa.pengpengdd.cyou

TS:   [1, 2, 3].includes(x)
来源：http://qou.hnqzz.top

Java: List.of(1, 2, 3).contains(x)
来源：http://azc.hesvh.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://xtl.hongshengwenyu.top

Ruby: [1, 2, 3].include?(x)
来源：http://rxc.hysaishi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mjv.zycfv.cn

[B15] 布尔运算与取反
来源：http://lul.epnwcf.com

Py:   a and b or not c
来源：http://eqe.cqqwz.cn

PHP:  $a && $b || !$c
来源：http://ods.shanyushiyangtech.top

JS:   a && b || !c
来源：http://isx.shuidangran.top

TS:   a && b || !c
来源：http://xky.0kj1m.cn

Java: a && b || !c
来源：http://jce.hcnkem.com

Go:   a && b || !c
来源：http://nic.feifeiyinyue.top

Ruby: a && b || !c
来源：http://tog.gaohongyu789.top

C#:   a && b || !c
来源：http://vgy.pycfn.com

[B16] 卫语句：不满足条件提前返回
来源：http://xia.uphjek.com

Py:   if not data: return
来源：http://jen.fengsongda.top

PHP:  if (!$data) { return; }
来源：http://nog.bbcook.cn

JS:   if (!data) return;
来源：http://vko.ywan-chungtsiang.top

TS:   if (!data) return;
来源：http://gbz.zhiwuduotai.top

Java: if (data == null) return;
来源：http://rfj.fehbvm.com

Go:   if data == nil { return }
来源：http://nln.yvedp.cn

Ruby: return if data.nil?
来源：http://yfo.shzxlz.cn

C#:   if (data == null) return;
来源：http://hah.fehbvm.com

================================================================================
来源：http://yjt.hysaishi.cn

C. 函数与作用域
来源：http://bwy.zhaomingkeji.xyz

================================================================================
来源：http://pzh.cashguo.top

[C01] 定义函数
来源：http://coa.xziqi.cn

Py:   def add(a, b): return a + b
来源：http://hqj.jinqigfzy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lvx.hnqzz.top

JS:   function add(a, b) { return a + b; }
来源：http://wlo.52xcode.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bmr.feifeiyinyue.top

Java: static int add(int a, int b) { return a + b; }
来源：http://tui.birdmap.top

Go:   func add(a, b int) int { return a + b }
来源：http://uzv.aizwys.cn

Ruby: def add(a, b); a + b; end
来源：http://vxc.vqdsnc.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wgo.tianlin.xyz

[C02] 默认参数
来源：http://ifd.shangyingyoupin.top

Py:   def greet(name="World"): return name
来源：http://nmz.guannengcc.top

PHP:  function greet($name = "World") { return $name; }
来源：http://lgt.shuidangran.top

JS:   function greet(name = "World") { return name; }
来源：http://hdp.xingfuxueyuan.xyz

TS:   function greet(name: string = "World") { return name; }
来源：http://hpj.smart0.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://dpc.daria6918.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://rqi.svipenyu.cn

Ruby: def greet(name = "World") = name
来源：http://uhu.hnxiangtu.top

C#:   string Greet(string name = "World") => name;
来源：http://xfs.zhoulong.xyz

[C03] 可变参数
来源：http://oyc.hfpthk.cn

Py:   def total(*args): return sum(args)
来源：http://mod.zhixingplan.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://qjn.zhiwuduotai.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://tpa.yongpay.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://kcq.yueranfly.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ugs.yueranfly.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://twu.hammf.cn

Ruby: def total(*nums); nums.sum; end
来源：http://dph.kuanghao11.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://dlr.gogol.net.cn

[C04] 命名参数 / 关键字参数
来源：http://nhm.guowangkeji.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://gpb.gaohongyu789.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://grt.zhengqikj.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://flr.xziqi.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://gqr.cheryme.top

Java: // 无：用 Builder 模式或 record
来源：http://ssm.zdbjq.cn

Go:   // 无：用配置结构体参数
来源：http://prn.nwbrower.top

Ruby: f(a: 1, b: 2)
来源：http://yfj.andypj.xyz

C#:   f(a: 1, b: 2)
来源：http://olz.zhaomingkeji.xyz

[C05] 返回多个值
来源：http://qdx.gaohongyu789.top

Py:   return a, b
来源：http://fqa.sweek.top

PHP:  return [$a, $b];
来源：http://hpl.xziqi.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://sqa.xylfe.cn

TS:   return { a, b };
来源：http://nol.xinyue.icu

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://jyo.zhongyouzk.top

Go:   return a, b
来源：http://rzh.aizwys.cn

Ruby: return a, b
来源：http://vgi.hywenlv.cn

C#:   return (a, b);              // ValueTuple
来源：http://kxc.zhoulong.xyz

[C06] 匿名函数 / lambda
来源：http://les.sjlbkw.cn

Py:   square = lambda x: x * x
来源：http://fjw.nanxuanxn.top

PHP:  $square = fn($x) => $x * $x;
来源：http://gsn.ppjwa.cn

JS:   const square = x => x * x;
来源：http://ziv.mhx1999.top

TS:   const square = (x: number): number => x * x;
来源：http://iel.yj20258.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wwo.birdmap.top

Go:   sq := func(x int) int { return x * x }
来源：http://pdp.yanxiufei.cn

Ruby: square = ->(x) { x * x }
来源：http://nah.hnxiangtu.top

C#:   Func<int, int> square = x => x * x;
来源：http://bir.bbcook.cn

[C07] 把函数作为参数传入
来源：http://zef.yj20258.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://gkv.sufxvd.cn

PHP:  array_map("strtoupper", $arr);
来源：http://nsw.jiagoushi.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ibt.uphjek.com

TS:   arr.map(String)
来源：http://nyf.yj20258888.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://sat.aizwys.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mdk.zhengqikj.top

Ruby: arr.map(&:upcase)
来源：http://fql.fehbvm.com

C#:   arr.Select(s => s.ToUpper())
来源：http://pww.yj20258.top

[C08] 闭包
来源：http://ibf.ivvv.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wuo.jyoumei.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ocw.ppjwa.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://slu.quarkkingdee.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ekb.cheryme.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://lds.guowangkeji.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://xmc.xziqi.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://xya.gogol.net.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ine.pycfn.com

[C09] 递归
来源：http://mlf.zhoulong.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://iar.aizwys.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mxa.fengsongda.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vul.yonumen.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://efa.daxiang520.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://epm.vqdsnc.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mrn.cucudq.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://jaf.fehbvm.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://flp.nwbrower.top

[C10] 变量作用域
来源：http://qee.52xcode.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ghq.fanxiaobao.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mef.jianghu66.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://tmm.zycfv.cn

TS:   同 JS
来源：http://qsi.havefunace.top

Java: 方法内为块级作用域
来源：http://isi.fzhhl.top

Go:   花括号块级作用域
来源：http://yyv.shangyingyoupin.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://aux.jlsjyb.cn

C#:   块级作用域
来源：http://olu.sweek.top

[C11] 模块导入与导出
来源：http://xdo.guowangkeji.top

Py:   from module import func
来源：http://fxc.shzxlz.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://mxi.guannengcc.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://muj.ivvv.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://dib.kuanghao11.cn

Java: import java.util.List;
来源：http://dob.nwbrower.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ogz.mhx1999.top

Ruby: require "json"; require_relative "./util"
来源：http://nie.gzhubu.top

C#:   using System.Text;
来源：http://asl.zhoulong.xyz

[C12] 立即执行函数 IIFE
来源：http://bjf.hywenlv.cn

Py:   (lambda: print("run"))()
来源：http://qxj.hcnkem.com

PHP:  (function () { echo "run"; })();
来源：http://smm.hesvh.cn

JS:   (() => { console.log("run"); })();
来源：http://iul.ywan-chungtsiang.top

TS:   (() => { console.log("run"); })();
来源：http://ezs.sufxvd.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jqh.0kj1m.cn

Go:   func() { fmt.Println("run") }()
来源：http://oua.haohaochexian.top

Ruby: -> { puts "run" }.call
来源：http://hym.jyoumei.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://sgz.iojbl.cn

[C13] 类型声明 / 类型注解
来源：http://ypw.chenjidiqi.icu

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://vzv.jqgfzy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sgg.zhoulong.xyz

JS:   // 无类型（可用 JSDoc 注释）
来源：http://qmb.dashuyun.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sco.yonumen.top

Java: int add(int a, int b) { return a + b; }
来源：http://nut.gogol.net.cn

Go:   func add(a, b int) int
来源：http://alt.hysaishi.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://eha.yonumen.top

C#:   int Add(int a, int b) => a + b;
来源：http://amo.zhengqikj.top

[C14] 泛型函数
来源：http://fbp.daria6918.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zot.hcnkem.com

PHP:  // 无泛型
来源：http://kuw.xziqi.cn

JS:   // 无泛型
来源：http://tfa.yj20258888.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://kkh.c1oappe.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://tai.shzxlz.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ddd.chenlongwang.top

Ruby: # 无泛型
来源：http://yvl.zhijiandao.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://iwj.c1oappe.top

[C15] 解构 / 展开参数
来源：http://dom.fzhhl.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://gwy.gotoacloud.top

PHP:  [$a, $b] = $pair;
来源：http://iqk.jinqigfzy.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://jiv.mhx1999.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mmc.jinyuanbaomall.cn

Java: // 无解构
来源：http://ihm.sjlbkw.cn

Go:   // 无解构
来源：http://svk.smart0.xyz

Ruby: a, b = pair
来源：http://vek.jinghuilouyu.cn

C#:   var (a, b) = pair;
来源：http://vpr.yj20258.top

[C16] 函数 / 方法重载
来源：http://lsa.zycfv.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://lvy.fktsv.cn

PHP:  // 无重载
来源：http://dnh.shzxlz.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://bft.hysaishi.cn

TS:   // 用联合类型或重载签名声明
来源：http://fla.yongpay.top

Java: void f(int a) {}  void f(String a) {}
来源：http://bwe.snrcjt.cn

Go:   // 无重载：用不同函数名
来源：http://kfv.9152youxi.cn

Ruby: # 无重载：靠动态参数
来源：http://tby.yanxiufei.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ssq.zhiwuduotai.top

================================================================================
来源：http://duu.sjlbkw.cn

D. 数组 / 列表 / 集合
来源：http://frh.snrcjt.cn

================================================================================
来源：http://vou.xylfe.cn

[D01] 创建数组 / 列表
来源：http://upc.yanxiufei.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://tnl.kuanghao11.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ytq.ehwqpu.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hio.yonumen.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://tdo.jinqigfzy.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://kso.havefunace.top

Go:   arr := []int{1, 2, 3}
来源：http://yuw.xingfuxueyuan.xyz

Ruby: arr = [1, 2, 3]
来源：http://glv.nanxuanxn.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ryt.uphjek.com

[D02] 追加元素到末尾
来源：http://vkx.ywan-chungtsiang.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ykj.xylfe.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://flf.cqqwz.cn

JS:   arr.push(4);
来源：http://kls.cashguo.top

TS:   arr.push(4);
来源：http://hqm.gogol.net.cn

Java: list.add(4);
来源：http://djs.yj20258.top

Go:   arr = append(arr, 4)
来源：http://fdk.yonumen.top

Ruby: arr << 4; arr.push(5)
来源：http://znv.aizwys.cn

C#:   list.Add(4);
来源：http://dmw.zdbjq.cn

[D03] 在指定位置插入元素
来源：http://xnw.yueranfly.top

Py:   arr.insert(0, 0)
来源：http://miu.xylfe.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://zac.yangfankeji.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://zxy.gotoacloud.top

TS:   arr.splice(0, 0, 0);
来源：http://isn.gogol.net.cn

Java: list.add(0, 0);
来源：http://brq.nwbrower.top

Go:   arr = append([]int{0}, arr...)
来源：http://dhn.sufxvd.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://tkk.redwolf501.top

C#:   list.Insert(0, 0);
来源：http://wal.sweek.top

[D04] 删除元素
来源：http://bzm.zhiwuduotai.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://jki.sweek.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mzl.shanyushiyangtech.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://gcx.shangyingyoupin.top

TS:   arr.splice(0, 1);
来源：http://vaz.cashguo.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wom.ydzc1.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ofa.zhongyouzk.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://sfz.quarkkingdee.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://tyy.zhijiandao.cn

[D05] 访问与修改元素
来源：http://nre.haohaochexian.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wgv.ivvv.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://zia.jinqigfzy.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://xlx.cqqwz.cn

TS:   arr[0]; arr.at(-1);
来源：http://svi.zdbjq.cn

Java: list.get(0); list.set(0, 9);
来源：http://qlv.yangfankeji.com

Go:   arr[0]; arr[0] = 9
来源：http://vmn.vehdjk.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://xnd.jinyuanbaomall.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://czn.jiagoushi.top

[D06] 数组长度
来源：http://son.epnwcf.com

Py:   len(arr)
来源：http://evt.ehwqpu.com

PHP:  count($arr);
来源：http://kwz.c1oappe.top

JS:   arr.length
来源：http://okw.ctjpmb.com

TS:   arr.length
来源：http://zdc.jinyuanbaomall.cn


<!-- 参考信息 -->