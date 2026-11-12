代发 wailian999

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://utj.meibo888.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://zcq.daxiang520.top

[B07] while 循环
来源：http://azq.chenjidiqi.icu

Py:   while i < 10: i += 1
来源：http://kpt.zhijiandao.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ggx.zhengqikj.top

JS:   while (i < 10) { i++; }
来源：http://fkj.shanyushiyangtech.top

TS:   while (i < 10) { i++; }
来源：http://usw.chenzaomai.com

Java: while (i < 10) { i++; }
来源：http://xnz.ydzc1.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://xwn.nanxinkj.top

Ruby: while i < 10; i += 1; end
来源：http://xdb.sysykeji.top

C#:   while (i < 10) { i++; }
来源：http://ggg.yj202588.top

[B08] do-while（至少执行一次）
来源：http://myx.c1oappe.top

Py:   # 无 do-while：用 while True + break
来源：http://uxv.cqqwz.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://vqo.zhiwuduotai.top

JS:   do { i++; } while (i < 10);
来源：http://dnm.hnxiangtu.top

TS:   do { i++; } while (i < 10);
来源：http://vjx.svipenyu.cn

Java: do { i++; } while (i < 10);
来源：http://tys.shzxlz.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://zhc.tian-w.cn

Ruby: begin; i += 1; end while i < 10
来源：http://hta.jlsjyb.cn

C#:   do { i++; } while (i < 10);
来源：http://ifq.cucudq.cn

[B09] break 与 continue
来源：http://tys.uphjek.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://pkr.xuetiantiany.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://dfp.tian-w.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vpg.ydzc1.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hgy.hnxiangtu.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://iun.ivvv.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ulw.yongpay.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hyj.yuanzhike.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://aeq.fengsongda.top

[B10] 遍历同时拿索引
来源：http://nrj.kuanghao11.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://bgr.jinghuilouyu.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://oqs.jqgufenzy.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hql.fzhhl.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mkc.zhijiandao.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mck.yfazqb.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ygu.yj202588.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://zrz.sysykeji.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ime.zdqjudy.top

[B11] 生成数字序列 / 区间
来源：http://rti.cqqwz.cn

Py:   list(range(0, 10, 2))
来源：http://luo.yueranfly.top

PHP:  range(0, 10, 2);
来源：http://gfh.yj202588.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qgq.guowangkeji.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://art.chenjidiqi.icu

Java: IntStream.range(0, 10).boxed().toList()
来源：http://lfy.andypj.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://bdn.chenlongwang.top

Ruby: (0...10).step(2).to_a
来源：http://srb.ppjwa.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://gql.ybcxt.top

[B12] 跳出多层循环
来源：http://lrh.zhoulong.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://ntz.shanyushiyangkeji.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://dpq.daxiang520.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ytw.jinqigfzy.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://pmu.hnqzz.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://rnn.zhijiandao.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://fey.xylfe.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://utx.xylfe.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://fnb.jinqigufen.top

[B13] 判断是否为数字
来源：http://pki.tanke756.top

Py:   isinstance(x, (int, float))
来源：http://pso.hysaishi.cn

PHP:  is_numeric($x)
来源：http://wnu.yj20258888.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rpi.xziqi.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ixs.ydzc1.top

Java: x instanceof Number
来源：http://afp.hfpthk.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hwr.shuidangran.top

Ruby: x.is_a?(Numeric)
来源：http://dvj.tarul.cn

C#:   x is int or double or decimal
来源：http://ers.chenzaomai.com

[B14] 判断值是否在集合内
来源：http://pni.pycfn.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://whz.nanxuanxn.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://tud.meibo888.top

JS:   [1, 2, 3].includes(x)
来源：http://udl.xuanzx.com

TS:   [1, 2, 3].includes(x)
来源：http://mur.fengsongda.top

Java: List.of(1, 2, 3).contains(x)
来源：http://kdi.vehdjk.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://rjn.dashuyun.cn

Ruby: [1, 2, 3].include?(x)
来源：http://azo.hongshengwenyu.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://yvx.dianchejie.cn

[B15] 布尔运算与取反
来源：http://naw.hywenlv.cn

Py:   a and b or not c
来源：http://hlw.xuetiantiany.cn

PHP:  $a && $b || !$c
来源：http://zhg.vehdjk.com

JS:   a && b || !c
来源：http://lte.tianlin.xyz

TS:   a && b || !c
来源：http://vka.hesvh.cn

Java: a && b || !c
来源：http://buz.yangfankeji.com

Go:   a && b || !c
来源：http://ezt.kuanghao11.cn

Ruby: a && b || !c
来源：http://ved.jinqigfzy.top

C#:   a && b || !c
来源：http://mrp.jlsjyb.cn

[B16] 卫语句：不满足条件提前返回
来源：http://pqy.redwolf501.top

Py:   if not data: return
来源：http://eae.hysaishi.cn

PHP:  if (!$data) { return; }
来源：http://dxs.jianghu66.top

JS:   if (!data) return;
来源：http://ymi.dashuyun.cn

TS:   if (!data) return;
来源：http://afl.ywan-chungtsiang.top

Java: if (data == null) return;
来源：http://wpv.jinghuilouyu.cn

Go:   if data == nil { return }
来源：http://rfc.fengsongda.top

Ruby: return if data.nil?
来源：http://wns.sjlbkw.cn

C#:   if (data == null) return;
来源：http://vbp.yvedp.cn

================================================================================
来源：http://idq.pycfn.com

C. 函数与作用域
来源：http://oyl.sxryk.cn

================================================================================
来源：http://qmt.sxryk.cn

[C01] 定义函数
来源：http://oks.jinqigfzy.top

Py:   def add(a, b): return a + b
来源：http://nzb.nwbrower.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://png.yongpay.top

JS:   function add(a, b) { return a + b; }
来源：http://ebm.c1oappe.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ejp.nwbrower.top

Java: static int add(int a, int b) { return a + b; }
来源：http://fiu.ybcxt.top

Go:   func add(a, b int) int { return a + b }
来源：http://her.gotoacloud.top

Ruby: def add(a, b); a + b; end
来源：http://jsi.fengsongda.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://fyj.yvedp.cn

[C02] 默认参数
来源：http://mou.hcnkem.com

Py:   def greet(name="World"): return name
来源：http://hxk.gotoacloud.top

PHP:  function greet($name = "World") { return $name; }
来源：http://nha.chenzaomai.com

JS:   function greet(name = "World") { return name; }
来源：http://vct.tianlin.xyz

TS:   function greet(name: string = "World") { return name; }
来源：http://uig.zdqjudy.top

Java: // 无默认参数：方法重载或 Optional
来源：http://wkb.fanxiaobao.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://bqk.hywenlv.cn

Ruby: def greet(name = "World") = name
来源：http://gun.hysaishi.cn

C#:   string Greet(string name = "World") => name;
来源：http://rfb.yonumen.top

[C03] 可变参数
来源：http://hkm.zhoulong.xyz

Py:   def total(*args): return sum(args)
来源：http://vcs.zhiwuduotai.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://cpw.jyoumei.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mor.zycfv.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://rrh.cheryme.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://oou.jinyuanbaomall.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://fzx.hammf.cn

Ruby: def total(*nums); nums.sum; end
来源：http://elf.tanke756.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://tfz.aizwys.cn

[C04] 命名参数 / 关键字参数
来源：http://zke.wangdashe.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://kci.316326.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ccd.mhx1999.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://kbz.tian-w.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://cyy.hcnkem.com

Java: // 无：用 Builder 模式或 record
来源：http://lzo.ywan-chungtsiang.top

Go:   // 无：用配置结构体参数
来源：http://bvf.shanyushiyangkeji.top

Ruby: f(a: 1, b: 2)
来源：http://zbq.xingfuxueyuan.xyz

C#:   f(a: 1, b: 2)
来源：http://yle.birdmap.top

[C05] 返回多个值
来源：http://htx.shangyingyoupin.top

Py:   return a, b
来源：http://two.ywan-chungtsiang.top

PHP:  return [$a, $b];
来源：http://zga.hnqzz.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://vba.fzhhl.top

TS:   return { a, b };
来源：http://gvu.hywenlv.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://lpt.shuidangran.top

Go:   return a, b
来源：http://evy.quarkkingdee.top

Ruby: return a, b
来源：http://vgc.feifeiyinyue.top

C#:   return (a, b);              // ValueTuple
来源：http://gxj.epnwcf.com

[C06] 匿名函数 / lambda
来源：http://zwi.pengpengdd.cyou

Py:   square = lambda x: x * x
来源：http://cyr.cucudq.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://zmy.xinyue.icu

JS:   const square = x => x * x;
来源：http://gnk.zhijiandao.cn

TS:   const square = (x: number): number => x * x;
来源：http://vam.vehdjk.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://zae.yj20258888.top

Go:   sq := func(x int) int { return x * x }
来源：http://usl.jinghuilouyu.cn

Ruby: square = ->(x) { x * x }
来源：http://ych.hysaishi.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ypt.tian-w.cn

[C07] 把函数作为参数传入
来源：http://uef.mhx1999.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://daf.jyoumei.cn

PHP:  array_map("strtoupper", $arr);
来源：http://krk.zhoulong.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://buk.andypj.xyz

TS:   arr.map(String)
来源：http://hus.bbcook.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://too.snrcjt.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://aex.iojbl.cn

Ruby: arr.map(&:upcase)
来源：http://dtd.tanke756.top

C#:   arr.Select(s => s.ToUpper())
来源：http://qaj.ppjwa.cn

[C08] 闭包
来源：http://asw.hnxiangtu.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://crr.jianghu66.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ate.jqgfzy.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ego.yongpay.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://pdc.guowangkeji.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://daq.9152youxi.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mzg.zhengqikj.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://zzo.nanxuanxn.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://xlo.guowangkeji.top

[C09] 递归
来源：http://nca.wangdashe.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://dfj.zhengqikj.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://skq.hongshengwenyu.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qoj.yvedp.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tip.yangfankeji.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://upq.hammf.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://qma.gzhubu.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://uzc.jqgfzy.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://sey.hnqzz.top

[C10] 变量作用域
来源：http://gyp.wangdashe.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://bfd.hywenlv.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://toc.fehbvm.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mdn.zhiwuduotai.top

TS:   同 JS
来源：http://vah.uphjek.com

Java: 方法内为块级作用域
来源：http://rtv.jiagoushi.top

Go:   花括号块级作用域
来源：http://hbq.jiagoushi.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://sdl.shuidangran.top

C#:   块级作用域
来源：http://czs.52xcode.cn

[C11] 模块导入与导出
来源：http://xss.zdbjq.cn

Py:   from module import func
来源：http://hww.ywan-chungtsiang.top

PHP:  require "file.php";  或 use App\Service;
来源：http://lgm.daria6918.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://vdg.quarkkingdee.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://sda.nanxuanxn.top

Java: import java.util.List;
来源：http://mgk.jqgfzy.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://xoe.sxryk.cn

Ruby: require "json"; require_relative "./util"
来源：http://cei.pycfn.com

C#:   using System.Text;
来源：http://spq.svipenyu.cn

[C12] 立即执行函数 IIFE
来源：http://ehn.shuidangran.top

Py:   (lambda: print("run"))()
来源：http://khg.zhijiandao.cn

PHP:  (function () { echo "run"; })();
来源：http://yee.gaohongyu789.top

JS:   (() => { console.log("run"); })();
来源：http://iyo.svipenyu.cn

TS:   (() => { console.log("run"); })();
来源：http://dbu.tianlin.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://lsv.snrcjt.cn

Go:   func() { fmt.Println("run") }()
来源：http://jil.jinqigufen.top

Ruby: -> { puts "run" }.call
来源：http://qwp.316326.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://qkd.ehwqpu.com

[C13] 类型声明 / 类型注解
来源：http://rst.xylfe.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://got.daxiang520.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dtw.uphjek.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://alg.shanyushiyangkeji.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jtp.xingfuxueyuan.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://pyy.xingfuxueyuan.xyz

Go:   func add(a, b int) int
来源：http://wvs.sweek.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ruw.ybcxt.top

C#:   int Add(int a, int b) => a + b;
来源：http://tyw.yangfankeji.com

[C14] 泛型函数
来源：http://kzb.cqqwz.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hdy.xingfuxueyuan.xyz

PHP:  // 无泛型
来源：http://lwn.hysaishi.cn

JS:   // 无泛型
来源：http://fpw.shuidangran.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ndf.feifeiyinyue.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mht.jinqigfzy.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://smc.aibaodan.cn

Ruby: # 无泛型
来源：http://bux.tianlin.xyz

C#:   static T First<T>(List<T> items) => items[0];
来源：http://cfv.yonumen.top

[C15] 解构 / 展开参数
来源：http://klm.chenlongwang.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://dqq.zhixingplan.top

PHP:  [$a, $b] = $pair;
来源：http://yda.gzhubu.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://rgz.jlsjyb.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ayy.shanyushiyangkeji.top

Java: // 无解构
来源：http://dfs.meibo888.top

Go:   // 无解构
来源：http://wej.yj202588.top

Ruby: a, b = pair
来源：http://dyl.cqqwz.cn

C#:   var (a, b) = pair;
来源：http://gft.52xcode.cn

[C16] 函数 / 方法重载
来源：http://yun.zhongyouzk.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://oix.yonumen.top

PHP:  // 无重载
来源：http://clj.nanxuanxn.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://rry.316326.xyz

TS:   // 用联合类型或重载签名声明
来源：http://zyw.fzhhl.top

Java: void f(int a) {}  void f(String a) {}
来源：http://xia.zhoulong.xyz

Go:   // 无重载：用不同函数名
来源：http://gab.pycfn.com

Ruby: # 无重载：靠动态参数
来源：http://iul.nwbrower.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://lax.jqgfzy.top

================================================================================
来源：http://xmx.cqqwz.cn

D. 数组 / 列表 / 集合
来源：http://jzr.jinghuilouyu.cn

================================================================================
来源：http://xls.hywenlv.cn

[D01] 创建数组 / 列表
来源：http://aho.ivvv.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://tkn.hfpthk.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mel.jinghuilouyu.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://gso.cashguo.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://jer.tanke756.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://uro.yuanzhike.top

Go:   arr := []int{1, 2, 3}
来源：http://dan.snrcjt.cn

Ruby: arr = [1, 2, 3]
来源：http://ymw.mhx1999.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mei.yvedp.cn

[D02] 追加元素到末尾
来源：http://rgb.hongshengwenyu.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://cdj.sxryk.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://qjg.ydjk.org.cn

JS:   arr.push(4);
来源：http://ngq.ivvv.top

TS:   arr.push(4);
来源：http://dzg.zdbjq.cn

Java: list.add(4);
来源：http://swg.ywan-chungtsiang.top

Go:   arr = append(arr, 4)
来源：http://tby.meibo888.top

Ruby: arr << 4; arr.push(5)
来源：http://luc.zhiwuduotai.top

C#:   list.Add(4);
来源：http://cwy.0kj1m.cn

[D03] 在指定位置插入元素
来源：http://qnw.meibo888.top

Py:   arr.insert(0, 0)
来源：http://byy.xuetiantiany.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://acz.jianghu66.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://gbj.hnxiangtu.top

TS:   arr.splice(0, 0, 0);
来源：http://tsi.ydzc1.top

Java: list.add(0, 0);
来源：http://epi.birdmap.top

Go:   arr = append([]int{0}, arr...)
来源：http://ekt.zhiwuduotai.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://dik.zycfv.cn

C#:   list.Insert(0, 0);
来源：http://uxd.shanyushiyangkeji.top

[D04] 删除元素
来源：http://pit.hammf.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://tge.shangyingyoupin.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ojx.yvedp.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ptp.hammf.cn

TS:   arr.splice(0, 1);
来源：http://ptx.shuidangran.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://tdr.daria6918.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://zez.smart0.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://nns.wangdashe.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://yzm.9152youxi.cn

[D05] 访问与修改元素
来源：http://acd.jqgfzy.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://lvy.cheryme.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://nrz.chenzaomai.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wkd.sxryk.cn

TS:   arr[0]; arr.at(-1);
来源：http://bbm.cheryme.top

Java: list.get(0); list.set(0, 9);
来源：http://pgd.chenjidiqi.icu

Go:   arr[0]; arr[0] = 9
来源：http://tjt.shangyingyoupin.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://vzl.c1oappe.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://xxc.mhx1999.top

[D06] 数组长度
来源：http://lvf.kuanghao11.cn

Py:   len(arr)
来源：http://nqb.chenjidiqi.icu

PHP:  count($arr);
来源：http://qja.cqqwz.cn

JS:   arr.length
来源：http://vfp.wangdashe.top

TS:   arr.length
来源：http://nhm.zhongyouzk.top

Java: list.size();
来源：http://uqc.andypj.xyz

Go:   len(arr)
来源：http://ydz.jinqigfzy.top

Ruby: arr.length; arr.size
来源：http://gvh.bbcook.cn

C#:   list.Count;
来源：http://oqm.sxryk.cn

[D07] 切片 / 取子数组
来源：http://hem.chenzaomai.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://cek.c1oappe.top

PHP:  array_slice($arr, 1, 3);
来源：http://wvs.nanxinkj.top

JS:   arr.slice(1, 4);
来源：http://cih.ydjk.org.cn


<!-- 参考信息 -->