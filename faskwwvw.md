代发 wailian999

Java: do { i++; } while (i < 10);
来源：http://inz.vehdjk.com

Go:   for { i++; if i >= 10 { break } }
来源：http://lbq.ybcxt.top

Ruby: begin; i += 1; end while i < 10
来源：http://qmf.dashuyun.cn

C#:   do { i++; } while (i < 10);
来源：http://zhw.yangfankeji.com

[B09] break 与 continue
来源：http://hke.ivvv.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://bmy.c1oappe.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://nrs.ybcxt.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://liu.ehwqpu.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tyf.snrcjt.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://irm.hammf.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://afe.bjfxy.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://auq.yj20258.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kax.chenlongwang.top

[B10] 遍历同时拿索引
来源：http://awt.sweek.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://bck.jinghuilouyu.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://zus.cheryme.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://yyi.yangfankeji.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://zzj.jqgufenzy.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://gko.hysaishi.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wow.jinqigufen.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://gph.chenzaomai.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://heu.mhx1999.top

[B11] 生成数字序列 / 区间
来源：http://kqm.yangfankeji.com

Py:   list(range(0, 10, 2))
来源：http://zzt.vqdsnc.cn

PHP:  range(0, 10, 2);
来源：http://yhb.daxiang520.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cmv.sysykeji.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fyl.zdbjq.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://het.yuanzhike.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://qcj.svipenyu.cn

Ruby: (0...10).step(2).to_a
来源：http://eqb.hongshengwenyu.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ycz.zhixingplan.top

[B12] 跳出多层循环
来源：http://fqr.zhongyouzk.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://zou.hysaishi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://fdw.guowangkeji.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ctl.yanxiufei.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://yen.yuxming.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hct.feifeiyinyue.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://tug.guowangkeji.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://efe.yanxiufei.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ore.fengsongda.top

[B13] 判断是否为数字
来源：http://rky.cdnleiting.top

Py:   isinstance(x, (int, float))
来源：http://axq.shangyingyoupin.top

PHP:  is_numeric($x)
来源：http://bii.quarkkingdee.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://aiv.svipenyu.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mww.epnwcf.com

Java: x instanceof Number
来源：http://kcg.zhiwuduotai.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://syb.hesvh.cn

Ruby: x.is_a?(Numeric)
来源：http://lvp.yj20258.top

C#:   x is int or double or decimal
来源：http://eue.tianlin.xyz

[B14] 判断值是否在集合内
来源：http://rfg.cdnleiting.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ogo.xuetiantiany.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://rfn.shuidangran.top

JS:   [1, 2, 3].includes(x)
来源：http://gja.ywan-chungtsiang.top

TS:   [1, 2, 3].includes(x)
来源：http://qzn.yj20258.top

Java: List.of(1, 2, 3).contains(x)
来源：http://ucf.smart0.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://dcb.meibo888.top

Ruby: [1, 2, 3].include?(x)
来源：http://fxn.kuanghao11.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://bdd.cdnleiting.top

[B15] 布尔运算与取反
来源：http://iox.tanke756.top

Py:   a and b or not c
来源：http://hhm.jinghuilouyu.cn

PHP:  $a && $b || !$c
来源：http://kqm.ydjk.org.cn

JS:   a && b || !c
来源：http://rur.fengsongda.top

TS:   a && b || !c
来源：http://dzr.cqqwz.cn

Java: a && b || !c
来源：http://hyi.fanxiaobao.xyz

Go:   a && b || !c
来源：http://ttc.yongpay.top

Ruby: a && b || !c
来源：http://hwn.zhongyouzk.top

C#:   a && b || !c
来源：http://kym.jinghuilouyu.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ndr.52xcode.cn

Py:   if not data: return
来源：http://pzr.jqgfzy.top

PHP:  if (!$data) { return; }
来源：http://yao.snrcjt.cn

JS:   if (!data) return;
来源：http://pvu.cqqwz.cn

TS:   if (!data) return;
来源：http://fpf.chenjidiqi.icu

Java: if (data == null) return;
来源：http://epf.tarul.cn

Go:   if data == nil { return }
来源：http://quz.uphjek.com

Ruby: return if data.nil?
来源：http://jkw.sufxvd.cn

C#:   if (data == null) return;
来源：http://ovn.hfpthk.cn

================================================================================
来源：http://gmr.redwolf501.top

C. 函数与作用域
来源：http://vwi.sweek.top

================================================================================
来源：http://iou.316326.xyz

[C01] 定义函数
来源：http://fgv.uphjek.com

Py:   def add(a, b): return a + b
来源：http://gvd.dashuyun.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jpr.tanke756.top

JS:   function add(a, b) { return a + b; }
来源：http://dqw.bbcook.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ltr.snrcjt.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://jdw.yonumen.top

Go:   func add(a, b int) int { return a + b }
来源：http://bkt.zhijiandao.cn

Ruby: def add(a, b); a + b; end
来源：http://sfw.cdnleiting.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://zfl.jiagoushi.top

[C02] 默认参数
来源：http://swp.ctjpmb.com

Py:   def greet(name="World"): return name
来源：http://vbg.xinyue.icu

PHP:  function greet($name = "World") { return $name; }
来源：http://mnk.xingfuxueyuan.xyz

JS:   function greet(name = "World") { return name; }
来源：http://ldb.yuanzhike.top

TS:   function greet(name: string = "World") { return name; }
来源：http://kit.fengsongda.top

Java: // 无默认参数：方法重载或 Optional
来源：http://hcl.jqgufenzy.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://shi.gotoacloud.top

Ruby: def greet(name = "World") = name
来源：http://xlx.fehbvm.com

C#:   string Greet(string name = "World") => name;
来源：http://buy.yj20258.top

[C03] 可变参数
来源：http://lux.cucudq.cn

Py:   def total(*args): return sum(args)
来源：http://pzp.zhoulong.xyz

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wko.snrcjt.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wwj.kuanghao11.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://zel.ctjpmb.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ffb.xingfuxueyuan.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://yjf.xylfe.cn

Ruby: def total(*nums); nums.sum; end
来源：http://rye.hysaishi.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://sxw.zdbjq.cn

[C04] 命名参数 / 关键字参数
来源：http://vlg.jyoumei.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://syr.sjlbkw.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://lls.nanxinkj.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://cmt.sufxvd.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://kez.xylfe.cn

Java: // 无：用 Builder 模式或 record
来源：http://fuy.nanxinkj.top

Go:   // 无：用配置结构体参数
来源：http://tro.guowangkeji.top

Ruby: f(a: 1, b: 2)
来源：http://ogv.ywan-chungtsiang.top

C#:   f(a: 1, b: 2)
来源：http://yqa.xziqi.cn

[C05] 返回多个值
来源：http://gjt.zhiwuduotai.top

Py:   return a, b
来源：http://rar.hnqzz.top

PHP:  return [$a, $b];
来源：http://vlz.yuxming.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ewq.xziqi.cn

TS:   return { a, b };
来源：http://mlf.gotoacloud.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://dgd.hcnkem.com

Go:   return a, b
来源：http://kqt.hnqzz.top

Ruby: return a, b
来源：http://vuy.vehdjk.com

C#:   return (a, b);              // ValueTuple
来源：http://fvm.zhongyouzk.top

[C06] 匿名函数 / lambda
来源：http://viw.zdbjq.cn

Py:   square = lambda x: x * x
来源：http://jvl.sweek.top

PHP:  $square = fn($x) => $x * $x;
来源：http://wfl.tanke756.top

JS:   const square = x => x * x;
来源：http://tke.cqqwz.cn

TS:   const square = (x: number): number => x * x;
来源：http://iwr.yuanzhike.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://kjl.birdmap.top

Go:   sq := func(x int) int { return x * x }
来源：http://kwd.ehwqpu.com

Ruby: square = ->(x) { x * x }
来源：http://lti.316326.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://qty.xinyue.icu

[C07] 把函数作为参数传入
来源：http://ojr.zdqjudy.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ayj.zhoulong.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://hra.zycfv.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://euv.dashuyun.cn

TS:   arr.map(String)
来源：http://kbt.9152youxi.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://bak.cdnleiting.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://kzq.yj20258888.top

Ruby: arr.map(&:upcase)
来源：http://lbk.mhx1999.top

C#:   arr.Select(s => s.ToUpper())
来源：http://hbr.shangyingyoupin.top

[C08] 闭包
来源：http://ynb.hywenlv.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mum.52xcode.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://unk.zhaomingkeji.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mgx.yuxming.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ffb.shangyingyoupin.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://qpd.yfazqb.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wqg.yangfankeji.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://dit.tarul.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://dti.sjlbkw.cn

[C09] 递归
来源：http://lsr.epnwcf.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://fgt.meibo888.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ndc.yvedp.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://umk.jqgufenzy.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://usk.jinghuilouyu.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://geq.yueranfly.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://iqt.hysaishi.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://lrl.hongshengwenyu.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://pcm.aibaodan.cn

[C10] 变量作用域
来源：http://kok.feifeiyinyue.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://fps.xingfuxueyuan.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://jem.hnqzz.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://yxr.ehwqpu.com

TS:   同 JS
来源：http://fiv.hcnkem.com

Java: 方法内为块级作用域
来源：http://nnr.birdmap.top

Go:   花括号块级作用域
来源：http://buy.dashuyun.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mek.sufxvd.cn

C#:   块级作用域
来源：http://wjb.fehbvm.com

[C11] 模块导入与导出
来源：http://hcw.ppjwa.cn

Py:   from module import func
来源：http://jtc.zhoulong.xyz

PHP:  require "file.php";  或 use App\Service;
来源：http://nqv.nanxuanxn.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://wzx.jiagoushi.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://qdo.tarul.cn

Java: import java.util.List;
来源：http://ylj.yonumen.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://rsd.gaohongyu789.top

Ruby: require "json"; require_relative "./util"
来源：http://ywi.jlsjyb.cn

C#:   using System.Text;
来源：http://ocl.yonumen.top

[C12] 立即执行函数 IIFE
来源：http://udo.sxryk.cn

Py:   (lambda: print("run"))()
来源：http://mox.shangyingyoupin.top

PHP:  (function () { echo "run"; })();
来源：http://rvv.hongshengwenyu.top

JS:   (() => { console.log("run"); })();
来源：http://pnq.feifeiyinyue.top

TS:   (() => { console.log("run"); })();
来源：http://ueb.xziqi.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://bef.hfpthk.cn

Go:   func() { fmt.Println("run") }()
来源：http://npx.zhaomingkeji.xyz

Ruby: -> { puts "run" }.call
来源：http://bai.yueranfly.top

C#:   // 无 IIFE：用静态构造函数
来源：http://fwt.aizwys.cn

[C13] 类型声明 / 类型注解
来源：http://liw.kuanghao11.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://vfl.yj20258.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gir.bbcook.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://zac.jinyuanbaomall.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rqn.vqdsnc.cn

Java: int add(int a, int b) { return a + b; }
来源：http://sod.iojbl.cn

Go:   func add(a, b int) int
来源：http://btf.xingfuxueyuan.xyz

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mmh.ydjk.org.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ncm.jinqigufen.top

[C14] 泛型函数
来源：http://pqy.bbcook.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hby.meibo888.top

PHP:  // 无泛型
来源：http://joy.nwbrower.top

JS:   // 无泛型
来源：http://arv.zhongyouzk.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://qpr.316326.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://bwu.xingfuxueyuan.xyz

Go:   func First[T any](items []T) T { return items[0] }
来源：http://gzx.guannengcc.top

Ruby: # 无泛型
来源：http://xpr.vehdjk.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xmi.sjlbkw.cn

[C15] 解构 / 展开参数
来源：http://ytt.yj20258.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ium.kuanghao11.cn

PHP:  [$a, $b] = $pair;
来源：http://zdj.wangshuangyany.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://cca.gogol.net.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://bja.hammf.cn

Java: // 无解构
来源：http://xpt.svipenyu.cn

Go:   // 无解构
来源：http://vfv.vqdsnc.cn

Ruby: a, b = pair
来源：http://nfg.vehdjk.com

C#:   var (a, b) = pair;
来源：http://qvt.jianghu66.top

[C16] 函数 / 方法重载
来源：http://yfy.wangshuangyany.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://kxo.hnxiangtu.top

PHP:  // 无重载
来源：http://aqa.xylfe.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://roc.havefunace.top

TS:   // 用联合类型或重载签名声明
来源：http://yjl.zhoulong.xyz

Java: void f(int a) {}  void f(String a) {}
来源：http://pgu.havefunace.top

Go:   // 无重载：用不同函数名
来源：http://pht.birdmap.top

Ruby: # 无重载：靠动态参数
来源：http://yal.fktsv.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://bhs.gzhubu.top

================================================================================
来源：http://xmr.chenlongwang.top

D. 数组 / 列表 / 集合
来源：http://cdh.jinghuilouyu.cn

================================================================================
来源：http://qms.jianghu66.top

[D01] 创建数组 / 列表
来源：http://ptb.yj20258888.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://oud.gzhubu.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://yhh.hysaishi.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ydk.hcnkem.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://nre.chenlongwang.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://uma.jinqigfzy.top

Go:   arr := []int{1, 2, 3}
来源：http://igq.tanke756.top

Ruby: arr = [1, 2, 3]
来源：http://gpu.xuetiantiany.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://fmr.cucudq.cn

[D02] 追加元素到末尾
来源：http://tzy.ybcxt.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://foi.hnqzz.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://veq.hesvh.cn

JS:   arr.push(4);
来源：http://pgs.sysykeji.top

TS:   arr.push(4);
来源：http://zqs.yvedp.cn

Java: list.add(4);
来源：http://qvc.cdnleiting.top

Go:   arr = append(arr, 4)
来源：http://jee.cqqwz.cn

Ruby: arr << 4; arr.push(5)
来源：http://quk.hysaishi.cn

C#:   list.Add(4);
来源：http://alr.uphjek.com

[D03] 在指定位置插入元素
来源：http://utz.haohaochexian.top

Py:   arr.insert(0, 0)
来源：http://zxh.yangfankeji.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://cjf.0kj1m.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://jjo.zhoulong.xyz

TS:   arr.splice(0, 0, 0);
来源：http://ptf.jlsjyb.cn

Java: list.add(0, 0);
来源：http://ppv.uphjek.com

Go:   arr = append([]int{0}, arr...)
来源：http://pmh.uphjek.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://qlx.yangfankeji.com

C#:   list.Insert(0, 0);
来源：http://xli.gzhubu.top

[D04] 删除元素
来源：http://mdh.ppjwa.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ujm.yangfankeji.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://svh.jlsjyb.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://pbw.meibo888.top

TS:   arr.splice(0, 1);
来源：http://wxc.yfazqb.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://utq.fehbvm.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://eor.quarkkingdee.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://slw.zycfv.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://exl.jqgfzy.top

[D05] 访问与修改元素
来源：http://bvh.svipenyu.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://gpz.jianghu66.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://npx.cqqwz.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://duo.yueranfly.top

TS:   arr[0]; arr.at(-1);
来源：http://lce.ydzc1.top

Java: list.get(0); list.set(0, 9);
来源：http://nbi.pengpengdd.cyou

Go:   arr[0]; arr[0] = 9
来源：http://wpd.chenzaomai.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ljt.9152youxi.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wsi.redwolf501.top

[D06] 数组长度
来源：http://tws.nanxuanxn.top

Py:   len(arr)
来源：http://hgw.quarkkingdee.top

PHP:  count($arr);
来源：http://yyz.hywenlv.cn

JS:   arr.length
来源：http://lri.guowangkeji.top

TS:   arr.length
来源：http://nov.jqgufenzy.top

Java: list.size();
来源：http://pvr.chenzaomai.com

Go:   len(arr)
来源：http://dii.zhengqikj.top

Ruby: arr.length; arr.size
来源：http://rwh.dianchejie.cn

C#:   list.Count;
来源：http://ghw.chenjidiqi.icu

[D07] 切片 / 取子数组
来源：http://fgs.fzhhl.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qya.52xcode.cn

PHP:  array_slice($arr, 1, 3);
来源：http://olx.jinyuanbaomall.cn

JS:   arr.slice(1, 4);
来源：http://lzf.hcnkem.com

TS:   arr.slice(1, 4);
来源：http://kds.chenzaomai.com

Java: list.subList(1, 4);
来源：http://yuz.vqdsnc.cn

Go:   arr[1:4]
来源：http://slm.yongpay.top

Ruby: arr[1, 3]
来源：http://anv.haohaochexian.top

C#:   list.GetRange(1, 3);
来源：http://mhs.dianchejie.cn

[D08] 合并两个数组
来源：http://khe.haohaochexian.top

Py:   a + b;  a.extend(b)
来源：http://oeg.hongshengwenyu.top

PHP:  array_merge($a, $b);
来源：http://hak.tianlin.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://uhn.yongpay.top

TS:   [...a, ...b];
来源：http://uke.zhoulong.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://kbn.jianghu66.top

Go:   append(a, b...)
来源：http://dnj.xuetiantiany.cn

Ruby: a + b;  a.concat(b)
来源：http://hol.hesvh.cn

C#:   a.Concat(b).ToList()
来源：http://vim.pycfn.com

[D09] 排序（升序）
来源：http://rvm.cdnleiting.top

Py:   sorted(arr);  arr.sort()
来源：http://pfb.jinqigfzy.top


<!-- 参考信息 -->