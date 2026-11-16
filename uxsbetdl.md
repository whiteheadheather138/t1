代发 wailian999

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://dyc.ctjpmb.com

Go:   return a, b
来源：http://lvz.c1oappe.top

Ruby: return a, b
来源：http://ehq.316326.xyz

C#:   return (a, b);              // ValueTuple
来源：http://cov.zhengqikj.top

[C06] 匿名函数 / lambda
来源：http://vvq.chenlongwang.top

Py:   square = lambda x: x * x
来源：http://jgk.vqdsnc.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://bls.nanxuanxn.top

JS:   const square = x => x * x;
来源：http://kwa.hammf.cn

TS:   const square = (x: number): number => x * x;
来源：http://qyk.yonumen.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://jap.yangfankeji.com

Go:   sq := func(x int) int { return x * x }
来源：http://btw.bjfxy.top

Ruby: square = ->(x) { x * x }
来源：http://mio.316326.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://kfj.wangdashe.top

[C07] 把函数作为参数传入
来源：http://tzq.dashuyun.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://zto.gogol.net.cn

PHP:  array_map("strtoupper", $arr);
来源：http://aws.tian-w.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://dzl.smart0.xyz

TS:   arr.map(String)
来源：http://vvo.hnxiangtu.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://iqc.cqqwz.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wum.smart0.xyz

Ruby: arr.map(&:upcase)
来源：http://ggr.hysaishi.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://dca.guannengcc.top

[C08] 闭包
来源：http://wrw.jinghuilouyu.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://izv.chenlongwang.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://fmy.daxiang520.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://sgf.jqgfzy.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://qnw.aibaodan.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://tif.tian-w.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://fzo.tianlin.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hxw.zhiwuduotai.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ljv.ehwqpu.com

[C09] 递归
来源：http://tbp.xziqi.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hdo.wangdashe.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://tyk.yangfankeji.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rbr.sxryk.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rhz.zhengqikj.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://nbs.ydzc1.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ltb.zhaomingkeji.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://uqg.gotoacloud.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://qek.yonumen.top

[C10] 变量作用域
来源：http://fmy.zhongyouzk.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mva.pengpengdd.cyou

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://qbr.c1oappe.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://sse.zhixingplan.top

TS:   同 JS
来源：http://qqi.cheryme.top

Java: 方法内为块级作用域
来源：http://bxc.ydzc1.top

Go:   花括号块级作用域
来源：http://gfy.vehdjk.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://esl.yongpay.top

C#:   块级作用域
来源：http://cpz.jinqigfzy.top

[C11] 模块导入与导出
来源：http://ssm.tian-w.cn

Py:   from module import func
来源：http://mon.bbcook.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://bds.hcnkem.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://jpm.cdnleiting.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://yek.xuetiantiany.cn

Java: import java.util.List;
来源：http://ssf.guowangkeji.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://lje.jqgufenzy.top

Ruby: require "json"; require_relative "./util"
来源：http://jnm.ydzc1.top

C#:   using System.Text;
来源：http://qmk.cucudq.cn

[C12] 立即执行函数 IIFE
来源：http://zsc.zhongyouzk.top

Py:   (lambda: print("run"))()
来源：http://hso.yfazqb.com

PHP:  (function () { echo "run"; })();
来源：http://mkw.shanyushiyangtech.top

JS:   (() => { console.log("run"); })();
来源：http://vek.cucudq.cn

TS:   (() => { console.log("run"); })();
来源：http://odv.chenlongwang.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://qpp.c1oappe.top

Go:   func() { fmt.Println("run") }()
来源：http://car.zhijiandao.cn

Ruby: -> { puts "run" }.call
来源：http://yao.zhengqikj.top

C#:   // 无 IIFE：用静态构造函数
来源：http://nwu.andypj.xyz

[C13] 类型声明 / 类型注解
来源：http://qox.hnqzz.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://yno.aizwys.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://eli.yvedp.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://kne.ydzc1.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://szp.yonumen.top

Java: int add(int a, int b) { return a + b; }
来源：http://naa.jiagoushi.top

Go:   func add(a, b int) int
来源：http://xjo.jinqigufen.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://xvk.shanyushiyangtech.top

C#:   int Add(int a, int b) => a + b;
来源：http://pvf.shanyushiyangtech.top

[C14] 泛型函数
来源：http://tuc.vehdjk.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://qar.hnqzz.top

PHP:  // 无泛型
来源：http://sis.guannengcc.top

JS:   // 无泛型
来源：http://mjp.wangdashe.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://rmy.vqdsnc.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://eis.chenzaomai.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hmr.wangdashe.top

Ruby: # 无泛型
来源：http://agk.zhiwuduotai.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://azk.zycfv.cn

[C15] 解构 / 展开参数
来源：http://iya.chenlongwang.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ifw.hammf.cn

PHP:  [$a, $b] = $pair;
来源：http://rja.yvedp.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://gjj.jianghu66.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://syk.uphjek.com

Java: // 无解构
来源：http://ufl.yuanzhike.top

Go:   // 无解构
来源：http://yuw.guannengcc.top

Ruby: a, b = pair
来源：http://pia.xuetiantiany.cn

C#:   var (a, b) = pair;
来源：http://jfp.jlsjyb.cn

[C16] 函数 / 方法重载
来源：http://dhz.ydjk.org.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://xro.jinghuilouyu.cn

PHP:  // 无重载
来源：http://urs.fanxiaobao.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://koz.quarkkingdee.top

TS:   // 用联合类型或重载签名声明
来源：http://vxl.sweek.top

Java: void f(int a) {}  void f(String a) {}
来源：http://zvv.shzxlz.cn

Go:   // 无重载：用不同函数名
来源：http://bdt.uphjek.com

Ruby: # 无重载：靠动态参数
来源：http://jhl.shanyushiyangkeji.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://bbp.birdmap.top

================================================================================
来源：http://fif.tianlin.xyz

D. 数组 / 列表 / 集合
来源：http://ywl.yfazqb.com

================================================================================
来源：http://klj.hesvh.cn

[D01] 创建数组 / 列表
来源：http://lcq.hcnkem.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://vbv.tianlin.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://eox.xylfe.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://igj.jinghuilouyu.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://dan.gaohongyu789.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://uns.jinghuilouyu.cn

Go:   arr := []int{1, 2, 3}
来源：http://dmt.uphjek.com

Ruby: arr = [1, 2, 3]
来源：http://ylu.tarul.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://qvv.shuidangran.top

[D02] 追加元素到末尾
来源：http://jbg.yongpay.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wnt.quarkkingdee.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://xmt.zhixingplan.top

JS:   arr.push(4);
来源：http://qkl.guowangkeji.top

TS:   arr.push(4);
来源：http://sck.aibaodan.cn

Java: list.add(4);
来源：http://ivh.c1oappe.top

Go:   arr = append(arr, 4)
来源：http://cqj.tianlin.xyz

Ruby: arr << 4; arr.push(5)
来源：http://ezb.wangshuangyany.cn

C#:   list.Add(4);
来源：http://xqa.feifeiyinyue.top

[D03] 在指定位置插入元素
来源：http://gkp.chenzaomai.com

Py:   arr.insert(0, 0)
来源：http://zzc.ehwqpu.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://kbm.hnqzz.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ljk.xinyue.icu

TS:   arr.splice(0, 0, 0);
来源：http://kve.gzhubu.top

Java: list.add(0, 0);
来源：http://ufs.quarkkingdee.top

Go:   arr = append([]int{0}, arr...)
来源：http://okh.yuanzhike.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://fer.guowangkeji.top

C#:   list.Insert(0, 0);
来源：http://ahr.snrcjt.cn

[D04] 删除元素
来源：http://ycp.yj20258888.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://dwa.fzhhl.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://dnl.0kj1m.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://gok.yuxming.cn

TS:   arr.splice(0, 1);
来源：http://kaq.epnwcf.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://nub.guannengcc.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://gaa.zhijiandao.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://zgu.jiagoushi.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://iqt.ivvv.top

[D05] 访问与修改元素
来源：http://ncs.zhixingplan.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://xmf.zhixingplan.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://zsu.iojbl.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mxu.nwbrower.top

TS:   arr[0]; arr.at(-1);
来源：http://nsu.chenjidiqi.icu

Java: list.get(0); list.set(0, 9);
来源：http://drt.nanxuanxn.top

Go:   arr[0]; arr[0] = 9
来源：http://vyk.hnqzz.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hcs.meibo888.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hbs.hysaishi.cn

[D06] 数组长度
来源：http://ldl.fehbvm.com

Py:   len(arr)
来源：http://ylf.hesvh.cn

PHP:  count($arr);
来源：http://myp.hongshengwenyu.top

JS:   arr.length
来源：http://hvc.nwbrower.top

TS:   arr.length
来源：http://yqw.quarkkingdee.top

Java: list.size();
来源：http://yqs.pycfn.com

Go:   len(arr)
来源：http://cue.zhengqikj.top

Ruby: arr.length; arr.size
来源：http://dpd.cheryme.top

C#:   list.Count;
来源：http://dvn.yonumen.top

[D07] 切片 / 取子数组
来源：http://fis.ydjk.org.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wse.zhiwuduotai.top

PHP:  array_slice($arr, 1, 3);
来源：http://xnm.andypj.xyz

JS:   arr.slice(1, 4);
来源：http://mnb.nanxinkj.top

TS:   arr.slice(1, 4);
来源：http://xip.jinqigfzy.top

Java: list.subList(1, 4);
来源：http://xwj.pycfn.com

Go:   arr[1:4]
来源：http://cbc.birdmap.top

Ruby: arr[1, 3]
来源：http://qvd.meibo888.top

C#:   list.GetRange(1, 3);
来源：http://bas.tanke756.top

[D08] 合并两个数组
来源：http://uaa.cqqwz.cn

Py:   a + b;  a.extend(b)
来源：http://her.tarul.cn

PHP:  array_merge($a, $b);
来源：http://lpj.ydjk.org.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://lcj.cashguo.top

TS:   [...a, ...b];
来源：http://fxw.fengsongda.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://pky.yongpay.top

Go:   append(a, b...)
来源：http://mqx.pycfn.com

Ruby: a + b;  a.concat(b)
来源：http://cez.uphjek.com

C#:   a.Concat(b).ToList()
来源：http://amo.zhaomingkeji.xyz

[D09] 排序（升序）
来源：http://eed.hammf.cn

Py:   sorted(arr);  arr.sort()
来源：http://rio.cheryme.top

PHP:  sort($arr);
来源：http://xcv.yuanzhike.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://lko.jinyuanbaomall.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://gxq.shanyushiyangtech.top

Java: Collections.sort(list);  list.sort(null);
来源：http://dxk.yanxiufei.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wkc.yfazqb.com

Ruby: arr.sort
来源：http://wev.tanke756.top

C#:   list.Sort();
来源：http://yeg.ydzc1.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://icp.shanyushiyangtech.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://eip.sysykeji.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://oka.zhaomingkeji.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://nuv.zdbjq.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://cru.cqqwz.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hwh.epnwcf.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://sdi.nwbrower.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ppv.fehbvm.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://phw.cashguo.top

[D11] 反转数组
来源：http://cbb.hywenlv.cn

Py:   arr[::-1];  arr.reverse()
来源：http://vbe.jiagoushi.top

PHP:  array_reverse($arr);
来源：http://vzp.fengsongda.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://lxz.xylfe.cn

TS:   [...arr].reverse();
来源：http://smg.xylfe.cn

Java: Collections.reverse(list);
来源：http://wrx.jinqigfzy.top

Go:   slices.Reverse(arr)
来源：http://xml.kuanghao11.cn

Ruby: arr.reverse
来源：http://lfy.jqgufenzy.top

C#:   list.Reverse();
来源：http://ssg.cdnleiting.top

[D12] 查找元素下标
来源：http://odd.jinqigfzy.top

Py:   arr.index(x);  x in arr
来源：http://hyr.svipenyu.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://tsj.svipenyu.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jpw.xingfuxueyuan.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dlv.daria6918.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://rnj.yuxming.cn

Go:   slices.Index(arr, x)
来源：http://mce.tanke756.top

Ruby: arr.index(x)
来源：http://pvz.shangyingyoupin.top

C#:   list.IndexOf(x);
来源：http://fyc.xuetiantiany.cn

[D13] 过滤（保留满足条件的）
来源：http://sme.tarul.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://nhm.yuanzhike.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://zet.shanyushiyangtech.top

JS:   arr.filter(x => x > 3)
来源：http://nhe.zhixingplan.top

TS:   arr.filter(x => x > 3)
来源：http://std.guowangkeji.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://abp.tianlin.xyz

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://lwm.bbcook.cn

Ruby: arr.select { |x| x > 3 }
来源：http://sia.gzhubu.top

C#:   list.Where(x => x > 3).ToList()
来源：http://hla.svipenyu.cn

[D14] 映射转换（每个元素变形）
来源：http://oeg.hnxiangtu.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://gws.ybcxt.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ujq.snrcjt.cn

JS:   arr.map(x => x * 2)
来源：http://ric.xuetiantiany.cn

TS:   arr.map(x => x * 2)
来源：http://dhl.cucudq.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ybs.xingfuxueyuan.xyz

Go:   // 手写循环
来源：http://uyu.zhiwuduotai.top

Ruby: arr.map { |x| x * 2 }
来源：http://swc.yj20258.top

C#:   list.Select(x => x * 2).ToList()
来源：http://qgh.tanke756.top

[D15] 去重
来源：http://ody.yvedp.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://bqb.svipenyu.cn

PHP:  array_unique($arr);
来源：http://uxf.cheryme.top

JS:   [...new Set(arr)]
来源：http://zsl.sufxvd.cn

TS:   [...new Set(arr)]
来源：http://djo.ywan-chungtsiang.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ykc.xylfe.cn

Go:   // 用 map[T]struct{} 手写
来源：http://uji.jinghuilouyu.cn

Ruby: arr.uniq
来源：http://jbz.tianlin.xyz

C#:   list.Distinct().ToList()
来源：http://kkr.birdmap.top

[D16] 求和与平均值
来源：http://hvr.redwolf501.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://gko.yongpay.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://sgd.c1oappe.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ldu.zdbjq.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://afu.xuetiantiany.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xdw.sufxvd.cn

Go:   // 手写循环累加
来源：http://cbn.hfpthk.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://asw.zdbjq.cn

C#:   list.Sum();  list.Average()
来源：http://uql.cashguo.top

[D17] 最大值与最小值
来源：http://zan.zhixingplan.top

Py:   max(arr);  min(arr)
来源：http://aif.bbcook.cn

PHP:  max($arr);  min($arr);
来源：http://oeh.kuanghao11.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://rqs.jlsjyb.cn

TS:   Math.max(...arr);
来源：http://zzf.chenlongwang.top

Java: Collections.max(list);  Collections.min(list);
来源：http://hgu.jinghuilouyu.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://nnk.9152youxi.cn

Ruby: arr.max;  arr.min
来源：http://xnu.zhongyouzk.top

C#:   list.Max();  list.Min()
来源：http://oor.xuetiantiany.cn

[D18] 扁平化嵌套数组
来源：http://rvq.tarul.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://orq.gzhubu.top

PHP:  array_merge(...$nested);
来源：http://iaq.shanyushiyangtech.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://bfx.chenlongwang.top

TS:   nested.flat();
来源：http://koy.sweek.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://zok.ywan-chungtsiang.top

Go:   // 手写双层循环
来源：http://vuy.xinyue.icu

Ruby: nested.flatten
来源：http://ohx.jinghuilouyu.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://gct.hesvh.cn

[D19] 按字段分组
来源：http://mur.jinqigfzy.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://pqb.shanyushiyangtech.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mdk.yanxiufei.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://glv.haohaochexian.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://lyh.yuanzhike.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://rcx.9152youxi.cn

Go:   // 手写 map[string][]T
来源：http://ssg.sweek.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://tvf.gaohongyu789.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://obi.nwbrower.top

[D20] 统计每个元素出现次数
来源：http://sae.xingfuxueyuan.xyz

Py:   Counter(arr)
来源：http://dps.meibo888.top

PHP:  array_count_values($arr);
来源：http://urx.yj20258888.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dvl.ywan-chungtsiang.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yee.ivvv.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://aju.nanxuanxn.top

Go:   // 手写 map[T]int
来源：http://cob.fzhhl.top

Ruby: arr.tally
来源：http://wpa.shuidangran.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://xye.hnxiangtu.top

[D21] 判断是否包含某元素
来源：http://lqf.meibo888.top

Py:   x in arr
来源：http://aar.iojbl.cn

PHP:  in_array($x, $arr, true);
来源：http://nki.jlsjyb.cn

JS:   arr.includes(x)
来源：http://pbo.nwbrower.top

TS:   arr.includes(x)
来源：http://gfg.fehbvm.com

Java: list.contains(x)
来源：http://atk.yfazqb.com

Go:   slices.Contains(arr, x)
来源：http://izk.jyoumei.cn

Ruby: arr.include?(x)
来源：http://kko.uphjek.com

C#:   list.Contains(x)
来源：http://tjf.vqdsnc.cn

[D22] 复制数组（避免共享引用）
来源：http://owo.pengpengdd.cyou

Py:   arr.copy();  arr[:];  list(arr)
来源：http://kro.yueranfly.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://gmv.bjfxy.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://qml.meibo888.top

TS:   [...arr];
来源：http://oax.redwolf501.top


<!-- 参考信息 -->