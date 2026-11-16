代发 wailian999

Java: do { i++; } while (i < 10);
来源：http://zng.sjlbkw.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ejc.tian-w.cn

Ruby: begin; i += 1; end while i < 10
来源：http://cdo.cucudq.cn

C#:   do { i++; } while (i < 10);
来源：http://gfk.fehbvm.com

[B09] break 与 continue
来源：http://har.xylfe.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://xpe.sysykeji.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://fom.yj20258888.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cnc.nwbrower.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zbb.iojbl.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://phb.c1oappe.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://thc.yfazqb.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://rsn.birdmap.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ybi.shanyushiyangtech.top

[B10] 遍历同时拿索引
来源：http://etj.cdnleiting.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://gnt.hesvh.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ehq.nanxuanxn.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://efw.snrcjt.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://cfs.yueranfly.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://gzw.ydzc1.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://svk.mhx1999.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://cpv.xinyue.icu

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ldh.snrcjt.cn

[B11] 生成数字序列 / 区间
来源：http://fsw.aizwys.cn

Py:   list(range(0, 10, 2))
来源：http://dts.sxryk.cn

PHP:  range(0, 10, 2);
来源：http://nui.zhaomingkeji.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://adj.fzhhl.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fax.xuetiantiany.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://olr.quarkkingdee.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://uho.feifeiyinyue.top

Ruby: (0...10).step(2).to_a
来源：http://zpp.zhiwuduotai.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wyq.aizwys.cn

[B12] 跳出多层循环
来源：http://dza.andypj.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://vip.shanyushiyangtech.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://okn.havefunace.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://urh.yj20258.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://zvu.meibo888.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://jjt.chenlongwang.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hjm.daxiang520.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://pjq.yfazqb.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ffw.fehbvm.com

[B13] 判断是否为数字
来源：http://ecy.sufxvd.cn

Py:   isinstance(x, (int, float))
来源：http://nlo.shanyushiyangkeji.top

PHP:  is_numeric($x)
来源：http://prj.zhoulong.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qsz.zhiwuduotai.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ixl.hywenlv.cn

Java: x instanceof Number
来源：http://rwx.wangshuangyany.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ffb.fehbvm.com

Ruby: x.is_a?(Numeric)
来源：http://eaj.gzhubu.top

C#:   x is int or double or decimal
来源：http://xbp.smart0.xyz

[B14] 判断值是否在集合内
来源：http://xcp.gotoacloud.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://bqy.xuanzx.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://aqg.nanxinkj.top

JS:   [1, 2, 3].includes(x)
来源：http://tla.hammf.cn

TS:   [1, 2, 3].includes(x)
来源：http://bqw.hfpthk.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://irh.zhixingplan.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ovp.haohaochexian.top

Ruby: [1, 2, 3].include?(x)
来源：http://wdv.52xcode.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ngg.xylfe.cn

[B15] 布尔运算与取反
来源：http://ceo.gzhubu.top

Py:   a and b or not c
来源：http://jqq.gzhubu.top

PHP:  $a && $b || !$c
来源：http://qsg.ctjpmb.com

JS:   a && b || !c
来源：http://the.vehdjk.com

TS:   a && b || !c
来源：http://xbg.feifeiyinyue.top

Java: a && b || !c
来源：http://wim.pengpengdd.cyou

Go:   a && b || !c
来源：http://smi.aizwys.cn

Ruby: a && b || !c
来源：http://urf.chenzaomai.com

C#:   a && b || !c
来源：http://nlk.zhixingplan.top

[B16] 卫语句：不满足条件提前返回
来源：http://jax.zhixingplan.top

Py:   if not data: return
来源：http://zwq.shanyushiyangtech.top

PHP:  if (!$data) { return; }
来源：http://ydw.chenzaomai.com

JS:   if (!data) return;
来源：http://esq.ydjk.org.cn

TS:   if (!data) return;
来源：http://knn.hnqzz.top

Java: if (data == null) return;
来源：http://rxj.guannengcc.top

Go:   if data == nil { return }
来源：http://utd.xuanzx.com

Ruby: return if data.nil?
来源：http://tcn.nwbrower.top

C#:   if (data == null) return;
来源：http://red.hnqzz.top

================================================================================
来源：http://knu.jqgufenzy.top

C. 函数与作用域
来源：http://qgc.nwbrower.top

================================================================================
来源：http://oxc.iojbl.cn

[C01] 定义函数
来源：http://ohm.jyoumei.cn

Py:   def add(a, b): return a + b
来源：http://rdn.zdqjudy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rlb.epnwcf.com

JS:   function add(a, b) { return a + b; }
来源：http://uwi.yueranfly.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wzs.shangyingyoupin.top

Java: static int add(int a, int b) { return a + b; }
来源：http://vda.jinqigfzy.top

Go:   func add(a, b int) int { return a + b }
来源：http://jfg.sxryk.cn

Ruby: def add(a, b); a + b; end
来源：http://rkc.xziqi.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://han.cdnleiting.top

[C02] 默认参数
来源：http://faw.cqqwz.cn

Py:   def greet(name="World"): return name
来源：http://lrk.ydzc1.top

PHP:  function greet($name = "World") { return $name; }
来源：http://aej.jinqigufen.top

JS:   function greet(name = "World") { return name; }
来源：http://kyf.jinghuilouyu.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://qgp.zhijiandao.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://lyh.cheryme.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://epq.nwbrower.top

Ruby: def greet(name = "World") = name
来源：http://uwy.yvedp.cn

C#:   string Greet(string name = "World") => name;
来源：http://gfx.hnxiangtu.top

[C03] 可变参数
来源：http://drc.hesvh.cn

Py:   def total(*args): return sum(args)
来源：http://ojl.guannengcc.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://aqd.shanyushiyangtech.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://bhi.yuxming.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ujo.daria6918.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://swy.zhoulong.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://zal.jinqigufen.top

Ruby: def total(*nums); nums.sum; end
来源：http://wod.guowangkeji.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://cvm.nwbrower.top

[C04] 命名参数 / 关键字参数
来源：http://cdy.hywenlv.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://cbo.fktsv.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://jtq.fanxiaobao.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://pfw.xinyue.icu

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://clr.bbcook.cn

Java: // 无：用 Builder 模式或 record
来源：http://ihe.fehbvm.com

Go:   // 无：用配置结构体参数
来源：http://wft.zhijiandao.cn

Ruby: f(a: 1, b: 2)
来源：http://vlo.ydjk.org.cn

C#:   f(a: 1, b: 2)
来源：http://lpk.xziqi.cn

[C05] 返回多个值
来源：http://eqx.feifeiyinyue.top

Py:   return a, b
来源：http://ipf.uphjek.com

PHP:  return [$a, $b];
来源：http://ivd.cucudq.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://eex.yj20258.top

TS:   return { a, b };
来源：http://eai.mhx1999.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://dgf.ywan-chungtsiang.top

Go:   return a, b
来源：http://tzx.cqqwz.cn

Ruby: return a, b
来源：http://vwl.iojbl.cn

C#:   return (a, b);              // ValueTuple
来源：http://qlz.shuidangran.top

[C06] 匿名函数 / lambda
来源：http://jlb.zhoulong.xyz

Py:   square = lambda x: x * x
来源：http://xmd.hcnkem.com

PHP:  $square = fn($x) => $x * $x;
来源：http://pkx.hywenlv.cn

JS:   const square = x => x * x;
来源：http://yiy.dashuyun.cn

TS:   const square = (x: number): number => x * x;
来源：http://jyp.shuidangran.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://whm.hammf.cn

Go:   sq := func(x int) int { return x * x }
来源：http://qkv.redwolf501.top

Ruby: square = ->(x) { x * x }
来源：http://vuu.yangfankeji.com

C#:   Func<int, int> square = x => x * x;
来源：http://ihj.zhixingplan.top

[C07] 把函数作为参数传入
来源：http://nwr.shangyingyoupin.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://qel.hongshengwenyu.top

PHP:  array_map("strtoupper", $arr);
来源：http://vij.xuanzx.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://rsg.0kj1m.cn

TS:   arr.map(String)
来源：http://fla.zhixingplan.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://jwg.zhixingplan.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://fao.sufxvd.cn

Ruby: arr.map(&:upcase)
来源：http://yjn.ywan-chungtsiang.top

C#:   arr.Select(s => s.ToUpper())
来源：http://wvy.jyoumei.cn

[C08] 闭包
来源：http://rzg.shanyushiyangkeji.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://rxa.uphjek.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mud.zhengqikj.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hhs.yongpay.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://jyq.daria6918.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://lki.wangshuangyany.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hxn.mhx1999.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hde.cqqwz.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://cmb.fanxiaobao.xyz

[C09] 递归
来源：http://spt.guowangkeji.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://tkw.fengsongda.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://npu.quarkkingdee.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kfp.316326.xyz

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qwn.hcnkem.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://bjr.nanxuanxn.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://nql.yueranfly.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://czk.tanke756.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://yng.tian-w.cn

[C10] 变量作用域
来源：http://eyl.cucudq.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://uve.ivvv.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://zsq.jinghuilouyu.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://cva.meibo888.top

TS:   同 JS
来源：http://kza.vqdsnc.cn

Java: 方法内为块级作用域
来源：http://jap.zdbjq.cn

Go:   花括号块级作用域
来源：http://cka.iojbl.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ggm.vqdsnc.cn

C#:   块级作用域
来源：http://wwj.nanxinkj.top

[C11] 模块导入与导出
来源：http://dzg.jinqigufen.top

Py:   from module import func
来源：http://cek.guowangkeji.top

PHP:  require "file.php";  或 use App\Service;
来源：http://jmt.jqgfzy.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://iml.haohaochexian.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://bzd.ivvv.top

Java: import java.util.List;
来源：http://wnr.yanxiufei.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://fzg.316326.xyz

Ruby: require "json"; require_relative "./util"
来源：http://wst.uphjek.com

C#:   using System.Text;
来源：http://cou.yvedp.cn

[C12] 立即执行函数 IIFE
来源：http://ycu.vehdjk.com

Py:   (lambda: print("run"))()
来源：http://ehv.hysaishi.cn

PHP:  (function () { echo "run"; })();
来源：http://pya.yuanzhike.top

JS:   (() => { console.log("run"); })();
来源：http://eta.gotoacloud.top

TS:   (() => { console.log("run"); })();
来源：http://vne.hfpthk.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://dcw.yj20258888.top

Go:   func() { fmt.Println("run") }()
来源：http://cvv.tianlin.xyz

Ruby: -> { puts "run" }.call
来源：http://ucy.ydjk.org.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://hwi.ctjpmb.com

[C13] 类型声明 / 类型注解
来源：http://alh.uphjek.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://bgi.yuxming.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kdg.ydzc1.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://arp.jqgufenzy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yhm.cucudq.cn

Java: int add(int a, int b) { return a + b; }
来源：http://qoy.aibaodan.cn

Go:   func add(a, b int) int
来源：http://pvy.andypj.xyz

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://jju.tanke756.top

C#:   int Add(int a, int b) => a + b;
来源：http://jjq.tianlin.xyz

[C14] 泛型函数
来源：http://lpw.xuanzx.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://eua.yanxiufei.cn

PHP:  // 无泛型
来源：http://ntg.chenjidiqi.icu

JS:   // 无泛型
来源：http://trz.sweek.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://pcm.jqgufenzy.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://gmj.nanxinkj.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://gwt.hywenlv.cn

Ruby: # 无泛型
来源：http://zcl.havefunace.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://dhy.yongpay.top

[C15] 解构 / 展开参数
来源：http://ylg.fehbvm.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xtg.ydjk.org.cn

PHP:  [$a, $b] = $pair;
来源：http://xmp.iojbl.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://kkx.sjlbkw.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ony.c1oappe.top

Java: // 无解构
来源：http://tbo.yanxiufei.cn

Go:   // 无解构
来源：http://szw.zycfv.cn

Ruby: a, b = pair
来源：http://veh.shanyushiyangtech.top

C#:   var (a, b) = pair;
来源：http://wor.9152youxi.cn

[C16] 函数 / 方法重载
来源：http://tfs.ehwqpu.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://icg.xinyue.icu

PHP:  // 无重载
来源：http://clk.uphjek.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://fhi.fzhhl.top

TS:   // 用联合类型或重载签名声明
来源：http://hvr.jlsjyb.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://rlp.hesvh.cn

Go:   // 无重载：用不同函数名
来源：http://jxj.iojbl.cn

Ruby: # 无重载：靠动态参数
来源：http://zwv.chenjidiqi.icu

C#:   void F(int a) {}  void F(string a) {}
来源：http://snt.yanxiufei.cn

================================================================================
来源：http://qtd.ybcxt.top

D. 数组 / 列表 / 集合
来源：http://yhm.yfazqb.com

================================================================================
来源：http://plq.aibaodan.cn

[D01] 创建数组 / 列表
来源：http://wqh.gotoacloud.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://rvx.vqdsnc.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://qri.wangshuangyany.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hvl.fktsv.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://nvz.jinyuanbaomall.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://kiz.yuanzhike.top

Go:   arr := []int{1, 2, 3}
来源：http://ygd.yj20258888.top

Ruby: arr = [1, 2, 3]
来源：http://ozr.pycfn.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://kms.shuidangran.top

[D02] 追加元素到末尾
来源：http://ofo.redwolf501.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://bmd.ydjk.org.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hqe.kuanghao11.cn

JS:   arr.push(4);
来源：http://ely.jinyuanbaomall.cn

TS:   arr.push(4);
来源：http://pjn.zhongyouzk.top

Java: list.add(4);
来源：http://lpw.zhaomingkeji.xyz

Go:   arr = append(arr, 4)
来源：http://jyh.ywan-chungtsiang.top

Ruby: arr << 4; arr.push(5)
来源：http://yav.feifeiyinyue.top

C#:   list.Add(4);
来源：http://mdd.yanxiufei.cn

[D03] 在指定位置插入元素
来源：http://qzt.xuanzx.com

Py:   arr.insert(0, 0)
来源：http://txr.wangdashe.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://xjp.sweek.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ypx.ehwqpu.com

TS:   arr.splice(0, 0, 0);
来源：http://tku.shangyingyoupin.top

Java: list.add(0, 0);
来源：http://xnf.hongshengwenyu.top

Go:   arr = append([]int{0}, arr...)
来源：http://rwp.fengsongda.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ori.dashuyun.cn

C#:   list.Insert(0, 0);
来源：http://ija.sjlbkw.cn

[D04] 删除元素
来源：http://kfi.hfpthk.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ply.chenlongwang.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wci.ppjwa.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ufn.nanxinkj.top

TS:   arr.splice(0, 1);
来源：http://tyj.tianlin.xyz

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://gvf.cucudq.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://kfx.haohaochexian.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://npv.sufxvd.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://utp.tian-w.cn

[D05] 访问与修改元素
来源：http://bbd.yanxiufei.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://iut.uphjek.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://plr.feifeiyinyue.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://bda.jqgufenzy.top

TS:   arr[0]; arr.at(-1);
来源：http://lve.andypj.xyz

Java: list.get(0); list.set(0, 9);
来源：http://fvs.yj20258888.top

Go:   arr[0]; arr[0] = 9
来源：http://tmw.xuanzx.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://pap.cheryme.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://dku.sufxvd.cn

[D06] 数组长度
来源：http://pgi.xziqi.cn

Py:   len(arr)
来源：http://zye.ppjwa.cn

PHP:  count($arr);
来源：http://cvu.cucudq.cn

JS:   arr.length
来源：http://mqb.ehwqpu.com

TS:   arr.length
来源：http://isj.zhixingplan.top

Java: list.size();
来源：http://cjt.shangyingyoupin.top

Go:   len(arr)
来源：http://cvd.shangyingyoupin.top

Ruby: arr.length; arr.size
来源：http://qhl.pycfn.com

C#:   list.Count;
来源：http://ncr.jinyuanbaomall.cn

[D07] 切片 / 取子数组
来源：http://svp.ctjpmb.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://kbr.tianlin.xyz

PHP:  array_slice($arr, 1, 3);
来源：http://yri.xuetiantiany.cn

JS:   arr.slice(1, 4);
来源：http://xdi.ivvv.top

TS:   arr.slice(1, 4);
来源：http://yzx.jinqigufen.top

Java: list.subList(1, 4);
来源：http://nkc.yuxming.cn

Go:   arr[1:4]
来源：http://xwd.iojbl.cn

Ruby: arr[1, 3]
来源：http://owv.hnxiangtu.top

C#:   list.GetRange(1, 3);
来源：http://uup.guowangkeji.top

[D08] 合并两个数组
来源：http://abh.gotoacloud.top

Py:   a + b;  a.extend(b)
来源：http://dcn.havefunace.top

PHP:  array_merge($a, $b);
来源：http://oyl.cashguo.top

JS:   [...a, ...b];  a.concat(b);
来源：http://zbd.shzxlz.cn

TS:   [...a, ...b];
来源：http://cat.bjfxy.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ogn.snrcjt.cn

Go:   append(a, b...)
来源：http://fpp.jiagoushi.top

Ruby: a + b;  a.concat(b)
来源：http://ajz.jqgufenzy.top

C#:   a.Concat(b).ToList()
来源：http://ctq.vehdjk.com

[D09] 排序（升序）
来源：http://zdw.havefunace.top

Py:   sorted(arr);  arr.sort()
来源：http://trz.zdbjq.cn


<!-- 参考信息 -->