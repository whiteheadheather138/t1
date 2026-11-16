代发 wailian999

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vbo.xylfe.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cxa.chenzaomai.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://rxu.zhijiandao.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://fve.316326.xyz

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://bfr.snrcjt.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ujv.sweek.top

[B07] while 循环
来源：http://phf.ppjwa.cn

Py:   while i < 10: i += 1
来源：http://sio.shanyushiyangkeji.top

PHP:  while ($i < 10) { $i++; }
来源：http://sxi.jinyuanbaomall.cn

JS:   while (i < 10) { i++; }
来源：http://akd.hammf.cn

TS:   while (i < 10) { i++; }
来源：http://bpq.birdmap.top

Java: while (i < 10) { i++; }
来源：http://dpj.hfpthk.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://jvv.guowangkeji.top

Ruby: while i < 10; i += 1; end
来源：http://mpw.tarul.cn

C#:   while (i < 10) { i++; }
来源：http://biz.haohaochexian.top

[B08] do-while（至少执行一次）
来源：http://aff.xylfe.cn

Py:   # 无 do-while：用 while True + break
来源：http://iov.zhongyouzk.top

PHP:  do { $i++; } while ($i < 10);
来源：http://wzr.wangshuangyany.cn

JS:   do { i++; } while (i < 10);
来源：http://vmf.ydjk.org.cn

TS:   do { i++; } while (i < 10);
来源：http://pnr.316326.xyz

Java: do { i++; } while (i < 10);
来源：http://izt.gzhubu.top

Go:   for { i++; if i >= 10 { break } }
来源：http://zcb.gaohongyu789.top

Ruby: begin; i += 1; end while i < 10
来源：http://sxr.zhixingplan.top

C#:   do { i++; } while (i < 10);
来源：http://oil.hywenlv.cn

[B09] break 与 continue
来源：http://biu.ywan-chungtsiang.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ees.9152youxi.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hmh.uphjek.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hhl.cashguo.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fjo.jlsjyb.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hyo.guowangkeji.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://jdj.xuanzx.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://aau.jinqigufen.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jgb.epnwcf.com

[B10] 遍历同时拿索引
来源：http://wji.meibo888.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ddp.sweek.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://kdi.zhiwuduotai.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ult.feifeiyinyue.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ttt.jinyuanbaomall.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ssn.guannengcc.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://gov.zhiwuduotai.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://tyz.yfazqb.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://tmm.52xcode.cn

[B11] 生成数字序列 / 区间
来源：http://ozb.cashguo.top

Py:   list(range(0, 10, 2))
来源：http://jhy.ybcxt.top

PHP:  range(0, 10, 2);
来源：http://cof.cucudq.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nco.xinyue.icu

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gow.tanke756.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://opk.xziqi.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://fgt.nanxuanxn.top

Ruby: (0...10).step(2).to_a
来源：http://xnf.shanyushiyangtech.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ygt.aizwys.cn

[B12] 跳出多层循环
来源：http://rfg.zhijiandao.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://cir.yvedp.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://mku.hnqzz.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://uac.jiagoushi.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://tpe.yvedp.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://byq.xziqi.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hjm.ybcxt.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ltc.yuanzhike.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hnv.fehbvm.com

[B13] 判断是否为数字
来源：http://bwe.uphjek.com

Py:   isinstance(x, (int, float))
来源：http://zql.meibo888.top

PHP:  is_numeric($x)
来源：http://meo.kuanghao11.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wng.ywan-chungtsiang.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kre.gotoacloud.top

Java: x instanceof Number
来源：http://icc.0kj1m.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://zkz.tian-w.cn

Ruby: x.is_a?(Numeric)
来源：http://hyh.jyoumei.cn

C#:   x is int or double or decimal
来源：http://zap.hysaishi.cn

[B14] 判断值是否在集合内
来源：http://azg.ivvv.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mjp.nanxinkj.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://drt.meibo888.top

JS:   [1, 2, 3].includes(x)
来源：http://tll.havefunace.top

TS:   [1, 2, 3].includes(x)
来源：http://zjg.epnwcf.com

Java: List.of(1, 2, 3).contains(x)
来源：http://tiq.meibo888.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ati.chenjidiqi.icu

Ruby: [1, 2, 3].include?(x)
来源：http://dhv.feifeiyinyue.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://krx.daxiang520.top

[B15] 布尔运算与取反
来源：http://eah.fehbvm.com

Py:   a and b or not c
来源：http://vfr.pycfn.com

PHP:  $a && $b || !$c
来源：http://vkq.cqqwz.cn

JS:   a && b || !c
来源：http://iqi.hammf.cn

TS:   a && b || !c
来源：http://waf.feifeiyinyue.top

Java: a && b || !c
来源：http://ulk.jiagoushi.top

Go:   a && b || !c
来源：http://ehq.ywan-chungtsiang.top

Ruby: a && b || !c
来源：http://vse.hesvh.cn

C#:   a && b || !c
来源：http://ygw.dianchejie.cn

[B16] 卫语句：不满足条件提前返回
来源：http://qpf.zhaomingkeji.xyz

Py:   if not data: return
来源：http://yen.gzhubu.top

PHP:  if (!$data) { return; }
来源：http://vsb.xinyue.icu

JS:   if (!data) return;
来源：http://jkv.guannengcc.top

TS:   if (!data) return;
来源：http://bbl.yvedp.cn

Java: if (data == null) return;
来源：http://rqq.fengsongda.top

Go:   if data == nil { return }
来源：http://qzw.zhaomingkeji.xyz

Ruby: return if data.nil?
来源：http://het.guannengcc.top

C#:   if (data == null) return;
来源：http://tzl.tian-w.cn

================================================================================
来源：http://akf.jqgufenzy.top

C. 函数与作用域
来源：http://kaw.redwolf501.top

================================================================================
来源：http://ccb.c1oappe.top

[C01] 定义函数
来源：http://yve.jinyuanbaomall.cn

Py:   def add(a, b): return a + b
来源：http://ldk.jinqigufen.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rhv.yj20258888.top

JS:   function add(a, b) { return a + b; }
来源：http://xli.yuanzhike.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://get.hongshengwenyu.top

Java: static int add(int a, int b) { return a + b; }
来源：http://ljk.epnwcf.com

Go:   func add(a, b int) int { return a + b }
来源：http://fjk.cdnleiting.top

Ruby: def add(a, b); a + b; end
来源：http://arv.ywan-chungtsiang.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ygo.ybcxt.top

[C02] 默认参数
来源：http://ykp.9152youxi.cn

Py:   def greet(name="World"): return name
来源：http://kca.316326.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://vqp.gzhubu.top

JS:   function greet(name = "World") { return name; }
来源：http://wze.wangshuangyany.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ggi.fehbvm.com

Java: // 无默认参数：方法重载或 Optional
来源：http://bnh.tian-w.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://tyd.fanxiaobao.xyz

Ruby: def greet(name = "World") = name
来源：http://yds.sjlbkw.cn

C#:   string Greet(string name = "World") => name;
来源：http://avt.yj202588.top

[C03] 可变参数
来源：http://dfn.ctjpmb.com

Py:   def total(*args): return sum(args)
来源：http://pek.gogol.net.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://kwf.yuanzhike.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://etx.chenjidiqi.icu

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://qbj.birdmap.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ftp.hnxiangtu.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://sjx.chenjidiqi.icu

Ruby: def total(*nums); nums.sum; end
来源：http://quh.meibo888.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hbj.gotoacloud.top

[C04] 命名参数 / 关键字参数
来源：http://spg.shanyushiyangtech.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://vgj.fktsv.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ksh.aizwys.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mrx.vehdjk.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://auk.wangdashe.top

Java: // 无：用 Builder 模式或 record
来源：http://kec.sufxvd.cn

Go:   // 无：用配置结构体参数
来源：http://qrf.guannengcc.top

Ruby: f(a: 1, b: 2)
来源：http://tem.c1oappe.top

C#:   f(a: 1, b: 2)
来源：http://qoy.bjfxy.top

[C05] 返回多个值
来源：http://oos.yuxming.cn

Py:   return a, b
来源：http://vie.hywenlv.cn

PHP:  return [$a, $b];
来源：http://xzn.yangfankeji.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://uwz.nanxinkj.top

TS:   return { a, b };
来源：http://edr.tarul.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://vai.bjfxy.top

Go:   return a, b
来源：http://jav.yanxiufei.cn

Ruby: return a, b
来源：http://kwb.vqdsnc.cn

C#:   return (a, b);              // ValueTuple
来源：http://mpb.fengsongda.top

[C06] 匿名函数 / lambda
来源：http://ybj.zycfv.cn

Py:   square = lambda x: x * x
来源：http://bpa.zhijiandao.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://quq.nwbrower.top

JS:   const square = x => x * x;
来源：http://oyo.zhiwuduotai.top

TS:   const square = (x: number): number => x * x;
来源：http://zau.dianchejie.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://gyh.birdmap.top

Go:   sq := func(x int) int { return x * x }
来源：http://qqp.hywenlv.cn

Ruby: square = ->(x) { x * x }
来源：http://xhx.jqgufenzy.top

C#:   Func<int, int> square = x => x * x;
来源：http://oth.ctjpmb.com

[C07] 把函数作为参数传入
来源：http://exw.birdmap.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://vqy.yongpay.top

PHP:  array_map("strtoupper", $arr);
来源：http://erz.daxiang520.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://lpv.chenjidiqi.icu

TS:   arr.map(String)
来源：http://waz.dianchejie.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://qgq.yvedp.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://jjr.ydjk.org.cn

Ruby: arr.map(&:upcase)
来源：http://spd.tian-w.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://xsm.mhx1999.top

[C08] 闭包
来源：http://jiu.hfpthk.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://toi.yangfankeji.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://pbh.ydjk.org.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://tlv.cucudq.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://yjq.sxryk.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ueo.zdbjq.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baj.wangshuangyany.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://tro.yj20258.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ynx.xylfe.cn

[C09] 递归
来源：http://czs.yangfankeji.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://nth.jianghu66.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://rny.meibo888.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rzk.nwbrower.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vjv.0kj1m.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ewf.zdqjudy.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://tvi.daria6918.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://nje.yj20258888.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://olt.sufxvd.cn

[C10] 变量作用域
来源：http://oyj.hnqzz.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://sqt.wangshuangyany.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://rkk.jianghu66.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://you.jinghuilouyu.cn

TS:   同 JS
来源：http://fqp.pycfn.com

Java: 方法内为块级作用域
来源：http://wxh.kuanghao11.cn

Go:   花括号块级作用域
来源：http://ziq.ydzc1.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hun.dianchejie.cn

C#:   块级作用域
来源：http://zuj.hesvh.cn

[C11] 模块导入与导出
来源：http://zcs.vqdsnc.cn

Py:   from module import func
来源：http://kqa.hnqzz.top

PHP:  require "file.php";  或 use App\Service;
来源：http://zke.hywenlv.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ahf.fzhhl.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://keq.316326.xyz

Java: import java.util.List;
来源：http://cvn.mhx1999.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hqq.daxiang520.top

Ruby: require "json"; require_relative "./util"
来源：http://umv.bjfxy.top

C#:   using System.Text;
来源：http://xux.tarul.cn

[C12] 立即执行函数 IIFE
来源：http://tsk.redwolf501.top

Py:   (lambda: print("run"))()
来源：http://gub.hfpthk.cn

PHP:  (function () { echo "run"; })();
来源：http://cyc.hammf.cn

JS:   (() => { console.log("run"); })();
来源：http://lwn.pycfn.com

TS:   (() => { console.log("run"); })();
来源：http://jlv.yueranfly.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://vxx.shanyushiyangkeji.top

Go:   func() { fmt.Println("run") }()
来源：http://icv.hywenlv.cn

Ruby: -> { puts "run" }.call
来源：http://jut.yonumen.top

C#:   // 无 IIFE：用静态构造函数
来源：http://whc.iojbl.cn

[C13] 类型声明 / 类型注解
来源：http://hxf.xuetiantiany.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://pka.9152youxi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jcn.zdbjq.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mrx.xuanzx.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zfz.guannengcc.top

Java: int add(int a, int b) { return a + b; }
来源：http://rvc.zhengqikj.top

Go:   func add(a, b int) int
来源：http://ttj.jinyuanbaomall.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://egh.jianghu66.top

C#:   int Add(int a, int b) => a + b;
来源：http://umc.daxiang520.top

[C14] 泛型函数
来源：http://hkc.zhijiandao.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ugd.tarul.cn

PHP:  // 无泛型
来源：http://saw.jinghuilouyu.cn

JS:   // 无泛型
来源：http://qnf.zhijiandao.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://kry.jinqigfzy.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://uqj.xuanzx.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://lxz.jqgufenzy.top

Ruby: # 无泛型
来源：http://uss.smart0.xyz

C#:   static T First<T>(List<T> items) => items[0];
来源：http://tdb.jyoumei.cn

[C15] 解构 / 展开参数
来源：http://wuh.jianghu66.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://euh.andypj.xyz

PHP:  [$a, $b] = $pair;
来源：http://tea.meibo888.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ain.jqgufenzy.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hhk.gzhubu.top

Java: // 无解构
来源：http://ieu.shuidangran.top

Go:   // 无解构
来源：http://xjr.yanxiufei.cn

Ruby: a, b = pair
来源：http://bke.jqgufenzy.top

C#:   var (a, b) = pair;
来源：http://rfz.meibo888.top

[C16] 函数 / 方法重载
来源：http://qes.zhoulong.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://qpk.gogol.net.cn

PHP:  // 无重载
来源：http://diz.sufxvd.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ugm.zhiwuduotai.top

TS:   // 用联合类型或重载签名声明
来源：http://wsb.52xcode.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://zxv.jlsjyb.cn

Go:   // 无重载：用不同函数名
来源：http://ldn.ehwqpu.com

Ruby: # 无重载：靠动态参数
来源：http://gos.tarul.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ddu.ydzc1.top

================================================================================
来源：http://giq.guannengcc.top

D. 数组 / 列表 / 集合
来源：http://ivj.dianchejie.cn

================================================================================
来源：http://fes.nanxuanxn.top

[D01] 创建数组 / 列表
来源：http://waw.dianchejie.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://zcm.cdnleiting.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://bzn.ydjk.org.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://boq.yfazqb.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://zyh.yongpay.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://jcj.ywan-chungtsiang.top

Go:   arr := []int{1, 2, 3}
来源：http://keh.hcnkem.com

Ruby: arr = [1, 2, 3]
来源：http://pve.havefunace.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://kex.birdmap.top

[D02] 追加元素到末尾
来源：http://vpb.sysykeji.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://pkj.jinqigfzy.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mhz.hywenlv.cn

JS:   arr.push(4);
来源：http://dlh.yj20258.top

TS:   arr.push(4);
来源：http://fbh.9152youxi.cn

Java: list.add(4);
来源：http://exw.zhixingplan.top

Go:   arr = append(arr, 4)
来源：http://mcm.yj20258888.top

Ruby: arr << 4; arr.push(5)
来源：http://mkf.316326.xyz

C#:   list.Add(4);
来源：http://bky.chenjidiqi.icu

[D03] 在指定位置插入元素
来源：http://vhr.hammf.cn

Py:   arr.insert(0, 0)
来源：http://udm.hnqzz.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://dol.hfpthk.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://cnx.andypj.xyz

TS:   arr.splice(0, 0, 0);
来源：http://ida.xingfuxueyuan.xyz

Java: list.add(0, 0);
来源：http://roo.yj20258888.top

Go:   arr = append([]int{0}, arr...)
来源：http://ome.andypj.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://xmy.hammf.cn

C#:   list.Insert(0, 0);
来源：http://zul.wangdashe.top

[D04] 删除元素
来源：http://jhc.chenjidiqi.icu

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://usa.cucudq.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://qkn.yuxming.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mxl.chenzaomai.com

TS:   arr.splice(0, 1);
来源：http://ejp.chenlongwang.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://zkf.nwbrower.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://drc.daxiang520.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://jlr.9152youxi.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://nho.tanke756.top

[D05] 访问与修改元素
来源：http://esh.sjlbkw.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://rfp.bbcook.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://duq.zdbjq.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://nnb.zhiwuduotai.top

TS:   arr[0]; arr.at(-1);
来源：http://lvg.cdnleiting.top

Java: list.get(0); list.set(0, 9);
来源：http://ldw.xylfe.cn

Go:   arr[0]; arr[0] = 9
来源：http://ugz.gotoacloud.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://aee.tarul.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://erb.fzhhl.top

[D06] 数组长度
来源：http://wfa.zdqjudy.top

Py:   len(arr)
来源：http://lnn.cqqwz.cn

PHP:  count($arr);
来源：http://hbn.vehdjk.com

JS:   arr.length
来源：http://vcx.jianghu66.top

TS:   arr.length
来源：http://toq.zdqjudy.top

Java: list.size();
来源：http://tvj.jqgufenzy.top

Go:   len(arr)
来源：http://mqw.ybcxt.top

Ruby: arr.length; arr.size
来源：http://but.kuanghao11.cn

C#:   list.Count;
来源：http://pvk.pycfn.com


<!-- 参考信息 -->