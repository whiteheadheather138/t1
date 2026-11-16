代发 wailian999

Py:   def add(a, b): return a + b
来源：http://pkq.andypj.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kjb.yuanzhike.top

JS:   function add(a, b) { return a + b; }
来源：http://udk.birdmap.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ctj.guowangkeji.top

Java: static int add(int a, int b) { return a + b; }
来源：http://nyk.yueranfly.top

Go:   func add(a, b int) int { return a + b }
来源：http://roc.xingfuxueyuan.xyz

Ruby: def add(a, b); a + b; end
来源：http://oia.hnqzz.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://fql.fengsongda.top

[C02] 默认参数
来源：http://nlc.nanxinkj.top

Py:   def greet(name="World"): return name
来源：http://zhi.meibo888.top

PHP:  function greet($name = "World") { return $name; }
来源：http://vxy.316326.xyz

JS:   function greet(name = "World") { return name; }
来源：http://lef.316326.xyz

TS:   function greet(name: string = "World") { return name; }
来源：http://hik.0kj1m.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ezy.uphjek.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ujx.zhongyouzk.top

Ruby: def greet(name = "World") = name
来源：http://xxn.xuetiantiany.cn

C#:   string Greet(string name = "World") => name;
来源：http://wzb.jinghuilouyu.cn

[C03] 可变参数
来源：http://ivy.9152youxi.cn

Py:   def total(*args): return sum(args)
来源：http://cqf.quarkkingdee.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://zrb.hcnkem.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mwn.hnxiangtu.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://vuo.epnwcf.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://pia.svipenyu.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://yny.hnxiangtu.top

Ruby: def total(*nums); nums.sum; end
来源：http://yxp.gogol.net.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mpy.c1oappe.top

[C04] 命名参数 / 关键字参数
来源：http://iez.hcnkem.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://qgp.daria6918.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://pkj.cashguo.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://nva.iojbl.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mvx.zhiwuduotai.top

Java: // 无：用 Builder 模式或 record
来源：http://ygw.yj202588.top

Go:   // 无：用配置结构体参数
来源：http://cmn.zhongyouzk.top

Ruby: f(a: 1, b: 2)
来源：http://dyc.hesvh.cn

C#:   f(a: 1, b: 2)
来源：http://bbo.jinyuanbaomall.cn

[C05] 返回多个值
来源：http://tew.sufxvd.cn

Py:   return a, b
来源：http://dci.316326.xyz

PHP:  return [$a, $b];
来源：http://cfr.svipenyu.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://fez.birdmap.top

TS:   return { a, b };
来源：http://pid.nanxinkj.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://etv.chenjidiqi.icu

Go:   return a, b
来源：http://yom.fengsongda.top

Ruby: return a, b
来源：http://rdo.zhixingplan.top

C#:   return (a, b);              // ValueTuple
来源：http://gqo.kuanghao11.cn

[C06] 匿名函数 / lambda
来源：http://axn.hywenlv.cn

Py:   square = lambda x: x * x
来源：http://dtg.chenzaomai.com

PHP:  $square = fn($x) => $x * $x;
来源：http://uro.sjlbkw.cn

JS:   const square = x => x * x;
来源：http://gdr.hywenlv.cn

TS:   const square = (x: number): number => x * x;
来源：http://rbz.c1oappe.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://rlk.jqgfzy.top

Go:   sq := func(x int) int { return x * x }
来源：http://ugp.dashuyun.cn

Ruby: square = ->(x) { x * x }
来源：http://xnu.redwolf501.top

C#:   Func<int, int> square = x => x * x;
来源：http://rgv.jinqigfzy.top

[C07] 把函数作为参数传入
来源：http://enq.hongshengwenyu.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://iqb.svipenyu.cn

PHP:  array_map("strtoupper", $arr);
来源：http://jzl.hnqzz.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://cht.dianchejie.cn

TS:   arr.map(String)
来源：http://vgi.quarkkingdee.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://tue.jinqigfzy.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://vqo.jinyuanbaomall.cn

Ruby: arr.map(&:upcase)
来源：http://qxu.dianchejie.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://twe.ydjk.org.cn

[C08] 闭包
来源：http://jyt.zhongyouzk.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://emv.zycfv.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ryo.jinyuanbaomall.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://dca.dashuyun.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://yjv.nanxinkj.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://axg.sweek.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://btz.cqqwz.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://azc.zdbjq.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://qma.svipenyu.cn

[C09] 递归
来源：http://nlc.smart0.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://jfa.snrcjt.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hwq.aibaodan.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xli.jiagoushi.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tkf.hnqzz.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://uty.feifeiyinyue.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://jbe.ctjpmb.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://jxz.cqqwz.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://pvi.fehbvm.com

[C10] 变量作用域
来源：http://ecv.shuidangran.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://zlh.gogol.net.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mdf.cheryme.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://szi.jianghu66.top

TS:   同 JS
来源：http://pwg.gotoacloud.top

Java: 方法内为块级作用域
来源：http://fay.mhx1999.top

Go:   花括号块级作用域
来源：http://woc.xuanzx.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://pge.gzhubu.top

C#:   块级作用域
来源：http://hln.zhixingplan.top

[C11] 模块导入与导出
来源：http://bfe.nwbrower.top

Py:   from module import func
来源：http://dbb.hnqzz.top

PHP:  require "file.php";  或 use App\Service;
来源：http://rlf.yj202588.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://iwt.quarkkingdee.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://jpw.52xcode.cn

Java: import java.util.List;
来源：http://fnv.birdmap.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://rgp.gaohongyu789.top

Ruby: require "json"; require_relative "./util"
来源：http://wef.smart0.xyz

C#:   using System.Text;
来源：http://kze.xziqi.cn

[C12] 立即执行函数 IIFE
来源：http://wve.ctjpmb.com

Py:   (lambda: print("run"))()
来源：http://ppd.yueranfly.top

PHP:  (function () { echo "run"; })();
来源：http://dxv.pycfn.com

JS:   (() => { console.log("run"); })();
来源：http://vqb.ybcxt.top

TS:   (() => { console.log("run"); })();
来源：http://lai.xingfuxueyuan.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hff.vehdjk.com

Go:   func() { fmt.Println("run") }()
来源：http://orn.316326.xyz

Ruby: -> { puts "run" }.call
来源：http://aai.gogol.net.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://krc.0kj1m.cn

[C13] 类型声明 / 类型注解
来源：http://tur.guannengcc.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://pfe.shanyushiyangtech.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hmk.birdmap.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://gcg.cqqwz.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://iqq.shuidangran.top

Java: int add(int a, int b) { return a + b; }
来源：http://dke.ywan-chungtsiang.top

Go:   func add(a, b int) int
来源：http://mpm.yonumen.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://vau.hesvh.cn

C#:   int Add(int a, int b) => a + b;
来源：http://kzt.zhixingplan.top

[C14] 泛型函数
来源：http://cla.yangfankeji.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://sxz.xylfe.cn

PHP:  // 无泛型
来源：http://zhl.yonumen.top

JS:   // 无泛型
来源：http://cib.guowangkeji.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://asu.shanyushiyangtech.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wvv.havefunace.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hyr.ehwqpu.com

Ruby: # 无泛型
来源：http://zlo.guannengcc.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://kua.nanxinkj.top

[C15] 解构 / 展开参数
来源：http://hki.aibaodan.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://iwv.aibaodan.cn

PHP:  [$a, $b] = $pair;
来源：http://bkl.epnwcf.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mgc.cqqwz.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://xzb.jyoumei.cn

Java: // 无解构
来源：http://jeq.yanxiufei.cn

Go:   // 无解构
来源：http://awa.dianchejie.cn

Ruby: a, b = pair
来源：http://kjx.hammf.cn

C#:   var (a, b) = pair;
来源：http://ocl.uphjek.com

[C16] 函数 / 方法重载
来源：http://axx.yfazqb.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ace.epnwcf.com

PHP:  // 无重载
来源：http://ncc.quarkkingdee.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://ilv.quarkkingdee.top

TS:   // 用联合类型或重载签名声明
来源：http://ych.mhx1999.top

Java: void f(int a) {}  void f(String a) {}
来源：http://xit.ywan-chungtsiang.top

Go:   // 无重载：用不同函数名
来源：http://ggo.haohaochexian.top

Ruby: # 无重载：靠动态参数
来源：http://exi.vqdsnc.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://goz.yongpay.top

================================================================================
来源：http://wtn.meibo888.top

D. 数组 / 列表 / 集合
来源：http://aku.jianghu66.top

================================================================================
来源：http://aaz.fengsongda.top

[D01] 创建数组 / 列表
来源：http://urz.nanxinkj.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://qzd.sufxvd.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hpk.svipenyu.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://xpg.jinyuanbaomall.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://jhr.dianchejie.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://xos.yonumen.top

Go:   arr := []int{1, 2, 3}
来源：http://uls.yj20258.top

Ruby: arr = [1, 2, 3]
来源：http://oir.yueranfly.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://jaz.yvedp.cn

[D02] 追加元素到末尾
来源：http://ubm.jlsjyb.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ekd.xinyue.icu

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://qet.fengsongda.top

JS:   arr.push(4);
来源：http://xjz.daxiang520.top

TS:   arr.push(4);
来源：http://ejm.pycfn.com

Java: list.add(4);
来源：http://qif.yanxiufei.cn

Go:   arr = append(arr, 4)
来源：http://aqb.sjlbkw.cn

Ruby: arr << 4; arr.push(5)
来源：http://wac.hysaishi.cn

C#:   list.Add(4);
来源：http://vdd.kuanghao11.cn

[D03] 在指定位置插入元素
来源：http://qms.xinyue.icu

Py:   arr.insert(0, 0)
来源：http://yby.hammf.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://tvq.daria6918.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hsl.sjlbkw.cn

TS:   arr.splice(0, 0, 0);
来源：http://vvf.sxryk.cn

Java: list.add(0, 0);
来源：http://qvv.mhx1999.top

Go:   arr = append([]int{0}, arr...)
来源：http://olt.nanxinkj.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://xpv.fengsongda.top

C#:   list.Insert(0, 0);
来源：http://ssw.shangyingyoupin.top

[D04] 删除元素
来源：http://rta.cqqwz.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://bjm.dashuyun.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://tcy.dianchejie.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://jcv.daria6918.cn

TS:   arr.splice(0, 1);
来源：http://nyz.shanyushiyangkeji.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://imd.vqdsnc.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://gxw.zhixingplan.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://nit.yangfankeji.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://rel.feifeiyinyue.top

[D05] 访问与修改元素
来源：http://mlh.yangfankeji.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://yfn.redwolf501.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://kfs.aizwys.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://oed.nwbrower.top

TS:   arr[0]; arr.at(-1);
来源：http://ucg.yongpay.top

Java: list.get(0); list.set(0, 9);
来源：http://rrp.chenzaomai.com

Go:   arr[0]; arr[0] = 9
来源：http://pht.ivvv.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hot.xuanzx.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ifq.jinghuilouyu.cn

[D06] 数组长度
来源：http://xup.zhiwuduotai.top

Py:   len(arr)
来源：http://jme.cucudq.cn

PHP:  count($arr);
来源：http://atz.yanxiufei.cn

JS:   arr.length
来源：http://nwl.quarkkingdee.top

TS:   arr.length
来源：http://qoe.sweek.top

Java: list.size();
来源：http://xrl.hcnkem.com

Go:   len(arr)
来源：http://vdn.nwbrower.top

Ruby: arr.length; arr.size
来源：http://xsi.cheryme.top

C#:   list.Count;
来源：http://zal.sweek.top

[D07] 切片 / 取子数组
来源：http://zwr.hammf.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://lbp.svipenyu.cn

PHP:  array_slice($arr, 1, 3);
来源：http://uej.zdbjq.cn

JS:   arr.slice(1, 4);
来源：http://hrn.ydjk.org.cn

TS:   arr.slice(1, 4);
来源：http://ril.zdbjq.cn

Java: list.subList(1, 4);
来源：http://roq.yfazqb.com

Go:   arr[1:4]
来源：http://pkb.bbcook.cn

Ruby: arr[1, 3]
来源：http://uub.zhijiandao.cn

C#:   list.GetRange(1, 3);
来源：http://qov.andypj.xyz

[D08] 合并两个数组
来源：http://bxz.jinyuanbaomall.cn

Py:   a + b;  a.extend(b)
来源：http://uxe.sjlbkw.cn

PHP:  array_merge($a, $b);
来源：http://vje.pengpengdd.cyou

JS:   [...a, ...b];  a.concat(b);
来源：http://nzs.epnwcf.com

TS:   [...a, ...b];
来源：http://ixt.wangdashe.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://qcs.ppjwa.cn

Go:   append(a, b...)
来源：http://szj.meibo888.top

Ruby: a + b;  a.concat(b)
来源：http://rhv.sufxvd.cn

C#:   a.Concat(b).ToList()
来源：http://hyi.cqqwz.cn

[D09] 排序（升序）
来源：http://jlm.zhoulong.xyz

Py:   sorted(arr);  arr.sort()
来源：http://avq.sjlbkw.cn

PHP:  sort($arr);
来源：http://lwt.316326.xyz

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wig.hammf.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://njc.cdnleiting.top

Java: Collections.sort(list);  list.sort(null);
来源：http://hag.chenlongwang.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mdt.zhaomingkeji.xyz

Ruby: arr.sort
来源：http://ijb.bbcook.cn

C#:   list.Sort();
来源：http://toh.jqgfzy.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://vdu.jinqigfzy.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ktx.shuidangran.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vrw.pengpengdd.cyou

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://iws.zhaomingkeji.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://cuh.zdbjq.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://bbr.jlsjyb.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://prw.zhijiandao.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://dqf.fzhhl.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://vyk.zhiwuduotai.top

[D11] 反转数组
来源：http://xya.tian-w.cn

Py:   arr[::-1];  arr.reverse()
来源：http://zxm.snrcjt.cn

PHP:  array_reverse($arr);
来源：http://fiz.xinyue.icu

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ivu.0kj1m.cn

TS:   [...arr].reverse();
来源：http://qbl.yueranfly.top

Java: Collections.reverse(list);
来源：http://zhx.yonumen.top

Go:   slices.Reverse(arr)
来源：http://ssh.yj20258888.top

Ruby: arr.reverse
来源：http://ugq.shzxlz.cn

C#:   list.Reverse();
来源：http://omw.shuidangran.top

[D12] 查找元素下标
来源：http://dlo.quarkkingdee.top

Py:   arr.index(x);  x in arr
来源：http://xzk.guannengcc.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://zbq.gogol.net.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dcz.cdnleiting.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qta.zhiwuduotai.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://obl.ywan-chungtsiang.top

Go:   slices.Index(arr, x)
来源：http://uao.jyoumei.cn

Ruby: arr.index(x)
来源：http://asp.sysykeji.top

C#:   list.IndexOf(x);
来源：http://vir.zycfv.cn

[D13] 过滤（保留满足条件的）
来源：http://eav.cdnleiting.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://dnz.chenjidiqi.icu

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://vfu.yuxming.cn

JS:   arr.filter(x => x > 3)
来源：http://wla.dashuyun.cn

TS:   arr.filter(x => x > 3)
来源：http://jhl.hnqzz.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://dti.yfazqb.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://nzp.fehbvm.com

Ruby: arr.select { |x| x > 3 }
来源：http://atp.yuanzhike.top

C#:   list.Where(x => x > 3).ToList()
来源：http://iuc.andypj.xyz

[D14] 映射转换（每个元素变形）
来源：http://oci.guannengcc.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://jit.mhx1999.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://cbl.shzxlz.cn

JS:   arr.map(x => x * 2)
来源：http://bwq.cashguo.top

TS:   arr.map(x => x * 2)
来源：http://xlx.ydjk.org.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://atv.zhiwuduotai.top

Go:   // 手写循环
来源：http://sja.zycfv.cn

Ruby: arr.map { |x| x * 2 }
来源：http://yam.havefunace.top

C#:   list.Select(x => x * 2).ToList()
来源：http://mus.shangyingyoupin.top

[D15] 去重
来源：http://bat.nanxinkj.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://nax.redwolf501.top

PHP:  array_unique($arr);
来源：http://wif.andypj.xyz

JS:   [...new Set(arr)]
来源：http://cjg.chenlongwang.top

TS:   [...new Set(arr)]
来源：http://ztd.guowangkeji.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://qgm.316326.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://xde.hcnkem.com

Ruby: arr.uniq
来源：http://way.9152youxi.cn

C#:   list.Distinct().ToList()
来源：http://iwy.sjlbkw.cn

[D16] 求和与平均值
来源：http://sgh.jyoumei.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://nco.tianlin.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ewq.hammf.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://tgu.haohaochexian.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ajx.gaohongyu789.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ska.yuxming.cn

Go:   // 手写循环累加
来源：http://aal.zdbjq.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://xva.sxryk.cn

C#:   list.Sum();  list.Average()
来源：http://pau.epnwcf.com

[D17] 最大值与最小值
来源：http://nvf.52xcode.cn

Py:   max(arr);  min(arr)
来源：http://pbx.yuanzhike.top

PHP:  max($arr);  min($arr);
来源：http://uyr.tanke756.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://tty.guowangkeji.top

TS:   Math.max(...arr);
来源：http://lno.hongshengwenyu.top

Java: Collections.max(list);  Collections.min(list);
来源：http://xah.zhiwuduotai.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://tyu.sweek.top

Ruby: arr.max;  arr.min
来源：http://jel.vqdsnc.cn

C#:   list.Max();  list.Min()
来源：http://vsh.epnwcf.com

[D18] 扁平化嵌套数组
来源：http://bsp.shangyingyoupin.top


<!-- 参考信息 -->