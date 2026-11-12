代发 wailian999

Java: do { i++; } while (i < 10);
来源：http://zzx.gotoacloud.top

Go:   for { i++; if i >= 10 { break } }
来源：http://efl.zhoulong.xyz

Ruby: begin; i += 1; end while i < 10
来源：http://urd.redwolf501.top

C#:   do { i++; } while (i < 10);
来源：http://dhe.jqgufenzy.top

[B09] break 与 continue
来源：http://hvn.fehbvm.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://jiz.c1oappe.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://sbz.yuxming.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cgu.zhongyouzk.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sra.zycfv.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ndy.jianghu66.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ppt.ppjwa.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ehl.yonumen.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ekf.shuidangran.top

[B10] 遍历同时拿索引
来源：http://lhw.jinqigufen.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://orm.yvedp.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://jrf.zhengqikj.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hlz.zhoulong.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ezn.fehbvm.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://fqp.zdqjudy.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://xkq.ivvv.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://iqt.tarul.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://gqd.cashguo.top

[B11] 生成数字序列 / 区间
来源：http://jzv.52xcode.cn

Py:   list(range(0, 10, 2))
来源：http://tzn.hcnkem.com

PHP:  range(0, 10, 2);
来源：http://ajj.birdmap.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vht.fktsv.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yxh.fzhhl.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://bvk.shangyingyoupin.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://djm.ydzc1.top

Ruby: (0...10).step(2).to_a
来源：http://aze.ivvv.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://gnm.zhijiandao.cn

[B12] 跳出多层循环
来源：http://hjt.gogol.net.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://mva.c1oappe.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://tyr.yangfankeji.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mpt.ppjwa.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://cll.gzhubu.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://xkm.hcnkem.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://nbu.gogol.net.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://klc.yongpay.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://azy.zhiwuduotai.top

[B13] 判断是否为数字
来源：http://ynp.52xcode.cn

Py:   isinstance(x, (int, float))
来源：http://asr.jiagoushi.top

PHP:  is_numeric($x)
来源：http://klu.quarkkingdee.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cac.zycfv.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vji.ctjpmb.com

Java: x instanceof Number
来源：http://sbz.havefunace.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://omv.mhx1999.top

Ruby: x.is_a?(Numeric)
来源：http://pmt.shanyushiyangtech.top

C#:   x is int or double or decimal
来源：http://cla.yj20258888.top

[B14] 判断值是否在集合内
来源：http://mgt.yangfankeji.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://vqr.sysykeji.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://nxs.wangdashe.top

JS:   [1, 2, 3].includes(x)
来源：http://keg.yj20258.top

TS:   [1, 2, 3].includes(x)
来源：http://pzh.aizwys.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://npd.tianlin.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://uhr.iojbl.cn

Ruby: [1, 2, 3].include?(x)
来源：http://isa.ehwqpu.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://znj.epnwcf.com

[B15] 布尔运算与取反
来源：http://fog.epnwcf.com

Py:   a and b or not c
来源：http://gcr.cqqwz.cn

PHP:  $a && $b || !$c
来源：http://wql.ydzc1.top

JS:   a && b || !c
来源：http://wnj.daria6918.cn

TS:   a && b || !c
来源：http://zvz.vehdjk.com

Java: a && b || !c
来源：http://whd.jinyuanbaomall.cn

Go:   a && b || !c
来源：http://zwt.zhiwuduotai.top

Ruby: a && b || !c
来源：http://oex.jqgufenzy.top

C#:   a && b || !c
来源：http://dzp.jinqigufen.top

[B16] 卫语句：不满足条件提前返回
来源：http://djd.vqdsnc.cn

Py:   if not data: return
来源：http://gli.ivvv.top

PHP:  if (!$data) { return; }
来源：http://hoh.ivvv.top

JS:   if (!data) return;
来源：http://mtv.zdbjq.cn

TS:   if (!data) return;
来源：http://ztl.zhaomingkeji.xyz

Java: if (data == null) return;
来源：http://xol.ydzc1.top

Go:   if data == nil { return }
来源：http://opk.fengsongda.top

Ruby: return if data.nil?
来源：http://mdo.uphjek.com

C#:   if (data == null) return;
来源：http://bxn.jqgufenzy.top

================================================================================
来源：http://mdk.jqgfzy.top

C. 函数与作用域
来源：http://ulk.wangshuangyany.cn

================================================================================
来源：http://pvm.birdmap.top

[C01] 定义函数
来源：http://xky.dashuyun.cn

Py:   def add(a, b): return a + b
来源：http://wzh.yj202588.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zjl.chenzaomai.com

JS:   function add(a, b) { return a + b; }
来源：http://dsg.zycfv.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kxn.52xcode.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://uzf.guowangkeji.top

Go:   func add(a, b int) int { return a + b }
来源：http://uwe.smart0.xyz

Ruby: def add(a, b); a + b; end
来源：http://knn.0kj1m.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://lcd.zhongyouzk.top

[C02] 默认参数
来源：http://tai.gaohongyu789.top

Py:   def greet(name="World"): return name
来源：http://xpv.jinqigfzy.top

PHP:  function greet($name = "World") { return $name; }
来源：http://oqz.hesvh.cn

JS:   function greet(name = "World") { return name; }
来源：http://aay.tanke756.top

TS:   function greet(name: string = "World") { return name; }
来源：http://uhq.ppjwa.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://lzy.hammf.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://lvi.ppjwa.cn

Ruby: def greet(name = "World") = name
来源：http://qcr.9152youxi.cn

C#:   string Greet(string name = "World") => name;
来源：http://dnu.daria6918.cn

[C03] 可变参数
来源：http://cvu.gotoacloud.top

Py:   def total(*args): return sum(args)
来源：http://coc.hongshengwenyu.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://cda.jinghuilouyu.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ily.cucudq.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://erq.zhengqikj.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://lup.nanxinkj.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wnd.tianlin.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://jit.pengpengdd.cyou

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://sir.cdnleiting.top

[C04] 命名参数 / 关键字参数
来源：http://zrf.svipenyu.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://sla.hesvh.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xgg.zdbjq.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://huf.yuxming.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://tkz.daxiang520.top

Java: // 无：用 Builder 模式或 record
来源：http://sdv.fengsongda.top

Go:   // 无：用配置结构体参数
来源：http://vyy.dianchejie.cn

Ruby: f(a: 1, b: 2)
来源：http://csy.uphjek.com

C#:   f(a: 1, b: 2)
来源：http://uuw.ydzc1.top

[C05] 返回多个值
来源：http://aac.sjlbkw.cn

Py:   return a, b
来源：http://ptx.jinyuanbaomall.cn

PHP:  return [$a, $b];
来源：http://foe.sysykeji.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://crf.chenlongwang.top

TS:   return { a, b };
来源：http://mip.fktsv.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://nid.gotoacloud.top

Go:   return a, b
来源：http://clg.zhiwuduotai.top

Ruby: return a, b
来源：http://jza.zhengqikj.top

C#:   return (a, b);              // ValueTuple
来源：http://xpt.guowangkeji.top

[C06] 匿名函数 / lambda
来源：http://ahe.jlsjyb.cn

Py:   square = lambda x: x * x
来源：http://pkg.aibaodan.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://bnn.gzhubu.top

JS:   const square = x => x * x;
来源：http://phl.cheryme.top

TS:   const square = (x: number): number => x * x;
来源：http://zhq.svipenyu.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://fyw.yj20258.top

Go:   sq := func(x int) int { return x * x }
来源：http://yis.yj20258.top

Ruby: square = ->(x) { x * x }
来源：http://xsg.xinyue.icu

C#:   Func<int, int> square = x => x * x;
来源：http://onu.hesvh.cn

[C07] 把函数作为参数传入
来源：http://jym.52xcode.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mzi.daxiang520.top

PHP:  array_map("strtoupper", $arr);
来源：http://tme.andypj.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://rzg.daria6918.cn

TS:   arr.map(String)
来源：http://cmc.zhijiandao.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://zmb.yuxming.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://cxp.chenjidiqi.icu

Ruby: arr.map(&:upcase)
来源：http://dgx.iojbl.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://rjp.redwolf501.top

[C08] 闭包
来源：http://fds.zhoulong.xyz

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mac.cqqwz.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mxw.yangfankeji.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ivd.jqgfzy.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wnq.chenjidiqi.icu

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ygq.cucudq.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ret.52xcode.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://adk.jqgfzy.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://utg.c1oappe.top

[C09] 递归
来源：http://mrm.yonumen.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ody.yj202588.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://iff.zhongyouzk.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dcj.xingfuxueyuan.xyz

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pdl.gaohongyu789.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://kdp.havefunace.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ugn.zhongyouzk.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://uue.ybcxt.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ush.sxryk.cn

[C10] 变量作用域
来源：http://gly.havefunace.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://yxg.shanyushiyangtech.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://tny.zhaomingkeji.xyz

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hoo.ehwqpu.com

TS:   同 JS
来源：http://dfq.epnwcf.com

Java: 方法内为块级作用域
来源：http://ubz.fengsongda.top

Go:   花括号块级作用域
来源：http://qxv.xingfuxueyuan.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://cvr.jinqigfzy.top

C#:   块级作用域
来源：http://xaf.ybcxt.top

[C11] 模块导入与导出
来源：http://wup.jinghuilouyu.cn

Py:   from module import func
来源：http://cif.hnqzz.top

PHP:  require "file.php";  或 use App\Service;
来源：http://pfa.gotoacloud.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://yjj.tian-w.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://pzt.0kj1m.cn

Java: import java.util.List;
来源：http://ckf.jinqigfzy.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hcr.zhengqikj.top

Ruby: require "json"; require_relative "./util"
来源：http://kuj.quarkkingdee.top

C#:   using System.Text;
来源：http://qgr.havefunace.top

[C12] 立即执行函数 IIFE
来源：http://crf.uphjek.com

Py:   (lambda: print("run"))()
来源：http://znh.daxiang520.top

PHP:  (function () { echo "run"; })();
来源：http://urq.fzhhl.top

JS:   (() => { console.log("run"); })();
来源：http://vof.cucudq.cn

TS:   (() => { console.log("run"); })();
来源：http://olp.fengsongda.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mpf.cashguo.top

Go:   func() { fmt.Println("run") }()
来源：http://zob.guowangkeji.top

Ruby: -> { puts "run" }.call
来源：http://foo.ehwqpu.com

C#:   // 无 IIFE：用静态构造函数
来源：http://mbw.sxryk.cn

[C13] 类型声明 / 类型注解
来源：http://alo.c1oappe.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://jpl.jinghuilouyu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kbq.hywenlv.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mut.xinyue.icu

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://khw.havefunace.top

Java: int add(int a, int b) { return a + b; }
来源：http://lah.dashuyun.cn

Go:   func add(a, b int) int
来源：http://mzx.jianghu66.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://qeo.0kj1m.cn

C#:   int Add(int a, int b) => a + b;
来源：http://sbu.zdbjq.cn

[C14] 泛型函数
来源：http://rzv.ydjk.org.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://dei.sufxvd.cn

PHP:  // 无泛型
来源：http://ogo.316326.xyz

JS:   // 无泛型
来源：http://vlm.cucudq.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://zql.nwbrower.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wtc.haohaochexian.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://erx.jinqigufen.top

Ruby: # 无泛型
来源：http://cfc.hammf.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://zmt.zdbjq.cn

[C15] 解构 / 展开参数
来源：http://gml.zhongyouzk.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://nik.sysykeji.top

PHP:  [$a, $b] = $pair;
来源：http://agd.cashguo.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xeu.yueranfly.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hhs.yj20258.top

Java: // 无解构
来源：http://xcq.bbcook.cn

Go:   // 无解构
来源：http://okq.tianlin.xyz

Ruby: a, b = pair
来源：http://ynk.hcnkem.com

C#:   var (a, b) = pair;
来源：http://cnc.yongpay.top

[C16] 函数 / 方法重载
来源：http://lsr.ybcxt.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vyb.yonumen.top

PHP:  // 无重载
来源：http://mlf.hesvh.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://obt.xingfuxueyuan.xyz

TS:   // 用联合类型或重载签名声明
来源：http://gfy.hammf.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://vxy.havefunace.top

Go:   // 无重载：用不同函数名
来源：http://vda.zhongyouzk.top

Ruby: # 无重载：靠动态参数
来源：http://cry.dianchejie.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://rtw.yonumen.top

================================================================================
来源：http://cwd.epnwcf.com

D. 数组 / 列表 / 集合
来源：http://xls.guowangkeji.top

================================================================================
来源：http://ctb.chenlongwang.top

[D01] 创建数组 / 列表
来源：http://ufe.jianghu66.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://zpv.0kj1m.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ufn.zhiwuduotai.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://sev.chenlongwang.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://kio.sweek.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://gma.zycfv.cn

Go:   arr := []int{1, 2, 3}
来源：http://qww.mhx1999.top

Ruby: arr = [1, 2, 3]
来源：http://wzf.aizwys.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://thv.cashguo.top

[D02] 追加元素到末尾
来源：http://wui.sjlbkw.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://oqp.yvedp.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://rug.jinyuanbaomall.cn

JS:   arr.push(4);
来源：http://zzr.sxryk.cn

TS:   arr.push(4);
来源：http://csd.hnqzz.top

Java: list.add(4);
来源：http://hvw.hnxiangtu.top

Go:   arr = append(arr, 4)
来源：http://fej.9152youxi.cn

Ruby: arr << 4; arr.push(5)
来源：http://kok.jqgfzy.top

C#:   list.Add(4);
来源：http://sjd.zhijiandao.cn

[D03] 在指定位置插入元素
来源：http://qaf.wangshuangyany.cn

Py:   arr.insert(0, 0)
来源：http://chu.chenlongwang.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://nmh.jianghu66.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://tmc.zhongyouzk.top

TS:   arr.splice(0, 0, 0);
来源：http://qau.jyoumei.cn

Java: list.add(0, 0);
来源：http://vrc.jinghuilouyu.cn

Go:   arr = append([]int{0}, arr...)
来源：http://nnh.andypj.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://gdf.hammf.cn

C#:   list.Insert(0, 0);
来源：http://bgk.jinqigufen.top

[D04] 删除元素
来源：http://tjc.fengsongda.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://fyg.yanxiufei.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://lxy.xingfuxueyuan.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xaj.ctjpmb.com

TS:   arr.splice(0, 1);
来源：http://gxd.zhijiandao.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ikq.xziqi.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://cvy.meibo888.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://bjb.yanxiufei.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://tae.yonumen.top

[D05] 访问与修改元素
来源：http://gfr.dianchejie.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://vyi.ywan-chungtsiang.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wxs.chenlongwang.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://nhi.hysaishi.cn

TS:   arr[0]; arr.at(-1);
来源：http://aab.hfpthk.cn

Java: list.get(0); list.set(0, 9);
来源：http://wbx.redwolf501.top

Go:   arr[0]; arr[0] = 9
来源：http://xsi.pycfn.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://oeg.fanxiaobao.xyz

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ihk.zycfv.cn

[D06] 数组长度
来源：http://aqg.cqqwz.cn

Py:   len(arr)
来源：http://myl.sysykeji.top

PHP:  count($arr);
来源：http://zsu.yangfankeji.com

JS:   arr.length
来源：http://ceu.yueranfly.top

TS:   arr.length
来源：http://fve.tianlin.xyz

Java: list.size();
来源：http://etq.gaohongyu789.top

Go:   len(arr)
来源：http://vfr.fzhhl.top

Ruby: arr.length; arr.size
来源：http://lsp.guannengcc.top

C#:   list.Count;
来源：http://ksz.yongpay.top

[D07] 切片 / 取子数组
来源：http://gvl.guannengcc.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wns.cucudq.cn

PHP:  array_slice($arr, 1, 3);
来源：http://prf.hywenlv.cn

JS:   arr.slice(1, 4);
来源：http://osa.yj202588.top

TS:   arr.slice(1, 4);
来源：http://xvd.jinqigfzy.top

Java: list.subList(1, 4);
来源：http://oaf.chenlongwang.top

Go:   arr[1:4]
来源：http://ztp.zhixingplan.top

Ruby: arr[1, 3]
来源：http://ape.zhaomingkeji.xyz

C#:   list.GetRange(1, 3);
来源：http://ans.sjlbkw.cn

[D08] 合并两个数组
来源：http://msa.yvedp.cn

Py:   a + b;  a.extend(b)
来源：http://xic.jinqigfzy.top

PHP:  array_merge($a, $b);
来源：http://mqw.ehwqpu.com

JS:   [...a, ...b];  a.concat(b);
来源：http://iix.chenzaomai.com

TS:   [...a, ...b];
来源：http://szj.zhengqikj.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://kpx.feifeiyinyue.top

Go:   append(a, b...)
来源：http://crg.jinqigufen.top

Ruby: a + b;  a.concat(b)
来源：http://szb.havefunace.top

C#:   a.Concat(b).ToList()
来源：http://dvk.ywan-chungtsiang.top

[D09] 排序（升序）
来源：http://qlm.jqgufenzy.top

Py:   sorted(arr);  arr.sort()
来源：http://ohw.shanyushiyangtech.top


<!-- 参考信息 -->