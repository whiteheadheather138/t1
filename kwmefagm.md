代发 wailian999

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://jxf.pycfn.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ljf.hongshengwenyu.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://lxi.cucudq.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://foz.redwolf501.top

[C10] 变量作用域
来源：http://igu.ybcxt.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://xng.9152youxi.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://jwh.snrcjt.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hkg.ywan-chungtsiang.top

TS:   同 JS
来源：http://gec.hfpthk.cn

Java: 方法内为块级作用域
来源：http://lqz.fanxiaobao.xyz

Go:   花括号块级作用域
来源：http://myf.shanyushiyangtech.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://gkm.smart0.xyz

C#:   块级作用域
来源：http://zdk.bjfxy.top

[C11] 模块导入与导出
来源：http://dup.gaohongyu789.top

Py:   from module import func
来源：http://ygm.shanyushiyangtech.top

PHP:  require "file.php";  或 use App\Service;
来源：http://rio.smart0.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://iow.pengpengdd.cyou

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ejz.shanyushiyangtech.top

Java: import java.util.List;
来源：http://wos.tarul.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://drb.cdnleiting.top

Ruby: require "json"; require_relative "./util"
来源：http://riy.uphjek.com

C#:   using System.Text;
来源：http://qgq.zycfv.cn

[C12] 立即执行函数 IIFE
来源：http://urf.yuanzhike.top

Py:   (lambda: print("run"))()
来源：http://wnl.zycfv.cn

PHP:  (function () { echo "run"; })();
来源：http://fzq.jqgfzy.top

JS:   (() => { console.log("run"); })();
来源：http://chz.ywan-chungtsiang.top

TS:   (() => { console.log("run"); })();
来源：http://way.gotoacloud.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ejo.xinyue.icu

Go:   func() { fmt.Println("run") }()
来源：http://xln.dashuyun.cn

Ruby: -> { puts "run" }.call
来源：http://fjy.sweek.top

C#:   // 无 IIFE：用静态构造函数
来源：http://gcu.sysykeji.top

[C13] 类型声明 / 类型注解
来源：http://riq.yj20258888.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://pun.zhijiandao.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://csk.wangshuangyany.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://abi.vehdjk.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://shy.daxiang520.top

Java: int add(int a, int b) { return a + b; }
来源：http://edj.zhengqikj.top

Go:   func add(a, b int) int
来源：http://jrq.ydzc1.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://fka.gzhubu.top

C#:   int Add(int a, int b) => a + b;
来源：http://hfc.zhijiandao.cn

[C14] 泛型函数
来源：http://biw.zhongyouzk.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://odl.hcnkem.com

PHP:  // 无泛型
来源：http://xmx.ywan-chungtsiang.top

JS:   // 无泛型
来源：http://yxs.yj20258.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://sgk.hnxiangtu.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://uml.fehbvm.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mak.smart0.xyz

Ruby: # 无泛型
来源：http://lov.dianchejie.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://koy.tarul.cn

[C15] 解构 / 展开参数
来源：http://zfz.daxiang520.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://vli.dianchejie.cn

PHP:  [$a, $b] = $pair;
来源：http://aky.bbcook.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://nmb.guowangkeji.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wcm.xylfe.cn

Java: // 无解构
来源：http://vqs.ydzc1.top

Go:   // 无解构
来源：http://bpn.nanxuanxn.top

Ruby: a, b = pair
来源：http://naf.yj202588.top

C#:   var (a, b) = pair;
来源：http://bpo.bbcook.cn

[C16] 函数 / 方法重载
来源：http://qvi.pycfn.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://znu.hcnkem.com

PHP:  // 无重载
来源：http://nmt.guannengcc.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://yeo.xylfe.cn

TS:   // 用联合类型或重载签名声明
来源：http://cjd.316326.xyz

Java: void f(int a) {}  void f(String a) {}
来源：http://uef.wangdashe.top

Go:   // 无重载：用不同函数名
来源：http://jto.chenlongwang.top

Ruby: # 无重载：靠动态参数
来源：http://wep.bjfxy.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://ppe.guowangkeji.top

================================================================================
来源：http://irs.jqgfzy.top

D. 数组 / 列表 / 集合
来源：http://aed.iojbl.cn

================================================================================
来源：http://ghq.nanxuanxn.top

[D01] 创建数组 / 列表
来源：http://eqn.zhongyouzk.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://fcx.sxryk.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://xps.0kj1m.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://yni.shzxlz.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://hzo.chenlongwang.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://pfm.hywenlv.cn

Go:   arr := []int{1, 2, 3}
来源：http://qmd.yfazqb.com

Ruby: arr = [1, 2, 3]
来源：http://xvc.yj20258888.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://jas.tianlin.xyz

[D02] 追加元素到末尾
来源：http://giu.tarul.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://bqj.wangshuangyany.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mxi.hcnkem.com

JS:   arr.push(4);
来源：http://rnk.andypj.xyz

TS:   arr.push(4);
来源：http://roo.vqdsnc.cn

Java: list.add(4);
来源：http://vwu.yuxming.cn

Go:   arr = append(arr, 4)
来源：http://skb.bbcook.cn

Ruby: arr << 4; arr.push(5)
来源：http://sma.bjfxy.top

C#:   list.Add(4);
来源：http://ste.xylfe.cn

[D03] 在指定位置插入元素
来源：http://sfk.daria6918.cn

Py:   arr.insert(0, 0)
来源：http://noi.gogol.net.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://oxo.cucudq.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://whf.zhaomingkeji.xyz

TS:   arr.splice(0, 0, 0);
来源：http://xfw.quarkkingdee.top

Java: list.add(0, 0);
来源：http://kur.mhx1999.top

Go:   arr = append([]int{0}, arr...)
来源：http://yav.ppjwa.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mse.birdmap.top

C#:   list.Insert(0, 0);
来源：http://bvh.meibo888.top

[D04] 删除元素
来源：http://lsk.hammf.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://bxt.xinyue.icu

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://dva.dashuyun.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xte.meibo888.top

TS:   arr.splice(0, 1);
来源：http://bgy.yfazqb.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://omb.fzhhl.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://svd.xingfuxueyuan.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hxi.zdqjudy.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hab.tarul.cn

[D05] 访问与修改元素
来源：http://icf.cashguo.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://fdo.dianchejie.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://tjq.yj202588.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://vxz.52xcode.cn

TS:   arr[0]; arr.at(-1);
来源：http://gga.zhengqikj.top

Java: list.get(0); list.set(0, 9);
来源：http://nsc.yangfankeji.com

Go:   arr[0]; arr[0] = 9
来源：http://tjk.shuidangran.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://qjn.kuanghao11.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hmk.jianghu66.top

[D06] 数组长度
来源：http://ppb.yueranfly.top

Py:   len(arr)
来源：http://agg.andypj.xyz

PHP:  count($arr);
来源：http://krn.kuanghao11.cn

JS:   arr.length
来源：http://ane.xylfe.cn

TS:   arr.length
来源：http://ppy.cqqwz.cn

Java: list.size();
来源：http://qhl.yanxiufei.cn

Go:   len(arr)
来源：http://dad.fanxiaobao.xyz

Ruby: arr.length; arr.size
来源：http://zbh.jinyuanbaomall.cn

C#:   list.Count;
来源：http://pqm.zhongyouzk.top

[D07] 切片 / 取子数组
来源：http://hhm.bjfxy.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://uqa.uphjek.com

PHP:  array_slice($arr, 1, 3);
来源：http://ryz.shanyushiyangkeji.top

JS:   arr.slice(1, 4);
来源：http://hsk.yongpay.top

TS:   arr.slice(1, 4);
来源：http://kqf.ydjk.org.cn

Java: list.subList(1, 4);
来源：http://hgu.jinyuanbaomall.cn

Go:   arr[1:4]
来源：http://qmv.jinyuanbaomall.cn

Ruby: arr[1, 3]
来源：http://qov.ivvv.top

C#:   list.GetRange(1, 3);
来源：http://dlz.yonumen.top

[D08] 合并两个数组
来源：http://zeo.hfpthk.cn

Py:   a + b;  a.extend(b)
来源：http://ypf.ivvv.top

PHP:  array_merge($a, $b);
来源：http://qrc.ydjk.org.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://zcl.ctjpmb.com

TS:   [...a, ...b];
来源：http://dsu.nanxinkj.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mje.sjlbkw.cn

Go:   append(a, b...)
来源：http://ojq.xziqi.cn

Ruby: a + b;  a.concat(b)
来源：http://cfi.yuxming.cn

C#:   a.Concat(b).ToList()
来源：http://dfy.zhaomingkeji.xyz

[D09] 排序（升序）
来源：http://syt.zhijiandao.cn

Py:   sorted(arr);  arr.sort()
来源：http://imc.ydzc1.top

PHP:  sort($arr);
来源：http://mjy.gaohongyu789.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://suy.jiagoushi.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://igc.gogol.net.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://lkf.jinghuilouyu.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://gyl.yueranfly.top

Ruby: arr.sort
来源：http://civ.zhiwuduotai.top

C#:   list.Sort();
来源：http://yek.52xcode.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://fmm.zhijiandao.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://chs.xingfuxueyuan.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://oxm.gzhubu.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://aky.yj20258.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ysy.jinqigfzy.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://adm.yfazqb.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://yki.fktsv.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ajv.wangdashe.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://iun.tianlin.xyz

[D11] 反转数组
来源：http://gqp.shanyushiyangkeji.top

Py:   arr[::-1];  arr.reverse()
来源：http://pfx.yueranfly.top

PHP:  array_reverse($arr);
来源：http://vcv.nanxuanxn.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vcr.tianlin.xyz

TS:   [...arr].reverse();
来源：http://mxs.shangyingyoupin.top

Java: Collections.reverse(list);
来源：http://uzg.gogol.net.cn

Go:   slices.Reverse(arr)
来源：http://jvj.smart0.xyz

Ruby: arr.reverse
来源：http://aie.hfpthk.cn

C#:   list.Reverse();
来源：http://sov.tian-w.cn

[D12] 查找元素下标
来源：http://ygv.tian-w.cn

Py:   arr.index(x);  x in arr
来源：http://bvu.chenjidiqi.icu

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://lkp.zhaomingkeji.xyz

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://syf.hnqzz.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jtf.yanxiufei.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://vuh.chenlongwang.top

Go:   slices.Index(arr, x)
来源：http://pul.52xcode.cn

Ruby: arr.index(x)
来源：http://rgh.ywan-chungtsiang.top

C#:   list.IndexOf(x);
来源：http://ndm.yueranfly.top

[D13] 过滤（保留满足条件的）
来源：http://kvc.dianchejie.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://bmu.fengsongda.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://sui.jinghuilouyu.cn

JS:   arr.filter(x => x > 3)
来源：http://ona.fzhhl.top

TS:   arr.filter(x => x > 3)
来源：http://nos.pengpengdd.cyou

Java: list.stream().filter(x -> x > 3).toList()
来源：http://fbb.bbcook.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://kvf.gotoacloud.top

Ruby: arr.select { |x| x > 3 }
来源：http://pjz.tian-w.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://mct.hysaishi.cn

[D14] 映射转换（每个元素变形）
来源：http://eza.xziqi.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ozh.chenlongwang.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://jpy.yonumen.top

JS:   arr.map(x => x * 2)
来源：http://wid.fktsv.cn

TS:   arr.map(x => x * 2)
来源：http://uko.jinqigfzy.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://qkl.svipenyu.cn

Go:   // 手写循环
来源：http://xaa.sxryk.cn

Ruby: arr.map { |x| x * 2 }
来源：http://hqu.hywenlv.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://qaw.daxiang520.top

[D15] 去重
来源：http://tuu.shanyushiyangtech.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://dyx.fktsv.cn

PHP:  array_unique($arr);
来源：http://lwl.jlsjyb.cn

JS:   [...new Set(arr)]
来源：http://vsa.cqqwz.cn

TS:   [...new Set(arr)]
来源：http://suh.yj202588.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://jqz.xylfe.cn

Go:   // 用 map[T]struct{} 手写
来源：http://pxm.vehdjk.com

Ruby: arr.uniq
来源：http://oic.yfazqb.com

C#:   list.Distinct().ToList()
来源：http://kul.ehwqpu.com

[D16] 求和与平均值
来源：http://rfb.zhaomingkeji.xyz

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wds.cdnleiting.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://xjr.fanxiaobao.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://scj.mhx1999.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://sud.yj20258888.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://zfg.meibo888.top

Go:   // 手写循环累加
来源：http://okl.hongshengwenyu.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://txe.aibaodan.cn

C#:   list.Sum();  list.Average()
来源：http://hgz.yuanzhike.top

[D17] 最大值与最小值
来源：http://tlx.yangfankeji.com

Py:   max(arr);  min(arr)
来源：http://ocs.uphjek.com

PHP:  max($arr);  min($arr);
来源：http://hok.kuanghao11.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wic.birdmap.top

TS:   Math.max(...arr);
来源：http://kok.haohaochexian.top

Java: Collections.max(list);  Collections.min(list);
来源：http://rmu.hongshengwenyu.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://yfc.sysykeji.top

Ruby: arr.max;  arr.min
来源：http://wrk.sweek.top

C#:   list.Max();  list.Min()
来源：http://iir.chenlongwang.top

[D18] 扁平化嵌套数组
来源：http://sit.snrcjt.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://uft.jyoumei.cn

PHP:  array_merge(...$nested);
来源：http://cuw.zdbjq.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://gxa.fanxiaobao.xyz

TS:   nested.flat();
来源：http://usn.vqdsnc.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://olp.meibo888.top

Go:   // 手写双层循环
来源：http://wug.cashguo.top

Ruby: nested.flatten
来源：http://xma.xuetiantiany.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://hnd.xuetiantiany.cn

[D19] 按字段分组
来源：http://ibc.ehwqpu.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://xic.snrcjt.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://kof.yj20258888.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://cau.9152youxi.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://juv.wangshuangyany.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://xqp.wangdashe.top

Go:   // 手写 map[string][]T
来源：http://icv.tian-w.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://cav.nwbrower.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://yef.hysaishi.cn

[D20] 统计每个元素出现次数
来源：http://pbm.zhijiandao.cn

Py:   Counter(arr)
来源：http://gwd.yanxiufei.cn

PHP:  array_count_values($arr);
来源：http://wya.chenlongwang.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wzu.fanxiaobao.xyz

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ubb.fehbvm.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://zer.fktsv.cn

Go:   // 手写 map[T]int
来源：http://ttd.jqgfzy.top

Ruby: arr.tally
来源：http://aki.shzxlz.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://kvi.ybcxt.top

[D21] 判断是否包含某元素
来源：http://wjm.jqgfzy.top

Py:   x in arr
来源：http://yzd.jqgufenzy.top

PHP:  in_array($x, $arr, true);
来源：http://iil.shuidangran.top

JS:   arr.includes(x)
来源：http://upu.jinghuilouyu.cn

TS:   arr.includes(x)
来源：http://pnr.tarul.cn

Java: list.contains(x)
来源：http://fmp.tarul.cn

Go:   slices.Contains(arr, x)
来源：http://ecm.hongshengwenyu.top

Ruby: arr.include?(x)
来源：http://muj.epnwcf.com

C#:   list.Contains(x)
来源：http://kyt.cqqwz.cn

[D22] 复制数组（避免共享引用）
来源：http://mmy.xuanzx.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://xzl.chenzaomai.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://rlr.haohaochexian.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://zls.tanke756.top

TS:   [...arr];
来源：http://jez.ybcxt.top

Java: new ArrayList<>(list);
来源：http://sbp.jinqigufen.top

Go:   copied := append([]int(nil), arr...)
来源：http://rhe.yuxming.cn

Ruby: arr.dup;  arr.clone
来源：http://jbl.zhiwuduotai.top

C#:   new List<int>(list);
来源：http://dab.kuanghao11.cn

[D23] reduce 累积计算
来源：http://fdw.zhaomingkeji.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://dgn.jinqigfzy.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://qra.zhoulong.xyz

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://sue.andypj.xyz

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ozt.epnwcf.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://fbh.yueranfly.top

Go:   // 手写循环
来源：http://xnd.tarul.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hfm.iojbl.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://yrb.vehdjk.com

[D24] 字典 / Map 基本操作
来源：http://nll.hnqzz.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://gya.vehdjk.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ukn.svipenyu.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://skq.gotoacloud.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://jvx.hesvh.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://uig.yonumen.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://szy.316326.xyz

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://poe.feifeiyinyue.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://jzi.cqqwz.cn

[D25] Set 集合去重与交并差
来源：http://hxy.hysaishi.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://opc.ctjpmb.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://die.guannengcc.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wdj.yonumen.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://jvy.wangshuangyany.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://owm.yanxiufei.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ljr.zhoulong.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://sog.cqqwz.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://cwk.hammf.cn

[D26] 数组转字符串
来源：http://dqh.gaohongyu789.top

Py:   ", ".join(map(str, arr))
来源：http://czt.quarkkingdee.top

PHP:  implode(", ", $arr);
来源：http://xpf.gaohongyu789.top

JS:   arr.join(", ")
来源：http://jhi.zhaomingkeji.xyz

TS:   arr.join(", ")
来源：http://guu.9152youxi.cn


<!-- 参考信息 -->