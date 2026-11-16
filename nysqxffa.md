代发 wailian999

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ykd.cqqwz.cn

Ruby: while i < 10; i += 1; end
来源：http://ofr.birdmap.top

C#:   while (i < 10) { i++; }
来源：http://jew.nanxinkj.top

[B08] do-while（至少执行一次）
来源：http://qdx.jqgufenzy.top

Py:   # 无 do-while：用 while True + break
来源：http://hmu.ydjk.org.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://wpq.svipenyu.cn

JS:   do { i++; } while (i < 10);
来源：http://ojm.sysykeji.top

TS:   do { i++; } while (i < 10);
来源：http://gdx.wangdashe.top

Java: do { i++; } while (i < 10);
来源：http://cli.bbcook.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://isf.jqgfzy.top

Ruby: begin; i += 1; end while i < 10
来源：http://zrt.yangfankeji.com

C#:   do { i++; } while (i < 10);
来源：http://nsg.jinqigfzy.top

[B09] break 与 continue
来源：http://yyt.meibo888.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://fhc.dashuyun.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://aze.kuanghao11.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tom.havefunace.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sqy.tian-w.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://iqm.smart0.xyz

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ffo.fzhhl.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://thn.hfpthk.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ayp.zhengqikj.top

[B10] 遍历同时拿索引
来源：http://wul.birdmap.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://xan.jiagoushi.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://cby.pengpengdd.cyou

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wny.bjfxy.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mlv.mhx1999.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://zaa.gotoacloud.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hxb.hnxiangtu.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://tyv.shanyushiyangtech.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wys.uphjek.com

[B11] 生成数字序列 / 区间
来源：http://xtv.jinqigufen.top

Py:   list(range(0, 10, 2))
来源：http://xyd.vqdsnc.cn

PHP:  range(0, 10, 2);
来源：http://jtd.hnxiangtu.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wmy.smart0.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dyo.chenlongwang.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://qsj.shanyushiyangtech.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://kpm.wangdashe.top

Ruby: (0...10).step(2).to_a
来源：http://wtq.hywenlv.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://fpo.ehwqpu.com

[B12] 跳出多层循环
来源：http://uzp.hysaishi.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://kpj.meibo888.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://cfx.redwolf501.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hoh.epnwcf.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://fdo.gaohongyu789.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://spc.hnxiangtu.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://rhx.zhoulong.xyz

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ngx.zdqjudy.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ylm.52xcode.cn

[B13] 判断是否为数字
来源：http://lus.zhiwuduotai.top

Py:   isinstance(x, (int, float))
来源：http://nyx.xinyue.icu

PHP:  is_numeric($x)
来源：http://qfe.xingfuxueyuan.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hef.chenjidiqi.icu

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yfh.xylfe.cn

Java: x instanceof Number
来源：http://eeg.smart0.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ngb.guowangkeji.top

Ruby: x.is_a?(Numeric)
来源：http://lsz.tarul.cn

C#:   x is int or double or decimal
来源：http://hqe.daria6918.cn

[B14] 判断值是否在集合内
来源：http://jxu.xuanzx.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://iko.jyoumei.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://gkg.daxiang520.top

JS:   [1, 2, 3].includes(x)
来源：http://svv.wangshuangyany.cn

TS:   [1, 2, 3].includes(x)
来源：http://qlb.xinyue.icu

Java: List.of(1, 2, 3).contains(x)
来源：http://kje.ppjwa.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mum.jinghuilouyu.cn

Ruby: [1, 2, 3].include?(x)
来源：http://olk.yanxiufei.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://odo.cucudq.cn

[B15] 布尔运算与取反
来源：http://cbi.shanyushiyangtech.top

Py:   a and b or not c
来源：http://jbc.meibo888.top

PHP:  $a && $b || !$c
来源：http://ily.hesvh.cn

JS:   a && b || !c
来源：http://lmt.jqgfzy.top

TS:   a && b || !c
来源：http://mfh.tian-w.cn

Java: a && b || !c
来源：http://csf.zycfv.cn

Go:   a && b || !c
来源：http://jky.bbcook.cn

Ruby: a && b || !c
来源：http://qvh.sufxvd.cn

C#:   a && b || !c
来源：http://gvy.ivvv.top

[B16] 卫语句：不满足条件提前返回
来源：http://njx.wangshuangyany.cn

Py:   if not data: return
来源：http://qij.sufxvd.cn

PHP:  if (!$data) { return; }
来源：http://skm.aizwys.cn

JS:   if (!data) return;
来源：http://plx.nanxuanxn.top

TS:   if (!data) return;
来源：http://jbr.shanyushiyangtech.top

Java: if (data == null) return;
来源：http://nhy.yonumen.top

Go:   if data == nil { return }
来源：http://upf.cheryme.top

Ruby: return if data.nil?
来源：http://qpm.zhongyouzk.top

C#:   if (data == null) return;
来源：http://dym.ppjwa.cn

================================================================================
来源：http://fvd.ydzc1.top

C. 函数与作用域
来源：http://bcm.guannengcc.top

================================================================================
来源：http://rzi.shanyushiyangkeji.top

[C01] 定义函数
来源：http://hlb.yonumen.top

Py:   def add(a, b): return a + b
来源：http://zhb.aizwys.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vpn.chenjidiqi.icu

JS:   function add(a, b) { return a + b; }
来源：http://ybk.sufxvd.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tgq.chenlongwang.top

Java: static int add(int a, int b) { return a + b; }
来源：http://cdv.ydzc1.top

Go:   func add(a, b int) int { return a + b }
来源：http://vgf.chenzaomai.com

Ruby: def add(a, b); a + b; end
来源：http://wlk.yfazqb.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://aiu.fktsv.cn

[C02] 默认参数
来源：http://udp.haohaochexian.top

Py:   def greet(name="World"): return name
来源：http://lph.bjfxy.top

PHP:  function greet($name = "World") { return $name; }
来源：http://lar.yongpay.top

JS:   function greet(name = "World") { return name; }
来源：http://vqt.pengpengdd.cyou

TS:   function greet(name: string = "World") { return name; }
来源：http://lni.daxiang520.top

Java: // 无默认参数：方法重载或 Optional
来源：http://ckq.jiagoushi.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://bpc.wangshuangyany.cn

Ruby: def greet(name = "World") = name
来源：http://olk.zhongyouzk.top

C#:   string Greet(string name = "World") => name;
来源：http://avg.ehwqpu.com

[C03] 可变参数
来源：http://rvk.ppjwa.cn

Py:   def total(*args): return sum(args)
来源：http://mnc.pengpengdd.cyou

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://qyd.zhixingplan.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://rku.fanxiaobao.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://lqs.yj20258888.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hxd.pycfn.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://pyb.shzxlz.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ede.pycfn.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zyy.guowangkeji.top

[C04] 命名参数 / 关键字参数
来源：http://otv.birdmap.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://qgm.jinqigufen.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://jrg.tian-w.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://dxt.yangfankeji.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://krs.gotoacloud.top

Java: // 无：用 Builder 模式或 record
来源：http://bco.ybcxt.top

Go:   // 无：用配置结构体参数
来源：http://xbg.pycfn.com

Ruby: f(a: 1, b: 2)
来源：http://jey.cashguo.top

C#:   f(a: 1, b: 2)
来源：http://rej.guowangkeji.top

[C05] 返回多个值
来源：http://grr.chenjidiqi.icu

Py:   return a, b
来源：http://jih.fktsv.cn

PHP:  return [$a, $b];
来源：http://ira.dashuyun.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://psp.xylfe.cn

TS:   return { a, b };
来源：http://yot.tian-w.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hii.hfpthk.cn

Go:   return a, b
来源：http://axq.shzxlz.cn

Ruby: return a, b
来源：http://mpq.yanxiufei.cn

C#:   return (a, b);              // ValueTuple
来源：http://syy.hnqzz.top

[C06] 匿名函数 / lambda
来源：http://xwu.daxiang520.top

Py:   square = lambda x: x * x
来源：http://jvi.gaohongyu789.top

PHP:  $square = fn($x) => $x * $x;
来源：http://iag.guowangkeji.top

JS:   const square = x => x * x;
来源：http://miq.jlsjyb.cn

TS:   const square = (x: number): number => x * x;
来源：http://wqc.jinyuanbaomall.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://tzw.zhijiandao.cn

Go:   sq := func(x int) int { return x * x }
来源：http://wnu.mhx1999.top

Ruby: square = ->(x) { x * x }
来源：http://nzv.snrcjt.cn

C#:   Func<int, int> square = x => x * x;
来源：http://qip.haohaochexian.top

[C07] 把函数作为参数传入
来源：http://hqv.svipenyu.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://bzj.yj20258888.top

PHP:  array_map("strtoupper", $arr);
来源：http://lbf.yj202588.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mlz.jinqigfzy.top

TS:   arr.map(String)
来源：http://iam.hfpthk.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://oht.jiagoushi.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://auz.kuanghao11.cn

Ruby: arr.map(&:upcase)
来源：http://rwi.ybcxt.top

C#:   arr.Select(s => s.ToUpper())
来源：http://yih.ybcxt.top

[C08] 闭包
来源：http://nuo.shuidangran.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wqc.zhoulong.xyz

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://rhv.fktsv.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ivg.cdnleiting.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://sam.shuidangran.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ihx.jlsjyb.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mpz.quarkkingdee.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mwg.xziqi.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://gke.shzxlz.cn

[C09] 递归
来源：http://dsy.vehdjk.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ikp.shanyushiyangkeji.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://irh.tanke756.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bem.yueranfly.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bgc.smart0.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://bvq.redwolf501.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ypj.yongpay.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wgu.jqgufenzy.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://eiq.jyoumei.cn

[C10] 变量作用域
来源：http://wcl.daria6918.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://fja.dashuyun.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ozi.pengpengdd.cyou

JS:   let/const 块级作用域，var 函数级作用域
来源：http://sbh.yfazqb.com

TS:   同 JS
来源：http://jlw.shuidangran.top

Java: 方法内为块级作用域
来源：http://pvu.ctjpmb.com

Go:   花括号块级作用域
来源：http://tak.ybcxt.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://nhw.xuetiantiany.cn

C#:   块级作用域
来源：http://fbp.cucudq.cn

[C11] 模块导入与导出
来源：http://czt.bbcook.cn

Py:   from module import func
来源：http://nik.hongshengwenyu.top

PHP:  require "file.php";  或 use App\Service;
来源：http://qkj.zhiwuduotai.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://mtm.guowangkeji.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mzt.jinqigfzy.top

Java: import java.util.List;
来源：http://biv.yanxiufei.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ybm.xinyue.icu

Ruby: require "json"; require_relative "./util"
来源：http://hkg.yvedp.cn

C#:   using System.Text;
来源：http://mxo.ppjwa.cn

[C12] 立即执行函数 IIFE
来源：http://goc.316326.xyz

Py:   (lambda: print("run"))()
来源：http://rjh.gogol.net.cn

PHP:  (function () { echo "run"; })();
来源：http://xfv.zhoulong.xyz

JS:   (() => { console.log("run"); })();
来源：http://atk.pengpengdd.cyou

TS:   (() => { console.log("run"); })();
来源：http://hhs.dianchejie.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jtu.hnqzz.top

Go:   func() { fmt.Println("run") }()
来源：http://lun.9152youxi.cn

Ruby: -> { puts "run" }.call
来源：http://uzp.shanyushiyangtech.top

C#:   // 无 IIFE：用静态构造函数
来源：http://fqn.9152youxi.cn

[C13] 类型声明 / 类型注解
来源：http://ktz.sweek.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://slq.feifeiyinyue.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vvw.gogol.net.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://diq.shanyushiyangtech.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vef.vehdjk.com

Java: int add(int a, int b) { return a + b; }
来源：http://pmb.quarkkingdee.top

Go:   func add(a, b int) int
来源：http://bmi.zdqjudy.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://cnt.gzhubu.top

C#:   int Add(int a, int b) => a + b;
来源：http://lfo.tanke756.top

[C14] 泛型函数
来源：http://eev.zhongyouzk.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://huw.fehbvm.com

PHP:  // 无泛型
来源：http://wwx.gzhubu.top

JS:   // 无泛型
来源：http://pgu.yuxming.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ebn.gotoacloud.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wch.sweek.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://eez.zhixingplan.top

Ruby: # 无泛型
来源：http://ezu.xinyue.icu

C#:   static T First<T>(List<T> items) => items[0];
来源：http://dxv.feifeiyinyue.top

[C15] 解构 / 展开参数
来源：http://fuy.sjlbkw.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://lrk.yongpay.top

PHP:  [$a, $b] = $pair;
来源：http://fjc.52xcode.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://lyh.aizwys.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mpg.hcnkem.com

Java: // 无解构
来源：http://prx.fehbvm.com

Go:   // 无解构
来源：http://nbk.sweek.top

Ruby: a, b = pair
来源：http://uml.chenzaomai.com

C#:   var (a, b) = pair;
来源：http://elo.jinqigufen.top

[C16] 函数 / 方法重载
来源：http://ios.xylfe.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://qvm.hywenlv.cn

PHP:  // 无重载
来源：http://zbw.zdbjq.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ggq.zhongyouzk.top

TS:   // 用联合类型或重载签名声明
来源：http://uhn.gogol.net.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://nws.bjfxy.top

Go:   // 无重载：用不同函数名
来源：http://mee.pycfn.com

Ruby: # 无重载：靠动态参数
来源：http://qtc.meibo888.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://nun.meibo888.top

================================================================================
来源：http://aja.yueranfly.top

D. 数组 / 列表 / 集合
来源：http://dqx.ehwqpu.com

================================================================================
来源：http://fuw.zhengqikj.top

[D01] 创建数组 / 列表
来源：http://ajd.yvedp.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://wni.zhaomingkeji.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ldx.havefunace.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://igk.chenjidiqi.icu

TS:   const arr: number[] = [1, 2, 3];
来源：http://ooy.dianchejie.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ros.guowangkeji.top

Go:   arr := []int{1, 2, 3}
来源：http://jam.guannengcc.top

Ruby: arr = [1, 2, 3]
来源：http://zlf.vqdsnc.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://vmg.tianlin.xyz

[D02] 追加元素到末尾
来源：http://kir.yvedp.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://dng.hammf.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://onf.tarul.cn

JS:   arr.push(4);
来源：http://qbt.yuxming.cn

TS:   arr.push(4);
来源：http://ljg.nanxuanxn.top

Java: list.add(4);
来源：http://zbk.yvedp.cn

Go:   arr = append(arr, 4)
来源：http://mcd.mhx1999.top

Ruby: arr << 4; arr.push(5)
来源：http://eei.jiagoushi.top

C#:   list.Add(4);
来源：http://bpy.andypj.xyz

[D03] 在指定位置插入元素
来源：http://rgj.shanyushiyangkeji.top

Py:   arr.insert(0, 0)
来源：http://voq.fanxiaobao.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://iox.52xcode.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mvv.yueranfly.top

TS:   arr.splice(0, 0, 0);
来源：http://czp.nanxinkj.top

Java: list.add(0, 0);
来源：http://rxi.yanxiufei.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ppb.cucudq.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ofh.hesvh.cn

C#:   list.Insert(0, 0);
来源：http://ixi.chenlongwang.top

[D04] 删除元素
来源：http://txh.zhongyouzk.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mby.xuanzx.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://raj.haohaochexian.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://oln.sweek.top

TS:   arr.splice(0, 1);
来源：http://pqe.hesvh.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://rbe.zdbjq.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://pil.bjfxy.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://bma.epnwcf.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://zms.0kj1m.cn

[D05] 访问与修改元素
来源：http://vzk.yj202588.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://xip.hywenlv.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://jqr.chenjidiqi.icu

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://pfj.yj20258888.top

TS:   arr[0]; arr.at(-1);
来源：http://asx.aibaodan.cn

Java: list.get(0); list.set(0, 9);
来源：http://rao.0kj1m.cn

Go:   arr[0]; arr[0] = 9
来源：http://qsd.andypj.xyz

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://znn.pycfn.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://sch.hysaishi.cn

[D06] 数组长度
来源：http://lit.nanxinkj.top

Py:   len(arr)
来源：http://vfq.nwbrower.top

PHP:  count($arr);
来源：http://fvd.hywenlv.cn

JS:   arr.length
来源：http://abx.chenjidiqi.icu

TS:   arr.length
来源：http://vmg.zhengqikj.top

Java: list.size();
来源：http://dbg.chenlongwang.top

Go:   len(arr)
来源：http://tzu.tanke756.top

Ruby: arr.length; arr.size
来源：http://tms.zhaomingkeji.xyz

C#:   list.Count;
来源：http://evm.xylfe.cn

[D07] 切片 / 取子数组
来源：http://zee.svipenyu.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wen.xuanzx.com

PHP:  array_slice($arr, 1, 3);
来源：http://ntd.gogol.net.cn

JS:   arr.slice(1, 4);
来源：http://wrm.52xcode.cn

TS:   arr.slice(1, 4);
来源：http://gsy.wangshuangyany.cn

Java: list.subList(1, 4);
来源：http://ofs.yanxiufei.cn

Go:   arr[1:4]
来源：http://thw.sjlbkw.cn

Ruby: arr[1, 3]
来源：http://lnx.andypj.xyz

C#:   list.GetRange(1, 3);
来源：http://xyl.vehdjk.com

[D08] 合并两个数组
来源：http://reo.yanxiufei.cn

Py:   a + b;  a.extend(b)
来源：http://asn.yj202588.top

PHP:  array_merge($a, $b);
来源：http://ufm.sxryk.cn


<!-- 参考信息 -->