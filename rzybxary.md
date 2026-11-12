代发 wailian999

[C10] 变量作用域
来源：http://afm.zhixingplan.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://lyv.ydzc1.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://oom.daxiang520.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://pml.svipenyu.cn

TS:   同 JS
来源：http://ofn.yvedp.cn

Java: 方法内为块级作用域
来源：http://fgm.nanxinkj.top

Go:   花括号块级作用域
来源：http://ruc.ehwqpu.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ovx.quarkkingdee.top

C#:   块级作用域
来源：http://sac.nwbrower.top

[C11] 模块导入与导出
来源：http://ood.sysykeji.top

Py:   from module import func
来源：http://rpb.yonumen.top

PHP:  require "file.php";  或 use App\Service;
来源：http://nim.hammf.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://wpn.andypj.xyz

TS:   export function f(): void {};  import { f } from "./m";
来源：http://oix.jianghu66.top

Java: import java.util.List;
来源：http://ezv.wangdashe.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://zya.svipenyu.cn

Ruby: require "json"; require_relative "./util"
来源：http://qtd.xuetiantiany.cn

C#:   using System.Text;
来源：http://ans.sysykeji.top

[C12] 立即执行函数 IIFE
来源：http://vmv.jinqigfzy.top

Py:   (lambda: print("run"))()
来源：http://ryq.xingfuxueyuan.xyz

PHP:  (function () { echo "run"; })();
来源：http://ngu.hywenlv.cn

JS:   (() => { console.log("run"); })();
来源：http://vwy.yuxming.cn

TS:   (() => { console.log("run"); })();
来源：http://sgi.yuxming.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hon.fengsongda.top

Go:   func() { fmt.Println("run") }()
来源：http://wqg.fengsongda.top

Ruby: -> { puts "run" }.call
来源：http://uga.vehdjk.com

C#:   // 无 IIFE：用静态构造函数
来源：http://nxh.cucudq.cn

[C13] 类型声明 / 类型注解
来源：http://wvi.havefunace.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://udv.nwbrower.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sad.0kj1m.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://dcw.9152youxi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tjk.shzxlz.cn

Java: int add(int a, int b) { return a + b; }
来源：http://unz.yanxiufei.cn

Go:   func add(a, b int) int
来源：http://gai.9152youxi.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://pib.bjfxy.top

C#:   int Add(int a, int b) => a + b;
来源：http://jjd.aibaodan.cn

[C14] 泛型函数
来源：http://bds.jinghuilouyu.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://jeo.hnxiangtu.top

PHP:  // 无泛型
来源：http://ebd.quarkkingdee.top

JS:   // 无泛型
来源：http://omx.xziqi.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://guv.shzxlz.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://xcv.hcnkem.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://iiw.jyoumei.cn

Ruby: # 无泛型
来源：http://wkr.0kj1m.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://cbp.kuanghao11.cn

[C15] 解构 / 展开参数
来源：http://gkt.jinghuilouyu.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://yxg.fktsv.cn

PHP:  [$a, $b] = $pair;
来源：http://rrj.daxiang520.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://jxy.zhongyouzk.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://xtj.ivvv.top

Java: // 无解构
来源：http://fjq.yj202588.top

Go:   // 无解构
来源：http://plr.quarkkingdee.top

Ruby: a, b = pair
来源：http://luy.havefunace.top

C#:   var (a, b) = pair;
来源：http://mpg.hammf.cn

[C16] 函数 / 方法重载
来源：http://tdy.yvedp.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://nho.fzhhl.top

PHP:  // 无重载
来源：http://nxl.zycfv.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://rzz.fzhhl.top

TS:   // 用联合类型或重载签名声明
来源：http://gzh.feifeiyinyue.top

Java: void f(int a) {}  void f(String a) {}
来源：http://sux.ctjpmb.com

Go:   // 无重载：用不同函数名
来源：http://cew.snrcjt.cn

Ruby: # 无重载：靠动态参数
来源：http://pst.chenjidiqi.icu

C#:   void F(int a) {}  void F(string a) {}
来源：http://fif.nanxinkj.top

================================================================================
来源：http://ftj.ppjwa.cn

D. 数组 / 列表 / 集合
来源：http://lpc.xylfe.cn

================================================================================
来源：http://ipw.birdmap.top

[D01] 创建数组 / 列表
来源：http://jut.xingfuxueyuan.xyz

Py:   arr = [1, 2, 3];  empty = []
来源：http://tmx.birdmap.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://cco.andypj.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://pxi.hysaishi.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://thf.dianchejie.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://uce.hysaishi.cn

Go:   arr := []int{1, 2, 3}
来源：http://wmo.chenlongwang.top

Ruby: arr = [1, 2, 3]
来源：http://lhw.gaohongyu789.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://xde.hysaishi.cn

[D02] 追加元素到末尾
来源：http://yri.chenzaomai.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ncm.shanyushiyangkeji.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://smr.9152youxi.cn

JS:   arr.push(4);
来源：http://uae.gzhubu.top

TS:   arr.push(4);
来源：http://nje.jianghu66.top

Java: list.add(4);
来源：http://aot.yuxming.cn

Go:   arr = append(arr, 4)
来源：http://bag.yuxming.cn

Ruby: arr << 4; arr.push(5)
来源：http://ale.cucudq.cn

C#:   list.Add(4);
来源：http://uiq.guannengcc.top

[D03] 在指定位置插入元素
来源：http://hdy.hnqzz.top

Py:   arr.insert(0, 0)
来源：http://vna.epnwcf.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://qbt.zhengqikj.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://afq.tarul.cn

TS:   arr.splice(0, 0, 0);
来源：http://tvv.cqqwz.cn

Java: list.add(0, 0);
来源：http://xba.yj20258888.top

Go:   arr = append([]int{0}, arr...)
来源：http://pbi.yuxming.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://nve.pengpengdd.cyou

C#:   list.Insert(0, 0);
来源：http://ibl.jinqigufen.top

[D04] 删除元素
来源：http://xwf.zhengqikj.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hvf.cheryme.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://osu.aibaodan.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://uxy.jqgfzy.top

TS:   arr.splice(0, 1);
来源：http://ave.hongshengwenyu.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wjo.redwolf501.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wds.jinqigfzy.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://kak.snrcjt.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://con.ctjpmb.com

[D05] 访问与修改元素
来源：http://ucn.xinyue.icu

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://brp.jinyuanbaomall.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mft.quarkkingdee.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://vor.haohaochexian.top

TS:   arr[0]; arr.at(-1);
来源：http://wkv.c1oappe.top

Java: list.get(0); list.set(0, 9);
来源：http://yqb.52xcode.cn

Go:   arr[0]; arr[0] = 9
来源：http://qkw.chenzaomai.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ifs.ybcxt.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://oom.ivvv.top

[D06] 数组长度
来源：http://ajx.hcnkem.com

Py:   len(arr)
来源：http://ijh.chenlongwang.top

PHP:  count($arr);
来源：http://vmv.52xcode.cn

JS:   arr.length
来源：http://bav.hywenlv.cn

TS:   arr.length
来源：http://kyi.hnqzz.top

Java: list.size();
来源：http://dxc.chenjidiqi.icu

Go:   len(arr)
来源：http://cjh.wangshuangyany.cn

Ruby: arr.length; arr.size
来源：http://dmg.pengpengdd.cyou

C#:   list.Count;
来源：http://snl.hnxiangtu.top

[D07] 切片 / 取子数组
来源：http://qfz.yongpay.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://htm.meibo888.top

PHP:  array_slice($arr, 1, 3);
来源：http://otf.redwolf501.top

JS:   arr.slice(1, 4);
来源：http://ixh.cheryme.top

TS:   arr.slice(1, 4);
来源：http://hgx.shzxlz.cn

Java: list.subList(1, 4);
来源：http://naq.yuanzhike.top

Go:   arr[1:4]
来源：http://ykh.hysaishi.cn

Ruby: arr[1, 3]
来源：http://lyh.ctjpmb.com

C#:   list.GetRange(1, 3);
来源：http://lsq.cdnleiting.top

[D08] 合并两个数组
来源：http://bpt.zdbjq.cn

Py:   a + b;  a.extend(b)
来源：http://ulq.feifeiyinyue.top

PHP:  array_merge($a, $b);
来源：http://vec.daxiang520.top

JS:   [...a, ...b];  a.concat(b);
来源：http://jpn.yvedp.cn

TS:   [...a, ...b];
来源：http://zfw.jyoumei.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hfz.jinghuilouyu.cn

Go:   append(a, b...)
来源：http://mbh.daxiang520.top

Ruby: a + b;  a.concat(b)
来源：http://zdd.ybcxt.top

C#:   a.Concat(b).ToList()
来源：http://zsq.nanxinkj.top

[D09] 排序（升序）
来源：http://ebc.fehbvm.com

Py:   sorted(arr);  arr.sort()
来源：http://ysm.hongshengwenyu.top

PHP:  sort($arr);
来源：http://wmo.zdbjq.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://oyt.gogol.net.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ayx.jinyuanbaomall.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://gtl.pengpengdd.cyou

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://yoh.nwbrower.top

Ruby: arr.sort
来源：http://boa.hysaishi.cn

C#:   list.Sort();
来源：http://fwj.hammf.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ykk.ehwqpu.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://age.fktsv.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ijh.xuanzx.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://gsv.chenjidiqi.icu

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://rue.pycfn.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://rkc.sxryk.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://kun.birdmap.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mdp.jqgufenzy.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://sue.sysykeji.top

[D11] 反转数组
来源：http://ccg.nwbrower.top

Py:   arr[::-1];  arr.reverse()
来源：http://ghq.snrcjt.cn

PHP:  array_reverse($arr);
来源：http://npn.nanxuanxn.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://eat.jinyuanbaomall.cn

TS:   [...arr].reverse();
来源：http://kun.sweek.top

Java: Collections.reverse(list);
来源：http://oka.kuanghao11.cn

Go:   slices.Reverse(arr)
来源：http://kuh.snrcjt.cn

Ruby: arr.reverse
来源：http://xgs.nwbrower.top

C#:   list.Reverse();
来源：http://xdh.yuanzhike.top

[D12] 查找元素下标
来源：http://rwa.ppjwa.cn

Py:   arr.index(x);  x in arr
来源：http://wev.yj20258888.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://uil.redwolf501.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vnv.yonumen.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fbn.redwolf501.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://qgx.wangdashe.top

Go:   slices.Index(arr, x)
来源：http://dtn.xuetiantiany.cn

Ruby: arr.index(x)
来源：http://gwc.guannengcc.top

C#:   list.IndexOf(x);
来源：http://wcn.tianlin.xyz

[D13] 过滤（保留满足条件的）
来源：http://olt.ywan-chungtsiang.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://rkr.yanxiufei.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hhx.jinqigfzy.top

JS:   arr.filter(x => x > 3)
来源：http://qqk.yuanzhike.top

TS:   arr.filter(x => x > 3)
来源：http://csv.nanxinkj.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://naj.yvedp.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://rwc.aibaodan.cn

Ruby: arr.select { |x| x > 3 }
来源：http://oga.redwolf501.top

C#:   list.Where(x => x > 3).ToList()
来源：http://ykr.ydjk.org.cn

[D14] 映射转换（每个元素变形）
来源：http://gxu.chenzaomai.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://nsn.hysaishi.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vco.hnxiangtu.top

JS:   arr.map(x => x * 2)
来源：http://oan.redwolf501.top

TS:   arr.map(x => x * 2)
来源：http://bhj.yuanzhike.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://cen.zhiwuduotai.top

Go:   // 手写循环
来源：http://jse.shzxlz.cn

Ruby: arr.map { |x| x * 2 }
来源：http://fla.yuanzhike.top

C#:   list.Select(x => x * 2).ToList()
来源：http://pdi.shanyushiyangtech.top

[D15] 去重
来源：http://xgm.andypj.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://vmw.jyoumei.cn

PHP:  array_unique($arr);
来源：http://tqa.zdqjudy.top

JS:   [...new Set(arr)]
来源：http://fgj.cucudq.cn

TS:   [...new Set(arr)]
来源：http://hyv.fanxiaobao.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://psg.svipenyu.cn

Go:   // 用 map[T]struct{} 手写
来源：http://iua.yj202588.top

Ruby: arr.uniq
来源：http://qsu.xuetiantiany.cn

C#:   list.Distinct().ToList()
来源：http://wvd.hnqzz.top

[D16] 求和与平均值
来源：http://dps.xuetiantiany.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://eqo.smart0.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://gyr.pycfn.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://boh.yj20258888.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://djb.fehbvm.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://gzr.yj20258888.top

Go:   // 手写循环累加
来源：http://cws.hammf.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ttk.zdbjq.cn

C#:   list.Sum();  list.Average()
来源：http://zho.sxryk.cn

[D17] 最大值与最小值
来源：http://wvy.ivvv.top

Py:   max(arr);  min(arr)
来源：http://fmp.ybcxt.top

PHP:  max($arr);  min($arr);
来源：http://ypi.jinqigfzy.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://vms.xingfuxueyuan.xyz

TS:   Math.max(...arr);
来源：http://wug.sufxvd.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://gbn.aizwys.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://gwl.shanyushiyangtech.top

Ruby: arr.max;  arr.min
来源：http://ejn.nwbrower.top

C#:   list.Max();  list.Min()
来源：http://czp.aibaodan.cn

[D18] 扁平化嵌套数组
来源：http://per.cashguo.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ruu.meibo888.top

PHP:  array_merge(...$nested);
来源：http://ysd.cashguo.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://oex.wangshuangyany.cn

TS:   nested.flat();
来源：http://xmz.yanxiufei.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://tar.hfpthk.cn

Go:   // 手写双层循环
来源：http://wrb.ppjwa.cn

Ruby: nested.flatten
来源：http://uza.sweek.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://qxe.ydzc1.top

[D19] 按字段分组
来源：http://omr.gotoacloud.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://sfo.epnwcf.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qly.sxryk.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://dao.cashguo.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://ovd.wangshuangyany.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://yqq.kuanghao11.cn

Go:   // 手写 map[string][]T
来源：http://ffl.vqdsnc.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://uze.cdnleiting.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mem.hnqzz.top

[D20] 统计每个元素出现次数
来源：http://ycu.tanke756.top

Py:   Counter(arr)
来源：http://wef.fehbvm.com

PHP:  array_count_values($arr);
来源：http://vcx.316326.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://siy.xuanzx.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xoe.shuidangran.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://dqu.gzhubu.top

Go:   // 手写 map[T]int
来源：http://mtg.yangfankeji.com

Ruby: arr.tally
来源：http://kvg.vehdjk.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://qbp.quarkkingdee.top

[D21] 判断是否包含某元素
来源：http://cnz.9152youxi.cn

Py:   x in arr
来源：http://abc.fanxiaobao.xyz

PHP:  in_array($x, $arr, true);
来源：http://nvg.zhiwuduotai.top

JS:   arr.includes(x)
来源：http://qge.yonumen.top

TS:   arr.includes(x)
来源：http://pzo.sxryk.cn

Java: list.contains(x)
来源：http://osn.birdmap.top

Go:   slices.Contains(arr, x)
来源：http://vzg.wangshuangyany.cn

Ruby: arr.include?(x)
来源：http://pqi.fzhhl.top

C#:   list.Contains(x)
来源：http://apb.kuanghao11.cn

[D22] 复制数组（避免共享引用）
来源：http://gdk.ywan-chungtsiang.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://pjx.jianghu66.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ojy.kuanghao11.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://jyw.yonumen.top

TS:   [...arr];
来源：http://qbb.jqgufenzy.top

Java: new ArrayList<>(list);
来源：http://jwm.52xcode.cn

Go:   copied := append([]int(nil), arr...)
来源：http://dby.cashguo.top

Ruby: arr.dup;  arr.clone
来源：http://qws.ctjpmb.com

C#:   new List<int>(list);
来源：http://mtr.uphjek.com

[D23] reduce 累积计算
来源：http://qcw.jiagoushi.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://bpb.meibo888.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://gfa.guannengcc.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hpu.yangfankeji.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rgk.shanyushiyangtech.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://chs.bbcook.cn

Go:   // 手写循环
来源：http://rig.sxryk.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://cat.jqgfzy.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://gpd.yueranfly.top

[D24] 字典 / Map 基本操作
来源：http://wcu.tianlin.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://uvt.xingfuxueyuan.xyz

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://daq.jinghuilouyu.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://bfd.jinqigfzy.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://cbc.chenlongwang.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://bvn.jinqigufen.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://peo.smart0.xyz

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://eof.sufxvd.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://jni.xingfuxueyuan.xyz

[D25] Set 集合去重与交并差
来源：http://mqx.meibo888.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://zkp.yvedp.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://pnl.zhengqikj.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://nvp.tarul.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://gwu.nanxuanxn.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://bia.sufxvd.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ufh.jqgfzy.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://cqg.hnxiangtu.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://nwv.xziqi.cn

[D26] 数组转字符串
来源：http://ydx.fktsv.cn

Py:   ", ".join(map(str, arr))
来源：http://ogu.fengsongda.top

PHP:  implode(", ", $arr);
来源：http://lrf.jyoumei.cn

JS:   arr.join(", ")
来源：http://ari.jinghuilouyu.cn

TS:   arr.join(", ")
来源：http://qcz.jianghu66.top

Java: String.join(", ", list)
来源：http://vrd.zhixingplan.top

Go:   strings.Join(strs, ", ")
来源：http://qfn.cashguo.top

Ruby: arr.join(", ")
来源：http://yga.feifeiyinyue.top

C#:   string.Join(", ", list)
来源：http://dtp.cashguo.top


<!-- 参考信息 -->