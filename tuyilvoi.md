代发 wailian999

PHP:  range(0, 10, 2);
来源：http://qtt.uphjek.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dzo.meibo888.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://izh.snrcjt.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://cqj.aibaodan.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mkm.sufxvd.cn

Ruby: (0...10).step(2).to_a
来源：http://dvi.ppjwa.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://lee.hongshengwenyu.top

[B12] 跳出多层循环
来源：http://pgv.yfazqb.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://rqt.zhijiandao.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://xne.snrcjt.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://bih.jiagoushi.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://gps.ehwqpu.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ypb.andypj.xyz

Go:   # 无标签：用布尔标志或抽成函数
来源：http://jvy.ydzc1.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://shr.feifeiyinyue.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://cgi.nanxinkj.top

[B13] 判断是否为数字
来源：http://cgm.yj20258888.top

Py:   isinstance(x, (int, float))
来源：http://wdx.andypj.xyz

PHP:  is_numeric($x)
来源：http://dkm.dashuyun.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zeg.epnwcf.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kgl.jinqigfzy.top

Java: x instanceof Number
来源：http://qqw.ppjwa.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hyz.hongshengwenyu.top

Ruby: x.is_a?(Numeric)
来源：http://rwt.feifeiyinyue.top

C#:   x is int or double or decimal
来源：http://ull.ivvv.top

[B14] 判断值是否在集合内
来源：http://hlm.nanxuanxn.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://tkn.shuidangran.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://avd.iojbl.cn

JS:   [1, 2, 3].includes(x)
来源：http://gqz.ybcxt.top

TS:   [1, 2, 3].includes(x)
来源：http://buz.zdqjudy.top

Java: List.of(1, 2, 3).contains(x)
来源：http://lnr.cqqwz.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ojv.fehbvm.com

Ruby: [1, 2, 3].include?(x)
来源：http://via.9152youxi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://whp.yj20258.top

[B15] 布尔运算与取反
来源：http://pat.zhoulong.xyz

Py:   a and b or not c
来源：http://see.yfazqb.com

PHP:  $a && $b || !$c
来源：http://fqj.hfpthk.cn

JS:   a && b || !c
来源：http://xlk.wangshuangyany.cn

TS:   a && b || !c
来源：http://hji.yonumen.top

Java: a && b || !c
来源：http://iny.jlsjyb.cn

Go:   a && b || !c
来源：http://ddt.shangyingyoupin.top

Ruby: a && b || !c
来源：http://riv.zdqjudy.top

C#:   a && b || !c
来源：http://xgy.shzxlz.cn

[B16] 卫语句：不满足条件提前返回
来源：http://nsk.havefunace.top

Py:   if not data: return
来源：http://lnt.fzhhl.top

PHP:  if (!$data) { return; }
来源：http://zna.c1oappe.top

JS:   if (!data) return;
来源：http://wom.jqgfzy.top

TS:   if (!data) return;
来源：http://szz.hesvh.cn

Java: if (data == null) return;
来源：http://srx.daxiang520.top

Go:   if data == nil { return }
来源：http://ytx.feifeiyinyue.top

Ruby: return if data.nil?
来源：http://vaq.xuetiantiany.cn

C#:   if (data == null) return;
来源：http://bdn.guowangkeji.top

================================================================================
来源：http://rft.aizwys.cn

C. 函数与作用域
来源：http://oxo.jinghuilouyu.cn

================================================================================
来源：http://abg.pengpengdd.cyou

[C01] 定义函数
来源：http://ayk.hongshengwenyu.top

Py:   def add(a, b): return a + b
来源：http://ygt.dashuyun.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kao.yfazqb.com

JS:   function add(a, b) { return a + b; }
来源：http://beq.jiagoushi.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://smo.yj20258888.top

Java: static int add(int a, int b) { return a + b; }
来源：http://uqb.jianghu66.top

Go:   func add(a, b int) int { return a + b }
来源：http://yro.chenlongwang.top

Ruby: def add(a, b); a + b; end
来源：http://pki.yueranfly.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://tsg.hammf.cn

[C02] 默认参数
来源：http://bud.meibo888.top

Py:   def greet(name="World"): return name
来源：http://iem.yongpay.top

PHP:  function greet($name = "World") { return $name; }
来源：http://ttt.meibo888.top

JS:   function greet(name = "World") { return name; }
来源：http://zyf.yanxiufei.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://jey.gaohongyu789.top

Java: // 无默认参数：方法重载或 Optional
来源：http://mhr.snrcjt.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://yne.hongshengwenyu.top

Ruby: def greet(name = "World") = name
来源：http://kmx.vqdsnc.cn

C#:   string Greet(string name = "World") => name;
来源：http://vkq.yfazqb.com

[C03] 可变参数
来源：http://ybc.cheryme.top

Py:   def total(*args): return sum(args)
来源：http://qsx.tarul.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://yri.yvedp.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://jos.nanxuanxn.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://gkl.yuanzhike.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://czg.tarul.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://itc.gotoacloud.top

Ruby: def total(*nums); nums.sum; end
来源：http://yqm.chenzaomai.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://het.xuetiantiany.cn

[C04] 命名参数 / 关键字参数
来源：http://dwi.shanyushiyangtech.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://can.shanyushiyangtech.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ams.zdbjq.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://kck.tarul.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://jkd.shangyingyoupin.top

Java: // 无：用 Builder 模式或 record
来源：http://yvu.zhongyouzk.top

Go:   // 无：用配置结构体参数
来源：http://qps.cqqwz.cn

Ruby: f(a: 1, b: 2)
来源：http://jfe.hnqzz.top

C#:   f(a: 1, b: 2)
来源：http://ree.jinghuilouyu.cn

[C05] 返回多个值
来源：http://mgs.shanyushiyangkeji.top

Py:   return a, b
来源：http://jpn.yueranfly.top

PHP:  return [$a, $b];
来源：http://kyn.shanyushiyangtech.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://jiq.bjfxy.top

TS:   return { a, b };
来源：http://mjn.guannengcc.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://sck.feifeiyinyue.top

Go:   return a, b
来源：http://lic.dashuyun.cn

Ruby: return a, b
来源：http://fia.fengsongda.top

C#:   return (a, b);              // ValueTuple
来源：http://vrh.cdnleiting.top

[C06] 匿名函数 / lambda
来源：http://stl.aizwys.cn

Py:   square = lambda x: x * x
来源：http://tjg.cucudq.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://znx.cqqwz.cn

JS:   const square = x => x * x;
来源：http://rbs.zhongyouzk.top

TS:   const square = (x: number): number => x * x;
来源：http://knw.svipenyu.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://apo.haohaochexian.top

Go:   sq := func(x int) int { return x * x }
来源：http://dtf.svipenyu.cn

Ruby: square = ->(x) { x * x }
来源：http://pis.aizwys.cn

C#:   Func<int, int> square = x => x * x;
来源：http://zhi.bjfxy.top

[C07] 把函数作为参数传入
来源：http://zov.jinqigfzy.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://rbr.fzhhl.top

PHP:  array_map("strtoupper", $arr);
来源：http://wxo.daxiang520.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://gpp.tarul.cn

TS:   arr.map(String)
来源：http://okr.zdqjudy.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://qgg.zhixingplan.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://swv.zdbjq.cn

Ruby: arr.map(&:upcase)
来源：http://vze.jinqigfzy.top

C#:   arr.Select(s => s.ToUpper())
来源：http://irt.ywan-chungtsiang.top

[C08] 闭包
来源：http://psl.ehwqpu.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://kay.hammf.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://xci.jinqigufen.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://awg.pycfn.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://iew.sweek.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://zyi.ppjwa.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jvw.jqgufenzy.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://jsb.yongpay.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ldq.yangfankeji.com

[C09] 递归
来源：http://bjk.zhoulong.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://jxi.iojbl.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://vjz.bbcook.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wjb.quarkkingdee.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pzx.dianchejie.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://drg.ehwqpu.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://lff.hcnkem.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://jbu.yangfankeji.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://qqn.haohaochexian.top

[C10] 变量作用域
来源：http://ido.shanyushiyangtech.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://iat.9152youxi.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://iiz.zdbjq.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wrr.sjlbkw.cn

TS:   同 JS
来源：http://ytb.shuidangran.top

Java: 方法内为块级作用域
来源：http://uml.andypj.xyz

Go:   花括号块级作用域
来源：http://jri.sysykeji.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://lpc.tianlin.xyz

C#:   块级作用域
来源：http://alh.pengpengdd.cyou

[C11] 模块导入与导出
来源：http://odx.havefunace.top

Py:   from module import func
来源：http://xpl.redwolf501.top

PHP:  require "file.php";  或 use App\Service;
来源：http://rub.zdqjudy.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://mdt.gzhubu.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://boy.yj20258888.top

Java: import java.util.List;
来源：http://nea.quarkkingdee.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://htq.jiagoushi.top

Ruby: require "json"; require_relative "./util"
来源：http://ief.zhengqikj.top

C#:   using System.Text;
来源：http://ktg.yfazqb.com

[C12] 立即执行函数 IIFE
来源：http://ltc.zhiwuduotai.top

Py:   (lambda: print("run"))()
来源：http://exp.bjfxy.top

PHP:  (function () { echo "run"; })();
来源：http://fcz.xylfe.cn

JS:   (() => { console.log("run"); })();
来源：http://wxn.nwbrower.top

TS:   (() => { console.log("run"); })();
来源：http://kwa.gzhubu.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://bcc.kuanghao11.cn

Go:   func() { fmt.Println("run") }()
来源：http://rpn.fehbvm.com

Ruby: -> { puts "run" }.call
来源：http://ejr.yueranfly.top

C#:   // 无 IIFE：用静态构造函数
来源：http://lnx.zdbjq.cn

[C13] 类型声明 / 类型注解
来源：http://uja.jinghuilouyu.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://xoa.jiagoushi.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cpf.shzxlz.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ygn.zdqjudy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vqm.shanyushiyangkeji.top

Java: int add(int a, int b) { return a + b; }
来源：http://vlr.dianchejie.cn

Go:   func add(a, b int) int
来源：http://mba.hnxiangtu.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hbo.guowangkeji.top

C#:   int Add(int a, int b) => a + b;
来源：http://lgm.cqqwz.cn

[C14] 泛型函数
来源：http://mtc.xuetiantiany.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://rrx.hnxiangtu.top

PHP:  // 无泛型
来源：http://tys.chenzaomai.com

JS:   // 无泛型
来源：http://yal.cdnleiting.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hwn.hywenlv.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://rsy.hywenlv.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://rwz.smart0.xyz

Ruby: # 无泛型
来源：http://seh.jinqigfzy.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://vtn.shanyushiyangtech.top

[C15] 解构 / 展开参数
来源：http://sjh.hfpthk.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://rpg.xziqi.cn

PHP:  [$a, $b] = $pair;
来源：http://ors.xylfe.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ojx.mhx1999.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://jtu.316326.xyz

Java: // 无解构
来源：http://qwl.shanyushiyangtech.top

Go:   // 无解构
来源：http://nwv.yj202588.top

Ruby: a, b = pair
来源：http://ioc.yj20258.top

C#:   var (a, b) = pair;
来源：http://qkc.hnqzz.top

[C16] 函数 / 方法重载
来源：http://uea.jinqigufen.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://nkl.jinghuilouyu.cn

PHP:  // 无重载
来源：http://xtf.xinyue.icu

JS:   // 无重载：靠 arguments.length 分支
来源：http://oyi.9152youxi.cn

TS:   // 用联合类型或重载签名声明
来源：http://zwc.guowangkeji.top

Java: void f(int a) {}  void f(String a) {}
来源：http://rcj.cqqwz.cn

Go:   // 无重载：用不同函数名
来源：http://psw.hnqzz.top

Ruby: # 无重载：靠动态参数
来源：http://mov.snrcjt.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ubh.xinyue.icu

================================================================================
来源：http://eyh.fktsv.cn

D. 数组 / 列表 / 集合
来源：http://ezy.yj20258.top

================================================================================
来源：http://lyl.ehwqpu.com

[D01] 创建数组 / 列表
来源：http://odf.xziqi.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://eil.yueranfly.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://unb.yfazqb.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://uot.cqqwz.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://udu.yuxming.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wjm.hammf.cn

Go:   arr := []int{1, 2, 3}
来源：http://ccq.bjfxy.top

Ruby: arr = [1, 2, 3]
来源：http://guj.xziqi.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://kcm.wangdashe.top

[D02] 追加元素到末尾
来源：http://qky.xuanzx.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://drk.vehdjk.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mor.fanxiaobao.xyz

JS:   arr.push(4);
来源：http://jmu.daria6918.cn

TS:   arr.push(4);
来源：http://npz.cashguo.top

Java: list.add(4);
来源：http://crq.jiagoushi.top

Go:   arr = append(arr, 4)
来源：http://wvk.ywan-chungtsiang.top

Ruby: arr << 4; arr.push(5)
来源：http://ctv.yj202588.top

C#:   list.Add(4);
来源：http://gcp.tarul.cn

[D03] 在指定位置插入元素
来源：http://mns.iojbl.cn

Py:   arr.insert(0, 0)
来源：http://syi.yueranfly.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://cnn.zhoulong.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hmu.316326.xyz

TS:   arr.splice(0, 0, 0);
来源：http://caw.ywan-chungtsiang.top

Java: list.add(0, 0);
来源：http://czt.ivvv.top

Go:   arr = append([]int{0}, arr...)
来源：http://jwv.jinyuanbaomall.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://edp.jqgufenzy.top

C#:   list.Insert(0, 0);
来源：http://fto.ctjpmb.com

[D04] 删除元素
来源：http://kfe.chenjidiqi.icu

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://owl.bjfxy.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://tha.jinqigufen.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://fhx.hywenlv.cn

TS:   arr.splice(0, 1);
来源：http://nyn.gaohongyu789.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://bvh.ydzc1.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://axr.zhiwuduotai.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ujf.hnqzz.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://grf.zhixingplan.top

[D05] 访问与修改元素
来源：http://yza.jiagoushi.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wqs.yvedp.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://klu.yonumen.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hci.ybcxt.top

TS:   arr[0]; arr.at(-1);
来源：http://men.ivvv.top

Java: list.get(0); list.set(0, 9);
来源：http://jpi.cdnleiting.top

Go:   arr[0]; arr[0] = 9
来源：http://ira.zhongyouzk.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://znf.tianlin.xyz

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://xdd.shanyushiyangkeji.top

[D06] 数组长度
来源：http://uap.fengsongda.top

Py:   len(arr)
来源：http://ocr.sjlbkw.cn

PHP:  count($arr);
来源：http://omd.gzhubu.top

JS:   arr.length
来源：http://kuj.jiagoushi.top

TS:   arr.length
来源：http://stg.hesvh.cn

Java: list.size();
来源：http://wco.epnwcf.com

Go:   len(arr)
来源：http://onn.epnwcf.com

Ruby: arr.length; arr.size
来源：http://sbw.shanyushiyangkeji.top

C#:   list.Count;
来源：http://pdy.fanxiaobao.xyz

[D07] 切片 / 取子数组
来源：http://lbb.52xcode.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://cyu.fzhhl.top

PHP:  array_slice($arr, 1, 3);
来源：http://djr.wangdashe.top

JS:   arr.slice(1, 4);
来源：http://zol.shzxlz.cn

TS:   arr.slice(1, 4);
来源：http://wbs.smart0.xyz

Java: list.subList(1, 4);
来源：http://gfh.zdbjq.cn

Go:   arr[1:4]
来源：http://dzu.jinghuilouyu.cn

Ruby: arr[1, 3]
来源：http://kpo.cdnleiting.top

C#:   list.GetRange(1, 3);
来源：http://sqf.jyoumei.cn

[D08] 合并两个数组
来源：http://glw.yonumen.top

Py:   a + b;  a.extend(b)
来源：http://bra.shzxlz.cn

PHP:  array_merge($a, $b);
来源：http://dxh.hnxiangtu.top

JS:   [...a, ...b];  a.concat(b);
来源：http://ctc.zycfv.cn

TS:   [...a, ...b];
来源：http://bvl.xuanzx.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://kiu.xylfe.cn

Go:   append(a, b...)
来源：http://gqa.jqgufenzy.top

Ruby: a + b;  a.concat(b)
来源：http://uio.shuidangran.top

C#:   a.Concat(b).ToList()
来源：http://egx.hnqzz.top

[D09] 排序（升序）
来源：http://tnu.yonumen.top

Py:   sorted(arr);  arr.sort()
来源：http://hrw.yfazqb.com

PHP:  sort($arr);
来源：http://bhm.cashguo.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://fiu.fanxiaobao.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://wgo.hfpthk.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://vff.haohaochexian.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://rxq.feifeiyinyue.top

Ruby: arr.sort
来源：http://llj.yj20258.top

C#:   list.Sort();
来源：http://vdz.xylfe.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://qlr.aibaodan.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://pee.redwolf501.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wlh.chenjidiqi.icu

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ddp.feifeiyinyue.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://lqh.ehwqpu.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ulw.guannengcc.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://dru.ehwqpu.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://upo.chenlongwang.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://yqx.svipenyu.cn

[D11] 反转数组
来源：http://utn.c1oappe.top

Py:   arr[::-1];  arr.reverse()
来源：http://ivw.jianghu66.top

PHP:  array_reverse($arr);
来源：http://snw.52xcode.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://irj.shanyushiyangtech.top

TS:   [...arr].reverse();
来源：http://osj.cheryme.top

Java: Collections.reverse(list);
来源：http://lkc.kuanghao11.cn

Go:   slices.Reverse(arr)
来源：http://vyr.zhengqikj.top

Ruby: arr.reverse
来源：http://xhm.cdnleiting.top


<!-- 参考信息 -->