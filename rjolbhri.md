代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bat.shzxlz.cn

[B10] 遍历同时拿索引
来源：http://dls.xuetiantiany.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://lqy.jinyuanbaomall.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://zfd.jqgfzy.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hzu.jiagoushi.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://qun.vqdsnc.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://qcw.ydjk.org.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://pcr.fktsv.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://sxz.aizwys.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://vcf.tianlin.xyz

[B11] 生成数字序列 / 区间
来源：http://jia.yueranfly.top

Py:   list(range(0, 10, 2))
来源：http://bwb.nanxinkj.top

PHP:  range(0, 10, 2);
来源：http://qcw.yuanzhike.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tnb.aizwys.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://aoi.mhx1999.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://yhj.yj202588.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://fhx.xziqi.cn

Ruby: (0...10).step(2).to_a
来源：http://bvp.jqgfzy.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ics.xuetiantiany.cn

[B12] 跳出多层循环
来源：http://uwm.meibo888.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://fbu.hfpthk.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://hmq.yj20258.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://tfy.fktsv.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wgk.zhijiandao.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://zov.jinyuanbaomall.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://owx.vehdjk.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://gar.fktsv.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://nwr.guowangkeji.top

[B13] 判断是否为数字
来源：http://nwl.jianghu66.top

Py:   isinstance(x, (int, float))
来源：http://nzr.cucudq.cn

PHP:  is_numeric($x)
来源：http://qrt.xuanzx.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://txo.nanxinkj.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fqd.hywenlv.cn

Java: x instanceof Number
来源：http://fwv.shzxlz.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://jkq.ybcxt.top

Ruby: x.is_a?(Numeric)
来源：http://kzr.gaohongyu789.top

C#:   x is int or double or decimal
来源：http://ybi.uphjek.com

[B14] 判断值是否在集合内
来源：http://ncw.chenzaomai.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://qvr.kuanghao11.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ynl.yonumen.top

JS:   [1, 2, 3].includes(x)
来源：http://uhr.meibo888.top

TS:   [1, 2, 3].includes(x)
来源：http://dkk.zycfv.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://suk.yangfankeji.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://qmq.nanxinkj.top

Ruby: [1, 2, 3].include?(x)
来源：http://gqh.hcnkem.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://atd.smart0.xyz

[B15] 布尔运算与取反
来源：http://fnp.ppjwa.cn

Py:   a and b or not c
来源：http://gqo.shzxlz.cn

PHP:  $a && $b || !$c
来源：http://nxu.xingfuxueyuan.xyz

JS:   a && b || !c
来源：http://vbx.yuanzhike.top

TS:   a && b || !c
来源：http://nuj.shanyushiyangtech.top

Java: a && b || !c
来源：http://xjz.gotoacloud.top

Go:   a && b || !c
来源：http://ozb.dashuyun.cn

Ruby: a && b || !c
来源：http://cbf.chenjidiqi.icu

C#:   a && b || !c
来源：http://gzl.ctjpmb.com

[B16] 卫语句：不满足条件提前返回
来源：http://uwl.jianghu66.top

Py:   if not data: return
来源：http://pcm.yuxming.cn

PHP:  if (!$data) { return; }
来源：http://oie.wangshuangyany.cn

JS:   if (!data) return;
来源：http://tbi.shuidangran.top

TS:   if (!data) return;
来源：http://mtu.redwolf501.top

Java: if (data == null) return;
来源：http://cce.yueranfly.top

Go:   if data == nil { return }
来源：http://plp.aibaodan.cn

Ruby: return if data.nil?
来源：http://jhx.xuetiantiany.cn

C#:   if (data == null) return;
来源：http://ibe.pengpengdd.cyou

================================================================================
来源：http://rnb.nanxuanxn.top

C. 函数与作用域
来源：http://chw.shangyingyoupin.top

================================================================================
来源：http://oue.fehbvm.com

[C01] 定义函数
来源：http://kma.redwolf501.top

Py:   def add(a, b): return a + b
来源：http://ofy.nanxuanxn.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mdd.bjfxy.top

JS:   function add(a, b) { return a + b; }
来源：http://blz.snrcjt.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mpp.jianghu66.top

Java: static int add(int a, int b) { return a + b; }
来源：http://lhd.guannengcc.top

Go:   func add(a, b int) int { return a + b }
来源：http://qem.zhengqikj.top

Ruby: def add(a, b); a + b; end
来源：http://jqq.hnqzz.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://odi.guowangkeji.top

[C02] 默认参数
来源：http://bue.zhixingplan.top

Py:   def greet(name="World"): return name
来源：http://kbh.shuidangran.top

PHP:  function greet($name = "World") { return $name; }
来源：http://xkz.tanke756.top

JS:   function greet(name = "World") { return name; }
来源：http://ytf.jqgufenzy.top

TS:   function greet(name: string = "World") { return name; }
来源：http://zod.andypj.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://knc.vehdjk.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://dlj.tarul.cn

Ruby: def greet(name = "World") = name
来源：http://val.daria6918.cn

C#:   string Greet(string name = "World") => name;
来源：http://nlu.kuanghao11.cn

[C03] 可变参数
来源：http://sua.yfazqb.com

Py:   def total(*args): return sum(args)
来源：http://txg.bbcook.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://dsi.jiagoushi.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://gih.c1oappe.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://zws.xingfuxueyuan.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://jxw.ehwqpu.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://chm.pycfn.com

Ruby: def total(*nums); nums.sum; end
来源：http://qpp.birdmap.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://tid.chenjidiqi.icu

[C04] 命名参数 / 关键字参数
来源：http://mwb.jqgufenzy.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://jem.birdmap.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://lky.gaohongyu789.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mvp.jinghuilouyu.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://jyr.zhengqikj.top

Java: // 无：用 Builder 模式或 record
来源：http://drg.jinghuilouyu.cn

Go:   // 无：用配置结构体参数
来源：http://zxo.hesvh.cn

Ruby: f(a: 1, b: 2)
来源：http://frn.yvedp.cn

C#:   f(a: 1, b: 2)
来源：http://jbh.jiagoushi.top

[C05] 返回多个值
来源：http://rmg.c1oappe.top

Py:   return a, b
来源：http://dcs.zdbjq.cn

PHP:  return [$a, $b];
来源：http://iox.yj20258888.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://wbx.havefunace.top

TS:   return { a, b };
来源：http://zzq.pycfn.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xcd.fehbvm.com

Go:   return a, b
来源：http://hrv.guannengcc.top

Ruby: return a, b
来源：http://mrp.nanxinkj.top

C#:   return (a, b);              // ValueTuple
来源：http://wfj.zhongyouzk.top

[C06] 匿名函数 / lambda
来源：http://cjx.vehdjk.com

Py:   square = lambda x: x * x
来源：http://kwq.dianchejie.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://yww.andypj.xyz

JS:   const square = x => x * x;
来源：http://ucp.cdnleiting.top

TS:   const square = (x: number): number => x * x;
来源：http://vzt.dianchejie.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://bgz.yongpay.top

Go:   sq := func(x int) int { return x * x }
来源：http://svz.cucudq.cn

Ruby: square = ->(x) { x * x }
来源：http://vuc.iojbl.cn

C#:   Func<int, int> square = x => x * x;
来源：http://jjf.0kj1m.cn

[C07] 把函数作为参数传入
来源：http://knw.gzhubu.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://knx.yangfankeji.com

PHP:  array_map("strtoupper", $arr);
来源：http://yjm.nanxinkj.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://clp.cucudq.cn

TS:   arr.map(String)
来源：http://zos.hcnkem.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://jou.yuanzhike.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://enx.zhijiandao.cn

Ruby: arr.map(&:upcase)
来源：http://fdv.xingfuxueyuan.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://lyp.smart0.xyz

[C08] 闭包
来源：http://vap.nanxinkj.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://rgr.jinqigfzy.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ugu.52xcode.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://nqw.vehdjk.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wkb.hesvh.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hid.xuetiantiany.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://fyd.hfpthk.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://njz.ybcxt.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://drb.epnwcf.com

[C09] 递归
来源：http://gse.shangyingyoupin.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://phw.bbcook.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://vxe.jinghuilouyu.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dah.zhoulong.xyz

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ztz.xylfe.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://alo.svipenyu.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://vji.tarul.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://lsi.yuanzhike.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://nhy.aizwys.cn

[C10] 变量作用域
来源：http://baj.pengpengdd.cyou

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://bja.chenzaomai.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hmn.hnxiangtu.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://zzk.hnxiangtu.top

TS:   同 JS
来源：http://sxs.feifeiyinyue.top

Java: 方法内为块级作用域
来源：http://pud.guannengcc.top

Go:   花括号块级作用域
来源：http://uds.jinqigufen.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ckq.dianchejie.cn

C#:   块级作用域
来源：http://wpa.yongpay.top

[C11] 模块导入与导出
来源：http://vym.iojbl.cn

Py:   from module import func
来源：http://lmq.hesvh.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://txh.fzhhl.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://mhw.vehdjk.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xyy.shuidangran.top

Java: import java.util.List;
来源：http://xnh.yangfankeji.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://uwl.fehbvm.com

Ruby: require "json"; require_relative "./util"
来源：http://qda.ydzc1.top

C#:   using System.Text;
来源：http://owa.hfpthk.cn

[C12] 立即执行函数 IIFE
来源：http://woy.bbcook.cn

Py:   (lambda: print("run"))()
来源：http://jnq.shzxlz.cn

PHP:  (function () { echo "run"; })();
来源：http://rvy.shzxlz.cn

JS:   (() => { console.log("run"); })();
来源：http://eri.cucudq.cn

TS:   (() => { console.log("run"); })();
来源：http://ihe.fanxiaobao.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://elz.andypj.xyz

Go:   func() { fmt.Println("run") }()
来源：http://mxz.shangyingyoupin.top

Ruby: -> { puts "run" }.call
来源：http://ajb.zhiwuduotai.top

C#:   // 无 IIFE：用静态构造函数
来源：http://usa.yvedp.cn

[C13] 类型声明 / 类型注解
来源：http://baa.daxiang520.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mzr.pengpengdd.cyou

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://avf.nwbrower.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hsx.bjfxy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rht.gogol.net.cn

Java: int add(int a, int b) { return a + b; }
来源：http://zda.316326.xyz

Go:   func add(a, b int) int
来源：http://jme.cdnleiting.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hwo.fzhhl.top

C#:   int Add(int a, int b) => a + b;
来源：http://oxw.wangdashe.top

[C14] 泛型函数
来源：http://bcg.zhiwuduotai.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ekv.zdqjudy.top

PHP:  // 无泛型
来源：http://suv.daria6918.cn

JS:   // 无泛型
来源：http://szr.sufxvd.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://luz.52xcode.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://cyo.wangdashe.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://eir.yonumen.top

Ruby: # 无泛型
来源：http://dna.jianghu66.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://clw.hfpthk.cn

[C15] 解构 / 展开参数
来源：http://whd.ydjk.org.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://qqs.jlsjyb.cn

PHP:  [$a, $b] = $pair;
来源：http://lfw.dianchejie.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://vtq.yj20258.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://sdc.svipenyu.cn

Java: // 无解构
来源：http://oyd.zhijiandao.cn

Go:   // 无解构
来源：http://jel.dashuyun.cn

Ruby: a, b = pair
来源：http://wif.fktsv.cn

C#:   var (a, b) = pair;
来源：http://zlf.nanxinkj.top

[C16] 函数 / 方法重载
来源：http://zsz.ivvv.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://bka.zhixingplan.top

PHP:  // 无重载
来源：http://kki.daria6918.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://xhx.nwbrower.top

TS:   // 用联合类型或重载签名声明
来源：http://ioq.zdbjq.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://xzv.aizwys.cn

Go:   // 无重载：用不同函数名
来源：http://inv.sysykeji.top

Ruby: # 无重载：靠动态参数
来源：http://mml.mhx1999.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://hbc.zhixingplan.top

================================================================================
来源：http://axn.gotoacloud.top

D. 数组 / 列表 / 集合
来源：http://jnx.jlsjyb.cn

================================================================================
来源：http://lsm.mhx1999.top

[D01] 创建数组 / 列表
来源：http://kfz.fktsv.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://aly.fzhhl.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://fpn.xziqi.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://lts.yj20258.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://hnx.hnxiangtu.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://yrx.c1oappe.top

Go:   arr := []int{1, 2, 3}
来源：http://dpj.gotoacloud.top

Ruby: arr = [1, 2, 3]
来源：http://gxa.jinyuanbaomall.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ivg.shanyushiyangkeji.top

[D02] 追加元素到末尾
来源：http://igs.jianghu66.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://vut.zhixingplan.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ahe.chenjidiqi.icu

JS:   arr.push(4);
来源：http://lec.ctjpmb.com

TS:   arr.push(4);
来源：http://cmo.haohaochexian.top

Java: list.add(4);
来源：http://npj.c1oappe.top

Go:   arr = append(arr, 4)
来源：http://qhy.zhaomingkeji.xyz

Ruby: arr << 4; arr.push(5)
来源：http://rpi.zhiwuduotai.top

C#:   list.Add(4);
来源：http://eab.cqqwz.cn

[D03] 在指定位置插入元素
来源：http://gdg.yuanzhike.top

Py:   arr.insert(0, 0)
来源：http://ydq.xuanzx.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://uut.hammf.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://fkj.ydzc1.top

TS:   arr.splice(0, 0, 0);
来源：http://qrk.snrcjt.cn

Java: list.add(0, 0);
来源：http://bat.zdqjudy.top

Go:   arr = append([]int{0}, arr...)
来源：http://zzk.guannengcc.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://pqp.tanke756.top

C#:   list.Insert(0, 0);
来源：http://ewk.uphjek.com

[D04] 删除元素
来源：http://hlj.yuxming.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://kcd.jiagoushi.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mdu.haohaochexian.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://vsz.fengsongda.top

TS:   arr.splice(0, 1);
来源：http://fet.haohaochexian.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wkt.nwbrower.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://svj.xylfe.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://dgx.ydjk.org.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://qjg.yongpay.top

[D05] 访问与修改元素
来源：http://ttd.tarul.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ndt.gogol.net.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ifn.xziqi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://xhn.yueranfly.top

TS:   arr[0]; arr.at(-1);
来源：http://rtk.xuetiantiany.cn

Java: list.get(0); list.set(0, 9);
来源：http://ntl.kuanghao11.cn

Go:   arr[0]; arr[0] = 9
来源：http://aqa.ydzc1.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://vff.hfpthk.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://vrc.52xcode.cn

[D06] 数组长度
来源：http://zks.gotoacloud.top

Py:   len(arr)
来源：http://vgb.nanxinkj.top

PHP:  count($arr);
来源：http://ywn.shangyingyoupin.top

JS:   arr.length
来源：http://bka.ywan-chungtsiang.top

TS:   arr.length
来源：http://ibx.kuanghao11.cn

Java: list.size();
来源：http://kjj.fktsv.cn

Go:   len(arr)
来源：http://kts.yangfankeji.com

Ruby: arr.length; arr.size
来源：http://enl.c1oappe.top

C#:   list.Count;
来源：http://yla.jqgufenzy.top

[D07] 切片 / 取子数组
来源：http://kyw.zhoulong.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://kaa.jiagoushi.top

PHP:  array_slice($arr, 1, 3);
来源：http://lqh.jinghuilouyu.cn

JS:   arr.slice(1, 4);
来源：http://tgr.dashuyun.cn

TS:   arr.slice(1, 4);
来源：http://cxc.jlsjyb.cn

Java: list.subList(1, 4);
来源：http://xbb.aibaodan.cn

Go:   arr[1:4]
来源：http://iiv.yangfankeji.com

Ruby: arr[1, 3]
来源：http://jem.sweek.top

C#:   list.GetRange(1, 3);
来源：http://obf.haohaochexian.top

[D08] 合并两个数组
来源：http://htj.fktsv.cn

Py:   a + b;  a.extend(b)
来源：http://dqg.0kj1m.cn

PHP:  array_merge($a, $b);
来源：http://neb.yj20258888.top

JS:   [...a, ...b];  a.concat(b);
来源：http://bsi.daria6918.cn

TS:   [...a, ...b];
来源：http://bmy.daxiang520.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hxd.nwbrower.top

Go:   append(a, b...)
来源：http://lyd.yvedp.cn

Ruby: a + b;  a.concat(b)
来源：http://lkk.nanxinkj.top

C#:   a.Concat(b).ToList()
来源：http://dwo.jinqigufen.top

[D09] 排序（升序）
来源：http://svy.feifeiyinyue.top

Py:   sorted(arr);  arr.sort()
来源：http://uar.gogol.net.cn

PHP:  sort($arr);
来源：http://atk.pengpengdd.cyou

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mvk.kuanghao11.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://qdf.jqgufenzy.top

Java: Collections.sort(list);  list.sort(null);
来源：http://nmy.nwbrower.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ppa.shangyingyoupin.top

Ruby: arr.sort
来源：http://cnx.zhoulong.xyz

C#:   list.Sort();
来源：http://har.yangfankeji.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://ken.jlsjyb.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://xoj.yj202588.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mzj.jianghu66.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://elg.andypj.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mcc.chenzaomai.com


<!-- 参考信息 -->