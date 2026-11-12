代发 wailian999

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://npw.meibo888.top

Ruby: while i < 10; i += 1; end
来源：http://rut.yj20258888.top

C#:   while (i < 10) { i++; }
来源：http://vvy.gogol.net.cn

[B08] do-while（至少执行一次）
来源：http://wxj.jinghuilouyu.cn

Py:   # 无 do-while：用 while True + break
来源：http://oxt.yfazqb.com

PHP:  do { $i++; } while ($i < 10);
来源：http://thf.zycfv.cn

JS:   do { i++; } while (i < 10);
来源：http://emt.hesvh.cn

TS:   do { i++; } while (i < 10);
来源：http://kxy.cqqwz.cn

Java: do { i++; } while (i < 10);
来源：http://wbb.zhaomingkeji.xyz

Go:   for { i++; if i >= 10 { break } }
来源：http://eve.gaohongyu789.top

Ruby: begin; i += 1; end while i < 10
来源：http://xcw.epnwcf.com

C#:   do { i++; } while (i < 10);
来源：http://vhd.sjlbkw.cn

[B09] break 与 continue
来源：http://dnj.mhx1999.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ebh.sjlbkw.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://kja.zycfv.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tlg.ctjpmb.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fmk.pengpengdd.cyou

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xzw.nanxuanxn.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ufa.pycfn.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://itk.daxiang520.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yua.tian-w.cn

[B10] 遍历同时拿索引
来源：http://vzt.birdmap.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://xlq.shzxlz.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://dpg.fzhhl.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xzc.hesvh.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://lqz.hnqzz.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://oie.iojbl.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://xfn.chenlongwang.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://kdb.52xcode.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mtt.hysaishi.cn

[B11] 生成数字序列 / 区间
来源：http://zyj.c1oappe.top

Py:   list(range(0, 10, 2))
来源：http://mrf.yonumen.top

PHP:  range(0, 10, 2);
来源：http://nzy.xuetiantiany.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://upi.zhijiandao.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ihs.xinyue.icu

Java: IntStream.range(0, 10).boxed().toList()
来源：http://nha.kuanghao11.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://eih.xuetiantiany.cn

Ruby: (0...10).step(2).to_a
来源：http://swp.yfazqb.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://xlj.hnqzz.top

[B12] 跳出多层循环
来源：http://wni.wangdashe.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://qno.pycfn.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://gdq.yj20258888.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://syd.yj20258.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ngp.daria6918.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://njj.52xcode.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ukj.feifeiyinyue.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://kgg.ctjpmb.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://roj.jinqigfzy.top

[B13] 判断是否为数字
来源：http://ffc.fktsv.cn

Py:   isinstance(x, (int, float))
来源：http://wsm.shanyushiyangtech.top

PHP:  is_numeric($x)
来源：http://cuo.zhixingplan.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ebd.xuetiantiany.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sjn.zhijiandao.cn

Java: x instanceof Number
来源：http://qwj.9152youxi.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://vfk.fzhhl.top

Ruby: x.is_a?(Numeric)
来源：http://ioz.yangfankeji.com

C#:   x is int or double or decimal
来源：http://mae.hysaishi.cn

[B14] 判断值是否在集合内
来源：http://ilk.shanyushiyangkeji.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://eel.jianghu66.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://tzf.jqgfzy.top

JS:   [1, 2, 3].includes(x)
来源：http://lmc.yfazqb.com

TS:   [1, 2, 3].includes(x)
来源：http://olf.sufxvd.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://rlr.fengsongda.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://sgt.hnqzz.top

Ruby: [1, 2, 3].include?(x)
来源：http://zno.guowangkeji.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://clt.hywenlv.cn

[B15] 布尔运算与取反
来源：http://iok.jinghuilouyu.cn

Py:   a and b or not c
来源：http://cqs.guannengcc.top

PHP:  $a && $b || !$c
来源：http://snj.xinyue.icu

JS:   a && b || !c
来源：http://qji.xuetiantiany.cn

TS:   a && b || !c
来源：http://gka.zhixingplan.top

Java: a && b || !c
来源：http://epd.fktsv.cn

Go:   a && b || !c
来源：http://yya.yueranfly.top

Ruby: a && b || !c
来源：http://olu.fktsv.cn

C#:   a && b || !c
来源：http://tmf.jqgfzy.top

[B16] 卫语句：不满足条件提前返回
来源：http://rcq.aizwys.cn

Py:   if not data: return
来源：http://uup.hnqzz.top

PHP:  if (!$data) { return; }
来源：http://trh.zhongyouzk.top

JS:   if (!data) return;
来源：http://mdl.jqgfzy.top

TS:   if (!data) return;
来源：http://wcr.quarkkingdee.top

Java: if (data == null) return;
来源：http://xjt.zdqjudy.top

Go:   if data == nil { return }
来源：http://vnq.dianchejie.cn

Ruby: return if data.nil?
来源：http://ndh.xinyue.icu

C#:   if (data == null) return;
来源：http://olq.xziqi.cn

================================================================================
来源：http://czo.snrcjt.cn

C. 函数与作用域
来源：http://qjg.dianchejie.cn

================================================================================
来源：http://hag.pycfn.com

[C01] 定义函数
来源：http://skq.chenjidiqi.icu

Py:   def add(a, b): return a + b
来源：http://eks.cucudq.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zua.snrcjt.cn

JS:   function add(a, b) { return a + b; }
来源：http://nzq.birdmap.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vyy.aizwys.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://dzf.feifeiyinyue.top

Go:   func add(a, b int) int { return a + b }
来源：http://adc.meibo888.top

Ruby: def add(a, b); a + b; end
来源：http://lld.sweek.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://kct.tarul.cn

[C02] 默认参数
来源：http://adr.tarul.cn

Py:   def greet(name="World"): return name
来源：http://kve.shanyushiyangkeji.top

PHP:  function greet($name = "World") { return $name; }
来源：http://bsv.gogol.net.cn

JS:   function greet(name = "World") { return name; }
来源：http://bph.xuanzx.com

TS:   function greet(name: string = "World") { return name; }
来源：http://upd.kuanghao11.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://qjn.zhengqikj.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://jjf.zhixingplan.top

Ruby: def greet(name = "World") = name
来源：http://mtc.sufxvd.cn

C#:   string Greet(string name = "World") => name;
来源：http://pdx.hywenlv.cn

[C03] 可变参数
来源：http://yto.fengsongda.top

Py:   def total(*args): return sum(args)
来源：http://faa.ppjwa.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://vvr.cashguo.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://lcf.zycfv.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ogx.xuanzx.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ilq.zhiwuduotai.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://eoy.jinyuanbaomall.cn

Ruby: def total(*nums); nums.sum; end
来源：http://gjf.havefunace.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://qcj.yonumen.top

[C04] 命名参数 / 关键字参数
来源：http://xra.ydjk.org.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://pdc.yfazqb.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://uak.zhaomingkeji.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://zwj.shangyingyoupin.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://bap.wangshuangyany.cn

Java: // 无：用 Builder 模式或 record
来源：http://akq.zhongyouzk.top

Go:   // 无：用配置结构体参数
来源：http://xpu.nwbrower.top

Ruby: f(a: 1, b: 2)
来源：http://tip.chenlongwang.top

C#:   f(a: 1, b: 2)
来源：http://egt.hcnkem.com

[C05] 返回多个值
来源：http://mth.jiagoushi.top

Py:   return a, b
来源：http://xcf.yfazqb.com

PHP:  return [$a, $b];
来源：http://bjj.9152youxi.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://jjg.nwbrower.top

TS:   return { a, b };
来源：http://yva.feifeiyinyue.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ion.dashuyun.cn

Go:   return a, b
来源：http://bpj.tanke756.top

Ruby: return a, b
来源：http://uem.fengsongda.top

C#:   return (a, b);              // ValueTuple
来源：http://ijy.jinqigfzy.top

[C06] 匿名函数 / lambda
来源：http://lfy.andypj.xyz

Py:   square = lambda x: x * x
来源：http://rnb.hywenlv.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ime.dashuyun.cn

JS:   const square = x => x * x;
来源：http://qjj.cheryme.top

TS:   const square = (x: number): number => x * x;
来源：http://ouo.gotoacloud.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ebd.bbcook.cn

Go:   sq := func(x int) int { return x * x }
来源：http://dev.haohaochexian.top

Ruby: square = ->(x) { x * x }
来源：http://axw.xziqi.cn

C#:   Func<int, int> square = x => x * x;
来源：http://xcq.hammf.cn

[C07] 把函数作为参数传入
来源：http://apw.gogol.net.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://usl.daria6918.cn

PHP:  array_map("strtoupper", $arr);
来源：http://lum.yongpay.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://tcz.jinqigufen.top

TS:   arr.map(String)
来源：http://xal.tianlin.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://qst.fanxiaobao.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hte.zhijiandao.cn

Ruby: arr.map(&:upcase)
来源：http://nay.yuxming.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ujs.sxryk.cn

[C08] 闭包
来源：http://qzb.9152youxi.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://gfk.quarkkingdee.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://xot.ywan-chungtsiang.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://eby.sufxvd.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://auy.jiagoushi.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://dqc.jqgufenzy.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://yjv.52xcode.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://qwc.feifeiyinyue.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://fpu.guowangkeji.top

[C09] 递归
来源：http://mrm.gogol.net.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://lpz.snrcjt.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://joh.hesvh.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ijv.yj20258888.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nud.tian-w.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://dfx.sysykeji.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://vxb.xuetiantiany.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://qrd.nanxuanxn.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://yrt.zhaomingkeji.xyz

[C10] 变量作用域
来源：http://bof.xziqi.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://vdy.uphjek.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://qys.epnwcf.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ppk.uphjek.com

TS:   同 JS
来源：http://gir.smart0.xyz

Java: 方法内为块级作用域
来源：http://bkd.redwolf501.top

Go:   花括号块级作用域
来源：http://gqt.zhaomingkeji.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://plx.sysykeji.top

C#:   块级作用域
来源：http://odg.pengpengdd.cyou

[C11] 模块导入与导出
来源：http://xqr.wangshuangyany.cn

Py:   from module import func
来源：http://crz.zdqjudy.top

PHP:  require "file.php";  或 use App\Service;
来源：http://pql.xuanzx.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://csj.epnwcf.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://tki.zhengqikj.top

Java: import java.util.List;
来源：http://zsv.yuanzhike.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://kjp.yanxiufei.cn

Ruby: require "json"; require_relative "./util"
来源：http://cgr.yuanzhike.top

C#:   using System.Text;
来源：http://pnq.daxiang520.top

[C12] 立即执行函数 IIFE
来源：http://pgu.shanyushiyangtech.top

Py:   (lambda: print("run"))()
来源：http://pyt.gotoacloud.top

PHP:  (function () { echo "run"; })();
来源：http://ukx.daxiang520.top

JS:   (() => { console.log("run"); })();
来源：http://ftd.iojbl.cn

TS:   (() => { console.log("run"); })();
来源：http://qog.shanyushiyangtech.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://pnu.hysaishi.cn

Go:   func() { fmt.Println("run") }()
来源：http://ojz.shangyingyoupin.top

Ruby: -> { puts "run" }.call
来源：http://gcg.aibaodan.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://otn.316326.xyz

[C13] 类型声明 / 类型注解
来源：http://lha.9152youxi.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ckk.zhengqikj.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sgc.zhiwuduotai.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://fnw.ybcxt.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ipt.52xcode.cn

Java: int add(int a, int b) { return a + b; }
来源：http://wdm.chenzaomai.com

Go:   func add(a, b int) int
来源：http://anl.jianghu66.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hjs.fanxiaobao.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://sqg.dashuyun.cn

[C14] 泛型函数
来源：http://jit.yonumen.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mio.shangyingyoupin.top

PHP:  // 无泛型
来源：http://zfo.chenzaomai.com

JS:   // 无泛型
来源：http://iyl.xuetiantiany.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ebn.chenjidiqi.icu

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://afy.andypj.xyz

Go:   func First[T any](items []T) T { return items[0] }
来源：http://yqz.jyoumei.cn

Ruby: # 无泛型
来源：http://crh.gzhubu.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ooq.haohaochexian.top

[C15] 解构 / 展开参数
来源：http://dul.jinqigufen.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://svn.zhaomingkeji.xyz

PHP:  [$a, $b] = $pair;
来源：http://vma.shuidangran.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wpl.daria6918.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ytj.aizwys.cn

Java: // 无解构
来源：http://nav.gzhubu.top

Go:   // 无解构
来源：http://npc.vehdjk.com

Ruby: a, b = pair
来源：http://ott.jlsjyb.cn

C#:   var (a, b) = pair;
来源：http://cjh.zhaomingkeji.xyz

[C16] 函数 / 方法重载
来源：http://msi.xinyue.icu

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ljt.hesvh.cn

PHP:  // 无重载
来源：http://jmd.chenzaomai.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://rxo.yongpay.top

TS:   // 用联合类型或重载签名声明
来源：http://tiw.0kj1m.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://hmk.zhongyouzk.top

Go:   // 无重载：用不同函数名
来源：http://nqd.jinqigufen.top

Ruby: # 无重载：靠动态参数
来源：http://zew.xinyue.icu

C#:   void F(int a) {}  void F(string a) {}
来源：http://dig.shangyingyoupin.top

================================================================================
来源：http://lww.xziqi.cn

D. 数组 / 列表 / 集合
来源：http://wlt.shuidangran.top

================================================================================
来源：http://waf.ydjk.org.cn

[D01] 创建数组 / 列表
来源：http://kab.daria6918.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://oph.yangfankeji.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://vpc.hysaishi.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://pbr.chenjidiqi.icu

TS:   const arr: number[] = [1, 2, 3];
来源：http://gxe.316326.xyz

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://kld.yuanzhike.top

Go:   arr := []int{1, 2, 3}
来源：http://pbv.vqdsnc.cn

Ruby: arr = [1, 2, 3]
来源：http://xaq.daria6918.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://xjv.bbcook.cn

[D02] 追加元素到末尾
来源：http://wxw.0kj1m.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://bmi.epnwcf.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://qvk.vehdjk.com

JS:   arr.push(4);
来源：http://cef.shzxlz.cn

TS:   arr.push(4);
来源：http://wrr.ybcxt.top

Java: list.add(4);
来源：http://rvf.zhengqikj.top

Go:   arr = append(arr, 4)
来源：http://bir.fanxiaobao.xyz

Ruby: arr << 4; arr.push(5)
来源：http://jwx.ybcxt.top

C#:   list.Add(4);
来源：http://jit.yuanzhike.top

[D03] 在指定位置插入元素
来源：http://oev.wangshuangyany.cn

Py:   arr.insert(0, 0)
来源：http://egy.yueranfly.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hex.0kj1m.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://kqt.guannengcc.top

TS:   arr.splice(0, 0, 0);
来源：http://ype.hcnkem.com

Java: list.add(0, 0);
来源：http://fjn.snrcjt.cn

Go:   arr = append([]int{0}, arr...)
来源：http://xib.feifeiyinyue.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://gdu.ppjwa.cn

C#:   list.Insert(0, 0);
来源：http://dlw.jlsjyb.cn

[D04] 删除元素
来源：http://gly.shanyushiyangkeji.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://sao.ydzc1.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://kpq.yanxiufei.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://neh.yj20258.top

TS:   arr.splice(0, 1);
来源：http://qio.nanxinkj.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://xqu.xziqi.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://vwr.xinyue.icu

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://bgg.shangyingyoupin.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://qsv.hesvh.cn

[D05] 访问与修改元素
来源：http://mov.birdmap.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://xsh.aibaodan.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://lyc.hfpthk.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://uyx.xingfuxueyuan.xyz

TS:   arr[0]; arr.at(-1);
来源：http://zyr.cucudq.cn

Java: list.get(0); list.set(0, 9);
来源：http://kgi.yj20258888.top

Go:   arr[0]; arr[0] = 9
来源：http://yve.hnxiangtu.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://lbv.9152youxi.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zco.shzxlz.cn

[D06] 数组长度
来源：http://wpq.kuanghao11.cn

Py:   len(arr)
来源：http://dpg.chenlongwang.top

PHP:  count($arr);
来源：http://vqb.jqgfzy.top

JS:   arr.length
来源：http://aer.vehdjk.com

TS:   arr.length
来源：http://jqu.tanke756.top

Java: list.size();
来源：http://kyp.bbcook.cn

Go:   len(arr)
来源：http://bax.316326.xyz

Ruby: arr.length; arr.size
来源：http://mxa.sxryk.cn

C#:   list.Count;
来源：http://zsb.zhaomingkeji.xyz

[D07] 切片 / 取子数组
来源：http://otb.zhiwuduotai.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://loz.gaohongyu789.top

PHP:  array_slice($arr, 1, 3);
来源：http://vea.hywenlv.cn

JS:   arr.slice(1, 4);
来源：http://eqr.yangfankeji.com

TS:   arr.slice(1, 4);
来源：http://vgq.shanyushiyangkeji.top

Java: list.subList(1, 4);
来源：http://cib.pengpengdd.cyou

Go:   arr[1:4]
来源：http://bzi.sxryk.cn

Ruby: arr[1, 3]
来源：http://oes.chenzaomai.com

C#:   list.GetRange(1, 3);
来源：http://dig.ybcxt.top

[D08] 合并两个数组
来源：http://nqg.hfpthk.cn

Py:   a + b;  a.extend(b)
来源：http://kmf.fktsv.cn

PHP:  array_merge($a, $b);
来源：http://rpf.jqgufenzy.top


<!-- 参考信息 -->