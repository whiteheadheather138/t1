代发 wailian999

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ppt.yj202588.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://fid.ybcxt.top

[B11] 生成数字序列 / 区间
来源：http://nmz.shanyushiyangtech.top

Py:   list(range(0, 10, 2))
来源：http://jrc.zdqjudy.top

PHP:  range(0, 10, 2);
来源：http://snn.cheryme.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lis.xinyue.icu

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jbz.vehdjk.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ujq.hesvh.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://bwk.gogol.net.cn

Ruby: (0...10).step(2).to_a
来源：http://blo.ydzc1.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://kna.sweek.top

[B12] 跳出多层循环
来源：http://ohm.xylfe.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://vhe.guowangkeji.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://bmx.fehbvm.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ogy.svipenyu.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://asb.jinghuilouyu.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ejr.zycfv.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://gxl.smart0.xyz

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://weh.pycfn.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://yrs.sufxvd.cn

[B13] 判断是否为数字
来源：http://iuj.haohaochexian.top

Py:   isinstance(x, (int, float))
来源：http://csw.jqgufenzy.top

PHP:  is_numeric($x)
来源：http://zbo.guannengcc.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qov.jqgufenzy.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kjy.daxiang520.top

Java: x instanceof Number
来源：http://wlf.yonumen.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mks.daria6918.cn

Ruby: x.is_a?(Numeric)
来源：http://buo.zhengqikj.top

C#:   x is int or double or decimal
来源：http://hdf.hammf.cn

[B14] 判断值是否在集合内
来源：http://ycw.yvedp.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jmb.sweek.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://yoz.bjfxy.top

JS:   [1, 2, 3].includes(x)
来源：http://xuv.jqgufenzy.top

TS:   [1, 2, 3].includes(x)
来源：http://pot.yuxming.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://cfu.nwbrower.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://nwa.daxiang520.top

Ruby: [1, 2, 3].include?(x)
来源：http://tff.epnwcf.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://tvp.nanxuanxn.top

[B15] 布尔运算与取反
来源：http://kmr.aizwys.cn

Py:   a and b or not c
来源：http://cju.feifeiyinyue.top

PHP:  $a && $b || !$c
来源：http://ugy.c1oappe.top

JS:   a && b || !c
来源：http://nga.cheryme.top

TS:   a && b || !c
来源：http://gfp.sysykeji.top

Java: a && b || !c
来源：http://wqk.xinyue.icu

Go:   a && b || !c
来源：http://ool.jianghu66.top

Ruby: a && b || !c
来源：http://yfp.xylfe.cn

C#:   a && b || !c
来源：http://ckk.jlsjyb.cn

[B16] 卫语句：不满足条件提前返回
来源：http://zfd.hcnkem.com

Py:   if not data: return
来源：http://msv.hnqzz.top

PHP:  if (!$data) { return; }
来源：http://dbn.jinyuanbaomall.cn

JS:   if (!data) return;
来源：http://gat.jinyuanbaomall.cn

TS:   if (!data) return;
来源：http://hzv.hywenlv.cn

Java: if (data == null) return;
来源：http://ydu.tanke756.top

Go:   if data == nil { return }
来源：http://gxa.snrcjt.cn

Ruby: return if data.nil?
来源：http://mwv.epnwcf.com

C#:   if (data == null) return;
来源：http://fkh.chenjidiqi.icu

================================================================================
来源：http://ssg.smart0.xyz

C. 函数与作用域
来源：http://ppb.wangshuangyany.cn

================================================================================
来源：http://wdd.zdqjudy.top

[C01] 定义函数
来源：http://bdq.epnwcf.com

Py:   def add(a, b): return a + b
来源：http://neu.jinghuilouyu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lhf.ivvv.top

JS:   function add(a, b) { return a + b; }
来源：http://zri.jianghu66.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ekm.meibo888.top

Java: static int add(int a, int b) { return a + b; }
来源：http://uln.xuanzx.com

Go:   func add(a, b int) int { return a + b }
来源：http://wzu.sxryk.cn

Ruby: def add(a, b); a + b; end
来源：http://pca.yuanzhike.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ejw.yj202588.top

[C02] 默认参数
来源：http://zeq.fengsongda.top

Py:   def greet(name="World"): return name
来源：http://twu.haohaochexian.top

PHP:  function greet($name = "World") { return $name; }
来源：http://ktd.vqdsnc.cn

JS:   function greet(name = "World") { return name; }
来源：http://jnd.bbcook.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://pwc.hfpthk.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://svr.yanxiufei.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://lvd.sjlbkw.cn

Ruby: def greet(name = "World") = name
来源：http://ykg.jinyuanbaomall.cn

C#:   string Greet(string name = "World") => name;
来源：http://nlv.shanyushiyangkeji.top

[C03] 可变参数
来源：http://omb.fanxiaobao.xyz

Py:   def total(*args): return sum(args)
来源：http://rhc.jiagoushi.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://fgl.ydjk.org.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://kwz.wangdashe.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://akz.ybcxt.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://nvw.cheryme.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://enf.zhijiandao.cn

Ruby: def total(*nums); nums.sum; end
来源：http://iet.chenjidiqi.icu

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ngh.yuanzhike.top

[C04] 命名参数 / 关键字参数
来源：http://tpx.yangfankeji.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://tcb.yanxiufei.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://rth.yuxming.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://gmi.jqgfzy.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://efi.svipenyu.cn

Java: // 无：用 Builder 模式或 record
来源：http://arh.quarkkingdee.top

Go:   // 无：用配置结构体参数
来源：http://mmk.hnqzz.top

Ruby: f(a: 1, b: 2)
来源：http://kqx.yueranfly.top

C#:   f(a: 1, b: 2)
来源：http://vao.yvedp.cn

[C05] 返回多个值
来源：http://euq.yongpay.top

Py:   return a, b
来源：http://bel.ehwqpu.com

PHP:  return [$a, $b];
来源：http://udc.tianlin.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://urd.ctjpmb.com

TS:   return { a, b };
来源：http://krd.zhoulong.xyz

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://rce.jiagoushi.top

Go:   return a, b
来源：http://ejg.yonumen.top

Ruby: return a, b
来源：http://cms.jinqigufen.top

C#:   return (a, b);              // ValueTuple
来源：http://kqd.hfpthk.cn

[C06] 匿名函数 / lambda
来源：http://bfh.c1oappe.top

Py:   square = lambda x: x * x
来源：http://iyx.pycfn.com

PHP:  $square = fn($x) => $x * $x;
来源：http://wgu.jqgfzy.top

JS:   const square = x => x * x;
来源：http://ska.ivvv.top

TS:   const square = (x: number): number => x * x;
来源：http://zle.gogol.net.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://qcg.shzxlz.cn

Go:   sq := func(x int) int { return x * x }
来源：http://jaf.hammf.cn

Ruby: square = ->(x) { x * x }
来源：http://azc.svipenyu.cn

C#:   Func<int, int> square = x => x * x;
来源：http://zgu.bjfxy.top

[C07] 把函数作为参数传入
来源：http://kos.ctjpmb.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://xhv.ivvv.top

PHP:  array_map("strtoupper", $arr);
来源：http://okf.fktsv.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://nmj.zhiwuduotai.top

TS:   arr.map(String)
来源：http://idx.yuxming.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mtj.cdnleiting.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://aux.jiagoushi.top

Ruby: arr.map(&:upcase)
来源：http://zly.xuanzx.com

C#:   arr.Select(s => s.ToUpper())
来源：http://zju.pengpengdd.cyou

[C08] 闭包
来源：http://qsq.haohaochexian.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ufs.9152youxi.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ouc.tanke756.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://oij.cheryme.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://yym.gaohongyu789.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://equ.chenlongwang.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ftz.fengsongda.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://nig.hysaishi.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://swm.vehdjk.com

[C09] 递归
来源：http://aus.shanyushiyangtech.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ncj.gogol.net.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://yqk.xingfuxueyuan.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sga.ehwqpu.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bbf.havefunace.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hqd.cheryme.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://cma.jlsjyb.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://fnq.vehdjk.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://eiq.jqgfzy.top

[C10] 变量作用域
来源：http://itl.ybcxt.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://nnz.jianghu66.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://huh.redwolf501.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://oyd.xuanzx.com

TS:   同 JS
来源：http://gkh.haohaochexian.top

Java: 方法内为块级作用域
来源：http://kgs.havefunace.top

Go:   花括号块级作用域
来源：http://abi.sufxvd.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://vrd.chenjidiqi.icu

C#:   块级作用域
来源：http://ugp.zhaomingkeji.xyz

[C11] 模块导入与导出
来源：http://jcg.hcnkem.com

Py:   from module import func
来源：http://ssu.yueranfly.top

PHP:  require "file.php";  或 use App\Service;
来源：http://iaw.yvedp.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://axy.zhixingplan.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://znt.smart0.xyz

Java: import java.util.List;
来源：http://vaf.sxryk.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://eng.yj20258.top

Ruby: require "json"; require_relative "./util"
来源：http://mol.9152youxi.cn

C#:   using System.Text;
来源：http://ehc.tian-w.cn

[C12] 立即执行函数 IIFE
来源：http://bxx.jinqigufen.top

Py:   (lambda: print("run"))()
来源：http://ete.shangyingyoupin.top

PHP:  (function () { echo "run"; })();
来源：http://aul.zhengqikj.top

JS:   (() => { console.log("run"); })();
来源：http://sxx.yj20258888.top

TS:   (() => { console.log("run"); })();
来源：http://wrh.aizwys.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://tlc.wangshuangyany.cn

Go:   func() { fmt.Println("run") }()
来源：http://dgp.cashguo.top

Ruby: -> { puts "run" }.call
来源：http://bcb.svipenyu.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://qts.tianlin.xyz

[C13] 类型声明 / 类型注解
来源：http://nlx.yvedp.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hed.gotoacloud.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qvn.nanxuanxn.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://nuq.snrcjt.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rhe.jinghuilouyu.cn

Java: int add(int a, int b) { return a + b; }
来源：http://wtv.tanke756.top

Go:   func add(a, b int) int
来源：http://yog.fzhhl.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://htq.gaohongyu789.top

C#:   int Add(int a, int b) => a + b;
来源：http://xby.meibo888.top

[C14] 泛型函数
来源：http://dtm.hongshengwenyu.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ahp.hcnkem.com

PHP:  // 无泛型
来源：http://qea.fengsongda.top

JS:   // 无泛型
来源：http://ukk.52xcode.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://pnw.fanxiaobao.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://zvz.feifeiyinyue.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://rsq.jinghuilouyu.cn

Ruby: # 无泛型
来源：http://ebj.zdbjq.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ulr.zdbjq.cn

[C15] 解构 / 展开参数
来源：http://sym.fzhhl.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wky.hfpthk.cn

PHP:  [$a, $b] = $pair;
来源：http://epa.shuidangran.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://bvo.nwbrower.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://jss.mhx1999.top

Java: // 无解构
来源：http://rce.xuetiantiany.cn

Go:   // 无解构
来源：http://bsr.hfpthk.cn

Ruby: a, b = pair
来源：http://err.ybcxt.top

C#:   var (a, b) = pair;
来源：http://jng.pycfn.com

[C16] 函数 / 方法重载
来源：http://zsb.birdmap.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://pov.hongshengwenyu.top

PHP:  // 无重载
来源：http://dog.jinghuilouyu.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://gqs.hysaishi.cn

TS:   // 用联合类型或重载签名声明
来源：http://ssk.epnwcf.com

Java: void f(int a) {}  void f(String a) {}
来源：http://ggn.havefunace.top

Go:   // 无重载：用不同函数名
来源：http://pze.sjlbkw.cn

Ruby: # 无重载：靠动态参数
来源：http://sbp.yonumen.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://pek.52xcode.cn

================================================================================
来源：http://hnp.hysaishi.cn

D. 数组 / 列表 / 集合
来源：http://mfb.gogol.net.cn

================================================================================
来源：http://fay.fehbvm.com

[D01] 创建数组 / 列表
来源：http://dkw.jiagoushi.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://fea.yfazqb.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://cim.cdnleiting.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ygb.zdbjq.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://vvh.dianchejie.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://swu.gogol.net.cn

Go:   arr := []int{1, 2, 3}
来源：http://crd.sweek.top

Ruby: arr = [1, 2, 3]
来源：http://eua.uphjek.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://uwv.daria6918.cn

[D02] 追加元素到末尾
来源：http://epp.wangdashe.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://pka.zdbjq.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://yum.ybcxt.top

JS:   arr.push(4);
来源：http://tpg.haohaochexian.top

TS:   arr.push(4);
来源：http://rfd.zhaomingkeji.xyz

Java: list.add(4);
来源：http://dxu.svipenyu.cn

Go:   arr = append(arr, 4)
来源：http://xze.guowangkeji.top

Ruby: arr << 4; arr.push(5)
来源：http://trg.0kj1m.cn

C#:   list.Add(4);
来源：http://afc.chenlongwang.top

[D03] 在指定位置插入元素
来源：http://lei.yj20258888.top

Py:   arr.insert(0, 0)
来源：http://ukn.xinyue.icu

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://esr.uphjek.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://gaa.xuetiantiany.cn

TS:   arr.splice(0, 0, 0);
来源：http://kzm.cucudq.cn

Java: list.add(0, 0);
来源：http://ese.xuanzx.com

Go:   arr = append([]int{0}, arr...)
来源：http://ock.52xcode.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ydl.xinyue.icu

C#:   list.Insert(0, 0);
来源：http://opp.dashuyun.cn

[D04] 删除元素
来源：http://vvt.nwbrower.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://qkp.birdmap.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://whk.meibo888.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://zqp.zhiwuduotai.top

TS:   arr.splice(0, 1);
来源：http://kfw.dashuyun.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://tif.daria6918.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://gvs.316326.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://zsv.ybcxt.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://nca.yj20258888.top

[D05] 访问与修改元素
来源：http://wwm.hysaishi.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://cib.daxiang520.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://did.yueranfly.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://dmb.hfpthk.cn

TS:   arr[0]; arr.at(-1);
来源：http://iph.tanke756.top

Java: list.get(0); list.set(0, 9);
来源：http://ivl.nwbrower.top

Go:   arr[0]; arr[0] = 9
来源：http://ksy.gogol.net.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://klz.sweek.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zmr.yj202588.top

[D06] 数组长度
来源：http://uhs.ybcxt.top

Py:   len(arr)
来源：http://tux.hcnkem.com

PHP:  count($arr);
来源：http://xhu.shanyushiyangtech.top

JS:   arr.length
来源：http://lwa.redwolf501.top

TS:   arr.length
来源：http://ghj.vehdjk.com

Java: list.size();
来源：http://xuz.sufxvd.cn

Go:   len(arr)
来源：http://ipr.shuidangran.top

Ruby: arr.length; arr.size
来源：http://hjs.tianlin.xyz

C#:   list.Count;
来源：http://hvv.gogol.net.cn

[D07] 切片 / 取子数组
来源：http://pcl.xziqi.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://lhk.316326.xyz

PHP:  array_slice($arr, 1, 3);
来源：http://rjx.tian-w.cn

JS:   arr.slice(1, 4);
来源：http://ydd.uphjek.com

TS:   arr.slice(1, 4);
来源：http://hxj.cheryme.top

Java: list.subList(1, 4);
来源：http://mie.jinqigufen.top

Go:   arr[1:4]
来源：http://ety.zhengqikj.top

Ruby: arr[1, 3]
来源：http://scy.fehbvm.com

C#:   list.GetRange(1, 3);
来源：http://bfk.nwbrower.top

[D08] 合并两个数组
来源：http://jqb.yongpay.top

Py:   a + b;  a.extend(b)
来源：http://gek.hesvh.cn

PHP:  array_merge($a, $b);
来源：http://yji.gaohongyu789.top

JS:   [...a, ...b];  a.concat(b);
来源：http://rob.shzxlz.cn

TS:   [...a, ...b];
来源：http://hsu.jinqigfzy.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ybn.cheryme.top

Go:   append(a, b...)
来源：http://zaf.yj202588.top

Ruby: a + b;  a.concat(b)
来源：http://yjb.ivvv.top

C#:   a.Concat(b).ToList()
来源：http://rqj.zhixingplan.top

[D09] 排序（升序）
来源：http://tjg.vehdjk.com

Py:   sorted(arr);  arr.sort()
来源：http://pqj.zhixingplan.top

PHP:  sort($arr);
来源：http://kfp.dashuyun.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://fsz.andypj.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://qou.vqdsnc.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://cky.meibo888.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://eku.kuanghao11.cn

Ruby: arr.sort
来源：http://qex.hongshengwenyu.top

C#:   list.Sort();
来源：http://vyu.sufxvd.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://uoh.shanyushiyangtech.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://cdh.zhixingplan.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://txe.ppjwa.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://rhc.quarkkingdee.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://irj.xylfe.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ivp.havefunace.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://pqs.fktsv.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ain.zhaomingkeji.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://piu.nanxinkj.top

[D11] 反转数组
来源：http://kyi.jyoumei.cn

Py:   arr[::-1];  arr.reverse()
来源：http://bof.yongpay.top

PHP:  array_reverse($arr);
来源：http://bhd.52xcode.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://cil.wangdashe.top


<!-- 参考信息 -->