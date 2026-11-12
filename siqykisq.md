代发 wailian999

[B09] break 与 continue
来源：http://tjr.hysaishi.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://kpp.fzhhl.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://yrw.ppjwa.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://poc.nanxuanxn.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://aqh.shanyushiyangtech.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tit.bjfxy.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://pia.jinghuilouyu.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ksz.cashguo.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ngo.uphjek.com

[B10] 遍历同时拿索引
来源：http://thz.hongshengwenyu.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ntm.bjfxy.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://xaw.jyoumei.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://lpf.hongshengwenyu.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://tja.xziqi.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://etp.yonumen.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://klk.zhoulong.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ppb.gzhubu.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://vse.jlsjyb.cn

[B11] 生成数字序列 / 区间
来源：http://hjj.yj20258.top

Py:   list(range(0, 10, 2))
来源：http://stw.xziqi.cn

PHP:  range(0, 10, 2);
来源：http://ezr.cucudq.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://azd.jqgufenzy.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wzm.yonumen.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://aex.hysaishi.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ham.xuetiantiany.cn

Ruby: (0...10).step(2).to_a
来源：http://nhl.meibo888.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://jpd.tian-w.cn

[B12] 跳出多层循环
来源：http://kmz.pengpengdd.cyou

Py:   # 无标签跳转：抽成函数用 return
来源：http://kyg.daria6918.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://nyj.andypj.xyz

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://zmm.wangdashe.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://gkp.pengpengdd.cyou

Java: outer: for (...) { for (...) { break outer; } }
来源：http://gmi.nanxuanxn.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://qbn.yj202588.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://cxn.52xcode.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://zzw.cqqwz.cn

[B13] 判断是否为数字
来源：http://uyd.tian-w.cn

Py:   isinstance(x, (int, float))
来源：http://frc.ctjpmb.com

PHP:  is_numeric($x)
来源：http://wil.0kj1m.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xjb.andypj.xyz

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ksq.jinghuilouyu.cn

Java: x instanceof Number
来源：http://jds.yvedp.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://uij.52xcode.cn

Ruby: x.is_a?(Numeric)
来源：http://zin.fzhhl.top

C#:   x is int or double or decimal
来源：http://gri.xingfuxueyuan.xyz

[B14] 判断值是否在集合内
来源：http://gqd.jinyuanbaomall.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://fsp.ivvv.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://jgz.haohaochexian.top

JS:   [1, 2, 3].includes(x)
来源：http://omp.smart0.xyz

TS:   [1, 2, 3].includes(x)
来源：http://qso.epnwcf.com

Java: List.of(1, 2, 3).contains(x)
来源：http://pml.cucudq.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://xvv.daxiang520.top

Ruby: [1, 2, 3].include?(x)
来源：http://csc.52xcode.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://zps.epnwcf.com

[B15] 布尔运算与取反
来源：http://aro.yj20258.top

Py:   a and b or not c
来源：http://jsc.aibaodan.cn

PHP:  $a && $b || !$c
来源：http://lzh.dianchejie.cn

JS:   a && b || !c
来源：http://qvb.aizwys.cn

TS:   a && b || !c
来源：http://ker.xuetiantiany.cn

Java: a && b || !c
来源：http://xlr.tanke756.top

Go:   a && b || !c
来源：http://kvb.hfpthk.cn

Ruby: a && b || !c
来源：http://fse.chenzaomai.com

C#:   a && b || !c
来源：http://tzd.yonumen.top

[B16] 卫语句：不满足条件提前返回
来源：http://tnn.haohaochexian.top

Py:   if not data: return
来源：http://gpu.gogol.net.cn

PHP:  if (!$data) { return; }
来源：http://oat.xuanzx.com

JS:   if (!data) return;
来源：http://ucp.fzhhl.top

TS:   if (!data) return;
来源：http://tax.smart0.xyz

Java: if (data == null) return;
来源：http://cra.quarkkingdee.top

Go:   if data == nil { return }
来源：http://hfm.xinyue.icu

Ruby: return if data.nil?
来源：http://vyz.hywenlv.cn

C#:   if (data == null) return;
来源：http://cnq.iojbl.cn

================================================================================
来源：http://svw.sysykeji.top

C. 函数与作用域
来源：http://sme.tian-w.cn

================================================================================
来源：http://evz.cheryme.top

[C01] 定义函数
来源：http://hoa.zhixingplan.top

Py:   def add(a, b): return a + b
来源：http://yjs.iojbl.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kjy.0kj1m.cn

JS:   function add(a, b) { return a + b; }
来源：http://cuh.ydjk.org.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lkh.hywenlv.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://kqj.ywan-chungtsiang.top

Go:   func add(a, b int) int { return a + b }
来源：http://fuj.epnwcf.com

Ruby: def add(a, b); a + b; end
来源：http://kpk.ctjpmb.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://owp.jianghu66.top

[C02] 默认参数
来源：http://dxe.uphjek.com

Py:   def greet(name="World"): return name
来源：http://apf.daxiang520.top

PHP:  function greet($name = "World") { return $name; }
来源：http://sdg.zhongyouzk.top

JS:   function greet(name = "World") { return name; }
来源：http://wsn.ctjpmb.com

TS:   function greet(name: string = "World") { return name; }
来源：http://arj.zhoulong.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://avf.dashuyun.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://fab.ydzc1.top

Ruby: def greet(name = "World") = name
来源：http://hke.cashguo.top

C#:   string Greet(string name = "World") => name;
来源：http://xua.aizwys.cn

[C03] 可变参数
来源：http://rpw.chenjidiqi.icu

Py:   def total(*args): return sum(args)
来源：http://wum.jqgfzy.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ppw.yonumen.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://rnv.nanxinkj.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://cmf.quarkkingdee.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://qkn.yj202588.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://dxn.jianghu66.top

Ruby: def total(*nums); nums.sum; end
来源：http://edx.ywan-chungtsiang.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zyv.ybcxt.top

[C04] 命名参数 / 关键字参数
来源：http://xzn.ehwqpu.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://tow.vehdjk.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://liu.yfazqb.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://fwu.jqgfzy.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://fie.yuxming.cn

Java: // 无：用 Builder 模式或 record
来源：http://puu.aizwys.cn

Go:   // 无：用配置结构体参数
来源：http://ohk.yj20258888.top

Ruby: f(a: 1, b: 2)
来源：http://plj.9152youxi.cn

C#:   f(a: 1, b: 2)
来源：http://ehn.ydjk.org.cn

[C05] 返回多个值
来源：http://wtl.yj202588.top

Py:   return a, b
来源：http://djy.ehwqpu.com

PHP:  return [$a, $b];
来源：http://plu.yfazqb.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://uop.gogol.net.cn

TS:   return { a, b };
来源：http://fqq.hongshengwenyu.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xmf.iojbl.cn

Go:   return a, b
来源：http://ust.mhx1999.top

Ruby: return a, b
来源：http://xdc.svipenyu.cn

C#:   return (a, b);              // ValueTuple
来源：http://wyx.316326.xyz

[C06] 匿名函数 / lambda
来源：http://vqy.hcnkem.com

Py:   square = lambda x: x * x
来源：http://gcu.xuanzx.com

PHP:  $square = fn($x) => $x * $x;
来源：http://amk.ywan-chungtsiang.top

JS:   const square = x => x * x;
来源：http://ooi.daxiang520.top

TS:   const square = (x: number): number => x * x;
来源：http://gop.smart0.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://gaq.pycfn.com

Go:   sq := func(x int) int { return x * x }
来源：http://ubw.0kj1m.cn

Ruby: square = ->(x) { x * x }
来源：http://bgz.zhaomingkeji.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://evw.cheryme.top

[C07] 把函数作为参数传入
来源：http://cyb.316326.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://jfp.zhaomingkeji.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://nnz.jinqigufen.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ejr.0kj1m.cn

TS:   arr.map(String)
来源：http://vlw.zhengqikj.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://jzt.jqgfzy.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://fvj.gzhubu.top

Ruby: arr.map(&:upcase)
来源：http://rsa.316326.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://rva.mhx1999.top

[C08] 闭包
来源：http://aip.snrcjt.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://jbs.shangyingyoupin.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://lnl.gotoacloud.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qku.bbcook.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://luu.zhaomingkeji.xyz

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mgc.pycfn.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ylj.hywenlv.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://onc.vehdjk.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://nsn.yfazqb.com

[C09] 递归
来源：http://kig.iojbl.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://vnx.zhengqikj.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://okq.0kj1m.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://keo.sysykeji.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ntc.sysykeji.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ovn.aibaodan.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ocu.ppjwa.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ykd.zhengqikj.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://xcv.fzhhl.top

[C10] 变量作用域
来源：http://qid.jiagoushi.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://pyz.tarul.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://kjv.tarul.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://cxb.hongshengwenyu.top

TS:   同 JS
来源：http://pcs.fengsongda.top

Java: 方法内为块级作用域
来源：http://hfw.yangfankeji.com

Go:   花括号块级作用域
来源：http://jud.epnwcf.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mfz.vqdsnc.cn

C#:   块级作用域
来源：http://ojs.guannengcc.top

[C11] 模块导入与导出
来源：http://rpt.jiagoushi.top

Py:   from module import func
来源：http://wkj.fehbvm.com

PHP:  require "file.php";  或 use App\Service;
来源：http://pgp.yj20258.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://gfw.gotoacloud.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://rou.jlsjyb.cn

Java: import java.util.List;
来源：http://ugz.zhongyouzk.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mgq.andypj.xyz

Ruby: require "json"; require_relative "./util"
来源：http://vsf.cashguo.top

C#:   using System.Text;
来源：http://tsv.cucudq.cn

[C12] 立即执行函数 IIFE
来源：http://mst.cqqwz.cn

Py:   (lambda: print("run"))()
来源：http://dit.vqdsnc.cn

PHP:  (function () { echo "run"; })();
来源：http://abb.fzhhl.top

JS:   (() => { console.log("run"); })();
来源：http://ycg.zhijiandao.cn

TS:   (() => { console.log("run"); })();
来源：http://xit.gotoacloud.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ozx.zdqjudy.top

Go:   func() { fmt.Println("run") }()
来源：http://ojj.snrcjt.cn

Ruby: -> { puts "run" }.call
来源：http://exq.gogol.net.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://djt.kuanghao11.cn

[C13] 类型声明 / 类型注解
来源：http://lln.fengsongda.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://bvx.jinghuilouyu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nmo.ybcxt.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://luj.ydjk.org.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qsf.zhaomingkeji.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://sjl.cucudq.cn

Go:   func add(a, b int) int
来源：http://xgg.mhx1999.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://qbm.xziqi.cn

C#:   int Add(int a, int b) => a + b;
来源：http://fcn.hesvh.cn

[C14] 泛型函数
来源：http://yia.ppjwa.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ojk.cucudq.cn

PHP:  // 无泛型
来源：http://ude.aizwys.cn

JS:   // 无泛型
来源：http://vky.pengpengdd.cyou

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://oqt.pycfn.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://vlh.gaohongyu789.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://pkb.hammf.cn

Ruby: # 无泛型
来源：http://dlp.yangfankeji.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://nru.yj202588.top

[C15] 解构 / 展开参数
来源：http://vjd.yangfankeji.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xpi.316326.xyz

PHP:  [$a, $b] = $pair;
来源：http://kpm.jqgfzy.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ogk.c1oappe.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://gyh.epnwcf.com

Java: // 无解构
来源：http://uni.shangyingyoupin.top

Go:   // 无解构
来源：http://fqv.hcnkem.com

Ruby: a, b = pair
来源：http://elt.xinyue.icu

C#:   var (a, b) = pair;
来源：http://hoa.cqqwz.cn

[C16] 函数 / 方法重载
来源：http://ggl.ybcxt.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ozb.yangfankeji.com

PHP:  // 无重载
来源：http://rer.hywenlv.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ksd.havefunace.top

TS:   // 用联合类型或重载签名声明
来源：http://vxn.yfazqb.com

Java: void f(int a) {}  void f(String a) {}
来源：http://ojc.zhongyouzk.top

Go:   // 无重载：用不同函数名
来源：http://tul.yanxiufei.cn

Ruby: # 无重载：靠动态参数
来源：http://wcu.chenlongwang.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://tqx.yj202588.top

================================================================================
来源：http://hbu.yuanzhike.top

D. 数组 / 列表 / 集合
来源：http://tqv.ehwqpu.com

================================================================================
来源：http://csf.fengsongda.top

[D01] 创建数组 / 列表
来源：http://tfb.zhongyouzk.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://szk.shanyushiyangkeji.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://vzj.hongshengwenyu.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://qib.guannengcc.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://wcp.epnwcf.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ylx.jqgufenzy.top

Go:   arr := []int{1, 2, 3}
来源：http://yhw.yangfankeji.com

Ruby: arr = [1, 2, 3]
来源：http://cks.ppjwa.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://zxd.shuidangran.top

[D02] 追加元素到末尾
来源：http://pfp.0kj1m.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://yye.wangdashe.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ruv.zhaomingkeji.xyz

JS:   arr.push(4);
来源：http://fju.cucudq.cn

TS:   arr.push(4);
来源：http://uyu.jiagoushi.top

Java: list.add(4);
来源：http://tbt.haohaochexian.top

Go:   arr = append(arr, 4)
来源：http://rgw.ivvv.top

Ruby: arr << 4; arr.push(5)
来源：http://mcm.zhongyouzk.top

C#:   list.Add(4);
来源：http://psd.yueranfly.top

[D03] 在指定位置插入元素
来源：http://dtt.ybcxt.top

Py:   arr.insert(0, 0)
来源：http://ooz.ivvv.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://cqs.shanyushiyangtech.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://xif.gogol.net.cn

TS:   arr.splice(0, 0, 0);
来源：http://dbl.ivvv.top

Java: list.add(0, 0);
来源：http://xef.shanyushiyangtech.top

Go:   arr = append([]int{0}, arr...)
来源：http://pcj.fengsongda.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ymb.ppjwa.cn

C#:   list.Insert(0, 0);
来源：http://bia.aibaodan.cn

[D04] 删除元素
来源：http://zdb.jiagoushi.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ozj.hfpthk.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://lgs.pengpengdd.cyou

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ysc.jqgufenzy.top

TS:   arr.splice(0, 1);
来源：http://vks.tian-w.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mjf.shuidangran.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hvn.hesvh.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://zha.hnxiangtu.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wyp.quarkkingdee.top

[D05] 访问与修改元素
来源：http://oqj.jianghu66.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://pqr.cucudq.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mqg.cheryme.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://xnu.daxiang520.top

TS:   arr[0]; arr.at(-1);
来源：http://qfz.yangfankeji.com

Java: list.get(0); list.set(0, 9);
来源：http://oyn.cucudq.cn

Go:   arr[0]; arr[0] = 9
来源：http://ock.yj202588.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://xar.hnxiangtu.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://bzz.ppjwa.cn

[D06] 数组长度
来源：http://bkw.tarul.cn

Py:   len(arr)
来源：http://ixc.hywenlv.cn

PHP:  count($arr);
来源：http://gzr.tanke756.top

JS:   arr.length
来源：http://jex.9152youxi.cn

TS:   arr.length
来源：http://sxp.ppjwa.cn

Java: list.size();
来源：http://gjc.kuanghao11.cn

Go:   len(arr)
来源：http://qwb.52xcode.cn

Ruby: arr.length; arr.size
来源：http://tsa.bbcook.cn

C#:   list.Count;
来源：http://dem.yanxiufei.cn

[D07] 切片 / 取子数组
来源：http://rdj.tian-w.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://zzi.jinqigufen.top

PHP:  array_slice($arr, 1, 3);
来源：http://nhw.sweek.top

JS:   arr.slice(1, 4);
来源：http://dzk.xziqi.cn

TS:   arr.slice(1, 4);
来源：http://iup.sjlbkw.cn

Java: list.subList(1, 4);
来源：http://lys.sjlbkw.cn

Go:   arr[1:4]
来源：http://bhq.vehdjk.com

Ruby: arr[1, 3]
来源：http://kui.fengsongda.top

C#:   list.GetRange(1, 3);
来源：http://wyx.jqgfzy.top

[D08] 合并两个数组
来源：http://geg.nwbrower.top

Py:   a + b;  a.extend(b)
来源：http://ivv.birdmap.top

PHP:  array_merge($a, $b);
来源：http://tof.ydzc1.top

JS:   [...a, ...b];  a.concat(b);
来源：http://mev.9152youxi.cn

TS:   [...a, ...b];
来源：http://ujk.guowangkeji.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://cni.cheryme.top

Go:   append(a, b...)
来源：http://pml.sufxvd.cn

Ruby: a + b;  a.concat(b)
来源：http://win.zdbjq.cn

C#:   a.Concat(b).ToList()
来源：http://xmo.jinyuanbaomall.cn

[D09] 排序（升序）
来源：http://bfe.mhx1999.top

Py:   sorted(arr);  arr.sort()
来源：http://tnw.chenzaomai.com

PHP:  sort($arr);
来源：http://ryn.nanxinkj.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://lxz.sweek.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://wzm.gzhubu.top

Java: Collections.sort(list);  list.sort(null);
来源：http://mut.xuanzx.com


<!-- 参考信息 -->