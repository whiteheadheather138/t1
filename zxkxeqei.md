代发 wailian999

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xgl.vehdjk.com

Java: x instanceof Number
来源：http://hxe.hfpthk.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://psq.yj20258.top

Ruby: x.is_a?(Numeric)
来源：http://gjd.gotoacloud.top

C#:   x is int or double or decimal
来源：http://ooq.wangshuangyany.cn

[B14] 判断值是否在集合内
来源：http://exz.cqqwz.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://yio.zhixingplan.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://bcy.smart0.xyz

JS:   [1, 2, 3].includes(x)
来源：http://gio.xziqi.cn

TS:   [1, 2, 3].includes(x)
来源：http://gny.chenjidiqi.icu

Java: List.of(1, 2, 3).contains(x)
来源：http://wwh.zdbjq.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://beg.hesvh.cn

Ruby: [1, 2, 3].include?(x)
来源：http://dds.9152youxi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://nlx.gzhubu.top

[B15] 布尔运算与取反
来源：http://sba.yj20258888.top

Py:   a and b or not c
来源：http://fxb.ydzc1.top

PHP:  $a && $b || !$c
来源：http://apu.xinyue.icu

JS:   a && b || !c
来源：http://efc.nanxuanxn.top

TS:   a && b || !c
来源：http://tip.daria6918.cn

Java: a && b || !c
来源：http://btu.tanke756.top

Go:   a && b || !c
来源：http://kcu.wangshuangyany.cn

Ruby: a && b || !c
来源：http://ubf.shanyushiyangkeji.top

C#:   a && b || !c
来源：http://auk.shuidangran.top

[B16] 卫语句：不满足条件提前返回
来源：http://mar.chenzaomai.com

Py:   if not data: return
来源：http://zhe.jinqigfzy.top

PHP:  if (!$data) { return; }
来源：http://jlq.jianghu66.top

JS:   if (!data) return;
来源：http://ktw.guannengcc.top

TS:   if (!data) return;
来源：http://yho.shzxlz.cn

Java: if (data == null) return;
来源：http://gql.yonumen.top

Go:   if data == nil { return }
来源：http://dud.xinyue.icu

Ruby: return if data.nil?
来源：http://bbu.gotoacloud.top

C#:   if (data == null) return;
来源：http://cui.xinyue.icu

================================================================================
来源：http://uht.sxryk.cn

C. 函数与作用域
来源：http://fpq.cashguo.top

================================================================================
来源：http://xtg.yj20258.top

[C01] 定义函数
来源：http://rmf.xziqi.cn

Py:   def add(a, b): return a + b
来源：http://nph.cashguo.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kap.aibaodan.cn

JS:   function add(a, b) { return a + b; }
来源：http://mwj.ydzc1.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zql.gotoacloud.top

Java: static int add(int a, int b) { return a + b; }
来源：http://ukm.yonumen.top

Go:   func add(a, b int) int { return a + b }
来源：http://uev.9152youxi.cn

Ruby: def add(a, b); a + b; end
来源：http://lfn.zhaomingkeji.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://rlb.hysaishi.cn

[C02] 默认参数
来源：http://sas.gzhubu.top

Py:   def greet(name="World"): return name
来源：http://lpr.fanxiaobao.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://oto.ydjk.org.cn

JS:   function greet(name = "World") { return name; }
来源：http://nwe.zhongyouzk.top

TS:   function greet(name: string = "World") { return name; }
来源：http://lud.ybcxt.top

Java: // 无默认参数：方法重载或 Optional
来源：http://spw.vehdjk.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hav.birdmap.top

Ruby: def greet(name = "World") = name
来源：http://god.hfpthk.cn

C#:   string Greet(string name = "World") => name;
来源：http://bkk.tianlin.xyz

[C03] 可变参数
来源：http://tbr.andypj.xyz

Py:   def total(*args): return sum(args)
来源：http://pfs.guowangkeji.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://emf.dianchejie.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://dgf.guowangkeji.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://vov.ywan-chungtsiang.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://agd.meibo888.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://yqi.xziqi.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ehc.quarkkingdee.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://xsc.cashguo.top

[C04] 命名参数 / 关键字参数
来源：http://pkr.vqdsnc.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://zhq.aibaodan.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://fao.hcnkem.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://kzu.yueranfly.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://zyg.fanxiaobao.xyz

Java: // 无：用 Builder 模式或 record
来源：http://diy.fktsv.cn

Go:   // 无：用配置结构体参数
来源：http://ueo.shzxlz.cn

Ruby: f(a: 1, b: 2)
来源：http://pen.jinyuanbaomall.cn

C#:   f(a: 1, b: 2)
来源：http://smq.svipenyu.cn

[C05] 返回多个值
来源：http://zha.hywenlv.cn

Py:   return a, b
来源：http://gum.xylfe.cn

PHP:  return [$a, $b];
来源：http://lga.andypj.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://tvu.birdmap.top

TS:   return { a, b };
来源：http://jkr.birdmap.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://jxs.shanyushiyangtech.top

Go:   return a, b
来源：http://bua.hammf.cn

Ruby: return a, b
来源：http://xke.hnxiangtu.top

C#:   return (a, b);              // ValueTuple
来源：http://jug.hywenlv.cn

[C06] 匿名函数 / lambda
来源：http://had.cdnleiting.top

Py:   square = lambda x: x * x
来源：http://xyz.0kj1m.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://kva.hywenlv.cn

JS:   const square = x => x * x;
来源：http://ioo.gzhubu.top

TS:   const square = (x: number): number => x * x;
来源：http://ohx.dianchejie.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://deg.yanxiufei.cn

Go:   sq := func(x int) int { return x * x }
来源：http://lqj.zhiwuduotai.top

Ruby: square = ->(x) { x * x }
来源：http://iws.nanxuanxn.top

C#:   Func<int, int> square = x => x * x;
来源：http://ztz.jiagoushi.top

[C07] 把函数作为参数传入
来源：http://gqz.jianghu66.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://qbq.zdqjudy.top

PHP:  array_map("strtoupper", $arr);
来源：http://uga.jianghu66.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://cgr.zhaomingkeji.xyz

TS:   arr.map(String)
来源：http://kia.tian-w.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://jzl.cheryme.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://owq.smart0.xyz

Ruby: arr.map(&:upcase)
来源：http://aas.aibaodan.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://sex.xingfuxueyuan.xyz

[C08] 闭包
来源：http://jei.snrcjt.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://bvv.yj20258.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://aay.kuanghao11.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://nor.zhengqikj.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ivb.nwbrower.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://iiu.fzhhl.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://khp.epnwcf.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://fkr.guowangkeji.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mzv.chenlongwang.top

[C09] 递归
来源：http://bzr.cheryme.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://urs.jiagoushi.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://iux.gogol.net.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sna.tian-w.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://apc.yangfankeji.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://jia.bjfxy.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ctm.52xcode.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mix.9152youxi.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://dbx.yj20258.top

[C10] 变量作用域
来源：http://sxw.gogol.net.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://edb.hywenlv.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://olh.havefunace.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://zst.sjlbkw.cn

TS:   同 JS
来源：http://tvt.zdqjudy.top

Java: 方法内为块级作用域
来源：http://rxc.smart0.xyz

Go:   花括号块级作用域
来源：http://jlq.ctjpmb.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://plj.ppjwa.cn

C#:   块级作用域
来源：http://yei.ivvv.top

[C11] 模块导入与导出
来源：http://udk.52xcode.cn

Py:   from module import func
来源：http://gvx.hongshengwenyu.top

PHP:  require "file.php";  或 use App\Service;
来源：http://hry.pycfn.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://vsq.dianchejie.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://aru.jinyuanbaomall.cn

Java: import java.util.List;
来源：http://zox.gogol.net.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mom.0kj1m.cn

Ruby: require "json"; require_relative "./util"
来源：http://xle.jlsjyb.cn

C#:   using System.Text;
来源：http://nda.hammf.cn

[C12] 立即执行函数 IIFE
来源：http://scb.ehwqpu.com

Py:   (lambda: print("run"))()
来源：http://zhx.0kj1m.cn

PHP:  (function () { echo "run"; })();
来源：http://ido.guowangkeji.top

JS:   (() => { console.log("run"); })();
来源：http://xvb.tarul.cn

TS:   (() => { console.log("run"); })();
来源：http://xza.hcnkem.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://qnc.xingfuxueyuan.xyz

Go:   func() { fmt.Println("run") }()
来源：http://plw.haohaochexian.top

Ruby: -> { puts "run" }.call
来源：http://lbg.cucudq.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://avq.zdqjudy.top

[C13] 类型声明 / 类型注解
来源：http://vwo.yuanzhike.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://rdt.c1oappe.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hbl.ppjwa.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://bnr.yueranfly.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qqm.zhiwuduotai.top

Java: int add(int a, int b) { return a + b; }
来源：http://dcx.zhixingplan.top

Go:   func add(a, b int) int
来源：http://fwl.c1oappe.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://nmo.sysykeji.top

C#:   int Add(int a, int b) => a + b;
来源：http://feb.cucudq.cn

[C14] 泛型函数
来源：http://inw.sjlbkw.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://xhw.bbcook.cn

PHP:  // 无泛型
来源：http://qah.dianchejie.cn

JS:   // 无泛型
来源：http://wdq.daxiang520.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://xuo.redwolf501.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://yix.kuanghao11.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://chw.aibaodan.cn

Ruby: # 无泛型
来源：http://qwt.chenlongwang.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://cmw.yuanzhike.top

[C15] 解构 / 展开参数
来源：http://ozf.zhijiandao.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://tmy.zhoulong.xyz

PHP:  [$a, $b] = $pair;
来源：http://zvu.xinyue.icu

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://gvo.shzxlz.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://pge.hcnkem.com

Java: // 无解构
来源：http://zfu.aibaodan.cn

Go:   // 无解构
来源：http://fal.shuidangran.top

Ruby: a, b = pair
来源：http://dwg.xuetiantiany.cn

C#:   var (a, b) = pair;
来源：http://stz.hesvh.cn

[C16] 函数 / 方法重载
来源：http://att.hnxiangtu.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hzp.uphjek.com

PHP:  // 无重载
来源：http://tbv.hongshengwenyu.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://ivs.tian-w.cn

TS:   // 用联合类型或重载签名声明
来源：http://uzi.jinghuilouyu.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://pow.hnqzz.top

Go:   // 无重载：用不同函数名
来源：http://mfj.fktsv.cn

Ruby: # 无重载：靠动态参数
来源：http://gfp.cqqwz.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://qgi.ppjwa.cn

================================================================================
来源：http://ajo.bbcook.cn

D. 数组 / 列表 / 集合
来源：http://eed.hywenlv.cn

================================================================================
来源：http://xxy.ctjpmb.com

[D01] 创建数组 / 列表
来源：http://slu.shanyushiyangkeji.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://uya.cqqwz.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wmc.xziqi.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://nkg.jiagoushi.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://olo.zhaomingkeji.xyz

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://npg.yj20258.top

Go:   arr := []int{1, 2, 3}
来源：http://dji.ivvv.top

Ruby: arr = [1, 2, 3]
来源：http://ama.nanxinkj.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://pej.cucudq.cn

[D02] 追加元素到末尾
来源：http://axz.sjlbkw.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://qng.zhijiandao.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mrk.yj20258.top

JS:   arr.push(4);
来源：http://kkn.cqqwz.cn

TS:   arr.push(4);
来源：http://aco.xuetiantiany.cn

Java: list.add(4);
来源：http://wlf.chenzaomai.com

Go:   arr = append(arr, 4)
来源：http://biu.svipenyu.cn

Ruby: arr << 4; arr.push(5)
来源：http://kos.yj20258.top

C#:   list.Add(4);
来源：http://zly.jiagoushi.top

[D03] 在指定位置插入元素
来源：http://ftm.cucudq.cn

Py:   arr.insert(0, 0)
来源：http://vxf.9152youxi.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://fxl.xylfe.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://kht.bbcook.cn

TS:   arr.splice(0, 0, 0);
来源：http://osl.ybcxt.top

Java: list.add(0, 0);
来源：http://olk.tanke756.top

Go:   arr = append([]int{0}, arr...)
来源：http://dfh.zycfv.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://vei.zdqjudy.top

C#:   list.Insert(0, 0);
来源：http://vhx.hnxiangtu.top

[D04] 删除元素
来源：http://ovi.jianghu66.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://gid.gzhubu.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://tii.0kj1m.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://fvk.pycfn.com

TS:   arr.splice(0, 1);
来源：http://kai.hammf.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://vue.tanke756.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://zvy.zhaomingkeji.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://dgy.nanxuanxn.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://yxj.svipenyu.cn

[D05] 访问与修改元素
来源：http://las.guowangkeji.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://sev.zhengqikj.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://fwu.zhiwuduotai.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://grl.fengsongda.top

TS:   arr[0]; arr.at(-1);
来源：http://gih.yangfankeji.com

Java: list.get(0); list.set(0, 9);
来源：http://jgb.ywan-chungtsiang.top

Go:   arr[0]; arr[0] = 9
来源：http://kfa.gotoacloud.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hta.vqdsnc.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wtu.cucudq.cn

[D06] 数组长度
来源：http://irx.daria6918.cn

Py:   len(arr)
来源：http://mjg.fktsv.cn

PHP:  count($arr);
来源：http://otp.tianlin.xyz

JS:   arr.length
来源：http://kll.guannengcc.top

TS:   arr.length
来源：http://rpj.fengsongda.top

Java: list.size();
来源：http://wal.wangshuangyany.cn

Go:   len(arr)
来源：http://fuy.ctjpmb.com

Ruby: arr.length; arr.size
来源：http://tyb.haohaochexian.top

C#:   list.Count;
来源：http://srg.gaohongyu789.top

[D07] 切片 / 取子数组
来源：http://apo.nanxuanxn.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ugl.dianchejie.cn

PHP:  array_slice($arr, 1, 3);
来源：http://wiu.zdqjudy.top

JS:   arr.slice(1, 4);
来源：http://rif.sweek.top

TS:   arr.slice(1, 4);
来源：http://kjq.jyoumei.cn

Java: list.subList(1, 4);
来源：http://bea.tanke756.top

Go:   arr[1:4]
来源：http://yyf.birdmap.top

Ruby: arr[1, 3]
来源：http://khp.dashuyun.cn

C#:   list.GetRange(1, 3);
来源：http://isz.zhijiandao.cn

[D08] 合并两个数组
来源：http://gac.quarkkingdee.top

Py:   a + b;  a.extend(b)
来源：http://svk.yuxming.cn

PHP:  array_merge($a, $b);
来源：http://hko.nanxuanxn.top

JS:   [...a, ...b];  a.concat(b);
来源：http://ota.ehwqpu.com

TS:   [...a, ...b];
来源：http://hch.tanke756.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://fpr.havefunace.top

Go:   append(a, b...)
来源：http://gvy.jinyuanbaomall.cn

Ruby: a + b;  a.concat(b)
来源：http://oey.yueranfly.top

C#:   a.Concat(b).ToList()
来源：http://rdn.chenlongwang.top

[D09] 排序（升序）
来源：http://mxs.zdbjq.cn

Py:   sorted(arr);  arr.sort()
来源：http://rng.bjfxy.top

PHP:  sort($arr);
来源：http://npt.feifeiyinyue.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://owf.nanxuanxn.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://nam.aizwys.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://kqx.jinqigufen.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://bkx.gogol.net.cn

Ruby: arr.sort
来源：http://wam.sxryk.cn

C#:   list.Sort();
来源：http://wgf.jqgufenzy.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://lga.316326.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://sjh.zdqjudy.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wcv.vehdjk.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://qpg.daxiang520.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://coy.jinqigufen.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://lvj.dashuyun.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://sdm.yj202588.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://jgx.yuanzhike.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://upw.hnxiangtu.top

[D11] 反转数组
来源：http://nsk.birdmap.top

Py:   arr[::-1];  arr.reverse()
来源：http://wig.gotoacloud.top

PHP:  array_reverse($arr);
来源：http://tkx.aizwys.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://bzq.svipenyu.cn

TS:   [...arr].reverse();
来源：http://dib.hywenlv.cn

Java: Collections.reverse(list);
来源：http://csj.shangyingyoupin.top

Go:   slices.Reverse(arr)
来源：http://eib.sysykeji.top

Ruby: arr.reverse
来源：http://zjb.birdmap.top

C#:   list.Reverse();
来源：http://bdt.gogol.net.cn

[D12] 查找元素下标
来源：http://tpe.svipenyu.cn

Py:   arr.index(x);  x in arr
来源：http://siw.hnqzz.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://jxl.cqqwz.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://akj.shzxlz.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://juq.316326.xyz

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://zyx.xuanzx.com

Go:   slices.Index(arr, x)
来源：http://hxu.uphjek.com

Ruby: arr.index(x)
来源：http://kwg.fktsv.cn

C#:   list.IndexOf(x);
来源：http://fbe.yfazqb.com

[D13] 过滤（保留满足条件的）
来源：http://wtp.hongshengwenyu.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://lbj.ehwqpu.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://yao.xziqi.cn

JS:   arr.filter(x => x > 3)
来源：http://tsi.52xcode.cn

TS:   arr.filter(x => x > 3)
来源：http://bow.shuidangran.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://cip.jianghu66.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://pow.ybcxt.top

Ruby: arr.select { |x| x > 3 }
来源：http://pra.shangyingyoupin.top

C#:   list.Where(x => x > 3).ToList()
来源：http://bov.fengsongda.top

[D14] 映射转换（每个元素变形）
来源：http://sda.aibaodan.cn


<!-- 参考信息 -->