代发 wailian999

TS:   同 JS
来源：http://eex.zhoulong.xyz

Java: 方法内为块级作用域
来源：http://xdj.cashguo.top

Go:   花括号块级作用域
来源：http://utc.xinyue.icu

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://yuy.yongpay.top

C#:   块级作用域
来源：http://xpc.dashuyun.cn

[C11] 模块导入与导出
来源：http://imu.tarul.cn

Py:   from module import func
来源：http://sac.dashuyun.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://gqr.ehwqpu.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://oah.havefunace.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://zat.bbcook.cn

Java: import java.util.List;
来源：http://rxt.hammf.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://vch.tarul.cn

Ruby: require "json"; require_relative "./util"
来源：http://pml.xingfuxueyuan.xyz

C#:   using System.Text;
来源：http://gzk.tanke756.top

[C12] 立即执行函数 IIFE
来源：http://wrr.zhixingplan.top

Py:   (lambda: print("run"))()
来源：http://mir.sufxvd.cn

PHP:  (function () { echo "run"; })();
来源：http://taw.yvedp.cn

JS:   (() => { console.log("run"); })();
来源：http://vez.daria6918.cn

TS:   (() => { console.log("run"); })();
来源：http://vfg.yuanzhike.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jin.cdnleiting.top

Go:   func() { fmt.Println("run") }()
来源：http://psp.sysykeji.top

Ruby: -> { puts "run" }.call
来源：http://jtb.yj20258888.top

C#:   // 无 IIFE：用静态构造函数
来源：http://itg.feifeiyinyue.top

[C13] 类型声明 / 类型注解
来源：http://buz.ybcxt.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://eyo.vehdjk.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rri.fanxiaobao.xyz

JS:   // 无类型（可用 JSDoc 注释）
来源：http://dmb.quarkkingdee.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yqa.fzhhl.top

Java: int add(int a, int b) { return a + b; }
来源：http://xls.jlsjyb.cn

Go:   func add(a, b int) int
来源：http://cwu.sysykeji.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://dsc.sweek.top

C#:   int Add(int a, int b) => a + b;
来源：http://dte.jianghu66.top

[C14] 泛型函数
来源：http://brw.jianghu66.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://oqi.sxryk.cn

PHP:  // 无泛型
来源：http://ecf.yj20258888.top

JS:   // 无泛型
来源：http://jra.ehwqpu.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://yba.smart0.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://nfh.jqgufenzy.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://htx.pycfn.com

Ruby: # 无泛型
来源：http://njx.chenlongwang.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ppt.nwbrower.top

[C15] 解构 / 展开参数
来源：http://kmt.zhoulong.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://lsn.gaohongyu789.top

PHP:  [$a, $b] = $pair;
来源：http://yyl.chenjidiqi.icu

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://vmb.jiagoushi.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hsq.shanyushiyangtech.top

Java: // 无解构
来源：http://lbc.meibo888.top

Go:   // 无解构
来源：http://mpt.zdqjudy.top

Ruby: a, b = pair
来源：http://jqp.bjfxy.top

C#:   var (a, b) = pair;
来源：http://mhh.0kj1m.cn

[C16] 函数 / 方法重载
来源：http://ogf.daxiang520.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vlc.shuidangran.top

PHP:  // 无重载
来源：http://naj.smart0.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://amk.xinyue.icu

TS:   // 用联合类型或重载签名声明
来源：http://dbt.yonumen.top

Java: void f(int a) {}  void f(String a) {}
来源：http://yoq.yvedp.cn

Go:   // 无重载：用不同函数名
来源：http://pci.cucudq.cn

Ruby: # 无重载：靠动态参数
来源：http://uzi.redwolf501.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://mwr.xylfe.cn

================================================================================
来源：http://mob.jinqigufen.top

D. 数组 / 列表 / 集合
来源：http://vhl.pycfn.com

================================================================================
来源：http://hbc.jinghuilouyu.cn

[D01] 创建数组 / 列表
来源：http://qvj.daria6918.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://pgh.ywan-chungtsiang.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://lhm.hnxiangtu.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://dvk.guowangkeji.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://zak.wangdashe.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://vxb.vqdsnc.cn

Go:   arr := []int{1, 2, 3}
来源：http://rla.zdqjudy.top

Ruby: arr = [1, 2, 3]
来源：http://cgn.xuanzx.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ybp.jinqigufen.top

[D02] 追加元素到末尾
来源：http://awu.hesvh.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://fbt.pengpengdd.cyou

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://iwr.yueranfly.top

JS:   arr.push(4);
来源：http://ffv.wangshuangyany.cn

TS:   arr.push(4);
来源：http://duf.jinqigfzy.top

Java: list.add(4);
来源：http://jqi.gzhubu.top

Go:   arr = append(arr, 4)
来源：http://hpz.jyoumei.cn

Ruby: arr << 4; arr.push(5)
来源：http://hmm.yueranfly.top

C#:   list.Add(4);
来源：http://lzu.cashguo.top

[D03] 在指定位置插入元素
来源：http://vwh.yj20258.top

Py:   arr.insert(0, 0)
来源：http://zps.tanke756.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://lbk.zycfv.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://qgs.vqdsnc.cn

TS:   arr.splice(0, 0, 0);
来源：http://gjk.yongpay.top

Java: list.add(0, 0);
来源：http://shp.mhx1999.top

Go:   arr = append([]int{0}, arr...)
来源：http://wpu.svipenyu.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://rma.nanxuanxn.top

C#:   list.Insert(0, 0);
来源：http://swg.havefunace.top

[D04] 删除元素
来源：http://fmd.hfpthk.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://qdt.zdbjq.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mkt.hfpthk.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mxk.chenjidiqi.icu

TS:   arr.splice(0, 1);
来源：http://fqd.zdqjudy.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://weq.zhiwuduotai.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ubu.jinyuanbaomall.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://scv.tarul.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://btc.birdmap.top

[D05] 访问与修改元素
来源：http://hdi.yuxming.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://efs.yj20258888.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://vrd.aibaodan.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://pai.kuanghao11.cn

TS:   arr[0]; arr.at(-1);
来源：http://par.yj20258.top

Java: list.get(0); list.set(0, 9);
来源：http://luf.9152youxi.cn

Go:   arr[0]; arr[0] = 9
来源：http://hxy.zhijiandao.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ewh.zhoulong.xyz

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zje.kuanghao11.cn

[D06] 数组长度
来源：http://afc.dianchejie.cn

Py:   len(arr)
来源：http://ide.jqgfzy.top

PHP:  count($arr);
来源：http://rhd.aizwys.cn

JS:   arr.length
来源：http://jgt.9152youxi.cn

TS:   arr.length
来源：http://odk.guowangkeji.top

Java: list.size();
来源：http://zac.daria6918.cn

Go:   len(arr)
来源：http://opx.cheryme.top

Ruby: arr.length; arr.size
来源：http://cyt.kuanghao11.cn

C#:   list.Count;
来源：http://tqd.hfpthk.cn

[D07] 切片 / 取子数组
来源：http://ibl.ydzc1.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://bfk.ehwqpu.com

PHP:  array_slice($arr, 1, 3);
来源：http://hbz.kuanghao11.cn

JS:   arr.slice(1, 4);
来源：http://cqi.c1oappe.top

TS:   arr.slice(1, 4);
来源：http://qah.jinqigufen.top

Java: list.subList(1, 4);
来源：http://dki.vqdsnc.cn

Go:   arr[1:4]
来源：http://vxa.daria6918.cn

Ruby: arr[1, 3]
来源：http://ggw.c1oappe.top

C#:   list.GetRange(1, 3);
来源：http://dpb.meibo888.top

[D08] 合并两个数组
来源：http://fwl.hongshengwenyu.top

Py:   a + b;  a.extend(b)
来源：http://tpz.fzhhl.top

PHP:  array_merge($a, $b);
来源：http://xcj.hnxiangtu.top

JS:   [...a, ...b];  a.concat(b);
来源：http://wxa.haohaochexian.top

TS:   [...a, ...b];
来源：http://wcs.shanyushiyangtech.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://tba.bjfxy.top

Go:   append(a, b...)
来源：http://sef.sjlbkw.cn

Ruby: a + b;  a.concat(b)
来源：http://xbp.ehwqpu.com

C#:   a.Concat(b).ToList()
来源：http://rhw.yj202588.top

[D09] 排序（升序）
来源：http://tld.yuxming.cn

Py:   sorted(arr);  arr.sort()
来源：http://rcd.pengpengdd.cyou

PHP:  sort($arr);
来源：http://rjt.9152youxi.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://xhg.redwolf501.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://itz.yongpay.top

Java: Collections.sort(list);  list.sort(null);
来源：http://buy.sysykeji.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://fmq.fanxiaobao.xyz

Ruby: arr.sort
来源：http://rhv.chenjidiqi.icu

C#:   list.Sort();
来源：http://rjl.jqgufenzy.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://ett.52xcode.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wxy.zhongyouzk.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yjo.zhiwuduotai.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://lfi.snrcjt.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://brv.wangdashe.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hoq.zdbjq.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://vnn.xingfuxueyuan.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://edd.yj20258.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qqs.xziqi.cn

[D11] 反转数组
来源：http://mrq.guannengcc.top

Py:   arr[::-1];  arr.reverse()
来源：http://sbb.hongshengwenyu.top

PHP:  array_reverse($arr);
来源：http://gpf.fehbvm.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wkc.shuidangran.top

TS:   [...arr].reverse();
来源：http://idh.yongpay.top

Java: Collections.reverse(list);
来源：http://mmd.iojbl.cn

Go:   slices.Reverse(arr)
来源：http://tip.uphjek.com

Ruby: arr.reverse
来源：http://xph.daxiang520.top

C#:   list.Reverse();
来源：http://jkn.wangdashe.top

[D12] 查找元素下标
来源：http://fnc.hongshengwenyu.top

Py:   arr.index(x);  x in arr
来源：http://mvb.haohaochexian.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://bdn.snrcjt.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yrw.yonumen.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fke.haohaochexian.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ewr.zhengqikj.top

Go:   slices.Index(arr, x)
来源：http://mzf.zhijiandao.cn

Ruby: arr.index(x)
来源：http://yzh.dianchejie.cn

C#:   list.IndexOf(x);
来源：http://gng.pengpengdd.cyou

[D13] 过滤（保留满足条件的）
来源：http://ilj.jinqigfzy.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://jfy.ywan-chungtsiang.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://nmh.sjlbkw.cn

JS:   arr.filter(x => x > 3)
来源：http://sjs.uphjek.com

TS:   arr.filter(x => x > 3)
来源：http://wuw.nanxinkj.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://goa.gzhubu.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ulc.jqgfzy.top

Ruby: arr.select { |x| x > 3 }
来源：http://xau.meibo888.top

C#:   list.Where(x => x > 3).ToList()
来源：http://jez.zhaomingkeji.xyz

[D14] 映射转换（每个元素变形）
来源：http://okk.smart0.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://lbr.ybcxt.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wwc.sweek.top

JS:   arr.map(x => x * 2)
来源：http://bly.gogol.net.cn

TS:   arr.map(x => x * 2)
来源：http://nrs.hywenlv.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://zwy.zdbjq.cn

Go:   // 手写循环
来源：http://psy.wangdashe.top

Ruby: arr.map { |x| x * 2 }
来源：http://ewq.feifeiyinyue.top

C#:   list.Select(x => x * 2).ToList()
来源：http://maw.zycfv.cn

[D15] 去重
来源：http://cbq.zycfv.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wet.zhengqikj.top

PHP:  array_unique($arr);
来源：http://ewk.hammf.cn

JS:   [...new Set(arr)]
来源：http://bob.yfazqb.com

TS:   [...new Set(arr)]
来源：http://rxd.redwolf501.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://pxm.hongshengwenyu.top

Go:   // 用 map[T]struct{} 手写
来源：http://twc.uphjek.com

Ruby: arr.uniq
来源：http://jcm.hesvh.cn

C#:   list.Distinct().ToList()
来源：http://jxt.ehwqpu.com

[D16] 求和与平均值
来源：http://idx.gogol.net.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ceq.shzxlz.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://gnd.ppjwa.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://tli.jinyuanbaomall.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://aha.fanxiaobao.xyz

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://abg.tarul.cn

Go:   // 手写循环累加
来源：http://osr.hnqzz.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://rkq.wangshuangyany.cn

C#:   list.Sum();  list.Average()
来源：http://qhx.jqgfzy.top

[D17] 最大值与最小值
来源：http://mxw.chenjidiqi.icu

Py:   max(arr);  min(arr)
来源：http://piq.yj20258888.top

PHP:  max($arr);  min($arr);
来源：http://ecc.zhaomingkeji.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://cvd.ywan-chungtsiang.top

TS:   Math.max(...arr);
来源：http://urm.yj20258888.top

Java: Collections.max(list);  Collections.min(list);
来源：http://emq.uphjek.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://xnu.xuanzx.com

Ruby: arr.max;  arr.min
来源：http://ntv.jinyuanbaomall.cn

C#:   list.Max();  list.Min()
来源：http://rud.nanxinkj.top

[D18] 扁平化嵌套数组
来源：http://dxg.ppjwa.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://yte.zhengqikj.top

PHP:  array_merge(...$nested);
来源：http://pxb.nwbrower.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://kjw.cheryme.top

TS:   nested.flat();
来源：http://nvy.gaohongyu789.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://eec.0kj1m.cn

Go:   // 手写双层循环
来源：http://spt.zhengqikj.top

Ruby: nested.flatten
来源：http://zrw.shangyingyoupin.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://jbw.yuxming.cn

[D19] 按字段分组
来源：http://zrs.hcnkem.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://skt.haohaochexian.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qnf.feifeiyinyue.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://vop.uphjek.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://lvo.guowangkeji.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://kus.ehwqpu.com

Go:   // 手写 map[string][]T
来源：http://dcl.nanxinkj.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://zgg.yj20258888.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hqp.kuanghao11.cn

[D20] 统计每个元素出现次数
来源：http://rnj.cdnleiting.top

Py:   Counter(arr)
来源：http://irk.sweek.top

PHP:  array_count_values($arr);
来源：http://hkj.zhiwuduotai.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://azk.shangyingyoupin.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nlv.yvedp.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://nox.tian-w.cn

Go:   // 手写 map[T]int
来源：http://wnw.yj202588.top

Ruby: arr.tally
来源：http://jqd.redwolf501.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://pgb.fehbvm.com

[D21] 判断是否包含某元素
来源：http://lwx.cheryme.top

Py:   x in arr
来源：http://pmc.zycfv.cn

PHP:  in_array($x, $arr, true);
来源：http://cro.shuidangran.top

JS:   arr.includes(x)
来源：http://ejb.jqgufenzy.top

TS:   arr.includes(x)
来源：http://ltn.xingfuxueyuan.xyz

Java: list.contains(x)
来源：http://akj.feifeiyinyue.top

Go:   slices.Contains(arr, x)
来源：http://dds.hywenlv.cn

Ruby: arr.include?(x)
来源：http://yef.dashuyun.cn

C#:   list.Contains(x)
来源：http://oui.zhiwuduotai.top

[D22] 复制数组（避免共享引用）
来源：http://ail.yj20258888.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://uhb.zhongyouzk.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wzw.zhijiandao.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://afs.daria6918.cn

TS:   [...arr];
来源：http://hap.zhixingplan.top

Java: new ArrayList<>(list);
来源：http://wug.yueranfly.top

Go:   copied := append([]int(nil), arr...)
来源：http://lvo.zdbjq.cn

Ruby: arr.dup;  arr.clone
来源：http://any.hongshengwenyu.top

C#:   new List<int>(list);
来源：http://fay.cdnleiting.top

[D23] reduce 累积计算
来源：http://ysk.tanke756.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://jmp.zhaomingkeji.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://skl.iojbl.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://oag.chenzaomai.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://iue.yvedp.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://zzn.xuetiantiany.cn

Go:   // 手写循环
来源：http://waw.guowangkeji.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://vnu.guowangkeji.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://cup.smart0.xyz

[D24] 字典 / Map 基本操作
来源：http://wmu.jinghuilouyu.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mko.zhongyouzk.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://dan.gogol.net.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://djs.ctjpmb.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://tkk.shuidangran.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ihx.tarul.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://nxk.ybcxt.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://uzi.hnqzz.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qdx.ctjpmb.com

[D25] Set 集合去重与交并差
来源：http://bfa.sysykeji.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wik.sysykeji.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://xjw.yvedp.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://xtm.fanxiaobao.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://dae.hongshengwenyu.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://oaz.xziqi.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://swo.nanxuanxn.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mdf.cheryme.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://idz.andypj.xyz

[D26] 数组转字符串
来源：http://qpl.hysaishi.cn

Py:   ", ".join(map(str, arr))
来源：http://htp.pengpengdd.cyou

PHP:  implode(", ", $arr);
来源：http://krf.yj202588.top

JS:   arr.join(", ")
来源：http://jqz.fehbvm.com

TS:   arr.join(", ")
来源：http://wnz.aizwys.cn

Java: String.join(", ", list)
来源：http://gdy.feifeiyinyue.top

Go:   strings.Join(strs, ", ")
来源：http://dgp.hcnkem.com

Ruby: arr.join(", ")
来源：http://pnc.sweek.top

C#:   string.Join(", ", list)
来源：http://uec.nanxinkj.top

================================================================================
来源：http://sdq.quarkkingdee.top

E. 字符串处理
来源：http://zku.yj202588.top

================================================================================
来源：http://mve.gaohongyu789.top

[E01] 拼接字符串
来源：http://jyf.tian-w.cn


<!-- 参考信息 -->