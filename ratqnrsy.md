代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://kqg.xuetiantiany.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://osx.xinyue.icu

JS:   do { i++; } while (i < 10);
来源：http://jeq.uphjek.com

TS:   do { i++; } while (i < 10);
来源：http://lzu.havefunace.top

Java: do { i++; } while (i < 10);
来源：http://spm.0kj1m.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://hev.cqqwz.cn

Ruby: begin; i += 1; end while i < 10
来源：http://dkd.zhijiandao.cn

C#:   do { i++; } while (i < 10);
来源：http://dny.52xcode.cn

[B09] break 与 continue
来源：http://lzx.fanxiaobao.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://qmc.aibaodan.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://qay.jinqigufen.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://psq.smart0.xyz

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ulq.mhx1999.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qye.fzhhl.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://cgo.xinyue.icu

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://nmg.pengpengdd.cyou

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mmf.ydzc1.top

[B10] 遍历同时拿索引
来源：http://zga.chenzaomai.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ngh.xingfuxueyuan.xyz

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://urh.zdqjudy.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://bhl.fanxiaobao.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://jen.yj20258888.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://eul.jyoumei.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://byo.meibo888.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://dfe.yj20258888.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://tju.bbcook.cn

[B11] 生成数字序列 / 区间
来源：http://tlt.chenzaomai.com

Py:   list(range(0, 10, 2))
来源：http://zbp.bjfxy.top

PHP:  range(0, 10, 2);
来源：http://sko.tarul.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jvn.zhijiandao.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dvc.hywenlv.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://fqk.gogol.net.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://nez.tian-w.cn

Ruby: (0...10).step(2).to_a
来源：http://qrd.cdnleiting.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ffz.shanyushiyangtech.top

[B12] 跳出多层循环
来源：http://mfh.shuidangran.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://jfi.dianchejie.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://qru.tanke756.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://jbk.smart0.xyz

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://iin.yueranfly.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://qmg.nanxuanxn.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://iya.tanke756.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://sbv.zhaomingkeji.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hey.yvedp.cn

[B13] 判断是否为数字
来源：http://rzf.sxryk.cn

Py:   isinstance(x, (int, float))
来源：http://vxo.yvedp.cn

PHP:  is_numeric($x)
来源：http://rjp.tanke756.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gge.kuanghao11.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://whz.yonumen.top

Java: x instanceof Number
来源：http://lty.ydjk.org.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://pvu.ehwqpu.com

Ruby: x.is_a?(Numeric)
来源：http://oyc.mhx1999.top

C#:   x is int or double or decimal
来源：http://oav.nanxuanxn.top

[B14] 判断值是否在集合内
来源：http://jxe.zhiwuduotai.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hax.jinyuanbaomall.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://pet.hammf.cn

JS:   [1, 2, 3].includes(x)
来源：http://rzf.ydzc1.top

TS:   [1, 2, 3].includes(x)
来源：http://mpa.bbcook.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://xth.gaohongyu789.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://avp.wangdashe.top

Ruby: [1, 2, 3].include?(x)
来源：http://cdt.chenjidiqi.icu

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://zgi.zhongyouzk.top

[B15] 布尔运算与取反
来源：http://cqz.gotoacloud.top

Py:   a and b or not c
来源：http://kqn.zhaomingkeji.xyz

PHP:  $a && $b || !$c
来源：http://pss.pengpengdd.cyou

JS:   a && b || !c
来源：http://lei.havefunace.top

TS:   a && b || !c
来源：http://igl.ivvv.top

Java: a && b || !c
来源：http://lxh.guowangkeji.top

Go:   a && b || !c
来源：http://sbr.zhongyouzk.top

Ruby: a && b || !c
来源：http://zgl.shanyushiyangkeji.top

C#:   a && b || !c
来源：http://jos.ctjpmb.com

[B16] 卫语句：不满足条件提前返回
来源：http://mim.ctjpmb.com

Py:   if not data: return
来源：http://aea.hywenlv.cn

PHP:  if (!$data) { return; }
来源：http://bss.xuanzx.com

JS:   if (!data) return;
来源：http://gpo.tarul.cn

TS:   if (!data) return;
来源：http://ilh.aizwys.cn

Java: if (data == null) return;
来源：http://nnr.zhiwuduotai.top

Go:   if data == nil { return }
来源：http://ixg.wangdashe.top

Ruby: return if data.nil?
来源：http://ewv.yj20258.top

C#:   if (data == null) return;
来源：http://eyx.birdmap.top

================================================================================
来源：http://hzk.tianlin.xyz

C. 函数与作用域
来源：http://yrj.fanxiaobao.xyz

================================================================================
来源：http://mnb.wangdashe.top

[C01] 定义函数
来源：http://aka.xinyue.icu

Py:   def add(a, b): return a + b
来源：http://nxn.yanxiufei.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wmh.fanxiaobao.xyz

JS:   function add(a, b) { return a + b; }
来源：http://xrf.fktsv.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://otg.zhaomingkeji.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://ciw.cdnleiting.top

Go:   func add(a, b int) int { return a + b }
来源：http://mzi.yangfankeji.com

Ruby: def add(a, b); a + b; end
来源：http://ohn.shanyushiyangkeji.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://vzu.gogol.net.cn

[C02] 默认参数
来源：http://edz.xinyue.icu

Py:   def greet(name="World"): return name
来源：http://xpw.ivvv.top

PHP:  function greet($name = "World") { return $name; }
来源：http://vis.redwolf501.top

JS:   function greet(name = "World") { return name; }
来源：http://czd.ehwqpu.com

TS:   function greet(name: string = "World") { return name; }
来源：http://yke.meibo888.top

Java: // 无默认参数：方法重载或 Optional
来源：http://mzy.fzhhl.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://lrt.yuanzhike.top

Ruby: def greet(name = "World") = name
来源：http://xvk.yvedp.cn

C#:   string Greet(string name = "World") => name;
来源：http://wnb.jyoumei.cn

[C03] 可变参数
来源：http://hqj.jinyuanbaomall.cn

Py:   def total(*args): return sum(args)
来源：http://sgz.gzhubu.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://slq.andypj.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ine.cdnleiting.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://eou.ctjpmb.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://cdx.jlsjyb.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ezg.yj20258.top

Ruby: def total(*nums); nums.sum; end
来源：http://vea.316326.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://diq.nanxuanxn.top

[C04] 命名参数 / 关键字参数
来源：http://xas.fehbvm.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://opu.cheryme.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ais.gogol.net.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://rwl.epnwcf.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://cwh.tian-w.cn

Java: // 无：用 Builder 模式或 record
来源：http://cia.yuanzhike.top

Go:   // 无：用配置结构体参数
来源：http://mnr.shanyushiyangkeji.top

Ruby: f(a: 1, b: 2)
来源：http://cbd.havefunace.top

C#:   f(a: 1, b: 2)
来源：http://ddd.gotoacloud.top

[C05] 返回多个值
来源：http://dze.jqgfzy.top

Py:   return a, b
来源：http://fpo.yj20258888.top

PHP:  return [$a, $b];
来源：http://blo.quarkkingdee.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://bre.vehdjk.com

TS:   return { a, b };
来源：http://duz.fehbvm.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xxz.birdmap.top

Go:   return a, b
来源：http://grt.uphjek.com

Ruby: return a, b
来源：http://msq.havefunace.top

C#:   return (a, b);              // ValueTuple
来源：http://xlj.chenjidiqi.icu

[C06] 匿名函数 / lambda
来源：http://mfs.pengpengdd.cyou

Py:   square = lambda x: x * x
来源：http://cxt.cheryme.top

PHP:  $square = fn($x) => $x * $x;
来源：http://wwz.sjlbkw.cn

JS:   const square = x => x * x;
来源：http://wmn.ctjpmb.com

TS:   const square = (x: number): number => x * x;
来源：http://sxt.jinqigufen.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ngb.sufxvd.cn

Go:   sq := func(x int) int { return x * x }
来源：http://gaz.nanxuanxn.top

Ruby: square = ->(x) { x * x }
来源：http://cum.hnxiangtu.top

C#:   Func<int, int> square = x => x * x;
来源：http://yad.yvedp.cn

[C07] 把函数作为参数传入
来源：http://uqb.sysykeji.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://rab.hfpthk.cn

PHP:  array_map("strtoupper", $arr);
来源：http://vzz.cheryme.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://tcj.sxryk.cn

TS:   arr.map(String)
来源：http://rxy.zhoulong.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://rna.jlsjyb.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://uxc.ywan-chungtsiang.top

Ruby: arr.map(&:upcase)
来源：http://kbf.yueranfly.top

C#:   arr.Select(s => s.ToUpper())
来源：http://cbr.sufxvd.cn

[C08] 闭包
来源：http://skt.nanxuanxn.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://fba.aibaodan.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://zhv.bjfxy.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://bfm.sysykeji.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://fnx.zhongyouzk.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://cxo.xylfe.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://deu.pycfn.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://koj.andypj.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://gpq.tarul.cn

[C09] 递归
来源：http://ngy.jinqigfzy.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://lvh.hesvh.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://zty.aibaodan.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rwx.nanxinkj.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pos.gogol.net.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://yjj.xuetiantiany.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://kul.chenzaomai.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wwb.yonumen.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://cwy.hnxiangtu.top

[C10] 变量作用域
来源：http://skr.jlsjyb.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://cwt.cashguo.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://fbu.hywenlv.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://szq.ydzc1.top

TS:   同 JS
来源：http://iqr.yueranfly.top

Java: 方法内为块级作用域
来源：http://uhu.jlsjyb.cn

Go:   花括号块级作用域
来源：http://hzk.nwbrower.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://uxe.pycfn.com

C#:   块级作用域
来源：http://tmg.yonumen.top

[C11] 模块导入与导出
来源：http://jxy.smart0.xyz

Py:   from module import func
来源：http://mjy.yj20258888.top

PHP:  require "file.php";  或 use App\Service;
来源：http://bgi.xylfe.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://bgr.zhongyouzk.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://uaw.jianghu66.top

Java: import java.util.List;
来源：http://xjf.cheryme.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://qcj.yuanzhike.top

Ruby: require "json"; require_relative "./util"
来源：http://pbn.sxryk.cn

C#:   using System.Text;
来源：http://zdu.haohaochexian.top

[C12] 立即执行函数 IIFE
来源：http://pnq.guowangkeji.top

Py:   (lambda: print("run"))()
来源：http://jax.epnwcf.com

PHP:  (function () { echo "run"; })();
来源：http://dqr.tian-w.cn

JS:   (() => { console.log("run"); })();
来源：http://tva.cucudq.cn

TS:   (() => { console.log("run"); })();
来源：http://pph.tarul.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://cwb.yj20258.top

Go:   func() { fmt.Println("run") }()
来源：http://bwf.quarkkingdee.top

Ruby: -> { puts "run" }.call
来源：http://yrq.fktsv.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://dga.gogol.net.cn

[C13] 类型声明 / 类型注解
来源：http://dwd.wangshuangyany.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://vfm.yongpay.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bqw.nanxinkj.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://xdh.9152youxi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rzi.zhijiandao.cn

Java: int add(int a, int b) { return a + b; }
来源：http://umi.smart0.xyz

Go:   func add(a, b int) int
来源：http://bet.fktsv.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ydg.zdqjudy.top

C#:   int Add(int a, int b) => a + b;
来源：http://qal.ywan-chungtsiang.top

[C14] 泛型函数
来源：http://zgc.ppjwa.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ips.yj20258.top

PHP:  // 无泛型
来源：http://dog.hfpthk.cn

JS:   // 无泛型
来源：http://hin.zhoulong.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wlg.9152youxi.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wrr.havefunace.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ivg.hesvh.cn

Ruby: # 无泛型
来源：http://ubw.hnqzz.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://bhw.cashguo.top

[C15] 解构 / 展开参数
来源：http://lfn.smart0.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://gie.tanke756.top

PHP:  [$a, $b] = $pair;
来源：http://jxb.mhx1999.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://llm.jinyuanbaomall.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wpz.ppjwa.cn

Java: // 无解构
来源：http://vfx.jyoumei.cn

Go:   // 无解构
来源：http://ukj.vehdjk.com

Ruby: a, b = pair
来源：http://jrc.cucudq.cn

C#:   var (a, b) = pair;
来源：http://hql.fzhhl.top

[C16] 函数 / 方法重载
来源：http://dvn.shanyushiyangkeji.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://lgy.zhiwuduotai.top

PHP:  // 无重载
来源：http://eoh.ybcxt.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://lkm.shanyushiyangtech.top

TS:   // 用联合类型或重载签名声明
来源：http://rib.fzhhl.top

Java: void f(int a) {}  void f(String a) {}
来源：http://bfo.zhongyouzk.top

Go:   // 无重载：用不同函数名
来源：http://kei.jiagoushi.top

Ruby: # 无重载：靠动态参数
来源：http://nop.yuanzhike.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://dld.zycfv.cn

================================================================================
来源：http://klo.dianchejie.cn

D. 数组 / 列表 / 集合
来源：http://bhr.shangyingyoupin.top

================================================================================
来源：http://bko.gzhubu.top

[D01] 创建数组 / 列表
来源：http://jdo.yueranfly.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://kut.xinyue.icu

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://omd.ywan-chungtsiang.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://zve.cdnleiting.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://svx.aibaodan.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://nit.tianlin.xyz

Go:   arr := []int{1, 2, 3}
来源：http://tnx.tarul.cn

Ruby: arr = [1, 2, 3]
来源：http://rrr.shanyushiyangkeji.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://xfn.guannengcc.top

[D02] 追加元素到末尾
来源：http://qtf.fzhhl.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://vte.tanke756.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://tex.nwbrower.top

JS:   arr.push(4);
来源：http://moc.wangshuangyany.cn

TS:   arr.push(4);
来源：http://mxr.nanxinkj.top

Java: list.add(4);
来源：http://vub.dashuyun.cn

Go:   arr = append(arr, 4)
来源：http://mtn.sufxvd.cn

Ruby: arr << 4; arr.push(5)
来源：http://okb.hysaishi.cn

C#:   list.Add(4);
来源：http://jed.nwbrower.top

[D03] 在指定位置插入元素
来源：http://zuo.hfpthk.cn

Py:   arr.insert(0, 0)
来源：http://cww.chenjidiqi.icu

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ysb.birdmap.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://nxz.sxryk.cn

TS:   arr.splice(0, 0, 0);
来源：http://euf.tianlin.xyz

Java: list.add(0, 0);
来源：http://eny.dianchejie.cn

Go:   arr = append([]int{0}, arr...)
来源：http://uiz.shzxlz.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://odm.smart0.xyz

C#:   list.Insert(0, 0);
来源：http://nuk.gaohongyu789.top

[D04] 删除元素
来源：http://sfn.zhaomingkeji.xyz

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://caq.uphjek.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://gkg.hysaishi.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hvj.hcnkem.com

TS:   arr.splice(0, 1);
来源：http://cqs.ivvv.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://egs.dashuyun.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://pmp.chenzaomai.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://jcr.chenzaomai.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://qie.zycfv.cn

[D05] 访问与修改元素
来源：http://ghz.52xcode.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ydx.hfpthk.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hjo.vehdjk.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://apf.cheryme.top

TS:   arr[0]; arr.at(-1);
来源：http://aeq.jyoumei.cn

Java: list.get(0); list.set(0, 9);
来源：http://qez.ydjk.org.cn

Go:   arr[0]; arr[0] = 9
来源：http://ccz.ybcxt.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://fps.bbcook.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://qgz.gzhubu.top

[D06] 数组长度
来源：http://vgb.uphjek.com

Py:   len(arr)
来源：http://ryc.yanxiufei.cn

PHP:  count($arr);
来源：http://qpm.yj202588.top

JS:   arr.length
来源：http://lvd.vqdsnc.cn

TS:   arr.length
来源：http://ewj.meibo888.top

Java: list.size();
来源：http://zda.nanxinkj.top

Go:   len(arr)
来源：http://izw.feifeiyinyue.top

Ruby: arr.length; arr.size
来源：http://bss.jqgfzy.top

C#:   list.Count;
来源：http://yvc.sxryk.cn

[D07] 切片 / 取子数组
来源：http://zbv.tianlin.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://klf.aibaodan.cn

PHP:  array_slice($arr, 1, 3);
来源：http://apb.hnqzz.top

JS:   arr.slice(1, 4);
来源：http://zfe.hongshengwenyu.top

TS:   arr.slice(1, 4);
来源：http://usw.havefunace.top

Java: list.subList(1, 4);
来源：http://bab.zhongyouzk.top

Go:   arr[1:4]
来源：http://rrb.fzhhl.top

Ruby: arr[1, 3]
来源：http://tni.jinqigufen.top

C#:   list.GetRange(1, 3);
来源：http://dto.ybcxt.top

[D08] 合并两个数组
来源：http://kzx.fengsongda.top

Py:   a + b;  a.extend(b)
来源：http://dsn.andypj.xyz

PHP:  array_merge($a, $b);
来源：http://jhr.hnxiangtu.top

JS:   [...a, ...b];  a.concat(b);
来源：http://qjy.hammf.cn

TS:   [...a, ...b];
来源：http://hyw.fktsv.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://voi.kuanghao11.cn

Go:   append(a, b...)
来源：http://ehb.fengsongda.top


<!-- 参考信息 -->