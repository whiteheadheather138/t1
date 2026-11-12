代发 wailian999

[C10] 变量作用域
来源：http://cfw.ywan-chungtsiang.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ceh.jinqigfzy.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ktz.shanyushiyangkeji.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://umd.ywan-chungtsiang.top

TS:   同 JS
来源：http://ccd.sjlbkw.cn

Java: 方法内为块级作用域
来源：http://cwz.52xcode.cn

Go:   花括号块级作用域
来源：http://urh.hnxiangtu.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://swh.hongshengwenyu.top

C#:   块级作用域
来源：http://mcn.wangdashe.top

[C11] 模块导入与导出
来源：http://lkn.kuanghao11.cn

Py:   from module import func
来源：http://ofb.bbcook.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://hrk.jianghu66.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://sgk.jqgufenzy.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://leo.snrcjt.cn

Java: import java.util.List;
来源：http://ddt.c1oappe.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://xzk.ppjwa.cn

Ruby: require "json"; require_relative "./util"
来源：http://ecn.meibo888.top

C#:   using System.Text;
来源：http://sui.sxryk.cn

[C12] 立即执行函数 IIFE
来源：http://awt.iojbl.cn

Py:   (lambda: print("run"))()
来源：http://wpk.nwbrower.top

PHP:  (function () { echo "run"; })();
来源：http://gcb.iojbl.cn

JS:   (() => { console.log("run"); })();
来源：http://afm.nwbrower.top

TS:   (() => { console.log("run"); })();
来源：http://aus.ydzc1.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://vzg.jianghu66.top

Go:   func() { fmt.Println("run") }()
来源：http://nwy.cqqwz.cn

Ruby: -> { puts "run" }.call
来源：http://dbd.zhengqikj.top

C#:   // 无 IIFE：用静态构造函数
来源：http://coj.tarul.cn

[C13] 类型声明 / 类型注解
来源：http://mti.ivvv.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://xvr.hcnkem.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://egd.daxiang520.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://pzc.aizwys.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zdr.yueranfly.top

Java: int add(int a, int b) { return a + b; }
来源：http://cxt.ywan-chungtsiang.top

Go:   func add(a, b int) int
来源：http://cwl.ydjk.org.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://tzb.fanxiaobao.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://vzp.daria6918.cn

[C14] 泛型函数
来源：http://zrp.zycfv.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://jbc.nwbrower.top

PHP:  // 无泛型
来源：http://iww.fehbvm.com

JS:   // 无泛型
来源：http://qbj.hnxiangtu.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://lvx.gzhubu.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://pue.hesvh.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mdi.yuanzhike.top

Ruby: # 无泛型
来源：http://kby.zdqjudy.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://nxi.cdnleiting.top

[C15] 解构 / 展开参数
来源：http://ufh.sxryk.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://atk.tian-w.cn

PHP:  [$a, $b] = $pair;
来源：http://hpw.hysaishi.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://fxc.gzhubu.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://tvf.cheryme.top

Java: // 无解构
来源：http://xvs.iojbl.cn

Go:   // 无解构
来源：http://gru.jianghu66.top

Ruby: a, b = pair
来源：http://xig.ywan-chungtsiang.top

C#:   var (a, b) = pair;
来源：http://aur.zdbjq.cn

[C16] 函数 / 方法重载
来源：http://zzx.guowangkeji.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://bkr.zycfv.cn

PHP:  // 无重载
来源：http://bud.smart0.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://iuq.zhongyouzk.top

TS:   // 用联合类型或重载签名声明
来源：http://vnk.316326.xyz

Java: void f(int a) {}  void f(String a) {}
来源：http://mia.jinyuanbaomall.cn

Go:   // 无重载：用不同函数名
来源：http://djz.zhaomingkeji.xyz

Ruby: # 无重载：靠动态参数
来源：http://sid.xinyue.icu

C#:   void F(int a) {}  void F(string a) {}
来源：http://cip.yj202588.top

================================================================================
来源：http://eok.pycfn.com

D. 数组 / 列表 / 集合
来源：http://jsm.gogol.net.cn

================================================================================
来源：http://xvf.gotoacloud.top

[D01] 创建数组 / 列表
来源：http://tmr.shanyushiyangkeji.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://dvv.zhongyouzk.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mkt.yj202588.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://tfu.chenjidiqi.icu

TS:   const arr: number[] = [1, 2, 3];
来源：http://rvn.daria6918.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://lqd.jinqigfzy.top

Go:   arr := []int{1, 2, 3}
来源：http://mqu.aibaodan.cn

Ruby: arr = [1, 2, 3]
来源：http://vxy.svipenyu.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://jyu.9152youxi.cn

[D02] 追加元素到末尾
来源：http://fzb.nanxuanxn.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://arm.quarkkingdee.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hwf.ydjk.org.cn

JS:   arr.push(4);
来源：http://jih.fktsv.cn

TS:   arr.push(4);
来源：http://eny.zdbjq.cn

Java: list.add(4);
来源：http://hlp.wangdashe.top

Go:   arr = append(arr, 4)
来源：http://okt.shanyushiyangtech.top

Ruby: arr << 4; arr.push(5)
来源：http://pnp.yonumen.top

C#:   list.Add(4);
来源：http://msx.haohaochexian.top

[D03] 在指定位置插入元素
来源：http://gke.nanxinkj.top

Py:   arr.insert(0, 0)
来源：http://rqg.nanxinkj.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://qyu.uphjek.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hom.sufxvd.cn

TS:   arr.splice(0, 0, 0);
来源：http://mxz.9152youxi.cn

Java: list.add(0, 0);
来源：http://fvu.chenzaomai.com

Go:   arr = append([]int{0}, arr...)
来源：http://ahv.zhiwuduotai.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://iyr.hesvh.cn

C#:   list.Insert(0, 0);
来源：http://xjp.yj202588.top

[D04] 删除元素
来源：http://myd.xuanzx.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://xir.nanxinkj.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mri.c1oappe.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://nhb.yj20258.top

TS:   arr.splice(0, 1);
来源：http://skf.sysykeji.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wsh.fehbvm.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ovi.tian-w.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://vvf.xziqi.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://yeh.zhengqikj.top

[D05] 访问与修改元素
来源：http://nao.quarkkingdee.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://llh.jinqigfzy.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ktq.daxiang520.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wsk.fehbvm.com

TS:   arr[0]; arr.at(-1);
来源：http://wea.cashguo.top

Java: list.get(0); list.set(0, 9);
来源：http://pzz.smart0.xyz

Go:   arr[0]; arr[0] = 9
来源：http://qfx.jiagoushi.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wth.zycfv.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://xtg.cucudq.cn

[D06] 数组长度
来源：http://bkj.cheryme.top

Py:   len(arr)
来源：http://ces.guannengcc.top

PHP:  count($arr);
来源：http://yhs.yanxiufei.cn

JS:   arr.length
来源：http://cho.aibaodan.cn

TS:   arr.length
来源：http://ony.fengsongda.top

Java: list.size();
来源：http://ilt.ehwqpu.com

Go:   len(arr)
来源：http://eyr.cqqwz.cn

Ruby: arr.length; arr.size
来源：http://fyi.gzhubu.top

C#:   list.Count;
来源：http://tcu.yongpay.top

[D07] 切片 / 取子数组
来源：http://lse.tanke756.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://izb.cucudq.cn

PHP:  array_slice($arr, 1, 3);
来源：http://gio.havefunace.top

JS:   arr.slice(1, 4);
来源：http://zqd.pycfn.com

TS:   arr.slice(1, 4);
来源：http://avq.jyoumei.cn

Java: list.subList(1, 4);
来源：http://glh.haohaochexian.top

Go:   arr[1:4]
来源：http://pek.feifeiyinyue.top

Ruby: arr[1, 3]
来源：http://qar.guannengcc.top

C#:   list.GetRange(1, 3);
来源：http://bsl.cucudq.cn

[D08] 合并两个数组
来源：http://kci.ivvv.top

Py:   a + b;  a.extend(b)
来源：http://yqd.kuanghao11.cn

PHP:  array_merge($a, $b);
来源：http://wbm.c1oappe.top

JS:   [...a, ...b];  a.concat(b);
来源：http://wvs.yvedp.cn

TS:   [...a, ...b];
来源：http://vfz.hnxiangtu.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://fnh.pycfn.com

Go:   append(a, b...)
来源：http://rmk.vehdjk.com

Ruby: a + b;  a.concat(b)
来源：http://pup.daria6918.cn

C#:   a.Concat(b).ToList()
来源：http://obr.ppjwa.cn

[D09] 排序（升序）
来源：http://cye.pengpengdd.cyou

Py:   sorted(arr);  arr.sort()
来源：http://jad.xziqi.cn

PHP:  sort($arr);
来源：http://mum.c1oappe.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://rwk.jinqigufen.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://ycy.sxryk.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://pdp.ctjpmb.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://dtk.cucudq.cn

Ruby: arr.sort
来源：http://oqj.gotoacloud.top

C#:   list.Sort();
来源：http://vip.gotoacloud.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://ois.shanyushiyangkeji.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://crd.hnqzz.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wrz.cqqwz.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://qmt.hnxiangtu.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://lve.gaohongyu789.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://efq.ydzc1.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://amk.tianlin.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://zev.xingfuxueyuan.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://llv.ydjk.org.cn

[D11] 反转数组
来源：http://tqa.xingfuxueyuan.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://nww.jinyuanbaomall.cn

PHP:  array_reverse($arr);
来源：http://ajj.xingfuxueyuan.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mrv.chenlongwang.top

TS:   [...arr].reverse();
来源：http://ybv.andypj.xyz

Java: Collections.reverse(list);
来源：http://jcs.zhaomingkeji.xyz

Go:   slices.Reverse(arr)
来源：http://ahi.jinghuilouyu.cn

Ruby: arr.reverse
来源：http://gof.hammf.cn

C#:   list.Reverse();
来源：http://yda.shzxlz.cn

[D12] 查找元素下标
来源：http://dyd.shanyushiyangtech.top

Py:   arr.index(x);  x in arr
来源：http://uom.hywenlv.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://cux.gzhubu.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lta.hammf.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://eqj.guannengcc.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://gtq.xingfuxueyuan.xyz

Go:   slices.Index(arr, x)
来源：http://hby.cqqwz.cn

Ruby: arr.index(x)
来源：http://tgw.xingfuxueyuan.xyz

C#:   list.IndexOf(x);
来源：http://bqx.ivvv.top

[D13] 过滤（保留满足条件的）
来源：http://dqt.xziqi.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qvj.gogol.net.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mok.gogol.net.cn

JS:   arr.filter(x => x > 3)
来源：http://gmz.ctjpmb.com

TS:   arr.filter(x => x > 3)
来源：http://vbg.dianchejie.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://avu.ywan-chungtsiang.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://yzb.shuidangran.top

Ruby: arr.select { |x| x > 3 }
来源：http://ngm.ehwqpu.com

C#:   list.Where(x => x > 3).ToList()
来源：http://fqh.snrcjt.cn

[D14] 映射转换（每个元素变形）
来源：http://kpf.cqqwz.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://yqr.cashguo.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hca.hnqzz.top

JS:   arr.map(x => x * 2)
来源：http://wai.ydjk.org.cn

TS:   arr.map(x => x * 2)
来源：http://sjb.sweek.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://gne.ybcxt.top

Go:   // 手写循环
来源：http://yyn.yj202588.top

Ruby: arr.map { |x| x * 2 }
来源：http://fcx.fehbvm.com

C#:   list.Select(x => x * 2).ToList()
来源：http://bll.tanke756.top

[D15] 去重
来源：http://zqb.zhongyouzk.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://dfy.zhengqikj.top

PHP:  array_unique($arr);
来源：http://gtb.fanxiaobao.xyz

JS:   [...new Set(arr)]
来源：http://xnv.sysykeji.top

TS:   [...new Set(arr)]
来源：http://vmm.kuanghao11.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ecr.zdqjudy.top

Go:   // 用 map[T]struct{} 手写
来源：http://uxz.zhoulong.xyz

Ruby: arr.uniq
来源：http://cfo.yuanzhike.top

C#:   list.Distinct().ToList()
来源：http://hxe.ybcxt.top

[D16] 求和与平均值
来源：http://hrm.zhoulong.xyz

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://omt.vehdjk.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ldq.zhixingplan.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ffw.sweek.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://kod.guowangkeji.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ebe.xziqi.cn

Go:   // 手写循环累加
来源：http://hfe.sjlbkw.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://jdz.zdbjq.cn

C#:   list.Sum();  list.Average()
来源：http://clm.sysykeji.top

[D17] 最大值与最小值
来源：http://acg.jqgfzy.top

Py:   max(arr);  min(arr)
来源：http://tlv.shzxlz.cn

PHP:  max($arr);  min($arr);
来源：http://wjf.yangfankeji.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://diu.sufxvd.cn

TS:   Math.max(...arr);
来源：http://gdk.sufxvd.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://czq.andypj.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://gkx.ydzc1.top

Ruby: arr.max;  arr.min
来源：http://zvx.hongshengwenyu.top

C#:   list.Max();  list.Min()
来源：http://xga.guannengcc.top

[D18] 扁平化嵌套数组
来源：http://vvo.hnqzz.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://bvs.fehbvm.com

PHP:  array_merge(...$nested);
来源：http://ovn.dianchejie.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://evw.sweek.top

TS:   nested.flat();
来源：http://spp.yuanzhike.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://daf.zhongyouzk.top

Go:   // 手写双层循环
来源：http://rou.wangdashe.top

Ruby: nested.flatten
来源：http://lgt.aibaodan.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ess.fanxiaobao.xyz

[D19] 按字段分组
来源：http://ral.nanxuanxn.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://sqj.yvedp.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://pnp.svipenyu.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://xei.dianchejie.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://rfv.sxryk.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ibs.fktsv.cn

Go:   // 手写 map[string][]T
来源：http://mjo.yj202588.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://tcd.yvedp.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://igm.xingfuxueyuan.xyz

[D20] 统计每个元素出现次数
来源：http://qyq.jlsjyb.cn

Py:   Counter(arr)
来源：http://osg.cheryme.top

PHP:  array_count_values($arr);
来源：http://sbd.tian-w.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://aym.hnqzz.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yno.yueranfly.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://xwh.iojbl.cn

Go:   // 手写 map[T]int
来源：http://het.zdqjudy.top

Ruby: arr.tally
来源：http://mvt.shanyushiyangkeji.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://bbe.ivvv.top

[D21] 判断是否包含某元素
来源：http://grn.cqqwz.cn

Py:   x in arr
来源：http://fet.jyoumei.cn

PHP:  in_array($x, $arr, true);
来源：http://dur.ybcxt.top

JS:   arr.includes(x)
来源：http://yku.jqgfzy.top

TS:   arr.includes(x)
来源：http://koi.hesvh.cn

Java: list.contains(x)
来源：http://cit.meibo888.top

Go:   slices.Contains(arr, x)
来源：http://bdg.shangyingyoupin.top

Ruby: arr.include?(x)
来源：http://bfi.sysykeji.top

C#:   list.Contains(x)
来源：http://axd.vqdsnc.cn

[D22] 复制数组（避免共享引用）
来源：http://lzi.redwolf501.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ylb.epnwcf.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://dhb.zhijiandao.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://aat.gotoacloud.top

TS:   [...arr];
来源：http://jwx.fzhhl.top

Java: new ArrayList<>(list);
来源：http://eod.vehdjk.com

Go:   copied := append([]int(nil), arr...)
来源：http://ndd.aizwys.cn

Ruby: arr.dup;  arr.clone
来源：http://wlk.tian-w.cn

C#:   new List<int>(list);
来源：http://qjy.xuanzx.com

[D23] reduce 累积计算
来源：http://ade.xuanzx.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zgw.zycfv.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://xfz.jianghu66.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kju.jiagoushi.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rej.tanke756.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://iny.uphjek.com

Go:   // 手写循环
来源：http://ajv.quarkkingdee.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://cns.jyoumei.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://pvz.zhongyouzk.top

[D24] 字典 / Map 基本操作
来源：http://mvv.yuxming.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://gkl.yangfankeji.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://dfn.chenzaomai.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://rys.cashguo.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://yop.jinghuilouyu.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mcq.vehdjk.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://lwk.feifeiyinyue.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://cep.hesvh.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mgt.bbcook.cn

[D25] Set 集合去重与交并差
来源：http://une.daxiang520.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wjh.haohaochexian.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://qnn.chenzaomai.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://rli.chenzaomai.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://oqm.guowangkeji.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://kfq.yanxiufei.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://bib.gogol.net.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://kyw.vqdsnc.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://yek.cheryme.top

[D26] 数组转字符串
来源：http://mkk.shangyingyoupin.top

Py:   ", ".join(map(str, arr))
来源：http://dtr.cucudq.cn

PHP:  implode(", ", $arr);
来源：http://kjx.xylfe.cn

JS:   arr.join(", ")
来源：http://kmm.shanyushiyangkeji.top

TS:   arr.join(", ")
来源：http://xbr.ivvv.top

Java: String.join(", ", list)
来源：http://kmm.nanxinkj.top

Go:   strings.Join(strs, ", ")
来源：http://ojr.xingfuxueyuan.xyz

Ruby: arr.join(", ")
来源：http://qhs.xziqi.cn

C#:   string.Join(", ", list)
来源：http://dyo.yangfankeji.com


<!-- 参考信息 -->