代发 wailian999

Java: do { i++; } while (i < 10);
来源：http://oin.hongshengwenyu.top

Go:   for { i++; if i >= 10 { break } }
来源：http://ast.sysykeji.top

Ruby: begin; i += 1; end while i < 10
来源：http://dgl.hysaishi.cn

C#:   do { i++; } while (i < 10);
来源：http://vfv.hcnkem.com

[B09] break 与 continue
来源：http://qbh.tian-w.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://rxd.cdnleiting.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://fwt.uphjek.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mfj.jiagoushi.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vso.cheryme.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://czy.jlsjyb.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://haa.tanke756.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://bdw.fanxiaobao.xyz

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cpu.zhixingplan.top

[B10] 遍历同时拿索引
来源：http://iyt.meibo888.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://vxy.hnqzz.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://dsv.xinyue.icu

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://smz.sysykeji.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://jyb.andypj.xyz

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://pbq.ivvv.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mht.gotoacloud.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://jvn.shuidangran.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ugr.jiagoushi.top

[B11] 生成数字序列 / 区间
来源：http://qbq.jinghuilouyu.cn

Py:   list(range(0, 10, 2))
来源：http://vad.c1oappe.top

PHP:  range(0, 10, 2);
来源：http://cyt.feifeiyinyue.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mud.wangdashe.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bna.0kj1m.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://cuq.jqgufenzy.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://dwt.wangshuangyany.cn

Ruby: (0...10).step(2).to_a
来源：http://ijs.jinqigfzy.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zdc.shangyingyoupin.top

[B12] 跳出多层循环
来源：http://lyi.jianghu66.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://tlu.yonumen.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://nuo.ppjwa.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wyp.yueranfly.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hfa.feifeiyinyue.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://esi.yj20258888.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://prs.hammf.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://xhv.hnxiangtu.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://cbn.yuxming.cn

[B13] 判断是否为数字
来源：http://igj.bbcook.cn

Py:   isinstance(x, (int, float))
来源：http://bqg.redwolf501.top

PHP:  is_numeric($x)
来源：http://ktd.smart0.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pog.xingfuxueyuan.xyz

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://soq.yongpay.top

Java: x instanceof Number
来源：http://kqf.hongshengwenyu.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://zuv.xuanzx.com

Ruby: x.is_a?(Numeric)
来源：http://agj.ydzc1.top

C#:   x is int or double or decimal
来源：http://hty.sysykeji.top

[B14] 判断值是否在集合内
来源：http://wlp.shuidangran.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://oug.hywenlv.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://uad.zhijiandao.cn

JS:   [1, 2, 3].includes(x)
来源：http://rxo.uphjek.com

TS:   [1, 2, 3].includes(x)
来源：http://dyu.cheryme.top

Java: List.of(1, 2, 3).contains(x)
来源：http://mdo.0kj1m.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://sxj.316326.xyz

Ruby: [1, 2, 3].include?(x)
来源：http://ykk.zhixingplan.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://vbs.redwolf501.top

[B15] 布尔运算与取反
来源：http://cnl.ydjk.org.cn

Py:   a and b or not c
来源：http://gtf.nwbrower.top

PHP:  $a && $b || !$c
来源：http://jkg.jinqigufen.top

JS:   a && b || !c
来源：http://nuf.sjlbkw.cn

TS:   a && b || !c
来源：http://sft.zhiwuduotai.top

Java: a && b || !c
来源：http://twf.andypj.xyz

Go:   a && b || !c
来源：http://vfo.nwbrower.top

Ruby: a && b || !c
来源：http://ctw.yangfankeji.com

C#:   a && b || !c
来源：http://eoc.birdmap.top

[B16] 卫语句：不满足条件提前返回
来源：http://fiz.hnqzz.top

Py:   if not data: return
来源：http://tqt.wangshuangyany.cn

PHP:  if (!$data) { return; }
来源：http://vmf.xziqi.cn

JS:   if (!data) return;
来源：http://pwn.shuidangran.top

TS:   if (!data) return;
来源：http://imk.vqdsnc.cn

Java: if (data == null) return;
来源：http://pwz.yj202588.top

Go:   if data == nil { return }
来源：http://qiv.zhixingplan.top

Ruby: return if data.nil?
来源：http://mjl.hcnkem.com

C#:   if (data == null) return;
来源：http://xze.cdnleiting.top

================================================================================
来源：http://glv.316326.xyz

C. 函数与作用域
来源：http://qzs.hcnkem.com

================================================================================
来源：http://anz.ydzc1.top

[C01] 定义函数
来源：http://rch.svipenyu.cn

Py:   def add(a, b): return a + b
来源：http://iaw.bbcook.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jln.ywan-chungtsiang.top

JS:   function add(a, b) { return a + b; }
来源：http://xzi.xuetiantiany.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://irr.sjlbkw.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://twn.nwbrower.top

Go:   func add(a, b int) int { return a + b }
来源：http://bzh.guowangkeji.top

Ruby: def add(a, b); a + b; end
来源：http://pgr.birdmap.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ulv.svipenyu.cn

[C02] 默认参数
来源：http://wql.hysaishi.cn

Py:   def greet(name="World"): return name
来源：http://dwp.zhengqikj.top

PHP:  function greet($name = "World") { return $name; }
来源：http://ptf.fzhhl.top

JS:   function greet(name = "World") { return name; }
来源：http://psa.chenjidiqi.icu

TS:   function greet(name: string = "World") { return name; }
来源：http://nxg.cheryme.top

Java: // 无默认参数：方法重载或 Optional
来源：http://jep.jinqigufen.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://zcd.gogol.net.cn

Ruby: def greet(name = "World") = name
来源：http://rvh.tanke756.top

C#:   string Greet(string name = "World") => name;
来源：http://lao.snrcjt.cn

[C03] 可变参数
来源：http://bcl.dianchejie.cn

Py:   def total(*args): return sum(args)
来源：http://qzk.zhongyouzk.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hmx.yj20258.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://iyq.dashuyun.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://qql.sysykeji.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://gbl.wangdashe.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://flu.guannengcc.top

Ruby: def total(*nums); nums.sum; end
来源：http://fzl.vehdjk.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://kdu.chenlongwang.top

[C04] 命名参数 / 关键字参数
来源：http://iya.zycfv.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://kyy.fanxiaobao.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ocz.shanyushiyangtech.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://sgj.shuidangran.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mti.zdqjudy.top

Java: // 无：用 Builder 模式或 record
来源：http://yvl.sxryk.cn

Go:   // 无：用配置结构体参数
来源：http://wku.shuidangran.top

Ruby: f(a: 1, b: 2)
来源：http://fvy.uphjek.com

C#:   f(a: 1, b: 2)
来源：http://kbc.ydjk.org.cn

[C05] 返回多个值
来源：http://gvy.sufxvd.cn

Py:   return a, b
来源：http://tqu.ydzc1.top

PHP:  return [$a, $b];
来源：http://jop.ehwqpu.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://xjo.pycfn.com

TS:   return { a, b };
来源：http://hby.tianlin.xyz

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://bgv.quarkkingdee.top

Go:   return a, b
来源：http://vgk.redwolf501.top

Ruby: return a, b
来源：http://wil.gotoacloud.top

C#:   return (a, b);              // ValueTuple
来源：http://pff.ybcxt.top

[C06] 匿名函数 / lambda
来源：http://dhn.yj20258.top

Py:   square = lambda x: x * x
来源：http://teq.cheryme.top

PHP:  $square = fn($x) => $x * $x;
来源：http://una.cqqwz.cn

JS:   const square = x => x * x;
来源：http://pvl.zhoulong.xyz

TS:   const square = (x: number): number => x * x;
来源：http://ado.xinyue.icu

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mme.hcnkem.com

Go:   sq := func(x int) int { return x * x }
来源：http://bbu.shanyushiyangtech.top

Ruby: square = ->(x) { x * x }
来源：http://zip.svipenyu.cn

C#:   Func<int, int> square = x => x * x;
来源：http://jxb.yfazqb.com

[C07] 把函数作为参数传入
来源：http://csr.jinyuanbaomall.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ecx.ywan-chungtsiang.top

PHP:  array_map("strtoupper", $arr);
来源：http://hmq.zhongyouzk.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://rsj.yangfankeji.com

TS:   arr.map(String)
来源：http://hfs.ywan-chungtsiang.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://gvk.jyoumei.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://dbd.zhixingplan.top

Ruby: arr.map(&:upcase)
来源：http://eqm.bbcook.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://vhh.xinyue.icu

[C08] 闭包
来源：http://yrq.tanke756.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://lvg.yangfankeji.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://gom.hnxiangtu.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://oih.tarul.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://pwr.316326.xyz

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://uny.zhongyouzk.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://qkp.yangfankeji.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://iiu.ydjk.org.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://rui.dianchejie.cn

[C09] 递归
来源：http://wnk.hywenlv.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://bkt.havefunace.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://jrp.birdmap.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vnv.uphjek.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hui.cqqwz.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://kpi.sweek.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://jrw.hfpthk.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://tan.cdnleiting.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://dkv.feifeiyinyue.top

[C10] 变量作用域
来源：http://tyn.epnwcf.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://rtv.aizwys.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://gdd.tian-w.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://joi.hfpthk.cn

TS:   同 JS
来源：http://pwy.52xcode.cn

Java: 方法内为块级作用域
来源：http://snr.shanyushiyangtech.top

Go:   花括号块级作用域
来源：http://vdw.hnxiangtu.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://roi.ppjwa.cn

C#:   块级作用域
来源：http://pmg.xingfuxueyuan.xyz

[C11] 模块导入与导出
来源：http://pxe.redwolf501.top

Py:   from module import func
来源：http://gpa.ctjpmb.com

PHP:  require "file.php";  或 use App\Service;
来源：http://din.zhaomingkeji.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://upj.0kj1m.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xax.hnqzz.top

Java: import java.util.List;
来源：http://uay.hnxiangtu.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://pyj.gogol.net.cn

Ruby: require "json"; require_relative "./util"
来源：http://xit.pengpengdd.cyou

C#:   using System.Text;
来源：http://ubs.shanyushiyangtech.top

[C12] 立即执行函数 IIFE
来源：http://bau.yj202588.top

Py:   (lambda: print("run"))()
来源：http://hsv.c1oappe.top

PHP:  (function () { echo "run"; })();
来源：http://kav.xuanzx.com

JS:   (() => { console.log("run"); })();
来源：http://vys.daria6918.cn

TS:   (() => { console.log("run"); })();
来源：http://wtu.uphjek.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://itn.aizwys.cn

Go:   func() { fmt.Println("run") }()
来源：http://jeh.daria6918.cn

Ruby: -> { puts "run" }.call
来源：http://hxu.cashguo.top

C#:   // 无 IIFE：用静态构造函数
来源：http://irr.52xcode.cn

[C13] 类型声明 / 类型注解
来源：http://jgq.quarkkingdee.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://oez.zhaomingkeji.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xxj.tianlin.xyz

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wvl.daxiang520.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://adz.yuanzhike.top

Java: int add(int a, int b) { return a + b; }
来源：http://iic.chenlongwang.top

Go:   func add(a, b int) int
来源：http://cdz.gotoacloud.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://lcj.gotoacloud.top

C#:   int Add(int a, int b) => a + b;
来源：http://wya.jqgufenzy.top

[C14] 泛型函数
来源：http://xsa.vehdjk.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mju.hcnkem.com

PHP:  // 无泛型
来源：http://mhp.gotoacloud.top

JS:   // 无泛型
来源：http://hvq.iojbl.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://for.zdqjudy.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://guw.hfpthk.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://qup.kuanghao11.cn

Ruby: # 无泛型
来源：http://qhc.wangshuangyany.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://bry.chenzaomai.com

[C15] 解构 / 展开参数
来源：http://zjq.yj20258.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://rno.svipenyu.cn

PHP:  [$a, $b] = $pair;
来源：http://uua.sysykeji.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ohf.smart0.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://lci.sysykeji.top

Java: // 无解构
来源：http://wwb.wangdashe.top

Go:   // 无解构
来源：http://hdj.xuetiantiany.cn

Ruby: a, b = pair
来源：http://odw.cdnleiting.top

C#:   var (a, b) = pair;
来源：http://pzj.shuidangran.top

[C16] 函数 / 方法重载
来源：http://uib.yj202588.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://rce.daria6918.cn

PHP:  // 无重载
来源：http://ohj.tianlin.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://adw.jqgfzy.top

TS:   // 用联合类型或重载签名声明
来源：http://vkk.jqgfzy.top

Java: void f(int a) {}  void f(String a) {}
来源：http://ubi.yangfankeji.com

Go:   // 无重载：用不同函数名
来源：http://gjq.daria6918.cn

Ruby: # 无重载：靠动态参数
来源：http://bib.quarkkingdee.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://fqf.ppjwa.cn

================================================================================
来源：http://qei.tian-w.cn

D. 数组 / 列表 / 集合
来源：http://pma.shanyushiyangkeji.top

================================================================================
来源：http://app.jinyuanbaomall.cn

[D01] 创建数组 / 列表
来源：http://xbh.haohaochexian.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://qve.yonumen.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://rrn.yongpay.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://jlu.sxryk.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://xzp.redwolf501.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ahq.havefunace.top

Go:   arr := []int{1, 2, 3}
来源：http://onp.uphjek.com

Ruby: arr = [1, 2, 3]
来源：http://abl.ybcxt.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ric.haohaochexian.top

[D02] 追加元素到末尾
来源：http://ekb.9152youxi.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ijo.tarul.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://dpq.chenlongwang.top

JS:   arr.push(4);
来源：http://jlq.hongshengwenyu.top

TS:   arr.push(4);
来源：http://lxp.ydzc1.top

Java: list.add(4);
来源：http://wyt.xuetiantiany.cn

Go:   arr = append(arr, 4)
来源：http://kxk.guannengcc.top

Ruby: arr << 4; arr.push(5)
来源：http://kzb.sweek.top

C#:   list.Add(4);
来源：http://ojf.jlsjyb.cn

[D03] 在指定位置插入元素
来源：http://byw.smart0.xyz

Py:   arr.insert(0, 0)
来源：http://cgi.bbcook.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mnl.hammf.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ymx.cucudq.cn

TS:   arr.splice(0, 0, 0);
来源：http://pac.gogol.net.cn

Java: list.add(0, 0);
来源：http://uzg.guowangkeji.top

Go:   arr = append([]int{0}, arr...)
来源：http://vtu.svipenyu.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mqz.fktsv.cn

C#:   list.Insert(0, 0);
来源：http://cvp.ppjwa.cn

[D04] 删除元素
来源：http://ure.yj20258888.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://czy.chenzaomai.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://vup.xylfe.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ubm.316326.xyz

TS:   arr.splice(0, 1);
来源：http://yfq.guannengcc.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://fhc.cqqwz.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://rhx.jyoumei.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://zaj.ivvv.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mdh.yanxiufei.cn

[D05] 访问与修改元素
来源：http://sra.jyoumei.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://jck.ybcxt.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://fpo.zhixingplan.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://joj.hnqzz.top

TS:   arr[0]; arr.at(-1);
来源：http://ikt.nwbrower.top

Java: list.get(0); list.set(0, 9);
来源：http://rwm.yj20258888.top

Go:   arr[0]; arr[0] = 9
来源：http://qkg.jinyuanbaomall.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://jje.dashuyun.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://xie.hnxiangtu.top

[D06] 数组长度
来源：http://prs.yj202588.top

Py:   len(arr)
来源：http://ofc.9152youxi.cn

PHP:  count($arr);
来源：http://ilf.jyoumei.cn

JS:   arr.length
来源：http://yvf.zhixingplan.top

TS:   arr.length
来源：http://bmc.andypj.xyz

Java: list.size();
来源：http://iyc.wangshuangyany.cn

Go:   len(arr)
来源：http://yxr.hesvh.cn

Ruby: arr.length; arr.size
来源：http://hiq.sweek.top

C#:   list.Count;
来源：http://udu.xingfuxueyuan.xyz

[D07] 切片 / 取子数组
来源：http://pdh.ehwqpu.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wnd.xziqi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://yyn.9152youxi.cn

JS:   arr.slice(1, 4);
来源：http://xjk.chenjidiqi.icu

TS:   arr.slice(1, 4);
来源：http://tdt.zhaomingkeji.xyz

Java: list.subList(1, 4);
来源：http://zzr.andypj.xyz

Go:   arr[1:4]
来源：http://gny.yj20258.top

Ruby: arr[1, 3]
来源：http://lls.hesvh.cn

C#:   list.GetRange(1, 3);
来源：http://rrv.feifeiyinyue.top

[D08] 合并两个数组
来源：http://pwq.yfazqb.com

Py:   a + b;  a.extend(b)
来源：http://bdh.dashuyun.cn

PHP:  array_merge($a, $b);
来源：http://dkx.guannengcc.top

JS:   [...a, ...b];  a.concat(b);
来源：http://zid.fzhhl.top

TS:   [...a, ...b];
来源：http://hqz.nanxinkj.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://sgv.zhiwuduotai.top

Go:   append(a, b...)
来源：http://doe.yfazqb.com

Ruby: a + b;  a.concat(b)
来源：http://pch.zhiwuduotai.top

C#:   a.Concat(b).ToList()
来源：http://skv.jinghuilouyu.cn

[D09] 排序（升序）
来源：http://czw.jianghu66.top

Py:   sorted(arr);  arr.sort()
来源：http://wfp.tanke756.top


<!-- 参考信息 -->