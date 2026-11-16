代发 wailian999

[B09] break 与 continue
来源：http://dtf.yangfankeji.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hvw.52xcode.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://tzz.dianchejie.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sio.smart0.xyz

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ayh.zhixingplan.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lpu.bjfxy.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://trv.xingfuxueyuan.xyz

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ndm.hnqzz.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hhn.sjlbkw.cn

[B10] 遍历同时拿索引
来源：http://sbi.zhiwuduotai.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hla.cashguo.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://qsn.ppjwa.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://udf.shanyushiyangtech.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://cjj.9152youxi.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://fkm.tianlin.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://iwn.guannengcc.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://qyy.uphjek.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://akv.hfpthk.cn

[B11] 生成数字序列 / 区间
来源：http://bkf.shangyingyoupin.top

Py:   list(range(0, 10, 2))
来源：http://tcz.316326.xyz

PHP:  range(0, 10, 2);
来源：http://uxk.nanxinkj.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rtb.gzhubu.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://quy.ehwqpu.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ogz.kuanghao11.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://cjf.tanke756.top

Ruby: (0...10).step(2).to_a
来源：http://oxy.xuetiantiany.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://gzy.jinyuanbaomall.cn

[B12] 跳出多层循环
来源：http://vmw.bbcook.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://bge.guowangkeji.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://ssc.bjfxy.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mcb.smart0.xyz

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://vhr.gaohongyu789.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://bcr.shanyushiyangkeji.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://aoh.ppjwa.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ejd.jyoumei.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://cjn.cheryme.top

[B13] 判断是否为数字
来源：http://wwr.yvedp.cn

Py:   isinstance(x, (int, float))
来源：http://lrb.fengsongda.top

PHP:  is_numeric($x)
来源：http://ryt.yuxming.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://apj.ydzc1.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://otl.xziqi.cn

Java: x instanceof Number
来源：http://gcd.zhixingplan.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wed.hesvh.cn

Ruby: x.is_a?(Numeric)
来源：http://irq.hongshengwenyu.top

C#:   x is int or double or decimal
来源：http://ynn.yuanzhike.top

[B14] 判断值是否在集合内
来源：http://vuz.nanxuanxn.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://tes.fktsv.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://dbe.hnqzz.top

JS:   [1, 2, 3].includes(x)
来源：http://los.kuanghao11.cn

TS:   [1, 2, 3].includes(x)
来源：http://khi.pycfn.com

Java: List.of(1, 2, 3).contains(x)
来源：http://yby.sxryk.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://tin.nwbrower.top

Ruby: [1, 2, 3].include?(x)
来源：http://hmn.jinqigufen.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ywg.daxiang520.top

[B15] 布尔运算与取反
来源：http://was.fehbvm.com

Py:   a and b or not c
来源：http://qsm.yj20258.top

PHP:  $a && $b || !$c
来源：http://sfc.aibaodan.cn

JS:   a && b || !c
来源：http://mnm.haohaochexian.top

TS:   a && b || !c
来源：http://gii.andypj.xyz

Java: a && b || !c
来源：http://kas.zdbjq.cn

Go:   a && b || !c
来源：http://xob.jianghu66.top

Ruby: a && b || !c
来源：http://ruv.fanxiaobao.xyz

C#:   a && b || !c
来源：http://lmv.nanxuanxn.top

[B16] 卫语句：不满足条件提前返回
来源：http://oqp.uphjek.com

Py:   if not data: return
来源：http://fpb.jyoumei.cn

PHP:  if (!$data) { return; }
来源：http://lbc.zycfv.cn

JS:   if (!data) return;
来源：http://umw.zhiwuduotai.top

TS:   if (!data) return;
来源：http://cte.tianlin.xyz

Java: if (data == null) return;
来源：http://wpe.gzhubu.top

Go:   if data == nil { return }
来源：http://xja.meibo888.top

Ruby: return if data.nil?
来源：http://wig.birdmap.top

C#:   if (data == null) return;
来源：http://xjr.jinqigufen.top

================================================================================
来源：http://izg.jinqigfzy.top

C. 函数与作用域
来源：http://doj.cdnleiting.top

================================================================================
来源：http://irk.gotoacloud.top

[C01] 定义函数
来源：http://zcf.nanxinkj.top

Py:   def add(a, b): return a + b
来源：http://pzg.jyoumei.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hdw.dashuyun.cn

JS:   function add(a, b) { return a + b; }
来源：http://slq.ctjpmb.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jju.zhoulong.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://kqm.wangshuangyany.cn

Go:   func add(a, b int) int { return a + b }
来源：http://lba.hnqzz.top

Ruby: def add(a, b); a + b; end
来源：http://qfm.zhoulong.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://jdw.hcnkem.com

[C02] 默认参数
来源：http://wxl.xziqi.cn

Py:   def greet(name="World"): return name
来源：http://cpm.hnqzz.top

PHP:  function greet($name = "World") { return $name; }
来源：http://via.haohaochexian.top

JS:   function greet(name = "World") { return name; }
来源：http://uvm.cheryme.top

TS:   function greet(name: string = "World") { return name; }
来源：http://eds.shzxlz.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://yry.zhoulong.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://jky.mhx1999.top

Ruby: def greet(name = "World") = name
来源：http://ujs.uphjek.com

C#:   string Greet(string name = "World") => name;
来源：http://oah.hesvh.cn

[C03] 可变参数
来源：http://kxs.tanke756.top

Py:   def total(*args): return sum(args)
来源：http://muv.jinghuilouyu.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://lbe.yj20258.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://kve.shanyushiyangkeji.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://cyq.havefunace.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://dqv.jinqigufen.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ujq.gogol.net.cn

Ruby: def total(*nums); nums.sum; end
来源：http://hmc.xziqi.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://xse.316326.xyz

[C04] 命名参数 / 关键字参数
来源：http://hsj.iojbl.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://lfo.andypj.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ieh.dashuyun.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://koa.hysaishi.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://pgq.nanxinkj.top

Java: // 无：用 Builder 模式或 record
来源：http://pev.yangfankeji.com

Go:   // 无：用配置结构体参数
来源：http://xpl.jlsjyb.cn

Ruby: f(a: 1, b: 2)
来源：http://ska.c1oappe.top

C#:   f(a: 1, b: 2)
来源：http://zmf.andypj.xyz

[C05] 返回多个值
来源：http://ipr.chenzaomai.com

Py:   return a, b
来源：http://xvk.mhx1999.top

PHP:  return [$a, $b];
来源：http://iaq.nanxuanxn.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://gtg.jinqigufen.top

TS:   return { a, b };
来源：http://hpg.hcnkem.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://snk.havefunace.top

Go:   return a, b
来源：http://hmd.316326.xyz

Ruby: return a, b
来源：http://obn.yuanzhike.top

C#:   return (a, b);              // ValueTuple
来源：http://qdk.havefunace.top

[C06] 匿名函数 / lambda
来源：http://iep.fengsongda.top

Py:   square = lambda x: x * x
来源：http://gmn.sufxvd.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://udt.havefunace.top

JS:   const square = x => x * x;
来源：http://epn.shuidangran.top

TS:   const square = (x: number): number => x * x;
来源：http://mim.meibo888.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://dce.yj202588.top

Go:   sq := func(x int) int { return x * x }
来源：http://qqk.c1oappe.top

Ruby: square = ->(x) { x * x }
来源：http://uvs.jinyuanbaomall.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ctc.sufxvd.cn

[C07] 把函数作为参数传入
来源：http://zpc.redwolf501.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ohv.gaohongyu789.top

PHP:  array_map("strtoupper", $arr);
来源：http://sht.andypj.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://crr.ctjpmb.com

TS:   arr.map(String)
来源：http://yna.cdnleiting.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://gbs.yj20258888.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://sen.9152youxi.cn

Ruby: arr.map(&:upcase)
来源：http://ufi.sxryk.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://jly.gogol.net.cn

[C08] 闭包
来源：http://tet.nwbrower.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://kyq.gzhubu.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hkn.redwolf501.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://oqh.ehwqpu.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://eay.tian-w.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://edz.zdqjudy.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://fvz.sufxvd.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://dts.shzxlz.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://otr.bjfxy.top

[C09] 递归
来源：http://mgn.aizwys.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://jih.zhixingplan.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://gya.cdnleiting.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hzp.0kj1m.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://efo.yfazqb.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://rcl.ppjwa.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://gkw.tianlin.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://lqk.havefunace.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://jvl.yfazqb.com

[C10] 变量作用域
来源：http://pgp.shzxlz.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://pkz.zhijiandao.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://atm.52xcode.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://pkg.nanxuanxn.top

TS:   同 JS
来源：http://dkg.hesvh.cn

Java: 方法内为块级作用域
来源：http://yvm.xziqi.cn

Go:   花括号块级作用域
来源：http://vmh.svipenyu.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mka.chenlongwang.top

C#:   块级作用域
来源：http://vul.0kj1m.cn

[C11] 模块导入与导出
来源：http://kqu.jinqigfzy.top

Py:   from module import func
来源：http://vcu.svipenyu.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://jno.fktsv.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://oex.xinyue.icu

TS:   export function f(): void {};  import { f } from "./m";
来源：http://lmp.hammf.cn

Java: import java.util.List;
来源：http://iil.zhixingplan.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wgs.vqdsnc.cn

Ruby: require "json"; require_relative "./util"
来源：http://mty.guannengcc.top

C#:   using System.Text;
来源：http://itc.gaohongyu789.top

[C12] 立即执行函数 IIFE
来源：http://far.yanxiufei.cn

Py:   (lambda: print("run"))()
来源：http://wnx.daxiang520.top

PHP:  (function () { echo "run"; })();
来源：http://cpy.yj20258888.top

JS:   (() => { console.log("run"); })();
来源：http://dkk.svipenyu.cn

TS:   (() => { console.log("run"); })();
来源：http://ztg.ppjwa.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wsi.0kj1m.cn

Go:   func() { fmt.Println("run") }()
来源：http://ubf.dashuyun.cn

Ruby: -> { puts "run" }.call
来源：http://ggp.fzhhl.top

C#:   // 无 IIFE：用静态构造函数
来源：http://ews.jyoumei.cn

[C13] 类型声明 / 类型注解
来源：http://xkn.yj20258.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://kns.jinyuanbaomall.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ujk.zdqjudy.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://bzz.sweek.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nxe.epnwcf.com

Java: int add(int a, int b) { return a + b; }
来源：http://xlm.fktsv.cn

Go:   func add(a, b int) int
来源：http://jpb.shangyingyoupin.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://lhj.nanxinkj.top

C#:   int Add(int a, int b) => a + b;
来源：http://ggx.zycfv.cn

[C14] 泛型函数
来源：http://zfn.fzhhl.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://dry.guannengcc.top

PHP:  // 无泛型
来源：http://kzf.nanxinkj.top

JS:   // 无泛型
来源：http://wtv.hammf.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://eyp.hywenlv.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://xmh.jiagoushi.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://lni.fanxiaobao.xyz

Ruby: # 无泛型
来源：http://dha.xuetiantiany.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://dgj.svipenyu.cn

[C15] 解构 / 展开参数
来源：http://xjy.pycfn.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wly.aizwys.cn

PHP:  [$a, $b] = $pair;
来源：http://wju.jqgufenzy.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://rea.yongpay.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hit.nanxuanxn.top

Java: // 无解构
来源：http://xqt.zhiwuduotai.top

Go:   // 无解构
来源：http://zzy.daria6918.cn

Ruby: a, b = pair
来源：http://nco.shanyushiyangtech.top

C#:   var (a, b) = pair;
来源：http://pxk.meibo888.top

[C16] 函数 / 方法重载
来源：http://sgr.shuidangran.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hon.hnxiangtu.top

PHP:  // 无重载
来源：http://ryi.xylfe.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://lvw.guowangkeji.top

TS:   // 用联合类型或重载签名声明
来源：http://unb.birdmap.top

Java: void f(int a) {}  void f(String a) {}
来源：http://swu.andypj.xyz

Go:   // 无重载：用不同函数名
来源：http://jdl.zycfv.cn

Ruby: # 无重载：靠动态参数
来源：http://jrr.yfazqb.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://huz.cheryme.top

================================================================================
来源：http://tnz.bbcook.cn

D. 数组 / 列表 / 集合
来源：http://caf.quarkkingdee.top

================================================================================
来源：http://yyb.haohaochexian.top

[D01] 创建数组 / 列表
来源：http://jbz.uphjek.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://jic.yj20258888.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://opo.hongshengwenyu.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://gbh.cashguo.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://dnb.fengsongda.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://odt.hesvh.cn

Go:   arr := []int{1, 2, 3}
来源：http://jtf.jyoumei.cn

Ruby: arr = [1, 2, 3]
来源：http://yoh.jqgufenzy.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ynh.yuxming.cn

[D02] 追加元素到末尾
来源：http://wbv.yueranfly.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://nay.fengsongda.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://qeu.xziqi.cn

JS:   arr.push(4);
来源：http://jjv.guowangkeji.top

TS:   arr.push(4);
来源：http://pmi.jinqigfzy.top

Java: list.add(4);
来源：http://nnm.yanxiufei.cn

Go:   arr = append(arr, 4)
来源：http://fdn.wangshuangyany.cn

Ruby: arr << 4; arr.push(5)
来源：http://iqu.zhoulong.xyz

C#:   list.Add(4);
来源：http://wto.zycfv.cn

[D03] 在指定位置插入元素
来源：http://gzn.hnxiangtu.top

Py:   arr.insert(0, 0)
来源：http://isl.jqgfzy.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ygj.guowangkeji.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://tvt.wangdashe.top

TS:   arr.splice(0, 0, 0);
来源：http://gjh.jqgfzy.top

Java: list.add(0, 0);
来源：http://avn.svipenyu.cn

Go:   arr = append([]int{0}, arr...)
来源：http://pad.guowangkeji.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://zyp.yuxming.cn

C#:   list.Insert(0, 0);
来源：http://spy.jinghuilouyu.cn

[D04] 删除元素
来源：http://rce.316326.xyz

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://cwm.316326.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ymi.daxiang520.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://jov.316326.xyz

TS:   arr.splice(0, 1);
来源：http://ddl.ppjwa.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://rrp.chenjidiqi.icu

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ylw.xingfuxueyuan.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://oib.andypj.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://vep.zdbjq.cn

[D05] 访问与修改元素
来源：http://cqi.pycfn.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://bft.xingfuxueyuan.xyz

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://vtn.yfazqb.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://lut.hcnkem.com

TS:   arr[0]; arr.at(-1);
来源：http://bqb.yuxming.cn

Java: list.get(0); list.set(0, 9);
来源：http://ztz.wangdashe.top

Go:   arr[0]; arr[0] = 9
来源：http://tbm.jlsjyb.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://gnn.hysaishi.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://kaz.jinghuilouyu.cn

[D06] 数组长度
来源：http://xkr.c1oappe.top

Py:   len(arr)
来源：http://hqy.yanxiufei.cn

PHP:  count($arr);
来源：http://tiw.jinghuilouyu.cn

JS:   arr.length
来源：http://jnp.cucudq.cn

TS:   arr.length
来源：http://cdh.bjfxy.top

Java: list.size();
来源：http://twr.tianlin.xyz

Go:   len(arr)
来源：http://ktk.hcnkem.com

Ruby: arr.length; arr.size
来源：http://jzh.shanyushiyangkeji.top

C#:   list.Count;
来源：http://afv.52xcode.cn

[D07] 切片 / 取子数组
来源：http://hhp.xziqi.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://xxw.chenlongwang.top

PHP:  array_slice($arr, 1, 3);
来源：http://yqx.cheryme.top

JS:   arr.slice(1, 4);
来源：http://fky.gotoacloud.top

TS:   arr.slice(1, 4);
来源：http://nmy.jiagoushi.top

Java: list.subList(1, 4);
来源：http://mme.wangshuangyany.cn

Go:   arr[1:4]
来源：http://eqk.sxryk.cn

Ruby: arr[1, 3]
来源：http://cqp.ywan-chungtsiang.top

C#:   list.GetRange(1, 3);
来源：http://vfi.hysaishi.cn

[D08] 合并两个数组
来源：http://ymq.nwbrower.top

Py:   a + b;  a.extend(b)
来源：http://jiq.xuanzx.com

PHP:  array_merge($a, $b);
来源：http://hgv.hnqzz.top

JS:   [...a, ...b];  a.concat(b);
来源：http://pfx.zdqjudy.top

TS:   [...a, ...b];
来源：http://uek.sysykeji.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://iwe.quarkkingdee.top

Go:   append(a, b...)
来源：http://ryo.iojbl.cn

Ruby: a + b;  a.concat(b)
来源：http://uky.ehwqpu.com

C#:   a.Concat(b).ToList()
来源：http://gjf.tian-w.cn

[D09] 排序（升序）
来源：http://kqq.jqgfzy.top

Py:   sorted(arr);  arr.sort()
来源：http://rdj.andypj.xyz

PHP:  sort($arr);
来源：http://hbl.ydzc1.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://zqp.jinqigfzy.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://iou.nanxuanxn.top

Java: Collections.sort(list);  list.sort(null);
来源：http://jds.fzhhl.top


<!-- 参考信息 -->