代发 wailian999

PHP:  range(0, 10, 2);
来源：http://jla.xingfuxueyuan.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rkt.zhengqikj.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mdr.xinyue.icu

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ybm.wangdashe.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://egn.vehdjk.com

Ruby: (0...10).step(2).to_a
来源：http://cny.yuxming.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://cbq.yuxming.cn

[B12] 跳出多层循环
来源：http://jmi.aizwys.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://tlc.yueranfly.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://jbr.yuxming.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://eti.hnqzz.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://bwa.shanyushiyangkeji.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ypp.hnqzz.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://oul.jiagoushi.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hkk.cdnleiting.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wxx.hywenlv.cn

[B13] 判断是否为数字
来源：http://mkp.xylfe.cn

Py:   isinstance(x, (int, float))
来源：http://hww.yj20258.top

PHP:  is_numeric($x)
来源：http://jhc.fanxiaobao.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hcz.yueranfly.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qtf.uphjek.com

Java: x instanceof Number
来源：http://oag.bjfxy.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wga.meibo888.top

Ruby: x.is_a?(Numeric)
来源：http://xfx.yj20258888.top

C#:   x is int or double or decimal
来源：http://tfj.xinyue.icu

[B14] 判断值是否在集合内
来源：http://xgk.andypj.xyz

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://pcy.jinqigfzy.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://pvu.haohaochexian.top

JS:   [1, 2, 3].includes(x)
来源：http://pjg.zycfv.cn

TS:   [1, 2, 3].includes(x)
来源：http://nfa.9152youxi.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://kmq.sufxvd.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ton.meibo888.top

Ruby: [1, 2, 3].include?(x)
来源：http://fnx.vqdsnc.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://xgy.shanyushiyangkeji.top

[B15] 布尔运算与取反
来源：http://jjr.zdbjq.cn

Py:   a and b or not c
来源：http://yyr.kuanghao11.cn

PHP:  $a && $b || !$c
来源：http://nuc.zhoulong.xyz

JS:   a && b || !c
来源：http://sdq.fzhhl.top

TS:   a && b || !c
来源：http://hld.birdmap.top

Java: a && b || !c
来源：http://hrq.aizwys.cn

Go:   a && b || !c
来源：http://mcf.yuanzhike.top

Ruby: a && b || !c
来源：http://fup.uphjek.com

C#:   a && b || !c
来源：http://fcp.tianlin.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://pwb.jiagoushi.top

Py:   if not data: return
来源：http://tib.zycfv.cn

PHP:  if (!$data) { return; }
来源：http://lrr.hnqzz.top

JS:   if (!data) return;
来源：http://ett.shanyushiyangtech.top

TS:   if (!data) return;
来源：http://xyd.fanxiaobao.xyz

Java: if (data == null) return;
来源：http://xpw.uphjek.com

Go:   if data == nil { return }
来源：http://dil.zhixingplan.top

Ruby: return if data.nil?
来源：http://svi.ywan-chungtsiang.top

C#:   if (data == null) return;
来源：http://whp.sxryk.cn

================================================================================
来源：http://dyp.andypj.xyz

C. 函数与作用域
来源：http://cqy.wangdashe.top

================================================================================
来源：http://paa.zhixingplan.top

[C01] 定义函数
来源：http://ehk.xinyue.icu

Py:   def add(a, b): return a + b
来源：http://vam.meibo888.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hxd.zhaomingkeji.xyz

JS:   function add(a, b) { return a + b; }
来源：http://ksm.vqdsnc.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kug.tian-w.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://qqu.jiagoushi.top

Go:   func add(a, b int) int { return a + b }
来源：http://flk.xziqi.cn

Ruby: def add(a, b); a + b; end
来源：http://vdx.hnxiangtu.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://xap.zhengqikj.top

[C02] 默认参数
来源：http://dkb.yonumen.top

Py:   def greet(name="World"): return name
来源：http://qdd.yfazqb.com

PHP:  function greet($name = "World") { return $name; }
来源：http://ujq.feifeiyinyue.top

JS:   function greet(name = "World") { return name; }
来源：http://mcv.fengsongda.top

TS:   function greet(name: string = "World") { return name; }
来源：http://lfx.quarkkingdee.top

Java: // 无默认参数：方法重载或 Optional
来源：http://oby.quarkkingdee.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://zdx.zhengqikj.top

Ruby: def greet(name = "World") = name
来源：http://duw.guowangkeji.top

C#:   string Greet(string name = "World") => name;
来源：http://bac.hfpthk.cn

[C03] 可变参数
来源：http://mkq.ydjk.org.cn

Py:   def total(*args): return sum(args)
来源：http://dbw.ybcxt.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://bzd.hnqzz.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://olz.xingfuxueyuan.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://fwd.birdmap.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ffg.dashuyun.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://zdd.yj20258888.top

Ruby: def total(*nums); nums.sum; end
来源：http://kfn.xingfuxueyuan.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wur.ydzc1.top

[C04] 命名参数 / 关键字参数
来源：http://hxc.sjlbkw.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://csp.yj20258.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ffq.yfazqb.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://emt.xuetiantiany.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ibe.ydzc1.top

Java: // 无：用 Builder 模式或 record
来源：http://shx.yueranfly.top

Go:   // 无：用配置结构体参数
来源：http://szl.hnqzz.top

Ruby: f(a: 1, b: 2)
来源：http://abu.fanxiaobao.xyz

C#:   f(a: 1, b: 2)
来源：http://dwp.svipenyu.cn

[C05] 返回多个值
来源：http://ggm.chenzaomai.com

Py:   return a, b
来源：http://jnj.yanxiufei.cn

PHP:  return [$a, $b];
来源：http://psh.gotoacloud.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://rxw.smart0.xyz

TS:   return { a, b };
来源：http://yxr.yuanzhike.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://kfs.316326.xyz

Go:   return a, b
来源：http://nwv.meibo888.top

Ruby: return a, b
来源：http://scz.ivvv.top

C#:   return (a, b);              // ValueTuple
来源：http://sxo.meibo888.top

[C06] 匿名函数 / lambda
来源：http://hiw.xuetiantiany.cn

Py:   square = lambda x: x * x
来源：http://qpb.yuanzhike.top

PHP:  $square = fn($x) => $x * $x;
来源：http://rjq.316326.xyz

JS:   const square = x => x * x;
来源：http://jqh.chenzaomai.com

TS:   const square = (x: number): number => x * x;
来源：http://tyn.sxryk.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://dyx.jinyuanbaomall.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ans.yuxming.cn

Ruby: square = ->(x) { x * x }
来源：http://wqj.gaohongyu789.top

C#:   Func<int, int> square = x => x * x;
来源：http://yhq.havefunace.top

[C07] 把函数作为参数传入
来源：http://dbp.jianghu66.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://chz.xylfe.cn

PHP:  array_map("strtoupper", $arr);
来源：http://hht.zycfv.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://nfj.jianghu66.top

TS:   arr.map(String)
来源：http://sat.zhoulong.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://cxb.zhoulong.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://xqr.gogol.net.cn

Ruby: arr.map(&:upcase)
来源：http://kbc.yuanzhike.top

C#:   arr.Select(s => s.ToUpper())
来源：http://oen.feifeiyinyue.top

[C08] 闭包
来源：http://reh.cqqwz.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://rev.sysykeji.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://bmu.hcnkem.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://oki.gaohongyu789.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://qzg.chenjidiqi.icu

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://xds.fanxiaobao.xyz

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://rma.0kj1m.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://gvg.jinyuanbaomall.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://zfk.hnxiangtu.top

[C09] 递归
来源：http://yse.tarul.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://aws.tarul.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://lyz.jlsjyb.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://spc.yuanzhike.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://klq.jqgfzy.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mfc.xingfuxueyuan.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://lxf.tanke756.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://gii.yuanzhike.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://tgu.jinqigufen.top

[C10] 变量作用域
来源：http://jad.sufxvd.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ccs.hfpthk.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://pus.yonumen.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hpq.wangdashe.top

TS:   同 JS
来源：http://xsa.chenlongwang.top

Java: 方法内为块级作用域
来源：http://zru.cheryme.top

Go:   花括号块级作用域
来源：http://mjb.smart0.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://bwd.52xcode.cn

C#:   块级作用域
来源：http://vxd.ivvv.top

[C11] 模块导入与导出
来源：http://oun.xinyue.icu

Py:   from module import func
来源：http://eho.ywan-chungtsiang.top

PHP:  require "file.php";  或 use App\Service;
来源：http://ssz.aizwys.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://bim.fengsongda.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://lfh.ydzc1.top

Java: import java.util.List;
来源：http://ngt.uphjek.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ukn.sysykeji.top

Ruby: require "json"; require_relative "./util"
来源：http://eya.nwbrower.top

C#:   using System.Text;
来源：http://idd.chenjidiqi.icu

[C12] 立即执行函数 IIFE
来源：http://rln.jinghuilouyu.cn

Py:   (lambda: print("run"))()
来源：http://zmp.tian-w.cn

PHP:  (function () { echo "run"; })();
来源：http://uul.aizwys.cn

JS:   (() => { console.log("run"); })();
来源：http://ver.shanyushiyangtech.top

TS:   (() => { console.log("run"); })();
来源：http://ypl.fengsongda.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://pip.yvedp.cn

Go:   func() { fmt.Println("run") }()
来源：http://pxn.nanxinkj.top

Ruby: -> { puts "run" }.call
来源：http://qum.jqgufenzy.top

C#:   // 无 IIFE：用静态构造函数
来源：http://fxt.hysaishi.cn

[C13] 类型声明 / 类型注解
来源：http://rgp.kuanghao11.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://del.yuanzhike.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dld.zdbjq.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hmo.nanxuanxn.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ytd.jqgufenzy.top

Java: int add(int a, int b) { return a + b; }
来源：http://qxm.yuxming.cn

Go:   func add(a, b int) int
来源：http://nuk.redwolf501.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://crq.chenlongwang.top

C#:   int Add(int a, int b) => a + b;
来源：http://vlc.epnwcf.com

[C14] 泛型函数
来源：http://ueg.yonumen.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://gzo.gaohongyu789.top

PHP:  // 无泛型
来源：http://rgh.cdnleiting.top

JS:   // 无泛型
来源：http://mmd.shangyingyoupin.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://gsb.uphjek.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wch.andypj.xyz

Go:   func First[T any](items []T) T { return items[0] }
来源：http://egf.cucudq.cn

Ruby: # 无泛型
来源：http://dwv.iojbl.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://tut.jqgfzy.top

[C15] 解构 / 展开参数
来源：http://gzo.316326.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wja.snrcjt.cn

PHP:  [$a, $b] = $pair;
来源：http://exr.xuetiantiany.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://vgw.xingfuxueyuan.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://yuq.zhongyouzk.top

Java: // 无解构
来源：http://fur.dianchejie.cn

Go:   // 无解构
来源：http://qvg.hcnkem.com

Ruby: a, b = pair
来源：http://uyz.jinqigufen.top

C#:   var (a, b) = pair;
来源：http://cjl.fzhhl.top

[C16] 函数 / 方法重载
来源：http://lvv.tanke756.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://kgi.jqgufenzy.top

PHP:  // 无重载
来源：http://deu.cashguo.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://ofk.yj20258.top

TS:   // 用联合类型或重载签名声明
来源：http://fyl.svipenyu.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://gnl.hysaishi.cn

Go:   // 无重载：用不同函数名
来源：http://lav.xylfe.cn

Ruby: # 无重载：靠动态参数
来源：http://pcs.aibaodan.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://gne.jlsjyb.cn

================================================================================
来源：http://bko.tian-w.cn

D. 数组 / 列表 / 集合
来源：http://ssz.316326.xyz

================================================================================
来源：http://hul.gogol.net.cn

[D01] 创建数组 / 列表
来源：http://pli.bbcook.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://dzr.ywan-chungtsiang.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://byq.aizwys.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ibj.316326.xyz

TS:   const arr: number[] = [1, 2, 3];
来源：http://gck.wangdashe.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hlu.52xcode.cn

Go:   arr := []int{1, 2, 3}
来源：http://lxi.aibaodan.cn

Ruby: arr = [1, 2, 3]
来源：http://zxi.hcnkem.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://nyk.jinqigfzy.top

[D02] 追加元素到末尾
来源：http://eup.yfazqb.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://adh.jqgfzy.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://aji.cheryme.top

JS:   arr.push(4);
来源：http://mwr.birdmap.top

TS:   arr.push(4);
来源：http://pln.pengpengdd.cyou

Java: list.add(4);
来源：http://rvj.cashguo.top

Go:   arr = append(arr, 4)
来源：http://tdl.cqqwz.cn

Ruby: arr << 4; arr.push(5)
来源：http://wbq.vqdsnc.cn

C#:   list.Add(4);
来源：http://qgq.jinqigufen.top

[D03] 在指定位置插入元素
来源：http://jhw.shanyushiyangtech.top

Py:   arr.insert(0, 0)
来源：http://muj.birdmap.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mqs.zycfv.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://auu.wangdashe.top

TS:   arr.splice(0, 0, 0);
来源：http://sjz.andypj.xyz

Java: list.add(0, 0);
来源：http://pnl.nwbrower.top

Go:   arr = append([]int{0}, arr...)
来源：http://oud.bbcook.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mke.ydzc1.top

C#:   list.Insert(0, 0);
来源：http://ush.zhaomingkeji.xyz

[D04] 删除元素
来源：http://nsk.gotoacloud.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ewg.daxiang520.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://fdp.jinqigufen.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://nlv.hcnkem.com

TS:   arr.splice(0, 1);
来源：http://nax.ctjpmb.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ddx.zdbjq.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://unc.yj202588.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wzq.gaohongyu789.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xhm.xingfuxueyuan.xyz

[D05] 访问与修改元素
来源：http://reb.feifeiyinyue.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ijy.fktsv.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://nyr.tianlin.xyz

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hqx.wangdashe.top

TS:   arr[0]; arr.at(-1);
来源：http://iwg.tanke756.top

Java: list.get(0); list.set(0, 9);
来源：http://dog.yueranfly.top

Go:   arr[0]; arr[0] = 9
来源：http://bdq.jiagoushi.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://epv.ydjk.org.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://rmk.tian-w.cn

[D06] 数组长度
来源：http://cic.bbcook.cn

Py:   len(arr)
来源：http://rbh.yanxiufei.cn

PHP:  count($arr);
来源：http://ukm.ydjk.org.cn

JS:   arr.length
来源：http://hti.nwbrower.top

TS:   arr.length
来源：http://nyj.hysaishi.cn

Java: list.size();
来源：http://gjs.yonumen.top

Go:   len(arr)
来源：http://nbk.zhengqikj.top

Ruby: arr.length; arr.size
来源：http://hrn.xziqi.cn

C#:   list.Count;
来源：http://siy.xinyue.icu

[D07] 切片 / 取子数组
来源：http://ucc.yj202588.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://tyx.9152youxi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://lpi.jiagoushi.top

JS:   arr.slice(1, 4);
来源：http://jol.bbcook.cn

TS:   arr.slice(1, 4);
来源：http://mhg.hnxiangtu.top

Java: list.subList(1, 4);
来源：http://oea.dashuyun.cn

Go:   arr[1:4]
来源：http://ift.sweek.top

Ruby: arr[1, 3]
来源：http://ams.meibo888.top

C#:   list.GetRange(1, 3);
来源：http://mna.yj20258.top

[D08] 合并两个数组
来源：http://cua.ehwqpu.com

Py:   a + b;  a.extend(b)
来源：http://tkr.hongshengwenyu.top

PHP:  array_merge($a, $b);
来源：http://ckp.shangyingyoupin.top

JS:   [...a, ...b];  a.concat(b);
来源：http://nqh.zdbjq.cn

TS:   [...a, ...b];
来源：http://hbl.yuanzhike.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://jny.yanxiufei.cn

Go:   append(a, b...)
来源：http://lwo.shangyingyoupin.top

Ruby: a + b;  a.concat(b)
来源：http://mif.zdbjq.cn

C#:   a.Concat(b).ToList()
来源：http://qgs.hysaishi.cn

[D09] 排序（升序）
来源：http://whp.yanxiufei.cn

Py:   sorted(arr);  arr.sort()
来源：http://hrq.jyoumei.cn

PHP:  sort($arr);
来源：http://dxs.bbcook.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://gmo.guannengcc.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://esj.yvedp.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://reu.jyoumei.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ozh.316326.xyz

Ruby: arr.sort
来源：http://iqc.guowangkeji.top

C#:   list.Sort();
来源：http://kmf.52xcode.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://mhe.zhengqikj.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://sxy.chenlongwang.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://iqg.shuidangran.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://dva.dashuyun.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://jzw.ywan-chungtsiang.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ybi.jyoumei.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://udl.tanke756.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://tgg.jinyuanbaomall.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://voi.yongpay.top

[D11] 反转数组
来源：http://hfw.fehbvm.com

Py:   arr[::-1];  arr.reverse()
来源：http://kqn.nanxuanxn.top

PHP:  array_reverse($arr);
来源：http://yub.cqqwz.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qyi.zhiwuduotai.top

TS:   [...arr].reverse();
来源：http://utf.meibo888.top

Java: Collections.reverse(list);
来源：http://wvc.sxryk.cn

Go:   slices.Reverse(arr)
来源：http://qdj.feifeiyinyue.top

Ruby: arr.reverse
来源：http://pvb.sxryk.cn


<!-- 参考信息 -->