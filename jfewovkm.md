代发 wailian999

TS:   同 JS
来源：http://kfi.aizwys.cn

Java: 方法内为块级作用域
来源：http://xlk.dianchejie.cn

Go:   花括号块级作用域
来源：http://sah.nanxuanxn.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ghq.ydzc1.top

C#:   块级作用域
来源：http://shn.hesvh.cn

[C11] 模块导入与导出
来源：http://hdv.ehwqpu.com

Py:   from module import func
来源：http://mck.pengpengdd.cyou

PHP:  require "file.php";  或 use App\Service;
来源：http://wzj.yangfankeji.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://ufq.iojbl.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://dbi.redwolf501.top

Java: import java.util.List;
来源：http://cnq.feifeiyinyue.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://gna.fktsv.cn

Ruby: require "json"; require_relative "./util"
来源：http://got.hcnkem.com

C#:   using System.Text;
来源：http://fqx.hongshengwenyu.top

[C12] 立即执行函数 IIFE
来源：http://nqp.vqdsnc.cn

Py:   (lambda: print("run"))()
来源：http://dpm.cdnleiting.top

PHP:  (function () { echo "run"; })();
来源：http://rmb.zhongyouzk.top

JS:   (() => { console.log("run"); })();
来源：http://qiq.fehbvm.com

TS:   (() => { console.log("run"); })();
来源：http://hln.jinqigfzy.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jzq.hysaishi.cn

Go:   func() { fmt.Println("run") }()
来源：http://iib.wangdashe.top

Ruby: -> { puts "run" }.call
来源：http://rhw.daxiang520.top

C#:   // 无 IIFE：用静态构造函数
来源：http://wzr.fktsv.cn

[C13] 类型声明 / 类型注解
来源：http://tgs.316326.xyz

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://yvv.xuetiantiany.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://edy.aizwys.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://opu.daria6918.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zfx.sysykeji.top

Java: int add(int a, int b) { return a + b; }
来源：http://ifu.uphjek.com

Go:   func add(a, b int) int
来源：http://xmr.gogol.net.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://xsa.sweek.top

C#:   int Add(int a, int b) => a + b;
来源：http://ygi.cucudq.cn

[C14] 泛型函数
来源：http://cru.zdqjudy.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zrq.hysaishi.cn

PHP:  // 无泛型
来源：http://kfo.hysaishi.cn

JS:   // 无泛型
来源：http://gan.nanxuanxn.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://nkz.yuanzhike.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://skc.yj20258888.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://stw.bjfxy.top

Ruby: # 无泛型
来源：http://ulm.zdqjudy.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mzw.ehwqpu.com

[C15] 解构 / 展开参数
来源：http://wkn.sxryk.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mpo.yfazqb.com

PHP:  [$a, $b] = $pair;
来源：http://fme.nanxuanxn.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://jib.yanxiufei.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://bcl.yuanzhike.top

Java: // 无解构
来源：http://deg.aizwys.cn

Go:   // 无解构
来源：http://whr.jinghuilouyu.cn

Ruby: a, b = pair
来源：http://koc.jianghu66.top

C#:   var (a, b) = pair;
来源：http://eul.jinghuilouyu.cn

[C16] 函数 / 方法重载
来源：http://dhw.zhengqikj.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vgq.0kj1m.cn

PHP:  // 无重载
来源：http://mrp.9152youxi.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://hgs.yj20258888.top

TS:   // 用联合类型或重载签名声明
来源：http://uqz.guowangkeji.top

Java: void f(int a) {}  void f(String a) {}
来源：http://drh.yj202588.top

Go:   // 无重载：用不同函数名
来源：http://lfd.bjfxy.top

Ruby: # 无重载：靠动态参数
来源：http://anf.wangshuangyany.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://dho.kuanghao11.cn

================================================================================
来源：http://xys.ehwqpu.com

D. 数组 / 列表 / 集合
来源：http://tkl.0kj1m.cn

================================================================================
来源：http://qse.c1oappe.top

[D01] 创建数组 / 列表
来源：http://qav.jqgfzy.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://vpd.dashuyun.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://jql.jianghu66.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://iot.tarul.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://pyw.bjfxy.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://kno.bjfxy.top

Go:   arr := []int{1, 2, 3}
来源：http://gaa.birdmap.top

Ruby: arr = [1, 2, 3]
来源：http://rfe.xylfe.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://xru.sufxvd.cn

[D02] 追加元素到末尾
来源：http://nyj.zhongyouzk.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://syb.fzhhl.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wxf.chenzaomai.com

JS:   arr.push(4);
来源：http://mla.birdmap.top

TS:   arr.push(4);
来源：http://exr.snrcjt.cn

Java: list.add(4);
来源：http://wvm.tian-w.cn

Go:   arr = append(arr, 4)
来源：http://tus.nanxuanxn.top

Ruby: arr << 4; arr.push(5)
来源：http://fgb.gotoacloud.top

C#:   list.Add(4);
来源：http://brt.xuanzx.com

[D03] 在指定位置插入元素
来源：http://uap.ybcxt.top

Py:   arr.insert(0, 0)
来源：http://wzx.cqqwz.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://fgy.yj20258888.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://bsz.yj20258888.top

TS:   arr.splice(0, 0, 0);
来源：http://xqu.sweek.top

Java: list.add(0, 0);
来源：http://xfq.jinghuilouyu.cn

Go:   arr = append([]int{0}, arr...)
来源：http://jbb.hysaishi.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://odh.fzhhl.top

C#:   list.Insert(0, 0);
来源：http://dyc.cashguo.top

[D04] 删除元素
来源：http://aqv.gogol.net.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://jep.xuetiantiany.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://knf.jlsjyb.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://bbu.xuanzx.com

TS:   arr.splice(0, 1);
来源：http://tpg.ctjpmb.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mql.daxiang520.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://uay.gaohongyu789.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://qac.jinqigufen.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://pzz.jyoumei.cn

[D05] 访问与修改元素
来源：http://wqd.fzhhl.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://yby.dianchejie.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://rus.ybcxt.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://qab.chenzaomai.com

TS:   arr[0]; arr.at(-1);
来源：http://brk.hammf.cn

Java: list.get(0); list.set(0, 9);
来源：http://nbu.chenjidiqi.icu

Go:   arr[0]; arr[0] = 9
来源：http://icp.zycfv.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://pzc.dianchejie.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://rmp.nanxuanxn.top

[D06] 数组长度
来源：http://pdl.sysykeji.top

Py:   len(arr)
来源：http://boi.sufxvd.cn

PHP:  count($arr);
来源：http://tzm.xingfuxueyuan.xyz

JS:   arr.length
来源：http://kyi.redwolf501.top

TS:   arr.length
来源：http://gex.zhengqikj.top

Java: list.size();
来源：http://bux.ivvv.top

Go:   len(arr)
来源：http://cbs.chenjidiqi.icu

Ruby: arr.length; arr.size
来源：http://gkg.jinqigfzy.top

C#:   list.Count;
来源：http://jee.guannengcc.top

[D07] 切片 / 取子数组
来源：http://nmu.ivvv.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://edd.shanyushiyangkeji.top

PHP:  array_slice($arr, 1, 3);
来源：http://qmd.gzhubu.top

JS:   arr.slice(1, 4);
来源：http://hxu.hfpthk.cn

TS:   arr.slice(1, 4);
来源：http://pqx.uphjek.com

Java: list.subList(1, 4);
来源：http://sca.yuxming.cn

Go:   arr[1:4]
来源：http://mmz.fengsongda.top

Ruby: arr[1, 3]
来源：http://jtn.nanxinkj.top

C#:   list.GetRange(1, 3);
来源：http://kom.shanyushiyangtech.top

[D08] 合并两个数组
来源：http://lhg.xylfe.cn

Py:   a + b;  a.extend(b)
来源：http://bol.jqgufenzy.top

PHP:  array_merge($a, $b);
来源：http://dbm.xuanzx.com

JS:   [...a, ...b];  a.concat(b);
来源：http://wgx.sweek.top

TS:   [...a, ...b];
来源：http://fwc.zdbjq.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://riw.zycfv.cn

Go:   append(a, b...)
来源：http://ece.hnqzz.top

Ruby: a + b;  a.concat(b)
来源：http://epp.vqdsnc.cn

C#:   a.Concat(b).ToList()
来源：http://gpo.jianghu66.top

[D09] 排序（升序）
来源：http://rtg.svipenyu.cn

Py:   sorted(arr);  arr.sort()
来源：http://pim.feifeiyinyue.top

PHP:  sort($arr);
来源：http://she.daxiang520.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ons.havefunace.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://hqv.jinyuanbaomall.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ghn.chenzaomai.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://lyw.jqgufenzy.top

Ruby: arr.sort
来源：http://lkp.uphjek.com

C#:   list.Sort();
来源：http://uap.0kj1m.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://qqc.zdbjq.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://nzo.shuidangran.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fyl.aibaodan.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://iey.gaohongyu789.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://myh.ywan-chungtsiang.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ubq.epnwcf.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://zke.smart0.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://zfs.gaohongyu789.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://fxi.yfazqb.com

[D11] 反转数组
来源：http://tve.daria6918.cn

Py:   arr[::-1];  arr.reverse()
来源：http://psz.jqgufenzy.top

PHP:  array_reverse($arr);
来源：http://imm.dianchejie.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://oau.yj20258888.top

TS:   [...arr].reverse();
来源：http://zlo.shzxlz.cn

Java: Collections.reverse(list);
来源：http://sik.pengpengdd.cyou

Go:   slices.Reverse(arr)
来源：http://utg.ctjpmb.com

Ruby: arr.reverse
来源：http://ocz.xziqi.cn

C#:   list.Reverse();
来源：http://csn.epnwcf.com

[D12] 查找元素下标
来源：http://mos.guowangkeji.top

Py:   arr.index(x);  x in arr
来源：http://ygd.gotoacloud.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://gdx.ydzc1.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zzj.uphjek.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dyk.jlsjyb.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://cjb.xingfuxueyuan.xyz

Go:   slices.Index(arr, x)
来源：http://wib.yueranfly.top

Ruby: arr.index(x)
来源：http://azt.chenlongwang.top

C#:   list.IndexOf(x);
来源：http://vbh.fktsv.cn

[D13] 过滤（保留满足条件的）
来源：http://irt.yanxiufei.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://kat.hnxiangtu.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://sey.jinyuanbaomall.cn

JS:   arr.filter(x => x > 3)
来源：http://kho.guannengcc.top

TS:   arr.filter(x => x > 3)
来源：http://yce.316326.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://xpz.yj20258.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ozp.jiagoushi.top

Ruby: arr.select { |x| x > 3 }
来源：http://prm.fehbvm.com

C#:   list.Where(x => x > 3).ToList()
来源：http://kxj.gotoacloud.top

[D14] 映射转换（每个元素变形）
来源：http://tzy.ydzc1.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wbr.sysykeji.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wfd.fengsongda.top

JS:   arr.map(x => x * 2)
来源：http://swy.gzhubu.top

TS:   arr.map(x => x * 2)
来源：http://wyy.aibaodan.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://kkh.ydzc1.top

Go:   // 手写循环
来源：http://rzo.chenjidiqi.icu

Ruby: arr.map { |x| x * 2 }
来源：http://gqs.fzhhl.top

C#:   list.Select(x => x * 2).ToList()
来源：http://esf.xuanzx.com

[D15] 去重
来源：http://qsm.xinyue.icu

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://vzr.sweek.top

PHP:  array_unique($arr);
来源：http://jol.feifeiyinyue.top

JS:   [...new Set(arr)]
来源：http://xal.pengpengdd.cyou

TS:   [...new Set(arr)]
来源：http://zml.hongshengwenyu.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hnl.feifeiyinyue.top

Go:   // 用 map[T]struct{} 手写
来源：http://izh.wangdashe.top

Ruby: arr.uniq
来源：http://efo.yongpay.top

C#:   list.Distinct().ToList()
来源：http://rzi.nanxuanxn.top

[D16] 求和与平均值
来源：http://hyu.316326.xyz

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://zwl.fktsv.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://lxq.tianlin.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://gxl.mhx1999.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://aae.gotoacloud.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://nqg.xziqi.cn

Go:   // 手写循环累加
来源：http://mvn.chenzaomai.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://fqm.yangfankeji.com

C#:   list.Sum();  list.Average()
来源：http://tvd.vehdjk.com

[D17] 最大值与最小值
来源：http://rjk.ybcxt.top

Py:   max(arr);  min(arr)
来源：http://tbg.yonumen.top

PHP:  max($arr);  min($arr);
来源：http://zak.guannengcc.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://yfg.shuidangran.top

TS:   Math.max(...arr);
来源：http://igc.cashguo.top

Java: Collections.max(list);  Collections.min(list);
来源：http://hei.hnqzz.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://iiz.daria6918.cn

Ruby: arr.max;  arr.min
来源：http://uge.jinyuanbaomall.cn

C#:   list.Max();  list.Min()
来源：http://oxc.vqdsnc.cn

[D18] 扁平化嵌套数组
来源：http://sie.epnwcf.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://tnc.fanxiaobao.xyz

PHP:  array_merge(...$nested);
来源：http://aav.vehdjk.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://jgv.xuetiantiany.cn

TS:   nested.flat();
来源：http://tst.jqgufenzy.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://rye.cucudq.cn

Go:   // 手写双层循环
来源：http://qqs.gogol.net.cn

Ruby: nested.flatten
来源：http://owm.yanxiufei.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://zgm.ybcxt.top

[D19] 按字段分组
来源：http://nmk.shuidangran.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mnh.fehbvm.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://plg.bjfxy.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://glx.guowangkeji.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://obv.yanxiufei.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://tnm.cucudq.cn

Go:   // 手写 map[string][]T
来源：http://dij.hammf.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://hou.zhongyouzk.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://xpy.yangfankeji.com

[D20] 统计每个元素出现次数
来源：http://ehy.52xcode.cn

Py:   Counter(arr)
来源：http://ejy.jiagoushi.top

PHP:  array_count_values($arr);
来源：http://azr.zhijiandao.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://uoe.tianlin.xyz

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ito.sufxvd.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://bnn.jinghuilouyu.cn

Go:   // 手写 map[T]int
来源：http://jzp.jqgufenzy.top

Ruby: arr.tally
来源：http://pty.ppjwa.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://yfm.jlsjyb.cn

[D21] 判断是否包含某元素
来源：http://ofq.yonumen.top

Py:   x in arr
来源：http://qzq.shanyushiyangtech.top

PHP:  in_array($x, $arr, true);
来源：http://sls.0kj1m.cn

JS:   arr.includes(x)
来源：http://pae.zhixingplan.top

TS:   arr.includes(x)
来源：http://kzb.cucudq.cn

Java: list.contains(x)
来源：http://hgx.xziqi.cn

Go:   slices.Contains(arr, x)
来源：http://dbb.birdmap.top

Ruby: arr.include?(x)
来源：http://fsx.gogol.net.cn

C#:   list.Contains(x)
来源：http://loi.redwolf501.top

[D22] 复制数组（避免共享引用）
来源：http://gzt.birdmap.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hsb.feifeiyinyue.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://jyb.feifeiyinyue.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://fas.fanxiaobao.xyz

TS:   [...arr];
来源：http://oik.dashuyun.cn

Java: new ArrayList<>(list);
来源：http://xpr.ctjpmb.com

Go:   copied := append([]int(nil), arr...)
来源：http://mxd.c1oappe.top

Ruby: arr.dup;  arr.clone
来源：http://qkg.iojbl.cn

C#:   new List<int>(list);
来源：http://vmc.cashguo.top

[D23] reduce 累积计算
来源：http://emf.yangfankeji.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hmv.sjlbkw.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://jaa.svipenyu.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://oyu.cdnleiting.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xoz.pengpengdd.cyou

Java: list.stream().reduce(0, Integer::sum)
来源：http://xuf.sxryk.cn

Go:   // 手写循环
来源：http://jjl.cqqwz.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://yxk.bjfxy.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://kle.zdqjudy.top

[D24] 字典 / Map 基本操作
来源：http://scp.tian-w.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://vhc.zhengqikj.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://jbr.hywenlv.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ybk.yongpay.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://usm.ivvv.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mne.cashguo.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://uyq.yfazqb.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://vyd.bbcook.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://iqz.cqqwz.cn

[D25] Set 集合去重与交并差
来源：http://wkz.hnqzz.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hds.nanxinkj.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://beh.iojbl.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://bkb.xingfuxueyuan.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://rpl.zhoulong.xyz

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://jfo.hysaishi.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://szo.kuanghao11.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://sbt.tarul.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://oxl.guannengcc.top

[D26] 数组转字符串
来源：http://vws.yangfankeji.com

Py:   ", ".join(map(str, arr))
来源：http://zlv.zhongyouzk.top

PHP:  implode(", ", $arr);
来源：http://rap.0kj1m.cn

JS:   arr.join(", ")
来源：http://lzr.zhaomingkeji.xyz

TS:   arr.join(", ")
来源：http://zvh.sjlbkw.cn

Java: String.join(", ", list)
来源：http://hca.ppjwa.cn

Go:   strings.Join(strs, ", ")
来源：http://yrs.nwbrower.top

Ruby: arr.join(", ")
来源：http://zym.gogol.net.cn

C#:   string.Join(", ", list)
来源：http://vin.shanyushiyangtech.top

================================================================================
来源：http://azs.hfpthk.cn

E. 字符串处理
来源：http://gek.havefunace.top

================================================================================
来源：http://jlc.ppjwa.cn

[E01] 拼接字符串
来源：http://xnk.dianchejie.cn


<!-- 参考信息 -->