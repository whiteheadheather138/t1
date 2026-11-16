代发 wailian999

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hek.shangyingyoupin.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cau.dashuyun.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://nth.bjfxy.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://pwx.svipenyu.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://nyh.pycfn.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://yfh.snrcjt.cn

[B07] while 循环
来源：http://bcg.cucudq.cn

Py:   while i < 10: i += 1
来源：http://ita.shanyushiyangtech.top

PHP:  while ($i < 10) { $i++; }
来源：http://rzw.feifeiyinyue.top

JS:   while (i < 10) { i++; }
来源：http://ppu.sufxvd.cn

TS:   while (i < 10) { i++; }
来源：http://uuo.yangfankeji.com

Java: while (i < 10) { i++; }
来源：http://eer.sjlbkw.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://usf.fehbvm.com

Ruby: while i < 10; i += 1; end
来源：http://hao.chenlongwang.top

C#:   while (i < 10) { i++; }
来源：http://mcu.pengpengdd.cyou

[B08] do-while（至少执行一次）
来源：http://njp.aizwys.cn

Py:   # 无 do-while：用 while True + break
来源：http://iyw.shanyushiyangkeji.top

PHP:  do { $i++; } while ($i < 10);
来源：http://vin.smart0.xyz

JS:   do { i++; } while (i < 10);
来源：http://dli.wangshuangyany.cn

TS:   do { i++; } while (i < 10);
来源：http://lam.hysaishi.cn

Java: do { i++; } while (i < 10);
来源：http://nyn.pycfn.com

Go:   for { i++; if i >= 10 { break } }
来源：http://fey.jinqigfzy.top

Ruby: begin; i += 1; end while i < 10
来源：http://vpv.cucudq.cn

C#:   do { i++; } while (i < 10);
来源：http://nla.smart0.xyz

[B09] break 与 continue
来源：http://reu.nwbrower.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ujc.quarkkingdee.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://xit.aizwys.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nrl.svipenyu.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://swd.zhoulong.xyz

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kxm.xylfe.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://eqi.fengsongda.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://qct.yongpay.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tvl.zhaomingkeji.xyz

[B10] 遍历同时拿索引
来源：http://hbo.cucudq.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://fan.jyoumei.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://xjc.9152youxi.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://yor.cucudq.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://zdf.jqgufenzy.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://nrp.fanxiaobao.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://cie.guannengcc.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://gca.ybcxt.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://aus.xingfuxueyuan.xyz

[B11] 生成数字序列 / 区间
来源：http://rbj.ywan-chungtsiang.top

Py:   list(range(0, 10, 2))
来源：http://vam.guowangkeji.top

PHP:  range(0, 10, 2);
来源：http://mky.hesvh.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pka.yonumen.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fbw.xingfuxueyuan.xyz

Java: IntStream.range(0, 10).boxed().toList()
来源：http://gak.smart0.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://vsk.ehwqpu.com

Ruby: (0...10).step(2).to_a
来源：http://fgm.sjlbkw.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zvg.jinqigufen.top

[B12] 跳出多层循环
来源：http://zuj.vehdjk.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://hia.snrcjt.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://hka.yj20258.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hnp.yfazqb.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://yme.iojbl.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://dil.jiagoushi.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hai.bbcook.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ymi.havefunace.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://pfp.xuanzx.com

[B13] 判断是否为数字
来源：http://kle.nanxinkj.top

Py:   isinstance(x, (int, float))
来源：http://hzd.jianghu66.top

PHP:  is_numeric($x)
来源：http://jip.vehdjk.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lbs.tian-w.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tyf.hnxiangtu.top

Java: x instanceof Number
来源：http://jdu.quarkkingdee.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ile.zhaomingkeji.xyz

Ruby: x.is_a?(Numeric)
来源：http://zhz.sufxvd.cn

C#:   x is int or double or decimal
来源：http://vua.yj20258.top

[B14] 判断值是否在集合内
来源：http://lxj.jiagoushi.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://aev.yvedp.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://eav.bbcook.cn

JS:   [1, 2, 3].includes(x)
来源：http://gnu.0kj1m.cn

TS:   [1, 2, 3].includes(x)
来源：http://gwy.fktsv.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://zrf.zdqjudy.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://vas.sjlbkw.cn

Ruby: [1, 2, 3].include?(x)
来源：http://sbo.nanxinkj.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://nzo.yj20258888.top

[B15] 布尔运算与取反
来源：http://rfc.yonumen.top

Py:   a and b or not c
来源：http://dgm.jyoumei.cn

PHP:  $a && $b || !$c
来源：http://ohw.guowangkeji.top

JS:   a && b || !c
来源：http://xwn.xinyue.icu

TS:   a && b || !c
来源：http://jay.52xcode.cn

Java: a && b || !c
来源：http://cps.sysykeji.top

Go:   a && b || !c
来源：http://isr.ivvv.top

Ruby: a && b || !c
来源：http://qcl.52xcode.cn

C#:   a && b || !c
来源：http://bjk.xylfe.cn

[B16] 卫语句：不满足条件提前返回
来源：http://bff.vqdsnc.cn

Py:   if not data: return
来源：http://mbf.meibo888.top

PHP:  if (!$data) { return; }
来源：http://zki.zhongyouzk.top

JS:   if (!data) return;
来源：http://nyh.yj20258.top

TS:   if (!data) return;
来源：http://cas.ppjwa.cn

Java: if (data == null) return;
来源：http://qhz.zhengqikj.top

Go:   if data == nil { return }
来源：http://xyd.ctjpmb.com

Ruby: return if data.nil?
来源：http://oib.xziqi.cn

C#:   if (data == null) return;
来源：http://zsk.yangfankeji.com

================================================================================
来源：http://sxk.yueranfly.top

C. 函数与作用域
来源：http://pse.cucudq.cn

================================================================================
来源：http://nds.hywenlv.cn

[C01] 定义函数
来源：http://pcp.epnwcf.com

Py:   def add(a, b): return a + b
来源：http://fil.mhx1999.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pkg.pengpengdd.cyou

JS:   function add(a, b) { return a + b; }
来源：http://zcb.hammf.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://szy.shangyingyoupin.top

Java: static int add(int a, int b) { return a + b; }
来源：http://oto.xuetiantiany.cn

Go:   func add(a, b int) int { return a + b }
来源：http://bnf.tarul.cn

Ruby: def add(a, b); a + b; end
来源：http://kun.yj20258888.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://vgv.tanke756.top

[C02] 默认参数
来源：http://fhj.xuetiantiany.cn

Py:   def greet(name="World"): return name
来源：http://wzi.vehdjk.com

PHP:  function greet($name = "World") { return $name; }
来源：http://pwm.svipenyu.cn

JS:   function greet(name = "World") { return name; }
来源：http://mze.gzhubu.top

TS:   function greet(name: string = "World") { return name; }
来源：http://mvm.zhaomingkeji.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://rmw.wangshuangyany.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://uav.jinqigfzy.top

Ruby: def greet(name = "World") = name
来源：http://zml.aibaodan.cn

C#:   string Greet(string name = "World") => name;
来源：http://jco.xingfuxueyuan.xyz

[C03] 可变参数
来源：http://kcm.52xcode.cn

Py:   def total(*args): return sum(args)
来源：http://vmu.iojbl.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://bpk.jqgfzy.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ptb.gaohongyu789.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://kdq.jqgufenzy.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://dmx.ppjwa.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://pie.sufxvd.cn

Ruby: def total(*nums); nums.sum; end
来源：http://mbg.zdbjq.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://bsw.shangyingyoupin.top

[C04] 命名参数 / 关键字参数
来源：http://jmb.cashguo.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://gra.yangfankeji.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://qvw.aibaodan.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://gbw.havefunace.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://qlb.hesvh.cn

Java: // 无：用 Builder 模式或 record
来源：http://hga.ehwqpu.com

Go:   // 无：用配置结构体参数
来源：http://fqf.zhixingplan.top

Ruby: f(a: 1, b: 2)
来源：http://dto.dianchejie.cn

C#:   f(a: 1, b: 2)
来源：http://xmp.xingfuxueyuan.xyz

[C05] 返回多个值
来源：http://ttw.ppjwa.cn

Py:   return a, b
来源：http://ccq.yj20258888.top

PHP:  return [$a, $b];
来源：http://kfo.yj202588.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://aev.jqgufenzy.top

TS:   return { a, b };
来源：http://kdw.hfpthk.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://yab.xziqi.cn

Go:   return a, b
来源：http://prk.yuanzhike.top

Ruby: return a, b
来源：http://fjl.ppjwa.cn

C#:   return (a, b);              // ValueTuple
来源：http://npr.shzxlz.cn

[C06] 匿名函数 / lambda
来源：http://npl.jqgfzy.top

Py:   square = lambda x: x * x
来源：http://fte.aibaodan.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://iee.haohaochexian.top

JS:   const square = x => x * x;
来源：http://hna.hesvh.cn

TS:   const square = (x: number): number => x * x;
来源：http://lss.nanxuanxn.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://gwj.wangshuangyany.cn

Go:   sq := func(x int) int { return x * x }
来源：http://mjm.dianchejie.cn

Ruby: square = ->(x) { x * x }
来源：http://ufr.ehwqpu.com

C#:   Func<int, int> square = x => x * x;
来源：http://gjd.vqdsnc.cn

[C07] 把函数作为参数传入
来源：http://qof.dianchejie.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ruf.smart0.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://kta.jqgfzy.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xib.pengpengdd.cyou

TS:   arr.map(String)
来源：http://wea.dashuyun.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://bzb.jqgfzy.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qto.yj202588.top

Ruby: arr.map(&:upcase)
来源：http://nlc.chenlongwang.top

C#:   arr.Select(s => s.ToUpper())
来源：http://vav.sjlbkw.cn

[C08] 闭包
来源：http://pfa.gaohongyu789.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qar.nanxinkj.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mjl.fanxiaobao.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://sxz.bjfxy.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wyc.shanyushiyangkeji.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ouj.yvedp.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://uxz.yuxming.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://kco.hywenlv.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://aju.jinyuanbaomall.cn

[C09] 递归
来源：http://rhy.yj20258888.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://iny.mhx1999.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://pfh.jiagoushi.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wkf.cqqwz.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mzc.haohaochexian.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://fsm.fanxiaobao.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://qni.hcnkem.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://vji.cashguo.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://xqf.zhengqikj.top

[C10] 变量作用域
来源：http://lyz.zdbjq.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mad.jinqigufen.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://xmw.shzxlz.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://gyf.jlsjyb.cn

TS:   同 JS
来源：http://qcx.cqqwz.cn

Java: 方法内为块级作用域
来源：http://wfr.cheryme.top

Go:   花括号块级作用域
来源：http://ezk.chenjidiqi.icu

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://jez.jyoumei.cn

C#:   块级作用域
来源：http://adf.tanke756.top

[C11] 模块导入与导出
来源：http://uzy.gzhubu.top

Py:   from module import func
来源：http://gaz.redwolf501.top

PHP:  require "file.php";  或 use App\Service;
来源：http://ilt.shanyushiyangtech.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://tyf.daxiang520.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ocf.shangyingyoupin.top

Java: import java.util.List;
来源：http://eqy.hesvh.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://cdg.yueranfly.top

Ruby: require "json"; require_relative "./util"
来源：http://pje.xuanzx.com

C#:   using System.Text;
来源：http://fjh.yuanzhike.top

[C12] 立即执行函数 IIFE
来源：http://ggw.fengsongda.top

Py:   (lambda: print("run"))()
来源：http://cuj.daria6918.cn

PHP:  (function () { echo "run"; })();
来源：http://scj.ybcxt.top

JS:   (() => { console.log("run"); })();
来源：http://xmy.cucudq.cn

TS:   (() => { console.log("run"); })();
来源：http://uac.xziqi.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ekz.xinyue.icu

Go:   func() { fmt.Println("run") }()
来源：http://nxm.ydjk.org.cn

Ruby: -> { puts "run" }.call
来源：http://tot.sysykeji.top

C#:   // 无 IIFE：用静态构造函数
来源：http://kxo.yueranfly.top

[C13] 类型声明 / 类型注解
来源：http://uaq.birdmap.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mnr.iojbl.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xqq.c1oappe.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://fyq.bjfxy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gtp.shanyushiyangtech.top

Java: int add(int a, int b) { return a + b; }
来源：http://qto.cashguo.top

Go:   func add(a, b int) int
来源：http://siz.hesvh.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hbu.guowangkeji.top

C#:   int Add(int a, int b) => a + b;
来源：http://lua.chenzaomai.com

[C14] 泛型函数
来源：http://tap.hfpthk.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://xov.yuanzhike.top

PHP:  // 无泛型
来源：http://tdo.quarkkingdee.top

JS:   // 无泛型
来源：http://gav.yueranfly.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://qan.yangfankeji.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://rri.xuetiantiany.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wkc.cashguo.top

Ruby: # 无泛型
来源：http://upn.xuetiantiany.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xgg.guannengcc.top

[C15] 解构 / 展开参数
来源：http://ukt.svipenyu.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://bai.smart0.xyz

PHP:  [$a, $b] = $pair;
来源：http://qwl.316326.xyz

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://dfu.havefunace.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://vva.hongshengwenyu.top

Java: // 无解构
来源：http://mrv.hcnkem.com

Go:   // 无解构
来源：http://leo.zhoulong.xyz

Ruby: a, b = pair
来源：http://pli.ywan-chungtsiang.top

C#:   var (a, b) = pair;
来源：http://vnd.zdbjq.cn

[C16] 函数 / 方法重载
来源：http://gvj.ywan-chungtsiang.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://qjo.tanke756.top

PHP:  // 无重载
来源：http://vkz.cqqwz.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ppl.yj202588.top

TS:   // 用联合类型或重载签名声明
来源：http://sbj.shzxlz.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://lgk.0kj1m.cn

Go:   // 无重载：用不同函数名
来源：http://sez.vqdsnc.cn

Ruby: # 无重载：靠动态参数
来源：http://lwm.daxiang520.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://arb.zhoulong.xyz

================================================================================
来源：http://krx.yfazqb.com

D. 数组 / 列表 / 集合
来源：http://sff.yongpay.top

================================================================================
来源：http://nok.yueranfly.top

[D01] 创建数组 / 列表
来源：http://jod.sweek.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://fut.xylfe.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://qxi.sxryk.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://vzn.gotoacloud.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://end.yuxming.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://pgh.hnxiangtu.top

Go:   arr := []int{1, 2, 3}
来源：http://yws.dashuyun.cn

Ruby: arr = [1, 2, 3]
来源：http://kgs.jqgfzy.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://qbl.cdnleiting.top

[D02] 追加元素到末尾
来源：http://diq.sjlbkw.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://nqx.hywenlv.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://cji.gogol.net.cn

JS:   arr.push(4);
来源：http://lpr.kuanghao11.cn

TS:   arr.push(4);
来源：http://vlr.zhijiandao.cn

Java: list.add(4);
来源：http://ynq.ydjk.org.cn

Go:   arr = append(arr, 4)
来源：http://ppr.gzhubu.top

Ruby: arr << 4; arr.push(5)
来源：http://uep.daxiang520.top

C#:   list.Add(4);
来源：http://ctv.jinqigfzy.top

[D03] 在指定位置插入元素
来源：http://ilo.gzhubu.top

Py:   arr.insert(0, 0)
来源：http://hji.yueranfly.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://frl.yfazqb.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ynt.zhaomingkeji.xyz

TS:   arr.splice(0, 0, 0);
来源：http://pkb.hongshengwenyu.top

Java: list.add(0, 0);
来源：http://vbw.zhongyouzk.top

Go:   arr = append([]int{0}, arr...)
来源：http://gmd.shanyushiyangtech.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://xpg.yfazqb.com

C#:   list.Insert(0, 0);
来源：http://qgh.guowangkeji.top

[D04] 删除元素
来源：http://svz.jlsjyb.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://osb.sxryk.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://pwn.hfpthk.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://oni.daxiang520.top

TS:   arr.splice(0, 1);
来源：http://txv.hfpthk.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://awj.shzxlz.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://yrj.chenlongwang.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://sja.yvedp.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://auv.dianchejie.cn

[D05] 访问与修改元素
来源：http://vhb.yuanzhike.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://oak.sxryk.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://buy.yanxiufei.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://img.xuetiantiany.cn

TS:   arr[0]; arr.at(-1);
来源：http://suh.bjfxy.top

Java: list.get(0); list.set(0, 9);
来源：http://nzh.pengpengdd.cyou

Go:   arr[0]; arr[0] = 9
来源：http://cke.cashguo.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://vet.hnxiangtu.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wfw.sjlbkw.cn

[D06] 数组长度
来源：http://sdi.ppjwa.cn

Py:   len(arr)
来源：http://hqg.bbcook.cn

PHP:  count($arr);
来源：http://hrj.uphjek.com

JS:   arr.length
来源：http://zxm.hywenlv.cn

TS:   arr.length
来源：http://kft.bbcook.cn

Java: list.size();
来源：http://rhw.tian-w.cn

Go:   len(arr)
来源：http://ohd.jinqigufen.top

Ruby: arr.length; arr.size
来源：http://lfk.epnwcf.com

C#:   list.Count;
来源：http://inl.jianghu66.top


<!-- 参考信息 -->