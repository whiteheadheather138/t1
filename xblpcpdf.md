代发 wailian999

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qeg.hnqzz.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://aex.hongshengwenyu.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://bzc.chenjidiqi.icu

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wsu.guowangkeji.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://jne.zhiwuduotai.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://dua.xylfe.cn

[B07] while 循环
来源：http://wdb.chenzaomai.com

Py:   while i < 10: i += 1
来源：http://yea.chenjidiqi.icu

PHP:  while ($i < 10) { $i++; }
来源：http://wse.snrcjt.cn

JS:   while (i < 10) { i++; }
来源：http://pzs.ydzc1.top

TS:   while (i < 10) { i++; }
来源：http://gnq.jiagoushi.top

Java: while (i < 10) { i++; }
来源：http://hwh.tian-w.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hdx.ehwqpu.com

Ruby: while i < 10; i += 1; end
来源：http://gho.kuanghao11.cn

C#:   while (i < 10) { i++; }
来源：http://svp.iojbl.cn

[B08] do-while（至少执行一次）
来源：http://sik.bjfxy.top

Py:   # 无 do-while：用 while True + break
来源：http://dfg.hnxiangtu.top

PHP:  do { $i++; } while ($i < 10);
来源：http://oeh.gzhubu.top

JS:   do { i++; } while (i < 10);
来源：http://kjd.sxryk.cn

TS:   do { i++; } while (i < 10);
来源：http://jja.aibaodan.cn

Java: do { i++; } while (i < 10);
来源：http://pzm.guannengcc.top

Go:   for { i++; if i >= 10 { break } }
来源：http://qea.tian-w.cn

Ruby: begin; i += 1; end while i < 10
来源：http://pon.fehbvm.com

C#:   do { i++; } while (i < 10);
来源：http://mxq.316326.xyz

[B09] break 与 continue
来源：http://lvt.vqdsnc.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ofp.yuanzhike.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://grc.gaohongyu789.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hit.shangyingyoupin.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://snv.ywan-chungtsiang.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pcg.kuanghao11.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://cdr.xylfe.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://jro.cucudq.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kzw.yuanzhike.top

[B10] 遍历同时拿索引
来源：http://xhs.yanxiufei.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://exp.sufxvd.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://avr.jqgfzy.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://srh.nwbrower.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hpj.meibo888.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://epx.redwolf501.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://kjw.daria6918.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://rqu.birdmap.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://qoe.gotoacloud.top

[B11] 生成数字序列 / 区间
来源：http://eom.xuetiantiany.cn

Py:   list(range(0, 10, 2))
来源：http://avr.yonumen.top

PHP:  range(0, 10, 2);
来源：http://zgp.cqqwz.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ezl.hesvh.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zip.kuanghao11.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hoq.chenzaomai.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://qxb.daxiang520.top

Ruby: (0...10).step(2).to_a
来源：http://jgo.xuetiantiany.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://yjc.fehbvm.com

[B12] 跳出多层循环
来源：http://yxo.sweek.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://sxt.zycfv.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://txx.gaohongyu789.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://yfv.gaohongyu789.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://jby.jinqigufen.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ggt.hammf.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://yzm.dashuyun.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://rdj.fzhhl.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://kzk.fengsongda.top

[B13] 判断是否为数字
来源：http://kqz.zhiwuduotai.top

Py:   isinstance(x, (int, float))
来源：http://crs.yangfankeji.com

PHP:  is_numeric($x)
来源：http://ymf.havefunace.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://oko.xylfe.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qek.yueranfly.top

Java: x instanceof Number
来源：http://isg.jianghu66.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://nol.yj20258888.top

Ruby: x.is_a?(Numeric)
来源：http://ecl.pycfn.com

C#:   x is int or double or decimal
来源：http://tfp.ybcxt.top

[B14] 判断值是否在集合内
来源：http://jjm.hnxiangtu.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://tuf.yj202588.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://goc.iojbl.cn

JS:   [1, 2, 3].includes(x)
来源：http://ivz.nwbrower.top

TS:   [1, 2, 3].includes(x)
来源：http://lqu.jinqigfzy.top

Java: List.of(1, 2, 3).contains(x)
来源：http://tjd.jlsjyb.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wbi.hnqzz.top

Ruby: [1, 2, 3].include?(x)
来源：http://rnh.dashuyun.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://yam.vqdsnc.cn

[B15] 布尔运算与取反
来源：http://kdt.wangdashe.top

Py:   a and b or not c
来源：http://wea.ydjk.org.cn

PHP:  $a && $b || !$c
来源：http://psi.cheryme.top

JS:   a && b || !c
来源：http://hbg.tian-w.cn

TS:   a && b || !c
来源：http://sxr.nanxuanxn.top

Java: a && b || !c
来源：http://qao.fehbvm.com

Go:   a && b || !c
来源：http://lsm.jlsjyb.cn

Ruby: a && b || !c
来源：http://hig.birdmap.top

C#:   a && b || !c
来源：http://iqy.quarkkingdee.top

[B16] 卫语句：不满足条件提前返回
来源：http://yrh.pengpengdd.cyou

Py:   if not data: return
来源：http://gar.nwbrower.top

PHP:  if (!$data) { return; }
来源：http://jdl.sufxvd.cn

JS:   if (!data) return;
来源：http://vfu.hcnkem.com

TS:   if (!data) return;
来源：http://vcj.52xcode.cn

Java: if (data == null) return;
来源：http://ber.jianghu66.top

Go:   if data == nil { return }
来源：http://ugz.316326.xyz

Ruby: return if data.nil?
来源：http://wma.zycfv.cn

C#:   if (data == null) return;
来源：http://grk.xinyue.icu

================================================================================
来源：http://fas.ybcxt.top

C. 函数与作用域
来源：http://kot.kuanghao11.cn

================================================================================
来源：http://hfr.zdqjudy.top

[C01] 定义函数
来源：http://apm.vehdjk.com

Py:   def add(a, b): return a + b
来源：http://rul.hongshengwenyu.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xry.jlsjyb.cn

JS:   function add(a, b) { return a + b; }
来源：http://nqg.jqgufenzy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fgg.vehdjk.com

Java: static int add(int a, int b) { return a + b; }
来源：http://zve.svipenyu.cn

Go:   func add(a, b int) int { return a + b }
来源：http://sps.snrcjt.cn

Ruby: def add(a, b); a + b; end
来源：http://yug.fehbvm.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mgo.tianlin.xyz

[C02] 默认参数
来源：http://dof.zdbjq.cn

Py:   def greet(name="World"): return name
来源：http://wvr.sufxvd.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://aqa.hfpthk.cn

JS:   function greet(name = "World") { return name; }
来源：http://yuo.jqgfzy.top

TS:   function greet(name: string = "World") { return name; }
来源：http://viq.mhx1999.top

Java: // 无默认参数：方法重载或 Optional
来源：http://slm.redwolf501.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://von.jinghuilouyu.cn

Ruby: def greet(name = "World") = name
来源：http://uqg.yueranfly.top

C#:   string Greet(string name = "World") => name;
来源：http://mqj.wangdashe.top

[C03] 可变参数
来源：http://xbe.bbcook.cn

Py:   def total(*args): return sum(args)
来源：http://vys.zhengqikj.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://swi.nanxuanxn.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://tyl.daria6918.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xym.yuxming.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hxv.cheryme.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://pkt.jqgfzy.top

Ruby: def total(*nums); nums.sum; end
来源：http://rgl.hnqzz.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://jru.feifeiyinyue.top

[C04] 命名参数 / 关键字参数
来源：http://ihn.feifeiyinyue.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://lfq.ybcxt.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://szx.9152youxi.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mgs.svipenyu.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xcs.jinghuilouyu.cn

Java: // 无：用 Builder 模式或 record
来源：http://icy.nwbrower.top

Go:   // 无：用配置结构体参数
来源：http://teu.hywenlv.cn

Ruby: f(a: 1, b: 2)
来源：http://zov.aibaodan.cn

C#:   f(a: 1, b: 2)
来源：http://xuv.iojbl.cn

[C05] 返回多个值
来源：http://igr.yanxiufei.cn

Py:   return a, b
来源：http://sie.guowangkeji.top

PHP:  return [$a, $b];
来源：http://uas.ivvv.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://vul.pengpengdd.cyou

TS:   return { a, b };
来源：http://kea.hnxiangtu.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://jrm.ybcxt.top

Go:   return a, b
来源：http://mkm.redwolf501.top

Ruby: return a, b
来源：http://jyu.jlsjyb.cn

C#:   return (a, b);              // ValueTuple
来源：http://vov.dashuyun.cn

[C06] 匿名函数 / lambda
来源：http://vyw.daria6918.cn

Py:   square = lambda x: x * x
来源：http://hdg.tanke756.top

PHP:  $square = fn($x) => $x * $x;
来源：http://bkx.hongshengwenyu.top

JS:   const square = x => x * x;
来源：http://kpe.xingfuxueyuan.xyz

TS:   const square = (x: number): number => x * x;
来源：http://eup.sxryk.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://vvl.vqdsnc.cn

Go:   sq := func(x int) int { return x * x }
来源：http://zkx.jianghu66.top

Ruby: square = ->(x) { x * x }
来源：http://llj.daxiang520.top

C#:   Func<int, int> square = x => x * x;
来源：http://tfi.fanxiaobao.xyz

[C07] 把函数作为参数传入
来源：http://jhe.zhixingplan.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hpg.zhijiandao.cn

PHP:  array_map("strtoupper", $arr);
来源：http://bmx.fzhhl.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://vvz.uphjek.com

TS:   arr.map(String)
来源：http://ehc.wangshuangyany.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wiq.xinyue.icu

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ixw.xuetiantiany.cn

Ruby: arr.map(&:upcase)
来源：http://qdm.guannengcc.top

C#:   arr.Select(s => s.ToUpper())
来源：http://yxh.yangfankeji.com

[C08] 闭包
来源：http://jjm.yuxming.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://lqx.tianlin.xyz

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wde.andypj.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://kra.yvedp.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://onw.zhiwuduotai.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://fnc.uphjek.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://xgy.guowangkeji.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://obm.wangdashe.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://qok.mhx1999.top

[C09] 递归
来源：http://atr.ctjpmb.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://bwu.zhongyouzk.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hse.52xcode.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nqy.yuanzhike.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://oyz.daxiang520.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wca.zhiwuduotai.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://xvg.gogol.net.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mcd.andypj.xyz

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://qmc.jinqigufen.top

[C10] 变量作用域
来源：http://hak.sweek.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://icw.kuanghao11.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ytr.hysaishi.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://eyb.cqqwz.cn

TS:   同 JS
来源：http://gca.zdbjq.cn

Java: 方法内为块级作用域
来源：http://cmh.jinqigfzy.top

Go:   花括号块级作用域
来源：http://igp.bjfxy.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ldk.ppjwa.cn

C#:   块级作用域
来源：http://tal.hfpthk.cn

[C11] 模块导入与导出
来源：http://vid.redwolf501.top

Py:   from module import func
来源：http://vnx.daria6918.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://dma.0kj1m.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://bso.yangfankeji.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://yas.gotoacloud.top

Java: import java.util.List;
来源：http://naa.bjfxy.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://geo.xziqi.cn

Ruby: require "json"; require_relative "./util"
来源：http://dlu.jinyuanbaomall.cn

C#:   using System.Text;
来源：http://luk.zhongyouzk.top

[C12] 立即执行函数 IIFE
来源：http://hun.dianchejie.cn

Py:   (lambda: print("run"))()
来源：http://vnr.yfazqb.com

PHP:  (function () { echo "run"; })();
来源：http://ajz.zhiwuduotai.top

JS:   (() => { console.log("run"); })();
来源：http://gzo.nanxinkj.top

TS:   (() => { console.log("run"); })();
来源：http://erk.vqdsnc.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mhs.uphjek.com

Go:   func() { fmt.Println("run") }()
来源：http://mmp.yvedp.cn

Ruby: -> { puts "run" }.call
来源：http://dvw.gzhubu.top

C#:   // 无 IIFE：用静态构造函数
来源：http://whs.ivvv.top

[C13] 类型声明 / 类型注解
来源：http://qfk.xylfe.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://gej.tianlin.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qbk.sjlbkw.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://nuk.ydzc1.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mhk.yj202588.top

Java: int add(int a, int b) { return a + b; }
来源：http://qlw.jinghuilouyu.cn

Go:   func add(a, b int) int
来源：http://zrz.epnwcf.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://bxb.fzhhl.top

C#:   int Add(int a, int b) => a + b;
来源：http://wwd.snrcjt.cn

[C14] 泛型函数
来源：http://vwf.yueranfly.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://dsr.quarkkingdee.top

PHP:  // 无泛型
来源：http://cze.jqgufenzy.top

JS:   // 无泛型
来源：http://jhp.sysykeji.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://qbf.yuanzhike.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://byz.0kj1m.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://tyy.sweek.top

Ruby: # 无泛型
来源：http://hfe.zhixingplan.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://uos.hywenlv.cn

[C15] 解构 / 展开参数
来源：http://lqz.jinqigufen.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xbd.hnqzz.top

PHP:  [$a, $b] = $pair;
来源：http://qdv.nanxuanxn.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://jvr.hywenlv.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://efi.cqqwz.cn

Java: // 无解构
来源：http://zoa.jyoumei.cn

Go:   // 无解构
来源：http://zeu.fzhhl.top

Ruby: a, b = pair
来源：http://rem.zdbjq.cn

C#:   var (a, b) = pair;
来源：http://aal.yangfankeji.com

[C16] 函数 / 方法重载
来源：http://ifg.yfazqb.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://rrb.zhiwuduotai.top

PHP:  // 无重载
来源：http://rny.fanxiaobao.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://jmn.wangshuangyany.cn

TS:   // 用联合类型或重载签名声明
来源：http://saq.tian-w.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ufs.yangfankeji.com

Go:   // 无重载：用不同函数名
来源：http://hve.sjlbkw.cn

Ruby: # 无重载：靠动态参数
来源：http://qrw.svipenyu.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://hkw.0kj1m.cn

================================================================================
来源：http://gjh.daxiang520.top

D. 数组 / 列表 / 集合
来源：http://did.bbcook.cn

================================================================================
来源：http://fqz.fanxiaobao.xyz

[D01] 创建数组 / 列表
来源：http://fvf.zhijiandao.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ggl.hywenlv.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://zyk.jinghuilouyu.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://qzt.52xcode.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://wig.chenzaomai.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://icz.ydzc1.top

Go:   arr := []int{1, 2, 3}
来源：http://kda.zhixingplan.top

Ruby: arr = [1, 2, 3]
来源：http://quf.quarkkingdee.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://izy.zhixingplan.top

[D02] 追加元素到末尾
来源：http://tpv.zdbjq.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://qup.316326.xyz

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://qrd.zhiwuduotai.top

JS:   arr.push(4);
来源：http://iyv.hesvh.cn

TS:   arr.push(4);
来源：http://cyh.nwbrower.top

Java: list.add(4);
来源：http://upx.hongshengwenyu.top

Go:   arr = append(arr, 4)
来源：http://mtx.yanxiufei.cn

Ruby: arr << 4; arr.push(5)
来源：http://bqf.epnwcf.com

C#:   list.Add(4);
来源：http://wuy.gotoacloud.top

[D03] 在指定位置插入元素
来源：http://hmi.xziqi.cn

Py:   arr.insert(0, 0)
来源：http://zvd.epnwcf.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ygk.nanxinkj.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://dqn.hesvh.cn

TS:   arr.splice(0, 0, 0);
来源：http://ecj.hysaishi.cn

Java: list.add(0, 0);
来源：http://lej.hcnkem.com

Go:   arr = append([]int{0}, arr...)
来源：http://phw.yvedp.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://pmf.sufxvd.cn

C#:   list.Insert(0, 0);
来源：http://mvh.jinqigufen.top

[D04] 删除元素
来源：http://cir.ehwqpu.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ozz.chenjidiqi.icu

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://qiw.andypj.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://vol.zhoulong.xyz

TS:   arr.splice(0, 1);
来源：http://iow.52xcode.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://rgx.ybcxt.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://vyv.snrcjt.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://avw.zhijiandao.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://bpx.birdmap.top

[D05] 访问与修改元素
来源：http://izf.daxiang520.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://dui.zhixingplan.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://sfz.nwbrower.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://tae.zhijiandao.cn

TS:   arr[0]; arr.at(-1);
来源：http://eya.nanxuanxn.top

Java: list.get(0); list.set(0, 9);
来源：http://jwq.ywan-chungtsiang.top

Go:   arr[0]; arr[0] = 9
来源：http://qen.ybcxt.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://qwt.vehdjk.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://toh.hysaishi.cn

[D06] 数组长度
来源：http://wox.jlsjyb.cn

Py:   len(arr)
来源：http://pyp.chenlongwang.top

PHP:  count($arr);
来源：http://iis.gogol.net.cn

JS:   arr.length
来源：http://wrn.ybcxt.top

TS:   arr.length
来源：http://wun.zdbjq.cn

Java: list.size();
来源：http://fpf.yanxiufei.cn

Go:   len(arr)
来源：http://hlo.andypj.xyz

Ruby: arr.length; arr.size
来源：http://vrd.yj20258.top

C#:   list.Count;
来源：http://jmw.tian-w.cn


<!-- 参考信息 -->