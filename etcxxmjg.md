代发 wailian999

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wes.316326.xyz

[B06] 遍历字典 / 对象
来源：http://liq.uphjek.com

Py:   for k, v in d.items(): print(k, v)
来源：http://bvv.zhiwuduotai.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://vlb.nanxuanxn.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://twr.sxryk.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rgp.sysykeji.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://kmm.epnwcf.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ixh.bjfxy.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ohy.yuxming.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://tmk.ppjwa.cn

[B07] while 循环
来源：http://hko.vqdsnc.cn

Py:   while i < 10: i += 1
来源：http://swr.tianlin.xyz

PHP:  while ($i < 10) { $i++; }
来源：http://ruj.fengsongda.top

JS:   while (i < 10) { i++; }
来源：http://akj.ppjwa.cn

TS:   while (i < 10) { i++; }
来源：http://asg.zhixingplan.top

Java: while (i < 10) { i++; }
来源：http://tbz.hnxiangtu.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://cun.jianghu66.top

Ruby: while i < 10; i += 1; end
来源：http://gzv.ivvv.top

C#:   while (i < 10) { i++; }
来源：http://ncx.9152youxi.cn

[B08] do-while（至少执行一次）
来源：http://ocv.tianlin.xyz

Py:   # 无 do-while：用 while True + break
来源：http://kux.snrcjt.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://azu.chenlongwang.top

JS:   do { i++; } while (i < 10);
来源：http://hou.pengpengdd.cyou

TS:   do { i++; } while (i < 10);
来源：http://ubr.zhixingplan.top

Java: do { i++; } while (i < 10);
来源：http://mvj.jinyuanbaomall.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://rfm.zycfv.cn

Ruby: begin; i += 1; end while i < 10
来源：http://cym.guannengcc.top

C#:   do { i++; } while (i < 10);
来源：http://rtv.zhoulong.xyz

[B09] break 与 continue
来源：http://ulg.sysykeji.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://yja.cheryme.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://qyb.hywenlv.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://odb.chenjidiqi.icu

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kwx.chenlongwang.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hlw.sweek.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://vct.xziqi.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hck.svipenyu.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ggj.jinghuilouyu.cn

[B10] 遍历同时拿索引
来源：http://mgm.cucudq.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ced.chenlongwang.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://spi.hesvh.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://vcx.ydjk.org.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://irr.cashguo.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ign.yueranfly.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://tvk.aibaodan.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://kbj.mhx1999.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ckm.sweek.top

[B11] 生成数字序列 / 区间
来源：http://siz.zhoulong.xyz

Py:   list(range(0, 10, 2))
来源：http://vom.aizwys.cn

PHP:  range(0, 10, 2);
来源：http://tte.cashguo.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://aqg.fktsv.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://eht.sxryk.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://pbs.svipenyu.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://uic.cucudq.cn

Ruby: (0...10).step(2).to_a
来源：http://vwd.xingfuxueyuan.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hbr.andypj.xyz

[B12] 跳出多层循环
来源：http://pva.iojbl.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://chm.yj20258888.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://mrq.c1oappe.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://fmt.xziqi.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://dui.bjfxy.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://etk.fktsv.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://jgn.vehdjk.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://nnr.yanxiufei.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://pke.jinqigfzy.top

[B13] 判断是否为数字
来源：http://hml.yangfankeji.com

Py:   isinstance(x, (int, float))
来源：http://xmu.sysykeji.top

PHP:  is_numeric($x)
来源：http://orh.sweek.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ptq.tianlin.xyz

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://epf.ywan-chungtsiang.top

Java: x instanceof Number
来源：http://ytc.snrcjt.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://xlu.yongpay.top

Ruby: x.is_a?(Numeric)
来源：http://afa.zycfv.cn

C#:   x is int or double or decimal
来源：http://bte.kuanghao11.cn

[B14] 判断值是否在集合内
来源：http://ihr.yangfankeji.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://tlf.zhoulong.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://cyt.ppjwa.cn

JS:   [1, 2, 3].includes(x)
来源：http://wjk.yuxming.cn

TS:   [1, 2, 3].includes(x)
来源：http://joh.fengsongda.top

Java: List.of(1, 2, 3).contains(x)
来源：http://swc.xuanzx.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://etb.yuanzhike.top

Ruby: [1, 2, 3].include?(x)
来源：http://sfo.hfpthk.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://qyv.yj20258.top

[B15] 布尔运算与取反
来源：http://hse.sysykeji.top

Py:   a and b or not c
来源：http://txe.nwbrower.top

PHP:  $a && $b || !$c
来源：http://ixn.redwolf501.top

JS:   a && b || !c
来源：http://mnm.nanxinkj.top

TS:   a && b || !c
来源：http://mtt.xuetiantiany.cn

Java: a && b || !c
来源：http://baa.yangfankeji.com

Go:   a && b || !c
来源：http://kue.feifeiyinyue.top

Ruby: a && b || !c
来源：http://clr.xinyue.icu

C#:   a && b || !c
来源：http://kyi.ybcxt.top

[B16] 卫语句：不满足条件提前返回
来源：http://kxl.zdqjudy.top

Py:   if not data: return
来源：http://dob.xziqi.cn

PHP:  if (!$data) { return; }
来源：http://izk.hywenlv.cn

JS:   if (!data) return;
来源：http://hbe.aibaodan.cn

TS:   if (!data) return;
来源：http://mlq.xingfuxueyuan.xyz

Java: if (data == null) return;
来源：http://hkn.chenzaomai.com

Go:   if data == nil { return }
来源：http://eae.52xcode.cn

Ruby: return if data.nil?
来源：http://rnz.shuidangran.top

C#:   if (data == null) return;
来源：http://vgi.zycfv.cn

================================================================================
来源：http://bfv.pycfn.com

C. 函数与作用域
来源：http://rhv.zhiwuduotai.top

================================================================================
来源：http://lxe.52xcode.cn

[C01] 定义函数
来源：http://skp.xylfe.cn

Py:   def add(a, b): return a + b
来源：http://rsy.zhoulong.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://uuy.zdqjudy.top

JS:   function add(a, b) { return a + b; }
来源：http://ynm.jinyuanbaomall.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ehq.ydjk.org.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ydb.kuanghao11.cn

Go:   func add(a, b int) int { return a + b }
来源：http://iws.gogol.net.cn

Ruby: def add(a, b); a + b; end
来源：http://mca.gzhubu.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hdl.hnxiangtu.top

[C02] 默认参数
来源：http://gjf.zdbjq.cn

Py:   def greet(name="World"): return name
来源：http://qpw.jiagoushi.top

PHP:  function greet($name = "World") { return $name; }
来源：http://jtm.jinghuilouyu.cn

JS:   function greet(name = "World") { return name; }
来源：http://lzc.daria6918.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://wzm.gotoacloud.top

Java: // 无默认参数：方法重载或 Optional
来源：http://pve.sxryk.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://eqd.ehwqpu.com

Ruby: def greet(name = "World") = name
来源：http://reg.zhiwuduotai.top

C#:   string Greet(string name = "World") => name;
来源：http://bda.jinqigfzy.top

[C03] 可变参数
来源：http://rzl.yangfankeji.com

Py:   def total(*args): return sum(args)
来源：http://bgn.xinyue.icu

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://rzf.ivvv.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://lil.hysaishi.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://lco.zhongyouzk.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ccz.redwolf501.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ffm.zhaomingkeji.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://tqe.hammf.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://rzz.52xcode.cn

[C04] 命名参数 / 关键字参数
来源：http://pam.fktsv.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://olc.pengpengdd.cyou

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://juh.jqgufenzy.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://rwo.iojbl.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://bvr.zdbjq.cn

Java: // 无：用 Builder 模式或 record
来源：http://lwr.xuanzx.com

Go:   // 无：用配置结构体参数
来源：http://ptq.tian-w.cn

Ruby: f(a: 1, b: 2)
来源：http://mri.zdqjudy.top

C#:   f(a: 1, b: 2)
来源：http://wqj.ppjwa.cn

[C05] 返回多个值
来源：http://ktp.jinyuanbaomall.cn

Py:   return a, b
来源：http://pkb.quarkkingdee.top

PHP:  return [$a, $b];
来源：http://nxf.ydjk.org.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://khy.wangdashe.top

TS:   return { a, b };
来源：http://vbz.epnwcf.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://oep.yuxming.cn

Go:   return a, b
来源：http://jnh.pycfn.com

Ruby: return a, b
来源：http://hak.hnxiangtu.top

C#:   return (a, b);              // ValueTuple
来源：http://myf.epnwcf.com

[C06] 匿名函数 / lambda
来源：http://hci.yuanzhike.top

Py:   square = lambda x: x * x
来源：http://cix.shangyingyoupin.top

PHP:  $square = fn($x) => $x * $x;
来源：http://pcc.jqgufenzy.top

JS:   const square = x => x * x;
来源：http://bsy.sxryk.cn

TS:   const square = (x: number): number => x * x;
来源：http://trh.jqgufenzy.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://zcg.andypj.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://ywm.dianchejie.cn

Ruby: square = ->(x) { x * x }
来源：http://gah.guowangkeji.top

C#:   Func<int, int> square = x => x * x;
来源：http://ygp.zdbjq.cn

[C07] 把函数作为参数传入
来源：http://azj.gzhubu.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://sta.zhaomingkeji.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://swf.hywenlv.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xgn.ywan-chungtsiang.top

TS:   arr.map(String)
来源：http://gcg.yj202588.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://tdt.ctjpmb.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://bew.xuanzx.com

Ruby: arr.map(&:upcase)
来源：http://ond.zhongyouzk.top

C#:   arr.Select(s => s.ToUpper())
来源：http://hlk.tarul.cn

[C08] 闭包
来源：http://zxf.fengsongda.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://kbw.yj202588.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ydw.haohaochexian.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://awx.dianchejie.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://dpz.sjlbkw.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://jgf.hysaishi.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ugh.shanyushiyangtech.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mxq.vqdsnc.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://gmk.aizwys.cn

[C09] 递归
来源：http://hhh.jyoumei.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ggb.cashguo.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://bju.zhixingplan.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wat.wangdashe.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rfk.redwolf501.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ill.cucudq.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mky.yj20258888.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://sni.chenlongwang.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://bxa.jqgfzy.top

[C10] 变量作用域
来源：http://dko.yj202588.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://iev.yanxiufei.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://rsv.yanxiufei.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://bxi.gaohongyu789.top

TS:   同 JS
来源：http://hng.quarkkingdee.top

Java: 方法内为块级作用域
来源：http://cym.gogol.net.cn

Go:   花括号块级作用域
来源：http://cqr.havefunace.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://akc.fanxiaobao.xyz

C#:   块级作用域
来源：http://rxg.gzhubu.top

[C11] 模块导入与导出
来源：http://wzn.shangyingyoupin.top

Py:   from module import func
来源：http://dsv.jinghuilouyu.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ovb.dianchejie.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://zvj.smart0.xyz

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hwr.uphjek.com

Java: import java.util.List;
来源：http://xwu.feifeiyinyue.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://cks.fktsv.cn

Ruby: require "json"; require_relative "./util"
来源：http://www.fktsv.cn

C#:   using System.Text;
来源：http://pnm.sjlbkw.cn

[C12] 立即执行函数 IIFE
来源：http://jry.daxiang520.top

Py:   (lambda: print("run"))()
来源：http://own.andypj.xyz

PHP:  (function () { echo "run"; })();
来源：http://jud.dashuyun.cn

JS:   (() => { console.log("run"); })();
来源：http://mkp.xziqi.cn

TS:   (() => { console.log("run"); })();
来源：http://ywc.vqdsnc.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://iso.epnwcf.com

Go:   func() { fmt.Println("run") }()
来源：http://hck.shanyushiyangtech.top

Ruby: -> { puts "run" }.call
来源：http://smz.xuanzx.com

C#:   // 无 IIFE：用静态构造函数
来源：http://lbw.ybcxt.top

[C13] 类型声明 / 类型注解
来源：http://rfh.zhoulong.xyz

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://eyv.shangyingyoupin.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fud.tian-w.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://icx.xingfuxueyuan.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mjs.c1oappe.top

Java: int add(int a, int b) { return a + b; }
来源：http://oic.bbcook.cn

Go:   func add(a, b int) int
来源：http://nli.jqgufenzy.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://eov.zdbjq.cn

C#:   int Add(int a, int b) => a + b;
来源：http://mpw.cheryme.top

[C14] 泛型函数
来源：http://gqe.yangfankeji.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zso.jlsjyb.cn

PHP:  // 无泛型
来源：http://zvb.jinghuilouyu.cn

JS:   // 无泛型
来源：http://szl.ydzc1.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://pzc.vehdjk.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hbv.yangfankeji.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://qnw.zdqjudy.top

Ruby: # 无泛型
来源：http://dwr.yfazqb.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://fpp.yvedp.cn

[C15] 解构 / 展开参数
来源：http://arf.wangshuangyany.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://tsy.gogol.net.cn

PHP:  [$a, $b] = $pair;
来源：http://vko.sweek.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://piw.c1oappe.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://pha.nwbrower.top

Java: // 无解构
来源：http://tuf.smart0.xyz

Go:   // 无解构
来源：http://yix.shangyingyoupin.top

Ruby: a, b = pair
来源：http://qrs.yj20258.top

C#:   var (a, b) = pair;
来源：http://lqc.redwolf501.top

[C16] 函数 / 方法重载
来源：http://tzk.zhiwuduotai.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://kpj.ehwqpu.com

PHP:  // 无重载
来源：http://ltr.xuetiantiany.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://zgr.smart0.xyz

TS:   // 用联合类型或重载签名声明
来源：http://lsk.tarul.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://hnp.hesvh.cn

Go:   // 无重载：用不同函数名
来源：http://myy.shzxlz.cn

Ruby: # 无重载：靠动态参数
来源：http://kli.sxryk.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://evi.jianghu66.top

================================================================================
来源：http://abh.yueranfly.top

D. 数组 / 列表 / 集合
来源：http://lss.9152youxi.cn

================================================================================
来源：http://snj.yanxiufei.cn

[D01] 创建数组 / 列表
来源：http://ytf.chenlongwang.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://dhk.hnxiangtu.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://kgr.nanxuanxn.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://fyc.quarkkingdee.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://mew.zhixingplan.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://fbi.hfpthk.cn

Go:   arr := []int{1, 2, 3}
来源：http://blo.chenlongwang.top

Ruby: arr = [1, 2, 3]
来源：http://rov.hammf.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://siv.smart0.xyz

[D02] 追加元素到末尾
来源：http://lub.ehwqpu.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://pik.fzhhl.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://jso.meibo888.top

JS:   arr.push(4);
来源：http://ihp.yvedp.cn

TS:   arr.push(4);
来源：http://slp.cashguo.top

Java: list.add(4);
来源：http://nlm.chenzaomai.com

Go:   arr = append(arr, 4)
来源：http://qih.guannengcc.top

Ruby: arr << 4; arr.push(5)
来源：http://kqh.jlsjyb.cn

C#:   list.Add(4);
来源：http://kam.smart0.xyz

[D03] 在指定位置插入元素
来源：http://krh.fzhhl.top

Py:   arr.insert(0, 0)
来源：http://uio.dianchejie.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hmc.cashguo.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://dkf.hfpthk.cn

TS:   arr.splice(0, 0, 0);
来源：http://ifb.cucudq.cn

Java: list.add(0, 0);
来源：http://yce.birdmap.top

Go:   arr = append([]int{0}, arr...)
来源：http://cro.ctjpmb.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://bhl.aibaodan.cn

C#:   list.Insert(0, 0);
来源：http://mpy.shanyushiyangtech.top

[D04] 删除元素
来源：http://agj.zycfv.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hws.gogol.net.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://lbz.jinghuilouyu.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ggq.mhx1999.top

TS:   arr.splice(0, 1);
来源：http://hla.epnwcf.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://yhj.bjfxy.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://pke.kuanghao11.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://krt.jinqigufen.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://yuv.yj202588.top

[D05] 访问与修改元素
来源：http://yza.yj20258.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://kpl.zhaomingkeji.xyz

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://arm.redwolf501.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://cut.quarkkingdee.top

TS:   arr[0]; arr.at(-1);
来源：http://irb.zhoulong.xyz

Java: list.get(0); list.set(0, 9);
来源：http://fxw.yj20258888.top

Go:   arr[0]; arr[0] = 9
来源：http://akf.yj20258888.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://bis.yongpay.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://qka.gzhubu.top

[D06] 数组长度
来源：http://hhp.zhongyouzk.top

Py:   len(arr)
来源：http://hez.yj202588.top

PHP:  count($arr);
来源：http://ppf.jinyuanbaomall.cn

JS:   arr.length
来源：http://qrm.jinqigufen.top

TS:   arr.length
来源：http://lkp.jlsjyb.cn


<!-- 参考信息 -->