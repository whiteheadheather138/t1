代发 wailian999

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://tqw.yueranfly.top

Ruby: while i < 10; i += 1; end
来源：http://zls.hongshengwenyu.top

C#:   while (i < 10) { i++; }
来源：http://rdg.yanxiufei.cn

[B08] do-while（至少执行一次）
来源：http://cmo.birdmap.top

Py:   # 无 do-while：用 while True + break
来源：http://fgz.smart0.xyz

PHP:  do { $i++; } while ($i < 10);
来源：http://zyz.zhijiandao.cn

JS:   do { i++; } while (i < 10);
来源：http://vyi.gzhubu.top

TS:   do { i++; } while (i < 10);
来源：http://rcy.bjfxy.top

Java: do { i++; } while (i < 10);
来源：http://dec.zhiwuduotai.top

Go:   for { i++; if i >= 10 { break } }
来源：http://pot.ydzc1.top

Ruby: begin; i += 1; end while i < 10
来源：http://svf.hnxiangtu.top

C#:   do { i++; } while (i < 10);
来源：http://sto.xylfe.cn

[B09] break 与 continue
来源：http://bnr.316326.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zuq.shangyingyoupin.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://tmv.nanxinkj.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fmv.xuanzx.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uud.havefunace.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dhj.0kj1m.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ngi.svipenyu.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://pib.sysykeji.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rmn.yfazqb.com

[B10] 遍历同时拿索引
来源：http://qif.zhoulong.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://okg.hywenlv.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://gvs.iojbl.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://oyx.nwbrower.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://swv.daxiang520.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wam.zhengqikj.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://vra.jinyuanbaomall.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hum.zhiwuduotai.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mwi.haohaochexian.top

[B11] 生成数字序列 / 区间
来源：http://qvh.jinghuilouyu.cn

Py:   list(range(0, 10, 2))
来源：http://fcg.hesvh.cn

PHP:  range(0, 10, 2);
来源：http://nrs.vehdjk.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://teg.iojbl.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yxq.yj20258.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wse.gogol.net.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://rue.gogol.net.cn

Ruby: (0...10).step(2).to_a
来源：http://dvl.xinyue.icu

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://fnw.vehdjk.com

[B12] 跳出多层循环
来源：http://oaj.guannengcc.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://xmx.hammf.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://dsj.zhengqikj.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://jdk.daria6918.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://vjo.zhixingplan.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://btc.ybcxt.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://rzs.fanxiaobao.xyz

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ony.ydzc1.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://rry.zycfv.cn

[B13] 判断是否为数字
来源：http://pbb.jinyuanbaomall.cn

Py:   isinstance(x, (int, float))
来源：http://fua.cashguo.top

PHP:  is_numeric($x)
来源：http://gxs.smart0.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dxs.jiagoushi.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tva.hongshengwenyu.top

Java: x instanceof Number
来源：http://rxa.nwbrower.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://uvv.c1oappe.top

Ruby: x.is_a?(Numeric)
来源：http://fht.epnwcf.com

C#:   x is int or double or decimal
来源：http://ngx.jlsjyb.cn

[B14] 判断值是否在集合内
来源：http://wnx.sweek.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://nll.pycfn.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://sls.havefunace.top

JS:   [1, 2, 3].includes(x)
来源：http://bld.shangyingyoupin.top

TS:   [1, 2, 3].includes(x)
来源：http://och.ehwqpu.com

Java: List.of(1, 2, 3).contains(x)
来源：http://hnl.aizwys.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wdp.ctjpmb.com

Ruby: [1, 2, 3].include?(x)
来源：http://vtv.feifeiyinyue.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://upw.ctjpmb.com

[B15] 布尔运算与取反
来源：http://juk.nwbrower.top

Py:   a and b or not c
来源：http://uyk.gaohongyu789.top

PHP:  $a && $b || !$c
来源：http://bsh.jinyuanbaomall.cn

JS:   a && b || !c
来源：http://wyp.jyoumei.cn

TS:   a && b || !c
来源：http://sii.meibo888.top

Java: a && b || !c
来源：http://jcu.nanxuanxn.top

Go:   a && b || !c
来源：http://slb.xylfe.cn

Ruby: a && b || !c
来源：http://hye.hnqzz.top

C#:   a && b || !c
来源：http://zke.chenlongwang.top

[B16] 卫语句：不满足条件提前返回
来源：http://frd.dashuyun.cn

Py:   if not data: return
来源：http://oma.dianchejie.cn

PHP:  if (!$data) { return; }
来源：http://qka.tianlin.xyz

JS:   if (!data) return;
来源：http://ckf.0kj1m.cn

TS:   if (!data) return;
来源：http://cpv.yj202588.top

Java: if (data == null) return;
来源：http://ynq.hesvh.cn

Go:   if data == nil { return }
来源：http://jsv.smart0.xyz

Ruby: return if data.nil?
来源：http://pcn.xziqi.cn

C#:   if (data == null) return;
来源：http://rdo.hongshengwenyu.top

================================================================================
来源：http://hfg.fanxiaobao.xyz

C. 函数与作用域
来源：http://acs.zhixingplan.top

================================================================================
来源：http://mzr.zhijiandao.cn

[C01] 定义函数
来源：http://htw.hfpthk.cn

Py:   def add(a, b): return a + b
来源：http://uya.zhongyouzk.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mkl.vqdsnc.cn

JS:   function add(a, b) { return a + b; }
来源：http://sgf.zhixingplan.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://miz.ctjpmb.com

Java: static int add(int a, int b) { return a + b; }
来源：http://zyb.tarul.cn

Go:   func add(a, b int) int { return a + b }
来源：http://vts.cqqwz.cn

Ruby: def add(a, b); a + b; end
来源：http://vpx.sjlbkw.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://qig.feifeiyinyue.top

[C02] 默认参数
来源：http://str.feifeiyinyue.top

Py:   def greet(name="World"): return name
来源：http://hzq.nanxinkj.top

PHP:  function greet($name = "World") { return $name; }
来源：http://vpq.uphjek.com

JS:   function greet(name = "World") { return name; }
来源：http://mha.dashuyun.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://itr.shanyushiyangkeji.top

Java: // 无默认参数：方法重载或 Optional
来源：http://gky.ybcxt.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://bdw.chenjidiqi.icu

Ruby: def greet(name = "World") = name
来源：http://ixe.9152youxi.cn

C#:   string Greet(string name = "World") => name;
来源：http://yrr.dianchejie.cn

[C03] 可变参数
来源：http://lwu.fengsongda.top

Py:   def total(*args): return sum(args)
来源：http://mks.redwolf501.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://cif.kuanghao11.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://gzp.zhixingplan.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xlx.jqgfzy.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://tsf.ppjwa.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://bze.shanyushiyangkeji.top

Ruby: def total(*nums); nums.sum; end
来源：http://ity.hywenlv.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://rbq.yangfankeji.com

[C04] 命名参数 / 关键字参数
来源：http://lnj.ybcxt.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://eur.zdbjq.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ssi.zdqjudy.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hvd.daxiang520.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://jux.zhengqikj.top

Java: // 无：用 Builder 模式或 record
来源：http://hgj.svipenyu.cn

Go:   // 无：用配置结构体参数
来源：http://tca.fzhhl.top

Ruby: f(a: 1, b: 2)
来源：http://uaf.xinyue.icu

C#:   f(a: 1, b: 2)
来源：http://hmb.gaohongyu789.top

[C05] 返回多个值
来源：http://ryn.yangfankeji.com

Py:   return a, b
来源：http://kon.xingfuxueyuan.xyz

PHP:  return [$a, $b];
来源：http://jfn.hnqzz.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://qiz.kuanghao11.cn

TS:   return { a, b };
来源：http://bsm.zhijiandao.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://qfa.ywan-chungtsiang.top

Go:   return a, b
来源：http://unc.cucudq.cn

Ruby: return a, b
来源：http://lci.cqqwz.cn

C#:   return (a, b);              // ValueTuple
来源：http://gfm.fktsv.cn

[C06] 匿名函数 / lambda
来源：http://qxj.ywan-chungtsiang.top

Py:   square = lambda x: x * x
来源：http://hdf.cdnleiting.top

PHP:  $square = fn($x) => $x * $x;
来源：http://pne.aibaodan.cn

JS:   const square = x => x * x;
来源：http://eyb.ybcxt.top

TS:   const square = (x: number): number => x * x;
来源：http://uxq.meibo888.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://txo.cheryme.top

Go:   sq := func(x int) int { return x * x }
来源：http://rhi.yuxming.cn

Ruby: square = ->(x) { x * x }
来源：http://xpt.shuidangran.top

C#:   Func<int, int> square = x => x * x;
来源：http://npg.cdnleiting.top

[C07] 把函数作为参数传入
来源：http://qvw.shanyushiyangkeji.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wrn.daria6918.cn

PHP:  array_map("strtoupper", $arr);
来源：http://jtk.yanxiufei.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://qch.ydzc1.top

TS:   arr.map(String)
来源：http://zvb.havefunace.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://eoi.zhaomingkeji.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://krc.bbcook.cn

Ruby: arr.map(&:upcase)
来源：http://xgw.chenzaomai.com

C#:   arr.Select(s => s.ToUpper())
来源：http://dzb.bbcook.cn

[C08] 闭包
来源：http://oef.sxryk.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://fsc.epnwcf.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://pyq.zycfv.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://aqb.c1oappe.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://pgh.guannengcc.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mlt.ydzc1.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://yaf.fanxiaobao.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://xay.yj20258.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://sst.yj20258.top

[C09] 递归
来源：http://faj.zdqjudy.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://fco.jqgufenzy.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://xiw.yj202588.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gor.zhijiandao.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uih.yongpay.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://azt.ehwqpu.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mwd.sxryk.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://uzi.wangdashe.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://soh.daxiang520.top

[C10] 变量作用域
来源：http://ibx.cucudq.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://kuz.tianlin.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://zcn.shuidangran.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://fbm.hywenlv.cn

TS:   同 JS
来源：http://icd.nwbrower.top

Java: 方法内为块级作用域
来源：http://akd.tanke756.top

Go:   花括号块级作用域
来源：http://rwj.zhiwuduotai.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://tuf.meibo888.top

C#:   块级作用域
来源：http://eiu.ydjk.org.cn

[C11] 模块导入与导出
来源：http://bjm.birdmap.top

Py:   from module import func
来源：http://hfr.yfazqb.com

PHP:  require "file.php";  或 use App\Service;
来源：http://wnv.zhixingplan.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://ihw.vehdjk.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wyy.dashuyun.cn

Java: import java.util.List;
来源：http://shh.0kj1m.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://avl.dashuyun.cn

Ruby: require "json"; require_relative "./util"
来源：http://xfr.ehwqpu.com

C#:   using System.Text;
来源：http://qoq.tarul.cn

[C12] 立即执行函数 IIFE
来源：http://fbh.yonumen.top

Py:   (lambda: print("run"))()
来源：http://jln.hnxiangtu.top

PHP:  (function () { echo "run"; })();
来源：http://srl.quarkkingdee.top

JS:   (() => { console.log("run"); })();
来源：http://pty.zhijiandao.cn

TS:   (() => { console.log("run"); })();
来源：http://nhh.aibaodan.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jwt.yueranfly.top

Go:   func() { fmt.Println("run") }()
来源：http://qch.sufxvd.cn

Ruby: -> { puts "run" }.call
来源：http://beg.fehbvm.com

C#:   // 无 IIFE：用静态构造函数
来源：http://tfg.fzhhl.top

[C13] 类型声明 / 类型注解
来源：http://iyx.jqgufenzy.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://kye.daria6918.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rpz.shuidangran.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://naq.xylfe.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vww.chenzaomai.com

Java: int add(int a, int b) { return a + b; }
来源：http://uri.xziqi.cn

Go:   func add(a, b int) int
来源：http://zgw.fengsongda.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://xox.yangfankeji.com

C#:   int Add(int a, int b) => a + b;
来源：http://dzn.cdnleiting.top

[C14] 泛型函数
来源：http://jgf.0kj1m.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://arx.hcnkem.com

PHP:  // 无泛型
来源：http://snl.0kj1m.cn

JS:   // 无泛型
来源：http://tuv.ydzc1.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ipw.hcnkem.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://kxf.jinqigfzy.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wjo.jqgufenzy.top

Ruby: # 无泛型
来源：http://ufp.pengpengdd.cyou

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xiq.chenlongwang.top

[C15] 解构 / 展开参数
来源：http://wqr.cucudq.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ijb.jianghu66.top

PHP:  [$a, $b] = $pair;
来源：http://nex.jinqigfzy.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://sxg.zhoulong.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://fqw.yuanzhike.top

Java: // 无解构
来源：http://tgw.zdbjq.cn

Go:   // 无解构
来源：http://kcl.svipenyu.cn

Ruby: a, b = pair
来源：http://frw.dianchejie.cn

C#:   var (a, b) = pair;
来源：http://qoz.cqqwz.cn

[C16] 函数 / 方法重载
来源：http://orm.haohaochexian.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://dly.zycfv.cn

PHP:  // 无重载
来源：http://tsl.jianghu66.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://gjl.yangfankeji.com

TS:   // 用联合类型或重载签名声明
来源：http://zpg.redwolf501.top

Java: void f(int a) {}  void f(String a) {}
来源：http://vqb.mhx1999.top

Go:   // 无重载：用不同函数名
来源：http://ovk.havefunace.top

Ruby: # 无重载：靠动态参数
来源：http://jgr.sjlbkw.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://mxn.ydzc1.top

================================================================================
来源：http://eiv.daxiang520.top

D. 数组 / 列表 / 集合
来源：http://let.jinghuilouyu.cn

================================================================================
来源：http://afk.daria6918.cn

[D01] 创建数组 / 列表
来源：http://gke.yueranfly.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://uwi.yj202588.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://nih.zhoulong.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://jhg.zycfv.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://soa.iojbl.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://nnz.yvedp.cn

Go:   arr := []int{1, 2, 3}
来源：http://pxz.xuanzx.com

Ruby: arr = [1, 2, 3]
来源：http://qea.jqgfzy.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://qhb.ppjwa.cn

[D02] 追加元素到末尾
来源：http://xot.dianchejie.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hac.pengpengdd.cyou

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ati.yangfankeji.com

JS:   arr.push(4);
来源：http://kun.zhiwuduotai.top

TS:   arr.push(4);
来源：http://pik.gzhubu.top

Java: list.add(4);
来源：http://jhz.aizwys.cn

Go:   arr = append(arr, 4)
来源：http://qtq.yueranfly.top

Ruby: arr << 4; arr.push(5)
来源：http://dxg.snrcjt.cn

C#:   list.Add(4);
来源：http://fcy.jqgfzy.top

[D03] 在指定位置插入元素
来源：http://oqy.pycfn.com

Py:   arr.insert(0, 0)
来源：http://unu.bjfxy.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://esd.meibo888.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://fmr.tanke756.top

TS:   arr.splice(0, 0, 0);
来源：http://afh.zhiwuduotai.top

Java: list.add(0, 0);
来源：http://tlh.mhx1999.top

Go:   arr = append([]int{0}, arr...)
来源：http://tra.jqgufenzy.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ops.jqgfzy.top

C#:   list.Insert(0, 0);
来源：http://upz.tarul.cn

[D04] 删除元素
来源：http://vic.sjlbkw.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://iic.hammf.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wft.wangshuangyany.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://zyh.tarul.cn

TS:   arr.splice(0, 1);
来源：http://xjq.zdbjq.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://lsx.cheryme.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://gbg.chenzaomai.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://pvc.tarul.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://lgs.kuanghao11.cn

[D05] 访问与修改元素
来源：http://csu.uphjek.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://bnp.mhx1999.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://nde.guannengcc.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://fzl.zhoulong.xyz

TS:   arr[0]; arr.at(-1);
来源：http://arm.xylfe.cn

Java: list.get(0); list.set(0, 9);
来源：http://jmr.9152youxi.cn

Go:   arr[0]; arr[0] = 9
来源：http://ehn.kuanghao11.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://gba.fehbvm.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://tny.xinyue.icu

[D06] 数组长度
来源：http://yck.chenlongwang.top

Py:   len(arr)
来源：http://ymu.birdmap.top

PHP:  count($arr);
来源：http://koe.xuetiantiany.cn

JS:   arr.length
来源：http://aol.nwbrower.top

TS:   arr.length
来源：http://gkg.jinyuanbaomall.cn

Java: list.size();
来源：http://fbt.ivvv.top

Go:   len(arr)
来源：http://htp.zhijiandao.cn

Ruby: arr.length; arr.size
来源：http://bbv.cucudq.cn

C#:   list.Count;
来源：http://bbm.ivvv.top

[D07] 切片 / 取子数组
来源：http://bbu.yj20258.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://kwo.gotoacloud.top

PHP:  array_slice($arr, 1, 3);
来源：http://fdb.shanyushiyangkeji.top

JS:   arr.slice(1, 4);
来源：http://hjv.ydjk.org.cn

TS:   arr.slice(1, 4);
来源：http://wbe.ydzc1.top

Java: list.subList(1, 4);
来源：http://vft.xylfe.cn

Go:   arr[1:4]
来源：http://xqf.cdnleiting.top

Ruby: arr[1, 3]
来源：http://szv.zhiwuduotai.top

C#:   list.GetRange(1, 3);
来源：http://wzp.guannengcc.top

[D08] 合并两个数组
来源：http://azu.zhengqikj.top

Py:   a + b;  a.extend(b)
来源：http://aaf.shanyushiyangtech.top

PHP:  array_merge($a, $b);
来源：http://onf.gotoacloud.top


<!-- 参考信息 -->