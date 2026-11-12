代发 wailian999

C#:   块级作用域
来源：http://sin.xylfe.cn

[C11] 模块导入与导出
来源：http://uqi.bjfxy.top

Py:   from module import func
来源：http://lau.shuidangran.top

PHP:  require "file.php";  或 use App\Service;
来源：http://fbb.shzxlz.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://iqr.yangfankeji.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://esi.meibo888.top

Java: import java.util.List;
来源：http://zzb.yuanzhike.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ewv.jyoumei.cn

Ruby: require "json"; require_relative "./util"
来源：http://evn.gotoacloud.top

C#:   using System.Text;
来源：http://kns.yvedp.cn

[C12] 立即执行函数 IIFE
来源：http://bmz.yanxiufei.cn

Py:   (lambda: print("run"))()
来源：http://vja.meibo888.top

PHP:  (function () { echo "run"; })();
来源：http://iol.ydjk.org.cn

JS:   (() => { console.log("run"); })();
来源：http://dyj.jiagoushi.top

TS:   (() => { console.log("run"); })();
来源：http://qmz.cashguo.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://gnv.vehdjk.com

Go:   func() { fmt.Println("run") }()
来源：http://bmb.wangdashe.top

Ruby: -> { puts "run" }.call
来源：http://gxo.fengsongda.top

C#:   // 无 IIFE：用静态构造函数
来源：http://iob.dashuyun.cn

[C13] 类型声明 / 类型注解
来源：http://pcb.gotoacloud.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://nke.jyoumei.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://euc.yanxiufei.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://qjw.mhx1999.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zqv.mhx1999.top

Java: int add(int a, int b) { return a + b; }
来源：http://iat.xuetiantiany.cn

Go:   func add(a, b int) int
来源：http://pcm.shanyushiyangtech.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://jgj.uphjek.com

C#:   int Add(int a, int b) => a + b;
来源：http://bna.hysaishi.cn

[C14] 泛型函数
来源：http://stn.gogol.net.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://clt.vehdjk.com

PHP:  // 无泛型
来源：http://jbj.gogol.net.cn

JS:   // 无泛型
来源：http://cib.yj202588.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://vay.pengpengdd.cyou

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://gig.jinyuanbaomall.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://smu.ybcxt.top

Ruby: # 无泛型
来源：http://cqp.zdqjudy.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://cta.cdnleiting.top

[C15] 解构 / 展开参数
来源：http://nak.ivvv.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://sqz.chenjidiqi.icu

PHP:  [$a, $b] = $pair;
来源：http://hsg.tianlin.xyz

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://lun.yongpay.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://nit.snrcjt.cn

Java: // 无解构
来源：http://goy.316326.xyz

Go:   // 无解构
来源：http://rab.xuanzx.com

Ruby: a, b = pair
来源：http://jzm.havefunace.top

C#:   var (a, b) = pair;
来源：http://mbh.yj20258.top

[C16] 函数 / 方法重载
来源：http://fgc.wangdashe.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://qnc.yj202588.top

PHP:  // 无重载
来源：http://xrp.yj202588.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://den.sweek.top

TS:   // 用联合类型或重载签名声明
来源：http://oor.316326.xyz

Java: void f(int a) {}  void f(String a) {}
来源：http://nxa.epnwcf.com

Go:   // 无重载：用不同函数名
来源：http://asp.yuxming.cn

Ruby: # 无重载：靠动态参数
来源：http://qte.hywenlv.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://vds.xinyue.icu

================================================================================
来源：http://xoy.bbcook.cn

D. 数组 / 列表 / 集合
来源：http://lkg.dashuyun.cn

================================================================================
来源：http://mhn.316326.xyz

[D01] 创建数组 / 列表
来源：http://rkn.svipenyu.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://iue.xuetiantiany.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://jpk.havefunace.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://yvu.316326.xyz

TS:   const arr: number[] = [1, 2, 3];
来源：http://cvp.gogol.net.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://fsu.jqgfzy.top

Go:   arr := []int{1, 2, 3}
来源：http://rzd.wangshuangyany.cn

Ruby: arr = [1, 2, 3]
来源：http://fol.xuanzx.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hvt.cheryme.top

[D02] 追加元素到末尾
来源：http://drb.mhx1999.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://tva.yuanzhike.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://dwp.ybcxt.top

JS:   arr.push(4);
来源：http://lrc.nanxuanxn.top

TS:   arr.push(4);
来源：http://nah.jinghuilouyu.cn

Java: list.add(4);
来源：http://pgf.sjlbkw.cn

Go:   arr = append(arr, 4)
来源：http://rde.hywenlv.cn

Ruby: arr << 4; arr.push(5)
来源：http://rkf.316326.xyz

C#:   list.Add(4);
来源：http://hhg.0kj1m.cn

[D03] 在指定位置插入元素
来源：http://esx.kuanghao11.cn

Py:   arr.insert(0, 0)
来源：http://xsv.9152youxi.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://art.xziqi.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://gqe.quarkkingdee.top

TS:   arr.splice(0, 0, 0);
来源：http://dtb.guannengcc.top

Java: list.add(0, 0);
来源：http://erv.bjfxy.top

Go:   arr = append([]int{0}, arr...)
来源：http://msx.ywan-chungtsiang.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ujr.yongpay.top

C#:   list.Insert(0, 0);
来源：http://eyf.yj20258888.top

[D04] 删除元素
来源：http://upd.yonumen.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ztk.sysykeji.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://rqr.daxiang520.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://fst.feifeiyinyue.top

TS:   arr.splice(0, 1);
来源：http://zrx.cashguo.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mgc.sweek.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://xjo.daria6918.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wtt.yuxming.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://aue.quarkkingdee.top

[D05] 访问与修改元素
来源：http://glv.mhx1999.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://izx.shzxlz.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://rcn.jianghu66.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ycs.wangdashe.top

TS:   arr[0]; arr.at(-1);
来源：http://pgw.hammf.cn

Java: list.get(0); list.set(0, 9);
来源：http://aeq.wangshuangyany.cn

Go:   arr[0]; arr[0] = 9
来源：http://snv.sweek.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://qym.iojbl.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://oql.yuxming.cn

[D06] 数组长度
来源：http://vzi.hywenlv.cn

Py:   len(arr)
来源：http://cyi.yj202588.top

PHP:  count($arr);
来源：http://xbe.jinqigfzy.top

JS:   arr.length
来源：http://val.jianghu66.top

TS:   arr.length
来源：http://ddl.hnxiangtu.top

Java: list.size();
来源：http://kov.hfpthk.cn

Go:   len(arr)
来源：http://hbo.haohaochexian.top

Ruby: arr.length; arr.size
来源：http://hja.hnxiangtu.top

C#:   list.Count;
来源：http://zmn.hfpthk.cn

[D07] 切片 / 取子数组
来源：http://lws.xuanzx.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ltd.yj202588.top

PHP:  array_slice($arr, 1, 3);
来源：http://eyq.0kj1m.cn

JS:   arr.slice(1, 4);
来源：http://lvq.kuanghao11.cn

TS:   arr.slice(1, 4);
来源：http://ogz.jinyuanbaomall.cn

Java: list.subList(1, 4);
来源：http://nvo.svipenyu.cn

Go:   arr[1:4]
来源：http://ppk.bbcook.cn

Ruby: arr[1, 3]
来源：http://bzc.iojbl.cn

C#:   list.GetRange(1, 3);
来源：http://wsn.birdmap.top

[D08] 合并两个数组
来源：http://bzj.chenzaomai.com

Py:   a + b;  a.extend(b)
来源：http://vzq.zhaomingkeji.xyz

PHP:  array_merge($a, $b);
来源：http://nte.gotoacloud.top

JS:   [...a, ...b];  a.concat(b);
来源：http://kfe.meibo888.top

TS:   [...a, ...b];
来源：http://aac.ctjpmb.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ayx.yfazqb.com

Go:   append(a, b...)
来源：http://hzd.jqgfzy.top

Ruby: a + b;  a.concat(b)
来源：http://mxe.ydzc1.top

C#:   a.Concat(b).ToList()
来源：http://snh.hnqzz.top

[D09] 排序（升序）
来源：http://nhe.tanke756.top

Py:   sorted(arr);  arr.sort()
来源：http://pcz.xziqi.cn

PHP:  sort($arr);
来源：http://oog.chenjidiqi.icu

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://tlo.316326.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://rln.chenjidiqi.icu

Java: Collections.sort(list);  list.sort(null);
来源：http://zmh.hysaishi.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ero.tarul.cn

Ruby: arr.sort
来源：http://ocb.hongshengwenyu.top

C#:   list.Sort();
来源：http://yrc.xylfe.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://rfl.tian-w.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mef.shzxlz.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mmv.xinyue.icu

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://non.c1oappe.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ncb.jinghuilouyu.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://tdu.jqgufenzy.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://iuv.chenzaomai.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://zbc.hywenlv.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://slz.birdmap.top

[D11] 反转数组
来源：http://fbp.yangfankeji.com

Py:   arr[::-1];  arr.reverse()
来源：http://gwh.zhaomingkeji.xyz

PHP:  array_reverse($arr);
来源：http://luj.svipenyu.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://kpk.jinghuilouyu.cn

TS:   [...arr].reverse();
来源：http://ijf.ivvv.top

Java: Collections.reverse(list);
来源：http://atx.xingfuxueyuan.xyz

Go:   slices.Reverse(arr)
来源：http://dlw.hesvh.cn

Ruby: arr.reverse
来源：http://fhu.fehbvm.com

C#:   list.Reverse();
来源：http://nkm.chenjidiqi.icu

[D12] 查找元素下标
来源：http://xej.fzhhl.top

Py:   arr.index(x);  x in arr
来源：http://nmi.cdnleiting.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://uhv.hysaishi.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wpl.jyoumei.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wzj.xingfuxueyuan.xyz

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://jdh.jinqigufen.top

Go:   slices.Index(arr, x)
来源：http://plu.daxiang520.top

Ruby: arr.index(x)
来源：http://jhz.fanxiaobao.xyz

C#:   list.IndexOf(x);
来源：http://cus.kuanghao11.cn

[D13] 过滤（保留满足条件的）
来源：http://azp.yuanzhike.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://log.jinyuanbaomall.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://nrn.gotoacloud.top

JS:   arr.filter(x => x > 3)
来源：http://szs.jianghu66.top

TS:   arr.filter(x => x > 3)
来源：http://njo.ehwqpu.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ixg.hywenlv.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://knr.yvedp.cn

Ruby: arr.select { |x| x > 3 }
来源：http://nhm.nanxuanxn.top

C#:   list.Where(x => x > 3).ToList()
来源：http://phl.zdqjudy.top

[D14] 映射转换（每个元素变形）
来源：http://fpf.cashguo.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://vcj.yangfankeji.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zbl.jqgfzy.top

JS:   arr.map(x => x * 2)
来源：http://qau.bjfxy.top

TS:   arr.map(x => x * 2)
来源：http://hba.ppjwa.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://rrw.gotoacloud.top

Go:   // 手写循环
来源：http://yzd.tarul.cn

Ruby: arr.map { |x| x * 2 }
来源：http://rcn.hnxiangtu.top

C#:   list.Select(x => x * 2).ToList()
来源：http://hjg.jinyuanbaomall.cn

[D15] 去重
来源：http://cpz.zhoulong.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hit.vehdjk.com

PHP:  array_unique($arr);
来源：http://bey.sufxvd.cn

JS:   [...new Set(arr)]
来源：http://fhx.shanyushiyangtech.top

TS:   [...new Set(arr)]
来源：http://eph.ivvv.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://pom.tianlin.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://fmy.jinqigfzy.top

Ruby: arr.uniq
来源：http://eyl.0kj1m.cn

C#:   list.Distinct().ToList()
来源：http://paw.cqqwz.cn

[D16] 求和与平均值
来源：http://dii.c1oappe.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ytu.ydzc1.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://fqb.jinghuilouyu.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://iah.c1oappe.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wms.zhixingplan.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://nba.jyoumei.cn

Go:   // 手写循环累加
来源：http://fpt.xuetiantiany.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://orx.jqgfzy.top

C#:   list.Sum();  list.Average()
来源：http://con.daxiang520.top

[D17] 最大值与最小值
来源：http://kny.redwolf501.top

Py:   max(arr);  min(arr)
来源：http://kld.zhiwuduotai.top

PHP:  max($arr);  min($arr);
来源：http://xfz.chenlongwang.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://kcl.tarul.cn

TS:   Math.max(...arr);
来源：http://wff.jlsjyb.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://dif.smart0.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ajy.xingfuxueyuan.xyz

Ruby: arr.max;  arr.min
来源：http://cpc.tanke756.top

C#:   list.Max();  list.Min()
来源：http://hpk.yonumen.top

[D18] 扁平化嵌套数组
来源：http://yuc.havefunace.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://val.xinyue.icu

PHP:  array_merge(...$nested);
来源：http://ohm.nanxinkj.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://gbh.ybcxt.top

TS:   nested.flat();
来源：http://tre.xuetiantiany.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://goj.dianchejie.cn

Go:   // 手写双层循环
来源：http://eni.sxryk.cn

Ruby: nested.flatten
来源：http://zvg.pengpengdd.cyou

C#:   nested.SelectMany(x => x).ToList()
来源：http://qwd.yonumen.top

[D19] 按字段分组
来源：http://gqv.zhoulong.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://shr.hcnkem.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mbx.mhx1999.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://jrx.ppjwa.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://pju.guannengcc.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://pjj.jinghuilouyu.cn

Go:   // 手写 map[string][]T
来源：http://xpp.ppjwa.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://sey.9152youxi.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://igi.zhixingplan.top

[D20] 统计每个元素出现次数
来源：http://wvp.xuetiantiany.cn

Py:   Counter(arr)
来源：http://iai.hammf.cn

PHP:  array_count_values($arr);
来源：http://yio.shuidangran.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wsq.zhijiandao.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://whx.ehwqpu.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wxf.hnqzz.top

Go:   // 手写 map[T]int
来源：http://cml.hysaishi.cn

Ruby: arr.tally
来源：http://xdh.yuanzhike.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://dwo.sjlbkw.cn

[D21] 判断是否包含某元素
来源：http://isd.tianlin.xyz

Py:   x in arr
来源：http://qcd.cucudq.cn

PHP:  in_array($x, $arr, true);
来源：http://amu.c1oappe.top

JS:   arr.includes(x)
来源：http://iux.jiagoushi.top

TS:   arr.includes(x)
来源：http://vwe.snrcjt.cn

Java: list.contains(x)
来源：http://win.c1oappe.top

Go:   slices.Contains(arr, x)
来源：http://lud.yuanzhike.top

Ruby: arr.include?(x)
来源：http://fly.kuanghao11.cn

C#:   list.Contains(x)
来源：http://sfz.hesvh.cn

[D22] 复制数组（避免共享引用）
来源：http://qjm.pengpengdd.cyou

Py:   arr.copy();  arr[:];  list(arr)
来源：http://uqd.ivvv.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://gbh.jqgufenzy.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://cfr.ctjpmb.com

TS:   [...arr];
来源：http://wlg.pengpengdd.cyou

Java: new ArrayList<>(list);
来源：http://dzt.hongshengwenyu.top

Go:   copied := append([]int(nil), arr...)
来源：http://qls.zhiwuduotai.top

Ruby: arr.dup;  arr.clone
来源：http://msc.mhx1999.top

C#:   new List<int>(list);
来源：http://fvn.fanxiaobao.xyz

[D23] reduce 累积计算
来源：http://msy.jqgfzy.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zxh.gotoacloud.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://rjr.tianlin.xyz

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dvd.cdnleiting.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rbb.c1oappe.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://nrk.yonumen.top

Go:   // 手写循环
来源：http://zbw.hnxiangtu.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://tss.tian-w.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://xmm.9152youxi.cn

[D24] 字典 / Map 基本操作
来源：http://auz.yvedp.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://jxh.sysykeji.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ddm.shangyingyoupin.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://dav.hnxiangtu.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://jbr.zhoulong.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://iom.sjlbkw.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://qwb.zhoulong.xyz

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://xbu.chenzaomai.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://yeq.zycfv.cn

[D25] Set 集合去重与交并差
来源：http://hyp.zdbjq.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://pvx.zdbjq.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ity.gaohongyu789.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://lqr.hnqzz.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://bje.xingfuxueyuan.xyz

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://arg.kuanghao11.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://lud.sjlbkw.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mag.sweek.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mtt.xylfe.cn

[D26] 数组转字符串
来源：http://stf.vehdjk.com

Py:   ", ".join(map(str, arr))
来源：http://oqs.jqgufenzy.top

PHP:  implode(", ", $arr);
来源：http://yyi.aizwys.cn

JS:   arr.join(", ")
来源：http://olj.hnxiangtu.top

TS:   arr.join(", ")
来源：http://nqg.daxiang520.top

Java: String.join(", ", list)
来源：http://ioy.xinyue.icu

Go:   strings.Join(strs, ", ")
来源：http://ttc.ydzc1.top

Ruby: arr.join(", ")
来源：http://qwk.zycfv.cn

C#:   string.Join(", ", list)
来源：http://iox.tarul.cn

================================================================================
来源：http://oez.sjlbkw.cn

E. 字符串处理
来源：http://cuj.yj202588.top

================================================================================
来源：http://neq.jyoumei.cn

[E01] 拼接字符串
来源：http://ukk.yj20258.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://lbe.fehbvm.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://adv.hammf.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://jjw.ybcxt.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://you.guowangkeji.top


<!-- 参考信息 -->