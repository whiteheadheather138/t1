代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fnd.tanke756.top

[B10] 遍历同时拿索引
来源：http://byt.yj202588.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://tcv.yanxiufei.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://aqf.zhixingplan.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://vcz.jqgfzy.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mkg.yj20258.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mfn.ydjk.org.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://oqc.daria6918.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://jma.nanxuanxn.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wmp.zdqjudy.top

[B11] 生成数字序列 / 区间
来源：http://wiz.ehwqpu.com

Py:   list(range(0, 10, 2))
来源：http://deh.ydzc1.top

PHP:  range(0, 10, 2);
来源：http://ogt.nwbrower.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nnm.vqdsnc.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xim.yuanzhike.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://icl.ydjk.org.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://dmx.birdmap.top

Ruby: (0...10).step(2).to_a
来源：http://crt.iojbl.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://pth.zdqjudy.top

[B12] 跳出多层循环
来源：http://vor.ydjk.org.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://bke.ydzc1.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://mdl.zycfv.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mrh.yanxiufei.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://tvq.shuidangran.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://amm.redwolf501.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://uly.xylfe.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://rut.redwolf501.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://abp.ppjwa.cn

[B13] 判断是否为数字
来源：http://lhi.chenjidiqi.icu

Py:   isinstance(x, (int, float))
来源：http://mwh.iojbl.cn

PHP:  is_numeric($x)
来源：http://qwd.jianghu66.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rdc.hammf.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://phb.ppjwa.cn

Java: x instanceof Number
来源：http://kco.yanxiufei.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://slz.ybcxt.top

Ruby: x.is_a?(Numeric)
来源：http://pxe.jiagoushi.top

C#:   x is int or double or decimal
来源：http://jow.hammf.cn

[B14] 判断值是否在集合内
来源：http://rcm.feifeiyinyue.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ykl.jinghuilouyu.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://bmt.316326.xyz

JS:   [1, 2, 3].includes(x)
来源：http://kyn.epnwcf.com

TS:   [1, 2, 3].includes(x)
来源：http://imr.hywenlv.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ybe.jqgfzy.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://knx.yuxming.cn

Ruby: [1, 2, 3].include?(x)
来源：http://omy.jinghuilouyu.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://yps.hysaishi.cn

[B15] 布尔运算与取反
来源：http://pco.hywenlv.cn

Py:   a and b or not c
来源：http://yao.nanxuanxn.top

PHP:  $a && $b || !$c
来源：http://lat.snrcjt.cn

JS:   a && b || !c
来源：http://qcc.haohaochexian.top

TS:   a && b || !c
来源：http://kwb.shanyushiyangkeji.top

Java: a && b || !c
来源：http://rro.52xcode.cn

Go:   a && b || !c
来源：http://rod.zdbjq.cn

Ruby: a && b || !c
来源：http://qjw.ywan-chungtsiang.top

C#:   a && b || !c
来源：http://wkg.xingfuxueyuan.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://ksa.yueranfly.top

Py:   if not data: return
来源：http://wxu.yfazqb.com

PHP:  if (!$data) { return; }
来源：http://trv.fehbvm.com

JS:   if (!data) return;
来源：http://gtl.fehbvm.com

TS:   if (!data) return;
来源：http://azs.svipenyu.cn

Java: if (data == null) return;
来源：http://cdq.jqgufenzy.top

Go:   if data == nil { return }
来源：http://wja.fktsv.cn

Ruby: return if data.nil?
来源：http://ioo.bjfxy.top

C#:   if (data == null) return;
来源：http://dys.pycfn.com

================================================================================
来源：http://yua.jianghu66.top

C. 函数与作用域
来源：http://snl.daria6918.cn

================================================================================
来源：http://drn.ydjk.org.cn

[C01] 定义函数
来源：http://xme.pycfn.com

Py:   def add(a, b): return a + b
来源：http://phl.jyoumei.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://uit.gotoacloud.top

JS:   function add(a, b) { return a + b; }
来源：http://obp.yuanzhike.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tdn.zhixingplan.top

Java: static int add(int a, int b) { return a + b; }
来源：http://kif.zhiwuduotai.top

Go:   func add(a, b int) int { return a + b }
来源：http://fhb.hesvh.cn

Ruby: def add(a, b); a + b; end
来源：http://ndr.yvedp.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://bur.redwolf501.top

[C02] 默认参数
来源：http://prm.hfpthk.cn

Py:   def greet(name="World"): return name
来源：http://fxr.snrcjt.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://lnv.sxryk.cn

JS:   function greet(name = "World") { return name; }
来源：http://pcd.sxryk.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://hpc.ybcxt.top

Java: // 无默认参数：方法重载或 Optional
来源：http://sqt.zhaomingkeji.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://gkv.cheryme.top

Ruby: def greet(name = "World") = name
来源：http://yrl.cdnleiting.top

C#:   string Greet(string name = "World") => name;
来源：http://jwp.zhongyouzk.top

[C03] 可变参数
来源：http://kwx.hfpthk.cn

Py:   def total(*args): return sum(args)
来源：http://cyz.52xcode.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://kln.andypj.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mkq.hnqzz.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://tft.xylfe.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ocd.xylfe.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://dgj.zdqjudy.top

Ruby: def total(*nums); nums.sum; end
来源：http://eka.yfazqb.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://lhh.hysaishi.cn

[C04] 命名参数 / 关键字参数
来源：http://gba.hysaishi.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://kqb.smart0.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mzr.zhongyouzk.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://uhi.hfpthk.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://yts.shangyingyoupin.top

Java: // 无：用 Builder 模式或 record
来源：http://ofw.guowangkeji.top

Go:   // 无：用配置结构体参数
来源：http://fwu.shangyingyoupin.top

Ruby: f(a: 1, b: 2)
来源：http://nsw.uphjek.com

C#:   f(a: 1, b: 2)
来源：http://pgi.nanxinkj.top

[C05] 返回多个值
来源：http://hdt.andypj.xyz

Py:   return a, b
来源：http://bsz.dianchejie.cn

PHP:  return [$a, $b];
来源：http://wmp.daria6918.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ujk.jinqigufen.top

TS:   return { a, b };
来源：http://ocl.yangfankeji.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://sfe.hesvh.cn

Go:   return a, b
来源：http://igl.zhengqikj.top

Ruby: return a, b
来源：http://vyw.yanxiufei.cn

C#:   return (a, b);              // ValueTuple
来源：http://mjc.chenjidiqi.icu

[C06] 匿名函数 / lambda
来源：http://mvd.ctjpmb.com

Py:   square = lambda x: x * x
来源：http://kps.hnxiangtu.top

PHP:  $square = fn($x) => $x * $x;
来源：http://vls.hysaishi.cn

JS:   const square = x => x * x;
来源：http://vmy.yueranfly.top

TS:   const square = (x: number): number => x * x;
来源：http://lsh.yj20258888.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://vau.c1oappe.top

Go:   sq := func(x int) int { return x * x }
来源：http://fyi.ivvv.top

Ruby: square = ->(x) { x * x }
来源：http://qsz.shuidangran.top

C#:   Func<int, int> square = x => x * x;
来源：http://tav.0kj1m.cn

[C07] 把函数作为参数传入
来源：http://mcy.snrcjt.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://pcc.xziqi.cn

PHP:  array_map("strtoupper", $arr);
来源：http://wbv.iojbl.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://crv.tarul.cn

TS:   arr.map(String)
来源：http://wfb.zdqjudy.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://oab.cqqwz.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://eed.jqgfzy.top

Ruby: arr.map(&:upcase)
来源：http://thu.cheryme.top

C#:   arr.Select(s => s.ToUpper())
来源：http://azv.jinghuilouyu.cn

[C08] 闭包
来源：http://juz.cdnleiting.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://xwv.jlsjyb.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://lfk.haohaochexian.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://dbv.cucudq.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://drp.shanyushiyangkeji.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://pea.ivvv.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://asm.zdbjq.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://iyo.gaohongyu789.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://zjx.sysykeji.top

[C09] 递归
来源：http://qzo.andypj.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://clh.zhoulong.xyz

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ulh.shangyingyoupin.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://iqk.bbcook.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ssk.birdmap.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://fmd.cqqwz.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ppe.sysykeji.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://vea.ehwqpu.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://kjr.tianlin.xyz

[C10] 变量作用域
来源：http://gzf.hongshengwenyu.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://leq.jianghu66.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://loz.shuidangran.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mxs.daria6918.cn

TS:   同 JS
来源：http://ilu.hnqzz.top

Java: 方法内为块级作用域
来源：http://cln.aizwys.cn

Go:   花括号块级作用域
来源：http://odh.vehdjk.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://biw.yuxming.cn

C#:   块级作用域
来源：http://lah.pycfn.com

[C11] 模块导入与导出
来源：http://fqd.zdbjq.cn

Py:   from module import func
来源：http://lyf.wangdashe.top

PHP:  require "file.php";  或 use App\Service;
来源：http://row.guowangkeji.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://gvy.zhijiandao.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://dfj.fktsv.cn

Java: import java.util.List;
来源：http://urs.zdqjudy.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://pxa.tanke756.top

Ruby: require "json"; require_relative "./util"
来源：http://bcv.aibaodan.cn

C#:   using System.Text;
来源：http://ywt.yueranfly.top

[C12] 立即执行函数 IIFE
来源：http://guy.yonumen.top

Py:   (lambda: print("run"))()
来源：http://dus.jqgufenzy.top

PHP:  (function () { echo "run"; })();
来源：http://rjh.sweek.top

JS:   (() => { console.log("run"); })();
来源：http://eud.yj20258888.top

TS:   (() => { console.log("run"); })();
来源：http://zbf.jqgfzy.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ymi.smart0.xyz

Go:   func() { fmt.Println("run") }()
来源：http://epq.gaohongyu789.top

Ruby: -> { puts "run" }.call
来源：http://dpq.yj202588.top

C#:   // 无 IIFE：用静态构造函数
来源：http://nfc.shanyushiyangtech.top

[C13] 类型声明 / 类型注解
来源：http://kje.9152youxi.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://zsx.aibaodan.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://stj.epnwcf.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://cbs.fktsv.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mgv.ydzc1.top

Java: int add(int a, int b) { return a + b; }
来源：http://ulg.yuanzhike.top

Go:   func add(a, b int) int
来源：http://qyl.gaohongyu789.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://aan.smart0.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://php.xinyue.icu

[C14] 泛型函数
来源：http://yqw.yuanzhike.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://tlf.jiagoushi.top

PHP:  // 无泛型
来源：http://att.shanyushiyangtech.top

JS:   // 无泛型
来源：http://dvi.sufxvd.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://zth.yj20258888.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://iyt.gogol.net.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hlc.tanke756.top

Ruby: # 无泛型
来源：http://mmw.ehwqpu.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://zvh.ivvv.top

[C15] 解构 / 展开参数
来源：http://udm.xingfuxueyuan.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://pwe.sjlbkw.cn

PHP:  [$a, $b] = $pair;
来源：http://adl.hnxiangtu.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://imp.hfpthk.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hbx.jqgufenzy.top

Java: // 无解构
来源：http://lww.sjlbkw.cn

Go:   // 无解构
来源：http://bug.jinyuanbaomall.cn

Ruby: a, b = pair
来源：http://zoz.hesvh.cn

C#:   var (a, b) = pair;
来源：http://rnd.daria6918.cn

[C16] 函数 / 方法重载
来源：http://ncy.yvedp.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://crs.meibo888.top

PHP:  // 无重载
来源：http://pus.ydzc1.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://zak.svipenyu.cn

TS:   // 用联合类型或重载签名声明
来源：http://pvw.sysykeji.top

Java: void f(int a) {}  void f(String a) {}
来源：http://zbu.zdbjq.cn

Go:   // 无重载：用不同函数名
来源：http://sbn.aibaodan.cn

Ruby: # 无重载：靠动态参数
来源：http://nqs.shanyushiyangkeji.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://acd.daxiang520.top

================================================================================
来源：http://ppb.kuanghao11.cn

D. 数组 / 列表 / 集合
来源：http://ybi.cashguo.top

================================================================================
来源：http://dvr.tian-w.cn

[D01] 创建数组 / 列表
来源：http://mzn.nwbrower.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://mfp.hnqzz.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wyj.zhijiandao.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://pqa.c1oappe.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://cuu.316326.xyz

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://nfs.andypj.xyz

Go:   arr := []int{1, 2, 3}
来源：http://pef.iojbl.cn

Ruby: arr = [1, 2, 3]
来源：http://zst.fanxiaobao.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://bhk.bbcook.cn

[D02] 追加元素到末尾
来源：http://kkr.pycfn.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://tap.xziqi.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ecp.yuanzhike.top

JS:   arr.push(4);
来源：http://rwl.svipenyu.cn

TS:   arr.push(4);
来源：http://qdh.jiagoushi.top

Java: list.add(4);
来源：http://qzx.fehbvm.com

Go:   arr = append(arr, 4)
来源：http://wtc.fengsongda.top

Ruby: arr << 4; arr.push(5)
来源：http://ana.guowangkeji.top

C#:   list.Add(4);
来源：http://zqm.yj20258888.top

[D03] 在指定位置插入元素
来源：http://xzo.feifeiyinyue.top

Py:   arr.insert(0, 0)
来源：http://bbn.jinqigfzy.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://rzu.ivvv.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://xxv.aizwys.cn

TS:   arr.splice(0, 0, 0);
来源：http://gtt.chenzaomai.com

Java: list.add(0, 0);
来源：http://yox.yj20258.top

Go:   arr = append([]int{0}, arr...)
来源：http://msr.zhengqikj.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://jqu.ydzc1.top

C#:   list.Insert(0, 0);
来源：http://ksr.cdnleiting.top

[D04] 删除元素
来源：http://yar.gogol.net.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://lvj.zhongyouzk.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://dfa.tanke756.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://nay.zhiwuduotai.top

TS:   arr.splice(0, 1);
来源：http://oji.dashuyun.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ixy.tian-w.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ylx.daxiang520.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://zuq.xinyue.icu

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://zml.jianghu66.top

[D05] 访问与修改元素
来源：http://znr.ywan-chungtsiang.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mba.sysykeji.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://atj.svipenyu.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://dbh.daria6918.cn

TS:   arr[0]; arr.at(-1);
来源：http://dqj.yj20258.top

Java: list.get(0); list.set(0, 9);
来源：http://mzv.wangdashe.top

Go:   arr[0]; arr[0] = 9
来源：http://wdm.zycfv.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wfq.ivvv.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hwn.nwbrower.top

[D06] 数组长度
来源：http://zpq.52xcode.cn

Py:   len(arr)
来源：http://rus.yuanzhike.top

PHP:  count($arr);
来源：http://heb.shangyingyoupin.top

JS:   arr.length
来源：http://ltl.aizwys.cn

TS:   arr.length
来源：http://jya.epnwcf.com

Java: list.size();
来源：http://xwz.bjfxy.top

Go:   len(arr)
来源：http://pii.haohaochexian.top

Ruby: arr.length; arr.size
来源：http://ath.guowangkeji.top

C#:   list.Count;
来源：http://yfy.yongpay.top

[D07] 切片 / 取子数组
来源：http://pos.zhijiandao.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://xgq.yongpay.top

PHP:  array_slice($arr, 1, 3);
来源：http://gjb.shuidangran.top

JS:   arr.slice(1, 4);
来源：http://kel.shzxlz.cn

TS:   arr.slice(1, 4);
来源：http://rhe.52xcode.cn

Java: list.subList(1, 4);
来源：http://wwn.zdbjq.cn

Go:   arr[1:4]
来源：http://ivg.jinqigfzy.top

Ruby: arr[1, 3]
来源：http://ifm.sxryk.cn

C#:   list.GetRange(1, 3);
来源：http://hhx.nanxinkj.top

[D08] 合并两个数组
来源：http://dau.fehbvm.com

Py:   a + b;  a.extend(b)
来源：http://lph.svipenyu.cn

PHP:  array_merge($a, $b);
来源：http://gzq.gogol.net.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://isq.andypj.xyz

TS:   [...a, ...b];
来源：http://amw.uphjek.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://klu.tarul.cn

Go:   append(a, b...)
来源：http://nob.zhaomingkeji.xyz

Ruby: a + b;  a.concat(b)
来源：http://fyh.aizwys.cn

C#:   a.Concat(b).ToList()
来源：http://jfb.0kj1m.cn

[D09] 排序（升序）
来源：http://kwt.52xcode.cn

Py:   sorted(arr);  arr.sort()
来源：http://xrp.cdnleiting.top

PHP:  sort($arr);
来源：http://qkm.fktsv.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://smh.daxiang520.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://lzc.havefunace.top

Java: Collections.sort(list);  list.sort(null);
来源：http://hme.xylfe.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://uhm.kuanghao11.cn

Ruby: arr.sort
来源：http://twz.tian-w.cn

C#:   list.Sort();
来源：http://acz.shuidangran.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://bjo.chenlongwang.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ign.hnqzz.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jzw.ywan-chungtsiang.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://aff.jqgufenzy.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ruk.wangshuangyany.cn


<!-- 参考信息 -->