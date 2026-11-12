代发 wailian999

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://rdx.zhoulong.xyz

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://omu.jinghuilouyu.cn

[B07] while 循环
来源：http://ptl.tianlin.xyz

Py:   while i < 10: i += 1
来源：http://xew.tianlin.xyz

PHP:  while ($i < 10) { $i++; }
来源：http://utx.bbcook.cn

JS:   while (i < 10) { i++; }
来源：http://xmm.ybcxt.top

TS:   while (i < 10) { i++; }
来源：http://ldm.iojbl.cn

Java: while (i < 10) { i++; }
来源：http://sir.nanxinkj.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://crf.zhijiandao.cn

Ruby: while i < 10; i += 1; end
来源：http://cdq.jiagoushi.top

C#:   while (i < 10) { i++; }
来源：http://fjh.havefunace.top

[B08] do-while（至少执行一次）
来源：http://wsl.aibaodan.cn

Py:   # 无 do-while：用 while True + break
来源：http://phq.guowangkeji.top

PHP:  do { $i++; } while ($i < 10);
来源：http://uia.xylfe.cn

JS:   do { i++; } while (i < 10);
来源：http://lqx.redwolf501.top

TS:   do { i++; } while (i < 10);
来源：http://uaj.tianlin.xyz

Java: do { i++; } while (i < 10);
来源：http://cnz.tanke756.top

Go:   for { i++; if i >= 10 { break } }
来源：http://mxb.sysykeji.top

Ruby: begin; i += 1; end while i < 10
来源：http://alo.nanxinkj.top

C#:   do { i++; } while (i < 10);
来源：http://nlc.wangdashe.top

[B09] break 与 continue
来源：http://jnf.shuidangran.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zes.cqqwz.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://uup.jyoumei.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mtf.yanxiufei.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rjt.shanyushiyangkeji.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yvc.andypj.xyz

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://bbp.ywan-chungtsiang.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://qdl.shzxlz.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zpa.wangshuangyany.cn

[B10] 遍历同时拿索引
来源：http://zgn.yonumen.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://xyr.svipenyu.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://afd.jinqigfzy.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://uix.shangyingyoupin.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://gwa.pycfn.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hwa.tarul.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://jnv.quarkkingdee.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://rnk.daria6918.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://yiy.yanxiufei.cn

[B11] 生成数字序列 / 区间
来源：http://lha.wangdashe.top

Py:   list(range(0, 10, 2))
来源：http://rzk.shuidangran.top

PHP:  range(0, 10, 2);
来源：http://src.cqqwz.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qwf.yuxming.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fil.jqgufenzy.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://pne.aibaodan.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wmr.guannengcc.top

Ruby: (0...10).step(2).to_a
来源：http://xjy.shanyushiyangkeji.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://jno.nwbrower.top

[B12] 跳出多层循环
来源：http://cty.wangshuangyany.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://pne.jinqigfzy.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://rjq.yongpay.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://stz.shangyingyoupin.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://nik.zhengqikj.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://tkq.fehbvm.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://lyr.daria6918.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://vvy.jyoumei.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://fcd.hesvh.cn

[B13] 判断是否为数字
来源：http://yma.316326.xyz

Py:   isinstance(x, (int, float))
来源：http://pzr.zhixingplan.top

PHP:  is_numeric($x)
来源：http://ari.hnxiangtu.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://spu.ydjk.org.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gcl.xingfuxueyuan.xyz

Java: x instanceof Number
来源：http://qgh.shuidangran.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://qwm.316326.xyz

Ruby: x.is_a?(Numeric)
来源：http://cnt.guannengcc.top

C#:   x is int or double or decimal
来源：http://enh.guowangkeji.top

[B14] 判断值是否在集合内
来源：http://dwh.jlsjyb.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jbo.jinqigfzy.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ihl.ivvv.top

JS:   [1, 2, 3].includes(x)
来源：http://vcp.andypj.xyz

TS:   [1, 2, 3].includes(x)
来源：http://lva.tianlin.xyz

Java: List.of(1, 2, 3).contains(x)
来源：http://aue.316326.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://qjt.wangshuangyany.cn

Ruby: [1, 2, 3].include?(x)
来源：http://gtz.yuanzhike.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mnd.zhijiandao.cn

[B15] 布尔运算与取反
来源：http://hdw.svipenyu.cn

Py:   a and b or not c
来源：http://mvr.sufxvd.cn

PHP:  $a && $b || !$c
来源：http://spu.cashguo.top

JS:   a && b || !c
来源：http://ukg.hywenlv.cn

TS:   a && b || !c
来源：http://hcm.sufxvd.cn

Java: a && b || !c
来源：http://pgq.bbcook.cn

Go:   a && b || !c
来源：http://mkf.epnwcf.com

Ruby: a && b || !c
来源：http://kfa.chenzaomai.com

C#:   a && b || !c
来源：http://ass.gotoacloud.top

[B16] 卫语句：不满足条件提前返回
来源：http://kjd.xinyue.icu

Py:   if not data: return
来源：http://tea.havefunace.top

PHP:  if (!$data) { return; }
来源：http://hby.fktsv.cn

JS:   if (!data) return;
来源：http://srg.gotoacloud.top

TS:   if (!data) return;
来源：http://ejw.9152youxi.cn

Java: if (data == null) return;
来源：http://gyu.havefunace.top

Go:   if data == nil { return }
来源：http://uvs.xuanzx.com

Ruby: return if data.nil?
来源：http://aoy.aizwys.cn

C#:   if (data == null) return;
来源：http://fuh.hnqzz.top

================================================================================
来源：http://wko.chenlongwang.top

C. 函数与作用域
来源：http://kwr.52xcode.cn

================================================================================
来源：http://wed.gzhubu.top

[C01] 定义函数
来源：http://oxe.pycfn.com

Py:   def add(a, b): return a + b
来源：http://zyr.shanyushiyangtech.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://awk.yonumen.top

JS:   function add(a, b) { return a + b; }
来源：http://ypp.ydjk.org.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sst.jinyuanbaomall.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://yse.hammf.cn

Go:   func add(a, b int) int { return a + b }
来源：http://kkg.tianlin.xyz

Ruby: def add(a, b); a + b; end
来源：http://cff.pycfn.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ldq.chenzaomai.com

[C02] 默认参数
来源：http://tph.andypj.xyz

Py:   def greet(name="World"): return name
来源：http://eve.yj202588.top

PHP:  function greet($name = "World") { return $name; }
来源：http://ymg.jiagoushi.top

JS:   function greet(name = "World") { return name; }
来源：http://nfl.jinqigfzy.top

TS:   function greet(name: string = "World") { return name; }
来源：http://tel.0kj1m.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://jiw.gotoacloud.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ztl.shanyushiyangtech.top

Ruby: def greet(name = "World") = name
来源：http://mkb.gotoacloud.top

C#:   string Greet(string name = "World") => name;
来源：http://pvp.tarul.cn

[C03] 可变参数
来源：http://ref.fengsongda.top

Py:   def total(*args): return sum(args)
来源：http://asz.redwolf501.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xqx.cucudq.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://qeg.zdbjq.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://pgw.fktsv.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mbc.svipenyu.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://eem.epnwcf.com

Ruby: def total(*nums); nums.sum; end
来源：http://jtp.redwolf501.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://xux.hnxiangtu.top

[C04] 命名参数 / 关键字参数
来源：http://tii.nanxinkj.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://isr.cheryme.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://zdz.jlsjyb.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://acr.jqgfzy.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://rdr.yanxiufei.cn

Java: // 无：用 Builder 模式或 record
来源：http://djr.yj20258888.top

Go:   // 无：用配置结构体参数
来源：http://ejz.ydjk.org.cn

Ruby: f(a: 1, b: 2)
来源：http://mtf.quarkkingdee.top

C#:   f(a: 1, b: 2)
来源：http://hdl.zhaomingkeji.xyz

[C05] 返回多个值
来源：http://tfu.zhixingplan.top

Py:   return a, b
来源：http://ctk.zycfv.cn

PHP:  return [$a, $b];
来源：http://xul.svipenyu.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ccu.chenjidiqi.icu

TS:   return { a, b };
来源：http://haq.kuanghao11.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ndg.9152youxi.cn

Go:   return a, b
来源：http://smr.ctjpmb.com

Ruby: return a, b
来源：http://okw.pycfn.com

C#:   return (a, b);              // ValueTuple
来源：http://yat.cqqwz.cn

[C06] 匿名函数 / lambda
来源：http://dxm.52xcode.cn

Py:   square = lambda x: x * x
来源：http://plj.ivvv.top

PHP:  $square = fn($x) => $x * $x;
来源：http://mcl.jianghu66.top

JS:   const square = x => x * x;
来源：http://lzw.xingfuxueyuan.xyz

TS:   const square = (x: number): number => x * x;
来源：http://pnr.chenzaomai.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://zcr.sjlbkw.cn

Go:   sq := func(x int) int { return x * x }
来源：http://xzr.birdmap.top

Ruby: square = ->(x) { x * x }
来源：http://fvs.yfazqb.com

C#:   Func<int, int> square = x => x * x;
来源：http://jyj.nwbrower.top

[C07] 把函数作为参数传入
来源：http://yxi.mhx1999.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://cub.fzhhl.top

PHP:  array_map("strtoupper", $arr);
来源：http://ldi.gotoacloud.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wof.jqgfzy.top

TS:   arr.map(String)
来源：http://dhe.sysykeji.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://sqn.chenlongwang.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://kfg.wangdashe.top

Ruby: arr.map(&:upcase)
来源：http://plo.jqgfzy.top

C#:   arr.Select(s => s.ToUpper())
来源：http://ell.cdnleiting.top

[C08] 闭包
来源：http://cqu.chenlongwang.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://poo.zhengqikj.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ueg.hammf.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ukg.ivvv.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://aqn.hysaishi.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://gpd.wangshuangyany.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://uhm.yj202588.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://gdz.hywenlv.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mcq.daxiang520.top

[C09] 递归
来源：http://onr.jyoumei.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://nlq.dianchejie.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://kbb.aibaodan.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ttv.yj20258.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://muu.shangyingyoupin.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://qrs.fanxiaobao.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://aeu.jqgfzy.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xzx.cashguo.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://fnz.zdqjudy.top

[C10] 变量作用域
来源：http://evo.gogol.net.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://jhs.zhoulong.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://lxh.tian-w.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://bmg.tarul.cn

TS:   同 JS
来源：http://zyp.jiagoushi.top

Java: 方法内为块级作用域
来源：http://tjr.zdqjudy.top

Go:   花括号块级作用域
来源：http://njc.jinqigfzy.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wkk.guowangkeji.top

C#:   块级作用域
来源：http://heu.sweek.top

[C11] 模块导入与导出
来源：http://rxf.jinyuanbaomall.cn

Py:   from module import func
来源：http://cbw.gogol.net.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://pru.svipenyu.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://fst.nwbrower.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://yln.vqdsnc.cn

Java: import java.util.List;
来源：http://mom.ehwqpu.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://kfo.ydzc1.top

Ruby: require "json"; require_relative "./util"
来源：http://bep.fzhhl.top

C#:   using System.Text;
来源：http://pmz.tarul.cn

[C12] 立即执行函数 IIFE
来源：http://trr.gotoacloud.top

Py:   (lambda: print("run"))()
来源：http://uzw.ydjk.org.cn

PHP:  (function () { echo "run"; })();
来源：http://wtq.yj20258888.top

JS:   (() => { console.log("run"); })();
来源：http://zec.ydjk.org.cn

TS:   (() => { console.log("run"); })();
来源：http://vrv.316326.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://aqw.smart0.xyz

Go:   func() { fmt.Println("run") }()
来源：http://was.jinyuanbaomall.cn

Ruby: -> { puts "run" }.call
来源：http://yli.sjlbkw.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://cnf.sxryk.cn

[C13] 类型声明 / 类型注解
来源：http://jmm.hnqzz.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://jrw.9152youxi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hss.yanxiufei.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://iqc.zdbjq.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vnh.gogol.net.cn

Java: int add(int a, int b) { return a + b; }
来源：http://jnd.smart0.xyz

Go:   func add(a, b int) int
来源：http://zgm.daxiang520.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ruq.ctjpmb.com

C#:   int Add(int a, int b) => a + b;
来源：http://etd.jyoumei.cn

[C14] 泛型函数
来源：http://kvq.guannengcc.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mic.nwbrower.top

PHP:  // 无泛型
来源：http://yvr.cqqwz.cn

JS:   // 无泛型
来源：http://ppr.svipenyu.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://iuf.quarkkingdee.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://cun.sufxvd.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ais.xingfuxueyuan.xyz

Ruby: # 无泛型
来源：http://ton.iojbl.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://fxw.zdqjudy.top

[C15] 解构 / 展开参数
来源：http://ycs.zhaomingkeji.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://fzy.zhiwuduotai.top

PHP:  [$a, $b] = $pair;
来源：http://oud.fktsv.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://img.52xcode.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://xmd.jqgfzy.top

Java: // 无解构
来源：http://que.xingfuxueyuan.xyz

Go:   // 无解构
来源：http://qbm.fehbvm.com

Ruby: a, b = pair
来源：http://qzk.cdnleiting.top

C#:   var (a, b) = pair;
来源：http://xmy.fengsongda.top

[C16] 函数 / 方法重载
来源：http://nwv.gogol.net.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://rdm.zhoulong.xyz

PHP:  // 无重载
来源：http://mgu.jlsjyb.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ggc.gotoacloud.top

TS:   // 用联合类型或重载签名声明
来源：http://gun.ywan-chungtsiang.top

Java: void f(int a) {}  void f(String a) {}
来源：http://pul.hysaishi.cn

Go:   // 无重载：用不同函数名
来源：http://hzb.fzhhl.top

Ruby: # 无重载：靠动态参数
来源：http://xbr.smart0.xyz

C#:   void F(int a) {}  void F(string a) {}
来源：http://quv.cashguo.top

================================================================================
来源：http://wlw.jlsjyb.cn

D. 数组 / 列表 / 集合
来源：http://ine.chenjidiqi.icu

================================================================================
来源：http://gnm.zhengqikj.top

[D01] 创建数组 / 列表
来源：http://bhw.c1oappe.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://sdq.birdmap.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://dcf.wangdashe.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://toq.yongpay.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://esb.svipenyu.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://eky.fengsongda.top

Go:   arr := []int{1, 2, 3}
来源：http://mpj.jiagoushi.top

Ruby: arr = [1, 2, 3]
来源：http://ovw.jqgufenzy.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://otv.gotoacloud.top

[D02] 追加元素到末尾
来源：http://atx.zhiwuduotai.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hyo.yj20258.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://pjy.iojbl.cn

JS:   arr.push(4);
来源：http://vmw.fzhhl.top

TS:   arr.push(4);
来源：http://uwl.jinqigfzy.top

Java: list.add(4);
来源：http://trc.ctjpmb.com

Go:   arr = append(arr, 4)
来源：http://shd.jinghuilouyu.cn

Ruby: arr << 4; arr.push(5)
来源：http://flf.jianghu66.top

C#:   list.Add(4);
来源：http://ond.cqqwz.cn

[D03] 在指定位置插入元素
来源：http://cxh.sysykeji.top

Py:   arr.insert(0, 0)
来源：http://eau.zhijiandao.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://yrs.meibo888.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://dhp.gzhubu.top

TS:   arr.splice(0, 0, 0);
来源：http://kug.xuetiantiany.cn

Java: list.add(0, 0);
来源：http://hxl.ybcxt.top

Go:   arr = append([]int{0}, arr...)
来源：http://rlc.cdnleiting.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://neb.jianghu66.top

C#:   list.Insert(0, 0);
来源：http://czf.tarul.cn

[D04] 删除元素
来源：http://vqp.iojbl.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://zbl.cucudq.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hrb.pycfn.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://uaf.fengsongda.top

TS:   arr.splice(0, 1);
来源：http://wja.wangdashe.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://amx.fehbvm.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://zag.316326.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://idy.shuidangran.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://zii.hnxiangtu.top

[D05] 访问与修改元素
来源：http://sln.uphjek.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://oqq.hnqzz.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://lro.chenlongwang.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://yxa.chenjidiqi.icu

TS:   arr[0]; arr.at(-1);
来源：http://ciz.zhongyouzk.top

Java: list.get(0); list.set(0, 9);
来源：http://bdh.fzhhl.top

Go:   arr[0]; arr[0] = 9
来源：http://iou.yueranfly.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://zhn.hesvh.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://rsp.zhixingplan.top

[D06] 数组长度
来源：http://kzj.yj20258888.top

Py:   len(arr)
来源：http://kao.zycfv.cn

PHP:  count($arr);
来源：http://yzh.yanxiufei.cn

JS:   arr.length
来源：http://jhb.0kj1m.cn

TS:   arr.length
来源：http://dbi.feifeiyinyue.top

Java: list.size();
来源：http://elx.snrcjt.cn

Go:   len(arr)
来源：http://zda.tianlin.xyz

Ruby: arr.length; arr.size
来源：http://ztf.zhixingplan.top

C#:   list.Count;
来源：http://phn.0kj1m.cn

[D07] 切片 / 取子数组
来源：http://hvt.fktsv.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qoe.zhoulong.xyz

PHP:  array_slice($arr, 1, 3);
来源：http://vst.yj20258.top

JS:   arr.slice(1, 4);
来源：http://ypw.jqgufenzy.top


<!-- 参考信息 -->