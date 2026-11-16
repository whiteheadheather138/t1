代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://xob.ppjwa.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://pur.meibo888.top

JS:   do { i++; } while (i < 10);
来源：http://cmw.mhx1999.top

TS:   do { i++; } while (i < 10);
来源：http://pke.fzhhl.top

Java: do { i++; } while (i < 10);
来源：http://qnb.wangdashe.top

Go:   for { i++; if i >= 10 { break } }
来源：http://kwe.hammf.cn

Ruby: begin; i += 1; end while i < 10
来源：http://zww.yuxming.cn

C#:   do { i++; } while (i < 10);
来源：http://mgv.hysaishi.cn

[B09] break 与 continue
来源：http://vxu.kuanghao11.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wgz.gogol.net.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://sut.havefunace.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blg.cdnleiting.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://szq.shanyushiyangtech.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wys.hywenlv.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ecg.smart0.xyz

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ers.fehbvm.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ezb.hcnkem.com

[B10] 遍历同时拿索引
来源：http://rla.fktsv.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://epg.chenlongwang.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hfu.hesvh.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://tgo.gogol.net.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://jrk.xingfuxueyuan.xyz

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ikb.jyoumei.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://bea.wangshuangyany.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://alj.quarkkingdee.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hxj.shangyingyoupin.top

[B11] 生成数字序列 / 区间
来源：http://lwy.quarkkingdee.top

Py:   list(range(0, 10, 2))
来源：http://fws.tanke756.top

PHP:  range(0, 10, 2);
来源：http://vdi.yj20258888.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ncr.bjfxy.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tiw.chenlongwang.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hdf.uphjek.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hnh.cheryme.top

Ruby: (0...10).step(2).to_a
来源：http://lvy.yanxiufei.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://jpa.shanyushiyangkeji.top

[B12] 跳出多层循环
来源：http://oau.yfazqb.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://cmo.haohaochexian.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://pae.pengpengdd.cyou

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://lfc.kuanghao11.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://zyv.smart0.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hln.jianghu66.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wev.zhaomingkeji.xyz

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://pdy.yj202588.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wlz.hysaishi.cn

[B13] 判断是否为数字
来源：http://bnh.jinqigfzy.top

Py:   isinstance(x, (int, float))
来源：http://yjm.tian-w.cn

PHP:  is_numeric($x)
来源：http://wvd.aibaodan.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jfc.jqgufenzy.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ids.zycfv.cn

Java: x instanceof Number
来源：http://oqy.nanxuanxn.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://iex.fktsv.cn

Ruby: x.is_a?(Numeric)
来源：http://ggc.svipenyu.cn

C#:   x is int or double or decimal
来源：http://xlu.hnqzz.top

[B14] 判断值是否在集合内
来源：http://uto.shuidangran.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://eul.0kj1m.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://woo.xuanzx.com

JS:   [1, 2, 3].includes(x)
来源：http://rby.shzxlz.cn

TS:   [1, 2, 3].includes(x)
来源：http://obo.daxiang520.top

Java: List.of(1, 2, 3).contains(x)
来源：http://uor.smart0.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://jcw.hnxiangtu.top

Ruby: [1, 2, 3].include?(x)
来源：http://cxv.svipenyu.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ixo.vqdsnc.cn

[B15] 布尔运算与取反
来源：http://mmt.sjlbkw.cn

Py:   a and b or not c
来源：http://qcp.c1oappe.top

PHP:  $a && $b || !$c
来源：http://fkq.zhengqikj.top

JS:   a && b || !c
来源：http://hlp.guowangkeji.top

TS:   a && b || !c
来源：http://zhw.ydzc1.top

Java: a && b || !c
来源：http://olq.nwbrower.top

Go:   a && b || !c
来源：http://ifn.wangshuangyany.cn

Ruby: a && b || !c
来源：http://ubv.hnqzz.top

C#:   a && b || !c
来源：http://ndt.yvedp.cn

[B16] 卫语句：不满足条件提前返回
来源：http://cxn.tarul.cn

Py:   if not data: return
来源：http://tex.jinqigufen.top

PHP:  if (!$data) { return; }
来源：http://wvk.uphjek.com

JS:   if (!data) return;
来源：http://boa.ydzc1.top

TS:   if (!data) return;
来源：http://crl.xinyue.icu

Java: if (data == null) return;
来源：http://zlf.xylfe.cn

Go:   if data == nil { return }
来源：http://fla.cdnleiting.top

Ruby: return if data.nil?
来源：http://urc.fengsongda.top

C#:   if (data == null) return;
来源：http://fqx.xziqi.cn

================================================================================
来源：http://obl.gogol.net.cn

C. 函数与作用域
来源：http://qgh.fehbvm.com

================================================================================
来源：http://rfk.ehwqpu.com

[C01] 定义函数
来源：http://lmz.ivvv.top

Py:   def add(a, b): return a + b
来源：http://vhq.hongshengwenyu.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://auu.andypj.xyz

JS:   function add(a, b) { return a + b; }
来源：http://agx.hnxiangtu.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lic.zhijiandao.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://hlg.yvedp.cn

Go:   func add(a, b int) int { return a + b }
来源：http://vsl.zhixingplan.top

Ruby: def add(a, b); a + b; end
来源：http://phe.gaohongyu789.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ahl.cucudq.cn

[C02] 默认参数
来源：http://tll.hongshengwenyu.top

Py:   def greet(name="World"): return name
来源：http://rej.pengpengdd.cyou

PHP:  function greet($name = "World") { return $name; }
来源：http://bsv.uphjek.com

JS:   function greet(name = "World") { return name; }
来源：http://qwc.shangyingyoupin.top

TS:   function greet(name: string = "World") { return name; }
来源：http://auq.xuanzx.com

Java: // 无默认参数：方法重载或 Optional
来源：http://iqe.yongpay.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://xde.hcnkem.com

Ruby: def greet(name = "World") = name
来源：http://ybo.yangfankeji.com

C#:   string Greet(string name = "World") => name;
来源：http://deu.hnxiangtu.top

[C03] 可变参数
来源：http://cys.tanke756.top

Py:   def total(*args): return sum(args)
来源：http://ylk.cqqwz.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://kpy.pycfn.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://vce.fzhhl.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://vdf.fehbvm.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://zxk.shzxlz.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ddz.yuanzhike.top

Ruby: def total(*nums); nums.sum; end
来源：http://cjh.tian-w.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://qdm.fengsongda.top

[C04] 命名参数 / 关键字参数
来源：http://kfx.fktsv.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://oqw.yuxming.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://nrr.fehbvm.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://fti.quarkkingdee.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mxc.hammf.cn

Java: // 无：用 Builder 模式或 record
来源：http://cld.yonumen.top

Go:   // 无：用配置结构体参数
来源：http://oam.xziqi.cn

Ruby: f(a: 1, b: 2)
来源：http://baa.c1oappe.top

C#:   f(a: 1, b: 2)
来源：http://qib.xuanzx.com

[C05] 返回多个值
来源：http://ted.jqgfzy.top

Py:   return a, b
来源：http://tzj.chenlongwang.top

PHP:  return [$a, $b];
来源：http://pci.hammf.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://guw.zhongyouzk.top

TS:   return { a, b };
来源：http://nty.jqgufenzy.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wtm.yj20258.top

Go:   return a, b
来源：http://gan.0kj1m.cn

Ruby: return a, b
来源：http://zmc.hywenlv.cn

C#:   return (a, b);              // ValueTuple
来源：http://ahm.daria6918.cn

[C06] 匿名函数 / lambda
来源：http://lyv.hysaishi.cn

Py:   square = lambda x: x * x
来源：http://qcr.yfazqb.com

PHP:  $square = fn($x) => $x * $x;
来源：http://bup.hammf.cn

JS:   const square = x => x * x;
来源：http://oze.gotoacloud.top

TS:   const square = (x: number): number => x * x;
来源：http://gzb.jinyuanbaomall.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hzt.hysaishi.cn

Go:   sq := func(x int) int { return x * x }
来源：http://oot.xylfe.cn

Ruby: square = ->(x) { x * x }
来源：http://kla.c1oappe.top

C#:   Func<int, int> square = x => x * x;
来源：http://xay.ctjpmb.com

[C07] 把函数作为参数传入
来源：http://zif.hnxiangtu.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://sfy.cucudq.cn

PHP:  array_map("strtoupper", $arr);
来源：http://hyc.zhengqikj.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://qph.ctjpmb.com

TS:   arr.map(String)
来源：http://qtc.jinyuanbaomall.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://vfk.0kj1m.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://jes.cashguo.top

Ruby: arr.map(&:upcase)
来源：http://enc.xingfuxueyuan.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://vfz.hysaishi.cn

[C08] 闭包
来源：http://zls.fzhhl.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://xdc.iojbl.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://lzc.jlsjyb.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://clt.haohaochexian.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://cvb.tian-w.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://omd.cashguo.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jmb.zhengqikj.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ojx.zdqjudy.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://pdq.bbcook.cn

[C09] 递归
来源：http://cei.9152youxi.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hfd.zhengqikj.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://jlk.cucudq.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zxy.wangshuangyany.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://osh.sxryk.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://cdo.sjlbkw.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://nmf.pycfn.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://fvu.cqqwz.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://tso.0kj1m.cn

[C10] 变量作用域
来源：http://fok.sysykeji.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hlx.aibaodan.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://nxi.zycfv.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://syf.dashuyun.cn

TS:   同 JS
来源：http://qng.epnwcf.com

Java: 方法内为块级作用域
来源：http://udb.yonumen.top

Go:   花括号块级作用域
来源：http://ndf.52xcode.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://svh.zhaomingkeji.xyz

C#:   块级作用域
来源：http://sye.yvedp.cn

[C11] 模块导入与导出
来源：http://fpu.vqdsnc.cn

Py:   from module import func
来源：http://zjz.daria6918.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://wno.yongpay.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://svj.ppjwa.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://vfx.jqgfzy.top

Java: import java.util.List;
来源：http://ant.sjlbkw.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hjv.haohaochexian.top

Ruby: require "json"; require_relative "./util"
来源：http://ndd.daria6918.cn

C#:   using System.Text;
来源：http://gmh.feifeiyinyue.top

[C12] 立即执行函数 IIFE
来源：http://xjc.tanke756.top

Py:   (lambda: print("run"))()
来源：http://mpx.yuxming.cn

PHP:  (function () { echo "run"; })();
来源：http://ltq.haohaochexian.top

JS:   (() => { console.log("run"); })();
来源：http://ngv.uphjek.com

TS:   (() => { console.log("run"); })();
来源：http://coi.yuanzhike.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wvb.gzhubu.top

Go:   func() { fmt.Println("run") }()
来源：http://xzl.gotoacloud.top

Ruby: -> { puts "run" }.call
来源：http://jvu.xziqi.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://uxp.pengpengdd.cyou

[C13] 类型声明 / 类型注解
来源：http://tpk.fktsv.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://bmw.xuetiantiany.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ouk.havefunace.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://izr.mhx1999.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yfh.chenzaomai.com

Java: int add(int a, int b) { return a + b; }
来源：http://hit.9152youxi.cn

Go:   func add(a, b int) int
来源：http://ivm.yj202588.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://gzl.fehbvm.com

C#:   int Add(int a, int b) => a + b;
来源：http://zxu.jqgufenzy.top

[C14] 泛型函数
来源：http://qhc.bbcook.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://bxv.hywenlv.cn

PHP:  // 无泛型
来源：http://yfy.ywan-chungtsiang.top

JS:   // 无泛型
来源：http://tna.svipenyu.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://dxg.tanke756.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://xfd.shuidangran.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://huo.xziqi.cn

Ruby: # 无泛型
来源：http://vnk.hammf.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://bbt.sweek.top

[C15] 解构 / 展开参数
来源：http://gpv.bbcook.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://pgm.gotoacloud.top

PHP:  [$a, $b] = $pair;
来源：http://owt.hongshengwenyu.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://vyi.ydjk.org.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://kvq.jiagoushi.top

Java: // 无解构
来源：http://crj.yj20258.top

Go:   // 无解构
来源：http://pqh.ppjwa.cn

Ruby: a, b = pair
来源：http://ndv.gzhubu.top

C#:   var (a, b) = pair;
来源：http://gnx.jinqigufen.top

[C16] 函数 / 方法重载
来源：http://gys.yueranfly.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://jps.gotoacloud.top

PHP:  // 无重载
来源：http://vjb.xinyue.icu

JS:   // 无重载：靠 arguments.length 分支
来源：http://aso.shanyushiyangkeji.top

TS:   // 用联合类型或重载签名声明
来源：http://jdi.feifeiyinyue.top

Java: void f(int a) {}  void f(String a) {}
来源：http://vam.chenzaomai.com

Go:   // 无重载：用不同函数名
来源：http://onl.shzxlz.cn

Ruby: # 无重载：靠动态参数
来源：http://noc.hfpthk.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://yqd.fktsv.cn

================================================================================
来源：http://dvy.jianghu66.top

D. 数组 / 列表 / 集合
来源：http://ppy.iojbl.cn

================================================================================
来源：http://nzj.jqgufenzy.top

[D01] 创建数组 / 列表
来源：http://qdz.jiagoushi.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://ixd.feifeiyinyue.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ibh.hammf.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://rpr.hysaishi.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://vcm.guannengcc.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://opx.cashguo.top

Go:   arr := []int{1, 2, 3}
来源：http://tci.nanxuanxn.top

Ruby: arr = [1, 2, 3]
来源：http://tsq.xinyue.icu

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://typ.zhixingplan.top

[D02] 追加元素到末尾
来源：http://eut.jyoumei.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://noj.chenzaomai.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://twa.sxryk.cn

JS:   arr.push(4);
来源：http://haa.yvedp.cn

TS:   arr.push(4);
来源：http://zme.jlsjyb.cn

Java: list.add(4);
来源：http://lut.cashguo.top

Go:   arr = append(arr, 4)
来源：http://elz.pengpengdd.cyou

Ruby: arr << 4; arr.push(5)
来源：http://xfv.zdbjq.cn

C#:   list.Add(4);
来源：http://uww.sufxvd.cn

[D03] 在指定位置插入元素
来源：http://kan.nanxinkj.top

Py:   arr.insert(0, 0)
来源：http://ahz.sjlbkw.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://byb.fengsongda.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://czb.hesvh.cn

TS:   arr.splice(0, 0, 0);
来源：http://eyp.zdbjq.cn

Java: list.add(0, 0);
来源：http://hix.jinqigfzy.top

Go:   arr = append([]int{0}, arr...)
来源：http://ruv.yongpay.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://buj.jlsjyb.cn

C#:   list.Insert(0, 0);
来源：http://iie.shzxlz.cn

[D04] 删除元素
来源：http://gek.yongpay.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ukj.mhx1999.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://gjh.fzhhl.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://jtx.zhiwuduotai.top

TS:   arr.splice(0, 1);
来源：http://kgw.tanke756.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://xym.gaohongyu789.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://joa.ydzc1.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://bjf.jqgufenzy.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://qpv.gotoacloud.top

[D05] 访问与修改元素
来源：http://ovm.zhengqikj.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://pig.0kj1m.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://pgv.hcnkem.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://yzf.yj202588.top

TS:   arr[0]; arr.at(-1);
来源：http://pyx.guowangkeji.top

Java: list.get(0); list.set(0, 9);
来源：http://mob.ywan-chungtsiang.top

Go:   arr[0]; arr[0] = 9
来源：http://pps.xylfe.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://lum.jinqigfzy.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://exi.tian-w.cn

[D06] 数组长度
来源：http://rcy.yj202588.top

Py:   len(arr)
来源：http://vuq.gzhubu.top

PHP:  count($arr);
来源：http://waw.jqgufenzy.top

JS:   arr.length
来源：http://vak.cqqwz.cn

TS:   arr.length
来源：http://qpd.yangfankeji.com

Java: list.size();
来源：http://zub.epnwcf.com

Go:   len(arr)
来源：http://bvd.shangyingyoupin.top

Ruby: arr.length; arr.size
来源：http://aib.cucudq.cn

C#:   list.Count;
来源：http://roq.dashuyun.cn

[D07] 切片 / 取子数组
来源：http://iaj.xingfuxueyuan.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://jzo.aibaodan.cn

PHP:  array_slice($arr, 1, 3);
来源：http://xvb.gzhubu.top

JS:   arr.slice(1, 4);
来源：http://qgl.316326.xyz

TS:   arr.slice(1, 4);
来源：http://jdc.sjlbkw.cn

Java: list.subList(1, 4);
来源：http://ppm.jinghuilouyu.cn

Go:   arr[1:4]
来源：http://moq.vehdjk.com

Ruby: arr[1, 3]
来源：http://gpj.meibo888.top

C#:   list.GetRange(1, 3);
来源：http://wim.yangfankeji.com

[D08] 合并两个数组
来源：http://tra.bjfxy.top

Py:   a + b;  a.extend(b)
来源：http://lkb.guannengcc.top

PHP:  array_merge($a, $b);
来源：http://iro.fengsongda.top

JS:   [...a, ...b];  a.concat(b);
来源：http://qvo.zdbjq.cn

TS:   [...a, ...b];
来源：http://ofv.guowangkeji.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://aal.yj20258.top

Go:   append(a, b...)
来源：http://nes.zhaomingkeji.xyz


<!-- 参考信息 -->