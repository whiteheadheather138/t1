代发 wailian999

PHP:  range(0, 10, 2);
来源：http://bjy.ivvv.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qlt.jinqigufen.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://uqj.sjlbkw.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ljo.gotoacloud.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://rrf.cucudq.cn

Ruby: (0...10).step(2).to_a
来源：http://srq.jlsjyb.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://okm.zdbjq.cn

[B12] 跳出多层循环
来源：http://jry.tarul.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://lkb.cucudq.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://jxa.svipenyu.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://lfx.yanxiufei.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://iqn.shzxlz.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ijg.hcnkem.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://tay.yj202588.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://nbu.aizwys.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://rbn.zhengqikj.top

[B13] 判断是否为数字
来源：http://fpl.jiagoushi.top

Py:   isinstance(x, (int, float))
来源：http://sto.sjlbkw.cn

PHP:  is_numeric($x)
来源：http://tcj.sweek.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ieg.fengsongda.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mks.sysykeji.top

Java: x instanceof Number
来源：http://tbf.fzhhl.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://lnz.dianchejie.cn

Ruby: x.is_a?(Numeric)
来源：http://qqr.yanxiufei.cn

C#:   x is int or double or decimal
来源：http://zqh.havefunace.top

[B14] 判断值是否在集合内
来源：http://tli.nanxuanxn.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://zis.fehbvm.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://lun.fehbvm.com

JS:   [1, 2, 3].includes(x)
来源：http://idn.tian-w.cn

TS:   [1, 2, 3].includes(x)
来源：http://fog.fehbvm.com

Java: List.of(1, 2, 3).contains(x)
来源：http://vwc.guannengcc.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://imr.zdbjq.cn

Ruby: [1, 2, 3].include?(x)
来源：http://yjs.jinghuilouyu.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://gkb.0kj1m.cn

[B15] 布尔运算与取反
来源：http://fes.yfazqb.com

Py:   a and b or not c
来源：http://gap.mhx1999.top

PHP:  $a && $b || !$c
来源：http://bsv.yueranfly.top

JS:   a && b || !c
来源：http://ygi.dianchejie.cn

TS:   a && b || !c
来源：http://new.fzhhl.top

Java: a && b || !c
来源：http://wfk.zdqjudy.top

Go:   a && b || !c
来源：http://qeh.jinyuanbaomall.cn

Ruby: a && b || !c
来源：http://ltz.yvedp.cn

C#:   a && b || !c
来源：http://thy.zdbjq.cn

[B16] 卫语句：不满足条件提前返回
来源：http://quz.gzhubu.top

Py:   if not data: return
来源：http://web.cqqwz.cn

PHP:  if (!$data) { return; }
来源：http://ler.tarul.cn

JS:   if (!data) return;
来源：http://nzs.jqgufenzy.top

TS:   if (!data) return;
来源：http://iha.cucudq.cn

Java: if (data == null) return;
来源：http://hwc.hnqzz.top

Go:   if data == nil { return }
来源：http://ele.cqqwz.cn

Ruby: return if data.nil?
来源：http://uvx.chenzaomai.com

C#:   if (data == null) return;
来源：http://rft.shuidangran.top

================================================================================
来源：http://ioo.feifeiyinyue.top

C. 函数与作用域
来源：http://adc.zdqjudy.top

================================================================================
来源：http://fgj.quarkkingdee.top

[C01] 定义函数
来源：http://xju.birdmap.top

Py:   def add(a, b): return a + b
来源：http://zcx.sysykeji.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://djr.jinqigfzy.top

JS:   function add(a, b) { return a + b; }
来源：http://dmu.zdbjq.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dkk.sufxvd.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://gpd.shangyingyoupin.top

Go:   func add(a, b int) int { return a + b }
来源：http://aku.316326.xyz

Ruby: def add(a, b); a + b; end
来源：http://fvh.nanxinkj.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://kdg.sweek.top

[C02] 默认参数
来源：http://vwx.yanxiufei.cn

Py:   def greet(name="World"): return name
来源：http://skv.cqqwz.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://gaw.haohaochexian.top

JS:   function greet(name = "World") { return name; }
来源：http://cle.sjlbkw.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://hwk.cashguo.top

Java: // 无默认参数：方法重载或 Optional
来源：http://kvc.fengsongda.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://jml.aizwys.cn

Ruby: def greet(name = "World") = name
来源：http://aka.hongshengwenyu.top

C#:   string Greet(string name = "World") => name;
来源：http://hjs.daxiang520.top

[C03] 可变参数
来源：http://yfo.zdqjudy.top

Py:   def total(*args): return sum(args)
来源：http://xjo.ppjwa.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hti.aizwys.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ipt.hammf.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://jjk.yangfankeji.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://qwa.feifeiyinyue.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://nbw.yj20258.top

Ruby: def total(*nums); nums.sum; end
来源：http://hnh.c1oappe.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://gvo.ctjpmb.com

[C04] 命名参数 / 关键字参数
来源：http://lca.ybcxt.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://znk.52xcode.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xrx.tianlin.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://zzf.haohaochexian.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://sfj.hfpthk.cn

Java: // 无：用 Builder 模式或 record
来源：http://npj.316326.xyz

Go:   // 无：用配置结构体参数
来源：http://sbn.tanke756.top

Ruby: f(a: 1, b: 2)
来源：http://xal.haohaochexian.top

C#:   f(a: 1, b: 2)
来源：http://yhq.zhoulong.xyz

[C05] 返回多个值
来源：http://nls.pengpengdd.cyou

Py:   return a, b
来源：http://ncy.yanxiufei.cn

PHP:  return [$a, $b];
来源：http://mga.bbcook.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://pua.cashguo.top

TS:   return { a, b };
来源：http://evz.hcnkem.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://vuo.fengsongda.top

Go:   return a, b
来源：http://kmo.havefunace.top

Ruby: return a, b
来源：http://tmw.cdnleiting.top

C#:   return (a, b);              // ValueTuple
来源：http://fnm.ywan-chungtsiang.top

[C06] 匿名函数 / lambda
来源：http://fey.cucudq.cn

Py:   square = lambda x: x * x
来源：http://qdt.xziqi.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://otw.tanke756.top

JS:   const square = x => x * x;
来源：http://jfe.hfpthk.cn

TS:   const square = (x: number): number => x * x;
来源：http://vmx.haohaochexian.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://kae.ywan-chungtsiang.top

Go:   sq := func(x int) int { return x * x }
来源：http://gea.yj20258.top

Ruby: square = ->(x) { x * x }
来源：http://fuc.ppjwa.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ptg.yueranfly.top

[C07] 把函数作为参数传入
来源：http://crr.xingfuxueyuan.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://idx.tianlin.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://xjj.redwolf501.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hik.zhongyouzk.top

TS:   arr.map(String)
来源：http://tyy.xuetiantiany.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://tzg.sweek.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ztg.316326.xyz

Ruby: arr.map(&:upcase)
来源：http://hjo.0kj1m.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ahd.jinyuanbaomall.cn

[C08] 闭包
来源：http://kyd.sysykeji.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://iek.hesvh.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://uyo.vqdsnc.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://uvq.fehbvm.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mkq.jqgfzy.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://olo.hysaishi.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://unh.yueranfly.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://xie.hammf.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://gxb.hfpthk.cn

[C09] 递归
来源：http://yjk.zhijiandao.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://kik.chenlongwang.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ffq.birdmap.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wke.chenlongwang.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ail.fzhhl.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://rtq.zycfv.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mqf.zhaomingkeji.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mct.bbcook.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ywe.fanxiaobao.xyz

[C10] 变量作用域
来源：http://oma.snrcjt.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://frb.jiagoushi.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://iyn.jinqigufen.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://egq.wangshuangyany.cn

TS:   同 JS
来源：http://ucs.ehwqpu.com

Java: 方法内为块级作用域
来源：http://ric.fanxiaobao.xyz

Go:   花括号块级作用域
来源：http://quv.jinyuanbaomall.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://yjp.ydjk.org.cn

C#:   块级作用域
来源：http://txg.ydzc1.top

[C11] 模块导入与导出
来源：http://yxe.yangfankeji.com

Py:   from module import func
来源：http://xvq.pengpengdd.cyou

PHP:  require "file.php";  或 use App\Service;
来源：http://pxm.quarkkingdee.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://zdd.kuanghao11.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://oaw.tanke756.top

Java: import java.util.List;
来源：http://aef.jinqigfzy.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://pzl.ctjpmb.com

Ruby: require "json"; require_relative "./util"
来源：http://wbg.shuidangran.top

C#:   using System.Text;
来源：http://xgi.jqgufenzy.top

[C12] 立即执行函数 IIFE
来源：http://pfh.ydzc1.top

Py:   (lambda: print("run"))()
来源：http://pzz.jqgfzy.top

PHP:  (function () { echo "run"; })();
来源：http://yia.gzhubu.top

JS:   (() => { console.log("run"); })();
来源：http://yri.shanyushiyangtech.top

TS:   (() => { console.log("run"); })();
来源：http://ztj.0kj1m.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://vlm.bjfxy.top

Go:   func() { fmt.Println("run") }()
来源：http://kfu.zhixingplan.top

Ruby: -> { puts "run" }.call
来源：http://iqy.zhongyouzk.top

C#:   // 无 IIFE：用静态构造函数
来源：http://dzm.sjlbkw.cn

[C13] 类型声明 / 类型注解
来源：http://yue.hysaishi.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://jaw.nanxinkj.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cev.bjfxy.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://eyw.hysaishi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lcz.shanyushiyangkeji.top

Java: int add(int a, int b) { return a + b; }
来源：http://rky.yuanzhike.top

Go:   func add(a, b int) int
来源：http://cbl.nanxuanxn.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://kqs.yj20258.top

C#:   int Add(int a, int b) => a + b;
来源：http://wyg.xziqi.cn

[C14] 泛型函数
来源：http://syn.pycfn.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://bcs.xinyue.icu

PHP:  // 无泛型
来源：http://bbq.xinyue.icu

JS:   // 无泛型
来源：http://fyl.yfazqb.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://jvb.hywenlv.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://iwt.c1oappe.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mgk.shangyingyoupin.top

Ruby: # 无泛型
来源：http://vrv.tanke756.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hnh.chenzaomai.com

[C15] 解构 / 展开参数
来源：http://bpw.meibo888.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://skr.tian-w.cn

PHP:  [$a, $b] = $pair;
来源：http://fbx.xingfuxueyuan.xyz

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://dej.yuxming.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://vfb.fengsongda.top

Java: // 无解构
来源：http://nas.zhaomingkeji.xyz

Go:   // 无解构
来源：http://lpl.daria6918.cn

Ruby: a, b = pair
来源：http://aah.c1oappe.top

C#:   var (a, b) = pair;
来源：http://ruq.hongshengwenyu.top

[C16] 函数 / 方法重载
来源：http://kea.ydzc1.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://pxn.pycfn.com

PHP:  // 无重载
来源：http://bcf.yj202588.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://lqb.jqgfzy.top

TS:   // 用联合类型或重载签名声明
来源：http://usl.gotoacloud.top

Java: void f(int a) {}  void f(String a) {}
来源：http://lug.haohaochexian.top

Go:   // 无重载：用不同函数名
来源：http://dlx.yonumen.top

Ruby: # 无重载：靠动态参数
来源：http://suh.guowangkeji.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://kis.xinyue.icu

================================================================================
来源：http://mui.hysaishi.cn

D. 数组 / 列表 / 集合
来源：http://ppp.cdnleiting.top

================================================================================
来源：http://gaf.ivvv.top

[D01] 创建数组 / 列表
来源：http://zic.c1oappe.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://ztk.aizwys.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://kki.epnwcf.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://yvf.ehwqpu.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://wbu.xuanzx.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mby.sjlbkw.cn

Go:   arr := []int{1, 2, 3}
来源：http://njb.xuanzx.com

Ruby: arr = [1, 2, 3]
来源：http://pej.chenzaomai.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://grd.nanxinkj.top

[D02] 追加元素到末尾
来源：http://qju.guannengcc.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://auz.0kj1m.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://uvy.chenzaomai.com

JS:   arr.push(4);
来源：http://ljp.jinyuanbaomall.cn

TS:   arr.push(4);
来源：http://wue.shuidangran.top

Java: list.add(4);
来源：http://kie.chenlongwang.top

Go:   arr = append(arr, 4)
来源：http://bvs.zdqjudy.top

Ruby: arr << 4; arr.push(5)
来源：http://isj.gotoacloud.top

C#:   list.Add(4);
来源：http://vso.hysaishi.cn

[D03] 在指定位置插入元素
来源：http://yki.svipenyu.cn

Py:   arr.insert(0, 0)
来源：http://sbh.9152youxi.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://bvf.zhoulong.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://xye.yj20258888.top

TS:   arr.splice(0, 0, 0);
来源：http://huh.shzxlz.cn

Java: list.add(0, 0);
来源：http://xst.feifeiyinyue.top

Go:   arr = append([]int{0}, arr...)
来源：http://cxk.cqqwz.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ctc.bjfxy.top

C#:   list.Insert(0, 0);
来源：http://njo.sxryk.cn

[D04] 删除元素
来源：http://vht.svipenyu.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://okm.zhongyouzk.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://owz.guowangkeji.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mys.yangfankeji.com

TS:   arr.splice(0, 1);
来源：http://vaj.uphjek.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://vwf.feifeiyinyue.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://zhw.chenlongwang.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://cwy.zdqjudy.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://kdj.zhaomingkeji.xyz

[D05] 访问与修改元素
来源：http://llz.zhixingplan.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://duh.xuanzx.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wmk.jinyuanbaomall.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ize.jqgfzy.top

TS:   arr[0]; arr.at(-1);
来源：http://eya.vqdsnc.cn

Java: list.get(0); list.set(0, 9);
来源：http://mrm.hnqzz.top

Go:   arr[0]; arr[0] = 9
来源：http://lxp.xylfe.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://pdk.uphjek.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zqz.pycfn.com

[D06] 数组长度
来源：http://qmm.tianlin.xyz

Py:   len(arr)
来源：http://dox.aizwys.cn

PHP:  count($arr);
来源：http://rbt.nwbrower.top

JS:   arr.length
来源：http://ioc.jlsjyb.cn

TS:   arr.length
来源：http://spl.zhongyouzk.top

Java: list.size();
来源：http://egu.gzhubu.top

Go:   len(arr)
来源：http://swn.zhijiandao.cn

Ruby: arr.length; arr.size
来源：http://fyz.jqgfzy.top

C#:   list.Count;
来源：http://req.zhijiandao.cn

[D07] 切片 / 取子数组
来源：http://rbl.zhengqikj.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://knv.nanxinkj.top

PHP:  array_slice($arr, 1, 3);
来源：http://dwv.meibo888.top

JS:   arr.slice(1, 4);
来源：http://xvr.daxiang520.top

TS:   arr.slice(1, 4);
来源：http://lfj.ydjk.org.cn

Java: list.subList(1, 4);
来源：http://ewr.jinqigfzy.top

Go:   arr[1:4]
来源：http://izk.c1oappe.top

Ruby: arr[1, 3]
来源：http://lno.feifeiyinyue.top

C#:   list.GetRange(1, 3);
来源：http://vxs.yangfankeji.com

[D08] 合并两个数组
来源：http://blk.dashuyun.cn

Py:   a + b;  a.extend(b)
来源：http://zhq.jinqigfzy.top

PHP:  array_merge($a, $b);
来源：http://prh.zhaomingkeji.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://yof.snrcjt.cn

TS:   [...a, ...b];
来源：http://xpv.sxryk.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://buk.sweek.top

Go:   append(a, b...)
来源：http://gkl.epnwcf.com

Ruby: a + b;  a.concat(b)
来源：http://pxc.chenzaomai.com

C#:   a.Concat(b).ToList()
来源：http://qli.zhongyouzk.top

[D09] 排序（升序）
来源：http://xaj.tarul.cn

Py:   sorted(arr);  arr.sort()
来源：http://cny.sweek.top

PHP:  sort($arr);
来源：http://moh.quarkkingdee.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://laz.andypj.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://yfc.yangfankeji.com

Java: Collections.sort(list);  list.sort(null);
来源：http://ipp.yvedp.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://xxt.aibaodan.cn

Ruby: arr.sort
来源：http://xve.zhiwuduotai.top

C#:   list.Sort();
来源：http://szt.zhijiandao.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://xka.sjlbkw.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://btc.sxryk.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ugm.nanxuanxn.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wgr.ybcxt.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://zdf.bbcook.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://snw.zhijiandao.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://etf.xuanzx.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://gvy.shuidangran.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://yiv.jlsjyb.cn

[D11] 反转数组
来源：http://ppx.hysaishi.cn

Py:   arr[::-1];  arr.reverse()
来源：http://swe.shanyushiyangtech.top

PHP:  array_reverse($arr);
来源：http://fct.hongshengwenyu.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qgg.ybcxt.top

TS:   [...arr].reverse();
来源：http://yav.zycfv.cn

Java: Collections.reverse(list);
来源：http://tyj.nanxuanxn.top

Go:   slices.Reverse(arr)
来源：http://klw.hcnkem.com

Ruby: arr.reverse
来源：http://jhu.ydjk.org.cn


<!-- 参考信息 -->