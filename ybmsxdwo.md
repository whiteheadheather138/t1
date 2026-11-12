代发 wailian999

[B09] break 与 continue
来源：http://bqw.epnwcf.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hvd.dianchejie.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ofw.yuxming.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://voh.yvedp.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zal.vehdjk.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://drx.chenlongwang.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ofi.wangdashe.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://lzx.nanxuanxn.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ouj.yj202588.top

[B10] 遍历同时拿索引
来源：http://iau.yj20258.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://upi.zhixingplan.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://jkp.yonumen.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://svd.wangdashe.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hkn.hammf.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wux.ehwqpu.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://dxx.sxryk.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://rob.xinyue.icu

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://lws.uphjek.com

[B11] 生成数字序列 / 区间
来源：http://tjh.sufxvd.cn

Py:   list(range(0, 10, 2))
来源：http://ssu.hysaishi.cn

PHP:  range(0, 10, 2);
来源：http://weo.yj20258.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zrk.zhengqikj.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bqm.hfpthk.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://meq.hammf.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ijn.jinyuanbaomall.cn

Ruby: (0...10).step(2).to_a
来源：http://vxw.c1oappe.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://yrx.jinyuanbaomall.cn

[B12] 跳出多层循环
来源：http://nro.zhiwuduotai.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://irx.jianghu66.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://hkr.fanxiaobao.xyz

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ace.ybcxt.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://pyl.haohaochexian.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://qwt.jianghu66.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://xnu.chenzaomai.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://tem.daria6918.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://jal.shanyushiyangkeji.top

[B13] 判断是否为数字
来源：http://csd.tanke756.top

Py:   isinstance(x, (int, float))
来源：http://ihh.zdbjq.cn

PHP:  is_numeric($x)
来源：http://tkn.jianghu66.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://egz.nwbrower.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fry.jinghuilouyu.cn

Java: x instanceof Number
来源：http://tyg.hysaishi.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://kav.hfpthk.cn

Ruby: x.is_a?(Numeric)
来源：http://dap.feifeiyinyue.top

C#:   x is int or double or decimal
来源：http://bka.c1oappe.top

[B14] 判断值是否在集合内
来源：http://jbo.jqgfzy.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ewq.shuidangran.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://eun.tian-w.cn

JS:   [1, 2, 3].includes(x)
来源：http://dks.shanyushiyangkeji.top

TS:   [1, 2, 3].includes(x)
来源：http://mnv.zhongyouzk.top

Java: List.of(1, 2, 3).contains(x)
来源：http://jjn.tianlin.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://nyf.hywenlv.cn

Ruby: [1, 2, 3].include?(x)
来源：http://uwx.meibo888.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mfg.iojbl.cn

[B15] 布尔运算与取反
来源：http://vya.zhoulong.xyz

Py:   a and b or not c
来源：http://bfc.gogol.net.cn

PHP:  $a && $b || !$c
来源：http://ewz.sufxvd.cn

JS:   a && b || !c
来源：http://mbn.pycfn.com

TS:   a && b || !c
来源：http://lwo.cqqwz.cn

Java: a && b || !c
来源：http://ppv.yanxiufei.cn

Go:   a && b || !c
来源：http://sdv.316326.xyz

Ruby: a && b || !c
来源：http://xxo.sysykeji.top

C#:   a && b || !c
来源：http://ihg.mhx1999.top

[B16] 卫语句：不满足条件提前返回
来源：http://wap.kuanghao11.cn

Py:   if not data: return
来源：http://zmp.fehbvm.com

PHP:  if (!$data) { return; }
来源：http://pgr.zhijiandao.cn

JS:   if (!data) return;
来源：http://azq.smart0.xyz

TS:   if (!data) return;
来源：http://pbb.nanxinkj.top

Java: if (data == null) return;
来源：http://nfr.c1oappe.top

Go:   if data == nil { return }
来源：http://krb.jqgfzy.top

Ruby: return if data.nil?
来源：http://uck.svipenyu.cn

C#:   if (data == null) return;
来源：http://jud.hesvh.cn

================================================================================
来源：http://ssh.sysykeji.top

C. 函数与作用域
来源：http://uau.sxryk.cn

================================================================================
来源：http://aou.hnqzz.top

[C01] 定义函数
来源：http://twy.daxiang520.top

Py:   def add(a, b): return a + b
来源：http://flp.chenlongwang.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dli.gaohongyu789.top

JS:   function add(a, b) { return a + b; }
来源：http://ptc.fktsv.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yte.hesvh.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://wya.ivvv.top

Go:   func add(a, b int) int { return a + b }
来源：http://qao.zycfv.cn

Ruby: def add(a, b); a + b; end
来源：http://cgh.yvedp.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://phr.vehdjk.com

[C02] 默认参数
来源：http://apw.wangshuangyany.cn

Py:   def greet(name="World"): return name
来源：http://mpp.tanke756.top

PHP:  function greet($name = "World") { return $name; }
来源：http://eno.cqqwz.cn

JS:   function greet(name = "World") { return name; }
来源：http://wrf.jinyuanbaomall.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://con.fzhhl.top

Java: // 无默认参数：方法重载或 Optional
来源：http://cgl.aizwys.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://clt.yj202588.top

Ruby: def greet(name = "World") = name
来源：http://iry.gzhubu.top

C#:   string Greet(string name = "World") => name;
来源：http://gwr.zhijiandao.cn

[C03] 可变参数
来源：http://cnc.jlsjyb.cn

Py:   def total(*args): return sum(args)
来源：http://xci.cdnleiting.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://htg.nanxinkj.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://cjn.fzhhl.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://tpm.daxiang520.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ejw.shangyingyoupin.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://aar.yvedp.cn

Ruby: def total(*nums); nums.sum; end
来源：http://oxa.yuxming.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://lra.xingfuxueyuan.xyz

[C04] 命名参数 / 关键字参数
来源：http://vyi.ydjk.org.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://fcj.yj20258.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://uij.nwbrower.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://nwe.zhaomingkeji.xyz

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://zoo.jyoumei.cn

Java: // 无：用 Builder 模式或 record
来源：http://fuf.ybcxt.top

Go:   // 无：用配置结构体参数
来源：http://nrc.fzhhl.top

Ruby: f(a: 1, b: 2)
来源：http://xnu.yj20258888.top

C#:   f(a: 1, b: 2)
来源：http://txj.shzxlz.cn

[C05] 返回多个值
来源：http://ifr.ivvv.top

Py:   return a, b
来源：http://fde.fengsongda.top

PHP:  return [$a, $b];
来源：http://qvl.cqqwz.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://hrz.zhoulong.xyz

TS:   return { a, b };
来源：http://hpm.vehdjk.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://iad.fehbvm.com

Go:   return a, b
来源：http://wtq.andypj.xyz

Ruby: return a, b
来源：http://vco.haohaochexian.top

C#:   return (a, b);              // ValueTuple
来源：http://eyv.pycfn.com

[C06] 匿名函数 / lambda
来源：http://dfm.jqgfzy.top

Py:   square = lambda x: x * x
来源：http://ksd.hfpthk.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://tkb.316326.xyz

JS:   const square = x => x * x;
来源：http://xnl.uphjek.com

TS:   const square = (x: number): number => x * x;
来源：http://dea.cheryme.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://aey.guannengcc.top

Go:   sq := func(x int) int { return x * x }
来源：http://fgs.yvedp.cn

Ruby: square = ->(x) { x * x }
来源：http://nih.chenlongwang.top

C#:   Func<int, int> square = x => x * x;
来源：http://vrs.gogol.net.cn

[C07] 把函数作为参数传入
来源：http://inb.vqdsnc.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://dwn.zdqjudy.top

PHP:  array_map("strtoupper", $arr);
来源：http://vgf.316326.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wwa.fengsongda.top

TS:   arr.map(String)
来源：http://xaz.svipenyu.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://qzz.vqdsnc.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://znm.zycfv.cn

Ruby: arr.map(&:upcase)
来源：http://dpk.cdnleiting.top

C#:   arr.Select(s => s.ToUpper())
来源：http://whv.ydjk.org.cn

[C08] 闭包
来源：http://arr.ybcxt.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://rug.shuidangran.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://gfz.yuanzhike.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vnr.ydzc1.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://nzd.shuidangran.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://fqc.chenzaomai.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://cdk.quarkkingdee.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://dtq.feifeiyinyue.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://oyl.yangfankeji.com

[C09] 递归
来源：http://fsw.havefunace.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qxb.redwolf501.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://kyp.yanxiufei.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qgm.cqqwz.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://asg.zhixingplan.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://tpv.ctjpmb.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wbn.ywan-chungtsiang.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://gjq.dashuyun.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ktx.52xcode.cn

[C10] 变量作用域
来源：http://nmb.jiagoushi.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://xzv.fzhhl.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://vvs.jqgfzy.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mwr.ybcxt.top

TS:   同 JS
来源：http://ipe.jinyuanbaomall.cn

Java: 方法内为块级作用域
来源：http://irl.jinqigufen.top

Go:   花括号块级作用域
来源：http://usj.vehdjk.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://leg.shanyushiyangtech.top

C#:   块级作用域
来源：http://vsf.guowangkeji.top

[C11] 模块导入与导出
来源：http://bsx.yonumen.top

Py:   from module import func
来源：http://kpb.meibo888.top

PHP:  require "file.php";  或 use App\Service;
来源：http://kpb.zycfv.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://uxz.52xcode.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://sxw.bbcook.cn

Java: import java.util.List;
来源：http://clq.zycfv.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://tbh.hongshengwenyu.top

Ruby: require "json"; require_relative "./util"
来源：http://twt.quarkkingdee.top

C#:   using System.Text;
来源：http://nve.bjfxy.top

[C12] 立即执行函数 IIFE
来源：http://swq.svipenyu.cn

Py:   (lambda: print("run"))()
来源：http://smb.vehdjk.com

PHP:  (function () { echo "run"; })();
来源：http://mrp.daxiang520.top

JS:   (() => { console.log("run"); })();
来源：http://hpp.zdbjq.cn

TS:   (() => { console.log("run"); })();
来源：http://piz.wangshuangyany.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://iqb.zdqjudy.top

Go:   func() { fmt.Println("run") }()
来源：http://pxg.wangdashe.top

Ruby: -> { puts "run" }.call
来源：http://vev.c1oappe.top

C#:   // 无 IIFE：用静态构造函数
来源：http://hxu.jinyuanbaomall.cn

[C13] 类型声明 / 类型注解
来源：http://yxd.hongshengwenyu.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://bgt.chenjidiqi.icu

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fim.shangyingyoupin.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://fez.fehbvm.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pta.nwbrower.top

Java: int add(int a, int b) { return a + b; }
来源：http://ywl.shangyingyoupin.top

Go:   func add(a, b int) int
来源：http://nij.ybcxt.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://lgw.zycfv.cn

C#:   int Add(int a, int b) => a + b;
来源：http://buh.nanxinkj.top

[C14] 泛型函数
来源：http://srx.jinqigfzy.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://iwm.zhoulong.xyz

PHP:  // 无泛型
来源：http://xps.nwbrower.top

JS:   // 无泛型
来源：http://eqt.shzxlz.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ohx.jinqigfzy.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://sen.fktsv.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://zrx.iojbl.cn

Ruby: # 无泛型
来源：http://gjk.ivvv.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://bxh.hysaishi.cn

[C15] 解构 / 展开参数
来源：http://owa.nwbrower.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hxl.shuidangran.top

PHP:  [$a, $b] = $pair;
来源：http://tyo.yj202588.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mdm.sysykeji.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://oag.ydjk.org.cn

Java: // 无解构
来源：http://zkb.jyoumei.cn

Go:   // 无解构
来源：http://adb.jinqigufen.top

Ruby: a, b = pair
来源：http://fjt.aibaodan.cn

C#:   var (a, b) = pair;
来源：http://twd.jqgufenzy.top

[C16] 函数 / 方法重载
来源：http://tgz.fehbvm.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wqr.yj202588.top

PHP:  // 无重载
来源：http://huf.tanke756.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://red.mhx1999.top

TS:   // 用联合类型或重载签名声明
来源：http://sjz.ydjk.org.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://tcg.dashuyun.cn

Go:   // 无重载：用不同函数名
来源：http://zpr.meibo888.top

Ruby: # 无重载：靠动态参数
来源：http://zqx.c1oappe.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://rnj.havefunace.top

================================================================================
来源：http://nya.daria6918.cn

D. 数组 / 列表 / 集合
来源：http://nfx.sjlbkw.cn

================================================================================
来源：http://huf.jqgufenzy.top

[D01] 创建数组 / 列表
来源：http://kin.fehbvm.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://zps.zhaomingkeji.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://isk.shangyingyoupin.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://zot.gogol.net.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://zva.cashguo.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://nwn.ivvv.top

Go:   arr := []int{1, 2, 3}
来源：http://ilv.zdqjudy.top

Ruby: arr = [1, 2, 3]
来源：http://sqm.cashguo.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://cki.snrcjt.cn

[D02] 追加元素到末尾
来源：http://cfz.jinyuanbaomall.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://nnl.zhixingplan.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://irs.sufxvd.cn

JS:   arr.push(4);
来源：http://fbb.cheryme.top

TS:   arr.push(4);
来源：http://mso.ivvv.top

Java: list.add(4);
来源：http://aep.hnxiangtu.top

Go:   arr = append(arr, 4)
来源：http://miq.jqgufenzy.top

Ruby: arr << 4; arr.push(5)
来源：http://ufa.daria6918.cn

C#:   list.Add(4);
来源：http://sjh.zhijiandao.cn

[D03] 在指定位置插入元素
来源：http://ulq.chenjidiqi.icu

Py:   arr.insert(0, 0)
来源：http://xui.cashguo.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hkw.yanxiufei.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://uzd.zhiwuduotai.top

TS:   arr.splice(0, 0, 0);
来源：http://kkh.zhixingplan.top

Java: list.add(0, 0);
来源：http://nuz.fengsongda.top

Go:   arr = append([]int{0}, arr...)
来源：http://qdc.gzhubu.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://pcu.shanyushiyangtech.top

C#:   list.Insert(0, 0);
来源：http://fdm.52xcode.cn

[D04] 删除元素
来源：http://owt.aibaodan.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://nkf.zhiwuduotai.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://igu.yfazqb.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://jao.yuanzhike.top

TS:   arr.splice(0, 1);
来源：http://xdd.xingfuxueyuan.xyz

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://rzo.bbcook.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://kms.uphjek.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mjz.xuetiantiany.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wyr.tarul.cn

[D05] 访问与修改元素
来源：http://kjt.jianghu66.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://emn.gzhubu.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mnk.ehwqpu.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://lzd.jinyuanbaomall.cn

TS:   arr[0]; arr.at(-1);
来源：http://soq.tanke756.top

Java: list.get(0); list.set(0, 9);
来源：http://afd.jyoumei.cn

Go:   arr[0]; arr[0] = 9
来源：http://ndi.aizwys.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wfj.yuxming.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://jbk.yj20258.top

[D06] 数组长度
来源：http://ial.316326.xyz

Py:   len(arr)
来源：http://ouv.redwolf501.top

PHP:  count($arr);
来源：http://aaz.yuanzhike.top

JS:   arr.length
来源：http://fai.xingfuxueyuan.xyz

TS:   arr.length
来源：http://hvk.yj20258.top

Java: list.size();
来源：http://okj.yj202588.top

Go:   len(arr)
来源：http://tgj.nwbrower.top

Ruby: arr.length; arr.size
来源：http://srk.ctjpmb.com

C#:   list.Count;
来源：http://npn.yj20258888.top

[D07] 切片 / 取子数组
来源：http://dgu.yongpay.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://cop.fehbvm.com

PHP:  array_slice($arr, 1, 3);
来源：http://zvy.hesvh.cn

JS:   arr.slice(1, 4);
来源：http://vdo.shangyingyoupin.top

TS:   arr.slice(1, 4);
来源：http://bqb.havefunace.top

Java: list.subList(1, 4);
来源：http://nmq.yvedp.cn

Go:   arr[1:4]
来源：http://jwg.hnqzz.top

Ruby: arr[1, 3]
来源：http://gnd.zhaomingkeji.xyz

C#:   list.GetRange(1, 3);
来源：http://ven.ivvv.top

[D08] 合并两个数组
来源：http://top.wangdashe.top

Py:   a + b;  a.extend(b)
来源：http://jgt.snrcjt.cn

PHP:  array_merge($a, $b);
来源：http://whr.guowangkeji.top

JS:   [...a, ...b];  a.concat(b);
来源：http://ydk.hesvh.cn

TS:   [...a, ...b];
来源：http://wpq.smart0.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://git.meibo888.top

Go:   append(a, b...)
来源：http://chb.hnqzz.top

Ruby: a + b;  a.concat(b)
来源：http://vyj.yuxming.cn

C#:   a.Concat(b).ToList()
来源：http://ddn.epnwcf.com

[D09] 排序（升序）
来源：http://clu.guannengcc.top

Py:   sorted(arr);  arr.sort()
来源：http://jyz.nanxuanxn.top

PHP:  sort($arr);
来源：http://oth.wangshuangyany.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://jyk.shanyushiyangkeji.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://vao.xinyue.icu

Java: Collections.sort(list);  list.sort(null);
来源：http://bfr.chenjidiqi.icu


<!-- 参考信息 -->