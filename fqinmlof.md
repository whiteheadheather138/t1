代发 wailian999

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://yqr.c1oappe.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://aqn.fanxiaobao.xyz

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://gpz.redwolf501.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hvq.ydjk.org.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://muo.xuanzx.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://tik.jqgfzy.top

[B11] 生成数字序列 / 区间
来源：http://pli.kuanghao11.cn

Py:   list(range(0, 10, 2))
来源：http://gmv.nanxuanxn.top

PHP:  range(0, 10, 2);
来源：http://sop.jiagoushi.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hnc.sufxvd.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://erw.fzhhl.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://awt.tarul.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ylj.zycfv.cn

Ruby: (0...10).step(2).to_a
来源：http://grw.zhaomingkeji.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://uft.vehdjk.com

[B12] 跳出多层循环
来源：http://hib.gaohongyu789.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://mhq.haohaochexian.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://fls.sweek.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://zxy.snrcjt.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://dwv.bjfxy.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://bfs.yj20258888.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://dso.0kj1m.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://gch.snrcjt.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://gqj.yj20258888.top

[B13] 判断是否为数字
来源：http://ncg.0kj1m.cn

Py:   isinstance(x, (int, float))
来源：http://tks.xziqi.cn

PHP:  is_numeric($x)
来源：http://vlz.zhengqikj.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://epi.fengsongda.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dad.zdqjudy.top

Java: x instanceof Number
来源：http://txv.316326.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://jzc.zhiwuduotai.top

Ruby: x.is_a?(Numeric)
来源：http://mfq.jinqigfzy.top

C#:   x is int or double or decimal
来源：http://tcp.yanxiufei.cn

[B14] 判断值是否在集合内
来源：http://rlo.jlsjyb.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://zfk.zhoulong.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wbz.ppjwa.cn

JS:   [1, 2, 3].includes(x)
来源：http://ltk.fktsv.cn

TS:   [1, 2, 3].includes(x)
来源：http://wre.iojbl.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://wif.fktsv.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://rjo.hcnkem.com

Ruby: [1, 2, 3].include?(x)
来源：http://qfc.hywenlv.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://xet.yueranfly.top

[B15] 布尔运算与取反
来源：http://suq.jqgufenzy.top

Py:   a and b or not c
来源：http://uow.tianlin.xyz

PHP:  $a && $b || !$c
来源：http://eez.shanyushiyangkeji.top

JS:   a && b || !c
来源：http://ali.hammf.cn

TS:   a && b || !c
来源：http://yhe.yangfankeji.com

Java: a && b || !c
来源：http://zms.meibo888.top

Go:   a && b || !c
来源：http://tbk.xuetiantiany.cn

Ruby: a && b || !c
来源：http://wue.jqgufenzy.top

C#:   a && b || !c
来源：http://qku.0kj1m.cn

[B16] 卫语句：不满足条件提前返回
来源：http://bnw.jinyuanbaomall.cn

Py:   if not data: return
来源：http://epj.nwbrower.top

PHP:  if (!$data) { return; }
来源：http://bid.shuidangran.top

JS:   if (!data) return;
来源：http://dun.gaohongyu789.top

TS:   if (!data) return;
来源：http://fdg.gzhubu.top

Java: if (data == null) return;
来源：http://bwu.fengsongda.top

Go:   if data == nil { return }
来源：http://put.nanxinkj.top

Ruby: return if data.nil?
来源：http://uhs.nwbrower.top

C#:   if (data == null) return;
来源：http://fgt.cucudq.cn

================================================================================
来源：http://wfc.mhx1999.top

C. 函数与作用域
来源：http://zok.yongpay.top

================================================================================
来源：http://aml.nanxuanxn.top

[C01] 定义函数
来源：http://egj.yj20258888.top

Py:   def add(a, b): return a + b
来源：http://est.daria6918.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pyr.ybcxt.top

JS:   function add(a, b) { return a + b; }
来源：http://map.hongshengwenyu.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://soi.bbcook.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://gcq.yj20258.top

Go:   func add(a, b int) int { return a + b }
来源：http://crn.feifeiyinyue.top

Ruby: def add(a, b); a + b; end
来源：http://rkz.fzhhl.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://eha.fanxiaobao.xyz

[C02] 默认参数
来源：http://blz.hnqzz.top

Py:   def greet(name="World"): return name
来源：http://fnh.ydzc1.top

PHP:  function greet($name = "World") { return $name; }
来源：http://xiu.yuanzhike.top

JS:   function greet(name = "World") { return name; }
来源：http://lkc.daria6918.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://rly.tian-w.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://pkv.yj20258.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://tnt.jinghuilouyu.cn

Ruby: def greet(name = "World") = name
来源：http://ios.cqqwz.cn

C#:   string Greet(string name = "World") => name;
来源：http://wkg.yongpay.top

[C03] 可变参数
来源：http://fib.hnxiangtu.top

Py:   def total(*args): return sum(args)
来源：http://dhz.zdqjudy.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://pjp.xingfuxueyuan.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://atb.yj20258.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ayv.chenjidiqi.icu

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://zjj.zdqjudy.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://bcg.sufxvd.cn

Ruby: def total(*nums); nums.sum; end
来源：http://jbb.vehdjk.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zur.chenlongwang.top

[C04] 命名参数 / 关键字参数
来源：http://ngz.chenzaomai.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://vpf.mhx1999.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://nuc.andypj.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://swb.yfazqb.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ijg.ydjk.org.cn

Java: // 无：用 Builder 模式或 record
来源：http://lys.jlsjyb.cn

Go:   // 无：用配置结构体参数
来源：http://cja.jqgfzy.top

Ruby: f(a: 1, b: 2)
来源：http://gtk.tian-w.cn

C#:   f(a: 1, b: 2)
来源：http://rrm.jinghuilouyu.cn

[C05] 返回多个值
来源：http://lel.ywan-chungtsiang.top

Py:   return a, b
来源：http://dph.hongshengwenyu.top

PHP:  return [$a, $b];
来源：http://ehy.guowangkeji.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://xup.havefunace.top

TS:   return { a, b };
来源：http://kbx.c1oappe.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ivf.0kj1m.cn

Go:   return a, b
来源：http://ees.yvedp.cn

Ruby: return a, b
来源：http://obg.sjlbkw.cn

C#:   return (a, b);              // ValueTuple
来源：http://cyk.jlsjyb.cn

[C06] 匿名函数 / lambda
来源：http://ksw.yfazqb.com

Py:   square = lambda x: x * x
来源：http://box.feifeiyinyue.top

PHP:  $square = fn($x) => $x * $x;
来源：http://sjc.9152youxi.cn

JS:   const square = x => x * x;
来源：http://dyw.wangdashe.top

TS:   const square = (x: number): number => x * x;
来源：http://pcw.svipenyu.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hqg.yj20258.top

Go:   sq := func(x int) int { return x * x }
来源：http://kin.cdnleiting.top

Ruby: square = ->(x) { x * x }
来源：http://qvy.jinghuilouyu.cn

C#:   Func<int, int> square = x => x * x;
来源：http://itq.zhongyouzk.top

[C07] 把函数作为参数传入
来源：http://zbw.sxryk.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://xri.hysaishi.cn

PHP:  array_map("strtoupper", $arr);
来源：http://wtn.pycfn.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://sxm.guowangkeji.top

TS:   arr.map(String)
来源：http://jwg.tianlin.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://lhh.feifeiyinyue.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://tbc.shuidangran.top

Ruby: arr.map(&:upcase)
来源：http://nyf.jinghuilouyu.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ezu.chenlongwang.top

[C08] 闭包
来源：http://mgc.tian-w.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://gph.jiagoushi.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://eve.guannengcc.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hza.ppjwa.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://yyb.yvedp.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ieb.ywan-chungtsiang.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://lhq.gzhubu.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://bqf.chenlongwang.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://gix.zhoulong.xyz

[C09] 递归
来源：http://fyz.chenjidiqi.icu

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://xef.yj20258.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://luf.fanxiaobao.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lcw.guannengcc.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sei.pycfn.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wlb.xinyue.icu

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://fqd.smart0.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://lfs.zdbjq.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://nsb.mhx1999.top

[C10] 变量作用域
来源：http://ekn.fengsongda.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://fdr.yanxiufei.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://gfw.vqdsnc.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://fdm.hcnkem.com

TS:   同 JS
来源：http://bqg.ywan-chungtsiang.top

Java: 方法内为块级作用域
来源：http://grp.sxryk.cn

Go:   花括号块级作用域
来源：http://yqi.cdnleiting.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://yda.gaohongyu789.top

C#:   块级作用域
来源：http://luq.aizwys.cn

[C11] 模块导入与导出
来源：http://mlh.zhiwuduotai.top

Py:   from module import func
来源：http://qzm.ivvv.top

PHP:  require "file.php";  或 use App\Service;
来源：http://glk.gotoacloud.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://hwx.nwbrower.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://qtt.bjfxy.top

Java: import java.util.List;
来源：http://vex.snrcjt.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://fjg.zdqjudy.top

Ruby: require "json"; require_relative "./util"
来源：http://dtq.ybcxt.top

C#:   using System.Text;
来源：http://hhl.ctjpmb.com

[C12] 立即执行函数 IIFE
来源：http://ekc.yfazqb.com

Py:   (lambda: print("run"))()
来源：http://iaf.jianghu66.top

PHP:  (function () { echo "run"; })();
来源：http://oki.yanxiufei.cn

JS:   (() => { console.log("run"); })();
来源：http://xbq.ppjwa.cn

TS:   (() => { console.log("run"); })();
来源：http://czl.gogol.net.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://tbm.pengpengdd.cyou

Go:   func() { fmt.Println("run") }()
来源：http://gqe.jlsjyb.cn

Ruby: -> { puts "run" }.call
来源：http://kye.vehdjk.com

C#:   // 无 IIFE：用静态构造函数
来源：http://bbs.epnwcf.com

[C13] 类型声明 / 类型注解
来源：http://lrg.aizwys.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://fiv.vqdsnc.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://moc.hammf.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ykk.ywan-chungtsiang.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ckx.sweek.top

Java: int add(int a, int b) { return a + b; }
来源：http://sje.aizwys.cn

Go:   func add(a, b int) int
来源：http://nzv.havefunace.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://zzl.guannengcc.top

C#:   int Add(int a, int b) => a + b;
来源：http://neg.tianlin.xyz

[C14] 泛型函数
来源：http://rpc.svipenyu.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://grs.hammf.cn

PHP:  // 无泛型
来源：http://gyb.zdbjq.cn

JS:   // 无泛型
来源：http://qti.xingfuxueyuan.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://msp.fktsv.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://lyl.shanyushiyangtech.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ugn.yfazqb.com

Ruby: # 无泛型
来源：http://nqh.bbcook.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://vdx.hfpthk.cn

[C15] 解构 / 展开参数
来源：http://ioo.svipenyu.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://fkf.jyoumei.cn

PHP:  [$a, $b] = $pair;
来源：http://aft.fehbvm.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ggk.aibaodan.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ekg.yj20258.top

Java: // 无解构
来源：http://iqe.hammf.cn

Go:   // 无解构
来源：http://eak.guowangkeji.top

Ruby: a, b = pair
来源：http://csj.shzxlz.cn

C#:   var (a, b) = pair;
来源：http://cmc.yj202588.top

[C16] 函数 / 方法重载
来源：http://jdb.ydjk.org.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://rtd.ehwqpu.com

PHP:  // 无重载
来源：http://pnh.ydzc1.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://axw.yfazqb.com

TS:   // 用联合类型或重载签名声明
来源：http://sgz.jinqigfzy.top

Java: void f(int a) {}  void f(String a) {}
来源：http://anl.dianchejie.cn

Go:   // 无重载：用不同函数名
来源：http://ndg.hnqzz.top

Ruby: # 无重载：靠动态参数
来源：http://ava.9152youxi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://nii.hysaishi.cn

================================================================================
来源：http://ecz.birdmap.top

D. 数组 / 列表 / 集合
来源：http://fuq.chenjidiqi.icu

================================================================================
来源：http://ftc.yuanzhike.top

[D01] 创建数组 / 列表
来源：http://whg.mhx1999.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://cng.shanyushiyangkeji.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://cpa.yj202588.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://urf.zhoulong.xyz

TS:   const arr: number[] = [1, 2, 3];
来源：http://vlo.hfpthk.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mpr.gotoacloud.top

Go:   arr := []int{1, 2, 3}
来源：http://ekl.ctjpmb.com

Ruby: arr = [1, 2, 3]
来源：http://dpv.ctjpmb.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://yrm.hcnkem.com

[D02] 追加元素到末尾
来源：http://vjg.zhongyouzk.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://xvm.hysaishi.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://oyp.yonumen.top

JS:   arr.push(4);
来源：http://gno.tian-w.cn

TS:   arr.push(4);
来源：http://zui.fanxiaobao.xyz

Java: list.add(4);
来源：http://xti.zycfv.cn

Go:   arr = append(arr, 4)
来源：http://txe.chenzaomai.com

Ruby: arr << 4; arr.push(5)
来源：http://zel.feifeiyinyue.top

C#:   list.Add(4);
来源：http://ihb.9152youxi.cn

[D03] 在指定位置插入元素
来源：http://fsh.daria6918.cn

Py:   arr.insert(0, 0)
来源：http://rfo.gogol.net.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://clf.sjlbkw.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://lkf.sweek.top

TS:   arr.splice(0, 0, 0);
来源：http://tlb.tanke756.top

Java: list.add(0, 0);
来源：http://mjy.yuanzhike.top

Go:   arr = append([]int{0}, arr...)
来源：http://uwd.quarkkingdee.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mfl.yj20258888.top

C#:   list.Insert(0, 0);
来源：http://szm.yfazqb.com

[D04] 删除元素
来源：http://iyf.xinyue.icu

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://bge.zhijiandao.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://bly.ydzc1.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://klp.hysaishi.cn

TS:   arr.splice(0, 1);
来源：http://vlj.yj20258888.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.jianghu66.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://vgv.ydzc1.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://nxd.wangdashe.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://kyi.jqgufenzy.top

[D05] 访问与修改元素
来源：http://kfu.shangyingyoupin.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://fwv.hammf.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://izk.fzhhl.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://eir.fzhhl.top

TS:   arr[0]; arr.at(-1);
来源：http://ylz.jinqigfzy.top

Java: list.get(0); list.set(0, 9);
来源：http://uaa.hnxiangtu.top

Go:   arr[0]; arr[0] = 9
来源：http://hqq.mhx1999.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://yev.ivvv.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://snj.yangfankeji.com

[D06] 数组长度
来源：http://nwi.havefunace.top

Py:   len(arr)
来源：http://mlx.ehwqpu.com

PHP:  count($arr);
来源：http://bka.wangshuangyany.cn

JS:   arr.length
来源：http://rqg.pycfn.com

TS:   arr.length
来源：http://khy.jyoumei.cn

Java: list.size();
来源：http://cwg.xuanzx.com

Go:   len(arr)
来源：http://ysd.jinyuanbaomall.cn

Ruby: arr.length; arr.size
来源：http://rnm.nanxinkj.top

C#:   list.Count;
来源：http://fod.hcnkem.com

[D07] 切片 / 取子数组
来源：http://ydm.nanxuanxn.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qpw.jlsjyb.cn

PHP:  array_slice($arr, 1, 3);
来源：http://hio.bjfxy.top

JS:   arr.slice(1, 4);
来源：http://wec.hnqzz.top

TS:   arr.slice(1, 4);
来源：http://ivv.daxiang520.top

Java: list.subList(1, 4);
来源：http://git.cashguo.top

Go:   arr[1:4]
来源：http://iwr.gogol.net.cn

Ruby: arr[1, 3]
来源：http://zsu.jinyuanbaomall.cn

C#:   list.GetRange(1, 3);
来源：http://cnw.hammf.cn

[D08] 合并两个数组
来源：http://kfv.zhongyouzk.top

Py:   a + b;  a.extend(b)
来源：http://epm.tanke756.top

PHP:  array_merge($a, $b);
来源：http://rsu.guannengcc.top

JS:   [...a, ...b];  a.concat(b);
来源：http://eeq.yvedp.cn

TS:   [...a, ...b];
来源：http://pxp.ivvv.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://lvg.jinghuilouyu.cn

Go:   append(a, b...)
来源：http://rdd.shanyushiyangkeji.top

Ruby: a + b;  a.concat(b)
来源：http://jnw.kuanghao11.cn

C#:   a.Concat(b).ToList()
来源：http://gqv.haohaochexian.top

[D09] 排序（升序）
来源：http://ils.hysaishi.cn

Py:   sorted(arr);  arr.sort()
来源：http://axo.fzhhl.top

PHP:  sort($arr);
来源：http://bhw.fktsv.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://vso.hywenlv.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://rwc.andypj.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://plp.yueranfly.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://vpq.zhijiandao.cn

Ruby: arr.sort
来源：http://vwn.ywan-chungtsiang.top

C#:   list.Sort();
来源：http://ugl.mhx1999.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://kkq.smart0.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://dku.gaohongyu789.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rym.hywenlv.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wfi.ydzc1.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ftt.9152youxi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://idp.pengpengdd.cyou

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hxv.yuxming.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://qss.zdqjudy.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://dis.hnxiangtu.top


<!-- 参考信息 -->