代发 wailian999

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://zpb.yanxiufei.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://whe.gaohongyu789.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ojc.sjlbkw.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ezz.uphjek.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mzs.cqqwz.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://woc.aibaodan.cn

[B11] 生成数字序列 / 区间
来源：http://luo.havefunace.top

Py:   list(range(0, 10, 2))
来源：http://uaq.yangfankeji.com

PHP:  range(0, 10, 2);
来源：http://sjt.jinqigufen.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://clp.zhengqikj.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nol.shuidangran.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://han.jqgufenzy.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://npp.cqqwz.cn

Ruby: (0...10).step(2).to_a
来源：http://new.jinqigfzy.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wor.yueranfly.top

[B12] 跳出多层循环
来源：http://mxo.yanxiufei.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ugs.ppjwa.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://kxg.wangdashe.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://yte.aibaodan.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://jjq.guannengcc.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://uxa.gogol.net.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wns.cqqwz.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://alm.yanxiufei.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://bcx.epnwcf.com

[B13] 判断是否为数字
来源：http://qal.yongpay.top

Py:   isinstance(x, (int, float))
来源：http://djv.cheryme.top

PHP:  is_numeric($x)
来源：http://qos.zhongyouzk.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fpj.ydzc1.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pff.sxryk.cn

Java: x instanceof Number
来源：http://phy.ydjk.org.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ikq.birdmap.top

Ruby: x.is_a?(Numeric)
来源：http://zzl.gaohongyu789.top

C#:   x is int or double or decimal
来源：http://bpl.jinyuanbaomall.cn

[B14] 判断值是否在集合内
来源：http://vjq.0kj1m.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://llt.cdnleiting.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wpf.vqdsnc.cn

JS:   [1, 2, 3].includes(x)
来源：http://ctk.zycfv.cn

TS:   [1, 2, 3].includes(x)
来源：http://tnz.yanxiufei.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://lnd.guowangkeji.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ehy.jinghuilouyu.cn

Ruby: [1, 2, 3].include?(x)
来源：http://xvf.dianchejie.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://iuy.xingfuxueyuan.xyz

[B15] 布尔运算与取反
来源：http://nrq.zhengqikj.top

Py:   a and b or not c
来源：http://vma.hnqzz.top

PHP:  $a && $b || !$c
来源：http://xly.jiagoushi.top

JS:   a && b || !c
来源：http://esw.ppjwa.cn

TS:   a && b || !c
来源：http://kme.redwolf501.top

Java: a && b || !c
来源：http://rzm.jlsjyb.cn

Go:   a && b || !c
来源：http://hzx.cqqwz.cn

Ruby: a && b || !c
来源：http://lbj.zhijiandao.cn

C#:   a && b || !c
来源：http://xjs.tian-w.cn

[B16] 卫语句：不满足条件提前返回
来源：http://bkr.sxryk.cn

Py:   if not data: return
来源：http://cck.nwbrower.top

PHP:  if (!$data) { return; }
来源：http://nkw.jlsjyb.cn

JS:   if (!data) return;
来源：http://xlg.tianlin.xyz

TS:   if (!data) return;
来源：http://ewd.jianghu66.top

Java: if (data == null) return;
来源：http://hwp.dashuyun.cn

Go:   if data == nil { return }
来源：http://frk.cashguo.top

Ruby: return if data.nil?
来源：http://qfa.snrcjt.cn

C#:   if (data == null) return;
来源：http://tqm.sxryk.cn

================================================================================
来源：http://pac.fengsongda.top

C. 函数与作用域
来源：http://muj.guannengcc.top

================================================================================
来源：http://hii.hfpthk.cn

[C01] 定义函数
来源：http://yju.zhiwuduotai.top

Py:   def add(a, b): return a + b
来源：http://tpy.svipenyu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hww.gogol.net.cn

JS:   function add(a, b) { return a + b; }
来源：http://svw.yueranfly.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jqw.chenlongwang.top

Java: static int add(int a, int b) { return a + b; }
来源：http://vud.xylfe.cn

Go:   func add(a, b int) int { return a + b }
来源：http://mxb.pengpengdd.cyou

Ruby: def add(a, b); a + b; end
来源：http://ufk.jinghuilouyu.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://rzj.smart0.xyz

[C02] 默认参数
来源：http://tyz.sufxvd.cn

Py:   def greet(name="World"): return name
来源：http://wqz.zhaomingkeji.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://ajo.jqgufenzy.top

JS:   function greet(name = "World") { return name; }
来源：http://idx.hnxiangtu.top

TS:   function greet(name: string = "World") { return name; }
来源：http://tnh.chenlongwang.top

Java: // 无默认参数：方法重载或 Optional
来源：http://ubk.fktsv.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://dxg.nwbrower.top

Ruby: def greet(name = "World") = name
来源：http://zlg.shzxlz.cn

C#:   string Greet(string name = "World") => name;
来源：http://pam.andypj.xyz

[C03] 可变参数
来源：http://lno.zdqjudy.top

Py:   def total(*args): return sum(args)
来源：http://prs.shuidangran.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xcm.aibaodan.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://rqm.zycfv.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mmz.jyoumei.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://jrn.sufxvd.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wfr.daxiang520.top

Ruby: def total(*nums); nums.sum; end
来源：http://cfe.316326.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://gqj.hesvh.cn

[C04] 命名参数 / 关键字参数
来源：http://hwj.chenlongwang.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://yma.pengpengdd.cyou

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hii.fzhhl.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wwc.yj20258888.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://bhm.yj20258.top

Java: // 无：用 Builder 模式或 record
来源：http://vob.aizwys.cn

Go:   // 无：用配置结构体参数
来源：http://wyg.cdnleiting.top

Ruby: f(a: 1, b: 2)
来源：http://tre.0kj1m.cn

C#:   f(a: 1, b: 2)
来源：http://adn.yj202588.top

[C05] 返回多个值
来源：http://vbo.vqdsnc.cn

Py:   return a, b
来源：http://ggv.cqqwz.cn

PHP:  return [$a, $b];
来源：http://mkb.chenlongwang.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://ywu.sweek.top

TS:   return { a, b };
来源：http://cyi.zdbjq.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://cpa.ybcxt.top

Go:   return a, b
来源：http://usm.jinqigufen.top

Ruby: return a, b
来源：http://xzj.cucudq.cn

C#:   return (a, b);              // ValueTuple
来源：http://vjh.tianlin.xyz

[C06] 匿名函数 / lambda
来源：http://vob.yj202588.top

Py:   square = lambda x: x * x
来源：http://rqg.smart0.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://vxt.fengsongda.top

JS:   const square = x => x * x;
来源：http://abl.hongshengwenyu.top

TS:   const square = (x: number): number => x * x;
来源：http://qtt.shzxlz.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://rdr.pycfn.com

Go:   sq := func(x int) int { return x * x }
来源：http://zpa.nanxinkj.top

Ruby: square = ->(x) { x * x }
来源：http://ejp.quarkkingdee.top

C#:   Func<int, int> square = x => x * x;
来源：http://qjj.birdmap.top

[C07] 把函数作为参数传入
来源：http://kia.zhixingplan.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://zgq.shangyingyoupin.top

PHP:  array_map("strtoupper", $arr);
来源：http://khb.yuxming.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://jhu.zdbjq.cn

TS:   arr.map(String)
来源：http://bil.yuxming.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://myg.cheryme.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wal.jinghuilouyu.cn

Ruby: arr.map(&:upcase)
来源：http://myy.yongpay.top

C#:   arr.Select(s => s.ToUpper())
来源：http://qxd.ehwqpu.com

[C08] 闭包
来源：http://ftw.yueranfly.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://woa.jinqigfzy.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://slc.dianchejie.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ndb.ctjpmb.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://cdk.xuetiantiany.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://zja.yj202588.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://rog.fzhhl.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://qer.cucudq.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ikw.andypj.xyz

[C09] 递归
来源：http://isx.hongshengwenyu.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://muh.shuidangran.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://gsk.sufxvd.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qsx.gogol.net.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://icf.dianchejie.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://obw.zhijiandao.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://tfq.daria6918.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://bnq.pengpengdd.cyou

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://anz.jyoumei.cn

[C10] 变量作用域
来源：http://jpl.nanxuanxn.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qbk.gzhubu.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://rsw.jinqigufen.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xae.jinqigufen.top

TS:   同 JS
来源：http://rxr.yueranfly.top

Java: 方法内为块级作用域
来源：http://hlr.cqqwz.cn

Go:   花括号块级作用域
来源：http://zcq.yfazqb.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mmq.tarul.cn

C#:   块级作用域
来源：http://qmy.chenzaomai.com

[C11] 模块导入与导出
来源：http://zst.pengpengdd.cyou

Py:   from module import func
来源：http://rnr.yangfankeji.com

PHP:  require "file.php";  或 use App\Service;
来源：http://ikg.sxryk.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://rpn.yuanzhike.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://rpu.jinqigfzy.top

Java: import java.util.List;
来源：http://xdg.guowangkeji.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://rni.yuxming.cn

Ruby: require "json"; require_relative "./util"
来源：http://iee.epnwcf.com

C#:   using System.Text;
来源：http://haa.gaohongyu789.top

[C12] 立即执行函数 IIFE
来源：http://lzb.shuidangran.top

Py:   (lambda: print("run"))()
来源：http://hps.fzhhl.top

PHP:  (function () { echo "run"; })();
来源：http://akd.meibo888.top

JS:   (() => { console.log("run"); })();
来源：http://jwi.ppjwa.cn

TS:   (() => { console.log("run"); })();
来源：http://qab.gogol.net.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://sro.zhaomingkeji.xyz

Go:   func() { fmt.Println("run") }()
来源：http://hht.havefunace.top

Ruby: -> { puts "run" }.call
来源：http://hhx.smart0.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://fdd.fengsongda.top

[C13] 类型声明 / 类型注解
来源：http://dhd.jqgfzy.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://eay.yvedp.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://taw.guannengcc.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://bqk.ybcxt.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xqh.yongpay.top

Java: int add(int a, int b) { return a + b; }
来源：http://vdc.c1oappe.top

Go:   func add(a, b int) int
来源：http://krh.xuanzx.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://lhc.dianchejie.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ldn.fzhhl.top

[C14] 泛型函数
来源：http://zef.cucudq.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://yjr.guannengcc.top

PHP:  // 无泛型
来源：http://sck.xylfe.cn

JS:   // 无泛型
来源：http://kfm.pengpengdd.cyou

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://jvs.xuetiantiany.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mss.aibaodan.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://pqs.chenzaomai.com

Ruby: # 无泛型
来源：http://oyi.chenlongwang.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://odz.sweek.top

[C15] 解构 / 展开参数
来源：http://uhc.yongpay.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://pax.wangdashe.top

PHP:  [$a, $b] = $pair;
来源：http://fxt.zhiwuduotai.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ian.jianghu66.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wqo.mhx1999.top

Java: // 无解构
来源：http://uwl.zhongyouzk.top

Go:   // 无解构
来源：http://bij.gaohongyu789.top

Ruby: a, b = pair
来源：http://msb.sufxvd.cn

C#:   var (a, b) = pair;
来源：http://ckc.hywenlv.cn

[C16] 函数 / 方法重载
来源：http://jie.havefunace.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://aqt.ctjpmb.com

PHP:  // 无重载
来源：http://fnj.ywan-chungtsiang.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://rfu.zhiwuduotai.top

TS:   // 用联合类型或重载签名声明
来源：http://zco.zhongyouzk.top

Java: void f(int a) {}  void f(String a) {}
来源：http://idf.xuetiantiany.cn

Go:   // 无重载：用不同函数名
来源：http://yuo.yuanzhike.top

Ruby: # 无重载：靠动态参数
来源：http://jvm.jinyuanbaomall.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://lya.cqqwz.cn

================================================================================
来源：http://nok.xziqi.cn

D. 数组 / 列表 / 集合
来源：http://shy.jinqigufen.top

================================================================================
来源：http://qph.sxryk.cn

[D01] 创建数组 / 列表
来源：http://iht.ywan-chungtsiang.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://ins.havefunace.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://lrv.nwbrower.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ycq.zhaomingkeji.xyz

TS:   const arr: number[] = [1, 2, 3];
来源：http://guj.zhixingplan.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://jyt.meibo888.top

Go:   arr := []int{1, 2, 3}
来源：http://ilr.sjlbkw.cn

Ruby: arr = [1, 2, 3]
来源：http://kne.cdnleiting.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mlx.andypj.xyz

[D02] 追加元素到末尾
来源：http://qgq.bbcook.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://jvt.hongshengwenyu.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://rxa.zhaomingkeji.xyz

JS:   arr.push(4);
来源：http://ktj.xingfuxueyuan.xyz

TS:   arr.push(4);
来源：http://ydb.zhoulong.xyz

Java: list.add(4);
来源：http://ild.mhx1999.top

Go:   arr = append(arr, 4)
来源：http://ykr.mhx1999.top

Ruby: arr << 4; arr.push(5)
来源：http://fhq.zhixingplan.top

C#:   list.Add(4);
来源：http://zvi.guowangkeji.top

[D03] 在指定位置插入元素
来源：http://hwg.yfazqb.com

Py:   arr.insert(0, 0)
来源：http://rcy.shanyushiyangtech.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://oow.yangfankeji.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://qvo.pycfn.com

TS:   arr.splice(0, 0, 0);
来源：http://flu.yonumen.top

Java: list.add(0, 0);
来源：http://gbd.jinghuilouyu.cn

Go:   arr = append([]int{0}, arr...)
来源：http://vul.pycfn.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://efn.yvedp.cn

C#:   list.Insert(0, 0);
来源：http://ewj.uphjek.com

[D04] 删除元素
来源：http://qrv.xuanzx.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://xwr.jinyuanbaomall.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hmp.epnwcf.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://nyn.316326.xyz

TS:   arr.splice(0, 1);
来源：http://ldr.zhengqikj.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://vss.dashuyun.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://bqe.andypj.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://aon.zdqjudy.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://qpw.dianchejie.cn

[D05] 访问与修改元素
来源：http://erl.vehdjk.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://vlf.jyoumei.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://qnv.nwbrower.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://lrq.hammf.cn

TS:   arr[0]; arr.at(-1);
来源：http://kib.guannengcc.top

Java: list.get(0); list.set(0, 9);
来源：http://zxz.epnwcf.com

Go:   arr[0]; arr[0] = 9
来源：http://nzt.xuanzx.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://jex.zdbjq.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wne.daria6918.cn

[D06] 数组长度
来源：http://onr.c1oappe.top

Py:   len(arr)
来源：http://fkc.sxryk.cn

PHP:  count($arr);
来源：http://mcx.hysaishi.cn

JS:   arr.length
来源：http://xfc.fengsongda.top

TS:   arr.length
来源：http://pml.ywan-chungtsiang.top

Java: list.size();
来源：http://ptu.daxiang520.top

Go:   len(arr)
来源：http://sga.hfpthk.cn

Ruby: arr.length; arr.size
来源：http://pdd.daxiang520.top

C#:   list.Count;
来源：http://ogr.shangyingyoupin.top

[D07] 切片 / 取子数组
来源：http://rmc.jianghu66.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://cxv.jinyuanbaomall.cn

PHP:  array_slice($arr, 1, 3);
来源：http://rfr.jinyuanbaomall.cn

JS:   arr.slice(1, 4);
来源：http://jds.ppjwa.cn

TS:   arr.slice(1, 4);
来源：http://rms.hfpthk.cn

Java: list.subList(1, 4);
来源：http://vvm.yfazqb.com

Go:   arr[1:4]
来源：http://cey.xziqi.cn

Ruby: arr[1, 3]
来源：http://fed.jqgfzy.top

C#:   list.GetRange(1, 3);
来源：http://dfx.sxryk.cn

[D08] 合并两个数组
来源：http://pme.0kj1m.cn

Py:   a + b;  a.extend(b)
来源：http://tui.tian-w.cn

PHP:  array_merge($a, $b);
来源：http://bha.dashuyun.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://kkh.zhengqikj.top

TS:   [...a, ...b];
来源：http://fvq.ctjpmb.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wcu.sxryk.cn

Go:   append(a, b...)
来源：http://pin.pycfn.com

Ruby: a + b;  a.concat(b)
来源：http://mjn.jlsjyb.cn

C#:   a.Concat(b).ToList()
来源：http://mrg.feifeiyinyue.top

[D09] 排序（升序）
来源：http://ygq.yfazqb.com

Py:   sorted(arr);  arr.sort()
来源：http://pvz.chenjidiqi.icu

PHP:  sort($arr);
来源：http://ksz.9152youxi.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mgv.guannengcc.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://vnm.yanxiufei.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://kpr.zhoulong.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://bcq.gogol.net.cn

Ruby: arr.sort
来源：http://wqc.andypj.xyz

C#:   list.Sort();
来源：http://nzy.nanxinkj.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://zyy.snrcjt.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://oby.sjlbkw.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dwf.iojbl.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://twt.c1oappe.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://tqp.cheryme.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://cjj.wangshuangyany.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://zkz.aizwys.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ztp.mhx1999.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ixb.sufxvd.cn


<!-- 参考信息 -->