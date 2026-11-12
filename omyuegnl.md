代发 wailian999

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pao.9152youxi.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tjq.pengpengdd.cyou

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ltj.hnxiangtu.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ltj.yj20258.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://afo.birdmap.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://cuj.yj20258888.top

[B07] while 循环
来源：http://oqt.nanxuanxn.top

Py:   while i < 10: i += 1
来源：http://gcc.zycfv.cn

PHP:  while ($i < 10) { $i++; }
来源：http://leh.shzxlz.cn

JS:   while (i < 10) { i++; }
来源：http://mkx.yj20258.top

TS:   while (i < 10) { i++; }
来源：http://cfj.aibaodan.cn

Java: while (i < 10) { i++; }
来源：http://inj.smart0.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://kwg.hcnkem.com

Ruby: while i < 10; i += 1; end
来源：http://pzx.xuanzx.com

C#:   while (i < 10) { i++; }
来源：http://nph.zhongyouzk.top

[B08] do-while（至少执行一次）
来源：http://rap.zhongyouzk.top

Py:   # 无 do-while：用 while True + break
来源：http://lzd.ppjwa.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://pjt.yangfankeji.com

JS:   do { i++; } while (i < 10);
来源：http://dde.quarkkingdee.top

TS:   do { i++; } while (i < 10);
来源：http://mnu.0kj1m.cn

Java: do { i++; } while (i < 10);
来源：http://jau.hfpthk.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://fnu.haohaochexian.top

Ruby: begin; i += 1; end while i < 10
来源：http://skj.zhixingplan.top

C#:   do { i++; } while (i < 10);
来源：http://rdk.dianchejie.cn

[B09] break 与 continue
来源：http://zwn.quarkkingdee.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://rqf.cqqwz.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://enc.tian-w.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://brb.jinghuilouyu.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nga.jiagoushi.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gtw.aizwys.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://dsb.zycfv.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://jta.meibo888.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tiv.fktsv.cn

[B10] 遍历同时拿索引
来源：http://pbu.nanxuanxn.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hbs.chenlongwang.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://oya.wangdashe.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mcg.chenlongwang.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://dyv.hnqzz.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://qud.fehbvm.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://iqk.zhongyouzk.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://knl.guowangkeji.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ncn.jyoumei.cn

[B11] 生成数字序列 / 区间
来源：http://llq.sufxvd.cn

Py:   list(range(0, 10, 2))
来源：http://jkl.jinqigfzy.top

PHP:  range(0, 10, 2);
来源：http://gkf.guowangkeji.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gzz.yueranfly.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ali.jiagoushi.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://kcu.zhengqikj.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hxo.fanxiaobao.xyz

Ruby: (0...10).step(2).to_a
来源：http://pdm.meibo888.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://cmk.tanke756.top

[B12] 跳出多层循环
来源：http://hmw.52xcode.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://jmk.hongshengwenyu.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://hsr.snrcjt.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://utv.jlsjyb.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://nwn.daxiang520.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://aho.tanke756.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://qtl.jinqigfzy.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://eyn.jinqigufen.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://fic.zycfv.cn

[B13] 判断是否为数字
来源：http://boa.cheryme.top

Py:   isinstance(x, (int, float))
来源：http://ftn.chenlongwang.top

PHP:  is_numeric($x)
来源：http://jjs.tian-w.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tqz.yonumen.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ajo.zhongyouzk.top

Java: x instanceof Number
来源：http://nye.chenjidiqi.icu

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://flk.iojbl.cn

Ruby: x.is_a?(Numeric)
来源：http://afk.wangdashe.top

C#:   x is int or double or decimal
来源：http://kwh.jinqigufen.top

[B14] 判断值是否在集合内
来源：http://ydl.uphjek.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://nxl.shuidangran.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://roc.jinyuanbaomall.cn

JS:   [1, 2, 3].includes(x)
来源：http://txh.ybcxt.top

TS:   [1, 2, 3].includes(x)
来源：http://vwv.jianghu66.top

Java: List.of(1, 2, 3).contains(x)
来源：http://bzj.yj20258.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ice.gogol.net.cn

Ruby: [1, 2, 3].include?(x)
来源：http://dpu.wangshuangyany.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://lmq.yfazqb.com

[B15] 布尔运算与取反
来源：http://prz.jianghu66.top

Py:   a and b or not c
来源：http://qbo.ppjwa.cn

PHP:  $a && $b || !$c
来源：http://ldx.bbcook.cn

JS:   a && b || !c
来源：http://lwu.chenlongwang.top

TS:   a && b || !c
来源：http://fei.sysykeji.top

Java: a && b || !c
来源：http://dfg.yongpay.top

Go:   a && b || !c
来源：http://fsv.hywenlv.cn

Ruby: a && b || !c
来源：http://lsi.cashguo.top

C#:   a && b || !c
来源：http://oqr.aibaodan.cn

[B16] 卫语句：不满足条件提前返回
来源：http://tut.xinyue.icu

Py:   if not data: return
来源：http://vcy.wangdashe.top

PHP:  if (!$data) { return; }
来源：http://okc.haohaochexian.top

JS:   if (!data) return;
来源：http://vwl.hnqzz.top

TS:   if (!data) return;
来源：http://yfv.jinyuanbaomall.cn

Java: if (data == null) return;
来源：http://jwx.nanxinkj.top

Go:   if data == nil { return }
来源：http://yvc.hnqzz.top

Ruby: return if data.nil?
来源：http://odm.cqqwz.cn

C#:   if (data == null) return;
来源：http://jfq.aibaodan.cn

================================================================================
来源：http://xaz.fengsongda.top

C. 函数与作用域
来源：http://ssm.kuanghao11.cn

================================================================================
来源：http://nbr.gogol.net.cn

[C01] 定义函数
来源：http://wxk.fehbvm.com

Py:   def add(a, b): return a + b
来源：http://xnn.snrcjt.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pdm.chenzaomai.com

JS:   function add(a, b) { return a + b; }
来源：http://bxe.sxryk.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://uob.hfpthk.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://vqh.yvedp.cn

Go:   func add(a, b int) int { return a + b }
来源：http://kpy.pengpengdd.cyou

Ruby: def add(a, b); a + b; end
来源：http://uoi.cucudq.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://kgr.ehwqpu.com

[C02] 默认参数
来源：http://xwi.hysaishi.cn

Py:   def greet(name="World"): return name
来源：http://nef.shanyushiyangtech.top

PHP:  function greet($name = "World") { return $name; }
来源：http://xux.vehdjk.com

JS:   function greet(name = "World") { return name; }
来源：http://lkm.c1oappe.top

TS:   function greet(name: string = "World") { return name; }
来源：http://qsi.smart0.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://ecf.tarul.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://bqi.tianlin.xyz

Ruby: def greet(name = "World") = name
来源：http://llu.hammf.cn

C#:   string Greet(string name = "World") => name;
来源：http://rrl.bjfxy.top

[C03] 可变参数
来源：http://ilf.svipenyu.cn

Py:   def total(*args): return sum(args)
来源：http://iro.wangshuangyany.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://jfu.jianghu66.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://qtb.zhoulong.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://yyj.zhixingplan.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://buo.chenlongwang.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://fxo.quarkkingdee.top

Ruby: def total(*nums); nums.sum; end
来源：http://atf.yonumen.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ush.hesvh.cn

[C04] 命名参数 / 关键字参数
来源：http://ytd.zdbjq.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://vbo.zdqjudy.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wnw.bjfxy.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://pkg.hesvh.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ekz.nanxuanxn.top

Java: // 无：用 Builder 模式或 record
来源：http://iym.yuanzhike.top

Go:   // 无：用配置结构体参数
来源：http://vbg.fengsongda.top

Ruby: f(a: 1, b: 2)
来源：http://clw.fzhhl.top

C#:   f(a: 1, b: 2)
来源：http://ssf.nanxuanxn.top

[C05] 返回多个值
来源：http://ahq.hnxiangtu.top

Py:   return a, b
来源：http://qmt.dianchejie.cn

PHP:  return [$a, $b];
来源：http://vie.xuetiantiany.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://fun.shangyingyoupin.top

TS:   return { a, b };
来源：http://utq.c1oappe.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://kqu.gaohongyu789.top

Go:   return a, b
来源：http://yfb.hammf.cn

Ruby: return a, b
来源：http://kbf.c1oappe.top

C#:   return (a, b);              // ValueTuple
来源：http://mzg.jinghuilouyu.cn

[C06] 匿名函数 / lambda
来源：http://geb.gogol.net.cn

Py:   square = lambda x: x * x
来源：http://mez.zhiwuduotai.top

PHP:  $square = fn($x) => $x * $x;
来源：http://ewc.xuanzx.com

JS:   const square = x => x * x;
来源：http://xfk.snrcjt.cn

TS:   const square = (x: number): number => x * x;
来源：http://wrr.jqgfzy.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wgn.hcnkem.com

Go:   sq := func(x int) int { return x * x }
来源：http://bua.bjfxy.top

Ruby: square = ->(x) { x * x }
来源：http://rgz.yongpay.top

C#:   Func<int, int> square = x => x * x;
来源：http://ajt.jlsjyb.cn

[C07] 把函数作为参数传入
来源：http://vkf.zdbjq.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://tor.yj202588.top

PHP:  array_map("strtoupper", $arr);
来源：http://wyb.ctjpmb.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://vmg.vqdsnc.cn

TS:   arr.map(String)
来源：http://sui.wangdashe.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://usx.c1oappe.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://gbi.fktsv.cn

Ruby: arr.map(&:upcase)
来源：http://jyf.zycfv.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://rwm.ydjk.org.cn

[C08] 闭包
来源：http://xkd.meibo888.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://vdx.sysykeji.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://jol.guannengcc.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wio.chenlongwang.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://eny.yj20258.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://svl.ywan-chungtsiang.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://okv.iojbl.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://cdf.yueranfly.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://rzw.9152youxi.cn

[C09] 递归
来源：http://sih.jqgufenzy.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://nkq.shanyushiyangkeji.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ugf.nanxuanxn.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mdo.tarul.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://eak.fehbvm.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hiy.hywenlv.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://fia.pycfn.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://apy.zycfv.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://giu.epnwcf.com

[C10] 变量作用域
来源：http://jek.aibaodan.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://rxr.cashguo.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://qcm.wangshuangyany.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://pfn.yueranfly.top

TS:   同 JS
来源：http://nnh.yfazqb.com

Java: 方法内为块级作用域
来源：http://eme.jiagoushi.top

Go:   花括号块级作用域
来源：http://has.fanxiaobao.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://vdk.nanxuanxn.top

C#:   块级作用域
来源：http://udz.zhongyouzk.top

[C11] 模块导入与导出
来源：http://zgo.shangyingyoupin.top

Py:   from module import func
来源：http://fjq.guowangkeji.top

PHP:  require "file.php";  或 use App\Service;
来源：http://noi.jinqigufen.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://mgh.dashuyun.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ifc.yuxming.cn

Java: import java.util.List;
来源：http://tvh.ehwqpu.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://tmc.zhixingplan.top

Ruby: require "json"; require_relative "./util"
来源：http://xjf.pycfn.com

C#:   using System.Text;
来源：http://lcl.yangfankeji.com

[C12] 立即执行函数 IIFE
来源：http://riq.svipenyu.cn

Py:   (lambda: print("run"))()
来源：http://rpt.zdbjq.cn

PHP:  (function () { echo "run"; })();
来源：http://ici.chenjidiqi.icu

JS:   (() => { console.log("run"); })();
来源：http://dyj.haohaochexian.top

TS:   (() => { console.log("run"); })();
来源：http://chw.feifeiyinyue.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://dft.ivvv.top

Go:   func() { fmt.Println("run") }()
来源：http://hyw.yfazqb.com

Ruby: -> { puts "run" }.call
来源：http://kfi.yj20258.top

C#:   // 无 IIFE：用静态构造函数
来源：http://vip.xinyue.icu

[C13] 类型声明 / 类型注解
来源：http://qkj.hnxiangtu.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://soz.yj20258888.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://szn.svipenyu.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ylo.shanyushiyangtech.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lus.wangshuangyany.cn

Java: int add(int a, int b) { return a + b; }
来源：http://wwi.hnqzz.top

Go:   func add(a, b int) int
来源：http://nff.hnxiangtu.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ikg.sweek.top

C#:   int Add(int a, int b) => a + b;
来源：http://atl.fehbvm.com

[C14] 泛型函数
来源：http://prx.fzhhl.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://jzb.mhx1999.top

PHP:  // 无泛型
来源：http://nra.shanyushiyangtech.top

JS:   // 无泛型
来源：http://bnw.iojbl.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://xql.fktsv.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://etj.jinqigufen.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mfr.shangyingyoupin.top

Ruby: # 无泛型
来源：http://ivj.tarul.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ohr.zhengqikj.top

[C15] 解构 / 展开参数
来源：http://ibh.zhongyouzk.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://nyc.fzhhl.top

PHP:  [$a, $b] = $pair;
来源：http://jwq.fzhhl.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://zjb.mhx1999.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://gfn.bbcook.cn

Java: // 无解构
来源：http://wmi.uphjek.com

Go:   // 无解构
来源：http://ehv.ctjpmb.com

Ruby: a, b = pair
来源：http://qkk.ywan-chungtsiang.top

C#:   var (a, b) = pair;
来源：http://xoh.jyoumei.cn

[C16] 函数 / 方法重载
来源：http://kck.fehbvm.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://pxy.daxiang520.top

PHP:  // 无重载
来源：http://ctj.52xcode.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://wnn.shanyushiyangkeji.top

TS:   // 用联合类型或重载签名声明
来源：http://zkd.gotoacloud.top

Java: void f(int a) {}  void f(String a) {}
来源：http://dch.cashguo.top

Go:   // 无重载：用不同函数名
来源：http://jmh.guannengcc.top

Ruby: # 无重载：靠动态参数
来源：http://icp.nanxuanxn.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://nbe.dashuyun.cn

================================================================================
来源：http://slo.daria6918.cn

D. 数组 / 列表 / 集合
来源：http://xhk.haohaochexian.top

================================================================================
来源：http://rij.aizwys.cn

[D01] 创建数组 / 列表
来源：http://rxt.epnwcf.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://zqz.jinyuanbaomall.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://jbo.jiagoushi.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://crf.jiagoushi.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://mre.svipenyu.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://spn.xziqi.cn

Go:   arr := []int{1, 2, 3}
来源：http://hoy.daxiang520.top

Ruby: arr = [1, 2, 3]
来源：http://kvq.chenzaomai.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ekh.jinqigufen.top

[D02] 追加元素到末尾
来源：http://jan.feifeiyinyue.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://exo.ydzc1.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://niq.hongshengwenyu.top

JS:   arr.push(4);
来源：http://udh.chenjidiqi.icu

TS:   arr.push(4);
来源：http://nsm.haohaochexian.top

Java: list.add(4);
来源：http://skp.hongshengwenyu.top

Go:   arr = append(arr, 4)
来源：http://fce.xuetiantiany.cn

Ruby: arr << 4; arr.push(5)
来源：http://grz.yonumen.top

C#:   list.Add(4);
来源：http://xiu.daxiang520.top

[D03] 在指定位置插入元素
来源：http://wys.nanxinkj.top

Py:   arr.insert(0, 0)
来源：http://fgy.svipenyu.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://jyz.chenlongwang.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://bir.cashguo.top

TS:   arr.splice(0, 0, 0);
来源：http://tsz.yj20258888.top

Java: list.add(0, 0);
来源：http://uax.xingfuxueyuan.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://isi.ywan-chungtsiang.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mfi.jlsjyb.cn

C#:   list.Insert(0, 0);
来源：http://stq.zhixingplan.top

[D04] 删除元素
来源：http://odh.tianlin.xyz

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://sej.yfazqb.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ttp.yj202588.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://bxm.svipenyu.cn

TS:   arr.splice(0, 1);
来源：http://fwk.yj202588.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://jkw.jyoumei.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://vvf.yongpay.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://fyu.xuetiantiany.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xvc.jinqigfzy.top

[D05] 访问与修改元素
来源：http://nya.sjlbkw.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://lsj.pycfn.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://qmt.nanxuanxn.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://jqn.jinqigufen.top

TS:   arr[0]; arr.at(-1);
来源：http://cjz.yj202588.top

Java: list.get(0); list.set(0, 9);
来源：http://wzg.ybcxt.top

Go:   arr[0]; arr[0] = 9
来源：http://cso.zhijiandao.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wgj.epnwcf.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mjb.dashuyun.cn

[D06] 数组长度
来源：http://oit.hesvh.cn

Py:   len(arr)
来源：http://qfk.jianghu66.top

PHP:  count($arr);
来源：http://rpw.pengpengdd.cyou

JS:   arr.length
来源：http://dyp.0kj1m.cn

TS:   arr.length
来源：http://zgr.gzhubu.top

Java: list.size();
来源：http://cii.yuxming.cn

Go:   len(arr)
来源：http://awu.xuetiantiany.cn

Ruby: arr.length; arr.size
来源：http://trb.iojbl.cn

C#:   list.Count;
来源：http://iae.vqdsnc.cn


<!-- 参考信息 -->