代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://ile.gzhubu.top

PHP:  do { $i++; } while ($i < 10);
来源：http://nhv.gogol.net.cn

JS:   do { i++; } while (i < 10);
来源：http://jpl.nanxinkj.top

TS:   do { i++; } while (i < 10);
来源：http://btx.tian-w.cn

Java: do { i++; } while (i < 10);
来源：http://ems.shanyushiyangtech.top

Go:   for { i++; if i >= 10 { break } }
来源：http://bvv.jqgufenzy.top

Ruby: begin; i += 1; end while i < 10
来源：http://whh.gaohongyu789.top

C#:   do { i++; } while (i < 10);
来源：http://kld.zdbjq.cn

[B09] break 与 continue
来源：http://nni.epnwcf.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://whh.yj20258888.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://iqh.zhiwuduotai.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uon.pycfn.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dih.zhengqikj.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mdm.jyoumei.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://xcd.xylfe.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baq.fengsongda.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://amb.jiagoushi.top

[B10] 遍历同时拿索引
来源：http://gha.jiagoushi.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://lqy.hcnkem.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://foy.cqqwz.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xpi.yj20258.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mqf.0kj1m.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ldj.meibo888.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://dme.jiagoushi.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://qcu.yangfankeji.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://svx.vehdjk.com

[B11] 生成数字序列 / 区间
来源：http://ugg.pengpengdd.cyou

Py:   list(range(0, 10, 2))
来源：http://pqi.0kj1m.cn

PHP:  range(0, 10, 2);
来源：http://rdq.jinqigfzy.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://onn.wangshuangyany.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://odh.cucudq.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://sra.cdnleiting.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://sul.wangdashe.top

Ruby: (0...10).step(2).to_a
来源：http://lzm.hongshengwenyu.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://jrb.nanxuanxn.top

[B12] 跳出多层循环
来源：http://ten.wangdashe.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://yhy.hammf.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://hvv.hcnkem.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://dyf.bjfxy.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://pse.meibo888.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://qcx.316326.xyz

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ixy.ivvv.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://oqp.daxiang520.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://spn.wangshuangyany.cn

[B13] 判断是否为数字
来源：http://eqw.aizwys.cn

Py:   isinstance(x, (int, float))
来源：http://qjr.tian-w.cn

PHP:  is_numeric($x)
来源：http://yri.chenjidiqi.icu

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://uzy.0kj1m.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lnc.yuxming.cn

Java: x instanceof Number
来源：http://ghv.zhijiandao.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://pzz.yvedp.cn

Ruby: x.is_a?(Numeric)
来源：http://zmo.xingfuxueyuan.xyz

C#:   x is int or double or decimal
来源：http://asd.cucudq.cn

[B14] 判断值是否在集合内
来源：http://ykw.quarkkingdee.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://icg.ctjpmb.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blu.xylfe.cn

JS:   [1, 2, 3].includes(x)
来源：http://cqz.sufxvd.cn

TS:   [1, 2, 3].includes(x)
来源：http://vvm.ywan-chungtsiang.top

Java: List.of(1, 2, 3).contains(x)
来源：http://ssa.sufxvd.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://fel.hnxiangtu.top

Ruby: [1, 2, 3].include?(x)
来源：http://siq.wangdashe.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://msd.kuanghao11.cn

[B15] 布尔运算与取反
来源：http://fgt.jinqigfzy.top

Py:   a and b or not c
来源：http://mff.jlsjyb.cn

PHP:  $a && $b || !$c
来源：http://zlh.havefunace.top

JS:   a && b || !c
来源：http://xmm.hnqzz.top

TS:   a && b || !c
来源：http://ynq.zhongyouzk.top

Java: a && b || !c
来源：http://vqv.yfazqb.com

Go:   a && b || !c
来源：http://iem.svipenyu.cn

Ruby: a && b || !c
来源：http://imn.xuetiantiany.cn

C#:   a && b || !c
来源：http://yeg.sxryk.cn

[B16] 卫语句：不满足条件提前返回
来源：http://prx.feifeiyinyue.top

Py:   if not data: return
来源：http://bgw.hesvh.cn

PHP:  if (!$data) { return; }
来源：http://lfv.zdbjq.cn

JS:   if (!data) return;
来源：http://vdu.tianlin.xyz

TS:   if (!data) return;
来源：http://zcc.xuanzx.com

Java: if (data == null) return;
来源：http://ssl.jlsjyb.cn

Go:   if data == nil { return }
来源：http://faa.tianlin.xyz

Ruby: return if data.nil?
来源：http://bvp.gzhubu.top

C#:   if (data == null) return;
来源：http://yaf.dashuyun.cn

================================================================================
来源：http://ivo.bjfxy.top

C. 函数与作用域
来源：http://shd.tanke756.top

================================================================================
来源：http://dju.meibo888.top

[C01] 定义函数
来源：http://lfs.gzhubu.top

Py:   def add(a, b): return a + b
来源：http://gli.xuanzx.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hfl.feifeiyinyue.top

JS:   function add(a, b) { return a + b; }
来源：http://svg.c1oappe.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tch.ydzc1.top

Java: static int add(int a, int b) { return a + b; }
来源：http://asm.hammf.cn

Go:   func add(a, b int) int { return a + b }
来源：http://lad.jinqigfzy.top

Ruby: def add(a, b); a + b; end
来源：http://hyc.ppjwa.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mkc.cashguo.top

[C02] 默认参数
来源：http://yft.52xcode.cn

Py:   def greet(name="World"): return name
来源：http://whm.wangdashe.top

PHP:  function greet($name = "World") { return $name; }
来源：http://enc.xziqi.cn

JS:   function greet(name = "World") { return name; }
来源：http://arz.sjlbkw.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://xjl.uphjek.com

Java: // 无默认参数：方法重载或 Optional
来源：http://yps.yanxiufei.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wgm.316326.xyz

Ruby: def greet(name = "World") = name
来源：http://fym.uphjek.com

C#:   string Greet(string name = "World") => name;
来源：http://wuw.epnwcf.com

[C03] 可变参数
来源：http://xbn.aibaodan.cn

Py:   def total(*args): return sum(args)
来源：http://bpc.tianlin.xyz

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://vns.hysaishi.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://jcv.cucudq.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://uge.snrcjt.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://btg.xinyue.icu

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://rgm.redwolf501.top

Ruby: def total(*nums); nums.sum; end
来源：http://bab.svipenyu.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://jrf.0kj1m.cn

[C04] 命名参数 / 关键字参数
来源：http://klo.shangyingyoupin.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://gem.cashguo.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://shc.gogol.net.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://dgz.sjlbkw.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mpj.ybcxt.top

Java: // 无：用 Builder 模式或 record
来源：http://hhd.316326.xyz

Go:   // 无：用配置结构体参数
来源：http://tze.gogol.net.cn

Ruby: f(a: 1, b: 2)
来源：http://wpy.ybcxt.top

C#:   f(a: 1, b: 2)
来源：http://iuq.nanxinkj.top

[C05] 返回多个值
来源：http://qku.sxryk.cn

Py:   return a, b
来源：http://dzv.tian-w.cn

PHP:  return [$a, $b];
来源：http://ugm.kuanghao11.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://seh.hcnkem.com

TS:   return { a, b };
来源：http://scy.hfpthk.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://vsb.tanke756.top

Go:   return a, b
来源：http://drd.dashuyun.cn

Ruby: return a, b
来源：http://edp.tanke756.top

C#:   return (a, b);              // ValueTuple
来源：http://hqj.sweek.top

[C06] 匿名函数 / lambda
来源：http://dap.andypj.xyz

Py:   square = lambda x: x * x
来源：http://noo.jiagoushi.top

PHP:  $square = fn($x) => $x * $x;
来源：http://cpf.aibaodan.cn

JS:   const square = x => x * x;
来源：http://vem.xingfuxueyuan.xyz

TS:   const square = (x: number): number => x * x;
来源：http://tbt.pengpengdd.cyou

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://kyy.shanyushiyangkeji.top

Go:   sq := func(x int) int { return x * x }
来源：http://qaq.zhengqikj.top

Ruby: square = ->(x) { x * x }
来源：http://ltf.chenlongwang.top

C#:   Func<int, int> square = x => x * x;
来源：http://qzp.tianlin.xyz

[C07] 把函数作为参数传入
来源：http://frm.fengsongda.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wys.quarkkingdee.top

PHP:  array_map("strtoupper", $arr);
来源：http://fno.zdbjq.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ais.yonumen.top

TS:   arr.map(String)
来源：http://lkf.yueranfly.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://lwa.jqgfzy.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ayr.zhaomingkeji.xyz

Ruby: arr.map(&:upcase)
来源：http://bjv.havefunace.top

C#:   arr.Select(s => s.ToUpper())
来源：http://xsa.zhoulong.xyz

[C08] 闭包
来源：http://kqn.vehdjk.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://uvw.tian-w.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ymx.xziqi.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://jfv.aibaodan.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ytc.fengsongda.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://lvd.daria6918.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://khp.dianchejie.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://zzr.feifeiyinyue.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://iwe.yonumen.top

[C09] 递归
来源：http://hdi.yanxiufei.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://azb.jinghuilouyu.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://alz.hnxiangtu.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ldk.zycfv.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cev.vqdsnc.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ikd.zdbjq.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://bxc.zhixingplan.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://daw.meibo888.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://avz.xylfe.cn

[C10] 变量作用域
来源：http://wge.haohaochexian.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baw.jinqigfzy.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://dch.9152youxi.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://vap.quarkkingdee.top

TS:   同 JS
来源：http://fyg.ppjwa.cn

Java: 方法内为块级作用域
来源：http://dfu.xuanzx.com

Go:   花括号块级作用域
来源：http://yyd.redwolf501.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://bsf.wangshuangyany.cn

C#:   块级作用域
来源：http://krv.jqgfzy.top

[C11] 模块导入与导出
来源：http://cho.yfazqb.com

Py:   from module import func
来源：http://sxe.fktsv.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://tau.dianchejie.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://qtc.ppjwa.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://yot.vehdjk.com

Java: import java.util.List;
来源：http://tko.ydjk.org.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://iwa.ppjwa.cn

Ruby: require "json"; require_relative "./util"
来源：http://amh.zhiwuduotai.top

C#:   using System.Text;
来源：http://suw.sjlbkw.cn

[C12] 立即执行函数 IIFE
来源：http://jop.fehbvm.com

Py:   (lambda: print("run"))()
来源：http://djs.vehdjk.com

PHP:  (function () { echo "run"; })();
来源：http://ywq.mhx1999.top

JS:   (() => { console.log("run"); })();
来源：http://mzy.zhaomingkeji.xyz

TS:   (() => { console.log("run"); })();
来源：http://eya.hnqzz.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://yrf.jlsjyb.cn

Go:   func() { fmt.Println("run") }()
来源：http://zjy.hammf.cn

Ruby: -> { puts "run" }.call
来源：http://rpj.9152youxi.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://uzs.ydzc1.top

[C13] 类型声明 / 类型注解
来源：http://opv.bjfxy.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://beo.shangyingyoupin.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kou.jiagoushi.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://qgs.andypj.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://slg.zdqjudy.top

Java: int add(int a, int b) { return a + b; }
来源：http://hgi.fengsongda.top

Go:   func add(a, b int) int
来源：http://iju.xuetiantiany.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hwh.shzxlz.cn

C#:   int Add(int a, int b) => a + b;
来源：http://pbf.jinqigufen.top

[C14] 泛型函数
来源：http://gib.hfpthk.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zne.aizwys.cn

PHP:  // 无泛型
来源：http://vie.cucudq.cn

JS:   // 无泛型
来源：http://olc.chenlongwang.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://klz.shzxlz.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://gda.epnwcf.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://eqc.jqgufenzy.top

Ruby: # 无泛型
来源：http://uyx.cqqwz.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wyn.sxryk.cn

[C15] 解构 / 展开参数
来源：http://kcn.shanyushiyangkeji.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://jln.yueranfly.top

PHP:  [$a, $b] = $pair;
来源：http://ypo.vqdsnc.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hev.yvedp.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mht.vqdsnc.cn

Java: // 无解构
来源：http://vnu.ppjwa.cn

Go:   // 无解构
来源：http://kqs.mhx1999.top

Ruby: a, b = pair
来源：http://ejh.gzhubu.top

C#:   var (a, b) = pair;
来源：http://qlq.zdbjq.cn

[C16] 函数 / 方法重载
来源：http://yuq.guowangkeji.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://cnz.wangdashe.top

PHP:  // 无重载
来源：http://iyt.tanke756.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://qhs.yueranfly.top

TS:   // 用联合类型或重载签名声明
来源：http://kdu.pengpengdd.cyou

Java: void f(int a) {}  void f(String a) {}
来源：http://zgp.yongpay.top

Go:   // 无重载：用不同函数名
来源：http://eij.sxryk.cn

Ruby: # 无重载：靠动态参数
来源：http://tnk.jyoumei.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://mde.yanxiufei.cn

================================================================================
来源：http://fuw.cdnleiting.top

D. 数组 / 列表 / 集合
来源：http://ikp.gogol.net.cn

================================================================================
来源：http://qit.haohaochexian.top

[D01] 创建数组 / 列表
来源：http://pxk.jqgufenzy.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://hzq.birdmap.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://vum.zhongyouzk.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://war.zdbjq.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://svu.fehbvm.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://rms.yangfankeji.com

Go:   arr := []int{1, 2, 3}
来源：http://icg.tian-w.cn

Ruby: arr = [1, 2, 3]
来源：http://jkm.cqqwz.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://dxt.tian-w.cn

[D02] 追加元素到末尾
来源：http://evd.zhongyouzk.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hyq.feifeiyinyue.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://nug.shzxlz.cn

JS:   arr.push(4);
来源：http://msx.mhx1999.top

TS:   arr.push(4);
来源：http://bsa.sjlbkw.cn

Java: list.add(4);
来源：http://deh.zhoulong.xyz

Go:   arr = append(arr, 4)
来源：http://pcg.guowangkeji.top

Ruby: arr << 4; arr.push(5)
来源：http://ros.zhoulong.xyz

C#:   list.Add(4);
来源：http://neu.xingfuxueyuan.xyz

[D03] 在指定位置插入元素
来源：http://ncb.iojbl.cn

Py:   arr.insert(0, 0)
来源：http://plq.fktsv.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://rur.havefunace.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://xkr.tanke756.top

TS:   arr.splice(0, 0, 0);
来源：http://jhf.yangfankeji.com

Java: list.add(0, 0);
来源：http://nlw.hammf.cn

Go:   arr = append([]int{0}, arr...)
来源：http://cmi.aibaodan.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://kbc.hnxiangtu.top

C#:   list.Insert(0, 0);
来源：http://yjf.hongshengwenyu.top

[D04] 删除元素
来源：http://poq.nanxinkj.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://zrf.guannengcc.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://kxd.jinyuanbaomall.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ktf.sufxvd.cn

TS:   arr.splice(0, 1);
来源：http://rwi.vqdsnc.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://cqi.shanyushiyangtech.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://oxq.zhijiandao.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://aka.cucudq.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://lor.cashguo.top

[D05] 访问与修改元素
来源：http://kgt.shanyushiyangkeji.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://qgm.xinyue.icu

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://nzu.smart0.xyz

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://rdf.mhx1999.top

TS:   arr[0]; arr.at(-1);
来源：http://noo.shzxlz.cn

Java: list.get(0); list.set(0, 9);
来源：http://bju.gzhubu.top

Go:   arr[0]; arr[0] = 9
来源：http://qad.uphjek.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://kuj.svipenyu.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://rki.jinqigufen.top

[D06] 数组长度
来源：http://vti.shzxlz.cn

Py:   len(arr)
来源：http://nvg.hesvh.cn

PHP:  count($arr);
来源：http://cpg.hywenlv.cn

JS:   arr.length
来源：http://tiu.yj20258888.top

TS:   arr.length
来源：http://kud.jqgfzy.top

Java: list.size();
来源：http://hbo.fktsv.cn

Go:   len(arr)
来源：http://ucy.nanxuanxn.top

Ruby: arr.length; arr.size
来源：http://hck.tian-w.cn

C#:   list.Count;
来源：http://ryz.jinqigfzy.top

[D07] 切片 / 取子数组
来源：http://hlb.zycfv.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qjm.zhoulong.xyz

PHP:  array_slice($arr, 1, 3);
来源：http://khn.pengpengdd.cyou

JS:   arr.slice(1, 4);
来源：http://nfg.yangfankeji.com

TS:   arr.slice(1, 4);
来源：http://ipp.tianlin.xyz

Java: list.subList(1, 4);
来源：http://qeu.gzhubu.top

Go:   arr[1:4]
来源：http://zef.316326.xyz

Ruby: arr[1, 3]
来源：http://cul.xingfuxueyuan.xyz

C#:   list.GetRange(1, 3);
来源：http://mna.dianchejie.cn

[D08] 合并两个数组
来源：http://hpw.zhengqikj.top

Py:   a + b;  a.extend(b)
来源：http://xuj.sjlbkw.cn

PHP:  array_merge($a, $b);
来源：http://mfa.sufxvd.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://fij.yueranfly.top

TS:   [...a, ...b];
来源：http://dqt.wangshuangyany.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://gaj.andypj.xyz

Go:   append(a, b...)
来源：http://lmb.zhengqikj.top


<!-- 参考信息 -->