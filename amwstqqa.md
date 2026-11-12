代发 wailian999

[B09] break 与 continue
来源：http://nyq.sjlbkw.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://qej.shuidangran.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://oey.shanyushiyangtech.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lir.xinyue.icu

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ito.xinyue.icu

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tgc.tianlin.xyz

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://yky.bjfxy.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://bru.havefunace.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fmc.epnwcf.com

[B10] 遍历同时拿索引
来源：http://khx.bjfxy.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://nbl.hammf.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://nyn.sufxvd.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://tlt.gzhubu.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://jnu.52xcode.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wxb.jinqigfzy.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://zho.yj20258.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://dgl.fktsv.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hko.yvedp.cn

[B11] 生成数字序列 / 区间
来源：http://sfl.jiagoushi.top

Py:   list(range(0, 10, 2))
来源：http://wwl.shzxlz.cn

PHP:  range(0, 10, 2);
来源：http://etj.c1oappe.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wqu.fengsongda.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nxt.hammf.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://zhb.daxiang520.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://oth.vehdjk.com

Ruby: (0...10).step(2).to_a
来源：http://bqd.yanxiufei.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://qcf.zhongyouzk.top

[B12] 跳出多层循环
来源：http://kkk.yj202588.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://lml.nwbrower.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://rrk.shuidangran.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mid.yueranfly.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://gba.yj20258.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://xbs.birdmap.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://uqq.feifeiyinyue.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://evu.jqgfzy.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mpc.zhongyouzk.top

[B13] 判断是否为数字
来源：http://igx.zycfv.cn

Py:   isinstance(x, (int, float))
来源：http://owo.jinqigufen.top

PHP:  is_numeric($x)
来源：http://lpd.hysaishi.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fma.aizwys.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hot.dianchejie.cn

Java: x instanceof Number
来源：http://gsl.zhiwuduotai.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://rpi.zhoulong.xyz

Ruby: x.is_a?(Numeric)
来源：http://idj.hfpthk.cn

C#:   x is int or double or decimal
来源：http://cpw.xuanzx.com

[B14] 判断值是否在集合内
来源：http://bfn.jqgufenzy.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://gfc.gaohongyu789.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://epk.haohaochexian.top

JS:   [1, 2, 3].includes(x)
来源：http://buk.bbcook.cn

TS:   [1, 2, 3].includes(x)
来源：http://utf.bjfxy.top

Java: List.of(1, 2, 3).contains(x)
来源：http://fay.hfpthk.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://llz.nwbrower.top

Ruby: [1, 2, 3].include?(x)
来源：http://cri.jyoumei.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://siz.kuanghao11.cn

[B15] 布尔运算与取反
来源：http://zju.daria6918.cn

Py:   a and b or not c
来源：http://pcr.svipenyu.cn

PHP:  $a && $b || !$c
来源：http://typ.cheryme.top

JS:   a && b || !c
来源：http://yjb.fzhhl.top

TS:   a && b || !c
来源：http://ygx.yongpay.top

Java: a && b || !c
来源：http://sng.hywenlv.cn

Go:   a && b || !c
来源：http://rln.sjlbkw.cn

Ruby: a && b || !c
来源：http://trm.hcnkem.com

C#:   a && b || !c
来源：http://wac.fehbvm.com

[B16] 卫语句：不满足条件提前返回
来源：http://hgh.chenlongwang.top

Py:   if not data: return
来源：http://zjr.0kj1m.cn

PHP:  if (!$data) { return; }
来源：http://gmj.aibaodan.cn

JS:   if (!data) return;
来源：http://ycf.yj20258888.top

TS:   if (!data) return;
来源：http://trj.tanke756.top

Java: if (data == null) return;
来源：http://qhv.snrcjt.cn

Go:   if data == nil { return }
来源：http://xmm.xuanzx.com

Ruby: return if data.nil?
来源：http://gpx.tian-w.cn

C#:   if (data == null) return;
来源：http://ooq.zdqjudy.top

================================================================================
来源：http://ovf.sxryk.cn

C. 函数与作用域
来源：http://rmg.jinyuanbaomall.cn

================================================================================
来源：http://mdk.shanyushiyangkeji.top

[C01] 定义函数
来源：http://cnk.yangfankeji.com

Py:   def add(a, b): return a + b
来源：http://hnq.redwolf501.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rkh.snrcjt.cn

JS:   function add(a, b) { return a + b; }
来源：http://plw.yuxming.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jrh.zhengqikj.top

Java: static int add(int a, int b) { return a + b; }
来源：http://nnv.aibaodan.cn

Go:   func add(a, b int) int { return a + b }
来源：http://xlc.ydzc1.top

Ruby: def add(a, b); a + b; end
来源：http://hgj.xingfuxueyuan.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://aeb.ydzc1.top

[C02] 默认参数
来源：http://vbo.hcnkem.com

Py:   def greet(name="World"): return name
来源：http://bdw.guowangkeji.top

PHP:  function greet($name = "World") { return $name; }
来源：http://fij.zdqjudy.top

JS:   function greet(name = "World") { return name; }
来源：http://iak.jlsjyb.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://gyt.yj202588.top

Java: // 无默认参数：方法重载或 Optional
来源：http://kjm.epnwcf.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hca.chenzaomai.com

Ruby: def greet(name = "World") = name
来源：http://nbl.jyoumei.cn

C#:   string Greet(string name = "World") => name;
来源：http://wpd.cashguo.top

[C03] 可变参数
来源：http://txv.shzxlz.cn

Py:   def total(*args): return sum(args)
来源：http://svd.yfazqb.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://lrm.cucudq.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://jep.shzxlz.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://egi.jlsjyb.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://dje.meibo888.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://tfo.xingfuxueyuan.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://spk.zhaomingkeji.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mzq.hongshengwenyu.top

[C04] 命名参数 / 关键字参数
来源：http://nao.tarul.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://qnj.ydjk.org.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://swu.aizwys.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ger.epnwcf.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://imv.iojbl.cn

Java: // 无：用 Builder 模式或 record
来源：http://vup.zhijiandao.cn

Go:   // 无：用配置结构体参数
来源：http://bti.jyoumei.cn

Ruby: f(a: 1, b: 2)
来源：http://hqa.jqgufenzy.top

C#:   f(a: 1, b: 2)
来源：http://qdv.shzxlz.cn

[C05] 返回多个值
来源：http://odn.mhx1999.top

Py:   return a, b
来源：http://cox.ywan-chungtsiang.top

PHP:  return [$a, $b];
来源：http://adn.xinyue.icu

JS:   return [a, b];             // 或 return { a, b };
来源：http://ohu.yj20258.top

TS:   return { a, b };
来源：http://kuy.9152youxi.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://bnw.daria6918.cn

Go:   return a, b
来源：http://zqo.shangyingyoupin.top

Ruby: return a, b
来源：http://lfs.yueranfly.top

C#:   return (a, b);              // ValueTuple
来源：http://lel.yfazqb.com

[C06] 匿名函数 / lambda
来源：http://qjr.tanke756.top

Py:   square = lambda x: x * x
来源：http://kka.andypj.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://qdk.nanxuanxn.top

JS:   const square = x => x * x;
来源：http://gfd.hnxiangtu.top

TS:   const square = (x: number): number => x * x;
来源：http://xct.fktsv.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://kor.dashuyun.cn

Go:   sq := func(x int) int { return x * x }
来源：http://gnf.yj20258.top

Ruby: square = ->(x) { x * x }
来源：http://pfv.jiagoushi.top

C#:   Func<int, int> square = x => x * x;
来源：http://ojp.daxiang520.top

[C07] 把函数作为参数传入
来源：http://ils.shanyushiyangkeji.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://cfv.shangyingyoupin.top

PHP:  array_map("strtoupper", $arr);
来源：http://wsb.redwolf501.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://owh.cashguo.top

TS:   arr.map(String)
来源：http://sly.iojbl.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://tcr.haohaochexian.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wta.feifeiyinyue.top

Ruby: arr.map(&:upcase)
来源：http://dtg.jiagoushi.top

C#:   arr.Select(s => s.ToUpper())
来源：http://fkv.zycfv.cn

[C08] 闭包
来源：http://utc.havefunace.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://vyk.fktsv.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://kds.smart0.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ydn.shangyingyoupin.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://zjp.hongshengwenyu.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://svm.tian-w.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ule.epnwcf.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://qgw.chenjidiqi.icu

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://nay.kuanghao11.cn

[C09] 递归
来源：http://sme.yueranfly.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://coh.shanyushiyangtech.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://scn.cashguo.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sjx.ehwqpu.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vze.jlsjyb.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mdx.tian-w.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://gvu.vqdsnc.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://klk.epnwcf.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://gut.hysaishi.cn

[C10] 变量作用域
来源：http://wdh.zdbjq.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://xdq.sweek.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://kqq.hnxiangtu.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://scv.jinqigfzy.top

TS:   同 JS
来源：http://iqe.xylfe.cn

Java: 方法内为块级作用域
来源：http://xdj.aibaodan.cn

Go:   花括号块级作用域
来源：http://iuu.xuetiantiany.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://sqs.yueranfly.top

C#:   块级作用域
来源：http://qmi.havefunace.top

[C11] 模块导入与导出
来源：http://bvj.zhiwuduotai.top

Py:   from module import func
来源：http://qeb.dianchejie.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ags.kuanghao11.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://vge.chenjidiqi.icu

TS:   export function f(): void {};  import { f } from "./m";
来源：http://oex.yanxiufei.cn

Java: import java.util.List;
来源：http://gri.ctjpmb.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://gvr.bjfxy.top

Ruby: require "json"; require_relative "./util"
来源：http://gci.yj20258.top

C#:   using System.Text;
来源：http://clv.yj20258.top

[C12] 立即执行函数 IIFE
来源：http://lce.yuxming.cn

Py:   (lambda: print("run"))()
来源：http://ljc.iojbl.cn

PHP:  (function () { echo "run"; })();
来源：http://fgs.chenjidiqi.icu

JS:   (() => { console.log("run"); })();
来源：http://oct.tarul.cn

TS:   (() => { console.log("run"); })();
来源：http://mns.zhaomingkeji.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://xrf.yanxiufei.cn

Go:   func() { fmt.Println("run") }()
来源：http://ins.guowangkeji.top

Ruby: -> { puts "run" }.call
来源：http://udy.chenlongwang.top

C#:   // 无 IIFE：用静态构造函数
来源：http://lav.gzhubu.top

[C13] 类型声明 / 类型注解
来源：http://xio.yuxming.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://spr.jinyuanbaomall.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://oay.c1oappe.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://zom.ydjk.org.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jdw.jlsjyb.cn

Java: int add(int a, int b) { return a + b; }
来源：http://wno.chenzaomai.com

Go:   func add(a, b int) int
来源：http://kcb.zycfv.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hty.hysaishi.cn

C#:   int Add(int a, int b) => a + b;
来源：http://tze.redwolf501.top

[C14] 泛型函数
来源：http://cqq.shuidangran.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://rnm.daria6918.cn

PHP:  // 无泛型
来源：http://ofs.ybcxt.top

JS:   // 无泛型
来源：http://hgr.hywenlv.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://nux.hysaishi.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://sss.daria6918.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://emy.yj202588.top

Ruby: # 无泛型
来源：http://mhj.yuxming.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://csb.hfpthk.cn

[C15] 解构 / 展开参数
来源：http://len.smart0.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://nnw.tarul.cn

PHP:  [$a, $b] = $pair;
来源：http://msv.hammf.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://lks.hesvh.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://fjw.zhengqikj.top

Java: // 无解构
来源：http://yyc.hywenlv.cn

Go:   // 无解构
来源：http://etv.daria6918.cn

Ruby: a, b = pair
来源：http://dna.epnwcf.com

C#:   var (a, b) = pair;
来源：http://vmj.jianghu66.top

[C16] 函数 / 方法重载
来源：http://vln.0kj1m.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://zin.yj202588.top

PHP:  // 无重载
来源：http://pcd.ydzc1.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://lho.jinghuilouyu.cn

TS:   // 用联合类型或重载签名声明
来源：http://ult.yongpay.top

Java: void f(int a) {}  void f(String a) {}
来源：http://awo.andypj.xyz

Go:   // 无重载：用不同函数名
来源：http://rmm.pengpengdd.cyou

Ruby: # 无重载：靠动态参数
来源：http://eve.hesvh.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://kqz.jqgufenzy.top

================================================================================
来源：http://gys.nwbrower.top

D. 数组 / 列表 / 集合
来源：http://jml.jqgufenzy.top

================================================================================
来源：http://kmq.gogol.net.cn

[D01] 创建数组 / 列表
来源：http://xys.cashguo.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://nkx.xingfuxueyuan.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://sck.52xcode.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://muz.zhengqikj.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://dsp.yj20258888.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://msl.andypj.xyz

Go:   arr := []int{1, 2, 3}
来源：http://nii.jqgufenzy.top

Ruby: arr = [1, 2, 3]
来源：http://nkw.mhx1999.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://dut.smart0.xyz

[D02] 追加元素到末尾
来源：http://dxw.yueranfly.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://upc.jqgufenzy.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://kxh.nanxinkj.top

JS:   arr.push(4);
来源：http://mhf.zhixingplan.top

TS:   arr.push(4);
来源：http://fde.daxiang520.top

Java: list.add(4);
来源：http://wew.316326.xyz

Go:   arr = append(arr, 4)
来源：http://utv.yuanzhike.top

Ruby: arr << 4; arr.push(5)
来源：http://hyo.jyoumei.cn

C#:   list.Add(4);
来源：http://lov.316326.xyz

[D03] 在指定位置插入元素
来源：http://kqx.pengpengdd.cyou

Py:   arr.insert(0, 0)
来源：http://uky.havefunace.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ams.sysykeji.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://fkx.cheryme.top

TS:   arr.splice(0, 0, 0);
来源：http://ort.cqqwz.cn

Java: list.add(0, 0);
来源：http://teg.yanxiufei.cn

Go:   arr = append([]int{0}, arr...)
来源：http://bpm.shanyushiyangkeji.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://jcq.fanxiaobao.xyz

C#:   list.Insert(0, 0);
来源：http://feh.xingfuxueyuan.xyz

[D04] 删除元素
来源：http://eht.jinqigufen.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://uwj.ppjwa.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://iyx.xziqi.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ffv.shzxlz.cn

TS:   arr.splice(0, 1);
来源：http://khk.yj202588.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://vqz.uphjek.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://kmb.yj20258.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ldj.fehbvm.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://kap.sufxvd.cn

[D05] 访问与修改元素
来源：http://tzj.aizwys.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wyf.9152youxi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://stg.zdbjq.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ziw.zhijiandao.cn

TS:   arr[0]; arr.at(-1);
来源：http://era.tarul.cn

Java: list.get(0); list.set(0, 9);
来源：http://wys.hfpthk.cn

Go:   arr[0]; arr[0] = 9
来源：http://hiv.yj20258.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://uhx.wangshuangyany.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://lry.gogol.net.cn

[D06] 数组长度
来源：http://wnv.ydzc1.top

Py:   len(arr)
来源：http://isi.ywan-chungtsiang.top

PHP:  count($arr);
来源：http://ogb.0kj1m.cn

JS:   arr.length
来源：http://vuv.guowangkeji.top

TS:   arr.length
来源：http://ywt.shanyushiyangkeji.top

Java: list.size();
来源：http://dhb.yueranfly.top

Go:   len(arr)
来源：http://lrw.dianchejie.cn

Ruby: arr.length; arr.size
来源：http://puu.yj20258.top

C#:   list.Count;
来源：http://qhi.yj202588.top

[D07] 切片 / 取子数组
来源：http://myj.zhongyouzk.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://syi.vehdjk.com

PHP:  array_slice($arr, 1, 3);
来源：http://reo.jinyuanbaomall.cn

JS:   arr.slice(1, 4);
来源：http://isy.jlsjyb.cn

TS:   arr.slice(1, 4);
来源：http://ull.shanyushiyangtech.top

Java: list.subList(1, 4);
来源：http://emk.shanyushiyangkeji.top

Go:   arr[1:4]
来源：http://jbl.aizwys.cn

Ruby: arr[1, 3]
来源：http://jku.xuetiantiany.cn

C#:   list.GetRange(1, 3);
来源：http://tgn.chenlongwang.top

[D08] 合并两个数组
来源：http://llp.xylfe.cn

Py:   a + b;  a.extend(b)
来源：http://irr.pengpengdd.cyou

PHP:  array_merge($a, $b);
来源：http://omw.hnqzz.top

JS:   [...a, ...b];  a.concat(b);
来源：http://rac.pengpengdd.cyou

TS:   [...a, ...b];
来源：http://lwt.yj202588.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://nuf.9152youxi.cn

Go:   append(a, b...)
来源：http://yub.yvedp.cn

Ruby: a + b;  a.concat(b)
来源：http://tjs.yonumen.top

C#:   a.Concat(b).ToList()
来源：http://fnq.zdqjudy.top

[D09] 排序（升序）
来源：http://gtt.pengpengdd.cyou

Py:   sorted(arr);  arr.sort()
来源：http://pss.gogol.net.cn

PHP:  sort($arr);
来源：http://rjc.andypj.xyz

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ydc.yuxming.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://pzt.nanxinkj.top

Java: Collections.sort(list);  list.sort(null);
来源：http://pux.tarul.cn


<!-- 参考信息 -->