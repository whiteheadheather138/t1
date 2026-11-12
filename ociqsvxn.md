代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://iau.fktsv.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://bxl.ehwqpu.com

JS:   do { i++; } while (i < 10);
来源：http://fld.xinyue.icu

TS:   do { i++; } while (i < 10);
来源：http://del.guannengcc.top

Java: do { i++; } while (i < 10);
来源：http://cme.shuidangran.top

Go:   for { i++; if i >= 10 { break } }
来源：http://cmt.aibaodan.cn

Ruby: begin; i += 1; end while i < 10
来源：http://fzm.nwbrower.top

C#:   do { i++; } while (i < 10);
来源：http://xse.52xcode.cn

[B09] break 与 continue
来源：http://oso.yuxming.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://muk.zhengqikj.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://tvy.zhijiandao.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://til.quarkkingdee.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qsw.sxryk.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ibe.hywenlv.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://qac.52xcode.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://gcc.ydzc1.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dtr.gotoacloud.top

[B10] 遍历同时拿索引
来源：http://fsf.hongshengwenyu.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://srm.fzhhl.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://bmc.ybcxt.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://brt.sufxvd.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://osr.cdnleiting.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://rja.snrcjt.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://tsj.sjlbkw.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://tuu.hfpthk.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://fhr.yj20258.top

[B11] 生成数字序列 / 区间
来源：http://uig.hesvh.cn

Py:   list(range(0, 10, 2))
来源：http://iyc.zdqjudy.top

PHP:  range(0, 10, 2);
来源：http://ztv.jinqigfzy.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dzu.xuetiantiany.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ixb.yuxming.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://sfw.wangdashe.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://paa.nwbrower.top

Ruby: (0...10).step(2).to_a
来源：http://yiw.uphjek.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://uuh.52xcode.cn

[B12] 跳出多层循环
来源：http://zve.cucudq.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://rsn.shzxlz.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://kky.hammf.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hlv.jinqigfzy.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wtg.chenlongwang.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://yjz.birdmap.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mzk.chenzaomai.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://efh.chenzaomai.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://jjl.xylfe.cn

[B13] 判断是否为数字
来源：http://opp.hongshengwenyu.top

Py:   isinstance(x, (int, float))
来源：http://bcy.chenjidiqi.icu

PHP:  is_numeric($x)
来源：http://hax.shanyushiyangkeji.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ltg.bbcook.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://aqf.shzxlz.cn

Java: x instanceof Number
来源：http://lhw.tarul.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://vbm.snrcjt.cn

Ruby: x.is_a?(Numeric)
来源：http://got.fzhhl.top

C#:   x is int or double or decimal
来源：http://ikj.shzxlz.cn

[B14] 判断值是否在集合内
来源：http://xer.andypj.xyz

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://myx.52xcode.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://igu.dashuyun.cn

JS:   [1, 2, 3].includes(x)
来源：http://hgu.quarkkingdee.top

TS:   [1, 2, 3].includes(x)
来源：http://qfl.jyoumei.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://sbr.ywan-chungtsiang.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://vyd.pycfn.com

Ruby: [1, 2, 3].include?(x)
来源：http://juj.fehbvm.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ghl.ybcxt.top

[B15] 布尔运算与取反
来源：http://kth.xziqi.cn

Py:   a and b or not c
来源：http://iwm.nwbrower.top

PHP:  $a && $b || !$c
来源：http://ghn.feifeiyinyue.top

JS:   a && b || !c
来源：http://klh.gotoacloud.top

TS:   a && b || !c
来源：http://fkt.yj20258888.top

Java: a && b || !c
来源：http://fri.haohaochexian.top

Go:   a && b || !c
来源：http://uch.zhoulong.xyz

Ruby: a && b || !c
来源：http://obh.wangdashe.top

C#:   a && b || !c
来源：http://sxn.hcnkem.com

[B16] 卫语句：不满足条件提前返回
来源：http://mbs.ydzc1.top

Py:   if not data: return
来源：http://nht.tian-w.cn

PHP:  if (!$data) { return; }
来源：http://ojl.snrcjt.cn

JS:   if (!data) return;
来源：http://eme.jqgfzy.top

TS:   if (!data) return;
来源：http://hed.iojbl.cn

Java: if (data == null) return;
来源：http://bkw.hnqzz.top

Go:   if data == nil { return }
来源：http://qov.yj202588.top

Ruby: return if data.nil?
来源：http://jra.jinqigufen.top

C#:   if (data == null) return;
来源：http://biu.sjlbkw.cn

================================================================================
来源：http://ota.zhoulong.xyz

C. 函数与作用域
来源：http://kft.mhx1999.top

================================================================================
来源：http://jng.tanke756.top

[C01] 定义函数
来源：http://vli.jinqigfzy.top

Py:   def add(a, b): return a + b
来源：http://ofp.hcnkem.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ivt.iojbl.cn

JS:   function add(a, b) { return a + b; }
来源：http://ves.xuanzx.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lii.bbcook.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://rea.xuanzx.com

Go:   func add(a, b int) int { return a + b }
来源：http://kur.52xcode.cn

Ruby: def add(a, b); a + b; end
来源：http://xqf.chenzaomai.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ise.9152youxi.cn

[C02] 默认参数
来源：http://ptw.jiagoushi.top

Py:   def greet(name="World"): return name
来源：http://nsl.cucudq.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://azz.hammf.cn

JS:   function greet(name = "World") { return name; }
来源：http://aby.tarul.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://twj.sweek.top

Java: // 无默认参数：方法重载或 Optional
来源：http://pia.iojbl.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://tok.guowangkeji.top

Ruby: def greet(name = "World") = name
来源：http://sql.hywenlv.cn

C#:   string Greet(string name = "World") => name;
来源：http://ngr.tian-w.cn

[C03] 可变参数
来源：http://cmy.cqqwz.cn

Py:   def total(*args): return sum(args)
来源：http://kfr.xinyue.icu

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xlg.daria6918.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://xnv.nwbrower.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://qov.xylfe.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ndh.hywenlv.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://abo.yangfankeji.com

Ruby: def total(*nums); nums.sum; end
来源：http://woq.dianchejie.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://dik.snrcjt.cn

[C04] 命名参数 / 关键字参数
来源：http://txe.xingfuxueyuan.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://vqw.birdmap.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ppf.yangfankeji.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xcj.gotoacloud.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://zzr.hysaishi.cn

Java: // 无：用 Builder 模式或 record
来源：http://mru.uphjek.com

Go:   // 无：用配置结构体参数
来源：http://gcq.ehwqpu.com

Ruby: f(a: 1, b: 2)
来源：http://wjn.tarul.cn

C#:   f(a: 1, b: 2)
来源：http://unx.gzhubu.top

[C05] 返回多个值
来源：http://dhc.bbcook.cn

Py:   return a, b
来源：http://smm.quarkkingdee.top

PHP:  return [$a, $b];
来源：http://ghd.zhijiandao.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://tjv.wangshuangyany.cn

TS:   return { a, b };
来源：http://sxm.tanke756.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://aqq.c1oappe.top

Go:   return a, b
来源：http://hcp.gogol.net.cn

Ruby: return a, b
来源：http://bml.jqgfzy.top

C#:   return (a, b);              // ValueTuple
来源：http://zxy.shzxlz.cn

[C06] 匿名函数 / lambda
来源：http://jph.chenzaomai.com

Py:   square = lambda x: x * x
来源：http://fyb.ydjk.org.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://bxd.nanxinkj.top

JS:   const square = x => x * x;
来源：http://xcd.52xcode.cn

TS:   const square = (x: number): number => x * x;
来源：http://mie.wangshuangyany.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://lcr.316326.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://gzj.yueranfly.top

Ruby: square = ->(x) { x * x }
来源：http://khe.shangyingyoupin.top

C#:   Func<int, int> square = x => x * x;
来源：http://cos.ctjpmb.com

[C07] 把函数作为参数传入
来源：http://huc.hfpthk.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://qdl.shanyushiyangtech.top

PHP:  array_map("strtoupper", $arr);
来源：http://fow.hywenlv.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://jsj.shanyushiyangkeji.top

TS:   arr.map(String)
来源：http://hcq.52xcode.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ulj.52xcode.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://dti.zhongyouzk.top

Ruby: arr.map(&:upcase)
来源：http://mfi.tian-w.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://omy.yanxiufei.cn

[C08] 闭包
来源：http://abb.cheryme.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://iyw.hywenlv.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://dqp.shangyingyoupin.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://uts.zhengqikj.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hts.andypj.xyz

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://fwm.jinqigufen.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wmc.hesvh.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://xxs.hesvh.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://anu.ybcxt.top

[C09] 递归
来源：http://jrz.chenzaomai.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://eag.yongpay.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://pji.shanyushiyangtech.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jvw.jyoumei.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hkx.ydzc1.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ppx.jianghu66.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ltm.nanxuanxn.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ocv.tian-w.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hwe.fehbvm.com

[C10] 变量作用域
来源：http://uxs.nanxuanxn.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://yzo.xuanzx.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ugq.gogol.net.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://apa.tarul.cn

TS:   同 JS
来源：http://vvz.fengsongda.top

Java: 方法内为块级作用域
来源：http://wou.jyoumei.cn

Go:   花括号块级作用域
来源：http://oqm.0kj1m.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://lbk.yj20258.top

C#:   块级作用域
来源：http://dto.chenlongwang.top

[C11] 模块导入与导出
来源：http://qgt.svipenyu.cn

Py:   from module import func
来源：http://pgm.yj20258888.top

PHP:  require "file.php";  或 use App\Service;
来源：http://aas.tian-w.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://vqd.zhongyouzk.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://zbf.c1oappe.top

Java: import java.util.List;
来源：http://hoh.52xcode.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://nwu.meibo888.top

Ruby: require "json"; require_relative "./util"
来源：http://dcf.chenlongwang.top

C#:   using System.Text;
来源：http://lqw.gotoacloud.top

[C12] 立即执行函数 IIFE
来源：http://sua.xziqi.cn

Py:   (lambda: print("run"))()
来源：http://hrk.yj20258888.top

PHP:  (function () { echo "run"; })();
来源：http://alu.sufxvd.cn

JS:   (() => { console.log("run"); })();
来源：http://vlv.ydjk.org.cn

TS:   (() => { console.log("run"); })();
来源：http://blc.sweek.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://cvi.c1oappe.top

Go:   func() { fmt.Println("run") }()
来源：http://vwz.yangfankeji.com

Ruby: -> { puts "run" }.call
来源：http://zgt.cqqwz.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://acb.fzhhl.top

[C13] 类型声明 / 类型注解
来源：http://awk.jinqigufen.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://lkr.yonumen.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://few.yanxiufei.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://iza.0kj1m.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ufc.hammf.cn

Java: int add(int a, int b) { return a + b; }
来源：http://xlb.hnqzz.top

Go:   func add(a, b int) int
来源：http://ren.jyoumei.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://zrp.birdmap.top

C#:   int Add(int a, int b) => a + b;
来源：http://csy.smart0.xyz

[C14] 泛型函数
来源：http://kpk.zhaomingkeji.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://php.yvedp.cn

PHP:  // 无泛型
来源：http://rgs.wangshuangyany.cn

JS:   // 无泛型
来源：http://yka.shzxlz.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://vdf.xinyue.icu

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://npv.quarkkingdee.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ttz.nanxinkj.top

Ruby: # 无泛型
来源：http://aez.uphjek.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hsi.jiagoushi.top

[C15] 解构 / 展开参数
来源：http://bkk.yvedp.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://obt.c1oappe.top

PHP:  [$a, $b] = $pair;
来源：http://gvq.nanxinkj.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://cum.ydzc1.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://rli.yj20258.top

Java: // 无解构
来源：http://yli.daxiang520.top

Go:   // 无解构
来源：http://cri.hnqzz.top

Ruby: a, b = pair
来源：http://ycx.epnwcf.com

C#:   var (a, b) = pair;
来源：http://ptj.dianchejie.cn

[C16] 函数 / 方法重载
来源：http://yhi.pengpengdd.cyou

Py:   # 无重载：用默认参数或 *args 变通
来源：http://qnz.ctjpmb.com

PHP:  // 无重载
来源：http://jwp.chenzaomai.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://zsx.dashuyun.cn

TS:   // 用联合类型或重载签名声明
来源：http://jtt.daria6918.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://bwy.hcnkem.com

Go:   // 无重载：用不同函数名
来源：http://zej.yvedp.cn

Ruby: # 无重载：靠动态参数
来源：http://ebl.zhiwuduotai.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://sqf.c1oappe.top

================================================================================
来源：http://dqo.chenjidiqi.icu

D. 数组 / 列表 / 集合
来源：http://max.fehbvm.com

================================================================================
来源：http://sab.c1oappe.top

[D01] 创建数组 / 列表
来源：http://quq.jlsjyb.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://lap.daxiang520.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mkl.vqdsnc.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://jso.hnqzz.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://gwd.snrcjt.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://dja.jinghuilouyu.cn

Go:   arr := []int{1, 2, 3}
来源：http://fpk.fengsongda.top

Ruby: arr = [1, 2, 3]
来源：http://nsy.xylfe.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://whv.9152youxi.cn

[D02] 追加元素到末尾
来源：http://xfy.nwbrower.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://usr.yongpay.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://szn.gotoacloud.top

JS:   arr.push(4);
来源：http://idj.ctjpmb.com

TS:   arr.push(4);
来源：http://cff.andypj.xyz

Java: list.add(4);
来源：http://vsb.yj20258888.top

Go:   arr = append(arr, 4)
来源：http://emj.xziqi.cn

Ruby: arr << 4; arr.push(5)
来源：http://yqf.jyoumei.cn

C#:   list.Add(4);
来源：http://rtl.chenjidiqi.icu

[D03] 在指定位置插入元素
来源：http://yzh.sweek.top

Py:   arr.insert(0, 0)
来源：http://flo.yanxiufei.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://xvx.jinghuilouyu.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://dnx.9152youxi.cn

TS:   arr.splice(0, 0, 0);
来源：http://svg.pengpengdd.cyou

Java: list.add(0, 0);
来源：http://yns.vqdsnc.cn

Go:   arr = append([]int{0}, arr...)
来源：http://rvo.havefunace.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://qjs.cashguo.top

C#:   list.Insert(0, 0);
来源：http://cbi.fehbvm.com

[D04] 删除元素
来源：http://pvu.dashuyun.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://zho.yangfankeji.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://uqh.wangshuangyany.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://iwi.shzxlz.cn

TS:   arr.splice(0, 1);
来源：http://cxt.zhixingplan.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hbe.chenzaomai.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://lmc.gzhubu.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://rxe.xylfe.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://gyj.tianlin.xyz

[D05] 访问与修改元素
来源：http://ckf.hysaishi.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://gpn.ehwqpu.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://jra.kuanghao11.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ono.guowangkeji.top

TS:   arr[0]; arr.at(-1);
来源：http://lbh.quarkkingdee.top

Java: list.get(0); list.set(0, 9);
来源：http://xfa.zhaomingkeji.xyz

Go:   arr[0]; arr[0] = 9
来源：http://cvt.feifeiyinyue.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hmx.uphjek.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hxj.snrcjt.cn

[D06] 数组长度
来源：http://zte.chenjidiqi.icu

Py:   len(arr)
来源：http://hhr.jqgfzy.top

PHP:  count($arr);
来源：http://asi.cqqwz.cn

JS:   arr.length
来源：http://yiz.hywenlv.cn

TS:   arr.length
来源：http://mxf.zhengqikj.top

Java: list.size();
来源：http://lre.yuxming.cn

Go:   len(arr)
来源：http://jbc.xingfuxueyuan.xyz

Ruby: arr.length; arr.size
来源：http://yxq.nwbrower.top

C#:   list.Count;
来源：http://pvx.fanxiaobao.xyz

[D07] 切片 / 取子数组
来源：http://bxp.fehbvm.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://urr.shanyushiyangtech.top

PHP:  array_slice($arr, 1, 3);
来源：http://ozn.haohaochexian.top

JS:   arr.slice(1, 4);
来源：http://gjs.ydzc1.top

TS:   arr.slice(1, 4);
来源：http://fcf.sysykeji.top

Java: list.subList(1, 4);
来源：http://vke.yfazqb.com

Go:   arr[1:4]
来源：http://zwd.tarul.cn

Ruby: arr[1, 3]
来源：http://hes.wangshuangyany.cn

C#:   list.GetRange(1, 3);
来源：http://ruc.yueranfly.top

[D08] 合并两个数组
来源：http://cow.yuanzhike.top

Py:   a + b;  a.extend(b)
来源：http://ckm.shzxlz.cn

PHP:  array_merge($a, $b);
来源：http://utg.yfazqb.com

JS:   [...a, ...b];  a.concat(b);
来源：http://udc.yangfankeji.com

TS:   [...a, ...b];
来源：http://lmy.yuanzhike.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://kfz.daria6918.cn

Go:   append(a, b...)
来源：http://ahv.shangyingyoupin.top


<!-- 参考信息 -->