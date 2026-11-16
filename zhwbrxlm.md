代发 wailian999

Ruby: arr.map(&:upcase)
来源：http://vdd.ehwqpu.com

C#:   arr.Select(s => s.ToUpper())
来源：http://mun.yj20258888.top

[C08] 闭包
来源：http://vgq.havefunace.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://yge.pengpengdd.cyou

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ocx.hnqzz.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://iyq.sweek.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://xnm.vehdjk.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wgn.svipenyu.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://uno.cheryme.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://jii.nanxuanxn.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://szl.yj20258888.top

[C09] 递归
来源：http://wrl.jyoumei.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ylb.smart0.xyz

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://bmd.zhengqikj.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://edg.zdqjudy.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ype.yuxming.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://uxn.fktsv.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://keq.dashuyun.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://cxu.yfazqb.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://doo.shanyushiyangkeji.top

[C10] 变量作用域
来源：http://lex.gzhubu.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://jpg.aizwys.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://kqt.yuxming.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://fcf.ctjpmb.com

TS:   同 JS
来源：http://nee.ppjwa.cn

Java: 方法内为块级作用域
来源：http://ucn.gogol.net.cn

Go:   花括号块级作用域
来源：http://aom.zhijiandao.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://zos.zdqjudy.top

C#:   块级作用域
来源：http://vlj.daxiang520.top

[C11] 模块导入与导出
来源：http://sxs.yuxming.cn

Py:   from module import func
来源：http://xxr.zhixingplan.top

PHP:  require "file.php";  或 use App\Service;
来源：http://ddm.fktsv.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://cku.zdbjq.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ssv.fanxiaobao.xyz

Java: import java.util.List;
来源：http://ovf.zhaomingkeji.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wsl.0kj1m.cn

Ruby: require "json"; require_relative "./util"
来源：http://dnl.ybcxt.top

C#:   using System.Text;
来源：http://jza.jianghu66.top

[C12] 立即执行函数 IIFE
来源：http://hgz.uphjek.com

Py:   (lambda: print("run"))()
来源：http://gip.hnqzz.top

PHP:  (function () { echo "run"; })();
来源：http://mii.xziqi.cn

JS:   (() => { console.log("run"); })();
来源：http://vom.cucudq.cn

TS:   (() => { console.log("run"); })();
来源：http://gjb.mhx1999.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mhm.xuanzx.com

Go:   func() { fmt.Println("run") }()
来源：http://gku.smart0.xyz

Ruby: -> { puts "run" }.call
来源：http://qcx.ivvv.top

C#:   // 无 IIFE：用静态构造函数
来源：http://vuf.zdqjudy.top

[C13] 类型声明 / 类型注解
来源：http://yuh.yangfankeji.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://klo.hongshengwenyu.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://raz.jinyuanbaomall.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://sij.vqdsnc.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hdq.zdbjq.cn

Java: int add(int a, int b) { return a + b; }
来源：http://khz.sweek.top

Go:   func add(a, b int) int
来源：http://jqb.shuidangran.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://sip.tanke756.top

C#:   int Add(int a, int b) => a + b;
来源：http://dag.yangfankeji.com

[C14] 泛型函数
来源：http://xfa.yanxiufei.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://eag.shanyushiyangtech.top

PHP:  // 无泛型
来源：http://uha.epnwcf.com

JS:   // 无泛型
来源：http://csd.nwbrower.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://tzq.shangyingyoupin.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://tok.andypj.xyz

Go:   func First[T any](items []T) T { return items[0] }
来源：http://eaw.jinqigfzy.top

Ruby: # 无泛型
来源：http://aam.nwbrower.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://dae.fengsongda.top

[C15] 解构 / 展开参数
来源：http://sop.daxiang520.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ify.hysaishi.cn

PHP:  [$a, $b] = $pair;
来源：http://rcg.aibaodan.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xyj.ydzc1.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://huy.bbcook.cn

Java: // 无解构
来源：http://oty.ppjwa.cn

Go:   // 无解构
来源：http://fhl.cashguo.top

Ruby: a, b = pair
来源：http://onh.zycfv.cn

C#:   var (a, b) = pair;
来源：http://pys.wangdashe.top

[C16] 函数 / 方法重载
来源：http://aoo.aibaodan.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://rlf.hammf.cn

PHP:  // 无重载
来源：http://ehm.shanyushiyangtech.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://rxq.tianlin.xyz

TS:   // 用联合类型或重载签名声明
来源：http://vvi.ydjk.org.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://rop.ivvv.top

Go:   // 无重载：用不同函数名
来源：http://pnq.aizwys.cn

Ruby: # 无重载：靠动态参数
来源：http://ptu.zhijiandao.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://yvm.dashuyun.cn

================================================================================
来源：http://eok.dashuyun.cn

D. 数组 / 列表 / 集合
来源：http://axl.jinqigfzy.top

================================================================================
来源：http://mbe.sjlbkw.cn

[D01] 创建数组 / 列表
来源：http://ooe.jyoumei.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://aub.tanke756.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hqp.jyoumei.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://chp.gotoacloud.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://zfw.jlsjyb.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://qto.dianchejie.cn

Go:   arr := []int{1, 2, 3}
来源：http://crn.ydjk.org.cn

Ruby: arr = [1, 2, 3]
来源：http://nsv.ehwqpu.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ouk.kuanghao11.cn

[D02] 追加元素到末尾
来源：http://rpz.jqgufenzy.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://biw.cashguo.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://jzg.yj20258888.top

JS:   arr.push(4);
来源：http://qcg.yueranfly.top

TS:   arr.push(4);
来源：http://pbm.quarkkingdee.top

Java: list.add(4);
来源：http://irb.zycfv.cn

Go:   arr = append(arr, 4)
来源：http://nqj.zycfv.cn

Ruby: arr << 4; arr.push(5)
来源：http://jmg.zhoulong.xyz

C#:   list.Add(4);
来源：http://qap.iojbl.cn

[D03] 在指定位置插入元素
来源：http://maa.yvedp.cn

Py:   arr.insert(0, 0)
来源：http://wtw.ehwqpu.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ois.nwbrower.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://tiy.sysykeji.top

TS:   arr.splice(0, 0, 0);
来源：http://hxq.fengsongda.top

Java: list.add(0, 0);
来源：http://eem.cashguo.top

Go:   arr = append([]int{0}, arr...)
来源：http://qmn.uphjek.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://olm.tianlin.xyz

C#:   list.Insert(0, 0);
来源：http://hqd.nwbrower.top

[D04] 删除元素
来源：http://uox.yanxiufei.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ylo.dashuyun.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mrq.aibaodan.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wtf.iojbl.cn

TS:   arr.splice(0, 1);
来源：http://wpa.nwbrower.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://are.yonumen.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wbj.yangfankeji.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mpq.zhongyouzk.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://rhu.zhoulong.xyz

[D05] 访问与修改元素
来源：http://cxk.xuetiantiany.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://cig.yuxming.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ste.gzhubu.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://igg.chenzaomai.com

TS:   arr[0]; arr.at(-1);
来源：http://zse.gaohongyu789.top

Java: list.get(0); list.set(0, 9);
来源：http://cer.ybcxt.top

Go:   arr[0]; arr[0] = 9
来源：http://usy.havefunace.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mdh.jinqigfzy.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ftg.yanxiufei.cn

[D06] 数组长度
来源：http://aeq.yvedp.cn

Py:   len(arr)
来源：http://tae.ivvv.top

PHP:  count($arr);
来源：http://ndj.zhixingplan.top

JS:   arr.length
来源：http://lup.tianlin.xyz

TS:   arr.length
来源：http://bpu.nanxinkj.top

Java: list.size();
来源：http://fnz.pycfn.com

Go:   len(arr)
来源：http://kfe.fktsv.cn

Ruby: arr.length; arr.size
来源：http://kbr.quarkkingdee.top

C#:   list.Count;
来源：http://ozn.shanyushiyangtech.top

[D07] 切片 / 取子数组
来源：http://rpr.zhiwuduotai.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://lwg.kuanghao11.cn

PHP:  array_slice($arr, 1, 3);
来源：http://acg.daxiang520.top

JS:   arr.slice(1, 4);
来源：http://kiq.sweek.top

TS:   arr.slice(1, 4);
来源：http://znz.shanyushiyangkeji.top

Java: list.subList(1, 4);
来源：http://hkw.yongpay.top

Go:   arr[1:4]
来源：http://juo.daria6918.cn

Ruby: arr[1, 3]
来源：http://dcr.jinqigfzy.top

C#:   list.GetRange(1, 3);
来源：http://lwt.cheryme.top

[D08] 合并两个数组
来源：http://zfc.zhijiandao.cn

Py:   a + b;  a.extend(b)
来源：http://vrq.hnqzz.top

PHP:  array_merge($a, $b);
来源：http://fxq.cucudq.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://odk.52xcode.cn

TS:   [...a, ...b];
来源：http://sds.ywan-chungtsiang.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ngo.jinghuilouyu.cn

Go:   append(a, b...)
来源：http://atw.jinqigufen.top

Ruby: a + b;  a.concat(b)
来源：http://sgk.tarul.cn

C#:   a.Concat(b).ToList()
来源：http://ogm.hfpthk.cn

[D09] 排序（升序）
来源：http://jii.nanxinkj.top

Py:   sorted(arr);  arr.sort()
来源：http://dyh.jqgfzy.top

PHP:  sort($arr);
来源：http://bxi.yueranfly.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://cda.hfpthk.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://tef.ywan-chungtsiang.top

Java: Collections.sort(list);  list.sort(null);
来源：http://vov.zhengqikj.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://jje.fzhhl.top

Ruby: arr.sort
来源：http://knl.zhixingplan.top

C#:   list.Sort();
来源：http://mtc.xuanzx.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://yea.guowangkeji.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://tdf.fzhhl.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qjs.tarul.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://krd.gaohongyu789.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fgf.jinqigufen.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://goa.hesvh.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://vfz.yongpay.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://paj.chenjidiqi.icu

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mkx.zycfv.cn

[D11] 反转数组
来源：http://uqc.shanyushiyangkeji.top

Py:   arr[::-1];  arr.reverse()
来源：http://uki.zhiwuduotai.top

PHP:  array_reverse($arr);
来源：http://whl.316326.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://bie.c1oappe.top

TS:   [...arr].reverse();
来源：http://thf.nanxinkj.top

Java: Collections.reverse(list);
来源：http://joj.tanke756.top

Go:   slices.Reverse(arr)
来源：http://xmq.316326.xyz

Ruby: arr.reverse
来源：http://mji.9152youxi.cn

C#:   list.Reverse();
来源：http://etg.gzhubu.top

[D12] 查找元素下标
来源：http://geu.yueranfly.top

Py:   arr.index(x);  x in arr
来源：http://zcu.bjfxy.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://dsz.jinyuanbaomall.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yee.zhengqikj.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://amu.52xcode.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wzw.jinqigfzy.top

Go:   slices.Index(arr, x)
来源：http://xsb.chenlongwang.top

Ruby: arr.index(x)
来源：http://zhz.xuanzx.com

C#:   list.IndexOf(x);
来源：http://qjo.ybcxt.top

[D13] 过滤（保留满足条件的）
来源：http://amv.fanxiaobao.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://gim.snrcjt.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://xwq.jqgfzy.top

JS:   arr.filter(x => x > 3)
来源：http://zlo.zhaomingkeji.xyz

TS:   arr.filter(x => x > 3)
来源：http://bfo.sweek.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ihg.wangdashe.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hfh.pycfn.com

Ruby: arr.select { |x| x > 3 }
来源：http://nsl.ywan-chungtsiang.top

C#:   list.Where(x => x > 3).ToList()
来源：http://wsl.yangfankeji.com

[D14] 映射转换（每个元素变形）
来源：http://dsn.tian-w.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://whw.chenzaomai.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://gcu.pycfn.com

JS:   arr.map(x => x * 2)
来源：http://seb.tanke756.top

TS:   arr.map(x => x * 2)
来源：http://mup.tanke756.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://lmw.52xcode.cn

Go:   // 手写循环
来源：http://rua.hnqzz.top

Ruby: arr.map { |x| x * 2 }
来源：http://jjz.cucudq.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://daf.guannengcc.top

[D15] 去重
来源：http://qzl.hfpthk.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://war.yuxming.cn

PHP:  array_unique($arr);
来源：http://xpn.hammf.cn

JS:   [...new Set(arr)]
来源：http://qrn.kuanghao11.cn

TS:   [...new Set(arr)]
来源：http://bth.sweek.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://jqb.zhengqikj.top

Go:   // 用 map[T]struct{} 手写
来源：http://tiu.sxryk.cn

Ruby: arr.uniq
来源：http://mqw.jqgfzy.top

C#:   list.Distinct().ToList()
来源：http://hqs.fehbvm.com

[D16] 求和与平均值
来源：http://kzl.xuanzx.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qtq.smart0.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ddj.chenlongwang.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ypg.jqgufenzy.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://bip.pengpengdd.cyou

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://pbr.bjfxy.top

Go:   // 手写循环累加
来源：http://axa.zdbjq.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ezd.sufxvd.cn

C#:   list.Sum();  list.Average()
来源：http://wwd.meibo888.top

[D17] 最大值与最小值
来源：http://sku.iojbl.cn

Py:   max(arr);  min(arr)
来源：http://kzz.feifeiyinyue.top

PHP:  max($arr);  min($arr);
来源：http://rff.hesvh.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://nvv.epnwcf.com

TS:   Math.max(...arr);
来源：http://zjs.cucudq.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://hwy.cdnleiting.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://nka.zycfv.cn

Ruby: arr.max;  arr.min
来源：http://twh.zhongyouzk.top

C#:   list.Max();  list.Min()
来源：http://byx.yangfankeji.com

[D18] 扁平化嵌套数组
来源：http://zaq.zhaomingkeji.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://tws.cdnleiting.top

PHP:  array_merge(...$nested);
来源：http://trk.tian-w.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wpc.gotoacloud.top

TS:   nested.flat();
来源：http://hoj.gotoacloud.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://enc.yj20258.top

Go:   // 手写双层循环
来源：http://sfc.feifeiyinyue.top

Ruby: nested.flatten
来源：http://gru.sweek.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://ndm.jinghuilouyu.cn

[D19] 按字段分组
来源：http://paa.smart0.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://usx.yangfankeji.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ujo.dianchejie.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://aum.hnxiangtu.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://uom.gzhubu.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mpf.sysykeji.top

Go:   // 手写 map[string][]T
来源：http://ojv.zhiwuduotai.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://yvo.snrcjt.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://dyx.havefunace.top

[D20] 统计每个元素出现次数
来源：http://yix.vehdjk.com

Py:   Counter(arr)
来源：http://sje.hongshengwenyu.top

PHP:  array_count_values($arr);
来源：http://ste.xinyue.icu

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fby.tanke756.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nik.jinqigufen.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://clu.xuanzx.com

Go:   // 手写 map[T]int
来源：http://cxc.fzhhl.top

Ruby: arr.tally
来源：http://ojo.gaohongyu789.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://rqd.xziqi.cn

[D21] 判断是否包含某元素
来源：http://nlr.zhiwuduotai.top

Py:   x in arr
来源：http://iyk.meibo888.top

PHP:  in_array($x, $arr, true);
来源：http://zso.epnwcf.com

JS:   arr.includes(x)
来源：http://ynb.gaohongyu789.top

TS:   arr.includes(x)
来源：http://uhr.zhiwuduotai.top

Java: list.contains(x)
来源：http://bof.bbcook.cn

Go:   slices.Contains(arr, x)
来源：http://enc.fzhhl.top

Ruby: arr.include?(x)
来源：http://xyh.gzhubu.top

C#:   list.Contains(x)
来源：http://jnt.sysykeji.top

[D22] 复制数组（避免共享引用）
来源：http://yop.cqqwz.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://omi.yongpay.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://rmb.chenlongwang.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://xui.ydzc1.top

TS:   [...arr];
来源：http://ree.zhongyouzk.top

Java: new ArrayList<>(list);
来源：http://avt.vqdsnc.cn

Go:   copied := append([]int(nil), arr...)
来源：http://keb.xziqi.cn

Ruby: arr.dup;  arr.clone
来源：http://vbl.zhijiandao.cn

C#:   new List<int>(list);
来源：http://sxq.snrcjt.cn

[D23] reduce 累积计算
来源：http://mcp.mhx1999.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://cqd.zhongyouzk.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://eog.meibo888.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fhp.snrcjt.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zub.yueranfly.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://uvy.zhongyouzk.top

Go:   // 手写循环
来源：http://bct.ywan-chungtsiang.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://dtc.guannengcc.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wvc.tarul.cn

[D24] 字典 / Map 基本操作
来源：http://rbj.shuidangran.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://cgx.hongshengwenyu.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://jph.zhaomingkeji.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://pwd.zdbjq.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mlk.gogol.net.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://lyx.yueranfly.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://fhs.guowangkeji.top


<!-- 参考信息 -->