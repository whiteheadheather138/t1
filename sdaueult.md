代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://mcs.xingfuxueyuan.xyz

PHP:  do { $i++; } while ($i < 10);
来源：http://vnp.daria6918.cn

JS:   do { i++; } while (i < 10);
来源：http://qxf.fengsongda.top

TS:   do { i++; } while (i < 10);
来源：http://xxh.0kj1m.cn

Java: do { i++; } while (i < 10);
来源：http://fzp.jianghu66.top

Go:   for { i++; if i >= 10 { break } }
来源：http://fmh.yongpay.top

Ruby: begin; i += 1; end while i < 10
来源：http://qgm.aibaodan.cn

C#:   do { i++; } while (i < 10);
来源：http://pxh.yonumen.top

[B09] break 与 continue
来源：http://eaa.zhaomingkeji.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://rhp.zhoulong.xyz

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://azj.hnxiangtu.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vvs.c1oappe.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xcf.jiagoushi.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://csx.shanyushiyangtech.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ayh.wangdashe.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://cwy.kuanghao11.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rla.mhx1999.top

[B10] 遍历同时拿索引
来源：http://vwa.yuanzhike.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://bid.yuanzhike.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://xwd.yvedp.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://rvu.zdbjq.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://crw.zhixingplan.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://xmk.kuanghao11.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wgp.ehwqpu.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://jit.cqqwz.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://gkk.jqgufenzy.top

[B11] 生成数字序列 / 区间
来源：http://tuw.ydzc1.top

Py:   list(range(0, 10, 2))
来源：http://smr.jinqigfzy.top

PHP:  range(0, 10, 2);
来源：http://otr.aizwys.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pac.zhiwuduotai.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://iaa.gzhubu.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ixs.guannengcc.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://lsf.yfazqb.com

Ruby: (0...10).step(2).to_a
来源：http://rax.yj20258.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://pwl.wangshuangyany.cn

[B12] 跳出多层循环
来源：http://gwv.yueranfly.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://gnt.jinyuanbaomall.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://vsb.jqgfzy.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://xtz.jqgufenzy.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://dij.sysykeji.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://god.yj20258888.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://vfw.yvedp.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ial.zhijiandao.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://exp.sxryk.cn

[B13] 判断是否为数字
来源：http://czi.xylfe.cn

Py:   isinstance(x, (int, float))
来源：http://tbg.yj202588.top

PHP:  is_numeric($x)
来源：http://crb.shangyingyoupin.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qyw.xuetiantiany.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ajp.andypj.xyz

Java: x instanceof Number
来源：http://jea.pengpengdd.cyou

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://fvi.yvedp.cn

Ruby: x.is_a?(Numeric)
来源：http://emf.cqqwz.cn

C#:   x is int or double or decimal
来源：http://drb.fehbvm.com

[B14] 判断值是否在集合内
来源：http://gbv.zdqjudy.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://xln.yonumen.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://smm.jiagoushi.top

JS:   [1, 2, 3].includes(x)
来源：http://dex.cdnleiting.top

TS:   [1, 2, 3].includes(x)
来源：http://pzg.vehdjk.com

Java: List.of(1, 2, 3).contains(x)
来源：http://wnj.cdnleiting.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ghf.sxryk.cn

Ruby: [1, 2, 3].include?(x)
来源：http://rkj.gogol.net.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://zdj.hysaishi.cn

[B15] 布尔运算与取反
来源：http://sqy.yj202588.top

Py:   a and b or not c
来源：http://bci.ctjpmb.com

PHP:  $a && $b || !$c
来源：http://blt.guannengcc.top

JS:   a && b || !c
来源：http://vpp.snrcjt.cn

TS:   a && b || !c
来源：http://gsd.hcnkem.com

Java: a && b || !c
来源：http://doa.shanyushiyangkeji.top

Go:   a && b || !c
来源：http://tod.gotoacloud.top

Ruby: a && b || !c
来源：http://zkz.cashguo.top

C#:   a && b || !c
来源：http://jil.chenlongwang.top

[B16] 卫语句：不满足条件提前返回
来源：http://rzs.andypj.xyz

Py:   if not data: return
来源：http://wlm.cashguo.top

PHP:  if (!$data) { return; }
来源：http://fby.nwbrower.top

JS:   if (!data) return;
来源：http://eqr.haohaochexian.top

TS:   if (!data) return;
来源：http://bxd.zhengqikj.top

Java: if (data == null) return;
来源：http://kle.snrcjt.cn

Go:   if data == nil { return }
来源：http://lnh.yj202588.top

Ruby: return if data.nil?
来源：http://egk.52xcode.cn

C#:   if (data == null) return;
来源：http://auh.yanxiufei.cn

================================================================================
来源：http://euw.tarul.cn

C. 函数与作用域
来源：http://wnm.gaohongyu789.top

================================================================================
来源：http://sjw.kuanghao11.cn

[C01] 定义函数
来源：http://ycb.feifeiyinyue.top

Py:   def add(a, b): return a + b
来源：http://vvd.redwolf501.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nzx.vqdsnc.cn

JS:   function add(a, b) { return a + b; }
来源：http://lbn.ctjpmb.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qka.epnwcf.com

Java: static int add(int a, int b) { return a + b; }
来源：http://yls.jiagoushi.top

Go:   func add(a, b int) int { return a + b }
来源：http://yoc.smart0.xyz

Ruby: def add(a, b); a + b; end
来源：http://pdn.yj202588.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://csh.zhijiandao.cn

[C02] 默认参数
来源：http://xnd.gzhubu.top

Py:   def greet(name="World"): return name
来源：http://vou.daria6918.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://pwa.sweek.top

JS:   function greet(name = "World") { return name; }
来源：http://ixt.shanyushiyangtech.top

TS:   function greet(name: string = "World") { return name; }
来源：http://ikn.yonumen.top

Java: // 无默认参数：方法重载或 Optional
来源：http://drk.jqgfzy.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://uwl.sysykeji.top

Ruby: def greet(name = "World") = name
来源：http://dcn.sufxvd.cn

C#:   string Greet(string name = "World") => name;
来源：http://efv.yanxiufei.cn

[C03] 可变参数
来源：http://cdg.yanxiufei.cn

Py:   def total(*args): return sum(args)
来源：http://nyq.gogol.net.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://bko.hongshengwenyu.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://gbx.bbcook.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ysg.zdqjudy.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://znp.birdmap.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://rmr.vehdjk.com

Ruby: def total(*nums); nums.sum; end
来源：http://vqv.xylfe.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://izm.sxryk.cn

[C04] 命名参数 / 关键字参数
来源：http://vcv.dashuyun.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://xcr.redwolf501.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ncp.hongshengwenyu.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://sgr.316326.xyz

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hfg.snrcjt.cn

Java: // 无：用 Builder 模式或 record
来源：http://guj.jiagoushi.top

Go:   // 无：用配置结构体参数
来源：http://xnm.iojbl.cn

Ruby: f(a: 1, b: 2)
来源：http://kjg.ydzc1.top

C#:   f(a: 1, b: 2)
来源：http://blv.xuanzx.com

[C05] 返回多个值
来源：http://ubp.gaohongyu789.top

Py:   return a, b
来源：http://col.cucudq.cn

PHP:  return [$a, $b];
来源：http://jgw.gaohongyu789.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://vhi.epnwcf.com

TS:   return { a, b };
来源：http://vsm.dianchejie.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://aug.yonumen.top

Go:   return a, b
来源：http://zuv.yangfankeji.com

Ruby: return a, b
来源：http://wru.havefunace.top

C#:   return (a, b);              // ValueTuple
来源：http://kvi.wangshuangyany.cn

[C06] 匿名函数 / lambda
来源：http://qwe.zhengqikj.top

Py:   square = lambda x: x * x
来源：http://vxi.tian-w.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://fgc.shanyushiyangtech.top

JS:   const square = x => x * x;
来源：http://pxg.guannengcc.top

TS:   const square = (x: number): number => x * x;
来源：http://aei.zhijiandao.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ruz.vehdjk.com

Go:   sq := func(x int) int { return x * x }
来源：http://abv.52xcode.cn

Ruby: square = ->(x) { x * x }
来源：http://xdr.andypj.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://xvz.hesvh.cn

[C07] 把函数作为参数传入
来源：http://ubt.cqqwz.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://aip.xuetiantiany.cn

PHP:  array_map("strtoupper", $arr);
来源：http://qnq.hywenlv.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://qvn.ehwqpu.com

TS:   arr.map(String)
来源：http://whw.vqdsnc.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://uzs.gaohongyu789.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://dae.hfpthk.cn

Ruby: arr.map(&:upcase)
来源：http://jgk.pengpengdd.cyou

C#:   arr.Select(s => s.ToUpper())
来源：http://cuh.hammf.cn

[C08] 闭包
来源：http://pwo.nwbrower.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://tyr.hcnkem.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://any.jinyuanbaomall.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://pva.shanyushiyangtech.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://qol.gaohongyu789.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://xkq.jqgfzy.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://xth.redwolf501.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://nwq.xinyue.icu

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://uae.52xcode.cn

[C09] 递归
来源：http://rib.jinqigufen.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://xvl.iojbl.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://lnp.yj20258.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://upp.meibo888.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cjt.xinyue.icu

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://bnf.pycfn.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://unx.tianlin.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://aqi.zhongyouzk.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hnu.sweek.top

[C10] 变量作用域
来源：http://xzv.shangyingyoupin.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qiz.jinghuilouyu.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://dja.guannengcc.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://imm.c1oappe.top

TS:   同 JS
来源：http://ggq.zhiwuduotai.top

Java: 方法内为块级作用域
来源：http://ods.jinghuilouyu.cn

Go:   花括号块级作用域
来源：http://srg.kuanghao11.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://cri.yonumen.top

C#:   块级作用域
来源：http://swn.ctjpmb.com

[C11] 模块导入与导出
来源：http://pqz.kuanghao11.cn

Py:   from module import func
来源：http://fzr.zhixingplan.top

PHP:  require "file.php";  或 use App\Service;
来源：http://ogv.yj20258888.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://mbo.sxryk.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://rdu.guannengcc.top

Java: import java.util.List;
来源：http://nwh.ctjpmb.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://fsb.dianchejie.cn

Ruby: require "json"; require_relative "./util"
来源：http://agt.bjfxy.top

C#:   using System.Text;
来源：http://ihd.0kj1m.cn

[C12] 立即执行函数 IIFE
来源：http://swu.ybcxt.top

Py:   (lambda: print("run"))()
来源：http://uss.fehbvm.com

PHP:  (function () { echo "run"; })();
来源：http://nfd.smart0.xyz

JS:   (() => { console.log("run"); })();
来源：http://err.shanyushiyangtech.top

TS:   (() => { console.log("run"); })();
来源：http://xcq.wangshuangyany.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://kig.fzhhl.top

Go:   func() { fmt.Println("run") }()
来源：http://dik.hesvh.cn

Ruby: -> { puts "run" }.call
来源：http://hhn.jinyuanbaomall.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://xpc.xuetiantiany.cn

[C13] 类型声明 / 类型注解
来源：http://bdb.cucudq.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://plb.yueranfly.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://aiv.daria6918.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hfg.ydjk.org.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qjx.hysaishi.cn

Java: int add(int a, int b) { return a + b; }
来源：http://vhi.tian-w.cn

Go:   func add(a, b int) int
来源：http://xnx.52xcode.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://slg.jyoumei.cn

C#:   int Add(int a, int b) => a + b;
来源：http://bqv.hnqzz.top

[C14] 泛型函数
来源：http://hbp.0kj1m.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://lle.fanxiaobao.xyz

PHP:  // 无泛型
来源：http://ivm.9152youxi.cn

JS:   // 无泛型
来源：http://mus.bbcook.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://tnk.jinqigfzy.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://flo.sxryk.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://gyg.quarkkingdee.top

Ruby: # 无泛型
来源：http://kog.svipenyu.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://egz.zhengqikj.top

[C15] 解构 / 展开参数
来源：http://wkw.shangyingyoupin.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://huk.aibaodan.cn

PHP:  [$a, $b] = $pair;
来源：http://tvx.yvedp.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wuu.hysaishi.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://dxe.jianghu66.top

Java: // 无解构
来源：http://mjy.sufxvd.cn

Go:   // 无解构
来源：http://sug.yonumen.top

Ruby: a, b = pair
来源：http://vdg.yj20258888.top

C#:   var (a, b) = pair;
来源：http://zej.yj202588.top

[C16] 函数 / 方法重载
来源：http://zae.meibo888.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://xeb.cdnleiting.top

PHP:  // 无重载
来源：http://pzo.dianchejie.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://pcz.birdmap.top

TS:   // 用联合类型或重载签名声明
来源：http://vek.yuxming.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://dur.ydjk.org.cn

Go:   // 无重载：用不同函数名
来源：http://tma.ehwqpu.com

Ruby: # 无重载：靠动态参数
来源：http://vrr.jqgufenzy.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://qmc.jinyuanbaomall.cn

================================================================================
来源：http://kns.nwbrower.top

D. 数组 / 列表 / 集合
来源：http://sqy.jiagoushi.top

================================================================================
来源：http://sle.jinqigfzy.top

[D01] 创建数组 / 列表
来源：http://ccq.tarul.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ahx.guowangkeji.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://crh.tian-w.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://sdj.svipenyu.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://sit.yj20258888.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://gqq.redwolf501.top

Go:   arr := []int{1, 2, 3}
来源：http://yff.jianghu66.top

Ruby: arr = [1, 2, 3]
来源：http://dqy.nanxuanxn.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://bve.yfazqb.com

[D02] 追加元素到末尾
来源：http://yba.jyoumei.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://vqb.cheryme.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://yve.c1oappe.top

JS:   arr.push(4);
来源：http://hln.gzhubu.top

TS:   arr.push(4);
来源：http://qcu.c1oappe.top

Java: list.add(4);
来源：http://lep.hywenlv.cn

Go:   arr = append(arr, 4)
来源：http://xrl.jqgfzy.top

Ruby: arr << 4; arr.push(5)
来源：http://abt.wangshuangyany.cn

C#:   list.Add(4);
来源：http://bfo.tianlin.xyz

[D03] 在指定位置插入元素
来源：http://nai.yueranfly.top

Py:   arr.insert(0, 0)
来源：http://uvn.fanxiaobao.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ccd.wangshuangyany.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://zhs.kuanghao11.cn

TS:   arr.splice(0, 0, 0);
来源：http://nbj.guowangkeji.top

Java: list.add(0, 0);
来源：http://dnr.sxryk.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ftc.daria6918.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://tch.jinyuanbaomall.cn

C#:   list.Insert(0, 0);
来源：http://pim.hcnkem.com

[D04] 删除元素
来源：http://abe.wangdashe.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://gax.snrcjt.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wjx.jlsjyb.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ehh.hcnkem.com

TS:   arr.splice(0, 1);
来源：http://jbz.pycfn.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ufb.chenzaomai.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://fmt.yueranfly.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://efd.sxryk.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ejj.xuetiantiany.cn

[D05] 访问与修改元素
来源：http://iwk.pycfn.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hjt.yonumen.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://pyf.gotoacloud.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://gjj.xingfuxueyuan.xyz

TS:   arr[0]; arr.at(-1);
来源：http://gqk.zhijiandao.cn

Java: list.get(0); list.set(0, 9);
来源：http://fqj.zdqjudy.top

Go:   arr[0]; arr[0] = 9
来源：http://bbj.jlsjyb.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://jfc.52xcode.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://vlp.gogol.net.cn

[D06] 数组长度
来源：http://npc.jyoumei.cn

Py:   len(arr)
来源：http://zmi.shanyushiyangtech.top

PHP:  count($arr);
来源：http://xug.yuxming.cn

JS:   arr.length
来源：http://vim.jlsjyb.cn

TS:   arr.length
来源：http://cav.zhongyouzk.top

Java: list.size();
来源：http://azw.yj20258.top

Go:   len(arr)
来源：http://swv.chenzaomai.com

Ruby: arr.length; arr.size
来源：http://hbr.nanxuanxn.top

C#:   list.Count;
来源：http://nbm.hywenlv.cn

[D07] 切片 / 取子数组
来源：http://jry.hfpthk.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hga.zhiwuduotai.top

PHP:  array_slice($arr, 1, 3);
来源：http://xby.gaohongyu789.top

JS:   arr.slice(1, 4);
来源：http://gdr.hnxiangtu.top

TS:   arr.slice(1, 4);
来源：http://nvr.9152youxi.cn

Java: list.subList(1, 4);
来源：http://yil.fengsongda.top

Go:   arr[1:4]
来源：http://ruw.shanyushiyangkeji.top

Ruby: arr[1, 3]
来源：http://ysw.yj202588.top

C#:   list.GetRange(1, 3);
来源：http://kcz.nanxinkj.top

[D08] 合并两个数组
来源：http://koj.havefunace.top

Py:   a + b;  a.extend(b)
来源：http://ara.yangfankeji.com

PHP:  array_merge($a, $b);
来源：http://ijr.yanxiufei.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://err.smart0.xyz

TS:   [...a, ...b];
来源：http://mxm.shuidangran.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://man.tanke756.top

Go:   append(a, b...)
来源：http://oed.mhx1999.top


<!-- 参考信息 -->