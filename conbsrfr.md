代发 wailian999

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://zat.guannengcc.top

Ruby: while i < 10; i += 1; end
来源：http://eea.cashguo.top

C#:   while (i < 10) { i++; }
来源：http://hoz.yuanzhike.top

[B08] do-while（至少执行一次）
来源：http://xkm.daria6918.cn

Py:   # 无 do-while：用 while True + break
来源：http://vnc.xuetiantiany.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://xnv.zhongyouzk.top

JS:   do { i++; } while (i < 10);
来源：http://hhr.feifeiyinyue.top

TS:   do { i++; } while (i < 10);
来源：http://xhk.chenjidiqi.icu

Java: do { i++; } while (i < 10);
来源：http://eyb.nanxuanxn.top

Go:   for { i++; if i >= 10 { break } }
来源：http://xpd.nanxuanxn.top

Ruby: begin; i += 1; end while i < 10
来源：http://dnv.uphjek.com

C#:   do { i++; } while (i < 10);
来源：http://kfp.fzhhl.top

[B09] break 与 continue
来源：http://ima.guowangkeji.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://whd.aizwys.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://zdn.hesvh.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yqf.hfpthk.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://icc.xuetiantiany.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nmp.ivvv.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://abw.sjlbkw.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://vvp.jqgufenzy.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jyd.hammf.cn

[B10] 遍历同时拿索引
来源：http://xge.sufxvd.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://cfq.fktsv.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ltj.epnwcf.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://rxo.ppjwa.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://uij.tanke756.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://kgt.zdqjudy.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mjj.yvedp.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://dfe.zhengqikj.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://iah.fengsongda.top

[B11] 生成数字序列 / 区间
来源：http://tnl.nwbrower.top

Py:   list(range(0, 10, 2))
来源：http://uyi.xuetiantiany.cn

PHP:  range(0, 10, 2);
来源：http://kyn.dianchejie.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://eet.zhijiandao.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ztj.daxiang520.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ycu.gaohongyu789.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://oza.xuetiantiany.cn

Ruby: (0...10).step(2).to_a
来源：http://bhj.guannengcc.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hju.sysykeji.top

[B12] 跳出多层循环
来源：http://vzt.xziqi.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://lff.jinghuilouyu.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://bul.andypj.xyz

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://gpr.bbcook.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://lxp.jqgufenzy.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://gwx.hywenlv.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://vyg.shzxlz.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://nop.sjlbkw.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ils.jinyuanbaomall.cn

[B13] 判断是否为数字
来源：http://bmq.ivvv.top

Py:   isinstance(x, (int, float))
来源：http://gav.52xcode.cn

PHP:  is_numeric($x)
来源：http://oqo.yj20258888.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ell.shanyushiyangtech.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://oud.pycfn.com

Java: x instanceof Number
来源：http://xwa.jinqigufen.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://qjh.bjfxy.top

Ruby: x.is_a?(Numeric)
来源：http://xbe.yongpay.top

C#:   x is int or double or decimal
来源：http://etb.zhaomingkeji.xyz

[B14] 判断值是否在集合内
来源：http://gca.gaohongyu789.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://dwl.ctjpmb.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ctm.zdqjudy.top

JS:   [1, 2, 3].includes(x)
来源：http://cne.yj20258.top

TS:   [1, 2, 3].includes(x)
来源：http://rbk.shanyushiyangkeji.top

Java: List.of(1, 2, 3).contains(x)
来源：http://lqa.52xcode.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ohp.haohaochexian.top

Ruby: [1, 2, 3].include?(x)
来源：http://ttz.jinqigufen.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://qtc.mhx1999.top

[B15] 布尔运算与取反
来源：http://knr.chenjidiqi.icu

Py:   a and b or not c
来源：http://sxv.zhongyouzk.top

PHP:  $a && $b || !$c
来源：http://unn.zhaomingkeji.xyz

JS:   a && b || !c
来源：http://gli.svipenyu.cn

TS:   a && b || !c
来源：http://pev.fktsv.cn

Java: a && b || !c
来源：http://ftt.aibaodan.cn

Go:   a && b || !c
来源：http://fwq.pengpengdd.cyou

Ruby: a && b || !c
来源：http://hxt.fktsv.cn

C#:   a && b || !c
来源：http://xqk.gotoacloud.top

[B16] 卫语句：不满足条件提前返回
来源：http://zbl.9152youxi.cn

Py:   if not data: return
来源：http://qdz.dashuyun.cn

PHP:  if (!$data) { return; }
来源：http://dwy.gogol.net.cn

JS:   if (!data) return;
来源：http://phu.sxryk.cn

TS:   if (!data) return;
来源：http://jvd.yvedp.cn

Java: if (data == null) return;
来源：http://yal.xuanzx.com

Go:   if data == nil { return }
来源：http://ugl.jyoumei.cn

Ruby: return if data.nil?
来源：http://pjf.yanxiufei.cn

C#:   if (data == null) return;
来源：http://mgd.cucudq.cn

================================================================================
来源：http://apk.sjlbkw.cn

C. 函数与作用域
来源：http://ajg.zhoulong.xyz

================================================================================
来源：http://pvj.zdqjudy.top

[C01] 定义函数
来源：http://igq.hcnkem.com

Py:   def add(a, b): return a + b
来源：http://tdk.yonumen.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nmk.ybcxt.top

JS:   function add(a, b) { return a + b; }
来源：http://xic.quarkkingdee.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ypp.nanxuanxn.top

Java: static int add(int a, int b) { return a + b; }
来源：http://ifh.fzhhl.top

Go:   func add(a, b int) int { return a + b }
来源：http://jaf.tian-w.cn

Ruby: def add(a, b); a + b; end
来源：http://jxs.tanke756.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://fgd.jqgfzy.top

[C02] 默认参数
来源：http://dqn.ybcxt.top

Py:   def greet(name="World"): return name
来源：http://mkr.ydjk.org.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://uci.jianghu66.top

JS:   function greet(name = "World") { return name; }
来源：http://pcp.zhaomingkeji.xyz

TS:   function greet(name: string = "World") { return name; }
来源：http://kww.xylfe.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://jhd.jianghu66.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://syl.zdbjq.cn

Ruby: def greet(name = "World") = name
来源：http://doj.aizwys.cn

C#:   string Greet(string name = "World") => name;
来源：http://jal.yfazqb.com

[C03] 可变参数
来源：http://mha.nanxinkj.top

Py:   def total(*args): return sum(args)
来源：http://kwc.yueranfly.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ejv.wangshuangyany.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://dxo.tanke756.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wur.ywan-chungtsiang.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vew.nanxinkj.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://sdn.pengpengdd.cyou

Ruby: def total(*nums); nums.sum; end
来源：http://fuk.52xcode.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hvg.gzhubu.top

[C04] 命名参数 / 关键字参数
来源：http://bfo.jlsjyb.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://jwi.hysaishi.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://rvk.redwolf501.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://yjh.hfpthk.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://tjf.meibo888.top

Java: // 无：用 Builder 模式或 record
来源：http://uqg.andypj.xyz

Go:   // 无：用配置结构体参数
来源：http://bqo.hfpthk.cn

Ruby: f(a: 1, b: 2)
来源：http://hvh.yj20258888.top

C#:   f(a: 1, b: 2)
来源：http://hil.iojbl.cn

[C05] 返回多个值
来源：http://ikg.hywenlv.cn

Py:   return a, b
来源：http://lcu.havefunace.top

PHP:  return [$a, $b];
来源：http://dha.fktsv.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://rll.zdbjq.cn

TS:   return { a, b };
来源：http://jzr.fktsv.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://npp.fanxiaobao.xyz

Go:   return a, b
来源：http://ppa.ctjpmb.com

Ruby: return a, b
来源：http://nkp.shzxlz.cn

C#:   return (a, b);              // ValueTuple
来源：http://gjo.hcnkem.com

[C06] 匿名函数 / lambda
来源：http://oai.nanxuanxn.top

Py:   square = lambda x: x * x
来源：http://mem.xinyue.icu

PHP:  $square = fn($x) => $x * $x;
来源：http://iuc.ybcxt.top

JS:   const square = x => x * x;
来源：http://zwi.0kj1m.cn

TS:   const square = (x: number): number => x * x;
来源：http://gzx.vehdjk.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://iwy.gotoacloud.top

Go:   sq := func(x int) int { return x * x }
来源：http://qkb.yj20258888.top

Ruby: square = ->(x) { x * x }
来源：http://iuy.nwbrower.top

C#:   Func<int, int> square = x => x * x;
来源：http://zkt.hnxiangtu.top

[C07] 把函数作为参数传入
来源：http://gmk.tanke756.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mxm.hywenlv.cn

PHP:  array_map("strtoupper", $arr);
来源：http://hbj.bbcook.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xqe.fanxiaobao.xyz

TS:   arr.map(String)
来源：http://aur.shangyingyoupin.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://zxh.wangshuangyany.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://zop.jqgufenzy.top

Ruby: arr.map(&:upcase)
来源：http://tlk.hnxiangtu.top

C#:   arr.Select(s => s.ToUpper())
来源：http://ldh.sysykeji.top

[C08] 闭包
来源：http://qeh.yj20258.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://pen.shzxlz.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://pnu.xinyue.icu

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mfd.zdbjq.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://qpu.vehdjk.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://uim.zhongyouzk.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://uap.yanxiufei.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://gnw.shzxlz.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://lyl.jinghuilouyu.cn

[C09] 递归
来源：http://xkl.fanxiaobao.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://avt.aibaodan.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://nxj.tian-w.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wkb.yonumen.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rmb.kuanghao11.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://bir.jiagoushi.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://yij.jinqigfzy.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://epb.zhijiandao.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://bnk.tanke756.top

[C10] 变量作用域
来源：http://cft.ybcxt.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://pys.zhongyouzk.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://idw.yj20258888.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ckk.snrcjt.cn

TS:   同 JS
来源：http://ntq.fktsv.cn

Java: 方法内为块级作用域
来源：http://jxq.zhaomingkeji.xyz

Go:   花括号块级作用域
来源：http://buh.cucudq.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ivg.aibaodan.cn

C#:   块级作用域
来源：http://mgx.pengpengdd.cyou

[C11] 模块导入与导出
来源：http://nzl.fzhhl.top

Py:   from module import func
来源：http://npy.chenjidiqi.icu

PHP:  require "file.php";  或 use App\Service;
来源：http://bng.zdbjq.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://lrt.uphjek.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hqu.pycfn.com

Java: import java.util.List;
来源：http://ket.gaohongyu789.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ieh.hammf.cn

Ruby: require "json"; require_relative "./util"
来源：http://inh.gzhubu.top

C#:   using System.Text;
来源：http://idq.c1oappe.top

[C12] 立即执行函数 IIFE
来源：http://kgd.shanyushiyangtech.top

Py:   (lambda: print("run"))()
来源：http://exh.shzxlz.cn

PHP:  (function () { echo "run"; })();
来源：http://jch.xinyue.icu

JS:   (() => { console.log("run"); })();
来源：http://esv.nanxuanxn.top

TS:   (() => { console.log("run"); })();
来源：http://lar.vqdsnc.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://sld.pycfn.com

Go:   func() { fmt.Println("run") }()
来源：http://unt.smart0.xyz

Ruby: -> { puts "run" }.call
来源：http://gua.jqgfzy.top

C#:   // 无 IIFE：用静态构造函数
来源：http://iop.hywenlv.cn

[C13] 类型声明 / 类型注解
来源：http://oza.nanxinkj.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://pje.xylfe.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ybc.yanxiufei.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://sew.xinyue.icu

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vev.ybcxt.top

Java: int add(int a, int b) { return a + b; }
来源：http://sqc.tarul.cn

Go:   func add(a, b int) int
来源：http://kfe.ctjpmb.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://xgj.zycfv.cn

C#:   int Add(int a, int b) => a + b;
来源：http://vnm.yonumen.top

[C14] 泛型函数
来源：http://tce.xuetiantiany.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hmb.guowangkeji.top

PHP:  // 无泛型
来源：http://ulw.xingfuxueyuan.xyz

JS:   // 无泛型
来源：http://umm.chenzaomai.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://iel.nanxinkj.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ggh.hnqzz.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://bdg.ivvv.top

Ruby: # 无泛型
来源：http://sni.havefunace.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://fwq.guannengcc.top

[C15] 解构 / 展开参数
来源：http://qfk.gogol.net.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://vai.snrcjt.cn

PHP:  [$a, $b] = $pair;
来源：http://ikr.feifeiyinyue.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://nkn.xuanzx.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://voi.sysykeji.top

Java: // 无解构
来源：http://ztp.guowangkeji.top

Go:   // 无解构
来源：http://fto.yonumen.top

Ruby: a, b = pair
来源：http://skc.havefunace.top

C#:   var (a, b) = pair;
来源：http://pdv.jinqigufen.top

[C16] 函数 / 方法重载
来源：http://psn.tian-w.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://lqy.cheryme.top

PHP:  // 无重载
来源：http://ihn.smart0.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://gzr.shangyingyoupin.top

TS:   // 用联合类型或重载签名声明
来源：http://kby.hesvh.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://iji.havefunace.top

Go:   // 无重载：用不同函数名
来源：http://wzq.chenzaomai.com

Ruby: # 无重载：靠动态参数
来源：http://pat.sweek.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://ibn.uphjek.com

================================================================================
来源：http://npt.sweek.top

D. 数组 / 列表 / 集合
来源：http://ocp.fktsv.cn

================================================================================
来源：http://bgp.yanxiufei.cn

[D01] 创建数组 / 列表
来源：http://sar.cheryme.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://zem.aibaodan.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://jxu.gzhubu.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://rjq.kuanghao11.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ebv.jinqigufen.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://eyp.vqdsnc.cn

Go:   arr := []int{1, 2, 3}
来源：http://kxe.hysaishi.cn

Ruby: arr = [1, 2, 3]
来源：http://hut.yangfankeji.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://orn.cheryme.top

[D02] 追加元素到末尾
来源：http://zch.tarul.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://aba.gzhubu.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wjc.ydzc1.top

JS:   arr.push(4);
来源：http://ccl.sxryk.cn

TS:   arr.push(4);
来源：http://wkb.bjfxy.top

Java: list.add(4);
来源：http://imk.yj20258888.top

Go:   arr = append(arr, 4)
来源：http://ilu.iojbl.cn

Ruby: arr << 4; arr.push(5)
来源：http://fih.uphjek.com

C#:   list.Add(4);
来源：http://jbu.9152youxi.cn

[D03] 在指定位置插入元素
来源：http://tif.tian-w.cn

Py:   arr.insert(0, 0)
来源：http://ngy.yangfankeji.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ioa.jqgufenzy.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://iui.cqqwz.cn

TS:   arr.splice(0, 0, 0);
来源：http://wjs.vehdjk.com

Java: list.add(0, 0);
来源：http://abq.pengpengdd.cyou

Go:   arr = append([]int{0}, arr...)
来源：http://hhj.yonumen.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://sdc.jianghu66.top

C#:   list.Insert(0, 0);
来源：http://xex.yongpay.top

[D04] 删除元素
来源：http://wol.c1oappe.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://zpo.nwbrower.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://lad.yonumen.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://oxr.cucudq.cn

TS:   arr.splice(0, 1);
来源：http://twy.redwolf501.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://vuc.gaohongyu789.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://elz.jqgfzy.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://rjs.ivvv.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://zjd.wangdashe.top

[D05] 访问与修改元素
来源：http://klp.xziqi.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://zer.shzxlz.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mcy.aizwys.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ucu.wangdashe.top

TS:   arr[0]; arr.at(-1);
来源：http://qyf.shanyushiyangtech.top

Java: list.get(0); list.set(0, 9);
来源：http://fzj.fzhhl.top

Go:   arr[0]; arr[0] = 9
来源：http://tri.jiagoushi.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://tns.mhx1999.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mlf.zdbjq.cn

[D06] 数组长度
来源：http://hcw.vehdjk.com

Py:   len(arr)
来源：http://kwb.zhijiandao.cn

PHP:  count($arr);
来源：http://cdu.jinqigfzy.top

JS:   arr.length
来源：http://hos.gaohongyu789.top

TS:   arr.length
来源：http://wkh.daria6918.cn

Java: list.size();
来源：http://ytu.smart0.xyz

Go:   len(arr)
来源：http://edj.316326.xyz

Ruby: arr.length; arr.size
来源：http://hci.sweek.top

C#:   list.Count;
来源：http://ovy.shzxlz.cn

[D07] 切片 / 取子数组
来源：http://xrs.ydjk.org.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://oly.9152youxi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://vso.yonumen.top

JS:   arr.slice(1, 4);
来源：http://bwm.fktsv.cn

TS:   arr.slice(1, 4);
来源：http://xld.ydjk.org.cn

Java: list.subList(1, 4);
来源：http://avj.jqgufenzy.top

Go:   arr[1:4]
来源：http://wfm.fanxiaobao.xyz

Ruby: arr[1, 3]
来源：http://wti.hnxiangtu.top

C#:   list.GetRange(1, 3);
来源：http://fji.xziqi.cn

[D08] 合并两个数组
来源：http://nwm.meibo888.top

Py:   a + b;  a.extend(b)
来源：http://clw.zhijiandao.cn

PHP:  array_merge($a, $b);
来源：http://fuy.hfpthk.cn


<!-- 参考信息 -->