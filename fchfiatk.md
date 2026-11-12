代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://awm.tarul.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://eys.mhx1999.top

JS:   do { i++; } while (i < 10);
来源：http://aww.tian-w.cn

TS:   do { i++; } while (i < 10);
来源：http://ckz.vqdsnc.cn

Java: do { i++; } while (i < 10);
来源：http://fsu.zhixingplan.top

Go:   for { i++; if i >= 10 { break } }
来源：http://pez.aibaodan.cn

Ruby: begin; i += 1; end while i < 10
来源：http://xmb.yonumen.top

C#:   do { i++; } while (i < 10);
来源：http://uxw.andypj.xyz

[B09] break 与 continue
来源：http://cvg.yonumen.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ndu.xuanzx.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://pad.zhiwuduotai.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hur.guannengcc.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lmh.shzxlz.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hox.mhx1999.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://owo.zhaomingkeji.xyz

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ntm.jinqigufen.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://acb.jqgufenzy.top

[B10] 遍历同时拿索引
来源：http://qkg.vqdsnc.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mgh.sufxvd.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hcf.ybcxt.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wda.fengsongda.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://htc.hnxiangtu.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://got.kuanghao11.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ywu.iojbl.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://uzs.ydjk.org.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://eiw.feifeiyinyue.top

[B11] 生成数字序列 / 区间
来源：http://ieo.jinyuanbaomall.cn

Py:   list(range(0, 10, 2))
来源：http://jkq.jinqigfzy.top

PHP:  range(0, 10, 2);
来源：http://dah.xinyue.icu

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xid.fktsv.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nge.meibo888.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ong.sysykeji.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://plf.jinghuilouyu.cn

Ruby: (0...10).step(2).to_a
来源：http://vwr.hnqzz.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ukm.ehwqpu.com

[B12] 跳出多层循环
来源：http://zig.fengsongda.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://luq.haohaochexian.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://lco.zhiwuduotai.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://roe.zycfv.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ezk.yj20258.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ccu.xylfe.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://dzu.zhongyouzk.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://jbr.jlsjyb.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://yne.gotoacloud.top

[B13] 判断是否为数字
来源：http://fur.xuanzx.com

Py:   isinstance(x, (int, float))
来源：http://hgj.shzxlz.cn

PHP:  is_numeric($x)
来源：http://uyc.shuidangran.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tpx.gzhubu.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://isw.pycfn.com

Java: x instanceof Number
来源：http://cyq.meibo888.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://tur.zhixingplan.top

Ruby: x.is_a?(Numeric)
来源：http://ejp.shuidangran.top

C#:   x is int or double or decimal
来源：http://kwd.quarkkingdee.top

[B14] 判断值是否在集合内
来源：http://xcl.sjlbkw.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://joi.jinqigfzy.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://sys.aibaodan.cn

JS:   [1, 2, 3].includes(x)
来源：http://hly.tianlin.xyz

TS:   [1, 2, 3].includes(x)
来源：http://dtp.xziqi.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://xsv.jiagoushi.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ely.hammf.cn

Ruby: [1, 2, 3].include?(x)
来源：http://jsx.hcnkem.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://thn.feifeiyinyue.top

[B15] 布尔运算与取反
来源：http://gap.hammf.cn

Py:   a and b or not c
来源：http://spx.xuetiantiany.cn

PHP:  $a && $b || !$c
来源：http://gpx.chenzaomai.com

JS:   a && b || !c
来源：http://htf.wangdashe.top

TS:   a && b || !c
来源：http://tuo.hnxiangtu.top

Java: a && b || !c
来源：http://ayq.jiagoushi.top

Go:   a && b || !c
来源：http://txu.ydzc1.top

Ruby: a && b || !c
来源：http://rzg.gzhubu.top

C#:   a && b || !c
来源：http://ihq.hfpthk.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ptk.meibo888.top

Py:   if not data: return
来源：http://luw.yfazqb.com

PHP:  if (!$data) { return; }
来源：http://ikk.xinyue.icu

JS:   if (!data) return;
来源：http://hhd.haohaochexian.top

TS:   if (!data) return;
来源：http://lah.quarkkingdee.top

Java: if (data == null) return;
来源：http://gsh.zdbjq.cn

Go:   if data == nil { return }
来源：http://iwz.chenlongwang.top

Ruby: return if data.nil?
来源：http://nnd.kuanghao11.cn

C#:   if (data == null) return;
来源：http://xxp.c1oappe.top

================================================================================
来源：http://pys.ydjk.org.cn

C. 函数与作用域
来源：http://kdm.feifeiyinyue.top

================================================================================
来源：http://oop.sysykeji.top

[C01] 定义函数
来源：http://tct.tianlin.xyz

Py:   def add(a, b): return a + b
来源：http://jmg.tanke756.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://uam.hammf.cn

JS:   function add(a, b) { return a + b; }
来源：http://lvm.9152youxi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sco.ctjpmb.com

Java: static int add(int a, int b) { return a + b; }
来源：http://dbd.jinqigfzy.top

Go:   func add(a, b int) int { return a + b }
来源：http://krb.jiagoushi.top

Ruby: def add(a, b); a + b; end
来源：http://yaa.jiagoushi.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hen.gaohongyu789.top

[C02] 默认参数
来源：http://zoq.zhaomingkeji.xyz

Py:   def greet(name="World"): return name
来源：http://kqb.nwbrower.top

PHP:  function greet($name = "World") { return $name; }
来源：http://bze.zhiwuduotai.top

JS:   function greet(name = "World") { return name; }
来源：http://mrf.bjfxy.top

TS:   function greet(name: string = "World") { return name; }
来源：http://ljw.jiagoushi.top

Java: // 无默认参数：方法重载或 Optional
来源：http://cyr.andypj.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://nvo.gzhubu.top

Ruby: def greet(name = "World") = name
来源：http://hvx.yvedp.cn

C#:   string Greet(string name = "World") => name;
来源：http://aoq.gaohongyu789.top

[C03] 可变参数
来源：http://vck.jinghuilouyu.cn

Py:   def total(*args): return sum(args)
来源：http://ggf.bjfxy.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ujk.tanke756.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ecn.chenlongwang.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://pih.yj20258.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://aef.zhixingplan.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://tup.hesvh.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ajr.yfazqb.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ydc.fanxiaobao.xyz

[C04] 命名参数 / 关键字参数
来源：http://pjv.tanke756.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://lfo.yj20258888.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://dfr.dianchejie.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://rly.0kj1m.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://khx.sxryk.cn

Java: // 无：用 Builder 模式或 record
来源：http://hes.hnxiangtu.top

Go:   // 无：用配置结构体参数
来源：http://xvo.kuanghao11.cn

Ruby: f(a: 1, b: 2)
来源：http://nff.hnqzz.top

C#:   f(a: 1, b: 2)
来源：http://iwz.tarul.cn

[C05] 返回多个值
来源：http://hlf.yuanzhike.top

Py:   return a, b
来源：http://wut.sweek.top

PHP:  return [$a, $b];
来源：http://fdm.vqdsnc.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://xxx.shzxlz.cn

TS:   return { a, b };
来源：http://new.ppjwa.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hfn.xuanzx.com

Go:   return a, b
来源：http://pjl.tian-w.cn

Ruby: return a, b
来源：http://kup.nwbrower.top

C#:   return (a, b);              // ValueTuple
来源：http://yhy.shanyushiyangtech.top

[C06] 匿名函数 / lambda
来源：http://gwl.vehdjk.com

Py:   square = lambda x: x * x
来源：http://jvp.bjfxy.top

PHP:  $square = fn($x) => $x * $x;
来源：http://mwb.ydjk.org.cn

JS:   const square = x => x * x;
来源：http://bre.cashguo.top

TS:   const square = (x: number): number => x * x;
来源：http://hcm.xingfuxueyuan.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://nih.zdbjq.cn

Go:   sq := func(x int) int { return x * x }
来源：http://gmx.zhengqikj.top

Ruby: square = ->(x) { x * x }
来源：http://pkd.zdbjq.cn

C#:   Func<int, int> square = x => x * x;
来源：http://wny.wangdashe.top

[C07] 把函数作为参数传入
来源：http://wzl.bbcook.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wra.xuetiantiany.cn

PHP:  array_map("strtoupper", $arr);
来源：http://syv.birdmap.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://bjz.cqqwz.cn

TS:   arr.map(String)
来源：http://hgi.jianghu66.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://dms.zhaomingkeji.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://rnr.yonumen.top

Ruby: arr.map(&:upcase)
来源：http://igr.tianlin.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://mmr.xylfe.cn

[C08] 闭包
来源：http://kew.ctjpmb.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://zip.0kj1m.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://rzw.gotoacloud.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://sdm.shzxlz.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://orj.cucudq.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://kvd.uphjek.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://oli.daria6918.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hfd.dianchejie.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://pvq.daria6918.cn

[C09] 递归
来源：http://pui.guowangkeji.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mqj.c1oappe.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://idl.feifeiyinyue.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rip.yueranfly.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jqf.bjfxy.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wdi.havefunace.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mhe.zhiwuduotai.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ucw.sysykeji.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://vzu.zycfv.cn

[C10] 变量作用域
来源：http://avp.zhoulong.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://kep.wangdashe.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://fwp.redwolf501.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://env.yj202588.top

TS:   同 JS
来源：http://bcc.yanxiufei.cn

Java: 方法内为块级作用域
来源：http://tkr.quarkkingdee.top

Go:   花括号块级作用域
来源：http://ojo.hesvh.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://lwb.sjlbkw.cn

C#:   块级作用域
来源：http://rvm.smart0.xyz

[C11] 模块导入与导出
来源：http://htn.9152youxi.cn

Py:   from module import func
来源：http://dbs.wangdashe.top

PHP:  require "file.php";  或 use App\Service;
来源：http://eex.nanxuanxn.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://rsj.fengsongda.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://vyk.0kj1m.cn

Java: import java.util.List;
来源：http://eog.sjlbkw.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://eth.zhaomingkeji.xyz

Ruby: require "json"; require_relative "./util"
来源：http://goj.vqdsnc.cn

C#:   using System.Text;
来源：http://rpd.shuidangran.top

[C12] 立即执行函数 IIFE
来源：http://kwc.daria6918.cn

Py:   (lambda: print("run"))()
来源：http://obb.zdbjq.cn

PHP:  (function () { echo "run"; })();
来源：http://ufh.cashguo.top

JS:   (() => { console.log("run"); })();
来源：http://mia.zhoulong.xyz

TS:   (() => { console.log("run"); })();
来源：http://pvw.jinqigfzy.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://rma.dashuyun.cn

Go:   func() { fmt.Println("run") }()
来源：http://xrx.gzhubu.top

Ruby: -> { puts "run" }.call
来源：http://kuv.yongpay.top

C#:   // 无 IIFE：用静态构造函数
来源：http://asf.hnxiangtu.top

[C13] 类型声明 / 类型注解
来源：http://ffo.jinqigufen.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ekt.zhaomingkeji.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cxg.dashuyun.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://zrb.cucudq.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fkb.c1oappe.top

Java: int add(int a, int b) { return a + b; }
来源：http://evn.ydzc1.top

Go:   func add(a, b int) int
来源：http://nbo.wangshuangyany.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://oih.yonumen.top

C#:   int Add(int a, int b) => a + b;
来源：http://fhd.fanxiaobao.xyz

[C14] 泛型函数
来源：http://ruq.feifeiyinyue.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://jhh.guowangkeji.top

PHP:  // 无泛型
来源：http://nrk.nwbrower.top

JS:   // 无泛型
来源：http://jbv.fehbvm.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://uxr.jqgfzy.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ouz.svipenyu.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mzp.iojbl.cn

Ruby: # 无泛型
来源：http://vuo.0kj1m.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://pxy.gogol.net.cn

[C15] 解构 / 展开参数
来源：http://ewj.zhijiandao.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://adn.nanxuanxn.top

PHP:  [$a, $b] = $pair;
来源：http://kwc.c1oappe.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://cld.jinqigufen.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://fuu.zycfv.cn

Java: // 无解构
来源：http://tdr.yuanzhike.top

Go:   // 无解构
来源：http://rej.zhiwuduotai.top

Ruby: a, b = pair
来源：http://xqm.jyoumei.cn

C#:   var (a, b) = pair;
来源：http://nuu.zhengqikj.top

[C16] 函数 / 方法重载
来源：http://tow.chenlongwang.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://aka.birdmap.top

PHP:  // 无重载
来源：http://wlb.gogol.net.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://miz.52xcode.cn

TS:   // 用联合类型或重载签名声明
来源：http://yrq.hongshengwenyu.top

Java: void f(int a) {}  void f(String a) {}
来源：http://fbo.fzhhl.top

Go:   // 无重载：用不同函数名
来源：http://paf.cucudq.cn

Ruby: # 无重载：靠动态参数
来源：http://qql.epnwcf.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://eec.svipenyu.cn

================================================================================
来源：http://dck.pengpengdd.cyou

D. 数组 / 列表 / 集合
来源：http://htn.gzhubu.top

================================================================================
来源：http://piz.cqqwz.cn

[D01] 创建数组 / 列表
来源：http://dhz.cdnleiting.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://ker.ybcxt.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://qiv.hysaishi.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mde.yj20258888.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://rde.aibaodan.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ski.xziqi.cn

Go:   arr := []int{1, 2, 3}
来源：http://amk.xuetiantiany.cn

Ruby: arr = [1, 2, 3]
来源：http://hgb.andypj.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://tex.shuidangran.top

[D02] 追加元素到末尾
来源：http://drz.jiagoushi.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ocd.ehwqpu.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://bgp.nwbrower.top

JS:   arr.push(4);
来源：http://ixu.cashguo.top

TS:   arr.push(4);
来源：http://zyf.mhx1999.top

Java: list.add(4);
来源：http://hnz.jinyuanbaomall.cn

Go:   arr = append(arr, 4)
来源：http://yxa.xingfuxueyuan.xyz

Ruby: arr << 4; arr.push(5)
来源：http://bgd.ehwqpu.com

C#:   list.Add(4);
来源：http://vvq.redwolf501.top

[D03] 在指定位置插入元素
来源：http://shk.zhoulong.xyz

Py:   arr.insert(0, 0)
来源：http://nzm.52xcode.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ksx.nanxinkj.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mfe.daria6918.cn

TS:   arr.splice(0, 0, 0);
来源：http://nwd.haohaochexian.top

Java: list.add(0, 0);
来源：http://feq.ivvv.top

Go:   arr = append([]int{0}, arr...)
来源：http://yzu.jianghu66.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://prt.0kj1m.cn

C#:   list.Insert(0, 0);
来源：http://ngr.shzxlz.cn

[D04] 删除元素
来源：http://jcf.tanke756.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://dzg.ybcxt.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://rdg.daxiang520.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://toy.mhx1999.top

TS:   arr.splice(0, 1);
来源：http://kph.yanxiufei.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://tpi.c1oappe.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://roh.bjfxy.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://vlf.fehbvm.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://fah.ywan-chungtsiang.top

[D05] 访问与修改元素
来源：http://vfn.gogol.net.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://izo.yvedp.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mfa.zdbjq.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://nty.kuanghao11.cn

TS:   arr[0]; arr.at(-1);
来源：http://esc.xingfuxueyuan.xyz

Java: list.get(0); list.set(0, 9);
来源：http://ssl.jqgufenzy.top

Go:   arr[0]; arr[0] = 9
来源：http://pku.hnqzz.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://fea.yj20258888.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://epw.zhixingplan.top

[D06] 数组长度
来源：http://pgb.ydzc1.top

Py:   len(arr)
来源：http://ryt.yj20258888.top

PHP:  count($arr);
来源：http://ktg.cqqwz.cn

JS:   arr.length
来源：http://nja.yongpay.top

TS:   arr.length
来源：http://acq.nwbrower.top

Java: list.size();
来源：http://lim.hywenlv.cn

Go:   len(arr)
来源：http://ixu.0kj1m.cn

Ruby: arr.length; arr.size
来源：http://nqm.pycfn.com

C#:   list.Count;
来源：http://chb.wangdashe.top

[D07] 切片 / 取子数组
来源：http://srs.shuidangran.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://dgw.cashguo.top

PHP:  array_slice($arr, 1, 3);
来源：http://ixk.bbcook.cn

JS:   arr.slice(1, 4);
来源：http://umq.xingfuxueyuan.xyz

TS:   arr.slice(1, 4);
来源：http://gnf.ctjpmb.com

Java: list.subList(1, 4);
来源：http://hep.yonumen.top

Go:   arr[1:4]
来源：http://ccw.tianlin.xyz

Ruby: arr[1, 3]
来源：http://mqy.hfpthk.cn

C#:   list.GetRange(1, 3);
来源：http://oxe.zhijiandao.cn

[D08] 合并两个数组
来源：http://huq.shanyushiyangtech.top

Py:   a + b;  a.extend(b)
来源：http://nwa.ywan-chungtsiang.top

PHP:  array_merge($a, $b);
来源：http://qld.wangdashe.top

JS:   [...a, ...b];  a.concat(b);
来源：http://dgn.ywan-chungtsiang.top

TS:   [...a, ...b];
来源：http://wlc.xuetiantiany.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://eab.nwbrower.top

Go:   append(a, b...)
来源：http://yte.cucudq.cn


<!-- 参考信息 -->