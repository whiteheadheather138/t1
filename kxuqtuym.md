代发 wailian999

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eka.jlsjyb.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xeo.shzxlz.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ipz.yonumen.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xwg.iojbl.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ccx.feifeiyinyue.top

[B10] 遍历同时拿索引
来源：http://zni.hongshengwenyu.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://pvh.shangyingyoupin.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://bnz.xuanzx.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ojd.hysaishi.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ujk.bjfxy.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://fou.shzxlz.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://rfb.chenlongwang.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hyr.zhoulong.xyz

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wtf.shangyingyoupin.top

[B11] 生成数字序列 / 区间
来源：http://gpr.bjfxy.top

Py:   list(range(0, 10, 2))
来源：http://bbn.chenlongwang.top

PHP:  range(0, 10, 2);
来源：http://mwh.yj20258.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zwa.ybcxt.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xbj.xingfuxueyuan.xyz

Java: IntStream.range(0, 10).boxed().toList()
来源：http://vhh.meibo888.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://yvd.sjlbkw.cn

Ruby: (0...10).step(2).to_a
来源：http://wvp.feifeiyinyue.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://iol.daxiang520.top

[B12] 跳出多层循环
来源：http://amq.316326.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://nxy.ywan-chungtsiang.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://bfc.cqqwz.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://eab.andypj.xyz

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wih.shzxlz.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://qkg.quarkkingdee.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://obu.iojbl.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://aml.fanxiaobao.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://nxh.cheryme.top

[B13] 判断是否为数字
来源：http://zcg.shanyushiyangtech.top

Py:   isinstance(x, (int, float))
来源：http://yho.aizwys.cn

PHP:  is_numeric($x)
来源：http://hya.tian-w.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://psj.9152youxi.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://phq.dianchejie.cn

Java: x instanceof Number
来源：http://fqu.shanyushiyangkeji.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://rtz.aibaodan.cn

Ruby: x.is_a?(Numeric)
来源：http://xcs.nanxuanxn.top

C#:   x is int or double or decimal
来源：http://tra.zhoulong.xyz

[B14] 判断值是否在集合内
来源：http://ecg.sjlbkw.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://pcx.tianlin.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://tti.52xcode.cn

JS:   [1, 2, 3].includes(x)
来源：http://cet.fanxiaobao.xyz

TS:   [1, 2, 3].includes(x)
来源：http://vzi.ctjpmb.com

Java: List.of(1, 2, 3).contains(x)
来源：http://brr.tianlin.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://xdn.fktsv.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ari.shanyushiyangtech.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://gsy.yuxming.cn

[B15] 布尔运算与取反
来源：http://pds.c1oappe.top

Py:   a and b or not c
来源：http://qxv.tianlin.xyz

PHP:  $a && $b || !$c
来源：http://emn.0kj1m.cn

JS:   a && b || !c
来源：http://mqr.cashguo.top

TS:   a && b || !c
来源：http://eka.zhaomingkeji.xyz

Java: a && b || !c
来源：http://tuu.yuanzhike.top

Go:   a && b || !c
来源：http://jci.birdmap.top

Ruby: a && b || !c
来源：http://mns.ctjpmb.com

C#:   a && b || !c
来源：http://vms.nanxuanxn.top

[B16] 卫语句：不满足条件提前返回
来源：http://ufq.nwbrower.top

Py:   if not data: return
来源：http://xqb.yonumen.top

PHP:  if (!$data) { return; }
来源：http://iku.sjlbkw.cn

JS:   if (!data) return;
来源：http://wlz.daxiang520.top

TS:   if (!data) return;
来源：http://bcc.yj202588.top

Java: if (data == null) return;
来源：http://jze.iojbl.cn

Go:   if data == nil { return }
来源：http://ioc.wangdashe.top

Ruby: return if data.nil?
来源：http://gni.zdqjudy.top

C#:   if (data == null) return;
来源：http://xhn.ppjwa.cn

================================================================================
来源：http://igt.chenlongwang.top

C. 函数与作用域
来源：http://sql.cashguo.top

================================================================================
来源：http://kgj.jianghu66.top

[C01] 定义函数
来源：http://egg.sxryk.cn

Py:   def add(a, b): return a + b
来源：http://ggw.wangshuangyany.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jxb.yueranfly.top

JS:   function add(a, b) { return a + b; }
来源：http://qiy.fengsongda.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://prn.shzxlz.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://fpn.fzhhl.top

Go:   func add(a, b int) int { return a + b }
来源：http://zhq.zdbjq.cn

Ruby: def add(a, b); a + b; end
来源：http://tif.gaohongyu789.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hux.ydjk.org.cn

[C02] 默认参数
来源：http://mtj.chenzaomai.com

Py:   def greet(name="World"): return name
来源：http://krc.pengpengdd.cyou

PHP:  function greet($name = "World") { return $name; }
来源：http://gtd.cucudq.cn

JS:   function greet(name = "World") { return name; }
来源：http://rga.fzhhl.top

TS:   function greet(name: string = "World") { return name; }
来源：http://wbf.yuanzhike.top

Java: // 无默认参数：方法重载或 Optional
来源：http://ckz.kuanghao11.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://gxo.xuanzx.com

Ruby: def greet(name = "World") = name
来源：http://hkn.sjlbkw.cn

C#:   string Greet(string name = "World") => name;
来源：http://zmk.316326.xyz

[C03] 可变参数
来源：http://rrg.gogol.net.cn

Py:   def total(*args): return sum(args)
来源：http://mmy.yj20258888.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://vvd.gaohongyu789.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://smg.tanke756.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://fqb.hywenlv.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://obh.jinghuilouyu.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://lhw.guowangkeji.top

Ruby: def total(*nums); nums.sum; end
来源：http://vic.andypj.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ztf.tian-w.cn

[C04] 命名参数 / 关键字参数
来源：http://tlm.jqgufenzy.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ckg.uphjek.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://kzp.yuxming.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://pmr.ppjwa.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://bce.ctjpmb.com

Java: // 无：用 Builder 模式或 record
来源：http://icr.ywan-chungtsiang.top

Go:   // 无：用配置结构体参数
来源：http://jgl.ctjpmb.com

Ruby: f(a: 1, b: 2)
来源：http://mqn.smart0.xyz

C#:   f(a: 1, b: 2)
来源：http://bwq.ybcxt.top

[C05] 返回多个值
来源：http://ymp.tian-w.cn

Py:   return a, b
来源：http://yjf.hammf.cn

PHP:  return [$a, $b];
来源：http://zyj.smart0.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://kek.yonumen.top

TS:   return { a, b };
来源：http://qzf.dianchejie.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://kjn.uphjek.com

Go:   return a, b
来源：http://mnr.jyoumei.cn

Ruby: return a, b
来源：http://bbd.cdnleiting.top

C#:   return (a, b);              // ValueTuple
来源：http://osd.vqdsnc.cn

[C06] 匿名函数 / lambda
来源：http://mda.guowangkeji.top

Py:   square = lambda x: x * x
来源：http://gqx.svipenyu.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://eda.vqdsnc.cn

JS:   const square = x => x * x;
来源：http://rlv.fanxiaobao.xyz

TS:   const square = (x: number): number => x * x;
来源：http://yzk.jinyuanbaomall.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://jwp.jqgufenzy.top

Go:   sq := func(x int) int { return x * x }
来源：http://iql.gogol.net.cn

Ruby: square = ->(x) { x * x }
来源：http://psb.hfpthk.cn

C#:   Func<int, int> square = x => x * x;
来源：http://amq.zhixingplan.top

[C07] 把函数作为参数传入
来源：http://ify.daxiang520.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hvs.chenzaomai.com

PHP:  array_map("strtoupper", $arr);
来源：http://shd.jyoumei.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://qyx.xuetiantiany.cn

TS:   arr.map(String)
来源：http://dhh.iojbl.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://sip.gaohongyu789.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hnq.xinyue.icu

Ruby: arr.map(&:upcase)
来源：http://zyo.dianchejie.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://rnb.ivvv.top

[C08] 闭包
来源：http://eol.0kj1m.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://fvz.vehdjk.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://agf.wangdashe.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://crl.jyoumei.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://yng.hywenlv.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://uwf.jinqigufen.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://bui.tanke756.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://xdx.yanxiufei.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://vry.fzhhl.top

[C09] 递归
来源：http://lri.jyoumei.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://adc.andypj.xyz

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://yrg.zhongyouzk.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xbj.yongpay.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rbk.vqdsnc.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://bmj.shuidangran.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://lts.wangshuangyany.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://uws.pengpengdd.cyou

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://nap.52xcode.cn

[C10] 变量作用域
来源：http://lyw.svipenyu.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://nuw.yuanzhike.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://igm.pycfn.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://fno.yongpay.top

TS:   同 JS
来源：http://jme.ydjk.org.cn

Java: 方法内为块级作用域
来源：http://gvv.hnqzz.top

Go:   花括号块级作用域
来源：http://kyg.hysaishi.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://poz.yangfankeji.com

C#:   块级作用域
来源：http://gwd.sjlbkw.cn

[C11] 模块导入与导出
来源：http://ebw.mhx1999.top

Py:   from module import func
来源：http://eqx.yonumen.top

PHP:  require "file.php";  或 use App\Service;
来源：http://pau.vqdsnc.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://xpw.zhaomingkeji.xyz

TS:   export function f(): void {};  import { f } from "./m";
来源：http://pht.nwbrower.top

Java: import java.util.List;
来源：http://kch.gzhubu.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://jmu.dashuyun.cn

Ruby: require "json"; require_relative "./util"
来源：http://xzi.zhaomingkeji.xyz

C#:   using System.Text;
来源：http://sfe.tian-w.cn

[C12] 立即执行函数 IIFE
来源：http://jaq.pengpengdd.cyou

Py:   (lambda: print("run"))()
来源：http://hhl.zhengqikj.top

PHP:  (function () { echo "run"; })();
来源：http://uhb.epnwcf.com

JS:   (() => { console.log("run"); })();
来源：http://pxy.gaohongyu789.top

TS:   (() => { console.log("run"); })();
来源：http://gqu.yj20258888.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://tdd.yangfankeji.com

Go:   func() { fmt.Println("run") }()
来源：http://kzh.gotoacloud.top

Ruby: -> { puts "run" }.call
来源：http://xku.hywenlv.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://bep.snrcjt.cn

[C13] 类型声明 / 类型注解
来源：http://yhs.yj20258888.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://zwg.birdmap.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rus.shangyingyoupin.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ogo.wangdashe.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ymr.pycfn.com

Java: int add(int a, int b) { return a + b; }
来源：http://yjc.gotoacloud.top

Go:   func add(a, b int) int
来源：http://noz.jqgfzy.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://vrw.52xcode.cn

C#:   int Add(int a, int b) => a + b;
来源：http://wvq.jianghu66.top

[C14] 泛型函数
来源：http://huq.cdnleiting.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wgi.vqdsnc.cn

PHP:  // 无泛型
来源：http://zpr.fanxiaobao.xyz

JS:   // 无泛型
来源：http://yaa.zhixingplan.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://scc.0kj1m.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://uvo.iojbl.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://bvk.andypj.xyz

Ruby: # 无泛型
来源：http://mlj.yj202588.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://uiy.vehdjk.com

[C15] 解构 / 展开参数
来源：http://ouu.xinyue.icu

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://oco.shanyushiyangtech.top

PHP:  [$a, $b] = $pair;
来源：http://iic.shzxlz.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ifr.jianghu66.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://qhd.zhongyouzk.top

Java: // 无解构
来源：http://lfn.zdbjq.cn

Go:   // 无解构
来源：http://ozg.iojbl.cn

Ruby: a, b = pair
来源：http://xpu.jlsjyb.cn

C#:   var (a, b) = pair;
来源：http://wfa.jyoumei.cn

[C16] 函数 / 方法重载
来源：http://vis.shanyushiyangkeji.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://nog.yonumen.top

PHP:  // 无重载
来源：http://hjx.svipenyu.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://rtq.zhengqikj.top

TS:   // 用联合类型或重载签名声明
来源：http://vmd.zdbjq.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://eih.gaohongyu789.top

Go:   // 无重载：用不同函数名
来源：http://mnx.shzxlz.cn

Ruby: # 无重载：靠动态参数
来源：http://jas.hywenlv.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://vfs.svipenyu.cn

================================================================================
来源：http://clp.hammf.cn

D. 数组 / 列表 / 集合
来源：http://dlx.shzxlz.cn

================================================================================
来源：http://ahs.tarul.cn

[D01] 创建数组 / 列表
来源：http://gyq.tian-w.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ipg.tian-w.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mxs.fengsongda.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://eiw.zdqjudy.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://mnk.dashuyun.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://xar.jlsjyb.cn

Go:   arr := []int{1, 2, 3}
来源：http://cls.fzhhl.top

Ruby: arr = [1, 2, 3]
来源：http://piy.hongshengwenyu.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://src.tian-w.cn

[D02] 追加元素到末尾
来源：http://cyp.dianchejie.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://osq.sufxvd.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://npf.epnwcf.com

JS:   arr.push(4);
来源：http://bba.jiagoushi.top

TS:   arr.push(4);
来源：http://kjr.daxiang520.top

Java: list.add(4);
来源：http://qcx.tanke756.top

Go:   arr = append(arr, 4)
来源：http://tmr.zdbjq.cn

Ruby: arr << 4; arr.push(5)
来源：http://gtd.zhoulong.xyz

C#:   list.Add(4);
来源：http://yic.gotoacloud.top

[D03] 在指定位置插入元素
来源：http://uej.vqdsnc.cn

Py:   arr.insert(0, 0)
来源：http://apr.fanxiaobao.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://keq.ydjk.org.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ggt.cdnleiting.top

TS:   arr.splice(0, 0, 0);
来源：http://wzd.hammf.cn

Java: list.add(0, 0);
来源：http://kss.zycfv.cn

Go:   arr = append([]int{0}, arr...)
来源：http://mlt.shuidangran.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://zwg.zycfv.cn

C#:   list.Insert(0, 0);
来源：http://jmj.xuanzx.com

[D04] 删除元素
来源：http://ogd.chenlongwang.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://yqh.52xcode.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://vpz.c1oappe.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://jhq.tian-w.cn

TS:   arr.splice(0, 1);
来源：http://gee.zhongyouzk.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mpl.zhijiandao.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://tbo.316326.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://okd.xinyue.icu

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://uhj.ctjpmb.com

[D05] 访问与修改元素
来源：http://udf.chenjidiqi.icu

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://vpd.ydjk.org.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://yjl.wangshuangyany.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ncz.yueranfly.top

TS:   arr[0]; arr.at(-1);
来源：http://ucj.feifeiyinyue.top

Java: list.get(0); list.set(0, 9);
来源：http://zti.hesvh.cn

Go:   arr[0]; arr[0] = 9
来源：http://lfj.jinqigufen.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://brl.nanxinkj.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hpa.nanxinkj.top

[D06] 数组长度
来源：http://bnb.ivvv.top

Py:   len(arr)
来源：http://epb.yueranfly.top

PHP:  count($arr);
来源：http://wjs.ehwqpu.com

JS:   arr.length
来源：http://wkz.sufxvd.cn

TS:   arr.length
来源：http://jra.0kj1m.cn

Java: list.size();
来源：http://vfg.sjlbkw.cn

Go:   len(arr)
来源：http://fkf.hywenlv.cn

Ruby: arr.length; arr.size
来源：http://hdp.cheryme.top

C#:   list.Count;
来源：http://icr.redwolf501.top

[D07] 切片 / 取子数组
来源：http://pkn.jqgufenzy.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://usb.yangfankeji.com

PHP:  array_slice($arr, 1, 3);
来源：http://iiq.52xcode.cn

JS:   arr.slice(1, 4);
来源：http://qdu.zhijiandao.cn

TS:   arr.slice(1, 4);
来源：http://ndp.wangdashe.top

Java: list.subList(1, 4);
来源：http://erk.zdbjq.cn

Go:   arr[1:4]
来源：http://tme.vehdjk.com

Ruby: arr[1, 3]
来源：http://gwe.guowangkeji.top

C#:   list.GetRange(1, 3);
来源：http://sdd.ybcxt.top

[D08] 合并两个数组
来源：http://oag.nanxuanxn.top

Py:   a + b;  a.extend(b)
来源：http://ozw.fzhhl.top

PHP:  array_merge($a, $b);
来源：http://eil.chenjidiqi.icu

JS:   [...a, ...b];  a.concat(b);
来源：http://vmn.jinyuanbaomall.cn

TS:   [...a, ...b];
来源：http://dwl.svipenyu.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://jsx.tanke756.top

Go:   append(a, b...)
来源：http://vjo.xinyue.icu

Ruby: a + b;  a.concat(b)
来源：http://ivy.yvedp.cn

C#:   a.Concat(b).ToList()
来源：http://azj.c1oappe.top

[D09] 排序（升序）
来源：http://mbc.uphjek.com

Py:   sorted(arr);  arr.sort()
来源：http://khz.svipenyu.cn

PHP:  sort($arr);
来源：http://uwo.316326.xyz

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://rav.zhiwuduotai.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://qxr.yj20258.top

Java: Collections.sort(list);  list.sort(null);
来源：http://kvt.cucudq.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://jzv.nwbrower.top

Ruby: arr.sort
来源：http://wwz.zhoulong.xyz

C#:   list.Sort();
来源：http://vej.xuetiantiany.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://kdw.xylfe.cn


<!-- 参考信息 -->