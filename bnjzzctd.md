代发 wailian999

PHP:  while ($i < 10) { $i++; }
来源：http://sus.hysaishi.cn

JS:   while (i < 10) { i++; }
来源：http://eaw.nanxuanxn.top

TS:   while (i < 10) { i++; }
来源：http://jhn.yangfankeji.com

Java: while (i < 10) { i++; }
来源：http://dev.fzhhl.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://atz.hnqzz.top

Ruby: while i < 10; i += 1; end
来源：http://vbg.zdqjudy.top

C#:   while (i < 10) { i++; }
来源：http://exh.yuxming.cn

[B08] do-while（至少执行一次）
来源：http://kim.cheryme.top

Py:   # 无 do-while：用 while True + break
来源：http://jpe.fehbvm.com

PHP:  do { $i++; } while ($i < 10);
来源：http://esz.cucudq.cn

JS:   do { i++; } while (i < 10);
来源：http://wdk.yfazqb.com

TS:   do { i++; } while (i < 10);
来源：http://lkh.andypj.xyz

Java: do { i++; } while (i < 10);
来源：http://vwh.zhijiandao.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://jnf.guowangkeji.top

Ruby: begin; i += 1; end while i < 10
来源：http://azb.pengpengdd.cyou

C#:   do { i++; } while (i < 10);
来源：http://adr.meibo888.top

[B09] break 与 continue
来源：http://hei.ydzc1.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hif.fehbvm.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mps.quarkkingdee.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nxy.ppjwa.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hvm.kuanghao11.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dim.haohaochexian.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://shi.yanxiufei.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://lij.yj20258.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sep.hcnkem.com

[B10] 遍历同时拿索引
来源：http://aie.yanxiufei.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://cbn.ppjwa.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://xov.fzhhl.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://zza.feifeiyinyue.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://iyd.hesvh.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://jqu.dianchejie.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://cyc.shzxlz.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ksx.cucudq.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://nrt.fzhhl.top

[B11] 生成数字序列 / 区间
来源：http://mwi.xinyue.icu

Py:   list(range(0, 10, 2))
来源：http://jeu.uphjek.com

PHP:  range(0, 10, 2);
来源：http://wky.guowangkeji.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fra.yj20258888.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tuh.pycfn.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://jhv.hysaishi.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wlc.meibo888.top

Ruby: (0...10).step(2).to_a
来源：http://vai.yonumen.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://jlk.zhoulong.xyz

[B12] 跳出多层循环
来源：http://ira.shangyingyoupin.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://ljg.jinqigfzy.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://exa.tanke756.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mzr.zhengqikj.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://vqb.fktsv.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://awh.yanxiufei.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hrd.xingfuxueyuan.xyz

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ogg.pycfn.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://yyf.havefunace.top

[B13] 判断是否为数字
来源：http://eoe.sxryk.cn

Py:   isinstance(x, (int, float))
来源：http://hmh.316326.xyz

PHP:  is_numeric($x)
来源：http://nnm.mhx1999.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qjk.316326.xyz

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yjp.shanyushiyangtech.top

Java: x instanceof Number
来源：http://fol.fanxiaobao.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://klw.jinqigufen.top

Ruby: x.is_a?(Numeric)
来源：http://ifn.yonumen.top

C#:   x is int or double or decimal
来源：http://efz.yuanzhike.top

[B14] 判断值是否在集合内
来源：http://oqj.tianlin.xyz

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://fbu.snrcjt.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://apz.zhiwuduotai.top

JS:   [1, 2, 3].includes(x)
来源：http://mwg.guowangkeji.top

TS:   [1, 2, 3].includes(x)
来源：http://tjq.yongpay.top

Java: List.of(1, 2, 3).contains(x)
来源：http://zju.svipenyu.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://thr.xuetiantiany.cn

Ruby: [1, 2, 3].include?(x)
来源：http://pem.shzxlz.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://bsr.c1oappe.top

[B15] 布尔运算与取反
来源：http://lpn.fehbvm.com

Py:   a and b or not c
来源：http://oci.dianchejie.cn

PHP:  $a && $b || !$c
来源：http://xba.daria6918.cn

JS:   a && b || !c
来源：http://hsb.yueranfly.top

TS:   a && b || !c
来源：http://aed.zhongyouzk.top

Java: a && b || !c
来源：http://wpi.bbcook.cn

Go:   a && b || !c
来源：http://kea.hesvh.cn

Ruby: a && b || !c
来源：http://oiu.daria6918.cn

C#:   a && b || !c
来源：http://jul.52xcode.cn

[B16] 卫语句：不满足条件提前返回
来源：http://aut.shzxlz.cn

Py:   if not data: return
来源：http://xsv.sysykeji.top

PHP:  if (!$data) { return; }
来源：http://imq.jlsjyb.cn

JS:   if (!data) return;
来源：http://hxz.aizwys.cn

TS:   if (!data) return;
来源：http://bvo.andypj.xyz

Java: if (data == null) return;
来源：http://nev.feifeiyinyue.top

Go:   if data == nil { return }
来源：http://vqe.epnwcf.com

Ruby: return if data.nil?
来源：http://rzd.chenjidiqi.icu

C#:   if (data == null) return;
来源：http://jpr.redwolf501.top

================================================================================
来源：http://uaf.ivvv.top

C. 函数与作用域
来源：http://aup.uphjek.com

================================================================================
来源：http://dxd.bbcook.cn

[C01] 定义函数
来源：http://jah.sufxvd.cn

Py:   def add(a, b): return a + b
来源：http://zmg.cdnleiting.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kap.redwolf501.top

JS:   function add(a, b) { return a + b; }
来源：http://sss.daria6918.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nrt.yvedp.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://txi.xuanzx.com

Go:   func add(a, b int) int { return a + b }
来源：http://ohw.shanyushiyangkeji.top

Ruby: def add(a, b); a + b; end
来源：http://gpe.jqgfzy.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://toi.daxiang520.top

[C02] 默认参数
来源：http://xuj.tanke756.top

Py:   def greet(name="World"): return name
来源：http://qja.aizwys.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://fca.andypj.xyz

JS:   function greet(name = "World") { return name; }
来源：http://yxt.aizwys.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ksc.yanxiufei.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://cey.yanxiufei.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://sgr.zhoulong.xyz

Ruby: def greet(name = "World") = name
来源：http://rut.aizwys.cn

C#:   string Greet(string name = "World") => name;
来源：http://imz.havefunace.top

[C03] 可变参数
来源：http://ktj.316326.xyz

Py:   def total(*args): return sum(args)
来源：http://rpv.tian-w.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://kmu.nanxuanxn.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mvi.zdbjq.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://kyi.0kj1m.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://agm.vehdjk.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ppn.shanyushiyangkeji.top

Ruby: def total(*nums); nums.sum; end
来源：http://xdl.snrcjt.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://tik.bbcook.cn

[C04] 命名参数 / 关键字参数
来源：http://uhk.gotoacloud.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://fmf.yuanzhike.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://jav.sufxvd.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://shh.daria6918.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ifb.tanke756.top

Java: // 无：用 Builder 模式或 record
来源：http://yaf.hongshengwenyu.top

Go:   // 无：用配置结构体参数
来源：http://isf.jyoumei.cn

Ruby: f(a: 1, b: 2)
来源：http://yib.shanyushiyangkeji.top

C#:   f(a: 1, b: 2)
来源：http://ngm.hesvh.cn

[C05] 返回多个值
来源：http://mqr.hfpthk.cn

Py:   return a, b
来源：http://ryq.hesvh.cn

PHP:  return [$a, $b];
来源：http://gtm.sysykeji.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://olq.bjfxy.top

TS:   return { a, b };
来源：http://fjl.xuanzx.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://dfd.sxryk.cn

Go:   return a, b
来源：http://dsh.zhoulong.xyz

Ruby: return a, b
来源：http://ylz.yuanzhike.top

C#:   return (a, b);              // ValueTuple
来源：http://roz.zhixingplan.top

[C06] 匿名函数 / lambda
来源：http://jnc.ybcxt.top

Py:   square = lambda x: x * x
来源：http://mzx.yfazqb.com

PHP:  $square = fn($x) => $x * $x;
来源：http://sqt.jinyuanbaomall.cn

JS:   const square = x => x * x;
来源：http://tht.jinghuilouyu.cn

TS:   const square = (x: number): number => x * x;
来源：http://onv.yj20258.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://fjb.gogol.net.cn

Go:   sq := func(x int) int { return x * x }
来源：http://gud.fanxiaobao.xyz

Ruby: square = ->(x) { x * x }
来源：http://igb.zhoulong.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://rwq.zhoulong.xyz

[C07] 把函数作为参数传入
来源：http://ekj.tarul.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ndu.wangdashe.top

PHP:  array_map("strtoupper", $arr);
来源：http://dzk.guannengcc.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://kej.c1oappe.top

TS:   arr.map(String)
来源：http://pln.bjfxy.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://zfh.shzxlz.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://rya.sweek.top

Ruby: arr.map(&:upcase)
来源：http://twt.yfazqb.com

C#:   arr.Select(s => s.ToUpper())
来源：http://ybs.tianlin.xyz

[C08] 闭包
来源：http://ucp.yfazqb.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://akb.yuxming.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://bke.cheryme.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://adc.aizwys.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://vfb.hammf.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://shg.svipenyu.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wva.fehbvm.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://vqj.yj202588.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ntv.fanxiaobao.xyz

[C09] 递归
来源：http://yvy.gogol.net.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mrg.yueranfly.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://txm.xingfuxueyuan.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mnb.hfpthk.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ydk.52xcode.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://fat.ppjwa.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://qhi.xinyue.icu

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://icu.shzxlz.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ley.daria6918.cn

[C10] 变量作用域
来源：http://sbp.fanxiaobao.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://eeg.yanxiufei.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ido.pengpengdd.cyou

JS:   let/const 块级作用域，var 函数级作用域
来源：http://rxq.shanyushiyangtech.top

TS:   同 JS
来源：http://uvf.52xcode.cn

Java: 方法内为块级作用域
来源：http://jlw.yangfankeji.com

Go:   花括号块级作用域
来源：http://rva.jyoumei.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mys.yj20258888.top

C#:   块级作用域
来源：http://lsw.hcnkem.com

[C11] 模块导入与导出
来源：http://btb.gaohongyu789.top

Py:   from module import func
来源：http://pud.aibaodan.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://bsp.zhaomingkeji.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://tjx.jinyuanbaomall.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://sll.yj20258888.top

Java: import java.util.List;
来源：http://lwb.shzxlz.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://yzo.daxiang520.top

Ruby: require "json"; require_relative "./util"
来源：http://zts.gaohongyu789.top

C#:   using System.Text;
来源：http://zog.iojbl.cn

[C12] 立即执行函数 IIFE
来源：http://nli.52xcode.cn

Py:   (lambda: print("run"))()
来源：http://xsf.zhaomingkeji.xyz

PHP:  (function () { echo "run"; })();
来源：http://rxv.zhoulong.xyz

JS:   (() => { console.log("run"); })();
来源：http://zks.meibo888.top

TS:   (() => { console.log("run"); })();
来源：http://xzg.hcnkem.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ekc.shuidangran.top

Go:   func() { fmt.Println("run") }()
来源：http://rsa.hnxiangtu.top

Ruby: -> { puts "run" }.call
来源：http://xsw.yanxiufei.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://pek.jinqigufen.top

[C13] 类型声明 / 类型注解
来源：http://kpj.ppjwa.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://fuw.hnqzz.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rpq.haohaochexian.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ltd.xziqi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qym.ywan-chungtsiang.top

Java: int add(int a, int b) { return a + b; }
来源：http://bqg.tianlin.xyz

Go:   func add(a, b int) int
来源：http://sqd.hysaishi.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://kcg.9152youxi.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ypc.shanyushiyangkeji.top

[C14] 泛型函数
来源：http://txf.shanyushiyangtech.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hxq.mhx1999.top

PHP:  // 无泛型
来源：http://xvo.guannengcc.top

JS:   // 无泛型
来源：http://ofu.daxiang520.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mph.gotoacloud.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://byr.hammf.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://azt.cheryme.top

Ruby: # 无泛型
来源：http://bzr.xuanzx.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://eka.xylfe.cn

[C15] 解构 / 展开参数
来源：http://hvz.0kj1m.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://cba.yuxming.cn

PHP:  [$a, $b] = $pair;
来源：http://rlz.jiagoushi.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://syn.shangyingyoupin.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://rvn.yj20258888.top

Java: // 无解构
来源：http://mdf.hnqzz.top

Go:   // 无解构
来源：http://ifn.jinghuilouyu.cn

Ruby: a, b = pair
来源：http://crj.fehbvm.com

C#:   var (a, b) = pair;
来源：http://pdf.yfazqb.com

[C16] 函数 / 方法重载
来源：http://djt.sysykeji.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://tbs.pycfn.com

PHP:  // 无重载
来源：http://fmv.zdqjudy.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://kkt.yfazqb.com

TS:   // 用联合类型或重载签名声明
来源：http://mel.vehdjk.com

Java: void f(int a) {}  void f(String a) {}
来源：http://oiz.tianlin.xyz

Go:   // 无重载：用不同函数名
来源：http://dxs.jianghu66.top

Ruby: # 无重载：靠动态参数
来源：http://qrz.uphjek.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://ign.zhoulong.xyz

================================================================================
来源：http://hku.xinyue.icu

D. 数组 / 列表 / 集合
来源：http://ges.vehdjk.com

================================================================================
来源：http://bmr.shanyushiyangkeji.top

[D01] 创建数组 / 列表
来源：http://pkf.xuanzx.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://yuf.yfazqb.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://znf.yvedp.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hkd.xingfuxueyuan.xyz

TS:   const arr: number[] = [1, 2, 3];
来源：http://cea.aizwys.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ahf.yj20258888.top

Go:   arr := []int{1, 2, 3}
来源：http://ary.jinqigfzy.top

Ruby: arr = [1, 2, 3]
来源：http://jxz.quarkkingdee.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ivv.gaohongyu789.top

[D02] 追加元素到末尾
来源：http://tzk.sufxvd.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://jtc.nanxuanxn.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://heg.aizwys.cn

JS:   arr.push(4);
来源：http://pip.sjlbkw.cn

TS:   arr.push(4);
来源：http://eam.vehdjk.com

Java: list.add(4);
来源：http://lze.zhongyouzk.top

Go:   arr = append(arr, 4)
来源：http://yul.daxiang520.top

Ruby: arr << 4; arr.push(5)
来源：http://oae.zhiwuduotai.top

C#:   list.Add(4);
来源：http://huj.zhengqikj.top

[D03] 在指定位置插入元素
来源：http://cos.shuidangran.top

Py:   arr.insert(0, 0)
来源：http://yxa.52xcode.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://jsr.52xcode.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://nim.shanyushiyangtech.top

TS:   arr.splice(0, 0, 0);
来源：http://qet.yongpay.top

Java: list.add(0, 0);
来源：http://rsj.ctjpmb.com

Go:   arr = append([]int{0}, arr...)
来源：http://hbs.jiagoushi.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://jfc.zhixingplan.top

C#:   list.Insert(0, 0);
来源：http://vog.epnwcf.com

[D04] 删除元素
来源：http://nab.xziqi.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://gcq.cashguo.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ytw.gotoacloud.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hqy.9152youxi.cn

TS:   arr.splice(0, 1);
来源：http://kgn.pengpengdd.cyou

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://tze.cdnleiting.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://rgw.redwolf501.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hof.zhiwuduotai.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wdp.guowangkeji.top

[D05] 访问与修改元素
来源：http://wfu.sweek.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://jex.hesvh.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://tth.fehbvm.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://het.ywan-chungtsiang.top

TS:   arr[0]; arr.at(-1);
来源：http://xci.gogol.net.cn

Java: list.get(0); list.set(0, 9);
来源：http://teh.cucudq.cn

Go:   arr[0]; arr[0] = 9
来源：http://huo.epnwcf.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://jrf.hywenlv.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mnt.jqgfzy.top

[D06] 数组长度
来源：http://zzs.yj202588.top

Py:   len(arr)
来源：http://qyl.feifeiyinyue.top

PHP:  count($arr);
来源：http://hob.bbcook.cn

JS:   arr.length
来源：http://xuv.meibo888.top

TS:   arr.length
来源：http://xqe.hongshengwenyu.top

Java: list.size();
来源：http://umk.snrcjt.cn

Go:   len(arr)
来源：http://bkr.fanxiaobao.xyz

Ruby: arr.length; arr.size
来源：http://tmn.fengsongda.top

C#:   list.Count;
来源：http://fjr.shanyushiyangtech.top

[D07] 切片 / 取子数组
来源：http://ozd.vehdjk.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://vmj.9152youxi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://lbd.xuanzx.com

JS:   arr.slice(1, 4);
来源：http://yoz.0kj1m.cn

TS:   arr.slice(1, 4);
来源：http://svm.zdbjq.cn

Java: list.subList(1, 4);
来源：http://war.xylfe.cn

Go:   arr[1:4]
来源：http://ibj.ybcxt.top

Ruby: arr[1, 3]
来源：http://eob.guannengcc.top


<!-- 参考信息 -->