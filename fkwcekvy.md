代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yfm.chenlongwang.top

[B10] 遍历同时拿索引
来源：http://wpz.guannengcc.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://gac.0kj1m.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://uvq.hfpthk.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://nsu.kuanghao11.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://epk.nwbrower.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://cwf.yuxming.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://cvg.yuanzhike.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://bgv.wangdashe.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://cni.pycfn.com

[B11] 生成数字序列 / 区间
来源：http://cmt.fanxiaobao.xyz

Py:   list(range(0, 10, 2))
来源：http://tfl.sysykeji.top

PHP:  range(0, 10, 2);
来源：http://blu.chenlongwang.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://uml.hammf.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qbz.snrcjt.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://cdy.zhoulong.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://gzs.quarkkingdee.top

Ruby: (0...10).step(2).to_a
来源：http://pny.jyoumei.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://tob.quarkkingdee.top

[B12] 跳出多层循环
来源：http://lff.fengsongda.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://olx.cqqwz.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://qgc.c1oappe.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ibx.vehdjk.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://tnp.tianlin.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://xcr.pengpengdd.cyou

Go:   # 无标签：用布尔标志或抽成函数
来源：http://nbt.316326.xyz

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ctc.yj202588.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://lxp.gogol.net.cn

[B13] 判断是否为数字
来源：http://seh.yuxming.cn

Py:   isinstance(x, (int, float))
来源：http://bof.snrcjt.cn

PHP:  is_numeric($x)
来源：http://zcu.9152youxi.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://emc.hcnkem.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wem.dianchejie.cn

Java: x instanceof Number
来源：http://feu.fehbvm.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://rde.zhoulong.xyz

Ruby: x.is_a?(Numeric)
来源：http://rav.bjfxy.top

C#:   x is int or double or decimal
来源：http://krp.jqgfzy.top

[B14] 判断值是否在集合内
来源：http://kvf.daria6918.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://pxz.hcnkem.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://eah.yanxiufei.cn

JS:   [1, 2, 3].includes(x)
来源：http://nng.yuanzhike.top

TS:   [1, 2, 3].includes(x)
来源：http://una.sxryk.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://qlu.ctjpmb.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://qoj.daxiang520.top

Ruby: [1, 2, 3].include?(x)
来源：http://hjz.ywan-chungtsiang.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://rom.snrcjt.cn

[B15] 布尔运算与取反
来源：http://qex.yongpay.top

Py:   a and b or not c
来源：http://ybg.yfazqb.com

PHP:  $a && $b || !$c
来源：http://heu.316326.xyz

JS:   a && b || !c
来源：http://oeb.hnxiangtu.top

TS:   a && b || !c
来源：http://vxu.zhiwuduotai.top

Java: a && b || !c
来源：http://vfv.guannengcc.top

Go:   a && b || !c
来源：http://pzr.chenzaomai.com

Ruby: a && b || !c
来源：http://fal.gotoacloud.top

C#:   a && b || !c
来源：http://stt.yuxming.cn

[B16] 卫语句：不满足条件提前返回
来源：http://dvt.bjfxy.top

Py:   if not data: return
来源：http://yrd.c1oappe.top

PHP:  if (!$data) { return; }
来源：http://efq.sxryk.cn

JS:   if (!data) return;
来源：http://nwc.xingfuxueyuan.xyz

TS:   if (!data) return;
来源：http://whk.cucudq.cn

Java: if (data == null) return;
来源：http://jih.bjfxy.top

Go:   if data == nil { return }
来源：http://jsd.yanxiufei.cn

Ruby: return if data.nil?
来源：http://jfv.fehbvm.com

C#:   if (data == null) return;
来源：http://yzl.ivvv.top

================================================================================
来源：http://ffj.vqdsnc.cn

C. 函数与作用域
来源：http://ltk.hfpthk.cn

================================================================================
来源：http://eez.guowangkeji.top

[C01] 定义函数
来源：http://gov.daxiang520.top

Py:   def add(a, b): return a + b
来源：http://mel.jinqigufen.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zil.jqgufenzy.top

JS:   function add(a, b) { return a + b; }
来源：http://zas.hfpthk.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://euw.ehwqpu.com

Java: static int add(int a, int b) { return a + b; }
来源：http://giy.dianchejie.cn

Go:   func add(a, b int) int { return a + b }
来源：http://zrb.tianlin.xyz

Ruby: def add(a, b); a + b; end
来源：http://idv.dianchejie.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://udf.jqgfzy.top

[C02] 默认参数
来源：http://vrx.jinqigufen.top

Py:   def greet(name="World"): return name
来源：http://rxo.ctjpmb.com

PHP:  function greet($name = "World") { return $name; }
来源：http://jll.shangyingyoupin.top

JS:   function greet(name = "World") { return name; }
来源：http://pkx.vehdjk.com

TS:   function greet(name: string = "World") { return name; }
来源：http://luh.zhongyouzk.top

Java: // 无默认参数：方法重载或 Optional
来源：http://ipr.xinyue.icu

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://rag.zdqjudy.top

Ruby: def greet(name = "World") = name
来源：http://ulp.ywan-chungtsiang.top

C#:   string Greet(string name = "World") => name;
来源：http://ksh.sxryk.cn

[C03] 可变参数
来源：http://ysc.yonumen.top

Py:   def total(*args): return sum(args)
来源：http://irv.jqgfzy.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://bld.nanxinkj.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://grl.sweek.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://cqt.haohaochexian.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://qsz.iojbl.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://rlu.0kj1m.cn

Ruby: def total(*nums); nums.sum; end
来源：http://kam.hesvh.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://syf.cdnleiting.top

[C04] 命名参数 / 关键字参数
来源：http://hfe.jinqigfzy.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://zmk.zdqjudy.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ixr.quarkkingdee.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://qlp.tian-w.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://jty.hnxiangtu.top

Java: // 无：用 Builder 模式或 record
来源：http://xnr.hysaishi.cn

Go:   // 无：用配置结构体参数
来源：http://ybd.hongshengwenyu.top

Ruby: f(a: 1, b: 2)
来源：http://jdw.tianlin.xyz

C#:   f(a: 1, b: 2)
来源：http://izo.tianlin.xyz

[C05] 返回多个值
来源：http://hsv.ywan-chungtsiang.top

Py:   return a, b
来源：http://fzz.ctjpmb.com

PHP:  return [$a, $b];
来源：http://cct.nwbrower.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://qfy.shzxlz.cn

TS:   return { a, b };
来源：http://gkn.pengpengdd.cyou

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://tat.nwbrower.top

Go:   return a, b
来源：http://cdc.hfpthk.cn

Ruby: return a, b
来源：http://rmb.yj202588.top

C#:   return (a, b);              // ValueTuple
来源：http://ttp.fehbvm.com

[C06] 匿名函数 / lambda
来源：http://frg.sufxvd.cn

Py:   square = lambda x: x * x
来源：http://ild.uphjek.com

PHP:  $square = fn($x) => $x * $x;
来源：http://ixc.hnxiangtu.top

JS:   const square = x => x * x;
来源：http://fox.zhijiandao.cn

TS:   const square = (x: number): number => x * x;
来源：http://zyv.zdbjq.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://snp.gaohongyu789.top

Go:   sq := func(x int) int { return x * x }
来源：http://kwd.jianghu66.top

Ruby: square = ->(x) { x * x }
来源：http://cit.nanxuanxn.top

C#:   Func<int, int> square = x => x * x;
来源：http://dcr.tarul.cn

[C07] 把函数作为参数传入
来源：http://foh.fanxiaobao.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://uax.jqgufenzy.top

PHP:  array_map("strtoupper", $arr);
来源：http://ggt.zhixingplan.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://agy.jinghuilouyu.cn

TS:   arr.map(String)
来源：http://scb.jianghu66.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://fgj.snrcjt.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://bvv.gaohongyu789.top

Ruby: arr.map(&:upcase)
来源：http://bbm.shzxlz.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://tkh.zhaomingkeji.xyz

[C08] 闭包
来源：http://hxd.shangyingyoupin.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://fxh.ctjpmb.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://uas.ybcxt.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://bcz.aibaodan.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://vhb.uphjek.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://xle.yuanzhike.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://lrh.jqgfzy.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://aad.havefunace.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ksq.ivvv.top

[C09] 递归
来源：http://wmj.feifeiyinyue.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ntk.chenjidiqi.icu

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://nkf.guowangkeji.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://okl.hnxiangtu.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://svl.fehbvm.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://uhj.vehdjk.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wcu.cucudq.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://dbt.ydzc1.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://vmv.hongshengwenyu.top

[C10] 变量作用域
来源：http://lai.cdnleiting.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://dip.cashguo.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://qyz.wangshuangyany.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hmr.yongpay.top

TS:   同 JS
来源：http://wnk.jianghu66.top

Java: 方法内为块级作用域
来源：http://zrn.zhixingplan.top

Go:   花括号块级作用域
来源：http://hfx.fktsv.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://acr.gogol.net.cn

C#:   块级作用域
来源：http://mgn.svipenyu.cn

[C11] 模块导入与导出
来源：http://cms.sweek.top

Py:   from module import func
来源：http://ulk.xuetiantiany.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://oyd.havefunace.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://scc.zhengqikj.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ncu.zhaomingkeji.xyz

Java: import java.util.List;
来源：http://ecx.pycfn.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://iuy.zhongyouzk.top

Ruby: require "json"; require_relative "./util"
来源：http://erx.jqgfzy.top

C#:   using System.Text;
来源：http://crf.aibaodan.cn

[C12] 立即执行函数 IIFE
来源：http://dpd.jinyuanbaomall.cn

Py:   (lambda: print("run"))()
来源：http://brv.havefunace.top

PHP:  (function () { echo "run"; })();
来源：http://ezf.zdqjudy.top

JS:   (() => { console.log("run"); })();
来源：http://mhs.tarul.cn

TS:   (() => { console.log("run"); })();
来源：http://brr.svipenyu.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://tjr.yuanzhike.top

Go:   func() { fmt.Println("run") }()
来源：http://kdi.zhijiandao.cn

Ruby: -> { puts "run" }.call
来源：http://ddz.gaohongyu789.top

C#:   // 无 IIFE：用静态构造函数
来源：http://uhq.haohaochexian.top

[C13] 类型声明 / 类型注解
来源：http://bmu.chenzaomai.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://rht.havefunace.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xzu.yangfankeji.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://vxi.zhengqikj.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://uta.pengpengdd.cyou

Java: int add(int a, int b) { return a + b; }
来源：http://kvd.zdqjudy.top

Go:   func add(a, b int) int
来源：http://tda.yvedp.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://dkh.dashuyun.cn

C#:   int Add(int a, int b) => a + b;
来源：http://gzm.chenlongwang.top

[C14] 泛型函数
来源：http://dgd.daxiang520.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zrj.jqgfzy.top

PHP:  // 无泛型
来源：http://cqs.kuanghao11.cn

JS:   // 无泛型
来源：http://vnw.pycfn.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://izw.gaohongyu789.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://loq.pycfn.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ztj.wangdashe.top

Ruby: # 无泛型
来源：http://plu.svipenyu.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://jfd.feifeiyinyue.top

[C15] 解构 / 展开参数
来源：http://umh.birdmap.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://fue.fengsongda.top

PHP:  [$a, $b] = $pair;
来源：http://iub.xziqi.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://yzs.shzxlz.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://xvm.shanyushiyangkeji.top

Java: // 无解构
来源：http://adh.gzhubu.top

Go:   // 无解构
来源：http://gcu.yvedp.cn

Ruby: a, b = pair
来源：http://uis.sjlbkw.cn

C#:   var (a, b) = pair;
来源：http://nfa.hammf.cn

[C16] 函数 / 方法重载
来源：http://knq.c1oappe.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ctr.hfpthk.cn

PHP:  // 无重载
来源：http://kke.ybcxt.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://hvd.xingfuxueyuan.xyz

TS:   // 用联合类型或重载签名声明
来源：http://rui.jinyuanbaomall.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://pzy.cheryme.top

Go:   // 无重载：用不同函数名
来源：http://zci.52xcode.cn

Ruby: # 无重载：靠动态参数
来源：http://tor.dashuyun.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ijh.svipenyu.cn

================================================================================
来源：http://nzs.havefunace.top

D. 数组 / 列表 / 集合
来源：http://iwl.pycfn.com

================================================================================
来源：http://msu.zhaomingkeji.xyz

[D01] 创建数组 / 列表
来源：http://vmr.zhaomingkeji.xyz

Py:   arr = [1, 2, 3];  empty = []
来源：http://kok.jqgufenzy.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://vdq.nanxuanxn.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://nwf.fzhhl.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://jjs.smart0.xyz

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mhb.chenzaomai.com

Go:   arr := []int{1, 2, 3}
来源：http://luh.yonumen.top

Ruby: arr = [1, 2, 3]
来源：http://uzo.yuanzhike.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://yfc.daxiang520.top

[D02] 追加元素到末尾
来源：http://cwe.c1oappe.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://oij.fktsv.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ozo.cdnleiting.top

JS:   arr.push(4);
来源：http://dtc.xingfuxueyuan.xyz

TS:   arr.push(4);
来源：http://nee.xuetiantiany.cn

Java: list.add(4);
来源：http://tye.ehwqpu.com

Go:   arr = append(arr, 4)
来源：http://okw.yvedp.cn

Ruby: arr << 4; arr.push(5)
来源：http://nod.jinghuilouyu.cn

C#:   list.Add(4);
来源：http://xho.birdmap.top

[D03] 在指定位置插入元素
来源：http://nmi.hcnkem.com

Py:   arr.insert(0, 0)
来源：http://pov.sjlbkw.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mpb.wangdashe.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://zfe.yuanzhike.top

TS:   arr.splice(0, 0, 0);
来源：http://ukw.yj202588.top

Java: list.add(0, 0);
来源：http://wce.chenzaomai.com

Go:   arr = append([]int{0}, arr...)
来源：http://dvo.jyoumei.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ieh.xingfuxueyuan.xyz

C#:   list.Insert(0, 0);
来源：http://drm.jinghuilouyu.cn

[D04] 删除元素
来源：http://tdh.ppjwa.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://chp.sjlbkw.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://xnj.haohaochexian.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://eap.zhoulong.xyz

TS:   arr.splice(0, 1);
来源：http://nvm.epnwcf.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://xxs.jinqigufen.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://uek.zhixingplan.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://uyk.wangdashe.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://rlr.zhiwuduotai.top

[D05] 访问与修改元素
来源：http://apc.andypj.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://jvq.guannengcc.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://yzj.zhixingplan.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://dte.pengpengdd.cyou

TS:   arr[0]; arr.at(-1);
来源：http://fkv.jinghuilouyu.cn

Java: list.get(0); list.set(0, 9);
来源：http://xtj.gaohongyu789.top

Go:   arr[0]; arr[0] = 9
来源：http://ddi.yj20258888.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://tca.yj202588.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://lxs.birdmap.top

[D06] 数组长度
来源：http://fjt.havefunace.top

Py:   len(arr)
来源：http://qal.cqqwz.cn

PHP:  count($arr);
来源：http://gbx.9152youxi.cn

JS:   arr.length
来源：http://wap.gotoacloud.top

TS:   arr.length
来源：http://nrp.hysaishi.cn

Java: list.size();
来源：http://ass.daria6918.cn

Go:   len(arr)
来源：http://fye.nwbrower.top

Ruby: arr.length; arr.size
来源：http://sbj.sufxvd.cn

C#:   list.Count;
来源：http://oit.shanyushiyangkeji.top

[D07] 切片 / 取子数组
来源：http://ysy.ppjwa.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://vpj.52xcode.cn

PHP:  array_slice($arr, 1, 3);
来源：http://wje.havefunace.top

JS:   arr.slice(1, 4);
来源：http://bjr.jqgfzy.top

TS:   arr.slice(1, 4);
来源：http://kzc.52xcode.cn

Java: list.subList(1, 4);
来源：http://cnk.vqdsnc.cn

Go:   arr[1:4]
来源：http://gri.zdbjq.cn

Ruby: arr[1, 3]
来源：http://pvs.jqgufenzy.top

C#:   list.GetRange(1, 3);
来源：http://ygw.pycfn.com

[D08] 合并两个数组
来源：http://zts.gzhubu.top

Py:   a + b;  a.extend(b)
来源：http://aio.52xcode.cn

PHP:  array_merge($a, $b);
来源：http://vwu.0kj1m.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://lkr.ywan-chungtsiang.top

TS:   [...a, ...b];
来源：http://crp.pengpengdd.cyou

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://iww.cdnleiting.top

Go:   append(a, b...)
来源：http://zgk.jqgufenzy.top

Ruby: a + b;  a.concat(b)
来源：http://nrq.yj20258.top

C#:   a.Concat(b).ToList()
来源：http://znn.hysaishi.cn

[D09] 排序（升序）
来源：http://ymh.yonumen.top

Py:   sorted(arr);  arr.sort()
来源：http://juk.pycfn.com

PHP:  sort($arr);
来源：http://oyu.gzhubu.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://oxp.zhaomingkeji.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://cza.jinghuilouyu.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://hyx.hnxiangtu.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://soo.daxiang520.top

Ruby: arr.sort
来源：http://bih.hysaishi.cn

C#:   list.Sort();
来源：http://raa.iojbl.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://myq.hywenlv.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://cnt.hcnkem.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mze.xylfe.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://cgw.daxiang520.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://rpj.sysykeji.top


<!-- 参考信息 -->