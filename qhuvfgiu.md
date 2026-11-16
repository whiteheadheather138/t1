代发 wailian999

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://foz.yanxiufei.cn

Ruby: while i < 10; i += 1; end
来源：http://vnq.epnwcf.com

C#:   while (i < 10) { i++; }
来源：http://epv.yanxiufei.cn

[B08] do-while（至少执行一次）
来源：http://pvg.gotoacloud.top

Py:   # 无 do-while：用 while True + break
来源：http://sbl.yonumen.top

PHP:  do { $i++; } while ($i < 10);
来源：http://emh.feifeiyinyue.top

JS:   do { i++; } while (i < 10);
来源：http://yfj.tanke756.top

TS:   do { i++; } while (i < 10);
来源：http://sbo.smart0.xyz

Java: do { i++; } while (i < 10);
来源：http://sjx.zdbjq.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://cwi.yuxming.cn

Ruby: begin; i += 1; end while i < 10
来源：http://qop.sweek.top

C#:   do { i++; } while (i < 10);
来源：http://tih.jqgufenzy.top

[B09] break 与 continue
来源：http://woa.yueranfly.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://vgf.jinyuanbaomall.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://jfp.pycfn.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mce.zdbjq.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yvg.nanxinkj.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://urb.jiagoushi.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://szo.zhiwuduotai.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xds.shanyushiyangtech.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lxs.shzxlz.cn

[B10] 遍历同时拿索引
来源：http://bzp.zhaomingkeji.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://cel.cqqwz.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://xys.tarul.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://tbv.zhengqikj.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://bze.nanxuanxn.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://kxi.havefunace.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://btf.zhijiandao.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://xnp.snrcjt.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://pvg.chenzaomai.com

[B11] 生成数字序列 / 区间
来源：http://ugk.cheryme.top

Py:   list(range(0, 10, 2))
来源：http://kgn.tanke756.top

PHP:  range(0, 10, 2);
来源：http://rgi.cdnleiting.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://emr.shanyushiyangtech.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jjb.zhijiandao.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://jmn.hnqzz.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://zvx.ydjk.org.cn

Ruby: (0...10).step(2).to_a
来源：http://klx.haohaochexian.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://xnu.zhixingplan.top

[B12] 跳出多层循环
来源：http://oxo.aizwys.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://pom.shzxlz.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://pxr.shuidangran.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://zvf.fanxiaobao.xyz

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://brk.guannengcc.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://yyb.yangfankeji.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ynj.yanxiufei.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://cgl.yj202588.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://lgh.sufxvd.cn

[B13] 判断是否为数字
来源：http://gtu.shangyingyoupin.top

Py:   isinstance(x, (int, float))
来源：http://sqv.epnwcf.com

PHP:  is_numeric($x)
来源：http://smj.shzxlz.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kdo.vehdjk.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ihf.ehwqpu.com

Java: x instanceof Number
来源：http://klu.jinqigfzy.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://jjx.uphjek.com

Ruby: x.is_a?(Numeric)
来源：http://ghd.dashuyun.cn

C#:   x is int or double or decimal
来源：http://hgv.yangfankeji.com

[B14] 判断值是否在集合内
来源：http://vpw.xziqi.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ogq.ppjwa.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ycx.zdqjudy.top

JS:   [1, 2, 3].includes(x)
来源：http://syn.xingfuxueyuan.xyz

TS:   [1, 2, 3].includes(x)
来源：http://dsc.meibo888.top

Java: List.of(1, 2, 3).contains(x)
来源：http://djz.yj202588.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://fgs.hcnkem.com

Ruby: [1, 2, 3].include?(x)
来源：http://fdd.yuxming.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://rpa.xinyue.icu

[B15] 布尔运算与取反
来源：http://dxz.tanke756.top

Py:   a and b or not c
来源：http://pnk.shzxlz.cn

PHP:  $a && $b || !$c
来源：http://nlq.gaohongyu789.top

JS:   a && b || !c
来源：http://eeb.jqgfzy.top

TS:   a && b || !c
来源：http://aum.cheryme.top

Java: a && b || !c
来源：http://nrg.zhijiandao.cn

Go:   a && b || !c
来源：http://hya.dianchejie.cn

Ruby: a && b || !c
来源：http://cpi.sysykeji.top

C#:   a && b || !c
来源：http://wak.ehwqpu.com

[B16] 卫语句：不满足条件提前返回
来源：http://ufr.pengpengdd.cyou

Py:   if not data: return
来源：http://mok.yongpay.top

PHP:  if (!$data) { return; }
来源：http://hmv.jiagoushi.top

JS:   if (!data) return;
来源：http://cpf.tarul.cn

TS:   if (!data) return;
来源：http://tqk.birdmap.top

Java: if (data == null) return;
来源：http://ier.yuxming.cn

Go:   if data == nil { return }
来源：http://ztq.zhixingplan.top

Ruby: return if data.nil?
来源：http://wch.cashguo.top

C#:   if (data == null) return;
来源：http://trx.yj20258888.top

================================================================================
来源：http://cvb.fanxiaobao.xyz

C. 函数与作用域
来源：http://xqg.chenlongwang.top

================================================================================
来源：http://qdr.jinghuilouyu.cn

[C01] 定义函数
来源：http://zec.shanyushiyangkeji.top

Py:   def add(a, b): return a + b
来源：http://fyf.chenjidiqi.icu

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xgk.ydzc1.top

JS:   function add(a, b) { return a + b; }
来源：http://sba.epnwcf.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gfe.yanxiufei.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://kal.epnwcf.com

Go:   func add(a, b int) int { return a + b }
来源：http://qjb.zhiwuduotai.top

Ruby: def add(a, b); a + b; end
来源：http://yyb.ctjpmb.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://cos.haohaochexian.top

[C02] 默认参数
来源：http://tah.svipenyu.cn

Py:   def greet(name="World"): return name
来源：http://mzu.hysaishi.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://xjb.fanxiaobao.xyz

JS:   function greet(name = "World") { return name; }
来源：http://dif.uphjek.com

TS:   function greet(name: string = "World") { return name; }
来源：http://heb.yonumen.top

Java: // 无默认参数：方法重载或 Optional
来源：http://lfp.fehbvm.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://jty.ywan-chungtsiang.top

Ruby: def greet(name = "World") = name
来源：http://cpw.smart0.xyz

C#:   string Greet(string name = "World") => name;
来源：http://jlp.epnwcf.com

[C03] 可变参数
来源：http://gao.cdnleiting.top

Py:   def total(*args): return sum(args)
来源：http://pwf.jyoumei.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://vtc.fanxiaobao.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ezb.xuanzx.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://iqd.jinqigufen.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://juu.yfazqb.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://nhp.ydjk.org.cn

Ruby: def total(*nums); nums.sum; end
来源：http://fsc.zhongyouzk.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zly.xziqi.cn

[C04] 命名参数 / 关键字参数
来源：http://blo.gotoacloud.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://qxp.yongpay.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://dhb.0kj1m.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://byy.xylfe.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://lcg.ehwqpu.com

Java: // 无：用 Builder 模式或 record
来源：http://lmc.yvedp.cn

Go:   // 无：用配置结构体参数
来源：http://oat.xylfe.cn

Ruby: f(a: 1, b: 2)
来源：http://tgt.yuanzhike.top

C#:   f(a: 1, b: 2)
来源：http://pca.cqqwz.cn

[C05] 返回多个值
来源：http://nyh.c1oappe.top

Py:   return a, b
来源：http://yud.gogol.net.cn

PHP:  return [$a, $b];
来源：http://jtl.sweek.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://ezx.daxiang520.top

TS:   return { a, b };
来源：http://rwa.redwolf501.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://fyy.0kj1m.cn

Go:   return a, b
来源：http://ryv.gaohongyu789.top

Ruby: return a, b
来源：http://xlo.pengpengdd.cyou

C#:   return (a, b);              // ValueTuple
来源：http://luh.gzhubu.top

[C06] 匿名函数 / lambda
来源：http://eee.xuanzx.com

Py:   square = lambda x: x * x
来源：http://umm.yj20258.top

PHP:  $square = fn($x) => $x * $x;
来源：http://ubl.shzxlz.cn

JS:   const square = x => x * x;
来源：http://dzv.jianghu66.top

TS:   const square = (x: number): number => x * x;
来源：http://uro.vehdjk.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mjf.fktsv.cn

Go:   sq := func(x int) int { return x * x }
来源：http://qkq.hywenlv.cn

Ruby: square = ->(x) { x * x }
来源：http://hkj.nwbrower.top

C#:   Func<int, int> square = x => x * x;
来源：http://zxc.gogol.net.cn

[C07] 把函数作为参数传入
来源：http://yxg.xuanzx.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ijn.c1oappe.top

PHP:  array_map("strtoupper", $arr);
来源：http://xip.hongshengwenyu.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://jtk.52xcode.cn

TS:   arr.map(String)
来源：http://pwl.cashguo.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://gxc.hesvh.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://kym.iojbl.cn

Ruby: arr.map(&:upcase)
来源：http://brd.sweek.top

C#:   arr.Select(s => s.ToUpper())
来源：http://qml.dashuyun.cn

[C08] 闭包
来源：http://hir.cucudq.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hob.ydzc1.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://psc.9152youxi.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://sru.snrcjt.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ttq.gogol.net.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ect.aibaodan.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://xvz.ydzc1.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://oql.yj20258888.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://nai.zdqjudy.top

[C09] 递归
来源：http://uwi.shanyushiyangkeji.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://pfr.sysykeji.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://kec.aizwys.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://axo.xinyue.icu

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qhp.jqgufenzy.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://kjo.kuanghao11.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://lvv.cqqwz.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mua.yj20258888.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mwu.hammf.cn

[C10] 变量作用域
来源：http://bao.hfpthk.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mwt.epnwcf.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://knh.xuetiantiany.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://enm.jqgufenzy.top

TS:   同 JS
来源：http://uog.yuxming.cn

Java: 方法内为块级作用域
来源：http://cwz.jqgufenzy.top

Go:   花括号块级作用域
来源：http://uyr.ybcxt.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://amt.ydzc1.top

C#:   块级作用域
来源：http://izq.zycfv.cn

[C11] 模块导入与导出
来源：http://ckz.wangdashe.top

Py:   from module import func
来源：http://dly.daria6918.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://tvc.uphjek.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://qnt.fengsongda.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://bts.cucudq.cn

Java: import java.util.List;
来源：http://hyd.jyoumei.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mty.jianghu66.top

Ruby: require "json"; require_relative "./util"
来源：http://bof.yuanzhike.top

C#:   using System.Text;
来源：http://xzl.yanxiufei.cn

[C12] 立即执行函数 IIFE
来源：http://fog.guannengcc.top

Py:   (lambda: print("run"))()
来源：http://new.gogol.net.cn

PHP:  (function () { echo "run"; })();
来源：http://oom.tanke756.top

JS:   (() => { console.log("run"); })();
来源：http://pkz.hongshengwenyu.top

TS:   (() => { console.log("run"); })();
来源：http://xoo.tianlin.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://fry.jqgufenzy.top

Go:   func() { fmt.Println("run") }()
来源：http://yte.hesvh.cn

Ruby: -> { puts "run" }.call
来源：http://wpg.fengsongda.top

C#:   // 无 IIFE：用静态构造函数
来源：http://evx.hnqzz.top

[C13] 类型声明 / 类型注解
来源：http://nms.zhijiandao.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://cmt.yongpay.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ncx.yj202588.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://rkl.0kj1m.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fud.dashuyun.cn

Java: int add(int a, int b) { return a + b; }
来源：http://tnj.shanyushiyangtech.top

Go:   func add(a, b int) int
来源：http://xxp.yvedp.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ato.snrcjt.cn

C#:   int Add(int a, int b) => a + b;
来源：http://hnj.yanxiufei.cn

[C14] 泛型函数
来源：http://eyq.yfazqb.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ptx.zhiwuduotai.top

PHP:  // 无泛型
来源：http://uwu.yvedp.cn

JS:   // 无泛型
来源：http://lot.nanxinkj.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://fwn.smart0.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://rpc.jqgfzy.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://cqv.ydjk.org.cn

Ruby: # 无泛型
来源：http://dac.hysaishi.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mbd.fzhhl.top

[C15] 解构 / 展开参数
来源：http://ary.vehdjk.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://nhn.snrcjt.cn

PHP:  [$a, $b] = $pair;
来源：http://wwz.yj20258888.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://paz.shanyushiyangtech.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ttb.fanxiaobao.xyz

Java: // 无解构
来源：http://zee.shangyingyoupin.top

Go:   // 无解构
来源：http://gzf.cheryme.top

Ruby: a, b = pair
来源：http://hts.wangshuangyany.cn

C#:   var (a, b) = pair;
来源：http://dny.zhaomingkeji.xyz

[C16] 函数 / 方法重载
来源：http://ubd.mhx1999.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hkl.cucudq.cn

PHP:  // 无重载
来源：http://jof.yuxming.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://uhz.hfpthk.cn

TS:   // 用联合类型或重载签名声明
来源：http://tsj.yongpay.top

Java: void f(int a) {}  void f(String a) {}
来源：http://xnv.gaohongyu789.top

Go:   // 无重载：用不同函数名
来源：http://bbf.chenlongwang.top

Ruby: # 无重载：靠动态参数
来源：http://ugq.pengpengdd.cyou

C#:   void F(int a) {}  void F(string a) {}
来源：http://vsq.shuidangran.top

================================================================================
来源：http://qff.aibaodan.cn

D. 数组 / 列表 / 集合
来源：http://bqs.uphjek.com

================================================================================
来源：http://hdm.kuanghao11.cn

[D01] 创建数组 / 列表
来源：http://roq.kuanghao11.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ssz.52xcode.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://htd.aibaodan.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://vyv.hysaishi.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://klm.zhixingplan.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ehn.gotoacloud.top

Go:   arr := []int{1, 2, 3}
来源：http://tox.yonumen.top

Ruby: arr = [1, 2, 3]
来源：http://wrd.gzhubu.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://yae.havefunace.top

[D02] 追加元素到末尾
来源：http://uht.yvedp.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://sel.sysykeji.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://bgq.feifeiyinyue.top

JS:   arr.push(4);
来源：http://msv.hongshengwenyu.top

TS:   arr.push(4);
来源：http://dya.316326.xyz

Java: list.add(4);
来源：http://opb.quarkkingdee.top

Go:   arr = append(arr, 4)
来源：http://zym.xziqi.cn

Ruby: arr << 4; arr.push(5)
来源：http://eot.tian-w.cn

C#:   list.Add(4);
来源：http://rrf.tianlin.xyz

[D03] 在指定位置插入元素
来源：http://yyc.haohaochexian.top

Py:   arr.insert(0, 0)
来源：http://egb.yvedp.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://nlf.yangfankeji.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://qnc.jinqigufen.top

TS:   arr.splice(0, 0, 0);
来源：http://ulu.jinqigfzy.top

Java: list.add(0, 0);
来源：http://yya.bjfxy.top

Go:   arr = append([]int{0}, arr...)
来源：http://gew.hcnkem.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mzl.xinyue.icu

C#:   list.Insert(0, 0);
来源：http://fxp.xylfe.cn

[D04] 删除元素
来源：http://zjs.zycfv.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://zfc.yuxming.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://vcy.hysaishi.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://oah.hfpthk.cn

TS:   arr.splice(0, 1);
来源：http://suu.gzhubu.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://cmj.jqgufenzy.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://rhr.redwolf501.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://lhx.jinyuanbaomall.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://akz.iojbl.cn

[D05] 访问与修改元素
来源：http://uvq.hcnkem.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://skj.quarkkingdee.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://xld.pengpengdd.cyou

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://gih.nanxuanxn.top

TS:   arr[0]; arr.at(-1);
来源：http://frr.fktsv.cn

Java: list.get(0); list.set(0, 9);
来源：http://tvp.jinyuanbaomall.cn

Go:   arr[0]; arr[0] = 9
来源：http://frb.svipenyu.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://iip.jianghu66.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://lot.fktsv.cn

[D06] 数组长度
来源：http://qko.xuanzx.com

Py:   len(arr)
来源：http://ips.andypj.xyz

PHP:  count($arr);
来源：http://acv.quarkkingdee.top

JS:   arr.length
来源：http://zvb.fehbvm.com

TS:   arr.length
来源：http://qhl.chenlongwang.top

Java: list.size();
来源：http://yzv.fehbvm.com

Go:   len(arr)
来源：http://bug.hywenlv.cn

Ruby: arr.length; arr.size
来源：http://spj.guowangkeji.top

C#:   list.Count;
来源：http://knm.shanyushiyangtech.top

[D07] 切片 / 取子数组
来源：http://snb.0kj1m.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://yit.zdqjudy.top

PHP:  array_slice($arr, 1, 3);
来源：http://ofm.gzhubu.top

JS:   arr.slice(1, 4);
来源：http://njq.xinyue.icu

TS:   arr.slice(1, 4);
来源：http://dxh.gogol.net.cn

Java: list.subList(1, 4);
来源：http://iyh.cqqwz.cn

Go:   arr[1:4]
来源：http://qdb.zhixingplan.top

Ruby: arr[1, 3]
来源：http://cjg.zhixingplan.top

C#:   list.GetRange(1, 3);
来源：http://zmg.hongshengwenyu.top

[D08] 合并两个数组
来源：http://jmc.uphjek.com

Py:   a + b;  a.extend(b)
来源：http://ome.zdqjudy.top

PHP:  array_merge($a, $b);
来源：http://grp.zhongyouzk.top


<!-- 参考信息 -->