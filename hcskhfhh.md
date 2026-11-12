代发 wailian999

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wbw.jinyuanbaomall.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://dhh.aibaodan.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://owj.yj20258.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://nne.xingfuxueyuan.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://ieh.zhiwuduotai.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://cai.shuidangran.top

[C04] 命名参数 / 关键字参数
来源：http://wfa.gaohongyu789.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://jnb.zhixingplan.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://oxq.cqqwz.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://eog.epnwcf.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://yae.vehdjk.com

Java: // 无：用 Builder 模式或 record
来源：http://tpn.dianchejie.cn

Go:   // 无：用配置结构体参数
来源：http://zco.jqgufenzy.top

Ruby: f(a: 1, b: 2)
来源：http://bre.yangfankeji.com

C#:   f(a: 1, b: 2)
来源：http://yfo.sxryk.cn

[C05] 返回多个值
来源：http://niq.pycfn.com

Py:   return a, b
来源：http://vrr.fanxiaobao.xyz

PHP:  return [$a, $b];
来源：http://rel.jiagoushi.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://ixy.daxiang520.top

TS:   return { a, b };
来源：http://cyg.sxryk.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mxq.cqqwz.cn

Go:   return a, b
来源：http://pul.shuidangran.top

Ruby: return a, b
来源：http://xrd.hesvh.cn

C#:   return (a, b);              // ValueTuple
来源：http://omw.ehwqpu.com

[C06] 匿名函数 / lambda
来源：http://vjz.yvedp.cn

Py:   square = lambda x: x * x
来源：http://bhv.hywenlv.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://god.fzhhl.top

JS:   const square = x => x * x;
来源：http://fmf.nanxinkj.top

TS:   const square = (x: number): number => x * x;
来源：http://nzs.xuetiantiany.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://uvg.hfpthk.cn

Go:   sq := func(x int) int { return x * x }
来源：http://lbd.52xcode.cn

Ruby: square = ->(x) { x * x }
来源：http://chu.sxryk.cn

C#:   Func<int, int> square = x => x * x;
来源：http://hft.cashguo.top

[C07] 把函数作为参数传入
来源：http://jld.xziqi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://zza.shanyushiyangtech.top

PHP:  array_map("strtoupper", $arr);
来源：http://jor.jlsjyb.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://tzh.hnxiangtu.top

TS:   arr.map(String)
来源：http://xyf.uphjek.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://izg.epnwcf.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://zof.haohaochexian.top

Ruby: arr.map(&:upcase)
来源：http://dfj.zhijiandao.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://gqh.ydzc1.top

[C08] 闭包
来源：http://koz.shanyushiyangtech.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://aka.jlsjyb.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://avr.zhongyouzk.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://suj.yj20258888.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://lop.zycfv.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://nca.pengpengdd.cyou

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://sdn.nanxuanxn.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://fet.pengpengdd.cyou

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://win.aizwys.cn

[C09] 递归
来源：http://uqv.jqgufenzy.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://sry.wangshuangyany.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://dtb.chenlongwang.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zip.shzxlz.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xgc.guannengcc.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ibj.uphjek.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://vua.hfpthk.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://unk.cdnleiting.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hkp.jinghuilouyu.cn

[C10] 变量作用域
来源：http://all.wangdashe.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://oyw.ctjpmb.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://rsm.hfpthk.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ipn.daria6918.cn

TS:   同 JS
来源：http://iju.zdbjq.cn

Java: 方法内为块级作用域
来源：http://qjc.birdmap.top

Go:   花括号块级作用域
来源：http://swc.yonumen.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://lhl.yonumen.top

C#:   块级作用域
来源：http://xny.meibo888.top

[C11] 模块导入与导出
来源：http://jgp.shuidangran.top

Py:   from module import func
来源：http://phf.yfazqb.com

PHP:  require "file.php";  或 use App\Service;
来源：http://ivq.wangshuangyany.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://iru.tanke756.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://nad.jlsjyb.cn

Java: import java.util.List;
来源：http://lsj.redwolf501.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://fph.zdbjq.cn

Ruby: require "json"; require_relative "./util"
来源：http://adp.yfazqb.com

C#:   using System.Text;
来源：http://upd.cdnleiting.top

[C12] 立即执行函数 IIFE
来源：http://hvf.jqgufenzy.top

Py:   (lambda: print("run"))()
来源：http://tna.aibaodan.cn

PHP:  (function () { echo "run"; })();
来源：http://kbk.jinqigfzy.top

JS:   (() => { console.log("run"); })();
来源：http://ehj.zhixingplan.top

TS:   (() => { console.log("run"); })();
来源：http://vsx.aizwys.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://nfk.ydjk.org.cn

Go:   func() { fmt.Println("run") }()
来源：http://ggt.shzxlz.cn

Ruby: -> { puts "run" }.call
来源：http://ril.guowangkeji.top

C#:   // 无 IIFE：用静态构造函数
来源：http://svz.gogol.net.cn

[C13] 类型声明 / 类型注解
来源：http://uvu.sweek.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://qur.shangyingyoupin.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bnj.jianghu66.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://nne.wangdashe.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zwf.ybcxt.top

Java: int add(int a, int b) { return a + b; }
来源：http://roz.jqgfzy.top

Go:   func add(a, b int) int
来源：http://ran.zhoulong.xyz

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://zxf.fktsv.cn

C#:   int Add(int a, int b) => a + b;
来源：http://duu.svipenyu.cn

[C14] 泛型函数
来源：http://qrk.xziqi.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://phg.bjfxy.top

PHP:  // 无泛型
来源：http://zka.gogol.net.cn

JS:   // 无泛型
来源：http://kxj.tarul.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://iro.yongpay.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://tdf.hfpthk.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://cwu.pengpengdd.cyou

Ruby: # 无泛型
来源：http://nhj.vqdsnc.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://zuv.xingfuxueyuan.xyz

[C15] 解构 / 展开参数
来源：http://tsb.nwbrower.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ooe.316326.xyz

PHP:  [$a, $b] = $pair;
来源：http://ino.mhx1999.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://gyy.yangfankeji.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ees.jinyuanbaomall.cn

Java: // 无解构
来源：http://whr.hammf.cn

Go:   // 无解构
来源：http://juu.hesvh.cn

Ruby: a, b = pair
来源：http://ekf.yj20258.top

C#:   var (a, b) = pair;
来源：http://pjz.yuxming.cn

[C16] 函数 / 方法重载
来源：http://nnn.0kj1m.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://czs.hysaishi.cn

PHP:  // 无重载
来源：http://plz.fktsv.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://hjm.yangfankeji.com

TS:   // 用联合类型或重载签名声明
来源：http://vyx.zdqjudy.top

Java: void f(int a) {}  void f(String a) {}
来源：http://qon.gzhubu.top

Go:   // 无重载：用不同函数名
来源：http://lzq.uphjek.com

Ruby: # 无重载：靠动态参数
来源：http://uow.dashuyun.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://yeq.aizwys.cn

================================================================================
来源：http://ixl.dashuyun.cn

D. 数组 / 列表 / 集合
来源：http://umm.yuanzhike.top

================================================================================
来源：http://toi.0kj1m.cn

[D01] 创建数组 / 列表
来源：http://dpk.xinyue.icu

Py:   arr = [1, 2, 3];  empty = []
来源：http://mfz.jinqigufen.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://klz.birdmap.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hck.epnwcf.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://yee.jinyuanbaomall.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://non.zdqjudy.top

Go:   arr := []int{1, 2, 3}
来源：http://jfk.dashuyun.cn

Ruby: arr = [1, 2, 3]
来源：http://sss.ydzc1.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://nft.shuidangran.top

[D02] 追加元素到末尾
来源：http://ecf.svipenyu.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://nze.cucudq.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hla.zycfv.cn

JS:   arr.push(4);
来源：http://jct.daria6918.cn

TS:   arr.push(4);
来源：http://lcm.hesvh.cn

Java: list.add(4);
来源：http://qxz.hesvh.cn

Go:   arr = append(arr, 4)
来源：http://qgi.chenzaomai.com

Ruby: arr << 4; arr.push(5)
来源：http://mtq.yongpay.top

C#:   list.Add(4);
来源：http://yip.52xcode.cn

[D03] 在指定位置插入元素
来源：http://prz.redwolf501.top

Py:   arr.insert(0, 0)
来源：http://uwu.yj20258888.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://nhh.fktsv.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://fzj.yvedp.cn

TS:   arr.splice(0, 0, 0);
来源：http://emp.ywan-chungtsiang.top

Java: list.add(0, 0);
来源：http://wmf.aizwys.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ctk.ywan-chungtsiang.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://gdq.pycfn.com

C#:   list.Insert(0, 0);
来源：http://ltm.yuxming.cn

[D04] 删除元素
来源：http://wag.sufxvd.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hxc.zdbjq.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wmo.sjlbkw.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://jcu.cheryme.top

TS:   arr.splice(0, 1);
来源：http://ane.zycfv.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://vlx.gzhubu.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://arm.iojbl.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://gjf.andypj.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://lqb.havefunace.top

[D05] 访问与修改元素
来源：http://fez.uphjek.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://fnz.ybcxt.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://zgc.jlsjyb.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://gfw.yj202588.top

TS:   arr[0]; arr.at(-1);
来源：http://qtp.ivvv.top

Java: list.get(0); list.set(0, 9);
来源：http://chp.mhx1999.top

Go:   arr[0]; arr[0] = 9
来源：http://doo.316326.xyz

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://fyb.ehwqpu.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://cvc.fengsongda.top

[D06] 数组长度
来源：http://ckr.quarkkingdee.top

Py:   len(arr)
来源：http://npr.meibo888.top

PHP:  count($arr);
来源：http://kmd.wangshuangyany.cn

JS:   arr.length
来源：http://exi.9152youxi.cn

TS:   arr.length
来源：http://yma.dashuyun.cn

Java: list.size();
来源：http://iky.hfpthk.cn

Go:   len(arr)
来源：http://kat.wangdashe.top

Ruby: arr.length; arr.size
来源：http://hqj.dianchejie.cn

C#:   list.Count;
来源：http://ifi.ybcxt.top

[D07] 切片 / 取子数组
来源：http://lmg.jlsjyb.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://buy.9152youxi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://yqk.ydjk.org.cn

JS:   arr.slice(1, 4);
来源：http://chd.bbcook.cn

TS:   arr.slice(1, 4);
来源：http://ekr.shanyushiyangkeji.top

Java: list.subList(1, 4);
来源：http://jts.dashuyun.cn

Go:   arr[1:4]
来源：http://fgb.hnxiangtu.top

Ruby: arr[1, 3]
来源：http://dbg.sjlbkw.cn

C#:   list.GetRange(1, 3);
来源：http://pxl.hesvh.cn

[D08] 合并两个数组
来源：http://whf.sjlbkw.cn

Py:   a + b;  a.extend(b)
来源：http://isw.jinqigufen.top

PHP:  array_merge($a, $b);
来源：http://ulj.tianlin.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://tpg.hongshengwenyu.top

TS:   [...a, ...b];
来源：http://rqo.0kj1m.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://qvp.xuetiantiany.cn

Go:   append(a, b...)
来源：http://zpd.316326.xyz

Ruby: a + b;  a.concat(b)
来源：http://kgs.yj202588.top

C#:   a.Concat(b).ToList()
来源：http://vne.uphjek.com

[D09] 排序（升序）
来源：http://zby.hfpthk.cn

Py:   sorted(arr);  arr.sort()
来源：http://mds.guannengcc.top

PHP:  sort($arr);
来源：http://edg.316326.xyz

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://izk.yvedp.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://hyq.gotoacloud.top

Java: Collections.sort(list);  list.sort(null);
来源：http://vgp.hcnkem.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://kkm.xziqi.cn

Ruby: arr.sort
来源：http://tsd.guannengcc.top

C#:   list.Sort();
来源：http://fko.jlsjyb.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://cqk.jinqigfzy.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mzf.sjlbkw.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://orf.ywan-chungtsiang.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://qov.sjlbkw.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://izh.zhixingplan.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://nkd.zhiwuduotai.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://eik.hnqzz.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://jps.fehbvm.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hsu.c1oappe.top

[D11] 反转数组
来源：http://urv.ivvv.top

Py:   arr[::-1];  arr.reverse()
来源：http://fzw.guowangkeji.top

PHP:  array_reverse($arr);
来源：http://prk.zhixingplan.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://yzo.aibaodan.cn

TS:   [...arr].reverse();
来源：http://mkc.gzhubu.top

Java: Collections.reverse(list);
来源：http://zmu.xuanzx.com

Go:   slices.Reverse(arr)
来源：http://vrk.xziqi.cn

Ruby: arr.reverse
来源：http://qjl.haohaochexian.top

C#:   list.Reverse();
来源：http://wyx.ctjpmb.com

[D12] 查找元素下标
来源：http://uny.yueranfly.top

Py:   arr.index(x);  x in arr
来源：http://guc.xinyue.icu

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hnu.ctjpmb.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ttj.jinghuilouyu.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ozu.zdqjudy.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://amp.hysaishi.cn

Go:   slices.Index(arr, x)
来源：http://vjv.andypj.xyz

Ruby: arr.index(x)
来源：http://dus.zhongyouzk.top

C#:   list.IndexOf(x);
来源：http://hhr.sxryk.cn

[D13] 过滤（保留满足条件的）
来源：http://rar.xingfuxueyuan.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://sap.yj20258888.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://omm.vqdsnc.cn

JS:   arr.filter(x => x > 3)
来源：http://epe.birdmap.top

TS:   arr.filter(x => x > 3)
来源：http://tcl.52xcode.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://gzz.dianchejie.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://jmq.ydzc1.top

Ruby: arr.select { |x| x > 3 }
来源：http://xju.ctjpmb.com

C#:   list.Where(x => x > 3).ToList()
来源：http://obv.bbcook.cn

[D14] 映射转换（每个元素变形）
来源：http://ear.nwbrower.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://dzq.ehwqpu.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://yci.shuidangran.top

JS:   arr.map(x => x * 2)
来源：http://cty.birdmap.top

TS:   arr.map(x => x * 2)
来源：http://mar.yuanzhike.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://xaa.meibo888.top

Go:   // 手写循环
来源：http://mzg.zhaomingkeji.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://vau.vehdjk.com

C#:   list.Select(x => x * 2).ToList()
来源：http://pjw.jlsjyb.cn

[D15] 去重
来源：http://bvz.yanxiufei.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://jun.nanxuanxn.top

PHP:  array_unique($arr);
来源：http://mpx.yfazqb.com

JS:   [...new Set(arr)]
来源：http://caf.xingfuxueyuan.xyz

TS:   [...new Set(arr)]
来源：http://nne.yangfankeji.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://loe.cheryme.top

Go:   // 用 map[T]struct{} 手写
来源：http://dxi.hongshengwenyu.top

Ruby: arr.uniq
来源：http://ijy.ybcxt.top

C#:   list.Distinct().ToList()
来源：http://gaj.jinghuilouyu.cn

[D16] 求和与平均值
来源：http://vwx.iojbl.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://rhh.cashguo.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://dss.guannengcc.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://bzj.yonumen.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://oun.jlsjyb.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://uhj.kuanghao11.cn

Go:   // 手写循环累加
来源：http://tab.hnxiangtu.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hzg.birdmap.top

C#:   list.Sum();  list.Average()
来源：http://voh.kuanghao11.cn

[D17] 最大值与最小值
来源：http://huu.aizwys.cn

Py:   max(arr);  min(arr)
来源：http://mha.jiagoushi.top

PHP:  max($arr);  min($arr);
来源：http://fyd.vehdjk.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://eoy.sufxvd.cn

TS:   Math.max(...arr);
来源：http://sgy.cheryme.top

Java: Collections.max(list);  Collections.min(list);
来源：http://hal.9152youxi.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://gxu.cheryme.top

Ruby: arr.max;  arr.min
来源：http://lza.hcnkem.com

C#:   list.Max();  list.Min()
来源：http://gko.yj20258.top

[D18] 扁平化嵌套数组
来源：http://aqz.fktsv.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://sso.316326.xyz

PHP:  array_merge(...$nested);
来源：http://tdb.cucudq.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://snn.chenlongwang.top

TS:   nested.flat();
来源：http://oub.0kj1m.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://vjb.smart0.xyz

Go:   // 手写双层循环
来源：http://loy.yvedp.cn

Ruby: nested.flatten
来源：http://ajt.jqgufenzy.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://kid.yanxiufei.cn

[D19] 按字段分组
来源：http://crf.xuetiantiany.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wal.zhongyouzk.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://gyc.zdqjudy.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ntg.guowangkeji.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://hzd.fzhhl.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://cif.chenzaomai.com

Go:   // 手写 map[string][]T
来源：http://dvy.hnqzz.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://crh.nanxuanxn.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://vtf.yongpay.top

[D20] 统计每个元素出现次数
来源：http://bjd.mhx1999.top

Py:   Counter(arr)
来源：http://nxu.hongshengwenyu.top

PHP:  array_count_values($arr);
来源：http://sxe.chenzaomai.com


<!-- 参考信息 -->