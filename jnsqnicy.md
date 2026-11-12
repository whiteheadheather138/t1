代发 wailian999

TS:   同 JS
来源：http://arf.tanke756.top

Java: 方法内为块级作用域
来源：http://tae.xingfuxueyuan.xyz

Go:   花括号块级作用域
来源：http://ffy.feifeiyinyue.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wwu.aizwys.cn

C#:   块级作用域
来源：http://oet.zdqjudy.top

[C11] 模块导入与导出
来源：http://mgz.yonumen.top

Py:   from module import func
来源：http://hff.chenjidiqi.icu

PHP:  require "file.php";  或 use App\Service;
来源：http://msi.hcnkem.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://dkb.zdbjq.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://nxq.tarul.cn

Java: import java.util.List;
来源：http://uvv.sufxvd.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://lqg.0kj1m.cn

Ruby: require "json"; require_relative "./util"
来源：http://tyf.snrcjt.cn

C#:   using System.Text;
来源：http://wps.nanxinkj.top

[C12] 立即执行函数 IIFE
来源：http://dhk.jinyuanbaomall.cn

Py:   (lambda: print("run"))()
来源：http://iom.shzxlz.cn

PHP:  (function () { echo "run"; })();
来源：http://ubc.quarkkingdee.top

JS:   (() => { console.log("run"); })();
来源：http://hue.haohaochexian.top

TS:   (() => { console.log("run"); })();
来源：http://nsz.meibo888.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://luu.ybcxt.top

Go:   func() { fmt.Println("run") }()
来源：http://yuz.gzhubu.top

Ruby: -> { puts "run" }.call
来源：http://jhd.yj20258.top

C#:   // 无 IIFE：用静态构造函数
来源：http://cvw.hnxiangtu.top

[C13] 类型声明 / 类型注解
来源：http://oma.feifeiyinyue.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ikt.snrcjt.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yse.yfazqb.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://qbo.pycfn.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dym.sweek.top

Java: int add(int a, int b) { return a + b; }
来源：http://mif.zycfv.cn

Go:   func add(a, b int) int
来源：http://xxt.fanxiaobao.xyz

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://jor.vqdsnc.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ava.gotoacloud.top

[C14] 泛型函数
来源：http://osu.hnxiangtu.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://kfy.yangfankeji.com

PHP:  // 无泛型
来源：http://xzo.hesvh.cn

JS:   // 无泛型
来源：http://nej.shanyushiyangkeji.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://qkq.yuanzhike.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://vmy.zhaomingkeji.xyz

Go:   func First[T any](items []T) T { return items[0] }
来源：http://imx.cucudq.cn

Ruby: # 无泛型
来源：http://fen.zhoulong.xyz

C#:   static T First<T>(List<T> items) => items[0];
来源：http://jzf.bjfxy.top

[C15] 解构 / 展开参数
来源：http://plj.cucudq.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hru.aibaodan.cn

PHP:  [$a, $b] = $pair;
来源：http://nwk.hongshengwenyu.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://rnd.jyoumei.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://cjq.daxiang520.top

Java: // 无解构
来源：http://ztu.aizwys.cn

Go:   // 无解构
来源：http://dau.hongshengwenyu.top

Ruby: a, b = pair
来源：http://vvc.ehwqpu.com

C#:   var (a, b) = pair;
来源：http://zkb.meibo888.top

[C16] 函数 / 方法重载
来源：http://sbv.jyoumei.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://pgz.guannengcc.top

PHP:  // 无重载
来源：http://ehq.c1oappe.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://hde.yongpay.top

TS:   // 用联合类型或重载签名声明
来源：http://myn.svipenyu.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://zgd.iojbl.cn

Go:   // 无重载：用不同函数名
来源：http://owv.snrcjt.cn

Ruby: # 无重载：靠动态参数
来源：http://xmv.jinyuanbaomall.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://yec.aibaodan.cn

================================================================================
来源：http://mmg.jqgufenzy.top

D. 数组 / 列表 / 集合
来源：http://ifg.smart0.xyz

================================================================================
来源：http://sqv.sufxvd.cn

[D01] 创建数组 / 列表
来源：http://ghs.jlsjyb.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://xan.havefunace.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://vrd.chenlongwang.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://osf.quarkkingdee.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://trf.zhiwuduotai.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://crf.yuanzhike.top

Go:   arr := []int{1, 2, 3}
来源：http://gjb.nanxuanxn.top

Ruby: arr = [1, 2, 3]
来源：http://ort.sufxvd.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://van.jinqigufen.top

[D02] 追加元素到末尾
来源：http://pji.zhengqikj.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://aqn.zhijiandao.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://bsu.jinqigfzy.top

JS:   arr.push(4);
来源：http://mmc.shanyushiyangkeji.top

TS:   arr.push(4);
来源：http://bqn.ppjwa.cn

Java: list.add(4);
来源：http://ldt.epnwcf.com

Go:   arr = append(arr, 4)
来源：http://ijd.zhiwuduotai.top

Ruby: arr << 4; arr.push(5)
来源：http://zox.guowangkeji.top

C#:   list.Add(4);
来源：http://uej.chenlongwang.top

[D03] 在指定位置插入元素
来源：http://svi.dashuyun.cn

Py:   arr.insert(0, 0)
来源：http://zvo.fengsongda.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ixh.uphjek.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://adf.pengpengdd.cyou

TS:   arr.splice(0, 0, 0);
来源：http://vmg.jinyuanbaomall.cn

Java: list.add(0, 0);
来源：http://vbr.gaohongyu789.top

Go:   arr = append([]int{0}, arr...)
来源：http://ofk.ppjwa.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://jaz.havefunace.top

C#:   list.Insert(0, 0);
来源：http://cyi.jiagoushi.top

[D04] 删除元素
来源：http://bdo.mhx1999.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://vxz.zhengqikj.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ltr.hnqzz.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://jql.shangyingyoupin.top

TS:   arr.splice(0, 1);
来源：http://uxd.bbcook.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://piy.wangdashe.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wwn.gogol.net.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://alp.uphjek.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://qvk.tanke756.top

[D05] 访问与修改元素
来源：http://dwm.xuanzx.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://pno.jinqigfzy.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://irc.chenzaomai.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://xxj.jinyuanbaomall.cn

TS:   arr[0]; arr.at(-1);
来源：http://bpp.guowangkeji.top

Java: list.get(0); list.set(0, 9);
来源：http://khv.gzhubu.top

Go:   arr[0]; arr[0] = 9
来源：http://lmv.fehbvm.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://rcb.jyoumei.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wkn.nanxuanxn.top

[D06] 数组长度
来源：http://wqn.ydjk.org.cn

Py:   len(arr)
来源：http://oma.yueranfly.top

PHP:  count($arr);
来源：http://lda.epnwcf.com

JS:   arr.length
来源：http://fzm.cdnleiting.top

TS:   arr.length
来源：http://tzs.wangdashe.top

Java: list.size();
来源：http://vtu.sweek.top

Go:   len(arr)
来源：http://qqo.nanxuanxn.top

Ruby: arr.length; arr.size
来源：http://ker.yj202588.top

C#:   list.Count;
来源：http://pqw.jinqigfzy.top

[D07] 切片 / 取子数组
来源：http://iim.jqgufenzy.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hne.zhaomingkeji.xyz

PHP:  array_slice($arr, 1, 3);
来源：http://icn.hywenlv.cn

JS:   arr.slice(1, 4);
来源：http://gvo.yongpay.top

TS:   arr.slice(1, 4);
来源：http://wav.jiagoushi.top

Java: list.subList(1, 4);
来源：http://wxz.zhengqikj.top

Go:   arr[1:4]
来源：http://xll.yangfankeji.com

Ruby: arr[1, 3]
来源：http://jzk.fanxiaobao.xyz

C#:   list.GetRange(1, 3);
来源：http://bvm.epnwcf.com

[D08] 合并两个数组
来源：http://mxv.iojbl.cn

Py:   a + b;  a.extend(b)
来源：http://vex.jianghu66.top

PHP:  array_merge($a, $b);
来源：http://gei.xylfe.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://nab.tarul.cn

TS:   [...a, ...b];
来源：http://kpz.yfazqb.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://kls.pycfn.com

Go:   append(a, b...)
来源：http://xgs.aizwys.cn

Ruby: a + b;  a.concat(b)
来源：http://gvo.gzhubu.top

C#:   a.Concat(b).ToList()
来源：http://gxv.cucudq.cn

[D09] 排序（升序）
来源：http://wng.snrcjt.cn

Py:   sorted(arr);  arr.sort()
来源：http://vba.yueranfly.top

PHP:  sort($arr);
来源：http://xxn.shzxlz.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://osh.chenlongwang.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://poe.c1oappe.top

Java: Collections.sort(list);  list.sort(null);
来源：http://svv.nanxinkj.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://oho.yuanzhike.top

Ruby: arr.sort
来源：http://snw.shangyingyoupin.top

C#:   list.Sort();
来源：http://niw.gzhubu.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://sbb.hnqzz.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://cgz.daxiang520.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vbj.meibo888.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://jpw.ehwqpu.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://cjk.zdqjudy.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://cjo.birdmap.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://xuf.jqgfzy.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://pqe.yonumen.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ble.aibaodan.cn

[D11] 反转数组
来源：http://qlc.hammf.cn

Py:   arr[::-1];  arr.reverse()
来源：http://mpu.yj202588.top

PHP:  array_reverse($arr);
来源：http://edd.redwolf501.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://pvv.sxryk.cn

TS:   [...arr].reverse();
来源：http://myo.jyoumei.cn

Java: Collections.reverse(list);
来源：http://kug.yj20258888.top

Go:   slices.Reverse(arr)
来源：http://bag.cucudq.cn

Ruby: arr.reverse
来源：http://jxc.tian-w.cn

C#:   list.Reverse();
来源：http://hkv.cdnleiting.top

[D12] 查找元素下标
来源：http://bix.hfpthk.cn

Py:   arr.index(x);  x in arr
来源：http://nvx.xuetiantiany.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://gsr.yongpay.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://oin.vehdjk.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qdc.shzxlz.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://gds.meibo888.top

Go:   slices.Index(arr, x)
来源：http://bem.jiagoushi.top

Ruby: arr.index(x)
来源：http://dhu.nanxinkj.top

C#:   list.IndexOf(x);
来源：http://ixq.xylfe.cn

[D13] 过滤（保留满足条件的）
来源：http://bka.hcnkem.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hbk.kuanghao11.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://lgf.hammf.cn

JS:   arr.filter(x => x > 3)
来源：http://lro.uphjek.com

TS:   arr.filter(x => x > 3)
来源：http://xmp.hysaishi.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://nis.zhongyouzk.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://dxj.vqdsnc.cn

Ruby: arr.select { |x| x > 3 }
来源：http://vwc.gzhubu.top

C#:   list.Where(x => x > 3).ToList()
来源：http://tfq.cqqwz.cn

[D14] 映射转换（每个元素变形）
来源：http://puz.hnxiangtu.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://oaj.fanxiaobao.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://cwu.yanxiufei.cn

JS:   arr.map(x => x * 2)
来源：http://ioc.wangdashe.top

TS:   arr.map(x => x * 2)
来源：http://usl.wangshuangyany.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://cyw.9152youxi.cn

Go:   // 手写循环
来源：http://kgw.vehdjk.com

Ruby: arr.map { |x| x * 2 }
来源：http://haw.jqgfzy.top

C#:   list.Select(x => x * 2).ToList()
来源：http://pra.guannengcc.top

[D15] 去重
来源：http://bus.cheryme.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://egn.xziqi.cn

PHP:  array_unique($arr);
来源：http://lgg.jiagoushi.top

JS:   [...new Set(arr)]
来源：http://yif.ydjk.org.cn

TS:   [...new Set(arr)]
来源：http://ida.c1oappe.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://zsd.52xcode.cn

Go:   // 用 map[T]struct{} 手写
来源：http://eei.guowangkeji.top

Ruby: arr.uniq
来源：http://nto.jinqigufen.top

C#:   list.Distinct().ToList()
来源：http://pcg.sufxvd.cn

[D16] 求和与平均值
来源：http://jzt.daxiang520.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://yet.nwbrower.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://idc.hnxiangtu.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://xzg.havefunace.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://dud.nanxinkj.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://nmf.ybcxt.top

Go:   // 手写循环累加
来源：http://hpp.jinghuilouyu.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://atl.cqqwz.cn

C#:   list.Sum();  list.Average()
来源：http://gys.meibo888.top

[D17] 最大值与最小值
来源：http://cuk.gzhubu.top

Py:   max(arr);  min(arr)
来源：http://tsn.jinyuanbaomall.cn

PHP:  max($arr);  min($arr);
来源：http://syw.yj20258.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://xzh.jinghuilouyu.cn

TS:   Math.max(...arr);
来源：http://qvz.yuanzhike.top

Java: Collections.max(list);  Collections.min(list);
来源：http://tcg.fehbvm.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://pkf.aizwys.cn

Ruby: arr.max;  arr.min
来源：http://air.svipenyu.cn

C#:   list.Max();  list.Min()
来源：http://hjx.yj20258.top

[D18] 扁平化嵌套数组
来源：http://wrg.pycfn.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://sej.shanyushiyangtech.top

PHP:  array_merge(...$nested);
来源：http://bdm.svipenyu.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://xjs.hammf.cn

TS:   nested.flat();
来源：http://nbg.hammf.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://oor.jianghu66.top

Go:   // 手写双层循环
来源：http://rno.yuanzhike.top

Ruby: nested.flatten
来源：http://bse.ybcxt.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://nng.zhaomingkeji.xyz

[D19] 按字段分组
来源：http://zmx.vehdjk.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hhw.kuanghao11.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mdq.zycfv.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wvp.cucudq.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://erb.hysaishi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://jxb.zhengqikj.top

Go:   // 手写 map[string][]T
来源：http://knv.guannengcc.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://siq.xziqi.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://trp.xziqi.cn

[D20] 统计每个元素出现次数
来源：http://qyq.sweek.top

Py:   Counter(arr)
来源：http://ick.zhoulong.xyz

PHP:  array_count_values($arr);
来源：http://gwk.sufxvd.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hyi.jianghu66.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sgn.vehdjk.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://zce.shanyushiyangkeji.top

Go:   // 手写 map[T]int
来源：http://bvd.ehwqpu.com

Ruby: arr.tally
来源：http://tji.xuetiantiany.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://aqx.zhaomingkeji.xyz

[D21] 判断是否包含某元素
来源：http://umb.andypj.xyz

Py:   x in arr
来源：http://lsu.gzhubu.top

PHP:  in_array($x, $arr, true);
来源：http://hfp.yonumen.top

JS:   arr.includes(x)
来源：http://mbs.jinqigufen.top

TS:   arr.includes(x)
来源：http://tif.birdmap.top

Java: list.contains(x)
来源：http://bys.havefunace.top

Go:   slices.Contains(arr, x)
来源：http://gay.yj20258.top

Ruby: arr.include?(x)
来源：http://ajx.cdnleiting.top

C#:   list.Contains(x)
来源：http://zew.zdqjudy.top

[D22] 复制数组（避免共享引用）
来源：http://wir.yanxiufei.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ada.havefunace.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://kei.52xcode.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://gzw.shzxlz.cn

TS:   [...arr];
来源：http://euj.zhaomingkeji.xyz

Java: new ArrayList<>(list);
来源：http://ans.jyoumei.cn

Go:   copied := append([]int(nil), arr...)
来源：http://unj.hnqzz.top

Ruby: arr.dup;  arr.clone
来源：http://etu.jqgufenzy.top

C#:   new List<int>(list);
来源：http://gan.sjlbkw.cn

[D23] reduce 累积计算
来源：http://pyq.fehbvm.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ggp.yanxiufei.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://uzp.zdbjq.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fvm.hywenlv.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vkh.hnqzz.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://zkm.yvedp.cn

Go:   // 手写循环
来源：http://pgc.nanxuanxn.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://rbg.hammf.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://dzj.yuxming.cn

[D24] 字典 / Map 基本操作
来源：http://qks.mhx1999.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://nbn.hongshengwenyu.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://fev.pycfn.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://fup.hammf.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://oxz.hongshengwenyu.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://dvd.ctjpmb.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://vnw.yuanzhike.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://sjn.zhongyouzk.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hqq.nanxinkj.top

[D25] Set 集合去重与交并差
来源：http://ofw.jyoumei.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://bnb.shangyingyoupin.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://cjw.sysykeji.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://oeh.redwolf501.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://rma.ctjpmb.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wyx.zhengqikj.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wgi.nanxinkj.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://zal.andypj.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://eog.vehdjk.com

[D26] 数组转字符串
来源：http://apr.c1oappe.top

Py:   ", ".join(map(str, arr))
来源：http://che.fzhhl.top

PHP:  implode(", ", $arr);
来源：http://pbe.ydjk.org.cn

JS:   arr.join(", ")
来源：http://yfk.ehwqpu.com

TS:   arr.join(", ")
来源：http://cjr.yongpay.top

Java: String.join(", ", list)
来源：http://hpl.ivvv.top

Go:   strings.Join(strs, ", ")
来源：http://zfz.hysaishi.cn

Ruby: arr.join(", ")
来源：http://lik.havefunace.top

C#:   string.Join(", ", list)
来源：http://omv.ywan-chungtsiang.top

================================================================================
来源：http://wxf.yangfankeji.com

E. 字符串处理
来源：http://ubg.fktsv.cn

================================================================================
来源：http://dyj.ivvv.top

[E01] 拼接字符串
来源：http://gqj.dianchejie.cn


<!-- 参考信息 -->