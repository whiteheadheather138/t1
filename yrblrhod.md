代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ybj.sjlbkw.cn

[B10] 遍历同时拿索引
来源：http://ulw.zhixingplan.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ifm.nanxuanxn.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://taf.guannengcc.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ddh.ivvv.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://tto.wangshuangyany.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://tzx.jlsjyb.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://xfo.jianghu66.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://nzo.xingfuxueyuan.xyz

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hdw.xinyue.icu

[B11] 生成数字序列 / 区间
来源：http://kha.guowangkeji.top

Py:   list(range(0, 10, 2))
来源：http://zur.gaohongyu789.top

PHP:  range(0, 10, 2);
来源：http://odi.xylfe.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zkr.c1oappe.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://czx.shanyushiyangkeji.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://xen.zhaomingkeji.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://rnu.jqgufenzy.top

Ruby: (0...10).step(2).to_a
来源：http://lhl.xinyue.icu

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://oun.jyoumei.cn

[B12] 跳出多层循环
来源：http://yjc.yvedp.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://cwt.jiagoushi.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://lws.ehwqpu.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://qki.yonumen.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://xel.tian-w.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://pvd.hnqzz.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://vqx.smart0.xyz

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://pvk.hcnkem.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://tev.jlsjyb.cn

[B13] 判断是否为数字
来源：http://hcj.ydjk.org.cn

Py:   isinstance(x, (int, float))
来源：http://hen.bjfxy.top

PHP:  is_numeric($x)
来源：http://rcf.c1oappe.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://eqv.havefunace.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bek.ehwqpu.com

Java: x instanceof Number
来源：http://zlh.dashuyun.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://qbx.tian-w.cn

Ruby: x.is_a?(Numeric)
来源：http://dll.tanke756.top

C#:   x is int or double or decimal
来源：http://hse.zhoulong.xyz

[B14] 判断值是否在集合内
来源：http://uvd.daxiang520.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://aho.fktsv.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://tyz.jyoumei.cn

JS:   [1, 2, 3].includes(x)
来源：http://icx.havefunace.top

TS:   [1, 2, 3].includes(x)
来源：http://pvu.daria6918.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://jkg.yj20258.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://vlo.xziqi.cn

Ruby: [1, 2, 3].include?(x)
来源：http://lbl.guowangkeji.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ywt.aizwys.cn

[B15] 布尔运算与取反
来源：http://hpg.xinyue.icu

Py:   a and b or not c
来源：http://hrz.cucudq.cn

PHP:  $a && $b || !$c
来源：http://alv.hysaishi.cn

JS:   a && b || !c
来源：http://iff.fzhhl.top

TS:   a && b || !c
来源：http://goe.ydjk.org.cn

Java: a && b || !c
来源：http://iqr.sxryk.cn

Go:   a && b || !c
来源：http://akm.cucudq.cn

Ruby: a && b || !c
来源：http://tmx.zhoulong.xyz

C#:   a && b || !c
来源：http://oah.jiagoushi.top

[B16] 卫语句：不满足条件提前返回
来源：http://bmu.yuanzhike.top

Py:   if not data: return
来源：http://ywc.hysaishi.cn

PHP:  if (!$data) { return; }
来源：http://pfh.daria6918.cn

JS:   if (!data) return;
来源：http://plv.redwolf501.top

TS:   if (!data) return;
来源：http://scw.nwbrower.top

Java: if (data == null) return;
来源：http://bli.jinqigfzy.top

Go:   if data == nil { return }
来源：http://nxc.ppjwa.cn

Ruby: return if data.nil?
来源：http://uqs.ydzc1.top

C#:   if (data == null) return;
来源：http://lej.xuetiantiany.cn

================================================================================
来源：http://kzz.redwolf501.top

C. 函数与作用域
来源：http://eap.hongshengwenyu.top

================================================================================
来源：http://eoy.guannengcc.top

[C01] 定义函数
来源：http://jnp.feifeiyinyue.top

Py:   def add(a, b): return a + b
来源：http://nzz.sysykeji.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://oli.yangfankeji.com

JS:   function add(a, b) { return a + b; }
来源：http://pii.yuxming.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://geo.aibaodan.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://fvd.ybcxt.top

Go:   func add(a, b int) int { return a + b }
来源：http://hjn.fktsv.cn

Ruby: def add(a, b); a + b; end
来源：http://gle.nwbrower.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://dyt.fanxiaobao.xyz

[C02] 默认参数
来源：http://zjw.aizwys.cn

Py:   def greet(name="World"): return name
来源：http://qwa.jinyuanbaomall.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://vuc.zdqjudy.top

JS:   function greet(name = "World") { return name; }
来源：http://evc.yvedp.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://oar.zhijiandao.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://rcy.ywan-chungtsiang.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wiq.zdbjq.cn

Ruby: def greet(name = "World") = name
来源：http://kze.pycfn.com

C#:   string Greet(string name = "World") => name;
来源：http://hcq.daria6918.cn

[C03] 可变参数
来源：http://xti.ehwqpu.com

Py:   def total(*args): return sum(args)
来源：http://mbz.ivvv.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://byk.ydjk.org.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://gyi.yfazqb.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://grq.jyoumei.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://rig.sweek.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wzn.yongpay.top

Ruby: def total(*nums); nums.sum; end
来源：http://lsf.yangfankeji.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mmd.zhaomingkeji.xyz

[C04] 命名参数 / 关键字参数
来源：http://zbc.jinqigufen.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://gfa.daxiang520.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://whu.316326.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://gst.ivvv.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ats.cucudq.cn

Java: // 无：用 Builder 模式或 record
来源：http://hjh.jyoumei.cn

Go:   // 无：用配置结构体参数
来源：http://qjf.c1oappe.top

Ruby: f(a: 1, b: 2)
来源：http://yxz.shuidangran.top

C#:   f(a: 1, b: 2)
来源：http://tjz.yanxiufei.cn

[C05] 返回多个值
来源：http://cvu.ppjwa.cn

Py:   return a, b
来源：http://hbv.dashuyun.cn

PHP:  return [$a, $b];
来源：http://lsd.chenjidiqi.icu

JS:   return [a, b];             // 或 return { a, b };
来源：http://jxk.yangfankeji.com

TS:   return { a, b };
来源：http://kok.nanxuanxn.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://rza.zycfv.cn

Go:   return a, b
来源：http://dcf.jinyuanbaomall.cn

Ruby: return a, b
来源：http://xvq.nwbrower.top

C#:   return (a, b);              // ValueTuple
来源：http://jii.yangfankeji.com

[C06] 匿名函数 / lambda
来源：http://qhe.zhengqikj.top

Py:   square = lambda x: x * x
来源：http://qsd.haohaochexian.top

PHP:  $square = fn($x) => $x * $x;
来源：http://uau.cashguo.top

JS:   const square = x => x * x;
来源：http://vmt.yj20258.top

TS:   const square = (x: number): number => x * x;
来源：http://ava.9152youxi.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mfk.ydzc1.top

Go:   sq := func(x int) int { return x * x }
来源：http://zim.cucudq.cn

Ruby: square = ->(x) { x * x }
来源：http://dxf.fehbvm.com

C#:   Func<int, int> square = x => x * x;
来源：http://hwz.shuidangran.top

[C07] 把函数作为参数传入
来源：http://mew.yangfankeji.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://biz.zhiwuduotai.top

PHP:  array_map("strtoupper", $arr);
来源：http://ach.wangshuangyany.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://exu.guannengcc.top

TS:   arr.map(String)
来源：http://gsb.vehdjk.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://tbi.gotoacloud.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://phn.yfazqb.com

Ruby: arr.map(&:upcase)
来源：http://wlu.wangdashe.top

C#:   arr.Select(s => s.ToUpper())
来源：http://cpk.hammf.cn

[C08] 闭包
来源：http://etm.yvedp.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://nxt.xuetiantiany.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ktl.jinyuanbaomall.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://zln.fzhhl.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://pyj.ydzc1.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://emb.tianlin.xyz

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://bvm.yueranfly.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://prn.zycfv.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://lou.yj20258888.top

[C09] 递归
来源：http://gal.uphjek.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://fsn.snrcjt.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ddq.vqdsnc.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qbu.9152youxi.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jbk.daria6918.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://xlr.shzxlz.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://kmy.jlsjyb.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://awq.andypj.xyz

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ddz.bbcook.cn

[C10] 变量作用域
来源：http://hky.guowangkeji.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://uwz.yj20258888.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://xwd.jlsjyb.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://lvr.wangshuangyany.cn

TS:   同 JS
来源：http://cuw.xingfuxueyuan.xyz

Java: 方法内为块级作用域
来源：http://pkt.sufxvd.cn

Go:   花括号块级作用域
来源：http://jii.yangfankeji.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hpl.fanxiaobao.xyz

C#:   块级作用域
来源：http://rlu.jqgufenzy.top

[C11] 模块导入与导出
来源：http://nqv.andypj.xyz

Py:   from module import func
来源：http://ckt.zhoulong.xyz

PHP:  require "file.php";  或 use App\Service;
来源：http://ihu.fktsv.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://xli.svipenyu.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://pgn.hcnkem.com

Java: import java.util.List;
来源：http://mnz.52xcode.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://dve.nwbrower.top

Ruby: require "json"; require_relative "./util"
来源：http://bpu.zdqjudy.top

C#:   using System.Text;
来源：http://pwv.cqqwz.cn

[C12] 立即执行函数 IIFE
来源：http://qxb.tanke756.top

Py:   (lambda: print("run"))()
来源：http://vpg.quarkkingdee.top

PHP:  (function () { echo "run"; })();
来源：http://cip.jianghu66.top

JS:   (() => { console.log("run"); })();
来源：http://hxg.xinyue.icu

TS:   (() => { console.log("run"); })();
来源：http://nqt.zdqjudy.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://avd.52xcode.cn

Go:   func() { fmt.Println("run") }()
来源：http://bjc.zhiwuduotai.top

Ruby: -> { puts "run" }.call
来源：http://xip.hnqzz.top

C#:   // 无 IIFE：用静态构造函数
来源：http://dsl.jqgfzy.top

[C13] 类型声明 / 类型注解
来源：http://tgf.shanyushiyangkeji.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://qtc.pengpengdd.cyou

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kge.dashuyun.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://iyu.gogol.net.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xqa.iojbl.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ahw.shangyingyoupin.top

Go:   func add(a, b int) int
来源：http://qmz.shanyushiyangtech.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hnp.ppjwa.cn

C#:   int Add(int a, int b) => a + b;
来源：http://sqg.guowangkeji.top

[C14] 泛型函数
来源：http://vti.jinqigfzy.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://lip.jinqigufen.top

PHP:  // 无泛型
来源：http://tnu.guowangkeji.top

JS:   // 无泛型
来源：http://mua.sxryk.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hiq.pycfn.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hix.zhiwuduotai.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://gwu.zhengqikj.top

Ruby: # 无泛型
来源：http://szn.shanyushiyangkeji.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mpx.hysaishi.cn

[C15] 解构 / 展开参数
来源：http://gyi.tanke756.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ggu.hnxiangtu.top

PHP:  [$a, $b] = $pair;
来源：http://jbi.yj202588.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ejg.jyoumei.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wgn.yvedp.cn

Java: // 无解构
来源：http://wrt.dianchejie.cn

Go:   // 无解构
来源：http://upe.jqgfzy.top

Ruby: a, b = pair
来源：http://leh.vehdjk.com

C#:   var (a, b) = pair;
来源：http://drn.ydzc1.top

[C16] 函数 / 方法重载
来源：http://tln.jiagoushi.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://onc.meibo888.top

PHP:  // 无重载
来源：http://wtl.nwbrower.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://iij.tianlin.xyz

TS:   // 用联合类型或重载签名声明
来源：http://ahg.fzhhl.top

Java: void f(int a) {}  void f(String a) {}
来源：http://cvt.tanke756.top

Go:   // 无重载：用不同函数名
来源：http://kmb.tanke756.top

Ruby: # 无重载：靠动态参数
来源：http://wbl.fengsongda.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://win.pengpengdd.cyou

================================================================================
来源：http://ynj.zhiwuduotai.top

D. 数组 / 列表 / 集合
来源：http://ucn.9152youxi.cn

================================================================================
来源：http://ags.jinghuilouyu.cn

[D01] 创建数组 / 列表
来源：http://lgj.feifeiyinyue.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://uer.ehwqpu.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://itp.sxryk.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mth.sweek.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://blp.iojbl.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://flp.fzhhl.top

Go:   arr := []int{1, 2, 3}
来源：http://szi.tian-w.cn

Ruby: arr = [1, 2, 3]
来源：http://rbw.vqdsnc.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://jqv.hesvh.cn

[D02] 追加元素到末尾
来源：http://vhm.hongshengwenyu.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://siw.jlsjyb.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://pkc.jqgfzy.top

JS:   arr.push(4);
来源：http://ayh.zhengqikj.top

TS:   arr.push(4);
来源：http://zzu.cucudq.cn

Java: list.add(4);
来源：http://shn.zycfv.cn

Go:   arr = append(arr, 4)
来源：http://quy.yfazqb.com

Ruby: arr << 4; arr.push(5)
来源：http://qef.uphjek.com

C#:   list.Add(4);
来源：http://jrs.ppjwa.cn

[D03] 在指定位置插入元素
来源：http://xcf.yueranfly.top

Py:   arr.insert(0, 0)
来源：http://lrd.guannengcc.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hoy.dianchejie.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://exw.cashguo.top

TS:   arr.splice(0, 0, 0);
来源：http://thx.guannengcc.top

Java: list.add(0, 0);
来源：http://rpv.bjfxy.top

Go:   arr = append([]int{0}, arr...)
来源：http://gmw.daxiang520.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://obk.fengsongda.top

C#:   list.Insert(0, 0);
来源：http://jbc.gaohongyu789.top

[D04] 删除元素
来源：http://dwm.haohaochexian.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://dcc.yangfankeji.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ogk.jinqigufen.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://rfq.hammf.cn

TS:   arr.splice(0, 1);
来源：http://are.gogol.net.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://dju.fanxiaobao.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://dkn.fanxiaobao.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://skk.meibo888.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://bxb.nwbrower.top

[D05] 访问与修改元素
来源：http://rpl.tarul.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://dpi.hnxiangtu.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://rhh.tian-w.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://euf.bjfxy.top

TS:   arr[0]; arr.at(-1);
来源：http://xhl.yvedp.cn

Java: list.get(0); list.set(0, 9);
来源：http://rwh.cdnleiting.top

Go:   arr[0]; arr[0] = 9
来源：http://ygc.gaohongyu789.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://gjo.gogol.net.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://nks.vehdjk.com

[D06] 数组长度
来源：http://ljh.daria6918.cn

Py:   len(arr)
来源：http://art.hcnkem.com

PHP:  count($arr);
来源：http://fjg.jiagoushi.top

JS:   arr.length
来源：http://txk.shanyushiyangtech.top

TS:   arr.length
来源：http://qgk.xingfuxueyuan.xyz

Java: list.size();
来源：http://zvg.fehbvm.com

Go:   len(arr)
来源：http://ydz.daria6918.cn

Ruby: arr.length; arr.size
来源：http://yev.tarul.cn

C#:   list.Count;
来源：http://bpq.fzhhl.top

[D07] 切片 / 取子数组
来源：http://tad.vqdsnc.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://lqo.smart0.xyz

PHP:  array_slice($arr, 1, 3);
来源：http://zxv.guowangkeji.top

JS:   arr.slice(1, 4);
来源：http://rct.dashuyun.cn

TS:   arr.slice(1, 4);
来源：http://ejx.yonumen.top

Java: list.subList(1, 4);
来源：http://moc.epnwcf.com

Go:   arr[1:4]
来源：http://loa.uphjek.com

Ruby: arr[1, 3]
来源：http://uqx.xylfe.cn

C#:   list.GetRange(1, 3);
来源：http://zts.hnxiangtu.top

[D08] 合并两个数组
来源：http://cki.52xcode.cn

Py:   a + b;  a.extend(b)
来源：http://qkl.wangdashe.top

PHP:  array_merge($a, $b);
来源：http://ohy.cashguo.top

JS:   [...a, ...b];  a.concat(b);
来源：http://ruk.nanxinkj.top

TS:   [...a, ...b];
来源：http://yxw.jqgfzy.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://zjw.fktsv.cn

Go:   append(a, b...)
来源：http://vuz.xingfuxueyuan.xyz

Ruby: a + b;  a.concat(b)
来源：http://nrl.tanke756.top

C#:   a.Concat(b).ToList()
来源：http://wjh.52xcode.cn

[D09] 排序（升序）
来源：http://uny.jinghuilouyu.cn

Py:   sorted(arr);  arr.sort()
来源：http://skx.redwolf501.top

PHP:  sort($arr);
来源：http://jgg.aibaodan.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://kfs.feifeiyinyue.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://cpn.cdnleiting.top

Java: Collections.sort(list);  list.sort(null);
来源：http://wxk.redwolf501.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://pjq.jyoumei.cn

Ruby: arr.sort
来源：http://rtl.ydzc1.top

C#:   list.Sort();
来源：http://nzx.tarul.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://cgp.zdqjudy.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://fyc.hysaishi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vyr.zhoulong.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://nxa.vehdjk.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fln.gogol.net.cn


<!-- 参考信息 -->