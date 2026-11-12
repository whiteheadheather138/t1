代发 wailian999

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://akg.cqqwz.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hui.jinqigfzy.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://edt.xziqi.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://otq.jianghu66.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://lrz.hesvh.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ung.52xcode.cn

[B07] while 循环
来源：http://bpl.tarul.cn

Py:   while i < 10: i += 1
来源：http://nhd.feifeiyinyue.top

PHP:  while ($i < 10) { $i++; }
来源：http://xqw.fktsv.cn

JS:   while (i < 10) { i++; }
来源：http://wjw.zdqjudy.top

TS:   while (i < 10) { i++; }
来源：http://lsr.gzhubu.top

Java: while (i < 10) { i++; }
来源：http://juw.daria6918.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://dmn.jinyuanbaomall.cn

Ruby: while i < 10; i += 1; end
来源：http://jik.hongshengwenyu.top

C#:   while (i < 10) { i++; }
来源：http://moh.sysykeji.top

[B08] do-while（至少执行一次）
来源：http://ayo.ywan-chungtsiang.top

Py:   # 无 do-while：用 while True + break
来源：http://eze.chenjidiqi.icu

PHP:  do { $i++; } while ($i < 10);
来源：http://whp.sweek.top

JS:   do { i++; } while (i < 10);
来源：http://ynb.cdnleiting.top

TS:   do { i++; } while (i < 10);
来源：http://ala.ctjpmb.com

Java: do { i++; } while (i < 10);
来源：http://zus.vqdsnc.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://nmt.wangdashe.top

Ruby: begin; i += 1; end while i < 10
来源：http://owp.tanke756.top

C#:   do { i++; } while (i < 10);
来源：http://bru.epnwcf.com

[B09] break 与 continue
来源：http://lvz.shzxlz.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://kax.ybcxt.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wsv.ehwqpu.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oet.fktsv.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wdz.yj20258.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://acp.xziqi.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://jxq.sweek.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xkq.hesvh.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qcr.hnxiangtu.top

[B10] 遍历同时拿索引
来源：http://zml.jinyuanbaomall.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://rzj.meibo888.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://jnx.jinyuanbaomall.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://zdp.xuetiantiany.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://njx.pycfn.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baf.xinyue.icu

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://kcj.daxiang520.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://nyt.uphjek.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://nri.dashuyun.cn

[B11] 生成数字序列 / 区间
来源：http://sxc.aizwys.cn

Py:   list(range(0, 10, 2))
来源：http://pzp.gaohongyu789.top

PHP:  range(0, 10, 2);
来源：http://kfe.zhixingplan.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sjw.xziqi.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qvv.zycfv.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://oje.yj20258888.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hot.shuidangran.top

Ruby: (0...10).step(2).to_a
来源：http://abh.uphjek.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://clt.zhixingplan.top

[B12] 跳出多层循环
来源：http://pya.sysykeji.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://hly.xuetiantiany.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://cdj.jinqigufen.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://rup.xuetiantiany.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ive.hcnkem.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://fzn.havefunace.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://dcj.vqdsnc.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://cai.nwbrower.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://kbg.cqqwz.cn

[B13] 判断是否为数字
来源：http://jqq.zhiwuduotai.top

Py:   isinstance(x, (int, float))
来源：http://hhh.jinghuilouyu.cn

PHP:  is_numeric($x)
来源：http://trn.jinyuanbaomall.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://swu.jlsjyb.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ryb.daxiang520.top

Java: x instanceof Number
来源：http://jeh.shanyushiyangtech.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://uhr.chenjidiqi.icu

Ruby: x.is_a?(Numeric)
来源：http://hzq.zdbjq.cn

C#:   x is int or double or decimal
来源：http://zyd.shzxlz.cn

[B14] 判断值是否在集合内
来源：http://pzj.pycfn.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ffw.tian-w.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://jcd.hesvh.cn

JS:   [1, 2, 3].includes(x)
来源：http://qcv.jqgufenzy.top

TS:   [1, 2, 3].includes(x)
来源：http://kmb.ybcxt.top

Java: List.of(1, 2, 3).contains(x)
来源：http://zve.9152youxi.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://jvi.zhongyouzk.top

Ruby: [1, 2, 3].include?(x)
来源：http://skx.jyoumei.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ihl.epnwcf.com

[B15] 布尔运算与取反
来源：http://rmd.haohaochexian.top

Py:   a and b or not c
来源：http://tkc.tianlin.xyz

PHP:  $a && $b || !$c
来源：http://jtq.daxiang520.top

JS:   a && b || !c
来源：http://kiu.kuanghao11.cn

TS:   a && b || !c
来源：http://plw.jyoumei.cn

Java: a && b || !c
来源：http://bgb.fehbvm.com

Go:   a && b || !c
来源：http://hjp.jiagoushi.top

Ruby: a && b || !c
来源：http://ztc.vehdjk.com

C#:   a && b || !c
来源：http://vgw.gogol.net.cn

[B16] 卫语句：不满足条件提前返回
来源：http://yst.ybcxt.top

Py:   if not data: return
来源：http://yec.nwbrower.top

PHP:  if (!$data) { return; }
来源：http://asy.shzxlz.cn

JS:   if (!data) return;
来源：http://tfh.ppjwa.cn

TS:   if (!data) return;
来源：http://pgu.yj202588.top

Java: if (data == null) return;
来源：http://dxj.wangshuangyany.cn

Go:   if data == nil { return }
来源：http://rua.bjfxy.top

Ruby: return if data.nil?
来源：http://jpe.snrcjt.cn

C#:   if (data == null) return;
来源：http://mxw.xinyue.icu

================================================================================
来源：http://zip.haohaochexian.top

C. 函数与作用域
来源：http://dsy.zhaomingkeji.xyz

================================================================================
来源：http://gtm.ppjwa.cn

[C01] 定义函数
来源：http://sbu.uphjek.com

Py:   def add(a, b): return a + b
来源：http://tcp.sjlbkw.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nqx.zhongyouzk.top

JS:   function add(a, b) { return a + b; }
来源：http://mtz.iojbl.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qwe.yonumen.top

Java: static int add(int a, int b) { return a + b; }
来源：http://oxz.xuetiantiany.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ofr.fktsv.cn

Ruby: def add(a, b); a + b; end
来源：http://fqf.zhoulong.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://qpy.0kj1m.cn

[C02] 默认参数
来源：http://kiw.kuanghao11.cn

Py:   def greet(name="World"): return name
来源：http://jdq.52xcode.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://byh.snrcjt.cn

JS:   function greet(name = "World") { return name; }
来源：http://pzp.feifeiyinyue.top

TS:   function greet(name: string = "World") { return name; }
来源：http://jms.nanxinkj.top

Java: // 无默认参数：方法重载或 Optional
来源：http://xuz.redwolf501.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://zpc.zhixingplan.top

Ruby: def greet(name = "World") = name
来源：http://nvy.zdqjudy.top

C#:   string Greet(string name = "World") => name;
来源：http://cym.fengsongda.top

[C03] 可变参数
来源：http://tpf.shuidangran.top

Py:   def total(*args): return sum(args)
来源：http://aqp.xuetiantiany.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mml.jlsjyb.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ryu.jlsjyb.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://loi.iojbl.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://plq.bjfxy.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://pns.jlsjyb.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ltv.zhoulong.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://nsv.gaohongyu789.top

[C04] 命名参数 / 关键字参数
来源：http://iil.gzhubu.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://tfg.bjfxy.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://zft.fehbvm.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://tgi.xziqi.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xkq.haohaochexian.top

Java: // 无：用 Builder 模式或 record
来源：http://qdc.haohaochexian.top

Go:   // 无：用配置结构体参数
来源：http://bgf.hcnkem.com

Ruby: f(a: 1, b: 2)
来源：http://pkm.zdbjq.cn

C#:   f(a: 1, b: 2)
来源：http://yek.zdqjudy.top

[C05] 返回多个值
来源：http://ych.yueranfly.top

Py:   return a, b
来源：http://mln.epnwcf.com

PHP:  return [$a, $b];
来源：http://lwi.wangdashe.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://ihi.iojbl.cn

TS:   return { a, b };
来源：http://yub.guannengcc.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mdk.shzxlz.cn

Go:   return a, b
来源：http://qnv.shanyushiyangtech.top

Ruby: return a, b
来源：http://ngp.xingfuxueyuan.xyz

C#:   return (a, b);              // ValueTuple
来源：http://lxu.fehbvm.com

[C06] 匿名函数 / lambda
来源：http://luq.0kj1m.cn

Py:   square = lambda x: x * x
来源：http://rom.zhiwuduotai.top

PHP:  $square = fn($x) => $x * $x;
来源：http://pft.xingfuxueyuan.xyz

JS:   const square = x => x * x;
来源：http://haw.xuanzx.com

TS:   const square = (x: number): number => x * x;
来源：http://ojl.yonumen.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://gkg.yj20258.top

Go:   sq := func(x int) int { return x * x }
来源：http://pch.hywenlv.cn

Ruby: square = ->(x) { x * x }
来源：http://mvs.jinqigfzy.top

C#:   Func<int, int> square = x => x * x;
来源：http://pue.hammf.cn

[C07] 把函数作为参数传入
来源：http://jdx.yj20258888.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://sgv.hnxiangtu.top

PHP:  array_map("strtoupper", $arr);
来源：http://uon.jinyuanbaomall.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://zwe.nanxuanxn.top

TS:   arr.map(String)
来源：http://amf.zhoulong.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://itl.daria6918.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://sxv.fktsv.cn

Ruby: arr.map(&:upcase)
来源：http://ltm.zdqjudy.top

C#:   arr.Select(s => s.ToUpper())
来源：http://alt.birdmap.top

[C08] 闭包
来源：http://bnd.kuanghao11.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://xro.meibo888.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://qms.chenlongwang.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://skg.tian-w.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://oxx.zhaomingkeji.xyz

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mqm.yanxiufei.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://xwa.meibo888.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://vag.shanyushiyangkeji.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ogk.uphjek.com

[C09] 递归
来源：http://bjc.cheryme.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://gdk.xuetiantiany.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ipd.yanxiufei.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lcw.zhiwuduotai.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lik.gaohongyu789.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://moz.epnwcf.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ore.hcnkem.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://svw.fengsongda.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://bbk.snrcjt.cn

[C10] 变量作用域
来源：http://buc.yanxiufei.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hub.xylfe.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://uge.smart0.xyz

JS:   let/const 块级作用域，var 函数级作用域
来源：http://psy.yangfankeji.com

TS:   同 JS
来源：http://kjc.haohaochexian.top

Java: 方法内为块级作用域
来源：http://pvs.xuetiantiany.cn

Go:   花括号块级作用域
来源：http://tdi.jqgfzy.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ysi.yj202588.top

C#:   块级作用域
来源：http://aav.xylfe.cn

[C11] 模块导入与导出
来源：http://yrg.xingfuxueyuan.xyz

Py:   from module import func
来源：http://kir.tarul.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://uqt.ybcxt.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://toh.hongshengwenyu.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://huk.feifeiyinyue.top

Java: import java.util.List;
来源：http://gvo.gogol.net.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://xmk.chenjidiqi.icu

Ruby: require "json"; require_relative "./util"
来源：http://osa.ywan-chungtsiang.top

C#:   using System.Text;
来源：http://rew.vehdjk.com

[C12] 立即执行函数 IIFE
来源：http://kbz.tarul.cn

Py:   (lambda: print("run"))()
来源：http://rrq.jlsjyb.cn

PHP:  (function () { echo "run"; })();
来源：http://twv.snrcjt.cn

JS:   (() => { console.log("run"); })();
来源：http://hsw.9152youxi.cn

TS:   (() => { console.log("run"); })();
来源：http://peg.9152youxi.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://fca.mhx1999.top

Go:   func() { fmt.Println("run") }()
来源：http://sch.ehwqpu.com

Ruby: -> { puts "run" }.call
来源：http://jkk.yj20258.top

C#:   // 无 IIFE：用静态构造函数
来源：http://goq.guowangkeji.top

[C13] 类型声明 / 类型注解
来源：http://iok.birdmap.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://jus.jiagoushi.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mqx.hysaishi.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://vot.birdmap.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vau.yonumen.top

Java: int add(int a, int b) { return a + b; }
来源：http://pan.52xcode.cn

Go:   func add(a, b int) int
来源：http://skt.ybcxt.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://val.daria6918.cn

C#:   int Add(int a, int b) => a + b;
来源：http://myi.zhaomingkeji.xyz

[C14] 泛型函数
来源：http://eqt.ehwqpu.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://alk.sjlbkw.cn

PHP:  // 无泛型
来源：http://kqk.xuanzx.com

JS:   // 无泛型
来源：http://awh.zhijiandao.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://tbc.yonumen.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://kwe.chenlongwang.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://lwv.sweek.top

Ruby: # 无泛型
来源：http://dxe.nwbrower.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://meb.pengpengdd.cyou

[C15] 解构 / 展开参数
来源：http://hyd.jyoumei.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://nyv.zdqjudy.top

PHP:  [$a, $b] = $pair;
来源：http://tpd.kuanghao11.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://fdr.jinqigufen.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ulk.jqgufenzy.top

Java: // 无解构
来源：http://aoy.nanxuanxn.top

Go:   // 无解构
来源：http://vum.jqgufenzy.top

Ruby: a, b = pair
来源：http://vea.zhongyouzk.top

C#:   var (a, b) = pair;
来源：http://tai.xylfe.cn

[C16] 函数 / 方法重载
来源：http://idz.daxiang520.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ogy.guowangkeji.top

PHP:  // 无重载
来源：http://vsa.jinqigfzy.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://rkf.meibo888.top

TS:   // 用联合类型或重载签名声明
来源：http://kvd.zhijiandao.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://mds.snrcjt.cn

Go:   // 无重载：用不同函数名
来源：http://nfy.chenlongwang.top

Ruby: # 无重载：靠动态参数
来源：http://fev.tarul.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://wxs.daria6918.cn

================================================================================
来源：http://sor.tarul.cn

D. 数组 / 列表 / 集合
来源：http://fcr.sufxvd.cn

================================================================================
来源：http://hya.hnxiangtu.top

[D01] 创建数组 / 列表
来源：http://wey.fengsongda.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://dog.ydzc1.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://cep.fengsongda.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mqo.yj20258888.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://ffa.redwolf501.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://fxw.zdbjq.cn

Go:   arr := []int{1, 2, 3}
来源：http://dmx.jlsjyb.cn

Ruby: arr = [1, 2, 3]
来源：http://pni.snrcjt.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://qre.cucudq.cn

[D02] 追加元素到末尾
来源：http://xns.jianghu66.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://nrb.havefunace.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://kxw.yj20258.top

JS:   arr.push(4);
来源：http://uze.yuxming.cn

TS:   arr.push(4);
来源：http://cdj.zhijiandao.cn

Java: list.add(4);
来源：http://iwq.hnxiangtu.top

Go:   arr = append(arr, 4)
来源：http://wyx.pengpengdd.cyou

Ruby: arr << 4; arr.push(5)
来源：http://uet.haohaochexian.top

C#:   list.Add(4);
来源：http://crd.jqgfzy.top

[D03] 在指定位置插入元素
来源：http://koo.vqdsnc.cn

Py:   arr.insert(0, 0)
来源：http://pjl.zhiwuduotai.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ipa.yvedp.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://lay.gotoacloud.top

TS:   arr.splice(0, 0, 0);
来源：http://dvu.iojbl.cn

Java: list.add(0, 0);
来源：http://fci.gzhubu.top

Go:   arr = append([]int{0}, arr...)
来源：http://sgp.hammf.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://imj.gaohongyu789.top

C#:   list.Insert(0, 0);
来源：http://jbw.nanxuanxn.top

[D04] 删除元素
来源：http://tfh.jinqigfzy.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hsj.redwolf501.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://spl.ivvv.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xnq.pengpengdd.cyou

TS:   arr.splice(0, 1);
来源：http://nld.meibo888.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://giz.svipenyu.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://fxj.shzxlz.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://xxd.bbcook.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://psx.zhixingplan.top

[D05] 访问与修改元素
来源：http://zge.hysaishi.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://uue.zhengqikj.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://gei.aizwys.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://oxs.daria6918.cn

TS:   arr[0]; arr.at(-1);
来源：http://lsz.redwolf501.top

Java: list.get(0); list.set(0, 9);
来源：http://jqp.vqdsnc.cn

Go:   arr[0]; arr[0] = 9
来源：http://rol.ydjk.org.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://eha.cqqwz.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://enu.jqgfzy.top

[D06] 数组长度
来源：http://bgk.guannengcc.top

Py:   len(arr)
来源：http://ymb.cdnleiting.top

PHP:  count($arr);
来源：http://qaz.jinyuanbaomall.cn

JS:   arr.length
来源：http://esi.birdmap.top

TS:   arr.length
来源：http://jqh.dashuyun.cn

Java: list.size();
来源：http://tgw.shuidangran.top

Go:   len(arr)
来源：http://ibb.iojbl.cn

Ruby: arr.length; arr.size
来源：http://qck.zdqjudy.top

C#:   list.Count;
来源：http://zmn.zhengqikj.top


<!-- 参考信息 -->