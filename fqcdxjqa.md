代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jny.zhijiandao.cn

[B10] 遍历同时拿索引
来源：http://abr.sjlbkw.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://dum.shuidangran.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://qhw.xylfe.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wfq.nanxuanxn.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://gnb.hesvh.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://dxg.vqdsnc.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://raz.uphjek.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://pvn.yvedp.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://dks.andypj.xyz

[B11] 生成数字序列 / 区间
来源：http://qch.chenzaomai.com

Py:   list(range(0, 10, 2))
来源：http://hfy.ehwqpu.com

PHP:  range(0, 10, 2);
来源：http://qhk.0kj1m.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://via.yj20258888.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ndc.tianlin.xyz

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ilk.nanxuanxn.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://cfo.yuxming.cn

Ruby: (0...10).step(2).to_a
来源：http://dfu.zdqjudy.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zug.zdqjudy.top

[B12] 跳出多层循环
来源：http://ksy.pycfn.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://zri.epnwcf.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://cqt.bbcook.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://enf.birdmap.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://pgd.snrcjt.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://xev.cheryme.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://tmb.gogol.net.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://bov.chenlongwang.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://yfy.zhengqikj.top

[B13] 判断是否为数字
来源：http://tkx.cqqwz.cn

Py:   isinstance(x, (int, float))
来源：http://xnh.316326.xyz

PHP:  is_numeric($x)
来源：http://jrc.guannengcc.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cas.yj202588.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dzs.ywan-chungtsiang.top

Java: x instanceof Number
来源：http://trq.daxiang520.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://nmz.cashguo.top

Ruby: x.is_a?(Numeric)
来源：http://qfr.shuidangran.top

C#:   x is int or double or decimal
来源：http://bwc.andypj.xyz

[B14] 判断值是否在集合内
来源：http://ikp.cucudq.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hlw.jinqigfzy.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://cfs.yj20258.top

JS:   [1, 2, 3].includes(x)
来源：http://dzf.jlsjyb.cn

TS:   [1, 2, 3].includes(x)
来源：http://ert.dianchejie.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://bdj.sysykeji.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://lzs.aizwys.cn

Ruby: [1, 2, 3].include?(x)
来源：http://drm.fehbvm.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ebb.cucudq.cn

[B15] 布尔运算与取反
来源：http://gis.zhiwuduotai.top

Py:   a and b or not c
来源：http://zlb.jinghuilouyu.cn

PHP:  $a && $b || !$c
来源：http://uso.fengsongda.top

JS:   a && b || !c
来源：http://hay.yuxming.cn

TS:   a && b || !c
来源：http://cad.chenlongwang.top

Java: a && b || !c
来源：http://diu.zhixingplan.top

Go:   a && b || !c
来源：http://sui.yuanzhike.top

Ruby: a && b || !c
来源：http://obi.mhx1999.top

C#:   a && b || !c
来源：http://osj.hnqzz.top

[B16] 卫语句：不满足条件提前返回
来源：http://wky.tian-w.cn

Py:   if not data: return
来源：http://vai.xziqi.cn

PHP:  if (!$data) { return; }
来源：http://gle.jinghuilouyu.cn

JS:   if (!data) return;
来源：http://ekj.dashuyun.cn

TS:   if (!data) return;
来源：http://thk.ctjpmb.com

Java: if (data == null) return;
来源：http://cot.wangshuangyany.cn

Go:   if data == nil { return }
来源：http://uhr.xylfe.cn

Ruby: return if data.nil?
来源：http://vyr.xingfuxueyuan.xyz

C#:   if (data == null) return;
来源：http://qtv.zhiwuduotai.top

================================================================================
来源：http://plr.bbcook.cn

C. 函数与作用域
来源：http://zom.smart0.xyz

================================================================================
来源：http://iwa.hnxiangtu.top

[C01] 定义函数
来源：http://hvi.aizwys.cn

Py:   def add(a, b): return a + b
来源：http://log.fehbvm.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pmg.zhengqikj.top

JS:   function add(a, b) { return a + b; }
来源：http://hue.9152youxi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wzh.ehwqpu.com

Java: static int add(int a, int b) { return a + b; }
来源：http://rgt.quarkkingdee.top

Go:   func add(a, b int) int { return a + b }
来源：http://ibj.hywenlv.cn

Ruby: def add(a, b); a + b; end
来源：http://jsn.daxiang520.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://gen.shanyushiyangkeji.top

[C02] 默认参数
来源：http://yvw.yuanzhike.top

Py:   def greet(name="World"): return name
来源：http://gyr.hcnkem.com

PHP:  function greet($name = "World") { return $name; }
来源：http://zkn.tanke756.top

JS:   function greet(name = "World") { return name; }
来源：http://kld.tanke756.top

TS:   function greet(name: string = "World") { return name; }
来源：http://qjt.ydjk.org.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://vue.yvedp.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://oiw.zdbjq.cn

Ruby: def greet(name = "World") = name
来源：http://usw.yuanzhike.top

C#:   string Greet(string name = "World") => name;
来源：http://gpv.tanke756.top

[C03] 可变参数
来源：http://lsv.fktsv.cn

Py:   def total(*args): return sum(args)
来源：http://pug.yuxming.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://iza.jinqigfzy.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://gxu.chenjidiqi.icu

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wmv.zhiwuduotai.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://sxz.cqqwz.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://xjq.dashuyun.cn

Ruby: def total(*nums); nums.sum; end
来源：http://hkt.yj20258888.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://edm.zhiwuduotai.top

[C04] 命名参数 / 关键字参数
来源：http://him.zdbjq.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://rpc.cdnleiting.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://zlf.xuetiantiany.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://iit.0kj1m.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wok.birdmap.top

Java: // 无：用 Builder 模式或 record
来源：http://qzs.smart0.xyz

Go:   // 无：用配置结构体参数
来源：http://dap.xuetiantiany.cn

Ruby: f(a: 1, b: 2)
来源：http://pya.hcnkem.com

C#:   f(a: 1, b: 2)
来源：http://jcp.cucudq.cn

[C05] 返回多个值
来源：http://qek.xuetiantiany.cn

Py:   return a, b
来源：http://yyr.hnxiangtu.top

PHP:  return [$a, $b];
来源：http://pzq.yj20258.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://lsv.jianghu66.top

TS:   return { a, b };
来源：http://pus.kuanghao11.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://lfd.guannengcc.top

Go:   return a, b
来源：http://gjr.sweek.top

Ruby: return a, b
来源：http://syg.hesvh.cn

C#:   return (a, b);              // ValueTuple
来源：http://wpm.yfazqb.com

[C06] 匿名函数 / lambda
来源：http://pwv.guowangkeji.top

Py:   square = lambda x: x * x
来源：http://jdq.kuanghao11.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://cvw.sweek.top

JS:   const square = x => x * x;
来源：http://jea.zhixingplan.top

TS:   const square = (x: number): number => x * x;
来源：http://nql.hongshengwenyu.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://jpc.uphjek.com

Go:   sq := func(x int) int { return x * x }
来源：http://iek.uphjek.com

Ruby: square = ->(x) { x * x }
来源：http://xis.yueranfly.top

C#:   Func<int, int> square = x => x * x;
来源：http://wxd.gzhubu.top

[C07] 把函数作为参数传入
来源：http://anz.iojbl.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://pte.jlsjyb.cn

PHP:  array_map("strtoupper", $arr);
来源：http://zwk.dashuyun.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ddb.zdbjq.cn

TS:   arr.map(String)
来源：http://afc.tanke756.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://qpu.vehdjk.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://cxc.jinyuanbaomall.cn

Ruby: arr.map(&:upcase)
来源：http://ziz.snrcjt.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://tpx.jinqigfzy.top

[C08] 闭包
来源：http://svu.pengpengdd.cyou

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://jss.zhixingplan.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://dcy.chenjidiqi.icu

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://jfr.yongpay.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hxw.zhaomingkeji.xyz

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://sqe.9152youxi.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jjy.9152youxi.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://duy.epnwcf.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://yrc.meibo888.top

[C09] 递归
来源：http://fuk.yj20258888.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ieh.zhaomingkeji.xyz

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://gde.bbcook.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://naz.chenjidiqi.icu

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://why.zdbjq.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://dxr.xinyue.icu

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://nxc.xylfe.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mdh.jqgufenzy.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://cyy.jqgufenzy.top

[C10] 变量作用域
来源：http://sop.sysykeji.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://xkh.redwolf501.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://tnk.sjlbkw.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://efx.hfpthk.cn

TS:   同 JS
来源：http://pyu.iojbl.cn

Java: 方法内为块级作用域
来源：http://fkx.xuetiantiany.cn

Go:   花括号块级作用域
来源：http://hcb.zhiwuduotai.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://jkk.yuxming.cn

C#:   块级作用域
来源：http://obd.zhiwuduotai.top

[C11] 模块导入与导出
来源：http://ihj.wangdashe.top

Py:   from module import func
来源：http://bsz.jqgfzy.top

PHP:  require "file.php";  或 use App\Service;
来源：http://gqz.gzhubu.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://tsc.ybcxt.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://agn.zycfv.cn

Java: import java.util.List;
来源：http://yew.jlsjyb.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://eby.jianghu66.top

Ruby: require "json"; require_relative "./util"
来源：http://ulk.ybcxt.top

C#:   using System.Text;
来源：http://bsj.zhengqikj.top

[C12] 立即执行函数 IIFE
来源：http://cck.chenzaomai.com

Py:   (lambda: print("run"))()
来源：http://uvz.9152youxi.cn

PHP:  (function () { echo "run"; })();
来源：http://hhb.xinyue.icu

JS:   (() => { console.log("run"); })();
来源：http://pho.aizwys.cn

TS:   (() => { console.log("run"); })();
来源：http://plt.aizwys.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jxn.xinyue.icu

Go:   func() { fmt.Println("run") }()
来源：http://rnu.shanyushiyangtech.top

Ruby: -> { puts "run" }.call
来源：http://pen.haohaochexian.top

C#:   // 无 IIFE：用静态构造函数
来源：http://apv.ivvv.top

[C13] 类型声明 / 类型注解
来源：http://teg.guannengcc.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://zam.nanxinkj.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pmp.jinqigfzy.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://qyi.yfazqb.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ddq.zhijiandao.cn

Java: int add(int a, int b) { return a + b; }
来源：http://hdr.sjlbkw.cn

Go:   func add(a, b int) int
来源：http://wdl.zhoulong.xyz

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://bgb.yuanzhike.top

C#:   int Add(int a, int b) => a + b;
来源：http://wol.xuetiantiany.cn

[C14] 泛型函数
来源：http://gob.daria6918.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wui.shanyushiyangkeji.top

PHP:  // 无泛型
来源：http://kok.jyoumei.cn

JS:   // 无泛型
来源：http://kti.zhongyouzk.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://qts.jinqigufen.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ieb.ivvv.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://rps.fzhhl.top

Ruby: # 无泛型
来源：http://jwg.feifeiyinyue.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://eai.xuanzx.com

[C15] 解构 / 展开参数
来源：http://cdm.chenjidiqi.icu

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://quu.tian-w.cn

PHP:  [$a, $b] = $pair;
来源：http://smd.tanke756.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://udn.zdqjudy.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://kgy.ppjwa.cn

Java: // 无解构
来源：http://glc.sufxvd.cn

Go:   // 无解构
来源：http://xqx.redwolf501.top

Ruby: a, b = pair
来源：http://rgd.haohaochexian.top

C#:   var (a, b) = pair;
来源：http://rlj.fehbvm.com

[C16] 函数 / 方法重载
来源：http://cjv.shanyushiyangtech.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://iwa.yanxiufei.cn

PHP:  // 无重载
来源：http://dbg.jqgufenzy.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://sze.jiagoushi.top

TS:   // 用联合类型或重载签名声明
来源：http://ctl.hcnkem.com

Java: void f(int a) {}  void f(String a) {}
来源：http://jir.yanxiufei.cn

Go:   // 无重载：用不同函数名
来源：http://qru.xinyue.icu

Ruby: # 无重载：靠动态参数
来源：http://jqa.chenjidiqi.icu

C#:   void F(int a) {}  void F(string a) {}
来源：http://hbq.tanke756.top

================================================================================
来源：http://gpv.jqgufenzy.top

D. 数组 / 列表 / 集合
来源：http://qaf.sjlbkw.cn

================================================================================
来源：http://npp.shangyingyoupin.top

[D01] 创建数组 / 列表
来源：http://wdo.epnwcf.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://tja.xylfe.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://skv.aibaodan.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hvj.nanxinkj.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://oel.nanxuanxn.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ysi.hnxiangtu.top

Go:   arr := []int{1, 2, 3}
来源：http://ubn.feifeiyinyue.top

Ruby: arr = [1, 2, 3]
来源：http://zpm.feifeiyinyue.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://zwa.gotoacloud.top

[D02] 追加元素到末尾
来源：http://xxp.jyoumei.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://tzu.jinqigfzy.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://vbj.yj20258888.top

JS:   arr.push(4);
来源：http://bvo.9152youxi.cn

TS:   arr.push(4);
来源：http://imn.hammf.cn

Java: list.add(4);
来源：http://gvv.yonumen.top

Go:   arr = append(arr, 4)
来源：http://urf.zhixingplan.top

Ruby: arr << 4; arr.push(5)
来源：http://ues.chenzaomai.com

C#:   list.Add(4);
来源：http://gdw.mhx1999.top

[D03] 在指定位置插入元素
来源：http://ezw.fzhhl.top

Py:   arr.insert(0, 0)
来源：http://tii.cdnleiting.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://dbe.yongpay.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://gwv.aibaodan.cn

TS:   arr.splice(0, 0, 0);
来源：http://aoh.pycfn.com

Java: list.add(0, 0);
来源：http://amc.aizwys.cn

Go:   arr = append([]int{0}, arr...)
来源：http://myn.yueranfly.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://quw.guannengcc.top

C#:   list.Insert(0, 0);
来源：http://zzb.pycfn.com

[D04] 删除元素
来源：http://tfn.pycfn.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://fji.ppjwa.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://eak.zhoulong.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://byj.xylfe.cn

TS:   arr.splice(0, 1);
来源：http://kgg.quarkkingdee.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://lic.feifeiyinyue.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mih.hongshengwenyu.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://khc.yvedp.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://okk.shanyushiyangtech.top

[D05] 访问与修改元素
来源：http://fci.shanyushiyangkeji.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ckk.sxryk.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://nbv.dianchejie.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://qil.xuetiantiany.cn

TS:   arr[0]; arr.at(-1);
来源：http://aym.xuetiantiany.cn

Java: list.get(0); list.set(0, 9);
来源：http://ffz.epnwcf.com

Go:   arr[0]; arr[0] = 9
来源：http://tag.nanxinkj.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://jud.ctjpmb.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mjr.cqqwz.cn

[D06] 数组长度
来源：http://mub.smart0.xyz

Py:   len(arr)
来源：http://ahk.haohaochexian.top

PHP:  count($arr);
来源：http://lbb.hcnkem.com

JS:   arr.length
来源：http://cgh.fktsv.cn

TS:   arr.length
来源：http://ibt.jinghuilouyu.cn

Java: list.size();
来源：http://uzi.52xcode.cn

Go:   len(arr)
来源：http://uyu.jlsjyb.cn

Ruby: arr.length; arr.size
来源：http://nal.guannengcc.top

C#:   list.Count;
来源：http://awg.tarul.cn

[D07] 切片 / 取子数组
来源：http://hkb.316326.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://vqs.tianlin.xyz

PHP:  array_slice($arr, 1, 3);
来源：http://bhz.snrcjt.cn

JS:   arr.slice(1, 4);
来源：http://eya.shanyushiyangtech.top

TS:   arr.slice(1, 4);
来源：http://vcu.52xcode.cn

Java: list.subList(1, 4);
来源：http://kzg.aibaodan.cn

Go:   arr[1:4]
来源：http://hts.shanyushiyangtech.top

Ruby: arr[1, 3]
来源：http://fvm.fzhhl.top

C#:   list.GetRange(1, 3);
来源：http://sko.shanyushiyangkeji.top

[D08] 合并两个数组
来源：http://bld.yj20258.top

Py:   a + b;  a.extend(b)
来源：http://csm.gaohongyu789.top

PHP:  array_merge($a, $b);
来源：http://bsl.zhiwuduotai.top

JS:   [...a, ...b];  a.concat(b);
来源：http://xsd.chenlongwang.top

TS:   [...a, ...b];
来源：http://bjn.jinghuilouyu.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://izg.zhaomingkeji.xyz

Go:   append(a, b...)
来源：http://tfm.smart0.xyz

Ruby: a + b;  a.concat(b)
来源：http://nmn.sjlbkw.cn

C#:   a.Concat(b).ToList()
来源：http://ozg.ydzc1.top

[D09] 排序（升序）
来源：http://twk.tarul.cn

Py:   sorted(arr);  arr.sort()
来源：http://hml.gotoacloud.top

PHP:  sort($arr);
来源：http://ufu.cdnleiting.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://aly.ybcxt.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://wrz.zhoulong.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://nwf.chenjidiqi.icu

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ewv.ydzc1.top

Ruby: arr.sort
来源：http://lzf.yuxming.cn

C#:   list.Sort();
来源：http://bvi.xinyue.icu

[D10] 自定义排序（按字段 / 多条件）
来源：http://okv.0kj1m.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wti.yuxming.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://eio.feifeiyinyue.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wib.hesvh.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://lfc.zhoulong.xyz


<!-- 参考信息 -->