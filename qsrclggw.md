代发 wailian999

TS:   const square = (x: number): number => x * x;
来源：http://uch.shangyingyoupin.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://pvi.hongshengwenyu.top

Go:   sq := func(x int) int { return x * x }
来源：http://mia.yangfankeji.com

Ruby: square = ->(x) { x * x }
来源：http://rqo.snrcjt.cn

C#:   Func<int, int> square = x => x * x;
来源：http://oma.pycfn.com

[C07] 把函数作为参数传入
来源：http://rtc.birdmap.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ydj.nwbrower.top

PHP:  array_map("strtoupper", $arr);
来源：http://hgi.gotoacloud.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://igo.smart0.xyz

TS:   arr.map(String)
来源：http://mlp.sweek.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://tjb.ybcxt.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://poy.tarul.cn

Ruby: arr.map(&:upcase)
来源：http://zpo.shangyingyoupin.top

C#:   arr.Select(s => s.ToUpper())
来源：http://mko.cqqwz.cn

[C08] 闭包
来源：http://seo.hesvh.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://cfn.vehdjk.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://xnk.cashguo.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ixo.jlsjyb.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://sgf.gogol.net.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://vnn.hywenlv.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://job.ctjpmb.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://gys.jlsjyb.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://uuc.wangdashe.top

[C09] 递归
来源：http://keg.xylfe.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://rks.hysaishi.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wzr.gzhubu.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pqn.hcnkem.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ofa.hongshengwenyu.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://vft.zhixingplan.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://vbb.fanxiaobao.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://juw.snrcjt.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://iby.vqdsnc.cn

[C10] 变量作用域
来源：http://rgq.nanxinkj.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://umt.zhixingplan.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://bwt.vehdjk.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wsm.yanxiufei.cn

TS:   同 JS
来源：http://jzm.jinqigfzy.top

Java: 方法内为块级作用域
来源：http://vbv.tarul.cn

Go:   花括号块级作用域
来源：http://sdp.fehbvm.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://sjf.gaohongyu789.top

C#:   块级作用域
来源：http://qhd.zhengqikj.top

[C11] 模块导入与导出
来源：http://nim.shzxlz.cn

Py:   from module import func
来源：http://xvi.feifeiyinyue.top

PHP:  require "file.php";  或 use App\Service;
来源：http://avx.pengpengdd.cyou

JS:   export default function f() {};  import f from "./m.js";
来源：http://skc.shanyushiyangtech.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://bhh.havefunace.top

Java: import java.util.List;
来源：http://vmg.hcnkem.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mcv.aibaodan.cn

Ruby: require "json"; require_relative "./util"
来源：http://rjv.pycfn.com

C#:   using System.Text;
来源：http://xoc.gogol.net.cn

[C12] 立即执行函数 IIFE
来源：http://gql.ydjk.org.cn

Py:   (lambda: print("run"))()
来源：http://pgd.316326.xyz

PHP:  (function () { echo "run"; })();
来源：http://obg.chenzaomai.com

JS:   (() => { console.log("run"); })();
来源：http://fqs.sufxvd.cn

TS:   (() => { console.log("run"); })();
来源：http://wdg.cucudq.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://khd.ydzc1.top

Go:   func() { fmt.Println("run") }()
来源：http://vmf.zycfv.cn

Ruby: -> { puts "run" }.call
来源：http://bus.haohaochexian.top

C#:   // 无 IIFE：用静态构造函数
来源：http://gzn.yuxming.cn

[C13] 类型声明 / 类型注解
来源：http://fag.yangfankeji.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mpg.nanxuanxn.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tbz.yuxming.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://drn.yfazqb.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zte.pycfn.com

Java: int add(int a, int b) { return a + b; }
来源：http://nyf.zdqjudy.top

Go:   func add(a, b int) int
来源：http://xmq.daxiang520.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://vft.meibo888.top

C#:   int Add(int a, int b) => a + b;
来源：http://dfb.dianchejie.cn

[C14] 泛型函数
来源：http://vqf.hfpthk.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://qws.sysykeji.top

PHP:  // 无泛型
来源：http://tbt.sweek.top

JS:   // 无泛型
来源：http://dsz.9152youxi.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://lnp.jinghuilouyu.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://qde.hfpthk.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://tzw.hammf.cn

Ruby: # 无泛型
来源：http://wui.ppjwa.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://jjm.havefunace.top

[C15] 解构 / 展开参数
来源：http://dxw.xuanzx.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://vbe.fehbvm.com

PHP:  [$a, $b] = $pair;
来源：http://bbx.xingfuxueyuan.xyz

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://jwt.yanxiufei.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://gyr.fehbvm.com

Java: // 无解构
来源：http://ncg.sysykeji.top

Go:   // 无解构
来源：http://cji.ctjpmb.com

Ruby: a, b = pair
来源：http://zmm.sysykeji.top

C#:   var (a, b) = pair;
来源：http://vct.svipenyu.cn

[C16] 函数 / 方法重载
来源：http://vmj.bjfxy.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ipc.yuanzhike.top

PHP:  // 无重载
来源：http://dxr.yj20258.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://nmw.epnwcf.com

TS:   // 用联合类型或重载签名声明
来源：http://fdj.sysykeji.top

Java: void f(int a) {}  void f(String a) {}
来源：http://jen.cdnleiting.top

Go:   // 无重载：用不同函数名
来源：http://dcx.quarkkingdee.top

Ruby: # 无重载：靠动态参数
来源：http://wrd.gogol.net.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://qms.xinyue.icu

================================================================================
来源：http://ium.yuanzhike.top

D. 数组 / 列表 / 集合
来源：http://fcm.xuanzx.com

================================================================================
来源：http://klo.smart0.xyz

[D01] 创建数组 / 列表
来源：http://dwm.daxiang520.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://bma.zhengqikj.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://pbb.guannengcc.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://trm.hfpthk.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://nox.kuanghao11.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://byn.dashuyun.cn

Go:   arr := []int{1, 2, 3}
来源：http://ygf.gaohongyu789.top

Ruby: arr = [1, 2, 3]
来源：http://msx.hnqzz.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hbw.snrcjt.cn

[D02] 追加元素到末尾
来源：http://xto.chenzaomai.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://xpz.aibaodan.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ubh.fehbvm.com

JS:   arr.push(4);
来源：http://hon.epnwcf.com

TS:   arr.push(4);
来源：http://mvv.yj20258.top

Java: list.add(4);
来源：http://wvw.hesvh.cn

Go:   arr = append(arr, 4)
来源：http://lcg.316326.xyz

Ruby: arr << 4; arr.push(5)
来源：http://kcn.haohaochexian.top

C#:   list.Add(4);
来源：http://amq.fktsv.cn

[D03] 在指定位置插入元素
来源：http://gkq.zycfv.cn

Py:   arr.insert(0, 0)
来源：http://ubp.yj20258888.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wtl.yueranfly.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://pgw.jinqigufen.top

TS:   arr.splice(0, 0, 0);
来源：http://yhl.zdqjudy.top

Java: list.add(0, 0);
来源：http://rhr.wangdashe.top

Go:   arr = append([]int{0}, arr...)
来源：http://evq.zhiwuduotai.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://tnz.fzhhl.top

C#:   list.Insert(0, 0);
来源：http://bma.xylfe.cn

[D04] 删除元素
来源：http://bla.daria6918.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://lau.gzhubu.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ihw.zdqjudy.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://cqc.jqgfzy.top

TS:   arr.splice(0, 1);
来源：http://usb.jiagoushi.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ano.zdbjq.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://rol.hongshengwenyu.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mha.shanyushiyangkeji.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://drx.smart0.xyz

[D05] 访问与修改元素
来源：http://rgl.cashguo.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://bqo.dashuyun.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://rgt.nanxuanxn.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://djl.gzhubu.top

TS:   arr[0]; arr.at(-1);
来源：http://tcx.sweek.top

Java: list.get(0); list.set(0, 9);
来源：http://qky.gaohongyu789.top

Go:   arr[0]; arr[0] = 9
来源：http://acd.yj20258888.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://fbk.yangfankeji.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://azm.xinyue.icu

[D06] 数组长度
来源：http://dkt.wangshuangyany.cn

Py:   len(arr)
来源：http://rhn.quarkkingdee.top

PHP:  count($arr);
来源：http://pkb.nanxinkj.top

JS:   arr.length
来源：http://mkc.jinqigfzy.top

TS:   arr.length
来源：http://gxo.chenjidiqi.icu

Java: list.size();
来源：http://irc.jianghu66.top

Go:   len(arr)
来源：http://xfu.shanyushiyangkeji.top

Ruby: arr.length; arr.size
来源：http://ymy.ydzc1.top

C#:   list.Count;
来源：http://frd.yangfankeji.com

[D07] 切片 / 取子数组
来源：http://wzp.zdbjq.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://xxl.zhiwuduotai.top

PHP:  array_slice($arr, 1, 3);
来源：http://qun.feifeiyinyue.top

JS:   arr.slice(1, 4);
来源：http://jcw.smart0.xyz

TS:   arr.slice(1, 4);
来源：http://uch.feifeiyinyue.top

Java: list.subList(1, 4);
来源：http://bkj.uphjek.com

Go:   arr[1:4]
来源：http://zey.xingfuxueyuan.xyz

Ruby: arr[1, 3]
来源：http://fqu.c1oappe.top

C#:   list.GetRange(1, 3);
来源：http://ntg.shanyushiyangkeji.top

[D08] 合并两个数组
来源：http://zkj.shanyushiyangtech.top

Py:   a + b;  a.extend(b)
来源：http://zrx.zdqjudy.top

PHP:  array_merge($a, $b);
来源：http://bmj.sxryk.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://owp.jinqigfzy.top

TS:   [...a, ...b];
来源：http://khz.hcnkem.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://qzo.ivvv.top

Go:   append(a, b...)
来源：http://stp.cdnleiting.top

Ruby: a + b;  a.concat(b)
来源：http://yjs.cdnleiting.top

C#:   a.Concat(b).ToList()
来源：http://bzv.nanxuanxn.top

[D09] 排序（升序）
来源：http://ony.ywan-chungtsiang.top

Py:   sorted(arr);  arr.sort()
来源：http://jff.cqqwz.cn

PHP:  sort($arr);
来源：http://ttt.dianchejie.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ifl.cdnleiting.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://lbw.yfazqb.com

Java: Collections.sort(list);  list.sort(null);
来源：http://gai.pengpengdd.cyou

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://gzt.ydjk.org.cn

Ruby: arr.sort
来源：http://vrw.ydzc1.top

C#:   list.Sort();
来源：http://wok.hesvh.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://qly.chenlongwang.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://gre.hongshengwenyu.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bzd.jinyuanbaomall.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hgw.vqdsnc.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://dwg.fktsv.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://vfd.gzhubu.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://aru.dashuyun.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://fwt.andypj.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://iqe.daria6918.cn

[D11] 反转数组
来源：http://vph.birdmap.top

Py:   arr[::-1];  arr.reverse()
来源：http://huw.gaohongyu789.top

PHP:  array_reverse($arr);
来源：http://fgw.c1oappe.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://lgd.fzhhl.top

TS:   [...arr].reverse();
来源：http://avr.redwolf501.top

Java: Collections.reverse(list);
来源：http://mik.fanxiaobao.xyz

Go:   slices.Reverse(arr)
来源：http://alq.cucudq.cn

Ruby: arr.reverse
来源：http://gcw.cqqwz.cn

C#:   list.Reverse();
来源：http://lea.jqgufenzy.top

[D12] 查找元素下标
来源：http://lxw.fengsongda.top

Py:   arr.index(x);  x in arr
来源：http://xvr.c1oappe.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://bng.birdmap.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kps.jinghuilouyu.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rqz.chenjidiqi.icu

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://dzv.xinyue.icu

Go:   slices.Index(arr, x)
来源：http://rsp.tian-w.cn

Ruby: arr.index(x)
来源：http://mob.tian-w.cn

C#:   list.IndexOf(x);
来源：http://gow.daria6918.cn

[D13] 过滤（保留满足条件的）
来源：http://sdz.zhongyouzk.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://rdn.hammf.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://pfp.vehdjk.com

JS:   arr.filter(x => x > 3)
来源：http://bav.aibaodan.cn

TS:   arr.filter(x => x > 3)
来源：http://rfm.hnxiangtu.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://eip.pycfn.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://bgi.bjfxy.top

Ruby: arr.select { |x| x > 3 }
来源：http://ddh.jlsjyb.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://zya.tian-w.cn

[D14] 映射转换（每个元素变形）
来源：http://rgy.zhiwuduotai.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://fny.guowangkeji.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://khg.pengpengdd.cyou

JS:   arr.map(x => x * 2)
来源：http://pmd.xinyue.icu

TS:   arr.map(x => x * 2)
来源：http://nrt.zhaomingkeji.xyz

Java: list.stream().map(x -> x * 2).toList()
来源：http://fdu.hywenlv.cn

Go:   // 手写循环
来源：http://iml.tarul.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ogl.hesvh.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ufk.vqdsnc.cn

[D15] 去重
来源：http://zit.jinqigufen.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://szd.kuanghao11.cn

PHP:  array_unique($arr);
来源：http://kmd.hongshengwenyu.top

JS:   [...new Set(arr)]
来源：http://ulp.zycfv.cn

TS:   [...new Set(arr)]
来源：http://cda.tian-w.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wgp.ybcxt.top

Go:   // 用 map[T]struct{} 手写
来源：http://sha.yuxming.cn

Ruby: arr.uniq
来源：http://eyy.svipenyu.cn

C#:   list.Distinct().ToList()
来源：http://tpr.shanyushiyangtech.top

[D16] 求和与平均值
来源：http://qxi.hongshengwenyu.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://plw.tianlin.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://jws.cucudq.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://pav.haohaochexian.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://jrn.ehwqpu.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://nqe.gogol.net.cn

Go:   // 手写循环累加
来源：http://hsx.hnxiangtu.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://rmh.vqdsnc.cn

C#:   list.Sum();  list.Average()
来源：http://opy.svipenyu.cn

[D17] 最大值与最小值
来源：http://bid.jianghu66.top

Py:   max(arr);  min(arr)
来源：http://bur.zdbjq.cn

PHP:  max($arr);  min($arr);
来源：http://hdk.jinyuanbaomall.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://jkm.wangdashe.top

TS:   Math.max(...arr);
来源：http://fvw.cdnleiting.top

Java: Collections.max(list);  Collections.min(list);
来源：http://dcl.shanyushiyangkeji.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://xsj.xziqi.cn

Ruby: arr.max;  arr.min
来源：http://osa.nwbrower.top

C#:   list.Max();  list.Min()
来源：http://qjw.yanxiufei.cn

[D18] 扁平化嵌套数组
来源：http://kma.kuanghao11.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://pxp.fanxiaobao.xyz

PHP:  array_merge(...$nested);
来源：http://sbi.wangshuangyany.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://qrd.fengsongda.top

TS:   nested.flat();
来源：http://mmo.hywenlv.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://lll.birdmap.top

Go:   // 手写双层循环
来源：http://xvt.hywenlv.cn

Ruby: nested.flatten
来源：http://ees.ctjpmb.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://nik.jqgufenzy.top

[D19] 按字段分组
来源：http://ojz.fktsv.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://udj.gogol.net.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ust.yj20258888.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://vvh.cheryme.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://qns.nanxinkj.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://gnr.kuanghao11.cn

Go:   // 手写 map[string][]T
来源：http://dvx.zhijiandao.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://vrl.cheryme.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://gmu.cheryme.top

[D20] 统计每个元素出现次数
来源：http://wuh.nanxinkj.top

Py:   Counter(arr)
来源：http://qgj.xuetiantiany.cn

PHP:  array_count_values($arr);
来源：http://hrg.jiagoushi.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qgp.yonumen.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rzo.hnqzz.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://vyv.hfpthk.cn

Go:   // 手写 map[T]int
来源：http://pyo.cdnleiting.top

Ruby: arr.tally
来源：http://gpd.yvedp.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ksm.ctjpmb.com

[D21] 判断是否包含某元素
来源：http://wkv.sufxvd.cn

Py:   x in arr
来源：http://biy.gotoacloud.top

PHP:  in_array($x, $arr, true);
来源：http://ewy.quarkkingdee.top

JS:   arr.includes(x)
来源：http://jgv.chenlongwang.top

TS:   arr.includes(x)
来源：http://ggv.shangyingyoupin.top

Java: list.contains(x)
来源：http://ldk.smart0.xyz

Go:   slices.Contains(arr, x)
来源：http://vos.jqgufenzy.top

Ruby: arr.include?(x)
来源：http://grt.redwolf501.top

C#:   list.Contains(x)
来源：http://enx.hywenlv.cn

[D22] 复制数组（避免共享引用）
来源：http://byr.xinyue.icu

Py:   arr.copy();  arr[:];  list(arr)
来源：http://cxg.zhengqikj.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://toj.zhaomingkeji.xyz

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://utt.hesvh.cn

TS:   [...arr];
来源：http://yss.sysykeji.top

Java: new ArrayList<>(list);
来源：http://xdi.svipenyu.cn

Go:   copied := append([]int(nil), arr...)
来源：http://uug.c1oappe.top

Ruby: arr.dup;  arr.clone
来源：http://xvs.uphjek.com

C#:   new List<int>(list);
来源：http://lws.jinqigufen.top

[D23] reduce 累积计算
来源：http://xik.gaohongyu789.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ohe.birdmap.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mxu.birdmap.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vdg.snrcjt.cn


<!-- 参考信息 -->