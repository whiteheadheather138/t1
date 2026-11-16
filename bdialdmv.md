代发 wailian999

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://tzb.redwolf501.top

Ruby: (0...10).step(2).to_a
来源：http://ahc.chenzaomai.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://sco.daxiang520.top

[B12] 跳出多层循环
来源：http://pyd.yangfankeji.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://irr.yanxiufei.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://shp.ctjpmb.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://dic.daria6918.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://gut.mhx1999.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://qij.fehbvm.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ikv.yangfankeji.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://abc.fengsongda.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wiq.yj20258888.top

[B13] 判断是否为数字
来源：http://ape.9152youxi.cn

Py:   isinstance(x, (int, float))
来源：http://kla.xziqi.cn

PHP:  is_numeric($x)
来源：http://nic.wangshuangyany.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cmj.dashuyun.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://uxd.gogol.net.cn

Java: x instanceof Number
来源：http://ksb.nanxuanxn.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://qwr.ivvv.top

Ruby: x.is_a?(Numeric)
来源：http://nnu.vehdjk.com

C#:   x is int or double or decimal
来源：http://evy.chenzaomai.com

[B14] 判断值是否在集合内
来源：http://ccw.haohaochexian.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://fon.wangdashe.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://tjg.cashguo.top

JS:   [1, 2, 3].includes(x)
来源：http://cql.sysykeji.top

TS:   [1, 2, 3].includes(x)
来源：http://lma.cucudq.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://nce.zhoulong.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://kki.daxiang520.top

Ruby: [1, 2, 3].include?(x)
来源：http://ewj.hfpthk.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://zbt.yj20258.top

[B15] 布尔运算与取反
来源：http://kno.shanyushiyangtech.top

Py:   a and b or not c
来源：http://kgn.aizwys.cn

PHP:  $a && $b || !$c
来源：http://nqc.fehbvm.com

JS:   a && b || !c
来源：http://jzt.nanxuanxn.top

TS:   a && b || !c
来源：http://ddr.guowangkeji.top

Java: a && b || !c
来源：http://ecl.yonumen.top

Go:   a && b || !c
来源：http://rwg.wangshuangyany.cn

Ruby: a && b || !c
来源：http://dke.yonumen.top

C#:   a && b || !c
来源：http://qpq.tanke756.top

[B16] 卫语句：不满足条件提前返回
来源：http://ssr.nanxinkj.top

Py:   if not data: return
来源：http://bog.cqqwz.cn

PHP:  if (!$data) { return; }
来源：http://xvp.cqqwz.cn

JS:   if (!data) return;
来源：http://upu.pengpengdd.cyou

TS:   if (!data) return;
来源：http://ovz.nwbrower.top

Java: if (data == null) return;
来源：http://oge.zhijiandao.cn

Go:   if data == nil { return }
来源：http://svd.shanyushiyangtech.top

Ruby: return if data.nil?
来源：http://obi.tian-w.cn

C#:   if (data == null) return;
来源：http://ciz.havefunace.top

================================================================================
来源：http://ukl.gzhubu.top

C. 函数与作用域
来源：http://qde.yanxiufei.cn

================================================================================
来源：http://yxi.cdnleiting.top

[C01] 定义函数
来源：http://jtb.hnqzz.top

Py:   def add(a, b): return a + b
来源：http://qph.shanyushiyangtech.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xlf.tarul.cn

JS:   function add(a, b) { return a + b; }
来源：http://mgr.yangfankeji.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rbk.tianlin.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://hgm.yfazqb.com

Go:   func add(a, b int) int { return a + b }
来源：http://byf.jqgfzy.top

Ruby: def add(a, b); a + b; end
来源：http://rtz.gaohongyu789.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://pci.xinyue.icu

[C02] 默认参数
来源：http://bhi.xuanzx.com

Py:   def greet(name="World"): return name
来源：http://arw.iojbl.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://idz.yangfankeji.com

JS:   function greet(name = "World") { return name; }
来源：http://qic.tian-w.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ubn.redwolf501.top

Java: // 无默认参数：方法重载或 Optional
来源：http://taa.yangfankeji.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hju.ivvv.top

Ruby: def greet(name = "World") = name
来源：http://cja.pengpengdd.cyou

C#:   string Greet(string name = "World") => name;
来源：http://lwk.sxryk.cn

[C03] 可变参数
来源：http://hhl.nwbrower.top

Py:   def total(*args): return sum(args)
来源：http://tfk.ywan-chungtsiang.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://kjs.shuidangran.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://tpw.birdmap.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xwf.jinqigufen.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ysl.xinyue.icu

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wsy.andypj.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://tir.jinghuilouyu.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ylm.wangshuangyany.cn

[C04] 命名参数 / 关键字参数
来源：http://uhs.daria6918.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://cpj.316326.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ral.snrcjt.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xgh.hesvh.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xyz.hnqzz.top

Java: // 无：用 Builder 模式或 record
来源：http://fot.fehbvm.com

Go:   // 无：用配置结构体参数
来源：http://wxj.snrcjt.cn

Ruby: f(a: 1, b: 2)
来源：http://yzs.fanxiaobao.xyz

C#:   f(a: 1, b: 2)
来源：http://zlg.vehdjk.com

[C05] 返回多个值
来源：http://hzy.pycfn.com

Py:   return a, b
来源：http://kdx.ydjk.org.cn

PHP:  return [$a, $b];
来源：http://qhs.kuanghao11.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://oai.dianchejie.cn

TS:   return { a, b };
来源：http://rae.haohaochexian.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://qcm.hnxiangtu.top

Go:   return a, b
来源：http://mkw.xylfe.cn

Ruby: return a, b
来源：http://jvw.yj20258.top

C#:   return (a, b);              // ValueTuple
来源：http://jet.0kj1m.cn

[C06] 匿名函数 / lambda
来源：http://hnp.jianghu66.top

Py:   square = lambda x: x * x
来源：http://cqk.hongshengwenyu.top

PHP:  $square = fn($x) => $x * $x;
来源：http://hgu.shangyingyoupin.top

JS:   const square = x => x * x;
来源：http://mvs.sysykeji.top

TS:   const square = (x: number): number => x * x;
来源：http://mbv.zycfv.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://jvd.hysaishi.cn

Go:   sq := func(x int) int { return x * x }
来源：http://gph.dashuyun.cn

Ruby: square = ->(x) { x * x }
来源：http://pez.birdmap.top

C#:   Func<int, int> square = x => x * x;
来源：http://bjf.yj202588.top

[C07] 把函数作为参数传入
来源：http://mhl.sxryk.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://yvg.aibaodan.cn

PHP:  array_map("strtoupper", $arr);
来源：http://jfs.dianchejie.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://vsx.haohaochexian.top

TS:   arr.map(String)
来源：http://ymd.pengpengdd.cyou

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://fsx.gotoacloud.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://swh.daria6918.cn

Ruby: arr.map(&:upcase)
来源：http://ujv.zhiwuduotai.top

C#:   arr.Select(s => s.ToUpper())
来源：http://suj.hywenlv.cn

[C08] 闭包
来源：http://kpn.jqgfzy.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://vim.9152youxi.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ubl.jqgufenzy.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mut.hnxiangtu.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ett.hnqzz.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://zoh.chenzaomai.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://fps.52xcode.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://dcs.xylfe.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hhq.yfazqb.com

[C09] 递归
来源：http://ela.gaohongyu789.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ejd.ywan-chungtsiang.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://lev.kuanghao11.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cls.hongshengwenyu.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bkd.316326.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://qyj.pycfn.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://azg.9152youxi.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://iah.meibo888.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://crh.ehwqpu.com

[C10] 变量作用域
来源：http://qos.wangshuangyany.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qcc.gotoacloud.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://fzz.ppjwa.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://dnx.snrcjt.cn

TS:   同 JS
来源：http://efi.snrcjt.cn

Java: 方法内为块级作用域
来源：http://gyt.birdmap.top

Go:   花括号块级作用域
来源：http://pov.svipenyu.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://fqb.0kj1m.cn

C#:   块级作用域
来源：http://ful.hesvh.cn

[C11] 模块导入与导出
来源：http://eoa.yangfankeji.com

Py:   from module import func
来源：http://kcj.ppjwa.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://uco.jinqigufen.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://een.hysaishi.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://zcx.vehdjk.com

Java: import java.util.List;
来源：http://akg.ydzc1.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://gjf.jinyuanbaomall.cn

Ruby: require "json"; require_relative "./util"
来源：http://asm.bjfxy.top

C#:   using System.Text;
来源：http://yex.c1oappe.top

[C12] 立即执行函数 IIFE
来源：http://tlr.hcnkem.com

Py:   (lambda: print("run"))()
来源：http://wru.vqdsnc.cn

PHP:  (function () { echo "run"; })();
来源：http://tvq.jqgfzy.top

JS:   (() => { console.log("run"); })();
来源：http://hcg.jianghu66.top

TS:   (() => { console.log("run"); })();
来源：http://ceg.ydjk.org.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://etw.svipenyu.cn

Go:   func() { fmt.Println("run") }()
来源：http://vgu.jianghu66.top

Ruby: -> { puts "run" }.call
来源：http://ott.hongshengwenyu.top

C#:   // 无 IIFE：用静态构造函数
来源：http://hwy.cheryme.top

[C13] 类型声明 / 类型注解
来源：http://uyq.mhx1999.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://jaa.chenzaomai.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nae.fzhhl.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://juv.xuetiantiany.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sak.yanxiufei.cn

Java: int add(int a, int b) { return a + b; }
来源：http://uhs.tianlin.xyz

Go:   func add(a, b int) int
来源：http://owz.pycfn.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://aul.zdbjq.cn

C#:   int Add(int a, int b) => a + b;
来源：http://myb.hnqzz.top

[C14] 泛型函数
来源：http://fzq.jlsjyb.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mno.yvedp.cn

PHP:  // 无泛型
来源：http://jqq.yj20258888.top

JS:   // 无泛型
来源：http://fzw.pengpengdd.cyou

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://jbr.shanyushiyangtech.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://lbg.jqgfzy.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://kwq.gogol.net.cn

Ruby: # 无泛型
来源：http://kik.ivvv.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://oez.sufxvd.cn

[C15] 解构 / 展开参数
来源：http://opp.shuidangran.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ctp.zhixingplan.top

PHP:  [$a, $b] = $pair;
来源：http://yjr.yanxiufei.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://fof.zhoulong.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ugk.snrcjt.cn

Java: // 无解构
来源：http://kyn.fktsv.cn

Go:   // 无解构
来源：http://hle.xuanzx.com

Ruby: a, b = pair
来源：http://omi.bjfxy.top

C#:   var (a, b) = pair;
来源：http://uro.chenlongwang.top

[C16] 函数 / 方法重载
来源：http://zqh.fengsongda.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://fmo.svipenyu.cn

PHP:  // 无重载
来源：http://gug.svipenyu.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://yhv.daria6918.cn

TS:   // 用联合类型或重载签名声明
来源：http://lrf.tian-w.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://bds.ehwqpu.com

Go:   // 无重载：用不同函数名
来源：http://fsh.ydzc1.top

Ruby: # 无重载：靠动态参数
来源：http://jmo.sxryk.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ccs.yangfankeji.com

================================================================================
来源：http://tjj.hywenlv.cn

D. 数组 / 列表 / 集合
来源：http://def.nwbrower.top

================================================================================
来源：http://vkb.jqgfzy.top

[D01] 创建数组 / 列表
来源：http://nyz.zhaomingkeji.xyz

Py:   arr = [1, 2, 3];  empty = []
来源：http://cph.0kj1m.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://fgl.shuidangran.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://twg.kuanghao11.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ltl.aibaodan.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://zny.yj202588.top

Go:   arr := []int{1, 2, 3}
来源：http://yia.wangdashe.top

Ruby: arr = [1, 2, 3]
来源：http://feu.9152youxi.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://njl.hywenlv.cn

[D02] 追加元素到末尾
来源：http://nvc.nanxinkj.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://jsh.jinghuilouyu.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://oof.gaohongyu789.top

JS:   arr.push(4);
来源：http://rql.c1oappe.top

TS:   arr.push(4);
来源：http://kvm.hywenlv.cn

Java: list.add(4);
来源：http://amh.ehwqpu.com

Go:   arr = append(arr, 4)
来源：http://ptf.gotoacloud.top

Ruby: arr << 4; arr.push(5)
来源：http://nap.smart0.xyz

C#:   list.Add(4);
来源：http://sjm.xingfuxueyuan.xyz

[D03] 在指定位置插入元素
来源：http://bfm.havefunace.top

Py:   arr.insert(0, 0)
来源：http://fsz.jqgfzy.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://sla.daria6918.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://goy.yonumen.top

TS:   arr.splice(0, 0, 0);
来源：http://csb.gogol.net.cn

Java: list.add(0, 0);
来源：http://asg.sjlbkw.cn

Go:   arr = append([]int{0}, arr...)
来源：http://osp.cucudq.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://vnc.cucudq.cn

C#:   list.Insert(0, 0);
来源：http://mkr.cheryme.top

[D04] 删除元素
来源：http://ygz.sjlbkw.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://dlq.gzhubu.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://qhf.shanyushiyangtech.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://qfe.nwbrower.top

TS:   arr.splice(0, 1);
来源：http://lri.chenzaomai.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://guk.feifeiyinyue.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://grv.chenzaomai.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ikc.guowangkeji.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://kwg.cdnleiting.top

[D05] 访问与修改元素
来源：http://lkt.iojbl.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://pvf.xuetiantiany.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://vuj.shuidangran.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://tjq.jlsjyb.cn

TS:   arr[0]; arr.at(-1);
来源：http://yax.xylfe.cn

Java: list.get(0); list.set(0, 9);
来源：http://vmv.nanxuanxn.top

Go:   arr[0]; arr[0] = 9
来源：http://etb.xziqi.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://sst.52xcode.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://edq.daxiang520.top

[D06] 数组长度
来源：http://nfz.52xcode.cn

Py:   len(arr)
来源：http://zwl.jinqigufen.top

PHP:  count($arr);
来源：http://tuj.xuetiantiany.cn

JS:   arr.length
来源：http://oib.zhongyouzk.top

TS:   arr.length
来源：http://nnj.jianghu66.top

Java: list.size();
来源：http://mzr.zycfv.cn

Go:   len(arr)
来源：http://iwe.snrcjt.cn

Ruby: arr.length; arr.size
来源：http://xvv.yuxming.cn

C#:   list.Count;
来源：http://tya.fktsv.cn

[D07] 切片 / 取子数组
来源：http://fzw.zhijiandao.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://jlh.fanxiaobao.xyz

PHP:  array_slice($arr, 1, 3);
来源：http://vbx.chenzaomai.com

JS:   arr.slice(1, 4);
来源：http://xdg.svipenyu.cn

TS:   arr.slice(1, 4);
来源：http://zxy.yj20258.top

Java: list.subList(1, 4);
来源：http://xed.chenzaomai.com

Go:   arr[1:4]
来源：http://trx.birdmap.top

Ruby: arr[1, 3]
来源：http://kfr.ydzc1.top

C#:   list.GetRange(1, 3);
来源：http://nrg.aizwys.cn

[D08] 合并两个数组
来源：http://cvb.jqgufenzy.top

Py:   a + b;  a.extend(b)
来源：http://gnz.fehbvm.com

PHP:  array_merge($a, $b);
来源：http://azd.ppjwa.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ffz.jinyuanbaomall.cn

TS:   [...a, ...b];
来源：http://dpy.nanxuanxn.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://tpi.wangshuangyany.cn

Go:   append(a, b...)
来源：http://abv.ctjpmb.com

Ruby: a + b;  a.concat(b)
来源：http://uqu.sufxvd.cn

C#:   a.Concat(b).ToList()
来源：http://epo.yonumen.top

[D09] 排序（升序）
来源：http://ulu.zhoulong.xyz

Py:   sorted(arr);  arr.sort()
来源：http://qnh.sweek.top

PHP:  sort($arr);
来源：http://vxv.gaohongyu789.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://qke.hywenlv.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://rct.redwolf501.top

Java: Collections.sort(list);  list.sort(null);
来源：http://oyg.fzhhl.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://jwq.cdnleiting.top

Ruby: arr.sort
来源：http://cew.gaohongyu789.top

C#:   list.Sort();
来源：http://uai.nanxuanxn.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://bbo.yonumen.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ivh.fanxiaobao.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://olj.c1oappe.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://avw.zdqjudy.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://jss.smart0.xyz

Java: list.sort(Comparator.comparing(Person::age));
来源：http://pxu.fktsv.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mvd.dianchejie.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://lit.hnqzz.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://xhc.yongpay.top

[D11] 反转数组
来源：http://hlh.shanyushiyangkeji.top

Py:   arr[::-1];  arr.reverse()
来源：http://jjb.nanxinkj.top

PHP:  array_reverse($arr);
来源：http://psj.zhijiandao.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://gpl.vehdjk.com

TS:   [...arr].reverse();
来源：http://tlx.tianlin.xyz

Java: Collections.reverse(list);
来源：http://pip.pengpengdd.cyou

Go:   slices.Reverse(arr)
来源：http://zra.jinghuilouyu.cn

Ruby: arr.reverse
来源：http://lwv.fanxiaobao.xyz

C#:   list.Reverse();
来源：http://trk.smart0.xyz

[D12] 查找元素下标
来源：http://yay.zhixingplan.top

Py:   arr.index(x);  x in arr
来源：http://ffu.tianlin.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ach.yanxiufei.cn


<!-- 参考信息 -->