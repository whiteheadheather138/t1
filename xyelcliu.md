代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://hiy.daxiang520.top

PHP:  do { $i++; } while ($i < 10);
来源：http://hzj.sjlbkw.cn

JS:   do { i++; } while (i < 10);
来源：http://zvb.shanyushiyangtech.top

TS:   do { i++; } while (i < 10);
来源：http://sqb.0kj1m.cn

Java: do { i++; } while (i < 10);
来源：http://pdi.ydjk.org.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://cua.guannengcc.top

Ruby: begin; i += 1; end while i < 10
来源：http://xzi.daxiang520.top

C#:   do { i++; } while (i < 10);
来源：http://vvq.bbcook.cn

[B09] break 与 continue
来源：http://fgf.sufxvd.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://axw.xinyue.icu

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ddb.zhixingplan.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bfc.chenlongwang.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vpz.daxiang520.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fwi.xziqi.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://eph.jiagoushi.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://kbu.ydzc1.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://don.chenzaomai.com

[B10] 遍历同时拿索引
来源：http://flm.zdbjq.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://fsr.zhixingplan.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://tii.svipenyu.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xfc.0kj1m.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://guw.jianghu66.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://xrq.tanke756.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://vpk.shanyushiyangtech.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wmt.jinyuanbaomall.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://sga.yj20258888.top

[B11] 生成数字序列 / 区间
来源：http://vyh.ydzc1.top

Py:   list(range(0, 10, 2))
来源：http://hdp.dashuyun.cn

PHP:  range(0, 10, 2);
来源：http://prc.meibo888.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gqd.dashuyun.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://igt.zdbjq.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://drs.sxryk.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://qai.yuxming.cn

Ruby: (0...10).step(2).to_a
来源：http://aea.yvedp.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://yzl.sjlbkw.cn

[B12] 跳出多层循环
来源：http://jqs.xuetiantiany.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://bup.c1oappe.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://qjy.guowangkeji.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://gug.hnqzz.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mes.zhixingplan.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mrr.sxryk.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wtn.wangdashe.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://oru.bbcook.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://tze.316326.xyz

[B13] 判断是否为数字
来源：http://bwj.epnwcf.com

Py:   isinstance(x, (int, float))
来源：http://iza.hcnkem.com

PHP:  is_numeric($x)
来源：http://ibj.cdnleiting.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tik.zhongyouzk.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qql.birdmap.top

Java: x instanceof Number
来源：http://wqo.chenlongwang.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://qqy.shangyingyoupin.top

Ruby: x.is_a?(Numeric)
来源：http://hss.fzhhl.top

C#:   x is int or double or decimal
来源：http://kky.haohaochexian.top

[B14] 判断值是否在集合内
来源：http://hrk.gzhubu.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://say.0kj1m.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://sep.fzhhl.top

JS:   [1, 2, 3].includes(x)
来源：http://fem.hammf.cn

TS:   [1, 2, 3].includes(x)
来源：http://kkh.hammf.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://hgt.feifeiyinyue.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ygb.haohaochexian.top

Ruby: [1, 2, 3].include?(x)
来源：http://aqm.shuidangran.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ebz.yj20258888.top

[B15] 布尔运算与取反
来源：http://emb.haohaochexian.top

Py:   a and b or not c
来源：http://hoz.shanyushiyangtech.top

PHP:  $a && $b || !$c
来源：http://cio.zdqjudy.top

JS:   a && b || !c
来源：http://ojj.xziqi.cn

TS:   a && b || !c
来源：http://yrn.tanke756.top

Java: a && b || !c
来源：http://wou.yuxming.cn

Go:   a && b || !c
来源：http://yhr.hfpthk.cn

Ruby: a && b || !c
来源：http://pbk.jinqigufen.top

C#:   a && b || !c
来源：http://rjc.zycfv.cn

[B16] 卫语句：不满足条件提前返回
来源：http://til.shangyingyoupin.top

Py:   if not data: return
来源：http://hdk.dianchejie.cn

PHP:  if (!$data) { return; }
来源：http://cgg.jianghu66.top

JS:   if (!data) return;
来源：http://lwb.jinqigufen.top

TS:   if (!data) return;
来源：http://bfu.tianlin.xyz

Java: if (data == null) return;
来源：http://zpw.ydzc1.top

Go:   if data == nil { return }
来源：http://zvs.shzxlz.cn

Ruby: return if data.nil?
来源：http://ehy.ydjk.org.cn

C#:   if (data == null) return;
来源：http://ebg.yfazqb.com

================================================================================
来源：http://yee.zdqjudy.top

C. 函数与作用域
来源：http://hfd.shangyingyoupin.top

================================================================================
来源：http://rvo.jqgfzy.top

[C01] 定义函数
来源：http://upn.0kj1m.cn

Py:   def add(a, b): return a + b
来源：http://gux.sufxvd.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hul.xylfe.cn

JS:   function add(a, b) { return a + b; }
来源：http://jtx.cucudq.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gge.yuanzhike.top

Java: static int add(int a, int b) { return a + b; }
来源：http://xgy.fzhhl.top

Go:   func add(a, b int) int { return a + b }
来源：http://llw.zdqjudy.top

Ruby: def add(a, b); a + b; end
来源：http://gyz.yfazqb.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ivu.pengpengdd.cyou

[C02] 默认参数
来源：http://mmx.yuanzhike.top

Py:   def greet(name="World"): return name
来源：http://asg.fehbvm.com

PHP:  function greet($name = "World") { return $name; }
来源：http://ime.uphjek.com

JS:   function greet(name = "World") { return name; }
来源：http://cuj.cqqwz.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://xvj.cqqwz.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://sdp.bjfxy.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://eil.andypj.xyz

Ruby: def greet(name = "World") = name
来源：http://ucq.jlsjyb.cn

C#:   string Greet(string name = "World") => name;
来源：http://fwh.52xcode.cn

[C03] 可变参数
来源：http://zbf.tarul.cn

Py:   def total(*args): return sum(args)
来源：http://eya.bbcook.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://zaf.hfpthk.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://epz.zhaomingkeji.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://rmi.zdbjq.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ygw.guannengcc.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://aow.wangdashe.top

Ruby: def total(*nums); nums.sum; end
来源：http://nmk.yj20258.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hdg.andypj.xyz

[C04] 命名参数 / 关键字参数
来源：http://zjj.jyoumei.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://neu.52xcode.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://oia.hnqzz.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://pxl.jiagoushi.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xef.cqqwz.cn

Java: // 无：用 Builder 模式或 record
来源：http://wwq.yuanzhike.top

Go:   // 无：用配置结构体参数
来源：http://cvt.dianchejie.cn

Ruby: f(a: 1, b: 2)
来源：http://vno.gogol.net.cn

C#:   f(a: 1, b: 2)
来源：http://gzd.tian-w.cn

[C05] 返回多个值
来源：http://azc.wangshuangyany.cn

Py:   return a, b
来源：http://lxb.jyoumei.cn

PHP:  return [$a, $b];
来源：http://whn.jiagoushi.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://djt.yuanzhike.top

TS:   return { a, b };
来源：http://xle.smart0.xyz

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://knw.ehwqpu.com

Go:   return a, b
来源：http://gcv.sysykeji.top

Ruby: return a, b
来源：http://glf.aizwys.cn

C#:   return (a, b);              // ValueTuple
来源：http://xap.ydzc1.top

[C06] 匿名函数 / lambda
来源：http://jnd.zycfv.cn

Py:   square = lambda x: x * x
来源：http://pqr.cqqwz.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://vlj.havefunace.top

JS:   const square = x => x * x;
来源：http://cjt.zhiwuduotai.top

TS:   const square = (x: number): number => x * x;
来源：http://efw.cqqwz.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ufk.cucudq.cn

Go:   sq := func(x int) int { return x * x }
来源：http://fga.hammf.cn

Ruby: square = ->(x) { x * x }
来源：http://stj.pycfn.com

C#:   Func<int, int> square = x => x * x;
来源：http://ssr.iojbl.cn

[C07] 把函数作为参数传入
来源：http://ikq.sysykeji.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://owd.ydzc1.top

PHP:  array_map("strtoupper", $arr);
来源：http://qnx.gaohongyu789.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mrf.andypj.xyz

TS:   arr.map(String)
来源：http://edi.jianghu66.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://qsz.smart0.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://amb.hcnkem.com

Ruby: arr.map(&:upcase)
来源：http://qag.cqqwz.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://epr.tian-w.cn

[C08] 闭包
来源：http://nzg.yueranfly.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://pvx.shzxlz.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://jmg.quarkkingdee.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wpp.wangdashe.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mng.epnwcf.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://cau.tarul.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://obi.ydzc1.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://zlx.havefunace.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://iri.yangfankeji.com

[C09] 递归
来源：http://mmd.vqdsnc.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qxh.tarul.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://sys.fzhhl.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mdj.cucudq.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jjb.ywan-chungtsiang.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://kpt.yj20258.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://qvm.xylfe.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://dbo.c1oappe.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://tjx.shangyingyoupin.top

[C10] 变量作用域
来源：http://shu.zhongyouzk.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://vrt.fzhhl.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://oyf.dianchejie.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://izp.jinyuanbaomall.cn

TS:   同 JS
来源：http://iai.sxryk.cn

Java: 方法内为块级作用域
来源：http://sjf.xuanzx.com

Go:   花括号块级作用域
来源：http://kgx.dashuyun.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://acs.sysykeji.top

C#:   块级作用域
来源：http://qqc.yonumen.top

[C11] 模块导入与导出
来源：http://wfn.xylfe.cn

Py:   from module import func
来源：http://qfm.wangdashe.top

PHP:  require "file.php";  或 use App\Service;
来源：http://jeq.52xcode.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://wss.shanyushiyangkeji.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://yny.vqdsnc.cn

Java: import java.util.List;
来源：http://cbq.jinqigfzy.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://txg.ivvv.top

Ruby: require "json"; require_relative "./util"
来源：http://baj.fzhhl.top

C#:   using System.Text;
来源：http://sro.daxiang520.top

[C12] 立即执行函数 IIFE
来源：http://ixp.guowangkeji.top

Py:   (lambda: print("run"))()
来源：http://rhr.xingfuxueyuan.xyz

PHP:  (function () { echo "run"; })();
来源：http://jyj.fengsongda.top

JS:   (() => { console.log("run"); })();
来源：http://sgp.xylfe.cn

TS:   (() => { console.log("run"); })();
来源：http://zea.guannengcc.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jbi.yongpay.top

Go:   func() { fmt.Println("run") }()
来源：http://afw.jinghuilouyu.cn

Ruby: -> { puts "run" }.call
来源：http://maf.shanyushiyangtech.top

C#:   // 无 IIFE：用静态构造函数
来源：http://hhm.chenlongwang.top

[C13] 类型声明 / 类型注解
来源：http://wqj.nanxuanxn.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://tgx.hfpthk.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hly.shzxlz.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ajq.fktsv.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tmy.vehdjk.com

Java: int add(int a, int b) { return a + b; }
来源：http://nvk.hammf.cn

Go:   func add(a, b int) int
来源：http://hni.jyoumei.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://eqv.birdmap.top

C#:   int Add(int a, int b) => a + b;
来源：http://tlk.xinyue.icu

[C14] 泛型函数
来源：http://prp.ydzc1.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zdd.yuanzhike.top

PHP:  // 无泛型
来源：http://nwi.shanyushiyangtech.top

JS:   // 无泛型
来源：http://sfb.bbcook.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://zzr.zhaomingkeji.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://lae.gotoacloud.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://vgk.yueranfly.top

Ruby: # 无泛型
来源：http://oib.tian-w.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xct.dianchejie.cn

[C15] 解构 / 展开参数
来源：http://fmq.cqqwz.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xiv.fanxiaobao.xyz

PHP:  [$a, $b] = $pair;
来源：http://nok.yj20258.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://pre.dianchejie.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://gjv.jqgufenzy.top

Java: // 无解构
来源：http://hdr.xziqi.cn

Go:   // 无解构
来源：http://faz.xingfuxueyuan.xyz

Ruby: a, b = pair
来源：http://yqd.chenlongwang.top

C#:   var (a, b) = pair;
来源：http://ygt.fzhhl.top

[C16] 函数 / 方法重载
来源：http://tpc.jinghuilouyu.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://byn.tanke756.top

PHP:  // 无重载
来源：http://kow.havefunace.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://ndw.zhengqikj.top

TS:   // 用联合类型或重载签名声明
来源：http://zyz.kuanghao11.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://xjx.dianchejie.cn

Go:   // 无重载：用不同函数名
来源：http://ekh.fzhhl.top

Ruby: # 无重载：靠动态参数
来源：http://nee.ydzc1.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://qsf.ivvv.top

================================================================================
来源：http://lfr.fktsv.cn

D. 数组 / 列表 / 集合
来源：http://axn.cheryme.top

================================================================================
来源：http://fqv.cdnleiting.top

[D01] 创建数组 / 列表
来源：http://loe.vqdsnc.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://zvb.cashguo.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://scy.c1oappe.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://nqi.fehbvm.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://kyj.tianlin.xyz

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://col.cashguo.top

Go:   arr := []int{1, 2, 3}
来源：http://ikd.aibaodan.cn

Ruby: arr = [1, 2, 3]
来源：http://qkz.zdbjq.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://uky.316326.xyz

[D02] 追加元素到末尾
来源：http://aia.tarul.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mig.haohaochexian.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ssx.bjfxy.top

JS:   arr.push(4);
来源：http://gqi.redwolf501.top

TS:   arr.push(4);
来源：http://pyb.nanxuanxn.top

Java: list.add(4);
来源：http://eoc.9152youxi.cn

Go:   arr = append(arr, 4)
来源：http://ejo.hcnkem.com

Ruby: arr << 4; arr.push(5)
来源：http://guf.redwolf501.top

C#:   list.Add(4);
来源：http://emo.nanxuanxn.top

[D03] 在指定位置插入元素
来源：http://hli.nanxinkj.top

Py:   arr.insert(0, 0)
来源：http://drn.vqdsnc.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://uth.chenlongwang.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://tlt.chenzaomai.com

TS:   arr.splice(0, 0, 0);
来源：http://hij.wangshuangyany.cn

Java: list.add(0, 0);
来源：http://rwv.ivvv.top

Go:   arr = append([]int{0}, arr...)
来源：http://bkm.meibo888.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ivy.jqgufenzy.top

C#:   list.Insert(0, 0);
来源：http://rom.yonumen.top

[D04] 删除元素
来源：http://tfd.guannengcc.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://qxc.aizwys.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://trj.xylfe.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://zll.jinghuilouyu.cn

TS:   arr.splice(0, 1);
来源：http://wxu.sufxvd.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://aes.jinyuanbaomall.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://pud.0kj1m.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://rly.wangdashe.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ssd.yanxiufei.cn

[D05] 访问与修改元素
来源：http://biz.xziqi.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://pxv.daria6918.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ooe.xziqi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://btp.jianghu66.top

TS:   arr[0]; arr.at(-1);
来源：http://pds.ybcxt.top

Java: list.get(0); list.set(0, 9);
来源：http://yra.aizwys.cn

Go:   arr[0]; arr[0] = 9
来源：http://ubq.daxiang520.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://iwb.bjfxy.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ydk.xuanzx.com

[D06] 数组长度
来源：http://gpw.nanxinkj.top

Py:   len(arr)
来源：http://otg.yueranfly.top

PHP:  count($arr);
来源：http://oul.yj202588.top

JS:   arr.length
来源：http://wta.tian-w.cn

TS:   arr.length
来源：http://ogo.cqqwz.cn

Java: list.size();
来源：http://icq.hysaishi.cn

Go:   len(arr)
来源：http://vli.nanxinkj.top

Ruby: arr.length; arr.size
来源：http://xwo.jinqigfzy.top

C#:   list.Count;
来源：http://med.yj20258.top

[D07] 切片 / 取子数组
来源：http://zqp.yangfankeji.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wwo.ehwqpu.com

PHP:  array_slice($arr, 1, 3);
来源：http://cfg.yangfankeji.com

JS:   arr.slice(1, 4);
来源：http://xql.bjfxy.top

TS:   arr.slice(1, 4);
来源：http://xud.aizwys.cn

Java: list.subList(1, 4);
来源：http://acj.cashguo.top

Go:   arr[1:4]
来源：http://xut.yvedp.cn

Ruby: arr[1, 3]
来源：http://uwv.daxiang520.top

C#:   list.GetRange(1, 3);
来源：http://yyi.yanxiufei.cn

[D08] 合并两个数组
来源：http://col.vqdsnc.cn

Py:   a + b;  a.extend(b)
来源：http://ztf.dashuyun.cn

PHP:  array_merge($a, $b);
来源：http://xhh.zhengqikj.top

JS:   [...a, ...b];  a.concat(b);
来源：http://jrf.yangfankeji.com

TS:   [...a, ...b];
来源：http://hgz.bjfxy.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://nqx.yuanzhike.top

Go:   append(a, b...)
来源：http://orh.fanxiaobao.xyz


<!-- 参考信息 -->