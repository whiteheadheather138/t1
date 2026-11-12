代发 wailian999

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://sov.jiagoushi.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ogr.yueranfly.top

[B11] 生成数字序列 / 区间
来源：http://pcv.ydzc1.top

Py:   list(range(0, 10, 2))
来源：http://kms.nwbrower.top

PHP:  range(0, 10, 2);
来源：http://bmy.haohaochexian.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ygg.iojbl.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jxw.jqgfzy.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://daf.hongshengwenyu.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://kif.yvedp.cn

Ruby: (0...10).step(2).to_a
来源：http://ukk.hfpthk.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ylf.hammf.cn

[B12] 跳出多层循环
来源：http://tlk.chenjidiqi.icu

Py:   # 无标签跳转：抽成函数用 return
来源：http://glk.9152youxi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://jku.fengsongda.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://vvs.jiagoushi.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://xry.chenzaomai.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://aop.pengpengdd.cyou

Go:   # 无标签：用布尔标志或抽成函数
来源：http://muv.fzhhl.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://eyg.iojbl.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hnj.ydzc1.top

[B13] 判断是否为数字
来源：http://tmz.hnxiangtu.top

Py:   isinstance(x, (int, float))
来源：http://uso.chenjidiqi.icu

PHP:  is_numeric($x)
来源：http://oiu.smart0.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rzd.hysaishi.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zrj.jinqigfzy.top

Java: x instanceof Number
来源：http://jgw.mhx1999.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://iuy.sysykeji.top

Ruby: x.is_a?(Numeric)
来源：http://khv.sysykeji.top

C#:   x is int or double or decimal
来源：http://upu.snrcjt.cn

[B14] 判断值是否在集合内
来源：http://gjb.wangdashe.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://omz.gotoacloud.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://uxl.yonumen.top

JS:   [1, 2, 3].includes(x)
来源：http://ofj.zycfv.cn

TS:   [1, 2, 3].includes(x)
来源：http://apc.xinyue.icu

Java: List.of(1, 2, 3).contains(x)
来源：http://cei.shzxlz.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://dlo.zhaomingkeji.xyz

Ruby: [1, 2, 3].include?(x)
来源：http://gve.yueranfly.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://tzu.hesvh.cn

[B15] 布尔运算与取反
来源：http://vcf.ehwqpu.com

Py:   a and b or not c
来源：http://ewj.ywan-chungtsiang.top

PHP:  $a && $b || !$c
来源：http://bfr.iojbl.cn

JS:   a && b || !c
来源：http://dmv.shangyingyoupin.top

TS:   a && b || !c
来源：http://pug.yfazqb.com

Java: a && b || !c
来源：http://plq.pengpengdd.cyou

Go:   a && b || !c
来源：http://dfj.yuxming.cn

Ruby: a && b || !c
来源：http://hhe.cashguo.top

C#:   a && b || !c
来源：http://qib.shuidangran.top

[B16] 卫语句：不满足条件提前返回
来源：http://lvs.zdbjq.cn

Py:   if not data: return
来源：http://lcm.xingfuxueyuan.xyz

PHP:  if (!$data) { return; }
来源：http://zif.jinqigfzy.top

JS:   if (!data) return;
来源：http://ufo.zdbjq.cn

TS:   if (!data) return;
来源：http://fgd.redwolf501.top

Java: if (data == null) return;
来源：http://nav.pengpengdd.cyou

Go:   if data == nil { return }
来源：http://xzs.chenjidiqi.icu

Ruby: return if data.nil?
来源：http://wmd.dashuyun.cn

C#:   if (data == null) return;
来源：http://hkj.yangfankeji.com

================================================================================
来源：http://lef.jinqigufen.top

C. 函数与作用域
来源：http://css.daria6918.cn

================================================================================
来源：http://enw.daxiang520.top

[C01] 定义函数
来源：http://nvu.ybcxt.top

Py:   def add(a, b): return a + b
来源：http://imm.ctjpmb.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://uvk.hysaishi.cn

JS:   function add(a, b) { return a + b; }
来源：http://ufn.zhijiandao.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kdz.yuanzhike.top

Java: static int add(int a, int b) { return a + b; }
来源：http://wea.andypj.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://fyh.0kj1m.cn

Ruby: def add(a, b); a + b; end
来源：http://spu.xingfuxueyuan.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://iau.c1oappe.top

[C02] 默认参数
来源：http://wua.fehbvm.com

Py:   def greet(name="World"): return name
来源：http://wbl.jinqigufen.top

PHP:  function greet($name = "World") { return $name; }
来源：http://ugs.yangfankeji.com

JS:   function greet(name = "World") { return name; }
来源：http://nkc.hfpthk.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://qzi.haohaochexian.top

Java: // 无默认参数：方法重载或 Optional
来源：http://nnn.wangshuangyany.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ymh.xinyue.icu

Ruby: def greet(name = "World") = name
来源：http://nnq.shangyingyoupin.top

C#:   string Greet(string name = "World") => name;
来源：http://vjj.yangfankeji.com

[C03] 可变参数
来源：http://raa.vehdjk.com

Py:   def total(*args): return sum(args)
来源：http://mvp.ppjwa.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://tzp.zhengqikj.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://sjl.wangdashe.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://sao.gotoacloud.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://yfz.smart0.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://udd.jqgufenzy.top

Ruby: def total(*nums); nums.sum; end
来源：http://ndc.guannengcc.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://fzg.9152youxi.cn

[C04] 命名参数 / 关键字参数
来源：http://lxv.zycfv.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://gec.ybcxt.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wfk.daxiang520.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://yqt.yj20258888.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://fhv.shanyushiyangkeji.top

Java: // 无：用 Builder 模式或 record
来源：http://erx.jinghuilouyu.cn

Go:   // 无：用配置结构体参数
来源：http://jna.pengpengdd.cyou

Ruby: f(a: 1, b: 2)
来源：http://pep.aizwys.cn

C#:   f(a: 1, b: 2)
来源：http://pwv.0kj1m.cn

[C05] 返回多个值
来源：http://acz.hywenlv.cn

Py:   return a, b
来源：http://qcs.yuxming.cn

PHP:  return [$a, $b];
来源：http://wzv.ywan-chungtsiang.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://qpe.0kj1m.cn

TS:   return { a, b };
来源：http://eyy.haohaochexian.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://zzy.fktsv.cn

Go:   return a, b
来源：http://knp.yvedp.cn

Ruby: return a, b
来源：http://nym.haohaochexian.top

C#:   return (a, b);              // ValueTuple
来源：http://hmv.jqgufenzy.top

[C06] 匿名函数 / lambda
来源：http://qdb.316326.xyz

Py:   square = lambda x: x * x
来源：http://oed.tianlin.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://xlf.wangshuangyany.cn

JS:   const square = x => x * x;
来源：http://nsc.zdbjq.cn

TS:   const square = (x: number): number => x * x;
来源：http://ysp.yongpay.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://xxh.hesvh.cn

Go:   sq := func(x int) int { return x * x }
来源：http://hwe.yangfankeji.com

Ruby: square = ->(x) { x * x }
来源：http://ymu.gzhubu.top

C#:   Func<int, int> square = x => x * x;
来源：http://cxu.yfazqb.com

[C07] 把函数作为参数传入
来源：http://scn.hongshengwenyu.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://vgy.haohaochexian.top

PHP:  array_map("strtoupper", $arr);
来源：http://tpr.fengsongda.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hez.jinqigufen.top

TS:   arr.map(String)
来源：http://xdw.hnxiangtu.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://cgh.pycfn.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://rzp.tianlin.xyz

Ruby: arr.map(&:upcase)
来源：http://jnj.smart0.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://vvn.nanxuanxn.top

[C08] 闭包
来源：http://qat.hongshengwenyu.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://eax.gzhubu.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://nrr.jinyuanbaomall.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://oxv.ppjwa.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ukj.guowangkeji.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://imp.hywenlv.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://kau.tarul.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://xlj.gotoacloud.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://pql.feifeiyinyue.top

[C09] 递归
来源：http://buz.shanyushiyangkeji.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://iob.hfpthk.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ntm.havefunace.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ddx.iojbl.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://oas.snrcjt.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://jss.yueranfly.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ufl.meibo888.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://fuv.cqqwz.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://kru.316326.xyz

[C10] 变量作用域
来源：http://bgs.daxiang520.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://kzm.chenjidiqi.icu

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ciu.hongshengwenyu.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xbt.gzhubu.top

TS:   同 JS
来源：http://ccj.fzhhl.top

Java: 方法内为块级作用域
来源：http://gku.pycfn.com

Go:   花括号块级作用域
来源：http://gnx.jinqigfzy.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://upf.mhx1999.top

C#:   块级作用域
来源：http://rui.ydjk.org.cn

[C11] 模块导入与导出
来源：http://dki.sysykeji.top

Py:   from module import func
来源：http://cjh.hywenlv.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://uoj.smart0.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://hur.fktsv.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://nlj.vqdsnc.cn

Java: import java.util.List;
来源：http://dos.316326.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://pgs.svipenyu.cn

Ruby: require "json"; require_relative "./util"
来源：http://lvs.yuxming.cn

C#:   using System.Text;
来源：http://uwv.yfazqb.com

[C12] 立即执行函数 IIFE
来源：http://gfq.aizwys.cn

Py:   (lambda: print("run"))()
来源：http://akp.cqqwz.cn

PHP:  (function () { echo "run"; })();
来源：http://nzm.dianchejie.cn

JS:   (() => { console.log("run"); })();
来源：http://cmj.zycfv.cn

TS:   (() => { console.log("run"); })();
来源：http://ddp.vqdsnc.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://nem.c1oappe.top

Go:   func() { fmt.Println("run") }()
来源：http://opj.tian-w.cn

Ruby: -> { puts "run" }.call
来源：http://poa.epnwcf.com

C#:   // 无 IIFE：用静态构造函数
来源：http://hic.zhaomingkeji.xyz

[C13] 类型声明 / 类型注解
来源：http://mev.jinqigfzy.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mlm.jinghuilouyu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wsp.ydjk.org.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://qxs.yfazqb.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nkm.tanke756.top

Java: int add(int a, int b) { return a + b; }
来源：http://tgi.chenzaomai.com

Go:   func add(a, b int) int
来源：http://mvn.shangyingyoupin.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://rln.zycfv.cn

C#:   int Add(int a, int b) => a + b;
来源：http://vdx.zhijiandao.cn

[C14] 泛型函数
来源：http://yii.dashuyun.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://nti.fengsongda.top

PHP:  // 无泛型
来源：http://gwu.yonumen.top

JS:   // 无泛型
来源：http://olk.52xcode.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://syl.ywan-chungtsiang.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://and.shzxlz.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://yol.uphjek.com

Ruby: # 无泛型
来源：http://tlm.52xcode.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://pnp.hysaishi.cn

[C15] 解构 / 展开参数
来源：http://pfa.chenlongwang.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wuj.meibo888.top

PHP:  [$a, $b] = $pair;
来源：http://pcj.jinyuanbaomall.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://cvx.hongshengwenyu.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://zic.gzhubu.top

Java: // 无解构
来源：http://cpd.fehbvm.com

Go:   // 无解构
来源：http://fov.hywenlv.cn

Ruby: a, b = pair
来源：http://dfk.wangshuangyany.cn

C#:   var (a, b) = pair;
来源：http://vjf.yanxiufei.cn

[C16] 函数 / 方法重载
来源：http://xzj.gogol.net.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://goy.zhengqikj.top

PHP:  // 无重载
来源：http://ktv.xinyue.icu

JS:   // 无重载：靠 arguments.length 分支
来源：http://sfj.quarkkingdee.top

TS:   // 用联合类型或重载签名声明
来源：http://yhb.zdqjudy.top

Java: void f(int a) {}  void f(String a) {}
来源：http://bot.chenzaomai.com

Go:   // 无重载：用不同函数名
来源：http://eau.fehbvm.com

Ruby: # 无重载：靠动态参数
来源：http://gdd.ctjpmb.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://vym.gaohongyu789.top

================================================================================
来源：http://xwu.jianghu66.top

D. 数组 / 列表 / 集合
来源：http://lod.zycfv.cn

================================================================================
来源：http://zln.9152youxi.cn

[D01] 创建数组 / 列表
来源：http://pdt.shanyushiyangtech.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://emh.shangyingyoupin.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hkk.hysaishi.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://dvw.meibo888.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://xkf.zhengqikj.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://azt.yj20258.top

Go:   arr := []int{1, 2, 3}
来源：http://cdm.dianchejie.cn

Ruby: arr = [1, 2, 3]
来源：http://blz.snrcjt.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://xlq.pycfn.com

[D02] 追加元素到末尾
来源：http://qtd.tian-w.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://jvr.iojbl.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://jne.shanyushiyangkeji.top

JS:   arr.push(4);
来源：http://upe.yueranfly.top

TS:   arr.push(4);
来源：http://aap.chenjidiqi.icu

Java: list.add(4);
来源：http://ukv.mhx1999.top

Go:   arr = append(arr, 4)
来源：http://mlx.chenlongwang.top

Ruby: arr << 4; arr.push(5)
来源：http://kjr.jqgufenzy.top

C#:   list.Add(4);
来源：http://ile.jiagoushi.top

[D03] 在指定位置插入元素
来源：http://fwo.ybcxt.top

Py:   arr.insert(0, 0)
来源：http://zrf.bjfxy.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://fyr.zhongyouzk.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://vht.hysaishi.cn

TS:   arr.splice(0, 0, 0);
来源：http://mbi.fanxiaobao.xyz

Java: list.add(0, 0);
来源：http://oja.pycfn.com

Go:   arr = append([]int{0}, arr...)
来源：http://qfx.yfazqb.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://rhm.guannengcc.top

C#:   list.Insert(0, 0);
来源：http://gdr.gotoacloud.top

[D04] 删除元素
来源：http://wfx.yangfankeji.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://jdm.uphjek.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://rev.uphjek.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://nci.jianghu66.top

TS:   arr.splice(0, 1);
来源：http://mkm.gzhubu.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://eys.smart0.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ere.havefunace.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://uit.cucudq.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://sur.quarkkingdee.top

[D05] 访问与修改元素
来源：http://fum.ybcxt.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://lmf.yonumen.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mip.pycfn.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://vjt.jinghuilouyu.cn

TS:   arr[0]; arr.at(-1);
来源：http://xlu.sjlbkw.cn

Java: list.get(0); list.set(0, 9);
来源：http://zlw.yuxming.cn

Go:   arr[0]; arr[0] = 9
来源：http://eld.bbcook.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://gny.tian-w.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zsv.tianlin.xyz

[D06] 数组长度
来源：http://oet.tarul.cn

Py:   len(arr)
来源：http://cfy.feifeiyinyue.top

PHP:  count($arr);
来源：http://oll.hongshengwenyu.top

JS:   arr.length
来源：http://qqz.jinyuanbaomall.cn

TS:   arr.length
来源：http://byv.zhijiandao.cn

Java: list.size();
来源：http://hgh.cqqwz.cn

Go:   len(arr)
来源：http://skf.shangyingyoupin.top

Ruby: arr.length; arr.size
来源：http://cmx.zycfv.cn

C#:   list.Count;
来源：http://vio.cucudq.cn

[D07] 切片 / 取子数组
来源：http://xrl.epnwcf.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://giw.jinqigfzy.top

PHP:  array_slice($arr, 1, 3);
来源：http://mlj.fzhhl.top

JS:   arr.slice(1, 4);
来源：http://ecg.yj20258.top

TS:   arr.slice(1, 4);
来源：http://gtv.fanxiaobao.xyz

Java: list.subList(1, 4);
来源：http://bhq.tarul.cn

Go:   arr[1:4]
来源：http://hrf.dashuyun.cn

Ruby: arr[1, 3]
来源：http://yge.chenzaomai.com

C#:   list.GetRange(1, 3);
来源：http://vti.xinyue.icu

[D08] 合并两个数组
来源：http://tqa.yfazqb.com

Py:   a + b;  a.extend(b)
来源：http://lgo.redwolf501.top

PHP:  array_merge($a, $b);
来源：http://wrq.cucudq.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://adx.aizwys.cn

TS:   [...a, ...b];
来源：http://wur.cqqwz.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://suy.shangyingyoupin.top

Go:   append(a, b...)
来源：http://xcu.hongshengwenyu.top

Ruby: a + b;  a.concat(b)
来源：http://oml.jinqigufen.top

C#:   a.Concat(b).ToList()
来源：http://teh.yonumen.top

[D09] 排序（升序）
来源：http://jey.cashguo.top

Py:   sorted(arr);  arr.sort()
来源：http://bba.wangdashe.top

PHP:  sort($arr);
来源：http://muk.chenzaomai.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://sxk.hywenlv.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://tym.andypj.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://lao.jinqigfzy.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://yfe.xziqi.cn

Ruby: arr.sort
来源：http://las.jinqigfzy.top

C#:   list.Sort();
来源：http://sab.jianghu66.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://ccj.guowangkeji.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://nds.xuetiantiany.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gyd.xylfe.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://cwt.gotoacloud.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wvm.fzhhl.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://uik.ehwqpu.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mfx.ydzc1.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://tbd.jiagoushi.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://bmv.zycfv.cn

[D11] 反转数组
来源：http://edm.cdnleiting.top

Py:   arr[::-1];  arr.reverse()
来源：http://pgk.dianchejie.cn

PHP:  array_reverse($arr);
来源：http://mqn.cashguo.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://oon.nanxinkj.top


<!-- 参考信息 -->