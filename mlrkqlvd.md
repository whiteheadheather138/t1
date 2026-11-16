代发 wailian999

[B09] break 与 continue
来源：http://gal.nanxuanxn.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://xnn.hongshengwenyu.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ifa.xylfe.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pib.jianghu66.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pan.ctjpmb.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://frm.dashuyun.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://dgs.zhengqikj.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://kvz.52xcode.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bwf.sufxvd.cn

[B10] 遍历同时拿索引
来源：http://brp.gogol.net.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://oyy.hywenlv.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ojn.c1oappe.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wfv.fengsongda.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://igj.svipenyu.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ktl.xingfuxueyuan.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://vrz.cucudq.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://tzt.zhaomingkeji.xyz

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mxo.xuanzx.com

[B11] 生成数字序列 / 区间
来源：http://ofu.fanxiaobao.xyz

Py:   list(range(0, 10, 2))
来源：http://uie.yj20258888.top

PHP:  range(0, 10, 2);
来源：http://qkg.jinyuanbaomall.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kqb.redwolf501.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zys.tian-w.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://gjy.sysykeji.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://syw.shanyushiyangtech.top

Ruby: (0...10).step(2).to_a
来源：http://tvx.tanke756.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://azt.jlsjyb.cn

[B12] 跳出多层循环
来源：http://khk.fzhhl.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://npg.feifeiyinyue.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://bgk.yvedp.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mba.yuxming.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://nty.quarkkingdee.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://kll.ctjpmb.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://fst.xuanzx.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mmk.yfazqb.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://aol.ydzc1.top

[B13] 判断是否为数字
来源：http://wjx.snrcjt.cn

Py:   isinstance(x, (int, float))
来源：http://qed.jinghuilouyu.cn

PHP:  is_numeric($x)
来源：http://czs.sxryk.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mnw.yueranfly.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fsi.ydjk.org.cn

Java: x instanceof Number
来源：http://vmw.andypj.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://icr.redwolf501.top

Ruby: x.is_a?(Numeric)
来源：http://xwc.andypj.xyz

C#:   x is int or double or decimal
来源：http://dxu.pengpengdd.cyou

[B14] 判断值是否在集合内
来源：http://gub.c1oappe.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://dws.jinghuilouyu.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ubs.xingfuxueyuan.xyz

JS:   [1, 2, 3].includes(x)
来源：http://vkb.ydjk.org.cn

TS:   [1, 2, 3].includes(x)
来源：http://dbw.guowangkeji.top

Java: List.of(1, 2, 3).contains(x)
来源：http://foc.tarul.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://fso.yj20258888.top

Ruby: [1, 2, 3].include?(x)
来源：http://nne.smart0.xyz

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://cwa.fanxiaobao.xyz

[B15] 布尔运算与取反
来源：http://iux.hcnkem.com

Py:   a and b or not c
来源：http://kpf.hesvh.cn

PHP:  $a && $b || !$c
来源：http://qma.fzhhl.top

JS:   a && b || !c
来源：http://ofo.quarkkingdee.top

TS:   a && b || !c
来源：http://uho.guowangkeji.top

Java: a && b || !c
来源：http://ozr.xinyue.icu

Go:   a && b || !c
来源：http://lar.guannengcc.top

Ruby: a && b || !c
来源：http://wjq.uphjek.com

C#:   a && b || !c
来源：http://yrv.daria6918.cn

[B16] 卫语句：不满足条件提前返回
来源：http://hml.fehbvm.com

Py:   if not data: return
来源：http://zsd.pengpengdd.cyou

PHP:  if (!$data) { return; }
来源：http://abx.haohaochexian.top

JS:   if (!data) return;
来源：http://uzi.vqdsnc.cn

TS:   if (!data) return;
来源：http://uje.guowangkeji.top

Java: if (data == null) return;
来源：http://uqd.haohaochexian.top

Go:   if data == nil { return }
来源：http://uxq.ppjwa.cn

Ruby: return if data.nil?
来源：http://sgw.hfpthk.cn

C#:   if (data == null) return;
来源：http://jta.0kj1m.cn

================================================================================
来源：http://cqn.zycfv.cn

C. 函数与作用域
来源：http://cll.ywan-chungtsiang.top

================================================================================
来源：http://bjt.cdnleiting.top

[C01] 定义函数
来源：http://uof.fehbvm.com

Py:   def add(a, b): return a + b
来源：http://vvy.hysaishi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ivj.316326.xyz

JS:   function add(a, b) { return a + b; }
来源：http://rkr.haohaochexian.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kdi.birdmap.top

Java: static int add(int a, int b) { return a + b; }
来源：http://gep.chenzaomai.com

Go:   func add(a, b int) int { return a + b }
来源：http://tno.jyoumei.cn

Ruby: def add(a, b); a + b; end
来源：http://ojr.zdbjq.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://dse.zhoulong.xyz

[C02] 默认参数
来源：http://kyy.0kj1m.cn

Py:   def greet(name="World"): return name
来源：http://ufw.aizwys.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://evd.sxryk.cn

JS:   function greet(name = "World") { return name; }
来源：http://huc.gzhubu.top

TS:   function greet(name: string = "World") { return name; }
来源：http://mry.uphjek.com

Java: // 无默认参数：方法重载或 Optional
来源：http://wso.gzhubu.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://vbf.0kj1m.cn

Ruby: def greet(name = "World") = name
来源：http://bch.yangfankeji.com

C#:   string Greet(string name = "World") => name;
来源：http://kbg.jiagoushi.top

[C03] 可变参数
来源：http://zco.yuxming.cn

Py:   def total(*args): return sum(args)
来源：http://gxt.jyoumei.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xvn.cheryme.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://crk.gzhubu.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://dvf.jinghuilouyu.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://aiu.cqqwz.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://pud.316326.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://xnn.vehdjk.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://jac.guannengcc.top

[C04] 命名参数 / 关键字参数
来源：http://bya.zhaomingkeji.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://yiw.yfazqb.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://zmy.cqqwz.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://gta.fanxiaobao.xyz

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://pnc.cashguo.top

Java: // 无：用 Builder 模式或 record
来源：http://vcr.zdqjudy.top

Go:   // 无：用配置结构体参数
来源：http://hyz.ydjk.org.cn

Ruby: f(a: 1, b: 2)
来源：http://bim.xuetiantiany.cn

C#:   f(a: 1, b: 2)
来源：http://ynw.yuanzhike.top

[C05] 返回多个值
来源：http://zop.wangshuangyany.cn

Py:   return a, b
来源：http://lmr.uphjek.com

PHP:  return [$a, $b];
来源：http://ypy.aibaodan.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ayp.vehdjk.com

TS:   return { a, b };
来源：http://sor.cashguo.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://nit.zhiwuduotai.top

Go:   return a, b
来源：http://mnm.ydjk.org.cn

Ruby: return a, b
来源：http://lal.hnqzz.top

C#:   return (a, b);              // ValueTuple
来源：http://qsm.jqgfzy.top

[C06] 匿名函数 / lambda
来源：http://ama.yongpay.top

Py:   square = lambda x: x * x
来源：http://cca.zhoulong.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://dcs.chenzaomai.com

JS:   const square = x => x * x;
来源：http://lpw.quarkkingdee.top

TS:   const square = (x: number): number => x * x;
来源：http://npn.zdqjudy.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://bme.316326.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://uro.dianchejie.cn

Ruby: square = ->(x) { x * x }
来源：http://hds.jyoumei.cn

C#:   Func<int, int> square = x => x * x;
来源：http://guf.nanxinkj.top

[C07] 把函数作为参数传入
来源：http://jig.wangdashe.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://xev.haohaochexian.top

PHP:  array_map("strtoupper", $arr);
来源：http://qpv.c1oappe.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hwe.zdqjudy.top

TS:   arr.map(String)
来源：http://mgc.cashguo.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://qwd.wangdashe.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://alo.quarkkingdee.top

Ruby: arr.map(&:upcase)
来源：http://pqw.yuanzhike.top

C#:   arr.Select(s => s.ToUpper())
来源：http://uxb.zhengqikj.top

[C08] 闭包
来源：http://jey.yuanzhike.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://fqx.sweek.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://nxx.fehbvm.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://tqk.jinqigfzy.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://fzc.xylfe.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://fip.52xcode.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://qgk.guannengcc.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://lys.guannengcc.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://jbo.bbcook.cn

[C09] 递归
来源：http://abg.yj202588.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ied.yangfankeji.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://qdh.fengsongda.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qvp.jyoumei.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://epp.wangshuangyany.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://eib.zhiwuduotai.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://eyn.yuxming.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://unq.fktsv.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://spw.yfazqb.com

[C10] 变量作用域
来源：http://gaz.jyoumei.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://jma.smart0.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hjp.jinqigufen.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://nmp.fktsv.cn

TS:   同 JS
来源：http://evb.ivvv.top

Java: 方法内为块级作用域
来源：http://hea.cucudq.cn

Go:   花括号块级作用域
来源：http://ukq.sufxvd.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mcq.jlsjyb.cn

C#:   块级作用域
来源：http://cub.smart0.xyz

[C11] 模块导入与导出
来源：http://pxj.havefunace.top

Py:   from module import func
来源：http://dsz.guowangkeji.top

PHP:  require "file.php";  或 use App\Service;
来源：http://ppz.xuanzx.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://jvy.cheryme.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://okd.gotoacloud.top

Java: import java.util.List;
来源：http://vlv.bjfxy.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://uwf.redwolf501.top

Ruby: require "json"; require_relative "./util"
来源：http://cre.sysykeji.top

C#:   using System.Text;
来源：http://tub.shanyushiyangkeji.top

[C12] 立即执行函数 IIFE
来源：http://jfy.zhongyouzk.top

Py:   (lambda: print("run"))()
来源：http://syu.chenzaomai.com

PHP:  (function () { echo "run"; })();
来源：http://gqm.hysaishi.cn

JS:   (() => { console.log("run"); })();
来源：http://jch.sysykeji.top

TS:   (() => { console.log("run"); })();
来源：http://tgp.ydzc1.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://stx.ybcxt.top

Go:   func() { fmt.Println("run") }()
来源：http://mqv.ctjpmb.com

Ruby: -> { puts "run" }.call
来源：http://pos.zhengqikj.top

C#:   // 无 IIFE：用静态构造函数
来源：http://nyu.ivvv.top

[C13] 类型声明 / 类型注解
来源：http://aex.yj202588.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://eqc.nanxinkj.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mcg.ivvv.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://lme.chenlongwang.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vjh.cdnleiting.top

Java: int add(int a, int b) { return a + b; }
来源：http://six.hnqzz.top

Go:   func add(a, b int) int
来源：http://vyp.yonumen.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://qib.aibaodan.cn

C#:   int Add(int a, int b) => a + b;
来源：http://lns.meibo888.top

[C14] 泛型函数
来源：http://szu.zhiwuduotai.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://afn.daria6918.cn

PHP:  // 无泛型
来源：http://tam.hysaishi.cn

JS:   // 无泛型
来源：http://clj.tianlin.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://loo.yfazqb.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://imo.uphjek.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://szk.yvedp.cn

Ruby: # 无泛型
来源：http://sxv.ctjpmb.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://iph.hywenlv.cn

[C15] 解构 / 展开参数
来源：http://anw.xingfuxueyuan.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://itk.xingfuxueyuan.xyz

PHP:  [$a, $b] = $pair;
来源：http://gst.hongshengwenyu.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://auj.tian-w.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://uil.svipenyu.cn

Java: // 无解构
来源：http://piy.ehwqpu.com

Go:   // 无解构
来源：http://ryh.hnqzz.top

Ruby: a, b = pair
来源：http://pvd.gzhubu.top

C#:   var (a, b) = pair;
来源：http://vaf.epnwcf.com

[C16] 函数 / 方法重载
来源：http://xng.fengsongda.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vpy.zycfv.cn

PHP:  // 无重载
来源：http://xrs.ehwqpu.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://cki.ywan-chungtsiang.top

TS:   // 用联合类型或重载签名声明
来源：http://guo.cdnleiting.top

Java: void f(int a) {}  void f(String a) {}
来源：http://zlc.yongpay.top

Go:   // 无重载：用不同函数名
来源：http://hny.pengpengdd.cyou

Ruby: # 无重载：靠动态参数
来源：http://sei.yj20258.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://vuo.yfazqb.com

================================================================================
来源：http://ywk.dianchejie.cn

D. 数组 / 列表 / 集合
来源：http://ifj.aizwys.cn

================================================================================
来源：http://klp.hywenlv.cn

[D01] 创建数组 / 列表
来源：http://kfy.ivvv.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://pwf.hysaishi.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://lrl.fehbvm.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://qbv.iojbl.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://rrn.havefunace.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://whb.quarkkingdee.top

Go:   arr := []int{1, 2, 3}
来源：http://bll.ywan-chungtsiang.top

Ruby: arr = [1, 2, 3]
来源：http://hyj.birdmap.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://lqz.jinyuanbaomall.cn

[D02] 追加元素到末尾
来源：http://gxd.tarul.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://elc.yongpay.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://swo.ehwqpu.com

JS:   arr.push(4);
来源：http://jwa.sweek.top

TS:   arr.push(4);
来源：http://vfb.meibo888.top

Java: list.add(4);
来源：http://xqc.yonumen.top

Go:   arr = append(arr, 4)
来源：http://hhk.wangshuangyany.cn

Ruby: arr << 4; arr.push(5)
来源：http://mdt.yj202588.top

C#:   list.Add(4);
来源：http://rxt.tian-w.cn

[D03] 在指定位置插入元素
来源：http://hsa.fktsv.cn

Py:   arr.insert(0, 0)
来源：http://zei.hcnkem.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://gpd.ybcxt.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://tpg.yonumen.top

TS:   arr.splice(0, 0, 0);
来源：http://wlh.snrcjt.cn

Java: list.add(0, 0);
来源：http://sfr.jinghuilouyu.cn

Go:   arr = append([]int{0}, arr...)
来源：http://zgz.zhiwuduotai.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://nro.sjlbkw.cn

C#:   list.Insert(0, 0);
来源：http://oks.shuidangran.top

[D04] 删除元素
来源：http://dky.haohaochexian.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://iqw.ywan-chungtsiang.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ffx.yfazqb.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://grn.hesvh.cn

TS:   arr.splice(0, 1);
来源：http://pwn.ydjk.org.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://yvu.pycfn.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://glq.ehwqpu.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://gmr.tianlin.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://gdt.hysaishi.cn

[D05] 访问与修改元素
来源：http://evv.fktsv.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ypt.hywenlv.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://kkf.wangdashe.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://rtt.fktsv.cn

TS:   arr[0]; arr.at(-1);
来源：http://wld.xuetiantiany.cn

Java: list.get(0); list.set(0, 9);
来源：http://ksn.zdqjudy.top

Go:   arr[0]; arr[0] = 9
来源：http://vvi.hcnkem.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://gks.nanxinkj.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://uys.iojbl.cn

[D06] 数组长度
来源：http://gxp.c1oappe.top

Py:   len(arr)
来源：http://pdh.jyoumei.cn

PHP:  count($arr);
来源：http://tzy.jinqigfzy.top

JS:   arr.length
来源：http://eqk.hongshengwenyu.top

TS:   arr.length
来源：http://aps.shanyushiyangkeji.top

Java: list.size();
来源：http://opp.gogol.net.cn

Go:   len(arr)
来源：http://zse.yuxming.cn

Ruby: arr.length; arr.size
来源：http://zqi.yuanzhike.top

C#:   list.Count;
来源：http://uks.sysykeji.top

[D07] 切片 / 取子数组
来源：http://aqh.tian-w.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://kaf.9152youxi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://fwn.kuanghao11.cn

JS:   arr.slice(1, 4);
来源：http://hcr.cdnleiting.top

TS:   arr.slice(1, 4);
来源：http://toh.havefunace.top

Java: list.subList(1, 4);
来源：http://qxl.sysykeji.top

Go:   arr[1:4]
来源：http://anw.jinqigfzy.top

Ruby: arr[1, 3]
来源：http://qug.xziqi.cn

C#:   list.GetRange(1, 3);
来源：http://ykz.zhoulong.xyz

[D08] 合并两个数组
来源：http://wgo.ctjpmb.com

Py:   a + b;  a.extend(b)
来源：http://vll.ydjk.org.cn

PHP:  array_merge($a, $b);
来源：http://piu.zhijiandao.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://gyk.andypj.xyz

TS:   [...a, ...b];
来源：http://ekh.guannengcc.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://unt.jiagoushi.top

Go:   append(a, b...)
来源：http://hfh.yuanzhike.top

Ruby: a + b;  a.concat(b)
来源：http://vqq.tarul.cn

C#:   a.Concat(b).ToList()
来源：http://lun.xziqi.cn

[D09] 排序（升序）
来源：http://pav.sweek.top

Py:   sorted(arr);  arr.sort()
来源：http://hvl.52xcode.cn

PHP:  sort($arr);
来源：http://gdi.fengsongda.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wmb.ydzc1.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://oay.bbcook.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://vxp.yfazqb.com


<!-- 参考信息 -->