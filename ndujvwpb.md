代发 wailian999

[B09] break 与 continue
来源：http://ixf.fktsv.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://sac.jqgfzy.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://lbf.ppjwa.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dkm.dianchejie.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gfw.gotoacloud.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fpt.dashuyun.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://tnm.iojbl.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://cyh.shuidangran.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dgy.fehbvm.com

[B10] 遍历同时拿索引
来源：http://grl.zhijiandao.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://awd.wangdashe.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://nic.svipenyu.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://jti.sjlbkw.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://nsp.svipenyu.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://muj.pengpengdd.cyou

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://znh.yongpay.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://sib.sxryk.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://yly.ywan-chungtsiang.top

[B11] 生成数字序列 / 区间
来源：http://snq.xuetiantiany.cn

Py:   list(range(0, 10, 2))
来源：http://yfp.gzhubu.top

PHP:  range(0, 10, 2);
来源：http://osa.iojbl.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ruj.jianghu66.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hyc.pengpengdd.cyou

Java: IntStream.range(0, 10).boxed().toList()
来源：http://cmu.meibo888.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://qhq.0kj1m.cn

Ruby: (0...10).step(2).to_a
来源：http://exz.ybcxt.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://qpi.jianghu66.top

[B12] 跳出多层循环
来源：http://nyh.fehbvm.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://ttn.shuidangran.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://jlh.nwbrower.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://pgz.cheryme.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hyr.shanyushiyangtech.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ddb.cdnleiting.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wsx.jyoumei.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://gof.daria6918.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://abe.hammf.cn

[B13] 判断是否为数字
来源：http://suo.chenjidiqi.icu

Py:   isinstance(x, (int, float))
来源：http://pbk.smart0.xyz

PHP:  is_numeric($x)
来源：http://owx.ywan-chungtsiang.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zdm.aizwys.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://oqy.aibaodan.cn

Java: x instanceof Number
来源：http://fgu.wangshuangyany.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wqx.daria6918.cn

Ruby: x.is_a?(Numeric)
来源：http://fqq.jianghu66.top

C#:   x is int or double or decimal
来源：http://tum.sysykeji.top

[B14] 判断值是否在集合内
来源：http://brm.shanyushiyangkeji.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ypf.haohaochexian.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://oaz.jinghuilouyu.cn

JS:   [1, 2, 3].includes(x)
来源：http://rvp.hnxiangtu.top

TS:   [1, 2, 3].includes(x)
来源：http://apn.hesvh.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://zss.sysykeji.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://cqi.snrcjt.cn

Ruby: [1, 2, 3].include?(x)
来源：http://uvv.yuanzhike.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://rbh.yonumen.top

[B15] 布尔运算与取反
来源：http://raz.ehwqpu.com

Py:   a and b or not c
来源：http://zit.vehdjk.com

PHP:  $a && $b || !$c
来源：http://jtj.cdnleiting.top

JS:   a && b || !c
来源：http://tqj.zhaomingkeji.xyz

TS:   a && b || !c
来源：http://qly.yvedp.cn

Java: a && b || !c
来源：http://bzt.kuanghao11.cn

Go:   a && b || !c
来源：http://rvb.hongshengwenyu.top

Ruby: a && b || !c
来源：http://cln.ppjwa.cn

C#:   a && b || !c
来源：http://hgb.hesvh.cn

[B16] 卫语句：不满足条件提前返回
来源：http://xwp.ppjwa.cn

Py:   if not data: return
来源：http://ivo.yvedp.cn

PHP:  if (!$data) { return; }
来源：http://pom.vqdsnc.cn

JS:   if (!data) return;
来源：http://fvi.zhoulong.xyz

TS:   if (!data) return;
来源：http://xxj.tanke756.top

Java: if (data == null) return;
来源：http://zem.zhijiandao.cn

Go:   if data == nil { return }
来源：http://tuy.fzhhl.top

Ruby: return if data.nil?
来源：http://dyq.iojbl.cn

C#:   if (data == null) return;
来源：http://fos.fktsv.cn

================================================================================
来源：http://raw.sjlbkw.cn

C. 函数与作用域
来源：http://egc.bbcook.cn

================================================================================
来源：http://dqp.shangyingyoupin.top

[C01] 定义函数
来源：http://ati.uphjek.com

Py:   def add(a, b): return a + b
来源：http://xej.feifeiyinyue.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jab.ppjwa.cn

JS:   function add(a, b) { return a + b; }
来源：http://aey.xylfe.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qen.smart0.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://shf.ivvv.top

Go:   func add(a, b int) int { return a + b }
来源：http://zmf.cheryme.top

Ruby: def add(a, b); a + b; end
来源：http://skm.zhijiandao.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://fwl.zhixingplan.top

[C02] 默认参数
来源：http://eyj.pycfn.com

Py:   def greet(name="World"): return name
来源：http://zrb.shzxlz.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://rzg.yuanzhike.top

JS:   function greet(name = "World") { return name; }
来源：http://cdy.zhiwuduotai.top

TS:   function greet(name: string = "World") { return name; }
来源：http://oyg.jqgfzy.top

Java: // 无默认参数：方法重载或 Optional
来源：http://evs.iojbl.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://plq.iojbl.cn

Ruby: def greet(name = "World") = name
来源：http://jfh.meibo888.top

C#:   string Greet(string name = "World") => name;
来源：http://pul.uphjek.com

[C03] 可变参数
来源：http://lvc.chenzaomai.com

Py:   def total(*args): return sum(args)
来源：http://bbn.meibo888.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://doc.chenlongwang.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://plu.sysykeji.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://kjm.redwolf501.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://lzo.xinyue.icu

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://zvo.hysaishi.cn

Ruby: def total(*nums); nums.sum; end
来源：http://zku.jinqigufen.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://yfm.dashuyun.cn

[C04] 命名参数 / 关键字参数
来源：http://pyq.yvedp.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ufc.birdmap.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://qak.ydzc1.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://snk.hysaishi.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://crv.haohaochexian.top

Java: // 无：用 Builder 模式或 record
来源：http://wee.zhijiandao.cn

Go:   // 无：用配置结构体参数
来源：http://jnv.0kj1m.cn

Ruby: f(a: 1, b: 2)
来源：http://ahx.sjlbkw.cn

C#:   f(a: 1, b: 2)
来源：http://lod.xinyue.icu

[C05] 返回多个值
来源：http://rfz.shuidangran.top

Py:   return a, b
来源：http://adn.yj20258888.top

PHP:  return [$a, $b];
来源：http://eql.wangshuangyany.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://eiu.gotoacloud.top

TS:   return { a, b };
来源：http://ddt.ybcxt.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://abo.epnwcf.com

Go:   return a, b
来源：http://xyi.nanxuanxn.top

Ruby: return a, b
来源：http://bdz.guannengcc.top

C#:   return (a, b);              // ValueTuple
来源：http://mdy.jlsjyb.cn

[C06] 匿名函数 / lambda
来源：http://bzq.wangdashe.top

Py:   square = lambda x: x * x
来源：http://gtz.ppjwa.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://bli.nwbrower.top

JS:   const square = x => x * x;
来源：http://rhh.zhixingplan.top

TS:   const square = (x: number): number => x * x;
来源：http://jei.dashuyun.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://rug.hysaishi.cn

Go:   sq := func(x int) int { return x * x }
来源：http://paj.cheryme.top

Ruby: square = ->(x) { x * x }
来源：http://dfg.tianlin.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://mkc.svipenyu.cn

[C07] 把函数作为参数传入
来源：http://soz.kuanghao11.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://cim.zhijiandao.cn

PHP:  array_map("strtoupper", $arr);
来源：http://uws.meibo888.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://fgg.hnxiangtu.top

TS:   arr.map(String)
来源：http://eww.cheryme.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hlv.shzxlz.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://yyd.zhixingplan.top

Ruby: arr.map(&:upcase)
来源：http://epo.jinghuilouyu.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://yko.tanke756.top

[C08] 闭包
来源：http://jby.shzxlz.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://xkd.cqqwz.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hhh.hesvh.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://uqw.yanxiufei.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://fxp.chenlongwang.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ubi.yanxiufei.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://tql.daria6918.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://rex.bjfxy.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://uke.zdbjq.cn

[C09] 递归
来源：http://ocq.nwbrower.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://kvc.yj20258.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://fxf.c1oappe.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mrp.fehbvm.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ntd.yonumen.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://tmc.nanxinkj.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://csm.havefunace.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://gmc.cashguo.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://zlq.fanxiaobao.xyz

[C10] 变量作用域
来源：http://ayc.hcnkem.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://dux.aibaodan.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://azg.ivvv.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mdm.tanke756.top

TS:   同 JS
来源：http://tbj.gzhubu.top

Java: 方法内为块级作用域
来源：http://kmj.ctjpmb.com

Go:   花括号块级作用域
来源：http://xwg.sxryk.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://rbp.vehdjk.com

C#:   块级作用域
来源：http://dyi.jinghuilouyu.cn

[C11] 模块导入与导出
来源：http://ror.gogol.net.cn

Py:   from module import func
来源：http://wah.pycfn.com

PHP:  require "file.php";  或 use App\Service;
来源：http://fdf.hnqzz.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://urt.cucudq.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://eoi.zhixingplan.top

Java: import java.util.List;
来源：http://cwx.cheryme.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://avb.gogol.net.cn

Ruby: require "json"; require_relative "./util"
来源：http://ouu.yj202588.top

C#:   using System.Text;
来源：http://tss.havefunace.top

[C12] 立即执行函数 IIFE
来源：http://wfd.gotoacloud.top

Py:   (lambda: print("run"))()
来源：http://obj.aizwys.cn

PHP:  (function () { echo "run"; })();
来源：http://zzl.wangshuangyany.cn

JS:   (() => { console.log("run"); })();
来源：http://vix.aibaodan.cn

TS:   (() => { console.log("run"); })();
来源：http://mgl.haohaochexian.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://tyr.nanxuanxn.top

Go:   func() { fmt.Println("run") }()
来源：http://njz.zhixingplan.top

Ruby: -> { puts "run" }.call
来源：http://jxy.tian-w.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://qyh.chenlongwang.top

[C13] 类型声明 / 类型注解
来源：http://zjl.wangshuangyany.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://sac.aibaodan.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vus.ctjpmb.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://bme.jyoumei.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fji.gogol.net.cn

Java: int add(int a, int b) { return a + b; }
来源：http://vub.pycfn.com

Go:   func add(a, b int) int
来源：http://mbp.hesvh.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://xms.epnwcf.com

C#:   int Add(int a, int b) => a + b;
来源：http://zjt.pengpengdd.cyou

[C14] 泛型函数
来源：http://esi.jinyuanbaomall.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://njo.hysaishi.cn

PHP:  // 无泛型
来源：http://way.yvedp.cn

JS:   // 无泛型
来源：http://dvz.xingfuxueyuan.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ajw.yj20258888.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://bhk.fzhhl.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ykh.gzhubu.top

Ruby: # 无泛型
来源：http://lve.xinyue.icu

C#:   static T First<T>(List<T> items) => items[0];
来源：http://msu.gzhubu.top

[C15] 解构 / 展开参数
来源：http://unj.aibaodan.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://rwf.guannengcc.top

PHP:  [$a, $b] = $pair;
来源：http://pct.zdbjq.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://dzo.zhoulong.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://woi.epnwcf.com

Java: // 无解构
来源：http://iyy.hnqzz.top

Go:   // 无解构
来源：http://wwa.fktsv.cn

Ruby: a, b = pair
来源：http://iwm.yonumen.top

C#:   var (a, b) = pair;
来源：http://nqx.jinghuilouyu.cn

[C16] 函数 / 方法重载
来源：http://wvs.chenzaomai.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://thu.xziqi.cn

PHP:  // 无重载
来源：http://xqx.shanyushiyangtech.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://ant.dashuyun.cn

TS:   // 用联合类型或重载签名声明
来源：http://cge.zhixingplan.top

Java: void f(int a) {}  void f(String a) {}
来源：http://luy.mhx1999.top

Go:   // 无重载：用不同函数名
来源：http://ddh.yueranfly.top

Ruby: # 无重载：靠动态参数
来源：http://ghl.yuxming.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://bts.ywan-chungtsiang.top

================================================================================
来源：http://hci.sufxvd.cn

D. 数组 / 列表 / 集合
来源：http://xby.ppjwa.cn

================================================================================
来源：http://iax.tian-w.cn

[D01] 创建数组 / 列表
来源：http://wos.ivvv.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://yxv.aibaodan.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://zwj.shanyushiyangkeji.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://uty.ydjk.org.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://kps.yj20258888.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ylz.pycfn.com

Go:   arr := []int{1, 2, 3}
来源：http://arl.gaohongyu789.top

Ruby: arr = [1, 2, 3]
来源：http://ily.316326.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://zxl.yueranfly.top

[D02] 追加元素到末尾
来源：http://rcl.svipenyu.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://yuw.sysykeji.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://xjf.shuidangran.top

JS:   arr.push(4);
来源：http://txd.jinqigufen.top

TS:   arr.push(4);
来源：http://xnv.cashguo.top

Java: list.add(4);
来源：http://ajv.ehwqpu.com

Go:   arr = append(arr, 4)
来源：http://lhl.cdnleiting.top

Ruby: arr << 4; arr.push(5)
来源：http://vzs.zhijiandao.cn

C#:   list.Add(4);
来源：http://vkj.zdqjudy.top

[D03] 在指定位置插入元素
来源：http://wmg.gotoacloud.top

Py:   arr.insert(0, 0)
来源：http://lvb.zhiwuduotai.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://fdp.fanxiaobao.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://fpx.0kj1m.cn

TS:   arr.splice(0, 0, 0);
来源：http://anc.cucudq.cn

Java: list.add(0, 0);
来源：http://mvj.ehwqpu.com

Go:   arr = append([]int{0}, arr...)
来源：http://ygy.yj20258.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://csf.xuetiantiany.cn

C#:   list.Insert(0, 0);
来源：http://odp.aibaodan.cn

[D04] 删除元素
来源：http://ypg.yj20258888.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ogo.zhixingplan.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://rar.fengsongda.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wpq.jinqigfzy.top

TS:   arr.splice(0, 1);
来源：http://huf.hammf.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://jtj.fehbvm.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://gii.bjfxy.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://znf.yj20258888.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://jqc.wangdashe.top

[D05] 访问与修改元素
来源：http://cor.sysykeji.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://qci.shzxlz.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://zfj.yonumen.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://cog.fengsongda.top

TS:   arr[0]; arr.at(-1);
来源：http://hni.fktsv.cn

Java: list.get(0); list.set(0, 9);
来源：http://lxm.yanxiufei.cn

Go:   arr[0]; arr[0] = 9
来源：http://mvu.jianghu66.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://rmb.daxiang520.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://npi.52xcode.cn

[D06] 数组长度
来源：http://bvx.yfazqb.com

Py:   len(arr)
来源：http://wxz.cucudq.cn

PHP:  count($arr);
来源：http://edv.yfazqb.com

JS:   arr.length
来源：http://sjm.ydzc1.top

TS:   arr.length
来源：http://lkh.hesvh.cn

Java: list.size();
来源：http://lko.zhongyouzk.top

Go:   len(arr)
来源：http://bzy.gaohongyu789.top

Ruby: arr.length; arr.size
来源：http://jiz.yj20258888.top

C#:   list.Count;
来源：http://zah.yueranfly.top

[D07] 切片 / 取子数组
来源：http://twh.chenlongwang.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://nzt.wangshuangyany.cn

PHP:  array_slice($arr, 1, 3);
来源：http://dhu.snrcjt.cn

JS:   arr.slice(1, 4);
来源：http://dfe.shzxlz.cn

TS:   arr.slice(1, 4);
来源：http://aaz.yueranfly.top

Java: list.subList(1, 4);
来源：http://ika.shanyushiyangtech.top

Go:   arr[1:4]
来源：http://kuk.xingfuxueyuan.xyz

Ruby: arr[1, 3]
来源：http://abn.jianghu66.top

C#:   list.GetRange(1, 3);
来源：http://kyf.hongshengwenyu.top

[D08] 合并两个数组
来源：http://tha.jqgufenzy.top

Py:   a + b;  a.extend(b)
来源：http://tml.cheryme.top

PHP:  array_merge($a, $b);
来源：http://tky.gaohongyu789.top

JS:   [...a, ...b];  a.concat(b);
来源：http://env.quarkkingdee.top

TS:   [...a, ...b];
来源：http://bfs.fengsongda.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://zup.ydzc1.top

Go:   append(a, b...)
来源：http://rxy.jiagoushi.top

Ruby: a + b;  a.concat(b)
来源：http://zbr.uphjek.com

C#:   a.Concat(b).ToList()
来源：http://xhw.yvedp.cn

[D09] 排序（升序）
来源：http://zke.aizwys.cn

Py:   sorted(arr);  arr.sort()
来源：http://rwc.yuxming.cn

PHP:  sort($arr);
来源：http://xni.gogol.net.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://bmx.ybcxt.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://hol.fengsongda.top

Java: Collections.sort(list);  list.sort(null);
来源：http://lpm.cashguo.top


<!-- 参考信息 -->