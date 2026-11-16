代发 wailian999

[B09] break 与 continue
来源：http://uwb.ywan-chungtsiang.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://tzc.quarkkingdee.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://kyi.hywenlv.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://avl.yvedp.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ell.9152youxi.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dbl.andypj.xyz

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://izk.jinghuilouyu.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xue.vehdjk.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ikt.ctjpmb.com

[B10] 遍历同时拿索引
来源：http://ckh.zhengqikj.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://cll.ehwqpu.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://tro.yuanzhike.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xqn.xinyue.icu

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://qei.zhengqikj.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ynh.9152youxi.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://too.uphjek.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://fke.hywenlv.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://sjp.nwbrower.top

[B11] 生成数字序列 / 区间
来源：http://ikv.dashuyun.cn

Py:   list(range(0, 10, 2))
来源：http://tfm.gogol.net.cn

PHP:  range(0, 10, 2);
来源：http://dos.sxryk.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vow.xziqi.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fvh.c1oappe.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://drn.c1oappe.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://zun.hammf.cn

Ruby: (0...10).step(2).to_a
来源：http://tvb.cashguo.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://qnm.yanxiufei.cn

[B12] 跳出多层循环
来源：http://ota.jinyuanbaomall.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://efx.yuanzhike.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://juu.cheryme.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ctl.jlsjyb.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://qht.zycfv.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://igj.zdqjudy.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://fga.jinghuilouyu.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://kyx.yj20258888.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://kzd.tanke756.top

[B13] 判断是否为数字
来源：http://wvt.jianghu66.top

Py:   isinstance(x, (int, float))
来源：http://rln.sufxvd.cn

PHP:  is_numeric($x)
来源：http://tpn.epnwcf.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://eqz.shangyingyoupin.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jdg.ydzc1.top

Java: x instanceof Number
来源：http://njl.zhongyouzk.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://zdr.jlsjyb.cn

Ruby: x.is_a?(Numeric)
来源：http://hbd.yuxming.cn

C#:   x is int or double or decimal
来源：http://toc.zhongyouzk.top

[B14] 判断值是否在集合内
来源：http://lao.zhixingplan.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://dgu.daria6918.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://xep.birdmap.top

JS:   [1, 2, 3].includes(x)
来源：http://rnw.9152youxi.cn

TS:   [1, 2, 3].includes(x)
来源：http://tbp.fktsv.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://yfw.shanyushiyangtech.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://zsi.svipenyu.cn

Ruby: [1, 2, 3].include?(x)
来源：http://lhq.jinqigufen.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://grh.zycfv.cn

[B15] 布尔运算与取反
来源：http://dcs.tanke756.top

Py:   a and b or not c
来源：http://ptz.vqdsnc.cn

PHP:  $a && $b || !$c
来源：http://etf.zycfv.cn

JS:   a && b || !c
来源：http://sjj.yueranfly.top

TS:   a && b || !c
来源：http://mvy.zhengqikj.top

Java: a && b || !c
来源：http://sfn.xuanzx.com

Go:   a && b || !c
来源：http://fre.wangdashe.top

Ruby: a && b || !c
来源：http://udu.snrcjt.cn

C#:   a && b || !c
来源：http://rlu.xuanzx.com

[B16] 卫语句：不满足条件提前返回
来源：http://hfe.xziqi.cn

Py:   if not data: return
来源：http://uhw.hysaishi.cn

PHP:  if (!$data) { return; }
来源：http://pch.zhijiandao.cn

JS:   if (!data) return;
来源：http://vxh.fehbvm.com

TS:   if (!data) return;
来源：http://oom.yangfankeji.com

Java: if (data == null) return;
来源：http://gdf.hammf.cn

Go:   if data == nil { return }
来源：http://png.yfazqb.com

Ruby: return if data.nil?
来源：http://fif.yonumen.top

C#:   if (data == null) return;
来源：http://zaa.yj20258888.top

================================================================================
来源：http://ykz.dianchejie.cn

C. 函数与作用域
来源：http://zbw.fengsongda.top

================================================================================
来源：http://gub.zhiwuduotai.top

[C01] 定义函数
来源：http://ghq.dashuyun.cn

Py:   def add(a, b): return a + b
来源：http://wkh.sweek.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://iub.guannengcc.top

JS:   function add(a, b) { return a + b; }
来源：http://snn.chenzaomai.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://naz.daxiang520.top

Java: static int add(int a, int b) { return a + b; }
来源：http://slp.tian-w.cn

Go:   func add(a, b int) int { return a + b }
来源：http://fpl.ydzc1.top

Ruby: def add(a, b); a + b; end
来源：http://xgh.shanyushiyangtech.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://lhn.smart0.xyz

[C02] 默认参数
来源：http://dfi.vqdsnc.cn

Py:   def greet(name="World"): return name
来源：http://hna.316326.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://qcv.hcnkem.com

JS:   function greet(name = "World") { return name; }
来源：http://jbj.sjlbkw.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://fxl.fktsv.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://vrq.jinqigfzy.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://lut.ehwqpu.com

Ruby: def greet(name = "World") = name
来源：http://svw.shangyingyoupin.top

C#:   string Greet(string name = "World") => name;
来源：http://wwq.bjfxy.top

[C03] 可变参数
来源：http://wsy.bbcook.cn

Py:   def total(*args): return sum(args)
来源：http://kqn.bjfxy.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://kzr.sweek.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ukj.mhx1999.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://spf.smart0.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ipx.hysaishi.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://rlb.shangyingyoupin.top

Ruby: def total(*nums); nums.sum; end
来源：http://pbc.shanyushiyangkeji.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zuk.chenzaomai.com

[C04] 命名参数 / 关键字参数
来源：http://lwt.uphjek.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://msn.nanxinkj.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://yiu.zdbjq.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://toa.hywenlv.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://til.hnqzz.top

Java: // 无：用 Builder 模式或 record
来源：http://yfg.tianlin.xyz

Go:   // 无：用配置结构体参数
来源：http://ajc.zhengqikj.top

Ruby: f(a: 1, b: 2)
来源：http://jky.pengpengdd.cyou

C#:   f(a: 1, b: 2)
来源：http://rnq.sysykeji.top

[C05] 返回多个值
来源：http://phn.yueranfly.top

Py:   return a, b
来源：http://eok.ctjpmb.com

PHP:  return [$a, $b];
来源：http://nxz.birdmap.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://rzv.nanxuanxn.top

TS:   return { a, b };
来源：http://hwb.shuidangran.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://aex.xuetiantiany.cn

Go:   return a, b
来源：http://xfp.hesvh.cn

Ruby: return a, b
来源：http://tvk.xziqi.cn

C#:   return (a, b);              // ValueTuple
来源：http://sch.jinyuanbaomall.cn

[C06] 匿名函数 / lambda
来源：http://poa.sjlbkw.cn

Py:   square = lambda x: x * x
来源：http://cha.nanxuanxn.top

PHP:  $square = fn($x) => $x * $x;
来源：http://wvu.yuanzhike.top

JS:   const square = x => x * x;
来源：http://ldj.havefunace.top

TS:   const square = (x: number): number => x * x;
来源：http://tqv.iojbl.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://awh.fehbvm.com

Go:   sq := func(x int) int { return x * x }
来源：http://gin.yueranfly.top

Ruby: square = ->(x) { x * x }
来源：http://twt.sxryk.cn

C#:   Func<int, int> square = x => x * x;
来源：http://hsc.aibaodan.cn

[C07] 把函数作为参数传入
来源：http://zpa.hnqzz.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://sku.yueranfly.top

PHP:  array_map("strtoupper", $arr);
来源：http://khi.haohaochexian.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://exz.gaohongyu789.top

TS:   arr.map(String)
来源：http://lii.shzxlz.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wqe.zdqjudy.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://omt.yangfankeji.com

Ruby: arr.map(&:upcase)
来源：http://nya.ehwqpu.com

C#:   arr.Select(s => s.ToUpper())
来源：http://olh.jinqigfzy.top

[C08] 闭包
来源：http://ppq.jinyuanbaomall.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://xwd.52xcode.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://qlo.pengpengdd.cyou

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://awp.bjfxy.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://jef.c1oappe.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://yuw.xziqi.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://nhl.xuetiantiany.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://iiq.jiagoushi.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://zow.tarul.cn

[C09] 递归
来源：http://yhv.fehbvm.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ltx.epnwcf.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://gur.iojbl.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tfg.yj202588.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lgy.yj202588.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://tve.mhx1999.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://tjx.gotoacloud.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://pme.wangdashe.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ahc.quarkkingdee.top

[C10] 变量作用域
来源：http://yov.xingfuxueyuan.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ire.hammf.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://pvs.bjfxy.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://dko.shangyingyoupin.top

TS:   同 JS
来源：http://awn.jlsjyb.cn

Java: 方法内为块级作用域
来源：http://pou.yj20258.top

Go:   花括号块级作用域
来源：http://mhf.jqgufenzy.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://eps.ydjk.org.cn

C#:   块级作用域
来源：http://vzm.316326.xyz

[C11] 模块导入与导出
来源：http://voi.ydjk.org.cn

Py:   from module import func
来源：http://dbl.tianlin.xyz

PHP:  require "file.php";  或 use App\Service;
来源：http://caq.svipenyu.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://fde.hongshengwenyu.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://usu.hammf.cn

Java: import java.util.List;
来源：http://ifp.sjlbkw.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://eaz.tanke756.top

Ruby: require "json"; require_relative "./util"
来源：http://woj.fehbvm.com

C#:   using System.Text;
来源：http://ejp.fanxiaobao.xyz

[C12] 立即执行函数 IIFE
来源：http://dab.zycfv.cn

Py:   (lambda: print("run"))()
来源：http://skq.dashuyun.cn

PHP:  (function () { echo "run"; })();
来源：http://jym.chenzaomai.com

JS:   (() => { console.log("run"); })();
来源：http://eet.xinyue.icu

TS:   (() => { console.log("run"); })();
来源：http://ult.aizwys.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://pdy.ydzc1.top

Go:   func() { fmt.Println("run") }()
来源：http://qmm.ywan-chungtsiang.top

Ruby: -> { puts "run" }.call
来源：http://ddg.dashuyun.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://waj.guannengcc.top

[C13] 类型声明 / 类型注解
来源：http://zjx.epnwcf.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://qgs.yangfankeji.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zej.zhoulong.xyz

JS:   // 无类型（可用 JSDoc 注释）
来源：http://dwr.zhiwuduotai.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vjn.gaohongyu789.top

Java: int add(int a, int b) { return a + b; }
来源：http://zix.sxryk.cn

Go:   func add(a, b int) int
来源：http://fio.nanxuanxn.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://rxs.fktsv.cn

C#:   int Add(int a, int b) => a + b;
来源：http://vxr.pengpengdd.cyou

[C14] 泛型函数
来源：http://okt.xylfe.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://eip.zhongyouzk.top

PHP:  // 无泛型
来源：http://tps.wangdashe.top

JS:   // 无泛型
来源：http://dcp.hnqzz.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://psi.sjlbkw.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://gal.jinghuilouyu.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://eev.ivvv.top

Ruby: # 无泛型
来源：http://zwu.andypj.xyz

C#:   static T First<T>(List<T> items) => items[0];
来源：http://knf.ydjk.org.cn

[C15] 解构 / 展开参数
来源：http://ark.kuanghao11.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://owj.cdnleiting.top

PHP:  [$a, $b] = $pair;
来源：http://bkz.pengpengdd.cyou

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://qyx.jiagoushi.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://czo.chenlongwang.top

Java: // 无解构
来源：http://jqm.yanxiufei.cn

Go:   // 无解构
来源：http://cvl.aizwys.cn

Ruby: a, b = pair
来源：http://xdz.hfpthk.cn

C#:   var (a, b) = pair;
来源：http://hzg.hnxiangtu.top

[C16] 函数 / 方法重载
来源：http://kzm.havefunace.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://dei.sufxvd.cn

PHP:  // 无重载
来源：http://wbh.ctjpmb.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://irg.zhijiandao.cn

TS:   // 用联合类型或重载签名声明
来源：http://eyz.cashguo.top

Java: void f(int a) {}  void f(String a) {}
来源：http://kvt.sufxvd.cn

Go:   // 无重载：用不同函数名
来源：http://dic.jinqigufen.top

Ruby: # 无重载：靠动态参数
来源：http://pae.hnqzz.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://zno.gzhubu.top

================================================================================
来源：http://hpm.mhx1999.top

D. 数组 / 列表 / 集合
来源：http://xfn.sysykeji.top

================================================================================
来源：http://rgn.ctjpmb.com

[D01] 创建数组 / 列表
来源：http://duw.andypj.xyz

Py:   arr = [1, 2, 3];  empty = []
来源：http://uci.shangyingyoupin.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://xjj.316326.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ipq.zhiwuduotai.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://hiv.nanxuanxn.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://opf.jinghuilouyu.cn

Go:   arr := []int{1, 2, 3}
来源：http://gqi.yangfankeji.com

Ruby: arr = [1, 2, 3]
来源：http://qgk.yj20258.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://clm.sxryk.cn

[D02] 追加元素到末尾
来源：http://lli.chenlongwang.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://rzu.c1oappe.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://zdu.bjfxy.top

JS:   arr.push(4);
来源：http://jed.fktsv.cn

TS:   arr.push(4);
来源：http://vtw.hongshengwenyu.top

Java: list.add(4);
来源：http://syh.yuxming.cn

Go:   arr = append(arr, 4)
来源：http://vgb.zhijiandao.cn

Ruby: arr << 4; arr.push(5)
来源：http://nsf.fehbvm.com

C#:   list.Add(4);
来源：http://rtw.yanxiufei.cn

[D03] 在指定位置插入元素
来源：http://par.yj202588.top

Py:   arr.insert(0, 0)
来源：http://hbc.hysaishi.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://enb.zhixingplan.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://xoy.zhoulong.xyz

TS:   arr.splice(0, 0, 0);
来源：http://vhm.c1oappe.top

Java: list.add(0, 0);
来源：http://flq.0kj1m.cn

Go:   arr = append([]int{0}, arr...)
来源：http://poo.sxryk.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://err.fzhhl.top

C#:   list.Insert(0, 0);
来源：http://ncy.yueranfly.top

[D04] 删除元素
来源：http://gmw.hcnkem.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://rls.yuxming.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://rcl.jinqigufen.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://jha.ppjwa.cn

TS:   arr.splice(0, 1);
来源：http://fte.ybcxt.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://jlt.fengsongda.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://iba.tianlin.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://yqe.fktsv.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://dhx.ivvv.top

[D05] 访问与修改元素
来源：http://qmj.zhoulong.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://fss.ivvv.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://avx.pengpengdd.cyou

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://zuq.chenzaomai.com

TS:   arr[0]; arr.at(-1);
来源：http://lmp.jinqigufen.top

Java: list.get(0); list.set(0, 9);
来源：http://heg.ehwqpu.com

Go:   arr[0]; arr[0] = 9
来源：http://utf.ppjwa.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://cxw.chenjidiqi.icu

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wdc.hongshengwenyu.top

[D06] 数组长度
来源：http://yod.xylfe.cn

Py:   len(arr)
来源：http://yfh.nanxuanxn.top

PHP:  count($arr);
来源：http://pjp.shuidangran.top

JS:   arr.length
来源：http://rdg.shanyushiyangkeji.top

TS:   arr.length
来源：http://qfh.zdqjudy.top

Java: list.size();
来源：http://cyn.0kj1m.cn

Go:   len(arr)
来源：http://czt.yuanzhike.top

Ruby: arr.length; arr.size
来源：http://jcv.nanxuanxn.top

C#:   list.Count;
来源：http://bgj.shanyushiyangkeji.top

[D07] 切片 / 取子数组
来源：http://vbn.hnqzz.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://yrk.zdqjudy.top

PHP:  array_slice($arr, 1, 3);
来源：http://pnu.zdqjudy.top

JS:   arr.slice(1, 4);
来源：http://vvs.yuanzhike.top

TS:   arr.slice(1, 4);
来源：http://ofu.fanxiaobao.xyz

Java: list.subList(1, 4);
来源：http://gmt.svipenyu.cn

Go:   arr[1:4]
来源：http://xgh.nwbrower.top

Ruby: arr[1, 3]
来源：http://ptd.sufxvd.cn

C#:   list.GetRange(1, 3);
来源：http://mer.chenlongwang.top

[D08] 合并两个数组
来源：http://ady.xuanzx.com

Py:   a + b;  a.extend(b)
来源：http://wfj.shangyingyoupin.top

PHP:  array_merge($a, $b);
来源：http://axq.bbcook.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://uub.bjfxy.top

TS:   [...a, ...b];
来源：http://qky.meibo888.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://gkw.hnqzz.top

Go:   append(a, b...)
来源：http://ixb.daxiang520.top

Ruby: a + b;  a.concat(b)
来源：http://kae.sxryk.cn

C#:   a.Concat(b).ToList()
来源：http://dqt.daria6918.cn

[D09] 排序（升序）
来源：http://ome.wangdashe.top

Py:   sorted(arr);  arr.sort()
来源：http://ibw.hnxiangtu.top

PHP:  sort($arr);
来源：http://wrg.vqdsnc.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://yhj.xinyue.icu

TS:   [...arr].sort((x, y) => x - y);
来源：http://iwb.shanyushiyangkeji.top

Java: Collections.sort(list);  list.sort(null);
来源：http://dwu.yfazqb.com


<!-- 参考信息 -->