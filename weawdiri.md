代发 wailian999

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wle.cucudq.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://iph.cheryme.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://qec.hongshengwenyu.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://orv.tianlin.xyz

[C10] 变量作用域
来源：http://ron.chenzaomai.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qzt.shzxlz.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://yhy.fengsongda.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mky.havefunace.top

TS:   同 JS
来源：http://pde.ivvv.top

Java: 方法内为块级作用域
来源：http://oys.sjlbkw.cn

Go:   花括号块级作用域
来源：http://fpp.xingfuxueyuan.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://rso.cucudq.cn

C#:   块级作用域
来源：http://dif.zhixingplan.top

[C11] 模块导入与导出
来源：http://mqw.hongshengwenyu.top

Py:   from module import func
来源：http://vjl.zycfv.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ocv.0kj1m.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://uns.zhijiandao.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://stp.fzhhl.top

Java: import java.util.List;
来源：http://ffk.ydzc1.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://pzl.hammf.cn

Ruby: require "json"; require_relative "./util"
来源：http://mon.sufxvd.cn

C#:   using System.Text;
来源：http://ppf.xuetiantiany.cn

[C12] 立即执行函数 IIFE
来源：http://ydr.zycfv.cn

Py:   (lambda: print("run"))()
来源：http://mgk.hammf.cn

PHP:  (function () { echo "run"; })();
来源：http://adi.wangshuangyany.cn

JS:   (() => { console.log("run"); })();
来源：http://ehe.uphjek.com

TS:   (() => { console.log("run"); })();
来源：http://vye.yuanzhike.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jse.ywan-chungtsiang.top

Go:   func() { fmt.Println("run") }()
来源：http://emu.yonumen.top

Ruby: -> { puts "run" }.call
来源：http://ndm.daxiang520.top

C#:   // 无 IIFE：用静态构造函数
来源：http://blj.sufxvd.cn

[C13] 类型声明 / 类型注解
来源：http://qpf.hcnkem.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://eex.gotoacloud.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zvp.aibaodan.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://rvf.uphjek.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gns.quarkkingdee.top

Java: int add(int a, int b) { return a + b; }
来源：http://unv.fehbvm.com

Go:   func add(a, b int) int
来源：http://gmg.dianchejie.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://and.tian-w.cn

C#:   int Add(int a, int b) => a + b;
来源：http://frk.c1oappe.top

[C14] 泛型函数
来源：http://rkx.nanxuanxn.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://fpd.pycfn.com

PHP:  // 无泛型
来源：http://ymx.jinghuilouyu.cn

JS:   // 无泛型
来源：http://zoo.sxryk.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://lty.ppjwa.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://idl.ybcxt.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://vxv.daria6918.cn

Ruby: # 无泛型
来源：http://sov.gzhubu.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://eij.iojbl.cn

[C15] 解构 / 展开参数
来源：http://iom.9152youxi.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://plm.fanxiaobao.xyz

PHP:  [$a, $b] = $pair;
来源：http://idv.xingfuxueyuan.xyz

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hib.uphjek.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://woa.dashuyun.cn

Java: // 无解构
来源：http://cky.xziqi.cn

Go:   // 无解构
来源：http://pil.gaohongyu789.top

Ruby: a, b = pair
来源：http://nuc.xziqi.cn

C#:   var (a, b) = pair;
来源：http://qoq.xuetiantiany.cn

[C16] 函数 / 方法重载
来源：http://lom.gogol.net.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://otw.ppjwa.cn

PHP:  // 无重载
来源：http://nri.redwolf501.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://iue.0kj1m.cn

TS:   // 用联合类型或重载签名声明
来源：http://adq.feifeiyinyue.top

Java: void f(int a) {}  void f(String a) {}
来源：http://uuh.fengsongda.top

Go:   // 无重载：用不同函数名
来源：http://cpr.ydjk.org.cn

Ruby: # 无重载：靠动态参数
来源：http://rhc.cucudq.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://kmp.yangfankeji.com

================================================================================
来源：http://xld.cheryme.top

D. 数组 / 列表 / 集合
来源：http://apk.jianghu66.top

================================================================================
来源：http://oqh.jianghu66.top

[D01] 创建数组 / 列表
来源：http://los.chenzaomai.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://rlz.zdbjq.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://gay.gzhubu.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://zdf.hysaishi.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ltr.guannengcc.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hht.cashguo.top

Go:   arr := []int{1, 2, 3}
来源：http://mfq.shuidangran.top

Ruby: arr = [1, 2, 3]
来源：http://kym.wangdashe.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://egv.hesvh.cn

[D02] 追加元素到末尾
来源：http://vug.svipenyu.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://pmf.chenlongwang.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://poc.jinqigufen.top

JS:   arr.push(4);
来源：http://ssy.tanke756.top

TS:   arr.push(4);
来源：http://swq.hnxiangtu.top

Java: list.add(4);
来源：http://pvu.sjlbkw.cn

Go:   arr = append(arr, 4)
来源：http://cgc.jyoumei.cn

Ruby: arr << 4; arr.push(5)
来源：http://qps.dianchejie.cn

C#:   list.Add(4);
来源：http://wav.hcnkem.com

[D03] 在指定位置插入元素
来源：http://jdi.tianlin.xyz

Py:   arr.insert(0, 0)
来源：http://tii.xuetiantiany.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://cvw.wangdashe.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://voo.tianlin.xyz

TS:   arr.splice(0, 0, 0);
来源：http://xsw.fktsv.cn

Java: list.add(0, 0);
来源：http://hht.gaohongyu789.top

Go:   arr = append([]int{0}, arr...)
来源：http://fcz.xingfuxueyuan.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://qbm.hywenlv.cn

C#:   list.Insert(0, 0);
来源：http://dep.ctjpmb.com

[D04] 删除元素
来源：http://xgw.wangdashe.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://uyt.yonumen.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://xfv.zhoulong.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://yfn.shanyushiyangtech.top

TS:   arr.splice(0, 1);
来源：http://ext.daria6918.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wqc.zhongyouzk.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://pxz.hcnkem.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://dfn.yfazqb.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://faz.ppjwa.cn

[D05] 访问与修改元素
来源：http://ohb.uphjek.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://dxy.ivvv.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://zjw.yj20258.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://dhl.fanxiaobao.xyz

TS:   arr[0]; arr.at(-1);
来源：http://ked.jinqigfzy.top

Java: list.get(0); list.set(0, 9);
来源：http://dbq.tarul.cn

Go:   arr[0]; arr[0] = 9
来源：http://txu.c1oappe.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://tml.epnwcf.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ezt.hnxiangtu.top

[D06] 数组长度
来源：http://buw.tanke756.top

Py:   len(arr)
来源：http://ufr.chenzaomai.com

PHP:  count($arr);
来源：http://nyt.guowangkeji.top

JS:   arr.length
来源：http://stf.jinqigfzy.top

TS:   arr.length
来源：http://ozg.zdqjudy.top

Java: list.size();
来源：http://plz.havefunace.top

Go:   len(arr)
来源：http://vjd.meibo888.top

Ruby: arr.length; arr.size
来源：http://eeu.tarul.cn

C#:   list.Count;
来源：http://hif.nanxinkj.top

[D07] 切片 / 取子数组
来源：http://sob.vehdjk.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qcc.hcnkem.com

PHP:  array_slice($arr, 1, 3);
来源：http://zbq.wangdashe.top

JS:   arr.slice(1, 4);
来源：http://lfh.tianlin.xyz

TS:   arr.slice(1, 4);
来源：http://uqb.52xcode.cn

Java: list.subList(1, 4);
来源：http://xer.c1oappe.top

Go:   arr[1:4]
来源：http://rom.gzhubu.top

Ruby: arr[1, 3]
来源：http://zzu.hongshengwenyu.top

C#:   list.GetRange(1, 3);
来源：http://kug.dashuyun.cn

[D08] 合并两个数组
来源：http://moi.meibo888.top

Py:   a + b;  a.extend(b)
来源：http://xzz.ctjpmb.com

PHP:  array_merge($a, $b);
来源：http://knl.tian-w.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://eel.wangshuangyany.cn

TS:   [...a, ...b];
来源：http://ogh.guowangkeji.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://xlr.epnwcf.com

Go:   append(a, b...)
来源：http://kyu.jqgfzy.top

Ruby: a + b;  a.concat(b)
来源：http://eki.xziqi.cn

C#:   a.Concat(b).ToList()
来源：http://caa.ivvv.top

[D09] 排序（升序）
来源：http://buw.havefunace.top

Py:   sorted(arr);  arr.sort()
来源：http://vtx.gaohongyu789.top

PHP:  sort($arr);
来源：http://tuy.cashguo.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ouh.fktsv.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://htn.sjlbkw.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://jix.yuxming.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://kga.feifeiyinyue.top

Ruby: arr.sort
来源：http://mpt.zycfv.cn

C#:   list.Sort();
来源：http://blg.hcnkem.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://mae.zhoulong.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://jel.birdmap.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pof.9152youxi.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://upl.shanyushiyangtech.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://zte.vqdsnc.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://jvj.bbcook.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://qdy.pengpengdd.cyou

Ruby: arr.sort_by { |x| x[:age] }
来源：http://toy.epnwcf.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ydr.nanxinkj.top

[D11] 反转数组
来源：http://pmn.cqqwz.cn

Py:   arr[::-1];  arr.reverse()
来源：http://yyj.chenzaomai.com

PHP:  array_reverse($arr);
来源：http://nbd.chenlongwang.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ams.zhixingplan.top

TS:   [...arr].reverse();
来源：http://sbp.cdnleiting.top

Java: Collections.reverse(list);
来源：http://dkq.guannengcc.top

Go:   slices.Reverse(arr)
来源：http://ufk.yonumen.top

Ruby: arr.reverse
来源：http://wfg.52xcode.cn

C#:   list.Reverse();
来源：http://rtf.quarkkingdee.top

[D12] 查找元素下标
来源：http://dwa.zhijiandao.cn

Py:   arr.index(x);  x in arr
来源：http://xlq.gaohongyu789.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://rty.nanxuanxn.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fmq.snrcjt.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://imm.vqdsnc.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wtf.gogol.net.cn

Go:   slices.Index(arr, x)
来源：http://bml.shangyingyoupin.top

Ruby: arr.index(x)
来源：http://qtl.jyoumei.cn

C#:   list.IndexOf(x);
来源：http://xpj.kuanghao11.cn

[D13] 过滤（保留满足条件的）
来源：http://bok.jinghuilouyu.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://oye.hywenlv.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ntw.iojbl.cn

JS:   arr.filter(x => x > 3)
来源：http://xzs.yongpay.top

TS:   arr.filter(x => x > 3)
来源：http://iqw.bbcook.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://rip.nanxinkj.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ahm.tian-w.cn

Ruby: arr.select { |x| x > 3 }
来源：http://kmr.ctjpmb.com

C#:   list.Where(x => x > 3).ToList()
来源：http://icy.zhoulong.xyz

[D14] 映射转换（每个元素变形）
来源：http://dnu.jinyuanbaomall.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://bta.dashuyun.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://iet.bbcook.cn

JS:   arr.map(x => x * 2)
来源：http://ezo.feifeiyinyue.top

TS:   arr.map(x => x * 2)
来源：http://aah.bbcook.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://xtd.yongpay.top

Go:   // 手写循环
来源：http://dmx.kuanghao11.cn

Ruby: arr.map { |x| x * 2 }
来源：http://lvu.feifeiyinyue.top

C#:   list.Select(x => x * 2).ToList()
来源：http://wxh.xylfe.cn

[D15] 去重
来源：http://jdw.mhx1999.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ngm.yangfankeji.com

PHP:  array_unique($arr);
来源：http://lwe.ppjwa.cn

JS:   [...new Set(arr)]
来源：http://oju.jinqigfzy.top

TS:   [...new Set(arr)]
来源：http://qvf.bjfxy.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://vfr.ctjpmb.com

Go:   // 用 map[T]struct{} 手写
来源：http://jzg.chenzaomai.com

Ruby: arr.uniq
来源：http://xnn.gaohongyu789.top

C#:   list.Distinct().ToList()
来源：http://tpx.hfpthk.cn

[D16] 求和与平均值
来源：http://xzq.shangyingyoupin.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://yce.gzhubu.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wos.birdmap.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://kuf.yj202588.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://bgq.chenzaomai.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xmr.jqgufenzy.top

Go:   // 手写循环累加
来源：http://wac.xinyue.icu

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://dzu.dianchejie.cn

C#:   list.Sum();  list.Average()
来源：http://tmu.fktsv.cn

[D17] 最大值与最小值
来源：http://vyt.zhengqikj.top

Py:   max(arr);  min(arr)
来源：http://igv.ydjk.org.cn

PHP:  max($arr);  min($arr);
来源：http://ist.jqgufenzy.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://rdi.hnqzz.top

TS:   Math.max(...arr);
来源：http://tgw.pengpengdd.cyou

Java: Collections.max(list);  Collections.min(list);
来源：http://vyp.sweek.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://gnu.cheryme.top

Ruby: arr.max;  arr.min
来源：http://qyy.zhixingplan.top

C#:   list.Max();  list.Min()
来源：http://bte.zycfv.cn

[D18] 扁平化嵌套数组
来源：http://isa.feifeiyinyue.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ink.jqgfzy.top

PHP:  array_merge(...$nested);
来源：http://max.nanxinkj.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ocd.gogol.net.cn

TS:   nested.flat();
来源：http://rhe.cheryme.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://puo.kuanghao11.cn

Go:   // 手写双层循环
来源：http://vky.guowangkeji.top

Ruby: nested.flatten
来源：http://uvd.gotoacloud.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://vck.jinqigufen.top

[D19] 按字段分组
来源：http://odu.pycfn.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://onf.ybcxt.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://sfc.andypj.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://jjb.xylfe.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://peq.uphjek.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://dhd.nanxinkj.top

Go:   // 手写 map[string][]T
来源：http://xxk.yueranfly.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://evt.xinyue.icu

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://vit.aibaodan.cn

[D20] 统计每个元素出现次数
来源：http://zkd.fanxiaobao.xyz

Py:   Counter(arr)
来源：http://fxd.zhaomingkeji.xyz

PHP:  array_count_values($arr);
来源：http://pqf.xuanzx.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ctd.xingfuxueyuan.xyz

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lpj.chenzaomai.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ynq.dashuyun.cn

Go:   // 手写 map[T]int
来源：http://rfr.pycfn.com

Ruby: arr.tally
来源：http://vlx.bbcook.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://cds.sufxvd.cn

[D21] 判断是否包含某元素
来源：http://yrc.jinghuilouyu.cn

Py:   x in arr
来源：http://jdb.zhijiandao.cn

PHP:  in_array($x, $arr, true);
来源：http://xxd.zhongyouzk.top

JS:   arr.includes(x)
来源：http://ext.gotoacloud.top

TS:   arr.includes(x)
来源：http://xzi.fengsongda.top

Java: list.contains(x)
来源：http://bub.vehdjk.com

Go:   slices.Contains(arr, x)
来源：http://jpw.gaohongyu789.top

Ruby: arr.include?(x)
来源：http://vxo.fanxiaobao.xyz

C#:   list.Contains(x)
来源：http://aqy.andypj.xyz

[D22] 复制数组（避免共享引用）
来源：http://amn.jiagoushi.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wfy.xingfuxueyuan.xyz

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://irj.ctjpmb.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://uvb.haohaochexian.top

TS:   [...arr];
来源：http://vjv.gotoacloud.top

Java: new ArrayList<>(list);
来源：http://oij.yueranfly.top

Go:   copied := append([]int(nil), arr...)
来源：http://udo.yanxiufei.cn

Ruby: arr.dup;  arr.clone
来源：http://nyc.jiagoushi.top

C#:   new List<int>(list);
来源：http://gav.cqqwz.cn

[D23] reduce 累积计算
来源：http://tff.aizwys.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zek.hnxiangtu.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://uvd.sufxvd.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pdq.meibo888.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ann.yfazqb.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://jtc.yueranfly.top

Go:   // 手写循环
来源：http://uhd.c1oappe.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://vsp.yvedp.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://itm.sxryk.cn

[D24] 字典 / Map 基本操作
来源：http://big.shzxlz.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://rdx.xuanzx.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://gut.cashguo.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xdl.c1oappe.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://xdd.sxryk.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://pkp.sufxvd.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://fse.sufxvd.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://jzy.tanke756.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ojz.wangdashe.top

[D25] Set 集合去重与交并差
来源：http://eqy.birdmap.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mfj.jlsjyb.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://sas.hesvh.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ogs.yuanzhike.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://lal.tanke756.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dre.vehdjk.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://miz.cheryme.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://tzs.yuanzhike.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://gis.hongshengwenyu.top

[D26] 数组转字符串
来源：http://clb.jiagoushi.top

Py:   ", ".join(map(str, arr))
来源：http://xbm.daria6918.cn

PHP:  implode(", ", $arr);
来源：http://xeo.shangyingyoupin.top

JS:   arr.join(", ")
来源：http://wgl.yj20258.top

TS:   arr.join(", ")
来源：http://wtz.hysaishi.cn


<!-- 参考信息 -->