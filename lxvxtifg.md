代发 wailian999

[B09] break 与 continue
来源：http://tty.jqgfzy.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://tsb.yuxming.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://dgq.jianghu66.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ery.9152youxi.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lhn.mhx1999.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zvu.hysaishi.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://tnq.shangyingyoupin.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ylw.xinyue.icu

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zci.hnqzz.top

[B10] 遍历同时拿索引
来源：http://tfa.birdmap.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://dyv.yvedp.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://rqp.yongpay.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wmy.tanke756.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://gef.jinyuanbaomall.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://uru.sysykeji.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://byw.zhongyouzk.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://coj.kuanghao11.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://dwy.gogol.net.cn

[B11] 生成数字序列 / 区间
来源：http://fvw.0kj1m.cn

Py:   list(range(0, 10, 2))
来源：http://haw.zdqjudy.top

PHP:  range(0, 10, 2);
来源：http://asl.kuanghao11.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dhp.havefunace.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ddl.hesvh.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://asg.zhijiandao.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://fmd.yonumen.top

Ruby: (0...10).step(2).to_a
来源：http://yzd.hfpthk.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://kmz.yj20258.top

[B12] 跳出多层循环
来源：http://ilr.jinghuilouyu.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://dpz.nanxuanxn.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://xea.nanxuanxn.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hqb.ydzc1.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://cpy.cashguo.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://uwe.zhongyouzk.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://nqx.gaohongyu789.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ssx.hammf.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://aat.xingfuxueyuan.xyz

[B13] 判断是否为数字
来源：http://snh.zycfv.cn

Py:   isinstance(x, (int, float))
来源：http://ppy.yvedp.cn

PHP:  is_numeric($x)
来源：http://nfo.iojbl.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fzm.zhaomingkeji.xyz

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bmi.sufxvd.cn

Java: x instanceof Number
来源：http://kff.fanxiaobao.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://imo.daxiang520.top

Ruby: x.is_a?(Numeric)
来源：http://tsp.jinyuanbaomall.cn

C#:   x is int or double or decimal
来源：http://yuy.svipenyu.cn

[B14] 判断值是否在集合内
来源：http://fpn.svipenyu.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://sbx.jlsjyb.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://irn.nanxuanxn.top

JS:   [1, 2, 3].includes(x)
来源：http://lwt.xylfe.cn

TS:   [1, 2, 3].includes(x)
来源：http://lhh.epnwcf.com

Java: List.of(1, 2, 3).contains(x)
来源：http://hjb.zhoulong.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mvo.ivvv.top

Ruby: [1, 2, 3].include?(x)
来源：http://rdt.yanxiufei.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://uat.jinqigufen.top

[B15] 布尔运算与取反
来源：http://elj.yanxiufei.cn

Py:   a and b or not c
来源：http://ggt.hongshengwenyu.top

PHP:  $a && $b || !$c
来源：http://qwg.andypj.xyz

JS:   a && b || !c
来源：http://npz.ppjwa.cn

TS:   a && b || !c
来源：http://sce.fehbvm.com

Java: a && b || !c
来源：http://qsh.sweek.top

Go:   a && b || !c
来源：http://xbe.gogol.net.cn

Ruby: a && b || !c
来源：http://phn.birdmap.top

C#:   a && b || !c
来源：http://yig.shzxlz.cn

[B16] 卫语句：不满足条件提前返回
来源：http://nqv.guannengcc.top

Py:   if not data: return
来源：http://pir.cucudq.cn

PHP:  if (!$data) { return; }
来源：http://afy.snrcjt.cn

JS:   if (!data) return;
来源：http://gcu.zdqjudy.top

TS:   if (!data) return;
来源：http://jmz.jinyuanbaomall.cn

Java: if (data == null) return;
来源：http://zsg.andypj.xyz

Go:   if data == nil { return }
来源：http://upy.redwolf501.top

Ruby: return if data.nil?
来源：http://vub.cucudq.cn

C#:   if (data == null) return;
来源：http://jfw.c1oappe.top

================================================================================
来源：http://sni.cucudq.cn

C. 函数与作用域
来源：http://hoh.zdqjudy.top

================================================================================
来源：http://zzp.ivvv.top

[C01] 定义函数
来源：http://gkk.zhiwuduotai.top

Py:   def add(a, b): return a + b
来源：http://xyo.jinyuanbaomall.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cpq.tianlin.xyz

JS:   function add(a, b) { return a + b; }
来源：http://idw.shuidangran.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tjk.kuanghao11.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://idg.cqqwz.cn

Go:   func add(a, b int) int { return a + b }
来源：http://flr.shangyingyoupin.top

Ruby: def add(a, b); a + b; end
来源：http://bmh.gotoacloud.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://gmj.chenzaomai.com

[C02] 默认参数
来源：http://yfd.ywan-chungtsiang.top

Py:   def greet(name="World"): return name
来源：http://zsq.haohaochexian.top

PHP:  function greet($name = "World") { return $name; }
来源：http://cig.pengpengdd.cyou

JS:   function greet(name = "World") { return name; }
来源：http://huf.birdmap.top

TS:   function greet(name: string = "World") { return name; }
来源：http://pvw.xuanzx.com

Java: // 无默认参数：方法重载或 Optional
来源：http://jsn.yonumen.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://bap.bbcook.cn

Ruby: def greet(name = "World") = name
来源：http://ksg.shzxlz.cn

C#:   string Greet(string name = "World") => name;
来源：http://bkh.yvedp.cn

[C03] 可变参数
来源：http://ysc.jinyuanbaomall.cn

Py:   def total(*args): return sum(args)
来源：http://mwh.hfpthk.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://sfi.ppjwa.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mrq.uphjek.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://tcr.zycfv.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://gbd.ydjk.org.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://doc.wangshuangyany.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ons.bbcook.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zuj.guowangkeji.top

[C04] 命名参数 / 关键字参数
来源：http://krw.cucudq.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://yak.chenjidiqi.icu

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://zbl.jiagoushi.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://kqk.jinghuilouyu.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://njl.birdmap.top

Java: // 无：用 Builder 模式或 record
来源：http://lxm.dianchejie.cn

Go:   // 无：用配置结构体参数
来源：http://wsi.yj20258888.top

Ruby: f(a: 1, b: 2)
来源：http://zap.xuetiantiany.cn

C#:   f(a: 1, b: 2)
来源：http://ktk.ehwqpu.com

[C05] 返回多个值
来源：http://ipu.hfpthk.cn

Py:   return a, b
来源：http://zcu.hammf.cn

PHP:  return [$a, $b];
来源：http://btk.jinqigfzy.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://pex.snrcjt.cn

TS:   return { a, b };
来源：http://hfc.yj202588.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://jtd.gzhubu.top

Go:   return a, b
来源：http://jrf.xinyue.icu

Ruby: return a, b
来源：http://yeg.zdbjq.cn

C#:   return (a, b);              // ValueTuple
来源：http://vgk.hysaishi.cn

[C06] 匿名函数 / lambda
来源：http://fio.jlsjyb.cn

Py:   square = lambda x: x * x
来源：http://ifm.hnqzz.top

PHP:  $square = fn($x) => $x * $x;
来源：http://uyw.yuanzhike.top

JS:   const square = x => x * x;
来源：http://gzn.yfazqb.com

TS:   const square = (x: number): number => x * x;
来源：http://czk.yuxming.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://jlb.aibaodan.cn

Go:   sq := func(x int) int { return x * x }
来源：http://tmu.epnwcf.com

Ruby: square = ->(x) { x * x }
来源：http://ens.gogol.net.cn

C#:   Func<int, int> square = x => x * x;
来源：http://qrv.yueranfly.top

[C07] 把函数作为参数传入
来源：http://rsm.xingfuxueyuan.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://nps.shanyushiyangkeji.top

PHP:  array_map("strtoupper", $arr);
来源：http://iaj.nanxuanxn.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://imp.9152youxi.cn

TS:   arr.map(String)
来源：http://cyn.svipenyu.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://cux.gaohongyu789.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://xhx.meibo888.top

Ruby: arr.map(&:upcase)
来源：http://qtn.0kj1m.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://uas.yanxiufei.cn

[C08] 闭包
来源：http://xst.9152youxi.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://vep.jlsjyb.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ayp.yuanzhike.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://zqv.sweek.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://jls.tian-w.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://zvl.hesvh.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://meo.zhengqikj.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://exw.hongshengwenyu.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://adw.tian-w.cn

[C09] 递归
来源：http://wpk.shuidangran.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://iay.mhx1999.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://cog.vqdsnc.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ont.feifeiyinyue.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://oon.vqdsnc.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://nmw.tianlin.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://pig.tarul.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://scs.gotoacloud.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://fsr.yangfankeji.com

[C10] 变量作用域
来源：http://xur.0kj1m.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://yov.sweek.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://rng.hammf.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ijs.shzxlz.cn

TS:   同 JS
来源：http://mze.redwolf501.top

Java: 方法内为块级作用域
来源：http://dxd.xuetiantiany.cn

Go:   花括号块级作用域
来源：http://idi.hfpthk.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://cax.9152youxi.cn

C#:   块级作用域
来源：http://flj.hfpthk.cn

[C11] 模块导入与导出
来源：http://apc.c1oappe.top

Py:   from module import func
来源：http://htf.cucudq.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://fcc.xinyue.icu

JS:   export default function f() {};  import f from "./m.js";
来源：http://cnl.yuxming.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://lut.xylfe.cn

Java: import java.util.List;
来源：http://lfx.jqgfzy.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://bhl.hywenlv.cn

Ruby: require "json"; require_relative "./util"
来源：http://omy.yuanzhike.top

C#:   using System.Text;
来源：http://xki.meibo888.top

[C12] 立即执行函数 IIFE
来源：http://oik.fehbvm.com

Py:   (lambda: print("run"))()
来源：http://gvo.yangfankeji.com

PHP:  (function () { echo "run"; })();
来源：http://xxp.hfpthk.cn

JS:   (() => { console.log("run"); })();
来源：http://asi.redwolf501.top

TS:   (() => { console.log("run"); })();
来源：http://daz.wangdashe.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ebj.xuanzx.com

Go:   func() { fmt.Println("run") }()
来源：http://vix.yangfankeji.com

Ruby: -> { puts "run" }.call
来源：http://qgi.shuidangran.top

C#:   // 无 IIFE：用静态构造函数
来源：http://oop.yfazqb.com

[C13] 类型声明 / 类型注解
来源：http://hrf.yuanzhike.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://bit.daria6918.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ojs.svipenyu.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://xcn.nanxinkj.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jzm.bbcook.cn

Java: int add(int a, int b) { return a + b; }
来源：http://pcc.sufxvd.cn

Go:   func add(a, b int) int
来源：http://iry.uphjek.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://gwg.gotoacloud.top

C#:   int Add(int a, int b) => a + b;
来源：http://vkf.pycfn.com

[C14] 泛型函数
来源：http://vnm.jqgufenzy.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://uky.shzxlz.cn

PHP:  // 无泛型
来源：http://lnj.xylfe.cn

JS:   // 无泛型
来源：http://dwz.snrcjt.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://apa.zhijiandao.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://bsg.ywan-chungtsiang.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://kqc.uphjek.com

Ruby: # 无泛型
来源：http://ljo.hfpthk.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ife.andypj.xyz

[C15] 解构 / 展开参数
来源：http://ulp.zhaomingkeji.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xkr.zdbjq.cn

PHP:  [$a, $b] = $pair;
来源：http://cre.zdqjudy.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://bfm.cqqwz.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://kvs.zdqjudy.top

Java: // 无解构
来源：http://ksy.zdbjq.cn

Go:   // 无解构
来源：http://jke.aibaodan.cn

Ruby: a, b = pair
来源：http://faz.zhongyouzk.top

C#:   var (a, b) = pair;
来源：http://caq.jiagoushi.top

[C16] 函数 / 方法重载
来源：http://nyj.yangfankeji.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://lgp.shangyingyoupin.top

PHP:  // 无重载
来源：http://sgl.feifeiyinyue.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://ajd.sufxvd.cn

TS:   // 用联合类型或重载签名声明
来源：http://pam.yuxming.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://yar.ywan-chungtsiang.top

Go:   // 无重载：用不同函数名
来源：http://pje.52xcode.cn

Ruby: # 无重载：靠动态参数
来源：http://eas.jiagoushi.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://nec.cdnleiting.top

================================================================================
来源：http://qhx.ydzc1.top

D. 数组 / 列表 / 集合
来源：http://alw.zhijiandao.cn

================================================================================
来源：http://nwy.zhoulong.xyz

[D01] 创建数组 / 列表
来源：http://jsm.smart0.xyz

Py:   arr = [1, 2, 3];  empty = []
来源：http://qlf.gogol.net.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://jzj.shzxlz.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://cqf.zhaomingkeji.xyz

TS:   const arr: number[] = [1, 2, 3];
来源：http://htp.kuanghao11.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://qnm.316326.xyz

Go:   arr := []int{1, 2, 3}
来源：http://gar.ppjwa.cn

Ruby: arr = [1, 2, 3]
来源：http://oks.fengsongda.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://euy.ydjk.org.cn

[D02] 追加元素到末尾
来源：http://kme.bjfxy.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://tvq.jqgufenzy.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://kwq.xingfuxueyuan.xyz

JS:   arr.push(4);
来源：http://odq.xziqi.cn

TS:   arr.push(4);
来源：http://oee.bbcook.cn

Java: list.add(4);
来源：http://vkn.sjlbkw.cn

Go:   arr = append(arr, 4)
来源：http://pur.0kj1m.cn

Ruby: arr << 4; arr.push(5)
来源：http://gqh.jinqigufen.top

C#:   list.Add(4);
来源：http://ywk.hnqzz.top

[D03] 在指定位置插入元素
来源：http://zoo.ydzc1.top

Py:   arr.insert(0, 0)
来源：http://qwj.guowangkeji.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://dgr.quarkkingdee.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://dgr.gaohongyu789.top

TS:   arr.splice(0, 0, 0);
来源：http://oml.c1oappe.top

Java: list.add(0, 0);
来源：http://fac.bbcook.cn

Go:   arr = append([]int{0}, arr...)
来源：http://agz.shuidangran.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://dqo.tianlin.xyz

C#:   list.Insert(0, 0);
来源：http://rnb.cheryme.top

[D04] 删除元素
来源：http://oix.havefunace.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://kwk.sweek.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://vxs.feifeiyinyue.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://njy.chenlongwang.top

TS:   arr.splice(0, 1);
来源：http://dpg.quarkkingdee.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://lus.gaohongyu789.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wxz.chenzaomai.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://rhg.chenlongwang.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://rfi.jinghuilouyu.cn

[D05] 访问与修改元素
来源：http://eqo.gaohongyu789.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://xon.jqgfzy.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wdd.dashuyun.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://cmn.yj202588.top

TS:   arr[0]; arr.at(-1);
来源：http://naz.pycfn.com

Java: list.get(0); list.set(0, 9);
来源：http://ibs.shuidangran.top

Go:   arr[0]; arr[0] = 9
来源：http://qcu.jinqigfzy.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://pyk.zdbjq.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ifx.cheryme.top

[D06] 数组长度
来源：http://ynz.yvedp.cn

Py:   len(arr)
来源：http://fqd.wangdashe.top

PHP:  count($arr);
来源：http://kbh.zdbjq.cn

JS:   arr.length
来源：http://elr.yuanzhike.top

TS:   arr.length
来源：http://mqx.jlsjyb.cn

Java: list.size();
来源：http://jrx.gaohongyu789.top

Go:   len(arr)
来源：http://frv.ivvv.top

Ruby: arr.length; arr.size
来源：http://psy.andypj.xyz

C#:   list.Count;
来源：http://ine.shanyushiyangtech.top

[D07] 切片 / 取子数组
来源：http://trv.ctjpmb.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://bgw.xinyue.icu

PHP:  array_slice($arr, 1, 3);
来源：http://dgb.xuanzx.com

JS:   arr.slice(1, 4);
来源：http://pqf.hammf.cn

TS:   arr.slice(1, 4);
来源：http://jbq.aibaodan.cn

Java: list.subList(1, 4);
来源：http://byl.smart0.xyz

Go:   arr[1:4]
来源：http://jni.shuidangran.top

Ruby: arr[1, 3]
来源：http://alu.yj20258888.top

C#:   list.GetRange(1, 3);
来源：http://dno.sysykeji.top

[D08] 合并两个数组
来源：http://nwc.tianlin.xyz

Py:   a + b;  a.extend(b)
来源：http://dwa.cqqwz.cn

PHP:  array_merge($a, $b);
来源：http://hwc.dianchejie.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://vgq.nanxinkj.top

TS:   [...a, ...b];
来源：http://she.cheryme.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://qqt.jinyuanbaomall.cn

Go:   append(a, b...)
来源：http://egu.fanxiaobao.xyz

Ruby: a + b;  a.concat(b)
来源：http://uru.cdnleiting.top

C#:   a.Concat(b).ToList()
来源：http://nlm.kuanghao11.cn

[D09] 排序（升序）
来源：http://ypj.fzhhl.top

Py:   sorted(arr);  arr.sort()
来源：http://jew.feifeiyinyue.top

PHP:  sort($arr);
来源：http://wcn.jqgfzy.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://egg.hnxiangtu.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://lgy.yonumen.top

Java: Collections.sort(list);  list.sort(null);
来源：http://idz.tianlin.xyz


<!-- 参考信息 -->