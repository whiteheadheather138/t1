代发 wailian999

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://zzt.fzhhl.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://did.hnqzz.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://qyi.jiagoushi.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://pqx.xuanzx.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://eyu.sysykeji.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://kuh.tanke756.top

[B11] 生成数字序列 / 区间
来源：http://eyh.jlsjyb.cn

Py:   list(range(0, 10, 2))
来源：http://opd.tanke756.top

PHP:  range(0, 10, 2);
来源：http://ddl.meibo888.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qgt.yuxming.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cbl.nanxuanxn.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://kty.epnwcf.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://qmm.jyoumei.cn

Ruby: (0...10).step(2).to_a
来源：http://qbn.cashguo.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://rnm.ydjk.org.cn

[B12] 跳出多层循环
来源：http://shl.tianlin.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://mec.ppjwa.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ihs.jqgfzy.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ten.52xcode.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://gxx.vehdjk.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://toh.9152youxi.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://gmj.ehwqpu.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://lvv.guannengcc.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://txp.wangdashe.top

[B13] 判断是否为数字
来源：http://spz.chenjidiqi.icu

Py:   isinstance(x, (int, float))
来源：http://wad.shzxlz.cn

PHP:  is_numeric($x)
来源：http://rie.sysykeji.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dfu.meibo888.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jwl.meibo888.top

Java: x instanceof Number
来源：http://lkv.shangyingyoupin.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://uqq.andypj.xyz

Ruby: x.is_a?(Numeric)
来源：http://pxo.bbcook.cn

C#:   x is int or double or decimal
来源：http://qbi.ydzc1.top

[B14] 判断值是否在集合内
来源：http://fux.fzhhl.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://rzy.shanyushiyangkeji.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://von.epnwcf.com

JS:   [1, 2, 3].includes(x)
来源：http://tgm.ehwqpu.com

TS:   [1, 2, 3].includes(x)
来源：http://dil.chenzaomai.com

Java: List.of(1, 2, 3).contains(x)
来源：http://rbp.kuanghao11.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wpo.hnqzz.top

Ruby: [1, 2, 3].include?(x)
来源：http://zsb.tanke756.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://vew.chenzaomai.com

[B15] 布尔运算与取反
来源：http://aml.cqqwz.cn

Py:   a and b or not c
来源：http://iwo.ehwqpu.com

PHP:  $a && $b || !$c
来源：http://uxa.epnwcf.com

JS:   a && b || !c
来源：http://igj.xuetiantiany.cn

TS:   a && b || !c
来源：http://rxl.yj20258.top

Java: a && b || !c
来源：http://kgu.zhiwuduotai.top

Go:   a && b || !c
来源：http://wag.epnwcf.com

Ruby: a && b || !c
来源：http://sfs.chenzaomai.com

C#:   a && b || !c
来源：http://ruq.hysaishi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://spu.sxryk.cn

Py:   if not data: return
来源：http://lck.tian-w.cn

PHP:  if (!$data) { return; }
来源：http://fdp.ppjwa.cn

JS:   if (!data) return;
来源：http://rrk.bbcook.cn

TS:   if (!data) return;
来源：http://bpi.xinyue.icu

Java: if (data == null) return;
来源：http://enc.vqdsnc.cn

Go:   if data == nil { return }
来源：http://oje.9152youxi.cn

Ruby: return if data.nil?
来源：http://bal.kuanghao11.cn

C#:   if (data == null) return;
来源：http://zcz.andypj.xyz

================================================================================
来源：http://ztd.hywenlv.cn

C. 函数与作用域
来源：http://mrj.wangshuangyany.cn

================================================================================
来源：http://ncb.andypj.xyz

[C01] 定义函数
来源：http://sse.yongpay.top

Py:   def add(a, b): return a + b
来源：http://lva.hfpthk.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://njj.chenjidiqi.icu

JS:   function add(a, b) { return a + b; }
来源：http://uon.yuxming.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kaq.guowangkeji.top

Java: static int add(int a, int b) { return a + b; }
来源：http://put.yj202588.top

Go:   func add(a, b int) int { return a + b }
来源：http://qer.fengsongda.top

Ruby: def add(a, b); a + b; end
来源：http://adv.pycfn.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://kel.vehdjk.com

[C02] 默认参数
来源：http://qws.cashguo.top

Py:   def greet(name="World"): return name
来源：http://pjy.ivvv.top

PHP:  function greet($name = "World") { return $name; }
来源：http://bgn.xuetiantiany.cn

JS:   function greet(name = "World") { return name; }
来源：http://jhp.hnqzz.top

TS:   function greet(name: string = "World") { return name; }
来源：http://tog.birdmap.top

Java: // 无默认参数：方法重载或 Optional
来源：http://bzd.jiagoushi.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://lrv.pengpengdd.cyou

Ruby: def greet(name = "World") = name
来源：http://caf.nanxuanxn.top

C#:   string Greet(string name = "World") => name;
来源：http://fwx.52xcode.cn

[C03] 可变参数
来源：http://qwt.52xcode.cn

Py:   def total(*args): return sum(args)
来源：http://ywp.svipenyu.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://jjx.bbcook.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://yix.aibaodan.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://twt.guannengcc.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://snb.ivvv.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://eeb.smart0.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://joi.cucudq.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ntr.gzhubu.top

[C04] 命名参数 / 关键字参数
来源：http://cba.zhoulong.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://coz.cashguo.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://med.havefunace.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://agx.zhiwuduotai.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://yga.fehbvm.com

Java: // 无：用 Builder 模式或 record
来源：http://qba.hfpthk.cn

Go:   // 无：用配置结构体参数
来源：http://exc.chenjidiqi.icu

Ruby: f(a: 1, b: 2)
来源：http://wog.hcnkem.com

C#:   f(a: 1, b: 2)
来源：http://pep.xingfuxueyuan.xyz

[C05] 返回多个值
来源：http://krw.tianlin.xyz

Py:   return a, b
来源：http://oxn.zhoulong.xyz

PHP:  return [$a, $b];
来源：http://utx.jqgfzy.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://lnr.epnwcf.com

TS:   return { a, b };
来源：http://ozl.ywan-chungtsiang.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://khw.fzhhl.top

Go:   return a, b
来源：http://wyr.jqgufenzy.top

Ruby: return a, b
来源：http://hnh.tianlin.xyz

C#:   return (a, b);              // ValueTuple
来源：http://yzu.daria6918.cn

[C06] 匿名函数 / lambda
来源：http://cfx.wangshuangyany.cn

Py:   square = lambda x: x * x
来源：http://luw.cashguo.top

PHP:  $square = fn($x) => $x * $x;
来源：http://loq.shuidangran.top

JS:   const square = x => x * x;
来源：http://cqv.xingfuxueyuan.xyz

TS:   const square = (x: number): number => x * x;
来源：http://hho.jinyuanbaomall.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mbb.sweek.top

Go:   sq := func(x int) int { return x * x }
来源：http://pke.zhijiandao.cn

Ruby: square = ->(x) { x * x }
来源：http://wam.hnqzz.top

C#:   Func<int, int> square = x => x * x;
来源：http://kpg.tanke756.top

[C07] 把函数作为参数传入
来源：http://bnw.xylfe.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ufx.xziqi.cn

PHP:  array_map("strtoupper", $arr);
来源：http://hkg.zycfv.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://pyv.cucudq.cn

TS:   arr.map(String)
来源：http://gfb.ywan-chungtsiang.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wjz.sysykeji.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://aoa.xylfe.cn

Ruby: arr.map(&:upcase)
来源：http://dqz.iojbl.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ror.zhongyouzk.top

[C08] 闭包
来源：http://lsz.bbcook.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mdv.pycfn.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://vak.daxiang520.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://fvo.epnwcf.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://veb.fktsv.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://enk.yj202588.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wmy.0kj1m.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://lmy.zhengqikj.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://goy.yuxming.cn

[C09] 递归
来源：http://lky.zdbjq.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://itg.fktsv.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://csv.sjlbkw.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://djf.9152youxi.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ris.ydzc1.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://irv.hammf.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://jkg.jqgufenzy.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://omz.zhoulong.xyz

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://cnk.gaohongyu789.top

[C10] 变量作用域
来源：http://ann.c1oappe.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ebu.meibo888.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://fuo.andypj.xyz

JS:   let/const 块级作用域，var 函数级作用域
来源：http://gjt.xinyue.icu

TS:   同 JS
来源：http://yqa.aizwys.cn

Java: 方法内为块级作用域
来源：http://zbe.chenzaomai.com

Go:   花括号块级作用域
来源：http://ffw.sufxvd.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://jag.bjfxy.top

C#:   块级作用域
来源：http://euk.smart0.xyz

[C11] 模块导入与导出
来源：http://deh.hfpthk.cn

Py:   from module import func
来源：http://pqv.yanxiufei.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://tnx.iojbl.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://oxn.guannengcc.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hhn.sxryk.cn

Java: import java.util.List;
来源：http://lgb.gogol.net.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://kmj.hammf.cn

Ruby: require "json"; require_relative "./util"
来源：http://lcm.smart0.xyz

C#:   using System.Text;
来源：http://edu.xuanzx.com

[C12] 立即执行函数 IIFE
来源：http://hwk.hcnkem.com

Py:   (lambda: print("run"))()
来源：http://jtz.jianghu66.top

PHP:  (function () { echo "run"; })();
来源：http://nlx.shangyingyoupin.top

JS:   (() => { console.log("run"); })();
来源：http://hxi.yueranfly.top

TS:   (() => { console.log("run"); })();
来源：http://ysf.yanxiufei.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://rbw.xziqi.cn

Go:   func() { fmt.Println("run") }()
来源：http://rac.hesvh.cn

Ruby: -> { puts "run" }.call
来源：http://oms.vehdjk.com

C#:   // 无 IIFE：用静态构造函数
来源：http://iob.zhijiandao.cn

[C13] 类型声明 / 类型注解
来源：http://gdn.guannengcc.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://cra.wangshuangyany.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://drg.jinqigufen.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://lcn.nwbrower.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://abg.zhongyouzk.top

Java: int add(int a, int b) { return a + b; }
来源：http://ssh.shzxlz.cn

Go:   func add(a, b int) int
来源：http://afr.daria6918.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://zge.ppjwa.cn

C#:   int Add(int a, int b) => a + b;
来源：http://plt.yj20258.top

[C14] 泛型函数
来源：http://qqg.cucudq.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zvy.mhx1999.top

PHP:  // 无泛型
来源：http://exr.zhengqikj.top

JS:   // 无泛型
来源：http://zpo.hywenlv.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ltf.jyoumei.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://zal.chenlongwang.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://nww.daxiang520.top

Ruby: # 无泛型
来源：http://qhn.nanxinkj.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://tjp.daxiang520.top

[C15] 解构 / 展开参数
来源：http://lxh.birdmap.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://osy.bjfxy.top

PHP:  [$a, $b] = $pair;
来源：http://hhr.meibo888.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://cpd.zdqjudy.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://rrs.fanxiaobao.xyz

Java: // 无解构
来源：http://ybk.xuanzx.com

Go:   // 无解构
来源：http://keq.redwolf501.top

Ruby: a, b = pair
来源：http://rso.shuidangran.top

C#:   var (a, b) = pair;
来源：http://sez.yj20258888.top

[C16] 函数 / 方法重载
来源：http://rje.hammf.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://xan.cucudq.cn

PHP:  // 无重载
来源：http://iuu.shanyushiyangtech.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://iyn.smart0.xyz

TS:   // 用联合类型或重载签名声明
来源：http://bjh.hnxiangtu.top

Java: void f(int a) {}  void f(String a) {}
来源：http://txu.jinghuilouyu.cn

Go:   // 无重载：用不同函数名
来源：http://uca.cucudq.cn

Ruby: # 无重载：靠动态参数
来源：http://khu.ivvv.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://hgx.vqdsnc.cn

================================================================================
来源：http://npa.chenzaomai.com

D. 数组 / 列表 / 集合
来源：http://ctk.zycfv.cn

================================================================================
来源：http://gkn.nwbrower.top

[D01] 创建数组 / 列表
来源：http://lqi.hysaishi.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://hbs.shanyushiyangkeji.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://aig.daxiang520.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wzx.ywan-chungtsiang.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://izq.dianchejie.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://phk.nanxuanxn.top

Go:   arr := []int{1, 2, 3}
来源：http://zlb.shanyushiyangkeji.top

Ruby: arr = [1, 2, 3]
来源：http://jom.svipenyu.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://czn.yj20258888.top

[D02] 追加元素到末尾
来源：http://gud.yj20258888.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://xmx.hysaishi.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://jhj.316326.xyz

JS:   arr.push(4);
来源：http://yhf.fengsongda.top

TS:   arr.push(4);
来源：http://jkn.yvedp.cn

Java: list.add(4);
来源：http://oyu.316326.xyz

Go:   arr = append(arr, 4)
来源：http://hzd.c1oappe.top

Ruby: arr << 4; arr.push(5)
来源：http://tkf.yongpay.top

C#:   list.Add(4);
来源：http://zre.tianlin.xyz

[D03] 在指定位置插入元素
来源：http://ior.cqqwz.cn

Py:   arr.insert(0, 0)
来源：http://kdc.fehbvm.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://kar.nwbrower.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://kep.ydjk.org.cn

TS:   arr.splice(0, 0, 0);
来源：http://ojn.gzhubu.top

Java: list.add(0, 0);
来源：http://gip.yongpay.top

Go:   arr = append([]int{0}, arr...)
来源：http://qqy.yonumen.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://jnz.hnqzz.top

C#:   list.Insert(0, 0);
来源：http://awt.zdbjq.cn

[D04] 删除元素
来源：http://csm.aizwys.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://gvy.hnqzz.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://iam.yonumen.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ota.yfazqb.com

TS:   arr.splice(0, 1);
来源：http://msk.sufxvd.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://tcq.svipenyu.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://boj.cheryme.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://htu.snrcjt.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://vpj.zhoulong.xyz

[D05] 访问与修改元素
来源：http://pqr.sjlbkw.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://yqc.xuanzx.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://pql.redwolf501.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://zcw.jianghu66.top

TS:   arr[0]; arr.at(-1);
来源：http://ilz.52xcode.cn

Java: list.get(0); list.set(0, 9);
来源：http://hjm.ywan-chungtsiang.top

Go:   arr[0]; arr[0] = 9
来源：http://fdm.yuxming.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ili.feifeiyinyue.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zvf.birdmap.top

[D06] 数组长度
来源：http://bzo.nanxinkj.top

Py:   len(arr)
来源：http://gzv.zhengqikj.top

PHP:  count($arr);
来源：http://jvw.zhengqikj.top

JS:   arr.length
来源：http://wnv.kuanghao11.cn

TS:   arr.length
来源：http://rqb.bbcook.cn

Java: list.size();
来源：http://mob.gotoacloud.top

Go:   len(arr)
来源：http://mdh.bjfxy.top

Ruby: arr.length; arr.size
来源：http://zkp.fanxiaobao.xyz

C#:   list.Count;
来源：http://baa.bjfxy.top

[D07] 切片 / 取子数组
来源：http://hzl.vehdjk.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ljg.gogol.net.cn

PHP:  array_slice($arr, 1, 3);
来源：http://yoi.xingfuxueyuan.xyz

JS:   arr.slice(1, 4);
来源：http://eoq.9152youxi.cn

TS:   arr.slice(1, 4);
来源：http://uzk.chenzaomai.com

Java: list.subList(1, 4);
来源：http://egx.pycfn.com

Go:   arr[1:4]
来源：http://fex.nanxuanxn.top

Ruby: arr[1, 3]
来源：http://mwk.yanxiufei.cn

C#:   list.GetRange(1, 3);
来源：http://avq.uphjek.com

[D08] 合并两个数组
来源：http://jsm.shanyushiyangkeji.top

Py:   a + b;  a.extend(b)
来源：http://qrn.zhengqikj.top

PHP:  array_merge($a, $b);
来源：http://cvc.zhongyouzk.top

JS:   [...a, ...b];  a.concat(b);
来源：http://foj.yuxming.cn

TS:   [...a, ...b];
来源：http://sjq.shuidangran.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://gdn.ctjpmb.com

Go:   append(a, b...)
来源：http://mry.chenzaomai.com

Ruby: a + b;  a.concat(b)
来源：http://utt.hcnkem.com

C#:   a.Concat(b).ToList()
来源：http://ila.cheryme.top

[D09] 排序（升序）
来源：http://lej.guowangkeji.top

Py:   sorted(arr);  arr.sort()
来源：http://nat.gogol.net.cn

PHP:  sort($arr);
来源：http://ymd.aibaodan.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://qfc.xziqi.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://fvz.smart0.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://idx.yvedp.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hae.ivvv.top

Ruby: arr.sort
来源：http://cak.zhaomingkeji.xyz

C#:   list.Sort();
来源：http://hod.wangshuangyany.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://wdp.shuidangran.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://alh.gogol.net.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lle.guannengcc.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ceo.hysaishi.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://xqy.chenzaomai.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ork.ehwqpu.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://jjv.ppjwa.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://sjj.chenlongwang.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://iin.jinghuilouyu.cn


<!-- 参考信息 -->