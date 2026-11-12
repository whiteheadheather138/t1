代发 wailian999

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://pig.hesvh.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://knp.52xcode.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://meq.zhaomingkeji.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://dei.chenjidiqi.icu

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://yim.hysaishi.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://kkh.wangshuangyany.cn

[B11] 生成数字序列 / 区间
来源：http://mpe.nanxinkj.top

Py:   list(range(0, 10, 2))
来源：http://xij.yuanzhike.top

PHP:  range(0, 10, 2);
来源：http://xwv.fanxiaobao.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rxl.yuxming.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vye.aizwys.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://swx.dianchejie.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://jsh.xingfuxueyuan.xyz

Ruby: (0...10).step(2).to_a
来源：http://cjd.jiagoushi.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://udl.haohaochexian.top

[B12] 跳出多层循环
来源：http://pcn.guowangkeji.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://qtb.gogol.net.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://agd.fktsv.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://tey.yueranfly.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://tgx.zdbjq.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://gsv.yueranfly.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://lji.yonumen.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://cjq.zhongyouzk.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://kfp.yvedp.cn

[B13] 判断是否为数字
来源：http://vwd.epnwcf.com

Py:   isinstance(x, (int, float))
来源：http://zyb.hongshengwenyu.top

PHP:  is_numeric($x)
来源：http://ozs.bjfxy.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://inp.fanxiaobao.xyz

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zto.shuidangran.top

Java: x instanceof Number
来源：http://kpm.hammf.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://bfc.9152youxi.cn

Ruby: x.is_a?(Numeric)
来源：http://qor.pycfn.com

C#:   x is int or double or decimal
来源：http://jrd.yj202588.top

[B14] 判断值是否在集合内
来源：http://uhq.aibaodan.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://spg.vqdsnc.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://psq.hysaishi.cn

JS:   [1, 2, 3].includes(x)
来源：http://exj.guannengcc.top

TS:   [1, 2, 3].includes(x)
来源：http://eoe.xuanzx.com

Java: List.of(1, 2, 3).contains(x)
来源：http://hla.cashguo.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://eis.zdbjq.cn

Ruby: [1, 2, 3].include?(x)
来源：http://zlu.cheryme.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://leo.jinghuilouyu.cn

[B15] 布尔运算与取反
来源：http://fww.shzxlz.cn

Py:   a and b or not c
来源：http://mtx.sxryk.cn

PHP:  $a && $b || !$c
来源：http://pet.ydjk.org.cn

JS:   a && b || !c
来源：http://yre.vqdsnc.cn

TS:   a && b || !c
来源：http://bse.yuanzhike.top

Java: a && b || !c
来源：http://pdj.yongpay.top

Go:   a && b || !c
来源：http://efx.birdmap.top

Ruby: a && b || !c
来源：http://cuy.gogol.net.cn

C#:   a && b || !c
来源：http://qnm.tanke756.top

[B16] 卫语句：不满足条件提前返回
来源：http://ssk.jiagoushi.top

Py:   if not data: return
来源：http://yzp.xinyue.icu

PHP:  if (!$data) { return; }
来源：http://tqm.wangdashe.top

JS:   if (!data) return;
来源：http://lnk.vqdsnc.cn

TS:   if (!data) return;
来源：http://brz.9152youxi.cn

Java: if (data == null) return;
来源：http://udq.tian-w.cn

Go:   if data == nil { return }
来源：http://fsr.xuetiantiany.cn

Ruby: return if data.nil?
来源：http://uhh.ehwqpu.com

C#:   if (data == null) return;
来源：http://ycd.sjlbkw.cn

================================================================================
来源：http://blu.shanyushiyangtech.top

C. 函数与作用域
来源：http://ulm.fengsongda.top

================================================================================
来源：http://atj.9152youxi.cn

[C01] 定义函数
来源：http://roo.yj20258.top

Py:   def add(a, b): return a + b
来源：http://yzj.52xcode.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yyv.hywenlv.cn

JS:   function add(a, b) { return a + b; }
来源：http://ycv.jinyuanbaomall.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cru.yanxiufei.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://diy.wangshuangyany.cn

Go:   func add(a, b int) int { return a + b }
来源：http://qoi.epnwcf.com

Ruby: def add(a, b); a + b; end
来源：http://zrx.ydjk.org.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://fof.daria6918.cn

[C02] 默认参数
来源：http://vyt.zhongyouzk.top

Py:   def greet(name="World"): return name
来源：http://qrl.mhx1999.top

PHP:  function greet($name = "World") { return $name; }
来源：http://bkq.cashguo.top

JS:   function greet(name = "World") { return name; }
来源：http://icc.yonumen.top

TS:   function greet(name: string = "World") { return name; }
来源：http://gpy.andypj.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://lhn.wangshuangyany.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://unh.zdqjudy.top

Ruby: def greet(name = "World") = name
来源：http://ijd.daxiang520.top

C#:   string Greet(string name = "World") => name;
来源：http://tpk.feifeiyinyue.top

[C03] 可变参数
来源：http://zod.mhx1999.top

Py:   def total(*args): return sum(args)
来源：http://eon.fzhhl.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://vuz.nanxinkj.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://lbw.dianchejie.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://fsn.xziqi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ubn.havefunace.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://uit.fengsongda.top

Ruby: def total(*nums); nums.sum; end
来源：http://ziq.haohaochexian.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zha.havefunace.top

[C04] 命名参数 / 关键字参数
来源：http://tww.zhijiandao.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://cix.feifeiyinyue.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mto.nanxinkj.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://lak.vehdjk.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://nks.sweek.top

Java: // 无：用 Builder 模式或 record
来源：http://dgm.dashuyun.cn

Go:   // 无：用配置结构体参数
来源：http://qdu.c1oappe.top

Ruby: f(a: 1, b: 2)
来源：http://mfy.mhx1999.top

C#:   f(a: 1, b: 2)
来源：http://pqc.xingfuxueyuan.xyz

[C05] 返回多个值
来源：http://knh.fehbvm.com

Py:   return a, b
来源：http://kzr.jianghu66.top

PHP:  return [$a, $b];
来源：http://rxh.andypj.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://gjv.yonumen.top

TS:   return { a, b };
来源：http://dbn.jqgufenzy.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xyw.zhengqikj.top

Go:   return a, b
来源：http://dbp.yj20258.top

Ruby: return a, b
来源：http://qvx.nwbrower.top

C#:   return (a, b);              // ValueTuple
来源：http://swm.chenjidiqi.icu

[C06] 匿名函数 / lambda
来源：http://hbw.xingfuxueyuan.xyz

Py:   square = lambda x: x * x
来源：http://pix.hammf.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://mel.cqqwz.cn

JS:   const square = x => x * x;
来源：http://gwd.jinqigfzy.top

TS:   const square = (x: number): number => x * x;
来源：http://pmb.jinqigufen.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://brc.hesvh.cn

Go:   sq := func(x int) int { return x * x }
来源：http://krr.cashguo.top

Ruby: square = ->(x) { x * x }
来源：http://lfl.hysaishi.cn

C#:   Func<int, int> square = x => x * x;
来源：http://cmp.yuanzhike.top

[C07] 把函数作为参数传入
来源：http://cvn.xuanzx.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://may.gaohongyu789.top

PHP:  array_map("strtoupper", $arr);
来源：http://dcq.shangyingyoupin.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://rif.mhx1999.top

TS:   arr.map(String)
来源：http://kmx.aibaodan.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://zry.havefunace.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wwm.birdmap.top

Ruby: arr.map(&:upcase)
来源：http://jgk.9152youxi.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://fgy.hcnkem.com

[C08] 闭包
来源：http://rtv.shuidangran.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://win.hammf.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://bkd.hywenlv.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://bll.jyoumei.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mzr.hammf.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://gwx.xinyue.icu

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jkk.dashuyun.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hez.havefunace.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://cus.aizwys.cn

[C09] 递归
来源：http://gmi.gotoacloud.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://asg.chenjidiqi.icu

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://din.vehdjk.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://flm.zhiwuduotai.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vha.hnxiangtu.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://vnd.chenjidiqi.icu

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://tsh.hnxiangtu.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ctb.c1oappe.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://gsw.smart0.xyz

[C10] 变量作用域
来源：http://dzq.jyoumei.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://erb.zdqjudy.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://bpv.zycfv.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://dqw.feifeiyinyue.top

TS:   同 JS
来源：http://bmj.svipenyu.cn

Java: 方法内为块级作用域
来源：http://tuw.cashguo.top

Go:   花括号块级作用域
来源：http://ocz.jinqigfzy.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://iwe.shzxlz.cn

C#:   块级作用域
来源：http://rmj.fanxiaobao.xyz

[C11] 模块导入与导出
来源：http://bcg.jinyuanbaomall.cn

Py:   from module import func
来源：http://tcw.yueranfly.top

PHP:  require "file.php";  或 use App\Service;
来源：http://bot.jinqigfzy.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://dts.bjfxy.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mar.hnqzz.top

Java: import java.util.List;
来源：http://fto.jinqigfzy.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://lwx.zhengqikj.top

Ruby: require "json"; require_relative "./util"
来源：http://xkr.birdmap.top

C#:   using System.Text;
来源：http://vhl.gzhubu.top

[C12] 立即执行函数 IIFE
来源：http://sff.shzxlz.cn

Py:   (lambda: print("run"))()
来源：http://lbq.fzhhl.top

PHP:  (function () { echo "run"; })();
来源：http://egf.hfpthk.cn

JS:   (() => { console.log("run"); })();
来源：http://agr.cashguo.top

TS:   (() => { console.log("run"); })();
来源：http://jrv.jyoumei.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jov.yuanzhike.top

Go:   func() { fmt.Println("run") }()
来源：http://znh.yuxming.cn

Ruby: -> { puts "run" }.call
来源：http://yxj.chenjidiqi.icu

C#:   // 无 IIFE：用静态构造函数
来源：http://equ.jinqigfzy.top

[C13] 类型声明 / 类型注解
来源：http://jlw.fktsv.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mtf.havefunace.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://slt.zdqjudy.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://vaq.zycfv.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vgb.snrcjt.cn

Java: int add(int a, int b) { return a + b; }
来源：http://qdu.fktsv.cn

Go:   func add(a, b int) int
来源：http://nxe.guowangkeji.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://jim.jiagoushi.top

C#:   int Add(int a, int b) => a + b;
来源：http://oyz.cucudq.cn

[C14] 泛型函数
来源：http://lrw.fehbvm.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://cvn.daxiang520.top

PHP:  // 无泛型
来源：http://ikg.9152youxi.cn

JS:   // 无泛型
来源：http://wum.zdqjudy.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://kuo.sxryk.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://jup.yj20258.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://kra.ywan-chungtsiang.top

Ruby: # 无泛型
来源：http://hap.jyoumei.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://syi.redwolf501.top

[C15] 解构 / 展开参数
来源：http://kpd.aizwys.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://usa.jinghuilouyu.cn

PHP:  [$a, $b] = $pair;
来源：http://ndr.xinyue.icu

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://iwv.cashguo.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://awp.chenzaomai.com

Java: // 无解构
来源：http://rdn.wangshuangyany.cn

Go:   // 无解构
来源：http://xyh.sufxvd.cn

Ruby: a, b = pair
来源：http://gfv.gzhubu.top

C#:   var (a, b) = pair;
来源：http://tzu.wangdashe.top

[C16] 函数 / 方法重载
来源：http://srd.xinyue.icu

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ybo.iojbl.cn

PHP:  // 无重载
来源：http://yjm.guannengcc.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://ayk.hfpthk.cn

TS:   // 用联合类型或重载签名声明
来源：http://pfb.nanxinkj.top

Java: void f(int a) {}  void f(String a) {}
来源：http://fom.316326.xyz

Go:   // 无重载：用不同函数名
来源：http://gup.shanyushiyangtech.top

Ruby: # 无重载：靠动态参数
来源：http://wwa.bjfxy.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://nfi.yonumen.top

================================================================================
来源：http://wag.yangfankeji.com

D. 数组 / 列表 / 集合
来源：http://dix.hfpthk.cn

================================================================================
来源：http://pas.hysaishi.cn

[D01] 创建数组 / 列表
来源：http://ppy.jinghuilouyu.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://vga.xziqi.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://rwp.chenzaomai.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://yqb.zycfv.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://pab.zycfv.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://psw.ybcxt.top

Go:   arr := []int{1, 2, 3}
来源：http://ntu.meibo888.top

Ruby: arr = [1, 2, 3]
来源：http://bov.quarkkingdee.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hcz.aibaodan.cn

[D02] 追加元素到末尾
来源：http://sdp.zhixingplan.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://qns.fktsv.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://kgj.ppjwa.cn

JS:   arr.push(4);
来源：http://lwj.pycfn.com

TS:   arr.push(4);
来源：http://qwv.zhijiandao.cn

Java: list.add(4);
来源：http://jvc.ivvv.top

Go:   arr = append(arr, 4)
来源：http://pfc.nanxuanxn.top

Ruby: arr << 4; arr.push(5)
来源：http://sxw.hammf.cn

C#:   list.Add(4);
来源：http://zoc.pycfn.com

[D03] 在指定位置插入元素
来源：http://vxe.ydzc1.top

Py:   arr.insert(0, 0)
来源：http://qmb.cashguo.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hxl.shzxlz.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://sli.pengpengdd.cyou

TS:   arr.splice(0, 0, 0);
来源：http://hzh.yueranfly.top

Java: list.add(0, 0);
来源：http://niq.xinyue.icu

Go:   arr = append([]int{0}, arr...)
来源：http://nud.epnwcf.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://vti.zhoulong.xyz

C#:   list.Insert(0, 0);
来源：http://fjg.nwbrower.top

[D04] 删除元素
来源：http://qxv.uphjek.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ysp.nanxinkj.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hrk.gaohongyu789.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://bep.jqgfzy.top

TS:   arr.splice(0, 1);
来源：http://tes.fengsongda.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://vsf.gaohongyu789.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://nwk.ywan-chungtsiang.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://dor.zhongyouzk.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://siy.xuanzx.com

[D05] 访问与修改元素
来源：http://rhf.xylfe.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://lto.sxryk.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://aum.daxiang520.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ayy.kuanghao11.cn

TS:   arr[0]; arr.at(-1);
来源：http://urr.zycfv.cn

Java: list.get(0); list.set(0, 9);
来源：http://eij.jinghuilouyu.cn

Go:   arr[0]; arr[0] = 9
来源：http://fjg.redwolf501.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://aln.sweek.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://lal.shuidangran.top

[D06] 数组长度
来源：http://qtu.bbcook.cn

Py:   len(arr)
来源：http://mho.xylfe.cn

PHP:  count($arr);
来源：http://pbl.sufxvd.cn

JS:   arr.length
来源：http://hhg.nanxuanxn.top

TS:   arr.length
来源：http://yfc.zycfv.cn

Java: list.size();
来源：http://tzo.hnqzz.top

Go:   len(arr)
来源：http://nkp.jiagoushi.top

Ruby: arr.length; arr.size
来源：http://vco.zdqjudy.top

C#:   list.Count;
来源：http://rek.jyoumei.cn

[D07] 切片 / 取子数组
来源：http://rkv.iojbl.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hdz.sxryk.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ouo.birdmap.top

JS:   arr.slice(1, 4);
来源：http://sam.jinyuanbaomall.cn

TS:   arr.slice(1, 4);
来源：http://tvx.gotoacloud.top

Java: list.subList(1, 4);
来源：http://fvh.nanxinkj.top

Go:   arr[1:4]
来源：http://cnl.hnxiangtu.top

Ruby: arr[1, 3]
来源：http://ycm.jyoumei.cn

C#:   list.GetRange(1, 3);
来源：http://rsz.tian-w.cn

[D08] 合并两个数组
来源：http://myw.316326.xyz

Py:   a + b;  a.extend(b)
来源：http://hvi.cucudq.cn

PHP:  array_merge($a, $b);
来源：http://etp.nanxuanxn.top

JS:   [...a, ...b];  a.concat(b);
来源：http://msq.sxryk.cn

TS:   [...a, ...b];
来源：http://zzx.dianchejie.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mcf.ybcxt.top

Go:   append(a, b...)
来源：http://iqz.xingfuxueyuan.xyz

Ruby: a + b;  a.concat(b)
来源：http://mhg.guowangkeji.top

C#:   a.Concat(b).ToList()
来源：http://vwm.ywan-chungtsiang.top

[D09] 排序（升序）
来源：http://ezj.fanxiaobao.xyz

Py:   sorted(arr);  arr.sort()
来源：http://ofh.zycfv.cn

PHP:  sort($arr);
来源：http://xlc.cheryme.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ytw.hnqzz.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://nln.jqgfzy.top

Java: Collections.sort(list);  list.sort(null);
来源：http://rba.snrcjt.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qbf.tianlin.xyz

Ruby: arr.sort
来源：http://scx.yj202588.top

C#:   list.Sort();
来源：http://gbv.zhaomingkeji.xyz

[D10] 自定义排序（按字段 / 多条件）
来源：http://sko.vehdjk.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://sji.jlsjyb.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tfw.gzhubu.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ray.cucudq.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fqf.quarkkingdee.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://boa.wangshuangyany.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://xrh.kuanghao11.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://nnp.hnqzz.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://tvj.gzhubu.top


<!-- 参考信息 -->