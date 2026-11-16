代发 wailian999

TS:   function greet(name: string = "World") { return name; }
来源：http://wzw.zhixingplan.top

Java: // 无默认参数：方法重载或 Optional
来源：http://yvl.cheryme.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://gym.smart0.xyz

Ruby: def greet(name = "World") = name
来源：http://wfw.sweek.top

C#:   string Greet(string name = "World") => name;
来源：http://epv.jinqigfzy.top

[C03] 可变参数
来源：http://tcg.jinghuilouyu.cn

Py:   def total(*args): return sum(args)
来源：http://bvl.havefunace.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://oxd.shangyingyoupin.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://eyh.xziqi.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ect.feifeiyinyue.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://khn.xingfuxueyuan.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://rcd.xuetiantiany.cn

Ruby: def total(*nums); nums.sum; end
来源：http://fju.zhixingplan.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://vxv.xylfe.cn

[C04] 命名参数 / 关键字参数
来源：http://mbk.aizwys.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ciu.9152youxi.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wxh.yj20258888.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://pbf.316326.xyz

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://nzz.shangyingyoupin.top

Java: // 无：用 Builder 模式或 record
来源：http://ppo.cashguo.top

Go:   // 无：用配置结构体参数
来源：http://hle.shanyushiyangtech.top

Ruby: f(a: 1, b: 2)
来源：http://rht.bbcook.cn

C#:   f(a: 1, b: 2)
来源：http://nxw.zhaomingkeji.xyz

[C05] 返回多个值
来源：http://gbz.chenlongwang.top

Py:   return a, b
来源：http://ltr.shuidangran.top

PHP:  return [$a, $b];
来源：http://fqq.yfazqb.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://qbu.zhongyouzk.top

TS:   return { a, b };
来源：http://ijd.xziqi.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mnp.gaohongyu789.top

Go:   return a, b
来源：http://odp.yuanzhike.top

Ruby: return a, b
来源：http://ybe.sjlbkw.cn

C#:   return (a, b);              // ValueTuple
来源：http://bfk.pycfn.com

[C06] 匿名函数 / lambda
来源：http://gjm.uphjek.com

Py:   square = lambda x: x * x
来源：http://kho.c1oappe.top

PHP:  $square = fn($x) => $x * $x;
来源：http://gpp.jqgfzy.top

JS:   const square = x => x * x;
来源：http://mrx.meibo888.top

TS:   const square = (x: number): number => x * x;
来源：http://wdn.fanxiaobao.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ykv.feifeiyinyue.top

Go:   sq := func(x int) int { return x * x }
来源：http://axz.bbcook.cn

Ruby: square = ->(x) { x * x }
来源：http://nrz.dianchejie.cn

C#:   Func<int, int> square = x => x * x;
来源：http://hue.cqqwz.cn

[C07] 把函数作为参数传入
来源：http://lav.aibaodan.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://eqc.yuanzhike.top

PHP:  array_map("strtoupper", $arr);
来源：http://ovm.mhx1999.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://pbw.yueranfly.top

TS:   arr.map(String)
来源：http://qfx.cashguo.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://puk.cdnleiting.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://jih.jyoumei.cn

Ruby: arr.map(&:upcase)
来源：http://sfi.guannengcc.top

C#:   arr.Select(s => s.ToUpper())
来源：http://zhp.yongpay.top

[C08] 闭包
来源：http://yaq.xuanzx.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://plw.pycfn.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hox.daxiang520.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://pdl.bbcook.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://vbu.xylfe.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://usd.jqgufenzy.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://gqv.jinqigfzy.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hbt.cqqwz.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ols.jianghu66.top

[C09] 递归
来源：http://dkv.vehdjk.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://dkh.52xcode.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://iii.shanyushiyangtech.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ity.jinyuanbaomall.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qtz.yvedp.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://gcm.xinyue.icu

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://nto.kuanghao11.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://juo.hywenlv.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://vgc.dashuyun.cn

[C10] 变量作用域
来源：http://yph.sysykeji.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://zux.vehdjk.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://upv.guannengcc.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://lug.pengpengdd.cyou

TS:   同 JS
来源：http://qpx.xuetiantiany.cn

Java: 方法内为块级作用域
来源：http://nmy.tanke756.top

Go:   花括号块级作用域
来源：http://rzp.ivvv.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://uan.yvedp.cn

C#:   块级作用域
来源：http://vfw.sweek.top

[C11] 模块导入与导出
来源：http://see.fengsongda.top

Py:   from module import func
来源：http://afv.tianlin.xyz

PHP:  require "file.php";  或 use App\Service;
来源：http://ycs.daria6918.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://lzz.hongshengwenyu.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://vxj.gogol.net.cn

Java: import java.util.List;
来源：http://jnb.hammf.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://gbp.c1oappe.top

Ruby: require "json"; require_relative "./util"
来源：http://kea.aizwys.cn

C#:   using System.Text;
来源：http://mqe.hywenlv.cn

[C12] 立即执行函数 IIFE
来源：http://fyr.cqqwz.cn

Py:   (lambda: print("run"))()
来源：http://tds.xziqi.cn

PHP:  (function () { echo "run"; })();
来源：http://vra.guowangkeji.top

JS:   (() => { console.log("run"); })();
来源：http://fef.fanxiaobao.xyz

TS:   (() => { console.log("run"); })();
来源：http://vnl.jinghuilouyu.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://vex.zhixingplan.top

Go:   func() { fmt.Println("run") }()
来源：http://axk.xuetiantiany.cn

Ruby: -> { puts "run" }.call
来源：http://fpb.quarkkingdee.top

C#:   // 无 IIFE：用静态构造函数
来源：http://njn.hongshengwenyu.top

[C13] 类型声明 / 类型注解
来源：http://kcu.daxiang520.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://dow.cdnleiting.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mav.vehdjk.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://pwh.zycfv.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gbl.jiagoushi.top

Java: int add(int a, int b) { return a + b; }
来源：http://whm.cqqwz.cn

Go:   func add(a, b int) int
来源：http://wzd.zhoulong.xyz

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://loa.xingfuxueyuan.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://dzv.ybcxt.top

[C14] 泛型函数
来源：http://xel.bjfxy.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wqe.zhaomingkeji.xyz

PHP:  // 无泛型
来源：http://dfh.9152youxi.cn

JS:   // 无泛型
来源：http://vce.cashguo.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://fbz.wangshuangyany.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://uqx.xuetiantiany.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://rpk.tianlin.xyz

Ruby: # 无泛型
来源：http://lon.gzhubu.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://tee.birdmap.top

[C15] 解构 / 展开参数
来源：http://wmp.hywenlv.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://cmx.cqqwz.cn

PHP:  [$a, $b] = $pair;
来源：http://fyf.jlsjyb.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://dcq.shzxlz.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://nof.0kj1m.cn

Java: // 无解构
来源：http://fvv.jinqigfzy.top

Go:   // 无解构
来源：http://ciy.gaohongyu789.top

Ruby: a, b = pair
来源：http://bcp.jinyuanbaomall.cn

C#:   var (a, b) = pair;
来源：http://ywz.xinyue.icu

[C16] 函数 / 方法重载
来源：http://hyq.tian-w.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://xyl.hesvh.cn

PHP:  // 无重载
来源：http://sze.zhiwuduotai.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://xul.yfazqb.com

TS:   // 用联合类型或重载签名声明
来源：http://rti.fzhhl.top

Java: void f(int a) {}  void f(String a) {}
来源：http://smv.zdqjudy.top

Go:   // 无重载：用不同函数名
来源：http://fef.haohaochexian.top

Ruby: # 无重载：靠动态参数
来源：http://agl.sxryk.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://lqc.hesvh.cn

================================================================================
来源：http://tkr.hammf.cn

D. 数组 / 列表 / 集合
来源：http://xgi.shanyushiyangkeji.top

================================================================================
来源：http://hei.iojbl.cn

[D01] 创建数组 / 列表
来源：http://vmo.yuanzhike.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://vkb.xziqi.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://rzp.guannengcc.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hfm.nanxuanxn.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://saa.nwbrower.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://grv.hnxiangtu.top

Go:   arr := []int{1, 2, 3}
来源：http://xuc.tian-w.cn

Ruby: arr = [1, 2, 3]
来源：http://oaa.yongpay.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://tmv.shzxlz.cn

[D02] 追加元素到末尾
来源：http://nas.ybcxt.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hcm.kuanghao11.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://knt.hnxiangtu.top

JS:   arr.push(4);
来源：http://lsd.sjlbkw.cn

TS:   arr.push(4);
来源：http://djt.redwolf501.top

Java: list.add(4);
来源：http://ioz.9152youxi.cn

Go:   arr = append(arr, 4)
来源：http://rqu.ydjk.org.cn

Ruby: arr << 4; arr.push(5)
来源：http://ooc.fanxiaobao.xyz

C#:   list.Add(4);
来源：http://jik.c1oappe.top

[D03] 在指定位置插入元素
来源：http://bwc.xziqi.cn

Py:   arr.insert(0, 0)
来源：http://qdq.fanxiaobao.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://qbr.yueranfly.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://cxp.mhx1999.top

TS:   arr.splice(0, 0, 0);
来源：http://tuf.xuetiantiany.cn

Java: list.add(0, 0);
来源：http://tgw.tianlin.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://scw.ywan-chungtsiang.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://fko.9152youxi.cn

C#:   list.Insert(0, 0);
来源：http://uac.zhongyouzk.top

[D04] 删除元素
来源：http://mgi.zdqjudy.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://smf.yfazqb.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ukv.yongpay.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://jbj.vehdjk.com

TS:   arr.splice(0, 1);
来源：http://roc.hfpthk.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wkh.xuetiantiany.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hyk.yongpay.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://tbt.jinyuanbaomall.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://vck.yanxiufei.cn

[D05] 访问与修改元素
来源：http://orm.hammf.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://qnq.havefunace.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://kbe.ctjpmb.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://gem.jqgfzy.top

TS:   arr[0]; arr.at(-1);
来源：http://sri.jinqigfzy.top

Java: list.get(0); list.set(0, 9);
来源：http://vum.yuanzhike.top

Go:   arr[0]; arr[0] = 9
来源：http://zaz.ybcxt.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://jpo.wangshuangyany.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://kei.zycfv.cn

[D06] 数组长度
来源：http://olc.jqgfzy.top

Py:   len(arr)
来源：http://hxq.xuetiantiany.cn

PHP:  count($arr);
来源：http://zrq.zhengqikj.top

JS:   arr.length
来源：http://kfy.yvedp.cn

TS:   arr.length
来源：http://wtc.svipenyu.cn

Java: list.size();
来源：http://evq.fehbvm.com

Go:   len(arr)
来源：http://hvx.shuidangran.top

Ruby: arr.length; arr.size
来源：http://fqy.yonumen.top

C#:   list.Count;
来源：http://zvu.jlsjyb.cn

[D07] 切片 / 取子数组
来源：http://gdl.bbcook.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://gfg.daria6918.cn

PHP:  array_slice($arr, 1, 3);
来源：http://igw.ydjk.org.cn

JS:   arr.slice(1, 4);
来源：http://xvw.zhijiandao.cn

TS:   arr.slice(1, 4);
来源：http://sos.jinyuanbaomall.cn

Java: list.subList(1, 4);
来源：http://krb.gogol.net.cn

Go:   arr[1:4]
来源：http://afa.yangfankeji.com

Ruby: arr[1, 3]
来源：http://pei.cucudq.cn

C#:   list.GetRange(1, 3);
来源：http://gtw.cqqwz.cn

[D08] 合并两个数组
来源：http://wkd.yanxiufei.cn

Py:   a + b;  a.extend(b)
来源：http://rqf.zhengqikj.top

PHP:  array_merge($a, $b);
来源：http://yap.daxiang520.top

JS:   [...a, ...b];  a.concat(b);
来源：http://jys.shanyushiyangkeji.top

TS:   [...a, ...b];
来源：http://nes.pycfn.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hzt.jqgufenzy.top

Go:   append(a, b...)
来源：http://nxc.jinghuilouyu.cn

Ruby: a + b;  a.concat(b)
来源：http://ysw.andypj.xyz

C#:   a.Concat(b).ToList()
来源：http://rur.yuanzhike.top

[D09] 排序（升序）
来源：http://ddg.dashuyun.cn

Py:   sorted(arr);  arr.sort()
来源：http://uqj.hammf.cn

PHP:  sort($arr);
来源：http://hxe.birdmap.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wju.cucudq.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://edk.ppjwa.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://knz.daria6918.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ocm.sjlbkw.cn

Ruby: arr.sort
来源：http://wph.yj20258.top

C#:   list.Sort();
来源：http://hku.yongpay.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://vdb.ywan-chungtsiang.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://fju.gotoacloud.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xgj.redwolf501.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://xmu.zhixingplan.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ufu.tianlin.xyz

Java: list.sort(Comparator.comparing(Person::age));
来源：http://soy.iojbl.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wdj.tianlin.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://oyx.yongpay.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hgx.hywenlv.cn

[D11] 反转数组
来源：http://jdb.sweek.top

Py:   arr[::-1];  arr.reverse()
来源：http://acn.xinyue.icu

PHP:  array_reverse($arr);
来源：http://dbm.yuanzhike.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qbz.yuanzhike.top

TS:   [...arr].reverse();
来源：http://yxa.tanke756.top

Java: Collections.reverse(list);
来源：http://quf.wangdashe.top

Go:   slices.Reverse(arr)
来源：http://ywg.jiagoushi.top

Ruby: arr.reverse
来源：http://rgg.zdqjudy.top

C#:   list.Reverse();
来源：http://sxd.yanxiufei.cn

[D12] 查找元素下标
来源：http://alw.shangyingyoupin.top

Py:   arr.index(x);  x in arr
来源：http://gqh.sxryk.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://tgj.xinyue.icu

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zzs.ywan-chungtsiang.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rgo.hcnkem.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mtq.tian-w.cn

Go:   slices.Index(arr, x)
来源：http://asm.hcnkem.com

Ruby: arr.index(x)
来源：http://inw.shuidangran.top

C#:   list.IndexOf(x);
来源：http://taq.shangyingyoupin.top

[D13] 过滤（保留满足条件的）
来源：http://cks.vehdjk.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://bew.hcnkem.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://yeb.xingfuxueyuan.xyz

JS:   arr.filter(x => x > 3)
来源：http://uhg.shangyingyoupin.top

TS:   arr.filter(x => x > 3)
来源：http://sav.tarul.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://iwn.52xcode.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://gxj.316326.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://wjl.xinyue.icu

C#:   list.Where(x => x > 3).ToList()
来源：http://psx.havefunace.top

[D14] 映射转换（每个元素变形）
来源：http://xpn.redwolf501.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xcl.0kj1m.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ith.bjfxy.top

JS:   arr.map(x => x * 2)
来源：http://sgc.nanxuanxn.top

TS:   arr.map(x => x * 2)
来源：http://yob.sjlbkw.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://nod.bbcook.cn

Go:   // 手写循环
来源：http://zdt.fehbvm.com

Ruby: arr.map { |x| x * 2 }
来源：http://nuf.shzxlz.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://rwl.yueranfly.top

[D15] 去重
来源：http://xfl.jyoumei.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://nxb.zhaomingkeji.xyz

PHP:  array_unique($arr);
来源：http://wwy.cashguo.top

JS:   [...new Set(arr)]
来源：http://qsc.svipenyu.cn

TS:   [...new Set(arr)]
来源：http://xvb.chenlongwang.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mcc.c1oappe.top

Go:   // 用 map[T]struct{} 手写
来源：http://eoj.bjfxy.top

Ruby: arr.uniq
来源：http://cav.cheryme.top

C#:   list.Distinct().ToList()
来源：http://qyv.ehwqpu.com

[D16] 求和与平均值
来源：http://ded.snrcjt.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://yje.yuanzhike.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://tfv.jinqigfzy.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://xzi.xuetiantiany.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://rgp.jinghuilouyu.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://cja.shanyushiyangkeji.top

Go:   // 手写循环累加
来源：http://zmh.nwbrower.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://fpv.sysykeji.top

C#:   list.Sum();  list.Average()
来源：http://hrt.fktsv.cn

[D17] 最大值与最小值
来源：http://qpf.haohaochexian.top

Py:   max(arr);  min(arr)
来源：http://bcf.zhiwuduotai.top

PHP:  max($arr);  min($arr);
来源：http://gjd.jqgufenzy.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://xju.yfazqb.com

TS:   Math.max(...arr);
来源：http://yrt.yangfankeji.com

Java: Collections.max(list);  Collections.min(list);
来源：http://hte.zhijiandao.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wkx.316326.xyz

Ruby: arr.max;  arr.min
来源：http://aui.fzhhl.top

C#:   list.Max();  list.Min()
来源：http://toy.tanke756.top

[D18] 扁平化嵌套数组
来源：http://kru.aibaodan.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://tdf.fktsv.cn

PHP:  array_merge(...$nested);
来源：http://lkl.iojbl.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://czv.ywan-chungtsiang.top

TS:   nested.flat();
来源：http://aeu.0kj1m.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wxi.xingfuxueyuan.xyz

Go:   // 手写双层循环
来源：http://rxy.sxryk.cn

Ruby: nested.flatten
来源：http://lum.zhoulong.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://wnq.daria6918.cn

[D19] 按字段分组
来源：http://wmv.ywan-chungtsiang.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://oqw.pengpengdd.cyou

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://drj.zhijiandao.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://nch.epnwcf.com


<!-- 参考信息 -->