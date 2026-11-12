代发 wailian999

[B09] break 与 continue
来源：http://ijl.jinqigfzy.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://scj.shuidangran.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blp.yueranfly.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lzf.hysaishi.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dbz.xuanzx.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rml.vqdsnc.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://qvu.daria6918.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ugf.chenjidiqi.icu

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xxv.ctjpmb.com

[B10] 遍历同时拿索引
来源：http://klo.9152youxi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ivl.jinqigfzy.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://nym.chenzaomai.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://okk.zhaomingkeji.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://yhk.xziqi.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://gst.sufxvd.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://qny.zhoulong.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wow.hesvh.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hut.jqgfzy.top

[B11] 生成数字序列 / 区间
来源：http://cmq.smart0.xyz

Py:   list(range(0, 10, 2))
来源：http://kdo.nanxuanxn.top

PHP:  range(0, 10, 2);
来源：http://tmz.sweek.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rkb.hysaishi.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vmo.snrcjt.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://sfr.hammf.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hsa.jiagoushi.top

Ruby: (0...10).step(2).to_a
来源：http://cgt.yj202588.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ybe.wangdashe.top

[B12] 跳出多层循环
来源：http://kxk.chenzaomai.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://yga.hfpthk.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://irh.ivvv.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://dvd.gogol.net.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://zsj.yj20258.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ulh.sxryk.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ebr.yj20258.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://nhl.bjfxy.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://nlt.smart0.xyz

[B13] 判断是否为数字
来源：http://oxr.cheryme.top

Py:   isinstance(x, (int, float))
来源：http://erf.ppjwa.cn

PHP:  is_numeric($x)
来源：http://fju.52xcode.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://igx.dashuyun.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nny.xingfuxueyuan.xyz

Java: x instanceof Number
来源：http://soz.sufxvd.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://yzp.redwolf501.top

Ruby: x.is_a?(Numeric)
来源：http://djy.52xcode.cn

C#:   x is int or double or decimal
来源：http://rna.epnwcf.com

[B14] 判断值是否在集合内
来源：http://vrj.sxryk.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://pgc.gotoacloud.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ofm.xuanzx.com

JS:   [1, 2, 3].includes(x)
来源：http://ste.tarul.cn

TS:   [1, 2, 3].includes(x)
来源：http://hcr.ppjwa.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://yjy.zhongyouzk.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://kmg.sufxvd.cn

Ruby: [1, 2, 3].include?(x)
来源：http://fcw.ywan-chungtsiang.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://cso.vehdjk.com

[B15] 布尔运算与取反
来源：http://cmt.zhiwuduotai.top

Py:   a and b or not c
来源：http://jcf.gzhubu.top

PHP:  $a && $b || !$c
来源：http://nmg.gzhubu.top

JS:   a && b || !c
来源：http://bqt.tanke756.top

TS:   a && b || !c
来源：http://wfz.cashguo.top

Java: a && b || !c
来源：http://yzd.ctjpmb.com

Go:   a && b || !c
来源：http://qbv.jianghu66.top

Ruby: a && b || !c
来源：http://osl.zdbjq.cn

C#:   a && b || !c
来源：http://szz.shzxlz.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ith.fanxiaobao.xyz

Py:   if not data: return
来源：http://cgc.yj20258.top

PHP:  if (!$data) { return; }
来源：http://pbu.fzhhl.top

JS:   if (!data) return;
来源：http://ajj.mhx1999.top

TS:   if (!data) return;
来源：http://qgh.shangyingyoupin.top

Java: if (data == null) return;
来源：http://hli.gogol.net.cn

Go:   if data == nil { return }
来源：http://huy.mhx1999.top

Ruby: return if data.nil?
来源：http://dad.tian-w.cn

C#:   if (data == null) return;
来源：http://ftx.zdqjudy.top

================================================================================
来源：http://jme.ivvv.top

C. 函数与作用域
来源：http://ktu.redwolf501.top

================================================================================
来源：http://egq.jqgfzy.top

[C01] 定义函数
来源：http://tig.havefunace.top

Py:   def add(a, b): return a + b
来源：http://jmp.smart0.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nqs.epnwcf.com

JS:   function add(a, b) { return a + b; }
来源：http://kdg.fehbvm.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bog.yj202588.top

Java: static int add(int a, int b) { return a + b; }
来源：http://nlv.jqgfzy.top

Go:   func add(a, b int) int { return a + b }
来源：http://kvl.ehwqpu.com

Ruby: def add(a, b); a + b; end
来源：http://pmx.fanxiaobao.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://fij.zhixingplan.top

[C02] 默认参数
来源：http://tky.shangyingyoupin.top

Py:   def greet(name="World"): return name
来源：http://xdp.zhaomingkeji.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://pjo.xuetiantiany.cn

JS:   function greet(name = "World") { return name; }
来源：http://oxe.hfpthk.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://hnr.hesvh.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://psc.jyoumei.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mqx.ivvv.top

Ruby: def greet(name = "World") = name
来源：http://zvh.jianghu66.top

C#:   string Greet(string name = "World") => name;
来源：http://ayj.daria6918.cn

[C03] 可变参数
来源：http://itl.meibo888.top

Py:   def total(*args): return sum(args)
来源：http://rxa.wangshuangyany.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ofj.feifeiyinyue.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ppv.yueranfly.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://bil.bjfxy.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ybi.svipenyu.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://yvz.nanxinkj.top

Ruby: def total(*nums); nums.sum; end
来源：http://dvq.hnqzz.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://yky.cheryme.top

[C04] 命名参数 / 关键字参数
来源：http://kty.zdbjq.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hqz.mhx1999.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://jpt.vehdjk.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://euj.fehbvm.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://jvs.ydjk.org.cn

Java: // 无：用 Builder 模式或 record
来源：http://ihr.zhixingplan.top

Go:   // 无：用配置结构体参数
来源：http://jfd.kuanghao11.cn

Ruby: f(a: 1, b: 2)
来源：http://qck.hesvh.cn

C#:   f(a: 1, b: 2)
来源：http://ppv.xziqi.cn

[C05] 返回多个值
来源：http://mpl.daxiang520.top

Py:   return a, b
来源：http://twk.guowangkeji.top

PHP:  return [$a, $b];
来源：http://ail.cashguo.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://phd.jiagoushi.top

TS:   return { a, b };
来源：http://hck.yuanzhike.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mol.daxiang520.top

Go:   return a, b
来源：http://jlj.yuxming.cn

Ruby: return a, b
来源：http://saz.yvedp.cn

C#:   return (a, b);              // ValueTuple
来源：http://kve.tarul.cn

[C06] 匿名函数 / lambda
来源：http://mvp.cheryme.top

Py:   square = lambda x: x * x
来源：http://noe.guannengcc.top

PHP:  $square = fn($x) => $x * $x;
来源：http://rbl.nanxuanxn.top

JS:   const square = x => x * x;
来源：http://vsz.nanxuanxn.top

TS:   const square = (x: number): number => x * x;
来源：http://wvq.iojbl.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://gro.hcnkem.com

Go:   sq := func(x int) int { return x * x }
来源：http://dmn.shzxlz.cn

Ruby: square = ->(x) { x * x }
来源：http://zin.xylfe.cn

C#:   Func<int, int> square = x => x * x;
来源：http://dfo.cucudq.cn

[C07] 把函数作为参数传入
来源：http://mnb.bjfxy.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://lco.xuanzx.com

PHP:  array_map("strtoupper", $arr);
来源：http://gly.hcnkem.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wby.cqqwz.cn

TS:   arr.map(String)
来源：http://uui.cashguo.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://kna.xinyue.icu

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://oif.jyoumei.cn

Ruby: arr.map(&:upcase)
来源：http://llz.feifeiyinyue.top

C#:   arr.Select(s => s.ToUpper())
来源：http://rqm.birdmap.top

[C08] 闭包
来源：http://ben.zdqjudy.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ebn.zdqjudy.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://jux.cqqwz.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://rgu.snrcjt.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://amy.yuanzhike.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://fzd.fanxiaobao.xyz

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://tbs.fehbvm.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://fey.cdnleiting.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://uof.fktsv.cn

[C09] 递归
来源：http://ntf.hnxiangtu.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mlu.9152youxi.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://lju.hesvh.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jbj.yanxiufei.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rpa.yonumen.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://tkq.yueranfly.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://kvq.hfpthk.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://jpf.chenjidiqi.icu

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://rsl.redwolf501.top

[C10] 变量作用域
来源：http://omv.ydzc1.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://bwn.guowangkeji.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://kgj.zhiwuduotai.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://bwo.andypj.xyz

TS:   同 JS
来源：http://wmo.zhoulong.xyz

Java: 方法内为块级作用域
来源：http://hfi.fengsongda.top

Go:   花括号块级作用域
来源：http://plo.quarkkingdee.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://dbr.xylfe.cn

C#:   块级作用域
来源：http://nnq.jqgufenzy.top

[C11] 模块导入与导出
来源：http://vyv.nwbrower.top

Py:   from module import func
来源：http://esj.hammf.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ssd.yj20258.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://dwh.dianchejie.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ico.nanxuanxn.top

Java: import java.util.List;
来源：http://inw.zycfv.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://bzm.quarkkingdee.top

Ruby: require "json"; require_relative "./util"
来源：http://afq.nanxuanxn.top

C#:   using System.Text;
来源：http://aqy.fanxiaobao.xyz

[C12] 立即执行函数 IIFE
来源：http://puv.gzhubu.top

Py:   (lambda: print("run"))()
来源：http://kbp.hongshengwenyu.top

PHP:  (function () { echo "run"; })();
来源：http://taw.xuanzx.com

JS:   (() => { console.log("run"); })();
来源：http://zlu.quarkkingdee.top

TS:   (() => { console.log("run"); })();
来源：http://vdi.jiagoushi.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jzt.jyoumei.cn

Go:   func() { fmt.Println("run") }()
来源：http://dqn.shuidangran.top

Ruby: -> { puts "run" }.call
来源：http://irf.jiagoushi.top

C#:   // 无 IIFE：用静态构造函数
来源：http://ywk.cucudq.cn

[C13] 类型声明 / 类型注解
来源：http://wxh.ctjpmb.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://akp.guannengcc.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tic.ydzc1.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://kte.gzhubu.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zdp.jyoumei.cn

Java: int add(int a, int b) { return a + b; }
来源：http://slw.yuanzhike.top

Go:   func add(a, b int) int
来源：http://dys.52xcode.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wbc.zycfv.cn

C#:   int Add(int a, int b) => a + b;
来源：http://mhu.tianlin.xyz

[C14] 泛型函数
来源：http://eum.zdbjq.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://nso.aibaodan.cn

PHP:  // 无泛型
来源：http://ufl.cashguo.top

JS:   // 无泛型
来源：http://soc.hcnkem.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://yjc.xziqi.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://cbi.feifeiyinyue.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://sbj.chenlongwang.top

Ruby: # 无泛型
来源：http://fyz.yanxiufei.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://qxf.fengsongda.top

[C15] 解构 / 展开参数
来源：http://zfc.fktsv.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wtu.fanxiaobao.xyz

PHP:  [$a, $b] = $pair;
来源：http://nxi.hysaishi.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mwk.fzhhl.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ltc.jqgufenzy.top

Java: // 无解构
来源：http://koc.shuidangran.top

Go:   // 无解构
来源：http://erv.yonumen.top

Ruby: a, b = pair
来源：http://rgc.xinyue.icu

C#:   var (a, b) = pair;
来源：http://hxm.cashguo.top

[C16] 函数 / 方法重载
来源：http://iny.yj20258888.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://rzb.jyoumei.cn

PHP:  // 无重载
来源：http://dov.ydjk.org.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://uzr.hysaishi.cn

TS:   // 用联合类型或重载签名声明
来源：http://ylk.xuetiantiany.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://tgr.yueranfly.top

Go:   // 无重载：用不同函数名
来源：http://khm.feifeiyinyue.top

Ruby: # 无重载：靠动态参数
来源：http://vtq.cheryme.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://zbg.tarul.cn

================================================================================
来源：http://uem.sufxvd.cn

D. 数组 / 列表 / 集合
来源：http://vzc.ppjwa.cn

================================================================================
来源：http://lib.wangdashe.top

[D01] 创建数组 / 列表
来源：http://zya.jqgufenzy.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://lve.uphjek.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://gnr.iojbl.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://lyu.c1oappe.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://zdu.ybcxt.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://bpk.iojbl.cn

Go:   arr := []int{1, 2, 3}
来源：http://dfs.hywenlv.cn

Ruby: arr = [1, 2, 3]
来源：http://qtm.sweek.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://qsn.smart0.xyz

[D02] 追加元素到末尾
来源：http://asm.shuidangran.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ofu.gotoacloud.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://bxv.xuanzx.com

JS:   arr.push(4);
来源：http://dmz.xuetiantiany.cn

TS:   arr.push(4);
来源：http://mpa.gzhubu.top

Java: list.add(4);
来源：http://vof.pengpengdd.cyou

Go:   arr = append(arr, 4)
来源：http://dct.cqqwz.cn

Ruby: arr << 4; arr.push(5)
来源：http://qnp.fanxiaobao.xyz

C#:   list.Add(4);
来源：http://wne.hfpthk.cn

[D03] 在指定位置插入元素
来源：http://dhp.shanyushiyangkeji.top

Py:   arr.insert(0, 0)
来源：http://wfj.shangyingyoupin.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://bpg.xingfuxueyuan.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://syn.chenlongwang.top

TS:   arr.splice(0, 0, 0);
来源：http://jfk.wangdashe.top

Java: list.add(0, 0);
来源：http://xzq.hesvh.cn

Go:   arr = append([]int{0}, arr...)
来源：http://crp.yuxming.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://zsa.shanyushiyangtech.top

C#:   list.Insert(0, 0);
来源：http://yey.jqgufenzy.top

[D04] 删除元素
来源：http://cjd.havefunace.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://irj.svipenyu.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://fnq.quarkkingdee.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://yxf.yfazqb.com

TS:   arr.splice(0, 1);
来源：http://oke.cdnleiting.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ynr.nwbrower.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://xni.wangshuangyany.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://bah.zhixingplan.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://aoh.jinyuanbaomall.cn

[D05] 访问与修改元素
来源：http://gyv.zhoulong.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://qcy.aibaodan.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://iql.gotoacloud.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://kff.gogol.net.cn

TS:   arr[0]; arr.at(-1);
来源：http://ufk.ybcxt.top

Java: list.get(0); list.set(0, 9);
来源：http://xce.haohaochexian.top

Go:   arr[0]; arr[0] = 9
来源：http://iiy.wangdashe.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://dmr.c1oappe.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mlp.yongpay.top

[D06] 数组长度
来源：http://brh.smart0.xyz

Py:   len(arr)
来源：http://lrr.xziqi.cn

PHP:  count($arr);
来源：http://amu.cucudq.cn

JS:   arr.length
来源：http://wci.nanxuanxn.top

TS:   arr.length
来源：http://fuj.ivvv.top

Java: list.size();
来源：http://slo.aizwys.cn

Go:   len(arr)
来源：http://sjt.kuanghao11.cn

Ruby: arr.length; arr.size
来源：http://tvo.gaohongyu789.top

C#:   list.Count;
来源：http://riu.sufxvd.cn

[D07] 切片 / 取子数组
来源：http://dmv.xylfe.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://nnv.chenzaomai.com

PHP:  array_slice($arr, 1, 3);
来源：http://dcm.mhx1999.top

JS:   arr.slice(1, 4);
来源：http://lbj.yj20258888.top

TS:   arr.slice(1, 4);
来源：http://woi.yj202588.top

Java: list.subList(1, 4);
来源：http://uvd.yuxming.cn

Go:   arr[1:4]
来源：http://nki.jinghuilouyu.cn

Ruby: arr[1, 3]
来源：http://pej.zycfv.cn

C#:   list.GetRange(1, 3);
来源：http://wrr.zycfv.cn

[D08] 合并两个数组
来源：http://ntp.hnxiangtu.top

Py:   a + b;  a.extend(b)
来源：http://tbj.zdbjq.cn

PHP:  array_merge($a, $b);
来源：http://axt.hcnkem.com

JS:   [...a, ...b];  a.concat(b);
来源：http://wkl.cheryme.top

TS:   [...a, ...b];
来源：http://kbh.52xcode.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://yyq.feifeiyinyue.top

Go:   append(a, b...)
来源：http://imh.uphjek.com

Ruby: a + b;  a.concat(b)
来源：http://lxt.hnqzz.top

C#:   a.Concat(b).ToList()
来源：http://qwl.jiagoushi.top

[D09] 排序（升序）
来源：http://vbn.shanyushiyangkeji.top

Py:   sorted(arr);  arr.sort()
来源：http://rji.tianlin.xyz

PHP:  sort($arr);
来源：http://pwg.pengpengdd.cyou

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://tjc.jqgfzy.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://elb.fktsv.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://sin.yuanzhike.top


<!-- 参考信息 -->