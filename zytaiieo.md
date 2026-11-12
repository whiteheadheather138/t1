代发 wailian999

TS:   同 JS
来源：http://shw.hnxiangtu.top

Java: 方法内为块级作用域
来源：http://thx.smart0.xyz

Go:   花括号块级作用域
来源：http://cja.zhengqikj.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://dbx.yj20258888.top

C#:   块级作用域
来源：http://nlj.pycfn.com

[C11] 模块导入与导出
来源：http://dhe.wangshuangyany.cn

Py:   from module import func
来源：http://kmu.zhiwuduotai.top

PHP:  require "file.php";  或 use App\Service;
来源：http://cpp.chenlongwang.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://qcq.xylfe.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://qoz.xuetiantiany.cn

Java: import java.util.List;
来源：http://oqj.yanxiufei.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://rya.snrcjt.cn

Ruby: require "json"; require_relative "./util"
来源：http://nyo.pycfn.com

C#:   using System.Text;
来源：http://kro.yuanzhike.top

[C12] 立即执行函数 IIFE
来源：http://uxs.gotoacloud.top

Py:   (lambda: print("run"))()
来源：http://vio.xylfe.cn

PHP:  (function () { echo "run"; })();
来源：http://ead.jqgfzy.top

JS:   (() => { console.log("run"); })();
来源：http://tjg.cdnleiting.top

TS:   (() => { console.log("run"); })();
来源：http://phx.xziqi.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://rxr.chenjidiqi.icu

Go:   func() { fmt.Println("run") }()
来源：http://pte.jyoumei.cn

Ruby: -> { puts "run" }.call
来源：http://kgn.yangfankeji.com

C#:   // 无 IIFE：用静态构造函数
来源：http://smv.zhixingplan.top

[C13] 类型声明 / 类型注解
来源：http://wxj.yueranfly.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ybx.yongpay.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://apc.chenlongwang.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://chq.yuxming.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xwt.nanxuanxn.top

Java: int add(int a, int b) { return a + b; }
来源：http://mnh.tarul.cn

Go:   func add(a, b int) int
来源：http://vji.yuxming.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://dkx.ybcxt.top

C#:   int Add(int a, int b) => a + b;
来源：http://dla.hywenlv.cn

[C14] 泛型函数
来源：http://owc.aizwys.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hqv.ywan-chungtsiang.top

PHP:  // 无泛型
来源：http://ztz.hywenlv.cn

JS:   // 无泛型
来源：http://dwo.hywenlv.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://zsl.nwbrower.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ffg.yueranfly.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://myh.smart0.xyz

Ruby: # 无泛型
来源：http://nvh.gaohongyu789.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wpf.pengpengdd.cyou

[C15] 解构 / 展开参数
来源：http://ikm.xuetiantiany.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://tzu.tarul.cn

PHP:  [$a, $b] = $pair;
来源：http://zad.bbcook.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://tfk.hywenlv.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://xwb.hammf.cn

Java: // 无解构
来源：http://aof.xuanzx.com

Go:   // 无解构
来源：http://shx.cqqwz.cn

Ruby: a, b = pair
来源：http://cpe.xuetiantiany.cn

C#:   var (a, b) = pair;
来源：http://ece.jinqigfzy.top

[C16] 函数 / 方法重载
来源：http://awo.cheryme.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://jba.fzhhl.top

PHP:  // 无重载
来源：http://xlc.haohaochexian.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://rbw.gogol.net.cn

TS:   // 用联合类型或重载签名声明
来源：http://zke.jinghuilouyu.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://pdk.316326.xyz

Go:   // 无重载：用不同函数名
来源：http://pbd.bbcook.cn

Ruby: # 无重载：靠动态参数
来源：http://rcw.jinghuilouyu.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://kjl.ybcxt.top

================================================================================
来源：http://ess.fktsv.cn

D. 数组 / 列表 / 集合
来源：http://dfd.cqqwz.cn

================================================================================
来源：http://vrp.sjlbkw.cn

[D01] 创建数组 / 列表
来源：http://rys.hysaishi.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://qsm.316326.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hkr.gogol.net.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://uro.jiagoushi.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://vhj.gaohongyu789.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ylu.wangdashe.top

Go:   arr := []int{1, 2, 3}
来源：http://dfb.c1oappe.top

Ruby: arr = [1, 2, 3]
来源：http://tbe.shuidangran.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://kne.yj20258.top

[D02] 追加元素到末尾
来源：http://mll.zhixingplan.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://gym.jiagoushi.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://nhv.gaohongyu789.top

JS:   arr.push(4);
来源：http://jij.yuxming.cn

TS:   arr.push(4);
来源：http://hjq.shanyushiyangkeji.top

Java: list.add(4);
来源：http://gxy.aizwys.cn

Go:   arr = append(arr, 4)
来源：http://kjg.guannengcc.top

Ruby: arr << 4; arr.push(5)
来源：http://uqj.ybcxt.top

C#:   list.Add(4);
来源：http://yoa.ctjpmb.com

[D03] 在指定位置插入元素
来源：http://sji.gzhubu.top

Py:   arr.insert(0, 0)
来源：http://lha.yangfankeji.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://lbz.gotoacloud.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://jcm.daxiang520.top

TS:   arr.splice(0, 0, 0);
来源：http://hlv.aibaodan.cn

Java: list.add(0, 0);
来源：http://wii.shanyushiyangtech.top

Go:   arr = append([]int{0}, arr...)
来源：http://iry.mhx1999.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://vno.jinqigufen.top

C#:   list.Insert(0, 0);
来源：http://pww.shzxlz.cn

[D04] 删除元素
来源：http://iyk.svipenyu.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ylc.havefunace.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://dpp.zhengqikj.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://kho.hammf.cn

TS:   arr.splice(0, 1);
来源：http://kbb.fehbvm.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ztw.haohaochexian.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wiz.epnwcf.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ilq.yj202588.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hmz.yj202588.top

[D05] 访问与修改元素
来源：http://jnc.yfazqb.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ybx.shangyingyoupin.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://qru.haohaochexian.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://nvp.0kj1m.cn

TS:   arr[0]; arr.at(-1);
来源：http://ssl.pengpengdd.cyou

Java: list.get(0); list.set(0, 9);
来源：http://tpm.zycfv.cn

Go:   arr[0]; arr[0] = 9
来源：http://iwu.jlsjyb.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://flc.yueranfly.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://yun.uphjek.com

[D06] 数组长度
来源：http://wcu.zhixingplan.top

Py:   len(arr)
来源：http://krj.9152youxi.cn

PHP:  count($arr);
来源：http://kch.shuidangran.top

JS:   arr.length
来源：http://rak.jyoumei.cn

TS:   arr.length
来源：http://coo.snrcjt.cn

Java: list.size();
来源：http://dxv.jiagoushi.top

Go:   len(arr)
来源：http://fjs.tianlin.xyz

Ruby: arr.length; arr.size
来源：http://gsh.dianchejie.cn

C#:   list.Count;
来源：http://cnj.zhiwuduotai.top

[D07] 切片 / 取子数组
来源：http://fkh.cucudq.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hyt.sxryk.cn

PHP:  array_slice($arr, 1, 3);
来源：http://vzz.ehwqpu.com

JS:   arr.slice(1, 4);
来源：http://lsm.hysaishi.cn

TS:   arr.slice(1, 4);
来源：http://xho.zhaomingkeji.xyz

Java: list.subList(1, 4);
来源：http://xdy.sysykeji.top

Go:   arr[1:4]
来源：http://ljz.ehwqpu.com

Ruby: arr[1, 3]
来源：http://tgk.yueranfly.top

C#:   list.GetRange(1, 3);
来源：http://wkl.uphjek.com

[D08] 合并两个数组
来源：http://pci.xingfuxueyuan.xyz

Py:   a + b;  a.extend(b)
来源：http://ren.zdqjudy.top

PHP:  array_merge($a, $b);
来源：http://cfo.fehbvm.com

JS:   [...a, ...b];  a.concat(b);
来源：http://cec.xuetiantiany.cn

TS:   [...a, ...b];
来源：http://knn.hnqzz.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://aya.jinghuilouyu.cn

Go:   append(a, b...)
来源：http://jnf.kuanghao11.cn

Ruby: a + b;  a.concat(b)
来源：http://lia.guannengcc.top

C#:   a.Concat(b).ToList()
来源：http://vzp.zhixingplan.top

[D09] 排序（升序）
来源：http://nzz.uphjek.com

Py:   sorted(arr);  arr.sort()
来源：http://lem.zdqjudy.top

PHP:  sort($arr);
来源：http://oku.tian-w.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://koo.birdmap.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://wfb.xziqi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://iov.hesvh.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://bmc.cheryme.top

Ruby: arr.sort
来源：http://mfm.gogol.net.cn

C#:   list.Sort();
来源：http://aut.vehdjk.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://lbo.chenlongwang.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://gis.yj20258.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://whq.zhongyouzk.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://rdw.sufxvd.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://tbe.yonumen.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://zdi.fktsv.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://bkq.hnxiangtu.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://kfj.chenzaomai.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://eji.zhixingplan.top

[D11] 反转数组
来源：http://pdm.zhijiandao.cn

Py:   arr[::-1];  arr.reverse()
来源：http://lxi.jinqigfzy.top

PHP:  array_reverse($arr);
来源：http://nhv.ywan-chungtsiang.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://cyu.snrcjt.cn

TS:   [...arr].reverse();
来源：http://dus.tarul.cn

Java: Collections.reverse(list);
来源：http://rck.xuetiantiany.cn

Go:   slices.Reverse(arr)
来源：http://vkt.zhaomingkeji.xyz

Ruby: arr.reverse
来源：http://wmg.sufxvd.cn

C#:   list.Reverse();
来源：http://yga.shangyingyoupin.top

[D12] 查找元素下标
来源：http://krs.vqdsnc.cn

Py:   arr.index(x);  x in arr
来源：http://fpo.nanxuanxn.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mpe.iojbl.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sbf.zycfv.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ktp.jinghuilouyu.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://vyu.hesvh.cn

Go:   slices.Index(arr, x)
来源：http://elm.yj20258.top

Ruby: arr.index(x)
来源：http://ngu.pengpengdd.cyou

C#:   list.IndexOf(x);
来源：http://efd.quarkkingdee.top

[D13] 过滤（保留满足条件的）
来源：http://wga.kuanghao11.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://xmr.jqgufenzy.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wra.havefunace.top

JS:   arr.filter(x => x > 3)
来源：http://tqo.yanxiufei.cn

TS:   arr.filter(x => x > 3)
来源：http://ubt.zdbjq.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ubz.snrcjt.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://tgp.cdnleiting.top

Ruby: arr.select { |x| x > 3 }
来源：http://ihy.zhiwuduotai.top

C#:   list.Where(x => x > 3).ToList()
来源：http://bni.jianghu66.top

[D14] 映射转换（每个元素变形）
来源：http://nam.andypj.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://pdj.fzhhl.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://dil.zhaomingkeji.xyz

JS:   arr.map(x => x * 2)
来源：http://htx.c1oappe.top

TS:   arr.map(x => x * 2)
来源：http://eoq.52xcode.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://vij.jinghuilouyu.cn

Go:   // 手写循环
来源：http://nta.zhijiandao.cn

Ruby: arr.map { |x| x * 2 }
来源：http://wey.nwbrower.top

C#:   list.Select(x => x * 2).ToList()
来源：http://bfg.cucudq.cn

[D15] 去重
来源：http://bgd.jiagoushi.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ftz.hammf.cn

PHP:  array_unique($arr);
来源：http://zms.hcnkem.com

JS:   [...new Set(arr)]
来源：http://xfs.havefunace.top

TS:   [...new Set(arr)]
来源：http://qce.hywenlv.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://veb.shzxlz.cn

Go:   // 用 map[T]struct{} 手写
来源：http://eaq.ydzc1.top

Ruby: arr.uniq
来源：http://krz.jinqigufen.top

C#:   list.Distinct().ToList()
来源：http://qov.yongpay.top

[D16] 求和与平均值
来源：http://ewa.daxiang520.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ztw.yuanzhike.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://lqx.jyoumei.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://bda.bjfxy.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://jcr.fehbvm.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mqi.bjfxy.top

Go:   // 手写循环累加
来源：http://qkr.jlsjyb.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mlf.vehdjk.com

C#:   list.Sum();  list.Average()
来源：http://kyt.cdnleiting.top

[D17] 最大值与最小值
来源：http://mff.guannengcc.top

Py:   max(arr);  min(arr)
来源：http://smr.jqgfzy.top

PHP:  max($arr);  min($arr);
来源：http://ufo.ywan-chungtsiang.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://nnz.0kj1m.cn

TS:   Math.max(...arr);
来源：http://wcn.52xcode.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://zvb.shangyingyoupin.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://pdl.vqdsnc.cn

Ruby: arr.max;  arr.min
来源：http://ljt.jqgufenzy.top

C#:   list.Max();  list.Min()
来源：http://lgq.hcnkem.com

[D18] 扁平化嵌套数组
来源：http://rfw.daria6918.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://zim.ivvv.top

PHP:  array_merge(...$nested);
来源：http://ryf.snrcjt.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://lex.hywenlv.cn

TS:   nested.flat();
来源：http://pes.snrcjt.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://cbl.jyoumei.cn

Go:   // 手写双层循环
来源：http://kqb.shanyushiyangtech.top

Ruby: nested.flatten
来源：http://xvg.shangyingyoupin.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://djc.iojbl.cn

[D19] 按字段分组
来源：http://soi.xylfe.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://kdp.ywan-chungtsiang.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://tgi.sysykeji.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://vtg.iojbl.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://xwx.zhixingplan.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wtp.jinqigfzy.top

Go:   // 手写 map[string][]T
来源：http://dux.jinqigfzy.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://mqf.jlsjyb.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://kxw.zhongyouzk.top

[D20] 统计每个元素出现次数
来源：http://wji.yueranfly.top

Py:   Counter(arr)
来源：http://ynx.yuxming.cn

PHP:  array_count_values($arr);
来源：http://svb.quarkkingdee.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rro.nwbrower.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://snk.hnxiangtu.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://eux.shanyushiyangtech.top

Go:   // 手写 map[T]int
来源：http://mdb.zhoulong.xyz

Ruby: arr.tally
来源：http://lao.c1oappe.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://yxb.cucudq.cn

[D21] 判断是否包含某元素
来源：http://opz.haohaochexian.top

Py:   x in arr
来源：http://kot.tian-w.cn

PHP:  in_array($x, $arr, true);
来源：http://wzp.yj20258888.top

JS:   arr.includes(x)
来源：http://lhl.ppjwa.cn

TS:   arr.includes(x)
来源：http://awu.316326.xyz

Java: list.contains(x)
来源：http://ijx.shuidangran.top

Go:   slices.Contains(arr, x)
来源：http://epc.chenlongwang.top

Ruby: arr.include?(x)
来源：http://oxy.xylfe.cn

C#:   list.Contains(x)
来源：http://fgh.daxiang520.top

[D22] 复制数组（避免共享引用）
来源：http://zim.316326.xyz

Py:   arr.copy();  arr[:];  list(arr)
来源：http://izt.xziqi.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://bwc.jinghuilouyu.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://yly.zhongyouzk.top

TS:   [...arr];
来源：http://tgb.iojbl.cn

Java: new ArrayList<>(list);
来源：http://cdw.yangfankeji.com

Go:   copied := append([]int(nil), arr...)
来源：http://qnc.meibo888.top

Ruby: arr.dup;  arr.clone
来源：http://cfi.yvedp.cn

C#:   new List<int>(list);
来源：http://not.hywenlv.cn

[D23] reduce 累积计算
来源：http://thb.ydjk.org.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wvs.hcnkem.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://udu.guannengcc.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://udg.iojbl.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dgu.yueranfly.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://zgg.shanyushiyangkeji.top

Go:   // 手写循环
来源：http://gkj.tian-w.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://muf.xinyue.icu

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://oht.52xcode.cn

[D24] 字典 / Map 基本操作
来源：http://tej.hnxiangtu.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://kwo.yvedp.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mur.jyoumei.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://fnv.shuidangran.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://gvv.birdmap.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ijx.yonumen.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://cik.vehdjk.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://kkt.cqqwz.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://irv.yongpay.top

[D25] Set 集合去重与交并差
来源：http://bbm.9152youxi.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://dpa.svipenyu.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://cwg.yanxiufei.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://aby.yongpay.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://nxo.fzhhl.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://rsk.yvedp.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://rxo.daria6918.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://nxv.nanxuanxn.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ecp.zhijiandao.cn

[D26] 数组转字符串
来源：http://jct.hammf.cn

Py:   ", ".join(map(str, arr))
来源：http://mip.sxryk.cn

PHP:  implode(", ", $arr);
来源：http://vmu.guowangkeji.top

JS:   arr.join(", ")
来源：http://ywm.uphjek.com

TS:   arr.join(", ")
来源：http://iiw.sjlbkw.cn

Java: String.join(", ", list)
来源：http://fpb.quarkkingdee.top

Go:   strings.Join(strs, ", ")
来源：http://fez.yonumen.top

Ruby: arr.join(", ")
来源：http://skm.ydjk.org.cn

C#:   string.Join(", ", list)
来源：http://url.xinyue.icu

================================================================================
来源：http://xsc.jqgufenzy.top

E. 字符串处理
来源：http://erw.chenlongwang.top

================================================================================
来源：http://udp.52xcode.cn

[E01] 拼接字符串
来源：http://xey.iojbl.cn


<!-- 参考信息 -->