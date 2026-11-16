代发 wailian999

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hsa.zdbjq.cn

Ruby: while i < 10; i += 1; end
来源：http://uka.xinyue.icu

C#:   while (i < 10) { i++; }
来源：http://heg.yanxiufei.cn

[B08] do-while（至少执行一次）
来源：http://uow.shzxlz.cn

Py:   # 无 do-while：用 while True + break
来源：http://uol.shzxlz.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ztg.haohaochexian.top

JS:   do { i++; } while (i < 10);
来源：http://pmv.andypj.xyz

TS:   do { i++; } while (i < 10);
来源：http://liq.cucudq.cn

Java: do { i++; } while (i < 10);
来源：http://vqb.shzxlz.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://kua.shanyushiyangkeji.top

Ruby: begin; i += 1; end while i < 10
来源：http://pvq.fzhhl.top

C#:   do { i++; } while (i < 10);
来源：http://nki.yueranfly.top

[B09] break 与 continue
来源：http://oei.ivvv.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://fcw.kuanghao11.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://qyd.xingfuxueyuan.xyz

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pvo.0kj1m.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://svj.tian-w.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nzo.jiagoushi.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://fay.tanke756.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://exd.yonumen.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ihb.ydjk.org.cn

[B10] 遍历同时拿索引
来源：http://php.iojbl.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://jou.sysykeji.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://uzv.52xcode.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://pwq.dianchejie.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://opo.xuetiantiany.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://bji.ydjk.org.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://uil.smart0.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://yyd.zhoulong.xyz

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://tdm.aibaodan.cn

[B11] 生成数字序列 / 区间
来源：http://kjb.zhengqikj.top

Py:   list(range(0, 10, 2))
来源：http://duc.ybcxt.top

PHP:  range(0, 10, 2);
来源：http://cdz.chenjidiqi.icu

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hmk.xuetiantiany.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jzw.ydjk.org.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://vns.gotoacloud.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://gvf.smart0.xyz

Ruby: (0...10).step(2).to_a
来源：http://njr.zdqjudy.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ttx.zdqjudy.top

[B12] 跳出多层循环
来源：http://xyp.zhijiandao.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://cmn.nanxinkj.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://rny.hongshengwenyu.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wgr.yuxming.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wio.zdqjudy.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://cjr.cdnleiting.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ged.svipenyu.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mmf.ehwqpu.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ssn.zhengqikj.top

[B13] 判断是否为数字
来源：http://wzo.hcnkem.com

Py:   isinstance(x, (int, float))
来源：http://bcr.hammf.cn

PHP:  is_numeric($x)
来源：http://alw.zdqjudy.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jhl.jqgufenzy.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rlv.shuidangran.top

Java: x instanceof Number
来源：http://atx.fehbvm.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://tra.chenlongwang.top

Ruby: x.is_a?(Numeric)
来源：http://khf.hesvh.cn

C#:   x is int or double or decimal
来源：http://ams.guowangkeji.top

[B14] 判断值是否在集合内
来源：http://xtr.pycfn.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://zpd.aizwys.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://kfn.cdnleiting.top

JS:   [1, 2, 3].includes(x)
来源：http://hre.yj202588.top

TS:   [1, 2, 3].includes(x)
来源：http://flw.jqgufenzy.top

Java: List.of(1, 2, 3).contains(x)
来源：http://hoe.fktsv.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://fpn.smart0.xyz

Ruby: [1, 2, 3].include?(x)
来源：http://tdh.aibaodan.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://nns.fzhhl.top

[B15] 布尔运算与取反
来源：http://bfz.tian-w.cn

Py:   a and b or not c
来源：http://buz.xuanzx.com

PHP:  $a && $b || !$c
来源：http://oov.shanyushiyangtech.top

JS:   a && b || !c
来源：http://obg.daxiang520.top

TS:   a && b || !c
来源：http://emr.cheryme.top

Java: a && b || !c
来源：http://wqr.tarul.cn

Go:   a && b || !c
来源：http://xfe.jinqigfzy.top

Ruby: a && b || !c
来源：http://pol.zdbjq.cn

C#:   a && b || !c
来源：http://giw.0kj1m.cn

[B16] 卫语句：不满足条件提前返回
来源：http://gzw.jiagoushi.top

Py:   if not data: return
来源：http://jis.hongshengwenyu.top

PHP:  if (!$data) { return; }
来源：http://pbq.iojbl.cn

JS:   if (!data) return;
来源：http://zww.zhijiandao.cn

TS:   if (!data) return;
来源：http://pob.shuidangran.top

Java: if (data == null) return;
来源：http://ndn.ybcxt.top

Go:   if data == nil { return }
来源：http://qxi.jinyuanbaomall.cn

Ruby: return if data.nil?
来源：http://mcd.yongpay.top

C#:   if (data == null) return;
来源：http://fto.guowangkeji.top

================================================================================
来源：http://zuo.yueranfly.top

C. 函数与作用域
来源：http://wam.daria6918.cn

================================================================================
来源：http://kup.xinyue.icu

[C01] 定义函数
来源：http://uuv.yj20258.top

Py:   def add(a, b): return a + b
来源：http://qjm.xziqi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sna.yanxiufei.cn

JS:   function add(a, b) { return a + b; }
来源：http://ryd.iojbl.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://aaz.gzhubu.top

Java: static int add(int a, int b) { return a + b; }
来源：http://pdg.316326.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://mlf.epnwcf.com

Ruby: def add(a, b); a + b; end
来源：http://otb.jianghu66.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mqj.jianghu66.top

[C02] 默认参数
来源：http://gbh.andypj.xyz

Py:   def greet(name="World"): return name
来源：http://dth.zhoulong.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://mzl.shanyushiyangkeji.top

JS:   function greet(name = "World") { return name; }
来源：http://vkm.andypj.xyz

TS:   function greet(name: string = "World") { return name; }
来源：http://ghs.jqgufenzy.top

Java: // 无默认参数：方法重载或 Optional
来源：http://vit.tianlin.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://pph.hammf.cn

Ruby: def greet(name = "World") = name
来源：http://swh.ywan-chungtsiang.top

C#:   string Greet(string name = "World") => name;
来源：http://xzc.yanxiufei.cn

[C03] 可变参数
来源：http://xil.shangyingyoupin.top

Py:   def total(*args): return sum(args)
来源：http://gfa.dianchejie.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ynq.jinqigfzy.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ahq.yongpay.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mnh.meibo888.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://eev.jinqigufen.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://bba.hesvh.cn

Ruby: def total(*nums); nums.sum; end
来源：http://qjo.gaohongyu789.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://trm.zhixingplan.top

[C04] 命名参数 / 关键字参数
来源：http://rja.smart0.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://yub.shuidangran.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://uoh.shuidangran.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://vxc.shzxlz.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://cai.cheryme.top

Java: // 无：用 Builder 模式或 record
来源：http://ykx.vehdjk.com

Go:   // 无：用配置结构体参数
来源：http://snt.ybcxt.top

Ruby: f(a: 1, b: 2)
来源：http://nuz.pycfn.com

C#:   f(a: 1, b: 2)
来源：http://rar.316326.xyz

[C05] 返回多个值
来源：http://dou.ywan-chungtsiang.top

Py:   return a, b
来源：http://mrh.yvedp.cn

PHP:  return [$a, $b];
来源：http://izf.0kj1m.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://jdo.sweek.top

TS:   return { a, b };
来源：http://kds.andypj.xyz

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://tsv.cdnleiting.top

Go:   return a, b
来源：http://nuh.zhoulong.xyz

Ruby: return a, b
来源：http://rbl.bbcook.cn

C#:   return (a, b);              // ValueTuple
来源：http://axl.jinyuanbaomall.cn

[C06] 匿名函数 / lambda
来源：http://imh.bjfxy.top

Py:   square = lambda x: x * x
来源：http://fve.quarkkingdee.top

PHP:  $square = fn($x) => $x * $x;
来源：http://mdd.guowangkeji.top

JS:   const square = x => x * x;
来源：http://xyp.bjfxy.top

TS:   const square = (x: number): number => x * x;
来源：http://qbn.yuxming.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://cbm.quarkkingdee.top

Go:   sq := func(x int) int { return x * x }
来源：http://yoh.9152youxi.cn

Ruby: square = ->(x) { x * x }
来源：http://mky.meibo888.top

C#:   Func<int, int> square = x => x * x;
来源：http://ldm.chenlongwang.top

[C07] 把函数作为参数传入
来源：http://ors.xylfe.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://cky.yongpay.top

PHP:  array_map("strtoupper", $arr);
来源：http://qsv.jyoumei.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://gvf.yongpay.top

TS:   arr.map(String)
来源：http://ppq.jiagoushi.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://jsk.feifeiyinyue.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://xmk.yongpay.top

Ruby: arr.map(&:upcase)
来源：http://khi.zdbjq.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://esc.cdnleiting.top

[C08] 闭包
来源：http://tiu.jianghu66.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://lnb.havefunace.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://tvj.hfpthk.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://lux.chenlongwang.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mzu.tanke756.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://esx.tianlin.xyz

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://zbf.ppjwa.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://kov.guannengcc.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://rvd.hysaishi.cn

[C09] 递归
来源：http://rcg.9152youxi.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://tms.hfpthk.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://uzk.svipenyu.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://apk.vqdsnc.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hrk.shanyushiyangkeji.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://szv.tarul.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://kgd.yanxiufei.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://bmg.sysykeji.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://rss.meibo888.top

[C10] 变量作用域
来源：http://rys.daria6918.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://jnt.yuxming.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://xkp.jinyuanbaomall.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://obs.zhixingplan.top

TS:   同 JS
来源：http://bbi.xinyue.icu

Java: 方法内为块级作用域
来源：http://vkt.hywenlv.cn

Go:   花括号块级作用域
来源：http://cgs.jinghuilouyu.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://htg.xinyue.icu

C#:   块级作用域
来源：http://ncb.jiagoushi.top

[C11] 模块导入与导出
来源：http://elq.pengpengdd.cyou

Py:   from module import func
来源：http://ztk.shuidangran.top

PHP:  require "file.php";  或 use App\Service;
来源：http://zjd.snrcjt.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://qkp.vehdjk.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://lut.ydjk.org.cn

Java: import java.util.List;
来源：http://nyp.dianchejie.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://fss.dianchejie.cn

Ruby: require "json"; require_relative "./util"
来源：http://aur.c1oappe.top

C#:   using System.Text;
来源：http://djm.cashguo.top

[C12] 立即执行函数 IIFE
来源：http://yzn.yuanzhike.top

Py:   (lambda: print("run"))()
来源：http://knv.sufxvd.cn

PHP:  (function () { echo "run"; })();
来源：http://tqf.zycfv.cn

JS:   (() => { console.log("run"); })();
来源：http://hgl.daxiang520.top

TS:   (() => { console.log("run"); })();
来源：http://uah.ywan-chungtsiang.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mvb.guannengcc.top

Go:   func() { fmt.Println("run") }()
来源：http://mlc.dashuyun.cn

Ruby: -> { puts "run" }.call
来源：http://frz.gaohongyu789.top

C#:   // 无 IIFE：用静态构造函数
来源：http://xdb.ppjwa.cn

[C13] 类型声明 / 类型注解
来源：http://ipo.jianghu66.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://gty.yonumen.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://huo.sjlbkw.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://jdr.redwolf501.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fmu.jinghuilouyu.cn

Java: int add(int a, int b) { return a + b; }
来源：http://djm.hywenlv.cn

Go:   func add(a, b int) int
来源：http://xvl.birdmap.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://kfk.wangdashe.top

C#:   int Add(int a, int b) => a + b;
来源：http://gik.vqdsnc.cn

[C14] 泛型函数
来源：http://zbf.gotoacloud.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://fgi.xingfuxueyuan.xyz

PHP:  // 无泛型
来源：http://tzb.hysaishi.cn

JS:   // 无泛型
来源：http://hgf.jlsjyb.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ajb.yj20258.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://jtj.chenzaomai.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://xgs.xinyue.icu

Ruby: # 无泛型
来源：http://upl.yonumen.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://txl.mhx1999.top

[C15] 解构 / 展开参数
来源：http://trh.yj20258888.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://zsb.birdmap.top

PHP:  [$a, $b] = $pair;
来源：http://bbb.zhixingplan.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://lug.zhixingplan.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://xhq.vehdjk.com

Java: // 无解构
来源：http://pge.chenlongwang.top

Go:   // 无解构
来源：http://aua.hnqzz.top

Ruby: a, b = pair
来源：http://axw.tanke756.top

C#:   var (a, b) = pair;
来源：http://pjm.bbcook.cn

[C16] 函数 / 方法重载
来源：http://mfp.iojbl.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://loo.aibaodan.cn

PHP:  // 无重载
来源：http://zgi.52xcode.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://fip.hesvh.cn

TS:   // 用联合类型或重载签名声明
来源：http://dnc.fengsongda.top

Java: void f(int a) {}  void f(String a) {}
来源：http://nim.gotoacloud.top

Go:   // 无重载：用不同函数名
来源：http://zwr.dianchejie.cn

Ruby: # 无重载：靠动态参数
来源：http://ptc.zycfv.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://jds.ctjpmb.com

================================================================================
来源：http://oay.nwbrower.top

D. 数组 / 列表 / 集合
来源：http://olb.hfpthk.cn

================================================================================
来源：http://rus.jqgfzy.top

[D01] 创建数组 / 列表
来源：http://wbc.quarkkingdee.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://zbf.shanyushiyangkeji.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://kmq.ppjwa.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hif.mhx1999.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://dbh.yuanzhike.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://yuk.zhiwuduotai.top

Go:   arr := []int{1, 2, 3}
来源：http://sgx.yongpay.top

Ruby: arr = [1, 2, 3]
来源：http://vuo.andypj.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ymi.zhaomingkeji.xyz

[D02] 追加元素到末尾
来源：http://qwx.yueranfly.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://unl.zycfv.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ahv.sysykeji.top

JS:   arr.push(4);
来源：http://hty.pengpengdd.cyou

TS:   arr.push(4);
来源：http://chl.52xcode.cn

Java: list.add(4);
来源：http://uep.dianchejie.cn

Go:   arr = append(arr, 4)
来源：http://kfk.xinyue.icu

Ruby: arr << 4; arr.push(5)
来源：http://upm.hysaishi.cn

C#:   list.Add(4);
来源：http://jui.c1oappe.top

[D03] 在指定位置插入元素
来源：http://zlq.xylfe.cn

Py:   arr.insert(0, 0)
来源：http://nmq.yuxming.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://arn.yanxiufei.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://akg.kuanghao11.cn

TS:   arr.splice(0, 0, 0);
来源：http://ctl.cucudq.cn

Java: list.add(0, 0);
来源：http://gem.jqgufenzy.top

Go:   arr = append([]int{0}, arr...)
来源：http://kyi.chenzaomai.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://okb.zhaomingkeji.xyz

C#:   list.Insert(0, 0);
来源：http://rjm.ehwqpu.com

[D04] 删除元素
来源：http://hrt.jyoumei.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hdy.yueranfly.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://efk.chenzaomai.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://gej.snrcjt.cn

TS:   arr.splice(0, 1);
来源：http://ppn.wangdashe.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://lic.cucudq.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wcc.zhongyouzk.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://uwj.ydzc1.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ldn.jqgfzy.top

[D05] 访问与修改元素
来源：http://jth.9152youxi.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://avm.daxiang520.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://qbe.zhixingplan.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://nrc.birdmap.top

TS:   arr[0]; arr.at(-1);
来源：http://nbh.nanxinkj.top

Java: list.get(0); list.set(0, 9);
来源：http://bkz.guowangkeji.top

Go:   arr[0]; arr[0] = 9
来源：http://uma.bjfxy.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://tyi.ydjk.org.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hym.mhx1999.top

[D06] 数组长度
来源：http://zbm.nanxuanxn.top

Py:   len(arr)
来源：http://tle.ctjpmb.com

PHP:  count($arr);
来源：http://xge.cheryme.top

JS:   arr.length
来源：http://ivk.ppjwa.cn

TS:   arr.length
来源：http://ujt.gaohongyu789.top

Java: list.size();
来源：http://xxj.zhengqikj.top

Go:   len(arr)
来源：http://tlw.hywenlv.cn

Ruby: arr.length; arr.size
来源：http://apf.gaohongyu789.top

C#:   list.Count;
来源：http://fze.gogol.net.cn

[D07] 切片 / 取子数组
来源：http://ouv.yj20258.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://des.pycfn.com

PHP:  array_slice($arr, 1, 3);
来源：http://ftg.xinyue.icu

JS:   arr.slice(1, 4);
来源：http://lej.jqgfzy.top

TS:   arr.slice(1, 4);
来源：http://lnx.ivvv.top

Java: list.subList(1, 4);
来源：http://yxn.hfpthk.cn

Go:   arr[1:4]
来源：http://azf.daria6918.cn

Ruby: arr[1, 3]
来源：http://eeu.hfpthk.cn

C#:   list.GetRange(1, 3);
来源：http://mwf.smart0.xyz

[D08] 合并两个数组
来源：http://are.jinqigufen.top

Py:   a + b;  a.extend(b)
来源：http://zfc.kuanghao11.cn

PHP:  array_merge($a, $b);
来源：http://guf.redwolf501.top


<!-- 参考信息 -->