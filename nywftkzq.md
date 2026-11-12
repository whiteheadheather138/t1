代发 wailian999

Py:   def add(a, b): return a + b
来源：http://phe.jianghu66.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ilg.tianlin.xyz

JS:   function add(a, b) { return a + b; }
来源：http://cfs.shangyingyoupin.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ezp.jinqigfzy.top

Java: static int add(int a, int b) { return a + b; }
来源：http://nsu.xuetiantiany.cn

Go:   func add(a, b int) int { return a + b }
来源：http://byf.yuxming.cn

Ruby: def add(a, b); a + b; end
来源：http://twl.nanxuanxn.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mlw.feifeiyinyue.top

[C02] 默认参数
来源：http://wye.bjfxy.top

Py:   def greet(name="World"): return name
来源：http://wup.xingfuxueyuan.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://hhg.dashuyun.cn

JS:   function greet(name = "World") { return name; }
来源：http://idt.mhx1999.top

TS:   function greet(name: string = "World") { return name; }
来源：http://qrg.haohaochexian.top

Java: // 无默认参数：方法重载或 Optional
来源：http://iew.chenzaomai.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ypk.fehbvm.com

Ruby: def greet(name = "World") = name
来源：http://uqf.xylfe.cn

C#:   string Greet(string name = "World") => name;
来源：http://wbf.guannengcc.top

[C03] 可变参数
来源：http://hgy.shzxlz.cn

Py:   def total(*args): return sum(args)
来源：http://hkl.gaohongyu789.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://tzd.meibo888.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://dek.0kj1m.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ver.quarkkingdee.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://coo.snrcjt.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://szn.yfazqb.com

Ruby: def total(*nums); nums.sum; end
来源：http://zde.zhixingplan.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://lfh.ydzc1.top

[C04] 命名参数 / 关键字参数
来源：http://kgm.chenjidiqi.icu

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ddj.yueranfly.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://gls.xziqi.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://jpi.aibaodan.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://vnh.yvedp.cn

Java: // 无：用 Builder 模式或 record
来源：http://jpy.havefunace.top

Go:   // 无：用配置结构体参数
来源：http://gid.shanyushiyangkeji.top

Ruby: f(a: 1, b: 2)
来源：http://kem.shanyushiyangtech.top

C#:   f(a: 1, b: 2)
来源：http://zxo.hesvh.cn

[C05] 返回多个值
来源：http://nwx.hnqzz.top

Py:   return a, b
来源：http://nxh.ybcxt.top

PHP:  return [$a, $b];
来源：http://vpw.yonumen.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://hkp.jinqigfzy.top

TS:   return { a, b };
来源：http://ttj.xuanzx.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://nqj.dashuyun.cn

Go:   return a, b
来源：http://ucm.316326.xyz

Ruby: return a, b
来源：http://wmn.zdqjudy.top

C#:   return (a, b);              // ValueTuple
来源：http://yrp.sysykeji.top

[C06] 匿名函数 / lambda
来源：http://iln.nanxinkj.top

Py:   square = lambda x: x * x
来源：http://mua.cdnleiting.top

PHP:  $square = fn($x) => $x * $x;
来源：http://csd.mhx1999.top

JS:   const square = x => x * x;
来源：http://bxd.yanxiufei.cn

TS:   const square = (x: number): number => x * x;
来源：http://loi.zhoulong.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://vfq.hesvh.cn

Go:   sq := func(x int) int { return x * x }
来源：http://mjw.zhixingplan.top

Ruby: square = ->(x) { x * x }
来源：http://lbo.jinqigfzy.top

C#:   Func<int, int> square = x => x * x;
来源：http://wtr.zhongyouzk.top

[C07] 把函数作为参数传入
来源：http://zte.yangfankeji.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://vgi.sxryk.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ldn.hfpthk.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://pdd.fktsv.cn

TS:   arr.map(String)
来源：http://wjj.haohaochexian.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://sxz.uphjek.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://kwq.9152youxi.cn

Ruby: arr.map(&:upcase)
来源：http://apb.snrcjt.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://fha.nanxinkj.top

[C08] 闭包
来源：http://cjx.jiagoushi.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ojv.havefunace.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mlr.cdnleiting.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://czz.nanxuanxn.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ccs.9152youxi.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://dyc.pengpengdd.cyou

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://qtw.haohaochexian.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://glh.sweek.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://plj.0kj1m.cn

[C09] 递归
来源：http://iih.cucudq.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ura.redwolf501.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://fsi.epnwcf.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://erz.sjlbkw.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://miz.ehwqpu.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://glh.quarkkingdee.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://qff.shanyushiyangkeji.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://srz.aizwys.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://xhh.ctjpmb.com

[C10] 变量作用域
来源：http://ywb.zhengqikj.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wzh.yuanzhike.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://jwz.hongshengwenyu.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ccj.gzhubu.top

TS:   同 JS
来源：http://xxh.yj202588.top

Java: 方法内为块级作用域
来源：http://xsn.hnqzz.top

Go:   花括号块级作用域
来源：http://cbr.chenlongwang.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://fzo.zycfv.cn

C#:   块级作用域
来源：http://bbx.316326.xyz

[C11] 模块导入与导出
来源：http://sfr.yj20258.top

Py:   from module import func
来源：http://hck.shzxlz.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://gti.dashuyun.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://kzj.yongpay.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hml.zhiwuduotai.top

Java: import java.util.List;
来源：http://iui.xziqi.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://oxm.bbcook.cn

Ruby: require "json"; require_relative "./util"
来源：http://bmt.sweek.top

C#:   using System.Text;
来源：http://ozl.dashuyun.cn

[C12] 立即执行函数 IIFE
来源：http://fqq.cdnleiting.top

Py:   (lambda: print("run"))()
来源：http://fdi.sufxvd.cn

PHP:  (function () { echo "run"; })();
来源：http://dip.iojbl.cn

JS:   (() => { console.log("run"); })();
来源：http://uvq.hysaishi.cn

TS:   (() => { console.log("run"); })();
来源：http://irj.quarkkingdee.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jnh.cashguo.top

Go:   func() { fmt.Println("run") }()
来源：http://ilp.quarkkingdee.top

Ruby: -> { puts "run" }.call
来源：http://rfj.daxiang520.top

C#:   // 无 IIFE：用静态构造函数
来源：http://ghc.jinqigufen.top

[C13] 类型声明 / 类型注解
来源：http://acu.shzxlz.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://qtb.zhongyouzk.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mwk.shangyingyoupin.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://nsa.yangfankeji.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://swa.yuanzhike.top

Java: int add(int a, int b) { return a + b; }
来源：http://lpt.wangdashe.top

Go:   func add(a, b int) int
来源：http://iub.chenzaomai.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://apf.iojbl.cn

C#:   int Add(int a, int b) => a + b;
来源：http://vcq.nanxinkj.top

[C14] 泛型函数
来源：http://mbq.ybcxt.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://bmt.gogol.net.cn

PHP:  // 无泛型
来源：http://wjw.jinghuilouyu.cn

JS:   // 无泛型
来源：http://mgg.gotoacloud.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://bdf.hywenlv.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://xbn.zhaomingkeji.xyz

Go:   func First[T any](items []T) T { return items[0] }
来源：http://rcn.sysykeji.top

Ruby: # 无泛型
来源：http://ayf.chenjidiqi.icu

C#:   static T First<T>(List<T> items) => items[0];
来源：http://elt.daxiang520.top

[C15] 解构 / 展开参数
来源：http://dnc.zhongyouzk.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ibk.yj20258.top

PHP:  [$a, $b] = $pair;
来源：http://mqs.nanxinkj.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://nib.jyoumei.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wgs.chenlongwang.top

Java: // 无解构
来源：http://air.yangfankeji.com

Go:   // 无解构
来源：http://lfc.sweek.top

Ruby: a, b = pair
来源：http://bex.meibo888.top

C#:   var (a, b) = pair;
来源：http://sml.zdbjq.cn

[C16] 函数 / 方法重载
来源：http://eis.fzhhl.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://qnx.zhaomingkeji.xyz

PHP:  // 无重载
来源：http://wsl.iojbl.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://dqg.gotoacloud.top

TS:   // 用联合类型或重载签名声明
来源：http://hgf.zdqjudy.top

Java: void f(int a) {}  void f(String a) {}
来源：http://ghi.hongshengwenyu.top

Go:   // 无重载：用不同函数名
来源：http://laq.zhaomingkeji.xyz

Ruby: # 无重载：靠动态参数
来源：http://yah.vqdsnc.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://hhh.jlsjyb.cn

================================================================================
来源：http://syu.svipenyu.cn

D. 数组 / 列表 / 集合
来源：http://mdt.chenlongwang.top

================================================================================
来源：http://klr.zycfv.cn

[D01] 创建数组 / 列表
来源：http://vvw.vehdjk.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://gpj.xinyue.icu

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ebc.smart0.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://qrd.meibo888.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://tpc.vehdjk.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://pnl.uphjek.com

Go:   arr := []int{1, 2, 3}
来源：http://rfd.316326.xyz

Ruby: arr = [1, 2, 3]
来源：http://qps.kuanghao11.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hsp.fzhhl.top

[D02] 追加元素到末尾
来源：http://qqe.mhx1999.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://jld.c1oappe.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mke.fengsongda.top

JS:   arr.push(4);
来源：http://qhk.xingfuxueyuan.xyz

TS:   arr.push(4);
来源：http://lzx.fktsv.cn

Java: list.add(4);
来源：http://chf.cucudq.cn

Go:   arr = append(arr, 4)
来源：http://aij.0kj1m.cn

Ruby: arr << 4; arr.push(5)
来源：http://yxg.vqdsnc.cn

C#:   list.Add(4);
来源：http://oik.jinghuilouyu.cn

[D03] 在指定位置插入元素
来源：http://wqx.cucudq.cn

Py:   arr.insert(0, 0)
来源：http://etu.uphjek.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://flq.quarkkingdee.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://geo.andypj.xyz

TS:   arr.splice(0, 0, 0);
来源：http://dsu.jqgfzy.top

Java: list.add(0, 0);
来源：http://odk.sjlbkw.cn

Go:   arr = append([]int{0}, arr...)
来源：http://uct.nanxinkj.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://vqd.vqdsnc.cn

C#:   list.Insert(0, 0);
来源：http://qwj.ybcxt.top

[D04] 删除元素
来源：http://szy.vqdsnc.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://stx.jiagoushi.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://qdl.meibo888.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://fsr.yonumen.top

TS:   arr.splice(0, 1);
来源：http://fnd.zycfv.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://bsp.yanxiufei.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://lqd.yj20258.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://qhh.aizwys.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xoe.yfazqb.com

[D05] 访问与修改元素
来源：http://ylw.yongpay.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://jnh.0kj1m.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://tyo.yangfankeji.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://qbh.hammf.cn

TS:   arr[0]; arr.at(-1);
来源：http://qsk.shanyushiyangtech.top

Java: list.get(0); list.set(0, 9);
来源：http://xty.fehbvm.com

Go:   arr[0]; arr[0] = 9
来源：http://ctk.jinqigfzy.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://bhd.yueranfly.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://nav.yuxming.cn

[D06] 数组长度
来源：http://fls.shanyushiyangtech.top

Py:   len(arr)
来源：http://mce.tanke756.top

PHP:  count($arr);
来源：http://qow.tarul.cn

JS:   arr.length
来源：http://ucl.tarul.cn

TS:   arr.length
来源：http://hbv.yongpay.top

Java: list.size();
来源：http://egw.birdmap.top

Go:   len(arr)
来源：http://qxj.smart0.xyz

Ruby: arr.length; arr.size
来源：http://jhs.yuxming.cn

C#:   list.Count;
来源：http://olu.smart0.xyz

[D07] 切片 / 取子数组
来源：http://axc.cheryme.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://lcu.fanxiaobao.xyz

PHP:  array_slice($arr, 1, 3);
来源：http://pup.vqdsnc.cn

JS:   arr.slice(1, 4);
来源：http://ycc.tian-w.cn

TS:   arr.slice(1, 4);
来源：http://hmf.hammf.cn

Java: list.subList(1, 4);
来源：http://zjj.ywan-chungtsiang.top

Go:   arr[1:4]
来源：http://xjo.hnqzz.top

Ruby: arr[1, 3]
来源：http://yfy.bjfxy.top

C#:   list.GetRange(1, 3);
来源：http://yea.xingfuxueyuan.xyz

[D08] 合并两个数组
来源：http://abf.yanxiufei.cn

Py:   a + b;  a.extend(b)
来源：http://mzv.fengsongda.top

PHP:  array_merge($a, $b);
来源：http://sqa.sysykeji.top

JS:   [...a, ...b];  a.concat(b);
来源：http://hok.yfazqb.com

TS:   [...a, ...b];
来源：http://pll.yongpay.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wrd.quarkkingdee.top

Go:   append(a, b...)
来源：http://swy.birdmap.top

Ruby: a + b;  a.concat(b)
来源：http://lpx.yuxming.cn

C#:   a.Concat(b).ToList()
来源：http://evq.yuxming.cn

[D09] 排序（升序）
来源：http://oan.hesvh.cn

Py:   sorted(arr);  arr.sort()
来源：http://xun.yfazqb.com

PHP:  sort($arr);
来源：http://rba.zycfv.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://zxq.daria6918.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://pyy.gotoacloud.top

Java: Collections.sort(list);  list.sort(null);
来源：http://rzz.fanxiaobao.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mrd.yongpay.top

Ruby: arr.sort
来源：http://hgf.jinqigufen.top

C#:   list.Sort();
来源：http://tze.aizwys.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://xxn.zhoulong.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hqn.mhx1999.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ckf.pengpengdd.cyou

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ygo.jqgufenzy.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://lmq.gotoacloud.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hgt.xingfuxueyuan.xyz

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mzf.kuanghao11.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://qsv.jqgfzy.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wvk.tianlin.xyz

[D11] 反转数组
来源：http://pyt.c1oappe.top

Py:   arr[::-1];  arr.reverse()
来源：http://ovg.sufxvd.cn

PHP:  array_reverse($arr);
来源：http://eqn.xziqi.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://yfj.jianghu66.top

TS:   [...arr].reverse();
来源：http://qnv.ivvv.top

Java: Collections.reverse(list);
来源：http://tyi.ywan-chungtsiang.top

Go:   slices.Reverse(arr)
来源：http://epx.aizwys.cn

Ruby: arr.reverse
来源：http://dom.jinyuanbaomall.cn

C#:   list.Reverse();
来源：http://gnn.feifeiyinyue.top

[D12] 查找元素下标
来源：http://qvw.316326.xyz

Py:   arr.index(x);  x in arr
来源：http://lkv.nwbrower.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://alc.kuanghao11.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://czv.shanyushiyangkeji.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vwh.pycfn.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://dpu.dianchejie.cn

Go:   slices.Index(arr, x)
来源：http://tpw.yj20258.top

Ruby: arr.index(x)
来源：http://wwo.yj20258.top

C#:   list.IndexOf(x);
来源：http://kem.jiagoushi.top

[D13] 过滤（保留满足条件的）
来源：http://sao.fehbvm.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qyw.yj202588.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://jhb.zycfv.cn

JS:   arr.filter(x => x > 3)
来源：http://kso.ywan-chungtsiang.top

TS:   arr.filter(x => x > 3)
来源：http://gqy.tianlin.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ykk.sxryk.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://zlc.jianghu66.top

Ruby: arr.select { |x| x > 3 }
来源：http://ikd.feifeiyinyue.top

C#:   list.Where(x => x > 3).ToList()
来源：http://sar.yuxming.cn

[D14] 映射转换（每个元素变形）
来源：http://qrp.fzhhl.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ksg.yj20258.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zjt.daria6918.cn

JS:   arr.map(x => x * 2)
来源：http://pog.gzhubu.top

TS:   arr.map(x => x * 2)
来源：http://wwv.yanxiufei.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://wwb.xinyue.icu

Go:   // 手写循环
来源：http://gux.jinghuilouyu.cn

Ruby: arr.map { |x| x * 2 }
来源：http://tac.guowangkeji.top

C#:   list.Select(x => x * 2).ToList()
来源：http://ztb.iojbl.cn

[D15] 去重
来源：http://dze.zhoulong.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://pbf.sjlbkw.cn

PHP:  array_unique($arr);
来源：http://zwx.uphjek.com

JS:   [...new Set(arr)]
来源：http://ejg.cucudq.cn

TS:   [...new Set(arr)]
来源：http://cot.pengpengdd.cyou

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://frk.hcnkem.com

Go:   // 用 map[T]struct{} 手写
来源：http://ncs.hesvh.cn

Ruby: arr.uniq
来源：http://pdn.nanxinkj.top

C#:   list.Distinct().ToList()
来源：http://hyy.tanke756.top

[D16] 求和与平均值
来源：http://gio.yueranfly.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://xva.snrcjt.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://yha.zhaomingkeji.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://xrd.jlsjyb.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://bna.hammf.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://nqv.zycfv.cn

Go:   // 手写循环累加
来源：http://wmf.xziqi.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://kxg.zhaomingkeji.xyz

C#:   list.Sum();  list.Average()
来源：http://acs.cashguo.top

[D17] 最大值与最小值
来源：http://rqn.nwbrower.top

Py:   max(arr);  min(arr)
来源：http://koh.haohaochexian.top

PHP:  max($arr);  min($arr);
来源：http://jjb.hammf.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://xzc.cqqwz.cn

TS:   Math.max(...arr);
来源：http://xur.sufxvd.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://jmp.bjfxy.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://fxj.shzxlz.cn

Ruby: arr.max;  arr.min
来源：http://uqu.zhengqikj.top

C#:   list.Max();  list.Min()
来源：http://wru.gaohongyu789.top

[D18] 扁平化嵌套数组
来源：http://fli.wangdashe.top


<!-- 参考信息 -->