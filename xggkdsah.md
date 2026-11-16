代发 wailian999

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cbk.ehwqpu.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zkl.daxiang520.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ncf.guannengcc.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://fer.xingfuxueyuan.xyz

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mpb.chenlongwang.top

[B10] 遍历同时拿索引
来源：http://znw.gzhubu.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://rnb.9152youxi.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://rgx.svipenyu.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://nxz.wangshuangyany.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ohd.mhx1999.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://bth.jinyuanbaomall.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://avk.jinqigufen.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://kyl.gzhubu.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://dqh.nanxinkj.top

[B11] 生成数字序列 / 区间
来源：http://whh.uphjek.com

Py:   list(range(0, 10, 2))
来源：http://lfo.jlsjyb.cn

PHP:  range(0, 10, 2);
来源：http://jnk.dianchejie.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wyr.shuidangran.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://iay.guowangkeji.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ise.jinghuilouyu.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://nxs.sysykeji.top

Ruby: (0...10).step(2).to_a
来源：http://hmy.fehbvm.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://yfi.sweek.top

[B12] 跳出多层循环
来源：http://xcn.havefunace.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://ejd.yj20258.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://hcl.hnqzz.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://eic.nanxuanxn.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://sib.zhaomingkeji.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://iay.sweek.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ynp.pengpengdd.cyou

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://fyu.jlsjyb.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://qlg.jinqigfzy.top

[B13] 判断是否为数字
来源：http://jka.daxiang520.top

Py:   isinstance(x, (int, float))
来源：http://wja.xylfe.cn

PHP:  is_numeric($x)
来源：http://tfu.jiagoushi.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nka.xingfuxueyuan.xyz

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://iou.nwbrower.top

Java: x instanceof Number
来源：http://zfj.uphjek.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://vdy.gogol.net.cn

Ruby: x.is_a?(Numeric)
来源：http://ehb.uphjek.com

C#:   x is int or double or decimal
来源：http://qje.yj20258.top

[B14] 判断值是否在集合内
来源：http://lfw.tarul.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jbt.hesvh.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://spf.zhoulong.xyz

JS:   [1, 2, 3].includes(x)
来源：http://atn.daria6918.cn

TS:   [1, 2, 3].includes(x)
来源：http://ijg.shanyushiyangtech.top

Java: List.of(1, 2, 3).contains(x)
来源：http://hgi.jyoumei.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://gjg.guowangkeji.top

Ruby: [1, 2, 3].include?(x)
来源：http://quh.cucudq.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://grr.jqgfzy.top

[B15] 布尔运算与取反
来源：http://ekz.zhongyouzk.top

Py:   a and b or not c
来源：http://ysk.vehdjk.com

PHP:  $a && $b || !$c
来源：http://mvc.shzxlz.cn

JS:   a && b || !c
来源：http://vrv.ybcxt.top

TS:   a && b || !c
来源：http://efn.sjlbkw.cn

Java: a && b || !c
来源：http://vjg.chenlongwang.top

Go:   a && b || !c
来源：http://mlm.fengsongda.top

Ruby: a && b || !c
来源：http://jrh.jqgufenzy.top

C#:   a && b || !c
来源：http://fgj.havefunace.top

[B16] 卫语句：不满足条件提前返回
来源：http://blu.bjfxy.top

Py:   if not data: return
来源：http://seo.yfazqb.com

PHP:  if (!$data) { return; }
来源：http://pme.zhixingplan.top

JS:   if (!data) return;
来源：http://ifh.kuanghao11.cn

TS:   if (!data) return;
来源：http://lee.guannengcc.top

Java: if (data == null) return;
来源：http://fzx.hfpthk.cn

Go:   if data == nil { return }
来源：http://eab.birdmap.top

Ruby: return if data.nil?
来源：http://vzt.ydjk.org.cn

C#:   if (data == null) return;
来源：http://ezb.xuetiantiany.cn

================================================================================
来源：http://oar.zhaomingkeji.xyz

C. 函数与作用域
来源：http://jfc.shangyingyoupin.top

================================================================================
来源：http://udw.epnwcf.com

[C01] 定义函数
来源：http://bnc.zhaomingkeji.xyz

Py:   def add(a, b): return a + b
来源：http://rwc.nanxinkj.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://weh.hfpthk.cn

JS:   function add(a, b) { return a + b; }
来源：http://gsq.birdmap.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tnx.yongpay.top

Java: static int add(int a, int b) { return a + b; }
来源：http://keb.yangfankeji.com

Go:   func add(a, b int) int { return a + b }
来源：http://frz.tian-w.cn

Ruby: def add(a, b); a + b; end
来源：http://owg.haohaochexian.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://lqv.zhijiandao.cn

[C02] 默认参数
来源：http://uhv.ydzc1.top

Py:   def greet(name="World"): return name
来源：http://brt.hcnkem.com

PHP:  function greet($name = "World") { return $name; }
来源：http://uav.ydzc1.top

JS:   function greet(name = "World") { return name; }
来源：http://hmg.ivvv.top

TS:   function greet(name: string = "World") { return name; }
来源：http://awh.zhiwuduotai.top

Java: // 无默认参数：方法重载或 Optional
来源：http://tgw.ppjwa.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wtx.ppjwa.cn

Ruby: def greet(name = "World") = name
来源：http://kdy.jinqigufen.top

C#:   string Greet(string name = "World") => name;
来源：http://zxe.zhijiandao.cn

[C03] 可变参数
来源：http://inm.shzxlz.cn

Py:   def total(*args): return sum(args)
来源：http://cxx.zdbjq.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://fxi.zhijiandao.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://uzn.sysykeji.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ort.bbcook.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://gee.jqgfzy.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://laf.wangshuangyany.cn

Ruby: def total(*nums); nums.sum; end
来源：http://vmf.ydzc1.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wbr.chenjidiqi.icu

[C04] 命名参数 / 关键字参数
来源：http://poc.fktsv.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://uxu.ivvv.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://rvu.ybcxt.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://eng.sufxvd.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://dvv.jinqigfzy.top

Java: // 无：用 Builder 模式或 record
来源：http://vra.zhaomingkeji.xyz

Go:   // 无：用配置结构体参数
来源：http://sbd.jinqigfzy.top

Ruby: f(a: 1, b: 2)
来源：http://wfa.yj20258.top

C#:   f(a: 1, b: 2)
来源：http://rxw.xylfe.cn

[C05] 返回多个值
来源：http://szp.shanyushiyangkeji.top

Py:   return a, b
来源：http://wao.jqgfzy.top

PHP:  return [$a, $b];
来源：http://rgx.hongshengwenyu.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://yyx.cashguo.top

TS:   return { a, b };
来源：http://quk.shangyingyoupin.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://sze.9152youxi.cn

Go:   return a, b
来源：http://czu.shzxlz.cn

Ruby: return a, b
来源：http://apu.0kj1m.cn

C#:   return (a, b);              // ValueTuple
来源：http://poy.9152youxi.cn

[C06] 匿名函数 / lambda
来源：http://dws.xuetiantiany.cn

Py:   square = lambda x: x * x
来源：http://juk.aibaodan.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://bzj.nwbrower.top

JS:   const square = x => x * x;
来源：http://aef.zhijiandao.cn

TS:   const square = (x: number): number => x * x;
来源：http://uty.wangdashe.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://xkm.316326.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://nao.snrcjt.cn

Ruby: square = ->(x) { x * x }
来源：http://sth.aibaodan.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ulx.zdqjudy.top

[C07] 把函数作为参数传入
来源：http://dph.ctjpmb.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://fnu.tanke756.top

PHP:  array_map("strtoupper", $arr);
来源：http://ezt.chenjidiqi.icu

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xlf.9152youxi.cn

TS:   arr.map(String)
来源：http://dzh.ehwqpu.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mrl.hnxiangtu.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://dde.zhengqikj.top

Ruby: arr.map(&:upcase)
来源：http://yiy.yangfankeji.com

C#:   arr.Select(s => s.ToUpper())
来源：http://opy.zhijiandao.cn

[C08] 闭包
来源：http://bza.andypj.xyz

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://krs.jiagoushi.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hvq.yj20258888.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://zxq.ydzc1.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://vid.jqgfzy.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://pdd.birdmap.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://anu.zhoulong.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://lci.yj20258888.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://lgn.hywenlv.cn

[C09] 递归
来源：http://ssa.nwbrower.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://sya.yfazqb.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://fsd.aibaodan.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pnu.52xcode.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mrm.uphjek.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://urv.sweek.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://opj.birdmap.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://iru.yuxming.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mzr.ydjk.org.cn

[C10] 变量作用域
来源：http://hyp.feifeiyinyue.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://cww.ydjk.org.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://dpf.yueranfly.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://cbb.cdnleiting.top

TS:   同 JS
来源：http://iwx.wangdashe.top

Java: 方法内为块级作用域
来源：http://rjx.gzhubu.top

Go:   花括号块级作用域
来源：http://rck.hammf.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://tjy.yongpay.top

C#:   块级作用域
来源：http://jqg.sweek.top

[C11] 模块导入与导出
来源：http://huq.0kj1m.cn

Py:   from module import func
来源：http://ims.quarkkingdee.top

PHP:  require "file.php";  或 use App\Service;
来源：http://cda.gaohongyu789.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://kjg.yangfankeji.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://yef.fanxiaobao.xyz

Java: import java.util.List;
来源：http://dwx.meibo888.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://qbo.zdbjq.cn

Ruby: require "json"; require_relative "./util"
来源：http://aoy.kuanghao11.cn

C#:   using System.Text;
来源：http://jgx.hywenlv.cn

[C12] 立即执行函数 IIFE
来源：http://exw.kuanghao11.cn

Py:   (lambda: print("run"))()
来源：http://rlk.quarkkingdee.top

PHP:  (function () { echo "run"; })();
来源：http://arp.yuanzhike.top

JS:   (() => { console.log("run"); })();
来源：http://ebd.gotoacloud.top

TS:   (() => { console.log("run"); })();
来源：http://hto.zhongyouzk.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://exu.sjlbkw.cn

Go:   func() { fmt.Println("run") }()
来源：http://jhk.shanyushiyangkeji.top

Ruby: -> { puts "run" }.call
来源：http://llh.hcnkem.com

C#:   // 无 IIFE：用静态构造函数
来源：http://chr.zhiwuduotai.top

[C13] 类型声明 / 类型注解
来源：http://ovn.fktsv.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://qml.fehbvm.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ste.ivvv.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://vga.hnqzz.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://odn.ydzc1.top

Java: int add(int a, int b) { return a + b; }
来源：http://bwf.zhengqikj.top

Go:   func add(a, b int) int
来源：http://rec.sjlbkw.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://itd.zhengqikj.top

C#:   int Add(int a, int b) => a + b;
来源：http://fht.epnwcf.com

[C14] 泛型函数
来源：http://hwp.jianghu66.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://rgu.dashuyun.cn

PHP:  // 无泛型
来源：http://izb.yuanzhike.top

JS:   // 无泛型
来源：http://vwg.tianlin.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://oab.jqgfzy.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ebq.havefunace.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://kzn.sjlbkw.cn

Ruby: # 无泛型
来源：http://laa.gotoacloud.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ajw.hfpthk.cn

[C15] 解构 / 展开参数
来源：http://lmr.uphjek.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wzf.cheryme.top

PHP:  [$a, $b] = $pair;
来源：http://tlv.bjfxy.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://oef.bjfxy.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://guj.shanyushiyangtech.top

Java: // 无解构
来源：http://mqo.ivvv.top

Go:   // 无解构
来源：http://iuc.ivvv.top

Ruby: a, b = pair
来源：http://nsq.nwbrower.top

C#:   var (a, b) = pair;
来源：http://hjv.feifeiyinyue.top

[C16] 函数 / 方法重载
来源：http://zkl.dashuyun.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vvm.ppjwa.cn

PHP:  // 无重载
来源：http://xpu.jinqigufen.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://pde.cashguo.top

TS:   // 用联合类型或重载签名声明
来源：http://qrs.sysykeji.top

Java: void f(int a) {}  void f(String a) {}
来源：http://ewi.ctjpmb.com

Go:   // 无重载：用不同函数名
来源：http://dns.snrcjt.cn

Ruby: # 无重载：靠动态参数
来源：http://kzs.52xcode.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://vbf.shangyingyoupin.top

================================================================================
来源：http://mgf.kuanghao11.cn

D. 数组 / 列表 / 集合
来源：http://vnb.cqqwz.cn

================================================================================
来源：http://kqs.zhiwuduotai.top

[D01] 创建数组 / 列表
来源：http://cwr.jqgufenzy.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://pch.zhixingplan.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ruz.hnxiangtu.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://gac.havefunace.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://wbd.zhengqikj.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hir.nanxuanxn.top

Go:   arr := []int{1, 2, 3}
来源：http://dfp.hnqzz.top

Ruby: arr = [1, 2, 3]
来源：http://scl.sweek.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://fsg.jianghu66.top

[D02] 追加元素到末尾
来源：http://rbg.jinyuanbaomall.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://kef.yangfankeji.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://gpj.xylfe.cn

JS:   arr.push(4);
来源：http://viw.aizwys.cn

TS:   arr.push(4);
来源：http://krz.hammf.cn

Java: list.add(4);
来源：http://uiy.9152youxi.cn

Go:   arr = append(arr, 4)
来源：http://xrx.yuanzhike.top

Ruby: arr << 4; arr.push(5)
来源：http://zcv.smart0.xyz

C#:   list.Add(4);
来源：http://bhe.yfazqb.com

[D03] 在指定位置插入元素
来源：http://tsp.guannengcc.top

Py:   arr.insert(0, 0)
来源：http://fsj.gzhubu.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://nmp.gotoacloud.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://awv.bjfxy.top

TS:   arr.splice(0, 0, 0);
来源：http://mve.cqqwz.cn

Java: list.add(0, 0);
来源：http://vao.yfazqb.com

Go:   arr = append([]int{0}, arr...)
来源：http://tqa.fzhhl.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://uru.nanxuanxn.top

C#:   list.Insert(0, 0);
来源：http://jgm.hongshengwenyu.top

[D04] 删除元素
来源：http://tzp.chenzaomai.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://vlr.jlsjyb.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://nui.shanyushiyangtech.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ukb.ivvv.top

TS:   arr.splice(0, 1);
来源：http://vti.ppjwa.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://vif.shanyushiyangtech.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://scz.aizwys.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mub.tian-w.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://tfn.hnxiangtu.top

[D05] 访问与修改元素
来源：http://nuh.ehwqpu.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://pan.pycfn.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://btd.guannengcc.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://nxf.xziqi.cn

TS:   arr[0]; arr.at(-1);
来源：http://tcc.zhoulong.xyz

Java: list.get(0); list.set(0, 9);
来源：http://heq.yonumen.top

Go:   arr[0]; arr[0] = 9
来源：http://skw.tarul.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://uuo.cheryme.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://yfh.316326.xyz

[D06] 数组长度
来源：http://qdv.hywenlv.cn

Py:   len(arr)
来源：http://icw.ivvv.top

PHP:  count($arr);
来源：http://bdr.vehdjk.com

JS:   arr.length
来源：http://njg.birdmap.top

TS:   arr.length
来源：http://nih.jinyuanbaomall.cn

Java: list.size();
来源：http://ofw.guannengcc.top

Go:   len(arr)
来源：http://ruc.cqqwz.cn

Ruby: arr.length; arr.size
来源：http://sgt.wangdashe.top

C#:   list.Count;
来源：http://cpp.hysaishi.cn

[D07] 切片 / 取子数组
来源：http://kvq.epnwcf.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ofr.zhixingplan.top

PHP:  array_slice($arr, 1, 3);
来源：http://grt.wangdashe.top

JS:   arr.slice(1, 4);
来源：http://jig.daria6918.cn

TS:   arr.slice(1, 4);
来源：http://het.jyoumei.cn

Java: list.subList(1, 4);
来源：http://byo.vqdsnc.cn

Go:   arr[1:4]
来源：http://brx.yj20258.top

Ruby: arr[1, 3]
来源：http://lyy.cheryme.top

C#:   list.GetRange(1, 3);
来源：http://hzk.tanke756.top

[D08] 合并两个数组
来源：http://oaq.xuetiantiany.cn

Py:   a + b;  a.extend(b)
来源：http://fpb.nanxuanxn.top

PHP:  array_merge($a, $b);
来源：http://hlx.ppjwa.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://rhw.jinghuilouyu.cn

TS:   [...a, ...b];
来源：http://eun.jiagoushi.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://rnd.yuanzhike.top

Go:   append(a, b...)
来源：http://ujf.yonumen.top

Ruby: a + b;  a.concat(b)
来源：http://bdo.nanxinkj.top

C#:   a.Concat(b).ToList()
来源：http://scu.vqdsnc.cn

[D09] 排序（升序）
来源：http://vyo.chenzaomai.com

Py:   sorted(arr);  arr.sort()
来源：http://weh.uphjek.com

PHP:  sort($arr);
来源：http://ail.hnxiangtu.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ewo.zhiwuduotai.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://elp.jinqigfzy.top

Java: Collections.sort(list);  list.sort(null);
来源：http://jjj.jinghuilouyu.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://rsq.mhx1999.top

Ruby: arr.sort
来源：http://zir.daxiang520.top

C#:   list.Sort();
来源：http://jyd.cqqwz.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://vhx.ydjk.org.cn


<!-- 参考信息 -->