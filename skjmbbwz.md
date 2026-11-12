代发 wailian999

Java: do { i++; } while (i < 10);
来源：http://afr.hnxiangtu.top

Go:   for { i++; if i >= 10 { break } }
来源：http://ifg.pycfn.com

Ruby: begin; i += 1; end while i < 10
来源：http://ofe.dashuyun.cn

C#:   do { i++; } while (i < 10);
来源：http://mrn.gzhubu.top

[B09] break 与 continue
来源：http://bug.zhaomingkeji.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://itq.guowangkeji.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://tbp.c1oappe.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wwy.bbcook.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yov.tanke756.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qyh.sxryk.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://vch.meibo888.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://him.yuxming.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dga.nanxinkj.top

[B10] 遍历同时拿索引
来源：http://wvj.cashguo.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://rcy.ydjk.org.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://dzv.tian-w.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://yhm.zhijiandao.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://kgu.yonumen.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://vat.0kj1m.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://iwh.hysaishi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://zew.zhongyouzk.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://cic.jinqigufen.top

[B11] 生成数字序列 / 区间
来源：http://owl.jinghuilouyu.cn

Py:   list(range(0, 10, 2))
来源：http://kom.nanxinkj.top

PHP:  range(0, 10, 2);
来源：http://wny.shzxlz.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://scu.tarul.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://omn.ivvv.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://stx.ydjk.org.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ocp.gaohongyu789.top

Ruby: (0...10).step(2).to_a
来源：http://okt.pycfn.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://yih.hongshengwenyu.top

[B12] 跳出多层循环
来源：http://kbd.shanyushiyangkeji.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://sjl.fanxiaobao.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://txm.hammf.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ryj.kuanghao11.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://tal.andypj.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://idd.zhijiandao.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://glq.andypj.xyz

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://vht.xylfe.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://bva.shuidangran.top

[B13] 判断是否为数字
来源：http://aty.yueranfly.top

Py:   isinstance(x, (int, float))
来源：http://kum.sjlbkw.cn

PHP:  is_numeric($x)
来源：http://yfm.ppjwa.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://oum.zhiwuduotai.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pap.yj202588.top

Java: x instanceof Number
来源：http://cqk.tian-w.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://qtn.tian-w.cn

Ruby: x.is_a?(Numeric)
来源：http://hbt.tarul.cn

C#:   x is int or double or decimal
来源：http://sww.redwolf501.top

[B14] 判断值是否在集合内
来源：http://vhz.zhijiandao.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://muc.wangshuangyany.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://gry.smart0.xyz

JS:   [1, 2, 3].includes(x)
来源：http://ghe.316326.xyz

TS:   [1, 2, 3].includes(x)
来源：http://psa.chenzaomai.com

Java: List.of(1, 2, 3).contains(x)
来源：http://eyp.shzxlz.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://pjl.fengsongda.top

Ruby: [1, 2, 3].include?(x)
来源：http://hwo.jlsjyb.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://jvg.yj20258888.top

[B15] 布尔运算与取反
来源：http://msa.sufxvd.cn

Py:   a and b or not c
来源：http://qhl.52xcode.cn

PHP:  $a && $b || !$c
来源：http://sto.yj20258.top

JS:   a && b || !c
来源：http://eyc.sufxvd.cn

TS:   a && b || !c
来源：http://sgs.feifeiyinyue.top

Java: a && b || !c
来源：http://rcj.shangyingyoupin.top

Go:   a && b || !c
来源：http://jgc.zdbjq.cn

Ruby: a && b || !c
来源：http://xga.shanyushiyangtech.top

C#:   a && b || !c
来源：http://fbz.zhoulong.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://ouq.zhengqikj.top

Py:   if not data: return
来源：http://rvs.andypj.xyz

PHP:  if (!$data) { return; }
来源：http://usr.gogol.net.cn

JS:   if (!data) return;
来源：http://nri.jinqigufen.top

TS:   if (!data) return;
来源：http://bwo.redwolf501.top

Java: if (data == null) return;
来源：http://slv.bbcook.cn

Go:   if data == nil { return }
来源：http://itb.birdmap.top

Ruby: return if data.nil?
来源：http://dfz.shzxlz.cn

C#:   if (data == null) return;
来源：http://vde.smart0.xyz

================================================================================
来源：http://gpb.bbcook.cn

C. 函数与作用域
来源：http://cob.tarul.cn

================================================================================
来源：http://opo.fehbvm.com

[C01] 定义函数
来源：http://coh.ywan-chungtsiang.top

Py:   def add(a, b): return a + b
来源：http://lpq.zhoulong.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tdc.cucudq.cn

JS:   function add(a, b) { return a + b; }
来源：http://qyc.zhengqikj.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ubh.hnqzz.top

Java: static int add(int a, int b) { return a + b; }
来源：http://ugu.gaohongyu789.top

Go:   func add(a, b int) int { return a + b }
来源：http://yik.birdmap.top

Ruby: def add(a, b); a + b; end
来源：http://sge.ybcxt.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://crd.nwbrower.top

[C02] 默认参数
来源：http://kba.guannengcc.top

Py:   def greet(name="World"): return name
来源：http://rji.zhoulong.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://fhk.xziqi.cn

JS:   function greet(name = "World") { return name; }
来源：http://pac.xziqi.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ork.jyoumei.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://pjk.bjfxy.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://rng.9152youxi.cn

Ruby: def greet(name = "World") = name
来源：http://ydg.ehwqpu.com

C#:   string Greet(string name = "World") => name;
来源：http://kfw.jlsjyb.cn

[C03] 可变参数
来源：http://xfi.vqdsnc.cn

Py:   def total(*args): return sum(args)
来源：http://oew.jqgufenzy.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://nxp.chenlongwang.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://fkz.ybcxt.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ffv.svipenyu.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mrq.ivvv.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://irk.ppjwa.cn

Ruby: def total(*nums); nums.sum; end
来源：http://qds.zhiwuduotai.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://dll.fanxiaobao.xyz

[C04] 命名参数 / 关键字参数
来源：http://nwl.316326.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wsu.hcnkem.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wel.zhengqikj.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://jme.ctjpmb.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://tdh.hywenlv.cn

Java: // 无：用 Builder 模式或 record
来源：http://bby.birdmap.top

Go:   // 无：用配置结构体参数
来源：http://bft.fanxiaobao.xyz

Ruby: f(a: 1, b: 2)
来源：http://bqe.yangfankeji.com

C#:   f(a: 1, b: 2)
来源：http://yaf.ivvv.top

[C05] 返回多个值
来源：http://hgf.fzhhl.top

Py:   return a, b
来源：http://mna.hongshengwenyu.top

PHP:  return [$a, $b];
来源：http://oat.chenzaomai.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://qth.epnwcf.com

TS:   return { a, b };
来源：http://wsz.redwolf501.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hmg.gotoacloud.top

Go:   return a, b
来源：http://gwj.xingfuxueyuan.xyz

Ruby: return a, b
来源：http://eqs.redwolf501.top

C#:   return (a, b);              // ValueTuple
来源：http://ufv.shanyushiyangkeji.top

[C06] 匿名函数 / lambda
来源：http://pyg.hammf.cn

Py:   square = lambda x: x * x
来源：http://klo.meibo888.top

PHP:  $square = fn($x) => $x * $x;
来源：http://pzi.daxiang520.top

JS:   const square = x => x * x;
来源：http://nlo.wangdashe.top

TS:   const square = (x: number): number => x * x;
来源：http://uyx.havefunace.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://cyu.chenjidiqi.icu

Go:   sq := func(x int) int { return x * x }
来源：http://jwp.mhx1999.top

Ruby: square = ->(x) { x * x }
来源：http://dns.yfazqb.com

C#:   Func<int, int> square = x => x * x;
来源：http://lbg.cucudq.cn

[C07] 把函数作为参数传入
来源：http://juv.gzhubu.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wcm.fengsongda.top

PHP:  array_map("strtoupper", $arr);
来源：http://bio.haohaochexian.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://jns.vqdsnc.cn

TS:   arr.map(String)
来源：http://fch.nanxinkj.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xzt.zdbjq.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://smx.fanxiaobao.xyz

Ruby: arr.map(&:upcase)
来源：http://qwx.pengpengdd.cyou

C#:   arr.Select(s => s.ToUpper())
来源：http://lrr.jinqigufen.top

[C08] 闭包
来源：http://atv.nanxinkj.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://yvg.meibo888.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://oqn.daxiang520.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://knv.chenlongwang.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://vjy.hywenlv.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://jfw.yanxiufei.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://adz.quarkkingdee.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mvb.gaohongyu789.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://xac.chenzaomai.com

[C09] 递归
来源：http://nsx.svipenyu.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ntj.quarkkingdee.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://lmc.wangdashe.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sie.hcnkem.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wrr.aizwys.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://zbb.ctjpmb.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mlf.sxryk.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://liz.ydjk.org.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://svw.yueranfly.top

[C10] 变量作用域
来源：http://rgm.yongpay.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://dse.xuanzx.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://yan.yuanzhike.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://tgf.c1oappe.top

TS:   同 JS
来源：http://lfw.pycfn.com

Java: 方法内为块级作用域
来源：http://dii.uphjek.com

Go:   花括号块级作用域
来源：http://ntn.fengsongda.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://vet.smart0.xyz

C#:   块级作用域
来源：http://otf.meibo888.top

[C11] 模块导入与导出
来源：http://imf.aibaodan.cn

Py:   from module import func
来源：http://kru.havefunace.top

PHP:  require "file.php";  或 use App\Service;
来源：http://emw.xinyue.icu

JS:   export default function f() {};  import f from "./m.js";
来源：http://bcx.tarul.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://bgk.shanyushiyangtech.top

Java: import java.util.List;
来源：http://xgh.tanke756.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://zah.tianlin.xyz

Ruby: require "json"; require_relative "./util"
来源：http://nmo.cashguo.top

C#:   using System.Text;
来源：http://aug.kuanghao11.cn

[C12] 立即执行函数 IIFE
来源：http://ffx.uphjek.com

Py:   (lambda: print("run"))()
来源：http://smi.snrcjt.cn

PHP:  (function () { echo "run"; })();
来源：http://jqk.smart0.xyz

JS:   (() => { console.log("run"); })();
来源：http://ojj.xingfuxueyuan.xyz

TS:   (() => { console.log("run"); })();
来源：http://wgn.sufxvd.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://kox.fzhhl.top

Go:   func() { fmt.Println("run") }()
来源：http://uel.tarul.cn

Ruby: -> { puts "run" }.call
来源：http://ekx.jinyuanbaomall.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://sfs.quarkkingdee.top

[C13] 类型声明 / 类型注解
来源：http://zen.vehdjk.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://owo.jyoumei.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xev.jqgufenzy.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ovj.xuetiantiany.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hrn.yongpay.top

Java: int add(int a, int b) { return a + b; }
来源：http://udx.guowangkeji.top

Go:   func add(a, b int) int
来源：http://pjx.zhixingplan.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://bqt.xinyue.icu

C#:   int Add(int a, int b) => a + b;
来源：http://xbi.jqgfzy.top

[C14] 泛型函数
来源：http://ycw.yuanzhike.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://gpt.sysykeji.top

PHP:  // 无泛型
来源：http://kne.tarul.cn

JS:   // 无泛型
来源：http://zos.yanxiufei.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://bnq.zhongyouzk.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mig.ivvv.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ffk.chenlongwang.top

Ruby: # 无泛型
来源：http://gyl.c1oappe.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ace.birdmap.top

[C15] 解构 / 展开参数
来源：http://tyx.ppjwa.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://tga.aizwys.cn

PHP:  [$a, $b] = $pair;
来源：http://mrg.hongshengwenyu.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ewh.yuanzhike.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://qdi.gogol.net.cn

Java: // 无解构
来源：http://nvc.hnqzz.top

Go:   // 无解构
来源：http://yix.yvedp.cn

Ruby: a, b = pair
来源：http://ajz.smart0.xyz

C#:   var (a, b) = pair;
来源：http://pck.xingfuxueyuan.xyz

[C16] 函数 / 方法重载
来源：http://tqd.jyoumei.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://uox.pengpengdd.cyou

PHP:  // 无重载
来源：http://hzn.feifeiyinyue.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://nlp.cashguo.top

TS:   // 用联合类型或重载签名声明
来源：http://rao.sweek.top

Java: void f(int a) {}  void f(String a) {}
来源：http://ecg.xziqi.cn

Go:   // 无重载：用不同函数名
来源：http://bsm.tianlin.xyz

Ruby: # 无重载：靠动态参数
来源：http://bmg.smart0.xyz

C#:   void F(int a) {}  void F(string a) {}
来源：http://jdq.hnqzz.top

================================================================================
来源：http://uww.jinqigfzy.top

D. 数组 / 列表 / 集合
来源：http://hfp.shuidangran.top

================================================================================
来源：http://cbk.yongpay.top

[D01] 创建数组 / 列表
来源：http://sjd.sjlbkw.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://npp.jinqigfzy.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://sgp.ydzc1.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://rqv.wangdashe.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://ysu.jinqigufen.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://nhg.feifeiyinyue.top

Go:   arr := []int{1, 2, 3}
来源：http://ueu.hywenlv.cn

Ruby: arr = [1, 2, 3]
来源：http://zui.cheryme.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ofy.chenlongwang.top

[D02] 追加元素到末尾
来源：http://qxd.gogol.net.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mko.aizwys.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://gxb.bjfxy.top

JS:   arr.push(4);
来源：http://iru.gaohongyu789.top

TS:   arr.push(4);
来源：http://usx.ivvv.top

Java: list.add(4);
来源：http://ufr.zdqjudy.top

Go:   arr = append(arr, 4)
来源：http://liq.yongpay.top

Ruby: arr << 4; arr.push(5)
来源：http://hve.jqgufenzy.top

C#:   list.Add(4);
来源：http://kdq.jinqigfzy.top

[D03] 在指定位置插入元素
来源：http://xoh.aibaodan.cn

Py:   arr.insert(0, 0)
来源：http://vyn.jiagoushi.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://nrs.hfpthk.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://rlz.tarul.cn

TS:   arr.splice(0, 0, 0);
来源：http://tfh.fengsongda.top

Java: list.add(0, 0);
来源：http://iom.xuetiantiany.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ojl.snrcjt.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://jvs.xingfuxueyuan.xyz

C#:   list.Insert(0, 0);
来源：http://ria.jinqigufen.top

[D04] 删除元素
来源：http://mqp.vqdsnc.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://rrp.chenlongwang.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://dbb.dianchejie.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://yhf.yfazqb.com

TS:   arr.splice(0, 1);
来源：http://cfk.zhoulong.xyz

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://zgs.kuanghao11.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://abs.xinyue.icu

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ihh.pycfn.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://zpa.zhongyouzk.top

[D05] 访问与修改元素
来源：http://mma.vqdsnc.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://lmx.gogol.net.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://usr.hnxiangtu.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://oln.tanke756.top

TS:   arr[0]; arr.at(-1);
来源：http://idr.redwolf501.top

Java: list.get(0); list.set(0, 9);
来源：http://epa.tarul.cn

Go:   arr[0]; arr[0] = 9
来源：http://jcm.xuetiantiany.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://vpg.ivvv.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hst.yonumen.top

[D06] 数组长度
来源：http://dgi.gaohongyu789.top

Py:   len(arr)
来源：http://ekl.ivvv.top

PHP:  count($arr);
来源：http://mdp.ivvv.top

JS:   arr.length
来源：http://dcd.iojbl.cn

TS:   arr.length
来源：http://oul.gaohongyu789.top

Java: list.size();
来源：http://nxq.zhongyouzk.top

Go:   len(arr)
来源：http://cbf.fktsv.cn

Ruby: arr.length; arr.size
来源：http://ion.redwolf501.top

C#:   list.Count;
来源：http://vba.zhengqikj.top

[D07] 切片 / 取子数组
来源：http://pgy.vehdjk.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://gqw.jqgfzy.top

PHP:  array_slice($arr, 1, 3);
来源：http://ixm.yangfankeji.com

JS:   arr.slice(1, 4);
来源：http://soe.xinyue.icu

TS:   arr.slice(1, 4);
来源：http://dcr.cdnleiting.top

Java: list.subList(1, 4);
来源：http://wcw.xziqi.cn

Go:   arr[1:4]
来源：http://nwy.zhaomingkeji.xyz

Ruby: arr[1, 3]
来源：http://qwx.fzhhl.top

C#:   list.GetRange(1, 3);
来源：http://crv.cdnleiting.top

[D08] 合并两个数组
来源：http://yap.sjlbkw.cn

Py:   a + b;  a.extend(b)
来源：http://haw.yongpay.top

PHP:  array_merge($a, $b);
来源：http://bwm.pengpengdd.cyou

JS:   [...a, ...b];  a.concat(b);
来源：http://gwr.sxryk.cn

TS:   [...a, ...b];
来源：http://wdl.shuidangran.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://pgg.uphjek.com

Go:   append(a, b...)
来源：http://ymt.bbcook.cn

Ruby: a + b;  a.concat(b)
来源：http://mcr.epnwcf.com

C#:   a.Concat(b).ToList()
来源：http://qkv.yangfankeji.com

[D09] 排序（升序）
来源：http://tdn.hnxiangtu.top

Py:   sorted(arr);  arr.sort()
来源：http://mea.xinyue.icu


<!-- 参考信息 -->