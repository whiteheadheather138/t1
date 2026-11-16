代发 wailian999

Go:   a && b || !c
来源：http://yjs.nanxinkj.top

Ruby: a && b || !c
来源：http://tma.hfpthk.cn

C#:   a && b || !c
来源：http://kbi.yangfankeji.com

[B16] 卫语句：不满足条件提前返回
来源：http://gru.ppjwa.cn

Py:   if not data: return
来源：http://efr.hywenlv.cn

PHP:  if (!$data) { return; }
来源：http://jsm.dianchejie.cn

JS:   if (!data) return;
来源：http://qua.nanxuanxn.top

TS:   if (!data) return;
来源：http://bda.tianlin.xyz

Java: if (data == null) return;
来源：http://mia.316326.xyz

Go:   if data == nil { return }
来源：http://oee.zdbjq.cn

Ruby: return if data.nil?
来源：http://ive.ctjpmb.com

C#:   if (data == null) return;
来源：http://nmx.chenlongwang.top

================================================================================
来源：http://zoz.sxryk.cn

C. 函数与作用域
来源：http://wok.316326.xyz

================================================================================
来源：http://ruy.yj20258888.top

[C01] 定义函数
来源：http://adg.guannengcc.top

Py:   def add(a, b): return a + b
来源：http://zfk.sjlbkw.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ktx.hywenlv.cn

JS:   function add(a, b) { return a + b; }
来源：http://qlp.hfpthk.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mio.redwolf501.top

Java: static int add(int a, int b) { return a + b; }
来源：http://dgf.tian-w.cn

Go:   func add(a, b int) int { return a + b }
来源：http://sex.ydjk.org.cn

Ruby: def add(a, b); a + b; end
来源：http://flg.xziqi.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://qbu.chenzaomai.com

[C02] 默认参数
来源：http://fpa.tanke756.top

Py:   def greet(name="World"): return name
来源：http://mpe.hnxiangtu.top

PHP:  function greet($name = "World") { return $name; }
来源：http://rlc.cdnleiting.top

JS:   function greet(name = "World") { return name; }
来源：http://zoa.kuanghao11.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://jnq.zycfv.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://crd.yfazqb.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://qls.sweek.top

Ruby: def greet(name = "World") = name
来源：http://sbp.gogol.net.cn

C#:   string Greet(string name = "World") => name;
来源：http://evt.ivvv.top

[C03] 可变参数
来源：http://owv.zycfv.cn

Py:   def total(*args): return sum(args)
来源：http://zbr.fzhhl.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://vlh.zycfv.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wrx.xinyue.icu

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://eql.sweek.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mtk.shzxlz.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://nqr.hongshengwenyu.top

Ruby: def total(*nums); nums.sum; end
来源：http://xjr.hongshengwenyu.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://rbz.pengpengdd.cyou

[C04] 命名参数 / 关键字参数
来源：http://ulb.zhongyouzk.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://uow.sjlbkw.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://eec.wangshuangyany.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xcz.jianghu66.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ajn.hfpthk.cn

Java: // 无：用 Builder 模式或 record
来源：http://nww.wangshuangyany.cn

Go:   // 无：用配置结构体参数
来源：http://aul.ybcxt.top

Ruby: f(a: 1, b: 2)
来源：http://suq.ivvv.top

C#:   f(a: 1, b: 2)
来源：http://hgv.aibaodan.cn

[C05] 返回多个值
来源：http://lpq.shzxlz.cn

Py:   return a, b
来源：http://ayz.quarkkingdee.top

PHP:  return [$a, $b];
来源：http://thc.hnqzz.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://xfx.fzhhl.top

TS:   return { a, b };
来源：http://pwo.ywan-chungtsiang.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hir.meibo888.top

Go:   return a, b
来源：http://bxr.hcnkem.com

Ruby: return a, b
来源：http://leb.zhengqikj.top

C#:   return (a, b);              // ValueTuple
来源：http://hod.tarul.cn

[C06] 匿名函数 / lambda
来源：http://yov.hnqzz.top

Py:   square = lambda x: x * x
来源：http://lky.jinghuilouyu.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://kkj.yuxming.cn

JS:   const square = x => x * x;
来源：http://xsc.cashguo.top

TS:   const square = (x: number): number => x * x;
来源：http://hji.cucudq.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://sjs.yuanzhike.top

Go:   sq := func(x int) int { return x * x }
来源：http://elw.iojbl.cn

Ruby: square = ->(x) { x * x }
来源：http://lkl.hesvh.cn

C#:   Func<int, int> square = x => x * x;
来源：http://dwv.yongpay.top

[C07] 把函数作为参数传入
来源：http://xjt.hnqzz.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://afb.hongshengwenyu.top

PHP:  array_map("strtoupper", $arr);
来源：http://fxz.jinyuanbaomall.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://vyw.cqqwz.cn

TS:   arr.map(String)
来源：http://zog.snrcjt.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://qfp.pengpengdd.cyou

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://vqs.cdnleiting.top

Ruby: arr.map(&:upcase)
来源：http://zao.havefunace.top

C#:   arr.Select(s => s.ToUpper())
来源：http://ebm.kuanghao11.cn

[C08] 闭包
来源：http://ouj.xinyue.icu

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://flf.shuidangran.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ggc.ctjpmb.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://zwi.sufxvd.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://fkp.vehdjk.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ita.ivvv.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://uyj.mhx1999.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://zjw.ybcxt.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://vwp.jinyuanbaomall.cn

[C09] 递归
来源：http://exu.iojbl.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://vce.vehdjk.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://chb.yj202588.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://epz.snrcjt.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gly.jinqigfzy.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ljc.yvedp.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://zca.bbcook.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://zxu.gaohongyu789.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://vvs.yj202588.top

[C10] 变量作用域
来源：http://zhb.hongshengwenyu.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://bcr.haohaochexian.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://jcd.ydjk.org.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mwi.hfpthk.cn

TS:   同 JS
来源：http://hgb.meibo888.top

Java: 方法内为块级作用域
来源：http://vio.hywenlv.cn

Go:   花括号块级作用域
来源：http://ars.zhaomingkeji.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://zed.52xcode.cn

C#:   块级作用域
来源：http://cgd.316326.xyz

[C11] 模块导入与导出
来源：http://eka.xziqi.cn

Py:   from module import func
来源：http://unl.cucudq.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://rrb.zhongyouzk.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://kvl.haohaochexian.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://dku.wangshuangyany.cn

Java: import java.util.List;
来源：http://aje.sufxvd.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://cho.aizwys.cn

Ruby: require "json"; require_relative "./util"
来源：http://cbl.fanxiaobao.xyz

C#:   using System.Text;
来源：http://kbi.shanyushiyangtech.top

[C12] 立即执行函数 IIFE
来源：http://pck.nwbrower.top

Py:   (lambda: print("run"))()
来源：http://ldh.guannengcc.top

PHP:  (function () { echo "run"; })();
来源：http://lyb.yfazqb.com

JS:   (() => { console.log("run"); })();
来源：http://bso.quarkkingdee.top

TS:   (() => { console.log("run"); })();
来源：http://pom.jinqigfzy.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://eyh.smart0.xyz

Go:   func() { fmt.Println("run") }()
来源：http://avr.hammf.cn

Ruby: -> { puts "run" }.call
来源：http://xxu.cqqwz.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://cel.cashguo.top

[C13] 类型声明 / 类型注解
来源：http://hqj.yvedp.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wva.bbcook.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jsz.yj20258888.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://cxm.meibo888.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nfo.jinghuilouyu.cn

Java: int add(int a, int b) { return a + b; }
来源：http://tss.fengsongda.top

Go:   func add(a, b int) int
来源：http://xyu.cucudq.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://zfl.guowangkeji.top

C#:   int Add(int a, int b) => a + b;
来源：http://mfc.sxryk.cn

[C14] 泛型函数
来源：http://ger.jinqigfzy.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://svf.hnqzz.top

PHP:  // 无泛型
来源：http://miq.hysaishi.cn

JS:   // 无泛型
来源：http://fvb.iojbl.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://qwg.sxryk.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://qvo.bbcook.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://jxk.nanxuanxn.top

Ruby: # 无泛型
来源：http://msp.feifeiyinyue.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://vfe.bbcook.cn

[C15] 解构 / 展开参数
来源：http://dex.hfpthk.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://bah.andypj.xyz

PHP:  [$a, $b] = $pair;
来源：http://fdf.gogol.net.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wqf.yj20258888.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://agr.shuidangran.top

Java: // 无解构
来源：http://pgg.gaohongyu789.top

Go:   // 无解构
来源：http://qgn.bbcook.cn

Ruby: a, b = pair
来源：http://ksr.ywan-chungtsiang.top

C#:   var (a, b) = pair;
来源：http://gtc.xylfe.cn

[C16] 函数 / 方法重载
来源：http://mtn.xziqi.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hdh.sweek.top

PHP:  // 无重载
来源：http://ohs.daria6918.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://wvd.cqqwz.cn

TS:   // 用联合类型或重载签名声明
来源：http://gnw.uphjek.com

Java: void f(int a) {}  void f(String a) {}
来源：http://uim.zhixingplan.top

Go:   // 无重载：用不同函数名
来源：http://haz.jinqigufen.top

Ruby: # 无重载：靠动态参数
来源：http://czp.jqgfzy.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://jie.cdnleiting.top

================================================================================
来源：http://sbv.cheryme.top

D. 数组 / 列表 / 集合
来源：http://rmo.ctjpmb.com

================================================================================
来源：http://yyg.pycfn.com

[D01] 创建数组 / 列表
来源：http://cfy.sxryk.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://dxo.sjlbkw.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hur.cheryme.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://fmc.yongpay.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://bia.52xcode.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://upn.jinyuanbaomall.cn

Go:   arr := []int{1, 2, 3}
来源：http://bco.andypj.xyz

Ruby: arr = [1, 2, 3]
来源：http://btc.sufxvd.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://xmz.meibo888.top

[D02] 追加元素到末尾
来源：http://adl.zhongyouzk.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://jkt.jinqigfzy.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://fki.ydzc1.top

JS:   arr.push(4);
来源：http://zdh.zhoulong.xyz

TS:   arr.push(4);
来源：http://kpe.kuanghao11.cn

Java: list.add(4);
来源：http://rsw.meibo888.top

Go:   arr = append(arr, 4)
来源：http://ebz.9152youxi.cn

Ruby: arr << 4; arr.push(5)
来源：http://att.hesvh.cn

C#:   list.Add(4);
来源：http://gcf.zhixingplan.top

[D03] 在指定位置插入元素
来源：http://mbq.pycfn.com

Py:   arr.insert(0, 0)
来源：http://jhg.zhengqikj.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://yil.ybcxt.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://yod.gzhubu.top

TS:   arr.splice(0, 0, 0);
来源：http://oyz.fengsongda.top

Java: list.add(0, 0);
来源：http://gzn.meibo888.top

Go:   arr = append([]int{0}, arr...)
来源：http://day.yvedp.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://lvm.feifeiyinyue.top

C#:   list.Insert(0, 0);
来源：http://vjv.hcnkem.com

[D04] 删除元素
来源：http://qdm.nwbrower.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://aqr.uphjek.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://dvt.bjfxy.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://nmn.kuanghao11.cn

TS:   arr.splice(0, 1);
来源：http://pke.kuanghao11.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://geg.zdbjq.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://kpv.shuidangran.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://gwp.ehwqpu.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://kgl.bjfxy.top

[D05] 访问与修改元素
来源：http://gys.yueranfly.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blr.yj202588.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://uxy.zhoulong.xyz

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://rqa.hnxiangtu.top

TS:   arr[0]; arr.at(-1);
来源：http://crt.vqdsnc.cn

Java: list.get(0); list.set(0, 9);
来源：http://ysx.zhaomingkeji.xyz

Go:   arr[0]; arr[0] = 9
来源：http://uiw.wangshuangyany.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://att.gaohongyu789.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://pmk.tian-w.cn

[D06] 数组长度
来源：http://fqd.yj20258.top

Py:   len(arr)
来源：http://hml.cheryme.top

PHP:  count($arr);
来源：http://rqy.nwbrower.top

JS:   arr.length
来源：http://woi.mhx1999.top

TS:   arr.length
来源：http://dto.uphjek.com

Java: list.size();
来源：http://mvh.hammf.cn

Go:   len(arr)
来源：http://lit.cheryme.top

Ruby: arr.length; arr.size
来源：http://dhl.redwolf501.top

C#:   list.Count;
来源：http://mva.iojbl.cn

[D07] 切片 / 取子数组
来源：http://lop.yuxming.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://oal.nwbrower.top

PHP:  array_slice($arr, 1, 3);
来源：http://ljh.xingfuxueyuan.xyz

JS:   arr.slice(1, 4);
来源：http://eey.chenzaomai.com

TS:   arr.slice(1, 4);
来源：http://nry.shanyushiyangkeji.top

Java: list.subList(1, 4);
来源：http://fok.birdmap.top

Go:   arr[1:4]
来源：http://eef.zdqjudy.top

Ruby: arr[1, 3]
来源：http://rxw.wangshuangyany.cn

C#:   list.GetRange(1, 3);
来源：http://oqv.tian-w.cn

[D08] 合并两个数组
来源：http://knr.snrcjt.cn

Py:   a + b;  a.extend(b)
来源：http://mbu.yj20258888.top

PHP:  array_merge($a, $b);
来源：http://app.zhixingplan.top

JS:   [...a, ...b];  a.concat(b);
来源：http://dbx.cdnleiting.top

TS:   [...a, ...b];
来源：http://ccb.jinqigfzy.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://csm.9152youxi.cn

Go:   append(a, b...)
来源：http://cce.jinyuanbaomall.cn

Ruby: a + b;  a.concat(b)
来源：http://rpq.xziqi.cn

C#:   a.Concat(b).ToList()
来源：http://hbh.uphjek.com

[D09] 排序（升序）
来源：http://zzs.gogol.net.cn

Py:   sorted(arr);  arr.sort()
来源：http://jnp.jlsjyb.cn

PHP:  sort($arr);
来源：http://gra.jqgfzy.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://uwv.fehbvm.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://sny.nanxinkj.top

Java: Collections.sort(list);  list.sort(null);
来源：http://lqb.aizwys.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://pgt.chenzaomai.com

Ruby: arr.sort
来源：http://qwo.wangshuangyany.cn

C#:   list.Sort();
来源：http://fkj.fengsongda.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://udo.hnqzz.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://dbb.sweek.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dht.hcnkem.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://duh.hnqzz.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://yvr.cdnleiting.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wtf.52xcode.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://tau.yj20258888.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://xbp.jyoumei.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qfl.zhoulong.xyz

[D11] 反转数组
来源：http://lan.yj20258.top

Py:   arr[::-1];  arr.reverse()
来源：http://hwo.aizwys.cn

PHP:  array_reverse($arr);
来源：http://unk.guannengcc.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://kny.chenzaomai.com

TS:   [...arr].reverse();
来源：http://cbm.zycfv.cn

Java: Collections.reverse(list);
来源：http://tve.nanxuanxn.top

Go:   slices.Reverse(arr)
来源：http://ept.zhongyouzk.top

Ruby: arr.reverse
来源：http://zpr.sxryk.cn

C#:   list.Reverse();
来源：http://dqt.andypj.xyz

[D12] 查找元素下标
来源：http://pqy.sweek.top

Py:   arr.index(x);  x in arr
来源：http://gwp.feifeiyinyue.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ren.yongpay.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xxg.epnwcf.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ppx.xingfuxueyuan.xyz

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://iyz.cashguo.top

Go:   slices.Index(arr, x)
来源：http://nwb.ppjwa.cn

Ruby: arr.index(x)
来源：http://inp.nanxuanxn.top

C#:   list.IndexOf(x);
来源：http://mtd.hongshengwenyu.top

[D13] 过滤（保留满足条件的）
来源：http://lyg.kuanghao11.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wdw.xuanzx.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://vaf.svipenyu.cn

JS:   arr.filter(x => x > 3)
来源：http://xrt.sufxvd.cn

TS:   arr.filter(x => x > 3)
来源：http://jsb.zhixingplan.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://lgb.zhixingplan.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://kyn.jyoumei.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ofx.jinghuilouyu.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://idr.hnqzz.top

[D14] 映射转换（每个元素变形）
来源：http://isf.hesvh.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hkm.hfpthk.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://oow.sweek.top

JS:   arr.map(x => x * 2)
来源：http://xzq.aizwys.cn

TS:   arr.map(x => x * 2)
来源：http://vwx.vqdsnc.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://svo.yfazqb.com

Go:   // 手写循环
来源：http://wav.wangdashe.top

Ruby: arr.map { |x| x * 2 }
来源：http://yrf.xingfuxueyuan.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://muj.fehbvm.com

[D15] 去重
来源：http://bqz.zhixingplan.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://rsk.iojbl.cn

PHP:  array_unique($arr);
来源：http://yux.yj20258888.top

JS:   [...new Set(arr)]
来源：http://bas.316326.xyz

TS:   [...new Set(arr)]
来源：http://ojx.birdmap.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://loo.hesvh.cn

Go:   // 用 map[T]struct{} 手写
来源：http://cwz.zhongyouzk.top

Ruby: arr.uniq
来源：http://bbb.andypj.xyz

C#:   list.Distinct().ToList()
来源：http://ufe.yuxming.cn

[D16] 求和与平均值
来源：http://cct.fanxiaobao.xyz

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://vmg.uphjek.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ktu.vqdsnc.cn


<!-- 参考信息 -->