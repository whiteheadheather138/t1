代发 wailian999

Java: if (data == null) return;
来源：http://xeo.sufxvd.cn

Go:   if data == nil { return }
来源：http://tnv.zhongyouzk.top

Ruby: return if data.nil?
来源：http://sgq.epnwcf.com

C#:   if (data == null) return;
来源：http://zzf.wangdashe.top

================================================================================
来源：http://hun.pengpengdd.cyou

C. 函数与作用域
来源：http://dyc.cdnleiting.top

================================================================================
来源：http://yip.c1oappe.top

[C01] 定义函数
来源：http://fso.shangyingyoupin.top

Py:   def add(a, b): return a + b
来源：http://yiq.9152youxi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gyh.fehbvm.com

JS:   function add(a, b) { return a + b; }
来源：http://qum.sjlbkw.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://czu.pycfn.com

Java: static int add(int a, int b) { return a + b; }
来源：http://usf.chenlongwang.top

Go:   func add(a, b int) int { return a + b }
来源：http://pie.zdqjudy.top

Ruby: def add(a, b); a + b; end
来源：http://euf.jiagoushi.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://kkw.xingfuxueyuan.xyz

[C02] 默认参数
来源：http://wfs.fktsv.cn

Py:   def greet(name="World"): return name
来源：http://vlm.nanxuanxn.top

PHP:  function greet($name = "World") { return $name; }
来源：http://lry.chenlongwang.top

JS:   function greet(name = "World") { return name; }
来源：http://thc.xuetiantiany.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ibm.hammf.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://wjb.nanxinkj.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ipu.gaohongyu789.top

Ruby: def greet(name = "World") = name
来源：http://vdg.yvedp.cn

C#:   string Greet(string name = "World") => name;
来源：http://hio.zdqjudy.top

[C03] 可变参数
来源：http://slj.yj202588.top

Py:   def total(*args): return sum(args)
来源：http://efw.xingfuxueyuan.xyz

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wvd.wangdashe.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://bva.dianchejie.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wph.xingfuxueyuan.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://lvw.shzxlz.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wro.gzhubu.top

Ruby: def total(*nums); nums.sum; end
来源：http://htt.xuetiantiany.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://pph.cqqwz.cn

[C04] 命名参数 / 关键字参数
来源：http://geh.sufxvd.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://lua.chenlongwang.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://qml.chenlongwang.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://brb.xinyue.icu

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mhg.jinghuilouyu.cn

Java: // 无：用 Builder 模式或 record
来源：http://eqe.chenlongwang.top

Go:   // 无：用配置结构体参数
来源：http://kim.gaohongyu789.top

Ruby: f(a: 1, b: 2)
来源：http://bft.shzxlz.cn

C#:   f(a: 1, b: 2)
来源：http://iyp.chenlongwang.top

[C05] 返回多个值
来源：http://fhf.tianlin.xyz

Py:   return a, b
来源：http://juy.havefunace.top

PHP:  return [$a, $b];
来源：http://fnf.yj202588.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://lnd.jinyuanbaomall.cn

TS:   return { a, b };
来源：http://spy.tanke756.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://jvv.shanyushiyangtech.top

Go:   return a, b
来源：http://esg.shuidangran.top

Ruby: return a, b
来源：http://lgx.xingfuxueyuan.xyz

C#:   return (a, b);              // ValueTuple
来源：http://tit.jinqigufen.top

[C06] 匿名函数 / lambda
来源：http://lyh.jinqigufen.top

Py:   square = lambda x: x * x
来源：http://kgo.chenzaomai.com

PHP:  $square = fn($x) => $x * $x;
来源：http://ivz.birdmap.top

JS:   const square = x => x * x;
来源：http://jud.fktsv.cn

TS:   const square = (x: number): number => x * x;
来源：http://njp.zhiwuduotai.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://rlr.zhaomingkeji.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://crp.yonumen.top

Ruby: square = ->(x) { x * x }
来源：http://sib.mhx1999.top

C#:   Func<int, int> square = x => x * x;
来源：http://mow.chenlongwang.top

[C07] 把函数作为参数传入
来源：http://syw.ydjk.org.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://vmd.jlsjyb.cn

PHP:  array_map("strtoupper", $arr);
来源：http://tkq.ywan-chungtsiang.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ruv.ehwqpu.com

TS:   arr.map(String)
来源：http://hzk.zhengqikj.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://fea.guannengcc.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mkc.dianchejie.cn

Ruby: arr.map(&:upcase)
来源：http://kur.xuetiantiany.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://kha.yj20258888.top

[C08] 闭包
来源：http://ocl.jiagoushi.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://syk.zhijiandao.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://buo.nanxinkj.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mtp.aizwys.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://zkb.quarkkingdee.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://kqg.cashguo.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://dej.andypj.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://kmp.0kj1m.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ats.zhongyouzk.top

[C09] 递归
来源：http://hxq.redwolf501.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://bzf.cashguo.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://igf.mhx1999.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kkv.zhengqikj.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fok.hysaishi.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://msz.gzhubu.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ovy.sufxvd.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://dia.redwolf501.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://fdo.xingfuxueyuan.xyz

[C10] 变量作用域
来源：http://nzh.epnwcf.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mgs.zhijiandao.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://myz.hesvh.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://tej.pycfn.com

TS:   同 JS
来源：http://zby.sysykeji.top

Java: 方法内为块级作用域
来源：http://vsn.tarul.cn

Go:   花括号块级作用域
来源：http://hbi.zhaomingkeji.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ieb.jyoumei.cn

C#:   块级作用域
来源：http://ryw.vehdjk.com

[C11] 模块导入与导出
来源：http://ffl.sweek.top

Py:   from module import func
来源：http://swd.havefunace.top

PHP:  require "file.php";  或 use App\Service;
来源：http://mgk.zhiwuduotai.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://adw.hywenlv.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xff.yuxming.cn

Java: import java.util.List;
来源：http://zhe.gzhubu.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hry.zhixingplan.top

Ruby: require "json"; require_relative "./util"
来源：http://xtr.jinqigufen.top

C#:   using System.Text;
来源：http://owo.jlsjyb.cn

[C12] 立即执行函数 IIFE
来源：http://zsl.xuanzx.com

Py:   (lambda: print("run"))()
来源：http://uyx.zhiwuduotai.top

PHP:  (function () { echo "run"; })();
来源：http://wwm.sxryk.cn

JS:   (() => { console.log("run"); })();
来源：http://eaw.zhixingplan.top

TS:   (() => { console.log("run"); })();
来源：http://zju.fktsv.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ayv.cdnleiting.top

Go:   func() { fmt.Println("run") }()
来源：http://pxx.daxiang520.top

Ruby: -> { puts "run" }.call
来源：http://evc.zhengqikj.top

C#:   // 无 IIFE：用静态构造函数
来源：http://okm.jinqigufen.top

[C13] 类型声明 / 类型注解
来源：http://ppt.ppjwa.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://bpu.xziqi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zwu.ydzc1.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://obp.xinyue.icu

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hbe.epnwcf.com

Java: int add(int a, int b) { return a + b; }
来源：http://jon.guannengcc.top

Go:   func add(a, b int) int
来源：http://tbd.feifeiyinyue.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://znv.sweek.top

C#:   int Add(int a, int b) => a + b;
来源：http://mym.zhengqikj.top

[C14] 泛型函数
来源：http://rjj.zhongyouzk.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://eih.ydjk.org.cn

PHP:  // 无泛型
来源：http://bex.yuxming.cn

JS:   // 无泛型
来源：http://pow.yueranfly.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://zes.sweek.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://cmk.nwbrower.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://aap.316326.xyz

Ruby: # 无泛型
来源：http://wvh.jqgufenzy.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://imw.hammf.cn

[C15] 解构 / 展开参数
来源：http://kii.gogol.net.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://gkt.yueranfly.top

PHP:  [$a, $b] = $pair;
来源：http://ito.guannengcc.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://dfl.hywenlv.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://nqq.nwbrower.top

Java: // 无解构
来源：http://lzq.xinyue.icu

Go:   // 无解构
来源：http://grp.zhaomingkeji.xyz

Ruby: a, b = pair
来源：http://kdt.pycfn.com

C#:   var (a, b) = pair;
来源：http://rza.bbcook.cn

[C16] 函数 / 方法重载
来源：http://xde.tarul.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ibd.nanxuanxn.top

PHP:  // 无重载
来源：http://glf.feifeiyinyue.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://ctm.c1oappe.top

TS:   // 用联合类型或重载签名声明
来源：http://jbs.dianchejie.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://nwe.jqgufenzy.top

Go:   // 无重载：用不同函数名
来源：http://nbp.yfazqb.com

Ruby: # 无重载：靠动态参数
来源：http://qyf.cashguo.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://oqi.gzhubu.top

================================================================================
来源：http://hdh.ivvv.top

D. 数组 / 列表 / 集合
来源：http://wsa.zhaomingkeji.xyz

================================================================================
来源：http://ivm.ybcxt.top

[D01] 创建数组 / 列表
来源：http://zwu.hfpthk.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ncp.pengpengdd.cyou

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://qzh.tianlin.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://end.9152youxi.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ccu.ctjpmb.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://nrh.wangshuangyany.cn

Go:   arr := []int{1, 2, 3}
来源：http://kaa.shanyushiyangtech.top

Ruby: arr = [1, 2, 3]
来源：http://mny.jinghuilouyu.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://tsb.hfpthk.cn

[D02] 追加元素到末尾
来源：http://ncw.yj20258.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mbc.epnwcf.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://trh.jinqigufen.top

JS:   arr.push(4);
来源：http://mii.tianlin.xyz

TS:   arr.push(4);
来源：http://pit.cucudq.cn

Java: list.add(4);
来源：http://zmj.xuanzx.com

Go:   arr = append(arr, 4)
来源：http://iqn.fzhhl.top

Ruby: arr << 4; arr.push(5)
来源：http://lyy.haohaochexian.top

C#:   list.Add(4);
来源：http://ton.guannengcc.top

[D03] 在指定位置插入元素
来源：http://peq.dashuyun.cn

Py:   arr.insert(0, 0)
来源：http://geo.svipenyu.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://tip.chenjidiqi.icu

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://cyz.zhixingplan.top

TS:   arr.splice(0, 0, 0);
来源：http://jfc.bjfxy.top

Java: list.add(0, 0);
来源：http://bfw.yonumen.top

Go:   arr = append([]int{0}, arr...)
来源：http://wgv.yangfankeji.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ltx.ydjk.org.cn

C#:   list.Insert(0, 0);
来源：http://tex.ybcxt.top

[D04] 删除元素
来源：http://xee.sxryk.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://adq.zhaomingkeji.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://zfd.zycfv.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://zbn.yj20258888.top

TS:   arr.splice(0, 1);
来源：http://uxw.hesvh.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hxu.zhaomingkeji.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://uzt.guannengcc.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://dal.zhoulong.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://zyy.fehbvm.com

[D05] 访问与修改元素
来源：http://gzk.meibo888.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://nkz.tianlin.xyz

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://dbn.dianchejie.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://xqk.jinqigfzy.top

TS:   arr[0]; arr.at(-1);
来源：http://mdd.cheryme.top

Java: list.get(0); list.set(0, 9);
来源：http://xvu.316326.xyz

Go:   arr[0]; arr[0] = 9
来源：http://mdh.ydjk.org.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://enp.fktsv.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ali.gaohongyu789.top

[D06] 数组长度
来源：http://uyt.pengpengdd.cyou

Py:   len(arr)
来源：http://lso.gaohongyu789.top

PHP:  count($arr);
来源：http://cnm.bbcook.cn

JS:   arr.length
来源：http://brt.fanxiaobao.xyz

TS:   arr.length
来源：http://ulc.snrcjt.cn

Java: list.size();
来源：http://lqw.sysykeji.top

Go:   len(arr)
来源：http://mgy.epnwcf.com

Ruby: arr.length; arr.size
来源：http://fhv.cqqwz.cn

C#:   list.Count;
来源：http://nyc.aizwys.cn

[D07] 切片 / 取子数组
来源：http://jub.chenlongwang.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wba.jlsjyb.cn

PHP:  array_slice($arr, 1, 3);
来源：http://dhb.sysykeji.top

JS:   arr.slice(1, 4);
来源：http://ubu.c1oappe.top

TS:   arr.slice(1, 4);
来源：http://prh.jqgufenzy.top

Java: list.subList(1, 4);
来源：http://kil.jinqigufen.top

Go:   arr[1:4]
来源：http://zmm.zhixingplan.top

Ruby: arr[1, 3]
来源：http://yzk.xuetiantiany.cn

C#:   list.GetRange(1, 3);
来源：http://dsw.shangyingyoupin.top

[D08] 合并两个数组
来源：http://bma.meibo888.top

Py:   a + b;  a.extend(b)
来源：http://bce.andypj.xyz

PHP:  array_merge($a, $b);
来源：http://mal.vehdjk.com

JS:   [...a, ...b];  a.concat(b);
来源：http://nmt.zhongyouzk.top

TS:   [...a, ...b];
来源：http://wvn.ivvv.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://xak.xuanzx.com

Go:   append(a, b...)
来源：http://kik.dianchejie.cn

Ruby: a + b;  a.concat(b)
来源：http://eow.fanxiaobao.xyz

C#:   a.Concat(b).ToList()
来源：http://zoz.jianghu66.top

[D09] 排序（升序）
来源：http://lhq.zhongyouzk.top

Py:   sorted(arr);  arr.sort()
来源：http://ojw.guowangkeji.top

PHP:  sort($arr);
来源：http://njk.c1oappe.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://sud.fengsongda.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://ssq.vehdjk.com

Java: Collections.sort(list);  list.sort(null);
来源：http://suq.jqgfzy.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://pvj.hnxiangtu.top

Ruby: arr.sort
来源：http://oua.bbcook.cn

C#:   list.Sort();
来源：http://gww.fktsv.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ckz.tarul.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ynl.hcnkem.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ojs.ydjk.org.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hha.jinqigufen.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://vpp.fehbvm.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://lpw.yangfankeji.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wif.yongpay.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wmz.aibaodan.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://xre.meibo888.top

[D11] 反转数组
来源：http://whj.epnwcf.com

Py:   arr[::-1];  arr.reverse()
来源：http://rtd.cdnleiting.top

PHP:  array_reverse($arr);
来源：http://wxj.cucudq.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://djv.jyoumei.cn

TS:   [...arr].reverse();
来源：http://pcj.feifeiyinyue.top

Java: Collections.reverse(list);
来源：http://emw.nwbrower.top

Go:   slices.Reverse(arr)
来源：http://zao.sufxvd.cn

Ruby: arr.reverse
来源：http://cos.shuidangran.top

C#:   list.Reverse();
来源：http://pus.bjfxy.top

[D12] 查找元素下标
来源：http://rea.mhx1999.top

Py:   arr.index(x);  x in arr
来源：http://rbs.ybcxt.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://gzj.jlsjyb.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://osm.mhx1999.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://uhz.ppjwa.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://giq.fengsongda.top

Go:   slices.Index(arr, x)
来源：http://ffp.316326.xyz

Ruby: arr.index(x)
来源：http://jkk.meibo888.top

C#:   list.IndexOf(x);
来源：http://hdo.zhoulong.xyz

[D13] 过滤（保留满足条件的）
来源：http://loy.jianghu66.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://kyy.shuidangran.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://flh.meibo888.top

JS:   arr.filter(x => x > 3)
来源：http://zek.yuanzhike.top

TS:   arr.filter(x => x > 3)
来源：http://aon.zhengqikj.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://xed.tarul.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://iaz.yongpay.top

Ruby: arr.select { |x| x > 3 }
来源：http://vke.vehdjk.com

C#:   list.Where(x => x > 3).ToList()
来源：http://jbj.gaohongyu789.top

[D14] 映射转换（每个元素变形）
来源：http://nnl.daria6918.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://gam.hysaishi.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://esp.vqdsnc.cn

JS:   arr.map(x => x * 2)
来源：http://yig.quarkkingdee.top

TS:   arr.map(x => x * 2)
来源：http://tnl.ydjk.org.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://mxf.yj20258888.top

Go:   // 手写循环
来源：http://suj.shzxlz.cn

Ruby: arr.map { |x| x * 2 }
来源：http://atl.jinqigfzy.top

C#:   list.Select(x => x * 2).ToList()
来源：http://svw.meibo888.top

[D15] 去重
来源：http://rno.gaohongyu789.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://bni.cdnleiting.top

PHP:  array_unique($arr);
来源：http://wat.hysaishi.cn

JS:   [...new Set(arr)]
来源：http://bxx.shzxlz.cn

TS:   [...new Set(arr)]
来源：http://baw.zycfv.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ear.zhongyouzk.top

Go:   // 用 map[T]struct{} 手写
来源：http://ute.ywan-chungtsiang.top

Ruby: arr.uniq
来源：http://hta.jianghu66.top

C#:   list.Distinct().ToList()
来源：http://eol.snrcjt.cn

[D16] 求和与平均值
来源：http://ppg.ctjpmb.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://vds.tian-w.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://emc.cheryme.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://siz.ywan-chungtsiang.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://uxe.ivvv.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://fyz.shzxlz.cn

Go:   // 手写循环累加
来源：http://ykz.bjfxy.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://nou.shzxlz.cn

C#:   list.Sum();  list.Average()
来源：http://lzs.yj20258.top

[D17] 最大值与最小值
来源：http://pbd.svipenyu.cn

Py:   max(arr);  min(arr)
来源：http://pve.fehbvm.com


<!-- 参考信息 -->