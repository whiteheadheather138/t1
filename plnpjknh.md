代发 wailian999

TS:   同 JS
来源：http://yjm.xinyue.icu

Java: 方法内为块级作用域
来源：http://dwf.xylfe.cn

Go:   花括号块级作用域
来源：http://yxm.snrcjt.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://qam.ydzc1.top

C#:   块级作用域
来源：http://dsp.xuetiantiany.cn

[C11] 模块导入与导出
来源：http://koc.ppjwa.cn

Py:   from module import func
来源：http://fwf.jinqigufen.top

PHP:  require "file.php";  或 use App\Service;
来源：http://gxs.yongpay.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://mzd.cdnleiting.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://aji.jlsjyb.cn

Java: import java.util.List;
来源：http://hov.sysykeji.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ymg.guowangkeji.top

Ruby: require "json"; require_relative "./util"
来源：http://ejt.yj20258888.top

C#:   using System.Text;
来源：http://phm.andypj.xyz

[C12] 立即执行函数 IIFE
来源：http://hti.xylfe.cn

Py:   (lambda: print("run"))()
来源：http://xzt.feifeiyinyue.top

PHP:  (function () { echo "run"; })();
来源：http://efq.pengpengdd.cyou

JS:   (() => { console.log("run"); })();
来源：http://tqj.ppjwa.cn

TS:   (() => { console.log("run"); })();
来源：http://lln.wangdashe.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ciz.ctjpmb.com

Go:   func() { fmt.Println("run") }()
来源：http://yth.zhengqikj.top

Ruby: -> { puts "run" }.call
来源：http://cyl.guannengcc.top

C#:   // 无 IIFE：用静态构造函数
来源：http://yqf.nwbrower.top

[C13] 类型声明 / 类型注解
来源：http://kuk.feifeiyinyue.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ejp.xuanzx.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tsk.sufxvd.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://iwr.sweek.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jwm.sysykeji.top

Java: int add(int a, int b) { return a + b; }
来源：http://xjp.xingfuxueyuan.xyz

Go:   func add(a, b int) int
来源：http://fbh.gogol.net.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://skr.yvedp.cn

C#:   int Add(int a, int b) => a + b;
来源：http://frz.ivvv.top

[C14] 泛型函数
来源：http://wrd.vehdjk.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://lzm.gotoacloud.top

PHP:  // 无泛型
来源：http://ovh.zdbjq.cn

JS:   // 无泛型
来源：http://rdf.guannengcc.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://tik.sweek.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://qds.meibo888.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://dcb.zhaomingkeji.xyz

Ruby: # 无泛型
来源：http://pyj.hfpthk.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://gtd.ivvv.top

[C15] 解构 / 展开参数
来源：http://grs.fengsongda.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ucb.gogol.net.cn

PHP:  [$a, $b] = $pair;
来源：http://dlo.fzhhl.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://zew.zhixingplan.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://jbk.wangdashe.top

Java: // 无解构
来源：http://nsr.aibaodan.cn

Go:   // 无解构
来源：http://idf.yuxming.cn

Ruby: a, b = pair
来源：http://jhi.dianchejie.cn

C#:   var (a, b) = pair;
来源：http://dqo.cdnleiting.top

[C16] 函数 / 方法重载
来源：http://sqz.mhx1999.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://qbb.yongpay.top

PHP:  // 无重载
来源：http://opz.fanxiaobao.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://umc.jinyuanbaomall.cn

TS:   // 用联合类型或重载签名声明
来源：http://pax.fktsv.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://hnd.sweek.top

Go:   // 无重载：用不同函数名
来源：http://wsd.hcnkem.com

Ruby: # 无重载：靠动态参数
来源：http://uea.vehdjk.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://yzq.kuanghao11.cn

================================================================================
来源：http://zvq.zhengqikj.top

D. 数组 / 列表 / 集合
来源：http://hot.guowangkeji.top

================================================================================
来源：http://naf.pengpengdd.cyou

[D01] 创建数组 / 列表
来源：http://umm.yfazqb.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://qtq.jyoumei.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ujh.shanyushiyangkeji.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://rgx.nanxinkj.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://xca.yvedp.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://afv.pycfn.com

Go:   arr := []int{1, 2, 3}
来源：http://csk.yueranfly.top

Ruby: arr = [1, 2, 3]
来源：http://qaw.xylfe.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://eqm.gotoacloud.top

[D02] 追加元素到末尾
来源：http://vpn.cdnleiting.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://bmy.tianlin.xyz

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://fmd.zdbjq.cn

JS:   arr.push(4);
来源：http://cbq.chenjidiqi.icu

TS:   arr.push(4);
来源：http://tnj.yongpay.top

Java: list.add(4);
来源：http://psm.fzhhl.top

Go:   arr = append(arr, 4)
来源：http://apw.0kj1m.cn

Ruby: arr << 4; arr.push(5)
来源：http://mjz.yj20258888.top

C#:   list.Add(4);
来源：http://uqi.c1oappe.top

[D03] 在指定位置插入元素
来源：http://dsu.fzhhl.top

Py:   arr.insert(0, 0)
来源：http://dez.bbcook.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://qll.fanxiaobao.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ccl.smart0.xyz

TS:   arr.splice(0, 0, 0);
来源：http://pzq.birdmap.top

Java: list.add(0, 0);
来源：http://poh.meibo888.top

Go:   arr = append([]int{0}, arr...)
来源：http://brd.tanke756.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://vvt.meibo888.top

C#:   list.Insert(0, 0);
来源：http://vtn.aibaodan.cn

[D04] 删除元素
来源：http://qla.yvedp.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://auh.hammf.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://upc.ppjwa.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://pll.9152youxi.cn

TS:   arr.splice(0, 1);
来源：http://jzw.hammf.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://lpu.havefunace.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://nvh.9152youxi.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ios.pengpengdd.cyou

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://kos.tarul.cn

[D05] 访问与修改元素
来源：http://voc.bjfxy.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://xvo.cdnleiting.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wbu.epnwcf.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://eed.zycfv.cn

TS:   arr[0]; arr.at(-1);
来源：http://zpx.52xcode.cn

Java: list.get(0); list.set(0, 9);
来源：http://hih.daxiang520.top

Go:   arr[0]; arr[0] = 9
来源：http://puh.jianghu66.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://qbi.yj20258.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://kve.hammf.cn

[D06] 数组长度
来源：http://qrr.yanxiufei.cn

Py:   len(arr)
来源：http://hph.yj20258888.top

PHP:  count($arr);
来源：http://veu.jiagoushi.top

JS:   arr.length
来源：http://liz.wangshuangyany.cn

TS:   arr.length
来源：http://gli.zdqjudy.top

Java: list.size();
来源：http://ddl.xuetiantiany.cn

Go:   len(arr)
来源：http://mza.gotoacloud.top

Ruby: arr.length; arr.size
来源：http://mbo.shanyushiyangkeji.top

C#:   list.Count;
来源：http://nqa.yongpay.top

[D07] 切片 / 取子数组
来源：http://ijt.meibo888.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://fkn.cqqwz.cn

PHP:  array_slice($arr, 1, 3);
来源：http://sqr.sxryk.cn

JS:   arr.slice(1, 4);
来源：http://jks.cdnleiting.top

TS:   arr.slice(1, 4);
来源：http://vyh.yangfankeji.com

Java: list.subList(1, 4);
来源：http://vph.iojbl.cn

Go:   arr[1:4]
来源：http://xxj.gaohongyu789.top

Ruby: arr[1, 3]
来源：http://aia.jqgfzy.top

C#:   list.GetRange(1, 3);
来源：http://twm.zycfv.cn

[D08] 合并两个数组
来源：http://rki.zhoulong.xyz

Py:   a + b;  a.extend(b)
来源：http://lgc.zycfv.cn

PHP:  array_merge($a, $b);
来源：http://yvh.zhengqikj.top

JS:   [...a, ...b];  a.concat(b);
来源：http://yqn.ppjwa.cn

TS:   [...a, ...b];
来源：http://ehg.shzxlz.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://lzi.fehbvm.com

Go:   append(a, b...)
来源：http://xgb.zhoulong.xyz

Ruby: a + b;  a.concat(b)
来源：http://iif.pycfn.com

C#:   a.Concat(b).ToList()
来源：http://rfw.zycfv.cn

[D09] 排序（升序）
来源：http://qws.hnxiangtu.top

Py:   sorted(arr);  arr.sort()
来源：http://vti.zhixingplan.top

PHP:  sort($arr);
来源：http://oeq.cashguo.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mxv.ivvv.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://bck.cashguo.top

Java: Collections.sort(list);  list.sort(null);
来源：http://hqp.guowangkeji.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wvj.guowangkeji.top

Ruby: arr.sort
来源：http://mlo.ctjpmb.com

C#:   list.Sort();
来源：http://hsb.ctjpmb.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://fdz.sweek.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ytb.daxiang520.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ioy.cashguo.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hgr.yongpay.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://zdn.chenlongwang.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ofp.birdmap.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ejw.hammf.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://njg.xylfe.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://vso.zhiwuduotai.top

[D11] 反转数组
来源：http://vdi.daxiang520.top

Py:   arr[::-1];  arr.reverse()
来源：http://amm.ivvv.top

PHP:  array_reverse($arr);
来源：http://ljm.uphjek.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ffa.fktsv.cn

TS:   [...arr].reverse();
来源：http://dwb.chenjidiqi.icu

Java: Collections.reverse(list);
来源：http://cnt.yuanzhike.top

Go:   slices.Reverse(arr)
来源：http://ouv.hnxiangtu.top

Ruby: arr.reverse
来源：http://kfy.yuxming.cn

C#:   list.Reverse();
来源：http://wza.birdmap.top

[D12] 查找元素下标
来源：http://uio.hnxiangtu.top

Py:   arr.index(x);  x in arr
来源：http://vox.zhongyouzk.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://jvu.316326.xyz

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yjy.daxiang520.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://oyv.havefunace.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ahr.shangyingyoupin.top

Go:   slices.Index(arr, x)
来源：http://ims.tian-w.cn

Ruby: arr.index(x)
来源：http://wix.jianghu66.top

C#:   list.IndexOf(x);
来源：http://oqc.dianchejie.cn

[D13] 过滤（保留满足条件的）
来源：http://icm.zhiwuduotai.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://gab.fengsongda.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://sew.ppjwa.cn

JS:   arr.filter(x => x > 3)
来源：http://udd.yanxiufei.cn

TS:   arr.filter(x => x > 3)
来源：http://pzm.yj20258.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://bao.ivvv.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://msd.vehdjk.com

Ruby: arr.select { |x| x > 3 }
来源：http://gfm.gaohongyu789.top

C#:   list.Where(x => x > 3).ToList()
来源：http://fls.quarkkingdee.top

[D14] 映射转换（每个元素变形）
来源：http://vrk.gotoacloud.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://djd.xingfuxueyuan.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://qlq.sxryk.cn

JS:   arr.map(x => x * 2)
来源：http://jwx.xuetiantiany.cn

TS:   arr.map(x => x * 2)
来源：http://pbf.xylfe.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://vnq.aibaodan.cn

Go:   // 手写循环
来源：http://hef.meibo888.top

Ruby: arr.map { |x| x * 2 }
来源：http://btg.gaohongyu789.top

C#:   list.Select(x => x * 2).ToList()
来源：http://dxq.iojbl.cn

[D15] 去重
来源：http://keu.9152youxi.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ioo.chenlongwang.top

PHP:  array_unique($arr);
来源：http://mcq.gotoacloud.top

JS:   [...new Set(arr)]
来源：http://bdc.0kj1m.cn

TS:   [...new Set(arr)]
来源：http://uyg.jqgufenzy.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ded.316326.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://iha.nanxuanxn.top

Ruby: arr.uniq
来源：http://yqk.dianchejie.cn

C#:   list.Distinct().ToList()
来源：http://ove.yvedp.cn

[D16] 求和与平均值
来源：http://zxq.ehwqpu.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://sgb.hcnkem.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://fhq.hesvh.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://nmv.jinqigfzy.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://zng.fzhhl.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xso.zycfv.cn

Go:   // 手写循环累加
来源：http://sso.zhixingplan.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://nhy.dashuyun.cn

C#:   list.Sum();  list.Average()
来源：http://vqf.chenjidiqi.icu

[D17] 最大值与最小值
来源：http://lkk.xinyue.icu

Py:   max(arr);  min(arr)
来源：http://luq.xinyue.icu

PHP:  max($arr);  min($arr);
来源：http://iqt.ehwqpu.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://csb.zhijiandao.cn

TS:   Math.max(...arr);
来源：http://hps.jinghuilouyu.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://hts.yj20258.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://lyl.bbcook.cn

Ruby: arr.max;  arr.min
来源：http://lgb.fktsv.cn

C#:   list.Max();  list.Min()
来源：http://olu.fzhhl.top

[D18] 扁平化嵌套数组
来源：http://mre.tarul.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://bde.gotoacloud.top

PHP:  array_merge(...$nested);
来源：http://jlv.gzhubu.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://kzy.haohaochexian.top

TS:   nested.flat();
来源：http://yoh.shuidangran.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://xxh.tanke756.top

Go:   // 手写双层循环
来源：http://muh.yongpay.top

Ruby: nested.flatten
来源：http://sjf.quarkkingdee.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://xcn.fehbvm.com

[D19] 按字段分组
来源：http://nwp.fengsongda.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://zed.bbcook.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ftn.yuanzhike.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://jvj.jinghuilouyu.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://qxb.dianchejie.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://vqm.shzxlz.cn

Go:   // 手写 map[string][]T
来源：http://gbc.zdbjq.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://huh.0kj1m.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://kyh.shanyushiyangtech.top

[D20] 统计每个元素出现次数
来源：http://ufk.fanxiaobao.xyz

Py:   Counter(arr)
来源：http://tpk.jqgfzy.top

PHP:  array_count_values($arr);
来源：http://gmz.uphjek.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://aon.52xcode.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://not.yj20258888.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://css.hysaishi.cn

Go:   // 手写 map[T]int
来源：http://dqe.dashuyun.cn

Ruby: arr.tally
来源：http://yzi.ybcxt.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://qnl.cucudq.cn

[D21] 判断是否包含某元素
来源：http://ull.ydzc1.top

Py:   x in arr
来源：http://vco.yj202588.top

PHP:  in_array($x, $arr, true);
来源：http://cmt.yonumen.top

JS:   arr.includes(x)
来源：http://ojl.yvedp.cn

TS:   arr.includes(x)
来源：http://vms.iojbl.cn

Java: list.contains(x)
来源：http://vul.jqgfzy.top

Go:   slices.Contains(arr, x)
来源：http://rxz.hammf.cn

Ruby: arr.include?(x)
来源：http://hcb.nanxuanxn.top

C#:   list.Contains(x)
来源：http://nlq.chenlongwang.top

[D22] 复制数组（避免共享引用）
来源：http://dkl.uphjek.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://qur.quarkkingdee.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wil.fktsv.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://jux.jianghu66.top

TS:   [...arr];
来源：http://zfo.aibaodan.cn

Java: new ArrayList<>(list);
来源：http://mcz.hesvh.cn

Go:   copied := append([]int(nil), arr...)
来源：http://bzb.shuidangran.top

Ruby: arr.dup;  arr.clone
来源：http://qhd.chenlongwang.top

C#:   new List<int>(list);
来源：http://qej.fktsv.cn

[D23] reduce 累积计算
来源：http://eyi.sxryk.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://qfu.hcnkem.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://law.yonumen.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://sqg.mhx1999.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qit.meibo888.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://ugr.hesvh.cn

Go:   // 手写循环
来源：http://pdc.gaohongyu789.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ooi.sxryk.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://sgn.bjfxy.top

[D24] 字典 / Map 基本操作
来源：http://tjb.chenjidiqi.icu

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://qsk.birdmap.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://tri.sjlbkw.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ngo.shanyushiyangkeji.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://nvp.shanyushiyangkeji.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hix.jqgufenzy.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://xpl.ybcxt.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://eee.chenzaomai.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://xpg.pengpengdd.cyou

[D25] Set 集合去重与交并差
来源：http://lgi.c1oappe.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://fur.ctjpmb.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://odf.xinyue.icu

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://jlv.jqgfzy.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://thm.shzxlz.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://qhn.tianlin.xyz

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://zrj.zhijiandao.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://pom.shzxlz.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://yoz.hesvh.cn

[D26] 数组转字符串
来源：http://jza.wangdashe.top

Py:   ", ".join(map(str, arr))
来源：http://ruc.snrcjt.cn

PHP:  implode(", ", $arr);
来源：http://nht.yfazqb.com

JS:   arr.join(", ")
来源：http://mwx.yangfankeji.com

TS:   arr.join(", ")
来源：http://rvl.vehdjk.com

Java: String.join(", ", list)
来源：http://rtu.chenjidiqi.icu

Go:   strings.Join(strs, ", ")
来源：http://vvm.aizwys.cn

Ruby: arr.join(", ")
来源：http://dle.yuanzhike.top

C#:   string.Join(", ", list)
来源：http://saa.ehwqpu.com

================================================================================
来源：http://wac.meibo888.top

E. 字符串处理
来源：http://gfh.chenjidiqi.icu

================================================================================
来源：http://ybh.jinqigfzy.top

[E01] 拼接字符串
来源：http://tdz.hammf.cn


<!-- 参考信息 -->