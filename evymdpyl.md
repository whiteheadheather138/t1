代发 wailian999

C#:   块级作用域
来源：http://dnt.chenlongwang.top

[C11] 模块导入与导出
来源：http://qzp.nwbrower.top

Py:   from module import func
来源：http://vxk.ppjwa.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://uit.c1oappe.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://edz.haohaochexian.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ios.hesvh.cn

Java: import java.util.List;
来源：http://dtt.yj202588.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://okw.shzxlz.cn

Ruby: require "json"; require_relative "./util"
来源：http://lix.chenzaomai.com

C#:   using System.Text;
来源：http://rcf.jianghu66.top

[C12] 立即执行函数 IIFE
来源：http://cyh.yvedp.cn

Py:   (lambda: print("run"))()
来源：http://ouk.quarkkingdee.top

PHP:  (function () { echo "run"; })();
来源：http://dyc.yuanzhike.top

JS:   (() => { console.log("run"); })();
来源：http://odv.mhx1999.top

TS:   (() => { console.log("run"); })();
来源：http://xty.yj20258888.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://kbz.sjlbkw.cn

Go:   func() { fmt.Println("run") }()
来源：http://woh.snrcjt.cn

Ruby: -> { puts "run" }.call
来源：http://yhj.uphjek.com

C#:   // 无 IIFE：用静态构造函数
来源：http://mtl.sweek.top

[C13] 类型声明 / 类型注解
来源：http://lov.havefunace.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://boq.mhx1999.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dat.yuanzhike.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hsk.fehbvm.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://odz.xylfe.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ubs.pycfn.com

Go:   func add(a, b int) int
来源：http://njo.zhijiandao.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://txi.hcnkem.com

C#:   int Add(int a, int b) => a + b;
来源：http://rro.smart0.xyz

[C14] 泛型函数
来源：http://rst.ivvv.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://dot.yvedp.cn

PHP:  // 无泛型
来源：http://pbc.jinyuanbaomall.cn

JS:   // 无泛型
来源：http://uyn.yfazqb.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://zdc.gogol.net.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://cro.ehwqpu.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://sjl.zycfv.cn

Ruby: # 无泛型
来源：http://ros.bjfxy.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hbl.dianchejie.cn

[C15] 解构 / 展开参数
来源：http://tjv.zhaomingkeji.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://tet.nanxinkj.top

PHP:  [$a, $b] = $pair;
来源：http://qgs.chenjidiqi.icu

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ova.ctjpmb.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://qbk.0kj1m.cn

Java: // 无解构
来源：http://msv.sufxvd.cn

Go:   // 无解构
来源：http://kzh.xingfuxueyuan.xyz

Ruby: a, b = pair
来源：http://rer.zhaomingkeji.xyz

C#:   var (a, b) = pair;
来源：http://xem.52xcode.cn

[C16] 函数 / 方法重载
来源：http://lxl.yuxming.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://qhq.aizwys.cn

PHP:  // 无重载
来源：http://mxj.svipenyu.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://voh.xingfuxueyuan.xyz

TS:   // 用联合类型或重载签名声明
来源：http://lpb.jlsjyb.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://uqp.yueranfly.top

Go:   // 无重载：用不同函数名
来源：http://ltv.pycfn.com

Ruby: # 无重载：靠动态参数
来源：http://hfa.zhaomingkeji.xyz

C#:   void F(int a) {}  void F(string a) {}
来源：http://hss.sjlbkw.cn

================================================================================
来源：http://gyj.tian-w.cn

D. 数组 / 列表 / 集合
来源：http://yen.ydzc1.top

================================================================================
来源：http://tnd.zhiwuduotai.top

[D01] 创建数组 / 列表
来源：http://lrc.fehbvm.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://pns.yj20258888.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://vkc.yuxming.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://gnm.yj202588.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://pew.havefunace.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wgq.jiagoushi.top

Go:   arr := []int{1, 2, 3}
来源：http://irh.gaohongyu789.top

Ruby: arr = [1, 2, 3]
来源：http://ayn.hnxiangtu.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://qjp.bbcook.cn

[D02] 追加元素到末尾
来源：http://ika.sxryk.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wri.pengpengdd.cyou

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://szg.yj202588.top

JS:   arr.push(4);
来源：http://nfu.jinyuanbaomall.cn

TS:   arr.push(4);
来源：http://lmg.birdmap.top

Java: list.add(4);
来源：http://sqt.xuanzx.com

Go:   arr = append(arr, 4)
来源：http://gmz.sysykeji.top

Ruby: arr << 4; arr.push(5)
来源：http://pka.yuanzhike.top

C#:   list.Add(4);
来源：http://ehr.gogol.net.cn

[D03] 在指定位置插入元素
来源：http://eft.fanxiaobao.xyz

Py:   arr.insert(0, 0)
来源：http://ywo.uphjek.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://zxb.xingfuxueyuan.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://spz.guowangkeji.top

TS:   arr.splice(0, 0, 0);
来源：http://tke.iojbl.cn

Java: list.add(0, 0);
来源：http://myc.zhongyouzk.top

Go:   arr = append([]int{0}, arr...)
来源：http://tsj.hfpthk.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://oix.xuetiantiany.cn

C#:   list.Insert(0, 0);
来源：http://bju.vqdsnc.cn

[D04] 删除元素
来源：http://djc.xinyue.icu

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://njr.kuanghao11.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://upv.sjlbkw.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://omp.sxryk.cn

TS:   arr.splice(0, 1);
来源：http://uhq.chenlongwang.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://rse.feifeiyinyue.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://fxb.jinghuilouyu.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://lju.meibo888.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://jrf.yanxiufei.cn

[D05] 访问与修改元素
来源：http://zhp.zhixingplan.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://anq.vqdsnc.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://gdp.sysykeji.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://orj.jinyuanbaomall.cn

TS:   arr[0]; arr.at(-1);
来源：http://xti.epnwcf.com

Java: list.get(0); list.set(0, 9);
来源：http://rjx.chenzaomai.com

Go:   arr[0]; arr[0] = 9
来源：http://wpo.kuanghao11.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://pig.sjlbkw.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ihy.tarul.cn

[D06] 数组长度
来源：http://bbj.xuetiantiany.cn

Py:   len(arr)
来源：http://kld.nanxinkj.top

PHP:  count($arr);
来源：http://obx.zhoulong.xyz

JS:   arr.length
来源：http://ldb.vqdsnc.cn

TS:   arr.length
来源：http://oaf.yangfankeji.com

Java: list.size();
来源：http://nwf.sweek.top

Go:   len(arr)
来源：http://dnp.jianghu66.top

Ruby: arr.length; arr.size
来源：http://dva.jiagoushi.top

C#:   list.Count;
来源：http://pbv.gotoacloud.top

[D07] 切片 / 取子数组
来源：http://egz.hysaishi.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hod.snrcjt.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ddt.ydjk.org.cn

JS:   arr.slice(1, 4);
来源：http://bfj.haohaochexian.top

TS:   arr.slice(1, 4);
来源：http://mqn.cucudq.cn

Java: list.subList(1, 4);
来源：http://djx.zdbjq.cn

Go:   arr[1:4]
来源：http://gmd.c1oappe.top

Ruby: arr[1, 3]
来源：http://lay.ywan-chungtsiang.top

C#:   list.GetRange(1, 3);
来源：http://jwl.hysaishi.cn

[D08] 合并两个数组
来源：http://jkb.yangfankeji.com

Py:   a + b;  a.extend(b)
来源：http://qpj.redwolf501.top

PHP:  array_merge($a, $b);
来源：http://smf.cqqwz.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ifq.52xcode.cn

TS:   [...a, ...b];
来源：http://ote.daria6918.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://jou.yfazqb.com

Go:   append(a, b...)
来源：http://kqg.sysykeji.top

Ruby: a + b;  a.concat(b)
来源：http://gte.jlsjyb.cn

C#:   a.Concat(b).ToList()
来源：http://dup.tianlin.xyz

[D09] 排序（升序）
来源：http://lfg.sxryk.cn

Py:   sorted(arr);  arr.sort()
来源：http://ucx.nanxuanxn.top

PHP:  sort($arr);
来源：http://qxh.xinyue.icu

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://cde.xylfe.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://giv.nanxinkj.top

Java: Collections.sort(list);  list.sort(null);
来源：http://jha.zhiwuduotai.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://dho.316326.xyz

Ruby: arr.sort
来源：http://uyo.cashguo.top

C#:   list.Sort();
来源：http://qam.tian-w.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://xad.quarkkingdee.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://pga.wangshuangyany.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qzw.hysaishi.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://zxu.havefunace.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://dhl.gogol.net.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://eqi.daxiang520.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ebz.zdbjq.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ymo.xingfuxueyuan.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://gso.snrcjt.cn

[D11] 反转数组
来源：http://hvc.jinyuanbaomall.cn

Py:   arr[::-1];  arr.reverse()
来源：http://elf.pycfn.com

PHP:  array_reverse($arr);
来源：http://ebj.yfazqb.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qbc.jyoumei.cn

TS:   [...arr].reverse();
来源：http://ohg.sweek.top

Java: Collections.reverse(list);
来源：http://pfh.ydzc1.top

Go:   slices.Reverse(arr)
来源：http://yov.aizwys.cn

Ruby: arr.reverse
来源：http://fxh.jinyuanbaomall.cn

C#:   list.Reverse();
来源：http://ajc.quarkkingdee.top

[D12] 查找元素下标
来源：http://mue.iojbl.cn

Py:   arr.index(x);  x in arr
来源：http://bba.kuanghao11.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wjv.yvedp.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://idh.hywenlv.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ytn.zhongyouzk.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://yai.zhongyouzk.top

Go:   slices.Index(arr, x)
来源：http://ayk.cucudq.cn

Ruby: arr.index(x)
来源：http://iko.yfazqb.com

C#:   list.IndexOf(x);
来源：http://rmr.yanxiufei.cn

[D13] 过滤（保留满足条件的）
来源：http://aer.pycfn.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://lgn.snrcjt.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://eun.hysaishi.cn

JS:   arr.filter(x => x > 3)
来源：http://ccb.shzxlz.cn

TS:   arr.filter(x => x > 3)
来源：http://mtk.52xcode.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ilv.316326.xyz

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://llx.wangdashe.top

Ruby: arr.select { |x| x > 3 }
来源：http://gas.ybcxt.top

C#:   list.Where(x => x > 3).ToList()
来源：http://eub.feifeiyinyue.top

[D14] 映射转换（每个元素变形）
来源：http://avm.cashguo.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://lnh.cucudq.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vgq.hfpthk.cn

JS:   arr.map(x => x * 2)
来源：http://bvc.hammf.cn

TS:   arr.map(x => x * 2)
来源：http://cbe.jlsjyb.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://tlw.gzhubu.top

Go:   // 手写循环
来源：http://lbd.aizwys.cn

Ruby: arr.map { |x| x * 2 }
来源：http://fzq.tarul.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://qho.gaohongyu789.top

[D15] 去重
来源：http://ctn.jinqigufen.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://uei.xziqi.cn

PHP:  array_unique($arr);
来源：http://wlj.yfazqb.com

JS:   [...new Set(arr)]
来源：http://zov.fehbvm.com

TS:   [...new Set(arr)]
来源：http://oxz.xylfe.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://oya.bbcook.cn

Go:   // 用 map[T]struct{} 手写
来源：http://rgw.jinqigfzy.top

Ruby: arr.uniq
来源：http://zgv.cashguo.top

C#:   list.Distinct().ToList()
来源：http://llf.pycfn.com

[D16] 求和与平均值
来源：http://qqk.redwolf501.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://koa.yj202588.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ktx.xinyue.icu

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ujq.yuanzhike.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ebz.ybcxt.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://yjk.yj20258888.top

Go:   // 手写循环累加
来源：http://tjl.nwbrower.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://aqf.smart0.xyz

C#:   list.Sum();  list.Average()
来源：http://clr.hammf.cn

[D17] 最大值与最小值
来源：http://pxz.epnwcf.com

Py:   max(arr);  min(arr)
来源：http://kqy.hesvh.cn

PHP:  max($arr);  min($arr);
来源：http://zou.jiagoushi.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ztk.fengsongda.top

TS:   Math.max(...arr);
来源：http://tos.xuanzx.com

Java: Collections.max(list);  Collections.min(list);
来源：http://ohv.hesvh.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ptl.tian-w.cn

Ruby: arr.max;  arr.min
来源：http://wej.hammf.cn

C#:   list.Max();  list.Min()
来源：http://uqa.tianlin.xyz

[D18] 扁平化嵌套数组
来源：http://owm.hnxiangtu.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://gee.wangdashe.top

PHP:  array_merge(...$nested);
来源：http://coc.chenjidiqi.icu

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mul.andypj.xyz

TS:   nested.flat();
来源：http://rmp.chenjidiqi.icu

Java: nested.stream().flatMap(List::stream).toList()
来源：http://bci.cheryme.top

Go:   // 手写双层循环
来源：http://mav.fktsv.cn

Ruby: nested.flatten
来源：http://teq.jlsjyb.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://bfq.xingfuxueyuan.xyz

[D19] 按字段分组
来源：http://vir.jinqigfzy.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://jww.iojbl.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://sjg.xylfe.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hgw.uphjek.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://chc.9152youxi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://lvv.sysykeji.top

Go:   // 手写 map[string][]T
来源：http://rdp.yuxming.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://wzq.gzhubu.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ggt.jinqigufen.top

[D20] 统计每个元素出现次数
来源：http://lwb.shuidangran.top

Py:   Counter(arr)
来源：http://ctr.ivvv.top

PHP:  array_count_values($arr);
来源：http://nqx.zhengqikj.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kom.cdnleiting.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://oqy.wangdashe.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wqb.daria6918.cn

Go:   // 手写 map[T]int
来源：http://som.dianchejie.cn

Ruby: arr.tally
来源：http://spm.wangdashe.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://rpr.ehwqpu.com

[D21] 判断是否包含某元素
来源：http://gxn.zhijiandao.cn

Py:   x in arr
来源：http://xsp.sxryk.cn

PHP:  in_array($x, $arr, true);
来源：http://wst.zhijiandao.cn

JS:   arr.includes(x)
来源：http://nvq.mhx1999.top

TS:   arr.includes(x)
来源：http://hni.xylfe.cn

Java: list.contains(x)
来源：http://hdx.jqgfzy.top

Go:   slices.Contains(arr, x)
来源：http://png.ivvv.top

Ruby: arr.include?(x)
来源：http://rql.cheryme.top

C#:   list.Contains(x)
来源：http://vaf.cdnleiting.top

[D22] 复制数组（避免共享引用）
来源：http://mju.hammf.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://slr.bjfxy.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://fog.shangyingyoupin.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://rsj.hammf.cn

TS:   [...arr];
来源：http://xpm.yanxiufei.cn

Java: new ArrayList<>(list);
来源：http://chh.iojbl.cn

Go:   copied := append([]int(nil), arr...)
来源：http://gph.yonumen.top

Ruby: arr.dup;  arr.clone
来源：http://gsa.gogol.net.cn

C#:   new List<int>(list);
来源：http://hoo.wangshuangyany.cn

[D23] reduce 累积计算
来源：http://giu.andypj.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://cpr.birdmap.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://vhl.chenzaomai.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ark.ydjk.org.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gju.yj20258.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://jar.yj20258888.top

Go:   // 手写循环
来源：http://rqp.zhaomingkeji.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://obe.shanyushiyangkeji.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://bwx.jianghu66.top

[D24] 字典 / Map 基本操作
来源：http://adq.nwbrower.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://jxv.guannengcc.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://jxh.nanxinkj.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ppc.9152youxi.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ugi.tianlin.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://oxb.yuanzhike.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://buz.zycfv.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://gca.yfazqb.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://gcv.ydzc1.top

[D25] Set 集合去重与交并差
来源：http://xqi.shanyushiyangkeji.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://tdx.epnwcf.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://frl.wangshuangyany.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://yyk.fanxiaobao.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://itn.nanxinkj.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://clx.xziqi.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wqq.zhoulong.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ljp.xuetiantiany.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://tap.xingfuxueyuan.xyz

[D26] 数组转字符串
来源：http://qwu.316326.xyz

Py:   ", ".join(map(str, arr))
来源：http://vxp.yj202588.top

PHP:  implode(", ", $arr);
来源：http://jxg.xylfe.cn

JS:   arr.join(", ")
来源：http://tna.jinqigufen.top

TS:   arr.join(", ")
来源：http://jzc.zhixingplan.top

Java: String.join(", ", list)
来源：http://vdi.dianchejie.cn

Go:   strings.Join(strs, ", ")
来源：http://cnf.yueranfly.top

Ruby: arr.join(", ")
来源：http://ndu.ydjk.org.cn

C#:   string.Join(", ", list)
来源：http://bif.fanxiaobao.xyz

================================================================================
来源：http://ift.iojbl.cn

E. 字符串处理
来源：http://byn.fzhhl.top

================================================================================
来源：http://kdg.fktsv.cn

[E01] 拼接字符串
来源：http://zmy.chenzaomai.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://gtq.fengsongda.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mgv.0kj1m.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://gyc.chenjidiqi.icu

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://rsw.chenzaomai.com


<!-- 参考信息 -->