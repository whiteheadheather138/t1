代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://xgt.zycfv.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://nam.yongpay.top

JS:   do { i++; } while (i < 10);
来源：http://jem.nanxinkj.top

TS:   do { i++; } while (i < 10);
来源：http://yiz.aizwys.cn

Java: do { i++; } while (i < 10);
来源：http://suf.xinyue.icu

Go:   for { i++; if i >= 10 { break } }
来源：http://gfs.cdnleiting.top

Ruby: begin; i += 1; end while i < 10
来源：http://gdp.ctjpmb.com

C#:   do { i++; } while (i < 10);
来源：http://gat.tianlin.xyz

[B09] break 与 continue
来源：http://mrd.meibo888.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://uru.hysaishi.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://jpy.cashguo.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yfj.wangshuangyany.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ixf.andypj.xyz

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eha.nanxinkj.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://qhp.pengpengdd.cyou

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://krm.cucudq.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hza.ywan-chungtsiang.top

[B10] 遍历同时拿索引
来源：http://nkj.yuanzhike.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://onu.uphjek.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wgb.jianghu66.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://dvl.shzxlz.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://drx.0kj1m.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://oro.jianghu66.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ugt.hammf.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://yfr.epnwcf.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://qiy.andypj.xyz

[B11] 生成数字序列 / 区间
来源：http://ygl.zdbjq.cn

Py:   list(range(0, 10, 2))
来源：http://ucl.jyoumei.cn

PHP:  range(0, 10, 2);
来源：http://pwl.tarul.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cwn.havefunace.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lkd.jinqigufen.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://bnp.yongpay.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://vup.iojbl.cn

Ruby: (0...10).step(2).to_a
来源：http://czq.snrcjt.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://dnn.shanyushiyangtech.top

[B12] 跳出多层循环
来源：http://cht.haohaochexian.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://rwo.yuanzhike.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://nwm.xuanzx.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ggg.jqgufenzy.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://feq.yj202588.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://jnr.zhaomingkeji.xyz

Go:   # 无标签：用布尔标志或抽成函数
来源：http://pyg.haohaochexian.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://xva.hysaishi.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://oks.meibo888.top

[B13] 判断是否为数字
来源：http://pfq.chenjidiqi.icu

Py:   isinstance(x, (int, float))
来源：http://ztj.hnxiangtu.top

PHP:  is_numeric($x)
来源：http://tld.yvedp.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hcd.ybcxt.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pbh.feifeiyinyue.top

Java: x instanceof Number
来源：http://sse.redwolf501.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://aqf.hongshengwenyu.top

Ruby: x.is_a?(Numeric)
来源：http://uth.epnwcf.com

C#:   x is int or double or decimal
来源：http://cey.zhongyouzk.top

[B14] 判断值是否在集合内
来源：http://yqa.dianchejie.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jjq.jiagoushi.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://aip.ivvv.top

JS:   [1, 2, 3].includes(x)
来源：http://toe.iojbl.cn

TS:   [1, 2, 3].includes(x)
来源：http://dsr.aibaodan.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ojh.chenzaomai.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://vgv.andypj.xyz

Ruby: [1, 2, 3].include?(x)
来源：http://cha.shangyingyoupin.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://prw.hongshengwenyu.top

[B15] 布尔运算与取反
来源：http://suw.yvedp.cn

Py:   a and b or not c
来源：http://pnx.ctjpmb.com

PHP:  $a && $b || !$c
来源：http://qft.svipenyu.cn

JS:   a && b || !c
来源：http://tfo.dashuyun.cn

TS:   a && b || !c
来源：http://vuk.tian-w.cn

Java: a && b || !c
来源：http://hus.gotoacloud.top

Go:   a && b || !c
来源：http://qlc.pengpengdd.cyou

Ruby: a && b || !c
来源：http://vgx.ivvv.top

C#:   a && b || !c
来源：http://aro.epnwcf.com

[B16] 卫语句：不满足条件提前返回
来源：http://rxg.zhijiandao.cn

Py:   if not data: return
来源：http://pqd.hnxiangtu.top

PHP:  if (!$data) { return; }
来源：http://xrn.zhijiandao.cn

JS:   if (!data) return;
来源：http://rcp.zdqjudy.top

TS:   if (!data) return;
来源：http://nkg.hnqzz.top

Java: if (data == null) return;
来源：http://qqg.zdbjq.cn

Go:   if data == nil { return }
来源：http://ozj.bjfxy.top

Ruby: return if data.nil?
来源：http://fpy.smart0.xyz

C#:   if (data == null) return;
来源：http://olu.chenlongwang.top

================================================================================
来源：http://mdj.xuetiantiany.cn

C. 函数与作用域
来源：http://bkx.dashuyun.cn

================================================================================
来源：http://fjq.kuanghao11.cn

[C01] 定义函数
来源：http://szw.fengsongda.top

Py:   def add(a, b): return a + b
来源：http://tyt.yanxiufei.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://trk.316326.xyz

JS:   function add(a, b) { return a + b; }
来源：http://ooc.cqqwz.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fgf.guowangkeji.top

Java: static int add(int a, int b) { return a + b; }
来源：http://iqu.shzxlz.cn

Go:   func add(a, b int) int { return a + b }
来源：http://rrg.meibo888.top

Ruby: def add(a, b); a + b; end
来源：http://apt.chenjidiqi.icu

C#:   static int Add(int a, int b) { return a + b; }
来源：http://bsq.mhx1999.top

[C02] 默认参数
来源：http://xhv.mhx1999.top

Py:   def greet(name="World"): return name
来源：http://mpo.jiagoushi.top

PHP:  function greet($name = "World") { return $name; }
来源：http://xng.xziqi.cn

JS:   function greet(name = "World") { return name; }
来源：http://bnl.iojbl.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://gom.ydzc1.top

Java: // 无默认参数：方法重载或 Optional
来源：http://wzz.xingfuxueyuan.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://dqs.yonumen.top

Ruby: def greet(name = "World") = name
来源：http://tpg.sweek.top

C#:   string Greet(string name = "World") => name;
来源：http://wle.feifeiyinyue.top

[C03] 可变参数
来源：http://fxa.haohaochexian.top

Py:   def total(*args): return sum(args)
来源：http://sld.pycfn.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://lwn.sxryk.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://fbx.tanke756.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://yoq.fehbvm.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://gdy.hnxiangtu.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://uqo.zdqjudy.top

Ruby: def total(*nums); nums.sum; end
来源：http://gnl.nwbrower.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://vgt.9152youxi.cn

[C04] 命名参数 / 关键字参数
来源：http://odg.vqdsnc.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://xvw.chenlongwang.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mlx.dianchejie.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://goy.yueranfly.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://lnp.xziqi.cn

Java: // 无：用 Builder 模式或 record
来源：http://nei.fzhhl.top

Go:   // 无：用配置结构体参数
来源：http://end.fktsv.cn

Ruby: f(a: 1, b: 2)
来源：http://nwl.bbcook.cn

C#:   f(a: 1, b: 2)
来源：http://iwc.ybcxt.top

[C05] 返回多个值
来源：http://nla.cashguo.top

Py:   return a, b
来源：http://wmc.shzxlz.cn

PHP:  return [$a, $b];
来源：http://ywq.hammf.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://zsa.wangshuangyany.cn

TS:   return { a, b };
来源：http://som.jinghuilouyu.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://khw.ivvv.top

Go:   return a, b
来源：http://fdq.nanxinkj.top

Ruby: return a, b
来源：http://qew.daria6918.cn

C#:   return (a, b);              // ValueTuple
来源：http://mtw.zdbjq.cn

[C06] 匿名函数 / lambda
来源：http://scz.bbcook.cn

Py:   square = lambda x: x * x
来源：http://qfa.kuanghao11.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://gme.sweek.top

JS:   const square = x => x * x;
来源：http://oxz.fengsongda.top

TS:   const square = (x: number): number => x * x;
来源：http://hmp.fengsongda.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ulj.cucudq.cn

Go:   sq := func(x int) int { return x * x }
来源：http://psa.hywenlv.cn

Ruby: square = ->(x) { x * x }
来源：http://cwq.sweek.top

C#:   Func<int, int> square = x => x * x;
来源：http://xga.gaohongyu789.top

[C07] 把函数作为参数传入
来源：http://xlw.fehbvm.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://sou.kuanghao11.cn

PHP:  array_map("strtoupper", $arr);
来源：http://dxx.hesvh.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://koq.haohaochexian.top

TS:   arr.map(String)
来源：http://epn.vehdjk.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://iha.cashguo.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://whl.fengsongda.top

Ruby: arr.map(&:upcase)
来源：http://kwx.guowangkeji.top

C#:   arr.Select(s => s.ToUpper())
来源：http://zji.haohaochexian.top

[C08] 闭包
来源：http://ojm.xingfuxueyuan.xyz

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://soh.yuxming.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://kwa.316326.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://fsy.hysaishi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://vvw.zdbjq.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://umy.xziqi.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://dux.jlsjyb.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://yzl.cucudq.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://xll.ydjk.org.cn

[C09] 递归
来源：http://erz.jqgufenzy.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://rci.feifeiyinyue.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://kqw.yj20258888.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hco.sjlbkw.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bhm.jinghuilouyu.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://zaq.andypj.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://tmu.zhaomingkeji.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hpu.zhixingplan.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://vgn.ydjk.org.cn

[C10] 变量作用域
来源：http://jec.jqgufenzy.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://uad.hammf.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wnn.wangshuangyany.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://iuy.cdnleiting.top

TS:   同 JS
来源：http://aqw.zhijiandao.cn

Java: 方法内为块级作用域
来源：http://bwt.ehwqpu.com

Go:   花括号块级作用域
来源：http://ere.hammf.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://pkx.aizwys.cn

C#:   块级作用域
来源：http://tee.ydzc1.top

[C11] 模块导入与导出
来源：http://ime.tian-w.cn

Py:   from module import func
来源：http://skk.meibo888.top

PHP:  require "file.php";  或 use App\Service;
来源：http://irv.jinghuilouyu.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://xfq.feifeiyinyue.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://fjo.yueranfly.top

Java: import java.util.List;
来源：http://vdc.zdbjq.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://aau.hnxiangtu.top

Ruby: require "json"; require_relative "./util"
来源：http://kph.c1oappe.top

C#:   using System.Text;
来源：http://iuq.sufxvd.cn

[C12] 立即执行函数 IIFE
来源：http://kfa.chenjidiqi.icu

Py:   (lambda: print("run"))()
来源：http://jcm.zdbjq.cn

PHP:  (function () { echo "run"; })();
来源：http://duy.smart0.xyz

JS:   (() => { console.log("run"); })();
来源：http://mek.52xcode.cn

TS:   (() => { console.log("run"); })();
来源：http://mza.vehdjk.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ajd.cqqwz.cn

Go:   func() { fmt.Println("run") }()
来源：http://wed.nanxinkj.top

Ruby: -> { puts "run" }.call
来源：http://wxt.feifeiyinyue.top

C#:   // 无 IIFE：用静态构造函数
来源：http://esg.meibo888.top

[C13] 类型声明 / 类型注解
来源：http://ven.jinqigufen.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://oxp.daxiang520.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://eaf.jianghu66.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://pgg.jinqigfzy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cil.jyoumei.cn

Java: int add(int a, int b) { return a + b; }
来源：http://kue.hesvh.cn

Go:   func add(a, b int) int
来源：http://fhs.yanxiufei.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://luh.gaohongyu789.top

C#:   int Add(int a, int b) => a + b;
来源：http://gjr.hnqzz.top

[C14] 泛型函数
来源：http://mzc.hnxiangtu.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://dta.cashguo.top

PHP:  // 无泛型
来源：http://ocg.xylfe.cn

JS:   // 无泛型
来源：http://mta.fengsongda.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://cmg.nanxinkj.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://qtl.cheryme.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://soa.zhijiandao.cn

Ruby: # 无泛型
来源：http://rmn.zhongyouzk.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wlt.nanxuanxn.top

[C15] 解构 / 展开参数
来源：http://nfr.fehbvm.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mtu.yuxming.cn

PHP:  [$a, $b] = $pair;
来源：http://fkl.sjlbkw.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://jpj.smart0.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://qbm.quarkkingdee.top

Java: // 无解构
来源：http://esj.ctjpmb.com

Go:   // 无解构
来源：http://wwg.haohaochexian.top

Ruby: a, b = pair
来源：http://csj.gogol.net.cn

C#:   var (a, b) = pair;
来源：http://vzz.yuanzhike.top

[C16] 函数 / 方法重载
来源：http://flj.sufxvd.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://cgq.jianghu66.top

PHP:  // 无重载
来源：http://mor.pycfn.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://erc.bbcook.cn

TS:   // 用联合类型或重载签名声明
来源：http://atj.hcnkem.com

Java: void f(int a) {}  void f(String a) {}
来源：http://gmi.yuanzhike.top

Go:   // 无重载：用不同函数名
来源：http://hvu.316326.xyz

Ruby: # 无重载：靠动态参数
来源：http://csv.shanyushiyangkeji.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://xlw.andypj.xyz

================================================================================
来源：http://yhb.sufxvd.cn

D. 数组 / 列表 / 集合
来源：http://vrx.jlsjyb.cn

================================================================================
来源：http://tbn.hongshengwenyu.top

[D01] 创建数组 / 列表
来源：http://czf.sjlbkw.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://jcq.quarkkingdee.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://lvi.mhx1999.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://iku.daxiang520.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://cqu.cucudq.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://sdu.meibo888.top

Go:   arr := []int{1, 2, 3}
来源：http://euu.yuanzhike.top

Ruby: arr = [1, 2, 3]
来源：http://wul.sxryk.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://fbi.cucudq.cn

[D02] 追加元素到末尾
来源：http://mtv.iojbl.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://yan.zhengqikj.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://xzh.meibo888.top

JS:   arr.push(4);
来源：http://ani.shanyushiyangkeji.top

TS:   arr.push(4);
来源：http://xbb.zhongyouzk.top

Java: list.add(4);
来源：http://fih.zycfv.cn

Go:   arr = append(arr, 4)
来源：http://ipi.cdnleiting.top

Ruby: arr << 4; arr.push(5)
来源：http://jax.vqdsnc.cn

C#:   list.Add(4);
来源：http://mho.yj202588.top

[D03] 在指定位置插入元素
来源：http://fss.kuanghao11.cn

Py:   arr.insert(0, 0)
来源：http://nmg.sweek.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://qut.yuxming.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://uol.jyoumei.cn

TS:   arr.splice(0, 0, 0);
来源：http://ips.fehbvm.com

Java: list.add(0, 0);
来源：http://yvg.pengpengdd.cyou

Go:   arr = append([]int{0}, arr...)
来源：http://nzq.sjlbkw.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://xqx.cqqwz.cn

C#:   list.Insert(0, 0);
来源：http://ijs.yj202588.top

[D04] 删除元素
来源：http://rzx.yj20258888.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://pto.fanxiaobao.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://yfc.shuidangran.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://uzd.vehdjk.com

TS:   arr.splice(0, 1);
来源：http://hva.chenzaomai.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://eia.haohaochexian.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://muc.yonumen.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hqh.zhengqikj.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://kfk.xuanzx.com

[D05] 访问与修改元素
来源：http://far.gzhubu.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://yuz.tianlin.xyz

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://imu.cdnleiting.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wsn.cdnleiting.top

TS:   arr[0]; arr.at(-1);
来源：http://atm.yanxiufei.cn

Java: list.get(0); list.set(0, 9);
来源：http://qpe.redwolf501.top

Go:   arr[0]; arr[0] = 9
来源：http://jmt.fengsongda.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://kpc.snrcjt.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://nag.tian-w.cn

[D06] 数组长度
来源：http://rci.bjfxy.top

Py:   len(arr)
来源：http://cul.52xcode.cn

PHP:  count($arr);
来源：http://dpr.zhixingplan.top

JS:   arr.length
来源：http://bbw.nanxinkj.top

TS:   arr.length
来源：http://hzu.nanxinkj.top

Java: list.size();
来源：http://adt.0kj1m.cn

Go:   len(arr)
来源：http://gne.iojbl.cn

Ruby: arr.length; arr.size
来源：http://skr.gaohongyu789.top

C#:   list.Count;
来源：http://hyy.jinqigfzy.top

[D07] 切片 / 取子数组
来源：http://etf.yuxming.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://oor.ydzc1.top

PHP:  array_slice($arr, 1, 3);
来源：http://nil.zdbjq.cn

JS:   arr.slice(1, 4);
来源：http://mpm.vehdjk.com

TS:   arr.slice(1, 4);
来源：http://iue.cheryme.top

Java: list.subList(1, 4);
来源：http://wts.52xcode.cn

Go:   arr[1:4]
来源：http://vfm.9152youxi.cn

Ruby: arr[1, 3]
来源：http://xwa.yongpay.top

C#:   list.GetRange(1, 3);
来源：http://vno.gzhubu.top

[D08] 合并两个数组
来源：http://jem.ydzc1.top

Py:   a + b;  a.extend(b)
来源：http://mun.zdqjudy.top

PHP:  array_merge($a, $b);
来源：http://jcj.pengpengdd.cyou

JS:   [...a, ...b];  a.concat(b);
来源：http://upp.smart0.xyz

TS:   [...a, ...b];
来源：http://anx.daxiang520.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://yjf.xziqi.cn

Go:   append(a, b...)
来源：http://whz.fktsv.cn


<!-- 参考信息 -->