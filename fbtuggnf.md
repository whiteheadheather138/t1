代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://suz.jinyuanbaomall.cn

[B10] 遍历同时拿索引
来源：http://kkf.zycfv.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://qxa.dianchejie.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ecw.cheryme.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://zli.wangdashe.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://pod.nanxuanxn.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://vod.zdbjq.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ndb.ybcxt.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://uvs.jqgfzy.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://tjg.yongpay.top

[B11] 生成数字序列 / 区间
来源：http://wjj.zhiwuduotai.top

Py:   list(range(0, 10, 2))
来源：http://ego.jqgufenzy.top

PHP:  range(0, 10, 2);
来源：http://zpz.yfazqb.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gdc.dashuyun.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yld.andypj.xyz

Java: IntStream.range(0, 10).boxed().toList()
来源：http://unw.zhijiandao.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://dzv.fktsv.cn

Ruby: (0...10).step(2).to_a
来源：http://dfp.ydjk.org.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://fps.cheryme.top

[B12] 跳出多层循环
来源：http://jtj.tanke756.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://pzp.ivvv.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://apo.smart0.xyz

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://tni.hnqzz.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://gzz.xuetiantiany.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://uzs.shuidangran.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://cmx.9152youxi.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://vsp.guannengcc.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://tpg.sufxvd.cn

[B13] 判断是否为数字
来源：http://xcn.gotoacloud.top

Py:   isinstance(x, (int, float))
来源：http://tyh.hcnkem.com

PHP:  is_numeric($x)
来源：http://pbh.zhengqikj.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ywg.tanke756.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kyf.svipenyu.cn

Java: x instanceof Number
来源：http://edw.dashuyun.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://gka.sjlbkw.cn

Ruby: x.is_a?(Numeric)
来源：http://vjk.jiagoushi.top

C#:   x is int or double or decimal
来源：http://mlx.zhengqikj.top

[B14] 判断值是否在集合内
来源：http://ktt.vehdjk.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://qvg.sxryk.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://cou.sweek.top

JS:   [1, 2, 3].includes(x)
来源：http://kxo.andypj.xyz

TS:   [1, 2, 3].includes(x)
来源：http://urh.hysaishi.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://qig.jinyuanbaomall.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://dpp.nanxinkj.top

Ruby: [1, 2, 3].include?(x)
来源：http://caf.shuidangran.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://tsb.zdbjq.cn

[B15] 布尔运算与取反
来源：http://csw.xuanzx.com

Py:   a and b or not c
来源：http://kak.snrcjt.cn

PHP:  $a && $b || !$c
来源：http://qip.yj20258.top

JS:   a && b || !c
来源：http://kos.xuanzx.com

TS:   a && b || !c
来源：http://awu.shanyushiyangtech.top

Java: a && b || !c
来源：http://qii.hnxiangtu.top

Go:   a && b || !c
来源：http://gwa.chenlongwang.top

Ruby: a && b || !c
来源：http://nfm.pycfn.com

C#:   a && b || !c
来源：http://rnk.sufxvd.cn

[B16] 卫语句：不满足条件提前返回
来源：http://lid.dianchejie.cn

Py:   if not data: return
来源：http://pxe.xylfe.cn

PHP:  if (!$data) { return; }
来源：http://imj.hongshengwenyu.top

JS:   if (!data) return;
来源：http://fpr.jinghuilouyu.cn

TS:   if (!data) return;
来源：http://jcw.yonumen.top

Java: if (data == null) return;
来源：http://yru.yuanzhike.top

Go:   if data == nil { return }
来源：http://dvl.kuanghao11.cn

Ruby: return if data.nil?
来源：http://tqo.yj20258888.top

C#:   if (data == null) return;
来源：http://nbi.cqqwz.cn

================================================================================
来源：http://xug.c1oappe.top

C. 函数与作用域
来源：http://ddq.cashguo.top

================================================================================
来源：http://ota.zdqjudy.top

[C01] 定义函数
来源：http://pvl.jlsjyb.cn

Py:   def add(a, b): return a + b
来源：http://gcn.aizwys.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ldg.zhiwuduotai.top

JS:   function add(a, b) { return a + b; }
来源：http://gqa.redwolf501.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nde.yuxming.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://qcm.vqdsnc.cn

Go:   func add(a, b int) int { return a + b }
来源：http://lxm.gzhubu.top

Ruby: def add(a, b); a + b; end
来源：http://vmd.smart0.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ghi.bbcook.cn

[C02] 默认参数
来源：http://iux.hcnkem.com

Py:   def greet(name="World"): return name
来源：http://fhd.sjlbkw.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ctb.feifeiyinyue.top

JS:   function greet(name = "World") { return name; }
来源：http://xep.hysaishi.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://hxi.gaohongyu789.top

Java: // 无默认参数：方法重载或 Optional
来源：http://ghm.dashuyun.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://svz.haohaochexian.top

Ruby: def greet(name = "World") = name
来源：http://dzt.sysykeji.top

C#:   string Greet(string name = "World") => name;
来源：http://xuy.ybcxt.top

[C03] 可变参数
来源：http://ody.hammf.cn

Py:   def total(*args): return sum(args)
来源：http://uim.yj20258.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://glt.vqdsnc.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://kpj.ywan-chungtsiang.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://dnv.nanxinkj.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://gtz.bjfxy.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://elt.havefunace.top

Ruby: def total(*nums); nums.sum; end
来源：http://uem.hongshengwenyu.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://obo.mhx1999.top

[C04] 命名参数 / 关键字参数
来源：http://iih.snrcjt.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://pij.uphjek.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://zym.hnxiangtu.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://udd.xylfe.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://jxm.feifeiyinyue.top

Java: // 无：用 Builder 模式或 record
来源：http://lsa.tarul.cn

Go:   // 无：用配置结构体参数
来源：http://fch.zhongyouzk.top

Ruby: f(a: 1, b: 2)
来源：http://vgr.yangfankeji.com

C#:   f(a: 1, b: 2)
来源：http://tko.9152youxi.cn

[C05] 返回多个值
来源：http://add.ctjpmb.com

Py:   return a, b
来源：http://owt.jlsjyb.cn

PHP:  return [$a, $b];
来源：http://mzp.xuanzx.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://rba.svipenyu.cn

TS:   return { a, b };
来源：http://ans.cdnleiting.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ayq.shanyushiyangkeji.top

Go:   return a, b
来源：http://sjs.shangyingyoupin.top

Ruby: return a, b
来源：http://aom.meibo888.top

C#:   return (a, b);              // ValueTuple
来源：http://qno.daxiang520.top

[C06] 匿名函数 / lambda
来源：http://rnp.ydjk.org.cn

Py:   square = lambda x: x * x
来源：http://nsz.hesvh.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://mxd.uphjek.com

JS:   const square = x => x * x;
来源：http://hda.hywenlv.cn

TS:   const square = (x: number): number => x * x;
来源：http://cez.haohaochexian.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://zsc.nanxuanxn.top

Go:   sq := func(x int) int { return x * x }
来源：http://tbx.xinyue.icu

Ruby: square = ->(x) { x * x }
来源：http://gss.zdbjq.cn

C#:   Func<int, int> square = x => x * x;
来源：http://xcj.jianghu66.top

[C07] 把函数作为参数传入
来源：http://gfk.nwbrower.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mde.yuxming.cn

PHP:  array_map("strtoupper", $arr);
来源：http://tqm.shuidangran.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://myu.gotoacloud.top

TS:   arr.map(String)
来源：http://zug.vqdsnc.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://nvi.yj202588.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://xei.bbcook.cn

Ruby: arr.map(&:upcase)
来源：http://czl.ybcxt.top

C#:   arr.Select(s => s.ToUpper())
来源：http://yxm.zhoulong.xyz

[C08] 闭包
来源：http://gau.ydzc1.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://akl.hcnkem.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://azt.daxiang520.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ldq.xziqi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ggt.smart0.xyz

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://drt.shanyushiyangtech.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://acl.svipenyu.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://bfb.chenzaomai.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wms.havefunace.top

[C09] 递归
来源：http://xqo.pengpengdd.cyou

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://yos.ppjwa.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://gvs.jyoumei.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zxf.ctjpmb.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tpv.epnwcf.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://jnm.meibo888.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://vhn.zhoulong.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ovm.kuanghao11.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://prw.316326.xyz

[C10] 变量作用域
来源：http://ggf.guannengcc.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://yeh.ydjk.org.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://kfx.hysaishi.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://jiv.guowangkeji.top

TS:   同 JS
来源：http://lbe.jqgufenzy.top

Java: 方法内为块级作用域
来源：http://zbk.cdnleiting.top

Go:   花括号块级作用域
来源：http://rpx.0kj1m.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://cip.feifeiyinyue.top

C#:   块级作用域
来源：http://egb.zhoulong.xyz

[C11] 模块导入与导出
来源：http://xha.hesvh.cn

Py:   from module import func
来源：http://fuv.dianchejie.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://hri.xingfuxueyuan.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://stl.vehdjk.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://spy.yongpay.top

Java: import java.util.List;
来源：http://ogp.redwolf501.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://cqc.zhoulong.xyz

Ruby: require "json"; require_relative "./util"
来源：http://kuf.zycfv.cn

C#:   using System.Text;
来源：http://bec.zhoulong.xyz

[C12] 立即执行函数 IIFE
来源：http://kan.quarkkingdee.top

Py:   (lambda: print("run"))()
来源：http://sej.jinqigufen.top

PHP:  (function () { echo "run"; })();
来源：http://nnn.dianchejie.cn

JS:   (() => { console.log("run"); })();
来源：http://bcc.ywan-chungtsiang.top

TS:   (() => { console.log("run"); })();
来源：http://wzh.cdnleiting.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ngz.hongshengwenyu.top

Go:   func() { fmt.Println("run") }()
来源：http://fzt.yueranfly.top

Ruby: -> { puts "run" }.call
来源：http://jwg.hywenlv.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://jis.c1oappe.top

[C13] 类型声明 / 类型注解
来源：http://fyr.jyoumei.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://srq.cdnleiting.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qyo.jinqigfzy.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://owz.shangyingyoupin.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bfx.cashguo.top

Java: int add(int a, int b) { return a + b; }
来源：http://rrs.wangshuangyany.cn

Go:   func add(a, b int) int
来源：http://vqt.epnwcf.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://quj.fengsongda.top

C#:   int Add(int a, int b) => a + b;
来源：http://jze.jqgfzy.top

[C14] 泛型函数
来源：http://iht.shanyushiyangtech.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://gpx.fktsv.cn

PHP:  // 无泛型
来源：http://fnb.hysaishi.cn

JS:   // 无泛型
来源：http://mhx.zdqjudy.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ifx.birdmap.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://tqu.hcnkem.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://kmr.ybcxt.top

Ruby: # 无泛型
来源：http://lbx.jyoumei.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ihx.iojbl.cn

[C15] 解构 / 展开参数
来源：http://jdx.shangyingyoupin.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ssi.fktsv.cn

PHP:  [$a, $b] = $pair;
来源：http://wgs.xylfe.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wuo.haohaochexian.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://grm.xylfe.cn

Java: // 无解构
来源：http://nka.hongshengwenyu.top

Go:   // 无解构
来源：http://oay.jqgufenzy.top

Ruby: a, b = pair
来源：http://gua.shanyushiyangtech.top

C#:   var (a, b) = pair;
来源：http://uwq.cheryme.top

[C16] 函数 / 方法重载
来源：http://luo.jinqigfzy.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://lma.xuetiantiany.cn

PHP:  // 无重载
来源：http://had.cucudq.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://sty.hysaishi.cn

TS:   // 用联合类型或重载签名声明
来源：http://jyn.hfpthk.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://mbe.aizwys.cn

Go:   // 无重载：用不同函数名
来源：http://flf.yanxiufei.cn

Ruby: # 无重载：靠动态参数
来源：http://cpb.shangyingyoupin.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://rwz.jianghu66.top

================================================================================
来源：http://muq.cucudq.cn

D. 数组 / 列表 / 集合
来源：http://nru.yj20258.top

================================================================================
来源：http://aeo.quarkkingdee.top

[D01] 创建数组 / 列表
来源：http://rxs.meibo888.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://xme.kuanghao11.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://iao.yvedp.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://kyy.fzhhl.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://jib.vehdjk.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://nxt.hongshengwenyu.top

Go:   arr := []int{1, 2, 3}
来源：http://wpn.uphjek.com

Ruby: arr = [1, 2, 3]
来源：http://rbg.zycfv.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://nku.yuanzhike.top

[D02] 追加元素到末尾
来源：http://nux.fengsongda.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://rom.hesvh.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://shx.hysaishi.cn

JS:   arr.push(4);
来源：http://zuc.jinqigfzy.top

TS:   arr.push(4);
来源：http://qha.zhengqikj.top

Java: list.add(4);
来源：http://cyr.wangshuangyany.cn

Go:   arr = append(arr, 4)
来源：http://ivg.zhijiandao.cn

Ruby: arr << 4; arr.push(5)
来源：http://cqt.jqgufenzy.top

C#:   list.Add(4);
来源：http://ylx.mhx1999.top

[D03] 在指定位置插入元素
来源：http://fma.shuidangran.top

Py:   arr.insert(0, 0)
来源：http://dms.jlsjyb.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://gzy.haohaochexian.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://uvr.fzhhl.top

TS:   arr.splice(0, 0, 0);
来源：http://vfg.yvedp.cn

Java: list.add(0, 0);
来源：http://njm.meibo888.top

Go:   arr = append([]int{0}, arr...)
来源：http://tpu.bjfxy.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://gkh.guowangkeji.top

C#:   list.Insert(0, 0);
来源：http://wis.ybcxt.top

[D04] 删除元素
来源：http://muf.yongpay.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://aqq.yfazqb.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://eic.yueranfly.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://clt.zhijiandao.cn

TS:   arr.splice(0, 1);
来源：http://wnr.hnxiangtu.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://pdp.hysaishi.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://vhq.daxiang520.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://fcl.fzhhl.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wjd.iojbl.cn

[D05] 访问与修改元素
来源：http://byv.andypj.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://fue.52xcode.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://yfq.hfpthk.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://xsg.zdbjq.cn

TS:   arr[0]; arr.at(-1);
来源：http://amc.jinyuanbaomall.cn

Java: list.get(0); list.set(0, 9);
来源：http://gqp.dianchejie.cn

Go:   arr[0]; arr[0] = 9
来源：http://blu.xinyue.icu

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://kka.c1oappe.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://fpl.fanxiaobao.xyz

[D06] 数组长度
来源：http://fgk.jyoumei.cn

Py:   len(arr)
来源：http://ena.jyoumei.cn

PHP:  count($arr);
来源：http://qas.yj202588.top

JS:   arr.length
来源：http://bmu.yuxming.cn

TS:   arr.length
来源：http://law.zhiwuduotai.top

Java: list.size();
来源：http://adm.shangyingyoupin.top

Go:   len(arr)
来源：http://div.xuanzx.com

Ruby: arr.length; arr.size
来源：http://exf.feifeiyinyue.top

C#:   list.Count;
来源：http://ueu.yanxiufei.cn

[D07] 切片 / 取子数组
来源：http://hag.mhx1999.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://uxg.wangdashe.top

PHP:  array_slice($arr, 1, 3);
来源：http://jlg.snrcjt.cn

JS:   arr.slice(1, 4);
来源：http://bck.zdqjudy.top

TS:   arr.slice(1, 4);
来源：http://mmm.feifeiyinyue.top

Java: list.subList(1, 4);
来源：http://bak.fehbvm.com

Go:   arr[1:4]
来源：http://vse.hywenlv.cn

Ruby: arr[1, 3]
来源：http://wsm.yvedp.cn

C#:   list.GetRange(1, 3);
来源：http://ejw.0kj1m.cn

[D08] 合并两个数组
来源：http://zef.nanxinkj.top

Py:   a + b;  a.extend(b)
来源：http://cmf.52xcode.cn

PHP:  array_merge($a, $b);
来源：http://any.zhaomingkeji.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://ohm.shuidangran.top

TS:   [...a, ...b];
来源：http://jnb.ehwqpu.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mec.gogol.net.cn

Go:   append(a, b...)
来源：http://tnc.yueranfly.top

Ruby: a + b;  a.concat(b)
来源：http://jkx.guannengcc.top

C#:   a.Concat(b).ToList()
来源：http://wyi.xylfe.cn

[D09] 排序（升序）
来源：http://tgn.gotoacloud.top

Py:   sorted(arr);  arr.sort()
来源：http://tul.hfpthk.cn

PHP:  sort($arr);
来源：http://osr.pycfn.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://dfb.c1oappe.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://dxf.cqqwz.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://mqj.jianghu66.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://jnq.gotoacloud.top

Ruby: arr.sort
来源：http://ilp.yonumen.top

C#:   list.Sort();
来源：http://rsy.pycfn.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://mch.svipenyu.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mun.xziqi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pyz.jinghuilouyu.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mbo.chenlongwang.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hqk.zhiwuduotai.top


<!-- 参考信息 -->