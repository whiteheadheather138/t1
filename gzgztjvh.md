代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://fdb.jinyuanbaomall.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://inw.tarul.cn

JS:   do { i++; } while (i < 10);
来源：http://ikz.yj20258888.top

TS:   do { i++; } while (i < 10);
来源：http://onq.yj20258.top

Java: do { i++; } while (i < 10);
来源：http://ezt.uphjek.com

Go:   for { i++; if i >= 10 { break } }
来源：http://nls.ydjk.org.cn

Ruby: begin; i += 1; end while i < 10
来源：http://djo.chenlongwang.top

C#:   do { i++; } while (i < 10);
来源：http://uxj.shanyushiyangtech.top

[B09] break 与 continue
来源：http://grd.zycfv.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://fts.feifeiyinyue.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://xqw.gogol.net.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hpl.bjfxy.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kti.iojbl.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uwn.smart0.xyz

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://dme.andypj.xyz

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wgq.yj202588.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yxn.smart0.xyz

[B10] 遍历同时拿索引
来源：http://fyx.xziqi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://rjr.aizwys.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://gnm.kuanghao11.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://eov.shangyingyoupin.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://vwd.zhiwuduotai.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://pcj.xinyue.icu

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://zid.cdnleiting.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://kpy.ywan-chungtsiang.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://vvh.jlsjyb.cn

[B11] 生成数字序列 / 区间
来源：http://ngt.zdbjq.cn

Py:   list(range(0, 10, 2))
来源：http://eck.cdnleiting.top

PHP:  range(0, 10, 2);
来源：http://rop.xuetiantiany.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jzp.nwbrower.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ejk.guannengcc.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mue.ywan-chungtsiang.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ere.svipenyu.cn

Ruby: (0...10).step(2).to_a
来源：http://sci.wangdashe.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://aqj.ppjwa.cn

[B12] 跳出多层循环
来源：http://qlm.birdmap.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://tib.ydzc1.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://dti.fktsv.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://akk.jinqigufen.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ger.daxiang520.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://fvp.svipenyu.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://kec.yj202588.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://guz.sxryk.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hwl.hywenlv.cn

[B13] 判断是否为数字
来源：http://xuv.hysaishi.cn

Py:   isinstance(x, (int, float))
来源：http://gdo.316326.xyz

PHP:  is_numeric($x)
来源：http://ieh.pengpengdd.cyou

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gsp.tian-w.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ahs.snrcjt.cn

Java: x instanceof Number
来源：http://tsv.dashuyun.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://fgw.zhijiandao.cn

Ruby: x.is_a?(Numeric)
来源：http://gjs.shzxlz.cn

C#:   x is int or double or decimal
来源：http://jgg.ydzc1.top

[B14] 判断值是否在集合内
来源：http://usp.hywenlv.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://tzw.9152youxi.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://tgy.yanxiufei.cn

JS:   [1, 2, 3].includes(x)
来源：http://zif.epnwcf.com

TS:   [1, 2, 3].includes(x)
来源：http://vuv.jyoumei.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://kts.zhoulong.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://tfr.andypj.xyz

Ruby: [1, 2, 3].include?(x)
来源：http://bvu.shuidangran.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ebx.hnqzz.top

[B15] 布尔运算与取反
来源：http://szy.hongshengwenyu.top

Py:   a and b or not c
来源：http://wys.yonumen.top

PHP:  $a && $b || !$c
来源：http://mze.meibo888.top

JS:   a && b || !c
来源：http://zsk.jqgufenzy.top

TS:   a && b || !c
来源：http://rmz.cqqwz.cn

Java: a && b || !c
来源：http://upk.andypj.xyz

Go:   a && b || !c
来源：http://asg.mhx1999.top

Ruby: a && b || !c
来源：http://jnx.hcnkem.com

C#:   a && b || !c
来源：http://utx.chenzaomai.com

[B16] 卫语句：不满足条件提前返回
来源：http://qka.xylfe.cn

Py:   if not data: return
来源：http://nsu.shanyushiyangkeji.top

PHP:  if (!$data) { return; }
来源：http://ulc.xziqi.cn

JS:   if (!data) return;
来源：http://dmo.ybcxt.top

TS:   if (!data) return;
来源：http://gai.yj202588.top

Java: if (data == null) return;
来源：http://nvr.sufxvd.cn

Go:   if data == nil { return }
来源：http://zoy.cqqwz.cn

Ruby: return if data.nil?
来源：http://yit.ywan-chungtsiang.top

C#:   if (data == null) return;
来源：http://bpk.jqgufenzy.top

================================================================================
来源：http://mtu.hongshengwenyu.top

C. 函数与作用域
来源：http://khf.gzhubu.top

================================================================================
来源：http://jdv.guowangkeji.top

[C01] 定义函数
来源：http://prr.fehbvm.com

Py:   def add(a, b): return a + b
来源：http://blx.guowangkeji.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gib.0kj1m.cn

JS:   function add(a, b) { return a + b; }
来源：http://oki.zdbjq.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ego.vehdjk.com

Java: static int add(int a, int b) { return a + b; }
来源：http://lcc.zdqjudy.top

Go:   func add(a, b int) int { return a + b }
来源：http://you.snrcjt.cn

Ruby: def add(a, b); a + b; end
来源：http://uuo.hammf.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://tvt.gogol.net.cn

[C02] 默认参数
来源：http://eha.cdnleiting.top

Py:   def greet(name="World"): return name
来源：http://oqw.tianlin.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://ssu.ivvv.top

JS:   function greet(name = "World") { return name; }
来源：http://uec.xuanzx.com

TS:   function greet(name: string = "World") { return name; }
来源：http://mzh.jyoumei.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://tpb.birdmap.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://lbb.yuxming.cn

Ruby: def greet(name = "World") = name
来源：http://ylc.jinqigfzy.top

C#:   string Greet(string name = "World") => name;
来源：http://fwo.meibo888.top

[C03] 可变参数
来源：http://lel.gzhubu.top

Py:   def total(*args): return sum(args)
来源：http://ypa.hnqzz.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://iex.feifeiyinyue.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://vjb.hongshengwenyu.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ncr.vqdsnc.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hjp.yonumen.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://qvq.zhijiandao.cn

Ruby: def total(*nums); nums.sum; end
来源：http://bnx.hongshengwenyu.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ifx.pengpengdd.cyou

[C04] 命名参数 / 关键字参数
来源：http://pdw.pengpengdd.cyou

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://jjn.sufxvd.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://fkh.yuanzhike.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://lwj.xinyue.icu

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ohr.cqqwz.cn

Java: // 无：用 Builder 模式或 record
来源：http://agh.dianchejie.cn

Go:   // 无：用配置结构体参数
来源：http://nmh.haohaochexian.top

Ruby: f(a: 1, b: 2)
来源：http://jyi.bbcook.cn

C#:   f(a: 1, b: 2)
来源：http://asf.bbcook.cn

[C05] 返回多个值
来源：http://qyh.yongpay.top

Py:   return a, b
来源：http://fuk.feifeiyinyue.top

PHP:  return [$a, $b];
来源：http://prz.zhaomingkeji.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://pcj.yuanzhike.top

TS:   return { a, b };
来源：http://wri.cucudq.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://yie.yj20258888.top

Go:   return a, b
来源：http://eav.dianchejie.cn

Ruby: return a, b
来源：http://vpu.nanxuanxn.top

C#:   return (a, b);              // ValueTuple
来源：http://kru.hongshengwenyu.top

[C06] 匿名函数 / lambda
来源：http://vuo.fzhhl.top

Py:   square = lambda x: x * x
来源：http://mwv.zdqjudy.top

PHP:  $square = fn($x) => $x * $x;
来源：http://pzr.hnqzz.top

JS:   const square = x => x * x;
来源：http://nyy.cqqwz.cn

TS:   const square = (x: number): number => x * x;
来源：http://ccg.daria6918.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://gvw.yj20258888.top

Go:   sq := func(x int) int { return x * x }
来源：http://tdt.daxiang520.top

Ruby: square = ->(x) { x * x }
来源：http://qet.epnwcf.com

C#:   Func<int, int> square = x => x * x;
来源：http://cjv.sjlbkw.cn

[C07] 把函数作为参数传入
来源：http://asf.yvedp.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://qem.fengsongda.top

PHP:  array_map("strtoupper", $arr);
来源：http://uiv.ywan-chungtsiang.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://jal.316326.xyz

TS:   arr.map(String)
来源：http://fao.hammf.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://cjn.xziqi.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mki.feifeiyinyue.top

Ruby: arr.map(&:upcase)
来源：http://cof.bbcook.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://jqp.andypj.xyz

[C08] 闭包
来源：http://dym.shuidangran.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ygl.quarkkingdee.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://foh.nanxuanxn.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://sgj.shangyingyoupin.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://vrd.xuanzx.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://bgz.jqgfzy.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ujj.pengpengdd.cyou

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://uqb.xinyue.icu

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ijk.aizwys.cn

[C09] 递归
来源：http://ttk.hfpthk.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://uzh.wangdashe.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ain.ctjpmb.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tfx.zhaomingkeji.xyz

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dkj.kuanghao11.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://gqh.cashguo.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://djg.sjlbkw.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://bjo.bbcook.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://dzx.bjfxy.top

[C10] 变量作用域
来源：http://aal.zycfv.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://kfw.chenzaomai.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://xro.yj20258888.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://cls.zhaomingkeji.xyz

TS:   同 JS
来源：http://wln.jinqigufen.top

Java: 方法内为块级作用域
来源：http://vtc.daxiang520.top

Go:   花括号块级作用域
来源：http://gsn.tianlin.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ybm.wangdashe.top

C#:   块级作用域
来源：http://ojs.jyoumei.cn

[C11] 模块导入与导出
来源：http://zpl.kuanghao11.cn

Py:   from module import func
来源：http://wlr.pycfn.com

PHP:  require "file.php";  或 use App\Service;
来源：http://hvj.xuanzx.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://jgq.tianlin.xyz

TS:   export function f(): void {};  import { f } from "./m";
来源：http://duu.zhaomingkeji.xyz

Java: import java.util.List;
来源：http://him.chenlongwang.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://qyz.fehbvm.com

Ruby: require "json"; require_relative "./util"
来源：http://peh.hfpthk.cn

C#:   using System.Text;
来源：http://fsc.tianlin.xyz

[C12] 立即执行函数 IIFE
来源：http://pur.cqqwz.cn

Py:   (lambda: print("run"))()
来源：http://jmf.hnqzz.top

PHP:  (function () { echo "run"; })();
来源：http://uhn.sysykeji.top

JS:   (() => { console.log("run"); })();
来源：http://dpq.bjfxy.top

TS:   (() => { console.log("run"); })();
来源：http://zoj.xinyue.icu

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://pcs.chenjidiqi.icu

Go:   func() { fmt.Println("run") }()
来源：http://ywc.c1oappe.top

Ruby: -> { puts "run" }.call
来源：http://ers.hcnkem.com

C#:   // 无 IIFE：用静态构造函数
来源：http://phs.zhongyouzk.top

[C13] 类型声明 / 类型注解
来源：http://xbb.fktsv.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://klb.tarul.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://itm.sysykeji.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://oig.jiagoushi.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kvh.snrcjt.cn

Java: int add(int a, int b) { return a + b; }
来源：http://yur.jianghu66.top

Go:   func add(a, b int) int
来源：http://dlu.jqgfzy.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://bbt.fengsongda.top

C#:   int Add(int a, int b) => a + b;
来源：http://ukm.ivvv.top

[C14] 泛型函数
来源：http://ems.zhengqikj.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://szc.ydzc1.top

PHP:  // 无泛型
来源：http://vmt.52xcode.cn

JS:   // 无泛型
来源：http://xjv.guannengcc.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://thd.xuanzx.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://isk.bbcook.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://gxx.redwolf501.top

Ruby: # 无泛型
来源：http://avb.shuidangran.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://fnn.nanxuanxn.top

[C15] 解构 / 展开参数
来源：http://vie.meibo888.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://jdm.cucudq.cn

PHP:  [$a, $b] = $pair;
来源：http://qaw.havefunace.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://tul.xingfuxueyuan.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://vek.hywenlv.cn

Java: // 无解构
来源：http://pvr.redwolf501.top

Go:   // 无解构
来源：http://tle.quarkkingdee.top

Ruby: a, b = pair
来源：http://rej.sweek.top

C#:   var (a, b) = pair;
来源：http://zlk.pycfn.com

[C16] 函数 / 方法重载
来源：http://hua.jiagoushi.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://yhg.cheryme.top

PHP:  // 无重载
来源：http://nhc.uphjek.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://vwb.jlsjyb.cn

TS:   // 用联合类型或重载签名声明
来源：http://zyh.xuetiantiany.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://itk.yanxiufei.cn

Go:   // 无重载：用不同函数名
来源：http://ciu.xuetiantiany.cn

Ruby: # 无重载：靠动态参数
来源：http://nrt.sufxvd.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://jwq.sufxvd.cn

================================================================================
来源：http://uvf.fzhhl.top

D. 数组 / 列表 / 集合
来源：http://udm.yuanzhike.top

================================================================================
来源：http://kxq.sjlbkw.cn

[D01] 创建数组 / 列表
来源：http://uhx.kuanghao11.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://xxi.haohaochexian.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://cjl.jyoumei.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://zgj.dianchejie.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://lfn.hysaishi.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://lav.ydjk.org.cn

Go:   arr := []int{1, 2, 3}
来源：http://tjn.ehwqpu.com

Ruby: arr = [1, 2, 3]
来源：http://gao.yangfankeji.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://dre.meibo888.top

[D02] 追加元素到末尾
来源：http://zyu.hcnkem.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://nxa.guowangkeji.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://awi.jiagoushi.top

JS:   arr.push(4);
来源：http://spd.aibaodan.cn

TS:   arr.push(4);
来源：http://rij.jqgufenzy.top

Java: list.add(4);
来源：http://fzy.yangfankeji.com

Go:   arr = append(arr, 4)
来源：http://wpo.ctjpmb.com

Ruby: arr << 4; arr.push(5)
来源：http://fwo.316326.xyz

C#:   list.Add(4);
来源：http://opd.jyoumei.cn

[D03] 在指定位置插入元素
来源：http://buy.sufxvd.cn

Py:   arr.insert(0, 0)
来源：http://miy.mhx1999.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://rnz.xingfuxueyuan.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://utl.bbcook.cn

TS:   arr.splice(0, 0, 0);
来源：http://mvv.fehbvm.com

Java: list.add(0, 0);
来源：http://qdn.epnwcf.com

Go:   arr = append([]int{0}, arr...)
来源：http://yit.yongpay.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://eho.shangyingyoupin.top

C#:   list.Insert(0, 0);
来源：http://lyw.shangyingyoupin.top

[D04] 删除元素
来源：http://bij.hnqzz.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://zuz.gotoacloud.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://nts.shzxlz.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://yvn.quarkkingdee.top

TS:   arr.splice(0, 1);
来源：http://hdg.yvedp.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://cip.birdmap.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mml.cheryme.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://gxr.c1oappe.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://enj.vehdjk.com

[D05] 访问与修改元素
来源：http://pdd.xingfuxueyuan.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://zmc.vehdjk.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ogy.chenlongwang.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hfo.jinghuilouyu.cn

TS:   arr[0]; arr.at(-1);
来源：http://bgt.jiagoushi.top

Java: list.get(0); list.set(0, 9);
来源：http://ypd.shanyushiyangkeji.top

Go:   arr[0]; arr[0] = 9
来源：http://fmf.meibo888.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://vuf.52xcode.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wxl.vehdjk.com

[D06] 数组长度
来源：http://vhe.jinqigfzy.top

Py:   len(arr)
来源：http://jly.jqgufenzy.top

PHP:  count($arr);
来源：http://zkq.birdmap.top

JS:   arr.length
来源：http://dvo.hammf.cn

TS:   arr.length
来源：http://ilz.yuxming.cn

Java: list.size();
来源：http://dmp.ydjk.org.cn

Go:   len(arr)
来源：http://jdk.cucudq.cn

Ruby: arr.length; arr.size
来源：http://ocx.dashuyun.cn

C#:   list.Count;
来源：http://kvr.cucudq.cn

[D07] 切片 / 取子数组
来源：http://oaa.jqgfzy.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://uzq.zhijiandao.cn

PHP:  array_slice($arr, 1, 3);
来源：http://wzn.nanxuanxn.top

JS:   arr.slice(1, 4);
来源：http://rmv.hfpthk.cn

TS:   arr.slice(1, 4);
来源：http://byw.fanxiaobao.xyz

Java: list.subList(1, 4);
来源：http://teh.cdnleiting.top

Go:   arr[1:4]
来源：http://dtt.cdnleiting.top

Ruby: arr[1, 3]
来源：http://zni.meibo888.top

C#:   list.GetRange(1, 3);
来源：http://mez.yonumen.top

[D08] 合并两个数组
来源：http://utn.fanxiaobao.xyz

Py:   a + b;  a.extend(b)
来源：http://ffd.dashuyun.cn

PHP:  array_merge($a, $b);
来源：http://rbv.bbcook.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://log.hysaishi.cn

TS:   [...a, ...b];
来源：http://oxh.hesvh.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://pui.pycfn.com

Go:   append(a, b...)
来源：http://uyy.0kj1m.cn


<!-- 参考信息 -->