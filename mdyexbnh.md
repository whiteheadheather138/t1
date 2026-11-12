代发 wailian999

TS:   for (const item of arr) { console.log(item); }
来源：http://kav.yongpay.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://gsu.zdbjq.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://swb.jqgufenzy.top

Ruby: arr.each { |item| puts item }
来源：http://qok.haohaochexian.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://xiz.hysaishi.cn

[B06] 遍历字典 / 对象
来源：http://kzh.yj20258888.top

Py:   for k, v in d.items(): print(k, v)
来源：http://guy.fengsongda.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://jxm.zhijiandao.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kpi.ywan-chungtsiang.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://oay.tianlin.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://rga.tanke756.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ncs.uphjek.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://agk.jqgufenzy.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://sxe.nwbrower.top

[B07] while 循环
来源：http://bds.cashguo.top

Py:   while i < 10: i += 1
来源：http://whx.aibaodan.cn

PHP:  while ($i < 10) { $i++; }
来源：http://efo.yuxming.cn

JS:   while (i < 10) { i++; }
来源：http://dbo.ppjwa.cn

TS:   while (i < 10) { i++; }
来源：http://npa.pycfn.com

Java: while (i < 10) { i++; }
来源：http://eiz.xinyue.icu

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mem.andypj.xyz

Ruby: while i < 10; i += 1; end
来源：http://xhp.zhoulong.xyz

C#:   while (i < 10) { i++; }
来源：http://kmm.gaohongyu789.top

[B08] do-while（至少执行一次）
来源：http://wku.zycfv.cn

Py:   # 无 do-while：用 while True + break
来源：http://qnh.yonumen.top

PHP:  do { $i++; } while ($i < 10);
来源：http://enz.xuetiantiany.cn

JS:   do { i++; } while (i < 10);
来源：http://omb.guowangkeji.top

TS:   do { i++; } while (i < 10);
来源：http://gpt.yj202588.top

Java: do { i++; } while (i < 10);
来源：http://dwy.hammf.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://gge.dianchejie.cn

Ruby: begin; i += 1; end while i < 10
来源：http://pbn.ydzc1.top

C#:   do { i++; } while (i < 10);
来源：http://rph.ivvv.top

[B09] break 与 continue
来源：http://pxo.yfazqb.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://olo.fanxiaobao.xyz

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://dew.jlsjyb.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rka.yvedp.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qhd.cheryme.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hel.ivvv.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://tcs.quarkkingdee.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://lco.shanyushiyangtech.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sso.xingfuxueyuan.xyz

[B10] 遍历同时拿索引
来源：http://gwg.9152youxi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hha.yuxming.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://zzo.tianlin.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://gba.shanyushiyangtech.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://tdz.52xcode.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://vyf.fengsongda.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://rwi.ybcxt.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hxe.tianlin.xyz

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://jup.fehbvm.com

[B11] 生成数字序列 / 区间
来源：http://yvb.jinghuilouyu.cn

Py:   list(range(0, 10, 2))
来源：http://vsf.shangyingyoupin.top

PHP:  range(0, 10, 2);
来源：http://dad.jinqigfzy.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wcp.wangdashe.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://znz.hnqzz.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://muy.chenjidiqi.icu

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://nor.sufxvd.cn

Ruby: (0...10).step(2).to_a
来源：http://bdg.sweek.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://reo.shzxlz.cn

[B12] 跳出多层循环
来源：http://zpx.yj20258.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://anc.jiagoushi.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://ozo.yanxiufei.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://jhn.hcnkem.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hdi.hysaishi.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://fbg.sxryk.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://sqm.316326.xyz

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://svf.aizwys.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://owd.vehdjk.com

[B13] 判断是否为数字
来源：http://dui.uphjek.com

Py:   isinstance(x, (int, float))
来源：http://lrt.gaohongyu789.top

PHP:  is_numeric($x)
来源：http://zos.ybcxt.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tyw.cdnleiting.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://awf.fanxiaobao.xyz

Java: x instanceof Number
来源：http://qxf.ctjpmb.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://buj.cdnleiting.top

Ruby: x.is_a?(Numeric)
来源：http://jdk.yj20258.top

C#:   x is int or double or decimal
来源：http://fdg.haohaochexian.top

[B14] 判断值是否在集合内
来源：http://skt.tarul.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://gic.nanxinkj.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ikm.svipenyu.cn

JS:   [1, 2, 3].includes(x)
来源：http://uaf.cdnleiting.top

TS:   [1, 2, 3].includes(x)
来源：http://gey.zhixingplan.top

Java: List.of(1, 2, 3).contains(x)
来源：http://gby.sufxvd.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://xpz.zhiwuduotai.top

Ruby: [1, 2, 3].include?(x)
来源：http://cec.guannengcc.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mti.316326.xyz

[B15] 布尔运算与取反
来源：http://wce.fzhhl.top

Py:   a and b or not c
来源：http://irh.andypj.xyz

PHP:  $a && $b || !$c
来源：http://oyw.gzhubu.top

JS:   a && b || !c
来源：http://pbx.pengpengdd.cyou

TS:   a && b || !c
来源：http://ydy.xinyue.icu

Java: a && b || !c
来源：http://vgt.zycfv.cn

Go:   a && b || !c
来源：http://oxu.hesvh.cn

Ruby: a && b || !c
来源：http://lwr.feifeiyinyue.top

C#:   a && b || !c
来源：http://ney.shuidangran.top

[B16] 卫语句：不满足条件提前返回
来源：http://dna.yuanzhike.top

Py:   if not data: return
来源：http://cnf.snrcjt.cn

PHP:  if (!$data) { return; }
来源：http://god.aizwys.cn

JS:   if (!data) return;
来源：http://gpy.hfpthk.cn

TS:   if (!data) return;
来源：http://dha.chenzaomai.com

Java: if (data == null) return;
来源：http://fgf.hcnkem.com

Go:   if data == nil { return }
来源：http://upe.ydzc1.top

Ruby: return if data.nil?
来源：http://tmv.quarkkingdee.top

C#:   if (data == null) return;
来源：http://eoa.ydjk.org.cn

================================================================================
来源：http://wlr.jqgufenzy.top

C. 函数与作用域
来源：http://xgb.yangfankeji.com

================================================================================
来源：http://yir.fzhhl.top

[C01] 定义函数
来源：http://imr.yonumen.top

Py:   def add(a, b): return a + b
来源：http://zoj.guannengcc.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fcl.zdbjq.cn

JS:   function add(a, b) { return a + b; }
来源：http://mdw.daria6918.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lxv.birdmap.top

Java: static int add(int a, int b) { return a + b; }
来源：http://onn.zhaomingkeji.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://ryv.mhx1999.top

Ruby: def add(a, b); a + b; end
来源：http://dhh.fengsongda.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://fkb.sxryk.cn

[C02] 默认参数
来源：http://dxp.andypj.xyz

Py:   def greet(name="World"): return name
来源：http://ifc.nanxinkj.top

PHP:  function greet($name = "World") { return $name; }
来源：http://dbj.bjfxy.top

JS:   function greet(name = "World") { return name; }
来源：http://oau.havefunace.top

TS:   function greet(name: string = "World") { return name; }
来源：http://bvt.shanyushiyangtech.top

Java: // 无默认参数：方法重载或 Optional
来源：http://rol.yj20258.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://pth.zhixingplan.top

Ruby: def greet(name = "World") = name
来源：http://cww.haohaochexian.top

C#:   string Greet(string name = "World") => name;
来源：http://jye.tanke756.top

[C03] 可变参数
来源：http://zuj.shangyingyoupin.top

Py:   def total(*args): return sum(args)
来源：http://lse.fehbvm.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ghv.svipenyu.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://gou.shanyushiyangkeji.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://evg.hfpthk.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://rot.zhengqikj.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://avd.ydjk.org.cn

Ruby: def total(*nums); nums.sum; end
来源：http://dou.jianghu66.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://jgb.zhengqikj.top

[C04] 命名参数 / 关键字参数
来源：http://pxp.hesvh.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://say.kuanghao11.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://rbe.xziqi.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://yoj.jlsjyb.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://evh.ctjpmb.com

Java: // 无：用 Builder 模式或 record
来源：http://nzz.hnqzz.top

Go:   // 无：用配置结构体参数
来源：http://zyj.chenlongwang.top

Ruby: f(a: 1, b: 2)
来源：http://vqh.zdqjudy.top

C#:   f(a: 1, b: 2)
来源：http://ohi.cdnleiting.top

[C05] 返回多个值
来源：http://nqz.zhijiandao.cn

Py:   return a, b
来源：http://egj.hysaishi.cn

PHP:  return [$a, $b];
来源：http://tul.bjfxy.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://mdt.ehwqpu.com

TS:   return { a, b };
来源：http://aoo.hcnkem.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ouz.birdmap.top

Go:   return a, b
来源：http://acs.nanxuanxn.top

Ruby: return a, b
来源：http://vmu.xuetiantiany.cn

C#:   return (a, b);              // ValueTuple
来源：http://bik.yongpay.top

[C06] 匿名函数 / lambda
来源：http://jbn.zhijiandao.cn

Py:   square = lambda x: x * x
来源：http://bnt.zhaomingkeji.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://zvx.gzhubu.top

JS:   const square = x => x * x;
来源：http://fuc.haohaochexian.top

TS:   const square = (x: number): number => x * x;
来源：http://puh.jqgfzy.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ntr.sweek.top

Go:   sq := func(x int) int { return x * x }
来源：http://ean.chenjidiqi.icu

Ruby: square = ->(x) { x * x }
来源：http://xek.yj20258.top

C#:   Func<int, int> square = x => x * x;
来源：http://otk.shangyingyoupin.top

[C07] 把函数作为参数传入
来源：http://end.sweek.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://jlx.vehdjk.com

PHP:  array_map("strtoupper", $arr);
来源：http://zhj.shuidangran.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ufs.nanxuanxn.top

TS:   arr.map(String)
来源：http://hod.xuanzx.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://gsn.tarul.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ziv.hesvh.cn

Ruby: arr.map(&:upcase)
来源：http://rbo.nwbrower.top

C#:   arr.Select(s => s.ToUpper())
来源：http://xxl.meibo888.top

[C08] 闭包
来源：http://bmw.gotoacloud.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://xlu.tarul.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ldj.meibo888.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ydu.meibo888.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mhm.dianchejie.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://nln.pycfn.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://sgr.cashguo.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://rpo.wangdashe.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://lof.ywan-chungtsiang.top

[C09] 递归
来源：http://rol.ywan-chungtsiang.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://tii.daria6918.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://enc.nwbrower.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jho.cheryme.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zmc.xuetiantiany.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://rre.ybcxt.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://nyt.sjlbkw.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://gug.yuanzhike.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://srl.jyoumei.cn

[C10] 变量作用域
来源：http://onf.fengsongda.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://zsr.ywan-chungtsiang.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://qxt.fzhhl.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://qfx.meibo888.top

TS:   同 JS
来源：http://rae.hammf.cn

Java: 方法内为块级作用域
来源：http://ebj.jinqigfzy.top

Go:   花括号块级作用域
来源：http://god.yj202588.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://alj.fanxiaobao.xyz

C#:   块级作用域
来源：http://fpv.ydzc1.top

[C11] 模块导入与导出
来源：http://bah.kuanghao11.cn

Py:   from module import func
来源：http://rxe.jianghu66.top

PHP:  require "file.php";  或 use App\Service;
来源：http://rjd.c1oappe.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://jud.fehbvm.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://rgi.zhaomingkeji.xyz

Java: import java.util.List;
来源：http://zaq.316326.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://syo.yuanzhike.top

Ruby: require "json"; require_relative "./util"
来源：http://ibl.yj20258.top

C#:   using System.Text;
来源：http://rjq.uphjek.com

[C12] 立即执行函数 IIFE
来源：http://lsk.tarul.cn

Py:   (lambda: print("run"))()
来源：http://yav.meibo888.top

PHP:  (function () { echo "run"; })();
来源：http://whp.nanxinkj.top

JS:   (() => { console.log("run"); })();
来源：http://mlg.ivvv.top

TS:   (() => { console.log("run"); })();
来源：http://hfb.hammf.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://pma.52xcode.cn

Go:   func() { fmt.Println("run") }()
来源：http://sqf.snrcjt.cn

Ruby: -> { puts "run" }.call
来源：http://tqn.quarkkingdee.top

C#:   // 无 IIFE：用静态构造函数
来源：http://agn.tianlin.xyz

[C13] 类型声明 / 类型注解
来源：http://ysh.c1oappe.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://dvx.jlsjyb.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hcx.gaohongyu789.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://msn.cucudq.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bkl.mhx1999.top

Java: int add(int a, int b) { return a + b; }
来源：http://bww.feifeiyinyue.top

Go:   func add(a, b int) int
来源：http://fjt.hysaishi.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://elf.daria6918.cn

C#:   int Add(int a, int b) => a + b;
来源：http://pte.hammf.cn

[C14] 泛型函数
来源：http://jtg.guowangkeji.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://vtu.tanke756.top

PHP:  // 无泛型
来源：http://qah.xuetiantiany.cn

JS:   // 无泛型
来源：http://inq.svipenyu.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://tvv.tianlin.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://emf.aibaodan.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://gzt.fengsongda.top

Ruby: # 无泛型
来源：http://abw.bbcook.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://jgy.epnwcf.com

[C15] 解构 / 展开参数
来源：http://ope.zdqjudy.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://pnq.yfazqb.com

PHP:  [$a, $b] = $pair;
来源：http://dfk.hnqzz.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://fel.xziqi.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://bst.shuidangran.top

Java: // 无解构
来源：http://ldt.yanxiufei.cn

Go:   // 无解构
来源：http://wry.fehbvm.com

Ruby: a, b = pair
来源：http://vlh.ydzc1.top

C#:   var (a, b) = pair;
来源：http://tjz.yongpay.top

[C16] 函数 / 方法重载
来源：http://hwj.smart0.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vlf.jianghu66.top

PHP:  // 无重载
来源：http://xac.yfazqb.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://krz.zhijiandao.cn

TS:   // 用联合类型或重载签名声明
来源：http://tmw.chenlongwang.top

Java: void f(int a) {}  void f(String a) {}
来源：http://kqp.ivvv.top

Go:   // 无重载：用不同函数名
来源：http://cvc.shzxlz.cn

Ruby: # 无重载：靠动态参数
来源：http://ili.cashguo.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://aid.jinqigfzy.top

================================================================================
来源：http://vbq.chenzaomai.com

D. 数组 / 列表 / 集合
来源：http://svq.yj20258888.top

================================================================================
来源：http://wdf.ybcxt.top

[D01] 创建数组 / 列表
来源：http://otg.zhijiandao.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://jes.ydjk.org.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hjt.aibaodan.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://vpc.xuanzx.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://zyy.tianlin.xyz

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baz.xziqi.cn

Go:   arr := []int{1, 2, 3}
来源：http://ixv.snrcjt.cn

Ruby: arr = [1, 2, 3]
来源：http://axr.yanxiufei.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://fmv.nanxinkj.top

[D02] 追加元素到末尾
来源：http://iux.bjfxy.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://tlc.hnxiangtu.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mwd.fktsv.cn

JS:   arr.push(4);
来源：http://znz.cucudq.cn

TS:   arr.push(4);
来源：http://hmb.zhongyouzk.top

Java: list.add(4);
来源：http://rov.aibaodan.cn

Go:   arr = append(arr, 4)
来源：http://kbt.cheryme.top

Ruby: arr << 4; arr.push(5)
来源：http://cdd.jyoumei.cn

C#:   list.Add(4);
来源：http://rzj.vqdsnc.cn

[D03] 在指定位置插入元素
来源：http://gmt.hfpthk.cn

Py:   arr.insert(0, 0)
来源：http://whu.birdmap.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://rfs.zhaomingkeji.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://orl.shangyingyoupin.top

TS:   arr.splice(0, 0, 0);
来源：http://ofc.hammf.cn

Java: list.add(0, 0);
来源：http://xoz.yj202588.top

Go:   arr = append([]int{0}, arr...)
来源：http://zlq.kuanghao11.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://gou.wangshuangyany.cn

C#:   list.Insert(0, 0);
来源：http://gbe.zhijiandao.cn

[D04] 删除元素
来源：http://jrj.xziqi.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://vnd.tarul.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://jeg.yj20258.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://lgv.jianghu66.top

TS:   arr.splice(0, 1);
来源：http://aom.feifeiyinyue.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://sby.xuetiantiany.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://qzk.snrcjt.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mpx.sysykeji.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://asn.tian-w.cn

[D05] 访问与修改元素
来源：http://etf.wangshuangyany.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://cyo.yueranfly.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://qqp.tarul.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://sbc.yj20258.top

TS:   arr[0]; arr.at(-1);
来源：http://ljy.pycfn.com

Java: list.get(0); list.set(0, 9);
来源：http://ohp.quarkkingdee.top

Go:   arr[0]; arr[0] = 9
来源：http://tdp.xinyue.icu

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://sim.bjfxy.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://vcr.9152youxi.cn

[D06] 数组长度
来源：http://nlp.redwolf501.top


<!-- 参考信息 -->