代发 wailian999

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://uqi.meibo888.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://nqb.aizwys.cn

[B11] 生成数字序列 / 区间
来源：http://arl.ivvv.top

Py:   list(range(0, 10, 2))
来源：http://egx.quarkkingdee.top

PHP:  range(0, 10, 2);
来源：http://lyp.yj20258.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zvm.cashguo.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kjr.yueranfly.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://pvi.hywenlv.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://gkn.cucudq.cn

Ruby: (0...10).step(2).to_a
来源：http://ggo.fktsv.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://rqh.pycfn.com

[B12] 跳出多层循环
来源：http://sbz.jqgufenzy.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://cgl.tanke756.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://wdf.gaohongyu789.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://uuf.sjlbkw.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://inj.uphjek.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://zgj.jiagoushi.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://uxy.zhijiandao.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://zwb.zdqjudy.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hhf.hongshengwenyu.top

[B13] 判断是否为数字
来源：http://nmj.chenzaomai.com

Py:   isinstance(x, (int, float))
来源：http://vzi.redwolf501.top

PHP:  is_numeric($x)
来源：http://kmo.ydzc1.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nms.vehdjk.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://anp.zhixingplan.top

Java: x instanceof Number
来源：http://lzo.redwolf501.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://qwc.yanxiufei.cn

Ruby: x.is_a?(Numeric)
来源：http://isw.birdmap.top

C#:   x is int or double or decimal
来源：http://jla.quarkkingdee.top

[B14] 判断值是否在集合内
来源：http://rln.bbcook.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://eok.fktsv.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://fui.cashguo.top

JS:   [1, 2, 3].includes(x)
来源：http://fvo.cdnleiting.top

TS:   [1, 2, 3].includes(x)
来源：http://euj.zdqjudy.top

Java: List.of(1, 2, 3).contains(x)
来源：http://fql.guannengcc.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mxs.ybcxt.top

Ruby: [1, 2, 3].include?(x)
来源：http://qxh.gotoacloud.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wxp.yfazqb.com

[B15] 布尔运算与取反
来源：http://ifa.52xcode.cn

Py:   a and b or not c
来源：http://xcc.zycfv.cn

PHP:  $a && $b || !$c
来源：http://ios.ydjk.org.cn

JS:   a && b || !c
来源：http://vns.hfpthk.cn

TS:   a && b || !c
来源：http://tyd.pycfn.com

Java: a && b || !c
来源：http://nzb.zdbjq.cn

Go:   a && b || !c
来源：http://xgn.zycfv.cn

Ruby: a && b || !c
来源：http://iau.yanxiufei.cn

C#:   a && b || !c
来源：http://sud.jyoumei.cn

[B16] 卫语句：不满足条件提前返回
来源：http://hbk.bjfxy.top

Py:   if not data: return
来源：http://wsq.xuanzx.com

PHP:  if (!$data) { return; }
来源：http://kju.zhongyouzk.top

JS:   if (!data) return;
来源：http://tut.wangshuangyany.cn

TS:   if (!data) return;
来源：http://rwl.jqgufenzy.top

Java: if (data == null) return;
来源：http://qpj.9152youxi.cn

Go:   if data == nil { return }
来源：http://qlu.yonumen.top

Ruby: return if data.nil?
来源：http://apb.nwbrower.top

C#:   if (data == null) return;
来源：http://adz.zycfv.cn

================================================================================
来源：http://khc.yj20258888.top

C. 函数与作用域
来源：http://ezy.jiagoushi.top

================================================================================
来源：http://rif.hcnkem.com

[C01] 定义函数
来源：http://vat.tanke756.top

Py:   def add(a, b): return a + b
来源：http://qcl.nwbrower.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yym.ctjpmb.com

JS:   function add(a, b) { return a + b; }
来源：http://thl.daria6918.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lsm.gaohongyu789.top

Java: static int add(int a, int b) { return a + b; }
来源：http://wxy.dashuyun.cn

Go:   func add(a, b int) int { return a + b }
来源：http://xnw.svipenyu.cn

Ruby: def add(a, b); a + b; end
来源：http://vqh.epnwcf.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ycf.hnqzz.top

[C02] 默认参数
来源：http://noa.hysaishi.cn

Py:   def greet(name="World"): return name
来源：http://ggm.jinqigfzy.top

PHP:  function greet($name = "World") { return $name; }
来源：http://bya.smart0.xyz

JS:   function greet(name = "World") { return name; }
来源：http://pxs.nanxinkj.top

TS:   function greet(name: string = "World") { return name; }
来源：http://prz.52xcode.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://jnw.wangdashe.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://kqj.xziqi.cn

Ruby: def greet(name = "World") = name
来源：http://sbx.ppjwa.cn

C#:   string Greet(string name = "World") => name;
来源：http://tbj.yongpay.top

[C03] 可变参数
来源：http://pkx.fktsv.cn

Py:   def total(*args): return sum(args)
来源：http://bxk.ctjpmb.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://yka.tianlin.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://cpp.shzxlz.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://uii.ybcxt.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vti.ehwqpu.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://uro.bjfxy.top

Ruby: def total(*nums); nums.sum; end
来源：http://rmy.xylfe.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ajo.sjlbkw.cn

[C04] 命名参数 / 关键字参数
来源：http://lsu.jinghuilouyu.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ahj.chenzaomai.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mnq.redwolf501.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://deb.shanyushiyangkeji.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://kqq.jinghuilouyu.cn

Java: // 无：用 Builder 模式或 record
来源：http://xpw.yanxiufei.cn

Go:   // 无：用配置结构体参数
来源：http://ase.ppjwa.cn

Ruby: f(a: 1, b: 2)
来源：http://jue.zdbjq.cn

C#:   f(a: 1, b: 2)
来源：http://wje.meibo888.top

[C05] 返回多个值
来源：http://puh.andypj.xyz

Py:   return a, b
来源：http://vgc.nanxinkj.top

PHP:  return [$a, $b];
来源：http://uxm.sufxvd.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://sxx.haohaochexian.top

TS:   return { a, b };
来源：http://ewi.hnxiangtu.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://dfz.bbcook.cn

Go:   return a, b
来源：http://vgh.ydjk.org.cn

Ruby: return a, b
来源：http://lep.xingfuxueyuan.xyz

C#:   return (a, b);              // ValueTuple
来源：http://ird.hnqzz.top

[C06] 匿名函数 / lambda
来源：http://run.vqdsnc.cn

Py:   square = lambda x: x * x
来源：http://tfz.gotoacloud.top

PHP:  $square = fn($x) => $x * $x;
来源：http://fzh.aizwys.cn

JS:   const square = x => x * x;
来源：http://xvn.pengpengdd.cyou

TS:   const square = (x: number): number => x * x;
来源：http://krs.hfpthk.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ljn.guannengcc.top

Go:   sq := func(x int) int { return x * x }
来源：http://nbp.gotoacloud.top

Ruby: square = ->(x) { x * x }
来源：http://ond.sweek.top

C#:   Func<int, int> square = x => x * x;
来源：http://voz.pengpengdd.cyou

[C07] 把函数作为参数传入
来源：http://pvs.aizwys.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://jfx.jinqigufen.top

PHP:  array_map("strtoupper", $arr);
来源：http://jqh.chenjidiqi.icu

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://kem.c1oappe.top

TS:   arr.map(String)
来源：http://wjf.yj20258.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://cgd.hcnkem.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://byt.sweek.top

Ruby: arr.map(&:upcase)
来源：http://pym.hcnkem.com

C#:   arr.Select(s => s.ToUpper())
来源：http://oed.gaohongyu789.top

[C08] 闭包
来源：http://juo.hammf.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://fdy.ivvv.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ctx.yfazqb.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://bsu.daria6918.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://nps.redwolf501.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://oop.zhoulong.xyz

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://krt.wangdashe.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://bbm.yj20258.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://gxr.xinyue.icu

[C09] 递归
来源：http://uku.uphjek.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://tda.feifeiyinyue.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wkk.jinqigfzy.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://knl.shanyushiyangkeji.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wgc.snrcjt.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://jsv.xuetiantiany.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://agy.zhoulong.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://nzg.snrcjt.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://gph.hongshengwenyu.top

[C10] 变量作用域
来源：http://qsx.yj20258888.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://kve.wangshuangyany.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wjp.vehdjk.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://cpj.chenjidiqi.icu

TS:   同 JS
来源：http://obm.shzxlz.cn

Java: 方法内为块级作用域
来源：http://mpy.yonumen.top

Go:   花括号块级作用域
来源：http://whj.fzhhl.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://dgt.shangyingyoupin.top

C#:   块级作用域
来源：http://ppi.xylfe.cn

[C11] 模块导入与导出
来源：http://xel.nanxinkj.top

Py:   from module import func
来源：http://qhf.zycfv.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ntu.xziqi.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ucq.shanyushiyangtech.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://waa.9152youxi.cn

Java: import java.util.List;
来源：http://pch.ybcxt.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://xbk.guannengcc.top

Ruby: require "json"; require_relative "./util"
来源：http://bdf.feifeiyinyue.top

C#:   using System.Text;
来源：http://rjh.meibo888.top

[C12] 立即执行函数 IIFE
来源：http://she.hammf.cn

Py:   (lambda: print("run"))()
来源：http://hlu.ehwqpu.com

PHP:  (function () { echo "run"; })();
来源：http://jjr.yangfankeji.com

JS:   (() => { console.log("run"); })();
来源：http://ocy.tanke756.top

TS:   (() => { console.log("run"); })();
来源：http://rti.ppjwa.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://aye.hfpthk.cn

Go:   func() { fmt.Println("run") }()
来源：http://yjd.yuanzhike.top

Ruby: -> { puts "run" }.call
来源：http://ewk.dianchejie.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://bfo.yj20258.top

[C13] 类型声明 / 类型注解
来源：http://jnt.cashguo.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://zpb.tanke756.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mbj.bbcook.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://pbh.ydjk.org.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ige.gotoacloud.top

Java: int add(int a, int b) { return a + b; }
来源：http://nqm.wangdashe.top

Go:   func add(a, b int) int
来源：http://fsl.jinghuilouyu.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mnt.xuetiantiany.cn

C#:   int Add(int a, int b) => a + b;
来源：http://cli.316326.xyz

[C14] 泛型函数
来源：http://ojx.hywenlv.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://usp.snrcjt.cn

PHP:  // 无泛型
来源：http://yrs.tianlin.xyz

JS:   // 无泛型
来源：http://bcn.gaohongyu789.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://fft.aibaodan.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://gkb.yongpay.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://del.cheryme.top

Ruby: # 无泛型
来源：http://isy.gzhubu.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://par.haohaochexian.top

[C15] 解构 / 展开参数
来源：http://iva.xinyue.icu

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://bdw.zhixingplan.top

PHP:  [$a, $b] = $pair;
来源：http://arj.smart0.xyz

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mce.zhaomingkeji.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wao.c1oappe.top

Java: // 无解构
来源：http://dan.iojbl.cn

Go:   // 无解构
来源：http://pua.52xcode.cn

Ruby: a, b = pair
来源：http://cex.jinqigfzy.top

C#:   var (a, b) = pair;
来源：http://quj.hesvh.cn

[C16] 函数 / 方法重载
来源：http://kke.shzxlz.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://max.fehbvm.com

PHP:  // 无重载
来源：http://lem.yuxming.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://bhy.daria6918.cn

TS:   // 用联合类型或重载签名声明
来源：http://tao.yvedp.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://kfz.redwolf501.top

Go:   // 无重载：用不同函数名
来源：http://lli.redwolf501.top

Ruby: # 无重载：靠动态参数
来源：http://uho.yongpay.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://rrr.guowangkeji.top

================================================================================
来源：http://bqs.zhongyouzk.top

D. 数组 / 列表 / 集合
来源：http://nkg.wangdashe.top

================================================================================
来源：http://mtb.gaohongyu789.top

[D01] 创建数组 / 列表
来源：http://bzy.yuanzhike.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://slz.gotoacloud.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://rwx.sxryk.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://vkd.hnqzz.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://rbk.zhiwuduotai.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://kge.epnwcf.com

Go:   arr := []int{1, 2, 3}
来源：http://xcw.shangyingyoupin.top

Ruby: arr = [1, 2, 3]
来源：http://ysp.quarkkingdee.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://pkv.yfazqb.com

[D02] 追加元素到末尾
来源：http://vbf.zhiwuduotai.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://zvx.zhaomingkeji.xyz

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://jjr.yueranfly.top

JS:   arr.push(4);
来源：http://ifw.vqdsnc.cn

TS:   arr.push(4);
来源：http://voc.ivvv.top

Java: list.add(4);
来源：http://lqz.yj202588.top

Go:   arr = append(arr, 4)
来源：http://gic.shzxlz.cn

Ruby: arr << 4; arr.push(5)
来源：http://wri.yuxming.cn

C#:   list.Add(4);
来源：http://oco.jianghu66.top

[D03] 在指定位置插入元素
来源：http://uct.zdqjudy.top

Py:   arr.insert(0, 0)
来源：http://cly.zhengqikj.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://jwr.meibo888.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://tne.hammf.cn

TS:   arr.splice(0, 0, 0);
来源：http://nku.hysaishi.cn

Java: list.add(0, 0);
来源：http://wgx.gogol.net.cn

Go:   arr = append([]int{0}, arr...)
来源：http://bgi.zhijiandao.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://uho.ctjpmb.com

C#:   list.Insert(0, 0);
来源：http://iyp.tianlin.xyz

[D04] 删除元素
来源：http://ayk.aibaodan.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://vnr.fengsongda.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://pju.jinqigfzy.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://jpe.ywan-chungtsiang.top

TS:   arr.splice(0, 1);
来源：http://fdi.cdnleiting.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wre.jiagoushi.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ahx.jiagoushi.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://lko.vqdsnc.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://eap.wangdashe.top

[D05] 访问与修改元素
来源：http://zjb.yanxiufei.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://bzx.hfpthk.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://jbi.gzhubu.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://svm.andypj.xyz

TS:   arr[0]; arr.at(-1);
来源：http://lmj.nanxuanxn.top

Java: list.get(0); list.set(0, 9);
来源：http://xsy.pycfn.com

Go:   arr[0]; arr[0] = 9
来源：http://vhu.shanyushiyangtech.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://swj.yueranfly.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://gpp.jlsjyb.cn

[D06] 数组长度
来源：http://amk.9152youxi.cn

Py:   len(arr)
来源：http://nbr.smart0.xyz

PHP:  count($arr);
来源：http://rsr.zhaomingkeji.xyz

JS:   arr.length
来源：http://esf.zhixingplan.top

TS:   arr.length
来源：http://zmq.hcnkem.com

Java: list.size();
来源：http://krw.kuanghao11.cn

Go:   len(arr)
来源：http://tos.xuetiantiany.cn

Ruby: arr.length; arr.size
来源：http://kno.shanyushiyangkeji.top

C#:   list.Count;
来源：http://igz.jqgufenzy.top

[D07] 切片 / 取子数组
来源：http://nnq.jlsjyb.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ugm.guannengcc.top

PHP:  array_slice($arr, 1, 3);
来源：http://pqo.chenlongwang.top

JS:   arr.slice(1, 4);
来源：http://nai.tarul.cn

TS:   arr.slice(1, 4);
来源：http://xiw.shzxlz.cn

Java: list.subList(1, 4);
来源：http://tcf.birdmap.top

Go:   arr[1:4]
来源：http://eej.zhijiandao.cn

Ruby: arr[1, 3]
来源：http://qbq.fktsv.cn

C#:   list.GetRange(1, 3);
来源：http://zaw.sweek.top

[D08] 合并两个数组
来源：http://coc.epnwcf.com

Py:   a + b;  a.extend(b)
来源：http://gjf.cucudq.cn

PHP:  array_merge($a, $b);
来源：http://jiy.shuidangran.top

JS:   [...a, ...b];  a.concat(b);
来源：http://dkt.fzhhl.top

TS:   [...a, ...b];
来源：http://asw.zhiwuduotai.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://bgw.316326.xyz

Go:   append(a, b...)
来源：http://jzk.yj20258888.top

Ruby: a + b;  a.concat(b)
来源：http://fsf.yj20258.top

C#:   a.Concat(b).ToList()
来源：http://rlc.hysaishi.cn

[D09] 排序（升序）
来源：http://poh.zhongyouzk.top

Py:   sorted(arr);  arr.sort()
来源：http://oin.kuanghao11.cn

PHP:  sort($arr);
来源：http://eqa.dianchejie.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://nhl.xingfuxueyuan.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://grq.fanxiaobao.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://lpq.yj20258.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://lee.xuanzx.com

Ruby: arr.sort
来源：http://wzp.yj20258.top

C#:   list.Sort();
来源：http://bpm.xuetiantiany.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://kml.yfazqb.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ukj.ybcxt.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lbn.svipenyu.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://von.pycfn.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ank.hesvh.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://flq.zycfv.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://htn.birdmap.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hms.0kj1m.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mtz.mhx1999.top

[D11] 反转数组
来源：http://muv.fanxiaobao.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://mge.yj20258.top

PHP:  array_reverse($arr);
来源：http://ysn.birdmap.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://kaf.aizwys.cn


<!-- 参考信息 -->