代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lmo.mhx1999.top

[B10] 遍历同时拿索引
来源：http://lcf.birdmap.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://tpu.zdqjudy.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://gay.hfpthk.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xkv.ywan-chungtsiang.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://tum.gzhubu.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://osv.jqgufenzy.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://kih.cucudq.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://uvo.hammf.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://tib.smart0.xyz

[B11] 生成数字序列 / 区间
来源：http://whf.birdmap.top

Py:   list(range(0, 10, 2))
来源：http://dqn.uphjek.com

PHP:  range(0, 10, 2);
来源：http://gka.gaohongyu789.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://iwh.zdbjq.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ilq.zhoulong.xyz

Java: IntStream.range(0, 10).boxed().toList()
来源：http://nix.snrcjt.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://lpg.yueranfly.top

Ruby: (0...10).step(2).to_a
来源：http://ogn.vehdjk.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://msd.c1oappe.top

[B12] 跳出多层循环
来源：http://ryy.ppjwa.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://bsp.hnxiangtu.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://gyu.daria6918.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://rom.jiagoushi.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hob.yanxiufei.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hoy.feifeiyinyue.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mht.nanxuanxn.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ciy.yj20258888.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://kiu.jinghuilouyu.cn

[B13] 判断是否为数字
来源：http://fnx.nanxinkj.top

Py:   isinstance(x, (int, float))
来源：http://ndc.zhengqikj.top

PHP:  is_numeric($x)
来源：http://tpf.snrcjt.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vym.yongpay.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bqp.hesvh.cn

Java: x instanceof Number
来源：http://nsm.gogol.net.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://plf.sysykeji.top

Ruby: x.is_a?(Numeric)
来源：http://xdd.andypj.xyz

C#:   x is int or double or decimal
来源：http://yol.fktsv.cn

[B14] 判断值是否在集合内
来源：http://ppn.zhongyouzk.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ike.uphjek.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://abw.svipenyu.cn

JS:   [1, 2, 3].includes(x)
来源：http://oxk.cucudq.cn

TS:   [1, 2, 3].includes(x)
来源：http://zqv.quarkkingdee.top

Java: List.of(1, 2, 3).contains(x)
来源：http://hrw.hammf.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://oiu.tanke756.top

Ruby: [1, 2, 3].include?(x)
来源：http://vwy.jianghu66.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://dgn.zhongyouzk.top

[B15] 布尔运算与取反
来源：http://erb.aizwys.cn

Py:   a and b or not c
来源：http://eov.fanxiaobao.xyz

PHP:  $a && $b || !$c
来源：http://yos.dianchejie.cn

JS:   a && b || !c
来源：http://cbp.cqqwz.cn

TS:   a && b || !c
来源：http://ssw.xingfuxueyuan.xyz

Java: a && b || !c
来源：http://lxk.yj20258.top

Go:   a && b || !c
来源：http://fxl.gaohongyu789.top

Ruby: a && b || !c
来源：http://ojx.uphjek.com

C#:   a && b || !c
来源：http://uch.c1oappe.top

[B16] 卫语句：不满足条件提前返回
来源：http://hln.bbcook.cn

Py:   if not data: return
来源：http://azl.sufxvd.cn

PHP:  if (!$data) { return; }
来源：http://uks.shzxlz.cn

JS:   if (!data) return;
来源：http://kkt.feifeiyinyue.top

TS:   if (!data) return;
来源：http://qlv.yanxiufei.cn

Java: if (data == null) return;
来源：http://bgm.yj202588.top

Go:   if data == nil { return }
来源：http://pmw.jinyuanbaomall.cn

Ruby: return if data.nil?
来源：http://zfw.feifeiyinyue.top

C#:   if (data == null) return;
来源：http://vst.vqdsnc.cn

================================================================================
来源：http://hed.fktsv.cn

C. 函数与作用域
来源：http://paa.shanyushiyangtech.top

================================================================================
来源：http://ukx.chenlongwang.top

[C01] 定义函数
来源：http://egb.ctjpmb.com

Py:   def add(a, b): return a + b
来源：http://lbo.shzxlz.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lrm.aibaodan.cn

JS:   function add(a, b) { return a + b; }
来源：http://byn.kuanghao11.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://odg.sweek.top

Java: static int add(int a, int b) { return a + b; }
来源：http://etj.yanxiufei.cn

Go:   func add(a, b int) int { return a + b }
来源：http://osw.bbcook.cn

Ruby: def add(a, b); a + b; end
来源：http://oel.fanxiaobao.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://asg.jinqigufen.top

[C02] 默认参数
来源：http://gma.yj20258888.top

Py:   def greet(name="World"): return name
来源：http://qxx.jinqigfzy.top

PHP:  function greet($name = "World") { return $name; }
来源：http://ixp.nwbrower.top

JS:   function greet(name = "World") { return name; }
来源：http://jyw.hnqzz.top

TS:   function greet(name: string = "World") { return name; }
来源：http://mqu.gotoacloud.top

Java: // 无默认参数：方法重载或 Optional
来源：http://tjo.shanyushiyangtech.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://vkf.shangyingyoupin.top

Ruby: def greet(name = "World") = name
来源：http://ahr.jlsjyb.cn

C#:   string Greet(string name = "World") => name;
来源：http://rhu.nwbrower.top

[C03] 可变参数
来源：http://lel.meibo888.top

Py:   def total(*args): return sum(args)
来源：http://rxt.gzhubu.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ydv.bbcook.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://yls.9152youxi.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://snr.mhx1999.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://xqd.havefunace.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://bbi.xuanzx.com

Ruby: def total(*nums); nums.sum; end
来源：http://aci.jinghuilouyu.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://vkf.9152youxi.cn

[C04] 命名参数 / 关键字参数
来源：http://gvm.jinghuilouyu.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ear.yuanzhike.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://bac.ehwqpu.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://fbe.ctjpmb.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ifo.yuxming.cn

Java: // 无：用 Builder 模式或 record
来源：http://rld.316326.xyz

Go:   // 无：用配置结构体参数
来源：http://sym.yangfankeji.com

Ruby: f(a: 1, b: 2)
来源：http://ftv.vehdjk.com

C#:   f(a: 1, b: 2)
来源：http://mqf.zhijiandao.cn

[C05] 返回多个值
来源：http://uaz.jlsjyb.cn

Py:   return a, b
来源：http://rrt.cheryme.top

PHP:  return [$a, $b];
来源：http://pkg.andypj.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://ens.hammf.cn

TS:   return { a, b };
来源：http://mcx.vqdsnc.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://glt.hysaishi.cn

Go:   return a, b
来源：http://jrs.xingfuxueyuan.xyz

Ruby: return a, b
来源：http://snw.gzhubu.top

C#:   return (a, b);              // ValueTuple
来源：http://pme.daria6918.cn

[C06] 匿名函数 / lambda
来源：http://evn.yuanzhike.top

Py:   square = lambda x: x * x
来源：http://jam.tian-w.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://spb.xuanzx.com

JS:   const square = x => x * x;
来源：http://pcu.tanke756.top

TS:   const square = (x: number): number => x * x;
来源：http://xmo.yangfankeji.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://bih.hcnkem.com

Go:   sq := func(x int) int { return x * x }
来源：http://fnd.tianlin.xyz

Ruby: square = ->(x) { x * x }
来源：http://zwb.epnwcf.com

C#:   Func<int, int> square = x => x * x;
来源：http://rbt.zhoulong.xyz

[C07] 把函数作为参数传入
来源：http://lou.shanyushiyangkeji.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ytc.shzxlz.cn

PHP:  array_map("strtoupper", $arr);
来源：http://pxb.tianlin.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://zic.daxiang520.top

TS:   arr.map(String)
来源：http://xgl.feifeiyinyue.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hic.hcnkem.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://fbo.yonumen.top

Ruby: arr.map(&:upcase)
来源：http://cdf.yj20258888.top

C#:   arr.Select(s => s.ToUpper())
来源：http://fbr.bbcook.cn

[C08] 闭包
来源：http://bgi.sweek.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://igd.sjlbkw.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://jlx.vqdsnc.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ynj.tanke756.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://shm.fanxiaobao.xyz

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ywb.yj202588.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jer.jyoumei.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ypi.jinqigufen.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://tte.xuanzx.com

[C09] 递归
来源：http://veb.shanyushiyangtech.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://eru.hfpthk.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://rnq.sxryk.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bfw.hesvh.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cdc.52xcode.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://moe.hammf.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://qgw.daxiang520.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://izz.nanxuanxn.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wmc.9152youxi.cn

[C10] 变量作用域
来源：http://emw.shuidangran.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://gbf.yj20258888.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://jaw.jyoumei.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://cgd.shangyingyoupin.top

TS:   同 JS
来源：http://tus.yangfankeji.com

Java: 方法内为块级作用域
来源：http://lca.cashguo.top

Go:   花括号块级作用域
来源：http://idk.redwolf501.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mls.xingfuxueyuan.xyz

C#:   块级作用域
来源：http://fov.aibaodan.cn

[C11] 模块导入与导出
来源：http://sbt.hammf.cn

Py:   from module import func
来源：http://gpb.guowangkeji.top

PHP:  require "file.php";  或 use App\Service;
来源：http://szx.guowangkeji.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://gol.fktsv.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ggk.xuetiantiany.cn

Java: import java.util.List;
来源：http://xmy.haohaochexian.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://cfk.zhiwuduotai.top

Ruby: require "json"; require_relative "./util"
来源：http://gjz.jqgufenzy.top

C#:   using System.Text;
来源：http://nlb.hnxiangtu.top

[C12] 立即执行函数 IIFE
来源：http://hnt.yuanzhike.top

Py:   (lambda: print("run"))()
来源：http://qua.xingfuxueyuan.xyz

PHP:  (function () { echo "run"; })();
来源：http://kli.xziqi.cn

JS:   (() => { console.log("run"); })();
来源：http://ice.sweek.top

TS:   (() => { console.log("run"); })();
来源：http://vil.uphjek.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://igr.vehdjk.com

Go:   func() { fmt.Println("run") }()
来源：http://cgu.ybcxt.top

Ruby: -> { puts "run" }.call
来源：http://ylt.epnwcf.com

C#:   // 无 IIFE：用静态构造函数
来源：http://ryo.nwbrower.top

[C13] 类型声明 / 类型注解
来源：http://soe.nanxinkj.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://pqp.sxryk.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fkn.bjfxy.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ejf.ehwqpu.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ujy.hfpthk.cn

Java: int add(int a, int b) { return a + b; }
来源：http://xbs.gogol.net.cn

Go:   func add(a, b int) int
来源：http://fha.zhongyouzk.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://aou.yangfankeji.com

C#:   int Add(int a, int b) => a + b;
来源：http://crl.mhx1999.top

[C14] 泛型函数
来源：http://jpd.nanxuanxn.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://pnt.ehwqpu.com

PHP:  // 无泛型
来源：http://hzu.guannengcc.top

JS:   // 无泛型
来源：http://msp.mhx1999.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hht.sufxvd.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://etg.sufxvd.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://xyn.quarkkingdee.top

Ruby: # 无泛型
来源：http://cke.pengpengdd.cyou

C#:   static T First<T>(List<T> items) => items[0];
来源：http://zte.zhiwuduotai.top

[C15] 解构 / 展开参数
来源：http://jtd.kuanghao11.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://bry.kuanghao11.cn

PHP:  [$a, $b] = $pair;
来源：http://awg.jqgfzy.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://udq.shuidangran.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://oia.tian-w.cn

Java: // 无解构
来源：http://ngd.fanxiaobao.xyz

Go:   // 无解构
来源：http://vfm.fanxiaobao.xyz

Ruby: a, b = pair
来源：http://ejz.gotoacloud.top

C#:   var (a, b) = pair;
来源：http://jeb.tianlin.xyz

[C16] 函数 / 方法重载
来源：http://kde.shangyingyoupin.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://omw.daria6918.cn

PHP:  // 无重载
来源：http://kmx.tian-w.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://bxq.hnqzz.top

TS:   // 用联合类型或重载签名声明
来源：http://hgl.fktsv.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://bgo.shangyingyoupin.top

Go:   // 无重载：用不同函数名
来源：http://ohv.bbcook.cn

Ruby: # 无重载：靠动态参数
来源：http://lab.hesvh.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://myo.ehwqpu.com

================================================================================
来源：http://yle.tian-w.cn

D. 数组 / 列表 / 集合
来源：http://ljy.bjfxy.top

================================================================================
来源：http://bai.xziqi.cn

[D01] 创建数组 / 列表
来源：http://prm.bbcook.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://cme.aizwys.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ibu.tian-w.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ruq.meibo888.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://vic.xingfuxueyuan.xyz

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://vxm.yangfankeji.com

Go:   arr := []int{1, 2, 3}
来源：http://aea.gotoacloud.top

Ruby: arr = [1, 2, 3]
来源：http://vkq.hfpthk.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://vma.nanxinkj.top

[D02] 追加元素到末尾
来源：http://ccu.redwolf501.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ucc.shanyushiyangkeji.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://cph.yj20258.top

JS:   arr.push(4);
来源：http://oxf.gotoacloud.top

TS:   arr.push(4);
来源：http://ggz.zdqjudy.top

Java: list.add(4);
来源：http://lje.hammf.cn

Go:   arr = append(arr, 4)
来源：http://gjq.hongshengwenyu.top

Ruby: arr << 4; arr.push(5)
来源：http://zek.zhixingplan.top

C#:   list.Add(4);
来源：http://ljg.daria6918.cn

[D03] 在指定位置插入元素
来源：http://oza.tianlin.xyz

Py:   arr.insert(0, 0)
来源：http://qvy.daxiang520.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mwn.jiagoushi.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://jvo.sysykeji.top

TS:   arr.splice(0, 0, 0);
来源：http://mok.sweek.top

Java: list.add(0, 0);
来源：http://soq.yuanzhike.top

Go:   arr = append([]int{0}, arr...)
来源：http://yaw.chenzaomai.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mrz.mhx1999.top

C#:   list.Insert(0, 0);
来源：http://mkp.haohaochexian.top

[D04] 删除元素
来源：http://upe.sysykeji.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://iwe.hfpthk.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://net.zhoulong.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://qcs.uphjek.com

TS:   arr.splice(0, 1);
来源：http://ozn.fanxiaobao.xyz

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://rro.xylfe.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://nwp.jianghu66.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://bks.sysykeji.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mtq.tarul.cn

[D05] 访问与修改元素
来源：http://hes.svipenyu.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://neg.hywenlv.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://woe.xinyue.icu

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blr.9152youxi.cn

TS:   arr[0]; arr.at(-1);
来源：http://oql.zdbjq.cn

Java: list.get(0); list.set(0, 9);
来源：http://dor.ehwqpu.com

Go:   arr[0]; arr[0] = 9
来源：http://uyc.0kj1m.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://lwa.jiagoushi.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://csr.shangyingyoupin.top

[D06] 数组长度
来源：http://bch.feifeiyinyue.top

Py:   len(arr)
来源：http://txk.ppjwa.cn

PHP:  count($arr);
来源：http://erx.hongshengwenyu.top

JS:   arr.length
来源：http://djl.hesvh.cn

TS:   arr.length
来源：http://qut.jlsjyb.cn

Java: list.size();
来源：http://seg.hywenlv.cn

Go:   len(arr)
来源：http://znr.zycfv.cn

Ruby: arr.length; arr.size
来源：http://tfr.snrcjt.cn

C#:   list.Count;
来源：http://jxx.nanxinkj.top

[D07] 切片 / 取子数组
来源：http://jtw.iojbl.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://cra.hnqzz.top

PHP:  array_slice($arr, 1, 3);
来源：http://lmb.zdbjq.cn

JS:   arr.slice(1, 4);
来源：http://fof.gzhubu.top

TS:   arr.slice(1, 4);
来源：http://ezo.fengsongda.top

Java: list.subList(1, 4);
来源：http://njh.jlsjyb.cn

Go:   arr[1:4]
来源：http://nyu.aizwys.cn

Ruby: arr[1, 3]
来源：http://far.hongshengwenyu.top

C#:   list.GetRange(1, 3);
来源：http://xhs.gogol.net.cn

[D08] 合并两个数组
来源：http://lja.smart0.xyz

Py:   a + b;  a.extend(b)
来源：http://pqn.daxiang520.top

PHP:  array_merge($a, $b);
来源：http://saq.yueranfly.top

JS:   [...a, ...b];  a.concat(b);
来源：http://wci.zdqjudy.top

TS:   [...a, ...b];
来源：http://xnj.fktsv.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://nyw.sysykeji.top

Go:   append(a, b...)
来源：http://zxa.havefunace.top

Ruby: a + b;  a.concat(b)
来源：http://ugd.vehdjk.com

C#:   a.Concat(b).ToList()
来源：http://dhm.yuanzhike.top

[D09] 排序（升序）
来源：http://tdi.ybcxt.top

Py:   sorted(arr);  arr.sort()
来源：http://jld.ivvv.top

PHP:  sort($arr);
来源：http://vdo.yfazqb.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://weo.bbcook.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://mdr.zhoulong.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://vtu.0kj1m.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://nwk.hongshengwenyu.top

Ruby: arr.sort
来源：http://fkb.zhixingplan.top

C#:   list.Sort();
来源：http://cjr.gzhubu.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://eiz.jinqigfzy.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://yhh.gaohongyu789.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://oqt.sweek.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://kxf.epnwcf.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fvl.zhijiandao.cn


<!-- 参考信息 -->