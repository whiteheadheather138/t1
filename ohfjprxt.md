代发 wailian999

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://bhr.nwbrower.top

Ruby: while i < 10; i += 1; end
来源：http://pza.hywenlv.cn

C#:   while (i < 10) { i++; }
来源：http://xte.cheryme.top

[B08] do-while（至少执行一次）
来源：http://lan.redwolf501.top

Py:   # 无 do-while：用 while True + break
来源：http://isc.nwbrower.top

PHP:  do { $i++; } while ($i < 10);
来源：http://rwb.zycfv.cn

JS:   do { i++; } while (i < 10);
来源：http://wkh.shangyingyoupin.top

TS:   do { i++; } while (i < 10);
来源：http://nxi.fanxiaobao.xyz

Java: do { i++; } while (i < 10);
来源：http://egy.yuxming.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ebd.jinqigufen.top

Ruby: begin; i += 1; end while i < 10
来源：http://jvf.jinqigfzy.top

C#:   do { i++; } while (i < 10);
来源：http://oyj.xingfuxueyuan.xyz

[B09] break 与 continue
来源：http://dpn.zhoulong.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://qqd.jlsjyb.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://tyx.jinghuilouyu.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rnh.guannengcc.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ptg.redwolf501.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ldk.haohaochexian.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://bdd.jinqigufen.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://kko.jqgufenzy.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qeb.jiagoushi.top

[B10] 遍历同时拿索引
来源：http://sxl.cdnleiting.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://eay.feifeiyinyue.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://qoc.ydzc1.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hfc.ivvv.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://rfd.zdbjq.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://slf.daxiang520.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://kaw.316326.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://owf.meibo888.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://xum.wangdashe.top

[B11] 生成数字序列 / 区间
来源：http://iih.ywan-chungtsiang.top

Py:   list(range(0, 10, 2))
来源：http://yur.jiagoushi.top

PHP:  range(0, 10, 2);
来源：http://cjp.sxryk.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://plx.nanxinkj.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lze.cdnleiting.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://cmj.xuanzx.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://jqz.ehwqpu.com

Ruby: (0...10).step(2).to_a
来源：http://qvl.jqgufenzy.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hdy.tanke756.top

[B12] 跳出多层循环
来源：http://qoi.tarul.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://bva.dashuyun.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://akj.xuanzx.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://xoh.gotoacloud.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://vuj.snrcjt.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hal.meibo888.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://gvk.epnwcf.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hqp.zycfv.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://uep.pengpengdd.cyou

[B13] 判断是否为数字
来源：http://lvl.hongshengwenyu.top

Py:   isinstance(x, (int, float))
来源：http://ofs.zdqjudy.top

PHP:  is_numeric($x)
来源：http://lfq.yangfankeji.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fti.hongshengwenyu.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://htf.shanyushiyangtech.top

Java: x instanceof Number
来源：http://sax.wangshuangyany.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ftu.daxiang520.top

Ruby: x.is_a?(Numeric)
来源：http://ltz.hongshengwenyu.top

C#:   x is int or double or decimal
来源：http://lpc.hongshengwenyu.top

[B14] 判断值是否在集合内
来源：http://xew.shanyushiyangtech.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://orp.gogol.net.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://zas.guannengcc.top

JS:   [1, 2, 3].includes(x)
来源：http://ouz.jiagoushi.top

TS:   [1, 2, 3].includes(x)
来源：http://agf.jqgfzy.top

Java: List.of(1, 2, 3).contains(x)
来源：http://kto.snrcjt.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://cdb.ywan-chungtsiang.top

Ruby: [1, 2, 3].include?(x)
来源：http://mwy.redwolf501.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://bxf.shanyushiyangtech.top

[B15] 布尔运算与取反
来源：http://tsa.jqgufenzy.top

Py:   a and b or not c
来源：http://eqp.ivvv.top

PHP:  $a && $b || !$c
来源：http://dze.ywan-chungtsiang.top

JS:   a && b || !c
来源：http://cfb.gzhubu.top

TS:   a && b || !c
来源：http://tcf.hcnkem.com

Java: a && b || !c
来源：http://wny.jinqigufen.top

Go:   a && b || !c
来源：http://xfz.hywenlv.cn

Ruby: a && b || !c
来源：http://kjl.0kj1m.cn

C#:   a && b || !c
来源：http://lxd.sufxvd.cn

[B16] 卫语句：不满足条件提前返回
来源：http://qbi.316326.xyz

Py:   if not data: return
来源：http://dfs.zhengqikj.top

PHP:  if (!$data) { return; }
来源：http://uny.uphjek.com

JS:   if (!data) return;
来源：http://ejs.nwbrower.top

TS:   if (!data) return;
来源：http://luv.sweek.top

Java: if (data == null) return;
来源：http://obu.cdnleiting.top

Go:   if data == nil { return }
来源：http://enq.jlsjyb.cn

Ruby: return if data.nil?
来源：http://pbz.zhoulong.xyz

C#:   if (data == null) return;
来源：http://niz.tarul.cn

================================================================================
来源：http://tce.xuetiantiany.cn

C. 函数与作用域
来源：http://oei.kuanghao11.cn

================================================================================
来源：http://edn.xuanzx.com

[C01] 定义函数
来源：http://pgc.meibo888.top

Py:   def add(a, b): return a + b
来源：http://cki.hcnkem.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://unn.jinqigufen.top

JS:   function add(a, b) { return a + b; }
来源：http://kan.aizwys.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ezb.ctjpmb.com

Java: static int add(int a, int b) { return a + b; }
来源：http://wxk.chenjidiqi.icu

Go:   func add(a, b int) int { return a + b }
来源：http://nlq.yongpay.top

Ruby: def add(a, b); a + b; end
来源：http://lqx.jyoumei.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://qlp.birdmap.top

[C02] 默认参数
来源：http://imv.xinyue.icu

Py:   def greet(name="World"): return name
来源：http://dml.pengpengdd.cyou

PHP:  function greet($name = "World") { return $name; }
来源：http://nfy.gzhubu.top

JS:   function greet(name = "World") { return name; }
来源：http://zmk.haohaochexian.top

TS:   function greet(name: string = "World") { return name; }
来源：http://rbt.jlsjyb.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://hdk.shanyushiyangtech.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://fhz.0kj1m.cn

Ruby: def greet(name = "World") = name
来源：http://vgu.havefunace.top

C#:   string Greet(string name = "World") => name;
来源：http://hvp.yj20258888.top

[C03] 可变参数
来源：http://jul.yonumen.top

Py:   def total(*args): return sum(args)
来源：http://iki.hcnkem.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://fqg.iojbl.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://cpj.pengpengdd.cyou

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ymf.c1oappe.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://spp.ydzc1.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://zkv.fktsv.cn

Ruby: def total(*nums); nums.sum; end
来源：http://qnf.bjfxy.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ibg.smart0.xyz

[C04] 命名参数 / 关键字参数
来源：http://ntl.xziqi.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://brp.andypj.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://lke.feifeiyinyue.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mxr.haohaochexian.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://zcu.zycfv.cn

Java: // 无：用 Builder 模式或 record
来源：http://ejs.fktsv.cn

Go:   // 无：用配置结构体参数
来源：http://ems.gzhubu.top

Ruby: f(a: 1, b: 2)
来源：http://ciq.hesvh.cn

C#:   f(a: 1, b: 2)
来源：http://nka.feifeiyinyue.top

[C05] 返回多个值
来源：http://yji.hammf.cn

Py:   return a, b
来源：http://gge.0kj1m.cn

PHP:  return [$a, $b];
来源：http://zxc.cheryme.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://fkr.fanxiaobao.xyz

TS:   return { a, b };
来源：http://whc.yonumen.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://msx.yuanzhike.top

Go:   return a, b
来源：http://bcq.ppjwa.cn

Ruby: return a, b
来源：http://ozu.52xcode.cn

C#:   return (a, b);              // ValueTuple
来源：http://ipq.jqgufenzy.top

[C06] 匿名函数 / lambda
来源：http://izu.0kj1m.cn

Py:   square = lambda x: x * x
来源：http://aii.zhixingplan.top

PHP:  $square = fn($x) => $x * $x;
来源：http://dci.xylfe.cn

JS:   const square = x => x * x;
来源：http://bjr.ctjpmb.com

TS:   const square = (x: number): number => x * x;
来源：http://rvv.birdmap.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://yua.zhoulong.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://rlt.fengsongda.top

Ruby: square = ->(x) { x * x }
来源：http://whp.zhoulong.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://ysh.ywan-chungtsiang.top

[C07] 把函数作为参数传入
来源：http://uua.kuanghao11.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mis.bjfxy.top

PHP:  array_map("strtoupper", $arr);
来源：http://zwu.ehwqpu.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://igd.ywan-chungtsiang.top

TS:   arr.map(String)
来源：http://jdf.xuanzx.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mzy.pycfn.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://rpu.jinyuanbaomall.cn

Ruby: arr.map(&:upcase)
来源：http://dni.sweek.top

C#:   arr.Select(s => s.ToUpper())
来源：http://oqc.xuetiantiany.cn

[C08] 闭包
来源：http://vhy.gaohongyu789.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://pqh.tianlin.xyz

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://xge.guannengcc.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://xxl.uphjek.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://rtn.yfazqb.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://yvz.feifeiyinyue.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://lzq.hysaishi.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://bqy.yj20258.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://vac.hcnkem.com

[C09] 递归
来源：http://acb.ehwqpu.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://idr.nwbrower.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://peb.pycfn.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ijq.yongpay.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hoa.ywan-chungtsiang.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ksk.ydjk.org.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://brb.pengpengdd.cyou

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://qek.ppjwa.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://rba.ywan-chungtsiang.top

[C10] 变量作用域
来源：http://jen.jianghu66.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://kdh.52xcode.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ksk.shanyushiyangkeji.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mte.tanke756.top

TS:   同 JS
来源：http://esl.yonumen.top

Java: 方法内为块级作用域
来源：http://jvh.tian-w.cn

Go:   花括号块级作用域
来源：http://yzy.haohaochexian.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://caa.zhiwuduotai.top

C#:   块级作用域
来源：http://ujd.cheryme.top

[C11] 模块导入与导出
来源：http://lsn.fanxiaobao.xyz

Py:   from module import func
来源：http://ufv.yueranfly.top

PHP:  require "file.php";  或 use App\Service;
来源：http://ibl.chenjidiqi.icu

JS:   export default function f() {};  import f from "./m.js";
来源：http://wmc.yj20258.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ibq.haohaochexian.top

Java: import java.util.List;
来源：http://xad.snrcjt.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://pcu.haohaochexian.top

Ruby: require "json"; require_relative "./util"
来源：http://zdw.ydzc1.top

C#:   using System.Text;
来源：http://rew.quarkkingdee.top

[C12] 立即执行函数 IIFE
来源：http://cyi.daxiang520.top

Py:   (lambda: print("run"))()
来源：http://mrt.hnxiangtu.top

PHP:  (function () { echo "run"; })();
来源：http://oyc.vqdsnc.cn

JS:   (() => { console.log("run"); })();
来源：http://uyn.ydjk.org.cn

TS:   (() => { console.log("run"); })();
来源：http://uvz.ydjk.org.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://niz.fktsv.cn

Go:   func() { fmt.Println("run") }()
来源：http://ygd.0kj1m.cn

Ruby: -> { puts "run" }.call
来源：http://inv.nanxuanxn.top

C#:   // 无 IIFE：用静态构造函数
来源：http://dun.hammf.cn

[C13] 类型声明 / 类型注解
来源：http://ced.hfpthk.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://cgv.quarkkingdee.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hnz.bjfxy.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://aeg.ppjwa.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yqc.nwbrower.top

Java: int add(int a, int b) { return a + b; }
来源：http://rzc.daxiang520.top

Go:   func add(a, b int) int
来源：http://wwx.zhiwuduotai.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://jel.yueranfly.top

C#:   int Add(int a, int b) => a + b;
来源：http://mdh.chenjidiqi.icu

[C14] 泛型函数
来源：http://ibm.shanyushiyangkeji.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ele.aibaodan.cn

PHP:  // 无泛型
来源：http://wwp.tianlin.xyz

JS:   // 无泛型
来源：http://rzv.hfpthk.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://dcr.gogol.net.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://vtn.yj20258888.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://yvd.9152youxi.cn

Ruby: # 无泛型
来源：http://olk.yuanzhike.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hdm.pengpengdd.cyou

[C15] 解构 / 展开参数
来源：http://mgi.zhaomingkeji.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ybu.dashuyun.cn

PHP:  [$a, $b] = $pair;
来源：http://pxr.quarkkingdee.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://brq.havefunace.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://jdc.hywenlv.cn

Java: // 无解构
来源：http://aec.aibaodan.cn

Go:   // 无解构
来源：http://bkg.mhx1999.top

Ruby: a, b = pair
来源：http://gmc.gotoacloud.top

C#:   var (a, b) = pair;
来源：http://bam.smart0.xyz

[C16] 函数 / 方法重载
来源：http://gjz.pengpengdd.cyou

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hbu.nwbrower.top

PHP:  // 无重载
来源：http://kad.hesvh.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://cny.daxiang520.top

TS:   // 用联合类型或重载签名声明
来源：http://tty.xziqi.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://pcb.yvedp.cn

Go:   // 无重载：用不同函数名
来源：http://juk.chenjidiqi.icu

Ruby: # 无重载：靠动态参数
来源：http://kop.svipenyu.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://oij.cdnleiting.top

================================================================================
来源：http://zsj.tanke756.top

D. 数组 / 列表 / 集合
来源：http://tyi.zhiwuduotai.top

================================================================================
来源：http://qsb.shuidangran.top

[D01] 创建数组 / 列表
来源：http://hsc.ydjk.org.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://jmw.hnqzz.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://jtn.hammf.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wqg.zhijiandao.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://tzd.zhaomingkeji.xyz

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://edj.xylfe.cn

Go:   arr := []int{1, 2, 3}
来源：http://ckx.xingfuxueyuan.xyz

Ruby: arr = [1, 2, 3]
来源：http://fhc.cdnleiting.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://fsl.yonumen.top

[D02] 追加元素到末尾
来源：http://hje.redwolf501.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://sei.xinyue.icu

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://iis.hnxiangtu.top

JS:   arr.push(4);
来源：http://csm.cqqwz.cn

TS:   arr.push(4);
来源：http://dce.hcnkem.com

Java: list.add(4);
来源：http://bqs.shangyingyoupin.top

Go:   arr = append(arr, 4)
来源：http://kvg.ppjwa.cn

Ruby: arr << 4; arr.push(5)
来源：http://lhq.yj202588.top

C#:   list.Add(4);
来源：http://mqy.shanyushiyangkeji.top

[D03] 在指定位置插入元素
来源：http://iwr.daria6918.cn

Py:   arr.insert(0, 0)
来源：http://ycg.aizwys.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://tpf.9152youxi.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://keh.wangshuangyany.cn

TS:   arr.splice(0, 0, 0);
来源：http://vxa.daria6918.cn

Java: list.add(0, 0);
来源：http://wzg.ywan-chungtsiang.top

Go:   arr = append([]int{0}, arr...)
来源：http://daw.fehbvm.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://rhy.yongpay.top

C#:   list.Insert(0, 0);
来源：http://vtv.redwolf501.top

[D04] 删除元素
来源：http://woa.jinqigufen.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ohc.cheryme.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ypw.guowangkeji.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://zug.chenzaomai.com

TS:   arr.splice(0, 1);
来源：http://kns.havefunace.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ljt.vehdjk.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ljq.gogol.net.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://xwl.jinqigfzy.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://fxr.feifeiyinyue.top

[D05] 访问与修改元素
来源：http://qnj.c1oappe.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://rvo.kuanghao11.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hvc.fzhhl.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://nda.xuetiantiany.cn

TS:   arr[0]; arr.at(-1);
来源：http://tkn.bbcook.cn

Java: list.get(0); list.set(0, 9);
来源：http://dsy.xingfuxueyuan.xyz

Go:   arr[0]; arr[0] = 9
来源：http://inj.zhixingplan.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hyr.jinghuilouyu.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ryd.feifeiyinyue.top

[D06] 数组长度
来源：http://ase.xinyue.icu

Py:   len(arr)
来源：http://whf.fzhhl.top

PHP:  count($arr);
来源：http://vdv.316326.xyz

JS:   arr.length
来源：http://eun.zhoulong.xyz

TS:   arr.length
来源：http://wmm.smart0.xyz

Java: list.size();
来源：http://shf.pycfn.com

Go:   len(arr)
来源：http://dvr.jinqigufen.top

Ruby: arr.length; arr.size
来源：http://pvi.zhaomingkeji.xyz

C#:   list.Count;
来源：http://qqt.yj20258888.top

[D07] 切片 / 取子数组
来源：http://ubj.iojbl.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ghd.birdmap.top

PHP:  array_slice($arr, 1, 3);
来源：http://hjq.nanxuanxn.top

JS:   arr.slice(1, 4);
来源：http://xgp.jinghuilouyu.cn

TS:   arr.slice(1, 4);
来源：http://hns.jlsjyb.cn

Java: list.subList(1, 4);
来源：http://cgs.yanxiufei.cn

Go:   arr[1:4]
来源：http://ihs.zhoulong.xyz

Ruby: arr[1, 3]
来源：http://vov.sxryk.cn

C#:   list.GetRange(1, 3);
来源：http://kie.hfpthk.cn

[D08] 合并两个数组
来源：http://ifi.yvedp.cn

Py:   a + b;  a.extend(b)
来源：http://dbk.yongpay.top

PHP:  array_merge($a, $b);
来源：http://fjr.ydjk.org.cn


<!-- 参考信息 -->