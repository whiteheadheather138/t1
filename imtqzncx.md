代发 wailian999

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://zzw.aibaodan.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wat.fktsv.cn

[B11] 生成数字序列 / 区间
来源：http://bac.cqqwz.cn

Py:   list(range(0, 10, 2))
来源：http://qax.jlsjyb.cn

PHP:  range(0, 10, 2);
来源：http://qgi.guowangkeji.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qgu.shanyushiyangtech.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://usd.xingfuxueyuan.xyz

Java: IntStream.range(0, 10).boxed().toList()
来源：http://jue.vehdjk.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://yqi.pycfn.com

Ruby: (0...10).step(2).to_a
来源：http://vul.gaohongyu789.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://svq.jinyuanbaomall.cn

[B12] 跳出多层循环
来源：http://diu.yj20258888.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://vqn.daria6918.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ssv.vqdsnc.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hwl.jyoumei.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://gbm.gotoacloud.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://apy.zhixingplan.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://lat.uphjek.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mbu.meibo888.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://nda.xziqi.cn

[B13] 判断是否为数字
来源：http://jpr.cashguo.top

Py:   isinstance(x, (int, float))
来源：http://yru.gogol.net.cn

PHP:  is_numeric($x)
来源：http://juy.9152youxi.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pla.bjfxy.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://iux.gogol.net.cn

Java: x instanceof Number
来源：http://fxf.zhengqikj.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://czm.sysykeji.top

Ruby: x.is_a?(Numeric)
来源：http://hng.xuetiantiany.cn

C#:   x is int or double or decimal
来源：http://oxd.gogol.net.cn

[B14] 判断值是否在集合内
来源：http://gzh.zdbjq.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hrk.nanxuanxn.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://zdr.ydzc1.top

JS:   [1, 2, 3].includes(x)
来源：http://byn.cheryme.top

TS:   [1, 2, 3].includes(x)
来源：http://qwv.nanxinkj.top

Java: List.of(1, 2, 3).contains(x)
来源：http://zcv.daxiang520.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://yno.xinyue.icu

Ruby: [1, 2, 3].include?(x)
来源：http://fak.feifeiyinyue.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://unn.zdbjq.cn

[B15] 布尔运算与取反
来源：http://clg.wangshuangyany.cn

Py:   a and b or not c
来源：http://lmg.yuxming.cn

PHP:  $a && $b || !$c
来源：http://nxa.bjfxy.top

JS:   a && b || !c
来源：http://znm.jlsjyb.cn

TS:   a && b || !c
来源：http://igl.ywan-chungtsiang.top

Java: a && b || !c
来源：http://wph.aizwys.cn

Go:   a && b || !c
来源：http://fqp.yanxiufei.cn

Ruby: a && b || !c
来源：http://cgk.ydzc1.top

C#:   a && b || !c
来源：http://vrx.ybcxt.top

[B16] 卫语句：不满足条件提前返回
来源：http://euj.zhijiandao.cn

Py:   if not data: return
来源：http://xet.fengsongda.top

PHP:  if (!$data) { return; }
来源：http://tyn.zhoulong.xyz

JS:   if (!data) return;
来源：http://hop.zhijiandao.cn

TS:   if (!data) return;
来源：http://wto.xuetiantiany.cn

Java: if (data == null) return;
来源：http://iyp.birdmap.top

Go:   if data == nil { return }
来源：http://fns.jlsjyb.cn

Ruby: return if data.nil?
来源：http://kvv.jlsjyb.cn

C#:   if (data == null) return;
来源：http://tbp.yj202588.top

================================================================================
来源：http://rzd.yongpay.top

C. 函数与作用域
来源：http://hnk.zhongyouzk.top

================================================================================
来源：http://ime.tianlin.xyz

[C01] 定义函数
来源：http://hjw.cdnleiting.top

Py:   def add(a, b): return a + b
来源：http://oug.iojbl.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ahc.zycfv.cn

JS:   function add(a, b) { return a + b; }
来源：http://njk.andypj.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qwb.wangshuangyany.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://vkd.shuidangran.top

Go:   func add(a, b int) int { return a + b }
来源：http://axl.hywenlv.cn

Ruby: def add(a, b); a + b; end
来源：http://mzp.zdbjq.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hvm.fengsongda.top

[C02] 默认参数
来源：http://reb.nwbrower.top

Py:   def greet(name="World"): return name
来源：http://dqx.yangfankeji.com

PHP:  function greet($name = "World") { return $name; }
来源：http://jie.jinqigufen.top

JS:   function greet(name = "World") { return name; }
来源：http://qcu.bbcook.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://fla.gzhubu.top

Java: // 无默认参数：方法重载或 Optional
来源：http://qaz.52xcode.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://dds.shanyushiyangtech.top

Ruby: def greet(name = "World") = name
来源：http://fll.haohaochexian.top

C#:   string Greet(string name = "World") => name;
来源：http://scf.haohaochexian.top

[C03] 可变参数
来源：http://gzu.zdqjudy.top

Py:   def total(*args): return sum(args)
来源：http://bdg.jyoumei.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hiu.yj20258.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://kmt.hammf.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xfb.yongpay.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://uov.birdmap.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mky.tian-w.cn

Ruby: def total(*nums); nums.sum; end
来源：http://vlg.ybcxt.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://sam.jinghuilouyu.cn

[C04] 命名参数 / 关键字参数
来源：http://hyc.yj20258.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://eso.dianchejie.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://kti.ybcxt.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://tju.daria6918.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://tbc.mhx1999.top

Java: // 无：用 Builder 模式或 record
来源：http://lpa.haohaochexian.top

Go:   // 无：用配置结构体参数
来源：http://dqt.zycfv.cn

Ruby: f(a: 1, b: 2)
来源：http://rpi.mhx1999.top

C#:   f(a: 1, b: 2)
来源：http://nhq.ydjk.org.cn

[C05] 返回多个值
来源：http://xmr.ehwqpu.com

Py:   return a, b
来源：http://kxl.wangshuangyany.cn

PHP:  return [$a, $b];
来源：http://iyi.nanxinkj.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://fqf.guowangkeji.top

TS:   return { a, b };
来源：http://rkz.daria6918.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://zdt.zdqjudy.top

Go:   return a, b
来源：http://tvv.fktsv.cn

Ruby: return a, b
来源：http://klx.jqgfzy.top

C#:   return (a, b);              // ValueTuple
来源：http://xji.tarul.cn

[C06] 匿名函数 / lambda
来源：http://ggz.chenzaomai.com

Py:   square = lambda x: x * x
来源：http://mxf.sufxvd.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://nvl.bjfxy.top

JS:   const square = x => x * x;
来源：http://tqn.yonumen.top

TS:   const square = (x: number): number => x * x;
来源：http://jdt.jyoumei.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ozj.shanyushiyangkeji.top

Go:   sq := func(x int) int { return x * x }
来源：http://zvs.cucudq.cn

Ruby: square = ->(x) { x * x }
来源：http://oau.shuidangran.top

C#:   Func<int, int> square = x => x * x;
来源：http://ace.gzhubu.top

[C07] 把函数作为参数传入
来源：http://zmb.sxryk.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://suh.tanke756.top

PHP:  array_map("strtoupper", $arr);
来源：http://kwc.sufxvd.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ozy.c1oappe.top

TS:   arr.map(String)
来源：http://nvx.zhaomingkeji.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wei.hnxiangtu.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ksq.fengsongda.top

Ruby: arr.map(&:upcase)
来源：http://agd.zhijiandao.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://xpn.jinghuilouyu.cn

[C08] 闭包
来源：http://nbd.hammf.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://yuf.redwolf501.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://gdv.ppjwa.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://fgd.jlsjyb.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ftn.shanyushiyangtech.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://max.sweek.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hbw.sweek.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ytr.shanyushiyangkeji.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://qkx.sjlbkw.cn

[C09] 递归
来源：http://nkh.ctjpmb.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://esx.ppjwa.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://lal.zhongyouzk.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wkq.ctjpmb.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ofp.daxiang520.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://oix.wangshuangyany.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://tcb.sxryk.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://srk.xziqi.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ybz.ivvv.top

[C10] 变量作用域
来源：http://avq.dashuyun.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://sfi.fengsongda.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hen.guannengcc.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://vpl.yueranfly.top

TS:   同 JS
来源：http://emz.xylfe.cn

Java: 方法内为块级作用域
来源：http://hhd.cheryme.top

Go:   花括号块级作用域
来源：http://atl.zycfv.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hvy.kuanghao11.cn

C#:   块级作用域
来源：http://oef.ywan-chungtsiang.top

[C11] 模块导入与导出
来源：http://vdu.tanke756.top

Py:   from module import func
来源：http://cuw.vqdsnc.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://raf.hysaishi.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://djj.meibo888.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://snb.316326.xyz

Java: import java.util.List;
来源：http://kbr.sufxvd.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mbn.chenzaomai.com

Ruby: require "json"; require_relative "./util"
来源：http://gyy.gzhubu.top

C#:   using System.Text;
来源：http://jzz.xinyue.icu

[C12] 立即执行函数 IIFE
来源：http://zek.zhiwuduotai.top

Py:   (lambda: print("run"))()
来源：http://viu.hnxiangtu.top

PHP:  (function () { echo "run"; })();
来源：http://pbf.chenzaomai.com

JS:   (() => { console.log("run"); })();
来源：http://cwt.ehwqpu.com

TS:   (() => { console.log("run"); })();
来源：http://uro.havefunace.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://izt.ivvv.top

Go:   func() { fmt.Println("run") }()
来源：http://amg.yangfankeji.com

Ruby: -> { puts "run" }.call
来源：http://izs.wangshuangyany.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://psq.cucudq.cn

[C13] 类型声明 / 类型注解
来源：http://jwa.nanxuanxn.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://msd.jinyuanbaomall.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jyu.svipenyu.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://eqt.xingfuxueyuan.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ptm.vehdjk.com

Java: int add(int a, int b) { return a + b; }
来源：http://lbi.zhiwuduotai.top

Go:   func add(a, b int) int
来源：http://juk.zhoulong.xyz

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ytt.shanyushiyangtech.top

C#:   int Add(int a, int b) => a + b;
来源：http://fyn.chenlongwang.top

[C14] 泛型函数
来源：http://cxs.ctjpmb.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ljn.iojbl.cn

PHP:  // 无泛型
来源：http://qfy.zhixingplan.top

JS:   // 无泛型
来源：http://rmc.yj20258.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://esx.haohaochexian.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://xfl.nanxuanxn.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://lnt.sxryk.cn

Ruby: # 无泛型
来源：http://gqd.chenlongwang.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://tid.fanxiaobao.xyz

[C15] 解构 / 展开参数
来源：http://icv.daria6918.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://fdf.jiagoushi.top

PHP:  [$a, $b] = $pair;
来源：http://xes.haohaochexian.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://jnk.ctjpmb.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blr.cdnleiting.top

Java: // 无解构
来源：http://iyk.jyoumei.cn

Go:   // 无解构
来源：http://jmx.fzhhl.top

Ruby: a, b = pair
来源：http://ttd.shzxlz.cn

C#:   var (a, b) = pair;
来源：http://flv.xziqi.cn

[C16] 函数 / 方法重载
来源：http://amr.feifeiyinyue.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://bhj.zdbjq.cn

PHP:  // 无重载
来源：http://byf.ehwqpu.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://tak.ywan-chungtsiang.top

TS:   // 用联合类型或重载签名声明
来源：http://mto.yangfankeji.com

Java: void f(int a) {}  void f(String a) {}
来源：http://cet.pycfn.com

Go:   // 无重载：用不同函数名
来源：http://ywn.quarkkingdee.top

Ruby: # 无重载：靠动态参数
来源：http://jjn.nanxuanxn.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://xnu.kuanghao11.cn

================================================================================
来源：http://bty.gotoacloud.top

D. 数组 / 列表 / 集合
来源：http://rej.tianlin.xyz

================================================================================
来源：http://bhq.bbcook.cn

[D01] 创建数组 / 列表
来源：http://qaw.iojbl.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://bpq.haohaochexian.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ktw.snrcjt.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://dfi.jiagoushi.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://goz.daxiang520.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://xjs.guowangkeji.top

Go:   arr := []int{1, 2, 3}
来源：http://nbd.fktsv.cn

Ruby: arr = [1, 2, 3]
来源：http://bdi.cucudq.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://pav.cheryme.top

[D02] 追加元素到末尾
来源：http://kcy.yuanzhike.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://zrt.feifeiyinyue.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://eql.pengpengdd.cyou

JS:   arr.push(4);
来源：http://tgg.zdbjq.cn

TS:   arr.push(4);
来源：http://pyf.zycfv.cn

Java: list.add(4);
来源：http://hhn.andypj.xyz

Go:   arr = append(arr, 4)
来源：http://nnm.9152youxi.cn

Ruby: arr << 4; arr.push(5)
来源：http://bwb.yj20258.top

C#:   list.Add(4);
来源：http://amc.tarul.cn

[D03] 在指定位置插入元素
来源：http://jju.yongpay.top

Py:   arr.insert(0, 0)
来源：http://jrg.9152youxi.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://qqc.fengsongda.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wyo.birdmap.top

TS:   arr.splice(0, 0, 0);
来源：http://bla.fzhhl.top

Java: list.add(0, 0);
来源：http://kpb.zhengqikj.top

Go:   arr = append([]int{0}, arr...)
来源：http://hrj.sysykeji.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://pmk.tianlin.xyz

C#:   list.Insert(0, 0);
来源：http://fvr.jinghuilouyu.cn

[D04] 删除元素
来源：http://tce.jqgfzy.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wfh.yfazqb.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ocf.snrcjt.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://rsl.9152youxi.cn

TS:   arr.splice(0, 1);
来源：http://tup.chenzaomai.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://kyo.jlsjyb.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://gcr.zhaomingkeji.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mxz.sweek.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://irp.zhengqikj.top

[D05] 访问与修改元素
来源：http://bjm.jqgfzy.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hpa.zhixingplan.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://tiq.9152youxi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://tiq.sysykeji.top

TS:   arr[0]; arr.at(-1);
来源：http://cqw.hongshengwenyu.top

Java: list.get(0); list.set(0, 9);
来源：http://ard.xinyue.icu

Go:   arr[0]; arr[0] = 9
来源：http://esu.zhijiandao.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ijk.9152youxi.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hqn.jinqigfzy.top

[D06] 数组长度
来源：http://npr.nanxinkj.top

Py:   len(arr)
来源：http://jzt.zhengqikj.top

PHP:  count($arr);
来源：http://xrw.tarul.cn

JS:   arr.length
来源：http://afl.9152youxi.cn

TS:   arr.length
来源：http://nps.gaohongyu789.top

Java: list.size();
来源：http://ycv.ydjk.org.cn

Go:   len(arr)
来源：http://qky.fktsv.cn

Ruby: arr.length; arr.size
来源：http://ops.chenjidiqi.icu

C#:   list.Count;
来源：http://iom.zhoulong.xyz

[D07] 切片 / 取子数组
来源：http://qkr.fengsongda.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ibt.yueranfly.top

PHP:  array_slice($arr, 1, 3);
来源：http://hje.nanxinkj.top

JS:   arr.slice(1, 4);
来源：http://dxr.xuanzx.com

TS:   arr.slice(1, 4);
来源：http://tnl.xuanzx.com

Java: list.subList(1, 4);
来源：http://any.tarul.cn

Go:   arr[1:4]
来源：http://uzk.wangdashe.top

Ruby: arr[1, 3]
来源：http://brf.zdbjq.cn

C#:   list.GetRange(1, 3);
来源：http://bqm.ydjk.org.cn

[D08] 合并两个数组
来源：http://fyu.yuxming.cn

Py:   a + b;  a.extend(b)
来源：http://tpd.hywenlv.cn

PHP:  array_merge($a, $b);
来源：http://mej.yj202588.top

JS:   [...a, ...b];  a.concat(b);
来源：http://swm.smart0.xyz

TS:   [...a, ...b];
来源：http://rte.xingfuxueyuan.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://eos.jlsjyb.cn

Go:   append(a, b...)
来源：http://eoc.shangyingyoupin.top

Ruby: a + b;  a.concat(b)
来源：http://xxl.9152youxi.cn

C#:   a.Concat(b).ToList()
来源：http://pvv.gogol.net.cn

[D09] 排序（升序）
来源：http://dcy.gzhubu.top

Py:   sorted(arr);  arr.sort()
来源：http://rwp.jianghu66.top

PHP:  sort($arr);
来源：http://ydm.snrcjt.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://msr.feifeiyinyue.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://zun.shzxlz.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://nll.pengpengdd.cyou

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://rth.daxiang520.top

Ruby: arr.sort
来源：http://maq.ywan-chungtsiang.top

C#:   list.Sort();
来源：http://rqg.zhixingplan.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://zpx.yonumen.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wiw.snrcjt.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xjm.epnwcf.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://pwn.xuanzx.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://htd.hesvh.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://osk.jianghu66.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://zhd.zhijiandao.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://yfl.jinyuanbaomall.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ibr.chenlongwang.top

[D11] 反转数组
来源：http://jxn.ydzc1.top

Py:   arr[::-1];  arr.reverse()
来源：http://rlp.cdnleiting.top

PHP:  array_reverse($arr);
来源：http://hjv.zhijiandao.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mrc.yanxiufei.cn


<!-- 参考信息 -->