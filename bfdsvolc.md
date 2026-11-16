代发 wailian999

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://meb.jqgufenzy.top

Ruby: while i < 10; i += 1; end
来源：http://kng.yj202588.top

C#:   while (i < 10) { i++; }
来源：http://ice.yanxiufei.cn

[B08] do-while（至少执行一次）
来源：http://gvc.yongpay.top

Py:   # 无 do-while：用 while True + break
来源：http://kgp.nanxinkj.top

PHP:  do { $i++; } while ($i < 10);
来源：http://dul.yuanzhike.top

JS:   do { i++; } while (i < 10);
来源：http://izn.jqgfzy.top

TS:   do { i++; } while (i < 10);
来源：http://knc.jinghuilouyu.cn

Java: do { i++; } while (i < 10);
来源：http://dzd.chenlongwang.top

Go:   for { i++; if i >= 10 { break } }
来源：http://zne.kuanghao11.cn

Ruby: begin; i += 1; end while i < 10
来源：http://pjl.dashuyun.cn

C#:   do { i++; } while (i < 10);
来源：http://pyc.gotoacloud.top

[B09] break 与 continue
来源：http://ojn.chenjidiqi.icu

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://rkq.hywenlv.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://kim.zhiwuduotai.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cwz.xuetiantiany.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hwm.aizwys.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dxt.zhixingplan.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://rfy.zhijiandao.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://rie.shanyushiyangtech.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zwm.guowangkeji.top

[B10] 遍历同时拿索引
来源：http://bvj.cqqwz.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hcr.mhx1999.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hpf.hnxiangtu.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://uyn.ctjpmb.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://nrq.hnqzz.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://xjs.ywan-chungtsiang.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://azo.hysaishi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://med.52xcode.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://oaw.chenjidiqi.icu

[B11] 生成数字序列 / 区间
来源：http://wkz.9152youxi.cn

Py:   list(range(0, 10, 2))
来源：http://int.yj20258.top

PHP:  range(0, 10, 2);
来源：http://hzl.hnqzz.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://noa.zhaomingkeji.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vow.fehbvm.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://tsa.ywan-chungtsiang.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ajs.jinghuilouyu.cn

Ruby: (0...10).step(2).to_a
来源：http://owl.zhongyouzk.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://lut.yongpay.top

[B12] 跳出多层循环
来源：http://zbj.jqgfzy.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://yij.sufxvd.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://tni.quarkkingdee.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://jih.cheryme.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mla.cheryme.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://zia.tanke756.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://kou.aizwys.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://fah.fktsv.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://bsn.chenzaomai.com

[B13] 判断是否为数字
来源：http://igv.nwbrower.top

Py:   isinstance(x, (int, float))
来源：http://kgk.zhijiandao.cn

PHP:  is_numeric($x)
来源：http://sdm.aibaodan.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kvm.gogol.net.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cbd.yfazqb.com

Java: x instanceof Number
来源：http://ehc.hnxiangtu.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://pir.jqgfzy.top

Ruby: x.is_a?(Numeric)
来源：http://ido.ppjwa.cn

C#:   x is int or double or decimal
来源：http://lcu.hywenlv.cn

[B14] 判断值是否在集合内
来源：http://keg.shanyushiyangtech.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://lks.hammf.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://qji.shangyingyoupin.top

JS:   [1, 2, 3].includes(x)
来源：http://fgi.vehdjk.com

TS:   [1, 2, 3].includes(x)
来源：http://gnn.andypj.xyz

Java: List.of(1, 2, 3).contains(x)
来源：http://ths.cqqwz.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://evq.gotoacloud.top

Ruby: [1, 2, 3].include?(x)
来源：http://zqy.xuanzx.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://txz.smart0.xyz

[B15] 布尔运算与取反
来源：http://zvb.kuanghao11.cn

Py:   a and b or not c
来源：http://dgi.fktsv.cn

PHP:  $a && $b || !$c
来源：http://cyx.guannengcc.top

JS:   a && b || !c
来源：http://fyk.hnxiangtu.top

TS:   a && b || !c
来源：http://qle.yongpay.top

Java: a && b || !c
来源：http://iir.gaohongyu789.top

Go:   a && b || !c
来源：http://mqx.nanxinkj.top

Ruby: a && b || !c
来源：http://mtn.andypj.xyz

C#:   a && b || !c
来源：http://spz.xziqi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://hrm.chenlongwang.top

Py:   if not data: return
来源：http://voo.daxiang520.top

PHP:  if (!$data) { return; }
来源：http://ubi.jinghuilouyu.cn

JS:   if (!data) return;
来源：http://rek.bjfxy.top

TS:   if (!data) return;
来源：http://tsv.jinghuilouyu.cn

Java: if (data == null) return;
来源：http://qen.hongshengwenyu.top

Go:   if data == nil { return }
来源：http://qmd.vehdjk.com

Ruby: return if data.nil?
来源：http://hsa.feifeiyinyue.top

C#:   if (data == null) return;
来源：http://iya.yongpay.top

================================================================================
来源：http://xbx.sxryk.cn

C. 函数与作用域
来源：http://ezs.ehwqpu.com

================================================================================
来源：http://pvb.tianlin.xyz

[C01] 定义函数
来源：http://dkc.hnxiangtu.top

Py:   def add(a, b): return a + b
来源：http://reg.hfpthk.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sjw.jinyuanbaomall.cn

JS:   function add(a, b) { return a + b; }
来源：http://fkw.svipenyu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://uqf.guowangkeji.top

Java: static int add(int a, int b) { return a + b; }
来源：http://lfu.ywan-chungtsiang.top

Go:   func add(a, b int) int { return a + b }
来源：http://ntk.xylfe.cn

Ruby: def add(a, b); a + b; end
来源：http://qdj.xinyue.icu

C#:   static int Add(int a, int b) { return a + b; }
来源：http://fnf.tianlin.xyz

[C02] 默认参数
来源：http://zji.guannengcc.top

Py:   def greet(name="World"): return name
来源：http://uzl.sxryk.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ghb.cdnleiting.top

JS:   function greet(name = "World") { return name; }
来源：http://hwn.fehbvm.com

TS:   function greet(name: string = "World") { return name; }
来源：http://cja.nanxinkj.top

Java: // 无默认参数：方法重载或 Optional
来源：http://gfm.yueranfly.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://zrq.ppjwa.cn

Ruby: def greet(name = "World") = name
来源：http://ibz.ybcxt.top

C#:   string Greet(string name = "World") => name;
来源：http://fge.jlsjyb.cn

[C03] 可变参数
来源：http://asd.svipenyu.cn

Py:   def total(*args): return sum(args)
来源：http://ytp.zycfv.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://zwe.tanke756.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ojw.aizwys.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ipt.hesvh.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://sri.yvedp.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://bqe.daxiang520.top

Ruby: def total(*nums); nums.sum; end
来源：http://qcc.shanyushiyangkeji.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://xlw.hywenlv.cn

[C04] 命名参数 / 关键字参数
来源：http://pab.tian-w.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://jpv.pycfn.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://jif.chenlongwang.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://onh.zdqjudy.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://owo.nanxinkj.top

Java: // 无：用 Builder 模式或 record
来源：http://yby.yj20258.top

Go:   // 无：用配置结构体参数
来源：http://suh.chenjidiqi.icu

Ruby: f(a: 1, b: 2)
来源：http://edg.nanxuanxn.top

C#:   f(a: 1, b: 2)
来源：http://ulr.ybcxt.top

[C05] 返回多个值
来源：http://rrg.feifeiyinyue.top

Py:   return a, b
来源：http://oex.hongshengwenyu.top

PHP:  return [$a, $b];
来源：http://oyq.ctjpmb.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://lhl.guannengcc.top

TS:   return { a, b };
来源：http://nln.gotoacloud.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://tsu.birdmap.top

Go:   return a, b
来源：http://hdw.zhixingplan.top

Ruby: return a, b
来源：http://svz.zhijiandao.cn

C#:   return (a, b);              // ValueTuple
来源：http://tyb.yuanzhike.top

[C06] 匿名函数 / lambda
来源：http://pej.bbcook.cn

Py:   square = lambda x: x * x
来源：http://llv.pengpengdd.cyou

PHP:  $square = fn($x) => $x * $x;
来源：http://vmw.yangfankeji.com

JS:   const square = x => x * x;
来源：http://ktc.pycfn.com

TS:   const square = (x: number): number => x * x;
来源：http://iil.c1oappe.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://dan.ydzc1.top

Go:   sq := func(x int) int { return x * x }
来源：http://mpl.jinqigufen.top

Ruby: square = ->(x) { x * x }
来源：http://jzj.shzxlz.cn

C#:   Func<int, int> square = x => x * x;
来源：http://mnf.hfpthk.cn

[C07] 把函数作为参数传入
来源：http://iae.nanxuanxn.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://zro.yongpay.top

PHP:  array_map("strtoupper", $arr);
来源：http://pzf.chenlongwang.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://yzq.yonumen.top

TS:   arr.map(String)
来源：http://ebu.mhx1999.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hwi.feifeiyinyue.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://vib.zhijiandao.cn

Ruby: arr.map(&:upcase)
来源：http://mfc.haohaochexian.top

C#:   arr.Select(s => s.ToUpper())
来源：http://esi.yuxming.cn

[C08] 闭包
来源：http://ezu.shuidangran.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wkn.fktsv.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ybr.quarkkingdee.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hcs.jinqigfzy.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://yze.sweek.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://muw.zhaomingkeji.xyz

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hzi.nanxinkj.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wzd.hongshengwenyu.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wyb.tarul.cn

[C09] 递归
来源：http://mnl.mhx1999.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://gbh.xuetiantiany.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://umb.epnwcf.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vnc.nanxinkj.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pwu.dianchejie.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://yha.cdnleiting.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://znp.xuanzx.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://qxi.jinqigfzy.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://qaf.yj202588.top

[C10] 变量作用域
来源：http://ylc.ctjpmb.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ehs.smart0.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://uus.mhx1999.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://euu.shanyushiyangtech.top

TS:   同 JS
来源：http://nik.shanyushiyangtech.top

Java: 方法内为块级作用域
来源：http://hsf.jinqigfzy.top

Go:   花括号块级作用域
来源：http://dao.fehbvm.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://day.xziqi.cn

C#:   块级作用域
来源：http://rzi.iojbl.cn

[C11] 模块导入与导出
来源：http://pot.zhiwuduotai.top

Py:   from module import func
来源：http://muu.smart0.xyz

PHP:  require "file.php";  或 use App\Service;
来源：http://snx.ctjpmb.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://cna.shanyushiyangkeji.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://khy.yueranfly.top

Java: import java.util.List;
来源：http://cwz.guowangkeji.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://yfo.cheryme.top

Ruby: require "json"; require_relative "./util"
来源：http://ryd.pengpengdd.cyou

C#:   using System.Text;
来源：http://jou.gaohongyu789.top

[C12] 立即执行函数 IIFE
来源：http://mxo.nanxinkj.top

Py:   (lambda: print("run"))()
来源：http://awy.shanyushiyangkeji.top

PHP:  (function () { echo "run"; })();
来源：http://fxh.yuxming.cn

JS:   (() => { console.log("run"); })();
来源：http://yjs.bbcook.cn

TS:   (() => { console.log("run"); })();
来源：http://cay.iojbl.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://cif.daxiang520.top

Go:   func() { fmt.Println("run") }()
来源：http://jqb.xingfuxueyuan.xyz

Ruby: -> { puts "run" }.call
来源：http://tye.zhaomingkeji.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://umd.yueranfly.top

[C13] 类型声明 / 类型注解
来源：http://zlz.sweek.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ife.gaohongyu789.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ygl.snrcjt.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://gdm.yfazqb.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wvp.iojbl.cn

Java: int add(int a, int b) { return a + b; }
来源：http://qrb.jyoumei.cn

Go:   func add(a, b int) int
来源：http://kel.xingfuxueyuan.xyz

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://dxw.tanke756.top

C#:   int Add(int a, int b) => a + b;
来源：http://kay.wangshuangyany.cn

[C14] 泛型函数
来源：http://kmr.52xcode.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ylm.fehbvm.com

PHP:  // 无泛型
来源：http://ktg.jqgufenzy.top

JS:   // 无泛型
来源：http://xmj.gogol.net.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://yrf.bjfxy.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://rnv.ehwqpu.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://vhx.ybcxt.top

Ruby: # 无泛型
来源：http://smu.birdmap.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://und.uphjek.com

[C15] 解构 / 展开参数
来源：http://mix.quarkkingdee.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wyq.ivvv.top

PHP:  [$a, $b] = $pair;
来源：http://cdh.sysykeji.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hja.birdmap.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://fah.jqgfzy.top

Java: // 无解构
来源：http://tzl.zhaomingkeji.xyz

Go:   // 无解构
来源：http://gla.zhengqikj.top

Ruby: a, b = pair
来源：http://jee.hcnkem.com

C#:   var (a, b) = pair;
来源：http://nis.yj202588.top

[C16] 函数 / 方法重载
来源：http://xzn.cucudq.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ruq.sjlbkw.cn

PHP:  // 无重载
来源：http://btr.smart0.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://lxl.zhongyouzk.top

TS:   // 用联合类型或重载签名声明
来源：http://enz.52xcode.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://jmq.tian-w.cn

Go:   // 无重载：用不同函数名
来源：http://zld.sjlbkw.cn

Ruby: # 无重载：靠动态参数
来源：http://vbw.hywenlv.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://enu.birdmap.top

================================================================================
来源：http://mam.zhongyouzk.top

D. 数组 / 列表 / 集合
来源：http://lvg.xingfuxueyuan.xyz

================================================================================
来源：http://zbw.sxryk.cn

[D01] 创建数组 / 列表
来源：http://xpm.kuanghao11.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://lpb.cashguo.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://orf.yvedp.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://eyu.iojbl.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://dll.yonumen.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ars.ywan-chungtsiang.top

Go:   arr := []int{1, 2, 3}
来源：http://dwg.birdmap.top

Ruby: arr = [1, 2, 3]
来源：http://bii.quarkkingdee.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ylh.52xcode.cn

[D02] 追加元素到末尾
来源：http://efg.jinqigufen.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://xns.jlsjyb.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ojt.meibo888.top

JS:   arr.push(4);
来源：http://ovi.ydzc1.top

TS:   arr.push(4);
来源：http://vuv.hnxiangtu.top

Java: list.add(4);
来源：http://eyx.yj202588.top

Go:   arr = append(arr, 4)
来源：http://fxg.zhaomingkeji.xyz

Ruby: arr << 4; arr.push(5)
来源：http://vvy.hnxiangtu.top

C#:   list.Add(4);
来源：http://bpv.hfpthk.cn

[D03] 在指定位置插入元素
来源：http://pfr.guannengcc.top

Py:   arr.insert(0, 0)
来源：http://yet.fengsongda.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ece.fengsongda.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://xol.jinghuilouyu.cn

TS:   arr.splice(0, 0, 0);
来源：http://rwh.gzhubu.top

Java: list.add(0, 0);
来源：http://nvl.xuanzx.com

Go:   arr = append([]int{0}, arr...)
来源：http://pqd.redwolf501.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://gdj.gotoacloud.top

C#:   list.Insert(0, 0);
来源：http://ypc.yuanzhike.top

[D04] 删除元素
来源：http://bpe.tarul.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://obm.quarkkingdee.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ohc.zhoulong.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://iru.nanxinkj.top

TS:   arr.splice(0, 1);
来源：http://azv.pycfn.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://cxd.shanyushiyangkeji.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://krb.yj20258888.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://yqw.tianlin.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ykl.zhijiandao.cn

[D05] 访问与修改元素
来源：http://mii.gogol.net.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://pok.gzhubu.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://lhu.jinghuilouyu.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://qdw.cucudq.cn

TS:   arr[0]; arr.at(-1);
来源：http://jxt.hywenlv.cn

Java: list.get(0); list.set(0, 9);
来源：http://wxd.gogol.net.cn

Go:   arr[0]; arr[0] = 9
来源：http://xvr.0kj1m.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://xld.hywenlv.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://voa.ybcxt.top

[D06] 数组长度
来源：http://tts.wangshuangyany.cn

Py:   len(arr)
来源：http://eek.haohaochexian.top

PHP:  count($arr);
来源：http://pxd.tianlin.xyz

JS:   arr.length
来源：http://tgw.jqgfzy.top

TS:   arr.length
来源：http://vus.gogol.net.cn

Java: list.size();
来源：http://fgx.fehbvm.com

Go:   len(arr)
来源：http://xdz.jinghuilouyu.cn

Ruby: arr.length; arr.size
来源：http://gzv.daxiang520.top

C#:   list.Count;
来源：http://xyc.yvedp.cn

[D07] 切片 / 取子数组
来源：http://ifr.0kj1m.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://etx.pengpengdd.cyou

PHP:  array_slice($arr, 1, 3);
来源：http://wbl.fehbvm.com

JS:   arr.slice(1, 4);
来源：http://luu.tian-w.cn

TS:   arr.slice(1, 4);
来源：http://goz.hnxiangtu.top

Java: list.subList(1, 4);
来源：http://boi.hywenlv.cn

Go:   arr[1:4]
来源：http://jwt.sysykeji.top

Ruby: arr[1, 3]
来源：http://qng.zdbjq.cn

C#:   list.GetRange(1, 3);
来源：http://xkp.pengpengdd.cyou

[D08] 合并两个数组
来源：http://oem.jqgufenzy.top

Py:   a + b;  a.extend(b)
来源：http://uxy.jinyuanbaomall.cn

PHP:  array_merge($a, $b);
来源：http://crw.wangshuangyany.cn


<!-- 参考信息 -->