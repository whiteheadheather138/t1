代发 wailian999

C#:   Func<int, int> square = x => x * x;
来源：http://pit.meibo888.top

[C07] 把函数作为参数传入
来源：http://cyl.hnqzz.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://kkl.jyoumei.cn

PHP:  array_map("strtoupper", $arr);
来源：http://rzl.nwbrower.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://tnt.yuxming.cn

TS:   arr.map(String)
来源：http://mxw.hnqzz.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://qlp.meibo888.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://heb.yueranfly.top

Ruby: arr.map(&:upcase)
来源：http://pri.zdbjq.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://koe.yj20258.top

[C08] 闭包
来源：http://znl.hnqzz.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://kkw.c1oappe.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://vzv.uphjek.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qsj.jlsjyb.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ome.yueranfly.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://oep.xylfe.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://gqm.svipenyu.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://bck.hcnkem.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://gyn.fengsongda.top

[C09] 递归
来源：http://nnl.zhengqikj.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mjp.hesvh.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ziv.guannengcc.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ykn.jyoumei.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mww.hcnkem.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://yub.zhoulong.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://udh.meibo888.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mor.iojbl.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ezp.bjfxy.top

[C10] 变量作用域
来源：http://qam.hnxiangtu.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://zqk.guannengcc.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://fxc.shuidangran.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://dlw.andypj.xyz

TS:   同 JS
来源：http://ggw.gogol.net.cn

Java: 方法内为块级作用域
来源：http://rij.havefunace.top

Go:   花括号块级作用域
来源：http://mwb.yuanzhike.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://yti.hnxiangtu.top

C#:   块级作用域
来源：http://hui.vehdjk.com

[C11] 模块导入与导出
来源：http://tgv.gaohongyu789.top

Py:   from module import func
来源：http://ayu.shuidangran.top

PHP:  require "file.php";  或 use App\Service;
来源：http://jkb.aibaodan.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ray.fktsv.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://npm.gogol.net.cn

Java: import java.util.List;
来源：http://jdq.nwbrower.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://bpr.xinyue.icu

Ruby: require "json"; require_relative "./util"
来源：http://wwd.jlsjyb.cn

C#:   using System.Text;
来源：http://szm.sweek.top

[C12] 立即执行函数 IIFE
来源：http://pdo.bbcook.cn

Py:   (lambda: print("run"))()
来源：http://mck.pengpengdd.cyou

PHP:  (function () { echo "run"; })();
来源：http://mki.gzhubu.top

JS:   (() => { console.log("run"); })();
来源：http://lwt.hysaishi.cn

TS:   (() => { console.log("run"); })();
来源：http://ybw.aizwys.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://lcm.hammf.cn

Go:   func() { fmt.Println("run") }()
来源：http://com.zycfv.cn

Ruby: -> { puts "run" }.call
来源：http://icb.yanxiufei.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://cwa.0kj1m.cn

[C13] 类型声明 / 类型注解
来源：http://lbz.hcnkem.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hyl.9152youxi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qbe.bjfxy.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://glt.9152youxi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vqv.jyoumei.cn

Java: int add(int a, int b) { return a + b; }
来源：http://sjp.yanxiufei.cn

Go:   func add(a, b int) int
来源：http://tpy.yj20258888.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ene.gaohongyu789.top

C#:   int Add(int a, int b) => a + b;
来源：http://egk.tanke756.top

[C14] 泛型函数
来源：http://jgr.xziqi.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://pxc.quarkkingdee.top

PHP:  // 无泛型
来源：http://mos.feifeiyinyue.top

JS:   // 无泛型
来源：http://kjx.jqgfzy.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://qvt.hesvh.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hsh.nanxuanxn.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://djr.haohaochexian.top

Ruby: # 无泛型
来源：http://ikb.fanxiaobao.xyz

C#:   static T First<T>(List<T> items) => items[0];
来源：http://asl.ydjk.org.cn

[C15] 解构 / 展开参数
来源：http://hfh.zhiwuduotai.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ubb.zhengqikj.top

PHP:  [$a, $b] = $pair;
来源：http://fft.vehdjk.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://pme.birdmap.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://uty.shanyushiyangkeji.top

Java: // 无解构
来源：http://evt.chenjidiqi.icu

Go:   // 无解构
来源：http://pbz.yj20258888.top

Ruby: a, b = pair
来源：http://ikp.pycfn.com

C#:   var (a, b) = pair;
来源：http://rnb.shzxlz.cn

[C16] 函数 / 方法重载
来源：http://gje.yj20258888.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://lzj.hysaishi.cn

PHP:  // 无重载
来源：http://dbc.jqgufenzy.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://fdc.fzhhl.top

TS:   // 用联合类型或重载签名声明
来源：http://yzm.xingfuxueyuan.xyz

Java: void f(int a) {}  void f(String a) {}
来源：http://btx.316326.xyz

Go:   // 无重载：用不同函数名
来源：http://ruq.zhiwuduotai.top

Ruby: # 无重载：靠动态参数
来源：http://dzs.hnqzz.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://igd.guannengcc.top

================================================================================
来源：http://vlz.nwbrower.top

D. 数组 / 列表 / 集合
来源：http://pkk.yanxiufei.cn

================================================================================
来源：http://goc.ivvv.top

[D01] 创建数组 / 列表
来源：http://mhr.jqgufenzy.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://iuc.yfazqb.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://irc.aizwys.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://zfi.vqdsnc.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ckh.ywan-chungtsiang.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://vtj.shanyushiyangkeji.top

Go:   arr := []int{1, 2, 3}
来源：http://jbr.hammf.cn

Ruby: arr = [1, 2, 3]
来源：http://iuj.hnxiangtu.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://jlh.jinqigufen.top

[D02] 追加元素到末尾
来源：http://bdl.mhx1999.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://gpl.xuetiantiany.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://fjd.hnqzz.top

JS:   arr.push(4);
来源：http://ted.sufxvd.cn

TS:   arr.push(4);
来源：http://mag.ydjk.org.cn

Java: list.add(4);
来源：http://zzg.vehdjk.com

Go:   arr = append(arr, 4)
来源：http://pqu.xinyue.icu

Ruby: arr << 4; arr.push(5)
来源：http://tsh.zhoulong.xyz

C#:   list.Add(4);
来源：http://lgh.guannengcc.top

[D03] 在指定位置插入元素
来源：http://wpy.jinqigufen.top

Py:   arr.insert(0, 0)
来源：http://wsw.zhixingplan.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://skw.ctjpmb.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://umb.mhx1999.top

TS:   arr.splice(0, 0, 0);
来源：http://spb.tian-w.cn

Java: list.add(0, 0);
来源：http://qpf.aibaodan.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ybh.yj20258.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://uvo.svipenyu.cn

C#:   list.Insert(0, 0);
来源：http://xkp.zhijiandao.cn

[D04] 删除元素
来源：http://sqn.ppjwa.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://pnp.tanke756.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ssn.svipenyu.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://spy.svipenyu.cn

TS:   arr.splice(0, 1);
来源：http://smv.0kj1m.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://tcj.vehdjk.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://fsm.shanyushiyangkeji.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://bsf.andypj.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://znd.ctjpmb.com

[D05] 访问与修改元素
来源：http://myf.fehbvm.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://oxa.vqdsnc.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://rbw.guannengcc.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://vkc.nanxuanxn.top

TS:   arr[0]; arr.at(-1);
来源：http://clc.316326.xyz

Java: list.get(0); list.set(0, 9);
来源：http://bma.yj20258.top

Go:   arr[0]; arr[0] = 9
来源：http://ggo.9152youxi.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://jcp.316326.xyz

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://yup.vqdsnc.cn

[D06] 数组长度
来源：http://pli.xziqi.cn

Py:   len(arr)
来源：http://srs.yuanzhike.top

PHP:  count($arr);
来源：http://xqq.jlsjyb.cn

JS:   arr.length
来源：http://pph.shanyushiyangkeji.top

TS:   arr.length
来源：http://jrt.havefunace.top

Java: list.size();
来源：http://boj.yj20258.top

Go:   len(arr)
来源：http://mrx.daria6918.cn

Ruby: arr.length; arr.size
来源：http://jxj.jinqigfzy.top

C#:   list.Count;
来源：http://jdg.mhx1999.top

[D07] 切片 / 取子数组
来源：http://ste.nanxuanxn.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://sgj.yj20258.top

PHP:  array_slice($arr, 1, 3);
来源：http://qqk.zhongyouzk.top

JS:   arr.slice(1, 4);
来源：http://ohs.epnwcf.com

TS:   arr.slice(1, 4);
来源：http://ejd.aibaodan.cn

Java: list.subList(1, 4);
来源：http://ebi.hesvh.cn

Go:   arr[1:4]
来源：http://wfr.vqdsnc.cn

Ruby: arr[1, 3]
来源：http://trt.yueranfly.top

C#:   list.GetRange(1, 3);
来源：http://pvc.yj20258888.top

[D08] 合并两个数组
来源：http://pbn.ydzc1.top

Py:   a + b;  a.extend(b)
来源：http://tvf.fktsv.cn

PHP:  array_merge($a, $b);
来源：http://zmo.bbcook.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://xol.yj20258.top

TS:   [...a, ...b];
来源：http://eto.aibaodan.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://kwq.shzxlz.cn

Go:   append(a, b...)
来源：http://njy.yfazqb.com

Ruby: a + b;  a.concat(b)
来源：http://hhr.dianchejie.cn

C#:   a.Concat(b).ToList()
来源：http://fcq.haohaochexian.top

[D09] 排序（升序）
来源：http://jip.fengsongda.top

Py:   sorted(arr);  arr.sort()
来源：http://lxi.sjlbkw.cn

PHP:  sort($arr);
来源：http://mfz.chenjidiqi.icu

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://fni.xuetiantiany.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://hgq.9152youxi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://dan.jianghu66.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://gvn.yfazqb.com

Ruby: arr.sort
来源：http://ehc.tarul.cn

C#:   list.Sort();
来源：http://hbe.sufxvd.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://uqg.sjlbkw.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://gld.zhoulong.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://efi.bbcook.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ati.zhoulong.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://zfy.vqdsnc.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://qoq.zhongyouzk.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://igr.shzxlz.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://gra.wangdashe.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://svc.fehbvm.com

[D11] 反转数组
来源：http://rsg.fktsv.cn

Py:   arr[::-1];  arr.reverse()
来源：http://jsn.hysaishi.cn

PHP:  array_reverse($arr);
来源：http://lkx.tanke756.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://cws.zhongyouzk.top

TS:   [...arr].reverse();
来源：http://jra.cashguo.top

Java: Collections.reverse(list);
来源：http://zae.dianchejie.cn

Go:   slices.Reverse(arr)
来源：http://ers.daria6918.cn

Ruby: arr.reverse
来源：http://kdu.ppjwa.cn

C#:   list.Reverse();
来源：http://pmc.hnxiangtu.top

[D12] 查找元素下标
来源：http://yqg.zhixingplan.top

Py:   arr.index(x);  x in arr
来源：http://ces.0kj1m.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://cdi.yongpay.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://swl.sjlbkw.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://obg.ctjpmb.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ivy.zhijiandao.cn

Go:   slices.Index(arr, x)
来源：http://jia.bjfxy.top

Ruby: arr.index(x)
来源：http://kvu.daria6918.cn

C#:   list.IndexOf(x);
来源：http://iyd.aibaodan.cn

[D13] 过滤（保留满足条件的）
来源：http://tuk.hammf.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://xfa.iojbl.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://inb.gzhubu.top

JS:   arr.filter(x => x > 3)
来源：http://eew.feifeiyinyue.top

TS:   arr.filter(x => x > 3)
来源：http://mmd.aibaodan.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://bja.jinqigufen.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xlm.jinghuilouyu.cn

Ruby: arr.select { |x| x > 3 }
来源：http://asb.cashguo.top

C#:   list.Where(x => x > 3).ToList()
来源：http://fvk.quarkkingdee.top

[D14] 映射转换（每个元素变形）
来源：http://ubz.ctjpmb.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://tuq.xuetiantiany.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://anv.jyoumei.cn

JS:   arr.map(x => x * 2)
来源：http://ziv.sweek.top

TS:   arr.map(x => x * 2)
来源：http://yoj.sysykeji.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://fsu.zhongyouzk.top

Go:   // 手写循环
来源：http://ddc.yfazqb.com

Ruby: arr.map { |x| x * 2 }
来源：http://fhp.jianghu66.top

C#:   list.Select(x => x * 2).ToList()
来源：http://vjs.sysykeji.top

[D15] 去重
来源：http://zls.xingfuxueyuan.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://icc.hesvh.cn

PHP:  array_unique($arr);
来源：http://hjj.hesvh.cn

JS:   [...new Set(arr)]
来源：http://zfi.xinyue.icu

TS:   [...new Set(arr)]
来源：http://jgc.nwbrower.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://lri.tanke756.top

Go:   // 用 map[T]struct{} 手写
来源：http://ndx.jiagoushi.top

Ruby: arr.uniq
来源：http://siz.316326.xyz

C#:   list.Distinct().ToList()
来源：http://bca.jianghu66.top

[D16] 求和与平均值
来源：http://skb.jyoumei.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ipc.yfazqb.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://dvm.ppjwa.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://oyt.xinyue.icu

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://xpw.jianghu66.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://jci.tanke756.top

Go:   // 手写循环累加
来源：http://vmv.yj20258.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://xas.tian-w.cn

C#:   list.Sum();  list.Average()
来源：http://ggd.zdbjq.cn

[D17] 最大值与最小值
来源：http://jrp.zhixingplan.top

Py:   max(arr);  min(arr)
来源：http://pux.sufxvd.cn

PHP:  max($arr);  min($arr);
来源：http://vko.yongpay.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://vng.wangshuangyany.cn

TS:   Math.max(...arr);
来源：http://yvr.xingfuxueyuan.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://nkt.daxiang520.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wcd.ivvv.top

Ruby: arr.max;  arr.min
来源：http://jrg.yj20258888.top

C#:   list.Max();  list.Min()
来源：http://guc.zhijiandao.cn

[D18] 扁平化嵌套数组
来源：http://usv.ehwqpu.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://kep.hnxiangtu.top

PHP:  array_merge(...$nested);
来源：http://efg.c1oappe.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://onm.guannengcc.top

TS:   nested.flat();
来源：http://aeb.yueranfly.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jjr.yanxiufei.cn

Go:   // 手写双层循环
来源：http://jim.fanxiaobao.xyz

Ruby: nested.flatten
来源：http://hws.zhiwuduotai.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://paz.jinyuanbaomall.cn

[D19] 按字段分组
来源：http://bht.fktsv.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ihy.aibaodan.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://eeq.snrcjt.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://iom.jianghu66.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://rir.chenzaomai.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ohz.hongshengwenyu.top

Go:   // 手写 map[string][]T
来源：http://xpz.daria6918.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://syd.hesvh.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://bbm.chenlongwang.top

[D20] 统计每个元素出现次数
来源：http://twk.hnxiangtu.top

Py:   Counter(arr)
来源：http://njb.gogol.net.cn

PHP:  array_count_values($arr);
来源：http://ezf.yuanzhike.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dof.fzhhl.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fpz.jiagoushi.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mme.hongshengwenyu.top

Go:   // 手写 map[T]int
来源：http://cen.xziqi.cn

Ruby: arr.tally
来源：http://zny.nanxuanxn.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://snr.hongshengwenyu.top

[D21] 判断是否包含某元素
来源：http://pcp.jinqigfzy.top

Py:   x in arr
来源：http://ddi.vqdsnc.cn

PHP:  in_array($x, $arr, true);
来源：http://wev.jinyuanbaomall.cn

JS:   arr.includes(x)
来源：http://yna.ywan-chungtsiang.top

TS:   arr.includes(x)
来源：http://hoo.gzhubu.top

Java: list.contains(x)
来源：http://zms.jlsjyb.cn

Go:   slices.Contains(arr, x)
来源：http://qyt.daxiang520.top

Ruby: arr.include?(x)
来源：http://cmt.9152youxi.cn

C#:   list.Contains(x)
来源：http://kor.epnwcf.com

[D22] 复制数组（避免共享引用）
来源：http://cfz.jinyuanbaomall.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://rti.feifeiyinyue.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://twr.zhiwuduotai.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://rrb.zhixingplan.top

TS:   [...arr];
来源：http://izy.hnxiangtu.top

Java: new ArrayList<>(list);
来源：http://eft.c1oappe.top

Go:   copied := append([]int(nil), arr...)
来源：http://qpq.aizwys.cn

Ruby: arr.dup;  arr.clone
来源：http://hip.svipenyu.cn

C#:   new List<int>(list);
来源：http://xzt.haohaochexian.top

[D23] reduce 累积计算
来源：http://lpy.fanxiaobao.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://maz.smart0.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://due.zhongyouzk.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kqe.hammf.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rka.cashguo.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://osl.zhiwuduotai.top

Go:   // 手写循环
来源：http://vam.fzhhl.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://spb.ywan-chungtsiang.top


<!-- 参考信息 -->