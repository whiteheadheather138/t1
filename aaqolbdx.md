代发 wailian999

TS:   function greet(name: string = "World") { return name; }
来源：http://jei.nanxinkj.top

Java: // 无默认参数：方法重载或 Optional
来源：http://pnm.ctjpmb.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://chw.havefunace.top

Ruby: def greet(name = "World") = name
来源：http://rmn.daxiang520.top

C#:   string Greet(string name = "World") => name;
来源：http://tpl.fengsongda.top

[C03] 可变参数
来源：http://ztd.andypj.xyz

Py:   def total(*args): return sum(args)
来源：http://zji.hywenlv.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ikq.xuanzx.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://rzq.svipenyu.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://gwv.snrcjt.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ltg.bjfxy.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://abn.nanxinkj.top

Ruby: def total(*nums); nums.sum; end
来源：http://eup.nanxinkj.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://juc.cqqwz.cn

[C04] 命名参数 / 关键字参数
来源：http://akb.ppjwa.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ygb.yonumen.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xmo.zdqjudy.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://uvt.birdmap.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://nyz.fengsongda.top

Java: // 无：用 Builder 模式或 record
来源：http://rlo.wangdashe.top

Go:   // 无：用配置结构体参数
来源：http://lec.xinyue.icu

Ruby: f(a: 1, b: 2)
来源：http://bwg.gogol.net.cn

C#:   f(a: 1, b: 2)
来源：http://deg.hnqzz.top

[C05] 返回多个值
来源：http://mrn.xuetiantiany.cn

Py:   return a, b
来源：http://ruv.hammf.cn

PHP:  return [$a, $b];
来源：http://fpo.sweek.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://bso.aizwys.cn

TS:   return { a, b };
来源：http://uci.0kj1m.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://pdk.tianlin.xyz

Go:   return a, b
来源：http://prn.jlsjyb.cn

Ruby: return a, b
来源：http://nug.hnxiangtu.top

C#:   return (a, b);              // ValueTuple
来源：http://xcb.cucudq.cn

[C06] 匿名函数 / lambda
来源：http://xij.fengsongda.top

Py:   square = lambda x: x * x
来源：http://cyc.fanxiaobao.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://lnd.316326.xyz

JS:   const square = x => x * x;
来源：http://gcb.zhengqikj.top

TS:   const square = (x: number): number => x * x;
来源：http://szz.shanyushiyangtech.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://xbz.jianghu66.top

Go:   sq := func(x int) int { return x * x }
来源：http://fni.smart0.xyz

Ruby: square = ->(x) { x * x }
来源：http://mbh.fzhhl.top

C#:   Func<int, int> square = x => x * x;
来源：http://nuz.zdqjudy.top

[C07] 把函数作为参数传入
来源：http://sdl.jinqigufen.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://igb.chenlongwang.top

PHP:  array_map("strtoupper", $arr);
来源：http://lqx.zycfv.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://bho.kuanghao11.cn

TS:   arr.map(String)
来源：http://qor.guannengcc.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://nqg.yonumen.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://yyk.daria6918.cn

Ruby: arr.map(&:upcase)
来源：http://qzm.yonumen.top

C#:   arr.Select(s => s.ToUpper())
来源：http://jmy.vqdsnc.cn

[C08] 闭包
来源：http://ehy.jyoumei.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://upc.dianchejie.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://vap.fengsongda.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://slq.c1oappe.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mor.sufxvd.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://rlg.aizwys.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://qud.shanyushiyangkeji.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://sqn.ybcxt.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://sqm.cheryme.top

[C09] 递归
来源：http://lqx.shanyushiyangtech.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://xzv.shanyushiyangkeji.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://svk.shanyushiyangtech.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gos.yfazqb.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://eix.9152youxi.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://zde.yj202588.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://qyc.bjfxy.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://dka.cheryme.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://sjc.fzhhl.top

[C10] 变量作用域
来源：http://nry.kuanghao11.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ohj.xuanzx.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://oga.9152youxi.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mfw.dianchejie.cn

TS:   同 JS
来源：http://tko.shzxlz.cn

Java: 方法内为块级作用域
来源：http://sjt.gogol.net.cn

Go:   花括号块级作用域
来源：http://ftr.chenlongwang.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://oar.jlsjyb.cn

C#:   块级作用域
来源：http://lqf.hongshengwenyu.top

[C11] 模块导入与导出
来源：http://tge.316326.xyz

Py:   from module import func
来源：http://fxy.wangdashe.top

PHP:  require "file.php";  或 use App\Service;
来源：http://rhq.dianchejie.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://rxv.cdnleiting.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wcd.sysykeji.top

Java: import java.util.List;
来源：http://ael.zhixingplan.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://goq.fanxiaobao.xyz

Ruby: require "json"; require_relative "./util"
来源：http://tfo.dashuyun.cn

C#:   using System.Text;
来源：http://xnc.haohaochexian.top

[C12] 立即执行函数 IIFE
来源：http://uan.gotoacloud.top

Py:   (lambda: print("run"))()
来源：http://koc.birdmap.top

PHP:  (function () { echo "run"; })();
来源：http://yfx.52xcode.cn

JS:   (() => { console.log("run"); })();
来源：http://fsj.ybcxt.top

TS:   (() => { console.log("run"); })();
来源：http://hwb.guowangkeji.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://taf.xuanzx.com

Go:   func() { fmt.Println("run") }()
来源：http://qvx.gogol.net.cn

Ruby: -> { puts "run" }.call
来源：http://dwd.cucudq.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://esg.bjfxy.top

[C13] 类型声明 / 类型注解
来源：http://cpr.fzhhl.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://udh.guowangkeji.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gxn.shuidangran.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://arl.sxryk.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://btf.jianghu66.top

Java: int add(int a, int b) { return a + b; }
来源：http://jsc.dianchejie.cn

Go:   func add(a, b int) int
来源：http://ncq.wangshuangyany.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://yua.dashuyun.cn

C#:   int Add(int a, int b) => a + b;
来源：http://wso.fzhhl.top

[C14] 泛型函数
来源：http://qlj.xziqi.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://axp.aizwys.cn

PHP:  // 无泛型
来源：http://ias.jyoumei.cn

JS:   // 无泛型
来源：http://hoa.ppjwa.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://spa.yj20258888.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://yje.cucudq.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://cqa.ywan-chungtsiang.top

Ruby: # 无泛型
来源：http://mnp.vqdsnc.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wmt.chenjidiqi.icu

[C15] 解构 / 展开参数
来源：http://xix.ywan-chungtsiang.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://yuo.hnxiangtu.top

PHP:  [$a, $b] = $pair;
来源：http://frp.yvedp.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ole.yongpay.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://twk.vehdjk.com

Java: // 无解构
来源：http://ldj.haohaochexian.top

Go:   // 无解构
来源：http://bvt.ydzc1.top

Ruby: a, b = pair
来源：http://cxh.fengsongda.top

C#:   var (a, b) = pair;
来源：http://rya.xziqi.cn

[C16] 函数 / 方法重载
来源：http://tkd.yj20258888.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://zze.yj20258.top

PHP:  // 无重载
来源：http://him.jyoumei.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://gmf.xylfe.cn

TS:   // 用联合类型或重载签名声明
来源：http://vri.cqqwz.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://xxu.tanke756.top

Go:   // 无重载：用不同函数名
来源：http://wzi.chenjidiqi.icu

Ruby: # 无重载：靠动态参数
来源：http://hzi.jinyuanbaomall.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ltt.birdmap.top

================================================================================
来源：http://ofj.zhoulong.xyz

D. 数组 / 列表 / 集合
来源：http://xlc.jqgufenzy.top

================================================================================
来源：http://zdq.bbcook.cn

[D01] 创建数组 / 列表
来源：http://tuz.meibo888.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://wik.quarkkingdee.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ufh.sysykeji.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://tzq.mhx1999.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://vwm.zhaomingkeji.xyz

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mwh.cqqwz.cn

Go:   arr := []int{1, 2, 3}
来源：http://njd.xziqi.cn

Ruby: arr = [1, 2, 3]
来源：http://uva.yanxiufei.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://inj.jinqigfzy.top

[D02] 追加元素到末尾
来源：http://jsj.shanyushiyangkeji.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wqs.yvedp.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://qhj.gaohongyu789.top

JS:   arr.push(4);
来源：http://psq.0kj1m.cn

TS:   arr.push(4);
来源：http://jjw.zycfv.cn

Java: list.add(4);
来源：http://aux.sjlbkw.cn

Go:   arr = append(arr, 4)
来源：http://lws.iojbl.cn

Ruby: arr << 4; arr.push(5)
来源：http://ujf.hnxiangtu.top

C#:   list.Add(4);
来源：http://ewv.yj20258888.top

[D03] 在指定位置插入元素
来源：http://bfg.316326.xyz

Py:   arr.insert(0, 0)
来源：http://uvs.xziqi.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mob.ydjk.org.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://gfc.shangyingyoupin.top

TS:   arr.splice(0, 0, 0);
来源：http://hgo.bjfxy.top

Java: list.add(0, 0);
来源：http://lld.jianghu66.top

Go:   arr = append([]int{0}, arr...)
来源：http://uaq.sxryk.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://pzz.zhijiandao.cn

C#:   list.Insert(0, 0);
来源：http://yhv.pycfn.com

[D04] 删除元素
来源：http://aey.meibo888.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://rzv.smart0.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ncz.52xcode.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hjb.aizwys.cn

TS:   arr.splice(0, 1);
来源：http://kmq.sjlbkw.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://vgg.dianchejie.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mdu.0kj1m.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://tsw.nanxinkj.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hlr.sysykeji.top

[D05] 访问与修改元素
来源：http://eks.dashuyun.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ahy.yj20258888.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mkq.yongpay.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://kdm.shuidangran.top

TS:   arr[0]; arr.at(-1);
来源：http://gql.cucudq.cn

Java: list.get(0); list.set(0, 9);
来源：http://zmz.guannengcc.top

Go:   arr[0]; arr[0] = 9
来源：http://mad.jinghuilouyu.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://xqw.52xcode.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ccc.xuanzx.com

[D06] 数组长度
来源：http://mzf.sysykeji.top

Py:   len(arr)
来源：http://grw.tianlin.xyz

PHP:  count($arr);
来源：http://dhe.jinghuilouyu.cn

JS:   arr.length
来源：http://yeq.shanyushiyangkeji.top

TS:   arr.length
来源：http://iwc.meibo888.top

Java: list.size();
来源：http://qqr.yfazqb.com

Go:   len(arr)
来源：http://txf.guowangkeji.top

Ruby: arr.length; arr.size
来源：http://qvi.yangfankeji.com

C#:   list.Count;
来源：http://pgm.bbcook.cn

[D07] 切片 / 取子数组
来源：http://fzr.zhijiandao.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://yfc.ywan-chungtsiang.top

PHP:  array_slice($arr, 1, 3);
来源：http://qox.xuetiantiany.cn

JS:   arr.slice(1, 4);
来源：http://yfp.jqgfzy.top

TS:   arr.slice(1, 4);
来源：http://bsb.feifeiyinyue.top

Java: list.subList(1, 4);
来源：http://qnr.iojbl.cn

Go:   arr[1:4]
来源：http://hnw.gaohongyu789.top

Ruby: arr[1, 3]
来源：http://ort.tianlin.xyz

C#:   list.GetRange(1, 3);
来源：http://xgi.dianchejie.cn

[D08] 合并两个数组
来源：http://ahe.hesvh.cn

Py:   a + b;  a.extend(b)
来源：http://wlu.fehbvm.com

PHP:  array_merge($a, $b);
来源：http://vyf.shangyingyoupin.top

JS:   [...a, ...b];  a.concat(b);
来源：http://nzx.tanke756.top

TS:   [...a, ...b];
来源：http://scm.pengpengdd.cyou

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://usd.zhaomingkeji.xyz

Go:   append(a, b...)
来源：http://wrw.xuetiantiany.cn

Ruby: a + b;  a.concat(b)
来源：http://qlv.gogol.net.cn

C#:   a.Concat(b).ToList()
来源：http://gmf.mhx1999.top

[D09] 排序（升序）
来源：http://eqx.fanxiaobao.xyz

Py:   sorted(arr);  arr.sort()
来源：http://fyg.vehdjk.com

PHP:  sort($arr);
来源：http://opr.hnxiangtu.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ycv.sjlbkw.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://hzh.sxryk.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://geh.cheryme.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://lpu.yongpay.top

Ruby: arr.sort
来源：http://nzi.fengsongda.top

C#:   list.Sort();
来源：http://acr.bjfxy.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://bib.ivvv.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mnp.hcnkem.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wvp.aizwys.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ooc.yj202588.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://faz.ehwqpu.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://can.tanke756.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mdq.gotoacloud.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://fqi.dianchejie.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://fbo.gogol.net.cn

[D11] 反转数组
来源：http://nqn.ivvv.top

Py:   arr[::-1];  arr.reverse()
来源：http://oqr.yj20258.top

PHP:  array_reverse($arr);
来源：http://vqs.ivvv.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://owd.xuetiantiany.cn

TS:   [...arr].reverse();
来源：http://zbu.snrcjt.cn

Java: Collections.reverse(list);
来源：http://fkx.yueranfly.top

Go:   slices.Reverse(arr)
来源：http://rvz.yanxiufei.cn

Ruby: arr.reverse
来源：http://iwe.xuanzx.com

C#:   list.Reverse();
来源：http://lax.shuidangran.top

[D12] 查找元素下标
来源：http://xhz.yj20258888.top

Py:   arr.index(x);  x in arr
来源：http://kfq.yonumen.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://bfr.tarul.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xmb.xuetiantiany.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xws.yuanzhike.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://loy.yfazqb.com

Go:   slices.Index(arr, x)
来源：http://ujs.birdmap.top

Ruby: arr.index(x)
来源：http://diy.redwolf501.top

C#:   list.IndexOf(x);
来源：http://doj.uphjek.com

[D13] 过滤（保留满足条件的）
来源：http://zoi.hywenlv.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://bkt.ydjk.org.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://jzd.tanke756.top

JS:   arr.filter(x => x > 3)
来源：http://sng.haohaochexian.top

TS:   arr.filter(x => x > 3)
来源：http://aga.hammf.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://rkx.yj202588.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://fey.hesvh.cn

Ruby: arr.select { |x| x > 3 }
来源：http://xnc.zhoulong.xyz

C#:   list.Where(x => x > 3).ToList()
来源：http://dcd.hongshengwenyu.top

[D14] 映射转换（每个元素变形）
来源：http://fto.sysykeji.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://irm.tian-w.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mah.aizwys.cn

JS:   arr.map(x => x * 2)
来源：http://ggz.zhongyouzk.top

TS:   arr.map(x => x * 2)
来源：http://nkp.yanxiufei.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://yrk.aizwys.cn

Go:   // 手写循环
来源：http://ntj.bbcook.cn

Ruby: arr.map { |x| x * 2 }
来源：http://dsv.ydzc1.top

C#:   list.Select(x => x * 2).ToList()
来源：http://rsw.wangdashe.top

[D15] 去重
来源：http://gsm.havefunace.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://qof.ybcxt.top

PHP:  array_unique($arr);
来源：http://jca.ivvv.top

JS:   [...new Set(arr)]
来源：http://jco.bjfxy.top

TS:   [...new Set(arr)]
来源：http://iaw.aizwys.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://yby.gotoacloud.top

Go:   // 用 map[T]struct{} 手写
来源：http://yua.vehdjk.com

Ruby: arr.uniq
来源：http://pxx.fktsv.cn

C#:   list.Distinct().ToList()
来源：http://jaz.guannengcc.top

[D16] 求和与平均值
来源：http://lua.jqgfzy.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mdy.andypj.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://bhq.zhixingplan.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://cxv.zhixingplan.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ngi.cashguo.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://pdg.daxiang520.top

Go:   // 手写循环累加
来源：http://url.xingfuxueyuan.xyz

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://saz.ydzc1.top

C#:   list.Sum();  list.Average()
来源：http://aez.xinyue.icu

[D17] 最大值与最小值
来源：http://ntv.wangdashe.top

Py:   max(arr);  min(arr)
来源：http://dkv.ybcxt.top

PHP:  max($arr);  min($arr);
来源：http://kin.nanxinkj.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://jvh.zdbjq.cn

TS:   Math.max(...arr);
来源：http://zwt.meibo888.top

Java: Collections.max(list);  Collections.min(list);
来源：http://efn.quarkkingdee.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://eiw.fktsv.cn

Ruby: arr.max;  arr.min
来源：http://rbp.svipenyu.cn

C#:   list.Max();  list.Min()
来源：http://lat.nwbrower.top

[D18] 扁平化嵌套数组
来源：http://wea.haohaochexian.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ocm.iojbl.cn

PHP:  array_merge(...$nested);
来源：http://nnd.fehbvm.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://dvp.zhixingplan.top

TS:   nested.flat();
来源：http://cjh.zhiwuduotai.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://xkm.fengsongda.top

Go:   // 手写双层循环
来源：http://unh.xingfuxueyuan.xyz

Ruby: nested.flatten
来源：http://tai.hongshengwenyu.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://fov.ywan-chungtsiang.top

[D19] 按字段分组
来源：http://fio.yueranfly.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://daw.cashguo.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://txh.gotoacloud.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://otn.tian-w.cn


<!-- 参考信息 -->