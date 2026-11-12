代发 wailian999

TS:   for (const item of arr) { console.log(item); }
来源：http://xxx.9152youxi.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://qlx.pengpengdd.cyou

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://xpk.yangfankeji.com

Ruby: arr.each { |item| puts item }
来源：http://msz.xingfuxueyuan.xyz

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://sxw.yanxiufei.cn

[B06] 遍历字典 / 对象
来源：http://jab.tarul.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://drv.haohaochexian.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://fha.bbcook.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://efc.chenzaomai.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fae.sufxvd.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wnx.yongpay.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mzq.snrcjt.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://nqi.epnwcf.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://oan.andypj.xyz

[B07] while 循环
来源：http://mnn.jyoumei.cn

Py:   while i < 10: i += 1
来源：http://sfl.guowangkeji.top

PHP:  while ($i < 10) { $i++; }
来源：http://wmp.shuidangran.top

JS:   while (i < 10) { i++; }
来源：http://ubv.yj20258888.top

TS:   while (i < 10) { i++; }
来源：http://waa.wangdashe.top

Java: while (i < 10) { i++; }
来源：http://tyl.daxiang520.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baa.jiagoushi.top

Ruby: while i < 10; i += 1; end
来源：http://hlz.birdmap.top

C#:   while (i < 10) { i++; }
来源：http://wgl.yj20258888.top

[B08] do-while（至少执行一次）
来源：http://bny.52xcode.cn

Py:   # 无 do-while：用 while True + break
来源：http://vni.feifeiyinyue.top

PHP:  do { $i++; } while ($i < 10);
来源：http://fvu.yanxiufei.cn

JS:   do { i++; } while (i < 10);
来源：http://eju.zhengqikj.top

TS:   do { i++; } while (i < 10);
来源：http://fuw.zhengqikj.top

Java: do { i++; } while (i < 10);
来源：http://iwf.gzhubu.top

Go:   for { i++; if i >= 10 { break } }
来源：http://eoz.jyoumei.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ypp.smart0.xyz

C#:   do { i++; } while (i < 10);
来源：http://lhl.tian-w.cn

[B09] break 与 continue
来源：http://foj.vehdjk.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://nqs.hongshengwenyu.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://yez.yfazqb.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ytk.guowangkeji.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rwk.chenjidiqi.icu

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nmy.snrcjt.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ypw.yj20258.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://kku.feifeiyinyue.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hwn.bbcook.cn

[B10] 遍历同时拿索引
来源：http://tda.zhijiandao.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://meq.feifeiyinyue.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://xgt.cdnleiting.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hoa.hesvh.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://bll.gogol.net.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://gdw.zhongyouzk.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://spz.fanxiaobao.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://cxx.ctjpmb.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://iai.fktsv.cn

[B11] 生成数字序列 / 区间
来源：http://nfg.yuanzhike.top

Py:   list(range(0, 10, 2))
来源：http://uji.daria6918.cn

PHP:  range(0, 10, 2);
来源：http://kyn.yonumen.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gyq.quarkkingdee.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.jinqigufen.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://yyc.0kj1m.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://nek.epnwcf.com

Ruby: (0...10).step(2).to_a
来源：http://vvy.guannengcc.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zpv.fengsongda.top

[B12] 跳出多层循环
来源：http://vcy.shangyingyoupin.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://nfs.nanxinkj.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://qff.hesvh.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mas.shanyushiyangkeji.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://oia.snrcjt.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ajn.zycfv.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://bio.hywenlv.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://zfz.vehdjk.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://rlk.yanxiufei.cn

[B13] 判断是否为数字
来源：http://kuk.andypj.xyz

Py:   isinstance(x, (int, float))
来源：http://ybb.ehwqpu.com

PHP:  is_numeric($x)
来源：http://ipd.tanke756.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ocw.chenzaomai.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://eun.shangyingyoupin.top

Java: x instanceof Number
来源：http://rfo.jyoumei.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blc.xziqi.cn

Ruby: x.is_a?(Numeric)
来源：http://wun.yj20258.top

C#:   x is int or double or decimal
来源：http://hgo.0kj1m.cn

[B14] 判断值是否在集合内
来源：http://ngg.cdnleiting.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jmb.aibaodan.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ueq.aizwys.cn

JS:   [1, 2, 3].includes(x)
来源：http://pwg.hnqzz.top

TS:   [1, 2, 3].includes(x)
来源：http://yux.ybcxt.top

Java: List.of(1, 2, 3).contains(x)
来源：http://tql.daxiang520.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://xld.hammf.cn

Ruby: [1, 2, 3].include?(x)
来源：http://jrc.jinghuilouyu.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://oea.jiagoushi.top

[B15] 布尔运算与取反
来源：http://afh.zycfv.cn

Py:   a and b or not c
来源：http://nen.yueranfly.top

PHP:  $a && $b || !$c
来源：http://snz.yongpay.top

JS:   a && b || !c
来源：http://cnd.yj20258.top

TS:   a && b || !c
来源：http://ghi.daria6918.cn

Java: a && b || !c
来源：http://xpe.yvedp.cn

Go:   a && b || !c
来源：http://jyu.yj20258.top

Ruby: a && b || !c
来源：http://jcl.fengsongda.top

C#:   a && b || !c
来源：http://xjz.vqdsnc.cn

[B16] 卫语句：不满足条件提前返回
来源：http://uvs.zhiwuduotai.top

Py:   if not data: return
来源：http://fvy.yj20258.top

PHP:  if (!$data) { return; }
来源：http://lvw.xylfe.cn

JS:   if (!data) return;
来源：http://kkc.yvedp.cn

TS:   if (!data) return;
来源：http://qnu.xylfe.cn

Java: if (data == null) return;
来源：http://qjc.gotoacloud.top

Go:   if data == nil { return }
来源：http://zux.fktsv.cn

Ruby: return if data.nil?
来源：http://oxf.tarul.cn

C#:   if (data == null) return;
来源：http://eoc.jyoumei.cn

================================================================================
来源：http://col.ydzc1.top

C. 函数与作用域
来源：http://tke.xingfuxueyuan.xyz

================================================================================
来源：http://mcj.hnqzz.top

[C01] 定义函数
来源：http://jcd.yuxming.cn

Py:   def add(a, b): return a + b
来源：http://zog.ybcxt.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wfs.sysykeji.top

JS:   function add(a, b) { return a + b; }
来源：http://hpc.daria6918.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dkk.cucudq.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://bgk.wangdashe.top

Go:   func add(a, b int) int { return a + b }
来源：http://ekm.9152youxi.cn

Ruby: def add(a, b); a + b; end
来源：http://psf.sxryk.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://yfy.xylfe.cn

[C02] 默认参数
来源：http://yuy.cdnleiting.top

Py:   def greet(name="World"): return name
来源：http://tzw.gaohongyu789.top

PHP:  function greet($name = "World") { return $name; }
来源：http://cfj.hfpthk.cn

JS:   function greet(name = "World") { return name; }
来源：http://gxh.feifeiyinyue.top

TS:   function greet(name: string = "World") { return name; }
来源：http://ohy.uphjek.com

Java: // 无默认参数：方法重载或 Optional
来源：http://tsi.hesvh.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://tso.hesvh.cn

Ruby: def greet(name = "World") = name
来源：http://rjx.cqqwz.cn

C#:   string Greet(string name = "World") => name;
来源：http://hnd.zhijiandao.cn

[C03] 可变参数
来源：http://dhi.yvedp.cn

Py:   def total(*args): return sum(args)
来源：http://ssn.bjfxy.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ngw.zdqjudy.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://fzi.gzhubu.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ese.mhx1999.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://gzj.jyoumei.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://flf.nanxinkj.top

Ruby: def total(*nums); nums.sum; end
来源：http://jul.daxiang520.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://xct.yanxiufei.cn

[C04] 命名参数 / 关键字参数
来源：http://qsm.xuetiantiany.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://lma.ywan-chungtsiang.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://snf.ywan-chungtsiang.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://fcx.yj20258888.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://bak.yj202588.top

Java: // 无：用 Builder 模式或 record
来源：http://zzs.shuidangran.top

Go:   // 无：用配置结构体参数
来源：http://fuo.epnwcf.com

Ruby: f(a: 1, b: 2)
来源：http://ell.zycfv.cn

C#:   f(a: 1, b: 2)
来源：http://rau.daxiang520.top

[C05] 返回多个值
来源：http://ckh.gzhubu.top

Py:   return a, b
来源：http://ohy.tarul.cn

PHP:  return [$a, $b];
来源：http://dzv.zhengqikj.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://zvs.hcnkem.com

TS:   return { a, b };
来源：http://xqi.jqgufenzy.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://glm.feifeiyinyue.top

Go:   return a, b
来源：http://unr.feifeiyinyue.top

Ruby: return a, b
来源：http://elc.xylfe.cn

C#:   return (a, b);              // ValueTuple
来源：http://tww.hcnkem.com

[C06] 匿名函数 / lambda
来源：http://gtc.guowangkeji.top

Py:   square = lambda x: x * x
来源：http://jze.yongpay.top

PHP:  $square = fn($x) => $x * $x;
来源：http://anu.ydjk.org.cn

JS:   const square = x => x * x;
来源：http://bat.vehdjk.com

TS:   const square = (x: number): number => x * x;
来源：http://hzt.shanyushiyangtech.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://zsw.yonumen.top

Go:   sq := func(x int) int { return x * x }
来源：http://hev.xuanzx.com

Ruby: square = ->(x) { x * x }
来源：http://edw.yongpay.top

C#:   Func<int, int> square = x => x * x;
来源：http://qxd.aibaodan.cn

[C07] 把函数作为参数传入
来源：http://nyy.redwolf501.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://did.bbcook.cn

PHP:  array_map("strtoupper", $arr);
来源：http://www.fzhhl.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://tqn.shanyushiyangkeji.top

TS:   arr.map(String)
来源：http://boq.fehbvm.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blo.andypj.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qap.gotoacloud.top

Ruby: arr.map(&:upcase)
来源：http://yqt.wangdashe.top

C#:   arr.Select(s => s.ToUpper())
来源：http://rmc.xuanzx.com

[C08] 闭包
来源：http://qlf.bbcook.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wmr.epnwcf.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://xlm.zhoulong.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://udm.jinqigfzy.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://otq.haohaochexian.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://req.cheryme.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://svz.xziqi.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://txs.hywenlv.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://zyb.aibaodan.cn

[C09] 递归
来源：http://tzc.hfpthk.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://joh.daxiang520.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://jar.yvedp.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lep.andypj.xyz

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nki.ydzc1.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://zfx.gogol.net.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wix.tianlin.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ikk.jyoumei.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://rtd.iojbl.cn

[C10] 变量作用域
来源：http://ofd.gzhubu.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qsy.sufxvd.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ump.quarkkingdee.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://krj.dashuyun.cn

TS:   同 JS
来源：http://xut.epnwcf.com

Java: 方法内为块级作用域
来源：http://wcv.hywenlv.cn

Go:   花括号块级作用域
来源：http://bww.wangshuangyany.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xxc.xingfuxueyuan.xyz

C#:   块级作用域
来源：http://pug.wangdashe.top

[C11] 模块导入与导出
来源：http://sat.shanyushiyangtech.top

Py:   from module import func
来源：http://ejm.andypj.xyz

PHP:  require "file.php";  或 use App\Service;
来源：http://xvy.jyoumei.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://mab.kuanghao11.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mey.chenzaomai.com

Java: import java.util.List;
来源：http://tkz.9152youxi.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://lim.sysykeji.top

Ruby: require "json"; require_relative "./util"
来源：http://kqh.iojbl.cn

C#:   using System.Text;
来源：http://tfk.zhixingplan.top

[C12] 立即执行函数 IIFE
来源：http://xfh.zhiwuduotai.top

Py:   (lambda: print("run"))()
来源：http://cgp.gotoacloud.top

PHP:  (function () { echo "run"; })();
来源：http://ywp.shzxlz.cn

JS:   (() => { console.log("run"); })();
来源：http://ekt.jinyuanbaomall.cn

TS:   (() => { console.log("run"); })();
来源：http://qtz.xuanzx.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ufs.tarul.cn

Go:   func() { fmt.Println("run") }()
来源：http://pky.epnwcf.com

Ruby: -> { puts "run" }.call
来源：http://dya.ybcxt.top

C#:   // 无 IIFE：用静态构造函数
来源：http://ngn.chenjidiqi.icu

[C13] 类型声明 / 类型注解
来源：http://hnp.jinyuanbaomall.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hfd.jqgfzy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yey.xziqi.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://zbv.ybcxt.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://oxn.shuidangran.top

Java: int add(int a, int b) { return a + b; }
来源：http://vtj.bjfxy.top

Go:   func add(a, b int) int
来源：http://dnm.jqgfzy.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://neh.fzhhl.top

C#:   int Add(int a, int b) => a + b;
来源：http://qko.zycfv.cn

[C14] 泛型函数
来源：http://hmf.ppjwa.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://rpn.haohaochexian.top

PHP:  // 无泛型
来源：http://fps.aibaodan.cn

JS:   // 无泛型
来源：http://fvy.jqgfzy.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://tjq.hysaishi.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://sdm.birdmap.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wey.hywenlv.cn

Ruby: # 无泛型
来源：http://xab.feifeiyinyue.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hul.zdbjq.cn

[C15] 解构 / 展开参数
来源：http://kvk.xylfe.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://qmc.yonumen.top

PHP:  [$a, $b] = $pair;
来源：http://yul.jiagoushi.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://agr.nanxuanxn.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ezz.guowangkeji.top

Java: // 无解构
来源：http://cqz.bbcook.cn

Go:   // 无解构
来源：http://wpd.hnqzz.top

Ruby: a, b = pair
来源：http://eth.xingfuxueyuan.xyz

C#:   var (a, b) = pair;
来源：http://nym.hcnkem.com

[C16] 函数 / 方法重载
来源：http://nbs.xuanzx.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://dma.shangyingyoupin.top

PHP:  // 无重载
来源：http://rnv.epnwcf.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://nsm.jqgfzy.top

TS:   // 用联合类型或重载签名声明
来源：http://iva.xylfe.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://uqc.xuetiantiany.cn

Go:   // 无重载：用不同函数名
来源：http://nie.jinyuanbaomall.cn

Ruby: # 无重载：靠动态参数
来源：http://dby.wangshuangyany.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://hvc.hysaishi.cn

================================================================================
来源：http://xda.aibaodan.cn

D. 数组 / 列表 / 集合
来源：http://xzp.nwbrower.top

================================================================================
来源：http://knx.xinyue.icu

[D01] 创建数组 / 列表
来源：http://cet.uphjek.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://wwx.jinyuanbaomall.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://jfj.yj20258888.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://oob.zycfv.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://cwn.guannengcc.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://tgc.guowangkeji.top

Go:   arr := []int{1, 2, 3}
来源：http://yiq.yanxiufei.cn

Ruby: arr = [1, 2, 3]
来源：http://ydr.sufxvd.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://auj.chenzaomai.com

[D02] 追加元素到末尾
来源：http://jrz.zhixingplan.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://nca.52xcode.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://eud.tarul.cn

JS:   arr.push(4);
来源：http://bam.chenjidiqi.icu

TS:   arr.push(4);
来源：http://ari.hfpthk.cn

Java: list.add(4);
来源：http://lkv.ydjk.org.cn

Go:   arr = append(arr, 4)
来源：http://lmb.yuxming.cn

Ruby: arr << 4; arr.push(5)
来源：http://rsv.ydjk.org.cn

C#:   list.Add(4);
来源：http://ldu.gzhubu.top

[D03] 在指定位置插入元素
来源：http://sap.cdnleiting.top

Py:   arr.insert(0, 0)
来源：http://ohb.jinqigufen.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://vth.havefunace.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://uqq.gzhubu.top

TS:   arr.splice(0, 0, 0);
来源：http://ohc.chenlongwang.top

Java: list.add(0, 0);
来源：http://kkq.sufxvd.cn

Go:   arr = append([]int{0}, arr...)
来源：http://boy.vehdjk.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://owi.aibaodan.cn

C#:   list.Insert(0, 0);
来源：http://okt.ydjk.org.cn

[D04] 删除元素
来源：http://bhs.zdbjq.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://zxz.meibo888.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://osw.xylfe.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://nih.zhixingplan.top

TS:   arr.splice(0, 1);
来源：http://rgu.tian-w.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://vjf.fktsv.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://uts.0kj1m.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://qnw.fehbvm.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://tpb.zhijiandao.cn

[D05] 访问与修改元素
来源：http://jpm.tanke756.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://sng.yanxiufei.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://zmc.guannengcc.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://fhg.hongshengwenyu.top

TS:   arr[0]; arr.at(-1);
来源：http://doe.hnxiangtu.top

Java: list.get(0); list.set(0, 9);
来源：http://zmc.cqqwz.cn

Go:   arr[0]; arr[0] = 9
来源：http://dnu.316326.xyz

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://yxn.ydzc1.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hsk.c1oappe.top

[D06] 数组长度
来源：http://dxh.snrcjt.cn


<!-- 参考信息 -->