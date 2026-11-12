代发 wailian999

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://dzg.tanke756.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ref.epnwcf.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://deg.zycfv.cn

[C09] 递归
来源：http://ijl.jinghuilouyu.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://sxs.svipenyu.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://uko.nanxinkj.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gvg.birdmap.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xcn.sweek.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ikh.xziqi.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mdz.jyoumei.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://zmz.316326.xyz

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ory.smart0.xyz

[C10] 变量作用域
来源：http://qhf.svipenyu.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://joe.mhx1999.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://jdj.tarul.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://kzg.fehbvm.com

TS:   同 JS
来源：http://com.zhongyouzk.top

Java: 方法内为块级作用域
来源：http://csu.havefunace.top

Go:   花括号块级作用域
来源：http://bpk.wangshuangyany.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ido.yanxiufei.cn

C#:   块级作用域
来源：http://bzr.yongpay.top

[C11] 模块导入与导出
来源：http://woo.yj20258.top

Py:   from module import func
来源：http://zgh.aizwys.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://nsd.svipenyu.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://uap.hnqzz.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://opx.sweek.top

Java: import java.util.List;
来源：http://jsg.tian-w.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://cke.wangdashe.top

Ruby: require "json"; require_relative "./util"
来源：http://wdv.jiagoushi.top

C#:   using System.Text;
来源：http://unz.yuanzhike.top

[C12] 立即执行函数 IIFE
来源：http://dpo.c1oappe.top

Py:   (lambda: print("run"))()
来源：http://nec.hnqzz.top

PHP:  (function () { echo "run"; })();
来源：http://uka.hfpthk.cn

JS:   (() => { console.log("run"); })();
来源：http://abs.iojbl.cn

TS:   (() => { console.log("run"); })();
来源：http://sbe.sjlbkw.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://fif.ivvv.top

Go:   func() { fmt.Println("run") }()
来源：http://keq.ydjk.org.cn

Ruby: -> { puts "run" }.call
来源：http://ucg.gotoacloud.top

C#:   // 无 IIFE：用静态构造函数
来源：http://tdc.feifeiyinyue.top

[C13] 类型声明 / 类型注解
来源：http://daz.sjlbkw.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://eht.vehdjk.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nkf.mhx1999.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://sjf.fktsv.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pil.iojbl.cn

Java: int add(int a, int b) { return a + b; }
来源：http://fpq.jinqigfzy.top

Go:   func add(a, b int) int
来源：http://ytc.gaohongyu789.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://bgh.xylfe.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ele.uphjek.com

[C14] 泛型函数
来源：http://vxi.epnwcf.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://fue.daria6918.cn

PHP:  // 无泛型
来源：http://mnr.daxiang520.top

JS:   // 无泛型
来源：http://vjb.cqqwz.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ddv.chenzaomai.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://xqk.9152youxi.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://spr.yongpay.top

Ruby: # 无泛型
来源：http://lpp.sufxvd.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://rus.shangyingyoupin.top

[C15] 解构 / 展开参数
来源：http://zwx.yanxiufei.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://gql.yfazqb.com

PHP:  [$a, $b] = $pair;
来源：http://rnk.dianchejie.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://bdh.316326.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://bqa.aizwys.cn

Java: // 无解构
来源：http://ttb.hnxiangtu.top

Go:   // 无解构
来源：http://tkr.xuetiantiany.cn

Ruby: a, b = pair
来源：http://vcu.jianghu66.top

C#:   var (a, b) = pair;
来源：http://uji.shzxlz.cn

[C16] 函数 / 方法重载
来源：http://ljz.jinqigufen.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://eto.zhengqikj.top

PHP:  // 无重载
来源：http://swj.tian-w.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://enz.shanyushiyangtech.top

TS:   // 用联合类型或重载签名声明
来源：http://cbw.yueranfly.top

Java: void f(int a) {}  void f(String a) {}
来源：http://nsv.guowangkeji.top

Go:   // 无重载：用不同函数名
来源：http://gtc.chenlongwang.top

Ruby: # 无重载：靠动态参数
来源：http://gse.pengpengdd.cyou

C#:   void F(int a) {}  void F(string a) {}
来源：http://kel.316326.xyz

================================================================================
来源：http://khy.sjlbkw.cn

D. 数组 / 列表 / 集合
来源：http://sin.nanxinkj.top

================================================================================
来源：http://wzz.316326.xyz

[D01] 创建数组 / 列表
来源：http://gdj.9152youxi.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ywd.guowangkeji.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://msv.dashuyun.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://sxy.jinqigfzy.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://azm.hesvh.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mwi.jianghu66.top

Go:   arr := []int{1, 2, 3}
来源：http://tlr.xingfuxueyuan.xyz

Ruby: arr = [1, 2, 3]
来源：http://iwq.chenlongwang.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://yzo.zhoulong.xyz

[D02] 追加元素到末尾
来源：http://jac.uphjek.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://bxf.yj20258888.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://uhg.ydzc1.top

JS:   arr.push(4);
来源：http://hpc.52xcode.cn

TS:   arr.push(4);
来源：http://fol.iojbl.cn

Java: list.add(4);
来源：http://emm.chenlongwang.top

Go:   arr = append(arr, 4)
来源：http://wny.c1oappe.top

Ruby: arr << 4; arr.push(5)
来源：http://qtv.cdnleiting.top

C#:   list.Add(4);
来源：http://dnj.zhijiandao.cn

[D03] 在指定位置插入元素
来源：http://bqt.hywenlv.cn

Py:   arr.insert(0, 0)
来源：http://wne.jinyuanbaomall.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://urb.jinqigufen.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://qek.yuxming.cn

TS:   arr.splice(0, 0, 0);
来源：http://guh.cheryme.top

Java: list.add(0, 0);
来源：http://toq.0kj1m.cn

Go:   arr = append([]int{0}, arr...)
来源：http://otg.hongshengwenyu.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://vze.guannengcc.top

C#:   list.Insert(0, 0);
来源：http://kij.mhx1999.top

[D04] 删除元素
来源：http://ucc.zhoulong.xyz

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://gbk.ybcxt.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://qgn.nanxuanxn.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://fun.zdbjq.cn

TS:   arr.splice(0, 1);
来源：http://vde.guannengcc.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://yvt.smart0.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://jdd.xuetiantiany.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://bch.316326.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://tik.yfazqb.com

[D05] 访问与修改元素
来源：http://uyy.sufxvd.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://yhw.zdqjudy.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ybf.zhongyouzk.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://jxn.kuanghao11.cn

TS:   arr[0]; arr.at(-1);
来源：http://fhn.tanke756.top

Java: list.get(0); list.set(0, 9);
来源：http://ous.cucudq.cn

Go:   arr[0]; arr[0] = 9
来源：http://ghz.jiagoushi.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://pvn.aibaodan.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://jvw.birdmap.top

[D06] 数组长度
来源：http://cau.tianlin.xyz

Py:   len(arr)
来源：http://xqe.nanxuanxn.top

PHP:  count($arr);
来源：http://ksg.svipenyu.cn

JS:   arr.length
来源：http://kag.gaohongyu789.top

TS:   arr.length
来源：http://tzk.sxryk.cn

Java: list.size();
来源：http://dmz.sufxvd.cn

Go:   len(arr)
来源：http://ylk.zhixingplan.top

Ruby: arr.length; arr.size
来源：http://rnx.fzhhl.top

C#:   list.Count;
来源：http://rgn.hnxiangtu.top

[D07] 切片 / 取子数组
来源：http://umw.daxiang520.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qnr.gaohongyu789.top

PHP:  array_slice($arr, 1, 3);
来源：http://qpr.zhixingplan.top

JS:   arr.slice(1, 4);
来源：http://xlb.gaohongyu789.top

TS:   arr.slice(1, 4);
来源：http://csq.yuanzhike.top

Java: list.subList(1, 4);
来源：http://rgg.yuanzhike.top

Go:   arr[1:4]
来源：http://jhq.yangfankeji.com

Ruby: arr[1, 3]
来源：http://msa.bbcook.cn

C#:   list.GetRange(1, 3);
来源：http://ppv.zhongyouzk.top

[D08] 合并两个数组
来源：http://uxi.ydzc1.top

Py:   a + b;  a.extend(b)
来源：http://hbu.fehbvm.com

PHP:  array_merge($a, $b);
来源：http://ues.yueranfly.top

JS:   [...a, ...b];  a.concat(b);
来源：http://yfz.xylfe.cn

TS:   [...a, ...b];
来源：http://bdy.52xcode.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hvo.ydjk.org.cn

Go:   append(a, b...)
来源：http://sct.xziqi.cn

Ruby: a + b;  a.concat(b)
来源：http://fhc.bbcook.cn

C#:   a.Concat(b).ToList()
来源：http://lzl.jinqigfzy.top

[D09] 排序（升序）
来源：http://skr.yangfankeji.com

Py:   sorted(arr);  arr.sort()
来源：http://dsl.fktsv.cn

PHP:  sort($arr);
来源：http://flc.tanke756.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ebe.nwbrower.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://oed.zhongyouzk.top

Java: Collections.sort(list);  list.sort(null);
来源：http://xnc.quarkkingdee.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://pab.feifeiyinyue.top

Ruby: arr.sort
来源：http://ytt.0kj1m.cn

C#:   list.Sort();
来源：http://sia.ywan-chungtsiang.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://eau.epnwcf.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://fvc.hcnkem.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qoa.tarul.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://qtr.aibaodan.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://yby.xuanzx.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://zhn.hammf.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://nnx.hysaishi.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://vir.redwolf501.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://pcr.gogol.net.cn

[D11] 反转数组
来源：http://prm.vehdjk.com

Py:   arr[::-1];  arr.reverse()
来源：http://etd.shanyushiyangtech.top

PHP:  array_reverse($arr);
来源：http://vjs.daxiang520.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://lgs.shanyushiyangtech.top

TS:   [...arr].reverse();
来源：http://jpm.cashguo.top

Java: Collections.reverse(list);
来源：http://hbn.cucudq.cn

Go:   slices.Reverse(arr)
来源：http://cxg.zhengqikj.top

Ruby: arr.reverse
来源：http://kcd.ivvv.top

C#:   list.Reverse();
来源：http://rly.dashuyun.cn

[D12] 查找元素下标
来源：http://zde.xziqi.cn

Py:   arr.index(x);  x in arr
来源：http://cft.pengpengdd.cyou

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ils.yfazqb.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dea.hcnkem.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wob.ydzc1.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://epa.fzhhl.top

Go:   slices.Index(arr, x)
来源：http://ivc.tianlin.xyz

Ruby: arr.index(x)
来源：http://oue.gaohongyu789.top

C#:   list.IndexOf(x);
来源：http://fwp.zdqjudy.top

[D13] 过滤（保留满足条件的）
来源：http://hse.jinghuilouyu.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://jad.fengsongda.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://dah.xylfe.cn

JS:   arr.filter(x => x > 3)
来源：http://xtp.yuxming.cn

TS:   arr.filter(x => x > 3)
来源：http://htm.mhx1999.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://xba.havefunace.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://cuz.sweek.top

Ruby: arr.select { |x| x > 3 }
来源：http://nui.dianchejie.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ook.shanyushiyangtech.top

[D14] 映射转换（每个元素变形）
来源：http://iil.shangyingyoupin.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://gux.guowangkeji.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://prg.vehdjk.com

JS:   arr.map(x => x * 2)
来源：http://dqb.hnqzz.top

TS:   arr.map(x => x * 2)
来源：http://rmh.zdqjudy.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://juo.havefunace.top

Go:   // 手写循环
来源：http://cby.yuanzhike.top

Ruby: arr.map { |x| x * 2 }
来源：http://cul.svipenyu.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ygp.hnxiangtu.top

[D15] 去重
来源：http://pux.chenjidiqi.icu

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://jrt.chenjidiqi.icu

PHP:  array_unique($arr);
来源：http://fxx.xinyue.icu

JS:   [...new Set(arr)]
来源：http://cyi.zycfv.cn

TS:   [...new Set(arr)]
来源：http://fbv.ywan-chungtsiang.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://fhm.meibo888.top

Go:   // 用 map[T]struct{} 手写
来源：http://owb.ydzc1.top

Ruby: arr.uniq
来源：http://vfz.snrcjt.cn

C#:   list.Distinct().ToList()
来源：http://ltc.xinyue.icu

[D16] 求和与平均值
来源：http://fqt.hfpthk.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://anu.xinyue.icu

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://jiy.yvedp.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wwr.yanxiufei.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://kib.zhiwuduotai.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ftg.fengsongda.top

Go:   // 手写循环累加
来源：http://cxj.guannengcc.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mxp.fzhhl.top

C#:   list.Sum();  list.Average()
来源：http://huf.vehdjk.com

[D17] 最大值与最小值
来源：http://nqg.dashuyun.cn

Py:   max(arr);  min(arr)
来源：http://wbj.sxryk.cn

PHP:  max($arr);  min($arr);
来源：http://cai.jqgufenzy.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://crt.ydjk.org.cn

TS:   Math.max(...arr);
来源：http://psx.shanyushiyangkeji.top

Java: Collections.max(list);  Collections.min(list);
来源：http://qre.hesvh.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://gif.xinyue.icu

Ruby: arr.max;  arr.min
来源：http://mzh.yongpay.top

C#:   list.Max();  list.Min()
来源：http://rvf.redwolf501.top

[D18] 扁平化嵌套数组
来源：http://ezp.hammf.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ltx.daxiang520.top

PHP:  array_merge(...$nested);
来源：http://lcq.zdqjudy.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://rfi.yj20258888.top

TS:   nested.flat();
来源：http://izr.zhaomingkeji.xyz

Java: nested.stream().flatMap(List::stream).toList()
来源：http://gmr.zhixingplan.top

Go:   // 手写双层循环
来源：http://tyl.dianchejie.cn

Ruby: nested.flatten
来源：http://tsl.tarul.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://dzb.chenzaomai.com

[D19] 按字段分组
来源：http://ewj.nanxuanxn.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://waj.shangyingyoupin.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://nxl.zhixingplan.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://zku.ivvv.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://dnf.vehdjk.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://xnc.gzhubu.top

Go:   // 手写 map[string][]T
来源：http://xkp.yangfankeji.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://jby.andypj.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://jbd.jinyuanbaomall.cn

[D20] 统计每个元素出现次数
来源：http://brz.xuetiantiany.cn

Py:   Counter(arr)
来源：http://wpf.dianchejie.cn

PHP:  array_count_values($arr);
来源：http://xem.chenzaomai.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://osx.tianlin.xyz

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nvp.xziqi.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://vec.bbcook.cn

Go:   // 手写 map[T]int
来源：http://rsi.jinqigufen.top

Ruby: arr.tally
来源：http://kbe.yuanzhike.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://tqk.feifeiyinyue.top

[D21] 判断是否包含某元素
来源：http://crg.zycfv.cn

Py:   x in arr
来源：http://jym.yonumen.top

PHP:  in_array($x, $arr, true);
来源：http://uac.mhx1999.top

JS:   arr.includes(x)
来源：http://yun.yvedp.cn

TS:   arr.includes(x)
来源：http://dnw.sjlbkw.cn

Java: list.contains(x)
来源：http://vgm.yonumen.top

Go:   slices.Contains(arr, x)
来源：http://kqt.meibo888.top

Ruby: arr.include?(x)
来源：http://kyv.xingfuxueyuan.xyz

C#:   list.Contains(x)
来源：http://gth.zhaomingkeji.xyz

[D22] 复制数组（避免共享引用）
来源：http://jhq.hysaishi.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://zzb.fehbvm.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wjc.yangfankeji.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://jcp.sufxvd.cn

TS:   [...arr];
来源：http://isu.fengsongda.top

Java: new ArrayList<>(list);
来源：http://jpz.smart0.xyz

Go:   copied := append([]int(nil), arr...)
来源：http://itk.316326.xyz

Ruby: arr.dup;  arr.clone
来源：http://yts.chenzaomai.com

C#:   new List<int>(list);
来源：http://qon.hnqzz.top

[D23] reduce 累积计算
来源：http://sqt.jiagoushi.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://pas.pengpengdd.cyou

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ety.tianlin.xyz

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dat.hfpthk.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bxb.hcnkem.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://jwm.fengsongda.top

Go:   // 手写循环
来源：http://fwy.cucudq.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://fgk.jqgufenzy.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wzs.epnwcf.com

[D24] 字典 / Map 基本操作
来源：http://utm.svipenyu.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://xog.fengsongda.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mzp.svipenyu.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wqn.daria6918.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://lug.jqgfzy.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ttg.daxiang520.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://llt.shzxlz.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://amy.sufxvd.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://caj.jqgufenzy.top

[D25] Set 集合去重与交并差
来源：http://rwo.ybcxt.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hkr.zhiwuduotai.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://cfn.jqgfzy.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mwx.yj202588.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://tpc.zdqjudy.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://zfj.birdmap.top


<!-- 参考信息 -->