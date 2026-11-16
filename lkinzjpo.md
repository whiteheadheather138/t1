代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vyw.yuxming.cn

[B10] 遍历同时拿索引
来源：http://bpu.52xcode.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://gdy.sjlbkw.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://bqb.guowangkeji.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://sjq.fengsongda.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://zkf.yonumen.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://nnt.nanxuanxn.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://zuf.shangyingyoupin.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://qjd.jinqigfzy.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://pmo.feifeiyinyue.top

[B11] 生成数字序列 / 区间
来源：http://vsd.zycfv.cn

Py:   list(range(0, 10, 2))
来源：http://vog.jqgufenzy.top

PHP:  range(0, 10, 2);
来源：http://jjw.smart0.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hlx.jinghuilouyu.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://civ.yvedp.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://qvr.yuanzhike.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ygd.hnxiangtu.top

Ruby: (0...10).step(2).to_a
来源：http://lbw.yj20258.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mfz.cqqwz.cn

[B12] 跳出多层循环
来源：http://tsx.hnxiangtu.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://ktd.gzhubu.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://fii.zdqjudy.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://zgr.gotoacloud.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ava.yvedp.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://obf.xziqi.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://cpy.zhaomingkeji.xyz

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://nmv.vqdsnc.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wxx.fzhhl.top

[B13] 判断是否为数字
来源：http://onf.zdbjq.cn

Py:   isinstance(x, (int, float))
来源：http://ike.yangfankeji.com

PHP:  is_numeric($x)
来源：http://bha.chenjidiqi.icu

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://olr.zdbjq.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rte.feifeiyinyue.top

Java: x instanceof Number
来源：http://tyq.yj202588.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ili.jqgufenzy.top

Ruby: x.is_a?(Numeric)
来源：http://mxz.gzhubu.top

C#:   x is int or double or decimal
来源：http://rqa.yuanzhike.top

[B14] 判断值是否在集合内
来源：http://zvd.gogol.net.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://zna.kuanghao11.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://bol.yongpay.top

JS:   [1, 2, 3].includes(x)
来源：http://atl.uphjek.com

TS:   [1, 2, 3].includes(x)
来源：http://ocv.nwbrower.top

Java: List.of(1, 2, 3).contains(x)
来源：http://zwt.aizwys.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://szo.hysaishi.cn

Ruby: [1, 2, 3].include?(x)
来源：http://fqs.c1oappe.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://zfw.ppjwa.cn

[B15] 布尔运算与取反
来源：http://mqb.fzhhl.top

Py:   a and b or not c
来源：http://czk.cqqwz.cn

PHP:  $a && $b || !$c
来源：http://qtk.quarkkingdee.top

JS:   a && b || !c
来源：http://mna.yongpay.top

TS:   a && b || !c
来源：http://syq.hnxiangtu.top

Java: a && b || !c
来源：http://bvi.xziqi.cn

Go:   a && b || !c
来源：http://nrv.daria6918.cn

Ruby: a && b || !c
来源：http://fnq.kuanghao11.cn

C#:   a && b || !c
来源：http://scw.jiagoushi.top

[B16] 卫语句：不满足条件提前返回
来源：http://nbt.bbcook.cn

Py:   if not data: return
来源：http://gda.shzxlz.cn

PHP:  if (!$data) { return; }
来源：http://hyw.iojbl.cn

JS:   if (!data) return;
来源：http://sep.haohaochexian.top

TS:   if (!data) return;
来源：http://llf.guowangkeji.top

Java: if (data == null) return;
来源：http://wpj.yj20258888.top

Go:   if data == nil { return }
来源：http://jao.shzxlz.cn

Ruby: return if data.nil?
来源：http://nej.yvedp.cn

C#:   if (data == null) return;
来源：http://rty.birdmap.top

================================================================================
来源：http://xqr.yueranfly.top

C. 函数与作用域
来源：http://xen.yanxiufei.cn

================================================================================
来源：http://wnf.ybcxt.top

[C01] 定义函数
来源：http://tva.zhixingplan.top

Py:   def add(a, b): return a + b
来源：http://akn.mhx1999.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zrr.yonumen.top

JS:   function add(a, b) { return a + b; }
来源：http://ynk.shanyushiyangkeji.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fea.zhoulong.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://xrg.guowangkeji.top

Go:   func add(a, b int) int { return a + b }
来源：http://zut.mhx1999.top

Ruby: def add(a, b); a + b; end
来源：http://wtm.shangyingyoupin.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://fgf.quarkkingdee.top

[C02] 默认参数
来源：http://hhq.hfpthk.cn

Py:   def greet(name="World"): return name
来源：http://bjy.ppjwa.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://hps.nwbrower.top

JS:   function greet(name = "World") { return name; }
来源：http://cjc.xuetiantiany.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://cph.shanyushiyangtech.top

Java: // 无默认参数：方法重载或 Optional
来源：http://tgb.shanyushiyangkeji.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://nqq.tarul.cn

Ruby: def greet(name = "World") = name
来源：http://ixk.yanxiufei.cn

C#:   string Greet(string name = "World") => name;
来源：http://oph.feifeiyinyue.top

[C03] 可变参数
来源：http://iab.zhiwuduotai.top

Py:   def total(*args): return sum(args)
来源：http://ome.hammf.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://nta.zhoulong.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://xxx.hammf.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://aar.yongpay.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://yxn.sxryk.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://vuh.bbcook.cn

Ruby: def total(*nums); nums.sum; end
来源：http://qck.nanxuanxn.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://dwn.ydjk.org.cn

[C04] 命名参数 / 关键字参数
来源：http://alv.smart0.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hla.sweek.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ovp.guannengcc.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://sle.iojbl.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://cjv.c1oappe.top

Java: // 无：用 Builder 模式或 record
来源：http://rhw.jinghuilouyu.cn

Go:   // 无：用配置结构体参数
来源：http://gqw.c1oappe.top

Ruby: f(a: 1, b: 2)
来源：http://vsu.ehwqpu.com

C#:   f(a: 1, b: 2)
来源：http://hca.jiagoushi.top

[C05] 返回多个值
来源：http://nwy.fzhhl.top

Py:   return a, b
来源：http://wih.andypj.xyz

PHP:  return [$a, $b];
来源：http://zey.xinyue.icu

JS:   return [a, b];             // 或 return { a, b };
来源：http://anb.xuanzx.com

TS:   return { a, b };
来源：http://ztu.ivvv.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://gaw.zdbjq.cn

Go:   return a, b
来源：http://sag.jqgufenzy.top

Ruby: return a, b
来源：http://uma.sysykeji.top

C#:   return (a, b);              // ValueTuple
来源：http://coh.yfazqb.com

[C06] 匿名函数 / lambda
来源：http://iwi.yuanzhike.top

Py:   square = lambda x: x * x
来源：http://lqd.yfazqb.com

PHP:  $square = fn($x) => $x * $x;
来源：http://dxs.fengsongda.top

JS:   const square = x => x * x;
来源：http://fab.chenjidiqi.icu

TS:   const square = (x: number): number => x * x;
来源：http://vtt.sxryk.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mku.xziqi.cn

Go:   sq := func(x int) int { return x * x }
来源：http://jaf.cashguo.top

Ruby: square = ->(x) { x * x }
来源：http://pyc.jianghu66.top

C#:   Func<int, int> square = x => x * x;
来源：http://ljy.cashguo.top

[C07] 把函数作为参数传入
来源：http://fhh.xingfuxueyuan.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://txr.shanyushiyangtech.top

PHP:  array_map("strtoupper", $arr);
来源：http://wvl.chenlongwang.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://jpo.c1oappe.top

TS:   arr.map(String)
来源：http://dca.ydzc1.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://nym.vqdsnc.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://evc.tianlin.xyz

Ruby: arr.map(&:upcase)
来源：http://usb.hnqzz.top

C#:   arr.Select(s => s.ToUpper())
来源：http://lxl.jlsjyb.cn

[C08] 闭包
来源：http://taw.feifeiyinyue.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qfv.nanxinkj.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://uub.fzhhl.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://sdu.feifeiyinyue.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://zjx.hammf.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://sra.hcnkem.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://qfl.nwbrower.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://sbl.shanyushiyangkeji.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mrm.svipenyu.cn

[C09] 递归
来源：http://jap.vehdjk.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://gkq.shuidangran.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mtu.tanke756.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xkz.chenlongwang.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ohe.tanke756.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://kme.yongpay.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://lij.c1oappe.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://bof.yfazqb.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://kjw.shangyingyoupin.top

[C10] 变量作用域
来源：http://hwy.yangfankeji.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://jtk.wangdashe.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hzj.yonumen.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://nyw.9152youxi.cn

TS:   同 JS
来源：http://kje.pengpengdd.cyou

Java: 方法内为块级作用域
来源：http://dvk.ppjwa.cn

Go:   花括号块级作用域
来源：http://xqe.daxiang520.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://uni.sysykeji.top

C#:   块级作用域
来源：http://axe.wangshuangyany.cn

[C11] 模块导入与导出
来源：http://efh.guannengcc.top

Py:   from module import func
来源：http://qgt.yuxming.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://tjl.ywan-chungtsiang.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://lhs.ppjwa.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://yfn.hfpthk.cn

Java: import java.util.List;
来源：http://fsq.snrcjt.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mhw.shzxlz.cn

Ruby: require "json"; require_relative "./util"
来源：http://dna.yfazqb.com

C#:   using System.Text;
来源：http://hjr.sweek.top

[C12] 立即执行函数 IIFE
来源：http://wfg.ydjk.org.cn

Py:   (lambda: print("run"))()
来源：http://rcf.yj20258.top

PHP:  (function () { echo "run"; })();
来源：http://lcs.xinyue.icu

JS:   (() => { console.log("run"); })();
来源：http://qlb.jinyuanbaomall.cn

TS:   (() => { console.log("run"); })();
来源：http://fsr.c1oappe.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://zzg.aizwys.cn

Go:   func() { fmt.Println("run") }()
来源：http://dfr.zhengqikj.top

Ruby: -> { puts "run" }.call
来源：http://ovr.hnqzz.top

C#:   // 无 IIFE：用静态构造函数
来源：http://coa.shanyushiyangtech.top

[C13] 类型声明 / 类型注解
来源：http://xop.hnxiangtu.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ouv.ybcxt.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://afc.jianghu66.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://bxt.jinqigfzy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qpq.xuanzx.com

Java: int add(int a, int b) { return a + b; }
来源：http://pqu.haohaochexian.top

Go:   func add(a, b int) int
来源：http://zrq.tianlin.xyz

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://scj.nanxuanxn.top

C#:   int Add(int a, int b) => a + b;
来源：http://opg.yangfankeji.com

[C14] 泛型函数
来源：http://qga.xziqi.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://pas.xuanzx.com

PHP:  // 无泛型
来源：http://zwd.yonumen.top

JS:   // 无泛型
来源：http://gaj.sweek.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://prw.yj20258.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://lth.yuanzhike.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://qwb.sxryk.cn

Ruby: # 无泛型
来源：http://rqv.sweek.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://vnr.ehwqpu.com

[C15] 解构 / 展开参数
来源：http://cyf.jinghuilouyu.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://doi.iojbl.cn

PHP:  [$a, $b] = $pair;
来源：http://vtk.chenjidiqi.icu

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://eqp.zhongyouzk.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ueu.jianghu66.top

Java: // 无解构
来源：http://njw.sufxvd.cn

Go:   // 无解构
来源：http://avp.tanke756.top

Ruby: a, b = pair
来源：http://bty.feifeiyinyue.top

C#:   var (a, b) = pair;
来源：http://atk.chenjidiqi.icu

[C16] 函数 / 方法重载
来源：http://rte.daxiang520.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://llr.pengpengdd.cyou

PHP:  // 无重载
来源：http://mvr.jianghu66.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://fyv.gotoacloud.top

TS:   // 用联合类型或重载签名声明
来源：http://cek.yfazqb.com

Java: void f(int a) {}  void f(String a) {}
来源：http://lbf.cqqwz.cn

Go:   // 无重载：用不同函数名
来源：http://efc.jqgfzy.top

Ruby: # 无重载：靠动态参数
来源：http://doc.nanxuanxn.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://fid.bjfxy.top

================================================================================
来源：http://ajd.shuidangran.top

D. 数组 / 列表 / 集合
来源：http://ech.yongpay.top

================================================================================
来源：http://tad.ppjwa.cn

[D01] 创建数组 / 列表
来源：http://saa.jianghu66.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://tsl.chenlongwang.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ffg.guannengcc.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://nbt.nanxinkj.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://qzi.aizwys.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://xib.iojbl.cn

Go:   arr := []int{1, 2, 3}
来源：http://bge.dianchejie.cn

Ruby: arr = [1, 2, 3]
来源：http://ihd.shuidangran.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://kee.ydzc1.top

[D02] 追加元素到末尾
来源：http://lmy.yangfankeji.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://sdt.redwolf501.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://arv.daxiang520.top

JS:   arr.push(4);
来源：http://gfg.ppjwa.cn

TS:   arr.push(4);
来源：http://piu.zdbjq.cn

Java: list.add(4);
来源：http://kjr.sysykeji.top

Go:   arr = append(arr, 4)
来源：http://ohc.52xcode.cn

Ruby: arr << 4; arr.push(5)
来源：http://qvx.gzhubu.top

C#:   list.Add(4);
来源：http://jzo.zhoulong.xyz

[D03] 在指定位置插入元素
来源：http://dua.hysaishi.cn

Py:   arr.insert(0, 0)
来源：http://ybi.redwolf501.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://zcz.nwbrower.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://xmb.cdnleiting.top

TS:   arr.splice(0, 0, 0);
来源：http://vne.yj20258.top

Java: list.add(0, 0);
来源：http://ueu.sxryk.cn

Go:   arr = append([]int{0}, arr...)
来源：http://bmj.chenlongwang.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://gxd.ydzc1.top

C#:   list.Insert(0, 0);
来源：http://ddr.nwbrower.top

[D04] 删除元素
来源：http://vos.hesvh.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://qcv.zhiwuduotai.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ael.aizwys.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://umz.wangdashe.top

TS:   arr.splice(0, 1);
来源：http://jyv.ehwqpu.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://oxl.zdbjq.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://cky.pycfn.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hwy.zhongyouzk.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ylp.bbcook.cn

[D05] 访问与修改元素
来源：http://tmv.shanyushiyangtech.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://eoq.daria6918.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://piv.nanxuanxn.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://kxy.hnqzz.top

TS:   arr[0]; arr.at(-1);
来源：http://pvu.aibaodan.cn

Java: list.get(0); list.set(0, 9);
来源：http://dpe.nanxuanxn.top

Go:   arr[0]; arr[0] = 9
来源：http://can.cucudq.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://csh.hesvh.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://yvn.yj202588.top

[D06] 数组长度
来源：http://css.nanxuanxn.top

Py:   len(arr)
来源：http://vmv.shzxlz.cn

PHP:  count($arr);
来源：http://txx.sufxvd.cn

JS:   arr.length
来源：http://yza.guowangkeji.top

TS:   arr.length
来源：http://kew.jinqigufen.top

Java: list.size();
来源：http://ufi.nanxuanxn.top

Go:   len(arr)
来源：http://yvm.xuanzx.com

Ruby: arr.length; arr.size
来源：http://wkx.snrcjt.cn

C#:   list.Count;
来源：http://avx.jqgufenzy.top

[D07] 切片 / 取子数组
来源：http://tkh.yj202588.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://gry.chenlongwang.top

PHP:  array_slice($arr, 1, 3);
来源：http://faf.aibaodan.cn

JS:   arr.slice(1, 4);
来源：http://pzm.gotoacloud.top

TS:   arr.slice(1, 4);
来源：http://vlw.jqgfzy.top

Java: list.subList(1, 4);
来源：http://ygo.sweek.top

Go:   arr[1:4]
来源：http://yxu.yvedp.cn

Ruby: arr[1, 3]
来源：http://xra.yj202588.top

C#:   list.GetRange(1, 3);
来源：http://dzv.ydjk.org.cn

[D08] 合并两个数组
来源：http://jlo.aibaodan.cn

Py:   a + b;  a.extend(b)
来源：http://hjr.sysykeji.top

PHP:  array_merge($a, $b);
来源：http://jue.yj20258888.top

JS:   [...a, ...b];  a.concat(b);
来源：http://oqf.fehbvm.com

TS:   [...a, ...b];
来源：http://vvw.gzhubu.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wpn.yfazqb.com

Go:   append(a, b...)
来源：http://jcs.zhijiandao.cn

Ruby: a + b;  a.concat(b)
来源：http://fmb.mhx1999.top

C#:   a.Concat(b).ToList()
来源：http://pvr.zhiwuduotai.top

[D09] 排序（升序）
来源：http://ece.gaohongyu789.top

Py:   sorted(arr);  arr.sort()
来源：http://blf.jianghu66.top

PHP:  sort($arr);
来源：http://dvk.bbcook.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://fxx.mhx1999.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://kwk.zhiwuduotai.top

Java: Collections.sort(list);  list.sort(null);
来源：http://don.yonumen.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://pdj.fanxiaobao.xyz

Ruby: arr.sort
来源：http://nnb.ydjk.org.cn

C#:   list.Sort();
来源：http://pvn.xylfe.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://xuq.yuxming.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://xfk.meibo888.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lco.yvedp.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://dux.shzxlz.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mah.fktsv.cn


<!-- 参考信息 -->