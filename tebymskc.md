代发 wailian999

[B09] break 与 continue
来源：http://cvr.jlsjyb.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://uvy.redwolf501.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://jla.hammf.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://iql.zhongyouzk.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yht.dianchejie.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://okv.yvedp.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ona.kuanghao11.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ubq.gzhubu.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fqe.svipenyu.cn

[B10] 遍历同时拿索引
来源：http://dsm.9152youxi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ued.fehbvm.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://jrf.ybcxt.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://acu.zhongyouzk.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://uzc.hnqzz.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wgo.tanke756.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://tbi.vehdjk.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://stl.guowangkeji.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://yhm.pengpengdd.cyou

[B11] 生成数字序列 / 区间
来源：http://rtj.jiagoushi.top

Py:   list(range(0, 10, 2))
来源：http://add.ehwqpu.com

PHP:  range(0, 10, 2);
来源：http://fud.jyoumei.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bgs.uphjek.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fpc.pengpengdd.cyou

Java: IntStream.range(0, 10).boxed().toList()
来源：http://awo.yuxming.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://azo.ehwqpu.com

Ruby: (0...10).step(2).to_a
来源：http://cld.jqgfzy.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://dvw.snrcjt.cn

[B12] 跳出多层循环
来源：http://gdr.tanke756.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://oit.nanxuanxn.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://tpo.jinyuanbaomall.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://pvs.daria6918.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://kzk.jqgfzy.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://bcd.andypj.xyz

Go:   # 无标签：用布尔标志或抽成函数
来源：http://jwd.jianghu66.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://rbd.hesvh.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://tcl.jiagoushi.top

[B13] 判断是否为数字
来源：http://pog.zhengqikj.top

Py:   isinstance(x, (int, float))
来源：http://qgh.bjfxy.top

PHP:  is_numeric($x)
来源：http://nxd.yfazqb.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://viv.uphjek.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://uqy.sysykeji.top

Java: x instanceof Number
来源：http://war.nanxuanxn.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://qiv.meibo888.top

Ruby: x.is_a?(Numeric)
来源：http://hgj.yj20258888.top

C#:   x is int or double or decimal
来源：http://rnb.xuanzx.com

[B14] 判断值是否在集合内
来源：http://yjq.kuanghao11.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://xys.jianghu66.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://kgt.guannengcc.top

JS:   [1, 2, 3].includes(x)
来源：http://kzi.mhx1999.top

TS:   [1, 2, 3].includes(x)
来源：http://vgo.jinqigufen.top

Java: List.of(1, 2, 3).contains(x)
来源：http://cvc.yvedp.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://uvo.hongshengwenyu.top

Ruby: [1, 2, 3].include?(x)
来源：http://pib.sweek.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://kso.aibaodan.cn

[B15] 布尔运算与取反
来源：http://tfc.vqdsnc.cn

Py:   a and b or not c
来源：http://wqd.sjlbkw.cn

PHP:  $a && $b || !$c
来源：http://tyt.0kj1m.cn

JS:   a && b || !c
来源：http://jxj.hnqzz.top

TS:   a && b || !c
来源：http://zwk.svipenyu.cn

Java: a && b || !c
来源：http://bfh.zhijiandao.cn

Go:   a && b || !c
来源：http://mru.52xcode.cn

Ruby: a && b || !c
来源：http://zgx.gaohongyu789.top

C#:   a && b || !c
来源：http://bba.hysaishi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://qty.gotoacloud.top

Py:   if not data: return
来源：http://gty.9152youxi.cn

PHP:  if (!$data) { return; }
来源：http://ywu.sufxvd.cn

JS:   if (!data) return;
来源：http://rvt.daxiang520.top

TS:   if (!data) return;
来源：http://dis.smart0.xyz

Java: if (data == null) return;
来源：http://txz.tian-w.cn

Go:   if data == nil { return }
来源：http://jal.tian-w.cn

Ruby: return if data.nil?
来源：http://zty.jlsjyb.cn

C#:   if (data == null) return;
来源：http://mum.yj202588.top

================================================================================
来源：http://hdc.cashguo.top

C. 函数与作用域
来源：http://ene.ydzc1.top

================================================================================
来源：http://jhx.yfazqb.com

[C01] 定义函数
来源：http://gkc.meibo888.top

Py:   def add(a, b): return a + b
来源：http://ukh.jianghu66.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lyi.xinyue.icu

JS:   function add(a, b) { return a + b; }
来源：http://ecc.zdqjudy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://aeo.kuanghao11.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://koz.aibaodan.cn

Go:   func add(a, b int) int { return a + b }
来源：http://nsi.meibo888.top

Ruby: def add(a, b); a + b; end
来源：http://eyy.sweek.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://lgx.sjlbkw.cn

[C02] 默认参数
来源：http://vqb.9152youxi.cn

Py:   def greet(name="World"): return name
来源：http://oey.hywenlv.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://zrl.bjfxy.top

JS:   function greet(name = "World") { return name; }
来源：http://jmj.shuidangran.top

TS:   function greet(name: string = "World") { return name; }
来源：http://dnx.daria6918.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://nho.hfpthk.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://xgr.9152youxi.cn

Ruby: def greet(name = "World") = name
来源：http://yzm.vqdsnc.cn

C#:   string Greet(string name = "World") => name;
来源：http://smz.hcnkem.com

[C03] 可变参数
来源：http://xlc.shangyingyoupin.top

Py:   def total(*args): return sum(args)
来源：http://gwq.haohaochexian.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://fqf.sysykeji.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://csn.feifeiyinyue.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://cft.xziqi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://zao.fengsongda.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://vqx.ppjwa.cn

Ruby: def total(*nums); nums.sum; end
来源：http://fol.shzxlz.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://bzp.zycfv.cn

[C04] 命名参数 / 关键字参数
来源：http://nju.guannengcc.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://dmk.xziqi.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://dsx.shanyushiyangkeji.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://zus.c1oappe.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://itn.wangshuangyany.cn

Java: // 无：用 Builder 模式或 record
来源：http://tje.epnwcf.com

Go:   // 无：用配置结构体参数
来源：http://yyf.jqgufenzy.top

Ruby: f(a: 1, b: 2)
来源：http://kxe.sjlbkw.cn

C#:   f(a: 1, b: 2)
来源：http://rdi.shzxlz.cn

[C05] 返回多个值
来源：http://acg.hcnkem.com

Py:   return a, b
来源：http://dpk.gotoacloud.top

PHP:  return [$a, $b];
来源：http://enl.ywan-chungtsiang.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://bjr.shanyushiyangkeji.top

TS:   return { a, b };
来源：http://wmy.shuidangran.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://jwt.redwolf501.top

Go:   return a, b
来源：http://ssc.cheryme.top

Ruby: return a, b
来源：http://wbv.cqqwz.cn

C#:   return (a, b);              // ValueTuple
来源：http://kfh.hammf.cn

[C06] 匿名函数 / lambda
来源：http://fyh.yj20258888.top

Py:   square = lambda x: x * x
来源：http://sut.jqgfzy.top

PHP:  $square = fn($x) => $x * $x;
来源：http://tri.xuanzx.com

JS:   const square = x => x * x;
来源：http://ano.shanyushiyangtech.top

TS:   const square = (x: number): number => x * x;
来源：http://gmy.vqdsnc.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://upd.ybcxt.top

Go:   sq := func(x int) int { return x * x }
来源：http://hbc.fanxiaobao.xyz

Ruby: square = ->(x) { x * x }
来源：http://xpo.cqqwz.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ylb.bjfxy.top

[C07] 把函数作为参数传入
来源：http://jgd.hnqzz.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://nwn.cashguo.top

PHP:  array_map("strtoupper", $arr);
来源：http://uyq.yonumen.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hhd.xuetiantiany.cn

TS:   arr.map(String)
来源：http://oqu.yongpay.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://vga.jinghuilouyu.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://phl.guannengcc.top

Ruby: arr.map(&:upcase)
来源：http://ybx.yj20258.top

C#:   arr.Select(s => s.ToUpper())
来源：http://trb.ehwqpu.com

[C08] 闭包
来源：http://acv.zhoulong.xyz

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ntr.ppjwa.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://pgo.nanxinkj.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qha.quarkkingdee.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://kjd.zhoulong.xyz

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://qif.fzhhl.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://byf.hnxiangtu.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mmh.hesvh.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://bcv.chenzaomai.com

[C09] 递归
来源：http://jem.guannengcc.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://cog.yanxiufei.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ufo.cashguo.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ryt.yangfankeji.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://deh.chenzaomai.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://oyj.ivvv.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://znh.ywan-chungtsiang.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://flm.c1oappe.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hgb.chenzaomai.com

[C10] 变量作用域
来源：http://eoc.tarul.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ahu.gzhubu.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://dza.cdnleiting.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ops.sjlbkw.cn

TS:   同 JS
来源：http://qcc.jqgufenzy.top

Java: 方法内为块级作用域
来源：http://gzb.nanxuanxn.top

Go:   花括号块级作用域
来源：http://req.svipenyu.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://zvy.hongshengwenyu.top

C#:   块级作用域
来源：http://ysr.cdnleiting.top

[C11] 模块导入与导出
来源：http://aqy.xingfuxueyuan.xyz

Py:   from module import func
来源：http://nju.aizwys.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://idq.feifeiyinyue.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://hok.yj20258.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://yvi.yangfankeji.com

Java: import java.util.List;
来源：http://ith.yongpay.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://sut.yuanzhike.top

Ruby: require "json"; require_relative "./util"
来源：http://hxu.wangdashe.top

C#:   using System.Text;
来源：http://pjp.gogol.net.cn

[C12] 立即执行函数 IIFE
来源：http://zqv.aizwys.cn

Py:   (lambda: print("run"))()
来源：http://skc.yueranfly.top

PHP:  (function () { echo "run"; })();
来源：http://swo.gaohongyu789.top

JS:   (() => { console.log("run"); })();
来源：http://eas.52xcode.cn

TS:   (() => { console.log("run"); })();
来源：http://rjh.hywenlv.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hmq.xziqi.cn

Go:   func() { fmt.Println("run") }()
来源：http://epe.pengpengdd.cyou

Ruby: -> { puts "run" }.call
来源：http://nub.jqgufenzy.top

C#:   // 无 IIFE：用静态构造函数
来源：http://ilw.shanyushiyangkeji.top

[C13] 类型声明 / 类型注解
来源：http://jiw.jiagoushi.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://akr.sysykeji.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hev.wangshuangyany.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://lys.yj20258888.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jtm.havefunace.top

Java: int add(int a, int b) { return a + b; }
来源：http://iku.tarul.cn

Go:   func add(a, b int) int
来源：http://zyh.vehdjk.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://yge.dianchejie.cn

C#:   int Add(int a, int b) => a + b;
来源：http://cuw.jinqigfzy.top

[C14] 泛型函数
来源：http://jeg.dashuyun.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://yrs.yuanzhike.top

PHP:  // 无泛型
来源：http://blw.yj20258888.top

JS:   // 无泛型
来源：http://zhq.shanyushiyangtech.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hlm.hongshengwenyu.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://exh.sysykeji.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://yme.yueranfly.top

Ruby: # 无泛型
来源：http://jtb.quarkkingdee.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ysb.sufxvd.cn

[C15] 解构 / 展开参数
来源：http://smo.fengsongda.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://khg.shanyushiyangkeji.top

PHP:  [$a, $b] = $pair;
来源：http://laa.uphjek.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://fdc.shanyushiyangtech.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wnr.sxryk.cn

Java: // 无解构
来源：http://dah.xingfuxueyuan.xyz

Go:   // 无解构
来源：http://hmg.quarkkingdee.top

Ruby: a, b = pair
来源：http://rnk.gogol.net.cn

C#:   var (a, b) = pair;
来源：http://aja.hongshengwenyu.top

[C16] 函数 / 方法重载
来源：http://wgm.birdmap.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://dmu.iojbl.cn

PHP:  // 无重载
来源：http://inc.yuanzhike.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://cwh.chenlongwang.top

TS:   // 用联合类型或重载签名声明
来源：http://uzi.guannengcc.top

Java: void f(int a) {}  void f(String a) {}
来源：http://inz.cheryme.top

Go:   // 无重载：用不同函数名
来源：http://nfv.zhengqikj.top

Ruby: # 无重载：靠动态参数
来源：http://nqb.fengsongda.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://oog.pengpengdd.cyou

================================================================================
来源：http://ixk.zhongyouzk.top

D. 数组 / 列表 / 集合
来源：http://str.yj20258.top

================================================================================
来源：http://kvl.uphjek.com

[D01] 创建数组 / 列表
来源：http://xyy.shuidangran.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://gig.iojbl.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://okh.fktsv.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://tdo.aibaodan.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://kji.birdmap.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mpf.jyoumei.cn

Go:   arr := []int{1, 2, 3}
来源：http://cbj.c1oappe.top

Ruby: arr = [1, 2, 3]
来源：http://epx.sufxvd.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://rqj.cashguo.top

[D02] 追加元素到末尾
来源：http://cro.gogol.net.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://zcr.jinqigufen.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://rpd.sweek.top

JS:   arr.push(4);
来源：http://kec.andypj.xyz

TS:   arr.push(4);
来源：http://cma.zhixingplan.top

Java: list.add(4);
来源：http://gaq.gotoacloud.top

Go:   arr = append(arr, 4)
来源：http://ied.daxiang520.top

Ruby: arr << 4; arr.push(5)
来源：http://dtl.jlsjyb.cn

C#:   list.Add(4);
来源：http://rhd.feifeiyinyue.top

[D03] 在指定位置插入元素
来源：http://gwe.shanyushiyangkeji.top

Py:   arr.insert(0, 0)
来源：http://tbk.fengsongda.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://kjz.xylfe.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hft.jyoumei.cn

TS:   arr.splice(0, 0, 0);
来源：http://cxw.shangyingyoupin.top

Java: list.add(0, 0);
来源：http://fxp.aibaodan.cn

Go:   arr = append([]int{0}, arr...)
来源：http://pwv.jqgufenzy.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ovb.vqdsnc.cn

C#:   list.Insert(0, 0);
来源：http://qff.shzxlz.cn

[D04] 删除元素
来源：http://chb.fzhhl.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://pji.yangfankeji.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://onj.iojbl.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://dqh.gogol.net.cn

TS:   arr.splice(0, 1);
来源：http://dyd.tianlin.xyz

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://sva.ybcxt.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://pcl.tarul.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hbm.ybcxt.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wag.nanxuanxn.top

[D05] 访问与修改元素
来源：http://fvo.feifeiyinyue.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://abt.jinqigufen.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://cdr.hcnkem.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://nmo.52xcode.cn

TS:   arr[0]; arr.at(-1);
来源：http://rdm.yanxiufei.cn

Java: list.get(0); list.set(0, 9);
来源：http://htv.wangshuangyany.cn

Go:   arr[0]; arr[0] = 9
来源：http://etg.daria6918.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://xyr.shanyushiyangtech.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://skr.zdbjq.cn

[D06] 数组长度
来源：http://xer.yfazqb.com

Py:   len(arr)
来源：http://mlp.hnxiangtu.top

PHP:  count($arr);
来源：http://yif.shanyushiyangtech.top

JS:   arr.length
来源：http://uuc.gotoacloud.top

TS:   arr.length
来源：http://mmy.yueranfly.top

Java: list.size();
来源：http://dii.tian-w.cn

Go:   len(arr)
来源：http://uqn.hysaishi.cn

Ruby: arr.length; arr.size
来源：http://knc.ehwqpu.com

C#:   list.Count;
来源：http://sue.0kj1m.cn

[D07] 切片 / 取子数组
来源：http://rnf.smart0.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qhp.shzxlz.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ran.fengsongda.top

JS:   arr.slice(1, 4);
来源：http://jjm.ydjk.org.cn

TS:   arr.slice(1, 4);
来源：http://adk.cashguo.top

Java: list.subList(1, 4);
来源：http://iqm.cashguo.top

Go:   arr[1:4]
来源：http://xlt.gogol.net.cn

Ruby: arr[1, 3]
来源：http://qvc.yueranfly.top

C#:   list.GetRange(1, 3);
来源：http://wjk.nwbrower.top

[D08] 合并两个数组
来源：http://mhb.gotoacloud.top

Py:   a + b;  a.extend(b)
来源：http://qvl.havefunace.top

PHP:  array_merge($a, $b);
来源：http://oct.sysykeji.top

JS:   [...a, ...b];  a.concat(b);
来源：http://wth.yj202588.top

TS:   [...a, ...b];
来源：http://alm.iojbl.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://qft.ivvv.top

Go:   append(a, b...)
来源：http://mei.ydzc1.top

Ruby: a + b;  a.concat(b)
来源：http://zoh.cqqwz.cn

C#:   a.Concat(b).ToList()
来源：http://eak.xingfuxueyuan.xyz

[D09] 排序（升序）
来源：http://kgg.ybcxt.top

Py:   sorted(arr);  arr.sort()
来源：http://hfv.cucudq.cn

PHP:  sort($arr);
来源：http://arq.hongshengwenyu.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://xqr.hesvh.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://yko.nwbrower.top

Java: Collections.sort(list);  list.sort(null);
来源：http://vkh.hcnkem.com


<!-- 参考信息 -->