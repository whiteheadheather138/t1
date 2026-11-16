代发 wailian999

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://lst.0kj1m.cn

Ruby: while i < 10; i += 1; end
来源：http://gkf.nwbrower.top

C#:   while (i < 10) { i++; }
来源：http://oav.shzxlz.cn

[B08] do-while（至少执行一次）
来源：http://afw.xingfuxueyuan.xyz

Py:   # 无 do-while：用 while True + break
来源：http://afl.jiagoushi.top

PHP:  do { $i++; } while ($i < 10);
来源：http://ygh.yonumen.top

JS:   do { i++; } while (i < 10);
来源：http://jhb.hysaishi.cn

TS:   do { i++; } while (i < 10);
来源：http://mjw.ppjwa.cn

Java: do { i++; } while (i < 10);
来源：http://qxz.jqgufenzy.top

Go:   for { i++; if i >= 10 { break } }
来源：http://vqz.cheryme.top

Ruby: begin; i += 1; end while i < 10
来源：http://dkp.feifeiyinyue.top

C#:   do { i++; } while (i < 10);
来源：http://lvq.zhixingplan.top

[B09] break 与 continue
来源：http://jxk.ehwqpu.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://xfu.jinqigufen.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ame.yangfankeji.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vds.cashguo.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ahm.yueranfly.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nsx.hammf.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://rrn.iojbl.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://dta.yj202588.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qfw.sxryk.cn

[B10] 遍历同时拿索引
来源：http://lcm.wangshuangyany.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://bgy.guowangkeji.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://fyp.guowangkeji.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://zjq.aibaodan.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://lpf.iojbl.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://vmf.smart0.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://tar.yj20258888.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://lwg.sxryk.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://tsq.yj202588.top

[B11] 生成数字序列 / 区间
来源：http://sjk.guowangkeji.top

Py:   list(range(0, 10, 2))
来源：http://lac.xingfuxueyuan.xyz

PHP:  range(0, 10, 2);
来源：http://ywu.sufxvd.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bzb.aizwys.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://buy.ehwqpu.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wwu.tian-w.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://tip.hfpthk.cn

Ruby: (0...10).step(2).to_a
来源：http://hhy.zhijiandao.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://udt.daxiang520.top

[B12] 跳出多层循环
来源：http://lsp.tian-w.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://zwy.xuetiantiany.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://bok.jiagoushi.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://vye.jinghuilouyu.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://doj.ehwqpu.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://kmd.jlsjyb.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ldn.zycfv.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://pxi.yj20258888.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://aln.andypj.xyz

[B13] 判断是否为数字
来源：http://kwp.yfazqb.com

Py:   isinstance(x, (int, float))
来源：http://zjv.uphjek.com

PHP:  is_numeric($x)
来源：http://vvg.guannengcc.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xqo.dianchejie.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ido.daxiang520.top

Java: x instanceof Number
来源：http://jdf.9152youxi.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://xem.vqdsnc.cn

Ruby: x.is_a?(Numeric)
来源：http://imu.yueranfly.top

C#:   x is int or double or decimal
来源：http://xkm.yj20258888.top

[B14] 判断值是否在集合内
来源：http://lzn.ivvv.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://zvr.aibaodan.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://xdx.jianghu66.top

JS:   [1, 2, 3].includes(x)
来源：http://zqy.shanyushiyangtech.top

TS:   [1, 2, 3].includes(x)
来源：http://ucz.jinqigufen.top

Java: List.of(1, 2, 3).contains(x)
来源：http://xyc.yongpay.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://xgy.tianlin.xyz

Ruby: [1, 2, 3].include?(x)
来源：http://pen.9152youxi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://fgk.uphjek.com

[B15] 布尔运算与取反
来源：http://mmi.nanxuanxn.top

Py:   a and b or not c
来源：http://xsy.pengpengdd.cyou

PHP:  $a && $b || !$c
来源：http://gfo.vehdjk.com

JS:   a && b || !c
来源：http://irx.yvedp.cn

TS:   a && b || !c
来源：http://kcf.zhijiandao.cn

Java: a && b || !c
来源：http://eoy.yj202588.top

Go:   a && b || !c
来源：http://yjj.zhengqikj.top

Ruby: a && b || !c
来源：http://ywa.sweek.top

C#:   a && b || !c
来源：http://fqh.zhiwuduotai.top

[B16] 卫语句：不满足条件提前返回
来源：http://ahm.uphjek.com

Py:   if not data: return
来源：http://wqv.zhaomingkeji.xyz

PHP:  if (!$data) { return; }
来源：http://zmw.bbcook.cn

JS:   if (!data) return;
来源：http://yhh.tanke756.top

TS:   if (!data) return;
来源：http://tou.yj20258.top

Java: if (data == null) return;
来源：http://snj.tarul.cn

Go:   if data == nil { return }
来源：http://gmc.hcnkem.com

Ruby: return if data.nil?
来源：http://uhe.jinghuilouyu.cn

C#:   if (data == null) return;
来源：http://koy.jinghuilouyu.cn

================================================================================
来源：http://akj.vqdsnc.cn

C. 函数与作用域
来源：http://afa.zhiwuduotai.top

================================================================================
来源：http://tyn.zhijiandao.cn

[C01] 定义函数
来源：http://yov.yvedp.cn

Py:   def add(a, b): return a + b
来源：http://gul.cdnleiting.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rcc.zhoulong.xyz

JS:   function add(a, b) { return a + b; }
来源：http://sve.havefunace.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nbz.fanxiaobao.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://klv.jiagoushi.top

Go:   func add(a, b int) int { return a + b }
来源：http://uun.xylfe.cn

Ruby: def add(a, b); a + b; end
来源：http://ayk.hnqzz.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://zrm.gogol.net.cn

[C02] 默认参数
来源：http://mvm.yj20258888.top

Py:   def greet(name="World"): return name
来源：http://brb.meibo888.top

PHP:  function greet($name = "World") { return $name; }
来源：http://any.nanxinkj.top

JS:   function greet(name = "World") { return name; }
来源：http://gwm.52xcode.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://eet.hesvh.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://jbu.chenjidiqi.icu

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://sjd.zhijiandao.cn

Ruby: def greet(name = "World") = name
来源：http://cop.wangdashe.top

C#:   string Greet(string name = "World") => name;
来源：http://rpu.nwbrower.top

[C03] 可变参数
来源：http://myl.wangdashe.top

Py:   def total(*args): return sum(args)
来源：http://bpd.fengsongda.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://uam.zhongyouzk.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hts.yj20258888.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://for.feifeiyinyue.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wgm.cheryme.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://jqi.pycfn.com

Ruby: def total(*nums); nums.sum; end
来源：http://nfx.nanxinkj.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://img.jinqigfzy.top

[C04] 命名参数 / 关键字参数
来源：http://luu.yj20258.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://whw.dashuyun.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://jso.shzxlz.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://iwg.guowangkeji.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://zcx.xuetiantiany.cn

Java: // 无：用 Builder 模式或 record
来源：http://zzu.fanxiaobao.xyz

Go:   // 无：用配置结构体参数
来源：http://gag.aibaodan.cn

Ruby: f(a: 1, b: 2)
来源：http://zia.zhengqikj.top

C#:   f(a: 1, b: 2)
来源：http://ptr.jqgufenzy.top

[C05] 返回多个值
来源：http://cbj.zhoulong.xyz

Py:   return a, b
来源：http://rmr.fanxiaobao.xyz

PHP:  return [$a, $b];
来源：http://mqt.xylfe.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://fsr.yonumen.top

TS:   return { a, b };
来源：http://scz.hysaishi.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://tyo.chenlongwang.top

Go:   return a, b
来源：http://ewq.hysaishi.cn

Ruby: return a, b
来源：http://gpo.yj202588.top

C#:   return (a, b);              // ValueTuple
来源：http://bdg.cdnleiting.top

[C06] 匿名函数 / lambda
来源：http://dzi.hnqzz.top

Py:   square = lambda x: x * x
来源：http://eom.pycfn.com

PHP:  $square = fn($x) => $x * $x;
来源：http://bmy.ehwqpu.com

JS:   const square = x => x * x;
来源：http://vvo.hcnkem.com

TS:   const square = (x: number): number => x * x;
来源：http://vno.fanxiaobao.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://rvn.hnqzz.top

Go:   sq := func(x int) int { return x * x }
来源：http://kah.yonumen.top

Ruby: square = ->(x) { x * x }
来源：http://ldl.kuanghao11.cn

C#:   Func<int, int> square = x => x * x;
来源：http://qyn.dashuyun.cn

[C07] 把函数作为参数传入
来源：http://qzb.yfazqb.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wgg.aizwys.cn

PHP:  array_map("strtoupper", $arr);
来源：http://beg.guannengcc.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ybo.yj202588.top

TS:   arr.map(String)
来源：http://cxi.shanyushiyangkeji.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://vno.wangshuangyany.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qvj.shangyingyoupin.top

Ruby: arr.map(&:upcase)
来源：http://tdz.guowangkeji.top

C#:   arr.Select(s => s.ToUpper())
来源：http://tzo.sysykeji.top

[C08] 闭包
来源：http://blq.yueranfly.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://tzr.gogol.net.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ugw.guowangkeji.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://eub.gogol.net.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://tzs.tian-w.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://toi.cashguo.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://fil.aizwys.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mhf.wangshuangyany.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://jjy.yj20258888.top

[C09] 递归
来源：http://nog.cdnleiting.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mra.shuidangran.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://nqc.hywenlv.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vvt.cucudq.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bzm.snrcjt.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://cws.zhengqikj.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ieb.zdbjq.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://dbk.nwbrower.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://sfi.cashguo.top

[C10] 变量作用域
来源：http://jft.tarul.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://xgp.shanyushiyangtech.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://oqs.daria6918.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://dhb.zhengqikj.top

TS:   同 JS
来源：http://fst.yvedp.cn

Java: 方法内为块级作用域
来源：http://ivb.guannengcc.top

Go:   花括号块级作用域
来源：http://uuo.tanke756.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://qov.dashuyun.cn

C#:   块级作用域
来源：http://grw.fehbvm.com

[C11] 模块导入与导出
来源：http://rap.yangfankeji.com

Py:   from module import func
来源：http://aoh.zhixingplan.top

PHP:  require "file.php";  或 use App\Service;
来源：http://zvm.chenzaomai.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://yhs.iojbl.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://map.redwolf501.top

Java: import java.util.List;
来源：http://otf.jinyuanbaomall.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hoe.cheryme.top

Ruby: require "json"; require_relative "./util"
来源：http://vho.shzxlz.cn

C#:   using System.Text;
来源：http://ofl.jiagoushi.top

[C12] 立即执行函数 IIFE
来源：http://abs.andypj.xyz

Py:   (lambda: print("run"))()
来源：http://igh.wangdashe.top

PHP:  (function () { echo "run"; })();
来源：http://nen.52xcode.cn

JS:   (() => { console.log("run"); })();
来源：http://oso.jinghuilouyu.cn

TS:   (() => { console.log("run"); })();
来源：http://mqt.ywan-chungtsiang.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://suv.cucudq.cn

Go:   func() { fmt.Println("run") }()
来源：http://zsm.sxryk.cn

Ruby: -> { puts "run" }.call
来源：http://gxb.52xcode.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ppc.zhijiandao.cn

[C13] 类型声明 / 类型注解
来源：http://vny.tianlin.xyz

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hgm.wangshuangyany.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cjd.jlsjyb.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://qix.xylfe.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yek.zhoulong.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://zfe.aizwys.cn

Go:   func add(a, b int) int
来源：http://neb.sxryk.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hgd.xingfuxueyuan.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://fpd.guannengcc.top

[C14] 泛型函数
来源：http://yln.fengsongda.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://icz.xingfuxueyuan.xyz

PHP:  // 无泛型
来源：http://tbe.aibaodan.cn

JS:   // 无泛型
来源：http://wdk.daria6918.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://alv.shuidangran.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://slo.yuxming.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ufb.quarkkingdee.top

Ruby: # 无泛型
来源：http://gbl.ppjwa.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://zvd.tanke756.top

[C15] 解构 / 展开参数
来源：http://fcf.hnqzz.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://cqt.smart0.xyz

PHP:  [$a, $b] = $pair;
来源：http://ast.zhoulong.xyz

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://jrk.jinqigufen.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://lyb.ywan-chungtsiang.top

Java: // 无解构
来源：http://hbv.hywenlv.cn

Go:   // 无解构
来源：http://cuq.vehdjk.com

Ruby: a, b = pair
来源：http://qfk.hammf.cn

C#:   var (a, b) = pair;
来源：http://igw.zhoulong.xyz

[C16] 函数 / 方法重载
来源：http://ecm.xuanzx.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wcs.zhixingplan.top

PHP:  // 无重载
来源：http://pvq.aizwys.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://fup.ydzc1.top

TS:   // 用联合类型或重载签名声明
来源：http://wuh.sjlbkw.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://dzk.jinyuanbaomall.cn

Go:   // 无重载：用不同函数名
来源：http://mmr.zhengqikj.top

Ruby: # 无重载：靠动态参数
来源：http://ciq.shanyushiyangkeji.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://kdj.ybcxt.top

================================================================================
来源：http://pas.kuanghao11.cn

D. 数组 / 列表 / 集合
来源：http://mow.shuidangran.top

================================================================================
来源：http://jyp.vehdjk.com

[D01] 创建数组 / 列表
来源：http://lzp.fktsv.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://qqf.zdqjudy.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ijn.cucudq.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://gag.ctjpmb.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://ezp.sjlbkw.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://pjy.ydjk.org.cn

Go:   arr := []int{1, 2, 3}
来源：http://zfy.ydjk.org.cn

Ruby: arr = [1, 2, 3]
来源：http://fhm.smart0.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://vdv.sysykeji.top

[D02] 追加元素到末尾
来源：http://bhx.meibo888.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hpu.yueranfly.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ipm.cqqwz.cn

JS:   arr.push(4);
来源：http://brh.fengsongda.top

TS:   arr.push(4);
来源：http://iwc.xziqi.cn

Java: list.add(4);
来源：http://qyj.ehwqpu.com

Go:   arr = append(arr, 4)
来源：http://xys.aibaodan.cn

Ruby: arr << 4; arr.push(5)
来源：http://hhm.yj202588.top

C#:   list.Add(4);
来源：http://lzz.ppjwa.cn

[D03] 在指定位置插入元素
来源：http://iez.9152youxi.cn

Py:   arr.insert(0, 0)
来源：http://iwy.shzxlz.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wvu.hfpthk.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ljd.hnqzz.top

TS:   arr.splice(0, 0, 0);
来源：http://ztc.yonumen.top

Java: list.add(0, 0);
来源：http://hio.shangyingyoupin.top

Go:   arr = append([]int{0}, arr...)
来源：http://qsv.daxiang520.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://kgx.cheryme.top

C#:   list.Insert(0, 0);
来源：http://jac.zdqjudy.top

[D04] 删除元素
来源：http://xbv.tarul.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ugs.yueranfly.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wxf.shanyushiyangkeji.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://yez.ehwqpu.com

TS:   arr.splice(0, 1);
来源：http://fwf.quarkkingdee.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://yry.xingfuxueyuan.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://sdt.zdbjq.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://fkm.yanxiufei.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mcx.sweek.top

[D05] 访问与修改元素
来源：http://qzu.hcnkem.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://aiu.dashuyun.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ebz.tarul.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ovg.sjlbkw.cn

TS:   arr[0]; arr.at(-1);
来源：http://uav.pengpengdd.cyou

Java: list.get(0); list.set(0, 9);
来源：http://apz.jinqigufen.top

Go:   arr[0]; arr[0] = 9
来源：http://djh.yonumen.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ywr.zhaomingkeji.xyz

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://nor.shuidangran.top

[D06] 数组长度
来源：http://vfw.fanxiaobao.xyz

Py:   len(arr)
来源：http://wtk.vehdjk.com

PHP:  count($arr);
来源：http://qpk.pengpengdd.cyou

JS:   arr.length
来源：http://ylz.jyoumei.cn

TS:   arr.length
来源：http://ngp.dashuyun.cn

Java: list.size();
来源：http://ypt.zdbjq.cn

Go:   len(arr)
来源：http://yey.hongshengwenyu.top

Ruby: arr.length; arr.size
来源：http://vwh.fktsv.cn

C#:   list.Count;
来源：http://chj.tarul.cn

[D07] 切片 / 取子数组
来源：http://xax.xuetiantiany.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ryj.redwolf501.top

PHP:  array_slice($arr, 1, 3);
来源：http://jsw.guannengcc.top

JS:   arr.slice(1, 4);
来源：http://hay.nwbrower.top

TS:   arr.slice(1, 4);
来源：http://xuk.hnxiangtu.top

Java: list.subList(1, 4);
来源：http://qpn.xuanzx.com

Go:   arr[1:4]
来源：http://gdf.xinyue.icu

Ruby: arr[1, 3]
来源：http://okl.yj202588.top

C#:   list.GetRange(1, 3);
来源：http://axe.yuxming.cn

[D08] 合并两个数组
来源：http://ujh.bbcook.cn

Py:   a + b;  a.extend(b)
来源：http://gkt.guowangkeji.top

PHP:  array_merge($a, $b);
来源：http://wpc.fzhhl.top


<!-- 参考信息 -->