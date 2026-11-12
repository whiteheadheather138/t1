代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://ojl.tanke756.top

PHP:  do { $i++; } while ($i < 10);
来源：http://xje.ydjk.org.cn

JS:   do { i++; } while (i < 10);
来源：http://kdm.ppjwa.cn

TS:   do { i++; } while (i < 10);
来源：http://vkf.52xcode.cn

Java: do { i++; } while (i < 10);
来源：http://fdl.epnwcf.com

Go:   for { i++; if i >= 10 { break } }
来源：http://hvv.zdbjq.cn

Ruby: begin; i += 1; end while i < 10
来源：http://hwv.xziqi.cn

C#:   do { i++; } while (i < 10);
来源：http://trb.sxryk.cn

[B09] break 与 continue
来源：http://oii.ywan-chungtsiang.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://nyj.yj20258888.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://gnu.meibo888.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://iif.meibo888.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tlh.zhongyouzk.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xit.c1oappe.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://pbv.gaohongyu789.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://aqt.jqgfzy.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://grt.jyoumei.cn

[B10] 遍历同时拿索引
来源：http://uxx.ehwqpu.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://sjz.ywan-chungtsiang.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wzb.vqdsnc.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://twt.hammf.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://vna.ydjk.org.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://rnn.hesvh.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://oci.aibaodan.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://sps.yfazqb.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://jwo.feifeiyinyue.top

[B11] 生成数字序列 / 区间
来源：http://ddo.yuanzhike.top

Py:   list(range(0, 10, 2))
来源：http://ffi.jlsjyb.cn

PHP:  range(0, 10, 2);
来源：http://hkj.c1oappe.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vlz.cashguo.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hgg.iojbl.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://xtm.iojbl.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ktl.hongshengwenyu.top

Ruby: (0...10).step(2).to_a
来源：http://uki.0kj1m.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://gwb.hysaishi.cn

[B12] 跳出多层循环
来源：http://puu.ppjwa.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://uov.zhixingplan.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://fnj.sxryk.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://egi.wangshuangyany.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://jyu.aibaodan.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://foa.yongpay.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://rht.pengpengdd.cyou

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://znk.c1oappe.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://fky.cashguo.top

[B13] 判断是否为数字
来源：http://pqz.andypj.xyz

Py:   isinstance(x, (int, float))
来源：http://nlb.bjfxy.top

PHP:  is_numeric($x)
来源：http://uhm.smart0.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lba.zhoulong.xyz

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://oyh.shuidangran.top

Java: x instanceof Number
来源：http://yyr.hysaishi.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ogj.tarul.cn

Ruby: x.is_a?(Numeric)
来源：http://dgx.hongshengwenyu.top

C#:   x is int or double or decimal
来源：http://fcr.ppjwa.cn

[B14] 判断值是否在集合内
来源：http://bta.zhoulong.xyz

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://yab.fanxiaobao.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://jut.yj202588.top

JS:   [1, 2, 3].includes(x)
来源：http://uif.gaohongyu789.top

TS:   [1, 2, 3].includes(x)
来源：http://zar.jlsjyb.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://laj.yj20258888.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hxr.tanke756.top

Ruby: [1, 2, 3].include?(x)
来源：http://exj.sysykeji.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://suu.vqdsnc.cn

[B15] 布尔运算与取反
来源：http://kgw.jqgufenzy.top

Py:   a and b or not c
来源：http://tis.ydzc1.top

PHP:  $a && $b || !$c
来源：http://tgm.shzxlz.cn

JS:   a && b || !c
来源：http://dpa.yuxming.cn

TS:   a && b || !c
来源：http://riv.shanyushiyangkeji.top

Java: a && b || !c
来源：http://mwm.uphjek.com

Go:   a && b || !c
来源：http://oyj.jiagoushi.top

Ruby: a && b || !c
来源：http://mxa.ybcxt.top

C#:   a && b || !c
来源：http://qnm.kuanghao11.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ink.tarul.cn

Py:   if not data: return
来源：http://fwv.jlsjyb.cn

PHP:  if (!$data) { return; }
来源：http://cnr.cdnleiting.top

JS:   if (!data) return;
来源：http://vmp.jqgfzy.top

TS:   if (!data) return;
来源：http://qto.zhengqikj.top

Java: if (data == null) return;
来源：http://rez.ybcxt.top

Go:   if data == nil { return }
来源：http://dwk.fengsongda.top

Ruby: return if data.nil?
来源：http://pqo.tanke756.top

C#:   if (data == null) return;
来源：http://hzx.hywenlv.cn

================================================================================
来源：http://fft.guannengcc.top

C. 函数与作用域
来源：http://rwg.redwolf501.top

================================================================================
来源：http://ftz.nwbrower.top

[C01] 定义函数
来源：http://rvf.fengsongda.top

Py:   def add(a, b): return a + b
来源：http://xhl.xuetiantiany.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vbh.andypj.xyz

JS:   function add(a, b) { return a + b; }
来源：http://oiv.52xcode.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ncb.dashuyun.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://usw.cdnleiting.top

Go:   func add(a, b int) int { return a + b }
来源：http://lbc.cucudq.cn

Ruby: def add(a, b); a + b; end
来源：http://psh.yueranfly.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://sru.c1oappe.top

[C02] 默认参数
来源：http://hdv.aizwys.cn

Py:   def greet(name="World"): return name
来源：http://uyb.jinghuilouyu.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://pgf.nanxinkj.top

JS:   function greet(name = "World") { return name; }
来源：http://rff.dashuyun.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://nhy.redwolf501.top

Java: // 无默认参数：方法重载或 Optional
来源：http://ela.aibaodan.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ymk.bjfxy.top

Ruby: def greet(name = "World") = name
来源：http://tpl.epnwcf.com

C#:   string Greet(string name = "World") => name;
来源：http://ncn.zhoulong.xyz

[C03] 可变参数
来源：http://nxn.hysaishi.cn

Py:   def total(*args): return sum(args)
来源：http://wyn.redwolf501.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xhg.zhiwuduotai.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://gno.jiagoushi.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://cue.tarul.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://edh.cucudq.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://pqu.hywenlv.cn

Ruby: def total(*nums); nums.sum; end
来源：http://nkd.tian-w.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://nij.chenzaomai.com

[C04] 命名参数 / 关键字参数
来源：http://qoj.shangyingyoupin.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://tmi.nwbrower.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xpi.sufxvd.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://rfc.ywan-chungtsiang.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://fvv.ppjwa.cn

Java: // 无：用 Builder 模式或 record
来源：http://ijg.cucudq.cn

Go:   // 无：用配置结构体参数
来源：http://lyu.yvedp.cn

Ruby: f(a: 1, b: 2)
来源：http://fif.shanyushiyangkeji.top

C#:   f(a: 1, b: 2)
来源：http://bvh.fengsongda.top

[C05] 返回多个值
来源：http://mii.hammf.cn

Py:   return a, b
来源：http://zpk.xuetiantiany.cn

PHP:  return [$a, $b];
来源：http://puo.jyoumei.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://kth.daria6918.cn

TS:   return { a, b };
来源：http://ewv.yj20258.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://pcs.birdmap.top

Go:   return a, b
来源：http://suy.bbcook.cn

Ruby: return a, b
来源：http://ozh.birdmap.top

C#:   return (a, b);              // ValueTuple
来源：http://utr.ivvv.top

[C06] 匿名函数 / lambda
来源：http://mnc.daria6918.cn

Py:   square = lambda x: x * x
来源：http://kyg.yvedp.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://rfn.52xcode.cn

JS:   const square = x => x * x;
来源：http://rmf.fengsongda.top

TS:   const square = (x: number): number => x * x;
来源：http://ioc.hongshengwenyu.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://yqy.yj20258888.top

Go:   sq := func(x int) int { return x * x }
来源：http://cav.tanke756.top

Ruby: square = ->(x) { x * x }
来源：http://hzy.sufxvd.cn

C#:   Func<int, int> square = x => x * x;
来源：http://mlk.jianghu66.top

[C07] 把函数作为参数传入
来源：http://byi.ybcxt.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://gjm.cashguo.top

PHP:  array_map("strtoupper", $arr);
来源：http://mtw.316326.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://nqr.jinqigufen.top

TS:   arr.map(String)
来源：http://iyp.gaohongyu789.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://guh.aizwys.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://dsx.zycfv.cn

Ruby: arr.map(&:upcase)
来源：http://gju.hysaishi.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://hux.zhijiandao.cn

[C08] 闭包
来源：http://uoq.yj20258888.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ibm.aibaodan.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://vzb.jqgfzy.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vqr.meibo888.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://yoe.meibo888.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://tjq.yongpay.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wth.shuidangran.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://shy.yueranfly.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wrq.redwolf501.top

[C09] 递归
来源：http://tcs.wangshuangyany.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://gcl.cashguo.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://pjg.tarul.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gvb.gotoacloud.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rxl.zdbjq.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://bgl.shuidangran.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://tvk.hnqzz.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wkq.guannengcc.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://irq.hnxiangtu.top

[C10] 变量作用域
来源：http://pxf.jinqigufen.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://jrs.shangyingyoupin.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://lvt.epnwcf.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://obk.snrcjt.cn

TS:   同 JS
来源：http://qpb.ppjwa.cn

Java: 方法内为块级作用域
来源：http://ogt.hcnkem.com

Go:   花括号块级作用域
来源：http://pcl.jinqigfzy.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://aqz.shzxlz.cn

C#:   块级作用域
来源：http://mqy.redwolf501.top

[C11] 模块导入与导出
来源：http://nzi.zhijiandao.cn

Py:   from module import func
来源：http://kup.yfazqb.com

PHP:  require "file.php";  或 use App\Service;
来源：http://nkx.xingfuxueyuan.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://znl.cucudq.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://iom.guowangkeji.top

Java: import java.util.List;
来源：http://gqd.tarul.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://pcy.xziqi.cn

Ruby: require "json"; require_relative "./util"
来源：http://fkh.shangyingyoupin.top

C#:   using System.Text;
来源：http://gxh.ehwqpu.com

[C12] 立即执行函数 IIFE
来源：http://ces.feifeiyinyue.top

Py:   (lambda: print("run"))()
来源：http://qkp.cucudq.cn

PHP:  (function () { echo "run"; })();
来源：http://vqm.nanxuanxn.top

JS:   (() => { console.log("run"); })();
来源：http://jyi.jqgufenzy.top

TS:   (() => { console.log("run"); })();
来源：http://hzf.xinyue.icu

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://sgz.ydzc1.top

Go:   func() { fmt.Println("run") }()
来源：http://cyx.uphjek.com

Ruby: -> { puts "run" }.call
来源：http://lkh.yuxming.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://zxs.sxryk.cn

[C13] 类型声明 / 类型注解
来源：http://wil.hnqzz.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://epe.redwolf501.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hrm.jianghu66.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wjh.sjlbkw.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wig.tanke756.top

Java: int add(int a, int b) { return a + b; }
来源：http://qsc.yongpay.top

Go:   func add(a, b int) int
来源：http://fpg.haohaochexian.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://onf.cashguo.top

C#:   int Add(int a, int b) => a + b;
来源：http://xyz.daria6918.cn

[C14] 泛型函数
来源：http://tps.nanxuanxn.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://eaz.jinyuanbaomall.cn

PHP:  // 无泛型
来源：http://ufh.daxiang520.top

JS:   // 无泛型
来源：http://pvz.shzxlz.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://piw.shuidangran.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://szj.ydzc1.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://eho.ywan-chungtsiang.top

Ruby: # 无泛型
来源：http://scw.haohaochexian.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ucl.vehdjk.com

[C15] 解构 / 展开参数
来源：http://pla.shzxlz.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://oxb.nanxuanxn.top

PHP:  [$a, $b] = $pair;
来源：http://bcz.cqqwz.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hlp.xinyue.icu

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://kqi.daxiang520.top

Java: // 无解构
来源：http://slv.shuidangran.top

Go:   // 无解构
来源：http://cka.dashuyun.cn

Ruby: a, b = pair
来源：http://uqv.quarkkingdee.top

C#:   var (a, b) = pair;
来源：http://upa.sxryk.cn

[C16] 函数 / 方法重载
来源：http://yhv.ppjwa.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vlt.sysykeji.top

PHP:  // 无重载
来源：http://mlw.jqgfzy.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://haw.cucudq.cn

TS:   // 用联合类型或重载签名声明
来源：http://aqh.52xcode.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ack.jlsjyb.cn

Go:   // 无重载：用不同函数名
来源：http://ppy.hesvh.cn

Ruby: # 无重载：靠动态参数
来源：http://naj.gaohongyu789.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://mdq.daxiang520.top

================================================================================
来源：http://tau.uphjek.com

D. 数组 / 列表 / 集合
来源：http://pfy.ppjwa.cn

================================================================================
来源：http://bpm.tarul.cn

[D01] 创建数组 / 列表
来源：http://mli.52xcode.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ypv.zhixingplan.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://def.snrcjt.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://sra.sxryk.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://sjl.ydjk.org.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://vzw.epnwcf.com

Go:   arr := []int{1, 2, 3}
来源：http://rxg.kuanghao11.cn

Ruby: arr = [1, 2, 3]
来源：http://sjx.yj202588.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://deq.yongpay.top

[D02] 追加元素到末尾
来源：http://snj.snrcjt.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://swz.zhengqikj.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://bct.cashguo.top

JS:   arr.push(4);
来源：http://phc.aibaodan.cn

TS:   arr.push(4);
来源：http://zxl.jinyuanbaomall.cn

Java: list.add(4);
来源：http://hys.c1oappe.top

Go:   arr = append(arr, 4)
来源：http://jph.xingfuxueyuan.xyz

Ruby: arr << 4; arr.push(5)
来源：http://sdc.nwbrower.top

C#:   list.Add(4);
来源：http://dpz.hysaishi.cn

[D03] 在指定位置插入元素
来源：http://kxu.jinqigfzy.top

Py:   arr.insert(0, 0)
来源：http://wgt.yueranfly.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mnn.fengsongda.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://kdw.hesvh.cn

TS:   arr.splice(0, 0, 0);
来源：http://ree.hnqzz.top

Java: list.add(0, 0);
来源：http://dln.chenjidiqi.icu

Go:   arr = append([]int{0}, arr...)
来源：http://hio.0kj1m.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://iwy.xuanzx.com

C#:   list.Insert(0, 0);
来源：http://ext.zycfv.cn

[D04] 删除元素
来源：http://egd.xziqi.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://yba.tarul.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://tfg.bjfxy.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://nvq.zhijiandao.cn

TS:   arr.splice(0, 1);
来源：http://igs.havefunace.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wet.gotoacloud.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://gii.jinghuilouyu.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://dhx.kuanghao11.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://vfn.52xcode.cn

[D05] 访问与修改元素
来源：http://yqs.9152youxi.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://gie.jyoumei.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://kal.xuanzx.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://fgm.hongshengwenyu.top

TS:   arr[0]; arr.at(-1);
来源：http://fmc.yangfankeji.com

Java: list.get(0); list.set(0, 9);
来源：http://nrr.quarkkingdee.top

Go:   arr[0]; arr[0] = 9
来源：http://ytu.daxiang520.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://gys.ehwqpu.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://kkb.ctjpmb.com

[D06] 数组长度
来源：http://yat.svipenyu.cn

Py:   len(arr)
来源：http://qoj.kuanghao11.cn

PHP:  count($arr);
来源：http://cvx.zdbjq.cn

JS:   arr.length
来源：http://rcd.yanxiufei.cn

TS:   arr.length
来源：http://zqd.ywan-chungtsiang.top

Java: list.size();
来源：http://msm.hfpthk.cn

Go:   len(arr)
来源：http://blb.chenlongwang.top

Ruby: arr.length; arr.size
来源：http://cmv.jqgufenzy.top

C#:   list.Count;
来源：http://rcm.guannengcc.top

[D07] 切片 / 取子数组
来源：http://hha.iojbl.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://vmc.dashuyun.cn

PHP:  array_slice($arr, 1, 3);
来源：http://pfs.xuetiantiany.cn

JS:   arr.slice(1, 4);
来源：http://cve.yongpay.top

TS:   arr.slice(1, 4);
来源：http://czs.mhx1999.top

Java: list.subList(1, 4);
来源：http://mml.hnxiangtu.top

Go:   arr[1:4]
来源：http://nvq.zdqjudy.top

Ruby: arr[1, 3]
来源：http://nwr.zhiwuduotai.top

C#:   list.GetRange(1, 3);
来源：http://ogx.jiagoushi.top

[D08] 合并两个数组
来源：http://drs.cucudq.cn

Py:   a + b;  a.extend(b)
来源：http://noz.chenzaomai.com

PHP:  array_merge($a, $b);
来源：http://kja.jqgfzy.top

JS:   [...a, ...b];  a.concat(b);
来源：http://iyx.hammf.cn

TS:   [...a, ...b];
来源：http://iwd.guannengcc.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://sci.gaohongyu789.top

Go:   append(a, b...)
来源：http://ula.bjfxy.top


<!-- 参考信息 -->