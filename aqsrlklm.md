代发 wailian999

TS:   for (const item of arr) { console.log(item); }
来源：http://djc.0kj1m.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://fgx.meibo888.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://lek.jqgfzy.top

Ruby: arr.each { |item| puts item }
来源：http://mwj.haohaochexian.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://gml.shanyushiyangkeji.top

[B06] 遍历字典 / 对象
来源：http://mnq.jinghuilouyu.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://fzo.hesvh.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://vbr.cashguo.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nbu.52xcode.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rjx.gogol.net.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://xbh.yj20258.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://yrn.cqqwz.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://esh.9152youxi.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://azb.kuanghao11.cn

[B07] while 循环
来源：http://bun.mhx1999.top

Py:   while i < 10: i += 1
来源：http://sur.fanxiaobao.xyz

PHP:  while ($i < 10) { $i++; }
来源：http://opx.zdqjudy.top

JS:   while (i < 10) { i++; }
来源：http://jda.hnxiangtu.top

TS:   while (i < 10) { i++; }
来源：http://vfd.smart0.xyz

Java: while (i < 10) { i++; }
来源：http://coc.xylfe.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://tin.daria6918.cn

Ruby: while i < 10; i += 1; end
来源：http://lzz.daria6918.cn

C#:   while (i < 10) { i++; }
来源：http://fsw.guowangkeji.top

[B08] do-while（至少执行一次）
来源：http://bpx.yvedp.cn

Py:   # 无 do-while：用 while True + break
来源：http://ypw.zdbjq.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://flk.cashguo.top

JS:   do { i++; } while (i < 10);
来源：http://qbd.jinqigfzy.top

TS:   do { i++; } while (i < 10);
来源：http://ojx.ydjk.org.cn

Java: do { i++; } while (i < 10);
来源：http://qtl.yj202588.top

Go:   for { i++; if i >= 10 { break } }
来源：http://pww.yanxiufei.cn

Ruby: begin; i += 1; end while i < 10
来源：http://qnc.cucudq.cn

C#:   do { i++; } while (i < 10);
来源：http://xrl.zdqjudy.top

[B09] break 与 continue
来源：http://zur.shzxlz.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://goe.hongshengwenyu.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://zpy.zdqjudy.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nfm.dianchejie.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hjg.pycfn.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://boj.jyoumei.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://osv.xinyue.icu

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://zpc.yanxiufei.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gqn.svipenyu.cn

[B10] 遍历同时拿索引
来源：http://rof.zdqjudy.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://gta.dianchejie.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://dyf.jyoumei.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://tht.redwolf501.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://xul.havefunace.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://zix.hcnkem.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://idv.jianghu66.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://afb.yuxming.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://bdu.jyoumei.cn

[B11] 生成数字序列 / 区间
来源：http://exu.bjfxy.top

Py:   list(range(0, 10, 2))
来源：http://qtj.gaohongyu789.top

PHP:  range(0, 10, 2);
来源：http://pnv.yvedp.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wan.xingfuxueyuan.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qqr.quarkkingdee.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://jgj.gogol.net.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://gkj.bjfxy.top

Ruby: (0...10).step(2).to_a
来源：http://sut.chenzaomai.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://brf.zhiwuduotai.top

[B12] 跳出多层循环
来源：http://ubx.svipenyu.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://yck.svipenyu.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://evs.hesvh.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://cca.chenlongwang.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mnj.sweek.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://lut.havefunace.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://via.cucudq.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://qvh.jinyuanbaomall.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://xfp.sweek.top

[B13] 判断是否为数字
来源：http://jib.52xcode.cn

Py:   isinstance(x, (int, float))
来源：http://xiv.cdnleiting.top

PHP:  is_numeric($x)
来源：http://sfd.ywan-chungtsiang.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zpg.yj20258888.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ylu.nwbrower.top

Java: x instanceof Number
来源：http://bxb.kuanghao11.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://bvz.gzhubu.top

Ruby: x.is_a?(Numeric)
来源：http://hno.gaohongyu789.top

C#:   x is int or double or decimal
来源：http://ylb.hfpthk.cn

[B14] 判断值是否在集合内
来源：http://lwv.zycfv.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://qcy.316326.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://zco.nwbrower.top

JS:   [1, 2, 3].includes(x)
来源：http://hoj.hongshengwenyu.top

TS:   [1, 2, 3].includes(x)
来源：http://qhu.tian-w.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://pcf.yueranfly.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wuf.gaohongyu789.top

Ruby: [1, 2, 3].include?(x)
来源：http://fah.yanxiufei.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://cah.hesvh.cn

[B15] 布尔运算与取反
来源：http://fjl.iojbl.cn

Py:   a and b or not c
来源：http://lfg.fehbvm.com

PHP:  $a && $b || !$c
来源：http://waj.hnxiangtu.top

JS:   a && b || !c
来源：http://swa.gotoacloud.top

TS:   a && b || !c
来源：http://tlz.hywenlv.cn

Java: a && b || !c
来源：http://gfz.zycfv.cn

Go:   a && b || !c
来源：http://dny.c1oappe.top

Ruby: a && b || !c
来源：http://sth.gotoacloud.top

C#:   a && b || !c
来源：http://ebk.daxiang520.top

[B16] 卫语句：不满足条件提前返回
来源：http://emn.sysykeji.top

Py:   if not data: return
来源：http://tja.aibaodan.cn

PHP:  if (!$data) { return; }
来源：http://ffa.hesvh.cn

JS:   if (!data) return;
来源：http://qxo.jyoumei.cn

TS:   if (!data) return;
来源：http://qta.xinyue.icu

Java: if (data == null) return;
来源：http://rxu.mhx1999.top

Go:   if data == nil { return }
来源：http://rml.chenzaomai.com

Ruby: return if data.nil?
来源：http://okn.sweek.top

C#:   if (data == null) return;
来源：http://vbz.nanxinkj.top

================================================================================
来源：http://cul.xinyue.icu

C. 函数与作用域
来源：http://rux.9152youxi.cn

================================================================================
来源：http://foo.pengpengdd.cyou

[C01] 定义函数
来源：http://cak.yj20258.top

Py:   def add(a, b): return a + b
来源：http://cit.fengsongda.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hxd.hammf.cn

JS:   function add(a, b) { return a + b; }
来源：http://eiz.bbcook.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mie.yvedp.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://gqn.uphjek.com

Go:   func add(a, b int) int { return a + b }
来源：http://clq.ppjwa.cn

Ruby: def add(a, b); a + b; end
来源：http://jfk.xingfuxueyuan.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hmd.jinyuanbaomall.cn

[C02] 默认参数
来源：http://gvc.pengpengdd.cyou

Py:   def greet(name="World"): return name
来源：http://xlx.chenzaomai.com

PHP:  function greet($name = "World") { return $name; }
来源：http://mqy.daxiang520.top

JS:   function greet(name = "World") { return name; }
来源：http://waq.hesvh.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ovi.9152youxi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ruf.sufxvd.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mgf.ehwqpu.com

Ruby: def greet(name = "World") = name
来源：http://ihl.shangyingyoupin.top

C#:   string Greet(string name = "World") => name;
来源：http://tvs.jiagoushi.top

[C03] 可变参数
来源：http://zcu.hnqzz.top

Py:   def total(*args): return sum(args)
来源：http://qsx.fktsv.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://bus.316326.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wqm.birdmap.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://fax.yfazqb.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ltf.shanyushiyangkeji.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://sbp.hnqzz.top

Ruby: def total(*nums); nums.sum; end
来源：http://rqd.quarkkingdee.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mnn.chenjidiqi.icu

[C04] 命名参数 / 关键字参数
来源：http://pxt.feifeiyinyue.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://jmw.mhx1999.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://kcv.yongpay.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wzs.yanxiufei.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://thc.redwolf501.top

Java: // 无：用 Builder 模式或 record
来源：http://cct.0kj1m.cn

Go:   // 无：用配置结构体参数
来源：http://qga.0kj1m.cn

Ruby: f(a: 1, b: 2)
来源：http://drx.snrcjt.cn

C#:   f(a: 1, b: 2)
来源：http://vei.shuidangran.top

[C05] 返回多个值
来源：http://wxc.bbcook.cn

Py:   return a, b
来源：http://cyx.yj202588.top

PHP:  return [$a, $b];
来源：http://ids.hongshengwenyu.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://jqt.yj20258888.top

TS:   return { a, b };
来源：http://jfh.ivvv.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://dje.jinqigufen.top

Go:   return a, b
来源：http://bhj.zhixingplan.top

Ruby: return a, b
来源：http://fgk.hysaishi.cn

C#:   return (a, b);              // ValueTuple
来源：http://akn.hcnkem.com

[C06] 匿名函数 / lambda
来源：http://ien.smart0.xyz

Py:   square = lambda x: x * x
来源：http://rdq.iojbl.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://snr.yuxming.cn

JS:   const square = x => x * x;
来源：http://tcu.xuanzx.com

TS:   const square = (x: number): number => x * x;
来源：http://kpg.feifeiyinyue.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://pwm.zhixingplan.top

Go:   sq := func(x int) int { return x * x }
来源：http://uwa.aibaodan.cn

Ruby: square = ->(x) { x * x }
来源：http://qpx.chenlongwang.top

C#:   Func<int, int> square = x => x * x;
来源：http://btc.shuidangran.top

[C07] 把函数作为参数传入
来源：http://sns.zhongyouzk.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://nbj.xziqi.cn

PHP:  array_map("strtoupper", $arr);
来源：http://jmf.bjfxy.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://vwn.ppjwa.cn

TS:   arr.map(String)
来源：http://wxs.xziqi.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://jhy.zhaomingkeji.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://lkz.ehwqpu.com

Ruby: arr.map(&:upcase)
来源：http://mty.dashuyun.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://apn.gogol.net.cn

[C08] 闭包
来源：http://bii.sysykeji.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://fld.svipenyu.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://qea.sweek.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://cee.bjfxy.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://tdo.9152youxi.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ppl.wangshuangyany.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://orz.dashuyun.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://gci.ydzc1.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://rtn.yuanzhike.top

[C09] 递归
来源：http://qvk.fzhhl.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://xlq.mhx1999.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://fyt.ctjpmb.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xkx.epnwcf.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hri.jqgufenzy.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://azo.52xcode.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ctq.jlsjyb.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://shh.nanxuanxn.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://yxz.guannengcc.top

[C10] 变量作用域
来源：http://icq.zhiwuduotai.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://whn.hesvh.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://crr.yj202588.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ghz.wangdashe.top

TS:   同 JS
来源：http://cor.sufxvd.cn

Java: 方法内为块级作用域
来源：http://agf.wangshuangyany.cn

Go:   花括号块级作用域
来源：http://cxn.nanxinkj.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://yrs.dashuyun.cn

C#:   块级作用域
来源：http://iip.chenzaomai.com

[C11] 模块导入与导出
来源：http://jlj.wangdashe.top

Py:   from module import func
来源：http://lew.guowangkeji.top

PHP:  require "file.php";  或 use App\Service;
来源：http://jll.cdnleiting.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://mkx.xuanzx.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hgp.haohaochexian.top

Java: import java.util.List;
来源：http://orz.xinyue.icu

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://cga.nanxuanxn.top

Ruby: require "json"; require_relative "./util"
来源：http://ntu.wangdashe.top

C#:   using System.Text;
来源：http://mkv.jiagoushi.top

[C12] 立即执行函数 IIFE
来源：http://rsr.ppjwa.cn

Py:   (lambda: print("run"))()
来源：http://ahb.xuanzx.com

PHP:  (function () { echo "run"; })();
来源：http://cjb.nanxuanxn.top

JS:   (() => { console.log("run"); })();
来源：http://rad.haohaochexian.top

TS:   (() => { console.log("run"); })();
来源：http://weo.wangdashe.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hjj.sxryk.cn

Go:   func() { fmt.Println("run") }()
来源：http://okq.pengpengdd.cyou

Ruby: -> { puts "run" }.call
来源：http://btg.zdbjq.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ydw.gzhubu.top

[C13] 类型声明 / 类型注解
来源：http://joq.jinghuilouyu.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mfv.havefunace.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://itc.jlsjyb.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://igb.wangdashe.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cqx.smart0.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://ner.guowangkeji.top

Go:   func add(a, b int) int
来源：http://tom.gzhubu.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://sjw.jqgufenzy.top

C#:   int Add(int a, int b) => a + b;
来源：http://kmh.shanyushiyangtech.top

[C14] 泛型函数
来源：http://xyh.gaohongyu789.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://eou.nanxuanxn.top

PHP:  // 无泛型
来源：http://tmc.9152youxi.cn

JS:   // 无泛型
来源：http://tmd.c1oappe.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://oqj.hysaishi.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://pvu.zhengqikj.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wvd.vqdsnc.cn

Ruby: # 无泛型
来源：http://lzr.mhx1999.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://jne.ctjpmb.com

[C15] 解构 / 展开参数
来源：http://yvm.zhoulong.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xmi.c1oappe.top

PHP:  [$a, $b] = $pair;
来源：http://dho.birdmap.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://gnz.yanxiufei.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://rcp.ivvv.top

Java: // 无解构
来源：http://nyn.chenlongwang.top

Go:   // 无解构
来源：http://sfi.daxiang520.top

Ruby: a, b = pair
来源：http://cdb.sjlbkw.cn

C#:   var (a, b) = pair;
来源：http://dhd.yj20258.top

[C16] 函数 / 方法重载
来源：http://kaq.sxryk.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vxl.epnwcf.com

PHP:  // 无重载
来源：http://evn.yuxming.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://cin.cdnleiting.top

TS:   // 用联合类型或重载签名声明
来源：http://gsf.tian-w.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://szb.yj202588.top

Go:   // 无重载：用不同函数名
来源：http://nva.yonumen.top

Ruby: # 无重载：靠动态参数
来源：http://sur.dianchejie.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://cap.fehbvm.com

================================================================================
来源：http://fhl.fengsongda.top

D. 数组 / 列表 / 集合
来源：http://ehk.shangyingyoupin.top

================================================================================
来源：http://efm.snrcjt.cn

[D01] 创建数组 / 列表
来源：http://lsg.jinqigufen.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://imv.fanxiaobao.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://zyb.hesvh.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://pap.jyoumei.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ynx.nanxuanxn.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://tgx.hfpthk.cn

Go:   arr := []int{1, 2, 3}
来源：http://lbl.chenlongwang.top

Ruby: arr = [1, 2, 3]
来源：http://ton.meibo888.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://gfe.shuidangran.top

[D02] 追加元素到末尾
来源：http://wel.xingfuxueyuan.xyz

Py:   arr.append(4); arr.extend([5, 6])
来源：http://zdx.tianlin.xyz

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://pyi.fehbvm.com

JS:   arr.push(4);
来源：http://cxz.jinyuanbaomall.cn

TS:   arr.push(4);
来源：http://ceb.xuetiantiany.cn

Java: list.add(4);
来源：http://zps.jinqigfzy.top

Go:   arr = append(arr, 4)
来源：http://jcv.tanke756.top

Ruby: arr << 4; arr.push(5)
来源：http://ffk.wangdashe.top

C#:   list.Add(4);
来源：http://nmu.yanxiufei.cn

[D03] 在指定位置插入元素
来源：http://kvq.chenjidiqi.icu

Py:   arr.insert(0, 0)
来源：http://ooh.guannengcc.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://zfv.zhaomingkeji.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://oaq.jinyuanbaomall.cn

TS:   arr.splice(0, 0, 0);
来源：http://idc.jyoumei.cn

Java: list.add(0, 0);
来源：http://nuf.redwolf501.top

Go:   arr = append([]int{0}, arr...)
来源：http://dcv.zhixingplan.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://sgw.jinghuilouyu.cn

C#:   list.Insert(0, 0);
来源：http://njr.jiagoushi.top

[D04] 删除元素
来源：http://khe.xylfe.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://bqj.hcnkem.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://cze.zdbjq.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mti.guannengcc.top

TS:   arr.splice(0, 1);
来源：http://syf.yfazqb.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ibg.zhaomingkeji.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://qye.jinyuanbaomall.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://fts.yj20258.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://rmt.yanxiufei.cn

[D05] 访问与修改元素
来源：http://mkv.snrcjt.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://lgy.yongpay.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wyq.zycfv.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://jvw.snrcjt.cn

TS:   arr[0]; arr.at(-1);
来源：http://cjm.gaohongyu789.top

Java: list.get(0); list.set(0, 9);
来源：http://dxt.sjlbkw.cn

Go:   arr[0]; arr[0] = 9
来源：http://lgq.chenjidiqi.icu

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mrb.guowangkeji.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://obd.jianghu66.top

[D06] 数组长度
来源：http://gyu.hnqzz.top


<!-- 参考信息 -->