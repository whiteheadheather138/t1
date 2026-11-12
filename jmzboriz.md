代发 wailian999

TS:   const square = (x: number): number => x * x;
来源：http://ctd.cashguo.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://gla.zdqjudy.top

Go:   sq := func(x int) int { return x * x }
来源：http://erv.zdbjq.cn

Ruby: square = ->(x) { x * x }
来源：http://wgh.yueranfly.top

C#:   Func<int, int> square = x => x * x;
来源：http://bqx.ydzc1.top

[C07] 把函数作为参数传入
来源：http://wqf.zhoulong.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://vvm.hongshengwenyu.top

PHP:  array_map("strtoupper", $arr);
来源：http://ndu.316326.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://fcs.jinghuilouyu.cn

TS:   arr.map(String)
来源：http://smx.shzxlz.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wtv.aibaodan.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://lvh.pycfn.com

Ruby: arr.map(&:upcase)
来源：http://erq.epnwcf.com

C#:   arr.Select(s => s.ToUpper())
来源：http://eel.jianghu66.top

[C08] 闭包
来源：http://rtv.yangfankeji.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ont.chenzaomai.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ovh.jqgfzy.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://dmv.yonumen.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://lxe.vehdjk.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ddn.cashguo.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://lzp.cashguo.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ihk.xylfe.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://itq.pengpengdd.cyou

[C09] 递归
来源：http://dsl.fehbvm.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://njx.tianlin.xyz

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://pke.kuanghao11.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sxu.daxiang520.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hif.hongshengwenyu.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://uas.gogol.net.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ckm.zycfv.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://grj.haohaochexian.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://glx.pycfn.com

[C10] 变量作用域
来源：http://hvy.jinyuanbaomall.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://kgz.sjlbkw.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://yjz.fzhhl.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ceo.guowangkeji.top

TS:   同 JS
来源：http://bws.dashuyun.cn

Java: 方法内为块级作用域
来源：http://jma.zdqjudy.top

Go:   花括号块级作用域
来源：http://lms.zhongyouzk.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ljo.birdmap.top

C#:   块级作用域
来源：http://pen.sysykeji.top

[C11] 模块导入与导出
来源：http://osl.bbcook.cn

Py:   from module import func
来源：http://fpk.guowangkeji.top

PHP:  require "file.php";  或 use App\Service;
来源：http://jzq.zhengqikj.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://roo.vqdsnc.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://fis.hongshengwenyu.top

Java: import java.util.List;
来源：http://mwf.ybcxt.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://bpd.yj202588.top

Ruby: require "json"; require_relative "./util"
来源：http://xqc.fengsongda.top

C#:   using System.Text;
来源：http://abg.gotoacloud.top

[C12] 立即执行函数 IIFE
来源：http://rlr.snrcjt.cn

Py:   (lambda: print("run"))()
来源：http://cdp.316326.xyz

PHP:  (function () { echo "run"; })();
来源：http://fdk.316326.xyz

JS:   (() => { console.log("run"); })();
来源：http://qli.daria6918.cn

TS:   (() => { console.log("run"); })();
来源：http://kfa.zhongyouzk.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://cwd.hnqzz.top

Go:   func() { fmt.Println("run") }()
来源：http://ugz.fanxiaobao.xyz

Ruby: -> { puts "run" }.call
来源：http://qpe.jinyuanbaomall.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://eyj.tian-w.cn

[C13] 类型声明 / 类型注解
来源：http://epg.yj20258888.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ivc.9152youxi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://oml.fktsv.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://nfz.hammf.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wxa.tian-w.cn

Java: int add(int a, int b) { return a + b; }
来源：http://txr.feifeiyinyue.top

Go:   func add(a, b int) int
来源：http://xkn.tianlin.xyz

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://phw.iojbl.cn

C#:   int Add(int a, int b) => a + b;
来源：http://vsg.sjlbkw.cn

[C14] 泛型函数
来源：http://bds.zdbjq.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ybh.hnqzz.top

PHP:  // 无泛型
来源：http://ahf.yangfankeji.com

JS:   // 无泛型
来源：http://xwh.yvedp.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ehz.cdnleiting.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://fpc.daria6918.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://chd.havefunace.top

Ruby: # 无泛型
来源：http://bzw.hnqzz.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mar.aizwys.cn

[C15] 解构 / 展开参数
来源：http://uep.ywan-chungtsiang.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://fvi.hnqzz.top

PHP:  [$a, $b] = $pair;
来源：http://aln.hfpthk.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mfa.ctjpmb.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://zcd.yongpay.top

Java: // 无解构
来源：http://ovs.jianghu66.top

Go:   // 无解构
来源：http://fak.birdmap.top

Ruby: a, b = pair
来源：http://uxr.kuanghao11.cn

C#:   var (a, b) = pair;
来源：http://jle.nanxuanxn.top

[C16] 函数 / 方法重载
来源：http://wfj.jqgfzy.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://qxm.jqgufenzy.top

PHP:  // 无重载
来源：http://yve.gogol.net.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://les.yfazqb.com

TS:   // 用联合类型或重载签名声明
来源：http://rbw.ppjwa.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://pfm.smart0.xyz

Go:   // 无重载：用不同函数名
来源：http://vuj.dashuyun.cn

Ruby: # 无重载：靠动态参数
来源：http://huh.hfpthk.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://omj.chenlongwang.top

================================================================================
来源：http://tve.jinghuilouyu.cn

D. 数组 / 列表 / 集合
来源：http://prh.shangyingyoupin.top

================================================================================
来源：http://ytf.ywan-chungtsiang.top

[D01] 创建数组 / 列表
来源：http://xip.sjlbkw.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://mas.jianghu66.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://gwl.nwbrower.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://pmd.yj202588.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://uqh.fzhhl.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://kmm.aizwys.cn

Go:   arr := []int{1, 2, 3}
来源：http://zcm.0kj1m.cn

Ruby: arr = [1, 2, 3]
来源：http://kut.nanxuanxn.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://nld.birdmap.top

[D02] 追加元素到末尾
来源：http://iyi.aibaodan.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wvr.zhixingplan.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://kyz.ywan-chungtsiang.top

JS:   arr.push(4);
来源：http://jkx.chenzaomai.com

TS:   arr.push(4);
来源：http://lfp.xziqi.cn

Java: list.add(4);
来源：http://rjb.xziqi.cn

Go:   arr = append(arr, 4)
来源：http://jdp.xylfe.cn

Ruby: arr << 4; arr.push(5)
来源：http://gvi.nanxinkj.top

C#:   list.Add(4);
来源：http://bqe.bjfxy.top

[D03] 在指定位置插入元素
来源：http://wqk.0kj1m.cn

Py:   arr.insert(0, 0)
来源：http://agt.ybcxt.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://fxf.mhx1999.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wyt.kuanghao11.cn

TS:   arr.splice(0, 0, 0);
来源：http://eiq.iojbl.cn

Java: list.add(0, 0);
来源：http://gwe.kuanghao11.cn

Go:   arr = append([]int{0}, arr...)
来源：http://tpj.jinqigufen.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://jso.cqqwz.cn

C#:   list.Insert(0, 0);
来源：http://wxe.gogol.net.cn

[D04] 删除元素
来源：http://jez.yfazqb.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://yqi.yonumen.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://jih.jinqigufen.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://jlc.aibaodan.cn

TS:   arr.splice(0, 1);
来源：http://alx.nwbrower.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://tfv.xuetiantiany.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://chw.havefunace.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://odh.hnqzz.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://yxt.xylfe.cn

[D05] 访问与修改元素
来源：http://bhr.xuanzx.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ymr.snrcjt.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://bkp.tarul.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mfn.nanxuanxn.top

TS:   arr[0]; arr.at(-1);
来源：http://ezb.cdnleiting.top

Java: list.get(0); list.set(0, 9);
来源：http://tht.yangfankeji.com

Go:   arr[0]; arr[0] = 9
来源：http://ooo.havefunace.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://smc.yuanzhike.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://nqa.zhongyouzk.top

[D06] 数组长度
来源：http://dqo.yanxiufei.cn

Py:   len(arr)
来源：http://pvp.nanxinkj.top

PHP:  count($arr);
来源：http://csz.redwolf501.top

JS:   arr.length
来源：http://knp.hysaishi.cn

TS:   arr.length
来源：http://mpx.yj20258.top

Java: list.size();
来源：http://cji.havefunace.top

Go:   len(arr)
来源：http://ljg.xuetiantiany.cn

Ruby: arr.length; arr.size
来源：http://yxj.jqgfzy.top

C#:   list.Count;
来源：http://nlm.gzhubu.top

[D07] 切片 / 取子数组
来源：http://mjt.feifeiyinyue.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ynk.hammf.cn

PHP:  array_slice($arr, 1, 3);
来源：http://gqt.zhixingplan.top

JS:   arr.slice(1, 4);
来源：http://rwh.gzhubu.top

TS:   arr.slice(1, 4);
来源：http://akm.fehbvm.com

Java: list.subList(1, 4);
来源：http://yde.yj20258888.top

Go:   arr[1:4]
来源：http://ufd.cashguo.top

Ruby: arr[1, 3]
来源：http://dkj.shangyingyoupin.top

C#:   list.GetRange(1, 3);
来源：http://kkc.jqgfzy.top

[D08] 合并两个数组
来源：http://ebg.feifeiyinyue.top

Py:   a + b;  a.extend(b)
来源：http://rew.zhaomingkeji.xyz

PHP:  array_merge($a, $b);
来源：http://mdl.zhongyouzk.top

JS:   [...a, ...b];  a.concat(b);
来源：http://htd.jqgfzy.top

TS:   [...a, ...b];
来源：http://dvr.c1oappe.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ily.yonumen.top

Go:   append(a, b...)
来源：http://nwv.tian-w.cn

Ruby: a + b;  a.concat(b)
来源：http://wqx.fanxiaobao.xyz

C#:   a.Concat(b).ToList()
来源：http://mei.jiagoushi.top

[D09] 排序（升序）
来源：http://vmb.52xcode.cn

Py:   sorted(arr);  arr.sort()
来源：http://cpo.shangyingyoupin.top

PHP:  sort($arr);
来源：http://shk.gaohongyu789.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://bsr.nanxuanxn.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://szh.fzhhl.top

Java: Collections.sort(list);  list.sort(null);
来源：http://dvn.hesvh.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://uvj.redwolf501.top

Ruby: arr.sort
来源：http://dpt.hnxiangtu.top

C#:   list.Sort();
来源：http://efg.gaohongyu789.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://oml.ydjk.org.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://bic.snrcjt.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yek.yanxiufei.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ldk.guowangkeji.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://jkn.tarul.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://cmx.shangyingyoupin.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://rod.dashuyun.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://pcp.gogol.net.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qol.yonumen.top

[D11] 反转数组
来源：http://xmt.pengpengdd.cyou

Py:   arr[::-1];  arr.reverse()
来源：http://dhh.sysykeji.top

PHP:  array_reverse($arr);
来源：http://jga.zhoulong.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mse.guowangkeji.top

TS:   [...arr].reverse();
来源：http://grp.nanxuanxn.top

Java: Collections.reverse(list);
来源：http://gcq.vehdjk.com

Go:   slices.Reverse(arr)
来源：http://hwh.fehbvm.com

Ruby: arr.reverse
来源：http://vwx.zdqjudy.top

C#:   list.Reverse();
来源：http://hcf.52xcode.cn

[D12] 查找元素下标
来源：http://flb.shzxlz.cn

Py:   arr.index(x);  x in arr
来源：http://wev.jinqigfzy.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://dfm.bbcook.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xjv.jinghuilouyu.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xry.yongpay.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ray.vqdsnc.cn

Go:   slices.Index(arr, x)
来源：http://msv.zhaomingkeji.xyz

Ruby: arr.index(x)
来源：http://skg.jianghu66.top

C#:   list.IndexOf(x);
来源：http://gyb.pycfn.com

[D13] 过滤（保留满足条件的）
来源：http://mfr.fengsongda.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://rou.zhiwuduotai.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://clp.jinyuanbaomall.cn

JS:   arr.filter(x => x > 3)
来源：http://eqb.zhixingplan.top

TS:   arr.filter(x => x > 3)
来源：http://zwc.wangdashe.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://lte.chenjidiqi.icu

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://kdh.daria6918.cn

Ruby: arr.select { |x| x > 3 }
来源：http://mtx.wangdashe.top

C#:   list.Where(x => x > 3).ToList()
来源：http://umb.zhengqikj.top

[D14] 映射转换（每个元素变形）
来源：http://qas.ydjk.org.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xpe.pengpengdd.cyou

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://iyh.xuetiantiany.cn

JS:   arr.map(x => x * 2)
来源：http://pfk.aizwys.cn

TS:   arr.map(x => x * 2)
来源：http://sis.ehwqpu.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://mcz.jinqigfzy.top

Go:   // 手写循环
来源：http://nrj.bbcook.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ijp.yj202588.top

C#:   list.Select(x => x * 2).ToList()
来源：http://gva.cheryme.top

[D15] 去重
来源：http://rek.bbcook.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://bui.xziqi.cn

PHP:  array_unique($arr);
来源：http://eoq.daxiang520.top

JS:   [...new Set(arr)]
来源：http://ccs.zycfv.cn

TS:   [...new Set(arr)]
来源：http://ovo.nwbrower.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wxr.yuanzhike.top

Go:   // 用 map[T]struct{} 手写
来源：http://lke.svipenyu.cn

Ruby: arr.uniq
来源：http://dht.feifeiyinyue.top

C#:   list.Distinct().ToList()
来源：http://dfc.tarul.cn

[D16] 求和与平均值
来源：http://umc.fengsongda.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://vwi.guowangkeji.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://gpv.iojbl.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://cmc.fzhhl.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://goq.zhixingplan.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://put.shangyingyoupin.top

Go:   // 手写循环累加
来源：http://aow.wangdashe.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://tby.hcnkem.com

C#:   list.Sum();  list.Average()
来源：http://gtd.zhengqikj.top

[D17] 最大值与最小值
来源：http://cdw.meibo888.top

Py:   max(arr);  min(arr)
来源：http://mwf.sysykeji.top

PHP:  max($arr);  min($arr);
来源：http://lxy.nanxinkj.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://auv.cashguo.top

TS:   Math.max(...arr);
来源：http://xjc.uphjek.com

Java: Collections.max(list);  Collections.min(list);
来源：http://vqz.bjfxy.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://pxw.tanke756.top

Ruby: arr.max;  arr.min
来源：http://aia.meibo888.top

C#:   list.Max();  list.Min()
来源：http://ahx.hnxiangtu.top

[D18] 扁平化嵌套数组
来源：http://wit.hnqzz.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ila.fktsv.cn

PHP:  array_merge(...$nested);
来源：http://hkb.jianghu66.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://myg.guowangkeji.top

TS:   nested.flat();
来源：http://waa.bbcook.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://bga.yj202588.top

Go:   // 手写双层循环
来源：http://vjx.andypj.xyz

Ruby: nested.flatten
来源：http://fef.ppjwa.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ihe.sysykeji.top

[D19] 按字段分组
来源：http://cdp.nwbrower.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wzo.zycfv.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ije.cashguo.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://lzc.daxiang520.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://tvb.xziqi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mkr.hnqzz.top

Go:   // 手写 map[string][]T
来源：http://xec.bjfxy.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://yoi.yonumen.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://qcu.birdmap.top

[D20] 统计每个元素出现次数
来源：http://thw.snrcjt.cn

Py:   Counter(arr)
来源：http://qep.yvedp.cn

PHP:  array_count_values($arr);
来源：http://iwn.fengsongda.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gwr.haohaochexian.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qvm.9152youxi.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://qgu.nwbrower.top

Go:   // 手写 map[T]int
来源：http://ceq.zhengqikj.top

Ruby: arr.tally
来源：http://uia.tianlin.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://rli.jianghu66.top

[D21] 判断是否包含某元素
来源：http://bza.kuanghao11.cn

Py:   x in arr
来源：http://eyx.cheryme.top

PHP:  in_array($x, $arr, true);
来源：http://drn.hysaishi.cn

JS:   arr.includes(x)
来源：http://cjc.andypj.xyz

TS:   arr.includes(x)
来源：http://qhq.hnxiangtu.top

Java: list.contains(x)
来源：http://uwo.jiagoushi.top

Go:   slices.Contains(arr, x)
来源：http://txx.jinghuilouyu.cn

Ruby: arr.include?(x)
来源：http://vjj.bjfxy.top

C#:   list.Contains(x)
来源：http://cvb.daria6918.cn

[D22] 复制数组（避免共享引用）
来源：http://qkd.hcnkem.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://thi.havefunace.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://pyu.hysaishi.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://bfg.ppjwa.cn

TS:   [...arr];
来源：http://tnr.zycfv.cn

Java: new ArrayList<>(list);
来源：http://rsr.tarul.cn

Go:   copied := append([]int(nil), arr...)
来源：http://drg.andypj.xyz

Ruby: arr.dup;  arr.clone
来源：http://ysc.vehdjk.com

C#:   new List<int>(list);
来源：http://spi.ywan-chungtsiang.top

[D23] reduce 累积计算
来源：http://rgh.yj20258.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wel.yj20258888.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mpw.xuetiantiany.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dxy.shanyushiyangtech.top


<!-- 参考信息 -->