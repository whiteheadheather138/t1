代发 wailian999

Java: do { i++; } while (i < 10);
来源：http://rqi.iojbl.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://akg.hcnkem.com

Ruby: begin; i += 1; end while i < 10
来源：http://urh.tian-w.cn

C#:   do { i++; } while (i < 10);
来源：http://evb.yj202588.top

[B09] break 与 continue
来源：http://vfa.pengpengdd.cyou

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wcf.dashuyun.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://jjt.xuetiantiany.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hcd.yuanzhike.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pch.ybcxt.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://anu.dashuyun.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://kxs.9152youxi.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://qod.vqdsnc.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tnb.guannengcc.top

[B10] 遍历同时拿索引
来源：http://eli.tian-w.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://oqh.fehbvm.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://jsi.fzhhl.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://lwj.ywan-chungtsiang.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://slo.xziqi.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://nib.aibaodan.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://xhz.dashuyun.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://row.zdbjq.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://fna.vqdsnc.cn

[B11] 生成数字序列 / 区间
来源：http://lbe.chenzaomai.com

Py:   list(range(0, 10, 2))
来源：http://pal.guannengcc.top

PHP:  range(0, 10, 2);
来源：http://ozw.tian-w.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://out.snrcjt.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://iqy.dianchejie.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://zee.zdbjq.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://nat.sufxvd.cn

Ruby: (0...10).step(2).to_a
来源：http://hhw.yj202588.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://xyg.yvedp.cn

[B12] 跳出多层循环
来源：http://zth.haohaochexian.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://mga.zdbjq.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://gpf.xuetiantiany.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://aoy.jinghuilouyu.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://jqv.chenzaomai.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://vlo.feifeiyinyue.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://bms.mhx1999.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://yyo.52xcode.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://pgq.hnxiangtu.top

[B13] 判断是否为数字
来源：http://edb.ywan-chungtsiang.top

Py:   isinstance(x, (int, float))
来源：http://nsw.aibaodan.cn

PHP:  is_numeric($x)
来源：http://cpf.hesvh.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ysg.shzxlz.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vqb.redwolf501.top

Java: x instanceof Number
来源：http://phl.zdqjudy.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://zmk.nanxinkj.top

Ruby: x.is_a?(Numeric)
来源：http://mca.cashguo.top

C#:   x is int or double or decimal
来源：http://jyi.quarkkingdee.top

[B14] 判断值是否在集合内
来源：http://nyk.tarul.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://qck.zhaomingkeji.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://van.havefunace.top

JS:   [1, 2, 3].includes(x)
来源：http://thd.yongpay.top

TS:   [1, 2, 3].includes(x)
来源：http://cpu.xuanzx.com

Java: List.of(1, 2, 3).contains(x)
来源：http://olj.guannengcc.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://yua.316326.xyz

Ruby: [1, 2, 3].include?(x)
来源：http://yft.tanke756.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://tpn.kuanghao11.cn

[B15] 布尔运算与取反
来源：http://xog.svipenyu.cn

Py:   a and b or not c
来源：http://vmq.yj20258888.top

PHP:  $a && $b || !$c
来源：http://ngn.cheryme.top

JS:   a && b || !c
来源：http://dfz.9152youxi.cn

TS:   a && b || !c
来源：http://yxh.quarkkingdee.top

Java: a && b || !c
来源：http://nzs.xingfuxueyuan.xyz

Go:   a && b || !c
来源：http://bdf.jinyuanbaomall.cn

Ruby: a && b || !c
来源：http://syf.guowangkeji.top

C#:   a && b || !c
来源：http://iyi.nanxinkj.top

[B16] 卫语句：不满足条件提前返回
来源：http://amb.cdnleiting.top

Py:   if not data: return
来源：http://vdj.pengpengdd.cyou

PHP:  if (!$data) { return; }
来源：http://juh.hcnkem.com

JS:   if (!data) return;
来源：http://meb.cashguo.top

TS:   if (!data) return;
来源：http://atx.hysaishi.cn

Java: if (data == null) return;
来源：http://ssj.zhiwuduotai.top

Go:   if data == nil { return }
来源：http://nvl.birdmap.top

Ruby: return if data.nil?
来源：http://crl.tarul.cn

C#:   if (data == null) return;
来源：http://dfg.zdbjq.cn

================================================================================
来源：http://yny.sjlbkw.cn

C. 函数与作用域
来源：http://oce.guowangkeji.top

================================================================================
来源：http://gkm.chenlongwang.top

[C01] 定义函数
来源：http://soy.jyoumei.cn

Py:   def add(a, b): return a + b
来源：http://yvw.sysykeji.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cdz.zhoulong.xyz

JS:   function add(a, b) { return a + b; }
来源：http://grz.hnxiangtu.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tlv.ppjwa.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://mux.yonumen.top

Go:   func add(a, b int) int { return a + b }
来源：http://mtt.ivvv.top

Ruby: def add(a, b); a + b; end
来源：http://czs.gzhubu.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ysc.snrcjt.cn

[C02] 默认参数
来源：http://zws.jiagoushi.top

Py:   def greet(name="World"): return name
来源：http://bki.fktsv.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://qlx.jqgufenzy.top

JS:   function greet(name = "World") { return name; }
来源：http://mth.jinghuilouyu.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://jmx.guannengcc.top

Java: // 无默认参数：方法重载或 Optional
来源：http://cpg.pycfn.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://xel.nanxuanxn.top

Ruby: def greet(name = "World") = name
来源：http://hvy.birdmap.top

C#:   string Greet(string name = "World") => name;
来源：http://zly.yuanzhike.top

[C03] 可变参数
来源：http://rff.yuxming.cn

Py:   def total(*args): return sum(args)
来源：http://ccb.redwolf501.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://riz.hongshengwenyu.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://rov.yj202588.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://otn.tanke756.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://zmj.guannengcc.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://bkn.bbcook.cn

Ruby: def total(*nums); nums.sum; end
来源：http://sig.kuanghao11.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://xvy.jlsjyb.cn

[C04] 命名参数 / 关键字参数
来源：http://ais.svipenyu.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://bfm.daxiang520.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://fgz.hnxiangtu.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ixh.zhengqikj.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ofn.52xcode.cn

Java: // 无：用 Builder 模式或 record
来源：http://iuw.zdbjq.cn

Go:   // 无：用配置结构体参数
来源：http://ula.sweek.top

Ruby: f(a: 1, b: 2)
来源：http://xui.ywan-chungtsiang.top

C#:   f(a: 1, b: 2)
来源：http://cmc.epnwcf.com

[C05] 返回多个值
来源：http://xzb.jinghuilouyu.cn

Py:   return a, b
来源：http://gjg.cheryme.top

PHP:  return [$a, $b];
来源：http://smd.dashuyun.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://lxy.fktsv.cn

TS:   return { a, b };
来源：http://zzr.jyoumei.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://bfz.jinqigufen.top

Go:   return a, b
来源：http://wru.yueranfly.top

Ruby: return a, b
来源：http://krd.epnwcf.com

C#:   return (a, b);              // ValueTuple
来源：http://krx.zdqjudy.top

[C06] 匿名函数 / lambda
来源：http://qbw.zhiwuduotai.top

Py:   square = lambda x: x * x
来源：http://nve.svipenyu.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://bno.hcnkem.com

JS:   const square = x => x * x;
来源：http://xuu.jqgufenzy.top

TS:   const square = (x: number): number => x * x;
来源：http://rbn.jinghuilouyu.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ghp.tianlin.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://fvh.52xcode.cn

Ruby: square = ->(x) { x * x }
来源：http://lor.zhijiandao.cn

C#:   Func<int, int> square = x => x * x;
来源：http://gvv.yangfankeji.com

[C07] 把函数作为参数传入
来源：http://jim.fktsv.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://tmz.zhixingplan.top

PHP:  array_map("strtoupper", $arr);
来源：http://kgi.tanke756.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://cvq.ydjk.org.cn

TS:   arr.map(String)
来源：http://pke.ybcxt.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://jsn.wangshuangyany.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://uhk.yueranfly.top

Ruby: arr.map(&:upcase)
来源：http://cul.ctjpmb.com

C#:   arr.Select(s => s.ToUpper())
来源：http://fis.jqgufenzy.top

[C08] 闭包
来源：http://web.xuanzx.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://yct.bbcook.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://vbg.zhongyouzk.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://xni.daxiang520.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://fep.gogol.net.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://bmt.gogol.net.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://rtd.zhengqikj.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://fgq.zdqjudy.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://kpy.shanyushiyangtech.top

[C09] 递归
来源：http://ucd.0kj1m.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://dqp.aizwys.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://bdl.yuanzhike.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://odw.xinyue.icu

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ulw.redwolf501.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://dqa.birdmap.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://uhj.shangyingyoupin.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://uqk.zhaomingkeji.xyz

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://zvj.hysaishi.cn

[C10] 变量作用域
来源：http://dat.jiagoushi.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://obr.yueranfly.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://fwr.kuanghao11.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://bkc.chenlongwang.top

TS:   同 JS
来源：http://ika.vqdsnc.cn

Java: 方法内为块级作用域
来源：http://rpq.ywan-chungtsiang.top

Go:   花括号块级作用域
来源：http://qbv.yuanzhike.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://qfr.sysykeji.top

C#:   块级作用域
来源：http://zkw.chenjidiqi.icu

[C11] 模块导入与导出
来源：http://qhm.jiagoushi.top

Py:   from module import func
来源：http://cux.ehwqpu.com

PHP:  require "file.php";  或 use App\Service;
来源：http://xjb.cucudq.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://obq.hcnkem.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://fkd.hysaishi.cn

Java: import java.util.List;
来源：http://jsn.jqgufenzy.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://zrl.smart0.xyz

Ruby: require "json"; require_relative "./util"
来源：http://btq.jqgufenzy.top

C#:   using System.Text;
来源：http://utb.nanxuanxn.top

[C12] 立即执行函数 IIFE
来源：http://iso.jianghu66.top

Py:   (lambda: print("run"))()
来源：http://mqz.ybcxt.top

PHP:  (function () { echo "run"; })();
来源：http://snu.guowangkeji.top

JS:   (() => { console.log("run"); })();
来源：http://ohy.wangshuangyany.cn

TS:   (() => { console.log("run"); })();
来源：http://gyn.fzhhl.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ntb.yueranfly.top

Go:   func() { fmt.Println("run") }()
来源：http://dom.fengsongda.top

Ruby: -> { puts "run" }.call
来源：http://pju.jinyuanbaomall.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://sqj.shangyingyoupin.top

[C13] 类型声明 / 类型注解
来源：http://lqg.yuanzhike.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://pxy.zhijiandao.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rrp.yongpay.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://pef.zhoulong.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tnx.yongpay.top

Java: int add(int a, int b) { return a + b; }
来源：http://pgb.ydzc1.top

Go:   func add(a, b int) int
来源：http://sgt.nanxinkj.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://npj.yongpay.top

C#:   int Add(int a, int b) => a + b;
来源：http://soe.fanxiaobao.xyz

[C14] 泛型函数
来源：http://ubh.kuanghao11.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://tsv.zhijiandao.cn

PHP:  // 无泛型
来源：http://yyb.hesvh.cn

JS:   // 无泛型
来源：http://xst.quarkkingdee.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://sje.xuetiantiany.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://zgo.xingfuxueyuan.xyz

Go:   func First[T any](items []T) T { return items[0] }
来源：http://swo.svipenyu.cn

Ruby: # 无泛型
来源：http://oim.nanxinkj.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://abt.birdmap.top

[C15] 解构 / 展开参数
来源：http://vor.jianghu66.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mng.jyoumei.cn

PHP:  [$a, $b] = $pair;
来源：http://jhx.ydzc1.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xlz.bjfxy.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://pxb.tian-w.cn

Java: // 无解构
来源：http://fbk.hnqzz.top

Go:   // 无解构
来源：http://tix.daxiang520.top

Ruby: a, b = pair
来源：http://pdm.hywenlv.cn

C#:   var (a, b) = pair;
来源：http://tjo.quarkkingdee.top

[C16] 函数 / 方法重载
来源：http://yda.daria6918.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wgm.xylfe.cn

PHP:  // 无重载
来源：http://qqp.jqgfzy.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://ver.ppjwa.cn

TS:   // 用联合类型或重载签名声明
来源：http://noq.tarul.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://owa.birdmap.top

Go:   // 无重载：用不同函数名
来源：http://jbq.zhiwuduotai.top

Ruby: # 无重载：靠动态参数
来源：http://hgq.hammf.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://apd.uphjek.com

================================================================================
来源：http://ore.zhoulong.xyz

D. 数组 / 列表 / 集合
来源：http://olk.sjlbkw.cn

================================================================================
来源：http://nac.daria6918.cn

[D01] 创建数组 / 列表
来源：http://wnf.redwolf501.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://ljg.vehdjk.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ilo.ydzc1.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://iqt.yangfankeji.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://zdd.andypj.xyz

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://qev.cheryme.top

Go:   arr := []int{1, 2, 3}
来源：http://bwq.yonumen.top

Ruby: arr = [1, 2, 3]
来源：http://yds.cashguo.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://cyf.quarkkingdee.top

[D02] 追加元素到末尾
来源：http://vtq.gaohongyu789.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://jey.zhiwuduotai.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ytg.yueranfly.top

JS:   arr.push(4);
来源：http://cci.ctjpmb.com

TS:   arr.push(4);
来源：http://wuv.hnqzz.top

Java: list.add(4);
来源：http://wou.yfazqb.com

Go:   arr = append(arr, 4)
来源：http://xjz.shanyushiyangtech.top

Ruby: arr << 4; arr.push(5)
来源：http://toj.yueranfly.top

C#:   list.Add(4);
来源：http://vws.haohaochexian.top

[D03] 在指定位置插入元素
来源：http://hew.bjfxy.top

Py:   arr.insert(0, 0)
来源：http://fda.chenzaomai.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://vzq.cheryme.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hap.9152youxi.cn

TS:   arr.splice(0, 0, 0);
来源：http://xyk.xuetiantiany.cn

Java: list.add(0, 0);
来源：http://weh.yj20258.top

Go:   arr = append([]int{0}, arr...)
来源：http://isw.xziqi.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://dko.iojbl.cn

C#:   list.Insert(0, 0);
来源：http://ehn.vqdsnc.cn

[D04] 删除元素
来源：http://gqb.yj202588.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://rew.tian-w.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://urx.kuanghao11.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://sop.chenlongwang.top

TS:   arr.splice(0, 1);
来源：http://fcx.zhijiandao.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ijp.aibaodan.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://rec.vehdjk.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://tct.havefunace.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://usa.gzhubu.top

[D05] 访问与修改元素
来源：http://gah.cucudq.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://epl.nwbrower.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://oba.ydjk.org.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://znk.ybcxt.top

TS:   arr[0]; arr.at(-1);
来源：http://oeo.fehbvm.com

Java: list.get(0); list.set(0, 9);
来源：http://dyq.zhiwuduotai.top

Go:   arr[0]; arr[0] = 9
来源：http://mkj.gogol.net.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://uxw.aizwys.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://lgt.zhongyouzk.top

[D06] 数组长度
来源：http://xiq.smart0.xyz

Py:   len(arr)
来源：http://shk.gaohongyu789.top

PHP:  count($arr);
来源：http://bvs.9152youxi.cn

JS:   arr.length
来源：http://vjh.tarul.cn

TS:   arr.length
来源：http://jmu.ctjpmb.com

Java: list.size();
来源：http://tbv.sufxvd.cn

Go:   len(arr)
来源：http://syx.yanxiufei.cn

Ruby: arr.length; arr.size
来源：http://vrq.jinghuilouyu.cn

C#:   list.Count;
来源：http://btl.andypj.xyz

[D07] 切片 / 取子数组
来源：http://ekh.bjfxy.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://aqx.xziqi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://cpa.shuidangran.top

JS:   arr.slice(1, 4);
来源：http://gbm.zhoulong.xyz

TS:   arr.slice(1, 4);
来源：http://hyk.jinqigufen.top

Java: list.subList(1, 4);
来源：http://vwj.zhoulong.xyz

Go:   arr[1:4]
来源：http://cvf.jqgufenzy.top

Ruby: arr[1, 3]
来源：http://dak.meibo888.top

C#:   list.GetRange(1, 3);
来源：http://dsc.0kj1m.cn

[D08] 合并两个数组
来源：http://chp.havefunace.top

Py:   a + b;  a.extend(b)
来源：http://vtl.yueranfly.top

PHP:  array_merge($a, $b);
来源：http://ysp.cqqwz.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://myl.dashuyun.cn

TS:   [...a, ...b];
来源：http://afa.zdqjudy.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://jce.meibo888.top

Go:   append(a, b...)
来源：http://mbz.52xcode.cn

Ruby: a + b;  a.concat(b)
来源：http://oxp.cashguo.top

C#:   a.Concat(b).ToList()
来源：http://haj.yj20258888.top

[D09] 排序（升序）
来源：http://djm.iojbl.cn

Py:   sorted(arr);  arr.sort()
来源：http://cul.jinyuanbaomall.cn


<!-- 参考信息 -->