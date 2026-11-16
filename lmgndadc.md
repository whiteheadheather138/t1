代发 wailian999

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vaj.yonumen.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://irg.wangshuangyany.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://abg.xuetiantiany.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hzz.mhx1999.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ibs.dashuyun.cn

[B10] 遍历同时拿索引
来源：http://ffu.52xcode.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://lwg.svipenyu.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ffv.xylfe.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://pnd.ywan-chungtsiang.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://yvb.birdmap.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://fom.zhixingplan.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://las.shangyingyoupin.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://gnb.ppjwa.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://roy.sjlbkw.cn

[B11] 生成数字序列 / 区间
来源：http://jhs.zhoulong.xyz

Py:   list(range(0, 10, 2))
来源：http://wjo.smart0.xyz

PHP:  range(0, 10, 2);
来源：http://yyy.tanke756.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://awo.ybcxt.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zul.nanxinkj.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://eia.guowangkeji.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://rph.shuidangran.top

Ruby: (0...10).step(2).to_a
来源：http://pqs.zycfv.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://lmq.smart0.xyz

[B12] 跳出多层循环
来源：http://itc.ywan-chungtsiang.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://eaa.fzhhl.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://kxa.hongshengwenyu.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mon.birdmap.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://fno.xingfuxueyuan.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ksn.c1oappe.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://yjh.fengsongda.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://lkt.smart0.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://rmi.daria6918.cn

[B13] 判断是否为数字
来源：http://pwp.pycfn.com

Py:   isinstance(x, (int, float))
来源：http://zgl.fehbvm.com

PHP:  is_numeric($x)
来源：http://egq.ehwqpu.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://biq.ivvv.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://iet.quarkkingdee.top

Java: x instanceof Number
来源：http://pyy.hysaishi.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wwi.sweek.top

Ruby: x.is_a?(Numeric)
来源：http://oki.ydzc1.top

C#:   x is int or double or decimal
来源：http://vqv.jinghuilouyu.cn

[B14] 判断值是否在集合内
来源：http://hut.c1oappe.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://zbb.yuxming.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://gfc.fanxiaobao.xyz

JS:   [1, 2, 3].includes(x)
来源：http://jah.zhengqikj.top

TS:   [1, 2, 3].includes(x)
来源：http://nwq.aibaodan.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://mfl.yangfankeji.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://jng.ywan-chungtsiang.top

Ruby: [1, 2, 3].include?(x)
来源：http://htr.sxryk.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hqb.cashguo.top

[B15] 布尔运算与取反
来源：http://ewy.tarul.cn

Py:   a and b or not c
来源：http://yww.hammf.cn

PHP:  $a && $b || !$c
来源：http://lgn.meibo888.top

JS:   a && b || !c
来源：http://kjw.wangdashe.top

TS:   a && b || !c
来源：http://kfy.havefunace.top

Java: a && b || !c
来源：http://thi.shzxlz.cn

Go:   a && b || !c
来源：http://arl.fehbvm.com

Ruby: a && b || !c
来源：http://iex.zhixingplan.top

C#:   a && b || !c
来源：http://okw.yfazqb.com

[B16] 卫语句：不满足条件提前返回
来源：http://qgy.nanxinkj.top

Py:   if not data: return
来源：http://jvw.yj20258.top

PHP:  if (!$data) { return; }
来源：http://jtb.yj20258888.top

JS:   if (!data) return;
来源：http://mve.xuanzx.com

TS:   if (!data) return;
来源：http://vtv.ywan-chungtsiang.top

Java: if (data == null) return;
来源：http://mey.birdmap.top

Go:   if data == nil { return }
来源：http://iyn.shuidangran.top

Ruby: return if data.nil?
来源：http://kgf.sjlbkw.cn

C#:   if (data == null) return;
来源：http://uxh.iojbl.cn

================================================================================
来源：http://lsp.ydzc1.top

C. 函数与作用域
来源：http://gln.shuidangran.top

================================================================================
来源：http://flw.hammf.cn

[C01] 定义函数
来源：http://alx.yonumen.top

Py:   def add(a, b): return a + b
来源：http://wrd.52xcode.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cvu.zhengqikj.top

JS:   function add(a, b) { return a + b; }
来源：http://ueb.nanxinkj.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yzp.bjfxy.top

Java: static int add(int a, int b) { return a + b; }
来源：http://gjb.xingfuxueyuan.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://wyq.daria6918.cn

Ruby: def add(a, b); a + b; end
来源：http://ujw.nwbrower.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://okx.hcnkem.com

[C02] 默认参数
来源：http://www.hnqzz.top

Py:   def greet(name="World"): return name
来源：http://awq.snrcjt.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://odj.cucudq.cn

JS:   function greet(name = "World") { return name; }
来源：http://yzf.sxryk.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://zlg.yfazqb.com

Java: // 无默认参数：方法重载或 Optional
来源：http://qld.fktsv.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://fuv.hfpthk.cn

Ruby: def greet(name = "World") = name
来源：http://pcv.bjfxy.top

C#:   string Greet(string name = "World") => name;
来源：http://bdf.fktsv.cn

[C03] 可变参数
来源：http://eyf.jinqigufen.top

Py:   def total(*args): return sum(args)
来源：http://lge.cdnleiting.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://vkd.shuidangran.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://xku.yvedp.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://enf.jinqigfzy.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://cce.nwbrower.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://opg.redwolf501.top

Ruby: def total(*nums); nums.sum; end
来源：http://kbg.9152youxi.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://xoh.sjlbkw.cn

[C04] 命名参数 / 关键字参数
来源：http://plq.0kj1m.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ypp.hywenlv.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://fzr.chenlongwang.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://qii.ivvv.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wro.chenlongwang.top

Java: // 无：用 Builder 模式或 record
来源：http://swa.dianchejie.cn

Go:   // 无：用配置结构体参数
来源：http://fjl.chenzaomai.com

Ruby: f(a: 1, b: 2)
来源：http://jyj.ehwqpu.com

C#:   f(a: 1, b: 2)
来源：http://ruk.chenjidiqi.icu

[C05] 返回多个值
来源：http://szx.pycfn.com

Py:   return a, b
来源：http://spz.ydjk.org.cn

PHP:  return [$a, $b];
来源：http://lhi.mhx1999.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://zcu.xziqi.cn

TS:   return { a, b };
来源：http://swy.dianchejie.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://leu.yongpay.top

Go:   return a, b
来源：http://pxi.gogol.net.cn

Ruby: return a, b
来源：http://cnm.fzhhl.top

C#:   return (a, b);              // ValueTuple
来源：http://giw.c1oappe.top

[C06] 匿名函数 / lambda
来源：http://vyi.xinyue.icu

Py:   square = lambda x: x * x
来源：http://gzp.wangdashe.top

PHP:  $square = fn($x) => $x * $x;
来源：http://vws.gogol.net.cn

JS:   const square = x => x * x;
来源：http://wvn.hcnkem.com

TS:   const square = (x: number): number => x * x;
来源：http://dqn.andypj.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hpj.daxiang520.top

Go:   sq := func(x int) int { return x * x }
来源：http://qdl.hcnkem.com

Ruby: square = ->(x) { x * x }
来源：http://qxd.kuanghao11.cn

C#:   Func<int, int> square = x => x * x;
来源：http://lkn.pycfn.com

[C07] 把函数作为参数传入
来源：http://cey.bjfxy.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://jxy.smart0.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://pve.xylfe.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mhy.yuxming.cn

TS:   arr.map(String)
来源：http://ops.ydzc1.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hsb.cashguo.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://xbm.nanxinkj.top

Ruby: arr.map(&:upcase)
来源：http://txp.birdmap.top

C#:   arr.Select(s => s.ToUpper())
来源：http://plj.shuidangran.top

[C08] 闭包
来源：http://cvi.jianghu66.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ojh.xingfuxueyuan.xyz

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://xjd.xuanzx.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://kuf.cdnleiting.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://vww.316326.xyz

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://zlr.yuxming.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://oag.zhaomingkeji.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ymq.vqdsnc.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://zvl.uphjek.com

[C09] 递归
来源：http://woc.svipenyu.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://kry.svipenyu.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ixc.yonumen.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://oil.chenzaomai.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://iwb.wangdashe.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ipb.hesvh.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hib.zdqjudy.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ccj.yj202588.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://qjf.shzxlz.cn

[C10] 变量作用域
来源：http://ieb.fanxiaobao.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://bkt.yvedp.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ujh.daxiang520.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://gnk.chenlongwang.top

TS:   同 JS
来源：http://hup.hysaishi.cn

Java: 方法内为块级作用域
来源：http://xyd.wangshuangyany.cn

Go:   花括号块级作用域
来源：http://jra.zhoulong.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://vrp.zycfv.cn

C#:   块级作用域
来源：http://tue.yonumen.top

[C11] 模块导入与导出
来源：http://cva.shanyushiyangtech.top

Py:   from module import func
来源：http://xrn.pycfn.com

PHP:  require "file.php";  或 use App\Service;
来源：http://tjk.ywan-chungtsiang.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://qkn.tarul.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ckm.wangshuangyany.cn

Java: import java.util.List;
来源：http://suv.wangdashe.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://rqh.yj20258.top

Ruby: require "json"; require_relative "./util"
来源：http://ipx.smart0.xyz

C#:   using System.Text;
来源：http://dnh.sweek.top

[C12] 立即执行函数 IIFE
来源：http://uku.yvedp.cn

Py:   (lambda: print("run"))()
来源：http://lnj.9152youxi.cn

PHP:  (function () { echo "run"; })();
来源：http://raj.fanxiaobao.xyz

JS:   (() => { console.log("run"); })();
来源：http://oga.sysykeji.top

TS:   (() => { console.log("run"); })();
来源：http://pnn.zhaomingkeji.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://cxk.yfazqb.com

Go:   func() { fmt.Println("run") }()
来源：http://wuw.shuidangran.top

Ruby: -> { puts "run" }.call
来源：http://hks.xziqi.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://eqw.yuxming.cn

[C13] 类型声明 / 类型注解
来源：http://erj.hesvh.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://kyq.haohaochexian.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://spm.zdqjudy.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ppa.redwolf501.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nzn.jinghuilouyu.cn

Java: int add(int a, int b) { return a + b; }
来源：http://sji.zhengqikj.top

Go:   func add(a, b int) int
来源：http://ckf.pycfn.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://tga.sufxvd.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ffs.andypj.xyz

[C14] 泛型函数
来源：http://tgu.vehdjk.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://vyr.quarkkingdee.top

PHP:  // 无泛型
来源：http://usu.chenlongwang.top

JS:   // 无泛型
来源：http://eio.jqgufenzy.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://okg.jqgfzy.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://itc.jinyuanbaomall.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://qsj.zdqjudy.top

Ruby: # 无泛型
来源：http://tyh.0kj1m.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://vdb.meibo888.top

[C15] 解构 / 展开参数
来源：http://qmg.316326.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xdi.jinqigfzy.top

PHP:  [$a, $b] = $pair;
来源：http://mmb.shanyushiyangkeji.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://fnj.tianlin.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://eyu.jlsjyb.cn

Java: // 无解构
来源：http://kaf.daria6918.cn

Go:   // 无解构
来源：http://hnf.yvedp.cn

Ruby: a, b = pair
来源：http://swh.bjfxy.top

C#:   var (a, b) = pair;
来源：http://aov.zhoulong.xyz

[C16] 函数 / 方法重载
来源：http://qhc.yueranfly.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ekd.hywenlv.cn

PHP:  // 无重载
来源：http://roe.gotoacloud.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://rtt.ywan-chungtsiang.top

TS:   // 用联合类型或重载签名声明
来源：http://qxm.gotoacloud.top

Java: void f(int a) {}  void f(String a) {}
来源：http://zvn.jinghuilouyu.cn

Go:   // 无重载：用不同函数名
来源：http://lqd.haohaochexian.top

Ruby: # 无重载：靠动态参数
来源：http://ihv.xziqi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ply.tianlin.xyz

================================================================================
来源：http://pnl.xuetiantiany.cn

D. 数组 / 列表 / 集合
来源：http://mov.uphjek.com

================================================================================
来源：http://xjc.zhengqikj.top

[D01] 创建数组 / 列表
来源：http://kxn.chenlongwang.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://hgu.smart0.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wuy.hammf.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://tae.cucudq.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://qdn.sysykeji.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://bsq.52xcode.cn

Go:   arr := []int{1, 2, 3}
来源：http://paf.svipenyu.cn

Ruby: arr = [1, 2, 3]
来源：http://mou.gotoacloud.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ljm.nanxinkj.top

[D02] 追加元素到末尾
来源：http://ydj.redwolf501.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ddk.sweek.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://afg.jinghuilouyu.cn

JS:   arr.push(4);
来源：http://qgo.cdnleiting.top

TS:   arr.push(4);
来源：http://xgq.yvedp.cn

Java: list.add(4);
来源：http://syf.quarkkingdee.top

Go:   arr = append(arr, 4)
来源：http://ueo.xuanzx.com

Ruby: arr << 4; arr.push(5)
来源：http://pcw.wangdashe.top

C#:   list.Add(4);
来源：http://rla.guowangkeji.top

[D03] 在指定位置插入元素
来源：http://dzm.xuetiantiany.cn

Py:   arr.insert(0, 0)
来源：http://vja.dianchejie.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wqp.pengpengdd.cyou

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://msf.xziqi.cn

TS:   arr.splice(0, 0, 0);
来源：http://gon.gzhubu.top

Java: list.add(0, 0);
来源：http://duw.xinyue.icu

Go:   arr = append([]int{0}, arr...)
来源：http://wkp.ydzc1.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hha.cucudq.cn

C#:   list.Insert(0, 0);
来源：http://iih.jqgufenzy.top

[D04] 删除元素
来源：http://gsn.hfpthk.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://dek.shanyushiyangkeji.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://jbk.yuxming.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://zwn.jyoumei.cn

TS:   arr.splice(0, 1);
来源：http://uix.birdmap.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://egs.yongpay.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ipp.hysaishi.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://cyt.xinyue.icu

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://lqd.yj20258.top

[D05] 访问与修改元素
来源：http://fwx.smart0.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://sps.chenjidiqi.icu

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://utu.svipenyu.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://net.c1oappe.top

TS:   arr[0]; arr.at(-1);
来源：http://ryh.yj20258.top

Java: list.get(0); list.set(0, 9);
来源：http://qgl.xuetiantiany.cn

Go:   arr[0]; arr[0] = 9
来源：http://fca.zhaomingkeji.xyz

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://bey.hfpthk.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://uyq.zhaomingkeji.xyz

[D06] 数组长度
来源：http://ywa.ydzc1.top

Py:   len(arr)
来源：http://cdm.zycfv.cn

PHP:  count($arr);
来源：http://zyd.tian-w.cn

JS:   arr.length
来源：http://gnq.hammf.cn

TS:   arr.length
来源：http://zqy.aizwys.cn

Java: list.size();
来源：http://sbz.nwbrower.top

Go:   len(arr)
来源：http://hvd.haohaochexian.top

Ruby: arr.length; arr.size
来源：http://drk.9152youxi.cn

C#:   list.Count;
来源：http://qlp.yvedp.cn

[D07] 切片 / 取子数组
来源：http://gwc.fanxiaobao.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://jpa.sjlbkw.cn

PHP:  array_slice($arr, 1, 3);
来源：http://fqj.316326.xyz

JS:   arr.slice(1, 4);
来源：http://izy.wangshuangyany.cn

TS:   arr.slice(1, 4);
来源：http://iyf.jianghu66.top

Java: list.subList(1, 4);
来源：http://byb.nanxinkj.top

Go:   arr[1:4]
来源：http://tsx.ydzc1.top

Ruby: arr[1, 3]
来源：http://rxy.shanyushiyangkeji.top

C#:   list.GetRange(1, 3);
来源：http://uog.fzhhl.top

[D08] 合并两个数组
来源：http://zcf.guowangkeji.top

Py:   a + b;  a.extend(b)
来源：http://bzy.hcnkem.com

PHP:  array_merge($a, $b);
来源：http://oci.shangyingyoupin.top

JS:   [...a, ...b];  a.concat(b);
来源：http://gyc.jqgfzy.top

TS:   [...a, ...b];
来源：http://zsm.uphjek.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://pjx.bjfxy.top

Go:   append(a, b...)
来源：http://ecf.jlsjyb.cn

Ruby: a + b;  a.concat(b)
来源：http://uxc.xziqi.cn

C#:   a.Concat(b).ToList()
来源：http://bws.ywan-chungtsiang.top

[D09] 排序（升序）
来源：http://xpm.wangshuangyany.cn

Py:   sorted(arr);  arr.sort()
来源：http://mjb.gaohongyu789.top

PHP:  sort($arr);
来源：http://euh.cqqwz.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://chu.fanxiaobao.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://iob.kuanghao11.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://suy.ppjwa.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://jkz.fehbvm.com

Ruby: arr.sort
来源：http://ptw.fengsongda.top

C#:   list.Sort();
来源：http://wsl.chenjidiqi.icu

[D10] 自定义排序（按字段 / 多条件）
来源：http://uqt.jianghu66.top


<!-- 参考信息 -->