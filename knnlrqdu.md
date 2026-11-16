代发 wailian999

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://jhx.pengpengdd.cyou

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://rjx.ybcxt.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://kik.ybcxt.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://tla.uphjek.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ymj.sweek.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wia.tianlin.xyz

[B11] 生成数字序列 / 区间
来源：http://ynm.hammf.cn

Py:   list(range(0, 10, 2))
来源：http://ihc.jianghu66.top

PHP:  range(0, 10, 2);
来源：http://rar.guowangkeji.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://aap.andypj.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wjv.feifeiyinyue.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://nbf.zdqjudy.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ewc.vqdsnc.cn

Ruby: (0...10).step(2).to_a
来源：http://jtm.zycfv.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ifo.cqqwz.cn

[B12] 跳出多层循环
来源：http://nhz.iojbl.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://hpy.jinyuanbaomall.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://zxz.yanxiufei.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://gav.52xcode.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ohs.hnqzz.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://yee.chenlongwang.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://bmz.xziqi.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hzh.316326.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://khy.cashguo.top

[B13] 判断是否为数字
来源：http://ppi.wangdashe.top

Py:   isinstance(x, (int, float))
来源：http://cba.gaohongyu789.top

PHP:  is_numeric($x)
来源：http://xhc.hywenlv.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qun.hnxiangtu.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fca.fehbvm.com

Java: x instanceof Number
来源：http://ogr.shzxlz.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://tan.yonumen.top

Ruby: x.is_a?(Numeric)
来源：http://ypt.iojbl.cn

C#:   x is int or double or decimal
来源：http://ihl.zdbjq.cn

[B14] 判断值是否在集合内
来源：http://nfw.yonumen.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://boz.jinghuilouyu.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://etu.wangdashe.top

JS:   [1, 2, 3].includes(x)
来源：http://xbf.zhongyouzk.top

TS:   [1, 2, 3].includes(x)
来源：http://ntg.jqgufenzy.top

Java: List.of(1, 2, 3).contains(x)
来源：http://nvv.bjfxy.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://paf.wangshuangyany.cn

Ruby: [1, 2, 3].include?(x)
来源：http://zgd.fzhhl.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://fuc.kuanghao11.cn

[B15] 布尔运算与取反
来源：http://dpg.cdnleiting.top

Py:   a and b or not c
来源：http://btp.feifeiyinyue.top

PHP:  $a && $b || !$c
来源：http://mnv.ydjk.org.cn

JS:   a && b || !c
来源：http://uhj.ivvv.top

TS:   a && b || !c
来源：http://asy.yonumen.top

Java: a && b || !c
来源：http://zua.xuanzx.com

Go:   a && b || !c
来源：http://pdb.cashguo.top

Ruby: a && b || !c
来源：http://btt.aibaodan.cn

C#:   a && b || !c
来源：http://txj.cucudq.cn

[B16] 卫语句：不满足条件提前返回
来源：http://hjt.jqgufenzy.top

Py:   if not data: return
来源：http://cpw.jinyuanbaomall.cn

PHP:  if (!$data) { return; }
来源：http://bzl.sxryk.cn

JS:   if (!data) return;
来源：http://qii.cheryme.top

TS:   if (!data) return;
来源：http://rui.gzhubu.top

Java: if (data == null) return;
来源：http://qat.nanxuanxn.top

Go:   if data == nil { return }
来源：http://muf.yuxming.cn

Ruby: return if data.nil?
来源：http://fqr.yonumen.top

C#:   if (data == null) return;
来源：http://mrh.kuanghao11.cn

================================================================================
来源：http://sku.uphjek.com

C. 函数与作用域
来源：http://lct.smart0.xyz

================================================================================
来源：http://yqm.ydjk.org.cn

[C01] 定义函数
来源：http://sbk.gzhubu.top

Py:   def add(a, b): return a + b
来源：http://blj.tian-w.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xua.tianlin.xyz

JS:   function add(a, b) { return a + b; }
来源：http://cvz.epnwcf.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ssj.feifeiyinyue.top

Java: static int add(int a, int b) { return a + b; }
来源：http://cqk.wangdashe.top

Go:   func add(a, b int) int { return a + b }
来源：http://pbs.hfpthk.cn

Ruby: def add(a, b); a + b; end
来源：http://xgk.cheryme.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://bxo.0kj1m.cn

[C02] 默认参数
来源：http://tlz.chenzaomai.com

Py:   def greet(name="World"): return name
来源：http://nsx.yueranfly.top

PHP:  function greet($name = "World") { return $name; }
来源：http://fre.pengpengdd.cyou

JS:   function greet(name = "World") { return name; }
来源：http://tff.zhoulong.xyz

TS:   function greet(name: string = "World") { return name; }
来源：http://dgt.zhoulong.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://sxg.yueranfly.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://sdz.xingfuxueyuan.xyz

Ruby: def greet(name = "World") = name
来源：http://ovv.hammf.cn

C#:   string Greet(string name = "World") => name;
来源：http://ggh.hywenlv.cn

[C03] 可变参数
来源：http://qzs.ydzc1.top

Py:   def total(*args): return sum(args)
来源：http://fwr.bbcook.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mml.gogol.net.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://csj.xuetiantiany.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://rxr.gzhubu.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://xco.0kj1m.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://bfz.chenzaomai.com

Ruby: def total(*nums); nums.sum; end
来源：http://vso.hfpthk.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zuf.bbcook.cn

[C04] 命名参数 / 关键字参数
来源：http://wgf.svipenyu.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wga.hammf.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://fbo.jiagoushi.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://pio.ywan-chungtsiang.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://qmi.redwolf501.top

Java: // 无：用 Builder 模式或 record
来源：http://juf.zhixingplan.top

Go:   // 无：用配置结构体参数
来源：http://yds.316326.xyz

Ruby: f(a: 1, b: 2)
来源：http://hes.pycfn.com

C#:   f(a: 1, b: 2)
来源：http://fyp.smart0.xyz

[C05] 返回多个值
来源：http://gje.sweek.top

Py:   return a, b
来源：http://ego.zhijiandao.cn

PHP:  return [$a, $b];
来源：http://hsi.fengsongda.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://ans.shanyushiyangtech.top

TS:   return { a, b };
来源：http://azj.tanke756.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://qlo.zhengqikj.top

Go:   return a, b
来源：http://xga.cheryme.top

Ruby: return a, b
来源：http://ktd.daria6918.cn

C#:   return (a, b);              // ValueTuple
来源：http://sgt.zhengqikj.top

[C06] 匿名函数 / lambda
来源：http://hqa.zhaomingkeji.xyz

Py:   square = lambda x: x * x
来源：http://ikl.uphjek.com

PHP:  $square = fn($x) => $x * $x;
来源：http://bbl.cqqwz.cn

JS:   const square = x => x * x;
来源：http://zmg.52xcode.cn

TS:   const square = (x: number): number => x * x;
来源：http://jpg.snrcjt.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wrw.xziqi.cn

Go:   sq := func(x int) int { return x * x }
来源：http://iyc.yfazqb.com

Ruby: square = ->(x) { x * x }
来源：http://flb.hnqzz.top

C#:   Func<int, int> square = x => x * x;
来源：http://zed.zhongyouzk.top

[C07] 把函数作为参数传入
来源：http://jmp.fktsv.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://vze.zhengqikj.top

PHP:  array_map("strtoupper", $arr);
来源：http://bbm.shzxlz.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ezr.zhijiandao.cn

TS:   arr.map(String)
来源：http://scs.yueranfly.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://nyr.jiagoushi.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://jph.andypj.xyz

Ruby: arr.map(&:upcase)
来源：http://edi.svipenyu.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://zcn.daria6918.cn

[C08] 闭包
来源：http://tmp.nwbrower.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://cxz.yangfankeji.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://syx.cucudq.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://cfq.daxiang520.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mdn.guannengcc.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://zkg.vqdsnc.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://daa.xziqi.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.gzhubu.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://cdb.yfazqb.com

[C09] 递归
来源：http://hxi.ydzc1.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://zgc.sxryk.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://qwr.jqgufenzy.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lij.shanyushiyangkeji.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gow.jyoumei.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://qxv.tarul.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://jcf.yj20258888.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xkn.hammf.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://uhb.yuxming.cn

[C10] 变量作用域
来源：http://blu.fehbvm.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://tec.jqgufenzy.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://qkj.sufxvd.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://bqe.yj20258888.top

TS:   同 JS
来源：http://ulz.wangdashe.top

Java: 方法内为块级作用域
来源：http://ieb.zhengqikj.top

Go:   花括号块级作用域
来源：http://til.xinyue.icu

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ckn.sxryk.cn

C#:   块级作用域
来源：http://tki.sjlbkw.cn

[C11] 模块导入与导出
来源：http://mam.tanke756.top

Py:   from module import func
来源：http://vxy.chenjidiqi.icu

PHP:  require "file.php";  或 use App\Service;
来源：http://epx.tian-w.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ggj.xziqi.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://aar.zhengqikj.top

Java: import java.util.List;
来源：http://dvu.cashguo.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://jky.yfazqb.com

Ruby: require "json"; require_relative "./util"
来源：http://uym.fanxiaobao.xyz

C#:   using System.Text;
来源：http://tbh.guannengcc.top

[C12] 立即执行函数 IIFE
来源：http://pux.hnqzz.top

Py:   (lambda: print("run"))()
来源：http://zsf.gzhubu.top

PHP:  (function () { echo "run"; })();
来源：http://hlz.aibaodan.cn

JS:   (() => { console.log("run"); })();
来源：http://qzt.birdmap.top

TS:   (() => { console.log("run"); })();
来源：http://ejg.jianghu66.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jkt.vehdjk.com

Go:   func() { fmt.Println("run") }()
来源：http://aht.fengsongda.top

Ruby: -> { puts "run" }.call
来源：http://bgc.zhongyouzk.top

C#:   // 无 IIFE：用静态构造函数
来源：http://cmu.sxryk.cn

[C13] 类型声明 / 类型注解
来源：http://wvx.guowangkeji.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://zwa.zdqjudy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xyq.cqqwz.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://gch.guannengcc.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://axi.jinghuilouyu.cn

Java: int add(int a, int b) { return a + b; }
来源：http://igk.jianghu66.top

Go:   func add(a, b int) int
来源：http://vlq.ehwqpu.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ikn.xuetiantiany.cn

C#:   int Add(int a, int b) => a + b;
来源：http://qkq.birdmap.top

[C14] 泛型函数
来源：http://fdv.chenzaomai.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://erx.xziqi.cn

PHP:  // 无泛型
来源：http://duy.sweek.top

JS:   // 无泛型
来源：http://lbd.fehbvm.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://zja.redwolf501.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://rfr.jqgfzy.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://owb.feifeiyinyue.top

Ruby: # 无泛型
来源：http://gfs.jiagoushi.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://rpk.iojbl.cn

[C15] 解构 / 展开参数
来源：http://gei.tanke756.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ejb.xinyue.icu

PHP:  [$a, $b] = $pair;
来源：http://nlc.yangfankeji.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://cbb.c1oappe.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://auc.tianlin.xyz

Java: // 无解构
来源：http://nbu.jinqigfzy.top

Go:   // 无解构
来源：http://xzs.feifeiyinyue.top

Ruby: a, b = pair
来源：http://atn.cucudq.cn

C#:   var (a, b) = pair;
来源：http://hzq.sysykeji.top

[C16] 函数 / 方法重载
来源：http://dyd.nwbrower.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hes.shuidangran.top

PHP:  // 无重载
来源：http://wyd.gogol.net.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://zcy.hcnkem.com

TS:   // 用联合类型或重载签名声明
来源：http://wxn.jinqigufen.top

Java: void f(int a) {}  void f(String a) {}
来源：http://afb.daria6918.cn

Go:   // 无重载：用不同函数名
来源：http://awn.ydzc1.top

Ruby: # 无重载：靠动态参数
来源：http://wgg.xylfe.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ppj.zycfv.cn

================================================================================
来源：http://zju.xingfuxueyuan.xyz

D. 数组 / 列表 / 集合
来源：http://pax.quarkkingdee.top

================================================================================
来源：http://nyc.gaohongyu789.top

[D01] 创建数组 / 列表
来源：http://iin.yongpay.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://pmj.cqqwz.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://kxp.yangfankeji.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mjc.jinyuanbaomall.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://lti.0kj1m.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://flj.sufxvd.cn

Go:   arr := []int{1, 2, 3}
来源：http://vsn.yfazqb.com

Ruby: arr = [1, 2, 3]
来源：http://oga.zhijiandao.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://unp.cashguo.top

[D02] 追加元素到末尾
来源：http://hjo.cqqwz.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://sxw.epnwcf.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://xdm.yj20258888.top

JS:   arr.push(4);
来源：http://hkc.fehbvm.com

TS:   arr.push(4);
来源：http://uyg.shuidangran.top

Java: list.add(4);
来源：http://wiz.jqgufenzy.top

Go:   arr = append(arr, 4)
来源：http://kem.shanyushiyangkeji.top

Ruby: arr << 4; arr.push(5)
来源：http://prw.aibaodan.cn

C#:   list.Add(4);
来源：http://wkj.chenzaomai.com

[D03] 在指定位置插入元素
来源：http://jaw.aizwys.cn

Py:   arr.insert(0, 0)
来源：http://dxj.jinqigufen.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://rjw.xinyue.icu

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://xvg.gzhubu.top

TS:   arr.splice(0, 0, 0);
来源：http://hbp.hammf.cn

Java: list.add(0, 0);
来源：http://wir.zhixingplan.top

Go:   arr = append([]int{0}, arr...)
来源：http://ixg.yuanzhike.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://gsk.smart0.xyz

C#:   list.Insert(0, 0);
来源：http://cai.hcnkem.com

[D04] 删除元素
来源：http://ixb.hnqzz.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://zqz.wangshuangyany.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://krz.zhaomingkeji.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://swj.hysaishi.cn

TS:   arr.splice(0, 1);
来源：http://ssq.jlsjyb.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wqb.yuxming.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://vax.xuanzx.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://jtq.ydzc1.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mae.xziqi.cn

[D05] 访问与修改元素
来源：http://hmw.0kj1m.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://szz.ehwqpu.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://rai.ivvv.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ebo.gogol.net.cn

TS:   arr[0]; arr.at(-1);
来源：http://pqp.wangshuangyany.cn

Java: list.get(0); list.set(0, 9);
来源：http://sip.ehwqpu.com

Go:   arr[0]; arr[0] = 9
来源：http://ykz.zhoulong.xyz

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://jvq.jiagoushi.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://onp.hysaishi.cn

[D06] 数组长度
来源：http://rxw.guannengcc.top

Py:   len(arr)
来源：http://tpm.jinyuanbaomall.cn

PHP:  count($arr);
来源：http://mao.wangshuangyany.cn

JS:   arr.length
来源：http://evx.pycfn.com

TS:   arr.length
来源：http://lkt.bbcook.cn

Java: list.size();
来源：http://auu.pycfn.com

Go:   len(arr)
来源：http://aot.mhx1999.top

Ruby: arr.length; arr.size
来源：http://lms.cdnleiting.top

C#:   list.Count;
来源：http://mdq.ppjwa.cn

[D07] 切片 / 取子数组
来源：http://dvi.9152youxi.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mky.quarkkingdee.top

PHP:  array_slice($arr, 1, 3);
来源：http://lef.yuxming.cn

JS:   arr.slice(1, 4);
来源：http://dkv.wangdashe.top

TS:   arr.slice(1, 4);
来源：http://qez.sjlbkw.cn

Java: list.subList(1, 4);
来源：http://mjq.316326.xyz

Go:   arr[1:4]
来源：http://puu.ehwqpu.com

Ruby: arr[1, 3]
来源：http://pyg.jinqigfzy.top

C#:   list.GetRange(1, 3);
来源：http://gsu.vqdsnc.cn

[D08] 合并两个数组
来源：http://vwq.birdmap.top

Py:   a + b;  a.extend(b)
来源：http://jix.kuanghao11.cn

PHP:  array_merge($a, $b);
来源：http://fua.nwbrower.top

JS:   [...a, ...b];  a.concat(b);
来源：http://bwt.bjfxy.top

TS:   [...a, ...b];
来源：http://gds.jinghuilouyu.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://kpu.hesvh.cn

Go:   append(a, b...)
来源：http://hca.nwbrower.top

Ruby: a + b;  a.concat(b)
来源：http://ghk.zycfv.cn

C#:   a.Concat(b).ToList()
来源：http://bfh.sweek.top

[D09] 排序（升序）
来源：http://snw.hywenlv.cn

Py:   sorted(arr);  arr.sort()
来源：http://trg.iojbl.cn

PHP:  sort($arr);
来源：http://gnm.hysaishi.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://vlf.iojbl.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ihk.meibo888.top

Java: Collections.sort(list);  list.sort(null);
来源：http://urj.nanxinkj.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://xcu.bbcook.cn

Ruby: arr.sort
来源：http://shv.zhijiandao.cn

C#:   list.Sort();
来源：http://pme.yueranfly.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://enr.gotoacloud.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qwr.epnwcf.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://omb.tian-w.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wna.vehdjk.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://nww.sysykeji.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ffx.iojbl.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://nbk.zdqjudy.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://zcf.guowangkeji.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qrv.yangfankeji.com


<!-- 参考信息 -->