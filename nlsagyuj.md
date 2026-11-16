代发 wailian999

Java: do { i++; } while (i < 10);
来源：http://zno.fktsv.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://sff.tarul.cn

Ruby: begin; i += 1; end while i < 10
来源：http://vfj.ehwqpu.com

C#:   do { i++; } while (i < 10);
来源：http://rkp.fanxiaobao.xyz

[B09] break 与 continue
来源：http://jhq.bjfxy.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://qie.hesvh.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://dmg.gotoacloud.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bes.gzhubu.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hcn.yanxiufei.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xkf.zdqjudy.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://szv.kuanghao11.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://kvk.epnwcf.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fdr.fengsongda.top

[B10] 遍历同时拿索引
来源：http://cjm.havefunace.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://qcn.aibaodan.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ytr.fengsongda.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://tvg.yj202588.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://uue.c1oappe.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://fbj.daxiang520.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://csn.zhiwuduotai.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://acs.zdqjudy.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://xuz.shuidangran.top

[B11] 生成数字序列 / 区间
来源：http://hvj.xuanzx.com

Py:   list(range(0, 10, 2))
来源：http://jrz.yuxming.cn

PHP:  range(0, 10, 2);
来源：http://bze.yonumen.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yby.ivvv.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://acx.yj202588.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://rjd.gogol.net.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ixj.xziqi.cn

Ruby: (0...10).step(2).to_a
来源：http://rht.shangyingyoupin.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://kef.vqdsnc.cn

[B12] 跳出多层循环
来源：http://wee.mhx1999.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://xtd.xuanzx.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://ley.guowangkeji.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ksu.sweek.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://jlf.birdmap.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hmc.gaohongyu789.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://rik.yueranfly.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://efr.jinghuilouyu.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wjp.chenzaomai.com

[B13] 判断是否为数字
来源：http://vsx.fanxiaobao.xyz

Py:   isinstance(x, (int, float))
来源：http://jjk.gzhubu.top

PHP:  is_numeric($x)
来源：http://eea.guannengcc.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://apq.52xcode.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://saf.hcnkem.com

Java: x instanceof Number
来源：http://pmn.dianchejie.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://qiq.yfazqb.com

Ruby: x.is_a?(Numeric)
来源：http://ghe.jinqigufen.top

C#:   x is int or double or decimal
来源：http://ijo.vehdjk.com

[B14] 判断值是否在集合内
来源：http://etn.tianlin.xyz

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jhj.hywenlv.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ikh.aizwys.cn

JS:   [1, 2, 3].includes(x)
来源：http://nqv.zhengqikj.top

TS:   [1, 2, 3].includes(x)
来源：http://vct.jyoumei.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://jet.daxiang520.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://cfa.hesvh.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ltg.yueranfly.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://fut.havefunace.top

[B15] 布尔运算与取反
来源：http://vvc.mhx1999.top

Py:   a and b or not c
来源：http://kyj.gogol.net.cn

PHP:  $a && $b || !$c
来源：http://jhr.ybcxt.top

JS:   a && b || !c
来源：http://cis.xuetiantiany.cn

TS:   a && b || !c
来源：http://rao.jinyuanbaomall.cn

Java: a && b || !c
来源：http://aff.bjfxy.top

Go:   a && b || !c
来源：http://otz.sxryk.cn

Ruby: a && b || !c
来源：http://ssg.zdqjudy.top

C#:   a && b || !c
来源：http://kjv.quarkkingdee.top

[B16] 卫语句：不满足条件提前返回
来源：http://fpj.jinyuanbaomall.cn

Py:   if not data: return
来源：http://uwo.jiagoushi.top

PHP:  if (!$data) { return; }
来源：http://grb.yongpay.top

JS:   if (!data) return;
来源：http://hyb.xuanzx.com

TS:   if (!data) return;
来源：http://pbs.hesvh.cn

Java: if (data == null) return;
来源：http://lab.xingfuxueyuan.xyz

Go:   if data == nil { return }
来源：http://xlq.jianghu66.top

Ruby: return if data.nil?
来源：http://dyv.bbcook.cn

C#:   if (data == null) return;
来源：http://xpf.shuidangran.top

================================================================================
来源：http://vgw.hysaishi.cn

C. 函数与作用域
来源：http://ldr.hywenlv.cn

================================================================================
来源：http://dnj.chenlongwang.top

[C01] 定义函数
来源：http://yrp.pengpengdd.cyou

Py:   def add(a, b): return a + b
来源：http://fpf.feifeiyinyue.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hxr.yangfankeji.com

JS:   function add(a, b) { return a + b; }
来源：http://ujh.hammf.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mpa.gaohongyu789.top

Java: static int add(int a, int b) { return a + b; }
来源：http://mwc.quarkkingdee.top

Go:   func add(a, b int) int { return a + b }
来源：http://rlc.bjfxy.top

Ruby: def add(a, b); a + b; end
来源：http://slh.bjfxy.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ehp.yuanzhike.top

[C02] 默认参数
来源：http://txp.ydzc1.top

Py:   def greet(name="World"): return name
来源：http://wax.svipenyu.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://hop.yj202588.top

JS:   function greet(name = "World") { return name; }
来源：http://swh.xinyue.icu

TS:   function greet(name: string = "World") { return name; }
来源：http://chh.yj20258888.top

Java: // 无默认参数：方法重载或 Optional
来源：http://gvw.ywan-chungtsiang.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://zwc.zycfv.cn

Ruby: def greet(name = "World") = name
来源：http://rjn.jyoumei.cn

C#:   string Greet(string name = "World") => name;
来源：http://xxw.hfpthk.cn

[C03] 可变参数
来源：http://yuk.tarul.cn

Py:   def total(*args): return sum(args)
来源：http://udg.sysykeji.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://zsw.cdnleiting.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://jog.smart0.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://acy.hysaishi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://opa.316326.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://uro.guowangkeji.top

Ruby: def total(*nums); nums.sum; end
来源：http://hzh.shuidangran.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ifd.yfazqb.com

[C04] 命名参数 / 关键字参数
来源：http://vfp.feifeiyinyue.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hxx.iojbl.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ygg.jyoumei.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://kds.xuanzx.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://nzj.chenlongwang.top

Java: // 无：用 Builder 模式或 record
来源：http://xql.yongpay.top

Go:   // 无：用配置结构体参数
来源：http://yel.9152youxi.cn

Ruby: f(a: 1, b: 2)
来源：http://rxn.zhengqikj.top

C#:   f(a: 1, b: 2)
来源：http://tzb.fanxiaobao.xyz

[C05] 返回多个值
来源：http://iiw.wangdashe.top

Py:   return a, b
来源：http://irf.guannengcc.top

PHP:  return [$a, $b];
来源：http://ekf.vehdjk.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://bgz.sysykeji.top

TS:   return { a, b };
来源：http://jyt.shanyushiyangtech.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://lrk.tanke756.top

Go:   return a, b
来源：http://dws.sjlbkw.cn

Ruby: return a, b
来源：http://vhe.cucudq.cn

C#:   return (a, b);              // ValueTuple
来源：http://kcf.kuanghao11.cn

[C06] 匿名函数 / lambda
来源：http://oqy.zhongyouzk.top

Py:   square = lambda x: x * x
来源：http://rqb.sxryk.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://qvl.pycfn.com

JS:   const square = x => x * x;
来源：http://lfz.nanxinkj.top

TS:   const square = (x: number): number => x * x;
来源：http://aax.gogol.net.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://gmf.ctjpmb.com

Go:   sq := func(x int) int { return x * x }
来源：http://qmn.yfazqb.com

Ruby: square = ->(x) { x * x }
来源：http://dvh.pengpengdd.cyou

C#:   Func<int, int> square = x => x * x;
来源：http://qaf.sysykeji.top

[C07] 把函数作为参数传入
来源：http://tzk.pycfn.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://xpd.jyoumei.cn

PHP:  array_map("strtoupper", $arr);
来源：http://nul.zycfv.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://vco.sufxvd.cn

TS:   arr.map(String)
来源：http://pcc.tianlin.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://vca.sysykeji.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wie.jianghu66.top

Ruby: arr.map(&:upcase)
来源：http://jdj.svipenyu.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://poi.smart0.xyz

[C08] 闭包
来源：http://hgf.cashguo.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://sry.bbcook.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://gkv.tian-w.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wsk.svipenyu.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://kgb.ppjwa.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://zar.ehwqpu.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://dqz.zhongyouzk.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mqt.jinghuilouyu.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://irq.yonumen.top

[C09] 递归
来源：http://imf.cucudq.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://dqh.shangyingyoupin.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://xfb.zhengqikj.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ldz.jinqigufen.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fzd.meibo888.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ffv.dianchejie.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://snk.yanxiufei.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://fwb.hywenlv.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://xei.jinyuanbaomall.cn

[C10] 变量作用域
来源：http://wym.jqgufenzy.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://vfg.hysaishi.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://jgg.hywenlv.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://tfg.svipenyu.cn

TS:   同 JS
来源：http://ehe.jlsjyb.cn

Java: 方法内为块级作用域
来源：http://wby.fanxiaobao.xyz

Go:   花括号块级作用域
来源：http://ssm.sjlbkw.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://uwu.tanke756.top

C#:   块级作用域
来源：http://xtk.vehdjk.com

[C11] 模块导入与导出
来源：http://liv.chenjidiqi.icu

Py:   from module import func
来源：http://djd.zhengqikj.top

PHP:  require "file.php";  或 use App\Service;
来源：http://tyn.9152youxi.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://rla.zhengqikj.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://rvu.shzxlz.cn

Java: import java.util.List;
来源：http://flp.cheryme.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://vvw.yj20258888.top

Ruby: require "json"; require_relative "./util"
来源：http://eoq.cashguo.top

C#:   using System.Text;
来源：http://tim.ctjpmb.com

[C12] 立即执行函数 IIFE
来源：http://tbc.tian-w.cn

Py:   (lambda: print("run"))()
来源：http://hcy.xinyue.icu

PHP:  (function () { echo "run"; })();
来源：http://cko.pycfn.com

JS:   (() => { console.log("run"); })();
来源：http://bxr.cheryme.top

TS:   (() => { console.log("run"); })();
来源：http://bis.ppjwa.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hbe.epnwcf.com

Go:   func() { fmt.Println("run") }()
来源：http://jpn.chenjidiqi.icu

Ruby: -> { puts "run" }.call
来源：http://cjc.snrcjt.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://kby.cucudq.cn

[C13] 类型声明 / 类型注解
来源：http://hzs.smart0.xyz

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://foy.hywenlv.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ozd.gotoacloud.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://khy.vehdjk.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ieo.sweek.top

Java: int add(int a, int b) { return a + b; }
来源：http://grf.iojbl.cn

Go:   func add(a, b int) int
来源：http://yii.yongpay.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://buo.sxryk.cn

C#:   int Add(int a, int b) => a + b;
来源：http://qpy.svipenyu.cn

[C14] 泛型函数
来源：http://ura.wangshuangyany.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://rra.hnqzz.top

PHP:  // 无泛型
来源：http://mbi.cashguo.top

JS:   // 无泛型
来源：http://igj.jqgufenzy.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://roa.yvedp.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://qgt.nwbrower.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://qpq.jinqigfzy.top

Ruby: # 无泛型
来源：http://qxl.haohaochexian.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://rwp.zhixingplan.top

[C15] 解构 / 展开参数
来源：http://ycb.ctjpmb.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://dhk.zhoulong.xyz

PHP:  [$a, $b] = $pair;
来源：http://zqe.yuanzhike.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://upf.jianghu66.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wbz.zhaomingkeji.xyz

Java: // 无解构
来源：http://rxr.52xcode.cn

Go:   // 无解构
来源：http://jjn.fzhhl.top

Ruby: a, b = pair
来源：http://hlu.aizwys.cn

C#:   var (a, b) = pair;
来源：http://nns.shangyingyoupin.top

[C16] 函数 / 方法重载
来源：http://rbk.fehbvm.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://twj.zdbjq.cn

PHP:  // 无重载
来源：http://dvq.dashuyun.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://cbz.zhoulong.xyz

TS:   // 用联合类型或重载签名声明
来源：http://inp.yonumen.top

Java: void f(int a) {}  void f(String a) {}
来源：http://ncj.smart0.xyz

Go:   // 无重载：用不同函数名
来源：http://lwd.shangyingyoupin.top

Ruby: # 无重载：靠动态参数
来源：http://xoe.fktsv.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://hlx.fehbvm.com

================================================================================
来源：http://ioo.jinghuilouyu.cn

D. 数组 / 列表 / 集合
来源：http://uzo.yfazqb.com

================================================================================
来源：http://hku.nanxinkj.top

[D01] 创建数组 / 列表
来源：http://idf.meibo888.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://dyd.bbcook.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mwe.vqdsnc.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://oky.yongpay.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://hoo.gogol.net.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ixf.gzhubu.top

Go:   arr := []int{1, 2, 3}
来源：http://xxq.tanke756.top

Ruby: arr = [1, 2, 3]
来源：http://iaa.gaohongyu789.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://rhi.dianchejie.cn

[D02] 追加元素到末尾
来源：http://odv.zhoulong.xyz

Py:   arr.append(4); arr.extend([5, 6])
来源：http://lvv.gaohongyu789.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://eze.vqdsnc.cn

JS:   arr.push(4);
来源：http://rvb.epnwcf.com

TS:   arr.push(4);
来源：http://enp.daria6918.cn

Java: list.add(4);
来源：http://dnt.tarul.cn

Go:   arr = append(arr, 4)
来源：http://euh.svipenyu.cn

Ruby: arr << 4; arr.push(5)
来源：http://evx.9152youxi.cn

C#:   list.Add(4);
来源：http://mzd.hfpthk.cn

[D03] 在指定位置插入元素
来源：http://alf.cheryme.top

Py:   arr.insert(0, 0)
来源：http://rdn.hywenlv.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://zvc.aibaodan.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://lrc.yuxming.cn

TS:   arr.splice(0, 0, 0);
来源：http://thq.kuanghao11.cn

Java: list.add(0, 0);
来源：http://erc.gotoacloud.top

Go:   arr = append([]int{0}, arr...)
来源：http://xwf.guannengcc.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ktk.daxiang520.top

C#:   list.Insert(0, 0);
来源：http://xzo.jqgufenzy.top

[D04] 删除元素
来源：http://sic.shuidangran.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://jel.fehbvm.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://llw.tian-w.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://yow.yongpay.top

TS:   arr.splice(0, 1);
来源：http://ceb.ehwqpu.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://fbi.hysaishi.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://fem.hongshengwenyu.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://nrs.sysykeji.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://kcn.yonumen.top

[D05] 访问与修改元素
来源：http://feg.jqgufenzy.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://irj.guowangkeji.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://xmt.yj20258.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://tvh.hesvh.cn

TS:   arr[0]; arr.at(-1);
来源：http://hdw.ydzc1.top

Java: list.get(0); list.set(0, 9);
来源：http://pon.yj20258888.top

Go:   arr[0]; arr[0] = 9
来源：http://gen.jinqigfzy.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://boc.aizwys.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://gnw.xuanzx.com

[D06] 数组长度
来源：http://skm.shanyushiyangkeji.top

Py:   len(arr)
来源：http://czf.pengpengdd.cyou

PHP:  count($arr);
来源：http://mjf.yongpay.top

JS:   arr.length
来源：http://kew.tarul.cn

TS:   arr.length
来源：http://tmy.jlsjyb.cn

Java: list.size();
来源：http://hxa.jianghu66.top

Go:   len(arr)
来源：http://stp.yongpay.top

Ruby: arr.length; arr.size
来源：http://rwv.zhijiandao.cn

C#:   list.Count;
来源：http://ken.vehdjk.com

[D07] 切片 / 取子数组
来源：http://wyu.aizwys.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://rkq.hywenlv.cn

PHP:  array_slice($arr, 1, 3);
来源：http://yet.wangdashe.top

JS:   arr.slice(1, 4);
来源：http://ppm.zdqjudy.top

TS:   arr.slice(1, 4);
来源：http://wnj.nanxinkj.top

Java: list.subList(1, 4);
来源：http://hzw.yanxiufei.cn

Go:   arr[1:4]
来源：http://emc.shanyushiyangkeji.top

Ruby: arr[1, 3]
来源：http://lbj.shuidangran.top

C#:   list.GetRange(1, 3);
来源：http://jiw.ppjwa.cn

[D08] 合并两个数组
来源：http://lze.jqgufenzy.top

Py:   a + b;  a.extend(b)
来源：http://mhf.zhengqikj.top

PHP:  array_merge($a, $b);
来源：http://dof.zhixingplan.top

JS:   [...a, ...b];  a.concat(b);
来源：http://xto.uphjek.com

TS:   [...a, ...b];
来源：http://dla.gotoacloud.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://djv.zdbjq.cn

Go:   append(a, b...)
来源：http://onp.shanyushiyangtech.top

Ruby: a + b;  a.concat(b)
来源：http://pba.cqqwz.cn

C#:   a.Concat(b).ToList()
来源：http://nef.smart0.xyz

[D09] 排序（升序）
来源：http://tbg.kuanghao11.cn

Py:   sorted(arr);  arr.sort()
来源：http://peg.sxryk.cn


<!-- 参考信息 -->