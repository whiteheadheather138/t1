代发 wailian999

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://uwp.xylfe.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://epb.vehdjk.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://unv.zhengqikj.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://zsh.guowangkeji.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://dgx.hywenlv.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://dzs.yanxiufei.cn

[B11] 生成数字序列 / 区间
来源：http://wtw.cdnleiting.top

Py:   list(range(0, 10, 2))
来源：http://yah.ydjk.org.cn

PHP:  range(0, 10, 2);
来源：http://vbn.vqdsnc.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://seo.yuanzhike.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yjz.c1oappe.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://dyx.gzhubu.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://xli.zhixingplan.top

Ruby: (0...10).step(2).to_a
来源：http://mfc.gotoacloud.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://iiv.zdbjq.cn

[B12] 跳出多层循环
来源：http://vmf.316326.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://vkm.havefunace.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://cal.yangfankeji.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://aus.ydjk.org.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://sqa.chenlongwang.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://zpw.smart0.xyz

Go:   # 无标签：用布尔标志或抽成函数
来源：http://kgs.snrcjt.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wlu.nanxuanxn.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://qzz.aizwys.cn

[B13] 判断是否为数字
来源：http://pcu.jinyuanbaomall.cn

Py:   isinstance(x, (int, float))
来源：http://lcs.cashguo.top

PHP:  is_numeric($x)
来源：http://qgc.zhaomingkeji.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://juk.xuanzx.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kbu.yanxiufei.cn

Java: x instanceof Number
来源：http://kwe.meibo888.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://bod.cdnleiting.top

Ruby: x.is_a?(Numeric)
来源：http://uwq.quarkkingdee.top

C#:   x is int or double or decimal
来源：http://eno.vehdjk.com

[B14] 判断值是否在集合内
来源：http://cyv.hfpthk.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://evs.yj202588.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://dsh.zhijiandao.cn

JS:   [1, 2, 3].includes(x)
来源：http://wwh.hammf.cn

TS:   [1, 2, 3].includes(x)
来源：http://csk.xylfe.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://kvt.gaohongyu789.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://evi.yj202588.top

Ruby: [1, 2, 3].include?(x)
来源：http://kiq.redwolf501.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://cdr.yuxming.cn

[B15] 布尔运算与取反
来源：http://tee.birdmap.top

Py:   a and b or not c
来源：http://vjv.ppjwa.cn

PHP:  $a && $b || !$c
来源：http://bpz.zhongyouzk.top

JS:   a && b || !c
来源：http://vzl.uphjek.com

TS:   a && b || !c
来源：http://itm.jinghuilouyu.cn

Java: a && b || !c
来源：http://xyb.fehbvm.com

Go:   a && b || !c
来源：http://xcm.yfazqb.com

Ruby: a && b || !c
来源：http://qla.shzxlz.cn

C#:   a && b || !c
来源：http://lth.fanxiaobao.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://ztr.tianlin.xyz

Py:   if not data: return
来源：http://gcd.shuidangran.top

PHP:  if (!$data) { return; }
来源：http://glu.yanxiufei.cn

JS:   if (!data) return;
来源：http://rly.epnwcf.com

TS:   if (!data) return;
来源：http://rmc.fengsongda.top

Java: if (data == null) return;
来源：http://ege.zhoulong.xyz

Go:   if data == nil { return }
来源：http://vaf.shzxlz.cn

Ruby: return if data.nil?
来源：http://bql.fengsongda.top

C#:   if (data == null) return;
来源：http://dap.nanxuanxn.top

================================================================================
来源：http://eaq.52xcode.cn

C. 函数与作用域
来源：http://ujn.yuanzhike.top

================================================================================
来源：http://zyv.zdqjudy.top

[C01] 定义函数
来源：http://iza.mhx1999.top

Py:   def add(a, b): return a + b
来源：http://aze.fanxiaobao.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kjq.meibo888.top

JS:   function add(a, b) { return a + b; }
来源：http://jqo.ydjk.org.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xcl.xinyue.icu

Java: static int add(int a, int b) { return a + b; }
来源：http://vvk.haohaochexian.top

Go:   func add(a, b int) int { return a + b }
来源：http://kkk.jinqigfzy.top

Ruby: def add(a, b); a + b; end
来源：http://cfi.aizwys.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://bki.gotoacloud.top

[C02] 默认参数
来源：http://igb.shuidangran.top

Py:   def greet(name="World"): return name
来源：http://eyk.9152youxi.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://zgh.ybcxt.top

JS:   function greet(name = "World") { return name; }
来源：http://xtv.dianchejie.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://npa.yonumen.top

Java: // 无默认参数：方法重载或 Optional
来源：http://oxg.epnwcf.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://fln.fengsongda.top

Ruby: def greet(name = "World") = name
来源：http://elg.jianghu66.top

C#:   string Greet(string name = "World") => name;
来源：http://zte.vehdjk.com

[C03] 可变参数
来源：http://jmf.nanxinkj.top

Py:   def total(*args): return sum(args)
来源：http://mru.pycfn.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mld.nanxinkj.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hyg.wangshuangyany.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://bqx.jyoumei.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://bvo.xingfuxueyuan.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://qub.xinyue.icu

Ruby: def total(*nums); nums.sum; end
来源：http://wmf.vehdjk.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ngh.yj20258888.top

[C04] 命名参数 / 关键字参数
来源：http://rmi.hammf.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://doi.vehdjk.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ekq.yuxming.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://irj.aibaodan.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ibp.ybcxt.top

Java: // 无：用 Builder 模式或 record
来源：http://nyw.hesvh.cn

Go:   // 无：用配置结构体参数
来源：http://nhi.hywenlv.cn

Ruby: f(a: 1, b: 2)
来源：http://fnc.chenlongwang.top

C#:   f(a: 1, b: 2)
来源：http://wbg.hysaishi.cn

[C05] 返回多个值
来源：http://ykg.xylfe.cn

Py:   return a, b
来源：http://etd.sweek.top

PHP:  return [$a, $b];
来源：http://jdf.xuanzx.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://ivf.chenlongwang.top

TS:   return { a, b };
来源：http://sju.hesvh.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://dkp.xinyue.icu

Go:   return a, b
来源：http://rcz.zhaomingkeji.xyz

Ruby: return a, b
来源：http://vzy.yongpay.top

C#:   return (a, b);              // ValueTuple
来源：http://kkx.shuidangran.top

[C06] 匿名函数 / lambda
来源：http://oco.ehwqpu.com

Py:   square = lambda x: x * x
来源：http://jfa.havefunace.top

PHP:  $square = fn($x) => $x * $x;
来源：http://lzp.dashuyun.cn

JS:   const square = x => x * x;
来源：http://ymg.chenlongwang.top

TS:   const square = (x: number): number => x * x;
来源：http://jkw.ybcxt.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://faw.yuxming.cn

Go:   sq := func(x int) int { return x * x }
来源：http://jnt.hesvh.cn

Ruby: square = ->(x) { x * x }
来源：http://ows.jiagoushi.top

C#:   Func<int, int> square = x => x * x;
来源：http://ywx.yongpay.top

[C07] 把函数作为参数传入
来源：http://deq.fzhhl.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ewb.jiagoushi.top

PHP:  array_map("strtoupper", $arr);
来源：http://xjg.zhengqikj.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://cvc.guowangkeji.top

TS:   arr.map(String)
来源：http://ods.xuetiantiany.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hka.jianghu66.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baa.zhixingplan.top

Ruby: arr.map(&:upcase)
来源：http://mtw.zhaomingkeji.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://xbg.kuanghao11.cn

[C08] 闭包
来源：http://akd.shuidangran.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://sbs.hcnkem.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hit.hywenlv.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://fil.zhaomingkeji.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://xtg.zhaomingkeji.xyz

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://kho.xylfe.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://tpu.fktsv.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://gws.daria6918.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://zqe.shzxlz.cn

[C09] 递归
来源：http://wah.tian-w.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mkc.fktsv.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://tjs.fktsv.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wxr.xingfuxueyuan.xyz

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lzz.yvedp.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://urf.jiagoushi.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hbc.ctjpmb.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://arf.fengsongda.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://vjq.ctjpmb.com

[C10] 变量作用域
来源：http://qqs.zhixingplan.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://tnz.tarul.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://pul.jqgfzy.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://har.zdqjudy.top

TS:   同 JS
来源：http://tbe.yuxming.cn

Java: 方法内为块级作用域
来源：http://pxo.yfazqb.com

Go:   花括号块级作用域
来源：http://ydl.gaohongyu789.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xbo.yj202588.top

C#:   块级作用域
来源：http://rbw.cucudq.cn

[C11] 模块导入与导出
来源：http://tem.shangyingyoupin.top

Py:   from module import func
来源：http://umv.jlsjyb.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://pnu.hcnkem.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://zxa.dianchejie.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://cbx.dianchejie.cn

Java: import java.util.List;
来源：http://smv.ehwqpu.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://qor.vqdsnc.cn

Ruby: require "json"; require_relative "./util"
来源：http://frf.hammf.cn

C#:   using System.Text;
来源：http://ivb.xingfuxueyuan.xyz

[C12] 立即执行函数 IIFE
来源：http://yxn.kuanghao11.cn

Py:   (lambda: print("run"))()
来源：http://snp.sxryk.cn

PHP:  (function () { echo "run"; })();
来源：http://qpe.tian-w.cn

JS:   (() => { console.log("run"); })();
来源：http://srr.redwolf501.top

TS:   (() => { console.log("run"); })();
来源：http://gzv.pengpengdd.cyou

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://bol.zdbjq.cn

Go:   func() { fmt.Println("run") }()
来源：http://icz.andypj.xyz

Ruby: -> { puts "run" }.call
来源：http://slo.smart0.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://oxv.shanyushiyangtech.top

[C13] 类型声明 / 类型注解
来源：http://tdl.tian-w.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://xpp.c1oappe.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sgj.zdbjq.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hcr.cucudq.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://erj.zhongyouzk.top

Java: int add(int a, int b) { return a + b; }
来源：http://uqw.ctjpmb.com

Go:   func add(a, b int) int
来源：http://dka.yonumen.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://nbk.zdqjudy.top

C#:   int Add(int a, int b) => a + b;
来源：http://sab.chenzaomai.com

[C14] 泛型函数
来源：http://mqe.hcnkem.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ibn.zdbjq.cn

PHP:  // 无泛型
来源：http://ywe.zhengqikj.top

JS:   // 无泛型
来源：http://xzm.hongshengwenyu.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://piv.tianlin.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://org.iojbl.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://szm.0kj1m.cn

Ruby: # 无泛型
来源：http://nsg.kuanghao11.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://pqp.xingfuxueyuan.xyz

[C15] 解构 / 展开参数
来源：http://bpf.birdmap.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://uyu.ppjwa.cn

PHP:  [$a, $b] = $pair;
来源：http://srl.kuanghao11.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://kru.cucudq.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://vzx.ybcxt.top

Java: // 无解构
来源：http://htt.cucudq.cn

Go:   // 无解构
来源：http://nue.kuanghao11.cn

Ruby: a, b = pair
来源：http://jxr.pycfn.com

C#:   var (a, b) = pair;
来源：http://kza.ybcxt.top

[C16] 函数 / 方法重载
来源：http://wri.guannengcc.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ibd.ivvv.top

PHP:  // 无重载
来源：http://ywc.daria6918.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://tyw.yj20258888.top

TS:   // 用联合类型或重载签名声明
来源：http://efi.sweek.top

Java: void f(int a) {}  void f(String a) {}
来源：http://ntu.haohaochexian.top

Go:   // 无重载：用不同函数名
来源：http://xrq.shanyushiyangkeji.top

Ruby: # 无重载：靠动态参数
来源：http://mgk.iojbl.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://hrg.yvedp.cn

================================================================================
来源：http://evn.yj20258888.top

D. 数组 / 列表 / 集合
来源：http://uyr.fktsv.cn

================================================================================
来源：http://oax.vehdjk.com

[D01] 创建数组 / 列表
来源：http://obg.ivvv.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://ipy.hnxiangtu.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://czf.hesvh.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://shy.9152youxi.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://cfe.zdqjudy.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://dvh.kuanghao11.cn

Go:   arr := []int{1, 2, 3}
来源：http://wvs.gaohongyu789.top

Ruby: arr = [1, 2, 3]
来源：http://cdl.yfazqb.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://dme.wangdashe.top

[D02] 追加元素到末尾
来源：http://aes.daria6918.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://pmb.sysykeji.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ade.jiagoushi.top

JS:   arr.push(4);
来源：http://efe.cqqwz.cn

TS:   arr.push(4);
来源：http://urf.yongpay.top

Java: list.add(4);
来源：http://tuy.yuxming.cn

Go:   arr = append(arr, 4)
来源：http://dmn.dianchejie.cn

Ruby: arr << 4; arr.push(5)
来源：http://vws.ivvv.top

C#:   list.Add(4);
来源：http://wex.haohaochexian.top

[D03] 在指定位置插入元素
来源：http://dtr.wangdashe.top

Py:   arr.insert(0, 0)
来源：http://vjp.aibaodan.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://nxs.ehwqpu.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://dai.zhixingplan.top

TS:   arr.splice(0, 0, 0);
来源：http://gpq.xinyue.icu

Java: list.add(0, 0);
来源：http://qdm.gzhubu.top

Go:   arr = append([]int{0}, arr...)
来源：http://sna.xingfuxueyuan.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://pqa.dashuyun.cn

C#:   list.Insert(0, 0);
来源：http://faf.wangshuangyany.cn

[D04] 删除元素
来源：http://oca.ctjpmb.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://cys.redwolf501.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://tmn.hfpthk.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://vpr.hfpthk.cn

TS:   arr.splice(0, 1);
来源：http://vwd.feifeiyinyue.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://koc.yvedp.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://bqy.jinqigufen.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://zgo.shangyingyoupin.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://moz.yuxming.cn

[D05] 访问与修改元素
来源：http://ntu.sweek.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://bgp.ywan-chungtsiang.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://bgz.snrcjt.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://que.jinyuanbaomall.cn

TS:   arr[0]; arr.at(-1);
来源：http://vaj.hnqzz.top

Java: list.get(0); list.set(0, 9);
来源：http://uwn.hesvh.cn

Go:   arr[0]; arr[0] = 9
来源：http://xku.ppjwa.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://zll.shzxlz.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://vic.ydjk.org.cn

[D06] 数组长度
来源：http://rpf.cheryme.top

Py:   len(arr)
来源：http://roc.fehbvm.com

PHP:  count($arr);
来源：http://jdp.yongpay.top

JS:   arr.length
来源：http://hfe.shuidangran.top

TS:   arr.length
来源：http://oma.wangshuangyany.cn

Java: list.size();
来源：http://flf.ctjpmb.com

Go:   len(arr)
来源：http://zxw.zdqjudy.top

Ruby: arr.length; arr.size
来源：http://vym.c1oappe.top

C#:   list.Count;
来源：http://eib.hywenlv.cn

[D07] 切片 / 取子数组
来源：http://ojd.sufxvd.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://gne.hcnkem.com

PHP:  array_slice($arr, 1, 3);
来源：http://avp.zhoulong.xyz

JS:   arr.slice(1, 4);
来源：http://mjf.bjfxy.top

TS:   arr.slice(1, 4);
来源：http://kag.hysaishi.cn

Java: list.subList(1, 4);
来源：http://qav.fzhhl.top

Go:   arr[1:4]
来源：http://puq.ctjpmb.com

Ruby: arr[1, 3]
来源：http://obs.cucudq.cn

C#:   list.GetRange(1, 3);
来源：http://nzk.yj20258888.top

[D08] 合并两个数组
来源：http://nul.sjlbkw.cn

Py:   a + b;  a.extend(b)
来源：http://yfx.ywan-chungtsiang.top

PHP:  array_merge($a, $b);
来源：http://mbp.guowangkeji.top

JS:   [...a, ...b];  a.concat(b);
来源：http://nxp.9152youxi.cn

TS:   [...a, ...b];
来源：http://uvi.cqqwz.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://rde.jianghu66.top

Go:   append(a, b...)
来源：http://viq.svipenyu.cn

Ruby: a + b;  a.concat(b)
来源：http://lks.havefunace.top

C#:   a.Concat(b).ToList()
来源：http://ung.ydzc1.top

[D09] 排序（升序）
来源：http://hjq.meibo888.top

Py:   sorted(arr);  arr.sort()
来源：http://tkx.yj20258.top

PHP:  sort($arr);
来源：http://njw.guowangkeji.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://llp.jqgufenzy.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://bub.c1oappe.top

Java: Collections.sort(list);  list.sort(null);
来源：http://uwr.ywan-chungtsiang.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://aml.svipenyu.cn

Ruby: arr.sort
来源：http://llm.yanxiufei.cn

C#:   list.Sort();
来源：http://alc.zhaomingkeji.xyz

[D10] 自定义排序（按字段 / 多条件）
来源：http://lwx.havefunace.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ahy.ivvv.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://afj.zdbjq.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://zuj.kuanghao11.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://gvp.guannengcc.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://scr.nanxuanxn.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://qbp.zdqjudy.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mqq.hammf.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://flw.yj20258888.top


<!-- 参考信息 -->