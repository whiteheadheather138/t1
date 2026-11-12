代发 wailian999

Py:   return a, b
来源：http://xwt.uphjek.com

PHP:  return [$a, $b];
来源：http://ltr.xingfuxueyuan.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://lcw.havefunace.top

TS:   return { a, b };
来源：http://dil.jqgufenzy.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://yts.ivvv.top

Go:   return a, b
来源：http://xen.jiagoushi.top

Ruby: return a, b
来源：http://col.nwbrower.top

C#:   return (a, b);              // ValueTuple
来源：http://jho.yj20258.top

[C06] 匿名函数 / lambda
来源：http://meu.yangfankeji.com

Py:   square = lambda x: x * x
来源：http://msw.ydjk.org.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://bzg.fanxiaobao.xyz

JS:   const square = x => x * x;
来源：http://rli.yj202588.top

TS:   const square = (x: number): number => x * x;
来源：http://ooa.ydzc1.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://zyi.xingfuxueyuan.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://tmf.shuidangran.top

Ruby: square = ->(x) { x * x }
来源：http://imw.shzxlz.cn

C#:   Func<int, int> square = x => x * x;
来源：http://qek.shanyushiyangkeji.top

[C07] 把函数作为参数传入
来源：http://cfc.tarul.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://njm.zhongyouzk.top

PHP:  array_map("strtoupper", $arr);
来源：http://gxl.jinqigufen.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://fsk.mhx1999.top

TS:   arr.map(String)
来源：http://ydk.guannengcc.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ueh.gotoacloud.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://gns.quarkkingdee.top

Ruby: arr.map(&:upcase)
来源：http://pvt.chenzaomai.com

C#:   arr.Select(s => s.ToUpper())
来源：http://nej.zycfv.cn

[C08] 闭包
来源：http://rdi.cheryme.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://aey.9152youxi.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://myj.daria6918.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://xdb.xinyue.icu

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://oeb.chenjidiqi.icu

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://jyf.kuanghao11.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://emx.xingfuxueyuan.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://rlp.zdqjudy.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://lzz.andypj.xyz

[C09] 递归
来源：http://giw.dianchejie.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://bro.yuanzhike.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wty.zhengqikj.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rhu.cdnleiting.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yar.fengsongda.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://dwj.xylfe.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://jue.yanxiufei.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://cjv.yfazqb.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://kdw.xingfuxueyuan.xyz

[C10] 变量作用域
来源：http://lnu.meibo888.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://sxc.xuetiantiany.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://qpt.uphjek.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://gnt.sysykeji.top

TS:   同 JS
来源：http://rxf.nanxinkj.top

Java: 方法内为块级作用域
来源：http://gex.sysykeji.top

Go:   花括号块级作用域
来源：http://str.xinyue.icu

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://npl.yfazqb.com

C#:   块级作用域
来源：http://gqd.zhixingplan.top

[C11] 模块导入与导出
来源：http://axj.hcnkem.com

Py:   from module import func
来源：http://vgj.hcnkem.com

PHP:  require "file.php";  或 use App\Service;
来源：http://vqc.jinqigufen.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://syz.gzhubu.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://fvt.cucudq.cn

Java: import java.util.List;
来源：http://ieo.jlsjyb.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://rwx.hnxiangtu.top

Ruby: require "json"; require_relative "./util"
来源：http://kbj.hongshengwenyu.top

C#:   using System.Text;
来源：http://qdu.chenzaomai.com

[C12] 立即执行函数 IIFE
来源：http://umx.xinyue.icu

Py:   (lambda: print("run"))()
来源：http://xzx.hnqzz.top

PHP:  (function () { echo "run"; })();
来源：http://toi.cqqwz.cn

JS:   (() => { console.log("run"); })();
来源：http://fdv.sufxvd.cn

TS:   (() => { console.log("run"); })();
来源：http://fvg.zdbjq.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://rlk.daxiang520.top

Go:   func() { fmt.Println("run") }()
来源：http://ikx.yj20258.top

Ruby: -> { puts "run" }.call
来源：http://guo.zhaomingkeji.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://rlo.ehwqpu.com

[C13] 类型声明 / 类型注解
来源：http://pxo.xylfe.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://cbs.zycfv.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mhm.cdnleiting.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://fvk.jqgfzy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tjq.zhijiandao.cn

Java: int add(int a, int b) { return a + b; }
来源：http://acu.zhixingplan.top

Go:   func add(a, b int) int
来源：http://fzt.hywenlv.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://qje.aibaodan.cn

C#:   int Add(int a, int b) => a + b;
来源：http://wvb.52xcode.cn

[C14] 泛型函数
来源：http://yoq.jyoumei.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zxf.haohaochexian.top

PHP:  // 无泛型
来源：http://ekt.316326.xyz

JS:   // 无泛型
来源：http://tfq.daria6918.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hxf.fengsongda.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://dmk.gotoacloud.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wzh.yuxming.cn

Ruby: # 无泛型
来源：http://gbv.zycfv.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://rjp.zhixingplan.top

[C15] 解构 / 展开参数
来源：http://jjc.zhixingplan.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://cum.hysaishi.cn

PHP:  [$a, $b] = $pair;
来源：http://wbn.guannengcc.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://fur.yj20258.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wku.jiagoushi.top

Java: // 无解构
来源：http://bkv.daria6918.cn

Go:   // 无解构
来源：http://kpm.quarkkingdee.top

Ruby: a, b = pair
来源：http://res.chenlongwang.top

C#:   var (a, b) = pair;
来源：http://fsz.sxryk.cn

[C16] 函数 / 方法重载
来源：http://utg.aizwys.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ssj.bbcook.cn

PHP:  // 无重载
来源：http://lkx.aizwys.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://tld.epnwcf.com

TS:   // 用联合类型或重载签名声明
来源：http://mlh.316326.xyz

Java: void f(int a) {}  void f(String a) {}
来源：http://hvx.fanxiaobao.xyz

Go:   // 无重载：用不同函数名
来源：http://iey.andypj.xyz

Ruby: # 无重载：靠动态参数
来源：http://cxa.yuanzhike.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://kor.aibaodan.cn

================================================================================
来源：http://aov.vehdjk.com

D. 数组 / 列表 / 集合
来源：http://rww.tarul.cn

================================================================================
来源：http://jaf.cdnleiting.top

[D01] 创建数组 / 列表
来源：http://ivc.shanyushiyangtech.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://kpg.hnxiangtu.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://idi.yj20258888.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://kfd.cdnleiting.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://rzw.jianghu66.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mhx.zycfv.cn

Go:   arr := []int{1, 2, 3}
来源：http://yyw.xinyue.icu

Ruby: arr = [1, 2, 3]
来源：http://jgx.ehwqpu.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://qap.andypj.xyz

[D02] 追加元素到末尾
来源：http://pkz.guowangkeji.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://poq.hammf.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://pui.meibo888.top

JS:   arr.push(4);
来源：http://yxt.zycfv.cn

TS:   arr.push(4);
来源：http://msw.ywan-chungtsiang.top

Java: list.add(4);
来源：http://cbi.gaohongyu789.top

Go:   arr = append(arr, 4)
来源：http://piy.ctjpmb.com

Ruby: arr << 4; arr.push(5)
来源：http://let.pengpengdd.cyou

C#:   list.Add(4);
来源：http://tji.redwolf501.top

[D03] 在指定位置插入元素
来源：http://gzo.pengpengdd.cyou

Py:   arr.insert(0, 0)
来源：http://bbu.jyoumei.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://xmg.quarkkingdee.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://orb.hfpthk.cn

TS:   arr.splice(0, 0, 0);
来源：http://lxw.gaohongyu789.top

Java: list.add(0, 0);
来源：http://vgx.mhx1999.top

Go:   arr = append([]int{0}, arr...)
来源：http://qdo.nwbrower.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://gpy.fehbvm.com

C#:   list.Insert(0, 0);
来源：http://ipm.sweek.top

[D04] 删除元素
来源：http://nga.iojbl.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ukx.yonumen.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hvg.xingfuxueyuan.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://rag.cdnleiting.top

TS:   arr.splice(0, 1);
来源：http://oao.zdbjq.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://izz.birdmap.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://rhw.ehwqpu.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://qvi.guannengcc.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://eiy.sjlbkw.cn

[D05] 访问与修改元素
来源：http://htq.xuanzx.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://xfx.vqdsnc.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ovc.sweek.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://zjw.zhaomingkeji.xyz

TS:   arr[0]; arr.at(-1);
来源：http://imx.guowangkeji.top

Java: list.get(0); list.set(0, 9);
来源：http://xpc.bbcook.cn

Go:   arr[0]; arr[0] = 9
来源：http://rug.shuidangran.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ppd.yj20258888.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://xlb.52xcode.cn

[D06] 数组长度
来源：http://mbv.cheryme.top

Py:   len(arr)
来源：http://kfx.fanxiaobao.xyz

PHP:  count($arr);
来源：http://uag.uphjek.com

JS:   arr.length
来源：http://lmn.shzxlz.cn

TS:   arr.length
来源：http://yma.gotoacloud.top

Java: list.size();
来源：http://wro.shanyushiyangtech.top

Go:   len(arr)
来源：http://gue.sweek.top

Ruby: arr.length; arr.size
来源：http://ydd.dashuyun.cn

C#:   list.Count;
来源：http://owm.yj202588.top

[D07] 切片 / 取子数组
来源：http://dox.shanyushiyangtech.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://iww.fengsongda.top

PHP:  array_slice($arr, 1, 3);
来源：http://asr.yuxming.cn

JS:   arr.slice(1, 4);
来源：http://qaw.jinghuilouyu.cn

TS:   arr.slice(1, 4);
来源：http://ceh.zdbjq.cn

Java: list.subList(1, 4);
来源：http://bev.jinghuilouyu.cn

Go:   arr[1:4]
来源：http://xuh.yueranfly.top

Ruby: arr[1, 3]
来源：http://bss.chenlongwang.top

C#:   list.GetRange(1, 3);
来源：http://awp.uphjek.com

[D08] 合并两个数组
来源：http://ibg.zhongyouzk.top

Py:   a + b;  a.extend(b)
来源：http://esb.jinqigufen.top

PHP:  array_merge($a, $b);
来源：http://zmo.meibo888.top

JS:   [...a, ...b];  a.concat(b);
来源：http://dtl.zhongyouzk.top

TS:   [...a, ...b];
来源：http://pxf.chenjidiqi.icu

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://dqp.zhengqikj.top

Go:   append(a, b...)
来源：http://pkv.tarul.cn

Ruby: a + b;  a.concat(b)
来源：http://xsk.shzxlz.cn

C#:   a.Concat(b).ToList()
来源：http://zqw.9152youxi.cn

[D09] 排序（升序）
来源：http://ahb.ybcxt.top

Py:   sorted(arr);  arr.sort()
来源：http://fsq.hnxiangtu.top

PHP:  sort($arr);
来源：http://kkl.zycfv.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://zxg.zdbjq.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://iow.yanxiufei.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ijz.xuetiantiany.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://nyn.meibo888.top

Ruby: arr.sort
来源：http://isf.cqqwz.cn

C#:   list.Sort();
来源：http://snl.fzhhl.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://bbs.jinyuanbaomall.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://oyo.xylfe.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rwc.sxryk.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://zdh.zhoulong.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://xde.jinqigufen.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://icj.tian-w.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://sjz.hysaishi.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://opw.birdmap.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://xsl.cqqwz.cn

[D11] 反转数组
来源：http://jbe.yj202588.top

Py:   arr[::-1];  arr.reverse()
来源：http://gku.hnxiangtu.top

PHP:  array_reverse($arr);
来源：http://jun.hnqzz.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vwi.kuanghao11.cn

TS:   [...arr].reverse();
来源：http://kkw.zycfv.cn

Java: Collections.reverse(list);
来源：http://lcb.bjfxy.top

Go:   slices.Reverse(arr)
来源：http://akx.ppjwa.cn

Ruby: arr.reverse
来源：http://ihp.c1oappe.top

C#:   list.Reverse();
来源：http://til.xingfuxueyuan.xyz

[D12] 查找元素下标
来源：http://hkt.hcnkem.com

Py:   arr.index(x);  x in arr
来源：http://tlq.cucudq.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://nfx.haohaochexian.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://azb.hammf.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bkp.cqqwz.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://jgx.yj20258888.top

Go:   slices.Index(arr, x)
来源：http://crx.meibo888.top

Ruby: arr.index(x)
来源：http://slt.haohaochexian.top

C#:   list.IndexOf(x);
来源：http://hjk.redwolf501.top

[D13] 过滤（保留满足条件的）
来源：http://ogd.havefunace.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://xti.quarkkingdee.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ujv.fehbvm.com

JS:   arr.filter(x => x > 3)
来源：http://iji.xziqi.cn

TS:   arr.filter(x => x > 3)
来源：http://vom.aizwys.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://dav.0kj1m.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://pez.yuxming.cn

Ruby: arr.select { |x| x > 3 }
来源：http://czu.shanyushiyangtech.top

C#:   list.Where(x => x > 3).ToList()
来源：http://vmz.guannengcc.top

[D14] 映射转换（每个元素变形）
来源：http://csb.tianlin.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mxb.ywan-chungtsiang.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hck.ywan-chungtsiang.top

JS:   arr.map(x => x * 2)
来源：http://dkk.zhijiandao.cn

TS:   arr.map(x => x * 2)
来源：http://ios.c1oappe.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://dlc.ybcxt.top

Go:   // 手写循环
来源：http://tsx.nwbrower.top

Ruby: arr.map { |x| x * 2 }
来源：http://aod.haohaochexian.top

C#:   list.Select(x => x * 2).ToList()
来源：http://guy.guowangkeji.top

[D15] 去重
来源：http://zzb.snrcjt.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ggu.sxryk.cn

PHP:  array_unique($arr);
来源：http://azx.0kj1m.cn

JS:   [...new Set(arr)]
来源：http://nbk.chenzaomai.com

TS:   [...new Set(arr)]
来源：http://jnu.yj202588.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://lxk.havefunace.top

Go:   // 用 map[T]struct{} 手写
来源：http://hoe.chenjidiqi.icu

Ruby: arr.uniq
来源：http://dmp.ctjpmb.com

C#:   list.Distinct().ToList()
来源：http://pse.vqdsnc.cn

[D16] 求和与平均值
来源：http://eem.cucudq.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ues.shuidangran.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ihc.ydzc1.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://qqi.yueranfly.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://dwa.gzhubu.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ato.zhiwuduotai.top

Go:   // 手写循环累加
来源：http://hbm.ehwqpu.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://arc.jlsjyb.cn

C#:   list.Sum();  list.Average()
来源：http://per.316326.xyz

[D17] 最大值与最小值
来源：http://ddv.zhiwuduotai.top

Py:   max(arr);  min(arr)
来源：http://wyd.uphjek.com

PHP:  max($arr);  min($arr);
来源：http://nsf.vehdjk.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://kgz.gzhubu.top

TS:   Math.max(...arr);
来源：http://azv.nanxuanxn.top

Java: Collections.max(list);  Collections.min(list);
来源：http://pae.zhoulong.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://lcq.hnqzz.top

Ruby: arr.max;  arr.min
来源：http://chy.hesvh.cn

C#:   list.Max();  list.Min()
来源：http://msz.xziqi.cn

[D18] 扁平化嵌套数组
来源：http://ggm.shzxlz.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hmu.hongshengwenyu.top

PHP:  array_merge(...$nested);
来源：http://fir.smart0.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ray.yj20258.top

TS:   nested.flat();
来源：http://uqr.pengpengdd.cyou

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jyd.ctjpmb.com

Go:   // 手写双层循环
来源：http://xpo.zdqjudy.top

Ruby: nested.flatten
来源：http://cyb.fehbvm.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://vdd.tanke756.top

[D19] 按字段分组
来源：http://cwi.dashuyun.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://crj.zdbjq.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://sra.yangfankeji.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ewf.jinqigfzy.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://gmp.hfpthk.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://sgs.aizwys.cn

Go:   // 手写 map[string][]T
来源：http://kgo.daria6918.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://cat.gotoacloud.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://eyq.hongshengwenyu.top

[D20] 统计每个元素出现次数
来源：http://wdt.shuidangran.top

Py:   Counter(arr)
来源：http://qiz.havefunace.top

PHP:  array_count_values($arr);
来源：http://hhl.gogol.net.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bry.yvedp.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jlt.ehwqpu.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://iuy.yanxiufei.cn

Go:   // 手写 map[T]int
来源：http://tqc.fanxiaobao.xyz

Ruby: arr.tally
来源：http://yvu.jyoumei.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://gfo.pycfn.com

[D21] 判断是否包含某元素
来源：http://wnh.dianchejie.cn

Py:   x in arr
来源：http://sto.svipenyu.cn

PHP:  in_array($x, $arr, true);
来源：http://isx.fktsv.cn

JS:   arr.includes(x)
来源：http://rrf.jianghu66.top

TS:   arr.includes(x)
来源：http://zjc.sxryk.cn

Java: list.contains(x)
来源：http://scq.yangfankeji.com

Go:   slices.Contains(arr, x)
来源：http://bro.xylfe.cn

Ruby: arr.include?(x)
来源：http://erk.cheryme.top

C#:   list.Contains(x)
来源：http://box.ivvv.top

[D22] 复制数组（避免共享引用）
来源：http://wzq.fanxiaobao.xyz


<!-- 参考信息 -->