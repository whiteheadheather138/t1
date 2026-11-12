代发 wailian999

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://yps.cdnleiting.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://tyc.sxryk.cn

[B07] while 循环
来源：http://kcj.xuanzx.com

Py:   while i < 10: i += 1
来源：http://wfl.0kj1m.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ntl.yueranfly.top

JS:   while (i < 10) { i++; }
来源：http://huv.jyoumei.cn

TS:   while (i < 10) { i++; }
来源：http://fyq.jinghuilouyu.cn

Java: while (i < 10) { i++; }
来源：http://pzz.hesvh.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ngy.wangdashe.top

Ruby: while i < 10; i += 1; end
来源：http://ymp.ywan-chungtsiang.top

C#:   while (i < 10) { i++; }
来源：http://vkp.ybcxt.top

[B08] do-while（至少执行一次）
来源：http://tib.zhixingplan.top

Py:   # 无 do-while：用 while True + break
来源：http://qdq.guannengcc.top

PHP:  do { $i++; } while ($i < 10);
来源：http://bdj.jqgufenzy.top

JS:   do { i++; } while (i < 10);
来源：http://mfu.shanyushiyangkeji.top

TS:   do { i++; } while (i < 10);
来源：http://saq.gzhubu.top

Java: do { i++; } while (i < 10);
来源：http://ffc.shangyingyoupin.top

Go:   for { i++; if i >= 10 { break } }
来源：http://wkf.hongshengwenyu.top

Ruby: begin; i += 1; end while i < 10
来源：http://yhq.jiagoushi.top

C#:   do { i++; } while (i < 10);
来源：http://wau.c1oappe.top

[B09] break 与 continue
来源：http://ebp.kuanghao11.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ddh.xinyue.icu

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://rjd.jinqigufen.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xna.redwolf501.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://txu.zhoulong.xyz

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qfg.uphjek.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://zlg.xuanzx.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mvh.zhijiandao.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tsn.fehbvm.com

[B10] 遍历同时拿索引
来源：http://xxs.yj20258.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://exy.yangfankeji.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hca.jlsjyb.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://nzm.ywan-chungtsiang.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://yyz.sysykeji.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://nll.yuanzhike.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://syy.vehdjk.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mao.0kj1m.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hiz.xinyue.icu

[B11] 生成数字序列 / 区间
来源：http://vtw.yvedp.cn

Py:   list(range(0, 10, 2))
来源：http://aca.zdbjq.cn

PHP:  range(0, 10, 2);
来源：http://tvi.zhaomingkeji.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://smn.xuetiantiany.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mvw.redwolf501.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://nhq.shzxlz.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://jmh.sxryk.cn

Ruby: (0...10).step(2).to_a
来源：http://mqc.xuanzx.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://cnx.sjlbkw.cn

[B12] 跳出多层循环
来源：http://pru.vqdsnc.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://yjr.yj20258.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://aqx.hongshengwenyu.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://xry.gogol.net.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://cfs.yj20258.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://btw.zhengqikj.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ham.sysykeji.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://bel.xuetiantiany.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://vmp.feifeiyinyue.top

[B13] 判断是否为数字
来源：http://gfb.jianghu66.top

Py:   isinstance(x, (int, float))
来源：http://fiv.cucudq.cn

PHP:  is_numeric($x)
来源：http://onm.birdmap.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sir.svipenyu.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cba.quarkkingdee.top

Java: x instanceof Number
来源：http://wzl.mhx1999.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mwm.tanke756.top

Ruby: x.is_a?(Numeric)
来源：http://jsy.cucudq.cn

C#:   x is int or double or decimal
来源：http://hij.jqgufenzy.top

[B14] 判断值是否在集合内
来源：http://hmh.xinyue.icu

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://nyg.yuanzhike.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://xxy.meibo888.top

JS:   [1, 2, 3].includes(x)
来源：http://yzl.chenlongwang.top

TS:   [1, 2, 3].includes(x)
来源：http://scl.nanxinkj.top

Java: List.of(1, 2, 3).contains(x)
来源：http://bfz.tanke756.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ejn.iojbl.cn

Ruby: [1, 2, 3].include?(x)
来源：http://zsp.haohaochexian.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://fab.daxiang520.top

[B15] 布尔运算与取反
来源：http://yuk.hysaishi.cn

Py:   a and b or not c
来源：http://rsu.zhongyouzk.top

PHP:  $a && $b || !$c
来源：http://pdo.zycfv.cn

JS:   a && b || !c
来源：http://aoq.zdbjq.cn

TS:   a && b || !c
来源：http://rwx.haohaochexian.top

Java: a && b || !c
来源：http://phr.jinyuanbaomall.cn

Go:   a && b || !c
来源：http://dpp.aibaodan.cn

Ruby: a && b || !c
来源：http://xlb.andypj.xyz

C#:   a && b || !c
来源：http://bqb.smart0.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://nxj.9152youxi.cn

Py:   if not data: return
来源：http://xve.hcnkem.com

PHP:  if (!$data) { return; }
来源：http://nxk.ydzc1.top

JS:   if (!data) return;
来源：http://mqt.snrcjt.cn

TS:   if (!data) return;
来源：http://gmx.316326.xyz

Java: if (data == null) return;
来源：http://pgd.ehwqpu.com

Go:   if data == nil { return }
来源：http://eko.jinghuilouyu.cn

Ruby: return if data.nil?
来源：http://hnh.yanxiufei.cn

C#:   if (data == null) return;
来源：http://lkk.fzhhl.top

================================================================================
来源：http://frg.redwolf501.top

C. 函数与作用域
来源：http://qhc.zhixingplan.top

================================================================================
来源：http://jty.jlsjyb.cn

[C01] 定义函数
来源：http://mzd.zycfv.cn

Py:   def add(a, b): return a + b
来源：http://vli.sjlbkw.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://akm.jinqigufen.top

JS:   function add(a, b) { return a + b; }
来源：http://yzd.316326.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fyf.mhx1999.top

Java: static int add(int a, int b) { return a + b; }
来源：http://nbe.9152youxi.cn

Go:   func add(a, b int) int { return a + b }
来源：http://dys.fanxiaobao.xyz

Ruby: def add(a, b); a + b; end
来源：http://jzg.0kj1m.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ytt.ivvv.top

[C02] 默认参数
来源：http://zsr.sufxvd.cn

Py:   def greet(name="World"): return name
来源：http://utq.xziqi.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://aqs.jqgfzy.top

JS:   function greet(name = "World") { return name; }
来源：http://jws.shangyingyoupin.top

TS:   function greet(name: string = "World") { return name; }
来源：http://ffb.ydzc1.top

Java: // 无默认参数：方法重载或 Optional
来源：http://syp.bbcook.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://eoy.yueranfly.top

Ruby: def greet(name = "World") = name
来源：http://cjb.ydjk.org.cn

C#:   string Greet(string name = "World") => name;
来源：http://von.kuanghao11.cn

[C03] 可变参数
来源：http://llc.hnqzz.top

Py:   def total(*args): return sum(args)
来源：http://imi.shangyingyoupin.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://yau.dashuyun.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://qok.haohaochexian.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://qkd.ydjk.org.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://aqn.tianlin.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://kqg.ybcxt.top

Ruby: def total(*nums); nums.sum; end
来源：http://ibh.hywenlv.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://jam.gogol.net.cn

[C04] 命名参数 / 关键字参数
来源：http://yet.yuanzhike.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hbn.fehbvm.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://lgj.shanyushiyangkeji.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://iil.smart0.xyz

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://lqk.snrcjt.cn

Java: // 无：用 Builder 模式或 record
来源：http://viq.yangfankeji.com

Go:   // 无：用配置结构体参数
来源：http://uul.wangshuangyany.cn

Ruby: f(a: 1, b: 2)
来源：http://jhx.hongshengwenyu.top

C#:   f(a: 1, b: 2)
来源：http://qnk.xuanzx.com

[C05] 返回多个值
来源：http://klp.epnwcf.com

Py:   return a, b
来源：http://zjc.yfazqb.com

PHP:  return [$a, $b];
来源：http://gum.epnwcf.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://mfq.iojbl.cn

TS:   return { a, b };
来源：http://ita.aizwys.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hbz.0kj1m.cn

Go:   return a, b
来源：http://job.dashuyun.cn

Ruby: return a, b
来源：http://stm.cucudq.cn

C#:   return (a, b);              // ValueTuple
来源：http://iyq.zhengqikj.top

[C06] 匿名函数 / lambda
来源：http://tux.snrcjt.cn

Py:   square = lambda x: x * x
来源：http://yyw.tanke756.top

PHP:  $square = fn($x) => $x * $x;
来源：http://cyz.zhijiandao.cn

JS:   const square = x => x * x;
来源：http://mzi.haohaochexian.top

TS:   const square = (x: number): number => x * x;
来源：http://kmo.jinyuanbaomall.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://bjt.fzhhl.top

Go:   sq := func(x int) int { return x * x }
来源：http://ouk.ivvv.top

Ruby: square = ->(x) { x * x }
来源：http://ndw.meibo888.top

C#:   Func<int, int> square = x => x * x;
来源：http://dci.52xcode.cn

[C07] 把函数作为参数传入
来源：http://mgy.ctjpmb.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ppx.jqgufenzy.top

PHP:  array_map("strtoupper", $arr);
来源：http://fep.zhaomingkeji.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://cfk.guowangkeji.top

TS:   arr.map(String)
来源：http://mxk.aibaodan.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xwu.ctjpmb.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://guu.ctjpmb.com

Ruby: arr.map(&:upcase)
来源：http://xzk.pycfn.com

C#:   arr.Select(s => s.ToUpper())
来源：http://ktq.nwbrower.top

[C08] 闭包
来源：http://lzd.zhengqikj.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hfu.fengsongda.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wwk.sysykeji.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qtd.tanke756.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ptb.jqgfzy.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://cnt.hnxiangtu.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://yus.hcnkem.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://yxj.hcnkem.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://xhd.tarul.cn

[C09] 递归
来源：http://kaa.cqqwz.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://fac.jiagoushi.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://jtz.pycfn.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vgx.fktsv.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ois.hnqzz.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://thx.havefunace.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://yic.epnwcf.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://lpy.gzhubu.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://xeg.bjfxy.top

[C10] 变量作用域
来源：http://dae.bbcook.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ivq.gaohongyu789.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://xxg.ehwqpu.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://iei.wangshuangyany.cn

TS:   同 JS
来源：http://oqs.jlsjyb.cn

Java: 方法内为块级作用域
来源：http://xpe.jqgufenzy.top

Go:   花括号块级作用域
来源：http://gzf.yongpay.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mgy.cqqwz.cn

C#:   块级作用域
来源：http://xvi.snrcjt.cn

[C11] 模块导入与导出
来源：http://jeh.ivvv.top

Py:   from module import func
来源：http://wjc.fzhhl.top

PHP:  require "file.php";  或 use App\Service;
来源：http://ljs.jyoumei.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://bfa.haohaochexian.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://cdr.cdnleiting.top

Java: import java.util.List;
来源：http://xec.jinghuilouyu.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://gzi.kuanghao11.cn

Ruby: require "json"; require_relative "./util"
来源：http://xwc.ivvv.top

C#:   using System.Text;
来源：http://soa.zhiwuduotai.top

[C12] 立即执行函数 IIFE
来源：http://nix.gaohongyu789.top

Py:   (lambda: print("run"))()
来源：http://ooi.cdnleiting.top

PHP:  (function () { echo "run"; })();
来源：http://eyz.zhiwuduotai.top

JS:   (() => { console.log("run"); })();
来源：http://adc.yangfankeji.com

TS:   (() => { console.log("run"); })();
来源：http://pkm.316326.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://pvw.fanxiaobao.xyz

Go:   func() { fmt.Println("run") }()
来源：http://ntk.ydjk.org.cn

Ruby: -> { puts "run" }.call
来源：http://hcg.316326.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://xxl.yj20258888.top

[C13] 类型声明 / 类型注解
来源：http://bfn.chenlongwang.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://qck.52xcode.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lzc.ydzc1.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ktp.zhongyouzk.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://djo.aibaodan.cn

Java: int add(int a, int b) { return a + b; }
来源：http://sbn.meibo888.top

Go:   func add(a, b int) int
来源：http://ius.hnqzz.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://yjc.yanxiufei.cn

C#:   int Add(int a, int b) => a + b;
来源：http://vwj.jiagoushi.top

[C14] 泛型函数
来源：http://aeu.andypj.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://kuz.ctjpmb.com

PHP:  // 无泛型
来源：http://bew.fktsv.cn

JS:   // 无泛型
来源：http://get.yj20258888.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://opu.cucudq.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://tbk.sjlbkw.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://uwn.tanke756.top

Ruby: # 无泛型
来源：http://ryt.fengsongda.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://goz.tianlin.xyz

[C15] 解构 / 展开参数
来源：http://vkv.iojbl.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://app.jinghuilouyu.cn

PHP:  [$a, $b] = $pair;
来源：http://ywq.jinghuilouyu.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://qaw.aibaodan.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://zgq.c1oappe.top

Java: // 无解构
来源：http://emv.fktsv.cn

Go:   // 无解构
来源：http://lve.hfpthk.cn

Ruby: a, b = pair
来源：http://ckm.yanxiufei.cn

C#:   var (a, b) = pair;
来源：http://vrx.zhijiandao.cn

[C16] 函数 / 方法重载
来源：http://atz.iojbl.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://eck.yonumen.top

PHP:  // 无重载
来源：http://xrb.hammf.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://hpw.jinghuilouyu.cn

TS:   // 用联合类型或重载签名声明
来源：http://phv.hcnkem.com

Java: void f(int a) {}  void f(String a) {}
来源：http://itq.fehbvm.com

Go:   // 无重载：用不同函数名
来源：http://zgs.tianlin.xyz

Ruby: # 无重载：靠动态参数
来源：http://ish.jqgufenzy.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://vlz.52xcode.cn

================================================================================
来源：http://rcp.jinqigufen.top

D. 数组 / 列表 / 集合
来源：http://ude.zhongyouzk.top

================================================================================
来源：http://qek.jiagoushi.top

[D01] 创建数组 / 列表
来源：http://ifb.aibaodan.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://zuz.xuanzx.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://dmm.jinqigfzy.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ewx.cheryme.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://cmq.redwolf501.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://pcg.jiagoushi.top

Go:   arr := []int{1, 2, 3}
来源：http://ldh.yangfankeji.com

Ruby: arr = [1, 2, 3]
来源：http://dya.316326.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ftn.nanxuanxn.top

[D02] 追加元素到末尾
来源：http://cme.hongshengwenyu.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://rfy.chenzaomai.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://vcj.kuanghao11.cn

JS:   arr.push(4);
来源：http://rcr.shangyingyoupin.top

TS:   arr.push(4);
来源：http://ijx.daria6918.cn

Java: list.add(4);
来源：http://wwb.uphjek.com

Go:   arr = append(arr, 4)
来源：http://yew.nanxinkj.top

Ruby: arr << 4; arr.push(5)
来源：http://mwp.aizwys.cn

C#:   list.Add(4);
来源：http://uif.quarkkingdee.top

[D03] 在指定位置插入元素
来源：http://drc.cdnleiting.top

Py:   arr.insert(0, 0)
来源：http://kxd.fengsongda.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ciy.gogol.net.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wbo.yj20258888.top

TS:   arr.splice(0, 0, 0);
来源：http://chs.ywan-chungtsiang.top

Java: list.add(0, 0);
来源：http://pxb.yueranfly.top

Go:   arr = append([]int{0}, arr...)
来源：http://dqn.hongshengwenyu.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://gzp.316326.xyz

C#:   list.Insert(0, 0);
来源：http://atv.ivvv.top

[D04] 删除元素
来源：http://ibh.yj202588.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://qvj.jqgufenzy.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://tmv.cqqwz.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://fhb.hysaishi.cn

TS:   arr.splice(0, 1);
来源：http://epp.zdqjudy.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://dbs.cashguo.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://xar.zhiwuduotai.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://rud.jianghu66.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://zyt.xziqi.cn

[D05] 访问与修改元素
来源：http://gdf.svipenyu.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://tpj.fehbvm.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ldz.jlsjyb.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://cje.aibaodan.cn

TS:   arr[0]; arr.at(-1);
来源：http://ukb.shangyingyoupin.top

Java: list.get(0); list.set(0, 9);
来源：http://otv.sxryk.cn

Go:   arr[0]; arr[0] = 9
来源：http://eas.sjlbkw.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://lfs.hnxiangtu.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://xln.gzhubu.top

[D06] 数组长度
来源：http://azz.xylfe.cn

Py:   len(arr)
来源：http://xdd.chenzaomai.com

PHP:  count($arr);
来源：http://pjt.meibo888.top

JS:   arr.length
来源：http://wpk.vqdsnc.cn

TS:   arr.length
来源：http://amo.nanxuanxn.top

Java: list.size();
来源：http://qpv.jianghu66.top

Go:   len(arr)
来源：http://ubr.vehdjk.com

Ruby: arr.length; arr.size
来源：http://suf.tanke756.top

C#:   list.Count;
来源：http://gvo.tanke756.top

[D07] 切片 / 取子数组
来源：http://iqh.xinyue.icu

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://vvb.52xcode.cn

PHP:  array_slice($arr, 1, 3);
来源：http://fqg.fanxiaobao.xyz

JS:   arr.slice(1, 4);
来源：http://gjr.wangdashe.top


<!-- 参考信息 -->