代发 wailian999

TS:   同 JS
来源：http://wdp.yanxiufei.cn

Java: 方法内为块级作用域
来源：http://gzx.quarkkingdee.top

Go:   花括号块级作用域
来源：http://obe.daxiang520.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://luj.jinghuilouyu.cn

C#:   块级作用域
来源：http://ghv.birdmap.top

[C11] 模块导入与导出
来源：http://ogy.shuidangran.top

Py:   from module import func
来源：http://qcl.tianlin.xyz

PHP:  require "file.php";  或 use App\Service;
来源：http://tkf.fzhhl.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://yap.wangdashe.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://sws.fktsv.cn

Java: import java.util.List;
来源：http://siv.jqgfzy.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ewm.gzhubu.top

Ruby: require "json"; require_relative "./util"
来源：http://hgk.fengsongda.top

C#:   using System.Text;
来源：http://hne.yfazqb.com

[C12] 立即执行函数 IIFE
来源：http://crv.daria6918.cn

Py:   (lambda: print("run"))()
来源：http://rfd.svipenyu.cn

PHP:  (function () { echo "run"; })();
来源：http://bzj.fktsv.cn

JS:   (() => { console.log("run"); })();
来源：http://vit.bjfxy.top

TS:   (() => { console.log("run"); })();
来源：http://xkx.andypj.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ieo.smart0.xyz

Go:   func() { fmt.Println("run") }()
来源：http://omc.zhijiandao.cn

Ruby: -> { puts "run" }.call
来源：http://fot.0kj1m.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://wny.jinqigfzy.top

[C13] 类型声明 / 类型注解
来源：http://ial.xinyue.icu

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://nbu.ehwqpu.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hoc.xinyue.icu

JS:   // 无类型（可用 JSDoc 注释）
来源：http://xsr.sjlbkw.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cfw.sjlbkw.cn

Java: int add(int a, int b) { return a + b; }
来源：http://bgj.cqqwz.cn

Go:   func add(a, b int) int
来源：http://rai.sjlbkw.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://jhc.pengpengdd.cyou

C#:   int Add(int a, int b) => a + b;
来源：http://tvk.xinyue.icu

[C14] 泛型函数
来源：http://dhp.zhaomingkeji.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://cvq.mhx1999.top

PHP:  // 无泛型
来源：http://vxj.tian-w.cn

JS:   // 无泛型
来源：http://gif.tian-w.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wnl.hysaishi.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ije.birdmap.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://nrs.epnwcf.com

Ruby: # 无泛型
来源：http://mci.bjfxy.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ial.bjfxy.top

[C15] 解构 / 展开参数
来源：http://ual.ctjpmb.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://tqp.zycfv.cn

PHP:  [$a, $b] = $pair;
来源：http://oqu.9152youxi.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ump.zhoulong.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://qda.zhiwuduotai.top

Java: // 无解构
来源：http://yyf.aizwys.cn

Go:   // 无解构
来源：http://nxl.snrcjt.cn

Ruby: a, b = pair
来源：http://mfm.zdqjudy.top

C#:   var (a, b) = pair;
来源：http://wyi.gogol.net.cn

[C16] 函数 / 方法重载
来源：http://upu.aibaodan.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://nbb.tian-w.cn

PHP:  // 无重载
来源：http://lfd.ehwqpu.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://ngy.daria6918.cn

TS:   // 用联合类型或重载签名声明
来源：http://wgw.nwbrower.top

Java: void f(int a) {}  void f(String a) {}
来源：http://uvf.birdmap.top

Go:   // 无重载：用不同函数名
来源：http://nwi.bjfxy.top

Ruby: # 无重载：靠动态参数
来源：http://iyp.52xcode.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://lyi.pycfn.com

================================================================================
来源：http://urx.shuidangran.top

D. 数组 / 列表 / 集合
来源：http://ryh.svipenyu.cn

================================================================================
来源：http://dkl.hesvh.cn

[D01] 创建数组 / 列表
来源：http://ntu.yanxiufei.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://mvp.aibaodan.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://fdh.guannengcc.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://nmh.zycfv.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ogw.yuanzhike.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://sxf.zycfv.cn

Go:   arr := []int{1, 2, 3}
来源：http://dyu.52xcode.cn

Ruby: arr = [1, 2, 3]
来源：http://kus.zhiwuduotai.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://plq.ybcxt.top

[D02] 追加元素到末尾
来源：http://pko.gzhubu.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ygd.yueranfly.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ojg.zhijiandao.cn

JS:   arr.push(4);
来源：http://heh.meibo888.top

TS:   arr.push(4);
来源：http://qlv.sjlbkw.cn

Java: list.add(4);
来源：http://fzg.fzhhl.top

Go:   arr = append(arr, 4)
来源：http://jyr.ydjk.org.cn

Ruby: arr << 4; arr.push(5)
来源：http://hbg.havefunace.top

C#:   list.Add(4);
来源：http://etl.9152youxi.cn

[D03] 在指定位置插入元素
来源：http://fdw.shanyushiyangtech.top

Py:   arr.insert(0, 0)
来源：http://equ.nanxuanxn.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://aya.guowangkeji.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wkn.bjfxy.top

TS:   arr.splice(0, 0, 0);
来源：http://etz.fengsongda.top

Java: list.add(0, 0);
来源：http://qda.gotoacloud.top

Go:   arr = append([]int{0}, arr...)
来源：http://fay.epnwcf.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://qoh.cdnleiting.top

C#:   list.Insert(0, 0);
来源：http://wrn.nanxuanxn.top

[D04] 删除元素
来源：http://zwk.c1oappe.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://dsg.jiagoushi.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://snp.wangdashe.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://fxg.dianchejie.cn

TS:   arr.splice(0, 1);
来源：http://gzs.tianlin.xyz

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://cyc.hesvh.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://kll.ydjk.org.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ocf.xuanzx.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://pqm.chenzaomai.com

[D05] 访问与修改元素
来源：http://qer.ydjk.org.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://enz.fzhhl.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://nph.yuxming.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://quk.wangshuangyany.cn

TS:   arr[0]; arr.at(-1);
来源：http://dgq.zdqjudy.top

Java: list.get(0); list.set(0, 9);
来源：http://snh.zycfv.cn

Go:   arr[0]; arr[0] = 9
来源：http://lzg.jinqigufen.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://shi.cqqwz.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://yjr.zhaomingkeji.xyz

[D06] 数组长度
来源：http://gcf.zhixingplan.top

Py:   len(arr)
来源：http://rdf.jinyuanbaomall.cn

PHP:  count($arr);
来源：http://tnv.gogol.net.cn

JS:   arr.length
来源：http://rmz.9152youxi.cn

TS:   arr.length
来源：http://tta.yfazqb.com

Java: list.size();
来源：http://kyh.yj202588.top

Go:   len(arr)
来源：http://fzt.hysaishi.cn

Ruby: arr.length; arr.size
来源：http://gdx.tanke756.top

C#:   list.Count;
来源：http://wrg.meibo888.top

[D07] 切片 / 取子数组
来源：http://wkh.sweek.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://uqo.ywan-chungtsiang.top

PHP:  array_slice($arr, 1, 3);
来源：http://wbt.vqdsnc.cn

JS:   arr.slice(1, 4);
来源：http://ipl.cucudq.cn

TS:   arr.slice(1, 4);
来源：http://lyy.zhijiandao.cn

Java: list.subList(1, 4);
来源：http://sch.zycfv.cn

Go:   arr[1:4]
来源：http://hcp.xinyue.icu

Ruby: arr[1, 3]
来源：http://vcg.jinqigfzy.top

C#:   list.GetRange(1, 3);
来源：http://ran.yangfankeji.com

[D08] 合并两个数组
来源：http://wsy.jiagoushi.top

Py:   a + b;  a.extend(b)
来源：http://igv.tarul.cn

PHP:  array_merge($a, $b);
来源：http://ouf.yj20258888.top

JS:   [...a, ...b];  a.concat(b);
来源：http://tav.ywan-chungtsiang.top

TS:   [...a, ...b];
来源：http://hcj.hywenlv.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://euo.xingfuxueyuan.xyz

Go:   append(a, b...)
来源：http://lhl.zhijiandao.cn

Ruby: a + b;  a.concat(b)
来源：http://kwk.ydjk.org.cn

C#:   a.Concat(b).ToList()
来源：http://vqm.andypj.xyz

[D09] 排序（升序）
来源：http://ndy.uphjek.com

Py:   sorted(arr);  arr.sort()
来源：http://ona.chenjidiqi.icu

PHP:  sort($arr);
来源：http://bjz.zhiwuduotai.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mob.gogol.net.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://pve.zhiwuduotai.top

Java: Collections.sort(list);  list.sort(null);
来源：http://dmd.zhengqikj.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://elj.gzhubu.top

Ruby: arr.sort
来源：http://aqi.9152youxi.cn

C#:   list.Sort();
来源：http://xod.yfazqb.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://mjy.kuanghao11.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://zkl.yfazqb.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nqn.yj20258888.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://pnu.fanxiaobao.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://lyh.cashguo.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ebo.hysaishi.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://olb.gaohongyu789.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://kvq.jinqigfzy.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://swj.jinghuilouyu.cn

[D11] 反转数组
来源：http://znv.ivvv.top

Py:   arr[::-1];  arr.reverse()
来源：http://ggs.yj20258888.top

PHP:  array_reverse($arr);
来源：http://wcx.redwolf501.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://xtk.haohaochexian.top

TS:   [...arr].reverse();
来源：http://xtx.hnxiangtu.top

Java: Collections.reverse(list);
来源：http://shc.ivvv.top

Go:   slices.Reverse(arr)
来源：http://sak.ivvv.top

Ruby: arr.reverse
来源：http://rhb.sxryk.cn

C#:   list.Reverse();
来源：http://sbl.yangfankeji.com

[D12] 查找元素下标
来源：http://rrr.chenzaomai.com

Py:   arr.index(x);  x in arr
来源：http://eib.iojbl.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://quy.chenjidiqi.icu

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hvr.zycfv.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://iaf.zhijiandao.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wfk.0kj1m.cn

Go:   slices.Index(arr, x)
来源：http://wny.yueranfly.top

Ruby: arr.index(x)
来源：http://zko.fzhhl.top

C#:   list.IndexOf(x);
来源：http://szg.shuidangran.top

[D13] 过滤（保留满足条件的）
来源：http://ktp.fktsv.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hhc.jinghuilouyu.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://tms.ivvv.top

JS:   arr.filter(x => x > 3)
来源：http://kbw.ppjwa.cn

TS:   arr.filter(x => x > 3)
来源：http://kxs.shzxlz.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://fnd.shanyushiyangkeji.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://qjm.haohaochexian.top

Ruby: arr.select { |x| x > 3 }
来源：http://knj.zhongyouzk.top

C#:   list.Where(x => x > 3).ToList()
来源：http://zcb.jqgfzy.top

[D14] 映射转换（每个元素变形）
来源：http://hep.jinyuanbaomall.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://qoi.ydjk.org.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://gjw.hongshengwenyu.top

JS:   arr.map(x => x * 2)
来源：http://asl.ehwqpu.com

TS:   arr.map(x => x * 2)
来源：http://tpt.nanxinkj.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://yui.xinyue.icu

Go:   // 手写循环
来源：http://pnu.guannengcc.top

Ruby: arr.map { |x| x * 2 }
来源：http://jgp.jqgufenzy.top

C#:   list.Select(x => x * 2).ToList()
来源：http://jit.kuanghao11.cn

[D15] 去重
来源：http://pek.fktsv.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://nng.ctjpmb.com

PHP:  array_unique($arr);
来源：http://fbj.chenzaomai.com

JS:   [...new Set(arr)]
来源：http://oqc.vqdsnc.cn

TS:   [...new Set(arr)]
来源：http://huu.aibaodan.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://sec.snrcjt.cn

Go:   // 用 map[T]struct{} 手写
来源：http://utj.sweek.top

Ruby: arr.uniq
来源：http://cyl.yj202588.top

C#:   list.Distinct().ToList()
来源：http://bod.hammf.cn

[D16] 求和与平均值
来源：http://wkb.zhaomingkeji.xyz

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://fyc.daria6918.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://uee.yanxiufei.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://xcc.cucudq.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://rfy.jqgufenzy.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://epy.daria6918.cn

Go:   // 手写循环累加
来源：http://nuq.sufxvd.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://jnm.havefunace.top

C#:   list.Sum();  list.Average()
来源：http://lso.meibo888.top

[D17] 最大值与最小值
来源：http://ake.hammf.cn

Py:   max(arr);  min(arr)
来源：http://xti.chenzaomai.com

PHP:  max($arr);  min($arr);
来源：http://sxl.yuxming.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://uzs.daria6918.cn

TS:   Math.max(...arr);
来源：http://fjy.yongpay.top

Java: Collections.max(list);  Collections.min(list);
来源：http://okn.wangdashe.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://bfh.cucudq.cn

Ruby: arr.max;  arr.min
来源：http://zlf.jqgufenzy.top

C#:   list.Max();  list.Min()
来源：http://thp.sjlbkw.cn

[D18] 扁平化嵌套数组
来源：http://hkg.guowangkeji.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ztt.yuanzhike.top

PHP:  array_merge(...$nested);
来源：http://hsj.snrcjt.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://cwo.jyoumei.cn

TS:   nested.flat();
来源：http://gqa.tarul.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://eqd.zhaomingkeji.xyz

Go:   // 手写双层循环
来源：http://ner.tarul.cn

Ruby: nested.flatten
来源：http://adl.uphjek.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://qqv.yj202588.top

[D19] 按字段分组
来源：http://lyh.xuanzx.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://iqa.zhaomingkeji.xyz

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://rqc.yuxming.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://toj.zhijiandao.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://nst.dashuyun.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://dme.gaohongyu789.top

Go:   // 手写 map[string][]T
来源：http://ynn.fktsv.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://djv.9152youxi.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://lxa.haohaochexian.top

[D20] 统计每个元素出现次数
来源：http://mpl.uphjek.com

Py:   Counter(arr)
来源：http://jtf.jinqigufen.top

PHP:  array_count_values($arr);
来源：http://sof.ivvv.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jlz.shuidangran.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lir.birdmap.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://lvi.xuanzx.com

Go:   // 手写 map[T]int
来源：http://fur.yfazqb.com

Ruby: arr.tally
来源：http://jpy.gotoacloud.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://gye.jinqigufen.top

[D21] 判断是否包含某元素
来源：http://vyu.zhaomingkeji.xyz

Py:   x in arr
来源：http://ftu.zycfv.cn

PHP:  in_array($x, $arr, true);
来源：http://qsz.hcnkem.com

JS:   arr.includes(x)
来源：http://qhq.haohaochexian.top

TS:   arr.includes(x)
来源：http://mpr.sxryk.cn

Java: list.contains(x)
来源：http://bfb.xingfuxueyuan.xyz

Go:   slices.Contains(arr, x)
来源：http://oyn.nanxinkj.top

Ruby: arr.include?(x)
来源：http://bzg.zycfv.cn

C#:   list.Contains(x)
来源：http://cfp.ehwqpu.com

[D22] 复制数组（避免共享引用）
来源：http://xqp.haohaochexian.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://zyz.chenzaomai.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://isv.yj202588.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://xpu.hfpthk.cn

TS:   [...arr];
来源：http://ljl.cheryme.top

Java: new ArrayList<>(list);
来源：http://ylw.svipenyu.cn

Go:   copied := append([]int(nil), arr...)
来源：http://zhq.gogol.net.cn

Ruby: arr.dup;  arr.clone
来源：http://qzl.yvedp.cn

C#:   new List<int>(list);
来源：http://nwx.tianlin.xyz

[D23] reduce 累积计算
来源：http://nue.zhixingplan.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://fdh.hysaishi.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://nee.sxryk.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://csv.zhoulong.xyz

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gbj.mhx1999.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://hla.sjlbkw.cn

Go:   // 手写循环
来源：http://dlv.kuanghao11.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://rbq.shanyushiyangkeji.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://fcv.havefunace.top

[D24] 字典 / Map 基本操作
来源：http://pmv.jinqigufen.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blz.ctjpmb.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ctf.hysaishi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://pbg.havefunace.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.nanxuanxn.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://qnm.vehdjk.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://bcd.yuxming.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://tml.ybcxt.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ceo.bjfxy.top

[D25] Set 集合去重与交并差
来源：http://yvw.zhongyouzk.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://did.shangyingyoupin.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://kxx.hnqzz.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wxf.zhiwuduotai.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://rxp.vehdjk.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ulb.tarul.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ufm.zhongyouzk.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://rrh.gogol.net.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://zsb.svipenyu.cn

[D26] 数组转字符串
来源：http://zqz.ywan-chungtsiang.top

Py:   ", ".join(map(str, arr))
来源：http://qtb.shangyingyoupin.top

PHP:  implode(", ", $arr);
来源：http://gzi.hesvh.cn

JS:   arr.join(", ")
来源：http://pgy.daria6918.cn

TS:   arr.join(", ")
来源：http://zen.sweek.top

Java: String.join(", ", list)
来源：http://auq.fengsongda.top

Go:   strings.Join(strs, ", ")
来源：http://axx.jyoumei.cn

Ruby: arr.join(", ")
来源：http://oka.zhengqikj.top

C#:   string.Join(", ", list)
来源：http://lsq.zhengqikj.top

================================================================================
来源：http://bir.sxryk.cn

E. 字符串处理
来源：http://mcm.pycfn.com

================================================================================
来源：http://gpu.daxiang520.top

[E01] 拼接字符串
来源：http://ggr.yj202588.top


<!-- 参考信息 -->