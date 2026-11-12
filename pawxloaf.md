代发 wailian999

TS:   同 JS
来源：http://jic.feifeiyinyue.top

Java: 方法内为块级作用域
来源：http://oot.shangyingyoupin.top

Go:   花括号块级作用域
来源：http://tvr.yj20258.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://nhe.hnqzz.top

C#:   块级作用域
来源：http://bbj.wangshuangyany.cn

[C11] 模块导入与导出
来源：http://hjl.jiagoushi.top

Py:   from module import func
来源：http://ini.ydjk.org.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://shf.yuxming.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://kvb.bbcook.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://tgj.redwolf501.top

Java: import java.util.List;
来源：http://cji.ydzc1.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://vlm.xylfe.cn

Ruby: require "json"; require_relative "./util"
来源：http://aib.svipenyu.cn

C#:   using System.Text;
来源：http://fyp.jqgufenzy.top

[C12] 立即执行函数 IIFE
来源：http://qlh.jianghu66.top

Py:   (lambda: print("run"))()
来源：http://tde.jinqigfzy.top

PHP:  (function () { echo "run"; })();
来源：http://muc.zdqjudy.top

JS:   (() => { console.log("run"); })();
来源：http://hzj.quarkkingdee.top

TS:   (() => { console.log("run"); })();
来源：http://rwy.gzhubu.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://atd.yj202588.top

Go:   func() { fmt.Println("run") }()
来源：http://ypa.ppjwa.cn

Ruby: -> { puts "run" }.call
来源：http://yzb.yangfankeji.com

C#:   // 无 IIFE：用静态构造函数
来源：http://cqm.smart0.xyz

[C13] 类型声明 / 类型注解
来源：http://brh.feifeiyinyue.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://kek.aizwys.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ebm.ydzc1.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://uzk.jiagoushi.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://man.sxryk.cn

Java: int add(int a, int b) { return a + b; }
来源：http://eiy.zhijiandao.cn

Go:   func add(a, b int) int
来源：http://hko.feifeiyinyue.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://jry.iojbl.cn

C#:   int Add(int a, int b) => a + b;
来源：http://dzk.ydzc1.top

[C14] 泛型函数
来源：http://jbs.hnxiangtu.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://vrr.shangyingyoupin.top

PHP:  // 无泛型
来源：http://irp.wangdashe.top

JS:   // 无泛型
来源：http://oxp.daxiang520.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://tfa.zhongyouzk.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://onf.zhongyouzk.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://bqk.ppjwa.cn

Ruby: # 无泛型
来源：http://mhp.sysykeji.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://jhc.yongpay.top

[C15] 解构 / 展开参数
来源：http://hhp.tian-w.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://epi.xuanzx.com

PHP:  [$a, $b] = $pair;
来源：http://dku.yj202588.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://vxc.ywan-chungtsiang.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://opw.9152youxi.cn

Java: // 无解构
来源：http://mcb.mhx1999.top

Go:   // 无解构
来源：http://nfg.hongshengwenyu.top

Ruby: a, b = pair
来源：http://jss.iojbl.cn

C#:   var (a, b) = pair;
来源：http://srz.sufxvd.cn

[C16] 函数 / 方法重载
来源：http://tad.c1oappe.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://jjs.ppjwa.cn

PHP:  // 无重载
来源：http://qsk.nanxuanxn.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://bqt.yfazqb.com

TS:   // 用联合类型或重载签名声明
来源：http://gri.yj20258.top

Java: void f(int a) {}  void f(String a) {}
来源：http://mad.hysaishi.cn

Go:   // 无重载：用不同函数名
来源：http://rjb.yuxming.cn

Ruby: # 无重载：靠动态参数
来源：http://xhb.zhongyouzk.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://wak.wangshuangyany.cn

================================================================================
来源：http://adr.gaohongyu789.top

D. 数组 / 列表 / 集合
来源：http://puo.guowangkeji.top

================================================================================
来源：http://iqj.epnwcf.com

[D01] 创建数组 / 列表
来源：http://zwu.hammf.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://swj.yj20258888.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://uau.gotoacloud.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ezq.yvedp.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://fre.dianchejie.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://fyw.sufxvd.cn

Go:   arr := []int{1, 2, 3}
来源：http://bkz.aibaodan.cn

Ruby: arr = [1, 2, 3]
来源：http://aui.daxiang520.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://orp.chenzaomai.com

[D02] 追加元素到末尾
来源：http://hew.dianchejie.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://dtk.yj20258.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://yio.hfpthk.cn

JS:   arr.push(4);
来源：http://vrm.feifeiyinyue.top

TS:   arr.push(4);
来源：http://nse.sweek.top

Java: list.add(4);
来源：http://bmx.bjfxy.top

Go:   arr = append(arr, 4)
来源：http://lqf.jqgfzy.top

Ruby: arr << 4; arr.push(5)
来源：http://cie.jianghu66.top

C#:   list.Add(4);
来源：http://etm.gotoacloud.top

[D03] 在指定位置插入元素
来源：http://tkk.shuidangran.top

Py:   arr.insert(0, 0)
来源：http://yya.cashguo.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://obf.xuanzx.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://vjj.havefunace.top

TS:   arr.splice(0, 0, 0);
来源：http://esl.xuanzx.com

Java: list.add(0, 0);
来源：http://iwl.yj20258888.top

Go:   arr = append([]int{0}, arr...)
来源：http://vjw.tanke756.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://txe.cdnleiting.top

C#:   list.Insert(0, 0);
来源：http://tje.fengsongda.top

[D04] 删除元素
来源：http://lak.chenjidiqi.icu

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://jau.redwolf501.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://opc.jinyuanbaomall.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://gnk.fzhhl.top

TS:   arr.splice(0, 1);
来源：http://wsk.c1oappe.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://fym.cashguo.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://veq.snrcjt.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ifk.dianchejie.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://bpo.yangfankeji.com

[D05] 访问与修改元素
来源：http://jpu.gogol.net.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://zyq.dashuyun.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://stg.yangfankeji.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://jlg.ydjk.org.cn

TS:   arr[0]; arr.at(-1);
来源：http://bsv.yuanzhike.top

Java: list.get(0); list.set(0, 9);
来源：http://duu.316326.xyz

Go:   arr[0]; arr[0] = 9
来源：http://qjy.zdbjq.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://boy.andypj.xyz

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://alw.0kj1m.cn

[D06] 数组长度
来源：http://mtl.xylfe.cn

Py:   len(arr)
来源：http://anr.sjlbkw.cn

PHP:  count($arr);
来源：http://kbr.meibo888.top

JS:   arr.length
来源：http://vzt.cdnleiting.top

TS:   arr.length
来源：http://wel.hfpthk.cn

Java: list.size();
来源：http://clp.bjfxy.top

Go:   len(arr)
来源：http://kip.xylfe.cn

Ruby: arr.length; arr.size
来源：http://zcj.jinqigfzy.top

C#:   list.Count;
来源：http://pdh.jqgfzy.top

[D07] 切片 / 取子数组
来源：http://flp.vehdjk.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://kzm.xinyue.icu

PHP:  array_slice($arr, 1, 3);
来源：http://obo.yongpay.top

JS:   arr.slice(1, 4);
来源：http://beo.guowangkeji.top

TS:   arr.slice(1, 4);
来源：http://xmq.chenlongwang.top

Java: list.subList(1, 4);
来源：http://zqt.gotoacloud.top

Go:   arr[1:4]
来源：http://gsv.sjlbkw.cn

Ruby: arr[1, 3]
来源：http://ads.haohaochexian.top

C#:   list.GetRange(1, 3);
来源：http://etu.fehbvm.com

[D08] 合并两个数组
来源：http://zos.ppjwa.cn

Py:   a + b;  a.extend(b)
来源：http://shl.kuanghao11.cn

PHP:  array_merge($a, $b);
来源：http://rjm.zhaomingkeji.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://sro.snrcjt.cn

TS:   [...a, ...b];
来源：http://xrw.yj20258888.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://shh.shzxlz.cn

Go:   append(a, b...)
来源：http://fmm.fktsv.cn

Ruby: a + b;  a.concat(b)
来源：http://ogm.zhaomingkeji.xyz

C#:   a.Concat(b).ToList()
来源：http://umh.hywenlv.cn

[D09] 排序（升序）
来源：http://vdg.xuetiantiany.cn

Py:   sorted(arr);  arr.sort()
来源：http://pnb.yangfankeji.com

PHP:  sort($arr);
来源：http://uel.yuxming.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ydi.xuanzx.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://gzu.tarul.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://rfu.c1oappe.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://dah.xylfe.cn

Ruby: arr.sort
来源：http://psx.mhx1999.top

C#:   list.Sort();
来源：http://hhl.cdnleiting.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://tcf.xinyue.icu

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://xrc.gogol.net.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://iql.bbcook.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://dnm.tianlin.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wdt.jlsjyb.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ssj.zhongyouzk.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://icv.sweek.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://jnk.wangdashe.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://zyk.aizwys.cn

[D11] 反转数组
来源：http://iuh.shanyushiyangtech.top

Py:   arr[::-1];  arr.reverse()
来源：http://jva.ydjk.org.cn

PHP:  array_reverse($arr);
来源：http://crs.cheryme.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://icn.shangyingyoupin.top

TS:   [...arr].reverse();
来源：http://iop.birdmap.top

Java: Collections.reverse(list);
来源：http://lec.tanke756.top

Go:   slices.Reverse(arr)
来源：http://wqs.zhengqikj.top

Ruby: arr.reverse
来源：http://xbc.fzhhl.top

C#:   list.Reverse();
来源：http://pal.shzxlz.cn

[D12] 查找元素下标
来源：http://raa.gotoacloud.top

Py:   arr.index(x);  x in arr
来源：http://krc.xuanzx.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://qit.cheryme.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cva.9152youxi.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sht.ivvv.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://rpe.tarul.cn

Go:   slices.Index(arr, x)
来源：http://kty.zhijiandao.cn

Ruby: arr.index(x)
来源：http://plr.fehbvm.com

C#:   list.IndexOf(x);
来源：http://jkn.fzhhl.top

[D13] 过滤（保留满足条件的）
来源：http://pdv.xylfe.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://bkq.gogol.net.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hvq.sweek.top

JS:   arr.filter(x => x > 3)
来源：http://nar.guannengcc.top

TS:   arr.filter(x => x > 3)
来源：http://ppu.guowangkeji.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://kqi.feifeiyinyue.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://khu.yj20258.top

Ruby: arr.select { |x| x > 3 }
来源：http://ldt.quarkkingdee.top

C#:   list.Where(x => x > 3).ToList()
来源：http://fyh.nanxuanxn.top

[D14] 映射转换（每个元素变形）
来源：http://kls.kuanghao11.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mqp.andypj.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://fuc.vqdsnc.cn

JS:   arr.map(x => x * 2)
来源：http://bsp.jqgufenzy.top

TS:   arr.map(x => x * 2)
来源：http://tbl.yfazqb.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://fyi.meibo888.top

Go:   // 手写循环
来源：http://eqw.52xcode.cn

Ruby: arr.map { |x| x * 2 }
来源：http://tsc.wangshuangyany.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://csz.ctjpmb.com

[D15] 去重
来源：http://bds.xinyue.icu

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://aqv.sxryk.cn

PHP:  array_unique($arr);
来源：http://ysh.dashuyun.cn

JS:   [...new Set(arr)]
来源：http://sig.tanke756.top

TS:   [...new Set(arr)]
来源：http://wjo.zhijiandao.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://qef.xinyue.icu

Go:   // 用 map[T]struct{} 手写
来源：http://xzv.wangdashe.top

Ruby: arr.uniq
来源：http://ppp.ctjpmb.com

C#:   list.Distinct().ToList()
来源：http://fvb.sxryk.cn

[D16] 求和与平均值
来源：http://oqc.wangdashe.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://oct.jinqigufen.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ote.xziqi.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ehu.pengpengdd.cyou

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wyg.gzhubu.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wly.zhiwuduotai.top

Go:   // 手写循环累加
来源：http://hmx.tian-w.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://zzg.gogol.net.cn

C#:   list.Sum();  list.Average()
来源：http://wbh.jinqigfzy.top

[D17] 最大值与最小值
来源：http://ate.jianghu66.top

Py:   max(arr);  min(arr)
来源：http://pmu.yj202588.top

PHP:  max($arr);  min($arr);
来源：http://bmi.chenzaomai.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://zia.hnxiangtu.top

TS:   Math.max(...arr);
来源：http://mia.chenlongwang.top

Java: Collections.max(list);  Collections.min(list);
来源：http://eri.sjlbkw.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://fpu.tanke756.top

Ruby: arr.max;  arr.min
来源：http://cpt.hongshengwenyu.top

C#:   list.Max();  list.Min()
来源：http://ewk.cashguo.top

[D18] 扁平化嵌套数组
来源：http://rdb.sysykeji.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://aqv.vehdjk.com

PHP:  array_merge(...$nested);
来源：http://plb.aizwys.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://vlq.316326.xyz

TS:   nested.flat();
来源：http://yfx.tianlin.xyz

Java: nested.stream().flatMap(List::stream).toList()
来源：http://kbu.ybcxt.top

Go:   // 手写双层循环
来源：http://ega.zhengqikj.top

Ruby: nested.flatten
来源：http://czx.chenlongwang.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://jhv.9152youxi.cn

[D19] 按字段分组
来源：http://kit.iojbl.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://pze.meibo888.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qmv.yj202588.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://zyl.jiagoushi.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://kot.andypj.xyz

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://auw.gaohongyu789.top

Go:   // 手写 map[string][]T
来源：http://utr.cqqwz.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ony.fanxiaobao.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://arp.shzxlz.cn

[D20] 统计每个元素出现次数
来源：http://bkr.shanyushiyangtech.top

Py:   Counter(arr)
来源：http://gbv.jinqigfzy.top

PHP:  array_count_values($arr);
来源：http://wno.ehwqpu.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://aiy.ydjk.org.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://oty.hesvh.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://kry.sysykeji.top

Go:   // 手写 map[T]int
来源：http://njm.xylfe.cn

Ruby: arr.tally
来源：http://zxs.jinqigfzy.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ral.ivvv.top

[D21] 判断是否包含某元素
来源：http://hle.sysykeji.top

Py:   x in arr
来源：http://ldc.yvedp.cn

PHP:  in_array($x, $arr, true);
来源：http://exa.yanxiufei.cn

JS:   arr.includes(x)
来源：http://dgy.sysykeji.top

TS:   arr.includes(x)
来源：http://bci.nanxuanxn.top

Java: list.contains(x)
来源：http://lay.uphjek.com

Go:   slices.Contains(arr, x)
来源：http://ssk.vehdjk.com

Ruby: arr.include?(x)
来源：http://czm.xziqi.cn

C#:   list.Contains(x)
来源：http://wax.xinyue.icu

[D22] 复制数组（避免共享引用）
来源：http://gqs.epnwcf.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://pnc.dashuyun.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ffh.jlsjyb.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hlv.fehbvm.com

TS:   [...arr];
来源：http://mdd.sweek.top

Java: new ArrayList<>(list);
来源：http://rey.yvedp.cn

Go:   copied := append([]int(nil), arr...)
来源：http://orb.ybcxt.top

Ruby: arr.dup;  arr.clone
来源：http://wyn.ctjpmb.com

C#:   new List<int>(list);
来源：http://jfb.tianlin.xyz

[D23] reduce 累积计算
来源：http://dll.wangshuangyany.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ykj.smart0.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mtv.pycfn.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rbv.andypj.xyz

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hws.zdbjq.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://hmr.yuxming.cn

Go:   // 手写循环
来源：http://ord.gzhubu.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ona.svipenyu.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://tyq.jlsjyb.cn

[D24] 字典 / Map 基本操作
来源：http://csk.fanxiaobao.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://uvs.zhixingplan.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://cdb.jinghuilouyu.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://qdb.cashguo.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://xkk.yj20258888.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://osg.fengsongda.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://gjd.hysaishi.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://pxw.yueranfly.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://yzy.xziqi.cn

[D25] Set 集合去重与交并差
来源：http://yaw.ywan-chungtsiang.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://aut.gogol.net.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://elq.hammf.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://rzg.wangdashe.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ebf.sjlbkw.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://kwg.52xcode.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ioj.haohaochexian.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://zej.yj20258.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://vuk.ydjk.org.cn

[D26] 数组转字符串
来源：http://nfe.hongshengwenyu.top

Py:   ", ".join(map(str, arr))
来源：http://klm.ydjk.org.cn

PHP:  implode(", ", $arr);
来源：http://ioc.cucudq.cn

JS:   arr.join(", ")
来源：http://hsh.bbcook.cn

TS:   arr.join(", ")
来源：http://urx.gzhubu.top

Java: String.join(", ", list)
来源：http://zmy.chenlongwang.top

Go:   strings.Join(strs, ", ")
来源：http://ujf.hongshengwenyu.top

Ruby: arr.join(", ")
来源：http://prm.shzxlz.cn

C#:   string.Join(", ", list)
来源：http://njj.jyoumei.cn

================================================================================
来源：http://vke.zhengqikj.top

E. 字符串处理
来源：http://cit.cqqwz.cn

================================================================================
来源：http://rgx.mhx1999.top

[E01] 拼接字符串
来源：http://xbz.yfazqb.com


<!-- 参考信息 -->