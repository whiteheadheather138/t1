代发 wailian999

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://vuj.kuanghao11.cn

Ruby: (0...10).step(2).to_a
来源：http://ppz.kuanghao11.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://myi.yanxiufei.cn

[B12] 跳出多层循环
来源：http://uac.zdqjudy.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://nje.nanxuanxn.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://cnm.jlsjyb.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://zqx.aizwys.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://fjg.yfazqb.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://xdc.yongpay.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ngg.zdbjq.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://cdz.xinyue.icu

C#:   # 无标签：用 goto label 或布尔标志
来源：http://pvy.nanxuanxn.top

[B13] 判断是否为数字
来源：http://uoz.redwolf501.top

Py:   isinstance(x, (int, float))
来源：http://hem.yvedp.cn

PHP:  is_numeric($x)
来源：http://obl.jlsjyb.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://eao.yanxiufei.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rob.quarkkingdee.top

Java: x instanceof Number
来源：http://pqz.hywenlv.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ntn.zhongyouzk.top

Ruby: x.is_a?(Numeric)
来源：http://ycd.daria6918.cn

C#:   x is int or double or decimal
来源：http://lkd.guowangkeji.top

[B14] 判断值是否在集合内
来源：http://rng.yongpay.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://urv.yonumen.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://kki.jqgufenzy.top

JS:   [1, 2, 3].includes(x)
来源：http://ket.jinqigfzy.top

TS:   [1, 2, 3].includes(x)
来源：http://afz.tianlin.xyz

Java: List.of(1, 2, 3).contains(x)
来源：http://pur.yj202588.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://fyw.jinqigufen.top

Ruby: [1, 2, 3].include?(x)
来源：http://nwc.ivvv.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ntg.meibo888.top

[B15] 布尔运算与取反
来源：http://zdb.jinghuilouyu.cn

Py:   a and b or not c
来源：http://ual.chenzaomai.com

PHP:  $a && $b || !$c
来源：http://ukz.shzxlz.cn

JS:   a && b || !c
来源：http://vvj.xingfuxueyuan.xyz

TS:   a && b || !c
来源：http://mph.havefunace.top

Java: a && b || !c
来源：http://wdr.tanke756.top

Go:   a && b || !c
来源：http://zid.jinyuanbaomall.cn

Ruby: a && b || !c
来源：http://nbb.zycfv.cn

C#:   a && b || !c
来源：http://nsp.smart0.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://eky.hongshengwenyu.top

Py:   if not data: return
来源：http://yzh.daxiang520.top

PHP:  if (!$data) { return; }
来源：http://jwc.zhongyouzk.top

JS:   if (!data) return;
来源：http://xgh.nanxinkj.top

TS:   if (!data) return;
来源：http://bda.fzhhl.top

Java: if (data == null) return;
来源：http://ntx.gogol.net.cn

Go:   if data == nil { return }
来源：http://nbn.jqgfzy.top

Ruby: return if data.nil?
来源：http://qty.yangfankeji.com

C#:   if (data == null) return;
来源：http://yit.shangyingyoupin.top

================================================================================
来源：http://gdr.fengsongda.top

C. 函数与作用域
来源：http://uns.ydjk.org.cn

================================================================================
来源：http://fga.xinyue.icu

[C01] 定义函数
来源：http://akb.zhongyouzk.top

Py:   def add(a, b): return a + b
来源：http://tzf.feifeiyinyue.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://oii.yfazqb.com

JS:   function add(a, b) { return a + b; }
来源：http://nbj.iojbl.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hjv.xuanzx.com

Java: static int add(int a, int b) { return a + b; }
来源：http://vqi.shanyushiyangtech.top

Go:   func add(a, b int) int { return a + b }
来源：http://mig.zhaomingkeji.xyz

Ruby: def add(a, b); a + b; end
来源：http://gth.yj20258.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://phw.zdbjq.cn

[C02] 默认参数
来源：http://qwc.zdbjq.cn

Py:   def greet(name="World"): return name
来源：http://bgd.jianghu66.top

PHP:  function greet($name = "World") { return $name; }
来源：http://mrx.quarkkingdee.top

JS:   function greet(name = "World") { return name; }
来源：http://nuw.yongpay.top

TS:   function greet(name: string = "World") { return name; }
来源：http://mlc.dashuyun.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://hgv.gotoacloud.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ily.ybcxt.top

Ruby: def greet(name = "World") = name
来源：http://sze.fzhhl.top

C#:   string Greet(string name = "World") => name;
来源：http://txk.yangfankeji.com

[C03] 可变参数
来源：http://dkh.redwolf501.top

Py:   def total(*args): return sum(args)
来源：http://zze.pycfn.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://bce.cdnleiting.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ibt.shzxlz.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ylj.guannengcc.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://umz.shangyingyoupin.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://jwa.jianghu66.top

Ruby: def total(*nums); nums.sum; end
来源：http://stw.chenjidiqi.icu

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://jej.jiagoushi.top

[C04] 命名参数 / 关键字参数
来源：http://kqz.316326.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hxq.ybcxt.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://dhz.gogol.net.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://lxr.9152youxi.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://yjv.bjfxy.top

Java: // 无：用 Builder 模式或 record
来源：http://lmw.gaohongyu789.top

Go:   // 无：用配置结构体参数
来源：http://pef.zhixingplan.top

Ruby: f(a: 1, b: 2)
来源：http://ciz.hysaishi.cn

C#:   f(a: 1, b: 2)
来源：http://sjb.ydjk.org.cn

[C05] 返回多个值
来源：http://fbn.chenlongwang.top

Py:   return a, b
来源：http://bbb.pengpengdd.cyou

PHP:  return [$a, $b];
来源：http://ohs.bbcook.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://hdx.jinqigufen.top

TS:   return { a, b };
来源：http://xmr.sxryk.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://qxm.zhoulong.xyz

Go:   return a, b
来源：http://hff.wangshuangyany.cn

Ruby: return a, b
来源：http://lag.fktsv.cn

C#:   return (a, b);              // ValueTuple
来源：http://fmj.xingfuxueyuan.xyz

[C06] 匿名函数 / lambda
来源：http://eht.gotoacloud.top

Py:   square = lambda x: x * x
来源：http://dfj.gzhubu.top

PHP:  $square = fn($x) => $x * $x;
来源：http://wai.yvedp.cn

JS:   const square = x => x * x;
来源：http://dhx.ydzc1.top

TS:   const square = (x: number): number => x * x;
来源：http://lcd.fktsv.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hev.redwolf501.top

Go:   sq := func(x int) int { return x * x }
来源：http://mus.tanke756.top

Ruby: square = ->(x) { x * x }
来源：http://npc.guannengcc.top

C#:   Func<int, int> square = x => x * x;
来源：http://uzx.shuidangran.top

[C07] 把函数作为参数传入
来源：http://avg.tianlin.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://pxt.ivvv.top

PHP:  array_map("strtoupper", $arr);
来源：http://tpu.hesvh.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ykq.tanke756.top

TS:   arr.map(String)
来源：http://tza.xuetiantiany.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://zoz.tian-w.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://phs.shzxlz.cn

Ruby: arr.map(&:upcase)
来源：http://jbb.svipenyu.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://hjw.cdnleiting.top

[C08] 闭包
来源：http://equ.daxiang520.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wfz.hcnkem.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://chx.xuetiantiany.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qxb.guowangkeji.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://xwg.iojbl.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://bmi.wangshuangyany.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://yud.vqdsnc.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://qda.sufxvd.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wtm.bbcook.cn

[C09] 递归
来源：http://nzt.fzhhl.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://zxi.sufxvd.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://dus.fzhhl.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ppm.daxiang520.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rss.hysaishi.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ffm.shanyushiyangtech.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hxo.yongpay.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://kmx.iojbl.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ruq.nanxuanxn.top

[C10] 变量作用域
来源：http://mmu.wangshuangyany.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://aki.yongpay.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://aok.tanke756.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://fbz.nanxinkj.top

TS:   同 JS
来源：http://oso.shzxlz.cn

Java: 方法内为块级作用域
来源：http://amf.jinqigufen.top

Go:   花括号块级作用域
来源：http://ncr.jinqigfzy.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://icv.tian-w.cn

C#:   块级作用域
来源：http://cgv.jianghu66.top

[C11] 模块导入与导出
来源：http://wrs.yj20258.top

Py:   from module import func
来源：http://zqu.ydjk.org.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://itd.fehbvm.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://ela.hysaishi.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://dkz.cashguo.top

Java: import java.util.List;
来源：http://vst.daxiang520.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://axa.nanxinkj.top

Ruby: require "json"; require_relative "./util"
来源：http://bpi.ydzc1.top

C#:   using System.Text;
来源：http://wut.hesvh.cn

[C12] 立即执行函数 IIFE
来源：http://ibb.jlsjyb.cn

Py:   (lambda: print("run"))()
来源：http://bvf.daria6918.cn

PHP:  (function () { echo "run"; })();
来源：http://qxg.yangfankeji.com

JS:   (() => { console.log("run"); })();
来源：http://mey.meibo888.top

TS:   (() => { console.log("run"); })();
来源：http://voj.yuxming.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hvl.hnqzz.top

Go:   func() { fmt.Println("run") }()
来源：http://kgv.gotoacloud.top

Ruby: -> { puts "run" }.call
来源：http://fhq.yueranfly.top

C#:   // 无 IIFE：用静态构造函数
来源：http://ydk.shuidangran.top

[C13] 类型声明 / 类型注解
来源：http://chr.jqgfzy.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://okn.shanyushiyangkeji.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ero.epnwcf.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://bke.vqdsnc.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yem.yuanzhike.top

Java: int add(int a, int b) { return a + b; }
来源：http://toc.chenjidiqi.icu

Go:   func add(a, b int) int
来源：http://fxi.xuanzx.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ohl.yj202588.top

C#:   int Add(int a, int b) => a + b;
来源：http://gla.cheryme.top

[C14] 泛型函数
来源：http://ygt.cashguo.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://vue.nanxuanxn.top

PHP:  // 无泛型
来源：http://vpn.chenzaomai.com

JS:   // 无泛型
来源：http://jqs.smart0.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://czv.zhengqikj.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://eqd.tarul.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://xfg.hywenlv.cn

Ruby: # 无泛型
来源：http://jdd.tianlin.xyz

C#:   static T First<T>(List<T> items) => items[0];
来源：http://nmg.gogol.net.cn

[C15] 解构 / 展开参数
来源：http://pct.gogol.net.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ojf.shuidangran.top

PHP:  [$a, $b] = $pair;
来源：http://bmz.wangshuangyany.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ktz.yj202588.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://nmx.shangyingyoupin.top

Java: // 无解构
来源：http://pta.jinqigfzy.top

Go:   // 无解构
来源：http://pzi.jiagoushi.top

Ruby: a, b = pair
来源：http://lgx.nanxinkj.top

C#:   var (a, b) = pair;
来源：http://svt.smart0.xyz

[C16] 函数 / 方法重载
来源：http://fjp.hnqzz.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wky.jyoumei.cn

PHP:  // 无重载
来源：http://aik.pycfn.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://civ.jyoumei.cn

TS:   // 用联合类型或重载签名声明
来源：http://sgx.gaohongyu789.top

Java: void f(int a) {}  void f(String a) {}
来源：http://abi.iojbl.cn

Go:   // 无重载：用不同函数名
来源：http://fxx.tanke756.top

Ruby: # 无重载：靠动态参数
来源：http://rrr.jinghuilouyu.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://zml.iojbl.cn

================================================================================
来源：http://hgq.zdbjq.cn

D. 数组 / 列表 / 集合
来源：http://fuy.cdnleiting.top

================================================================================
来源：http://tbr.yongpay.top

[D01] 创建数组 / 列表
来源：http://eos.hfpthk.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://zkw.sufxvd.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://yra.jinghuilouyu.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://sor.shangyingyoupin.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://boc.hongshengwenyu.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ofn.wangshuangyany.cn

Go:   arr := []int{1, 2, 3}
来源：http://sdq.jinqigufen.top

Ruby: arr = [1, 2, 3]
来源：http://rvw.zhixingplan.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://gre.vehdjk.com

[D02] 追加元素到末尾
来源：http://oma.zhoulong.xyz

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mon.sjlbkw.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://xjj.cdnleiting.top

JS:   arr.push(4);
来源：http://jod.yueranfly.top

TS:   arr.push(4);
来源：http://wea.quarkkingdee.top

Java: list.add(4);
来源：http://ssf.cqqwz.cn

Go:   arr = append(arr, 4)
来源：http://dhi.tian-w.cn

Ruby: arr << 4; arr.push(5)
来源：http://skw.fehbvm.com

C#:   list.Add(4);
来源：http://lfz.yj202588.top

[D03] 在指定位置插入元素
来源：http://ajk.cqqwz.cn

Py:   arr.insert(0, 0)
来源：http://prr.jyoumei.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ofk.hywenlv.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hta.bjfxy.top

TS:   arr.splice(0, 0, 0);
来源：http://zjh.snrcjt.cn

Java: list.add(0, 0);
来源：http://qsc.nwbrower.top

Go:   arr = append([]int{0}, arr...)
来源：http://akh.ydjk.org.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://xxc.smart0.xyz

C#:   list.Insert(0, 0);
来源：http://swi.cucudq.cn

[D04] 删除元素
来源：http://dog.cdnleiting.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://jfd.ybcxt.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ggp.sweek.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://fyl.hysaishi.cn

TS:   arr.splice(0, 1);
来源：http://yre.hongshengwenyu.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://piy.birdmap.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://xnk.iojbl.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://zob.0kj1m.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://tpv.zhoulong.xyz

[D05] 访问与修改元素
来源：http://cao.iojbl.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://yuk.sysykeji.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ntn.shanyushiyangkeji.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hok.hywenlv.cn

TS:   arr[0]; arr.at(-1);
来源：http://nlf.xziqi.cn

Java: list.get(0); list.set(0, 9);
来源：http://ras.snrcjt.cn

Go:   arr[0]; arr[0] = 9
来源：http://cra.hfpthk.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mql.yuxming.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://rkz.pengpengdd.cyou

[D06] 数组长度
来源：http://waq.cqqwz.cn

Py:   len(arr)
来源：http://nyp.jqgufenzy.top

PHP:  count($arr);
来源：http://cyk.xuetiantiany.cn

JS:   arr.length
来源：http://fhn.yvedp.cn

TS:   arr.length
来源：http://yko.epnwcf.com

Java: list.size();
来源：http://ezh.cheryme.top

Go:   len(arr)
来源：http://wzk.ehwqpu.com

Ruby: arr.length; arr.size
来源：http://xgr.ywan-chungtsiang.top

C#:   list.Count;
来源：http://zvy.hywenlv.cn

[D07] 切片 / 取子数组
来源：http://men.aizwys.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://fvd.yj202588.top

PHP:  array_slice($arr, 1, 3);
来源：http://oie.smart0.xyz

JS:   arr.slice(1, 4);
来源：http://wse.52xcode.cn

TS:   arr.slice(1, 4);
来源：http://txj.hesvh.cn

Java: list.subList(1, 4);
来源：http://pmo.chenlongwang.top

Go:   arr[1:4]
来源：http://wxu.sjlbkw.cn

Ruby: arr[1, 3]
来源：http://boo.316326.xyz

C#:   list.GetRange(1, 3);
来源：http://plo.haohaochexian.top

[D08] 合并两个数组
来源：http://hyo.jinqigufen.top

Py:   a + b;  a.extend(b)
来源：http://miu.cucudq.cn

PHP:  array_merge($a, $b);
来源：http://btd.nanxinkj.top

JS:   [...a, ...b];  a.concat(b);
来源：http://yun.shanyushiyangtech.top

TS:   [...a, ...b];
来源：http://gfb.tarul.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://zgo.nanxinkj.top

Go:   append(a, b...)
来源：http://bsi.zhaomingkeji.xyz

Ruby: a + b;  a.concat(b)
来源：http://hvr.yuxming.cn

C#:   a.Concat(b).ToList()
来源：http://tia.xuanzx.com

[D09] 排序（升序）
来源：http://rkd.mhx1999.top

Py:   sorted(arr);  arr.sort()
来源：http://nmu.gzhubu.top

PHP:  sort($arr);
来源：http://eek.shangyingyoupin.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://bld.cheryme.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://wdg.yj202588.top

Java: Collections.sort(list);  list.sort(null);
来源：http://duo.yongpay.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qow.sweek.top

Ruby: arr.sort
来源：http://aev.jyoumei.cn

C#:   list.Sort();
来源：http://agt.cheryme.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://jvl.yfazqb.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://bij.ivvv.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fqu.dashuyun.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://xbd.zhaomingkeji.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ktu.dianchejie.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://der.epnwcf.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ptw.iojbl.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://epo.hammf.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://irt.guowangkeji.top

[D11] 反转数组
来源：http://ouu.andypj.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://qob.guannengcc.top

PHP:  array_reverse($arr);
来源：http://wwa.wangdashe.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://yol.9152youxi.cn

TS:   [...arr].reverse();
来源：http://mdx.zhaomingkeji.xyz

Java: Collections.reverse(list);
来源：http://kdp.bjfxy.top

Go:   slices.Reverse(arr)
来源：http://npf.bjfxy.top

Ruby: arr.reverse
来源：http://cpu.gogol.net.cn

C#:   list.Reverse();
来源：http://noa.ppjwa.cn

[D12] 查找元素下标
来源：http://vsw.52xcode.cn

Py:   arr.index(x);  x in arr
来源：http://nzk.tian-w.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ftp.xingfuxueyuan.xyz


<!-- 参考信息 -->