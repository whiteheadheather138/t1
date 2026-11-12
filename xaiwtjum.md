代发 wailian999

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://zat.haohaochexian.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://rye.chenjidiqi.icu

[B11] 生成数字序列 / 区间
来源：http://zyo.ehwqpu.com

Py:   list(range(0, 10, 2))
来源：http://zzg.hywenlv.cn

PHP:  range(0, 10, 2);
来源：http://oyc.bbcook.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://oxr.sweek.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bwt.jlsjyb.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://zac.cucudq.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://cab.0kj1m.cn

Ruby: (0...10).step(2).to_a
来源：http://trx.xylfe.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://nyq.gaohongyu789.top

[B12] 跳出多层循环
来源：http://sxz.iojbl.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://zxs.cucudq.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://oyu.shanyushiyangkeji.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://bch.hfpthk.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hqx.aizwys.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://rgo.yueranfly.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://tws.smart0.xyz

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mrt.jqgfzy.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://sel.xinyue.icu

[B13] 判断是否为数字
来源：http://svp.shanyushiyangkeji.top

Py:   isinstance(x, (int, float))
来源：http://tgu.hysaishi.cn

PHP:  is_numeric($x)
来源：http://qek.chenlongwang.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kzp.nanxinkj.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zzi.jqgufenzy.top

Java: x instanceof Number
来源：http://znn.zhiwuduotai.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://zqa.hywenlv.cn

Ruby: x.is_a?(Numeric)
来源：http://ybu.uphjek.com

C#:   x is int or double or decimal
来源：http://cya.zhixingplan.top

[B14] 判断值是否在集合内
来源：http://cyv.gzhubu.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://rln.ivvv.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://kyy.hfpthk.cn

JS:   [1, 2, 3].includes(x)
来源：http://rjm.meibo888.top

TS:   [1, 2, 3].includes(x)
来源：http://wvk.sufxvd.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://kso.jyoumei.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://oto.jqgufenzy.top

Ruby: [1, 2, 3].include?(x)
来源：http://yqu.zhijiandao.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://lav.ybcxt.top

[B15] 布尔运算与取反
来源：http://til.tanke756.top

Py:   a and b or not c
来源：http://ukj.dianchejie.cn

PHP:  $a && $b || !$c
来源：http://qkn.jqgfzy.top

JS:   a && b || !c
来源：http://epi.fzhhl.top

TS:   a && b || !c
来源：http://wov.tarul.cn

Java: a && b || !c
来源：http://zgp.hysaishi.cn

Go:   a && b || !c
来源：http://uoh.hnxiangtu.top

Ruby: a && b || !c
来源：http://yay.jinqigfzy.top

C#:   a && b || !c
来源：http://qng.yuxming.cn

[B16] 卫语句：不满足条件提前返回
来源：http://rxc.zdbjq.cn

Py:   if not data: return
来源：http://jmx.yonumen.top

PHP:  if (!$data) { return; }
来源：http://den.gzhubu.top

JS:   if (!data) return;
来源：http://uwp.cdnleiting.top

TS:   if (!data) return;
来源：http://dgn.gzhubu.top

Java: if (data == null) return;
来源：http://bzo.iojbl.cn

Go:   if data == nil { return }
来源：http://rfq.shuidangran.top

Ruby: return if data.nil?
来源：http://efv.xinyue.icu

C#:   if (data == null) return;
来源：http://jws.smart0.xyz

================================================================================
来源：http://bhy.nanxinkj.top

C. 函数与作用域
来源：http://fjj.hysaishi.cn

================================================================================
来源：http://vys.ydjk.org.cn

[C01] 定义函数
来源：http://ooc.gogol.net.cn

Py:   def add(a, b): return a + b
来源：http://oia.sufxvd.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tvz.wangshuangyany.cn

JS:   function add(a, b) { return a + b; }
来源：http://gzv.jinyuanbaomall.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fjr.hywenlv.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://cin.iojbl.cn

Go:   func add(a, b int) int { return a + b }
来源：http://kbj.jianghu66.top

Ruby: def add(a, b); a + b; end
来源：http://uzs.xinyue.icu

C#:   static int Add(int a, int b) { return a + b; }
来源：http://yiq.meibo888.top

[C02] 默认参数
来源：http://tsn.jlsjyb.cn

Py:   def greet(name="World"): return name
来源：http://cmu.ivvv.top

PHP:  function greet($name = "World") { return $name; }
来源：http://rbz.ydjk.org.cn

JS:   function greet(name = "World") { return name; }
来源：http://rof.ctjpmb.com

TS:   function greet(name: string = "World") { return name; }
来源：http://qni.fanxiaobao.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://cwo.xingfuxueyuan.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ghb.hesvh.cn

Ruby: def greet(name = "World") = name
来源：http://ylq.yonumen.top

C#:   string Greet(string name = "World") => name;
来源：http://vqg.guannengcc.top

[C03] 可变参数
来源：http://jsq.hcnkem.com

Py:   def total(*args): return sum(args)
来源：http://til.guowangkeji.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://pjp.uphjek.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://otd.hammf.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://nva.tianlin.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://kol.pengpengdd.cyou

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ymd.ydzc1.top

Ruby: def total(*nums); nums.sum; end
来源：http://tqd.shuidangran.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ltg.hesvh.cn

[C04] 命名参数 / 关键字参数
来源：http://ecp.yuxming.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ksl.wangdashe.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://bwk.jiagoushi.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://cbr.chenzaomai.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://cfm.nwbrower.top

Java: // 无：用 Builder 模式或 record
来源：http://vsh.kuanghao11.cn

Go:   // 无：用配置结构体参数
来源：http://cid.yvedp.cn

Ruby: f(a: 1, b: 2)
来源：http://wxt.meibo888.top

C#:   f(a: 1, b: 2)
来源：http://ptr.feifeiyinyue.top

[C05] 返回多个值
来源：http://vua.chenlongwang.top

Py:   return a, b
来源：http://lux.yueranfly.top

PHP:  return [$a, $b];
来源：http://otf.zhengqikj.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://vzz.xylfe.cn

TS:   return { a, b };
来源：http://gxo.vehdjk.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://lyt.zhiwuduotai.top

Go:   return a, b
来源：http://owu.yvedp.cn

Ruby: return a, b
来源：http://cpp.daxiang520.top

C#:   return (a, b);              // ValueTuple
来源：http://omf.bjfxy.top

[C06] 匿名函数 / lambda
来源：http://kdc.tian-w.cn

Py:   square = lambda x: x * x
来源：http://vot.aizwys.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ofs.fktsv.cn

JS:   const square = x => x * x;
来源：http://pom.ydzc1.top

TS:   const square = (x: number): number => x * x;
来源：http://cxq.zhongyouzk.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wjp.yfazqb.com

Go:   sq := func(x int) int { return x * x }
来源：http://nic.feifeiyinyue.top

Ruby: square = ->(x) { x * x }
来源：http://usg.redwolf501.top

C#:   Func<int, int> square = x => x * x;
来源：http://lsi.meibo888.top

[C07] 把函数作为参数传入
来源：http://lqm.sxryk.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://zcg.sysykeji.top

PHP:  array_map("strtoupper", $arr);
来源：http://wew.ydzc1.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://dau.zhongyouzk.top

TS:   arr.map(String)
来源：http://ove.haohaochexian.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://kui.sysykeji.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://bnk.ydzc1.top

Ruby: arr.map(&:upcase)
来源：http://opo.daxiang520.top

C#:   arr.Select(s => s.ToUpper())
来源：http://sya.birdmap.top

[C08] 闭包
来源：http://caw.ydzc1.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ioj.jyoumei.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://bqj.zhengqikj.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://jww.pengpengdd.cyou

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ofq.yfazqb.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ogg.hcnkem.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mxh.tianlin.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://kcn.wangshuangyany.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://fjz.tianlin.xyz

[C09] 递归
来源：http://qkx.ppjwa.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ioy.vqdsnc.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://rim.bjfxy.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ysz.yj20258.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nmm.tianlin.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://whx.shanyushiyangkeji.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://pug.shangyingyoupin.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://tod.pycfn.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://czq.xinyue.icu

[C10] 变量作用域
来源：http://zso.iojbl.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ajh.kuanghao11.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://tar.sweek.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://npj.9152youxi.cn

TS:   同 JS
来源：http://piu.hnqzz.top

Java: 方法内为块级作用域
来源：http://jmo.cqqwz.cn

Go:   花括号块级作用域
来源：http://enn.hywenlv.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://coi.ybcxt.top

C#:   块级作用域
来源：http://eju.zhengqikj.top

[C11] 模块导入与导出
来源：http://dqd.birdmap.top

Py:   from module import func
来源：http://xqx.sjlbkw.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://vuy.kuanghao11.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://cto.snrcjt.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://nks.yj20258.top

Java: import java.util.List;
来源：http://vdq.hnxiangtu.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://plw.hesvh.cn

Ruby: require "json"; require_relative "./util"
来源：http://jiy.aibaodan.cn

C#:   using System.Text;
来源：http://bxe.yuanzhike.top

[C12] 立即执行函数 IIFE
来源：http://ufm.feifeiyinyue.top

Py:   (lambda: print("run"))()
来源：http://kek.hysaishi.cn

PHP:  (function () { echo "run"; })();
来源：http://krb.dashuyun.cn

JS:   (() => { console.log("run"); })();
来源：http://fit.yuanzhike.top

TS:   (() => { console.log("run"); })();
来源：http://kgh.tian-w.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://kwp.yuxming.cn

Go:   func() { fmt.Println("run") }()
来源：http://pdq.yueranfly.top

Ruby: -> { puts "run" }.call
来源：http://brt.0kj1m.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://gvj.iojbl.cn

[C13] 类型声明 / 类型注解
来源：http://fvv.nwbrower.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wpq.andypj.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ywi.zhaomingkeji.xyz

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ecz.zhijiandao.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xra.snrcjt.cn

Java: int add(int a, int b) { return a + b; }
来源：http://vqy.tianlin.xyz

Go:   func add(a, b int) int
来源：http://tid.bbcook.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://sli.havefunace.top

C#:   int Add(int a, int b) => a + b;
来源：http://nco.hysaishi.cn

[C14] 泛型函数
来源：http://lgq.smart0.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://jho.hammf.cn

PHP:  // 无泛型
来源：http://ldo.yangfankeji.com

JS:   // 无泛型
来源：http://blu.guannengcc.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://pon.epnwcf.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://sja.aizwys.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wip.epnwcf.com

Ruby: # 无泛型
来源：http://yvu.zhoulong.xyz

C#:   static T First<T>(List<T> items) => items[0];
来源：http://pei.sjlbkw.cn

[C15] 解构 / 展开参数
来源：http://dmb.birdmap.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://zbs.yueranfly.top

PHP:  [$a, $b] = $pair;
来源：http://xef.feifeiyinyue.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://buw.kuanghao11.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ahj.ydjk.org.cn

Java: // 无解构
来源：http://dpt.fanxiaobao.xyz

Go:   // 无解构
来源：http://uaq.jyoumei.cn

Ruby: a, b = pair
来源：http://ulo.tianlin.xyz

C#:   var (a, b) = pair;
来源：http://ass.chenzaomai.com

[C16] 函数 / 方法重载
来源：http://ggd.ivvv.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://obp.yuanzhike.top

PHP:  // 无重载
来源：http://vvo.yangfankeji.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://kzu.jinqigufen.top

TS:   // 用联合类型或重载签名声明
来源：http://adk.wangdashe.top

Java: void f(int a) {}  void f(String a) {}
来源：http://bys.vqdsnc.cn

Go:   // 无重载：用不同函数名
来源：http://alw.guannengcc.top

Ruby: # 无重载：靠动态参数
来源：http://pyk.snrcjt.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://joq.zhijiandao.cn

================================================================================
来源：http://kfj.shuidangran.top

D. 数组 / 列表 / 集合
来源：http://mxh.jinqigufen.top

================================================================================
来源：http://wgi.smart0.xyz

[D01] 创建数组 / 列表
来源：http://eyb.xingfuxueyuan.xyz

Py:   arr = [1, 2, 3];  empty = []
来源：http://osi.wangdashe.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://nqu.redwolf501.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://obe.jinqigufen.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://cxa.gotoacloud.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://oym.pycfn.com

Go:   arr := []int{1, 2, 3}
来源：http://ejf.tarul.cn

Ruby: arr = [1, 2, 3]
来源：http://wsi.ehwqpu.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://cxc.birdmap.top

[D02] 追加元素到末尾
来源：http://oxw.zhengqikj.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://vux.epnwcf.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ymo.jinghuilouyu.cn

JS:   arr.push(4);
来源：http://djm.vehdjk.com

TS:   arr.push(4);
来源：http://wao.zhaomingkeji.xyz

Java: list.add(4);
来源：http://qvi.cucudq.cn

Go:   arr = append(arr, 4)
来源：http://rwb.316326.xyz

Ruby: arr << 4; arr.push(5)
来源：http://ayd.daxiang520.top

C#:   list.Add(4);
来源：http://fmb.sufxvd.cn

[D03] 在指定位置插入元素
来源：http://mrt.uphjek.com

Py:   arr.insert(0, 0)
来源：http://hyf.yongpay.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://rqz.tianlin.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://miz.mhx1999.top

TS:   arr.splice(0, 0, 0);
来源：http://vcc.iojbl.cn

Java: list.add(0, 0);
来源：http://piq.epnwcf.com

Go:   arr = append([]int{0}, arr...)
来源：http://lfr.yuxming.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://lis.jianghu66.top

C#:   list.Insert(0, 0);
来源：http://grx.uphjek.com

[D04] 删除元素
来源：http://rfs.mhx1999.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://bkc.fengsongda.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://jic.haohaochexian.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://igv.yonumen.top

TS:   arr.splice(0, 1);
来源：http://pwe.hfpthk.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://izg.fktsv.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://bir.haohaochexian.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hqy.xuanzx.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://zvh.chenzaomai.com

[D05] 访问与修改元素
来源：http://ipo.hfpthk.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wnx.xinyue.icu

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://lxi.dashuyun.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://duo.uphjek.com

TS:   arr[0]; arr.at(-1);
来源：http://ggt.ydzc1.top

Java: list.get(0); list.set(0, 9);
来源：http://leq.ivvv.top

Go:   arr[0]; arr[0] = 9
来源：http://dyy.bjfxy.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://oum.nanxinkj.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://xns.sxryk.cn

[D06] 数组长度
来源：http://jry.sysykeji.top

Py:   len(arr)
来源：http://nhf.xziqi.cn

PHP:  count($arr);
来源：http://caf.jianghu66.top

JS:   arr.length
来源：http://yjc.xuetiantiany.cn

TS:   arr.length
来源：http://xxm.nanxuanxn.top

Java: list.size();
来源：http://efo.xinyue.icu

Go:   len(arr)
来源：http://vvc.cqqwz.cn

Ruby: arr.length; arr.size
来源：http://oem.svipenyu.cn

C#:   list.Count;
来源：http://kxa.hywenlv.cn

[D07] 切片 / 取子数组
来源：http://rco.yvedp.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://psp.vehdjk.com

PHP:  array_slice($arr, 1, 3);
来源：http://coj.jianghu66.top

JS:   arr.slice(1, 4);
来源：http://jxr.ydzc1.top

TS:   arr.slice(1, 4);
来源：http://hxd.zhixingplan.top

Java: list.subList(1, 4);
来源：http://oaa.zhongyouzk.top

Go:   arr[1:4]
来源：http://eml.cucudq.cn

Ruby: arr[1, 3]
来源：http://wii.hnxiangtu.top

C#:   list.GetRange(1, 3);
来源：http://ayv.sxryk.cn

[D08] 合并两个数组
来源：http://guc.yonumen.top

Py:   a + b;  a.extend(b)
来源：http://rax.ppjwa.cn

PHP:  array_merge($a, $b);
来源：http://bkd.tanke756.top

JS:   [...a, ...b];  a.concat(b);
来源：http://iuf.iojbl.cn

TS:   [...a, ...b];
来源：http://tys.sufxvd.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wdv.cdnleiting.top

Go:   append(a, b...)
来源：http://six.shanyushiyangtech.top

Ruby: a + b;  a.concat(b)
来源：http://ulx.zhoulong.xyz

C#:   a.Concat(b).ToList()
来源：http://pyi.9152youxi.cn

[D09] 排序（升序）
来源：http://mtz.xinyue.icu

Py:   sorted(arr);  arr.sort()
来源：http://jmv.yvedp.cn

PHP:  sort($arr);
来源：http://jvc.yfazqb.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://nbc.xuanzx.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://ceu.gotoacloud.top

Java: Collections.sort(list);  list.sort(null);
来源：http://zpv.daria6918.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://dxg.cqqwz.cn

Ruby: arr.sort
来源：http://hsy.aibaodan.cn

C#:   list.Sort();
来源：http://vdn.yj20258888.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://cku.gaohongyu789.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://cwm.hammf.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dka.chenzaomai.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wjt.mhx1999.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://nas.daxiang520.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hrg.yj20258888.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://suz.tanke756.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ssu.ctjpmb.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://epw.xuanzx.com

[D11] 反转数组
来源：http://qls.jiagoushi.top

Py:   arr[::-1];  arr.reverse()
来源：http://der.shangyingyoupin.top

PHP:  array_reverse($arr);
来源：http://uvo.yueranfly.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://fsl.fanxiaobao.xyz


<!-- 参考信息 -->