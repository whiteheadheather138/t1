代发 wailian999

[B09] break 与 continue
来源：http://vjk.fengsongda.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://bxi.xuanzx.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://cgm.wangshuangyany.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://chw.yuanzhike.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yno.jqgufenzy.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dol.jqgufenzy.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ftr.uphjek.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hcd.tian-w.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kra.shanyushiyangtech.top

[B10] 遍历同时拿索引
来源：http://dco.ctjpmb.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://sml.chenjidiqi.icu

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://eny.ctjpmb.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://qjz.bjfxy.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://tsz.feifeiyinyue.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://kzl.dianchejie.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://gwd.zycfv.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://jue.yvedp.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://bce.tarul.cn

[B11] 生成数字序列 / 区间
来源：http://kwd.hcnkem.com

Py:   list(range(0, 10, 2))
来源：http://gxj.nanxinkj.top

PHP:  range(0, 10, 2);
来源：http://wjb.pengpengdd.cyou

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rdi.ydjk.org.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bie.andypj.xyz

Java: IntStream.range(0, 10).boxed().toList()
来源：http://pgd.jlsjyb.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://scc.sjlbkw.cn

Ruby: (0...10).step(2).to_a
来源：http://jmu.guannengcc.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://won.xingfuxueyuan.xyz

[B12] 跳出多层循环
来源：http://pav.zycfv.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://roq.hnxiangtu.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://lfu.snrcjt.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://xhq.shanyushiyangkeji.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ykb.cashguo.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ioh.iojbl.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wbn.hfpthk.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://nyp.jiagoushi.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://oqt.chenzaomai.com

[B13] 判断是否为数字
来源：http://dro.pycfn.com

Py:   isinstance(x, (int, float))
来源：http://lin.svipenyu.cn

PHP:  is_numeric($x)
来源：http://plx.nanxuanxn.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rkp.zhijiandao.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vyo.gogol.net.cn

Java: x instanceof Number
来源：http://ujz.xingfuxueyuan.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ood.sysykeji.top

Ruby: x.is_a?(Numeric)
来源：http://udj.tian-w.cn

C#:   x is int or double or decimal
来源：http://ibx.yj20258888.top

[B14] 判断值是否在集合内
来源：http://wrl.zdbjq.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://gli.shanyushiyangtech.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://iey.xuetiantiany.cn

JS:   [1, 2, 3].includes(x)
来源：http://yaz.jlsjyb.cn

TS:   [1, 2, 3].includes(x)
来源：http://lmt.gotoacloud.top

Java: List.of(1, 2, 3).contains(x)
来源：http://oiv.gogol.net.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://szp.jinyuanbaomall.cn

Ruby: [1, 2, 3].include?(x)
来源：http://uhf.zycfv.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://itm.havefunace.top

[B15] 布尔运算与取反
来源：http://glm.yanxiufei.cn

Py:   a and b or not c
来源：http://axh.ivvv.top

PHP:  $a && $b || !$c
来源：http://hth.tarul.cn

JS:   a && b || !c
来源：http://jdf.fktsv.cn

TS:   a && b || !c
来源：http://sls.chenlongwang.top

Java: a && b || !c
来源：http://ccv.xziqi.cn

Go:   a && b || !c
来源：http://vqg.ctjpmb.com

Ruby: a && b || !c
来源：http://ggp.c1oappe.top

C#:   a && b || !c
来源：http://hss.nanxuanxn.top

[B16] 卫语句：不满足条件提前返回
来源：http://ktq.yanxiufei.cn

Py:   if not data: return
来源：http://jcs.guowangkeji.top

PHP:  if (!$data) { return; }
来源：http://kii.hysaishi.cn

JS:   if (!data) return;
来源：http://rqm.yangfankeji.com

TS:   if (!data) return;
来源：http://tdg.yj20258.top

Java: if (data == null) return;
来源：http://vha.svipenyu.cn

Go:   if data == nil { return }
来源：http://fgj.bbcook.cn

Ruby: return if data.nil?
来源：http://ofe.jinghuilouyu.cn

C#:   if (data == null) return;
来源：http://sme.fanxiaobao.xyz

================================================================================
来源：http://xwx.yanxiufei.cn

C. 函数与作用域
来源：http://wdb.dianchejie.cn

================================================================================
来源：http://ssf.fengsongda.top

[C01] 定义函数
来源：http://kmy.pycfn.com

Py:   def add(a, b): return a + b
来源：http://hon.svipenyu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qrb.cdnleiting.top

JS:   function add(a, b) { return a + b; }
来源：http://uoo.guannengcc.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qos.daria6918.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://sud.jinqigfzy.top

Go:   func add(a, b int) int { return a + b }
来源：http://rbb.yangfankeji.com

Ruby: def add(a, b); a + b; end
来源：http://jyo.zhoulong.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://drk.hywenlv.cn

[C02] 默认参数
来源：http://amg.ctjpmb.com

Py:   def greet(name="World"): return name
来源：http://fox.gotoacloud.top

PHP:  function greet($name = "World") { return $name; }
来源：http://jfu.ywan-chungtsiang.top

JS:   function greet(name = "World") { return name; }
来源：http://hzh.sweek.top

TS:   function greet(name: string = "World") { return name; }
来源：http://kgr.zhengqikj.top

Java: // 无默认参数：方法重载或 Optional
来源：http://jhp.jqgufenzy.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://kzc.fanxiaobao.xyz

Ruby: def greet(name = "World") = name
来源：http://cbu.hesvh.cn

C#:   string Greet(string name = "World") => name;
来源：http://lcp.bbcook.cn

[C03] 可变参数
来源：http://chu.aibaodan.cn

Py:   def total(*args): return sum(args)
来源：http://fro.pengpengdd.cyou

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ebd.jinyuanbaomall.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://bnz.yj20258.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://lja.cheryme.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://nxe.sjlbkw.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://lpt.sufxvd.cn

Ruby: def total(*nums); nums.sum; end
来源：http://shd.pengpengdd.cyou

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://qxb.hesvh.cn

[C04] 命名参数 / 关键字参数
来源：http://bee.zhengqikj.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://nvb.hywenlv.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ymk.feifeiyinyue.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://kia.sweek.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://cgz.jyoumei.cn

Java: // 无：用 Builder 模式或 record
来源：http://tkv.hongshengwenyu.top

Go:   // 无：用配置结构体参数
来源：http://bet.fengsongda.top

Ruby: f(a: 1, b: 2)
来源：http://fja.snrcjt.cn

C#:   f(a: 1, b: 2)
来源：http://ixf.xziqi.cn

[C05] 返回多个值
来源：http://ird.nanxinkj.top

Py:   return a, b
来源：http://vac.fktsv.cn

PHP:  return [$a, $b];
来源：http://grc.yfazqb.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://ome.yanxiufei.cn

TS:   return { a, b };
来源：http://rie.ybcxt.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://slq.zhijiandao.cn

Go:   return a, b
来源：http://zma.xylfe.cn

Ruby: return a, b
来源：http://xds.haohaochexian.top

C#:   return (a, b);              // ValueTuple
来源：http://bui.tian-w.cn

[C06] 匿名函数 / lambda
来源：http://tbt.yj202588.top

Py:   square = lambda x: x * x
来源：http://odn.daria6918.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ydl.shangyingyoupin.top

JS:   const square = x => x * x;
来源：http://clt.tian-w.cn

TS:   const square = (x: number): number => x * x;
来源：http://poy.chenlongwang.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ayk.shanyushiyangkeji.top

Go:   sq := func(x int) int { return x * x }
来源：http://tzw.wangshuangyany.cn

Ruby: square = ->(x) { x * x }
来源：http://mhi.hammf.cn

C#:   Func<int, int> square = x => x * x;
来源：http://obu.zhoulong.xyz

[C07] 把函数作为参数传入
来源：http://xkm.shanyushiyangkeji.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://acb.sysykeji.top

PHP:  array_map("strtoupper", $arr);
来源：http://nyw.9152youxi.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://vrp.jinyuanbaomall.cn

TS:   arr.map(String)
来源：http://bcp.shanyushiyangtech.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://iyd.tarul.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://shj.bbcook.cn

Ruby: arr.map(&:upcase)
来源：http://bve.guannengcc.top

C#:   arr.Select(s => s.ToUpper())
来源：http://aeo.ctjpmb.com

[C08] 闭包
来源：http://sbx.haohaochexian.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qgz.xuetiantiany.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://zfk.yonumen.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qew.fanxiaobao.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://xpv.haohaochexian.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://cez.tian-w.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://kvm.ywan-chungtsiang.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://xvv.yangfankeji.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ouo.vehdjk.com

[C09] 递归
来源：http://mja.jyoumei.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ner.tarul.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ecz.sysykeji.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dof.xylfe.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uma.feifeiyinyue.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://dtx.shangyingyoupin.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://rgm.andypj.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://eqe.tanke756.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://dsd.hfpthk.cn

[C10] 变量作用域
来源：http://wer.yongpay.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://emw.pengpengdd.cyou

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://tml.iojbl.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ebz.sjlbkw.cn

TS:   同 JS
来源：http://ywy.aizwys.cn

Java: 方法内为块级作用域
来源：http://pqr.dashuyun.cn

Go:   花括号块级作用域
来源：http://uvo.hysaishi.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://qgk.ydzc1.top

C#:   块级作用域
来源：http://ekv.wangshuangyany.cn

[C11] 模块导入与导出
来源：http://owf.zdbjq.cn

Py:   from module import func
来源：http://nmw.hesvh.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://wlz.tianlin.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://jxb.cucudq.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://lqy.cqqwz.cn

Java: import java.util.List;
来源：http://rkc.ywan-chungtsiang.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mpz.zycfv.cn

Ruby: require "json"; require_relative "./util"
来源：http://zpn.wangdashe.top

C#:   using System.Text;
来源：http://hmj.ydjk.org.cn

[C12] 立即执行函数 IIFE
来源：http://wbr.jiagoushi.top

Py:   (lambda: print("run"))()
来源：http://mzk.hfpthk.cn

PHP:  (function () { echo "run"; })();
来源：http://xqs.mhx1999.top

JS:   (() => { console.log("run"); })();
来源：http://gfz.yueranfly.top

TS:   (() => { console.log("run"); })();
来源：http://kqx.fzhhl.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://tyg.fzhhl.top

Go:   func() { fmt.Println("run") }()
来源：http://ivy.ctjpmb.com

Ruby: -> { puts "run" }.call
来源：http://iso.zdqjudy.top

C#:   // 无 IIFE：用静态构造函数
来源：http://ian.yuanzhike.top

[C13] 类型声明 / 类型注解
来源：http://dsh.hammf.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://vkf.quarkkingdee.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dbg.sxryk.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://sis.hnqzz.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://irb.guowangkeji.top

Java: int add(int a, int b) { return a + b; }
来源：http://gil.fengsongda.top

Go:   func add(a, b int) int
来源：http://ozv.xziqi.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wjz.jinqigfzy.top

C#:   int Add(int a, int b) => a + b;
来源：http://byc.jinyuanbaomall.cn

[C14] 泛型函数
来源：http://rwd.cashguo.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://rcb.quarkkingdee.top

PHP:  // 无泛型
来源：http://ski.hongshengwenyu.top

JS:   // 无泛型
来源：http://jqs.feifeiyinyue.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://pre.gotoacloud.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://uhn.iojbl.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://khx.jinqigufen.top

Ruby: # 无泛型
来源：http://csg.52xcode.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://gnr.quarkkingdee.top

[C15] 解构 / 展开参数
来源：http://fsh.xinyue.icu

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://kph.52xcode.cn

PHP:  [$a, $b] = $pair;
来源：http://rzd.hcnkem.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xvs.jlsjyb.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://qtd.cheryme.top

Java: // 无解构
来源：http://djl.nanxinkj.top

Go:   // 无解构
来源：http://zjh.hfpthk.cn

Ruby: a, b = pair
来源：http://wck.hesvh.cn

C#:   var (a, b) = pair;
来源：http://dou.xingfuxueyuan.xyz

[C16] 函数 / 方法重载
来源：http://ykd.cashguo.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://nnc.xingfuxueyuan.xyz

PHP:  // 无重载
来源：http://mwy.chenjidiqi.icu

JS:   // 无重载：靠 arguments.length 分支
来源：http://ydj.jqgfzy.top

TS:   // 用联合类型或重载签名声明
来源：http://dwt.zhijiandao.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://toy.vehdjk.com

Go:   // 无重载：用不同函数名
来源：http://awo.xuanzx.com

Ruby: # 无重载：靠动态参数
来源：http://usj.0kj1m.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://shl.zdqjudy.top

================================================================================
来源：http://zxb.wangshuangyany.cn

D. 数组 / 列表 / 集合
来源：http://tah.yuanzhike.top

================================================================================
来源：http://jbf.dashuyun.cn

[D01] 创建数组 / 列表
来源：http://xvp.yj20258888.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://gpe.bjfxy.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://fgx.epnwcf.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mnc.jinqigufen.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://rvh.sysykeji.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://pau.dashuyun.cn

Go:   arr := []int{1, 2, 3}
来源：http://iof.gogol.net.cn

Ruby: arr = [1, 2, 3]
来源：http://lke.ydjk.org.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ezr.iojbl.cn

[D02] 追加元素到末尾
来源：http://zpn.hywenlv.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://jak.tianlin.xyz

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://cak.zhoulong.xyz

JS:   arr.push(4);
来源：http://bbo.zhiwuduotai.top

TS:   arr.push(4);
来源：http://dku.zhoulong.xyz

Java: list.add(4);
来源：http://ndv.mhx1999.top

Go:   arr = append(arr, 4)
来源：http://vfs.nanxuanxn.top

Ruby: arr << 4; arr.push(5)
来源：http://dmb.yongpay.top

C#:   list.Add(4);
来源：http://pvn.hnxiangtu.top

[D03] 在指定位置插入元素
来源：http://htl.shanyushiyangtech.top

Py:   arr.insert(0, 0)
来源：http://msv.jinyuanbaomall.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ury.daria6918.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://iri.xuanzx.com

TS:   arr.splice(0, 0, 0);
来源：http://xub.zdbjq.cn

Java: list.add(0, 0);
来源：http://hmp.ydzc1.top

Go:   arr = append([]int{0}, arr...)
来源：http://msm.ydjk.org.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://dsd.nanxuanxn.top

C#:   list.Insert(0, 0);
来源：http://gkr.cqqwz.cn

[D04] 删除元素
来源：http://zpb.xinyue.icu

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://tze.pycfn.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wtf.sufxvd.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ybi.cashguo.top

TS:   arr.splice(0, 1);
来源：http://obn.zhengqikj.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://xqq.xinyue.icu

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mvi.tanke756.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://izm.vqdsnc.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://qfz.fengsongda.top

[D05] 访问与修改元素
来源：http://aak.nanxuanxn.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://sku.fehbvm.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://szg.pengpengdd.cyou

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://vxo.uphjek.com

TS:   arr[0]; arr.at(-1);
来源：http://mug.dianchejie.cn

Java: list.get(0); list.set(0, 9);
来源：http://wne.ybcxt.top

Go:   arr[0]; arr[0] = 9
来源：http://yxb.haohaochexian.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://clg.xuetiantiany.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://usl.aizwys.cn

[D06] 数组长度
来源：http://osi.zhaomingkeji.xyz

Py:   len(arr)
来源：http://xop.daria6918.cn

PHP:  count($arr);
来源：http://wkw.jiagoushi.top

JS:   arr.length
来源：http://sta.svipenyu.cn

TS:   arr.length
来源：http://jmd.ydjk.org.cn

Java: list.size();
来源：http://pvo.guowangkeji.top

Go:   len(arr)
来源：http://jvg.vqdsnc.cn

Ruby: arr.length; arr.size
来源：http://lak.yj20258888.top

C#:   list.Count;
来源：http://ytx.cucudq.cn

[D07] 切片 / 取子数组
来源：http://qqw.jiagoushi.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hkn.vehdjk.com

PHP:  array_slice($arr, 1, 3);
来源：http://xav.zhongyouzk.top

JS:   arr.slice(1, 4);
来源：http://gux.wangshuangyany.cn

TS:   arr.slice(1, 4);
来源：http://gho.hesvh.cn

Java: list.subList(1, 4);
来源：http://eem.xinyue.icu

Go:   arr[1:4]
来源：http://noy.hongshengwenyu.top

Ruby: arr[1, 3]
来源：http://dug.meibo888.top

C#:   list.GetRange(1, 3);
来源：http://hky.zhoulong.xyz

[D08] 合并两个数组
来源：http://wrw.jinyuanbaomall.cn

Py:   a + b;  a.extend(b)
来源：http://fxo.gogol.net.cn

PHP:  array_merge($a, $b);
来源：http://ldi.epnwcf.com

JS:   [...a, ...b];  a.concat(b);
来源：http://mnz.shuidangran.top

TS:   [...a, ...b];
来源：http://skv.hywenlv.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wpm.shanyushiyangtech.top

Go:   append(a, b...)
来源：http://cpj.zhiwuduotai.top

Ruby: a + b;  a.concat(b)
来源：http://mcu.jinyuanbaomall.cn

C#:   a.Concat(b).ToList()
来源：http://ogf.jlsjyb.cn

[D09] 排序（升序）
来源：http://qbc.jiagoushi.top

Py:   sorted(arr);  arr.sort()
来源：http://wuh.jqgfzy.top

PHP:  sort($arr);
来源：http://vlo.yanxiufei.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ens.sweek.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://kqj.kuanghao11.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://tln.yvedp.cn


<!-- 参考信息 -->