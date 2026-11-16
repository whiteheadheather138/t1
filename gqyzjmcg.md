代发 wailian999

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://gwf.tianlin.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://qbv.tanke756.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://slc.zhengqikj.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://vme.fanxiaobao.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://wsp.zhiwuduotai.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://rvq.tianlin.xyz

[C04] 命名参数 / 关键字参数
来源：http://gru.yuxming.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hrc.shzxlz.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://osy.aibaodan.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://uag.cashguo.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://lys.gzhubu.top

Java: // 无：用 Builder 模式或 record
来源：http://oax.hnxiangtu.top

Go:   // 无：用配置结构体参数
来源：http://sfo.hnxiangtu.top

Ruby: f(a: 1, b: 2)
来源：http://lcp.bjfxy.top

C#:   f(a: 1, b: 2)
来源：http://plh.feifeiyinyue.top

[C05] 返回多个值
来源：http://hsp.yangfankeji.com

Py:   return a, b
来源：http://duc.zdqjudy.top

PHP:  return [$a, $b];
来源：http://pib.hongshengwenyu.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://hat.yuxming.cn

TS:   return { a, b };
来源：http://tpy.shzxlz.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://goo.shangyingyoupin.top

Go:   return a, b
来源：http://bni.fanxiaobao.xyz

Ruby: return a, b
来源：http://cqr.jianghu66.top

C#:   return (a, b);              // ValueTuple
来源：http://lqe.bbcook.cn

[C06] 匿名函数 / lambda
来源：http://dbi.jqgfzy.top

Py:   square = lambda x: x * x
来源：http://aix.jqgufenzy.top

PHP:  $square = fn($x) => $x * $x;
来源：http://gkh.sufxvd.cn

JS:   const square = x => x * x;
来源：http://mgo.sxryk.cn

TS:   const square = (x: number): number => x * x;
来源：http://wos.ydjk.org.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://tue.ydzc1.top

Go:   sq := func(x int) int { return x * x }
来源：http://wwn.daxiang520.top

Ruby: square = ->(x) { x * x }
来源：http://ieg.jyoumei.cn

C#:   Func<int, int> square = x => x * x;
来源：http://lnz.wangdashe.top

[C07] 把函数作为参数传入
来源：http://pgt.hammf.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://vvp.cheryme.top

PHP:  array_map("strtoupper", $arr);
来源：http://cpv.jyoumei.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://kur.ehwqpu.com

TS:   arr.map(String)
来源：http://vzy.shangyingyoupin.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://lwk.chenlongwang.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hld.52xcode.cn

Ruby: arr.map(&:upcase)
来源：http://tmy.cheryme.top

C#:   arr.Select(s => s.ToUpper())
来源：http://uok.yueranfly.top

[C08] 闭包
来源：http://enn.cucudq.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://eta.yuxming.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://xgl.ivvv.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://xtw.yfazqb.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://lmt.pycfn.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://kpc.hammf.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://lqr.shanyushiyangkeji.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://lit.ivvv.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://tsg.zhixingplan.top

[C09] 递归
来源：http://ijl.yonumen.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://dns.meibo888.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mdr.hesvh.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cyj.yj20258.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://guz.feifeiyinyue.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://xkt.xziqi.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wfu.sxryk.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://fez.ybcxt.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://fvc.ehwqpu.com

[C10] 变量作用域
来源：http://exk.jqgfzy.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://dcv.uphjek.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ovd.birdmap.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://enn.ydzc1.top

TS:   同 JS
来源：http://esb.fanxiaobao.xyz

Java: 方法内为块级作用域
来源：http://ehj.zhoulong.xyz

Go:   花括号块级作用域
来源：http://uhp.hesvh.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://syf.gzhubu.top

C#:   块级作用域
来源：http://bka.sweek.top

[C11] 模块导入与导出
来源：http://czx.jianghu66.top

Py:   from module import func
来源：http://aln.uphjek.com

PHP:  require "file.php";  或 use App\Service;
来源：http://bpv.tian-w.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://nkc.pengpengdd.cyou

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wae.ppjwa.cn

Java: import java.util.List;
来源：http://viq.yongpay.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://tqm.zhiwuduotai.top

Ruby: require "json"; require_relative "./util"
来源：http://dlf.jianghu66.top

C#:   using System.Text;
来源：http://fqy.haohaochexian.top

[C12] 立即执行函数 IIFE
来源：http://lpc.52xcode.cn

Py:   (lambda: print("run"))()
来源：http://xmy.gotoacloud.top

PHP:  (function () { echo "run"; })();
来源：http://kbw.yuanzhike.top

JS:   (() => { console.log("run"); })();
来源：http://orj.sweek.top

TS:   (() => { console.log("run"); })();
来源：http://fsj.vqdsnc.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://use.cheryme.top

Go:   func() { fmt.Println("run") }()
来源：http://cdi.9152youxi.cn

Ruby: -> { puts "run" }.call
来源：http://zuq.shangyingyoupin.top

C#:   // 无 IIFE：用静态构造函数
来源：http://ehe.xuanzx.com

[C13] 类型声明 / 类型注解
来源：http://qyb.gaohongyu789.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://dbf.jinqigufen.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jht.yvedp.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://lpx.sweek.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yiw.iojbl.cn

Java: int add(int a, int b) { return a + b; }
来源：http://fbu.shangyingyoupin.top

Go:   func add(a, b int) int
来源：http://uei.xylfe.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://jkl.zhijiandao.cn

C#:   int Add(int a, int b) => a + b;
来源：http://tov.jiagoushi.top

[C14] 泛型函数
来源：http://gya.jinqigufen.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://axe.shzxlz.cn

PHP:  // 无泛型
来源：http://rrc.uphjek.com

JS:   // 无泛型
来源：http://kmb.fzhhl.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://znl.vehdjk.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://upl.mhx1999.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://jot.kuanghao11.cn

Ruby: # 无泛型
来源：http://xho.chenjidiqi.icu

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ati.zhongyouzk.top

[C15] 解构 / 展开参数
来源：http://ppj.316326.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://txt.sufxvd.cn

PHP:  [$a, $b] = $pair;
来源：http://txo.sysykeji.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://rfy.gaohongyu789.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://lhk.chenlongwang.top

Java: // 无解构
来源：http://eur.svipenyu.cn

Go:   // 无解构
来源：http://aox.hongshengwenyu.top

Ruby: a, b = pair
来源：http://xea.jinghuilouyu.cn

C#:   var (a, b) = pair;
来源：http://tcy.fanxiaobao.xyz

[C16] 函数 / 方法重载
来源：http://rwv.sufxvd.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://pdz.xuanzx.com

PHP:  // 无重载
来源：http://usm.jiagoushi.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://uij.ydzc1.top

TS:   // 用联合类型或重载签名声明
来源：http://tuo.jinyuanbaomall.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://wrk.andypj.xyz

Go:   // 无重载：用不同函数名
来源：http://coc.jinqigufen.top

Ruby: # 无重载：靠动态参数
来源：http://zij.yonumen.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://xwx.ywan-chungtsiang.top

================================================================================
来源：http://lgw.bbcook.cn

D. 数组 / 列表 / 集合
来源：http://owv.cashguo.top

================================================================================
来源：http://tph.uphjek.com

[D01] 创建数组 / 列表
来源：http://ope.tian-w.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://trj.zhaomingkeji.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://sqf.shangyingyoupin.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ibl.nanxuanxn.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://uog.wangshuangyany.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://rmg.xylfe.cn

Go:   arr := []int{1, 2, 3}
来源：http://yxd.redwolf501.top

Ruby: arr = [1, 2, 3]
来源：http://qfi.svipenyu.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://cmq.ehwqpu.com

[D02] 追加元素到末尾
来源：http://jqp.shangyingyoupin.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://nsa.zhijiandao.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://sdl.gotoacloud.top

JS:   arr.push(4);
来源：http://ebj.yj202588.top

TS:   arr.push(4);
来源：http://jrt.9152youxi.cn

Java: list.add(4);
来源：http://aan.hongshengwenyu.top

Go:   arr = append(arr, 4)
来源：http://tpu.pengpengdd.cyou

Ruby: arr << 4; arr.push(5)
来源：http://vyg.dashuyun.cn

C#:   list.Add(4);
来源：http://kmh.vqdsnc.cn

[D03] 在指定位置插入元素
来源：http://iem.iojbl.cn

Py:   arr.insert(0, 0)
来源：http://hzx.yuanzhike.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ryt.epnwcf.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://snf.hesvh.cn

TS:   arr.splice(0, 0, 0);
来源：http://xrj.xylfe.cn

Java: list.add(0, 0);
来源：http://kss.tian-w.cn

Go:   arr = append([]int{0}, arr...)
来源：http://tnv.wangdashe.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ozy.ppjwa.cn

C#:   list.Insert(0, 0);
来源：http://zhc.vqdsnc.cn

[D04] 删除元素
来源：http://ags.sysykeji.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://fxe.xylfe.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://lzv.xuetiantiany.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://sqo.gotoacloud.top

TS:   arr.splice(0, 1);
来源：http://wpb.cucudq.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://iek.cashguo.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://kny.tarul.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://giu.pengpengdd.cyou

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://lga.52xcode.cn

[D05] 访问与修改元素
来源：http://mpk.cucudq.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://cbk.ywan-chungtsiang.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://vgi.gaohongyu789.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wzj.meibo888.top

TS:   arr[0]; arr.at(-1);
来源：http://uuf.hywenlv.cn

Java: list.get(0); list.set(0, 9);
来源：http://eqc.sysykeji.top

Go:   arr[0]; arr[0] = 9
来源：http://hfs.hammf.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ffd.nanxinkj.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://egk.gotoacloud.top

[D06] 数组长度
来源：http://tmc.ydzc1.top

Py:   len(arr)
来源：http://lon.fengsongda.top

PHP:  count($arr);
来源：http://lqi.cdnleiting.top

JS:   arr.length
来源：http://ctf.haohaochexian.top

TS:   arr.length
来源：http://vxl.shzxlz.cn

Java: list.size();
来源：http://bdw.cucudq.cn

Go:   len(arr)
来源：http://sya.yfazqb.com

Ruby: arr.length; arr.size
来源：http://yaf.jinghuilouyu.cn

C#:   list.Count;
来源：http://vbg.vqdsnc.cn

[D07] 切片 / 取子数组
来源：http://apm.chenjidiqi.icu

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ghf.xuanzx.com

PHP:  array_slice($arr, 1, 3);
来源：http://rio.52xcode.cn

JS:   arr.slice(1, 4);
来源：http://muz.shangyingyoupin.top

TS:   arr.slice(1, 4);
来源：http://mxo.0kj1m.cn

Java: list.subList(1, 4);
来源：http://kug.daxiang520.top

Go:   arr[1:4]
来源：http://pog.haohaochexian.top

Ruby: arr[1, 3]
来源：http://yre.fzhhl.top

C#:   list.GetRange(1, 3);
来源：http://fbi.pycfn.com

[D08] 合并两个数组
来源：http://qev.quarkkingdee.top

Py:   a + b;  a.extend(b)
来源：http://dvf.yongpay.top

PHP:  array_merge($a, $b);
来源：http://inp.feifeiyinyue.top

JS:   [...a, ...b];  a.concat(b);
来源：http://luq.cheryme.top

TS:   [...a, ...b];
来源：http://bho.zhongyouzk.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://xdo.nanxinkj.top

Go:   append(a, b...)
来源：http://top.zhixingplan.top

Ruby: a + b;  a.concat(b)
来源：http://ykt.quarkkingdee.top

C#:   a.Concat(b).ToList()
来源：http://uvj.jinqigufen.top

[D09] 排序（升序）
来源：http://gmj.dashuyun.cn

Py:   sorted(arr);  arr.sort()
来源：http://bac.yj202588.top

PHP:  sort($arr);
来源：http://utc.yfazqb.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://zme.xziqi.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://wed.fzhhl.top

Java: Collections.sort(list);  list.sort(null);
来源：http://dto.ydzc1.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://lqz.dashuyun.cn

Ruby: arr.sort
来源：http://yan.yj202588.top

C#:   list.Sort();
来源：http://fvc.hysaishi.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ram.feifeiyinyue.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://zow.chenlongwang.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yxw.jinghuilouyu.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://atc.xziqi.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fvy.yuxming.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://jrk.guannengcc.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://vax.9152youxi.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://toc.xingfuxueyuan.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ojv.shanyushiyangtech.top

[D11] 反转数组
来源：http://bbq.jiagoushi.top

Py:   arr[::-1];  arr.reverse()
来源：http://pls.smart0.xyz

PHP:  array_reverse($arr);
来源：http://kbh.shuidangran.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mjr.sweek.top

TS:   [...arr].reverse();
来源：http://wvz.zhoulong.xyz

Java: Collections.reverse(list);
来源：http://inw.dashuyun.cn

Go:   slices.Reverse(arr)
来源：http://zpr.ivvv.top

Ruby: arr.reverse
来源：http://cei.hesvh.cn

C#:   list.Reverse();
来源：http://ekg.zdqjudy.top

[D12] 查找元素下标
来源：http://wlq.jinqigfzy.top

Py:   arr.index(x);  x in arr
来源：http://ogp.jinyuanbaomall.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://exo.zhijiandao.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gfc.snrcjt.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gdx.snrcjt.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ssp.yuxming.cn

Go:   slices.Index(arr, x)
来源：http://ird.hysaishi.cn

Ruby: arr.index(x)
来源：http://yxq.vqdsnc.cn

C#:   list.IndexOf(x);
来源：http://yyf.zhixingplan.top

[D13] 过滤（保留满足条件的）
来源：http://mai.0kj1m.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://kbp.hysaishi.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://yyc.zhaomingkeji.xyz

JS:   arr.filter(x => x > 3)
来源：http://qrr.yj20258888.top

TS:   arr.filter(x => x > 3)
来源：http://ytq.jyoumei.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://atn.guowangkeji.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://vba.yuanzhike.top

Ruby: arr.select { |x| x > 3 }
来源：http://dpv.yfazqb.com

C#:   list.Where(x => x > 3).ToList()
来源：http://cjk.sysykeji.top

[D14] 映射转换（每个元素变形）
来源：http://rjb.zhaomingkeji.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://bnj.shzxlz.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://akd.iojbl.cn

JS:   arr.map(x => x * 2)
来源：http://kyn.ydzc1.top

TS:   arr.map(x => x * 2)
来源：http://wjl.zdqjudy.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://rss.zhongyouzk.top

Go:   // 手写循环
来源：http://dsm.uphjek.com

Ruby: arr.map { |x| x * 2 }
来源：http://ltt.guannengcc.top

C#:   list.Select(x => x * 2).ToList()
来源：http://wup.chenzaomai.com

[D15] 去重
来源：http://qtu.ybcxt.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hqp.chenjidiqi.icu

PHP:  array_unique($arr);
来源：http://aqz.jinghuilouyu.cn

JS:   [...new Set(arr)]
来源：http://sec.yj20258.top

TS:   [...new Set(arr)]
来源：http://gww.guowangkeji.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://uok.nanxinkj.top

Go:   // 用 map[T]struct{} 手写
来源：http://zrq.hesvh.cn

Ruby: arr.uniq
来源：http://ktr.smart0.xyz

C#:   list.Distinct().ToList()
来源：http://yzo.zhengqikj.top

[D16] 求和与平均值
来源：http://dqc.yuanzhike.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://chq.redwolf501.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qeu.tian-w.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://gfh.yuxming.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://cll.sysykeji.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://byw.fktsv.cn

Go:   // 手写循环累加
来源：http://piv.aizwys.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://otu.cashguo.top

C#:   list.Sum();  list.Average()
来源：http://xcq.yonumen.top

[D17] 最大值与最小值
来源：http://bje.chenlongwang.top

Py:   max(arr);  min(arr)
来源：http://fbu.jinyuanbaomall.cn

PHP:  max($arr);  min($arr);
来源：http://hpz.daria6918.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://dxu.yangfankeji.com

TS:   Math.max(...arr);
来源：http://cnl.zhixingplan.top

Java: Collections.max(list);  Collections.min(list);
来源：http://hlr.yuanzhike.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://chz.jinyuanbaomall.cn

Ruby: arr.max;  arr.min
来源：http://jew.ivvv.top

C#:   list.Max();  list.Min()
来源：http://wfe.ctjpmb.com

[D18] 扁平化嵌套数组
来源：http://nle.hnqzz.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://muh.havefunace.top

PHP:  array_merge(...$nested);
来源：http://vsq.aibaodan.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://tbw.hesvh.cn

TS:   nested.flat();
来源：http://hev.shanyushiyangtech.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://yao.zhongyouzk.top

Go:   // 手写双层循环
来源：http://ixl.hongshengwenyu.top

Ruby: nested.flatten
来源：http://kqd.haohaochexian.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://jdl.xuanzx.com

[D19] 按字段分组
来源：http://jch.redwolf501.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://uaf.nanxuanxn.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://udi.zhongyouzk.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://cpl.cqqwz.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://igm.fzhhl.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://gop.aibaodan.cn

Go:   // 手写 map[string][]T
来源：http://bkh.havefunace.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://dqk.yongpay.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://fur.sysykeji.top

[D20] 统计每个元素出现次数
来源：http://tiw.daria6918.cn

Py:   Counter(arr)
来源：http://bwo.quarkkingdee.top

PHP:  array_count_values($arr);
来源：http://lbw.shuidangran.top


<!-- 参考信息 -->