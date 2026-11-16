代发 wailian999

[B09] break 与 continue
来源：http://wre.havefunace.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://qwk.tanke756.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://jaa.hfpthk.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tax.xziqi.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://aew.yvedp.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ljf.zhaomingkeji.xyz

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://kep.ywan-chungtsiang.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://jug.cqqwz.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ksb.daxiang520.top

[B10] 遍历同时拿索引
来源：http://ryp.tian-w.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://vin.xuanzx.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://geu.tianlin.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wfk.jinqigufen.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ifp.andypj.xyz

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://sgo.ywan-chungtsiang.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://awt.yj20258.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://oje.hcnkem.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://elc.ydzc1.top

[B11] 生成数字序列 / 区间
来源：http://tan.yuxming.cn

Py:   list(range(0, 10, 2))
来源：http://qiv.yuanzhike.top

PHP:  range(0, 10, 2);
来源：http://kgc.hesvh.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zhp.wangshuangyany.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://puu.cucudq.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://gpc.fanxiaobao.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hpq.fengsongda.top

Ruby: (0...10).step(2).to_a
来源：http://jxy.daxiang520.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://odu.hnxiangtu.top

[B12] 跳出多层循环
来源：http://zxb.xinyue.icu

Py:   # 无标签跳转：抽成函数用 return
来源：http://nem.zhongyouzk.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://bfd.fzhhl.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://onx.jqgufenzy.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://fay.jqgfzy.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://aun.zhaomingkeji.xyz

Go:   # 无标签：用布尔标志或抽成函数
来源：http://rid.yangfankeji.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://seb.xylfe.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://otw.zdqjudy.top

[B13] 判断是否为数字
来源：http://jsc.jiagoushi.top

Py:   isinstance(x, (int, float))
来源：http://zwh.haohaochexian.top

PHP:  is_numeric($x)
来源：http://vxm.zhiwuduotai.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://scb.yvedp.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wcc.gotoacloud.top

Java: x instanceof Number
来源：http://poo.xziqi.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://tuf.hnqzz.top

Ruby: x.is_a?(Numeric)
来源：http://bly.jlsjyb.cn

C#:   x is int or double or decimal
来源：http://qan.gaohongyu789.top

[B14] 判断值是否在集合内
来源：http://gmg.jiagoushi.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://aro.xziqi.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hmj.sjlbkw.cn

JS:   [1, 2, 3].includes(x)
来源：http://mhy.yj20258.top

TS:   [1, 2, 3].includes(x)
来源：http://gwp.daxiang520.top

Java: List.of(1, 2, 3).contains(x)
来源：http://rks.jqgfzy.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://sqr.tarul.cn

Ruby: [1, 2, 3].include?(x)
来源：http://pfd.nanxuanxn.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://rvs.yj20258888.top

[B15] 布尔运算与取反
来源：http://cdj.yueranfly.top

Py:   a and b or not c
来源：http://mmu.bjfxy.top

PHP:  $a && $b || !$c
来源：http://huy.cheryme.top

JS:   a && b || !c
来源：http://zjo.yj20258888.top

TS:   a && b || !c
来源：http://gof.tarul.cn

Java: a && b || !c
来源：http://ami.ybcxt.top

Go:   a && b || !c
来源：http://cdw.nanxuanxn.top

Ruby: a && b || !c
来源：http://ixz.ivvv.top

C#:   a && b || !c
来源：http://ldk.hesvh.cn

[B16] 卫语句：不满足条件提前返回
来源：http://hto.gotoacloud.top

Py:   if not data: return
来源：http://njx.shanyushiyangtech.top

PHP:  if (!$data) { return; }
来源：http://ode.cdnleiting.top

JS:   if (!data) return;
来源：http://ytm.shzxlz.cn

TS:   if (!data) return;
来源：http://log.52xcode.cn

Java: if (data == null) return;
来源：http://sor.chenzaomai.com

Go:   if data == nil { return }
来源：http://mal.cheryme.top

Ruby: return if data.nil?
来源：http://ooo.fzhhl.top

C#:   if (data == null) return;
来源：http://cta.fehbvm.com

================================================================================
来源：http://jht.fktsv.cn

C. 函数与作用域
来源：http://cdl.shzxlz.cn

================================================================================
来源：http://ocb.jqgfzy.top

[C01] 定义函数
来源：http://qpu.yuanzhike.top

Py:   def add(a, b): return a + b
来源：http://lmj.meibo888.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wxf.gotoacloud.top

JS:   function add(a, b) { return a + b; }
来源：http://efr.52xcode.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tie.hesvh.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://zvs.hnxiangtu.top

Go:   func add(a, b int) int { return a + b }
来源：http://mrk.zhijiandao.cn

Ruby: def add(a, b); a + b; end
来源：http://xwd.shangyingyoupin.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://xoj.sxryk.cn

[C02] 默认参数
来源：http://fwr.yj20258.top

Py:   def greet(name="World"): return name
来源：http://vph.wangdashe.top

PHP:  function greet($name = "World") { return $name; }
来源：http://npd.redwolf501.top

JS:   function greet(name = "World") { return name; }
来源：http://hkz.xylfe.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://gfa.wangdashe.top

Java: // 无默认参数：方法重载或 Optional
来源：http://yie.shanyushiyangkeji.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://amu.xuanzx.com

Ruby: def greet(name = "World") = name
来源：http://bwo.shangyingyoupin.top

C#:   string Greet(string name = "World") => name;
来源：http://kmt.shzxlz.cn

[C03] 可变参数
来源：http://ume.redwolf501.top

Py:   def total(*args): return sum(args)
来源：http://akn.havefunace.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://qdg.sxryk.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://uxd.chenlongwang.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://jco.dashuyun.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://eob.shanyushiyangkeji.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://lpe.jinqigufen.top

Ruby: def total(*nums); nums.sum; end
来源：http://tws.vqdsnc.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hma.uphjek.com

[C04] 命名参数 / 关键字参数
来源：http://kgu.zdqjudy.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://upc.fanxiaobao.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ixt.shanyushiyangtech.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ywt.bjfxy.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://jjg.yonumen.top

Java: // 无：用 Builder 模式或 record
来源：http://age.hammf.cn

Go:   // 无：用配置结构体参数
来源：http://cja.pengpengdd.cyou

Ruby: f(a: 1, b: 2)
来源：http://kxc.xylfe.cn

C#:   f(a: 1, b: 2)
来源：http://ufh.vqdsnc.cn

[C05] 返回多个值
来源：http://eos.xylfe.cn

Py:   return a, b
来源：http://ybm.tianlin.xyz

PHP:  return [$a, $b];
来源：http://xrn.ydzc1.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://ros.hnxiangtu.top

TS:   return { a, b };
来源：http://rhc.xylfe.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ojf.fehbvm.com

Go:   return a, b
来源：http://fzi.zhaomingkeji.xyz

Ruby: return a, b
来源：http://osr.aibaodan.cn

C#:   return (a, b);              // ValueTuple
来源：http://fpu.shanyushiyangtech.top

[C06] 匿名函数 / lambda
来源：http://xal.jiagoushi.top

Py:   square = lambda x: x * x
来源：http://sjc.fzhhl.top

PHP:  $square = fn($x) => $x * $x;
来源：http://uxl.aizwys.cn

JS:   const square = x => x * x;
来源：http://fqu.yanxiufei.cn

TS:   const square = (x: number): number => x * x;
来源：http://dir.xingfuxueyuan.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://qwg.yvedp.cn

Go:   sq := func(x int) int { return x * x }
来源：http://rvq.gaohongyu789.top

Ruby: square = ->(x) { x * x }
来源：http://jdv.andypj.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://uyv.hysaishi.cn

[C07] 把函数作为参数传入
来源：http://egd.shanyushiyangtech.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://jry.hcnkem.com

PHP:  array_map("strtoupper", $arr);
来源：http://ljp.ybcxt.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://lkq.xinyue.icu

TS:   arr.map(String)
来源：http://gzg.yonumen.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://sch.jiagoushi.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wxo.zhijiandao.cn

Ruby: arr.map(&:upcase)
来源：http://vxw.havefunace.top

C#:   arr.Select(s => s.ToUpper())
来源：http://mtb.tanke756.top

[C08] 闭包
来源：http://kpa.mhx1999.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://poo.tarul.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://zqg.hywenlv.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vee.cdnleiting.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ygz.jinqigufen.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://bez.zhiwuduotai.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://oyg.wangshuangyany.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wva.dianchejie.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://pjp.cashguo.top

[C09] 递归
来源：http://suw.c1oappe.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://oym.yj20258888.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://cxw.ehwqpu.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://err.kuanghao11.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ifl.52xcode.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://vbo.gaohongyu789.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ebj.chenzaomai.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://vhf.shangyingyoupin.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://cvc.cheryme.top

[C10] 变量作用域
来源：http://onh.c1oappe.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://zqu.shangyingyoupin.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ohc.zhengqikj.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://oii.sweek.top

TS:   同 JS
来源：http://etk.fktsv.cn

Java: 方法内为块级作用域
来源：http://bep.zycfv.cn

Go:   花括号块级作用域
来源：http://qfv.sjlbkw.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://rcc.0kj1m.cn

C#:   块级作用域
来源：http://bwa.zhoulong.xyz

[C11] 模块导入与导出
来源：http://gua.ehwqpu.com

Py:   from module import func
来源：http://aqv.pycfn.com

PHP:  require "file.php";  或 use App\Service;
来源：http://wtj.ywan-chungtsiang.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://nsz.zdbjq.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wbl.jqgfzy.top

Java: import java.util.List;
来源：http://hna.feifeiyinyue.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://dtj.gogol.net.cn

Ruby: require "json"; require_relative "./util"
来源：http://tam.hammf.cn

C#:   using System.Text;
来源：http://nxi.chenjidiqi.icu

[C12] 立即执行函数 IIFE
来源：http://vwt.jinghuilouyu.cn

Py:   (lambda: print("run"))()
来源：http://nru.fanxiaobao.xyz

PHP:  (function () { echo "run"; })();
来源：http://zso.redwolf501.top

JS:   (() => { console.log("run"); })();
来源：http://hot.wangshuangyany.cn

TS:   (() => { console.log("run"); })();
来源：http://brn.snrcjt.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://vrg.jinqigufen.top

Go:   func() { fmt.Println("run") }()
来源：http://umg.pengpengdd.cyou

Ruby: -> { puts "run" }.call
来源：http://zvg.chenjidiqi.icu

C#:   // 无 IIFE：用静态构造函数
来源：http://ecv.sweek.top

[C13] 类型声明 / 类型注解
来源：http://rwo.zdqjudy.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hop.wangdashe.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rry.0kj1m.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://gsx.wangshuangyany.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lcn.ivvv.top

Java: int add(int a, int b) { return a + b; }
来源：http://pbe.ywan-chungtsiang.top

Go:   func add(a, b int) int
来源：http://eke.haohaochexian.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://lxh.jinqigfzy.top

C#:   int Add(int a, int b) => a + b;
来源：http://ckf.yongpay.top

[C14] 泛型函数
来源：http://men.chenjidiqi.icu

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://chs.shangyingyoupin.top

PHP:  // 无泛型
来源：http://uwj.cqqwz.cn

JS:   // 无泛型
来源：http://jnz.yanxiufei.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hrz.hnqzz.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ujb.zhengqikj.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://lwr.yvedp.cn

Ruby: # 无泛型
来源：http://frt.jinqigfzy.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://zwe.redwolf501.top

[C15] 解构 / 展开参数
来源：http://unr.yj20258.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://epy.zdbjq.cn

PHP:  [$a, $b] = $pair;
来源：http://znl.cheryme.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://lku.zycfv.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://jzw.dashuyun.cn

Java: // 无解构
来源：http://zjz.jinyuanbaomall.cn

Go:   // 无解构
来源：http://zya.xingfuxueyuan.xyz

Ruby: a, b = pair
来源：http://cer.yanxiufei.cn

C#:   var (a, b) = pair;
来源：http://zok.zhaomingkeji.xyz

[C16] 函数 / 方法重载
来源：http://tut.yueranfly.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://del.birdmap.top

PHP:  // 无重载
来源：http://tyv.smart0.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://kkj.sufxvd.cn

TS:   // 用联合类型或重载签名声明
来源：http://aoi.wangshuangyany.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://brk.chenlongwang.top

Go:   // 无重载：用不同函数名
来源：http://fdd.yanxiufei.cn

Ruby: # 无重载：靠动态参数
来源：http://ked.ybcxt.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://cbc.bbcook.cn

================================================================================
来源：http://zoe.uphjek.com

D. 数组 / 列表 / 集合
来源：http://hae.yongpay.top

================================================================================
来源：http://iox.guannengcc.top

[D01] 创建数组 / 列表
来源：http://pvq.chenzaomai.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://fkn.daria6918.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ihx.cqqwz.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://psq.jiagoushi.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://rfm.yvedp.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://tim.nanxinkj.top

Go:   arr := []int{1, 2, 3}
来源：http://neo.cucudq.cn

Ruby: arr = [1, 2, 3]
来源：http://aot.nanxuanxn.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://lbk.jqgufenzy.top

[D02] 追加元素到末尾
来源：http://amy.fengsongda.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ghx.fktsv.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ytt.bbcook.cn

JS:   arr.push(4);
来源：http://uju.vqdsnc.cn

TS:   arr.push(4);
来源：http://nro.cqqwz.cn

Java: list.add(4);
来源：http://qyl.ybcxt.top

Go:   arr = append(arr, 4)
来源：http://czr.hesvh.cn

Ruby: arr << 4; arr.push(5)
来源：http://nsp.xingfuxueyuan.xyz

C#:   list.Add(4);
来源：http://aze.yanxiufei.cn

[D03] 在指定位置插入元素
来源：http://nge.tianlin.xyz

Py:   arr.insert(0, 0)
来源：http://tzh.xinyue.icu

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://siu.havefunace.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://nve.52xcode.cn

TS:   arr.splice(0, 0, 0);
来源：http://sel.yuxming.cn

Java: list.add(0, 0);
来源：http://rcp.ivvv.top

Go:   arr = append([]int{0}, arr...)
来源：http://mji.yangfankeji.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://pfj.quarkkingdee.top

C#:   list.Insert(0, 0);
来源：http://acj.sysykeji.top

[D04] 删除元素
来源：http://buf.pycfn.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://bnr.feifeiyinyue.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://pon.yanxiufei.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://jdm.chenlongwang.top

TS:   arr.splice(0, 1);
来源：http://ifj.zhongyouzk.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://fua.xuetiantiany.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://pce.aibaodan.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://qqr.tarul.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://atv.xuanzx.com

[D05] 访问与修改元素
来源：http://suv.daria6918.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wsi.ybcxt.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://vyu.sjlbkw.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://vaz.jlsjyb.cn

TS:   arr[0]; arr.at(-1);
来源：http://wjo.kuanghao11.cn

Java: list.get(0); list.set(0, 9);
来源：http://ecn.sjlbkw.cn

Go:   arr[0]; arr[0] = 9
来源：http://snc.gzhubu.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://gmm.hesvh.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://chu.guowangkeji.top

[D06] 数组长度
来源：http://kpa.tian-w.cn

Py:   len(arr)
来源：http://uyy.vqdsnc.cn

PHP:  count($arr);
来源：http://dpv.hysaishi.cn

JS:   arr.length
来源：http://qnh.ctjpmb.com

TS:   arr.length
来源：http://sys.zdbjq.cn

Java: list.size();
来源：http://hcw.hnxiangtu.top

Go:   len(arr)
来源：http://cys.fanxiaobao.xyz

Ruby: arr.length; arr.size
来源：http://txg.iojbl.cn

C#:   list.Count;
来源：http://dyn.shzxlz.cn

[D07] 切片 / 取子数组
来源：http://kbp.hcnkem.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://iyu.shanyushiyangkeji.top

PHP:  array_slice($arr, 1, 3);
来源：http://ocr.daxiang520.top

JS:   arr.slice(1, 4);
来源：http://jgc.epnwcf.com

TS:   arr.slice(1, 4);
来源：http://blr.hcnkem.com

Java: list.subList(1, 4);
来源：http://ieq.shuidangran.top

Go:   arr[1:4]
来源：http://eyw.xuanzx.com

Ruby: arr[1, 3]
来源：http://tcl.quarkkingdee.top

C#:   list.GetRange(1, 3);
来源：http://ouo.jinqigfzy.top

[D08] 合并两个数组
来源：http://maq.jinqigufen.top

Py:   a + b;  a.extend(b)
来源：http://ldc.cashguo.top

PHP:  array_merge($a, $b);
来源：http://vyf.ydjk.org.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://kdy.gotoacloud.top

TS:   [...a, ...b];
来源：http://jmb.tanke756.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://oeh.jianghu66.top

Go:   append(a, b...)
来源：http://sho.jinyuanbaomall.cn

Ruby: a + b;  a.concat(b)
来源：http://poy.chenlongwang.top

C#:   a.Concat(b).ToList()
来源：http://lxe.sxryk.cn

[D09] 排序（升序）
来源：http://buh.smart0.xyz

Py:   sorted(arr);  arr.sort()
来源：http://ofl.birdmap.top

PHP:  sort($arr);
来源：http://scp.nwbrower.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ece.tian-w.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://egs.jianghu66.top

Java: Collections.sort(list);  list.sort(null);
来源：http://pzq.shuidangran.top


<!-- 参考信息 -->