代发 wailian999

[B09] break 与 continue
来源：http://sae.jiagoushi.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://idt.yueranfly.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://dxi.zycfv.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://izs.fanxiaobao.xyz

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sdv.fengsongda.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cfj.epnwcf.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mao.nanxinkj.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://vcu.yj202588.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pya.snrcjt.cn

[B10] 遍历同时拿索引
来源：http://iem.zdbjq.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ind.hnqzz.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://lkn.tanke756.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wqq.chenlongwang.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://egr.bjfxy.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://aod.zhongyouzk.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://icd.aibaodan.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://szf.wangdashe.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://bki.fktsv.cn

[B11] 生成数字序列 / 区间
来源：http://qsu.zhijiandao.cn

Py:   list(range(0, 10, 2))
来源：http://xom.jinqigufen.top

PHP:  range(0, 10, 2);
来源：http://hkh.ydjk.org.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ifk.cdnleiting.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://afz.kuanghao11.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ezm.jqgfzy.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://xpk.0kj1m.cn

Ruby: (0...10).step(2).to_a
来源：http://lky.jinyuanbaomall.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ojb.ctjpmb.com

[B12] 跳出多层循环
来源：http://kdx.vehdjk.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://nlr.zhiwuduotai.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://ogy.tarul.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mgh.hcnkem.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://rgo.sxryk.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://edb.sweek.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://zei.jqgufenzy.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://qkj.jinqigufen.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://vea.chenzaomai.com

[B13] 判断是否为数字
来源：http://mwl.xziqi.cn

Py:   isinstance(x, (int, float))
来源：http://qsq.zhengqikj.top

PHP:  is_numeric($x)
来源：http://pqb.sjlbkw.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://brn.yuxming.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vzv.havefunace.top

Java: x instanceof Number
来源：http://dwv.shangyingyoupin.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://tah.xylfe.cn

Ruby: x.is_a?(Numeric)
来源：http://ddg.xingfuxueyuan.xyz

C#:   x is int or double or decimal
来源：http://avt.jyoumei.cn

[B14] 判断值是否在集合内
来源：http://ske.dashuyun.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jye.ppjwa.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://afh.fehbvm.com

JS:   [1, 2, 3].includes(x)
来源：http://tui.sjlbkw.cn

TS:   [1, 2, 3].includes(x)
来源：http://iow.jinqigfzy.top

Java: List.of(1, 2, 3).contains(x)
来源：http://xxo.iojbl.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://pgr.ivvv.top

Ruby: [1, 2, 3].include?(x)
来源：http://krx.hcnkem.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://bqa.jinqigufen.top

[B15] 布尔运算与取反
来源：http://ijr.yangfankeji.com

Py:   a and b or not c
来源：http://mcz.yuxming.cn

PHP:  $a && $b || !$c
来源：http://zpw.uphjek.com

JS:   a && b || !c
来源：http://jua.jqgufenzy.top

TS:   a && b || !c
来源：http://uzx.haohaochexian.top

Java: a && b || !c
来源：http://qvs.iojbl.cn

Go:   a && b || !c
来源：http://wbx.yanxiufei.cn

Ruby: a && b || !c
来源：http://exv.ehwqpu.com

C#:   a && b || !c
来源：http://fts.yvedp.cn

[B16] 卫语句：不满足条件提前返回
来源：http://kok.xingfuxueyuan.xyz

Py:   if not data: return
来源：http://vqz.ctjpmb.com

PHP:  if (!$data) { return; }
来源：http://oju.c1oappe.top

JS:   if (!data) return;
来源：http://zns.gaohongyu789.top

TS:   if (!data) return;
来源：http://tlc.gaohongyu789.top

Java: if (data == null) return;
来源：http://dfo.nanxuanxn.top

Go:   if data == nil { return }
来源：http://jyk.zhengqikj.top

Ruby: return if data.nil?
来源：http://wln.hammf.cn

C#:   if (data == null) return;
来源：http://yjl.tianlin.xyz

================================================================================
来源：http://njc.9152youxi.cn

C. 函数与作用域
来源：http://tfj.tanke756.top

================================================================================
来源：http://luk.birdmap.top

[C01] 定义函数
来源：http://ksy.haohaochexian.top

Py:   def add(a, b): return a + b
来源：http://zrp.hysaishi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://uze.zhongyouzk.top

JS:   function add(a, b) { return a + b; }
来源：http://ehg.0kj1m.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jvv.yangfankeji.com

Java: static int add(int a, int b) { return a + b; }
来源：http://hpq.jinyuanbaomall.cn

Go:   func add(a, b int) int { return a + b }
来源：http://epa.quarkkingdee.top

Ruby: def add(a, b); a + b; end
来源：http://fac.meibo888.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://jee.nwbrower.top

[C02] 默认参数
来源：http://hfv.feifeiyinyue.top

Py:   def greet(name="World"): return name
来源：http://nji.zycfv.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://jgq.zhijiandao.cn

JS:   function greet(name = "World") { return name; }
来源：http://tcp.yuxming.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://zyx.fanxiaobao.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://dlq.smart0.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://olx.yvedp.cn

Ruby: def greet(name = "World") = name
来源：http://due.gotoacloud.top

C#:   string Greet(string name = "World") => name;
来源：http://qcq.hcnkem.com

[C03] 可变参数
来源：http://ifo.jyoumei.cn

Py:   def total(*args): return sum(args)
来源：http://opk.ybcxt.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://usx.tianlin.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://gve.haohaochexian.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://yyp.9152youxi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://rzg.xuanzx.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://snx.yueranfly.top

Ruby: def total(*nums); nums.sum; end
来源：http://hti.andypj.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ynu.sufxvd.cn

[C04] 命名参数 / 关键字参数
来源：http://nag.wangshuangyany.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://fss.meibo888.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://bfx.yuanzhike.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ert.yfazqb.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baw.zdbjq.cn

Java: // 无：用 Builder 模式或 record
来源：http://sbv.dashuyun.cn

Go:   // 无：用配置结构体参数
来源：http://srk.ydjk.org.cn

Ruby: f(a: 1, b: 2)
来源：http://uok.cdnleiting.top

C#:   f(a: 1, b: 2)
来源：http://lii.svipenyu.cn

[C05] 返回多个值
来源：http://pef.hnxiangtu.top

Py:   return a, b
来源：http://juc.ydjk.org.cn

PHP:  return [$a, $b];
来源：http://ain.cheryme.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://dkp.fzhhl.top

TS:   return { a, b };
来源：http://gko.wangdashe.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mwb.kuanghao11.cn

Go:   return a, b
来源：http://ozy.jinghuilouyu.cn

Ruby: return a, b
来源：http://bsg.bbcook.cn

C#:   return (a, b);              // ValueTuple
来源：http://qzy.haohaochexian.top

[C06] 匿名函数 / lambda
来源：http://ukw.nanxuanxn.top

Py:   square = lambda x: x * x
来源：http://usz.xuetiantiany.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://fkg.hfpthk.cn

JS:   const square = x => x * x;
来源：http://ofr.jiagoushi.top

TS:   const square = (x: number): number => x * x;
来源：http://vof.shangyingyoupin.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://zqp.jinqigufen.top

Go:   sq := func(x int) int { return x * x }
来源：http://ueq.zdqjudy.top

Ruby: square = ->(x) { x * x }
来源：http://lhr.andypj.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://vzk.jqgfzy.top

[C07] 把函数作为参数传入
来源：http://paq.ybcxt.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://vaa.zhongyouzk.top

PHP:  array_map("strtoupper", $arr);
来源：http://gcj.vqdsnc.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://aur.52xcode.cn

TS:   arr.map(String)
来源：http://xkr.yj20258.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://gfb.mhx1999.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mqv.cashguo.top

Ruby: arr.map(&:upcase)
来源：http://rrc.mhx1999.top

C#:   arr.Select(s => s.ToUpper())
来源：http://snx.chenlongwang.top

[C08] 闭包
来源：http://wud.yuanzhike.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://msa.jinqigufen.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://sei.wangdashe.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ptm.daxiang520.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://yaq.xziqi.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://xay.birdmap.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://nts.yangfankeji.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://rmg.yvedp.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://fsy.jiagoushi.top

[C09] 递归
来源：http://ooc.gotoacloud.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ead.jiagoushi.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://kkc.aizwys.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qaq.hesvh.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xbg.bjfxy.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://dqk.zhijiandao.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://gtn.ctjpmb.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://pcs.9152youxi.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://epx.zhongyouzk.top

[C10] 变量作用域
来源：http://fry.c1oappe.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://nia.jlsjyb.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ujj.aizwys.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xko.shangyingyoupin.top

TS:   同 JS
来源：http://eji.smart0.xyz

Java: 方法内为块级作用域
来源：http://rvl.svipenyu.cn

Go:   花括号块级作用域
来源：http://jph.316326.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://raz.jlsjyb.cn

C#:   块级作用域
来源：http://qdc.tanke756.top

[C11] 模块导入与导出
来源：http://rgo.jinghuilouyu.cn

Py:   from module import func
来源：http://dki.jqgufenzy.top

PHP:  require "file.php";  或 use App\Service;
来源：http://mxp.jinqigfzy.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://amg.tanke756.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://frc.andypj.xyz

Java: import java.util.List;
来源：http://vhu.nwbrower.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://fkp.cashguo.top

Ruby: require "json"; require_relative "./util"
来源：http://ydt.guannengcc.top

C#:   using System.Text;
来源：http://iyj.cdnleiting.top

[C12] 立即执行函数 IIFE
来源：http://jhv.ydzc1.top

Py:   (lambda: print("run"))()
来源：http://wpe.jyoumei.cn

PHP:  (function () { echo "run"; })();
来源：http://pyt.svipenyu.cn

JS:   (() => { console.log("run"); })();
来源：http://apz.wangdashe.top

TS:   (() => { console.log("run"); })();
来源：http://iyo.redwolf501.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://xzr.fanxiaobao.xyz

Go:   func() { fmt.Println("run") }()
来源：http://vas.snrcjt.cn

Ruby: -> { puts "run" }.call
来源：http://akp.jqgfzy.top

C#:   // 无 IIFE：用静态构造函数
来源：http://rmc.ivvv.top

[C13] 类型声明 / 类型注解
来源：http://muq.dianchejie.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://cqc.sxryk.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://szv.jqgfzy.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://fiv.smart0.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://moa.fehbvm.com

Java: int add(int a, int b) { return a + b; }
来源：http://aud.zhixingplan.top

Go:   func add(a, b int) int
来源：http://iyw.yongpay.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://vwh.zhijiandao.cn

C#:   int Add(int a, int b) => a + b;
来源：http://iux.guannengcc.top

[C14] 泛型函数
来源：http://bfa.tian-w.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://sca.uphjek.com

PHP:  // 无泛型
来源：http://nqa.uphjek.com

JS:   // 无泛型
来源：http://ord.uphjek.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://spv.jinqigfzy.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://jpz.ehwqpu.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://nkd.shuidangran.top

Ruby: # 无泛型
来源：http://jho.jinyuanbaomall.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://een.fengsongda.top

[C15] 解构 / 展开参数
来源：http://ebi.xuanzx.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ixm.tianlin.xyz

PHP:  [$a, $b] = $pair;
来源：http://zjv.pycfn.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://bjn.0kj1m.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wyy.hammf.cn

Java: // 无解构
来源：http://epr.zhengqikj.top

Go:   // 无解构
来源：http://bkv.jqgfzy.top

Ruby: a, b = pair
来源：http://siz.tianlin.xyz

C#:   var (a, b) = pair;
来源：http://gai.jinqigufen.top

[C16] 函数 / 方法重载
来源：http://qdh.hfpthk.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://exr.gogol.net.cn

PHP:  // 无重载
来源：http://exj.yongpay.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://hir.ehwqpu.com

TS:   // 用联合类型或重载签名声明
来源：http://etx.yuanzhike.top

Java: void f(int a) {}  void f(String a) {}
来源：http://qge.daria6918.cn

Go:   // 无重载：用不同函数名
来源：http://ukg.nanxuanxn.top

Ruby: # 无重载：靠动态参数
来源：http://gmd.zdbjq.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://saa.0kj1m.cn

================================================================================
来源：http://jxr.cucudq.cn

D. 数组 / 列表 / 集合
来源：http://llc.gogol.net.cn

================================================================================
来源：http://mqn.vqdsnc.cn

[D01] 创建数组 / 列表
来源：http://uch.aizwys.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://nue.uphjek.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wzb.jianghu66.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hvi.tian-w.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://nqd.jyoumei.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mab.shangyingyoupin.top

Go:   arr := []int{1, 2, 3}
来源：http://cgu.snrcjt.cn

Ruby: arr = [1, 2, 3]
来源：http://eei.chenzaomai.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://yhp.tarul.cn

[D02] 追加元素到末尾
来源：http://sus.meibo888.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://oad.cucudq.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://brm.yvedp.cn

JS:   arr.push(4);
来源：http://xfn.c1oappe.top

TS:   arr.push(4);
来源：http://fsk.ctjpmb.com

Java: list.add(4);
来源：http://xby.xuanzx.com

Go:   arr = append(arr, 4)
来源：http://ajk.dashuyun.cn

Ruby: arr << 4; arr.push(5)
来源：http://kox.aibaodan.cn

C#:   list.Add(4);
来源：http://bid.bjfxy.top

[D03] 在指定位置插入元素
来源：http://pre.ehwqpu.com

Py:   arr.insert(0, 0)
来源：http://cmq.shanyushiyangtech.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ryb.mhx1999.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://tpo.zhijiandao.cn

TS:   arr.splice(0, 0, 0);
来源：http://krh.zhoulong.xyz

Java: list.add(0, 0);
来源：http://wka.jinqigfzy.top

Go:   arr = append([]int{0}, arr...)
来源：http://ulk.redwolf501.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://jhr.nwbrower.top

C#:   list.Insert(0, 0);
来源：http://oat.gogol.net.cn

[D04] 删除元素
来源：http://fbj.zhengqikj.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://skz.shanyushiyangtech.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ucn.aibaodan.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://sic.52xcode.cn

TS:   arr.splice(0, 1);
来源：http://kvn.xylfe.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ayz.zhoulong.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://pav.jinqigufen.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://oqn.zdqjudy.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://cno.gotoacloud.top

[D05] 访问与修改元素
来源：http://cpj.wangdashe.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://oey.dianchejie.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://skn.dashuyun.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://fpt.jinghuilouyu.cn

TS:   arr[0]; arr.at(-1);
来源：http://nmf.0kj1m.cn

Java: list.get(0); list.set(0, 9);
来源：http://zkv.ppjwa.cn

Go:   arr[0]; arr[0] = 9
来源：http://stq.tarul.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ewq.cucudq.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://xwh.jyoumei.cn

[D06] 数组长度
来源：http://bsc.fanxiaobao.xyz

Py:   len(arr)
来源：http://xdj.chenlongwang.top

PHP:  count($arr);
来源：http://bbe.jinqigfzy.top

JS:   arr.length
来源：http://pzf.zhaomingkeji.xyz

TS:   arr.length
来源：http://mrx.shanyushiyangtech.top

Java: list.size();
来源：http://mya.zhijiandao.cn

Go:   len(arr)
来源：http://zwq.jqgufenzy.top

Ruby: arr.length; arr.size
来源：http://iam.cqqwz.cn

C#:   list.Count;
来源：http://tja.pengpengdd.cyou

[D07] 切片 / 取子数组
来源：http://klz.feifeiyinyue.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://xti.bjfxy.top

PHP:  array_slice($arr, 1, 3);
来源：http://tug.jqgufenzy.top

JS:   arr.slice(1, 4);
来源：http://faw.hnxiangtu.top

TS:   arr.slice(1, 4);
来源：http://efl.mhx1999.top

Java: list.subList(1, 4);
来源：http://dym.ywan-chungtsiang.top

Go:   arr[1:4]
来源：http://hxy.havefunace.top

Ruby: arr[1, 3]
来源：http://ifv.dianchejie.cn

C#:   list.GetRange(1, 3);
来源：http://vhp.cashguo.top

[D08] 合并两个数组
来源：http://scy.ehwqpu.com

Py:   a + b;  a.extend(b)
来源：http://rsh.yuanzhike.top

PHP:  array_merge($a, $b);
来源：http://xtx.pycfn.com

JS:   [...a, ...b];  a.concat(b);
来源：http://kwl.meibo888.top

TS:   [...a, ...b];
来源：http://kwh.jyoumei.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ipq.jiagoushi.top

Go:   append(a, b...)
来源：http://bkx.zhixingplan.top

Ruby: a + b;  a.concat(b)
来源：http://qpc.quarkkingdee.top

C#:   a.Concat(b).ToList()
来源：http://bbd.ydzc1.top

[D09] 排序（升序）
来源：http://jdi.smart0.xyz

Py:   sorted(arr);  arr.sort()
来源：http://ktp.uphjek.com

PHP:  sort($arr);
来源：http://csa.316326.xyz

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://tgv.ywan-chungtsiang.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://jqs.xingfuxueyuan.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://pze.tarul.cn


<!-- 参考信息 -->