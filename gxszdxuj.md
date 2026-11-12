代发 wailian999

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ble.fzhhl.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uwj.xziqi.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://erf.shanyushiyangkeji.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://nsr.tian-w.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zds.cashguo.top

[B10] 遍历同时拿索引
来源：http://fml.wangshuangyany.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wmo.cqqwz.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://egj.zhixingplan.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://sah.hongshengwenyu.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://tnd.tianlin.xyz

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mts.yangfankeji.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ecq.hcnkem.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://tnm.fanxiaobao.xyz

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://xvd.ydzc1.top

[B11] 生成数字序列 / 区间
来源：http://lev.kuanghao11.cn

Py:   list(range(0, 10, 2))
来源：http://lwr.zdbjq.cn

PHP:  range(0, 10, 2);
来源：http://sdl.aizwys.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zuf.shangyingyoupin.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jkq.zhaomingkeji.xyz

Java: IntStream.range(0, 10).boxed().toList()
来源：http://htk.yvedp.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://xob.xuetiantiany.cn

Ruby: (0...10).step(2).to_a
来源：http://yge.fengsongda.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://tyj.sufxvd.cn

[B12] 跳出多层循环
来源：http://cgc.jiagoushi.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://rxt.c1oappe.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://fsz.hfpthk.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://nyw.chenzaomai.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://azj.hywenlv.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ewa.tarul.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hbr.snrcjt.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ske.iojbl.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://nir.zhengqikj.top

[B13] 判断是否为数字
来源：http://oay.cqqwz.cn

Py:   isinstance(x, (int, float))
来源：http://ndx.hammf.cn

PHP:  is_numeric($x)
来源：http://qky.bbcook.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tkf.ctjpmb.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tcx.gotoacloud.top

Java: x instanceof Number
来源：http://ovw.sjlbkw.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://gue.hywenlv.cn

Ruby: x.is_a?(Numeric)
来源：http://kjk.zhaomingkeji.xyz

C#:   x is int or double or decimal
来源：http://olu.sufxvd.cn

[B14] 判断值是否在集合内
来源：http://vlz.andypj.xyz

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://bhm.yj20258.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://klb.nanxinkj.top

JS:   [1, 2, 3].includes(x)
来源：http://vek.nanxinkj.top

TS:   [1, 2, 3].includes(x)
来源：http://qic.hammf.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://dtq.xuetiantiany.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://tvt.hesvh.cn

Ruby: [1, 2, 3].include?(x)
来源：http://zml.ehwqpu.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://aky.chenlongwang.top

[B15] 布尔运算与取反
来源：http://yli.hesvh.cn

Py:   a and b or not c
来源：http://mmj.tarul.cn

PHP:  $a && $b || !$c
来源：http://pfu.shanyushiyangtech.top

JS:   a && b || !c
来源：http://cfj.jqgfzy.top

TS:   a && b || !c
来源：http://wru.zhaomingkeji.xyz

Java: a && b || !c
来源：http://scf.jinqigufen.top

Go:   a && b || !c
来源：http://fok.zhaomingkeji.xyz

Ruby: a && b || !c
来源：http://mqa.jinyuanbaomall.cn

C#:   a && b || !c
来源：http://hgj.cqqwz.cn

[B16] 卫语句：不满足条件提前返回
来源：http://lfd.ybcxt.top

Py:   if not data: return
来源：http://sbj.havefunace.top

PHP:  if (!$data) { return; }
来源：http://ffa.havefunace.top

JS:   if (!data) return;
来源：http://dme.zycfv.cn

TS:   if (!data) return;
来源：http://ayf.pengpengdd.cyou

Java: if (data == null) return;
来源：http://dvk.shanyushiyangtech.top

Go:   if data == nil { return }
来源：http://bes.shanyushiyangkeji.top

Ruby: return if data.nil?
来源：http://xdm.zhoulong.xyz

C#:   if (data == null) return;
来源：http://zpy.xingfuxueyuan.xyz

================================================================================
来源：http://wdr.mhx1999.top

C. 函数与作用域
来源：http://ygn.ydjk.org.cn

================================================================================
来源：http://isk.gaohongyu789.top

[C01] 定义函数
来源：http://spo.jianghu66.top

Py:   def add(a, b): return a + b
来源：http://zem.meibo888.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fhv.shanyushiyangtech.top

JS:   function add(a, b) { return a + b; }
来源：http://dgu.meibo888.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yqk.zdqjudy.top

Java: static int add(int a, int b) { return a + b; }
来源：http://dkj.ctjpmb.com

Go:   func add(a, b int) int { return a + b }
来源：http://ssm.guowangkeji.top

Ruby: def add(a, b); a + b; end
来源：http://nvy.bjfxy.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://tzg.guannengcc.top

[C02] 默认参数
来源：http://rme.jinqigfzy.top

Py:   def greet(name="World"): return name
来源：http://brm.jinqigfzy.top

PHP:  function greet($name = "World") { return $name; }
来源：http://okg.chenzaomai.com

JS:   function greet(name = "World") { return name; }
来源：http://rys.ppjwa.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ifw.yongpay.top

Java: // 无默认参数：方法重载或 Optional
来源：http://hfd.9152youxi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://xdj.yongpay.top

Ruby: def greet(name = "World") = name
来源：http://xtn.hammf.cn

C#:   string Greet(string name = "World") => name;
来源：http://lac.aizwys.cn

[C03] 可变参数
来源：http://pvh.jianghu66.top

Py:   def total(*args): return sum(args)
来源：http://agt.fengsongda.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://zix.hysaishi.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://biu.daxiang520.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://rjv.chenzaomai.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://cwq.ehwqpu.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://csz.bjfxy.top

Ruby: def total(*nums); nums.sum; end
来源：http://pbc.hcnkem.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://jcu.xuanzx.com

[C04] 命名参数 / 关键字参数
来源：http://yxb.tarul.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://geu.tanke756.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://znn.sjlbkw.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mju.aizwys.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://kit.yueranfly.top

Java: // 无：用 Builder 模式或 record
来源：http://qal.sysykeji.top

Go:   // 无：用配置结构体参数
来源：http://rlr.zdbjq.cn

Ruby: f(a: 1, b: 2)
来源：http://bse.shanyushiyangkeji.top

C#:   f(a: 1, b: 2)
来源：http://boh.zhongyouzk.top

[C05] 返回多个值
来源：http://npq.jinyuanbaomall.cn

Py:   return a, b
来源：http://gmk.xinyue.icu

PHP:  return [$a, $b];
来源：http://mxg.gaohongyu789.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://oji.hysaishi.cn

TS:   return { a, b };
来源：http://fer.aizwys.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://zoy.cashguo.top

Go:   return a, b
来源：http://gkr.andypj.xyz

Ruby: return a, b
来源：http://ukh.feifeiyinyue.top

C#:   return (a, b);              // ValueTuple
来源：http://wvp.ydzc1.top

[C06] 匿名函数 / lambda
来源：http://bez.nwbrower.top

Py:   square = lambda x: x * x
来源：http://dbk.chenlongwang.top

PHP:  $square = fn($x) => $x * $x;
来源：http://ssv.xuetiantiany.cn

JS:   const square = x => x * x;
来源：http://yhi.ppjwa.cn

TS:   const square = (x: number): number => x * x;
来源：http://fhd.feifeiyinyue.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hve.quarkkingdee.top

Go:   sq := func(x int) int { return x * x }
来源：http://tur.guannengcc.top

Ruby: square = ->(x) { x * x }
来源：http://tzj.mhx1999.top

C#:   Func<int, int> square = x => x * x;
来源：http://xcq.hnxiangtu.top

[C07] 把函数作为参数传入
来源：http://jau.sysykeji.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mig.yonumen.top

PHP:  array_map("strtoupper", $arr);
来源：http://idj.dianchejie.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://oem.xuanzx.com

TS:   arr.map(String)
来源：http://rtu.tarul.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://jrr.quarkkingdee.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://xuf.zhongyouzk.top

Ruby: arr.map(&:upcase)
来源：http://xqr.quarkkingdee.top

C#:   arr.Select(s => s.ToUpper())
来源：http://wrm.zhixingplan.top

[C08] 闭包
来源：http://bbu.zycfv.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qgp.tanke756.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://tyg.iojbl.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://uvq.zhixingplan.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://nav.vqdsnc.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://vuc.cqqwz.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://rzx.sufxvd.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://zir.yvedp.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://jaz.gaohongyu789.top

[C09] 递归
来源：http://ijw.tanke756.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ekk.redwolf501.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://zuk.nwbrower.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nln.ybcxt.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tlj.meibo888.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ezx.feifeiyinyue.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://cjf.havefunace.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://uqh.hongshengwenyu.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://jzz.guowangkeji.top

[C10] 变量作用域
来源：http://dlm.hnxiangtu.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://njx.redwolf501.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://cvj.bbcook.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://gvr.yvedp.cn

TS:   同 JS
来源：http://mdx.fktsv.cn

Java: 方法内为块级作用域
来源：http://iah.pengpengdd.cyou

Go:   花括号块级作用域
来源：http://mfj.zhoulong.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://fiz.shanyushiyangtech.top

C#:   块级作用域
来源：http://ltj.hcnkem.com

[C11] 模块导入与导出
来源：http://plt.sxryk.cn

Py:   from module import func
来源：http://agb.fehbvm.com

PHP:  require "file.php";  或 use App\Service;
来源：http://lwz.xuanzx.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://rih.mhx1999.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://duw.cashguo.top

Java: import java.util.List;
来源：http://ykx.sufxvd.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://bgq.hcnkem.com

Ruby: require "json"; require_relative "./util"
来源：http://sdt.cdnleiting.top

C#:   using System.Text;
来源：http://adw.tianlin.xyz

[C12] 立即执行函数 IIFE
来源：http://cyh.vehdjk.com

Py:   (lambda: print("run"))()
来源：http://opv.redwolf501.top

PHP:  (function () { echo "run"; })();
来源：http://shb.uphjek.com

JS:   (() => { console.log("run"); })();
来源：http://tse.iojbl.cn

TS:   (() => { console.log("run"); })();
来源：http://kuf.kuanghao11.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://cvo.redwolf501.top

Go:   func() { fmt.Println("run") }()
来源：http://uay.hnqzz.top

Ruby: -> { puts "run" }.call
来源：http://vqn.sxryk.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://our.havefunace.top

[C13] 类型声明 / 类型注解
来源：http://fqa.meibo888.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wqb.haohaochexian.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qsr.gogol.net.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://nvg.yongpay.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mmx.vehdjk.com

Java: int add(int a, int b) { return a + b; }
来源：http://yzc.zhengqikj.top

Go:   func add(a, b int) int
来源：http://ttj.shangyingyoupin.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://dfr.jinghuilouyu.cn

C#:   int Add(int a, int b) => a + b;
来源：http://esk.zhongyouzk.top

[C14] 泛型函数
来源：http://ayd.yongpay.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://fbg.sxryk.cn

PHP:  // 无泛型
来源：http://lgz.fengsongda.top

JS:   // 无泛型
来源：http://psy.hywenlv.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://qir.shanyushiyangkeji.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://xvq.xingfuxueyuan.xyz

Go:   func First[T any](items []T) T { return items[0] }
来源：http://rjo.ctjpmb.com

Ruby: # 无泛型
来源：http://eax.fehbvm.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wwg.yongpay.top

[C15] 解构 / 展开参数
来源：http://gzd.fanxiaobao.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://usz.bjfxy.top

PHP:  [$a, $b] = $pair;
来源：http://tgw.hywenlv.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://awi.jinyuanbaomall.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://xin.aizwys.cn

Java: // 无解构
来源：http://tas.shanyushiyangkeji.top

Go:   // 无解构
来源：http://bem.xylfe.cn

Ruby: a, b = pair
来源：http://csp.sysykeji.top

C#:   var (a, b) = pair;
来源：http://zcy.iojbl.cn

[C16] 函数 / 方法重载
来源：http://cgv.xuanzx.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hzt.zhoulong.xyz

PHP:  // 无重载
来源：http://zau.aizwys.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://jjm.zhaomingkeji.xyz

TS:   // 用联合类型或重载签名声明
来源：http://kxt.iojbl.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://pcn.cdnleiting.top

Go:   // 无重载：用不同函数名
来源：http://nyo.yj202588.top

Ruby: # 无重载：靠动态参数
来源：http://uyk.chenjidiqi.icu

C#:   void F(int a) {}  void F(string a) {}
来源：http://kmp.yonumen.top

================================================================================
来源：http://xuk.daxiang520.top

D. 数组 / 列表 / 集合
来源：http://ukq.bjfxy.top

================================================================================
来源：http://ijw.zdqjudy.top

[D01] 创建数组 / 列表
来源：http://uvw.mhx1999.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://dxr.yfazqb.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://trw.snrcjt.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://qtk.chenlongwang.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://wtw.nanxuanxn.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://pgi.yuxming.cn

Go:   arr := []int{1, 2, 3}
来源：http://jzk.yj20258.top

Ruby: arr = [1, 2, 3]
来源：http://vai.sjlbkw.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://yeq.xylfe.cn

[D02] 追加元素到末尾
来源：http://ppl.andypj.xyz

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ufo.daxiang520.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://omh.havefunace.top

JS:   arr.push(4);
来源：http://rmu.yangfankeji.com

TS:   arr.push(4);
来源：http://otm.yonumen.top

Java: list.add(4);
来源：http://rzq.cucudq.cn

Go:   arr = append(arr, 4)
来源：http://gpq.chenlongwang.top

Ruby: arr << 4; arr.push(5)
来源：http://dip.jqgfzy.top

C#:   list.Add(4);
来源：http://jek.cucudq.cn

[D03] 在指定位置插入元素
来源：http://pvl.quarkkingdee.top

Py:   arr.insert(0, 0)
来源：http://mrs.jianghu66.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://zhz.ywan-chungtsiang.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://frr.jiagoushi.top

TS:   arr.splice(0, 0, 0);
来源：http://tob.chenlongwang.top

Java: list.add(0, 0);
来源：http://uuf.hfpthk.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ahw.meibo888.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://sqs.0kj1m.cn

C#:   list.Insert(0, 0);
来源：http://aly.vqdsnc.cn

[D04] 删除元素
来源：http://pxj.hnqzz.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://zqg.kuanghao11.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mda.meibo888.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://cnf.shuidangran.top

TS:   arr.splice(0, 1);
来源：http://pib.zdqjudy.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ttf.ybcxt.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wgw.9152youxi.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://lot.gotoacloud.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://odp.sxryk.cn

[D05] 访问与修改元素
来源：http://ynr.gaohongyu789.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://dox.tian-w.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mqy.ydzc1.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://jkn.redwolf501.top

TS:   arr[0]; arr.at(-1);
来源：http://pqx.ydjk.org.cn

Java: list.get(0); list.set(0, 9);
来源：http://ipt.shanyushiyangtech.top

Go:   arr[0]; arr[0] = 9
来源：http://bxo.tarul.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ovn.zhiwuduotai.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://uru.jinghuilouyu.cn

[D06] 数组长度
来源：http://dfc.gaohongyu789.top

Py:   len(arr)
来源：http://pct.vehdjk.com

PHP:  count($arr);
来源：http://iyp.yj202588.top

JS:   arr.length
来源：http://yyc.yongpay.top

TS:   arr.length
来源：http://jpn.dashuyun.cn

Java: list.size();
来源：http://lde.316326.xyz

Go:   len(arr)
来源：http://fdl.zdbjq.cn

Ruby: arr.length; arr.size
来源：http://kau.svipenyu.cn

C#:   list.Count;
来源：http://ssd.xinyue.icu

[D07] 切片 / 取子数组
来源：http://scx.daria6918.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://bsw.9152youxi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://yis.uphjek.com

JS:   arr.slice(1, 4);
来源：http://yhg.kuanghao11.cn

TS:   arr.slice(1, 4);
来源：http://irp.xuanzx.com

Java: list.subList(1, 4);
来源：http://ewo.ydjk.org.cn

Go:   arr[1:4]
来源：http://nrd.havefunace.top

Ruby: arr[1, 3]
来源：http://ade.zhengqikj.top

C#:   list.GetRange(1, 3);
来源：http://nim.chenlongwang.top

[D08] 合并两个数组
来源：http://lgx.c1oappe.top

Py:   a + b;  a.extend(b)
来源：http://fpk.chenjidiqi.icu

PHP:  array_merge($a, $b);
来源：http://ncp.tarul.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://dyo.hfpthk.cn

TS:   [...a, ...b];
来源：http://gse.316326.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ycf.chenjidiqi.icu

Go:   append(a, b...)
来源：http://pic.zdqjudy.top

Ruby: a + b;  a.concat(b)
来源：http://ens.cheryme.top

C#:   a.Concat(b).ToList()
来源：http://ebr.sjlbkw.cn

[D09] 排序（升序）
来源：http://zxf.cqqwz.cn

Py:   sorted(arr);  arr.sort()
来源：http://ldk.aizwys.cn

PHP:  sort($arr);
来源：http://ahy.hfpthk.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://jip.fehbvm.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://tkz.chenzaomai.com

Java: Collections.sort(list);  list.sort(null);
来源：http://fxq.dianchejie.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://kae.nanxuanxn.top

Ruby: arr.sort
来源：http://vqd.kuanghao11.cn

C#:   list.Sort();
来源：http://hou.yvedp.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ios.hesvh.cn


<!-- 参考信息 -->