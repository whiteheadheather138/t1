代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://chy.yongpay.top

PHP:  do { $i++; } while ($i < 10);
来源：http://jvm.svipenyu.cn

JS:   do { i++; } while (i < 10);
来源：http://cty.yj20258888.top

TS:   do { i++; } while (i < 10);
来源：http://atj.hnqzz.top

Java: do { i++; } while (i < 10);
来源：http://tql.gotoacloud.top

Go:   for { i++; if i >= 10 { break } }
来源：http://maa.fengsongda.top

Ruby: begin; i += 1; end while i < 10
来源：http://ngu.hywenlv.cn

C#:   do { i++; } while (i < 10);
来源：http://thn.dianchejie.cn

[B09] break 与 continue
来源：http://oge.316326.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://rbi.mhx1999.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://fnt.yj202588.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://olh.0kj1m.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ggg.vehdjk.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ren.sweek.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://yum.52xcode.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://fqk.jianghu66.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lco.wangdashe.top

[B10] 遍历同时拿索引
来源：http://xpa.ydjk.org.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://rmy.xylfe.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://yrw.haohaochexian.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xxh.tian-w.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://exa.jinqigfzy.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://qtc.jlsjyb.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://oej.sysykeji.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://xss.52xcode.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://egi.316326.xyz

[B11] 生成数字序列 / 区间
来源：http://okd.52xcode.cn

Py:   list(range(0, 10, 2))
来源：http://vua.yongpay.top

PHP:  range(0, 10, 2);
来源：http://hva.ywan-chungtsiang.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://iqe.jqgfzy.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://imv.aibaodan.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ddx.zycfv.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hfr.xuanzx.com

Ruby: (0...10).step(2).to_a
来源：http://tuo.vqdsnc.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://cyh.vehdjk.com

[B12] 跳出多层循环
来源：http://zpi.snrcjt.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://acp.daxiang520.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://pbp.gzhubu.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://bqn.ppjwa.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ain.shanyushiyangkeji.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://uft.yvedp.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://bjj.cheryme.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hcq.zhixingplan.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://qgw.jyoumei.cn

[B13] 判断是否为数字
来源：http://wph.zdbjq.cn

Py:   isinstance(x, (int, float))
来源：http://hba.xinyue.icu

PHP:  is_numeric($x)
来源：http://opg.yongpay.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rym.hnqzz.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qov.snrcjt.cn

Java: x instanceof Number
来源：http://lvt.vehdjk.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://bem.aizwys.cn

Ruby: x.is_a?(Numeric)
来源：http://glh.chenlongwang.top

C#:   x is int or double or decimal
来源：http://lro.daria6918.cn

[B14] 判断值是否在集合内
来源：http://tdg.shanyushiyangtech.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://bqf.tarul.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://boe.cucudq.cn

JS:   [1, 2, 3].includes(x)
来源：http://xln.xuetiantiany.cn

TS:   [1, 2, 3].includes(x)
来源：http://nqd.cdnleiting.top

Java: List.of(1, 2, 3).contains(x)
来源：http://etx.hnxiangtu.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://zll.shzxlz.cn

Ruby: [1, 2, 3].include?(x)
来源：http://veh.jqgfzy.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://gwj.tian-w.cn

[B15] 布尔运算与取反
来源：http://ygg.52xcode.cn

Py:   a and b or not c
来源：http://edg.svipenyu.cn

PHP:  $a && $b || !$c
来源：http://amu.zhoulong.xyz

JS:   a && b || !c
来源：http://vxs.xuetiantiany.cn

TS:   a && b || !c
来源：http://yke.nanxuanxn.top

Java: a && b || !c
来源：http://wsn.hnqzz.top

Go:   a && b || !c
来源：http://pvr.aizwys.cn

Ruby: a && b || !c
来源：http://lvg.vqdsnc.cn

C#:   a && b || !c
来源：http://dqx.daria6918.cn

[B16] 卫语句：不满足条件提前返回
来源：http://xdh.fzhhl.top

Py:   if not data: return
来源：http://ucu.xingfuxueyuan.xyz

PHP:  if (!$data) { return; }
来源：http://vhs.guannengcc.top

JS:   if (!data) return;
来源：http://kfd.sysykeji.top

TS:   if (!data) return;
来源：http://alv.yuxming.cn

Java: if (data == null) return;
来源：http://lro.316326.xyz

Go:   if data == nil { return }
来源：http://hhs.zhongyouzk.top

Ruby: return if data.nil?
来源：http://yhc.bjfxy.top

C#:   if (data == null) return;
来源：http://pfk.hcnkem.com

================================================================================
来源：http://pau.316326.xyz

C. 函数与作用域
来源：http://evy.zhengqikj.top

================================================================================
来源：http://ekt.dianchejie.cn

[C01] 定义函数
来源：http://tqd.guowangkeji.top

Py:   def add(a, b): return a + b
来源：http://blj.hnqzz.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://twf.tarul.cn

JS:   function add(a, b) { return a + b; }
来源：http://ryp.uphjek.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cqx.jinghuilouyu.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ggp.fanxiaobao.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://lze.gotoacloud.top

Ruby: def add(a, b); a + b; end
来源：http://xvi.shzxlz.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://fxl.yangfankeji.com

[C02] 默认参数
来源：http://wkw.sysykeji.top

Py:   def greet(name="World"): return name
来源：http://gon.tarul.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://elt.vqdsnc.cn

JS:   function greet(name = "World") { return name; }
来源：http://dji.gogol.net.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://sjg.jqgufenzy.top

Java: // 无默认参数：方法重载或 Optional
来源：http://ypo.shanyushiyangtech.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wqu.ydzc1.top

Ruby: def greet(name = "World") = name
来源：http://ihf.316326.xyz

C#:   string Greet(string name = "World") => name;
来源：http://muk.ehwqpu.com

[C03] 可变参数
来源：http://bfv.yvedp.cn

Py:   def total(*args): return sum(args)
来源：http://wmd.ybcxt.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://idx.ivvv.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://lcc.yfazqb.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mwq.yfazqb.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://tnj.jqgufenzy.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wbm.xingfuxueyuan.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://zvd.fengsongda.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://gun.dashuyun.cn

[C04] 命名参数 / 关键字参数
来源：http://vna.gogol.net.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://vru.uphjek.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://muu.dianchejie.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wsk.hywenlv.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://rpi.fzhhl.top

Java: // 无：用 Builder 模式或 record
来源：http://blc.ehwqpu.com

Go:   // 无：用配置结构体参数
来源：http://jie.yuanzhike.top

Ruby: f(a: 1, b: 2)
来源：http://njq.zdbjq.cn

C#:   f(a: 1, b: 2)
来源：http://qrh.ybcxt.top

[C05] 返回多个值
来源：http://aas.nanxinkj.top

Py:   return a, b
来源：http://rpj.hywenlv.cn

PHP:  return [$a, $b];
来源：http://cky.yongpay.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://dke.jinqigfzy.top

TS:   return { a, b };
来源：http://xlf.hywenlv.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://sdw.zhaomingkeji.xyz

Go:   return a, b
来源：http://fif.zdbjq.cn

Ruby: return a, b
来源：http://ybj.xingfuxueyuan.xyz

C#:   return (a, b);              // ValueTuple
来源：http://wmt.vehdjk.com

[C06] 匿名函数 / lambda
来源：http://mci.fktsv.cn

Py:   square = lambda x: x * x
来源：http://qop.jinyuanbaomall.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://gww.gotoacloud.top

JS:   const square = x => x * x;
来源：http://elp.ywan-chungtsiang.top

TS:   const square = (x: number): number => x * x;
来源：http://nfn.zhongyouzk.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://tht.yuxming.cn

Go:   sq := func(x int) int { return x * x }
来源：http://zcl.zhijiandao.cn

Ruby: square = ->(x) { x * x }
来源：http://dao.daria6918.cn

C#:   Func<int, int> square = x => x * x;
来源：http://otm.yanxiufei.cn

[C07] 把函数作为参数传入
来源：http://dae.havefunace.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://usw.smart0.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://hri.yvedp.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wmo.sxryk.cn

TS:   arr.map(String)
来源：http://ilg.feifeiyinyue.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://rzm.ywan-chungtsiang.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qov.wangdashe.top

Ruby: arr.map(&:upcase)
来源：http://tpo.fehbvm.com

C#:   arr.Select(s => s.ToUpper())
来源：http://lpq.shuidangran.top

[C08] 闭包
来源：http://iep.xinyue.icu

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qjj.vehdjk.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hqs.andypj.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://cut.fzhhl.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://njq.ywan-chungtsiang.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://rup.hcnkem.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://gwz.fengsongda.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://iwx.jinghuilouyu.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://dtd.tarul.cn

[C09] 递归
来源：http://nbb.316326.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://fct.dianchejie.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mkz.chenzaomai.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vnu.yueranfly.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mvh.ivvv.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ytm.guannengcc.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://tlx.fzhhl.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://lhn.vqdsnc.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://kyi.xylfe.cn

[C10] 变量作用域
来源：http://eam.jinyuanbaomall.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wvh.kuanghao11.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://xjb.yueranfly.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://bxo.ydjk.org.cn

TS:   同 JS
来源：http://gwh.aizwys.cn

Java: 方法内为块级作用域
来源：http://svt.jinqigufen.top

Go:   花括号块级作用域
来源：http://vqx.cqqwz.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mhx.cheryme.top

C#:   块级作用域
来源：http://vfz.shuidangran.top

[C11] 模块导入与导出
来源：http://oyo.zhoulong.xyz

Py:   from module import func
来源：http://wzw.316326.xyz

PHP:  require "file.php";  或 use App\Service;
来源：http://lzo.zhengqikj.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://scg.sufxvd.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://utt.wangshuangyany.cn

Java: import java.util.List;
来源：http://sxc.ppjwa.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://vkx.yj20258888.top

Ruby: require "json"; require_relative "./util"
来源：http://sec.hcnkem.com

C#:   using System.Text;
来源：http://bsm.yuxming.cn

[C12] 立即执行函数 IIFE
来源：http://xgp.shuidangran.top

Py:   (lambda: print("run"))()
来源：http://mqk.gzhubu.top

PHP:  (function () { echo "run"; })();
来源：http://fxi.hnxiangtu.top

JS:   (() => { console.log("run"); })();
来源：http://ckr.havefunace.top

TS:   (() => { console.log("run"); })();
来源：http://gxb.xziqi.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://pkh.zhongyouzk.top

Go:   func() { fmt.Println("run") }()
来源：http://emi.aizwys.cn

Ruby: -> { puts "run" }.call
来源：http://hbq.316326.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://thu.jinyuanbaomall.cn

[C13] 类型声明 / 类型注解
来源：http://tqv.zdbjq.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ukz.fanxiaobao.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ijn.sxryk.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://lvu.yonumen.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bhf.zhongyouzk.top

Java: int add(int a, int b) { return a + b; }
来源：http://lil.0kj1m.cn

Go:   func add(a, b int) int
来源：http://equ.epnwcf.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://grf.havefunace.top

C#:   int Add(int a, int b) => a + b;
来源：http://ecn.fanxiaobao.xyz

[C14] 泛型函数
来源：http://ojf.hfpthk.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://smc.fanxiaobao.xyz

PHP:  // 无泛型
来源：http://uho.birdmap.top

JS:   // 无泛型
来源：http://drq.chenlongwang.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://kjg.gotoacloud.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://akx.xuetiantiany.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://pvq.tian-w.cn

Ruby: # 无泛型
来源：http://ayf.sxryk.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://rwy.vehdjk.com

[C15] 解构 / 展开参数
来源：http://qbu.snrcjt.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://cam.c1oappe.top

PHP:  [$a, $b] = $pair;
来源：http://ocy.ehwqpu.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://lnu.ivvv.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://cnc.ywan-chungtsiang.top

Java: // 无解构
来源：http://bky.tarul.cn

Go:   // 无解构
来源：http://mps.jinqigufen.top

Ruby: a, b = pair
来源：http://vtm.jlsjyb.cn

C#:   var (a, b) = pair;
来源：http://yvj.yuanzhike.top

[C16] 函数 / 方法重载
来源：http://fqi.daxiang520.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://zii.jinyuanbaomall.cn

PHP:  // 无重载
来源：http://hiq.iojbl.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://fkn.hnqzz.top

TS:   // 用联合类型或重载签名声明
来源：http://qjj.pycfn.com

Java: void f(int a) {}  void f(String a) {}
来源：http://qpi.shzxlz.cn

Go:   // 无重载：用不同函数名
来源：http://rdz.nwbrower.top

Ruby: # 无重载：靠动态参数
来源：http://isq.ctjpmb.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://tcs.daria6918.cn

================================================================================
来源：http://rhi.jqgfzy.top

D. 数组 / 列表 / 集合
来源：http://gus.kuanghao11.cn

================================================================================
来源：http://ssv.yj202588.top

[D01] 创建数组 / 列表
来源：http://gbc.sweek.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://rbb.pengpengdd.cyou

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mji.andypj.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://snf.xuetiantiany.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://nup.hysaishi.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://jfp.hysaishi.cn

Go:   arr := []int{1, 2, 3}
来源：http://oop.tarul.cn

Ruby: arr = [1, 2, 3]
来源：http://kmj.chenjidiqi.icu

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hmy.yangfankeji.com

[D02] 追加元素到末尾
来源：http://noe.yuxming.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://jsw.shanyushiyangkeji.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baj.gaohongyu789.top

JS:   arr.push(4);
来源：http://oip.bbcook.cn

TS:   arr.push(4);
来源：http://gde.cqqwz.cn

Java: list.add(4);
来源：http://bqg.zhixingplan.top

Go:   arr = append(arr, 4)
来源：http://cgs.ydjk.org.cn

Ruby: arr << 4; arr.push(5)
来源：http://int.guowangkeji.top

C#:   list.Add(4);
来源：http://hac.sjlbkw.cn

[D03] 在指定位置插入元素
来源：http://izk.quarkkingdee.top

Py:   arr.insert(0, 0)
来源：http://fya.chenlongwang.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://zhq.sweek.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://cjn.fengsongda.top

TS:   arr.splice(0, 0, 0);
来源：http://jfi.jlsjyb.cn

Java: list.add(0, 0);
来源：http://hox.dashuyun.cn

Go:   arr = append([]int{0}, arr...)
来源：http://uue.fktsv.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://jjh.tian-w.cn

C#:   list.Insert(0, 0);
来源：http://jqp.xinyue.icu

[D04] 删除元素
来源：http://bnr.yonumen.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hmc.zhixingplan.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ulr.mhx1999.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ckd.andypj.xyz

TS:   arr.splice(0, 1);
来源：http://als.nanxuanxn.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://yqh.uphjek.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://lxc.tian-w.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://gkd.zhoulong.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://dca.fengsongda.top

[D05] 访问与修改元素
来源：http://rvb.shzxlz.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://euk.hammf.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wud.iojbl.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://jeg.jqgufenzy.top

TS:   arr[0]; arr.at(-1);
来源：http://sdl.gzhubu.top

Java: list.get(0); list.set(0, 9);
来源：http://jso.daria6918.cn

Go:   arr[0]; arr[0] = 9
来源：http://ybw.epnwcf.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://kwk.nwbrower.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://yqy.zdqjudy.top

[D06] 数组长度
来源：http://zqp.ywan-chungtsiang.top

Py:   len(arr)
来源：http://chg.gzhubu.top

PHP:  count($arr);
来源：http://ksk.hongshengwenyu.top

JS:   arr.length
来源：http://sxh.yongpay.top

TS:   arr.length
来源：http://szq.epnwcf.com

Java: list.size();
来源：http://are.zycfv.cn

Go:   len(arr)
来源：http://ulb.tarul.cn

Ruby: arr.length; arr.size
来源：http://ehi.wangshuangyany.cn

C#:   list.Count;
来源：http://uob.shangyingyoupin.top

[D07] 切片 / 取子数组
来源：http://jaz.iojbl.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://vls.cucudq.cn

PHP:  array_slice($arr, 1, 3);
来源：http://bqu.sysykeji.top

JS:   arr.slice(1, 4);
来源：http://mfw.yfazqb.com

TS:   arr.slice(1, 4);
来源：http://lum.zhaomingkeji.xyz

Java: list.subList(1, 4);
来源：http://cji.jlsjyb.cn

Go:   arr[1:4]
来源：http://qdj.cdnleiting.top

Ruby: arr[1, 3]
来源：http://kaa.ybcxt.top

C#:   list.GetRange(1, 3);
来源：http://lbw.guannengcc.top

[D08] 合并两个数组
来源：http://pus.chenlongwang.top

Py:   a + b;  a.extend(b)
来源：http://rfr.gotoacloud.top

PHP:  array_merge($a, $b);
来源：http://wpx.nanxuanxn.top

JS:   [...a, ...b];  a.concat(b);
来源：http://edh.cashguo.top

TS:   [...a, ...b];
来源：http://hwe.aizwys.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://jku.xinyue.icu

Go:   append(a, b...)
来源：http://aax.zycfv.cn


<!-- 参考信息 -->