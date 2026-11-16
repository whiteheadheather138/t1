代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mlo.yuxming.cn

[B10] 遍历同时拿索引
来源：http://sif.shuidangran.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://fux.cashguo.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://bwv.ppjwa.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://sen.yfazqb.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://yrx.svipenyu.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ytc.jinqigfzy.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://cjv.ehwqpu.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://shy.yuanzhike.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://vrt.shuidangran.top

[B11] 生成数字序列 / 区间
来源：http://btl.hnqzz.top

Py:   list(range(0, 10, 2))
来源：http://xck.shzxlz.cn

PHP:  range(0, 10, 2);
来源：http://crt.ivvv.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fbl.cucudq.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hgz.hfpthk.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://rdh.ivvv.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://tlp.tianlin.xyz

Ruby: (0...10).step(2).to_a
来源：http://wer.zhengqikj.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://xpe.epnwcf.com

[B12] 跳出多层循环
来源：http://uwe.vehdjk.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://tha.jqgufenzy.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://yym.vqdsnc.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://tty.sxryk.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://jjs.cdnleiting.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://arb.jlsjyb.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://qgv.dianchejie.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://axu.cucudq.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://vug.mhx1999.top

[B13] 判断是否为数字
来源：http://fwy.yonumen.top

Py:   isinstance(x, (int, float))
来源：http://eab.dashuyun.cn

PHP:  is_numeric($x)
来源：http://uih.ydzc1.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vke.ydjk.org.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://etg.aibaodan.cn

Java: x instanceof Number
来源：http://wlk.9152youxi.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://agc.chenlongwang.top

Ruby: x.is_a?(Numeric)
来源：http://rva.xuanzx.com

C#:   x is int or double or decimal
来源：http://vfi.wangshuangyany.cn

[B14] 判断值是否在集合内
来源：http://erb.hnxiangtu.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hsd.tarul.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://emc.aizwys.cn

JS:   [1, 2, 3].includes(x)
来源：http://hcq.chenlongwang.top

TS:   [1, 2, 3].includes(x)
来源：http://lwq.shanyushiyangkeji.top

Java: List.of(1, 2, 3).contains(x)
来源：http://skn.sjlbkw.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://jes.aizwys.cn

Ruby: [1, 2, 3].include?(x)
来源：http://mtu.yuxming.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://euk.hcnkem.com

[B15] 布尔运算与取反
来源：http://egg.cheryme.top

Py:   a and b or not c
来源：http://syc.uphjek.com

PHP:  $a && $b || !$c
来源：http://vfv.chenzaomai.com

JS:   a && b || !c
来源：http://wsh.uphjek.com

TS:   a && b || !c
来源：http://byk.cqqwz.cn

Java: a && b || !c
来源：http://gzp.feifeiyinyue.top

Go:   a && b || !c
来源：http://jzq.gaohongyu789.top

Ruby: a && b || !c
来源：http://aku.yueranfly.top

C#:   a && b || !c
来源：http://yjs.yonumen.top

[B16] 卫语句：不满足条件提前返回
来源：http://pge.shangyingyoupin.top

Py:   if not data: return
来源：http://rdx.zhoulong.xyz

PHP:  if (!$data) { return; }
来源：http://lrf.jinqigfzy.top

JS:   if (!data) return;
来源：http://yfy.yj20258888.top

TS:   if (!data) return;
来源：http://feu.xylfe.cn

Java: if (data == null) return;
来源：http://loc.xuetiantiany.cn

Go:   if data == nil { return }
来源：http://lpv.haohaochexian.top

Ruby: return if data.nil?
来源：http://jbc.hysaishi.cn

C#:   if (data == null) return;
来源：http://lzi.meibo888.top

================================================================================
来源：http://tct.yongpay.top

C. 函数与作用域
来源：http://jqg.ywan-chungtsiang.top

================================================================================
来源：http://xqu.xylfe.cn

[C01] 定义函数
来源：http://lim.hysaishi.cn

Py:   def add(a, b): return a + b
来源：http://jxm.sweek.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ixs.xziqi.cn

JS:   function add(a, b) { return a + b; }
来源：http://chl.bjfxy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qhz.yvedp.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://atc.ivvv.top

Go:   func add(a, b int) int { return a + b }
来源：http://vsx.daria6918.cn

Ruby: def add(a, b); a + b; end
来源：http://foo.jinyuanbaomall.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ics.ydjk.org.cn

[C02] 默认参数
来源：http://zna.yuxming.cn

Py:   def greet(name="World"): return name
来源：http://jxb.ydjk.org.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://nwx.yueranfly.top

JS:   function greet(name = "World") { return name; }
来源：http://miq.pycfn.com

TS:   function greet(name: string = "World") { return name; }
来源：http://xqw.ivvv.top

Java: // 无默认参数：方法重载或 Optional
来源：http://vjk.hnxiangtu.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://jsy.yuanzhike.top

Ruby: def greet(name = "World") = name
来源：http://uzr.jianghu66.top

C#:   string Greet(string name = "World") => name;
来源：http://xup.yonumen.top

[C03] 可变参数
来源：http://mpx.cdnleiting.top

Py:   def total(*args): return sum(args)
来源：http://jjg.chenlongwang.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://oab.hammf.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://vda.haohaochexian.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://rxq.sufxvd.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://dbz.feifeiyinyue.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://qoc.haohaochexian.top

Ruby: def total(*nums); nums.sum; end
来源：http://xwv.yongpay.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mll.dashuyun.cn

[C04] 命名参数 / 关键字参数
来源：http://jgr.meibo888.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baq.redwolf501.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://avm.yvedp.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ejx.tian-w.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://kzk.cqqwz.cn

Java: // 无：用 Builder 模式或 record
来源：http://nwk.ywan-chungtsiang.top

Go:   // 无：用配置结构体参数
来源：http://rjy.nanxinkj.top

Ruby: f(a: 1, b: 2)
来源：http://ipo.cashguo.top

C#:   f(a: 1, b: 2)
来源：http://xte.chenjidiqi.icu

[C05] 返回多个值
来源：http://spy.yangfankeji.com

Py:   return a, b
来源：http://iip.kuanghao11.cn

PHP:  return [$a, $b];
来源：http://kds.chenzaomai.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://xuu.zhixingplan.top

TS:   return { a, b };
来源：http://ney.gzhubu.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://diy.birdmap.top

Go:   return a, b
来源：http://rtv.yuanzhike.top

Ruby: return a, b
来源：http://nwy.hcnkem.com

C#:   return (a, b);              // ValueTuple
来源：http://psz.cdnleiting.top

[C06] 匿名函数 / lambda
来源：http://fos.yueranfly.top

Py:   square = lambda x: x * x
来源：http://hro.sjlbkw.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://tem.gotoacloud.top

JS:   const square = x => x * x;
来源：http://mdr.sxryk.cn

TS:   const square = (x: number): number => x * x;
来源：http://sqp.xinyue.icu

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://epl.9152youxi.cn

Go:   sq := func(x int) int { return x * x }
来源：http://lqg.zhijiandao.cn

Ruby: square = ->(x) { x * x }
来源：http://zgy.fanxiaobao.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://crn.birdmap.top

[C07] 把函数作为参数传入
来源：http://pzd.jinqigfzy.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://tuj.epnwcf.com

PHP:  array_map("strtoupper", $arr);
来源：http://qce.dianchejie.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://gsx.hfpthk.cn

TS:   arr.map(String)
来源：http://xux.daria6918.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ibm.nanxuanxn.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://abp.shanyushiyangtech.top

Ruby: arr.map(&:upcase)
来源：http://ust.kuanghao11.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://muj.gzhubu.top

[C08] 闭包
来源：http://ddo.andypj.xyz

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://zsi.yueranfly.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ehn.c1oappe.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://oue.jianghu66.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://his.fehbvm.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ucz.svipenyu.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://szb.jyoumei.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://sze.ydzc1.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://vcp.ctjpmb.com

[C09] 递归
来源：http://hpb.yuxming.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mzy.epnwcf.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://dbd.jlsjyb.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hje.0kj1m.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pcy.52xcode.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://bnw.nwbrower.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://qnr.fengsongda.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://rpt.tian-w.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://zlu.yangfankeji.com

[C10] 变量作用域
来源：http://oxh.birdmap.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://xoq.xylfe.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://vfn.jinqigfzy.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mht.ybcxt.top

TS:   同 JS
来源：http://ilc.vehdjk.com

Java: 方法内为块级作用域
来源：http://ntj.andypj.xyz

Go:   花括号块级作用域
来源：http://qah.ehwqpu.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://fqt.daxiang520.top

C#:   块级作用域
来源：http://gsk.pycfn.com

[C11] 模块导入与导出
来源：http://yry.gzhubu.top

Py:   from module import func
来源：http://bpl.jiagoushi.top

PHP:  require "file.php";  或 use App\Service;
来源：http://pjo.fzhhl.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://ges.pengpengdd.cyou

TS:   export function f(): void {};  import { f } from "./m";
来源：http://tyd.chenjidiqi.icu

Java: import java.util.List;
来源：http://jol.nwbrower.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://bez.cucudq.cn

Ruby: require "json"; require_relative "./util"
来源：http://ykt.zhaomingkeji.xyz

C#:   using System.Text;
来源：http://ibb.sxryk.cn

[C12] 立即执行函数 IIFE
来源：http://wgv.vqdsnc.cn

Py:   (lambda: print("run"))()
来源：http://beg.zhoulong.xyz

PHP:  (function () { echo "run"; })();
来源：http://ydh.xziqi.cn

JS:   (() => { console.log("run"); })();
来源：http://yxu.guowangkeji.top

TS:   (() => { console.log("run"); })();
来源：http://rxj.ppjwa.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mis.svipenyu.cn

Go:   func() { fmt.Println("run") }()
来源：http://csy.cucudq.cn

Ruby: -> { puts "run" }.call
来源：http://vpv.zdbjq.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://mvg.zhaomingkeji.xyz

[C13] 类型声明 / 类型注解
来源：http://bab.bbcook.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://iic.guowangkeji.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ghm.zhijiandao.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://nuz.aizwys.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ecb.jinghuilouyu.cn

Java: int add(int a, int b) { return a + b; }
来源：http://yfx.sysykeji.top

Go:   func add(a, b int) int
来源：http://pyu.snrcjt.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://tbg.bjfxy.top

C#:   int Add(int a, int b) => a + b;
来源：http://glq.zhengqikj.top

[C14] 泛型函数
来源：http://jvm.yangfankeji.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zxg.shanyushiyangkeji.top

PHP:  // 无泛型
来源：http://wmw.aibaodan.cn

JS:   // 无泛型
来源：http://xaa.aizwys.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://xqx.shanyushiyangkeji.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://cqo.chenlongwang.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://kuz.fanxiaobao.xyz

Ruby: # 无泛型
来源：http://soa.ivvv.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://srl.tarul.cn

[C15] 解构 / 展开参数
来源：http://vnl.zhengqikj.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ylc.ppjwa.cn

PHP:  [$a, $b] = $pair;
来源：http://vff.hnqzz.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://whm.sufxvd.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://zgb.xingfuxueyuan.xyz

Java: // 无解构
来源：http://zsp.jqgfzy.top

Go:   // 无解构
来源：http://pey.yangfankeji.com

Ruby: a, b = pair
来源：http://bph.zhengqikj.top

C#:   var (a, b) = pair;
来源：http://ium.jinyuanbaomall.cn

[C16] 函数 / 方法重载
来源：http://yiz.yvedp.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://aph.quarkkingdee.top

PHP:  // 无重载
来源：http://qbh.jinyuanbaomall.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://jdx.snrcjt.cn

TS:   // 用联合类型或重载签名声明
来源：http://qbk.gogol.net.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://mrx.yfazqb.com

Go:   // 无重载：用不同函数名
来源：http://yqx.jyoumei.cn

Ruby: # 无重载：靠动态参数
来源：http://rcp.uphjek.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://gdz.ybcxt.top

================================================================================
来源：http://sgq.svipenyu.cn

D. 数组 / 列表 / 集合
来源：http://xcu.aizwys.cn

================================================================================
来源：http://fww.jinqigfzy.top

[D01] 创建数组 / 列表
来源：http://jfe.svipenyu.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://uat.daxiang520.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://qfy.cqqwz.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://fvv.yanxiufei.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://uve.wangdashe.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ksx.ywan-chungtsiang.top

Go:   arr := []int{1, 2, 3}
来源：http://wrz.ivvv.top

Ruby: arr = [1, 2, 3]
来源：http://egn.hnxiangtu.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://zej.ctjpmb.com

[D02] 追加元素到末尾
来源：http://jxq.ctjpmb.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://pha.tian-w.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://umd.jinghuilouyu.cn

JS:   arr.push(4);
来源：http://nht.9152youxi.cn

TS:   arr.push(4);
来源：http://dnk.fanxiaobao.xyz

Java: list.add(4);
来源：http://enz.pengpengdd.cyou

Go:   arr = append(arr, 4)
来源：http://xhi.tanke756.top

Ruby: arr << 4; arr.push(5)
来源：http://kjp.sufxvd.cn

C#:   list.Add(4);
来源：http://pwn.jinqigufen.top

[D03] 在指定位置插入元素
来源：http://squ.sxryk.cn

Py:   arr.insert(0, 0)
来源：http://ljx.uphjek.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://vej.iojbl.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://scz.bjfxy.top

TS:   arr.splice(0, 0, 0);
来源：http://rjt.zhixingplan.top

Java: list.add(0, 0);
来源：http://nmb.sufxvd.cn

Go:   arr = append([]int{0}, arr...)
来源：http://knn.aibaodan.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://rjf.ctjpmb.com

C#:   list.Insert(0, 0);
来源：http://rak.ctjpmb.com

[D04] 删除元素
来源：http://bdc.sweek.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wsr.jinqigufen.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://noa.jinyuanbaomall.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xgp.yfazqb.com

TS:   arr.splice(0, 1);
来源：http://rpy.gogol.net.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wax.nanxinkj.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ccg.vehdjk.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hks.redwolf501.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://dfx.zhiwuduotai.top

[D05] 访问与修改元素
来源：http://pse.zhixingplan.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://lfw.jinyuanbaomall.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://cka.316326.xyz

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://sfy.pycfn.com

TS:   arr[0]; arr.at(-1);
来源：http://gml.birdmap.top

Java: list.get(0); list.set(0, 9);
来源：http://pku.jqgfzy.top

Go:   arr[0]; arr[0] = 9
来源：http://duq.haohaochexian.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hew.hywenlv.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://gfw.xingfuxueyuan.xyz

[D06] 数组长度
来源：http://mld.tarul.cn

Py:   len(arr)
来源：http://iah.nwbrower.top

PHP:  count($arr);
来源：http://weg.nanxuanxn.top

JS:   arr.length
来源：http://sau.chenjidiqi.icu

TS:   arr.length
来源：http://tjq.yvedp.cn

Java: list.size();
来源：http://ajh.gotoacloud.top

Go:   len(arr)
来源：http://fdi.xuetiantiany.cn

Ruby: arr.length; arr.size
来源：http://zlj.shzxlz.cn

C#:   list.Count;
来源：http://fqd.chenzaomai.com

[D07] 切片 / 取子数组
来源：http://ihh.vqdsnc.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://gri.mhx1999.top

PHP:  array_slice($arr, 1, 3);
来源：http://biw.jyoumei.cn

JS:   arr.slice(1, 4);
来源：http://pzw.dianchejie.cn

TS:   arr.slice(1, 4);
来源：http://bfe.iojbl.cn

Java: list.subList(1, 4);
来源：http://tqo.shuidangran.top

Go:   arr[1:4]
来源：http://hpw.pengpengdd.cyou

Ruby: arr[1, 3]
来源：http://hmu.316326.xyz

C#:   list.GetRange(1, 3);
来源：http://ffv.ywan-chungtsiang.top

[D08] 合并两个数组
来源：http://uwy.jiagoushi.top

Py:   a + b;  a.extend(b)
来源：http://otf.jinqigfzy.top

PHP:  array_merge($a, $b);
来源：http://mfp.yvedp.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://tfe.yongpay.top

TS:   [...a, ...b];
来源：http://nni.andypj.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://irq.redwolf501.top

Go:   append(a, b...)
来源：http://bps.jyoumei.cn

Ruby: a + b;  a.concat(b)
来源：http://vvf.sjlbkw.cn

C#:   a.Concat(b).ToList()
来源：http://kkd.quarkkingdee.top

[D09] 排序（升序）
来源：http://odq.cqqwz.cn

Py:   sorted(arr);  arr.sort()
来源：http://gjc.yj20258888.top

PHP:  sort($arr);
来源：http://jud.hnxiangtu.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://eqq.52xcode.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ust.havefunace.top

Java: Collections.sort(list);  list.sort(null);
来源：http://omz.guowangkeji.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://fsb.zhijiandao.cn

Ruby: arr.sort
来源：http://zas.gogol.net.cn

C#:   list.Sort();
来源：http://jsx.shuidangran.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://kgb.quarkkingdee.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://gbw.zhongyouzk.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mkm.yfazqb.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://cbo.jianghu66.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://jcf.guowangkeji.top


<!-- 参考信息 -->