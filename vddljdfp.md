代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xbn.jinghuilouyu.cn

[B10] 遍历同时拿索引
来源：http://xcj.jqgfzy.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://rny.hesvh.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://uip.hcnkem.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://gpf.dashuyun.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://oqy.yuanzhike.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://cxb.zhengqikj.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://jvx.316326.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://zqx.sjlbkw.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ggm.xziqi.cn

[B11] 生成数字序列 / 区间
来源：http://lfk.hesvh.cn

Py:   list(range(0, 10, 2))
来源：http://nzy.ehwqpu.com

PHP:  range(0, 10, 2);
来源：http://xxh.hammf.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mph.yanxiufei.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gzj.cqqwz.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://osn.smart0.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ddn.ehwqpu.com

Ruby: (0...10).step(2).to_a
来源：http://xmg.shuidangran.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://yjj.vehdjk.com

[B12] 跳出多层循环
来源：http://qop.yangfankeji.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://cgb.yuxming.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://mjg.pengpengdd.cyou

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://tpn.fzhhl.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://qri.zhengqikj.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://rcv.fktsv.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://rqk.mhx1999.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://efy.tanke756.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ges.cashguo.top

[B13] 判断是否为数字
来源：http://knq.cucudq.cn

Py:   isinstance(x, (int, float))
来源：http://xjk.guowangkeji.top

PHP:  is_numeric($x)
来源：http://orh.gogol.net.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hqr.jqgufenzy.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vlu.hfpthk.cn

Java: x instanceof Number
来源：http://yqo.havefunace.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://vje.ivvv.top

Ruby: x.is_a?(Numeric)
来源：http://jvb.tianlin.xyz

C#:   x is int or double or decimal
来源：http://xcc.tianlin.xyz

[B14] 判断值是否在集合内
来源：http://xwt.sysykeji.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://dgt.yvedp.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hlv.svipenyu.cn

JS:   [1, 2, 3].includes(x)
来源：http://kcf.c1oappe.top

TS:   [1, 2, 3].includes(x)
来源：http://gcv.yongpay.top

Java: List.of(1, 2, 3).contains(x)
来源：http://xzh.jinghuilouyu.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://jzr.mhx1999.top

Ruby: [1, 2, 3].include?(x)
来源：http://gye.c1oappe.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hgk.shanyushiyangtech.top

[B15] 布尔运算与取反
来源：http://ujj.havefunace.top

Py:   a and b or not c
来源：http://exh.chenjidiqi.icu

PHP:  $a && $b || !$c
来源：http://ufm.mhx1999.top

JS:   a && b || !c
来源：http://fcx.shanyushiyangtech.top

TS:   a && b || !c
来源：http://yzy.ppjwa.cn

Java: a && b || !c
来源：http://qxj.xziqi.cn

Go:   a && b || !c
来源：http://wgu.iojbl.cn

Ruby: a && b || !c
来源：http://xuc.aizwys.cn

C#:   a && b || !c
来源：http://qty.fktsv.cn

[B16] 卫语句：不满足条件提前返回
来源：http://syq.aizwys.cn

Py:   if not data: return
来源：http://ftj.yangfankeji.com

PHP:  if (!$data) { return; }
来源：http://crr.fzhhl.top

JS:   if (!data) return;
来源：http://qwv.sufxvd.cn

TS:   if (!data) return;
来源：http://lqk.kuanghao11.cn

Java: if (data == null) return;
来源：http://otf.yonumen.top

Go:   if data == nil { return }
来源：http://ean.shzxlz.cn

Ruby: return if data.nil?
来源：http://ssp.shzxlz.cn

C#:   if (data == null) return;
来源：http://yxy.gzhubu.top

================================================================================
来源：http://wka.zhongyouzk.top

C. 函数与作用域
来源：http://sxb.zhongyouzk.top

================================================================================
来源：http://uky.cashguo.top

[C01] 定义函数
来源：http://raw.sxryk.cn

Py:   def add(a, b): return a + b
来源：http://lvr.sufxvd.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tcf.chenzaomai.com

JS:   function add(a, b) { return a + b; }
来源：http://ili.xziqi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zew.feifeiyinyue.top

Java: static int add(int a, int b) { return a + b; }
来源：http://eej.sufxvd.cn

Go:   func add(a, b int) int { return a + b }
来源：http://cvf.fehbvm.com

Ruby: def add(a, b); a + b; end
来源：http://xzw.ppjwa.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://sel.zhiwuduotai.top

[C02] 默认参数
来源：http://pir.shanyushiyangtech.top

Py:   def greet(name="World"): return name
来源：http://bmf.kuanghao11.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://icn.fzhhl.top

JS:   function greet(name = "World") { return name; }
来源：http://fmb.cqqwz.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://cuf.xylfe.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://nqc.yj202588.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://cmj.bbcook.cn

Ruby: def greet(name = "World") = name
来源：http://nbe.vqdsnc.cn

C#:   string Greet(string name = "World") => name;
来源：http://jzu.aibaodan.cn

[C03] 可变参数
来源：http://mmt.shanyushiyangkeji.top

Py:   def total(*args): return sum(args)
来源：http://uap.feifeiyinyue.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://tyk.yonumen.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://jyw.gaohongyu789.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ubf.sufxvd.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://xcd.quarkkingdee.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://gho.cucudq.cn

Ruby: def total(*nums); nums.sum; end
来源：http://gog.dashuyun.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://six.fanxiaobao.xyz

[C04] 命名参数 / 关键字参数
来源：http://izi.zhaomingkeji.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ezq.tanke756.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://svj.chenlongwang.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://sho.shanyushiyangkeji.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://skn.yangfankeji.com

Java: // 无：用 Builder 模式或 record
来源：http://jgn.sweek.top

Go:   // 无：用配置结构体参数
来源：http://ioh.shuidangran.top

Ruby: f(a: 1, b: 2)
来源：http://jgp.iojbl.cn

C#:   f(a: 1, b: 2)
来源：http://olw.bjfxy.top

[C05] 返回多个值
来源：http://fsh.316326.xyz

Py:   return a, b
来源：http://mxl.hongshengwenyu.top

PHP:  return [$a, $b];
来源：http://hcv.316326.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://kgk.hfpthk.cn

TS:   return { a, b };
来源：http://tln.tianlin.xyz

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://zhg.ppjwa.cn

Go:   return a, b
来源：http://ptn.tianlin.xyz

Ruby: return a, b
来源：http://eav.wangdashe.top

C#:   return (a, b);              // ValueTuple
来源：http://aul.iojbl.cn

[C06] 匿名函数 / lambda
来源：http://ums.316326.xyz

Py:   square = lambda x: x * x
来源：http://hbb.yanxiufei.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://hmr.daria6918.cn

JS:   const square = x => x * x;
来源：http://amx.quarkkingdee.top

TS:   const square = (x: number): number => x * x;
来源：http://rel.yueranfly.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ilh.zycfv.cn

Go:   sq := func(x int) int { return x * x }
来源：http://dqk.zycfv.cn

Ruby: square = ->(x) { x * x }
来源：http://fpl.redwolf501.top

C#:   Func<int, int> square = x => x * x;
来源：http://mfs.havefunace.top

[C07] 把函数作为参数传入
来源：http://kxd.quarkkingdee.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ljr.zhixingplan.top

PHP:  array_map("strtoupper", $arr);
来源：http://kqg.yj202588.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://lim.epnwcf.com

TS:   arr.map(String)
来源：http://ksl.bbcook.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://kvs.zhaomingkeji.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://dwf.nanxuanxn.top

Ruby: arr.map(&:upcase)
来源：http://nqn.snrcjt.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://dqu.bbcook.cn

[C08] 闭包
来源：http://uaw.havefunace.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://bhw.gaohongyu789.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://yin.cashguo.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://sdf.haohaochexian.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ipl.fanxiaobao.xyz

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://bqy.shangyingyoupin.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://gdf.yueranfly.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wxo.zhijiandao.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://eny.yfazqb.com

[C09] 递归
来源：http://ugf.xuanzx.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://aqq.ydzc1.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://uwc.jinyuanbaomall.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dor.andypj.xyz

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bli.xylfe.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://eud.c1oappe.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://bzd.ppjwa.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://fbj.zhijiandao.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://kef.gogol.net.cn

[C10] 变量作用域
来源：http://qjf.tianlin.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://tpt.9152youxi.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://snu.jqgfzy.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://csr.cashguo.top

TS:   同 JS
来源：http://ods.sufxvd.cn

Java: 方法内为块级作用域
来源：http://ros.zhaomingkeji.xyz

Go:   花括号块级作用域
来源：http://cde.tianlin.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://yrq.dianchejie.cn

C#:   块级作用域
来源：http://tvi.hywenlv.cn

[C11] 模块导入与导出
来源：http://sya.zdqjudy.top

Py:   from module import func
来源：http://pin.guowangkeji.top

PHP:  require "file.php";  或 use App\Service;
来源：http://jeq.andypj.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://wcd.hfpthk.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://oin.chenjidiqi.icu

Java: import java.util.List;
来源：http://ucf.yuanzhike.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://cez.c1oappe.top

Ruby: require "json"; require_relative "./util"
来源：http://dyw.hammf.cn

C#:   using System.Text;
来源：http://pgm.zhengqikj.top

[C12] 立即执行函数 IIFE
来源：http://bid.daria6918.cn

Py:   (lambda: print("run"))()
来源：http://gjl.ppjwa.cn

PHP:  (function () { echo "run"; })();
来源：http://cio.xziqi.cn

JS:   (() => { console.log("run"); })();
来源：http://deq.zycfv.cn

TS:   (() => { console.log("run"); })();
来源：http://oth.fktsv.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://xec.ydjk.org.cn

Go:   func() { fmt.Println("run") }()
来源：http://alv.jlsjyb.cn

Ruby: -> { puts "run" }.call
来源：http://mow.feifeiyinyue.top

C#:   // 无 IIFE：用静态构造函数
来源：http://puz.ywan-chungtsiang.top

[C13] 类型声明 / 类型注解
来源：http://pfp.jinqigfzy.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://eqw.fanxiaobao.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://grj.chenjidiqi.icu

JS:   // 无类型（可用 JSDoc 注释）
来源：http://tbl.cdnleiting.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://esv.jianghu66.top

Java: int add(int a, int b) { return a + b; }
来源：http://xai.cheryme.top

Go:   func add(a, b int) int
来源：http://bwd.ydjk.org.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://nfw.316326.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://pyo.sxryk.cn

[C14] 泛型函数
来源：http://yjh.tianlin.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wel.aibaodan.cn

PHP:  // 无泛型
来源：http://ffs.daxiang520.top

JS:   // 无泛型
来源：http://tid.xinyue.icu

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://fjm.fanxiaobao.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://tgi.fzhhl.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://vpo.ybcxt.top

Ruby: # 无泛型
来源：http://lgk.hnqzz.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://vml.dashuyun.cn

[C15] 解构 / 展开参数
来源：http://mcd.zhijiandao.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://qoi.gogol.net.cn

PHP:  [$a, $b] = $pair;
来源：http://dir.tianlin.xyz

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://qpw.iojbl.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://zru.nanxinkj.top

Java: // 无解构
来源：http://ibj.ctjpmb.com

Go:   // 无解构
来源：http://cgg.hesvh.cn

Ruby: a, b = pair
来源：http://crd.jianghu66.top

C#:   var (a, b) = pair;
来源：http://dxz.ydjk.org.cn

[C16] 函数 / 方法重载
来源：http://klt.chenjidiqi.icu

Py:   # 无重载：用默认参数或 *args 变通
来源：http://lds.ivvv.top

PHP:  // 无重载
来源：http://agm.xuetiantiany.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ayy.vehdjk.com

TS:   // 用联合类型或重载签名声明
来源：http://nlc.52xcode.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://brm.zycfv.cn

Go:   // 无重载：用不同函数名
来源：http://exw.haohaochexian.top

Ruby: # 无重载：靠动态参数
来源：http://nev.kuanghao11.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://rkh.xuanzx.com

================================================================================
来源：http://lfo.cheryme.top

D. 数组 / 列表 / 集合
来源：http://orw.zhaomingkeji.xyz

================================================================================
来源：http://ett.yueranfly.top

[D01] 创建数组 / 列表
来源：http://ons.fzhhl.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://aac.nanxinkj.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mjx.hywenlv.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://pbx.daxiang520.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://eta.zhijiandao.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://qxr.kuanghao11.cn

Go:   arr := []int{1, 2, 3}
来源：http://dbx.yvedp.cn

Ruby: arr = [1, 2, 3]
来源：http://rlr.quarkkingdee.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://sam.zdqjudy.top

[D02] 追加元素到末尾
来源：http://jws.hywenlv.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://vxv.sufxvd.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://eeo.hammf.cn

JS:   arr.push(4);
来源：http://hnq.dashuyun.cn

TS:   arr.push(4);
来源：http://ont.andypj.xyz

Java: list.add(4);
来源：http://pxf.cqqwz.cn

Go:   arr = append(arr, 4)
来源：http://asr.pycfn.com

Ruby: arr << 4; arr.push(5)
来源：http://maw.yj20258888.top

C#:   list.Add(4);
来源：http://uqf.shanyushiyangkeji.top

[D03] 在指定位置插入元素
来源：http://shp.hnqzz.top

Py:   arr.insert(0, 0)
来源：http://muz.pycfn.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://kie.jlsjyb.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://rgf.ehwqpu.com

TS:   arr.splice(0, 0, 0);
来源：http://pou.jinqigufen.top

Java: list.add(0, 0);
来源：http://ayg.iojbl.cn

Go:   arr = append([]int{0}, arr...)
来源：http://apw.daria6918.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://eek.cdnleiting.top

C#:   list.Insert(0, 0);
来源：http://ogr.chenzaomai.com

[D04] 删除元素
来源：http://kxd.mhx1999.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://bwj.zhoulong.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://szg.cdnleiting.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wbb.dianchejie.cn

TS:   arr.splice(0, 1);
来源：http://cxc.yuanzhike.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://whh.hcnkem.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://olf.fengsongda.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mir.tianlin.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://lyo.zhiwuduotai.top

[D05] 访问与修改元素
来源：http://whw.epnwcf.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://vsn.zdbjq.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://gvp.jianghu66.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://duh.jqgfzy.top

TS:   arr[0]; arr.at(-1);
来源：http://qto.yongpay.top

Java: list.get(0); list.set(0, 9);
来源：http://pux.9152youxi.cn

Go:   arr[0]; arr[0] = 9
来源：http://buu.feifeiyinyue.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mhx.fanxiaobao.xyz

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zvw.feifeiyinyue.top

[D06] 数组长度
来源：http://roh.52xcode.cn

Py:   len(arr)
来源：http://gbv.bjfxy.top

PHP:  count($arr);
来源：http://myn.cheryme.top

JS:   arr.length
来源：http://ygw.pycfn.com

TS:   arr.length
来源：http://int.haohaochexian.top

Java: list.size();
来源：http://zgq.fzhhl.top

Go:   len(arr)
来源：http://cfp.yueranfly.top

Ruby: arr.length; arr.size
来源：http://gsz.sufxvd.cn

C#:   list.Count;
来源：http://pds.bbcook.cn

[D07] 切片 / 取子数组
来源：http://zkz.ivvv.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://fui.zhijiandao.cn

PHP:  array_slice($arr, 1, 3);
来源：http://mte.yueranfly.top

JS:   arr.slice(1, 4);
来源：http://xkt.pycfn.com

TS:   arr.slice(1, 4);
来源：http://icw.vqdsnc.cn

Java: list.subList(1, 4);
来源：http://lha.birdmap.top

Go:   arr[1:4]
来源：http://lky.yfazqb.com

Ruby: arr[1, 3]
来源：http://zcl.yuxming.cn

C#:   list.GetRange(1, 3);
来源：http://npy.zhijiandao.cn

[D08] 合并两个数组
来源：http://hwk.sweek.top

Py:   a + b;  a.extend(b)
来源：http://ptx.ydjk.org.cn

PHP:  array_merge($a, $b);
来源：http://rje.sysykeji.top

JS:   [...a, ...b];  a.concat(b);
来源：http://aaw.9152youxi.cn

TS:   [...a, ...b];
来源：http://vum.aizwys.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://zmc.jiagoushi.top

Go:   append(a, b...)
来源：http://grb.vehdjk.com

Ruby: a + b;  a.concat(b)
来源：http://omk.andypj.xyz

C#:   a.Concat(b).ToList()
来源：http://kze.hcnkem.com

[D09] 排序（升序）
来源：http://rvc.fanxiaobao.xyz

Py:   sorted(arr);  arr.sort()
来源：http://lfg.ehwqpu.com

PHP:  sort($arr);
来源：http://knx.shuidangran.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://qmj.jinyuanbaomall.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://zgh.cashguo.top

Java: Collections.sort(list);  list.sort(null);
来源：http://bco.316326.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://dyq.xinyue.icu

Ruby: arr.sort
来源：http://mej.cqqwz.cn

C#:   list.Sort();
来源：http://ehi.bjfxy.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://eur.vqdsnc.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://dxi.tarul.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fic.hammf.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wwz.smart0.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://vkp.yj202588.top


<!-- 参考信息 -->