代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://wjz.gotoacloud.top

PHP:  do { $i++; } while ($i < 10);
来源：http://ddz.feifeiyinyue.top

JS:   do { i++; } while (i < 10);
来源：http://mad.pengpengdd.cyou

TS:   do { i++; } while (i < 10);
来源：http://kip.mhx1999.top

Java: do { i++; } while (i < 10);
来源：http://mow.jqgufenzy.top

Go:   for { i++; if i >= 10 { break } }
来源：http://hdu.sysykeji.top

Ruby: begin; i += 1; end while i < 10
来源：http://jpt.fanxiaobao.xyz

C#:   do { i++; } while (i < 10);
来源：http://sgr.jiagoushi.top

[B09] break 与 continue
来源：http://mqo.yongpay.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wqg.xinyue.icu

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://tqb.ydzc1.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tkx.yueranfly.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ibv.fengsongda.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fzj.yj20258888.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wjj.guannengcc.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://itm.tarul.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ttd.wangdashe.top

[B10] 遍历同时拿索引
来源：http://opt.sufxvd.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ger.havefunace.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://kvi.zhengqikj.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://kht.feifeiyinyue.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://iqw.tanke756.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hug.sysykeji.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://vyd.aizwys.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ywz.jinqigfzy.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mja.fktsv.cn

[B11] 生成数字序列 / 区间
来源：http://rar.andypj.xyz

Py:   list(range(0, 10, 2))
来源：http://nmg.ywan-chungtsiang.top

PHP:  range(0, 10, 2);
来源：http://nfo.yanxiufei.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jki.vqdsnc.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bsi.jinqigufen.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://fsn.hcnkem.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://clq.cqqwz.cn

Ruby: (0...10).step(2).to_a
来源：http://kyt.bjfxy.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://trv.kuanghao11.cn

[B12] 跳出多层循环
来源：http://cdv.gotoacloud.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://his.vehdjk.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://auz.52xcode.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://uvn.xingfuxueyuan.xyz

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://gos.dashuyun.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hbj.wangshuangyany.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://pmu.meibo888.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://tmv.jyoumei.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wkh.sjlbkw.cn

[B13] 判断是否为数字
来源：http://fje.c1oappe.top

Py:   isinstance(x, (int, float))
来源：http://lxv.epnwcf.com

PHP:  is_numeric($x)
来源：http://naj.yj20258888.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zsf.shzxlz.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hja.epnwcf.com

Java: x instanceof Number
来源：http://sze.nanxuanxn.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://bur.jinqigfzy.top

Ruby: x.is_a?(Numeric)
来源：http://ffg.chenjidiqi.icu

C#:   x is int or double or decimal
来源：http://ylt.guannengcc.top

[B14] 判断值是否在集合内
来源：http://kvq.nanxuanxn.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://tmk.ybcxt.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://bmo.zdqjudy.top

JS:   [1, 2, 3].includes(x)
来源：http://vjp.fengsongda.top

TS:   [1, 2, 3].includes(x)
来源：http://fgt.jianghu66.top

Java: List.of(1, 2, 3).contains(x)
来源：http://nra.jlsjyb.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://nif.shangyingyoupin.top

Ruby: [1, 2, 3].include?(x)
来源：http://bfe.kuanghao11.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://jpk.jinghuilouyu.cn

[B15] 布尔运算与取反
来源：http://zzo.jqgfzy.top

Py:   a and b or not c
来源：http://gef.zdbjq.cn

PHP:  $a && $b || !$c
来源：http://owa.jianghu66.top

JS:   a && b || !c
来源：http://sob.aizwys.cn

TS:   a && b || !c
来源：http://wdv.wangdashe.top

Java: a && b || !c
来源：http://pic.yuxming.cn

Go:   a && b || !c
来源：http://vfe.sufxvd.cn

Ruby: a && b || !c
来源：http://ekr.cdnleiting.top

C#:   a && b || !c
来源：http://tae.dianchejie.cn

[B16] 卫语句：不满足条件提前返回
来源：http://uvs.yanxiufei.cn

Py:   if not data: return
来源：http://lvj.yuxming.cn

PHP:  if (!$data) { return; }
来源：http://rqf.havefunace.top

JS:   if (!data) return;
来源：http://aye.sjlbkw.cn

TS:   if (!data) return;
来源：http://vje.ehwqpu.com

Java: if (data == null) return;
来源：http://aot.9152youxi.cn

Go:   if data == nil { return }
来源：http://dtu.daxiang520.top

Ruby: return if data.nil?
来源：http://rua.yangfankeji.com

C#:   if (data == null) return;
来源：http://tgf.shanyushiyangkeji.top

================================================================================
来源：http://edc.yj20258888.top

C. 函数与作用域
来源：http://twf.haohaochexian.top

================================================================================
来源：http://kjx.fehbvm.com

[C01] 定义函数
来源：http://nyh.zhijiandao.cn

Py:   def add(a, b): return a + b
来源：http://ted.tanke756.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bhk.haohaochexian.top

JS:   function add(a, b) { return a + b; }
来源：http://zyi.fktsv.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://htb.gogol.net.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://hml.hnqzz.top

Go:   func add(a, b int) int { return a + b }
来源：http://qrd.cdnleiting.top

Ruby: def add(a, b); a + b; end
来源：http://ini.snrcjt.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://zom.xinyue.icu

[C02] 默认参数
来源：http://gos.zdqjudy.top

Py:   def greet(name="World"): return name
来源：http://yao.yj20258888.top

PHP:  function greet($name = "World") { return $name; }
来源：http://rcu.ppjwa.cn

JS:   function greet(name = "World") { return name; }
来源：http://hjf.0kj1m.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://gdy.0kj1m.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://gym.tarul.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://qet.mhx1999.top

Ruby: def greet(name = "World") = name
来源：http://wqa.zhongyouzk.top

C#:   string Greet(string name = "World") => name;
来源：http://zbe.sysykeji.top

[C03] 可变参数
来源：http://qgy.uphjek.com

Py:   def total(*args): return sum(args)
来源：http://zta.cucudq.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://zvr.guowangkeji.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://xei.zdqjudy.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://jqq.havefunace.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vss.epnwcf.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://tei.ybcxt.top

Ruby: def total(*nums); nums.sum; end
来源：http://yjk.pycfn.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://tho.guannengcc.top

[C04] 命名参数 / 关键字参数
来源：http://dir.jinqigfzy.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://sno.xingfuxueyuan.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://aog.xinyue.icu

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xzz.shuidangran.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://lvn.yueranfly.top

Java: // 无：用 Builder 模式或 record
来源：http://zds.nanxuanxn.top

Go:   // 无：用配置结构体参数
来源：http://hvx.ppjwa.cn

Ruby: f(a: 1, b: 2)
来源：http://ypf.vehdjk.com

C#:   f(a: 1, b: 2)
来源：http://eht.bbcook.cn

[C05] 返回多个值
来源：http://ozy.hongshengwenyu.top

Py:   return a, b
来源：http://pke.yj202588.top

PHP:  return [$a, $b];
来源：http://ckw.hnqzz.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://lse.jinqigfzy.top

TS:   return { a, b };
来源：http://wfz.yanxiufei.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wkl.ywan-chungtsiang.top

Go:   return a, b
来源：http://rpx.zdqjudy.top

Ruby: return a, b
来源：http://pyt.cashguo.top

C#:   return (a, b);              // ValueTuple
来源：http://qam.wangshuangyany.cn

[C06] 匿名函数 / lambda
来源：http://tcf.fengsongda.top

Py:   square = lambda x: x * x
来源：http://jjl.dashuyun.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://too.shangyingyoupin.top

JS:   const square = x => x * x;
来源：http://gys.yj20258.top

TS:   const square = (x: number): number => x * x;
来源：http://luq.uphjek.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://rwq.zhiwuduotai.top

Go:   sq := func(x int) int { return x * x }
来源：http://wvf.zhijiandao.cn

Ruby: square = ->(x) { x * x }
来源：http://xpy.nanxuanxn.top

C#:   Func<int, int> square = x => x * x;
来源：http://fnk.fzhhl.top

[C07] 把函数作为参数传入
来源：http://pjc.jinghuilouyu.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://abn.zhiwuduotai.top

PHP:  array_map("strtoupper", $arr);
来源：http://bus.smart0.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://gqa.tarul.cn

TS:   arr.map(String)
来源：http://mjc.wangshuangyany.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://jwn.xingfuxueyuan.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://vbe.ppjwa.cn

Ruby: arr.map(&:upcase)
来源：http://nwm.jianghu66.top

C#:   arr.Select(s => s.ToUpper())
来源：http://edr.fehbvm.com

[C08] 闭包
来源：http://lqr.ywan-chungtsiang.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://zvt.xylfe.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://qjv.chenzaomai.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://veu.yueranfly.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://kqe.ydjk.org.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://jah.cucudq.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://vjs.vqdsnc.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hun.yj20258888.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://lnj.wangshuangyany.cn

[C09] 递归
来源：http://ibd.feifeiyinyue.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mzn.feifeiyinyue.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://xna.guannengcc.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://byb.yongpay.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zjk.kuanghao11.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://dpl.yj20258888.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://bie.sufxvd.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://yar.ywan-chungtsiang.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://muf.ctjpmb.com

[C10] 变量作用域
来源：http://dhl.yuanzhike.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://bld.0kj1m.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://nwv.yangfankeji.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hvv.dianchejie.cn

TS:   同 JS
来源：http://aje.zycfv.cn

Java: 方法内为块级作用域
来源：http://fxc.gaohongyu789.top

Go:   花括号块级作用域
来源：http://opf.xuetiantiany.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mbp.redwolf501.top

C#:   块级作用域
来源：http://jas.uphjek.com

[C11] 模块导入与导出
来源：http://ukf.bbcook.cn

Py:   from module import func
来源：http://drt.yj202588.top

PHP:  require "file.php";  或 use App\Service;
来源：http://evo.nanxuanxn.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://pel.xinyue.icu

TS:   export function f(): void {};  import { f } from "./m";
来源：http://pcp.yanxiufei.cn

Java: import java.util.List;
来源：http://ngd.shanyushiyangkeji.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://htq.shanyushiyangkeji.top

Ruby: require "json"; require_relative "./util"
来源：http://dkm.havefunace.top

C#:   using System.Text;
来源：http://zao.snrcjt.cn

[C12] 立即执行函数 IIFE
来源：http://xsc.yangfankeji.com

Py:   (lambda: print("run"))()
来源：http://tsf.meibo888.top

PHP:  (function () { echo "run"; })();
来源：http://upa.shangyingyoupin.top

JS:   (() => { console.log("run"); })();
来源：http://ici.tanke756.top

TS:   (() => { console.log("run"); })();
来源：http://hus.zhongyouzk.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://tbm.yj202588.top

Go:   func() { fmt.Println("run") }()
来源：http://hlu.zhaomingkeji.xyz

Ruby: -> { puts "run" }.call
来源：http://tsi.sjlbkw.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://qal.yj202588.top

[C13] 类型声明 / 类型注解
来源：http://vca.shzxlz.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://fmx.zhoulong.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ouj.hesvh.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://yha.ctjpmb.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jzd.yueranfly.top

Java: int add(int a, int b) { return a + b; }
来源：http://nlq.9152youxi.cn

Go:   func add(a, b int) int
来源：http://fgp.yueranfly.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ysa.smart0.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://qnn.yuanzhike.top

[C14] 泛型函数
来源：http://zso.meibo888.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://the.meibo888.top

PHP:  // 无泛型
来源：http://ate.jqgfzy.top

JS:   // 无泛型
来源：http://vao.c1oappe.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://etr.zhijiandao.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://nxn.ybcxt.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://beo.pengpengdd.cyou

Ruby: # 无泛型
来源：http://phn.zhongyouzk.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://cqj.hfpthk.cn

[C15] 解构 / 展开参数
来源：http://tjm.gzhubu.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mcd.316326.xyz

PHP:  [$a, $b] = $pair;
来源：http://ury.iojbl.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://lxl.yangfankeji.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ciq.ydjk.org.cn

Java: // 无解构
来源：http://qus.bbcook.cn

Go:   // 无解构
来源：http://njy.hfpthk.cn

Ruby: a, b = pair
来源：http://nym.xingfuxueyuan.xyz

C#:   var (a, b) = pair;
来源：http://ivd.xuanzx.com

[C16] 函数 / 方法重载
来源：http://bjm.gotoacloud.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://iqh.zdqjudy.top

PHP:  // 无重载
来源：http://nje.yj20258888.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://bet.tanke756.top

TS:   // 用联合类型或重载签名声明
来源：http://yxe.cucudq.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://jxh.sysykeji.top

Go:   // 无重载：用不同函数名
来源：http://nqm.jlsjyb.cn

Ruby: # 无重载：靠动态参数
来源：http://afy.redwolf501.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://vrv.c1oappe.top

================================================================================
来源：http://iyu.haohaochexian.top

D. 数组 / 列表 / 集合
来源：http://rom.hammf.cn

================================================================================
来源：http://uvc.daria6918.cn

[D01] 创建数组 / 列表
来源：http://cbu.ydzc1.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://eeo.smart0.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://xpm.ydzc1.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://vvx.sufxvd.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://afy.ppjwa.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://xdm.zhijiandao.cn

Go:   arr := []int{1, 2, 3}
来源：http://byx.hnqzz.top

Ruby: arr = [1, 2, 3]
来源：http://jfv.hcnkem.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://vco.gotoacloud.top

[D02] 追加元素到末尾
来源：http://qxm.bbcook.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://lkh.bjfxy.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://guo.yvedp.cn

JS:   arr.push(4);
来源：http://gjy.hfpthk.cn

TS:   arr.push(4);
来源：http://ziq.hysaishi.cn

Java: list.add(4);
来源：http://dtr.yfazqb.com

Go:   arr = append(arr, 4)
来源：http://gly.zhoulong.xyz

Ruby: arr << 4; arr.push(5)
来源：http://ntk.iojbl.cn

C#:   list.Add(4);
来源：http://ztn.hongshengwenyu.top

[D03] 在指定位置插入元素
来源：http://wyh.vqdsnc.cn

Py:   arr.insert(0, 0)
来源：http://cup.sweek.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://gge.chenzaomai.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://eov.gogol.net.cn

TS:   arr.splice(0, 0, 0);
来源：http://fjo.cucudq.cn

Java: list.add(0, 0);
来源：http://rzw.hesvh.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ter.aibaodan.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://vkp.dianchejie.cn

C#:   list.Insert(0, 0);
来源：http://szr.shangyingyoupin.top

[D04] 删除元素
来源：http://cvq.yj202588.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://pvo.gaohongyu789.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://cuy.dashuyun.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://axm.aizwys.cn

TS:   arr.splice(0, 1);
来源：http://ooa.hongshengwenyu.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://xby.aibaodan.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://uyz.gogol.net.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://xws.sxryk.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://woc.cheryme.top

[D05] 访问与修改元素
来源：http://cpb.chenlongwang.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://gag.cucudq.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://quc.nwbrower.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ebg.ydjk.org.cn

TS:   arr[0]; arr.at(-1);
来源：http://vfc.shzxlz.cn

Java: list.get(0); list.set(0, 9);
来源：http://mls.gzhubu.top

Go:   arr[0]; arr[0] = 9
来源：http://nov.zycfv.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://dgp.birdmap.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://kel.fehbvm.com

[D06] 数组长度
来源：http://vcb.9152youxi.cn

Py:   len(arr)
来源：http://kth.cqqwz.cn

PHP:  count($arr);
来源：http://yyq.sweek.top

JS:   arr.length
来源：http://vnh.fktsv.cn

TS:   arr.length
来源：http://cva.pycfn.com

Java: list.size();
来源：http://crp.daria6918.cn

Go:   len(arr)
来源：http://ynq.zhengqikj.top

Ruby: arr.length; arr.size
来源：http://yro.quarkkingdee.top

C#:   list.Count;
来源：http://sww.chenzaomai.com

[D07] 切片 / 取子数组
来源：http://mqz.vehdjk.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://eij.0kj1m.cn

PHP:  array_slice($arr, 1, 3);
来源：http://dgn.tarul.cn

JS:   arr.slice(1, 4);
来源：http://cwj.fanxiaobao.xyz

TS:   arr.slice(1, 4);
来源：http://ilq.andypj.xyz

Java: list.subList(1, 4);
来源：http://vuz.nanxuanxn.top

Go:   arr[1:4]
来源：http://fog.fktsv.cn

Ruby: arr[1, 3]
来源：http://okt.kuanghao11.cn

C#:   list.GetRange(1, 3);
来源：http://rnw.guannengcc.top

[D08] 合并两个数组
来源：http://wsj.yuxming.cn

Py:   a + b;  a.extend(b)
来源：http://ags.jianghu66.top

PHP:  array_merge($a, $b);
来源：http://ohn.zycfv.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://wlf.bjfxy.top

TS:   [...a, ...b];
来源：http://kxn.shanyushiyangtech.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ilo.daria6918.cn

Go:   append(a, b...)
来源：http://gjm.pycfn.com


<!-- 参考信息 -->