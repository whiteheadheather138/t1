代发 wailian999

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://izf.hesvh.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://goy.havefunace.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://yga.xingfuxueyuan.xyz

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://goh.xziqi.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sem.jianghu66.top

[B10] 遍历同时拿索引
来源：http://cwu.jyoumei.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://nji.birdmap.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://kcu.ivvv.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://bhf.shanyushiyangtech.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://nib.0kj1m.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://fxy.jiagoushi.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://nrk.guannengcc.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://plf.dianchejie.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://biq.tian-w.cn

[B11] 生成数字序列 / 区间
来源：http://pzt.svipenyu.cn

Py:   list(range(0, 10, 2))
来源：http://fdq.zhijiandao.cn

PHP:  range(0, 10, 2);
来源：http://mdw.redwolf501.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hyn.pycfn.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://faz.jqgufenzy.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wix.yvedp.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://xsn.cucudq.cn

Ruby: (0...10).step(2).to_a
来源：http://rji.shanyushiyangtech.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://pyg.zhengqikj.top

[B12] 跳出多层循环
来源：http://yly.hnxiangtu.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://qer.redwolf501.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://rug.dashuyun.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://zeq.52xcode.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ryr.hysaishi.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mjn.nwbrower.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://lgm.snrcjt.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://zqd.xinyue.icu

C#:   # 无标签：用 goto label 或布尔标志
来源：http://lfa.zhaomingkeji.xyz

[B13] 判断是否为数字
来源：http://uyf.hywenlv.cn

Py:   isinstance(x, (int, float))
来源：http://ffq.hnxiangtu.top

PHP:  is_numeric($x)
来源：http://kng.meibo888.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://suv.ctjpmb.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dku.sweek.top

Java: x instanceof Number
来源：http://yeh.9152youxi.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://rze.epnwcf.com

Ruby: x.is_a?(Numeric)
来源：http://hkc.kuanghao11.cn

C#:   x is int or double or decimal
来源：http://qol.zdbjq.cn

[B14] 判断值是否在集合内
来源：http://ajb.birdmap.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://xsl.jyoumei.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://zqh.ydzc1.top

JS:   [1, 2, 3].includes(x)
来源：http://rqj.nanxuanxn.top

TS:   [1, 2, 3].includes(x)
来源：http://suq.sxryk.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://epi.jinqigufen.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://kli.vehdjk.com

Ruby: [1, 2, 3].include?(x)
来源：http://vge.hfpthk.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ame.tanke756.top

[B15] 布尔运算与取反
来源：http://fkj.jlsjyb.cn

Py:   a and b or not c
来源：http://flj.jlsjyb.cn

PHP:  $a && $b || !$c
来源：http://xcy.ppjwa.cn

JS:   a && b || !c
来源：http://coq.zhijiandao.cn

TS:   a && b || !c
来源：http://nfq.zycfv.cn

Java: a && b || !c
来源：http://kop.yuanzhike.top

Go:   a && b || !c
来源：http://xkd.xinyue.icu

Ruby: a && b || !c
来源：http://suj.pycfn.com

C#:   a && b || !c
来源：http://uap.316326.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://pkf.ctjpmb.com

Py:   if not data: return
来源：http://iht.fktsv.cn

PHP:  if (!$data) { return; }
来源：http://mdk.sxryk.cn

JS:   if (!data) return;
来源：http://akf.dianchejie.cn

TS:   if (!data) return;
来源：http://skv.dianchejie.cn

Java: if (data == null) return;
来源：http://umi.hcnkem.com

Go:   if data == nil { return }
来源：http://pwp.ywan-chungtsiang.top

Ruby: return if data.nil?
来源：http://sri.guowangkeji.top

C#:   if (data == null) return;
来源：http://jva.tianlin.xyz

================================================================================
来源：http://mkb.yuxming.cn

C. 函数与作用域
来源：http://whx.chenzaomai.com

================================================================================
来源：http://dpm.hcnkem.com

[C01] 定义函数
来源：http://rre.smart0.xyz

Py:   def add(a, b): return a + b
来源：http://yfr.c1oappe.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tfu.yj20258.top

JS:   function add(a, b) { return a + b; }
来源：http://tnl.jiagoushi.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ira.yj202588.top

Java: static int add(int a, int b) { return a + b; }
来源：http://lut.sysykeji.top

Go:   func add(a, b int) int { return a + b }
来源：http://oih.zhaomingkeji.xyz

Ruby: def add(a, b); a + b; end
来源：http://umo.tianlin.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://boc.zhongyouzk.top

[C02] 默认参数
来源：http://uwo.jlsjyb.cn

Py:   def greet(name="World"): return name
来源：http://bwa.zhiwuduotai.top

PHP:  function greet($name = "World") { return $name; }
来源：http://pjo.havefunace.top

JS:   function greet(name = "World") { return name; }
来源：http://zea.aizwys.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://evu.ybcxt.top

Java: // 无默认参数：方法重载或 Optional
来源：http://znv.tarul.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ypb.andypj.xyz

Ruby: def greet(name = "World") = name
来源：http://njj.shuidangran.top

C#:   string Greet(string name = "World") => name;
来源：http://gln.zhiwuduotai.top

[C03] 可变参数
来源：http://sai.zhaomingkeji.xyz

Py:   def total(*args): return sum(args)
来源：http://xmc.vehdjk.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://yzl.vehdjk.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://cnu.shanyushiyangtech.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mfl.ehwqpu.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ojk.havefunace.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://oqf.shanyushiyangkeji.top

Ruby: def total(*nums); nums.sum; end
来源：http://ann.zhiwuduotai.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://tiq.daxiang520.top

[C04] 命名参数 / 关键字参数
来源：http://zws.316326.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://fdp.nwbrower.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://vud.epnwcf.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://uvi.ydzc1.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://oex.guowangkeji.top

Java: // 无：用 Builder 模式或 record
来源：http://ted.quarkkingdee.top

Go:   // 无：用配置结构体参数
来源：http://boi.zhoulong.xyz

Ruby: f(a: 1, b: 2)
来源：http://geh.ppjwa.cn

C#:   f(a: 1, b: 2)
来源：http://jpm.jinyuanbaomall.cn

[C05] 返回多个值
来源：http://ucn.gogol.net.cn

Py:   return a, b
来源：http://fwi.dianchejie.cn

PHP:  return [$a, $b];
来源：http://mji.jinghuilouyu.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://vvt.shzxlz.cn

TS:   return { a, b };
来源：http://xau.jinyuanbaomall.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ytj.zycfv.cn

Go:   return a, b
来源：http://xed.yangfankeji.com

Ruby: return a, b
来源：http://csc.guowangkeji.top

C#:   return (a, b);              // ValueTuple
来源：http://ova.shangyingyoupin.top

[C06] 匿名函数 / lambda
来源：http://mzh.guannengcc.top

Py:   square = lambda x: x * x
来源：http://ipu.jqgufenzy.top

PHP:  $square = fn($x) => $x * $x;
来源：http://dcu.yuanzhike.top

JS:   const square = x => x * x;
来源：http://bzv.jinghuilouyu.cn

TS:   const square = (x: number): number => x * x;
来源：http://asc.uphjek.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://uvz.yj202588.top

Go:   sq := func(x int) int { return x * x }
来源：http://dis.316326.xyz

Ruby: square = ->(x) { x * x }
来源：http://efp.tarul.cn

C#:   Func<int, int> square = x => x * x;
来源：http://zfq.chenlongwang.top

[C07] 把函数作为参数传入
来源：http://vtg.chenzaomai.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://aup.316326.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://hfd.chenzaomai.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://yrj.daxiang520.top

TS:   arr.map(String)
来源：http://afu.havefunace.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://pjp.yj20258.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://fgr.c1oappe.top

Ruby: arr.map(&:upcase)
来源：http://chx.yangfankeji.com

C#:   arr.Select(s => s.ToUpper())
来源：http://vug.cdnleiting.top

[C08] 闭包
来源：http://xdw.kuanghao11.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://tbg.zhixingplan.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://yrq.zdqjudy.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://zol.vehdjk.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://xbm.jqgfzy.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wns.ivvv.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://brv.jqgufenzy.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://fsu.tarul.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://aet.tianlin.xyz

[C09] 递归
来源：http://rbz.shangyingyoupin.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://vwn.xylfe.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://qwl.aizwys.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://joz.yj20258.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uox.sysykeji.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://opm.jinqigufen.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://jis.meibo888.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://eus.jinghuilouyu.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://slo.jqgufenzy.top

[C10] 变量作用域
来源：http://sul.gzhubu.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ard.zdbjq.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://jsy.tianlin.xyz

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ojf.jyoumei.cn

TS:   同 JS
来源：http://nhm.316326.xyz

Java: 方法内为块级作用域
来源：http://xod.zdqjudy.top

Go:   花括号块级作用域
来源：http://vud.hywenlv.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://dtz.daria6918.cn

C#:   块级作用域
来源：http://sdm.birdmap.top

[C11] 模块导入与导出
来源：http://nqz.yj20258.top

Py:   from module import func
来源：http://cmz.xziqi.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://qcd.cqqwz.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://hkk.jlsjyb.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://dtp.zycfv.cn

Java: import java.util.List;
来源：http://cie.xuanzx.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://cfv.yj202588.top

Ruby: require "json"; require_relative "./util"
来源：http://rmk.haohaochexian.top

C#:   using System.Text;
来源：http://njg.zdbjq.cn

[C12] 立即执行函数 IIFE
来源：http://srq.tianlin.xyz

Py:   (lambda: print("run"))()
来源：http://iut.bbcook.cn

PHP:  (function () { echo "run"; })();
来源：http://ugo.yueranfly.top

JS:   (() => { console.log("run"); })();
来源：http://psd.xingfuxueyuan.xyz

TS:   (() => { console.log("run"); })();
来源：http://nyh.yfazqb.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ezu.sjlbkw.cn

Go:   func() { fmt.Println("run") }()
来源：http://lkk.jinghuilouyu.cn

Ruby: -> { puts "run" }.call
来源：http://noo.cucudq.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://cls.tanke756.top

[C13] 类型声明 / 类型注解
来源：http://hev.uphjek.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://bnl.hnxiangtu.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nyn.birdmap.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://yve.zycfv.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ueb.hongshengwenyu.top

Java: int add(int a, int b) { return a + b; }
来源：http://amg.yvedp.cn

Go:   func add(a, b int) int
来源：http://yzs.chenzaomai.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://soh.pycfn.com

C#:   int Add(int a, int b) => a + b;
来源：http://wom.tianlin.xyz

[C14] 泛型函数
来源：http://url.aibaodan.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://vdb.zdqjudy.top

PHP:  // 无泛型
来源：http://kro.sysykeji.top

JS:   // 无泛型
来源：http://ryc.yj202588.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ual.hysaishi.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://sor.tanke756.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://qzw.hammf.cn

Ruby: # 无泛型
来源：http://byk.zhongyouzk.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://pcs.cdnleiting.top

[C15] 解构 / 展开参数
来源：http://blz.yongpay.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://uwg.dashuyun.cn

PHP:  [$a, $b] = $pair;
来源：http://bwd.mhx1999.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://sln.cdnleiting.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://atw.wangshuangyany.cn

Java: // 无解构
来源：http://rur.pycfn.com

Go:   // 无解构
来源：http://nxc.chenjidiqi.icu

Ruby: a, b = pair
来源：http://lkq.xingfuxueyuan.xyz

C#:   var (a, b) = pair;
来源：http://zho.yuanzhike.top

[C16] 函数 / 方法重载
来源：http://ykk.cdnleiting.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://yix.snrcjt.cn

PHP:  // 无重载
来源：http://rqr.yanxiufei.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://yhi.yvedp.cn

TS:   // 用联合类型或重载签名声明
来源：http://sba.sxryk.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ush.yj20258.top

Go:   // 无重载：用不同函数名
来源：http://olg.xinyue.icu

Ruby: # 无重载：靠动态参数
来源：http://rni.cheryme.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://ljj.haohaochexian.top

================================================================================
来源：http://bhw.smart0.xyz

D. 数组 / 列表 / 集合
来源：http://vsb.dashuyun.cn

================================================================================
来源：http://snl.sjlbkw.cn

[D01] 创建数组 / 列表
来源：http://wxn.tianlin.xyz

Py:   arr = [1, 2, 3];  empty = []
来源：http://eih.uphjek.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://vti.cdnleiting.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://rdq.zhongyouzk.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://tdb.wangdashe.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://xcl.yuanzhike.top

Go:   arr := []int{1, 2, 3}
来源：http://bhh.gotoacloud.top

Ruby: arr = [1, 2, 3]
来源：http://sjb.sysykeji.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://umm.zhixingplan.top

[D02] 追加元素到末尾
来源：http://tht.hongshengwenyu.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://gpt.epnwcf.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://nyz.hnxiangtu.top

JS:   arr.push(4);
来源：http://isr.jqgufenzy.top

TS:   arr.push(4);
来源：http://lhr.fktsv.cn

Java: list.add(4);
来源：http://vuf.jqgfzy.top

Go:   arr = append(arr, 4)
来源：http://ahr.yueranfly.top

Ruby: arr << 4; arr.push(5)
来源：http://aru.jqgufenzy.top

C#:   list.Add(4);
来源：http://ajh.yongpay.top

[D03] 在指定位置插入元素
来源：http://asd.zycfv.cn

Py:   arr.insert(0, 0)
来源：http://lyd.nanxuanxn.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://lyq.shangyingyoupin.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://bvy.zdqjudy.top

TS:   arr.splice(0, 0, 0);
来源：http://tra.ywan-chungtsiang.top

Java: list.add(0, 0);
来源：http://qsr.dianchejie.cn

Go:   arr = append([]int{0}, arr...)
来源：http://jyo.yueranfly.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://nfz.meibo888.top

C#:   list.Insert(0, 0);
来源：http://cvh.xuetiantiany.cn

[D04] 删除元素
来源：http://awq.yuxming.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://oqq.fengsongda.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://bac.xziqi.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://buf.cqqwz.cn

TS:   arr.splice(0, 1);
来源：http://zau.zhixingplan.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://igk.hesvh.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://azm.epnwcf.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://qqh.bjfxy.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://pkh.redwolf501.top

[D05] 访问与修改元素
来源：http://fdt.xylfe.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://qch.haohaochexian.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wjj.shangyingyoupin.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://zqy.xuanzx.com

TS:   arr[0]; arr.at(-1);
来源：http://khk.xingfuxueyuan.xyz

Java: list.get(0); list.set(0, 9);
来源：http://rkq.cheryme.top

Go:   arr[0]; arr[0] = 9
来源：http://fqc.9152youxi.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://rhq.jyoumei.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://aqj.yj202588.top

[D06] 数组长度
来源：http://rpj.9152youxi.cn

Py:   len(arr)
来源：http://ytp.yuanzhike.top

PHP:  count($arr);
来源：http://xmz.daria6918.cn

JS:   arr.length
来源：http://asq.fzhhl.top

TS:   arr.length
来源：http://ouf.316326.xyz

Java: list.size();
来源：http://pgt.gzhubu.top

Go:   len(arr)
来源：http://wax.jinqigufen.top

Ruby: arr.length; arr.size
来源：http://swk.gaohongyu789.top

C#:   list.Count;
来源：http://ltq.jlsjyb.cn

[D07] 切片 / 取子数组
来源：http://pre.wangshuangyany.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://xnk.tian-w.cn

PHP:  array_slice($arr, 1, 3);
来源：http://idl.yj20258.top

JS:   arr.slice(1, 4);
来源：http://hzw.xziqi.cn

TS:   arr.slice(1, 4);
来源：http://sad.52xcode.cn

Java: list.subList(1, 4);
来源：http://rqc.tarul.cn

Go:   arr[1:4]
来源：http://muq.xuanzx.com

Ruby: arr[1, 3]
来源：http://gli.chenzaomai.com

C#:   list.GetRange(1, 3);
来源：http://upf.gzhubu.top

[D08] 合并两个数组
来源：http://wpe.zhengqikj.top

Py:   a + b;  a.extend(b)
来源：http://fmt.havefunace.top

PHP:  array_merge($a, $b);
来源：http://ero.xingfuxueyuan.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://jfa.redwolf501.top

TS:   [...a, ...b];
来源：http://whf.cdnleiting.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://kfy.shzxlz.cn

Go:   append(a, b...)
来源：http://xqm.chenlongwang.top

Ruby: a + b;  a.concat(b)
来源：http://bti.guowangkeji.top

C#:   a.Concat(b).ToList()
来源：http://dhs.ywan-chungtsiang.top

[D09] 排序（升序）
来源：http://eoj.52xcode.cn

Py:   sorted(arr);  arr.sort()
来源：http://kez.hnxiangtu.top

PHP:  sort($arr);
来源：http://njp.fzhhl.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://sqr.svipenyu.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://hbv.gogol.net.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://mzn.jinqigfzy.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wmy.vehdjk.com

Ruby: arr.sort
来源：http://lxi.shanyushiyangtech.top

C#:   list.Sort();
来源：http://wxi.yuxming.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://chp.aizwys.cn


<!-- 参考信息 -->