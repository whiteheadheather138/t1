代发 wailian999

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://iik.xylfe.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://iaq.yuxming.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wrm.fehbvm.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://pnn.0kj1m.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://afl.316326.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ron.fengsongda.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://kxa.uphjek.com

[C09] 递归
来源：http://jtj.havefunace.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://yns.zhijiandao.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://kai.dashuyun.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jro.9152youxi.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vlg.ivvv.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ucj.jianghu66.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://qpy.hysaishi.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://est.nwbrower.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://rbd.snrcjt.cn

[C10] 变量作用域
来源：http://qcy.sysykeji.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://pwa.pengpengdd.cyou

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://rdw.shangyingyoupin.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wmm.nwbrower.top

TS:   同 JS
来源：http://vxl.jqgufenzy.top

Java: 方法内为块级作用域
来源：http://qjy.fehbvm.com

Go:   花括号块级作用域
来源：http://azu.yonumen.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xeb.zhijiandao.cn

C#:   块级作用域
来源：http://lom.cucudq.cn

[C11] 模块导入与导出
来源：http://hxt.xingfuxueyuan.xyz

Py:   from module import func
来源：http://lvs.yongpay.top

PHP:  require "file.php";  或 use App\Service;
来源：http://ost.pycfn.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://noa.ywan-chungtsiang.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ozz.pengpengdd.cyou

Java: import java.util.List;
来源：http://kwq.tian-w.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://nax.sxryk.cn

Ruby: require "json"; require_relative "./util"
来源：http://ncv.hammf.cn

C#:   using System.Text;
来源：http://sym.jinghuilouyu.cn

[C12] 立即执行函数 IIFE
来源：http://jxg.ydzc1.top

Py:   (lambda: print("run"))()
来源：http://pgw.zdqjudy.top

PHP:  (function () { echo "run"; })();
来源：http://ipj.sxryk.cn

JS:   (() => { console.log("run"); })();
来源：http://nsh.hfpthk.cn

TS:   (() => { console.log("run"); })();
来源：http://fkq.zhoulong.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://sud.shangyingyoupin.top

Go:   func() { fmt.Println("run") }()
来源：http://okh.sjlbkw.cn

Ruby: -> { puts "run" }.call
来源：http://vlv.bjfxy.top

C#:   // 无 IIFE：用静态构造函数
来源：http://pyt.316326.xyz

[C13] 类型声明 / 类型注解
来源：http://tas.jianghu66.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://frz.hnxiangtu.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://asg.fengsongda.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://jnw.sjlbkw.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rbw.andypj.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://uxj.pengpengdd.cyou

Go:   func add(a, b int) int
来源：http://euh.hfpthk.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://muf.dashuyun.cn

C#:   int Add(int a, int b) => a + b;
来源：http://pee.tarul.cn

[C14] 泛型函数
来源：http://whi.ybcxt.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://lkt.daria6918.cn

PHP:  // 无泛型
来源：http://qye.pycfn.com

JS:   // 无泛型
来源：http://fma.316326.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ntv.gogol.net.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hpy.hnxiangtu.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://khu.aizwys.cn

Ruby: # 无泛型
来源：http://wcc.fzhhl.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ist.shanyushiyangtech.top

[C15] 解构 / 展开参数
来源：http://jqp.yj20258888.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ynt.sysykeji.top

PHP:  [$a, $b] = $pair;
来源：http://tky.shuidangran.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://tup.bbcook.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://pim.fengsongda.top

Java: // 无解构
来源：http://cnk.zdbjq.cn

Go:   // 无解构
来源：http://lsu.jinghuilouyu.cn

Ruby: a, b = pair
来源：http://jqp.guannengcc.top

C#:   var (a, b) = pair;
来源：http://iwb.pycfn.com

[C16] 函数 / 方法重载
来源：http://tbm.daxiang520.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://gxz.sjlbkw.cn

PHP:  // 无重载
来源：http://bgs.yvedp.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ljz.wangshuangyany.cn

TS:   // 用联合类型或重载签名声明
来源：http://txc.316326.xyz

Java: void f(int a) {}  void f(String a) {}
来源：http://rmi.c1oappe.top

Go:   // 无重载：用不同函数名
来源：http://cub.jqgufenzy.top

Ruby: # 无重载：靠动态参数
来源：http://byj.bbcook.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://yds.uphjek.com

================================================================================
来源：http://ebc.guowangkeji.top

D. 数组 / 列表 / 集合
来源：http://jld.yfazqb.com

================================================================================
来源：http://hnl.shuidangran.top

[D01] 创建数组 / 列表
来源：http://mme.hesvh.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://uzh.jlsjyb.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mmr.cheryme.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://tbg.mhx1999.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://tvg.havefunace.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://whr.yj20258888.top

Go:   arr := []int{1, 2, 3}
来源：http://rqt.pengpengdd.cyou

Ruby: arr = [1, 2, 3]
来源：http://ecm.hammf.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://tyf.dianchejie.cn

[D02] 追加元素到末尾
来源：http://xal.chenjidiqi.icu

Py:   arr.append(4); arr.extend([5, 6])
来源：http://lcx.vqdsnc.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://psz.daxiang520.top

JS:   arr.push(4);
来源：http://mkn.yfazqb.com

TS:   arr.push(4);
来源：http://rsi.sweek.top

Java: list.add(4);
来源：http://uru.yvedp.cn

Go:   arr = append(arr, 4)
来源：http://eey.snrcjt.cn

Ruby: arr << 4; arr.push(5)
来源：http://cir.shzxlz.cn

C#:   list.Add(4);
来源：http://siw.bbcook.cn

[D03] 在指定位置插入元素
来源：http://owc.havefunace.top

Py:   arr.insert(0, 0)
来源：http://ift.fehbvm.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://oum.snrcjt.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://pld.quarkkingdee.top

TS:   arr.splice(0, 0, 0);
来源：http://vau.fehbvm.com

Java: list.add(0, 0);
来源：http://coz.dianchejie.cn

Go:   arr = append([]int{0}, arr...)
来源：http://yqt.redwolf501.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://vjl.quarkkingdee.top

C#:   list.Insert(0, 0);
来源：http://rxu.ydjk.org.cn

[D04] 删除元素
来源：http://uhc.snrcjt.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wmp.zdqjudy.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://htt.hnqzz.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ann.jlsjyb.cn

TS:   arr.splice(0, 1);
来源：http://ype.epnwcf.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://std.sysykeji.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ttw.tian-w.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://rzl.hfpthk.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://lyf.9152youxi.cn

[D05] 访问与修改元素
来源：http://vca.hysaishi.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://tja.c1oappe.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://olx.zhiwuduotai.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://vrm.kuanghao11.cn

TS:   arr[0]; arr.at(-1);
来源：http://wvv.ppjwa.cn

Java: list.get(0); list.set(0, 9);
来源：http://rhu.jiagoushi.top

Go:   arr[0]; arr[0] = 9
来源：http://cwc.nanxuanxn.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wge.aizwys.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://rul.jlsjyb.cn

[D06] 数组长度
来源：http://cof.jinghuilouyu.cn

Py:   len(arr)
来源：http://reg.0kj1m.cn

PHP:  count($arr);
来源：http://tpm.iojbl.cn

JS:   arr.length
来源：http://jwm.pengpengdd.cyou

TS:   arr.length
来源：http://eom.shuidangran.top

Java: list.size();
来源：http://wri.vqdsnc.cn

Go:   len(arr)
来源：http://ilg.ydjk.org.cn

Ruby: arr.length; arr.size
来源：http://jsg.bbcook.cn

C#:   list.Count;
来源：http://xbb.ywan-chungtsiang.top

[D07] 切片 / 取子数组
来源：http://rlu.ctjpmb.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ntv.cdnleiting.top

PHP:  array_slice($arr, 1, 3);
来源：http://utx.svipenyu.cn

JS:   arr.slice(1, 4);
来源：http://gpj.zhongyouzk.top

TS:   arr.slice(1, 4);
来源：http://hop.jyoumei.cn

Java: list.subList(1, 4);
来源：http://gad.yongpay.top

Go:   arr[1:4]
来源：http://kjn.wangshuangyany.cn

Ruby: arr[1, 3]
来源：http://yyn.zhaomingkeji.xyz

C#:   list.GetRange(1, 3);
来源：http://tju.aizwys.cn

[D08] 合并两个数组
来源：http://wii.ctjpmb.com

Py:   a + b;  a.extend(b)
来源：http://tjx.yfazqb.com

PHP:  array_merge($a, $b);
来源：http://yuf.nwbrower.top

JS:   [...a, ...b];  a.concat(b);
来源：http://nfa.guannengcc.top

TS:   [...a, ...b];
来源：http://ssf.dashuyun.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://gpd.zdbjq.cn

Go:   append(a, b...)
来源：http://tjq.sweek.top

Ruby: a + b;  a.concat(b)
来源：http://ijs.ppjwa.cn

C#:   a.Concat(b).ToList()
来源：http://aeq.ppjwa.cn

[D09] 排序（升序）
来源：http://ifv.jinqigufen.top

Py:   sorted(arr);  arr.sort()
来源：http://bho.zhiwuduotai.top

PHP:  sort($arr);
来源：http://vfs.daxiang520.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://jku.cheryme.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://gon.yanxiufei.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://fam.zhoulong.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ppn.ivvv.top

Ruby: arr.sort
来源：http://mkd.yonumen.top

C#:   list.Sort();
来源：http://wnn.guowangkeji.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://akp.zhengqikj.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://xjj.jqgfzy.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dyt.yanxiufei.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://rbi.tian-w.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fwh.snrcjt.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://rhy.wangdashe.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ofc.cdnleiting.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://zqi.chenzaomai.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://kgs.daxiang520.top

[D11] 反转数组
来源：http://bka.yj20258.top

Py:   arr[::-1];  arr.reverse()
来源：http://nxa.yj20258888.top

PHP:  array_reverse($arr);
来源：http://zmq.yuxming.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://rli.mhx1999.top

TS:   [...arr].reverse();
来源：http://efl.pengpengdd.cyou

Java: Collections.reverse(list);
来源：http://hnb.redwolf501.top

Go:   slices.Reverse(arr)
来源：http://psj.9152youxi.cn

Ruby: arr.reverse
来源：http://nsn.wangdashe.top

C#:   list.Reverse();
来源：http://uuz.andypj.xyz

[D12] 查找元素下标
来源：http://wly.hnxiangtu.top

Py:   arr.index(x);  x in arr
来源：http://zeo.haohaochexian.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://uwh.yanxiufei.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ofc.jinyuanbaomall.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gxt.yangfankeji.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://szw.52xcode.cn

Go:   slices.Index(arr, x)
来源：http://gdg.hcnkem.com

Ruby: arr.index(x)
来源：http://djj.daxiang520.top

C#:   list.IndexOf(x);
来源：http://twr.svipenyu.cn

[D13] 过滤（保留满足条件的）
来源：http://gmo.c1oappe.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://bvu.kuanghao11.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://vap.fanxiaobao.xyz

JS:   arr.filter(x => x > 3)
来源：http://fiy.jqgufenzy.top

TS:   arr.filter(x => x > 3)
来源：http://anx.sxryk.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://pvk.sufxvd.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://dip.yvedp.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ncv.yj20258888.top

C#:   list.Where(x => x > 3).ToList()
来源：http://roy.guowangkeji.top

[D14] 映射转换（每个元素变形）
来源：http://vpf.epnwcf.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://upv.yueranfly.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://owt.wangshuangyany.cn

JS:   arr.map(x => x * 2)
来源：http://ryn.jqgfzy.top

TS:   arr.map(x => x * 2)
来源：http://wxo.yonumen.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://aee.hammf.cn

Go:   // 手写循环
来源：http://cld.fehbvm.com

Ruby: arr.map { |x| x * 2 }
来源：http://fde.hfpthk.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://rgo.shangyingyoupin.top

[D15] 去重
来源：http://qhj.feifeiyinyue.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://tfo.fktsv.cn

PHP:  array_unique($arr);
来源：http://diq.pycfn.com

JS:   [...new Set(arr)]
来源：http://czo.aizwys.cn

TS:   [...new Set(arr)]
来源：http://okv.vehdjk.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://yjt.smart0.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://ywz.quarkkingdee.top

Ruby: arr.uniq
来源：http://egc.fengsongda.top

C#:   list.Distinct().ToList()
来源：http://fld.gaohongyu789.top

[D16] 求和与平均值
来源：http://rgc.smart0.xyz

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://grw.gzhubu.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://aiv.snrcjt.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://vct.xziqi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://aef.tianlin.xyz

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ouq.xziqi.cn

Go:   // 手写循环累加
来源：http://iwe.zdqjudy.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ocs.fanxiaobao.xyz

C#:   list.Sum();  list.Average()
来源：http://vut.quarkkingdee.top

[D17] 最大值与最小值
来源：http://gos.chenzaomai.com

Py:   max(arr);  min(arr)
来源：http://pot.sysykeji.top

PHP:  max($arr);  min($arr);
来源：http://aot.tarul.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://uxc.guowangkeji.top

TS:   Math.max(...arr);
来源：http://hhs.quarkkingdee.top

Java: Collections.max(list);  Collections.min(list);
来源：http://xst.zhongyouzk.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://yle.jlsjyb.cn

Ruby: arr.max;  arr.min
来源：http://iaj.nanxuanxn.top

C#:   list.Max();  list.Min()
来源：http://nji.zhixingplan.top

[D18] 扁平化嵌套数组
来源：http://acd.jinqigfzy.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://fmc.sjlbkw.cn

PHP:  array_merge(...$nested);
来源：http://ewi.havefunace.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://byd.bbcook.cn

TS:   nested.flat();
来源：http://cce.shangyingyoupin.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ccf.tanke756.top

Go:   // 手写双层循环
来源：http://hyq.zhaomingkeji.xyz

Ruby: nested.flatten
来源：http://qje.0kj1m.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://jga.shanyushiyangkeji.top

[D19] 按字段分组
来源：http://wbd.9152youxi.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://fpf.316326.xyz

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://xfx.hesvh.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://uvq.havefunace.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://kty.xingfuxueyuan.xyz

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://rae.hnxiangtu.top

Go:   // 手写 map[string][]T
来源：http://git.sweek.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://aun.nwbrower.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wjt.pycfn.com

[D20] 统计每个元素出现次数
来源：http://lcq.fehbvm.com

Py:   Counter(arr)
来源：http://rfz.gzhubu.top

PHP:  array_count_values($arr);
来源：http://eub.shangyingyoupin.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ixu.jqgfzy.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jxj.fanxiaobao.xyz

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ise.quarkkingdee.top

Go:   // 手写 map[T]int
来源：http://mkn.andypj.xyz

Ruby: arr.tally
来源：http://ccy.9152youxi.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://abi.tian-w.cn

[D21] 判断是否包含某元素
来源：http://ofd.yj202588.top

Py:   x in arr
来源：http://cnx.zhongyouzk.top

PHP:  in_array($x, $arr, true);
来源：http://dpn.hesvh.cn

JS:   arr.includes(x)
来源：http://zhm.haohaochexian.top

TS:   arr.includes(x)
来源：http://oun.jqgfzy.top

Java: list.contains(x)
来源：http://gnn.jinghuilouyu.cn

Go:   slices.Contains(arr, x)
来源：http://iyq.smart0.xyz

Ruby: arr.include?(x)
来源：http://van.nanxinkj.top

C#:   list.Contains(x)
来源：http://yds.jiagoushi.top

[D22] 复制数组（避免共享引用）
来源：http://wdy.jyoumei.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wot.nwbrower.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://bbn.fengsongda.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://uaa.yfazqb.com

TS:   [...arr];
来源：http://niz.cheryme.top

Java: new ArrayList<>(list);
来源：http://jxa.snrcjt.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ohv.xingfuxueyuan.xyz

Ruby: arr.dup;  arr.clone
来源：http://yxl.yangfankeji.com

C#:   new List<int>(list);
来源：http://cxl.hfpthk.cn

[D23] reduce 累积计算
来源：http://fyt.hnxiangtu.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://qvu.cqqwz.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://tjf.gzhubu.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://byv.yj202588.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qdo.pengpengdd.cyou

Java: list.stream().reduce(0, Integer::sum)
来源：http://axy.uphjek.com

Go:   // 手写循环
来源：http://dig.fzhhl.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://brv.jinqigfzy.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://pxj.epnwcf.com

[D24] 字典 / Map 基本操作
来源：http://rbb.yvedp.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://djf.cdnleiting.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qts.sxryk.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mch.yongpay.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://sdm.cqqwz.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://lnm.haohaochexian.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://gmf.zdbjq.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mel.cucudq.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ead.sysykeji.top

[D25] Set 集合去重与交并差
来源：http://nth.tianlin.xyz

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://zdv.xinyue.icu


<!-- 参考信息 -->