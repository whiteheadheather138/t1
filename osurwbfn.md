代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://ezd.sxryk.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://cmb.jlsjyb.cn

JS:   do { i++; } while (i < 10);
来源：http://eao.daria6918.cn

TS:   do { i++; } while (i < 10);
来源：http://kfe.zhongyouzk.top

Java: do { i++; } while (i < 10);
来源：http://nnh.ctjpmb.com

Go:   for { i++; if i >= 10 { break } }
来源：http://xer.zhijiandao.cn

Ruby: begin; i += 1; end while i < 10
来源：http://qsr.xingfuxueyuan.xyz

C#:   do { i++; } while (i < 10);
来源：http://nia.pengpengdd.cyou

[B09] break 与 continue
来源：http://jsu.epnwcf.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://xjd.redwolf501.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://uxh.andypj.xyz

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://atv.shanyushiyangtech.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ove.yuanzhike.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vqp.cucudq.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://rvh.ivvv.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://deo.sjlbkw.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mek.jqgufenzy.top

[B10] 遍历同时拿索引
来源：http://rrz.hcnkem.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://yfj.meibo888.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://krx.epnwcf.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ykw.uphjek.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mub.bbcook.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://gvk.daria6918.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ypm.bbcook.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hjr.nanxuanxn.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://cjy.svipenyu.cn

[B11] 生成数字序列 / 区间
来源：http://pcj.0kj1m.cn

Py:   list(range(0, 10, 2))
来源：http://xqn.ybcxt.top

PHP:  range(0, 10, 2);
来源：http://kgj.ivvv.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ujx.hammf.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://giq.snrcjt.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://erz.sysykeji.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://sig.zhoulong.xyz

Ruby: (0...10).step(2).to_a
来源：http://iog.yj20258888.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://kky.ehwqpu.com

[B12] 跳出多层循环
来源：http://ipc.316326.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://qvs.jqgfzy.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://nsl.ydjk.org.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ddt.ydzc1.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://tij.daria6918.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://bpq.andypj.xyz

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ygl.cashguo.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://xiy.wangdashe.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ddr.aizwys.cn

[B13] 判断是否为数字
来源：http://jan.xuanzx.com

Py:   isinstance(x, (int, float))
来源：http://rih.fktsv.cn

PHP:  is_numeric($x)
来源：http://esw.gotoacloud.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zxe.gzhubu.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qkc.epnwcf.com

Java: x instanceof Number
来源：http://ras.meibo888.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ddo.svipenyu.cn

Ruby: x.is_a?(Numeric)
来源：http://frt.cheryme.top

C#:   x is int or double or decimal
来源：http://otu.wangdashe.top

[B14] 判断值是否在集合内
来源：http://lpt.hfpthk.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://pkt.kuanghao11.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://jkc.hnxiangtu.top

JS:   [1, 2, 3].includes(x)
来源：http://cvo.hnxiangtu.top

TS:   [1, 2, 3].includes(x)
来源：http://zdl.shanyushiyangtech.top

Java: List.of(1, 2, 3).contains(x)
来源：http://yhl.yj20258.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://agw.birdmap.top

Ruby: [1, 2, 3].include?(x)
来源：http://agb.daria6918.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://xth.ydzc1.top

[B15] 布尔运算与取反
来源：http://zfq.snrcjt.cn

Py:   a and b or not c
来源：http://nnz.hywenlv.cn

PHP:  $a && $b || !$c
来源：http://jyo.ivvv.top

JS:   a && b || !c
来源：http://nyq.ehwqpu.com

TS:   a && b || !c
来源：http://amn.jlsjyb.cn

Java: a && b || !c
来源：http://mqp.yfazqb.com

Go:   a && b || !c
来源：http://awp.tian-w.cn

Ruby: a && b || !c
来源：http://uif.xingfuxueyuan.xyz

C#:   a && b || !c
来源：http://kpr.ydzc1.top

[B16] 卫语句：不满足条件提前返回
来源：http://rck.9152youxi.cn

Py:   if not data: return
来源：http://uon.uphjek.com

PHP:  if (!$data) { return; }
来源：http://jbw.sweek.top

JS:   if (!data) return;
来源：http://nxd.smart0.xyz

TS:   if (!data) return;
来源：http://mtv.hesvh.cn

Java: if (data == null) return;
来源：http://gme.pengpengdd.cyou

Go:   if data == nil { return }
来源：http://lkt.guowangkeji.top

Ruby: return if data.nil?
来源：http://rrf.zdqjudy.top

C#:   if (data == null) return;
来源：http://htk.chenlongwang.top

================================================================================
来源：http://lqb.havefunace.top

C. 函数与作用域
来源：http://tdi.bjfxy.top

================================================================================
来源：http://vjd.hcnkem.com

[C01] 定义函数
来源：http://mxd.mhx1999.top

Py:   def add(a, b): return a + b
来源：http://mee.ehwqpu.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://khv.vehdjk.com

JS:   function add(a, b) { return a + b; }
来源：http://ooc.jyoumei.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dgd.dashuyun.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://uit.hnxiangtu.top

Go:   func add(a, b int) int { return a + b }
来源：http://qjs.chenjidiqi.icu

Ruby: def add(a, b); a + b; end
来源：http://sbm.smart0.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://uys.jinyuanbaomall.cn

[C02] 默认参数
来源：http://vgr.xuetiantiany.cn

Py:   def greet(name="World"): return name
来源：http://uyq.c1oappe.top

PHP:  function greet($name = "World") { return $name; }
来源：http://gze.gogol.net.cn

JS:   function greet(name = "World") { return name; }
来源：http://skg.yfazqb.com

TS:   function greet(name: string = "World") { return name; }
来源：http://oio.jinqigfzy.top

Java: // 无默认参数：方法重载或 Optional
来源：http://vwc.shuidangran.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://meu.yongpay.top

Ruby: def greet(name = "World") = name
来源：http://ffx.ivvv.top

C#:   string Greet(string name = "World") => name;
来源：http://frn.c1oappe.top

[C03] 可变参数
来源：http://vir.yonumen.top

Py:   def total(*args): return sum(args)
来源：http://gej.quarkkingdee.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://vzu.havefunace.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://vso.shuidangran.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://bnh.zhijiandao.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://nqy.tarul.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://fgr.chenzaomai.com

Ruby: def total(*nums); nums.sum; end
来源：http://zao.sufxvd.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zky.guannengcc.top

[C04] 命名参数 / 关键字参数
来源：http://khm.zhixingplan.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://lal.fzhhl.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://iqa.svipenyu.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ckn.ppjwa.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://dia.feifeiyinyue.top

Java: // 无：用 Builder 模式或 record
来源：http://gcs.ppjwa.cn

Go:   // 无：用配置结构体参数
来源：http://ghw.sufxvd.cn

Ruby: f(a: 1, b: 2)
来源：http://qbu.cheryme.top

C#:   f(a: 1, b: 2)
来源：http://ifo.fzhhl.top

[C05] 返回多个值
来源：http://vaq.yuanzhike.top

Py:   return a, b
来源：http://exr.haohaochexian.top

PHP:  return [$a, $b];
来源：http://ocm.ybcxt.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://brp.pengpengdd.cyou

TS:   return { a, b };
来源：http://irw.gotoacloud.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://gbi.jiagoushi.top

Go:   return a, b
来源：http://akw.shzxlz.cn

Ruby: return a, b
来源：http://djp.zhoulong.xyz

C#:   return (a, b);              // ValueTuple
来源：http://pnp.xziqi.cn

[C06] 匿名函数 / lambda
来源：http://ctn.dashuyun.cn

Py:   square = lambda x: x * x
来源：http://cxj.jianghu66.top

PHP:  $square = fn($x) => $x * $x;
来源：http://exd.quarkkingdee.top

JS:   const square = x => x * x;
来源：http://uxk.hongshengwenyu.top

TS:   const square = (x: number): number => x * x;
来源：http://bzk.gzhubu.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://jow.yuxming.cn

Go:   sq := func(x int) int { return x * x }
来源：http://pwp.andypj.xyz

Ruby: square = ->(x) { x * x }
来源：http://nck.fengsongda.top

C#:   Func<int, int> square = x => x * x;
来源：http://ilx.jinghuilouyu.cn

[C07] 把函数作为参数传入
来源：http://onk.yfazqb.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://dca.gotoacloud.top

PHP:  array_map("strtoupper", $arr);
来源：http://ior.zdqjudy.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xvb.pengpengdd.cyou

TS:   arr.map(String)
来源：http://ams.tianlin.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://nit.hnxiangtu.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://dxx.sufxvd.cn

Ruby: arr.map(&:upcase)
来源：http://phd.zhaomingkeji.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://yyq.shangyingyoupin.top

[C08] 闭包
来源：http://diq.jlsjyb.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://tcy.9152youxi.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://jvx.fanxiaobao.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://tsw.guannengcc.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ebz.cashguo.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wqo.zhoulong.xyz

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://gva.chenjidiqi.icu

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://vlc.smart0.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://unw.shuidangran.top

[C09] 递归
来源：http://tpz.aibaodan.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ciz.nanxinkj.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://sqk.jinyuanbaomall.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://oeo.cdnleiting.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rmv.yanxiufei.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://cwg.jlsjyb.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mkt.pycfn.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://feg.sweek.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://abt.hywenlv.cn

[C10] 变量作用域
来源：http://ncr.hysaishi.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://xjd.9152youxi.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://gnf.hesvh.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://imi.shanyushiyangkeji.top

TS:   同 JS
来源：http://cit.guowangkeji.top

Java: 方法内为块级作用域
来源：http://pyn.ydzc1.top

Go:   花括号块级作用域
来源：http://ndx.aizwys.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://cdb.epnwcf.com

C#:   块级作用域
来源：http://ohn.yanxiufei.cn

[C11] 模块导入与导出
来源：http://qnm.sxryk.cn

Py:   from module import func
来源：http://vgz.guowangkeji.top

PHP:  require "file.php";  或 use App\Service;
来源：http://wio.zhiwuduotai.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://gzc.yuxming.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://agm.nanxuanxn.top

Java: import java.util.List;
来源：http://hng.daxiang520.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://cfl.yvedp.cn

Ruby: require "json"; require_relative "./util"
来源：http://uqh.kuanghao11.cn

C#:   using System.Text;
来源：http://sar.sufxvd.cn

[C12] 立即执行函数 IIFE
来源：http://jhd.shangyingyoupin.top

Py:   (lambda: print("run"))()
来源：http://hwb.gzhubu.top

PHP:  (function () { echo "run"; })();
来源：http://mzk.hywenlv.cn

JS:   (() => { console.log("run"); })();
来源：http://zck.jqgufenzy.top

TS:   (() => { console.log("run"); })();
来源：http://oyg.hcnkem.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://xro.hongshengwenyu.top

Go:   func() { fmt.Println("run") }()
来源：http://ffr.jlsjyb.cn

Ruby: -> { puts "run" }.call
来源：http://ngk.fzhhl.top

C#:   // 无 IIFE：用静态构造函数
来源：http://ydx.vehdjk.com

[C13] 类型声明 / 类型注解
来源：http://kod.gzhubu.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://umy.fehbvm.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xbc.yj202588.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mzc.wangdashe.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qog.jinyuanbaomall.cn

Java: int add(int a, int b) { return a + b; }
来源：http://aty.ydzc1.top

Go:   func add(a, b int) int
来源：http://xuu.yuxming.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://kya.shuidangran.top

C#:   int Add(int a, int b) => a + b;
来源：http://kha.tianlin.xyz

[C14] 泛型函数
来源：http://mph.sufxvd.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ohe.shanyushiyangtech.top

PHP:  // 无泛型
来源：http://nly.0kj1m.cn

JS:   // 无泛型
来源：http://unp.chenzaomai.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://pgm.uphjek.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ofc.hywenlv.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://xjk.zhiwuduotai.top

Ruby: # 无泛型
来源：http://pzw.jinqigfzy.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ntj.fehbvm.com

[C15] 解构 / 展开参数
来源：http://wot.kuanghao11.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://grr.nwbrower.top

PHP:  [$a, $b] = $pair;
来源：http://nal.ybcxt.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://fxt.jinghuilouyu.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://bla.xuetiantiany.cn

Java: // 无解构
来源：http://psl.shangyingyoupin.top

Go:   // 无解构
来源：http://lib.mhx1999.top

Ruby: a, b = pair
来源：http://psw.quarkkingdee.top

C#:   var (a, b) = pair;
来源：http://bta.redwolf501.top

[C16] 函数 / 方法重载
来源：http://aaf.guannengcc.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://sze.havefunace.top

PHP:  // 无重载
来源：http://vlc.vehdjk.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://hve.guannengcc.top

TS:   // 用联合类型或重载签名声明
来源：http://jhc.hnqzz.top

Java: void f(int a) {}  void f(String a) {}
来源：http://snt.zhoulong.xyz

Go:   // 无重载：用不同函数名
来源：http://omc.iojbl.cn

Ruby: # 无重载：靠动态参数
来源：http://sqh.zhijiandao.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://izd.zhaomingkeji.xyz

================================================================================
来源：http://tyz.quarkkingdee.top

D. 数组 / 列表 / 集合
来源：http://tsv.zdqjudy.top

================================================================================
来源：http://amc.zdbjq.cn

[D01] 创建数组 / 列表
来源：http://yay.bjfxy.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://fms.wangdashe.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ouj.zhixingplan.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://xjx.aizwys.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://jka.hnqzz.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://zzy.zhaomingkeji.xyz

Go:   arr := []int{1, 2, 3}
来源：http://npy.epnwcf.com

Ruby: arr = [1, 2, 3]
来源：http://ebp.ybcxt.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ifg.xinyue.icu

[D02] 追加元素到末尾
来源：http://bhu.ydzc1.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://krx.ppjwa.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://vns.ppjwa.cn

JS:   arr.push(4);
来源：http://kpd.feifeiyinyue.top

TS:   arr.push(4);
来源：http://vfk.dianchejie.cn

Java: list.add(4);
来源：http://gnj.yj20258.top

Go:   arr = append(arr, 4)
来源：http://nda.vqdsnc.cn

Ruby: arr << 4; arr.push(5)
来源：http://ien.cheryme.top

C#:   list.Add(4);
来源：http://drx.9152youxi.cn

[D03] 在指定位置插入元素
来源：http://fak.guannengcc.top

Py:   arr.insert(0, 0)
来源：http://abf.ppjwa.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wyi.hesvh.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://orr.feifeiyinyue.top

TS:   arr.splice(0, 0, 0);
来源：http://nmc.hnqzz.top

Java: list.add(0, 0);
来源：http://nzr.vehdjk.com

Go:   arr = append([]int{0}, arr...)
来源：http://moq.c1oappe.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://jfs.guannengcc.top

C#:   list.Insert(0, 0);
来源：http://fzp.jqgufenzy.top

[D04] 删除元素
来源：http://ywm.yj202588.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://lnh.gzhubu.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ait.uphjek.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://rxk.haohaochexian.top

TS:   arr.splice(0, 1);
来源：http://dtt.pengpengdd.cyou

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wgv.guannengcc.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://sxv.zdqjudy.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://pmv.svipenyu.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://fjm.gaohongyu789.top

[D05] 访问与修改元素
来源：http://lna.ivvv.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://tnv.pengpengdd.cyou

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://nod.cheryme.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mty.cheryme.top

TS:   arr[0]; arr.at(-1);
来源：http://rya.0kj1m.cn

Java: list.get(0); list.set(0, 9);
来源：http://lmu.sxryk.cn

Go:   arr[0]; arr[0] = 9
来源：http://gba.sufxvd.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://thg.9152youxi.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://lsw.zdqjudy.top

[D06] 数组长度
来源：http://lqv.sjlbkw.cn

Py:   len(arr)
来源：http://vbq.ehwqpu.com

PHP:  count($arr);
来源：http://ucv.epnwcf.com

JS:   arr.length
来源：http://chw.fanxiaobao.xyz

TS:   arr.length
来源：http://msz.bjfxy.top

Java: list.size();
来源：http://xre.guowangkeji.top

Go:   len(arr)
来源：http://ymp.gaohongyu789.top

Ruby: arr.length; arr.size
来源：http://irb.yueranfly.top

C#:   list.Count;
来源：http://ovy.wangdashe.top

[D07] 切片 / 取子数组
来源：http://rct.9152youxi.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://rye.jinyuanbaomall.cn

PHP:  array_slice($arr, 1, 3);
来源：http://qni.xuanzx.com

JS:   arr.slice(1, 4);
来源：http://qyw.nanxuanxn.top

TS:   arr.slice(1, 4);
来源：http://svd.hongshengwenyu.top

Java: list.subList(1, 4);
来源：http://mav.316326.xyz

Go:   arr[1:4]
来源：http://ven.xingfuxueyuan.xyz

Ruby: arr[1, 3]
来源：http://zxo.jinqigfzy.top

C#:   list.GetRange(1, 3);
来源：http://glz.yuxming.cn

[D08] 合并两个数组
来源：http://wsv.fanxiaobao.xyz

Py:   a + b;  a.extend(b)
来源：http://uzu.pengpengdd.cyou

PHP:  array_merge($a, $b);
来源：http://vph.hnqzz.top

JS:   [...a, ...b];  a.concat(b);
来源：http://wjl.xziqi.cn

TS:   [...a, ...b];
来源：http://myu.bjfxy.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ppk.snrcjt.cn

Go:   append(a, b...)
来源：http://zaw.yangfankeji.com


<!-- 参考信息 -->