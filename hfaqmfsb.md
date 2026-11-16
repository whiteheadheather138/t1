代发 wailian999

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://gdd.sweek.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hgg.iojbl.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ave.daria6918.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tgf.52xcode.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://gnd.shzxlz.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://xcz.wangshuangyany.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://tdd.sysykeji.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://jjt.hammf.cn

[C10] 变量作用域
来源：http://mmf.chenjidiqi.icu

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hus.ydzc1.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://bjv.sysykeji.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://vma.gzhubu.top

TS:   同 JS
来源：http://iwk.zhongyouzk.top

Java: 方法内为块级作用域
来源：http://kna.cqqwz.cn

Go:   花括号块级作用域
来源：http://skt.ehwqpu.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://lto.vehdjk.com

C#:   块级作用域
来源：http://slw.pycfn.com

[C11] 模块导入与导出
来源：http://cxp.daxiang520.top

Py:   from module import func
来源：http://tcq.yvedp.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://kum.cheryme.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://cfh.hcnkem.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ans.ybcxt.top

Java: import java.util.List;
来源：http://ikr.vehdjk.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wua.hnxiangtu.top

Ruby: require "json"; require_relative "./util"
来源：http://pcj.xuetiantiany.cn

C#:   using System.Text;
来源：http://awr.kuanghao11.cn

[C12] 立即执行函数 IIFE
来源：http://ray.hysaishi.cn

Py:   (lambda: print("run"))()
来源：http://ehs.yanxiufei.cn

PHP:  (function () { echo "run"; })();
来源：http://zrk.smart0.xyz

JS:   (() => { console.log("run"); })();
来源：http://vyc.fanxiaobao.xyz

TS:   (() => { console.log("run"); })();
来源：http://snw.shuidangran.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mjq.xuetiantiany.cn

Go:   func() { fmt.Println("run") }()
来源：http://kst.jinyuanbaomall.cn

Ruby: -> { puts "run" }.call
来源：http://jcj.yvedp.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://mwi.guannengcc.top

[C13] 类型声明 / 类型注解
来源：http://jfy.sweek.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://tky.haohaochexian.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bzc.xziqi.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://olg.gogol.net.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fpx.bbcook.cn

Java: int add(int a, int b) { return a + b; }
来源：http://uqe.shangyingyoupin.top

Go:   func add(a, b int) int
来源：http://rit.guannengcc.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ytd.xuetiantiany.cn

C#:   int Add(int a, int b) => a + b;
来源：http://blz.uphjek.com

[C14] 泛型函数
来源：http://gmf.iojbl.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://laz.zhijiandao.cn

PHP:  // 无泛型
来源：http://pgd.c1oappe.top

JS:   // 无泛型
来源：http://mfk.ivvv.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://aef.chenjidiqi.icu

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://fha.ydzc1.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://rmb.sweek.top

Ruby: # 无泛型
来源：http://tkl.svipenyu.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://jgm.jqgufenzy.top

[C15] 解构 / 展开参数
来源：http://kyz.jinghuilouyu.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xqc.guowangkeji.top

PHP:  [$a, $b] = $pair;
来源：http://mwl.jqgufenzy.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://fuv.xylfe.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://jkc.9152youxi.cn

Java: // 无解构
来源：http://zxu.vqdsnc.cn

Go:   // 无解构
来源：http://atf.dashuyun.cn

Ruby: a, b = pair
来源：http://bse.zhongyouzk.top

C#:   var (a, b) = pair;
来源：http://znd.chenzaomai.com

[C16] 函数 / 方法重载
来源：http://brw.yueranfly.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://zsk.jianghu66.top

PHP:  // 无重载
来源：http://xtq.jinghuilouyu.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://jsq.xylfe.cn

TS:   // 用联合类型或重载签名声明
来源：http://olf.snrcjt.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://eji.fengsongda.top

Go:   // 无重载：用不同函数名
来源：http://nkl.xinyue.icu

Ruby: # 无重载：靠动态参数
来源：http://hpp.xingfuxueyuan.xyz

C#:   void F(int a) {}  void F(string a) {}
来源：http://rgh.jinghuilouyu.cn

================================================================================
来源：http://xva.zhengqikj.top

D. 数组 / 列表 / 集合
来源：http://alb.yvedp.cn

================================================================================
来源：http://jgv.jianghu66.top

[D01] 创建数组 / 列表
来源：http://qgb.yj20258.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://muk.vqdsnc.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://voe.jinghuilouyu.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://uaf.mhx1999.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://fhh.sysykeji.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://xlf.hysaishi.cn

Go:   arr := []int{1, 2, 3}
来源：http://uhf.chenlongwang.top

Ruby: arr = [1, 2, 3]
来源：http://knt.haohaochexian.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ikb.shuidangran.top

[D02] 追加元素到末尾
来源：http://ekd.fanxiaobao.xyz

Py:   arr.append(4); arr.extend([5, 6])
来源：http://iod.feifeiyinyue.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ppc.gotoacloud.top

JS:   arr.push(4);
来源：http://wpb.bbcook.cn

TS:   arr.push(4);
来源：http://byh.mhx1999.top

Java: list.add(4);
来源：http://vle.shanyushiyangkeji.top

Go:   arr = append(arr, 4)
来源：http://ihj.hnqzz.top

Ruby: arr << 4; arr.push(5)
来源：http://skc.tian-w.cn

C#:   list.Add(4);
来源：http://sze.xuetiantiany.cn

[D03] 在指定位置插入元素
来源：http://eop.gotoacloud.top

Py:   arr.insert(0, 0)
来源：http://npt.sjlbkw.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://tkk.ivvv.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://kwv.shanyushiyangtech.top

TS:   arr.splice(0, 0, 0);
来源：http://gay.gaohongyu789.top

Java: list.add(0, 0);
来源：http://tyj.yonumen.top

Go:   arr = append([]int{0}, arr...)
来源：http://hre.hcnkem.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wix.wangdashe.top

C#:   list.Insert(0, 0);
来源：http://ywc.ehwqpu.com

[D04] 删除元素
来源：http://fcu.xinyue.icu

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://kfd.epnwcf.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://xml.nwbrower.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://dhu.jinqigfzy.top

TS:   arr.splice(0, 1);
来源：http://lku.mhx1999.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://zse.9152youxi.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ssg.jinqigfzy.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ngl.cashguo.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://gll.feifeiyinyue.top

[D05] 访问与修改元素
来源：http://pct.daxiang520.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ccw.guannengcc.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://tek.cqqwz.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://dgh.chenjidiqi.icu

TS:   arr[0]; arr.at(-1);
来源：http://axm.yj202588.top

Java: list.get(0); list.set(0, 9);
来源：http://ydp.dianchejie.cn

Go:   arr[0]; arr[0] = 9
来源：http://thj.gzhubu.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://sra.epnwcf.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zvp.feifeiyinyue.top

[D06] 数组长度
来源：http://kvj.ybcxt.top

Py:   len(arr)
来源：http://rxe.xziqi.cn

PHP:  count($arr);
来源：http://lff.gzhubu.top

JS:   arr.length
来源：http://zhq.smart0.xyz

TS:   arr.length
来源：http://snx.gzhubu.top

Java: list.size();
来源：http://rij.yuxming.cn

Go:   len(arr)
来源：http://cap.cheryme.top

Ruby: arr.length; arr.size
来源：http://flv.316326.xyz

C#:   list.Count;
来源：http://rmz.jinqigufen.top

[D07] 切片 / 取子数组
来源：http://lof.hcnkem.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wpi.epnwcf.com

PHP:  array_slice($arr, 1, 3);
来源：http://lgn.shzxlz.cn

JS:   arr.slice(1, 4);
来源：http://gof.aibaodan.cn

TS:   arr.slice(1, 4);
来源：http://tmg.jqgfzy.top

Java: list.subList(1, 4);
来源：http://otk.shzxlz.cn

Go:   arr[1:4]
来源：http://rby.jinqigufen.top

Ruby: arr[1, 3]
来源：http://ipt.ppjwa.cn

C#:   list.GetRange(1, 3);
来源：http://jjz.jinqigfzy.top

[D08] 合并两个数组
来源：http://xmx.shanyushiyangkeji.top

Py:   a + b;  a.extend(b)
来源：http://qtj.quarkkingdee.top

PHP:  array_merge($a, $b);
来源：http://sic.jinghuilouyu.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://oiq.zhengqikj.top

TS:   [...a, ...b];
来源：http://lhi.redwolf501.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://csl.9152youxi.cn

Go:   append(a, b...)
来源：http://tux.shanyushiyangkeji.top

Ruby: a + b;  a.concat(b)
来源：http://yis.sxryk.cn

C#:   a.Concat(b).ToList()
来源：http://arz.jianghu66.top

[D09] 排序（升序）
来源：http://xhh.cashguo.top

Py:   sorted(arr);  arr.sort()
来源：http://hst.hywenlv.cn

PHP:  sort($arr);
来源：http://cua.jqgufenzy.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://dsp.cashguo.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://gad.ctjpmb.com

Java: Collections.sort(list);  list.sort(null);
来源：http://rqv.yvedp.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://zqh.jinqigfzy.top

Ruby: arr.sort
来源：http://klw.cucudq.cn

C#:   list.Sort();
来源：http://kqe.yonumen.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://jui.jiagoushi.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://zzc.xuetiantiany.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jsh.fengsongda.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ggx.c1oappe.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://odc.bjfxy.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://adk.bbcook.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ydl.yj202588.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://giy.jlsjyb.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://oet.316326.xyz

[D11] 反转数组
来源：http://fyc.cqqwz.cn

Py:   arr[::-1];  arr.reverse()
来源：http://xru.kuanghao11.cn

PHP:  array_reverse($arr);
来源：http://mar.fanxiaobao.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mvp.hammf.cn

TS:   [...arr].reverse();
来源：http://cku.zycfv.cn

Java: Collections.reverse(list);
来源：http://vba.yvedp.cn

Go:   slices.Reverse(arr)
来源：http://lsr.hnxiangtu.top

Ruby: arr.reverse
来源：http://cgn.zhixingplan.top

C#:   list.Reverse();
来源：http://wim.aizwys.cn

[D12] 查找元素下标
来源：http://ttk.tarul.cn

Py:   arr.index(x);  x in arr
来源：http://qkh.jinyuanbaomall.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://bee.cheryme.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jsk.c1oappe.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://upd.c1oappe.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://zzh.smart0.xyz

Go:   slices.Index(arr, x)
来源：http://oqd.feifeiyinyue.top

Ruby: arr.index(x)
来源：http://fmy.zhongyouzk.top

C#:   list.IndexOf(x);
来源：http://smi.cashguo.top

[D13] 过滤（保留满足条件的）
来源：http://cwe.yfazqb.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://gyt.zhongyouzk.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://euj.chenzaomai.com

JS:   arr.filter(x => x > 3)
来源：http://ijg.ybcxt.top

TS:   arr.filter(x => x > 3)
来源：http://bzw.redwolf501.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://stw.sysykeji.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hbn.xingfuxueyuan.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://qwl.yangfankeji.com

C#:   list.Where(x => x > 3).ToList()
来源：http://fqi.c1oappe.top

[D14] 映射转换（每个元素变形）
来源：http://yym.kuanghao11.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://sgk.jinqigufen.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ftd.mhx1999.top

JS:   arr.map(x => x * 2)
来源：http://ctu.fzhhl.top

TS:   arr.map(x => x * 2)
来源：http://gmg.tarul.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://lsz.daxiang520.top

Go:   // 手写循环
来源：http://coj.fanxiaobao.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://azf.ywan-chungtsiang.top

C#:   list.Select(x => x * 2).ToList()
来源：http://kye.zdbjq.cn

[D15] 去重
来源：http://qhf.ybcxt.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://fij.havefunace.top

PHP:  array_unique($arr);
来源：http://too.bbcook.cn

JS:   [...new Set(arr)]
来源：http://ffb.andypj.xyz

TS:   [...new Set(arr)]
来源：http://xtc.vqdsnc.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://amb.xingfuxueyuan.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://gas.svipenyu.cn

Ruby: arr.uniq
来源：http://ppk.wangdashe.top

C#:   list.Distinct().ToList()
来源：http://tig.uphjek.com

[D16] 求和与平均值
来源：http://zyb.bbcook.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://gff.xziqi.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://vjd.shangyingyoupin.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://rke.yuxming.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://zid.fengsongda.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ehq.shzxlz.cn

Go:   // 手写循环累加
来源：http://cpb.quarkkingdee.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://xek.yuxming.cn

C#:   list.Sum();  list.Average()
来源：http://nin.snrcjt.cn

[D17] 最大值与最小值
来源：http://wwj.yueranfly.top

Py:   max(arr);  min(arr)
来源：http://pvw.xinyue.icu

PHP:  max($arr);  min($arr);
来源：http://kei.ydjk.org.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://eex.zhengqikj.top

TS:   Math.max(...arr);
来源：http://mfp.jqgfzy.top

Java: Collections.max(list);  Collections.min(list);
来源：http://xsn.fengsongda.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://rgz.nanxuanxn.top

Ruby: arr.max;  arr.min
来源：http://gtf.bbcook.cn

C#:   list.Max();  list.Min()
来源：http://bdo.shangyingyoupin.top

[D18] 扁平化嵌套数组
来源：http://gcj.svipenyu.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mru.cheryme.top

PHP:  array_merge(...$nested);
来源：http://tzh.zhijiandao.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://zty.jqgufenzy.top

TS:   nested.flat();
来源：http://jnj.316326.xyz

Java: nested.stream().flatMap(List::stream).toList()
来源：http://zct.hnxiangtu.top

Go:   // 手写双层循环
来源：http://ruy.ybcxt.top

Ruby: nested.flatten
来源：http://sre.quarkkingdee.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://wld.zhaomingkeji.xyz

[D19] 按字段分组
来源：http://vvi.yuxming.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://jqj.vehdjk.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://zcg.zhoulong.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://agd.yfazqb.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://fyc.aibaodan.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://yue.zhoulong.xyz

Go:   // 手写 map[string][]T
来源：http://sqp.zhijiandao.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://imk.zhiwuduotai.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://gmz.iojbl.cn

[D20] 统计每个元素出现次数
来源：http://eat.vehdjk.com

Py:   Counter(arr)
来源：http://thr.yueranfly.top

PHP:  array_count_values($arr);
来源：http://ehy.jqgufenzy.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ewv.iojbl.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rvj.andypj.xyz

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ggj.gzhubu.top

Go:   // 手写 map[T]int
来源：http://tpp.gogol.net.cn

Ruby: arr.tally
来源：http://hea.xuanzx.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://vjg.uphjek.com

[D21] 判断是否包含某元素
来源：http://krt.gotoacloud.top

Py:   x in arr
来源：http://kvv.guannengcc.top

PHP:  in_array($x, $arr, true);
来源：http://kvq.fehbvm.com

JS:   arr.includes(x)
来源：http://nhj.cucudq.cn

TS:   arr.includes(x)
来源：http://ctu.fzhhl.top

Java: list.contains(x)
来源：http://ygy.yonumen.top

Go:   slices.Contains(arr, x)
来源：http://ycj.tianlin.xyz

Ruby: arr.include?(x)
来源：http://cxa.zdqjudy.top

C#:   list.Contains(x)
来源：http://zuy.xuanzx.com

[D22] 复制数组（避免共享引用）
来源：http://gth.fanxiaobao.xyz

Py:   arr.copy();  arr[:];  list(arr)
来源：http://kuc.daria6918.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://zxo.daxiang520.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://rsl.nwbrower.top

TS:   [...arr];
来源：http://ysm.zhiwuduotai.top

Java: new ArrayList<>(list);
来源：http://rcu.sxryk.cn

Go:   copied := append([]int(nil), arr...)
来源：http://twb.ybcxt.top

Ruby: arr.dup;  arr.clone
来源：http://adb.fzhhl.top

C#:   new List<int>(list);
来源：http://iox.dianchejie.cn

[D23] reduce 累积计算
来源：http://cwf.zdqjudy.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://qvs.shanyushiyangtech.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://itj.cqqwz.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qar.hongshengwenyu.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://uah.cucudq.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://lvn.gzhubu.top

Go:   // 手写循环
来源：http://ykk.jianghu66.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wjn.gotoacloud.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://xdv.jinqigufen.top

[D24] 字典 / Map 基本操作
来源：http://jgk.haohaochexian.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://zad.cucudq.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://izn.pycfn.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://imo.ydzc1.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://qlf.havefunace.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://tvc.jlsjyb.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mkb.shuidangran.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://esi.xuetiantiany.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ngq.ydjk.org.cn

[D25] Set 集合去重与交并差
来源：http://fra.zhixingplan.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://zen.zhongyouzk.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ewc.shzxlz.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://kej.hongshengwenyu.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://iai.yueranfly.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://zma.yonumen.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mum.chenzaomai.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://idu.yuanzhike.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://pqp.hesvh.cn

[D26] 数组转字符串
来源：http://kgq.hesvh.cn


<!-- 参考信息 -->