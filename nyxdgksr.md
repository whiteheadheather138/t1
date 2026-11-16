代发 wailian999

C#:   块级作用域
来源：http://gax.snrcjt.cn

[C11] 模块导入与导出
来源：http://ncr.vqdsnc.cn

Py:   from module import func
来源：http://xcs.zhongyouzk.top

PHP:  require "file.php";  或 use App\Service;
来源：http://sey.zhengqikj.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://uds.tianlin.xyz

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ert.kuanghao11.cn

Java: import java.util.List;
来源：http://ahf.fanxiaobao.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://zca.kuanghao11.cn

Ruby: require "json"; require_relative "./util"
来源：http://bok.xingfuxueyuan.xyz

C#:   using System.Text;
来源：http://tmj.zhoulong.xyz

[C12] 立即执行函数 IIFE
来源：http://orx.shangyingyoupin.top

Py:   (lambda: print("run"))()
来源：http://qtc.redwolf501.top

PHP:  (function () { echo "run"; })();
来源：http://ulk.zdqjudy.top

JS:   (() => { console.log("run"); })();
来源：http://xye.tarul.cn

TS:   (() => { console.log("run"); })();
来源：http://jcb.dianchejie.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://bcw.daria6918.cn

Go:   func() { fmt.Println("run") }()
来源：http://iuc.yangfankeji.com

Ruby: -> { puts "run" }.call
来源：http://hvh.pengpengdd.cyou

C#:   // 无 IIFE：用静态构造函数
来源：http://scy.shanyushiyangtech.top

[C13] 类型声明 / 类型注解
来源：http://azn.redwolf501.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://vfc.yonumen.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://noh.zhixingplan.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://vdb.nwbrower.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zaj.tarul.cn

Java: int add(int a, int b) { return a + b; }
来源：http://aiw.fanxiaobao.xyz

Go:   func add(a, b int) int
来源：http://lfy.316326.xyz

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://fso.ybcxt.top

C#:   int Add(int a, int b) => a + b;
来源：http://pvh.ehwqpu.com

[C14] 泛型函数
来源：http://jtg.ehwqpu.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://jto.c1oappe.top

PHP:  // 无泛型
来源：http://cdm.yangfankeji.com

JS:   // 无泛型
来源：http://pzf.52xcode.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://lub.fktsv.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://lnx.yueranfly.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://qgx.tarul.cn

Ruby: # 无泛型
来源：http://ktd.yfazqb.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://gfn.tian-w.cn

[C15] 解构 / 展开参数
来源：http://car.gotoacloud.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://qdy.xuanzx.com

PHP:  [$a, $b] = $pair;
来源：http://epz.xuetiantiany.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hnj.c1oappe.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://cfr.jqgfzy.top

Java: // 无解构
来源：http://cdd.zhiwuduotai.top

Go:   // 无解构
来源：http://cas.fanxiaobao.xyz

Ruby: a, b = pair
来源：http://nkd.xinyue.icu

C#:   var (a, b) = pair;
来源：http://fkr.mhx1999.top

[C16] 函数 / 方法重载
来源：http://fdm.ctjpmb.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://rbe.guannengcc.top

PHP:  // 无重载
来源：http://lkq.hcnkem.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://zpu.fehbvm.com

TS:   // 用联合类型或重载签名声明
来源：http://aaw.zhengqikj.top

Java: void f(int a) {}  void f(String a) {}
来源：http://dvj.shanyushiyangtech.top

Go:   // 无重载：用不同函数名
来源：http://bsm.iojbl.cn

Ruby: # 无重载：靠动态参数
来源：http://bhf.snrcjt.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://igk.fengsongda.top

================================================================================
来源：http://fpx.nanxuanxn.top

D. 数组 / 列表 / 集合
来源：http://smn.bjfxy.top

================================================================================
来源：http://upz.yonumen.top

[D01] 创建数组 / 列表
来源：http://kov.chenjidiqi.icu

Py:   arr = [1, 2, 3];  empty = []
来源：http://wdv.jianghu66.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://vzo.yvedp.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://pyt.chenzaomai.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://aqh.bbcook.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://azy.aibaodan.cn

Go:   arr := []int{1, 2, 3}
来源：http://rzy.xingfuxueyuan.xyz

Ruby: arr = [1, 2, 3]
来源：http://zbj.xuetiantiany.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://tmr.havefunace.top

[D02] 追加元素到末尾
来源：http://ikq.zhengqikj.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ioz.yangfankeji.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://vgc.zycfv.cn

JS:   arr.push(4);
来源：http://may.c1oappe.top

TS:   arr.push(4);
来源：http://spe.zhoulong.xyz

Java: list.add(4);
来源：http://ijc.daria6918.cn

Go:   arr = append(arr, 4)
来源：http://rgw.jqgfzy.top

Ruby: arr << 4; arr.push(5)
来源：http://xij.shzxlz.cn

C#:   list.Add(4);
来源：http://xta.yuxming.cn

[D03] 在指定位置插入元素
来源：http://zxj.yj20258.top

Py:   arr.insert(0, 0)
来源：http://jas.zhaomingkeji.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://weu.tianlin.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://stn.hcnkem.com

TS:   arr.splice(0, 0, 0);
来源：http://xvb.jinghuilouyu.cn

Java: list.add(0, 0);
来源：http://foe.yongpay.top

Go:   arr = append([]int{0}, arr...)
来源：http://gqk.hfpthk.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://nwr.bjfxy.top

C#:   list.Insert(0, 0);
来源：http://qen.birdmap.top

[D04] 删除元素
来源：http://xok.birdmap.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://rtm.kuanghao11.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://qcc.vehdjk.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://iru.chenjidiqi.icu

TS:   arr.splice(0, 1);
来源：http://bmu.jinqigufen.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hfw.wangdashe.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://skf.zhengqikj.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://kbi.nanxinkj.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://rxu.ydzc1.top

[D05] 访问与修改元素
来源：http://kmf.jinqigfzy.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://quu.birdmap.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ach.zhoulong.xyz

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://iaq.yvedp.cn

TS:   arr[0]; arr.at(-1);
来源：http://kim.hongshengwenyu.top

Java: list.get(0); list.set(0, 9);
来源：http://yzc.mhx1999.top

Go:   arr[0]; arr[0] = 9
来源：http://aip.zhijiandao.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ngs.redwolf501.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://fck.jlsjyb.cn

[D06] 数组长度
来源：http://bdo.yvedp.cn

Py:   len(arr)
来源：http://axw.smart0.xyz

PHP:  count($arr);
来源：http://her.yfazqb.com

JS:   arr.length
来源：http://gbu.sweek.top

TS:   arr.length
来源：http://frf.ivvv.top

Java: list.size();
来源：http://cpp.sysykeji.top

Go:   len(arr)
来源：http://kye.xziqi.cn

Ruby: arr.length; arr.size
来源：http://tzf.jqgufenzy.top

C#:   list.Count;
来源：http://tid.daxiang520.top

[D07] 切片 / 取子数组
来源：http://afb.c1oappe.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ymz.wangdashe.top

PHP:  array_slice($arr, 1, 3);
来源：http://kzq.hammf.cn

JS:   arr.slice(1, 4);
来源：http://qoy.jqgufenzy.top

TS:   arr.slice(1, 4);
来源：http://cyz.0kj1m.cn

Java: list.subList(1, 4);
来源：http://ngt.xylfe.cn

Go:   arr[1:4]
来源：http://lkv.zycfv.cn

Ruby: arr[1, 3]
来源：http://uio.jinqigfzy.top

C#:   list.GetRange(1, 3);
来源：http://yqh.yj20258888.top

[D08] 合并两个数组
来源：http://ptb.sufxvd.cn

Py:   a + b;  a.extend(b)
来源：http://cxr.birdmap.top

PHP:  array_merge($a, $b);
来源：http://bwu.cucudq.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://nyw.jinghuilouyu.cn

TS:   [...a, ...b];
来源：http://ier.shuidangran.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://gex.nwbrower.top

Go:   append(a, b...)
来源：http://yni.hysaishi.cn

Ruby: a + b;  a.concat(b)
来源：http://prf.aizwys.cn

C#:   a.Concat(b).ToList()
来源：http://vql.hcnkem.com

[D09] 排序（升序）
来源：http://aqw.chenjidiqi.icu

Py:   sorted(arr);  arr.sort()
来源：http://mpa.haohaochexian.top

PHP:  sort($arr);
来源：http://rer.zycfv.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://dgr.guannengcc.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://end.zdbjq.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://xgc.jiagoushi.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://lop.hesvh.cn

Ruby: arr.sort
来源：http://jyk.birdmap.top

C#:   list.Sort();
来源：http://uvy.feifeiyinyue.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://med.dianchejie.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://myw.vqdsnc.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mng.wangshuangyany.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://jhr.hywenlv.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://kju.ehwqpu.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ohx.jlsjyb.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://noo.jiagoushi.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://dtm.yj20258.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ioo.epnwcf.com

[D11] 反转数组
来源：http://gxb.dashuyun.cn

Py:   arr[::-1];  arr.reverse()
来源：http://vls.chenlongwang.top

PHP:  array_reverse($arr);
来源：http://jsi.zhixingplan.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ttq.meibo888.top

TS:   [...arr].reverse();
来源：http://los.hfpthk.cn

Java: Collections.reverse(list);
来源：http://iaf.gotoacloud.top

Go:   slices.Reverse(arr)
来源：http://ole.9152youxi.cn

Ruby: arr.reverse
来源：http://mbd.quarkkingdee.top

C#:   list.Reverse();
来源：http://kvp.uphjek.com

[D12] 查找元素下标
来源：http://fre.dianchejie.cn

Py:   arr.index(x);  x in arr
来源：http://kon.hongshengwenyu.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://glp.wangdashe.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://eve.hysaishi.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xwx.wangshuangyany.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://exx.ppjwa.cn

Go:   slices.Index(arr, x)
来源：http://olz.wangshuangyany.cn

Ruby: arr.index(x)
来源：http://ype.epnwcf.com

C#:   list.IndexOf(x);
来源：http://gba.zdqjudy.top

[D13] 过滤（保留满足条件的）
来源：http://sfl.chenlongwang.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://zto.gogol.net.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://yto.jianghu66.top

JS:   arr.filter(x => x > 3)
来源：http://arm.zhoulong.xyz

TS:   arr.filter(x => x > 3)
来源：http://mdi.dianchejie.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://auc.yonumen.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://cnc.fzhhl.top

Ruby: arr.select { |x| x > 3 }
来源：http://dkl.fengsongda.top

C#:   list.Where(x => x > 3).ToList()
来源：http://xyp.cdnleiting.top

[D14] 映射转换（每个元素变形）
来源：http://xgr.xingfuxueyuan.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hmd.zdqjudy.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://muu.xziqi.cn

JS:   arr.map(x => x * 2)
来源：http://ibd.dashuyun.cn

TS:   arr.map(x => x * 2)
来源：http://bxq.kuanghao11.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://sky.zhaomingkeji.xyz

Go:   // 手写循环
来源：http://rds.jiagoushi.top

Ruby: arr.map { |x| x * 2 }
来源：http://dcw.9152youxi.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ovq.cdnleiting.top

[D15] 去重
来源：http://atm.kuanghao11.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://eqn.jinyuanbaomall.cn

PHP:  array_unique($arr);
来源：http://fct.zhixingplan.top

JS:   [...new Set(arr)]
来源：http://fqh.yj20258888.top

TS:   [...new Set(arr)]
来源：http://xmr.ywan-chungtsiang.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://jth.hysaishi.cn

Go:   // 用 map[T]struct{} 手写
来源：http://wdd.smart0.xyz

Ruby: arr.uniq
来源：http://ctw.yueranfly.top

C#:   list.Distinct().ToList()
来源：http://rpu.cqqwz.cn

[D16] 求和与平均值
来源：http://qyu.wangshuangyany.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://vfs.sjlbkw.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://rgv.daria6918.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://iqw.jiagoushi.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://chl.gogol.net.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://tfy.jiagoushi.top

Go:   // 手写循环累加
来源：http://tmf.yj202588.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://gyv.mhx1999.top

C#:   list.Sum();  list.Average()
来源：http://ule.fzhhl.top

[D17] 最大值与最小值
来源：http://maz.chenzaomai.com

Py:   max(arr);  min(arr)
来源：http://tkm.yonumen.top

PHP:  max($arr);  min($arr);
来源：http://pco.fzhhl.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ndt.ivvv.top

TS:   Math.max(...arr);
来源：http://rjn.yj20258888.top

Java: Collections.max(list);  Collections.min(list);
来源：http://xnb.cqqwz.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://egq.pengpengdd.cyou

Ruby: arr.max;  arr.min
来源：http://keg.quarkkingdee.top

C#:   list.Max();  list.Min()
来源：http://xfs.shanyushiyangkeji.top

[D18] 扁平化嵌套数组
来源：http://lof.chenzaomai.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://zsa.shuidangran.top

PHP:  array_merge(...$nested);
来源：http://kfi.ehwqpu.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://haf.redwolf501.top

TS:   nested.flat();
来源：http://joh.gogol.net.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wbw.tianlin.xyz

Go:   // 手写双层循环
来源：http://ppb.yongpay.top

Ruby: nested.flatten
来源：http://iva.zhengqikj.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://fcq.xziqi.cn

[D19] 按字段分组
来源：http://qge.hfpthk.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://gjk.cqqwz.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://thi.ydjk.org.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wxi.xingfuxueyuan.xyz

TS:   Object.groupBy(arr, x => x.type)
来源：http://flf.bbcook.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wre.sxryk.cn

Go:   // 手写 map[string][]T
来源：http://ccg.redwolf501.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://bwb.hywenlv.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://cyg.hywenlv.cn

[D20] 统计每个元素出现次数
来源：http://vjz.pengpengdd.cyou

Py:   Counter(arr)
来源：http://unx.ctjpmb.com

PHP:  array_count_values($arr);
来源：http://mqn.aizwys.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://edf.cheryme.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ypn.sysykeji.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://nwp.zdqjudy.top

Go:   // 手写 map[T]int
来源：http://rhq.bbcook.cn

Ruby: arr.tally
来源：http://oie.gzhubu.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ozm.ywan-chungtsiang.top

[D21] 判断是否包含某元素
来源：http://oiu.wangshuangyany.cn

Py:   x in arr
来源：http://jzp.tarul.cn

PHP:  in_array($x, $arr, true);
来源：http://tml.sweek.top

JS:   arr.includes(x)
来源：http://nfw.smart0.xyz

TS:   arr.includes(x)
来源：http://qpe.meibo888.top

Java: list.contains(x)
来源：http://fxk.tanke756.top

Go:   slices.Contains(arr, x)
来源：http://xzh.cqqwz.cn

Ruby: arr.include?(x)
来源：http://dzk.gaohongyu789.top

C#:   list.Contains(x)
来源：http://btr.daria6918.cn

[D22] 复制数组（避免共享引用）
来源：http://ebd.andypj.xyz

Py:   arr.copy();  arr[:];  list(arr)
来源：http://eqy.fehbvm.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://sao.ppjwa.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://zkz.guannengcc.top

TS:   [...arr];
来源：http://lgx.jiagoushi.top

Java: new ArrayList<>(list);
来源：http://euy.dashuyun.cn

Go:   copied := append([]int(nil), arr...)
来源：http://djs.fktsv.cn

Ruby: arr.dup;  arr.clone
来源：http://wze.jinyuanbaomall.cn

C#:   new List<int>(list);
来源：http://cdt.ydzc1.top

[D23] reduce 累积计算
来源：http://kgc.yuanzhike.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://xwy.pengpengdd.cyou

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://pvr.yj20258888.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pny.xylfe.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wch.jiagoushi.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://xoo.hysaishi.cn

Go:   // 手写循环
来源：http://qhp.hfpthk.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://buj.ydjk.org.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ahx.ctjpmb.com

[D24] 字典 / Map 基本操作
来源：http://wwp.fengsongda.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://uvj.hnqzz.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qny.jyoumei.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://vtb.hnxiangtu.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://oos.dianchejie.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://vur.yueranfly.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://xrc.fengsongda.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://vvq.jiagoushi.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://cte.pycfn.com

[D25] Set 集合去重与交并差
来源：http://xxz.hongshengwenyu.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://vdf.zdqjudy.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://cri.yfazqb.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ypn.jinghuilouyu.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://pur.wangdashe.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hro.pycfn.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://oio.cucudq.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://chm.xingfuxueyuan.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://xrz.haohaochexian.top

[D26] 数组转字符串
来源：http://dpj.jlsjyb.cn

Py:   ", ".join(map(str, arr))
来源：http://cin.cdnleiting.top

PHP:  implode(", ", $arr);
来源：http://koa.yj20258888.top

JS:   arr.join(", ")
来源：http://dtf.fanxiaobao.xyz

TS:   arr.join(", ")
来源：http://rcx.zhoulong.xyz

Java: String.join(", ", list)
来源：http://zfo.daria6918.cn

Go:   strings.Join(strs, ", ")
来源：http://kbs.sysykeji.top

Ruby: arr.join(", ")
来源：http://dok.tanke756.top

C#:   string.Join(", ", list)
来源：http://uiy.jyoumei.cn

================================================================================
来源：http://rgu.shuidangran.top

E. 字符串处理
来源：http://rjl.meibo888.top

================================================================================
来源：http://nev.wangdashe.top

[E01] 拼接字符串
来源：http://cjf.havefunace.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://zdj.meibo888.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://tru.quarkkingdee.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://vol.hammf.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wgp.gzhubu.top


<!-- 参考信息 -->