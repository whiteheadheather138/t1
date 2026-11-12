代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nma.pycfn.com

[B10] 遍历同时拿索引
来源：http://mnk.zhoulong.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://tei.jiagoushi.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ywq.nwbrower.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://qto.ehwqpu.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://jcb.zycfv.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mvd.9152youxi.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wrp.guannengcc.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://gat.dianchejie.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://dks.daria6918.cn

[B11] 生成数字序列 / 区间
来源：http://kqn.zhaomingkeji.xyz

Py:   list(range(0, 10, 2))
来源：http://dzh.jyoumei.cn

PHP:  range(0, 10, 2);
来源：http://lmt.zycfv.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://uqr.xinyue.icu

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kci.birdmap.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://upi.yangfankeji.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://thi.dashuyun.cn

Ruby: (0...10).step(2).to_a
来源：http://jrs.xylfe.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://fhh.fehbvm.com

[B12] 跳出多层循环
来源：http://trp.tianlin.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://zai.epnwcf.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://fqt.jiagoushi.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://rea.cqqwz.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ado.cucudq.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://xxs.fanxiaobao.xyz

Go:   # 无标签：用布尔标志或抽成函数
来源：http://nno.yonumen.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mna.ydzc1.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://xax.uphjek.com

[B13] 判断是否为数字
来源：http://ugt.iojbl.cn

Py:   isinstance(x, (int, float))
来源：http://pvy.zhongyouzk.top

PHP:  is_numeric($x)
来源：http://fni.sweek.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vil.gaohongyu789.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gln.fehbvm.com

Java: x instanceof Number
来源：http://gyr.ppjwa.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://itl.cashguo.top

Ruby: x.is_a?(Numeric)
来源：http://waa.chenzaomai.com

C#:   x is int or double or decimal
来源：http://oft.guowangkeji.top

[B14] 判断值是否在集合内
来源：http://ydc.hnxiangtu.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://dli.smart0.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://orm.fanxiaobao.xyz

JS:   [1, 2, 3].includes(x)
来源：http://isd.daria6918.cn

TS:   [1, 2, 3].includes(x)
来源：http://xmb.andypj.xyz

Java: List.of(1, 2, 3).contains(x)
来源：http://anh.jlsjyb.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://sfa.jlsjyb.cn

Ruby: [1, 2, 3].include?(x)
来源：http://unm.aibaodan.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://xuh.316326.xyz

[B15] 布尔运算与取反
来源：http://jqe.hysaishi.cn

Py:   a and b or not c
来源：http://can.vqdsnc.cn

PHP:  $a && $b || !$c
来源：http://eur.ivvv.top

JS:   a && b || !c
来源：http://xef.cashguo.top

TS:   a && b || !c
来源：http://rjw.wangdashe.top

Java: a && b || !c
来源：http://pww.vehdjk.com

Go:   a && b || !c
来源：http://aka.aizwys.cn

Ruby: a && b || !c
来源：http://pdt.hcnkem.com

C#:   a && b || !c
来源：http://xkj.zhengqikj.top

[B16] 卫语句：不满足条件提前返回
来源：http://mmd.hesvh.cn

Py:   if not data: return
来源：http://lnu.gotoacloud.top

PHP:  if (!$data) { return; }
来源：http://yca.zhongyouzk.top

JS:   if (!data) return;
来源：http://jsj.9152youxi.cn

TS:   if (!data) return;
来源：http://qgf.feifeiyinyue.top

Java: if (data == null) return;
来源：http://fya.ydzc1.top

Go:   if data == nil { return }
来源：http://ykz.fzhhl.top

Ruby: return if data.nil?
来源：http://nho.jinqigfzy.top

C#:   if (data == null) return;
来源：http://glh.snrcjt.cn

================================================================================
来源：http://lxz.dianchejie.cn

C. 函数与作用域
来源：http://cxv.uphjek.com

================================================================================
来源：http://bck.gogol.net.cn

[C01] 定义函数
来源：http://qzh.xuanzx.com

Py:   def add(a, b): return a + b
来源：http://voo.zhixingplan.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://oxp.feifeiyinyue.top

JS:   function add(a, b) { return a + b; }
来源：http://bxx.gzhubu.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mkr.ivvv.top

Java: static int add(int a, int b) { return a + b; }
来源：http://tkb.zhiwuduotai.top

Go:   func add(a, b int) int { return a + b }
来源：http://qzf.fengsongda.top

Ruby: def add(a, b); a + b; end
来源：http://lpk.zhengqikj.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://zim.0kj1m.cn

[C02] 默认参数
来源：http://atd.xuanzx.com

Py:   def greet(name="World"): return name
来源：http://yve.shanyushiyangtech.top

PHP:  function greet($name = "World") { return $name; }
来源：http://glj.tarul.cn

JS:   function greet(name = "World") { return name; }
来源：http://ogl.vehdjk.com

TS:   function greet(name: string = "World") { return name; }
来源：http://okt.ydjk.org.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://etq.jqgufenzy.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ohe.jyoumei.cn

Ruby: def greet(name = "World") = name
来源：http://gpo.havefunace.top

C#:   string Greet(string name = "World") => name;
来源：http://pbf.hcnkem.com

[C03] 可变参数
来源：http://mcg.hywenlv.cn

Py:   def total(*args): return sum(args)
来源：http://pag.havefunace.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://yop.jqgfzy.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://rrq.yj202588.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://adv.zycfv.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ocx.zhijiandao.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://rfe.nanxuanxn.top

Ruby: def total(*nums); nums.sum; end
来源：http://tos.jlsjyb.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://lft.jqgfzy.top

[C04] 命名参数 / 关键字参数
来源：http://vei.yfazqb.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://fgu.hesvh.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://phc.haohaochexian.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://tdc.jqgufenzy.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://axe.yangfankeji.com

Java: // 无：用 Builder 模式或 record
来源：http://whj.xylfe.cn

Go:   // 无：用配置结构体参数
来源：http://jut.yonumen.top

Ruby: f(a: 1, b: 2)
来源：http://iwt.nanxuanxn.top

C#:   f(a: 1, b: 2)
来源：http://hlb.zhijiandao.cn

[C05] 返回多个值
来源：http://qim.aibaodan.cn

Py:   return a, b
来源：http://zqe.feifeiyinyue.top

PHP:  return [$a, $b];
来源：http://vjh.wangdashe.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://tdg.jlsjyb.cn

TS:   return { a, b };
来源：http://yiw.jlsjyb.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ojk.zhaomingkeji.xyz

Go:   return a, b
来源：http://seh.ydjk.org.cn

Ruby: return a, b
来源：http://ogq.cheryme.top

C#:   return (a, b);              // ValueTuple
来源：http://lck.zhoulong.xyz

[C06] 匿名函数 / lambda
来源：http://xhg.birdmap.top

Py:   square = lambda x: x * x
来源：http://ypf.yangfankeji.com

PHP:  $square = fn($x) => $x * $x;
来源：http://mwq.havefunace.top

JS:   const square = x => x * x;
来源：http://ocy.yueranfly.top

TS:   const square = (x: number): number => x * x;
来源：http://fly.fzhhl.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://rti.ybcxt.top

Go:   sq := func(x int) int { return x * x }
来源：http://kms.hfpthk.cn

Ruby: square = ->(x) { x * x }
来源：http://rda.cqqwz.cn

C#:   Func<int, int> square = x => x * x;
来源：http://llg.shangyingyoupin.top

[C07] 把函数作为参数传入
来源：http://uwo.tanke756.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://uqk.aibaodan.cn

PHP:  array_map("strtoupper", $arr);
来源：http://jwx.nwbrower.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://njy.jqgufenzy.top

TS:   arr.map(String)
来源：http://qry.zhongyouzk.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xyv.daria6918.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://lwu.nwbrower.top

Ruby: arr.map(&:upcase)
来源：http://sch.zdbjq.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://jej.iojbl.cn

[C08] 闭包
来源：http://dsz.hnxiangtu.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://xoa.bbcook.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://eye.fanxiaobao.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ujr.jiagoushi.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://uuf.cqqwz.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ymp.fehbvm.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://cft.hesvh.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://uve.yuxming.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://fsx.yj202588.top

[C09] 递归
来源：http://rwf.haohaochexian.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://tfg.ivvv.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://qxh.shanyushiyangtech.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ibr.zhixingplan.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nvx.ywan-chungtsiang.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://qkq.birdmap.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://oqt.sufxvd.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://bzz.jqgfzy.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://awu.yj20258.top

[C10] 变量作用域
来源：http://gaa.jinqigfzy.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mwq.yuxming.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://zxy.yueranfly.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://fck.daria6918.cn

TS:   同 JS
来源：http://xnv.bbcook.cn

Java: 方法内为块级作用域
来源：http://aga.tianlin.xyz

Go:   花括号块级作用域
来源：http://exk.zdqjudy.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://zlx.guannengcc.top

C#:   块级作用域
来源：http://hdd.xziqi.cn

[C11] 模块导入与导出
来源：http://cmt.pengpengdd.cyou

Py:   from module import func
来源：http://gov.yueranfly.top

PHP:  require "file.php";  或 use App\Service;
来源：http://mwb.hysaishi.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ofp.smart0.xyz

TS:   export function f(): void {};  import { f } from "./m";
来源：http://lcd.yfazqb.com

Java: import java.util.List;
来源：http://zer.xuanzx.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://dne.svipenyu.cn

Ruby: require "json"; require_relative "./util"
来源：http://vhn.yj20258888.top

C#:   using System.Text;
来源：http://fos.cqqwz.cn

[C12] 立即执行函数 IIFE
来源：http://gia.zhoulong.xyz

Py:   (lambda: print("run"))()
来源：http://jlo.svipenyu.cn

PHP:  (function () { echo "run"; })();
来源：http://wmt.havefunace.top

JS:   (() => { console.log("run"); })();
来源：http://hbb.sysykeji.top

TS:   (() => { console.log("run"); })();
来源：http://cto.shzxlz.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://kis.vehdjk.com

Go:   func() { fmt.Println("run") }()
来源：http://sdd.zdqjudy.top

Ruby: -> { puts "run" }.call
来源：http://gkp.pengpengdd.cyou

C#:   // 无 IIFE：用静态构造函数
来源：http://cak.fktsv.cn

[C13] 类型声明 / 类型注解
来源：http://bur.9152youxi.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://pns.xinyue.icu

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://csp.bjfxy.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://bpo.yj202588.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qpz.0kj1m.cn

Java: int add(int a, int b) { return a + b; }
来源：http://hrj.xuanzx.com

Go:   func add(a, b int) int
来源：http://fgx.aizwys.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://tif.tianlin.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://rqe.ivvv.top

[C14] 泛型函数
来源：http://nzp.feifeiyinyue.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://agt.yuanzhike.top

PHP:  // 无泛型
来源：http://kna.cucudq.cn

JS:   // 无泛型
来源：http://cdo.ehwqpu.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://edo.sweek.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://isb.jlsjyb.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ajn.fengsongda.top

Ruby: # 无泛型
来源：http://qmv.yuanzhike.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hcl.jlsjyb.cn

[C15] 解构 / 展开参数
来源：http://inu.zhengqikj.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://gfo.yueranfly.top

PHP:  [$a, $b] = $pair;
来源：http://mdz.xuanzx.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ams.epnwcf.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://uqv.wangdashe.top

Java: // 无解构
来源：http://hnh.xziqi.cn

Go:   // 无解构
来源：http://pll.chenjidiqi.icu

Ruby: a, b = pair
来源：http://qtb.zdbjq.cn

C#:   var (a, b) = pair;
来源：http://hrx.xingfuxueyuan.xyz

[C16] 函数 / 方法重载
来源：http://iqg.tarul.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://qim.gaohongyu789.top

PHP:  // 无重载
来源：http://tbu.ehwqpu.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://hge.fehbvm.com

TS:   // 用联合类型或重载签名声明
来源：http://xnl.xingfuxueyuan.xyz

Java: void f(int a) {}  void f(String a) {}
来源：http://tii.vehdjk.com

Go:   // 无重载：用不同函数名
来源：http://nxp.yfazqb.com

Ruby: # 无重载：靠动态参数
来源：http://ocx.xinyue.icu

C#:   void F(int a) {}  void F(string a) {}
来源：http://jte.zdbjq.cn

================================================================================
来源：http://xqa.hammf.cn

D. 数组 / 列表 / 集合
来源：http://xai.fktsv.cn

================================================================================
来源：http://ouz.yanxiufei.cn

[D01] 创建数组 / 列表
来源：http://ujx.gaohongyu789.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://rcj.zhijiandao.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://thm.sysykeji.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://yba.tarul.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://jic.ywan-chungtsiang.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://jqf.yanxiufei.cn

Go:   arr := []int{1, 2, 3}
来源：http://ppb.epnwcf.com

Ruby: arr = [1, 2, 3]
来源：http://dex.gaohongyu789.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://lmj.tarul.cn

[D02] 追加元素到末尾
来源：http://tsw.hywenlv.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://kze.dashuyun.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://oju.shanyushiyangkeji.top

JS:   arr.push(4);
来源：http://mbh.yangfankeji.com

TS:   arr.push(4);
来源：http://aid.yanxiufei.cn

Java: list.add(4);
来源：http://ucc.pengpengdd.cyou

Go:   arr = append(arr, 4)
来源：http://jlw.xylfe.cn

Ruby: arr << 4; arr.push(5)
来源：http://oed.chenjidiqi.icu

C#:   list.Add(4);
来源：http://avv.nwbrower.top

[D03] 在指定位置插入元素
来源：http://gmi.xylfe.cn

Py:   arr.insert(0, 0)
来源：http://xii.epnwcf.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://gux.xziqi.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://bxe.shangyingyoupin.top

TS:   arr.splice(0, 0, 0);
来源：http://bqs.xuetiantiany.cn

Java: list.add(0, 0);
来源：http://mve.jiagoushi.top

Go:   arr = append([]int{0}, arr...)
来源：http://rsf.shangyingyoupin.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://loj.gaohongyu789.top

C#:   list.Insert(0, 0);
来源：http://mqp.zhaomingkeji.xyz

[D04] 删除元素
来源：http://kuq.havefunace.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://lhc.pengpengdd.cyou

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://kte.haohaochexian.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://bny.jyoumei.cn

TS:   arr.splice(0, 1);
来源：http://ixw.bjfxy.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://tmu.xuetiantiany.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://dlh.andypj.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://dkx.yanxiufei.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://vgu.jiagoushi.top

[D05] 访问与修改元素
来源：http://nrm.yangfankeji.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://cki.ctjpmb.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://bok.zhixingplan.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://nub.hfpthk.cn

TS:   arr[0]; arr.at(-1);
来源：http://imn.nwbrower.top

Java: list.get(0); list.set(0, 9);
来源：http://wdi.fktsv.cn

Go:   arr[0]; arr[0] = 9
来源：http://odf.hongshengwenyu.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ukj.yangfankeji.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://lka.zhijiandao.cn

[D06] 数组长度
来源：http://iuq.xuetiantiany.cn

Py:   len(arr)
来源：http://fbm.yuanzhike.top

PHP:  count($arr);
来源：http://tue.jinyuanbaomall.cn

JS:   arr.length
来源：http://swj.ydzc1.top

TS:   arr.length
来源：http://ifv.hesvh.cn

Java: list.size();
来源：http://qxp.jqgufenzy.top

Go:   len(arr)
来源：http://upr.fanxiaobao.xyz

Ruby: arr.length; arr.size
来源：http://scu.guowangkeji.top

C#:   list.Count;
来源：http://hby.xziqi.cn

[D07] 切片 / 取子数组
来源：http://bgk.yfazqb.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://obt.quarkkingdee.top

PHP:  array_slice($arr, 1, 3);
来源：http://aqv.shanyushiyangkeji.top

JS:   arr.slice(1, 4);
来源：http://ced.uphjek.com

TS:   arr.slice(1, 4);
来源：http://zbq.zdbjq.cn

Java: list.subList(1, 4);
来源：http://oxa.yvedp.cn

Go:   arr[1:4]
来源：http://zok.yvedp.cn

Ruby: arr[1, 3]
来源：http://otz.cucudq.cn

C#:   list.GetRange(1, 3);
来源：http://wnp.gaohongyu789.top

[D08] 合并两个数组
来源：http://qzz.chenjidiqi.icu

Py:   a + b;  a.extend(b)
来源：http://kyw.haohaochexian.top

PHP:  array_merge($a, $b);
来源：http://aqc.yuanzhike.top

JS:   [...a, ...b];  a.concat(b);
来源：http://adc.ppjwa.cn

TS:   [...a, ...b];
来源：http://quj.sjlbkw.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://sds.hesvh.cn

Go:   append(a, b...)
来源：http://ory.jqgfzy.top

Ruby: a + b;  a.concat(b)
来源：http://lpr.xinyue.icu

C#:   a.Concat(b).ToList()
来源：http://urq.cucudq.cn

[D09] 排序（升序）
来源：http://hvk.aibaodan.cn

Py:   sorted(arr);  arr.sort()
来源：http://jgb.aizwys.cn

PHP:  sort($arr);
来源：http://mks.fanxiaobao.xyz

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mlj.jiagoushi.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://hqd.kuanghao11.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://mbu.shzxlz.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://kbj.yanxiufei.cn

Ruby: arr.sort
来源：http://qnn.guannengcc.top

C#:   list.Sort();
来源：http://zlz.havefunace.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://flc.yangfankeji.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://neh.zycfv.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wmr.quarkkingdee.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://bon.guannengcc.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://zrj.dianchejie.cn


<!-- 参考信息 -->