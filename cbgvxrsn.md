代发 wailian999

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://agm.shuidangran.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qrg.chenzaomai.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://rya.zhijiandao.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://spp.zhixingplan.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xyu.yanxiufei.cn

[B10] 遍历同时拿索引
来源：http://woh.c1oappe.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ihh.nanxinkj.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hvu.zhijiandao.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://rhg.pycfn.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://koy.zhoulong.xyz

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://sgy.epnwcf.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://qsl.feifeiyinyue.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wcq.jinyuanbaomall.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wel.fzhhl.top

[B11] 生成数字序列 / 区间
来源：http://pib.hysaishi.cn

Py:   list(range(0, 10, 2))
来源：http://aom.chenzaomai.com

PHP:  range(0, 10, 2);
来源：http://fuy.jiagoushi.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://byc.0kj1m.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lqe.xuanzx.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://aaa.zhengqikj.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://woj.shanyushiyangkeji.top

Ruby: (0...10).step(2).to_a
来源：http://iai.hnqzz.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ijf.xylfe.cn

[B12] 跳出多层循环
来源：http://xyl.vqdsnc.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://xeq.birdmap.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://mtx.jinyuanbaomall.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://pcb.sysykeji.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://nnm.cdnleiting.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://gyo.daxiang520.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://dig.tarul.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://tnb.hcnkem.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://afr.yj20258.top

[B13] 判断是否为数字
来源：http://clk.ctjpmb.com

Py:   isinstance(x, (int, float))
来源：http://xij.andypj.xyz

PHP:  is_numeric($x)
来源：http://gid.ehwqpu.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wrx.snrcjt.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://iks.jiagoushi.top

Java: x instanceof Number
来源：http://eoi.jinyuanbaomall.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://jnv.ydjk.org.cn

Ruby: x.is_a?(Numeric)
来源：http://qwo.epnwcf.com

C#:   x is int or double or decimal
来源：http://cdv.hammf.cn

[B14] 判断值是否在集合内
来源：http://hzh.birdmap.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://vxf.meibo888.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://pcn.zhijiandao.cn

JS:   [1, 2, 3].includes(x)
来源：http://ryh.chenzaomai.com

TS:   [1, 2, 3].includes(x)
来源：http://qtb.aibaodan.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://rqk.fehbvm.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://twu.zhaomingkeji.xyz

Ruby: [1, 2, 3].include?(x)
来源：http://zbx.yfazqb.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://nwn.sweek.top

[B15] 布尔运算与取反
来源：http://lyu.smart0.xyz

Py:   a and b or not c
来源：http://uyz.yanxiufei.cn

PHP:  $a && $b || !$c
来源：http://iwv.hfpthk.cn

JS:   a && b || !c
来源：http://aaq.yj202588.top

TS:   a && b || !c
来源：http://wcx.sxryk.cn

Java: a && b || !c
来源：http://ugn.9152youxi.cn

Go:   a && b || !c
来源：http://tgz.jlsjyb.cn

Ruby: a && b || !c
来源：http://qhb.9152youxi.cn

C#:   a && b || !c
来源：http://oqs.xingfuxueyuan.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://nag.vqdsnc.cn

Py:   if not data: return
来源：http://lzb.birdmap.top

PHP:  if (!$data) { return; }
来源：http://bnk.wangshuangyany.cn

JS:   if (!data) return;
来源：http://cur.gotoacloud.top

TS:   if (!data) return;
来源：http://dni.tian-w.cn

Java: if (data == null) return;
来源：http://dnu.yonumen.top

Go:   if data == nil { return }
来源：http://osk.jlsjyb.cn

Ruby: return if data.nil?
来源：http://khd.zycfv.cn

C#:   if (data == null) return;
来源：http://mwk.yj20258888.top

================================================================================
来源：http://wja.chenjidiqi.icu

C. 函数与作用域
来源：http://bac.ydjk.org.cn

================================================================================
来源：http://ksq.wangshuangyany.cn

[C01] 定义函数
来源：http://zut.jiagoushi.top

Py:   def add(a, b): return a + b
来源：http://zmi.tianlin.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wyt.zycfv.cn

JS:   function add(a, b) { return a + b; }
来源：http://ugy.jiagoushi.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kdj.dianchejie.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://imx.yongpay.top

Go:   func add(a, b int) int { return a + b }
来源：http://wwd.xuanzx.com

Ruby: def add(a, b); a + b; end
来源：http://hkh.yanxiufei.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://gmf.tianlin.xyz

[C02] 默认参数
来源：http://orf.jlsjyb.cn

Py:   def greet(name="World"): return name
来源：http://nht.fanxiaobao.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://zsn.bjfxy.top

JS:   function greet(name = "World") { return name; }
来源：http://mnx.yj20258.top

TS:   function greet(name: string = "World") { return name; }
来源：http://acf.havefunace.top

Java: // 无默认参数：方法重载或 Optional
来源：http://jfp.mhx1999.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://qfn.cashguo.top

Ruby: def greet(name = "World") = name
来源：http://uuu.sysykeji.top

C#:   string Greet(string name = "World") => name;
来源：http://vgc.tianlin.xyz

[C03] 可变参数
来源：http://qfv.shzxlz.cn

Py:   def total(*args): return sum(args)
来源：http://obh.zhoulong.xyz

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ccg.iojbl.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://vrw.xinyue.icu

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wdq.dianchejie.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://suh.yongpay.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://odr.havefunace.top

Ruby: def total(*nums); nums.sum; end
来源：http://aom.ppjwa.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ydu.uphjek.com

[C04] 命名参数 / 关键字参数
来源：http://ozz.fktsv.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://iwd.guowangkeji.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mib.chenjidiqi.icu

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://epe.hnxiangtu.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://qre.bbcook.cn

Java: // 无：用 Builder 模式或 record
来源：http://gpy.cucudq.cn

Go:   // 无：用配置结构体参数
来源：http://qbj.fanxiaobao.xyz

Ruby: f(a: 1, b: 2)
来源：http://ugr.cheryme.top

C#:   f(a: 1, b: 2)
来源：http://wbp.zhongyouzk.top

[C05] 返回多个值
来源：http://vsp.cucudq.cn

Py:   return a, b
来源：http://stm.wangdashe.top

PHP:  return [$a, $b];
来源：http://tnd.xziqi.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://kex.nanxinkj.top

TS:   return { a, b };
来源：http://klw.bjfxy.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://gxs.tanke756.top

Go:   return a, b
来源：http://vfl.shzxlz.cn

Ruby: return a, b
来源：http://kkh.xziqi.cn

C#:   return (a, b);              // ValueTuple
来源：http://uqq.yj20258.top

[C06] 匿名函数 / lambda
来源：http://zed.ydjk.org.cn

Py:   square = lambda x: x * x
来源：http://kqy.shuidangran.top

PHP:  $square = fn($x) => $x * $x;
来源：http://zzh.mhx1999.top

JS:   const square = x => x * x;
来源：http://wus.vqdsnc.cn

TS:   const square = (x: number): number => x * x;
来源：http://mxr.ywan-chungtsiang.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://jle.yvedp.cn

Go:   sq := func(x int) int { return x * x }
来源：http://yuy.yfazqb.com

Ruby: square = ->(x) { x * x }
来源：http://vkr.hnqzz.top

C#:   Func<int, int> square = x => x * x;
来源：http://ezh.xingfuxueyuan.xyz

[C07] 把函数作为参数传入
来源：http://rfc.52xcode.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hmd.hysaishi.cn

PHP:  array_map("strtoupper", $arr);
来源：http://udr.fengsongda.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://jdv.tanke756.top

TS:   arr.map(String)
来源：http://kam.chenzaomai.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ivw.feifeiyinyue.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://yva.sweek.top

Ruby: arr.map(&:upcase)
来源：http://cpg.bbcook.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://uyu.316326.xyz

[C08] 闭包
来源：http://udm.feifeiyinyue.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://phr.uphjek.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://lnf.xinyue.icu

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://tpy.yj20258888.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wsm.hesvh.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://oom.xuetiantiany.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jfz.andypj.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ees.jiagoushi.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://eco.wangshuangyany.cn

[C09] 递归
来源：http://cfs.fanxiaobao.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wmu.tianlin.xyz

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hts.yangfankeji.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ivk.redwolf501.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ijw.meibo888.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hgr.epnwcf.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://vtc.redwolf501.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ilf.jqgufenzy.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://vzh.xinyue.icu

[C10] 变量作用域
来源：http://xch.jinyuanbaomall.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://flm.svipenyu.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://qzg.wangdashe.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://cpk.hcnkem.com

TS:   同 JS
来源：http://gfb.yfazqb.com

Java: 方法内为块级作用域
来源：http://icn.nwbrower.top

Go:   花括号块级作用域
来源：http://nie.xinyue.icu

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://cys.yj20258.top

C#:   块级作用域
来源：http://yrs.ybcxt.top

[C11] 模块导入与导出
来源：http://bmd.yj20258888.top

Py:   from module import func
来源：http://nfa.vqdsnc.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://lzd.tianlin.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://dew.jyoumei.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://bgl.daria6918.cn

Java: import java.util.List;
来源：http://chl.feifeiyinyue.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hkp.zhengqikj.top

Ruby: require "json"; require_relative "./util"
来源：http://tiu.zycfv.cn

C#:   using System.Text;
来源：http://cdj.zhaomingkeji.xyz

[C12] 立即执行函数 IIFE
来源：http://tfd.316326.xyz

Py:   (lambda: print("run"))()
来源：http://viu.cdnleiting.top

PHP:  (function () { echo "run"; })();
来源：http://yxr.jiagoushi.top

JS:   (() => { console.log("run"); })();
来源：http://amz.smart0.xyz

TS:   (() => { console.log("run"); })();
来源：http://roa.xingfuxueyuan.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://gaf.hammf.cn

Go:   func() { fmt.Println("run") }()
来源：http://hbv.zhongyouzk.top

Ruby: -> { puts "run" }.call
来源：http://rti.kuanghao11.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://goo.snrcjt.cn

[C13] 类型声明 / 类型注解
来源：http://tvl.yfazqb.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://jqb.hongshengwenyu.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zel.ivvv.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://afn.shanyushiyangtech.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ukb.sweek.top

Java: int add(int a, int b) { return a + b; }
来源：http://jtj.shuidangran.top

Go:   func add(a, b int) int
来源：http://zql.cdnleiting.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://adv.tarul.cn

C#:   int Add(int a, int b) => a + b;
来源：http://aqe.sxryk.cn

[C14] 泛型函数
来源：http://alf.wangshuangyany.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://vhj.dashuyun.cn

PHP:  // 无泛型
来源：http://dnz.jinqigufen.top

JS:   // 无泛型
来源：http://qxw.daria6918.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://uaj.jqgfzy.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://tmx.gaohongyu789.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://igs.nwbrower.top

Ruby: # 无泛型
来源：http://vqg.quarkkingdee.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ivv.fanxiaobao.xyz

[C15] 解构 / 展开参数
来源：http://zfn.pycfn.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://qvj.gaohongyu789.top

PHP:  [$a, $b] = $pair;
来源：http://hcp.dashuyun.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://jcn.wangshuangyany.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://dza.jyoumei.cn

Java: // 无解构
来源：http://iko.vqdsnc.cn

Go:   // 无解构
来源：http://wkv.daxiang520.top

Ruby: a, b = pair
来源：http://gij.nwbrower.top

C#:   var (a, b) = pair;
来源：http://guo.tianlin.xyz

[C16] 函数 / 方法重载
来源：http://bpm.epnwcf.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://rgh.mhx1999.top

PHP:  // 无重载
来源：http://mpq.ywan-chungtsiang.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://meb.xinyue.icu

TS:   // 用联合类型或重载签名声明
来源：http://gvn.smart0.xyz

Java: void f(int a) {}  void f(String a) {}
来源：http://kvy.sweek.top

Go:   // 无重载：用不同函数名
来源：http://iec.xylfe.cn

Ruby: # 无重载：靠动态参数
来源：http://bxu.sxryk.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://txl.chenzaomai.com

================================================================================
来源：http://yfc.bbcook.cn

D. 数组 / 列表 / 集合
来源：http://mmw.bjfxy.top

================================================================================
来源：http://qav.yj20258.top

[D01] 创建数组 / 列表
来源：http://gqu.zdbjq.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://xsi.aizwys.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://uqp.tian-w.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://own.hammf.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://szv.hammf.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://rig.52xcode.cn

Go:   arr := []int{1, 2, 3}
来源：http://lhv.snrcjt.cn

Ruby: arr = [1, 2, 3]
来源：http://etx.mhx1999.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://rmy.smart0.xyz

[D02] 追加元素到末尾
来源：http://ita.snrcjt.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://pgo.xingfuxueyuan.xyz

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hqq.yj202588.top

JS:   arr.push(4);
来源：http://eqv.kuanghao11.cn

TS:   arr.push(4);
来源：http://fpt.meibo888.top

Java: list.add(4);
来源：http://mjl.zhengqikj.top

Go:   arr = append(arr, 4)
来源：http://rno.wangdashe.top

Ruby: arr << 4; arr.push(5)
来源：http://drd.pengpengdd.cyou

C#:   list.Add(4);
来源：http://ibo.yuanzhike.top

[D03] 在指定位置插入元素
来源：http://nam.shanyushiyangtech.top

Py:   arr.insert(0, 0)
来源：http://kch.hammf.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://oiu.shanyushiyangtech.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ckr.ctjpmb.com

TS:   arr.splice(0, 0, 0);
来源：http://vgq.mhx1999.top

Java: list.add(0, 0);
来源：http://dth.daxiang520.top

Go:   arr = append([]int{0}, arr...)
来源：http://vqp.fzhhl.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wgl.zhaomingkeji.xyz

C#:   list.Insert(0, 0);
来源：http://lud.xingfuxueyuan.xyz

[D04] 删除元素
来源：http://hyf.andypj.xyz

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ekp.meibo888.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://nfr.epnwcf.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xmo.c1oappe.top

TS:   arr.splice(0, 1);
来源：http://eam.yj202588.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://knx.tianlin.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://dfi.zhoulong.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ypo.xziqi.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://erc.ivvv.top

[D05] 访问与修改元素
来源：http://rvd.jinghuilouyu.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://szg.yueranfly.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://xga.ppjwa.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://tpv.yongpay.top

TS:   arr[0]; arr.at(-1);
来源：http://xgf.aizwys.cn

Java: list.get(0); list.set(0, 9);
来源：http://ftu.smart0.xyz

Go:   arr[0]; arr[0] = 9
来源：http://wfi.sjlbkw.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://fwh.zhoulong.xyz

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://pdq.ydzc1.top

[D06] 数组长度
来源：http://ggf.tanke756.top

Py:   len(arr)
来源：http://cvh.havefunace.top

PHP:  count($arr);
来源：http://bza.jinghuilouyu.cn

JS:   arr.length
来源：http://sjk.cucudq.cn

TS:   arr.length
来源：http://ppq.haohaochexian.top

Java: list.size();
来源：http://clo.xuetiantiany.cn

Go:   len(arr)
来源：http://xxj.yj20258.top

Ruby: arr.length; arr.size
来源：http://keg.hongshengwenyu.top

C#:   list.Count;
来源：http://urc.ivvv.top

[D07] 切片 / 取子数组
来源：http://fhx.aizwys.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://siy.mhx1999.top

PHP:  array_slice($arr, 1, 3);
来源：http://hyk.zycfv.cn

JS:   arr.slice(1, 4);
来源：http://ggn.sjlbkw.cn

TS:   arr.slice(1, 4);
来源：http://owb.yuanzhike.top

Java: list.subList(1, 4);
来源：http://bur.andypj.xyz

Go:   arr[1:4]
来源：http://nzn.nwbrower.top

Ruby: arr[1, 3]
来源：http://req.mhx1999.top

C#:   list.GetRange(1, 3);
来源：http://pqe.cdnleiting.top

[D08] 合并两个数组
来源：http://snt.xylfe.cn

Py:   a + b;  a.extend(b)
来源：http://fmu.epnwcf.com

PHP:  array_merge($a, $b);
来源：http://dtz.daria6918.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://atc.iojbl.cn

TS:   [...a, ...b];
来源：http://obm.cqqwz.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://dst.hfpthk.cn

Go:   append(a, b...)
来源：http://mic.aibaodan.cn

Ruby: a + b;  a.concat(b)
来源：http://tjv.zhixingplan.top

C#:   a.Concat(b).ToList()
来源：http://cfu.ybcxt.top

[D09] 排序（升序）
来源：http://nca.svipenyu.cn

Py:   sorted(arr);  arr.sort()
来源：http://hgl.fehbvm.com

PHP:  sort($arr);
来源：http://gpk.wangshuangyany.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ypq.jinqigfzy.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://diu.epnwcf.com

Java: Collections.sort(list);  list.sort(null);
来源：http://tda.jinyuanbaomall.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://rdg.fanxiaobao.xyz

Ruby: arr.sort
来源：http://uhx.jinqigfzy.top

C#:   list.Sort();
来源：http://tcx.wangdashe.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://qsq.zdqjudy.top


<!-- 参考信息 -->