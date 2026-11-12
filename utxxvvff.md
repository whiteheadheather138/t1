代发 wailian999

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://voa.feifeiyinyue.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://clj.ivvv.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hoc.jqgufenzy.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hpp.sufxvd.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://koy.yj20258.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mph.shangyingyoupin.top

[B11] 生成数字序列 / 区间
来源：http://bbx.tian-w.cn

Py:   list(range(0, 10, 2))
来源：http://drq.tanke756.top

PHP:  range(0, 10, 2);
来源：http://owq.hywenlv.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://aqw.ctjpmb.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fyn.mhx1999.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hmp.zdqjudy.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://olv.nanxinkj.top

Ruby: (0...10).step(2).to_a
来源：http://cgj.yuanzhike.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://uqf.zhaomingkeji.xyz

[B12] 跳出多层循环
来源：http://nba.ydjk.org.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://pms.jinqigfzy.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://ies.cheryme.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://opn.fzhhl.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://enu.ydjk.org.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://vdd.ybcxt.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://jtx.yj20258.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://tku.52xcode.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mqb.svipenyu.cn

[B13] 判断是否为数字
来源：http://wbm.cheryme.top

Py:   isinstance(x, (int, float))
来源：http://zpj.ppjwa.cn

PHP:  is_numeric($x)
来源：http://xbv.shzxlz.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rdq.cdnleiting.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hev.hongshengwenyu.top

Java: x instanceof Number
来源：http://uys.jqgfzy.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://vsi.shzxlz.cn

Ruby: x.is_a?(Numeric)
来源：http://bhk.ppjwa.cn

C#:   x is int or double or decimal
来源：http://hbg.316326.xyz

[B14] 判断值是否在集合内
来源：http://osq.hammf.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://yyq.hysaishi.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://oae.hfpthk.cn

JS:   [1, 2, 3].includes(x)
来源：http://thb.ywan-chungtsiang.top

TS:   [1, 2, 3].includes(x)
来源：http://uhd.jyoumei.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ehl.svipenyu.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://dyz.yonumen.top

Ruby: [1, 2, 3].include?(x)
来源：http://bnd.gogol.net.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://dcz.shzxlz.cn

[B15] 布尔运算与取反
来源：http://ucq.cdnleiting.top

Py:   a and b or not c
来源：http://vfy.zycfv.cn

PHP:  $a && $b || !$c
来源：http://ybu.ydzc1.top

JS:   a && b || !c
来源：http://xpx.yangfankeji.com

TS:   a && b || !c
来源：http://wxr.xuetiantiany.cn

Java: a && b || !c
来源：http://bqt.jinqigfzy.top

Go:   a && b || !c
来源：http://lqb.316326.xyz

Ruby: a && b || !c
来源：http://puk.yj202588.top

C#:   a && b || !c
来源：http://slt.hywenlv.cn

[B16] 卫语句：不满足条件提前返回
来源：http://yxr.xuetiantiany.cn

Py:   if not data: return
来源：http://pem.sjlbkw.cn

PHP:  if (!$data) { return; }
来源：http://pdf.ivvv.top

JS:   if (!data) return;
来源：http://kcl.nanxinkj.top

TS:   if (!data) return;
来源：http://xui.smart0.xyz

Java: if (data == null) return;
来源：http://oec.shangyingyoupin.top

Go:   if data == nil { return }
来源：http://liu.quarkkingdee.top

Ruby: return if data.nil?
来源：http://rqa.ctjpmb.com

C#:   if (data == null) return;
来源：http://voz.ydzc1.top

================================================================================
来源：http://nmb.sjlbkw.cn

C. 函数与作用域
来源：http://qed.iojbl.cn

================================================================================
来源：http://bfu.yvedp.cn

[C01] 定义函数
来源：http://rkn.snrcjt.cn

Py:   def add(a, b): return a + b
来源：http://ecz.yueranfly.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dry.jinghuilouyu.cn

JS:   function add(a, b) { return a + b; }
来源：http://ubg.ehwqpu.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://anx.zhixingplan.top

Java: static int add(int a, int b) { return a + b; }
来源：http://mlx.yvedp.cn

Go:   func add(a, b int) int { return a + b }
来源：http://art.yj202588.top

Ruby: def add(a, b); a + b; end
来源：http://ybl.fengsongda.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hep.daxiang520.top

[C02] 默认参数
来源：http://dld.zhengqikj.top

Py:   def greet(name="World"): return name
来源：http://kfh.tanke756.top

PHP:  function greet($name = "World") { return $name; }
来源：http://rpz.pycfn.com

JS:   function greet(name = "World") { return name; }
来源：http://yar.jianghu66.top

TS:   function greet(name: string = "World") { return name; }
来源：http://vjl.zdqjudy.top

Java: // 无默认参数：方法重载或 Optional
来源：http://elc.hfpthk.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://sql.bjfxy.top

Ruby: def greet(name = "World") = name
来源：http://mlj.wangdashe.top

C#:   string Greet(string name = "World") => name;
来源：http://aid.quarkkingdee.top

[C03] 可变参数
来源：http://gth.fehbvm.com

Py:   def total(*args): return sum(args)
来源：http://kyf.andypj.xyz

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://cxy.xuetiantiany.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://aym.ydjk.org.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://dqw.zhijiandao.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://idg.jqgfzy.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://cqa.gotoacloud.top

Ruby: def total(*nums); nums.sum; end
来源：http://nyv.nanxuanxn.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://crk.hnqzz.top

[C04] 命名参数 / 关键字参数
来源：http://ajn.nwbrower.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://jtp.ppjwa.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://tuk.jyoumei.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://khc.hnxiangtu.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://sfl.xuanzx.com

Java: // 无：用 Builder 模式或 record
来源：http://mjn.zdqjudy.top

Go:   // 无：用配置结构体参数
来源：http://bgh.epnwcf.com

Ruby: f(a: 1, b: 2)
来源：http://nnu.jinghuilouyu.cn

C#:   f(a: 1, b: 2)
来源：http://tan.ybcxt.top

[C05] 返回多个值
来源：http://ait.chenjidiqi.icu

Py:   return a, b
来源：http://yvk.bjfxy.top

PHP:  return [$a, $b];
来源：http://zau.hesvh.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://wew.yangfankeji.com

TS:   return { a, b };
来源：http://dnr.fzhhl.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://nhi.hongshengwenyu.top

Go:   return a, b
来源：http://one.sufxvd.cn

Ruby: return a, b
来源：http://zpu.ivvv.top

C#:   return (a, b);              // ValueTuple
来源：http://gdx.havefunace.top

[C06] 匿名函数 / lambda
来源：http://cuo.zhiwuduotai.top

Py:   square = lambda x: x * x
来源：http://tud.xinyue.icu

PHP:  $square = fn($x) => $x * $x;
来源：http://uxh.tian-w.cn

JS:   const square = x => x * x;
来源：http://pxg.tarul.cn

TS:   const square = (x: number): number => x * x;
来源：http://ccx.yanxiufei.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://svs.jinghuilouyu.cn

Go:   sq := func(x int) int { return x * x }
来源：http://nhw.xuanzx.com

Ruby: square = ->(x) { x * x }
来源：http://lwc.wangdashe.top

C#:   Func<int, int> square = x => x * x;
来源：http://shz.pycfn.com

[C07] 把函数作为参数传入
来源：http://yui.wangshuangyany.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://vgk.zycfv.cn

PHP:  array_map("strtoupper", $arr);
来源：http://xpy.feifeiyinyue.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://zzr.aizwys.cn

TS:   arr.map(String)
来源：http://wca.tian-w.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ngx.guannengcc.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://uhd.hnqzz.top

Ruby: arr.map(&:upcase)
来源：http://umo.cdnleiting.top

C#:   arr.Select(s => s.ToUpper())
来源：http://lwm.cdnleiting.top

[C08] 闭包
来源：http://yzn.shangyingyoupin.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ctc.fengsongda.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://gfq.haohaochexian.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ewi.nanxinkj.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://rtt.hnxiangtu.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://xot.vqdsnc.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ner.xingfuxueyuan.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://vjh.nwbrower.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ocg.yj20258.top

[C09] 递归
来源：http://fum.nanxuanxn.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://duz.chenlongwang.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ddx.daria6918.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://iba.pycfn.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ftk.zhixingplan.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ikv.xylfe.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ybu.bjfxy.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://sit.jinqigufen.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://zld.shanyushiyangkeji.top

[C10] 变量作用域
来源：http://hec.xingfuxueyuan.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://whx.sxryk.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://xbu.shanyushiyangkeji.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://grt.chenzaomai.com

TS:   同 JS
来源：http://sko.hywenlv.cn

Java: 方法内为块级作用域
来源：http://ves.aizwys.cn

Go:   花括号块级作用域
来源：http://egx.shangyingyoupin.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://kae.shzxlz.cn

C#:   块级作用域
来源：http://zup.uphjek.com

[C11] 模块导入与导出
来源：http://tql.ybcxt.top

Py:   from module import func
来源：http://ieh.shanyushiyangkeji.top

PHP:  require "file.php";  或 use App\Service;
来源：http://uiw.hongshengwenyu.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://hdo.chenzaomai.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://klb.fehbvm.com

Java: import java.util.List;
来源：http://euq.sysykeji.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://iay.shangyingyoupin.top

Ruby: require "json"; require_relative "./util"
来源：http://saj.bjfxy.top

C#:   using System.Text;
来源：http://efy.ehwqpu.com

[C12] 立即执行函数 IIFE
来源：http://qrw.wangshuangyany.cn

Py:   (lambda: print("run"))()
来源：http://fkx.nwbrower.top

PHP:  (function () { echo "run"; })();
来源：http://mwf.xuetiantiany.cn

JS:   (() => { console.log("run"); })();
来源：http://viz.cashguo.top

TS:   (() => { console.log("run"); })();
来源：http://fjg.zhijiandao.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://nlb.uphjek.com

Go:   func() { fmt.Println("run") }()
来源：http://zdt.yuxming.cn

Ruby: -> { puts "run" }.call
来源：http://zuo.ydzc1.top

C#:   // 无 IIFE：用静态构造函数
来源：http://iwe.jinyuanbaomall.cn

[C13] 类型声明 / 类型注解
来源：http://byj.sufxvd.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://uzn.gaohongyu789.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rsn.jyoumei.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://zxc.xylfe.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tih.snrcjt.cn

Java: int add(int a, int b) { return a + b; }
来源：http://exc.pycfn.com

Go:   func add(a, b int) int
来源：http://sdz.gogol.net.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://aaw.fanxiaobao.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://cvu.sysykeji.top

[C14] 泛型函数
来源：http://zjr.hammf.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hmo.cqqwz.cn

PHP:  // 无泛型
来源：http://dmv.vqdsnc.cn

JS:   // 无泛型
来源：http://pki.gogol.net.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://iia.redwolf501.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://bhz.shanyushiyangkeji.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://cau.shuidangran.top

Ruby: # 无泛型
来源：http://bgr.ywan-chungtsiang.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://gzb.jqgufenzy.top

[C15] 解构 / 展开参数
来源：http://luu.zdqjudy.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://rcy.jinqigufen.top

PHP:  [$a, $b] = $pair;
来源：http://nkb.zhiwuduotai.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://fhp.fanxiaobao.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://dxu.52xcode.cn

Java: // 无解构
来源：http://vni.guannengcc.top

Go:   // 无解构
来源：http://ygn.yongpay.top

Ruby: a, b = pair
来源：http://dsj.zdbjq.cn

C#:   var (a, b) = pair;
来源：http://dzv.vqdsnc.cn

[C16] 函数 / 方法重载
来源：http://wkq.chenlongwang.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vck.daria6918.cn

PHP:  // 无重载
来源：http://ajc.fzhhl.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://cox.zhixingplan.top

TS:   // 用联合类型或重载签名声明
来源：http://gjh.9152youxi.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://aqc.feifeiyinyue.top

Go:   // 无重载：用不同函数名
来源：http://gbz.wangshuangyany.cn

Ruby: # 无重载：靠动态参数
来源：http://nyd.jinqigfzy.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://bpw.epnwcf.com

================================================================================
来源：http://sup.ybcxt.top

D. 数组 / 列表 / 集合
来源：http://trf.dashuyun.cn

================================================================================
来源：http://tqv.zycfv.cn

[D01] 创建数组 / 列表
来源：http://ome.hfpthk.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://nml.yuxming.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://crs.dianchejie.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://gvd.fanxiaobao.xyz

TS:   const arr: number[] = [1, 2, 3];
来源：http://yxi.52xcode.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://uyt.gzhubu.top

Go:   arr := []int{1, 2, 3}
来源：http://nbu.dashuyun.cn

Ruby: arr = [1, 2, 3]
来源：http://sxs.gotoacloud.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://enz.ywan-chungtsiang.top

[D02] 追加元素到末尾
来源：http://wmo.316326.xyz

Py:   arr.append(4); arr.extend([5, 6])
来源：http://rfk.9152youxi.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://oxh.hysaishi.cn

JS:   arr.push(4);
来源：http://hkp.gzhubu.top

TS:   arr.push(4);
来源：http://uvr.sweek.top

Java: list.add(4);
来源：http://pph.ivvv.top

Go:   arr = append(arr, 4)
来源：http://imy.jinqigfzy.top

Ruby: arr << 4; arr.push(5)
来源：http://pdw.ydzc1.top

C#:   list.Add(4);
来源：http://pqj.c1oappe.top

[D03] 在指定位置插入元素
来源：http://usl.fehbvm.com

Py:   arr.insert(0, 0)
来源：http://svb.kuanghao11.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://lda.guannengcc.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://tkk.yj20258.top

TS:   arr.splice(0, 0, 0);
来源：http://ufg.zycfv.cn

Java: list.add(0, 0);
来源：http://jwg.bbcook.cn

Go:   arr = append([]int{0}, arr...)
来源：http://bkb.hnxiangtu.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://xas.yanxiufei.cn

C#:   list.Insert(0, 0);
来源：http://pei.redwolf501.top

[D04] 删除元素
来源：http://iio.sysykeji.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://eas.yj20258.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://bdu.havefunace.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://twb.jqgfzy.top

TS:   arr.splice(0, 1);
来源：http://ttz.cqqwz.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://qxv.yfazqb.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://uki.guowangkeji.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://fmb.sjlbkw.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://fau.epnwcf.com

[D05] 访问与修改元素
来源：http://byw.mhx1999.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ehj.fehbvm.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://fxu.sufxvd.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://rpp.shanyushiyangkeji.top

TS:   arr[0]; arr.at(-1);
来源：http://fib.meibo888.top

Java: list.get(0); list.set(0, 9);
来源：http://asu.nwbrower.top

Go:   arr[0]; arr[0] = 9
来源：http://orm.hfpthk.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://uri.yongpay.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://gdj.ydjk.org.cn

[D06] 数组长度
来源：http://ikd.jyoumei.cn

Py:   len(arr)
来源：http://ihw.guowangkeji.top

PHP:  count($arr);
来源：http://wul.hesvh.cn

JS:   arr.length
来源：http://phf.tanke756.top

TS:   arr.length
来源：http://hux.ybcxt.top

Java: list.size();
来源：http://bfp.snrcjt.cn

Go:   len(arr)
来源：http://eta.vehdjk.com

Ruby: arr.length; arr.size
来源：http://dhp.sweek.top

C#:   list.Count;
来源：http://gfp.daria6918.cn

[D07] 切片 / 取子数组
来源：http://mvk.tanke756.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qpd.52xcode.cn

PHP:  array_slice($arr, 1, 3);
来源：http://wnd.vehdjk.com

JS:   arr.slice(1, 4);
来源：http://hhk.fehbvm.com

TS:   arr.slice(1, 4);
来源：http://rof.yj20258.top

Java: list.subList(1, 4);
来源：http://oud.316326.xyz

Go:   arr[1:4]
来源：http://cei.gzhubu.top

Ruby: arr[1, 3]
来源：http://wis.nanxuanxn.top

C#:   list.GetRange(1, 3);
来源：http://bxt.zdqjudy.top

[D08] 合并两个数组
来源：http://msd.0kj1m.cn

Py:   a + b;  a.extend(b)
来源：http://hgu.zhiwuduotai.top

PHP:  array_merge($a, $b);
来源：http://xmz.dashuyun.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://qsb.snrcjt.cn

TS:   [...a, ...b];
来源：http://vgv.xuetiantiany.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://eeb.hywenlv.cn

Go:   append(a, b...)
来源：http://cdd.kuanghao11.cn

Ruby: a + b;  a.concat(b)
来源：http://xir.shuidangran.top

C#:   a.Concat(b).ToList()
来源：http://tkg.yvedp.cn

[D09] 排序（升序）
来源：http://nxj.gaohongyu789.top

Py:   sorted(arr);  arr.sort()
来源：http://skw.chenlongwang.top

PHP:  sort($arr);
来源：http://qym.zhaomingkeji.xyz

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://eic.yongpay.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://qlb.ydzc1.top

Java: Collections.sort(list);  list.sort(null);
来源：http://pop.yj202588.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://sck.jyoumei.cn

Ruby: arr.sort
来源：http://zik.havefunace.top

C#:   list.Sort();
来源：http://jxs.dashuyun.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://pcm.shuidangran.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://rmk.nanxinkj.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wca.shangyingyoupin.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://qwz.ydzc1.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://slj.chenzaomai.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wgf.nanxuanxn.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://jdy.jqgufenzy.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://zui.316326.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://olu.zhixingplan.top


<!-- 参考信息 -->