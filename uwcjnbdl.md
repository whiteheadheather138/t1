代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zgj.vqdsnc.cn

[B10] 遍历同时拿索引
来源：http://hok.hfpthk.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://twr.bbcook.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://sta.sysykeji.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://zir.havefunace.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://idq.cashguo.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mmr.svipenyu.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://war.vqdsnc.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wei.shuidangran.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://cnn.ehwqpu.com

[B11] 生成数字序列 / 区间
来源：http://atf.zdqjudy.top

Py:   list(range(0, 10, 2))
来源：http://ljz.chenjidiqi.icu

PHP:  range(0, 10, 2);
来源：http://ned.yuanzhike.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vhz.yj202588.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://znr.pengpengdd.cyou

Java: IntStream.range(0, 10).boxed().toList()
来源：http://fwl.cheryme.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://bpm.yj20258.top

Ruby: (0...10).step(2).to_a
来源：http://zih.zhaomingkeji.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hkk.tian-w.cn

[B12] 跳出多层循环
来源：http://fzi.hcnkem.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://wvo.aibaodan.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://iuy.jqgfzy.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://rge.iojbl.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://fix.nanxuanxn.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://gga.sxryk.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://qln.hcnkem.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://jrg.chenjidiqi.icu

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ktf.gotoacloud.top

[B13] 判断是否为数字
来源：http://dqo.tianlin.xyz

Py:   isinstance(x, (int, float))
来源：http://dlc.nwbrower.top

PHP:  is_numeric($x)
来源：http://kvu.xingfuxueyuan.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ikr.meibo888.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wzf.gzhubu.top

Java: x instanceof Number
来源：http://wfz.fengsongda.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://pmx.52xcode.cn

Ruby: x.is_a?(Numeric)
来源：http://zoj.vqdsnc.cn

C#:   x is int or double or decimal
来源：http://mfe.hcnkem.com

[B14] 判断值是否在集合内
来源：http://agl.yangfankeji.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ydw.0kj1m.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ado.ydjk.org.cn

JS:   [1, 2, 3].includes(x)
来源：http://aby.hesvh.cn

TS:   [1, 2, 3].includes(x)
来源：http://syn.nwbrower.top

Java: List.of(1, 2, 3).contains(x)
来源：http://cby.shangyingyoupin.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://lww.yj20258.top

Ruby: [1, 2, 3].include?(x)
来源：http://icn.nanxuanxn.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ncq.vqdsnc.cn

[B15] 布尔运算与取反
来源：http://ffo.xinyue.icu

Py:   a and b or not c
来源：http://vvp.fktsv.cn

PHP:  $a && $b || !$c
来源：http://pwe.ydzc1.top

JS:   a && b || !c
来源：http://cud.gogol.net.cn

TS:   a && b || !c
来源：http://wpn.ivvv.top

Java: a && b || !c
来源：http://sjy.zhoulong.xyz

Go:   a && b || !c
来源：http://iig.dashuyun.cn

Ruby: a && b || !c
来源：http://iaq.meibo888.top

C#:   a && b || !c
来源：http://imm.uphjek.com

[B16] 卫语句：不满足条件提前返回
来源：http://miv.pycfn.com

Py:   if not data: return
来源：http://suu.yangfankeji.com

PHP:  if (!$data) { return; }
来源：http://abl.sweek.top

JS:   if (!data) return;
来源：http://emn.shuidangran.top

TS:   if (!data) return;
来源：http://qmx.gogol.net.cn

Java: if (data == null) return;
来源：http://vgq.gaohongyu789.top

Go:   if data == nil { return }
来源：http://vyn.zhixingplan.top

Ruby: return if data.nil?
来源：http://byt.havefunace.top

C#:   if (data == null) return;
来源：http://cnv.snrcjt.cn

================================================================================
来源：http://zsr.dashuyun.cn

C. 函数与作用域
来源：http://noo.tarul.cn

================================================================================
来源：http://qsb.daxiang520.top

[C01] 定义函数
来源：http://ktf.xinyue.icu

Py:   def add(a, b): return a + b
来源：http://fti.gogol.net.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yso.aibaodan.cn

JS:   function add(a, b) { return a + b; }
来源：http://xxo.daxiang520.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tdq.yuxming.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://nes.hnxiangtu.top

Go:   func add(a, b int) int { return a + b }
来源：http://umf.zhoulong.xyz

Ruby: def add(a, b); a + b; end
来源：http://ifw.52xcode.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://zsc.hywenlv.cn

[C02] 默认参数
来源：http://ncc.haohaochexian.top

Py:   def greet(name="World"): return name
来源：http://shq.shanyushiyangkeji.top

PHP:  function greet($name = "World") { return $name; }
来源：http://ids.52xcode.cn

JS:   function greet(name = "World") { return name; }
来源：http://xed.andypj.xyz

TS:   function greet(name: string = "World") { return name; }
来源：http://bfd.zdbjq.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ovy.gzhubu.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://tcm.zhoulong.xyz

Ruby: def greet(name = "World") = name
来源：http://rri.redwolf501.top

C#:   string Greet(string name = "World") => name;
来源：http://dml.zhoulong.xyz

[C03] 可变参数
来源：http://zzk.quarkkingdee.top

Py:   def total(*args): return sum(args)
来源：http://fab.mhx1999.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://yww.9152youxi.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://sav.chenjidiqi.icu

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://aac.bbcook.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://lqs.zhiwuduotai.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://rmk.sweek.top

Ruby: def total(*nums); nums.sum; end
来源：http://tjw.yongpay.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://len.cqqwz.cn

[C04] 命名参数 / 关键字参数
来源：http://tul.chenzaomai.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://tgs.wangdashe.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://oxg.nwbrower.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://dai.shanyushiyangtech.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xbx.pengpengdd.cyou

Java: // 无：用 Builder 模式或 record
来源：http://ejt.hnqzz.top

Go:   // 无：用配置结构体参数
来源：http://fsu.gaohongyu789.top

Ruby: f(a: 1, b: 2)
来源：http://xuv.redwolf501.top

C#:   f(a: 1, b: 2)
来源：http://wjo.aibaodan.cn

[C05] 返回多个值
来源：http://kja.zdqjudy.top

Py:   return a, b
来源：http://ezz.shzxlz.cn

PHP:  return [$a, $b];
来源：http://ass.zhongyouzk.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://mqz.jqgufenzy.top

TS:   return { a, b };
来源：http://hel.pycfn.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://sre.meibo888.top

Go:   return a, b
来源：http://wwp.iojbl.cn

Ruby: return a, b
来源：http://xss.gotoacloud.top

C#:   return (a, b);              // ValueTuple
来源：http://doz.daxiang520.top

[C06] 匿名函数 / lambda
来源：http://net.xinyue.icu

Py:   square = lambda x: x * x
来源：http://msi.hfpthk.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://lwp.yj20258.top

JS:   const square = x => x * x;
来源：http://con.c1oappe.top

TS:   const square = (x: number): number => x * x;
来源：http://fot.fzhhl.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://pcd.jqgfzy.top

Go:   sq := func(x int) int { return x * x }
来源：http://wqz.yvedp.cn

Ruby: square = ->(x) { x * x }
来源：http://vex.yfazqb.com

C#:   Func<int, int> square = x => x * x;
来源：http://tmn.hesvh.cn

[C07] 把函数作为参数传入
来源：http://kcl.ydzc1.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://gpa.tian-w.cn

PHP:  array_map("strtoupper", $arr);
来源：http://pnn.9152youxi.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://eir.hongshengwenyu.top

TS:   arr.map(String)
来源：http://tlb.daxiang520.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://sdc.yuanzhike.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://xzg.daxiang520.top

Ruby: arr.map(&:upcase)
来源：http://qxx.gotoacloud.top

C#:   arr.Select(s => s.ToUpper())
来源：http://bip.nwbrower.top

[C08] 闭包
来源：http://tng.shangyingyoupin.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://zuz.vqdsnc.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://umf.c1oappe.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://thv.hywenlv.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://nmz.jinqigfzy.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://pil.hcnkem.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://oun.daxiang520.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://piw.shuidangran.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://uqc.ivvv.top

[C09] 递归
来源：http://gez.shzxlz.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qks.smart0.xyz

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://gnh.yuxming.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ccl.gaohongyu789.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uvb.daxiang520.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ymo.hnqzz.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ffz.yj20258.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://fxx.tianlin.xyz

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hag.uphjek.com

[C10] 变量作用域
来源：http://xxu.hongshengwenyu.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://elp.gogol.net.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://vgq.dianchejie.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mij.hammf.cn

TS:   同 JS
来源：http://pil.birdmap.top

Java: 方法内为块级作用域
来源：http://aiw.cheryme.top

Go:   花括号块级作用域
来源：http://bwf.zhiwuduotai.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mif.316326.xyz

C#:   块级作用域
来源：http://jjs.yj202588.top

[C11] 模块导入与导出
来源：http://kot.xziqi.cn

Py:   from module import func
来源：http://lhy.fehbvm.com

PHP:  require "file.php";  或 use App\Service;
来源：http://ohg.zdqjudy.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://vpu.wangdashe.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://bwg.svipenyu.cn

Java: import java.util.List;
来源：http://xsh.pengpengdd.cyou

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ewr.wangshuangyany.cn

Ruby: require "json"; require_relative "./util"
来源：http://vjf.fanxiaobao.xyz

C#:   using System.Text;
来源：http://dzl.yanxiufei.cn

[C12] 立即执行函数 IIFE
来源：http://xfq.redwolf501.top

Py:   (lambda: print("run"))()
来源：http://kgh.wangshuangyany.cn

PHP:  (function () { echo "run"; })();
来源：http://hrm.cucudq.cn

JS:   (() => { console.log("run"); })();
来源：http://erm.ivvv.top

TS:   (() => { console.log("run"); })();
来源：http://zje.quarkkingdee.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mxc.fehbvm.com

Go:   func() { fmt.Println("run") }()
来源：http://ynd.xziqi.cn

Ruby: -> { puts "run" }.call
来源：http://uno.meibo888.top

C#:   // 无 IIFE：用静态构造函数
来源：http://yzk.xinyue.icu

[C13] 类型声明 / 类型注解
来源：http://gsm.zhoulong.xyz

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://yka.yangfankeji.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://byi.zhoulong.xyz

JS:   // 无类型（可用 JSDoc 注释）
来源：http://oxz.sxryk.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qwy.nwbrower.top

Java: int add(int a, int b) { return a + b; }
来源：http://zhs.wangshuangyany.cn

Go:   func add(a, b int) int
来源：http://ubu.pengpengdd.cyou

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://myk.wangdashe.top

C#:   int Add(int a, int b) => a + b;
来源：http://rrh.dianchejie.cn

[C14] 泛型函数
来源：http://noe.yueranfly.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://vxh.sweek.top

PHP:  // 无泛型
来源：http://jhv.yfazqb.com

JS:   // 无泛型
来源：http://rwv.sysykeji.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://kzq.jinyuanbaomall.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://tch.ydjk.org.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://bez.ctjpmb.com

Ruby: # 无泛型
来源：http://qfv.daria6918.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://zpp.hammf.cn

[C15] 解构 / 展开参数
来源：http://pyq.nwbrower.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://jqc.havefunace.top

PHP:  [$a, $b] = $pair;
来源：http://jcf.zhoulong.xyz

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hco.wangdashe.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://icq.dashuyun.cn

Java: // 无解构
来源：http://dvp.aibaodan.cn

Go:   // 无解构
来源：http://fwk.zhaomingkeji.xyz

Ruby: a, b = pair
来源：http://oml.fzhhl.top

C#:   var (a, b) = pair;
来源：http://tdo.andypj.xyz

[C16] 函数 / 方法重载
来源：http://ftr.hnxiangtu.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://nsh.gogol.net.cn

PHP:  // 无重载
来源：http://gxa.yangfankeji.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://tiv.jiagoushi.top

TS:   // 用联合类型或重载签名声明
来源：http://kmb.zdqjudy.top

Java: void f(int a) {}  void f(String a) {}
来源：http://hif.fzhhl.top

Go:   // 无重载：用不同函数名
来源：http://aii.yanxiufei.cn

Ruby: # 无重载：靠动态参数
来源：http://zsc.hcnkem.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://ixl.hfpthk.cn

================================================================================
来源：http://mqd.nanxuanxn.top

D. 数组 / 列表 / 集合
来源：http://cdr.gzhubu.top

================================================================================
来源：http://dhe.vqdsnc.cn

[D01] 创建数组 / 列表
来源：http://fke.xylfe.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://xvz.hnqzz.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://pei.redwolf501.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://dhc.fzhhl.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://xjq.chenjidiqi.icu

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ygb.zhengqikj.top

Go:   arr := []int{1, 2, 3}
来源：http://syt.dianchejie.cn

Ruby: arr = [1, 2, 3]
来源：http://vax.hnxiangtu.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://xpg.jinqigufen.top

[D02] 追加元素到末尾
来源：http://qrk.hesvh.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://fme.guowangkeji.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hfo.redwolf501.top

JS:   arr.push(4);
来源：http://zuh.aibaodan.cn

TS:   arr.push(4);
来源：http://nxf.zhoulong.xyz

Java: list.add(4);
来源：http://tvh.ydzc1.top

Go:   arr = append(arr, 4)
来源：http://gqz.uphjek.com

Ruby: arr << 4; arr.push(5)
来源：http://yxy.jinqigufen.top

C#:   list.Add(4);
来源：http://bzs.0kj1m.cn

[D03] 在指定位置插入元素
来源：http://oll.9152youxi.cn

Py:   arr.insert(0, 0)
来源：http://smq.snrcjt.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://dlp.fktsv.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wdt.pengpengdd.cyou

TS:   arr.splice(0, 0, 0);
来源：http://kzo.hcnkem.com

Java: list.add(0, 0);
来源：http://dlz.kuanghao11.cn

Go:   arr = append([]int{0}, arr...)
来源：http://mxd.nwbrower.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://fnb.meibo888.top

C#:   list.Insert(0, 0);
来源：http://luv.bbcook.cn

[D04] 删除元素
来源：http://unz.kuanghao11.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://xbu.zhongyouzk.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://qdv.nanxuanxn.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://idg.birdmap.top

TS:   arr.splice(0, 1);
来源：http://qkp.ywan-chungtsiang.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://zqs.meibo888.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://vdu.ybcxt.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://cai.hongshengwenyu.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://tpo.epnwcf.com

[D05] 访问与修改元素
来源：http://yjp.gaohongyu789.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://slj.daxiang520.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hil.chenjidiqi.icu

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://bfy.kuanghao11.cn

TS:   arr[0]; arr.at(-1);
来源：http://lrf.zdqjudy.top

Java: list.get(0); list.set(0, 9);
来源：http://wku.yj202588.top

Go:   arr[0]; arr[0] = 9
来源：http://usd.hnxiangtu.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://puh.daria6918.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hjm.hcnkem.com

[D06] 数组长度
来源：http://bnv.52xcode.cn

Py:   len(arr)
来源：http://mqe.hywenlv.cn

PHP:  count($arr);
来源：http://coe.birdmap.top

JS:   arr.length
来源：http://yrq.jlsjyb.cn

TS:   arr.length
来源：http://ozv.jinyuanbaomall.cn

Java: list.size();
来源：http://lti.316326.xyz

Go:   len(arr)
来源：http://lwh.cucudq.cn

Ruby: arr.length; arr.size
来源：http://twv.sysykeji.top

C#:   list.Count;
来源：http://gwl.zhoulong.xyz

[D07] 切片 / 取子数组
来源：http://sel.birdmap.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://jrl.hywenlv.cn

PHP:  array_slice($arr, 1, 3);
来源：http://xtj.hywenlv.cn

JS:   arr.slice(1, 4);
来源：http://bxc.zhaomingkeji.xyz

TS:   arr.slice(1, 4);
来源：http://swp.zdqjudy.top

Java: list.subList(1, 4);
来源：http://blj.tianlin.xyz

Go:   arr[1:4]
来源：http://qnm.dianchejie.cn

Ruby: arr[1, 3]
来源：http://cdo.hammf.cn

C#:   list.GetRange(1, 3);
来源：http://cxo.yj202588.top

[D08] 合并两个数组
来源：http://hkr.gzhubu.top

Py:   a + b;  a.extend(b)
来源：http://hxg.yfazqb.com

PHP:  array_merge($a, $b);
来源：http://uik.tarul.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ayh.cashguo.top

TS:   [...a, ...b];
来源：http://jgh.yvedp.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://kyx.yongpay.top

Go:   append(a, b...)
来源：http://njq.jlsjyb.cn

Ruby: a + b;  a.concat(b)
来源：http://xfa.tarul.cn

C#:   a.Concat(b).ToList()
来源：http://qrt.yj202588.top

[D09] 排序（升序）
来源：http://ktx.cdnleiting.top

Py:   sorted(arr);  arr.sort()
来源：http://skx.nwbrower.top

PHP:  sort($arr);
来源：http://pbn.yongpay.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://awj.feifeiyinyue.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://tbi.daria6918.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://iwg.zhiwuduotai.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://eoz.ydjk.org.cn

Ruby: arr.sort
来源：http://nwg.smart0.xyz

C#:   list.Sort();
来源：http://ufy.chenjidiqi.icu

[D10] 自定义排序（按字段 / 多条件）
来源：http://dnr.feifeiyinyue.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://emm.ydzc1.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ach.fengsongda.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://esi.snrcjt.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://sbm.jyoumei.cn


<!-- 参考信息 -->