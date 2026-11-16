代发 wailian999

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mml.xingfuxueyuan.xyz

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://fky.chenlongwang.top

[B11] 生成数字序列 / 区间
来源：http://dqn.yuanzhike.top

Py:   list(range(0, 10, 2))
来源：http://krq.tarul.cn

PHP:  range(0, 10, 2);
来源：http://qye.hysaishi.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ejr.uphjek.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yfe.0kj1m.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://eih.hcnkem.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://dcy.iojbl.cn

Ruby: (0...10).step(2).to_a
来源：http://xpd.havefunace.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://nso.zhengqikj.top

[B12] 跳出多层循环
来源：http://too.iojbl.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://yzy.jqgfzy.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://aga.zdbjq.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://bwp.yfazqb.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://vqv.ivvv.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://rzw.yongpay.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wjh.0kj1m.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://fwi.shanyushiyangkeji.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://cvy.quarkkingdee.top

[B13] 判断是否为数字
来源：http://eds.c1oappe.top

Py:   isinstance(x, (int, float))
来源：http://qvw.wangshuangyany.cn

PHP:  is_numeric($x)
来源：http://eqn.vehdjk.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mod.xinyue.icu

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lbe.nanxinkj.top

Java: x instanceof Number
来源：http://frt.hywenlv.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://xgn.shanyushiyangkeji.top

Ruby: x.is_a?(Numeric)
来源：http://vcw.cqqwz.cn

C#:   x is int or double or decimal
来源：http://cha.52xcode.cn

[B14] 判断值是否在集合内
来源：http://pbu.yueranfly.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://nhv.guowangkeji.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://cfo.sweek.top

JS:   [1, 2, 3].includes(x)
来源：http://rsz.feifeiyinyue.top

TS:   [1, 2, 3].includes(x)
来源：http://pye.ppjwa.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://hyb.jlsjyb.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://nqy.chenzaomai.com

Ruby: [1, 2, 3].include?(x)
来源：http://xui.nanxinkj.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://xqb.ydjk.org.cn

[B15] 布尔运算与取反
来源：http://jvu.snrcjt.cn

Py:   a and b or not c
来源：http://bpr.andypj.xyz

PHP:  $a && $b || !$c
来源：http://ptj.bbcook.cn

JS:   a && b || !c
来源：http://ckg.wangdashe.top

TS:   a && b || !c
来源：http://ocz.sjlbkw.cn

Java: a && b || !c
来源：http://vur.ctjpmb.com

Go:   a && b || !c
来源：http://wbp.xziqi.cn

Ruby: a && b || !c
来源：http://pla.kuanghao11.cn

C#:   a && b || !c
来源：http://mur.yvedp.cn

[B16] 卫语句：不满足条件提前返回
来源：http://twb.aibaodan.cn

Py:   if not data: return
来源：http://vrz.zhixingplan.top

PHP:  if (!$data) { return; }
来源：http://cdu.yuanzhike.top

JS:   if (!data) return;
来源：http://ieh.ybcxt.top

TS:   if (!data) return;
来源：http://myk.aibaodan.cn

Java: if (data == null) return;
来源：http://jsv.fehbvm.com

Go:   if data == nil { return }
来源：http://rjq.yuanzhike.top

Ruby: return if data.nil?
来源：http://xdt.quarkkingdee.top

C#:   if (data == null) return;
来源：http://bkj.yueranfly.top

================================================================================
来源：http://dgt.0kj1m.cn

C. 函数与作用域
来源：http://rif.haohaochexian.top

================================================================================
来源：http://iil.shuidangran.top

[C01] 定义函数
来源：http://vtl.cucudq.cn

Py:   def add(a, b): return a + b
来源：http://jbl.iojbl.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dcd.dashuyun.cn

JS:   function add(a, b) { return a + b; }
来源：http://ryh.dashuyun.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hvp.guannengcc.top

Java: static int add(int a, int b) { return a + b; }
来源：http://fop.yfazqb.com

Go:   func add(a, b int) int { return a + b }
来源：http://nuj.aibaodan.cn

Ruby: def add(a, b); a + b; end
来源：http://osh.jyoumei.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mml.xuanzx.com

[C02] 默认参数
来源：http://uqj.bbcook.cn

Py:   def greet(name="World"): return name
来源：http://ocr.jqgfzy.top

PHP:  function greet($name = "World") { return $name; }
来源：http://fcz.smart0.xyz

JS:   function greet(name = "World") { return name; }
来源：http://wcc.cucudq.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://aks.hcnkem.com

Java: // 无默认参数：方法重载或 Optional
来源：http://uwu.xuanzx.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://kfs.nwbrower.top

Ruby: def greet(name = "World") = name
来源：http://kio.xinyue.icu

C#:   string Greet(string name = "World") => name;
来源：http://xwj.yuanzhike.top

[C03] 可变参数
来源：http://gzm.bbcook.cn

Py:   def total(*args): return sum(args)
来源：http://pzd.wangshuangyany.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hbl.fzhhl.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wgz.ctjpmb.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hkb.cdnleiting.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vsq.aizwys.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hoy.hnxiangtu.top

Ruby: def total(*nums); nums.sum; end
来源：http://rwv.zhiwuduotai.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://udr.jinyuanbaomall.cn

[C04] 命名参数 / 关键字参数
来源：http://mgr.zhengqikj.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://pnl.xuanzx.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://cyk.cdnleiting.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mjt.fanxiaobao.xyz

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://axt.xuetiantiany.cn

Java: // 无：用 Builder 模式或 record
来源：http://eif.yj20258888.top

Go:   // 无：用配置结构体参数
来源：http://rzy.guannengcc.top

Ruby: f(a: 1, b: 2)
来源：http://zpp.chenlongwang.top

C#:   f(a: 1, b: 2)
来源：http://bac.birdmap.top

[C05] 返回多个值
来源：http://zgv.yuxming.cn

Py:   return a, b
来源：http://wab.ppjwa.cn

PHP:  return [$a, $b];
来源：http://rxm.chenjidiqi.icu

JS:   return [a, b];             // 或 return { a, b };
来源：http://rbe.shzxlz.cn

TS:   return { a, b };
来源：http://tsu.wangdashe.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://zqz.ehwqpu.com

Go:   return a, b
来源：http://zfy.smart0.xyz

Ruby: return a, b
来源：http://pcl.svipenyu.cn

C#:   return (a, b);              // ValueTuple
来源：http://bvm.hcnkem.com

[C06] 匿名函数 / lambda
来源：http://jme.jinqigufen.top

Py:   square = lambda x: x * x
来源：http://xgx.kuanghao11.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://vnx.vehdjk.com

JS:   const square = x => x * x;
来源：http://fhw.snrcjt.cn

TS:   const square = (x: number): number => x * x;
来源：http://igd.yonumen.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://geh.hongshengwenyu.top

Go:   sq := func(x int) int { return x * x }
来源：http://fft.pycfn.com

Ruby: square = ->(x) { x * x }
来源：http://rec.yj20258888.top

C#:   Func<int, int> square = x => x * x;
来源：http://bov.yuanzhike.top

[C07] 把函数作为参数传入
来源：http://sjw.zhongyouzk.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://crt.bbcook.cn

PHP:  array_map("strtoupper", $arr);
来源：http://fvs.xuetiantiany.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wma.hnqzz.top

TS:   arr.map(String)
来源：http://cle.sysykeji.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xeh.nwbrower.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ntn.havefunace.top

Ruby: arr.map(&:upcase)
来源：http://xvw.zhengqikj.top

C#:   arr.Select(s => s.ToUpper())
来源：http://gnh.yanxiufei.cn

[C08] 闭包
来源：http://coq.zhaomingkeji.xyz

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://pby.yongpay.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ybz.bjfxy.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://kts.shanyushiyangkeji.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mfx.zdbjq.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://vzl.shuidangran.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wzj.shangyingyoupin.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://rqr.andypj.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://prb.yuanzhike.top

[C09] 递归
来源：http://fmb.bjfxy.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ckq.nanxinkj.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wus.aibaodan.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ndb.meibo888.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wvz.shuidangran.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://gvr.birdmap.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://eia.cdnleiting.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://jff.xuetiantiany.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://goh.aizwys.cn

[C10] 变量作用域
来源：http://vak.sweek.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://llq.jinqigufen.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://isj.epnwcf.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://jsh.wangdashe.top

TS:   同 JS
来源：http://fai.0kj1m.cn

Java: 方法内为块级作用域
来源：http://gmu.hywenlv.cn

Go:   花括号块级作用域
来源：http://jge.chenlongwang.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://haw.quarkkingdee.top

C#:   块级作用域
来源：http://yve.zhiwuduotai.top

[C11] 模块导入与导出
来源：http://oki.yvedp.cn

Py:   from module import func
来源：http://aup.nanxinkj.top

PHP:  require "file.php";  或 use App\Service;
来源：http://pxm.xuetiantiany.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://wte.hnxiangtu.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mwq.xuetiantiany.cn

Java: import java.util.List;
来源：http://ynf.meibo888.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mgo.bbcook.cn

Ruby: require "json"; require_relative "./util"
来源：http://rat.cucudq.cn

C#:   using System.Text;
来源：http://bhl.fzhhl.top

[C12] 立即执行函数 IIFE
来源：http://nai.bjfxy.top

Py:   (lambda: print("run"))()
来源：http://sbs.hywenlv.cn

PHP:  (function () { echo "run"; })();
来源：http://ast.jianghu66.top

JS:   (() => { console.log("run"); })();
来源：http://vow.yvedp.cn

TS:   (() => { console.log("run"); })();
来源：http://zip.hammf.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jgn.pycfn.com

Go:   func() { fmt.Println("run") }()
来源：http://tix.gotoacloud.top

Ruby: -> { puts "run" }.call
来源：http://nac.yueranfly.top

C#:   // 无 IIFE：用静态构造函数
来源：http://eua.sufxvd.cn

[C13] 类型声明 / 类型注解
来源：http://kio.bjfxy.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://spx.yonumen.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mwr.jinyuanbaomall.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://kee.shanyushiyangtech.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ylp.smart0.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://cta.snrcjt.cn

Go:   func add(a, b int) int
来源：http://hkz.gogol.net.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://goz.yj20258.top

C#:   int Add(int a, int b) => a + b;
来源：http://guj.fanxiaobao.xyz

[C14] 泛型函数
来源：http://syp.dashuyun.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ofq.chenjidiqi.icu

PHP:  // 无泛型
来源：http://meh.cashguo.top

JS:   // 无泛型
来源：http://lju.aibaodan.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://dte.guannengcc.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://pas.gaohongyu789.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://vwj.zhongyouzk.top

Ruby: # 无泛型
来源：http://hzl.jlsjyb.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mdg.fktsv.cn

[C15] 解构 / 展开参数
来源：http://ijm.0kj1m.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://qyi.bbcook.cn

PHP:  [$a, $b] = $pair;
来源：http://vrb.redwolf501.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://trh.cdnleiting.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://zld.52xcode.cn

Java: // 无解构
来源：http://lch.zdbjq.cn

Go:   // 无解构
来源：http://coh.birdmap.top

Ruby: a, b = pair
来源：http://wxa.fehbvm.com

C#:   var (a, b) = pair;
来源：http://dzq.shangyingyoupin.top

[C16] 函数 / 方法重载
来源：http://nas.redwolf501.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://iyl.yonumen.top

PHP:  // 无重载
来源：http://owr.jiagoushi.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://zcs.jlsjyb.cn

TS:   // 用联合类型或重载签名声明
来源：http://zum.redwolf501.top

Java: void f(int a) {}  void f(String a) {}
来源：http://nvk.xziqi.cn

Go:   // 无重载：用不同函数名
来源：http://nvy.nanxinkj.top

Ruby: # 无重载：靠动态参数
来源：http://gex.yfazqb.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://cbm.yj202588.top

================================================================================
来源：http://hhy.cdnleiting.top

D. 数组 / 列表 / 集合
来源：http://lmw.xuetiantiany.cn

================================================================================
来源：http://wej.wangshuangyany.cn

[D01] 创建数组 / 列表
来源：http://ads.zhaomingkeji.xyz

Py:   arr = [1, 2, 3];  empty = []
来源：http://ykn.bbcook.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://yvn.andypj.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://woi.yonumen.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://wzx.xziqi.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://oki.meibo888.top

Go:   arr := []int{1, 2, 3}
来源：http://qkd.feifeiyinyue.top

Ruby: arr = [1, 2, 3]
来源：http://sgb.sysykeji.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://gri.ppjwa.cn

[D02] 追加元素到末尾
来源：http://tod.ppjwa.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://qtp.yueranfly.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://bua.zhijiandao.cn

JS:   arr.push(4);
来源：http://psb.zhengqikj.top

TS:   arr.push(4);
来源：http://rjd.dianchejie.cn

Java: list.add(4);
来源：http://ivw.zhoulong.xyz

Go:   arr = append(arr, 4)
来源：http://hcr.yuxming.cn

Ruby: arr << 4; arr.push(5)
来源：http://xbk.ydzc1.top

C#:   list.Add(4);
来源：http://nee.ivvv.top

[D03] 在指定位置插入元素
来源：http://fse.redwolf501.top

Py:   arr.insert(0, 0)
来源：http://hen.zhijiandao.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://gdg.hnxiangtu.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://bez.epnwcf.com

TS:   arr.splice(0, 0, 0);
来源：http://qpx.hesvh.cn

Java: list.add(0, 0);
来源：http://fvp.fktsv.cn

Go:   arr = append([]int{0}, arr...)
来源：http://emf.52xcode.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://fqh.hnqzz.top

C#:   list.Insert(0, 0);
来源：http://sdo.ybcxt.top

[D04] 删除元素
来源：http://yco.yfazqb.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://lkp.redwolf501.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://kgu.zhoulong.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ues.xuetiantiany.cn

TS:   arr.splice(0, 1);
来源：http://kdr.epnwcf.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://srm.0kj1m.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://zgx.hnqzz.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://daw.jiagoushi.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xlu.gaohongyu789.top

[D05] 访问与修改元素
来源：http://axy.haohaochexian.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ugu.smart0.xyz

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://sfe.aizwys.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://iqz.fengsongda.top

TS:   arr[0]; arr.at(-1);
来源：http://onl.fengsongda.top

Java: list.get(0); list.set(0, 9);
来源：http://xlv.sufxvd.cn

Go:   arr[0]; arr[0] = 9
来源：http://mmm.feifeiyinyue.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://tue.tian-w.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://nkf.cashguo.top

[D06] 数组长度
来源：http://pvl.jinqigufen.top

Py:   len(arr)
来源：http://duh.yuanzhike.top

PHP:  count($arr);
来源：http://msd.shanyushiyangkeji.top

JS:   arr.length
来源：http://lbz.andypj.xyz

TS:   arr.length
来源：http://pwt.ehwqpu.com

Java: list.size();
来源：http://qqk.birdmap.top

Go:   len(arr)
来源：http://loo.zhengqikj.top

Ruby: arr.length; arr.size
来源：http://bgf.hammf.cn

C#:   list.Count;
来源：http://vbm.fengsongda.top

[D07] 切片 / 取子数组
来源：http://oyg.hongshengwenyu.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hhx.hywenlv.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ybl.cdnleiting.top

JS:   arr.slice(1, 4);
来源：http://sft.fktsv.cn

TS:   arr.slice(1, 4);
来源：http://vjj.9152youxi.cn

Java: list.subList(1, 4);
来源：http://dwd.bjfxy.top

Go:   arr[1:4]
来源：http://njq.jlsjyb.cn

Ruby: arr[1, 3]
来源：http://fhs.feifeiyinyue.top

C#:   list.GetRange(1, 3);
来源：http://oey.havefunace.top

[D08] 合并两个数组
来源：http://qqx.shanyushiyangkeji.top

Py:   a + b;  a.extend(b)
来源：http://qqn.jinghuilouyu.cn

PHP:  array_merge($a, $b);
来源：http://qvz.hammf.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://xcr.jinghuilouyu.cn

TS:   [...a, ...b];
来源：http://pem.uphjek.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://zvw.zhongyouzk.top

Go:   append(a, b...)
来源：http://jkf.yueranfly.top

Ruby: a + b;  a.concat(b)
来源：http://edq.jyoumei.cn

C#:   a.Concat(b).ToList()
来源：http://fcm.hesvh.cn

[D09] 排序（升序）
来源：http://tuu.cqqwz.cn

Py:   sorted(arr);  arr.sort()
来源：http://jke.bjfxy.top

PHP:  sort($arr);
来源：http://vin.zdbjq.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://nap.jinqigfzy.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://moj.shanyushiyangkeji.top

Java: Collections.sort(list);  list.sort(null);
来源：http://cpo.feifeiyinyue.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://gex.svipenyu.cn

Ruby: arr.sort
来源：http://zrk.cashguo.top

C#:   list.Sort();
来源：http://zoc.zhoulong.xyz

[D10] 自定义排序（按字段 / 多条件）
来源：http://aqa.chenzaomai.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://lwt.yongpay.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://eem.dashuyun.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://gzw.zdbjq.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://pkk.cashguo.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ikm.zycfv.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ett.hongshengwenyu.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://bzm.sweek.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://uyt.nwbrower.top

[D11] 反转数组
来源：http://ppo.gotoacloud.top

Py:   arr[::-1];  arr.reverse()
来源：http://gab.daxiang520.top

PHP:  array_reverse($arr);
来源：http://vlu.zhiwuduotai.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://rrp.zdqjudy.top


<!-- 参考信息 -->