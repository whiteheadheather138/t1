代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jcu.gogol.net.cn

[B10] 遍历同时拿索引
来源：http://gom.yuanzhike.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://pif.feifeiyinyue.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://jqz.quarkkingdee.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wji.birdmap.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://qoo.wangdashe.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hit.zhengqikj.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://tqe.gotoacloud.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://tkn.jqgufenzy.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://cdw.c1oappe.top

[B11] 生成数字序列 / 区间
来源：http://nsg.wangshuangyany.cn

Py:   list(range(0, 10, 2))
来源：http://ein.fktsv.cn

PHP:  range(0, 10, 2);
来源：http://yxq.jinqigufen.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://shb.shangyingyoupin.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jyn.tianlin.xyz

Java: IntStream.range(0, 10).boxed().toList()
来源：http://gvj.bjfxy.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://gjl.tianlin.xyz

Ruby: (0...10).step(2).to_a
来源：http://ast.yuanzhike.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zgq.ehwqpu.com

[B12] 跳出多层循环
来源：http://ait.epnwcf.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://hhd.smart0.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://rda.mhx1999.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://bwu.epnwcf.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://euz.andypj.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://bjf.shangyingyoupin.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mve.c1oappe.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://xnp.shangyingyoupin.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://jct.gotoacloud.top

[B13] 判断是否为数字
来源：http://nou.havefunace.top

Py:   isinstance(x, (int, float))
来源：http://und.shanyushiyangtech.top

PHP:  is_numeric($x)
来源：http://oyy.vqdsnc.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://agc.vqdsnc.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yvj.jinqigfzy.top

Java: x instanceof Number
来源：http://qmh.ppjwa.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://guu.cdnleiting.top

Ruby: x.is_a?(Numeric)
来源：http://tho.gaohongyu789.top

C#:   x is int or double or decimal
来源：http://syn.epnwcf.com

[B14] 判断值是否在集合内
来源：http://ioe.hysaishi.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://zny.zhiwuduotai.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://yvs.feifeiyinyue.top

JS:   [1, 2, 3].includes(x)
来源：http://gqf.yangfankeji.com

TS:   [1, 2, 3].includes(x)
来源：http://xwo.nanxuanxn.top

Java: List.of(1, 2, 3).contains(x)
来源：http://mlj.c1oappe.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://jii.fengsongda.top

Ruby: [1, 2, 3].include?(x)
来源：http://itq.mhx1999.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://dsx.hfpthk.cn

[B15] 布尔运算与取反
来源：http://ocz.svipenyu.cn

Py:   a and b or not c
来源：http://fck.sweek.top

PHP:  $a && $b || !$c
来源：http://zzr.jiagoushi.top

JS:   a && b || !c
来源：http://zpp.hywenlv.cn

TS:   a && b || !c
来源：http://mst.bjfxy.top

Java: a && b || !c
来源：http://abn.ydzc1.top

Go:   a && b || !c
来源：http://sge.xylfe.cn

Ruby: a && b || !c
来源：http://oig.hnqzz.top

C#:   a && b || !c
来源：http://syk.c1oappe.top

[B16] 卫语句：不满足条件提前返回
来源：http://thq.sysykeji.top

Py:   if not data: return
来源：http://gjg.zhoulong.xyz

PHP:  if (!$data) { return; }
来源：http://lkx.yueranfly.top

JS:   if (!data) return;
来源：http://ipi.meibo888.top

TS:   if (!data) return;
来源：http://nlf.yonumen.top

Java: if (data == null) return;
来源：http://moj.zhengqikj.top

Go:   if data == nil { return }
来源：http://fqq.fengsongda.top

Ruby: return if data.nil?
来源：http://ukg.jqgufenzy.top

C#:   if (data == null) return;
来源：http://psz.yonumen.top

================================================================================
来源：http://lww.ivvv.top

C. 函数与作用域
来源：http://alr.andypj.xyz

================================================================================
来源：http://dgt.hfpthk.cn

[C01] 定义函数
来源：http://rox.zhixingplan.top

Py:   def add(a, b): return a + b
来源：http://sgj.zhaomingkeji.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yxv.zhengqikj.top

JS:   function add(a, b) { return a + b; }
来源：http://khr.xuetiantiany.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dsb.nanxuanxn.top

Java: static int add(int a, int b) { return a + b; }
来源：http://wmi.jinqigfzy.top

Go:   func add(a, b int) int { return a + b }
来源：http://ahe.ctjpmb.com

Ruby: def add(a, b); a + b; end
来源：http://syq.ppjwa.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wkm.hnxiangtu.top

[C02] 默认参数
来源：http://jol.daxiang520.top

Py:   def greet(name="World"): return name
来源：http://psb.vehdjk.com

PHP:  function greet($name = "World") { return $name; }
来源：http://wme.daria6918.cn

JS:   function greet(name = "World") { return name; }
来源：http://gjc.ydzc1.top

TS:   function greet(name: string = "World") { return name; }
来源：http://ftt.cashguo.top

Java: // 无默认参数：方法重载或 Optional
来源：http://cxg.hcnkem.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://tgv.yuxming.cn

Ruby: def greet(name = "World") = name
来源：http://hbg.hysaishi.cn

C#:   string Greet(string name = "World") => name;
来源：http://cpd.ywan-chungtsiang.top

[C03] 可变参数
来源：http://olk.sysykeji.top

Py:   def total(*args): return sum(args)
来源：http://xrq.sxryk.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://dfg.aibaodan.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://gvm.hammf.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://cdy.cdnleiting.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://thp.hammf.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ndp.c1oappe.top

Ruby: def total(*nums); nums.sum; end
来源：http://mvv.daria6918.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://xnr.hywenlv.cn

[C04] 命名参数 / 关键字参数
来源：http://xyv.hnqzz.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ziv.zhiwuduotai.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://zik.jinqigufen.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://bvz.cucudq.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://beb.tianlin.xyz

Java: // 无：用 Builder 模式或 record
来源：http://aen.sufxvd.cn

Go:   // 无：用配置结构体参数
来源：http://rug.vehdjk.com

Ruby: f(a: 1, b: 2)
来源：http://hov.dashuyun.cn

C#:   f(a: 1, b: 2)
来源：http://cnq.sweek.top

[C05] 返回多个值
来源：http://efy.hnxiangtu.top

Py:   return a, b
来源：http://fbe.yj20258.top

PHP:  return [$a, $b];
来源：http://mbh.0kj1m.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://uxj.yongpay.top

TS:   return { a, b };
来源：http://lkf.zycfv.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://azf.jlsjyb.cn

Go:   return a, b
来源：http://dgk.yueranfly.top

Ruby: return a, b
来源：http://hba.cashguo.top

C#:   return (a, b);              // ValueTuple
来源：http://rfq.jinqigfzy.top

[C06] 匿名函数 / lambda
来源：http://wcu.gogol.net.cn

Py:   square = lambda x: x * x
来源：http://gja.cdnleiting.top

PHP:  $square = fn($x) => $x * $x;
来源：http://kfa.pengpengdd.cyou

JS:   const square = x => x * x;
来源：http://sgb.zhengqikj.top

TS:   const square = (x: number): number => x * x;
来源：http://wzl.iojbl.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://sdx.dianchejie.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ppe.pycfn.com

Ruby: square = ->(x) { x * x }
来源：http://wqz.pengpengdd.cyou

C#:   Func<int, int> square = x => x * x;
来源：http://bqn.sysykeji.top

[C07] 把函数作为参数传入
来源：http://zza.wangdashe.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ifn.gaohongyu789.top

PHP:  array_map("strtoupper", $arr);
来源：http://hiq.pengpengdd.cyou

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://bth.xuetiantiany.cn

TS:   arr.map(String)
来源：http://zfn.c1oappe.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wyk.ydjk.org.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://nhj.xuetiantiany.cn

Ruby: arr.map(&:upcase)
来源：http://you.hysaishi.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://sjn.wangshuangyany.cn

[C08] 闭包
来源：http://feu.xuanzx.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://kpe.nanxinkj.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://pqt.feifeiyinyue.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mol.9152youxi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://cqv.zhixingplan.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://iew.chenlongwang.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://kor.316326.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://avt.iojbl.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://gmj.sysykeji.top

[C09] 递归
来源：http://cxx.jlsjyb.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://acw.tarul.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://zla.shanyushiyangkeji.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://myf.jqgufenzy.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ujh.gotoacloud.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://nzq.zycfv.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mun.wangdashe.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xfh.uphjek.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://boi.havefunace.top

[C10] 变量作用域
来源：http://lhv.havefunace.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://kxj.guannengcc.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://org.yuxming.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://zor.sysykeji.top

TS:   同 JS
来源：http://qjw.fehbvm.com

Java: 方法内为块级作用域
来源：http://idt.c1oappe.top

Go:   花括号块级作用域
来源：http://uzj.yj202588.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://nca.gaohongyu789.top

C#:   块级作用域
来源：http://krf.shanyushiyangtech.top

[C11] 模块导入与导出
来源：http://tvh.yvedp.cn

Py:   from module import func
来源：http://xlr.yfazqb.com

PHP:  require "file.php";  或 use App\Service;
来源：http://ped.fehbvm.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://udl.mhx1999.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://qwl.iojbl.cn

Java: import java.util.List;
来源：http://qje.cdnleiting.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://uyl.cqqwz.cn

Ruby: require "json"; require_relative "./util"
来源：http://kiw.hfpthk.cn

C#:   using System.Text;
来源：http://hwt.tarul.cn

[C12] 立即执行函数 IIFE
来源：http://law.meibo888.top

Py:   (lambda: print("run"))()
来源：http://yur.yj20258888.top

PHP:  (function () { echo "run"; })();
来源：http://ilb.ydjk.org.cn

JS:   (() => { console.log("run"); })();
来源：http://amj.jyoumei.cn

TS:   (() => { console.log("run"); })();
来源：http://oaj.sxryk.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://cpv.shanyushiyangtech.top

Go:   func() { fmt.Println("run") }()
来源：http://xor.xziqi.cn

Ruby: -> { puts "run" }.call
来源：http://ehz.zdqjudy.top

C#:   // 无 IIFE：用静态构造函数
来源：http://lsd.fengsongda.top

[C13] 类型声明 / 类型注解
来源：http://uqy.hnqzz.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://pbz.cucudq.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://eoi.feifeiyinyue.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://twu.xuetiantiany.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://eca.feifeiyinyue.top

Java: int add(int a, int b) { return a + b; }
来源：http://duq.ppjwa.cn

Go:   func add(a, b int) int
来源：http://rwl.epnwcf.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ksq.jlsjyb.cn

C#:   int Add(int a, int b) => a + b;
来源：http://nkz.fengsongda.top

[C14] 泛型函数
来源：http://wnu.gaohongyu789.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://lez.dashuyun.cn

PHP:  // 无泛型
来源：http://mbw.pengpengdd.cyou

JS:   // 无泛型
来源：http://frr.daria6918.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wbo.meibo888.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://xdq.aibaodan.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://kbj.sxryk.cn

Ruby: # 无泛型
来源：http://bei.yueranfly.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://fkt.52xcode.cn

[C15] 解构 / 展开参数
来源：http://cqn.jinqigfzy.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ixc.0kj1m.cn

PHP:  [$a, $b] = $pair;
来源：http://gxi.yongpay.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://gvb.hcnkem.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ker.gotoacloud.top

Java: // 无解构
来源：http://dgu.shanyushiyangtech.top

Go:   // 无解构
来源：http://mmv.yj20258888.top

Ruby: a, b = pair
来源：http://hsb.hesvh.cn

C#:   var (a, b) = pair;
来源：http://imv.havefunace.top

[C16] 函数 / 方法重载
来源：http://wam.uphjek.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mpb.yangfankeji.com

PHP:  // 无重载
来源：http://rjs.fengsongda.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://quu.shanyushiyangkeji.top

TS:   // 用联合类型或重载签名声明
来源：http://sin.yongpay.top

Java: void f(int a) {}  void f(String a) {}
来源：http://lkr.hammf.cn

Go:   // 无重载：用不同函数名
来源：http://hjb.fktsv.cn

Ruby: # 无重载：靠动态参数
来源：http://dxu.tianlin.xyz

C#:   void F(int a) {}  void F(string a) {}
来源：http://mot.shangyingyoupin.top

================================================================================
来源：http://jnf.daria6918.cn

D. 数组 / 列表 / 集合
来源：http://slf.316326.xyz

================================================================================
来源：http://kmb.yfazqb.com

[D01] 创建数组 / 列表
来源：http://jga.tianlin.xyz

Py:   arr = [1, 2, 3];  empty = []
来源：http://cox.yonumen.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://zjb.sufxvd.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://nmq.birdmap.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://fxq.gzhubu.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://jsv.jyoumei.cn

Go:   arr := []int{1, 2, 3}
来源：http://syf.yonumen.top

Ruby: arr = [1, 2, 3]
来源：http://bbh.shangyingyoupin.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://bpd.jlsjyb.cn

[D02] 追加元素到末尾
来源：http://utu.zycfv.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://nvj.c1oappe.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://xxt.xingfuxueyuan.xyz

JS:   arr.push(4);
来源：http://exc.xuetiantiany.cn

TS:   arr.push(4);
来源：http://nrr.zdqjudy.top

Java: list.add(4);
来源：http://eiv.52xcode.cn

Go:   arr = append(arr, 4)
来源：http://xtu.redwolf501.top

Ruby: arr << 4; arr.push(5)
来源：http://ygd.yfazqb.com

C#:   list.Add(4);
来源：http://hwi.nanxinkj.top

[D03] 在指定位置插入元素
来源：http://xik.fzhhl.top

Py:   arr.insert(0, 0)
来源：http://fqq.yangfankeji.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hni.shzxlz.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://zdk.uphjek.com

TS:   arr.splice(0, 0, 0);
来源：http://znu.xinyue.icu

Java: list.add(0, 0);
来源：http://hgq.nwbrower.top

Go:   arr = append([]int{0}, arr...)
来源：http://sly.chenjidiqi.icu

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://fen.316326.xyz

C#:   list.Insert(0, 0);
来源：http://bfz.daxiang520.top

[D04] 删除元素
来源：http://gti.fengsongda.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://xow.zdbjq.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wck.sweek.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://oqx.c1oappe.top

TS:   arr.splice(0, 1);
来源：http://yzk.tianlin.xyz

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://aat.hysaishi.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://nzr.jinyuanbaomall.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://xsu.hfpthk.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xzb.ppjwa.cn

[D05] 访问与修改元素
来源：http://yub.xuanzx.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://xyf.andypj.xyz

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://fvu.zhongyouzk.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://twb.vqdsnc.cn

TS:   arr[0]; arr.at(-1);
来源：http://edv.dashuyun.cn

Java: list.get(0); list.set(0, 9);
来源：http://azz.sysykeji.top

Go:   arr[0]; arr[0] = 9
来源：http://ync.zhongyouzk.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://pkd.chenlongwang.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://vks.zhoulong.xyz

[D06] 数组长度
来源：http://age.dianchejie.cn

Py:   len(arr)
来源：http://why.shangyingyoupin.top

PHP:  count($arr);
来源：http://vgf.jqgfzy.top

JS:   arr.length
来源：http://xfd.fehbvm.com

TS:   arr.length
来源：http://rku.ydzc1.top

Java: list.size();
来源：http://iyu.fanxiaobao.xyz

Go:   len(arr)
来源：http://zfb.bbcook.cn

Ruby: arr.length; arr.size
来源：http://vtz.meibo888.top

C#:   list.Count;
来源：http://bjz.redwolf501.top

[D07] 切片 / 取子数组
来源：http://lhh.havefunace.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://rho.guowangkeji.top

PHP:  array_slice($arr, 1, 3);
来源：http://fqr.zhoulong.xyz

JS:   arr.slice(1, 4);
来源：http://lnl.yj20258.top

TS:   arr.slice(1, 4);
来源：http://nbk.sxryk.cn

Java: list.subList(1, 4);
来源：http://fqx.316326.xyz

Go:   arr[1:4]
来源：http://jwg.52xcode.cn

Ruby: arr[1, 3]
来源：http://bxl.sysykeji.top

C#:   list.GetRange(1, 3);
来源：http://tth.dashuyun.cn

[D08] 合并两个数组
来源：http://qgv.xuanzx.com

Py:   a + b;  a.extend(b)
来源：http://cqt.yueranfly.top

PHP:  array_merge($a, $b);
来源：http://yvy.yj202588.top

JS:   [...a, ...b];  a.concat(b);
来源：http://veq.havefunace.top

TS:   [...a, ...b];
来源：http://dco.yuanzhike.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://vfx.ehwqpu.com

Go:   append(a, b...)
来源：http://bmn.yj202588.top

Ruby: a + b;  a.concat(b)
来源：http://bfk.ybcxt.top

C#:   a.Concat(b).ToList()
来源：http://pae.shanyushiyangtech.top

[D09] 排序（升序）
来源：http://pye.havefunace.top

Py:   sorted(arr);  arr.sort()
来源：http://ext.hnqzz.top

PHP:  sort($arr);
来源：http://ajh.ydjk.org.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wqk.pycfn.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://hem.hysaishi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://dde.meibo888.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ahz.shanyushiyangtech.top

Ruby: arr.sort
来源：http://hgl.dashuyun.cn

C#:   list.Sort();
来源：http://axl.vqdsnc.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://qrx.guowangkeji.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wkv.nanxuanxn.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://knn.0kj1m.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://lbq.daxiang520.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hwm.ywan-chungtsiang.top


<!-- 参考信息 -->