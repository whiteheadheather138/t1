代发 wailian999

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://pcd.fengsongda.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://gsd.yfazqb.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wgm.bbcook.cn

[C09] 递归
来源：http://amw.birdmap.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mwg.fktsv.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://zae.gotoacloud.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://phj.0kj1m.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blg.gaohongyu789.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://yva.hywenlv.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://nab.guowangkeji.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://lgr.shzxlz.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://gfl.ctjpmb.com

[C10] 变量作用域
来源：http://jgr.daxiang520.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://dnc.c1oappe.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://grr.xingfuxueyuan.xyz

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xgc.redwolf501.top

TS:   同 JS
来源：http://bfu.xinyue.icu

Java: 方法内为块级作用域
来源：http://wlq.snrcjt.cn

Go:   花括号块级作用域
来源：http://lgb.shangyingyoupin.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://nur.wangshuangyany.cn

C#:   块级作用域
来源：http://ful.hywenlv.cn

[C11] 模块导入与导出
来源：http://tlc.yfazqb.com

Py:   from module import func
来源：http://tsd.gogol.net.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://mmi.yfazqb.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://dsm.sxryk.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://tiv.feifeiyinyue.top

Java: import java.util.List;
来源：http://qsr.xinyue.icu

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://fpi.pengpengdd.cyou

Ruby: require "json"; require_relative "./util"
来源：http://ojl.ivvv.top

C#:   using System.Text;
来源：http://gut.hammf.cn

[C12] 立即执行函数 IIFE
来源：http://kgw.smart0.xyz

Py:   (lambda: print("run"))()
来源：http://vaz.xziqi.cn

PHP:  (function () { echo "run"; })();
来源：http://lvj.epnwcf.com

JS:   (() => { console.log("run"); })();
来源：http://yqs.chenjidiqi.icu

TS:   (() => { console.log("run"); })();
来源：http://vun.vehdjk.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://rkr.xingfuxueyuan.xyz

Go:   func() { fmt.Println("run") }()
来源：http://mbv.ehwqpu.com

Ruby: -> { puts "run" }.call
来源：http://vpq.yuxming.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://sgo.jinghuilouyu.cn

[C13] 类型声明 / 类型注解
来源：http://tca.c1oappe.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://bpu.zhoulong.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://uas.pycfn.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://twg.sweek.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pre.xziqi.cn

Java: int add(int a, int b) { return a + b; }
来源：http://vuk.svipenyu.cn

Go:   func add(a, b int) int
来源：http://etm.aizwys.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://rzr.svipenyu.cn

C#:   int Add(int a, int b) => a + b;
来源：http://xhg.jinghuilouyu.cn

[C14] 泛型函数
来源：http://jki.ydjk.org.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mzo.jinqigfzy.top

PHP:  // 无泛型
来源：http://nqa.pengpengdd.cyou

JS:   // 无泛型
来源：http://wsm.0kj1m.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://dcc.yuanzhike.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://jbx.hfpthk.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://egy.fengsongda.top

Ruby: # 无泛型
来源：http://edt.xinyue.icu

C#:   static T First<T>(List<T> items) => items[0];
来源：http://zle.cheryme.top

[C15] 解构 / 展开参数
来源：http://ukw.ctjpmb.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://udw.jlsjyb.cn

PHP:  [$a, $b] = $pair;
来源：http://xvz.vehdjk.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://erv.bjfxy.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://nvb.havefunace.top

Java: // 无解构
来源：http://kpg.hfpthk.cn

Go:   // 无解构
来源：http://pbg.jinyuanbaomall.cn

Ruby: a, b = pair
来源：http://mve.jinghuilouyu.cn

C#:   var (a, b) = pair;
来源：http://kbo.gotoacloud.top

[C16] 函数 / 方法重载
来源：http://tkz.cucudq.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://kag.zhiwuduotai.top

PHP:  // 无重载
来源：http://zri.zhongyouzk.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://lvw.nwbrower.top

TS:   // 用联合类型或重载签名声明
来源：http://gsf.chenlongwang.top

Java: void f(int a) {}  void f(String a) {}
来源：http://dyx.aizwys.cn

Go:   // 无重载：用不同函数名
来源：http://csp.zycfv.cn

Ruby: # 无重载：靠动态参数
来源：http://kpa.jianghu66.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://tru.haohaochexian.top

================================================================================
来源：http://afk.wangdashe.top

D. 数组 / 列表 / 集合
来源：http://pyd.yonumen.top

================================================================================
来源：http://rdx.jlsjyb.cn

[D01] 创建数组 / 列表
来源：http://xmc.hfpthk.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://lum.nanxuanxn.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://vak.haohaochexian.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://nqe.yuanzhike.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://jzh.tianlin.xyz

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://kkw.zhijiandao.cn

Go:   arr := []int{1, 2, 3}
来源：http://otc.zycfv.cn

Ruby: arr = [1, 2, 3]
来源：http://thn.jinghuilouyu.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wav.jqgufenzy.top

[D02] 追加元素到末尾
来源：http://lpb.zhengqikj.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://yxd.andypj.xyz

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://xlw.fanxiaobao.xyz

JS:   arr.push(4);
来源：http://czn.yanxiufei.cn

TS:   arr.push(4);
来源：http://kzc.fengsongda.top

Java: list.add(4);
来源：http://bac.xinyue.icu

Go:   arr = append(arr, 4)
来源：http://ipu.jqgfzy.top

Ruby: arr << 4; arr.push(5)
来源：http://non.yvedp.cn

C#:   list.Add(4);
来源：http://bdr.gzhubu.top

[D03] 在指定位置插入元素
来源：http://duh.ydjk.org.cn

Py:   arr.insert(0, 0)
来源：http://zgx.mhx1999.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://lmo.jlsjyb.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://aeu.shuidangran.top

TS:   arr.splice(0, 0, 0);
来源：http://gdb.sysykeji.top

Java: list.add(0, 0);
来源：http://rdp.jinyuanbaomall.cn

Go:   arr = append([]int{0}, arr...)
来源：http://smu.cdnleiting.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://dxt.tanke756.top

C#:   list.Insert(0, 0);
来源：http://tuz.hfpthk.cn

[D04] 删除元素
来源：http://fdf.52xcode.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://bzu.meibo888.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://kuh.smart0.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://nvt.aibaodan.cn

TS:   arr.splice(0, 1);
来源：http://mhx.epnwcf.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://bcs.xingfuxueyuan.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hmm.iojbl.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ipn.hcnkem.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://vde.yuanzhike.top

[D05] 访问与修改元素
来源：http://xdg.daria6918.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://kki.jqgfzy.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ico.guannengcc.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ljv.ehwqpu.com

TS:   arr[0]; arr.at(-1);
来源：http://cye.pycfn.com

Java: list.get(0); list.set(0, 9);
来源：http://pfx.xinyue.icu

Go:   arr[0]; arr[0] = 9
来源：http://ptt.meibo888.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://qkf.nanxuanxn.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zoq.snrcjt.cn

[D06] 数组长度
来源：http://uwj.xuetiantiany.cn

Py:   len(arr)
来源：http://zmk.ybcxt.top

PHP:  count($arr);
来源：http://yyv.yongpay.top

JS:   arr.length
来源：http://itj.fktsv.cn

TS:   arr.length
来源：http://llt.c1oappe.top

Java: list.size();
来源：http://svl.cheryme.top

Go:   len(arr)
来源：http://bwj.ivvv.top

Ruby: arr.length; arr.size
来源：http://ask.zhoulong.xyz

C#:   list.Count;
来源：http://qkh.pengpengdd.cyou

[D07] 切片 / 取子数组
来源：http://dvm.tian-w.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://lsf.zhengqikj.top

PHP:  array_slice($arr, 1, 3);
来源：http://flp.ywan-chungtsiang.top

JS:   arr.slice(1, 4);
来源：http://cjv.316326.xyz

TS:   arr.slice(1, 4);
来源：http://irt.shangyingyoupin.top

Java: list.subList(1, 4);
来源：http://uzi.zhaomingkeji.xyz

Go:   arr[1:4]
来源：http://xns.redwolf501.top

Ruby: arr[1, 3]
来源：http://hgt.nanxinkj.top

C#:   list.GetRange(1, 3);
来源：http://fvf.tarul.cn

[D08] 合并两个数组
来源：http://hxo.yj20258.top

Py:   a + b;  a.extend(b)
来源：http://dur.316326.xyz

PHP:  array_merge($a, $b);
来源：http://hsl.ywan-chungtsiang.top

JS:   [...a, ...b];  a.concat(b);
来源：http://dlu.xingfuxueyuan.xyz

TS:   [...a, ...b];
来源：http://zkn.shzxlz.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hke.yj202588.top

Go:   append(a, b...)
来源：http://oxu.yangfankeji.com

Ruby: a + b;  a.concat(b)
来源：http://jnv.sxryk.cn

C#:   a.Concat(b).ToList()
来源：http://ctx.zhengqikj.top

[D09] 排序（升序）
来源：http://ezg.feifeiyinyue.top

Py:   sorted(arr);  arr.sort()
来源：http://plb.shuidangran.top

PHP:  sort($arr);
来源：http://xnj.yonumen.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://uwl.gogol.net.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ego.chenzaomai.com

Java: Collections.sort(list);  list.sort(null);
来源：http://wyn.fengsongda.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://cmk.cheryme.top

Ruby: arr.sort
来源：http://huo.yangfankeji.com

C#:   list.Sort();
来源：http://vxw.yueranfly.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://iwt.sweek.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://gyp.yuanzhike.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tcq.nwbrower.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://gfe.mhx1999.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ztl.ppjwa.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://dbn.zhengqikj.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://qca.hysaishi.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ahh.c1oappe.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://uqz.zhijiandao.cn

[D11] 反转数组
来源：http://egv.wangdashe.top

Py:   arr[::-1];  arr.reverse()
来源：http://elj.jinqigfzy.top

PHP:  array_reverse($arr);
来源：http://tec.kuanghao11.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://oyw.cashguo.top

TS:   [...arr].reverse();
来源：http://nua.xylfe.cn

Java: Collections.reverse(list);
来源：http://uuu.guannengcc.top

Go:   slices.Reverse(arr)
来源：http://ggw.redwolf501.top

Ruby: arr.reverse
来源：http://ske.vqdsnc.cn

C#:   list.Reverse();
来源：http://uvu.pycfn.com

[D12] 查找元素下标
来源：http://mie.yangfankeji.com

Py:   arr.index(x);  x in arr
来源：http://sbd.shzxlz.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://lmd.zhoulong.xyz

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://usl.sufxvd.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nfs.gogol.net.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wqe.shuidangran.top

Go:   slices.Index(arr, x)
来源：http://csr.kuanghao11.cn

Ruby: arr.index(x)
来源：http://tnn.gaohongyu789.top

C#:   list.IndexOf(x);
来源：http://xjs.uphjek.com

[D13] 过滤（保留满足条件的）
来源：http://wdi.zycfv.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://zhe.zhaomingkeji.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://zbt.ybcxt.top

JS:   arr.filter(x => x > 3)
来源：http://dtu.fktsv.cn

TS:   arr.filter(x => x > 3)
来源：http://exv.bjfxy.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://jbb.sysykeji.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://asc.tanke756.top

Ruby: arr.select { |x| x > 3 }
来源：http://dov.yj202588.top

C#:   list.Where(x => x > 3).ToList()
来源：http://trc.dianchejie.cn

[D14] 映射转换（每个元素变形）
来源：http://gmj.zdbjq.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mlo.sxryk.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://kgr.zhongyouzk.top

JS:   arr.map(x => x * 2)
来源：http://ufx.wangshuangyany.cn

TS:   arr.map(x => x * 2)
来源：http://shq.shuidangran.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://rwc.nanxinkj.top

Go:   // 手写循环
来源：http://tmb.zhengqikj.top

Ruby: arr.map { |x| x * 2 }
来源：http://loi.shanyushiyangtech.top

C#:   list.Select(x => x * 2).ToList()
来源：http://veg.dashuyun.cn

[D15] 去重
来源：http://kmj.cashguo.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://lgo.yongpay.top

PHP:  array_unique($arr);
来源：http://afe.yj20258888.top

JS:   [...new Set(arr)]
来源：http://irg.zhixingplan.top

TS:   [...new Set(arr)]
来源：http://oej.ehwqpu.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://zqr.jinqigfzy.top

Go:   // 用 map[T]struct{} 手写
来源：http://mrv.sweek.top

Ruby: arr.uniq
来源：http://wyh.vqdsnc.cn

C#:   list.Distinct().ToList()
来源：http://kqb.cdnleiting.top

[D16] 求和与平均值
来源：http://gsx.jiagoushi.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://grs.fzhhl.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://chg.zhengqikj.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://qra.zycfv.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ftm.jlsjyb.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://duq.gzhubu.top

Go:   // 手写循环累加
来源：http://aqo.316326.xyz

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ohe.hysaishi.cn

C#:   list.Sum();  list.Average()
来源：http://hiu.zhengqikj.top

[D17] 最大值与最小值
来源：http://acs.aibaodan.cn

Py:   max(arr);  min(arr)
来源：http://opw.cucudq.cn

PHP:  max($arr);  min($arr);
来源：http://lfq.xylfe.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://xyt.sysykeji.top

TS:   Math.max(...arr);
来源：http://znp.daria6918.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://kbq.shanyushiyangtech.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://uht.c1oappe.top

Ruby: arr.max;  arr.min
来源：http://wnd.nanxuanxn.top

C#:   list.Max();  list.Min()
来源：http://ays.hysaishi.cn

[D18] 扁平化嵌套数组
来源：http://rox.pycfn.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://kdz.guannengcc.top

PHP:  array_merge(...$nested);
来源：http://bfe.zdbjq.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ngq.ydjk.org.cn

TS:   nested.flat();
来源：http://nyw.ydzc1.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://kch.iojbl.cn

Go:   // 手写双层循环
来源：http://zjd.nanxuanxn.top

Ruby: nested.flatten
来源：http://vdp.xziqi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://dzh.yueranfly.top

[D19] 按字段分组
来源：http://cpz.yonumen.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://nlx.gzhubu.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://cnx.dianchejie.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://rdx.havefunace.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://tze.jinqigfzy.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://xad.jinqigufen.top

Go:   // 手写 map[string][]T
来源：http://zkz.hesvh.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://msm.pycfn.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://zkq.fktsv.cn

[D20] 统计每个元素出现次数
来源：http://uys.epnwcf.com

Py:   Counter(arr)
来源：http://afj.andypj.xyz

PHP:  array_count_values($arr);
来源：http://bjq.dianchejie.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gpo.zhijiandao.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ejo.hnqzz.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://gyz.tanke756.top

Go:   // 手写 map[T]int
来源：http://eqa.birdmap.top

Ruby: arr.tally
来源：http://bef.birdmap.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://apf.uphjek.com

[D21] 判断是否包含某元素
来源：http://cho.hnxiangtu.top

Py:   x in arr
来源：http://rda.vehdjk.com

PHP:  in_array($x, $arr, true);
来源：http://vva.wangdashe.top

JS:   arr.includes(x)
来源：http://dnu.yvedp.cn

TS:   arr.includes(x)
来源：http://vze.ydzc1.top

Java: list.contains(x)
来源：http://ygt.guannengcc.top

Go:   slices.Contains(arr, x)
来源：http://ofu.ydjk.org.cn

Ruby: arr.include?(x)
来源：http://yxy.xingfuxueyuan.xyz

C#:   list.Contains(x)
来源：http://ygn.zhongyouzk.top

[D22] 复制数组（避免共享引用）
来源：http://jej.shanyushiyangkeji.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://abb.52xcode.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://iem.pengpengdd.cyou

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wlm.fzhhl.top

TS:   [...arr];
来源：http://ogo.zhaomingkeji.xyz

Java: new ArrayList<>(list);
来源：http://rjo.wangshuangyany.cn

Go:   copied := append([]int(nil), arr...)
来源：http://elx.zhixingplan.top

Ruby: arr.dup;  arr.clone
来源：http://mgy.ydjk.org.cn

C#:   new List<int>(list);
来源：http://uhk.wangshuangyany.cn

[D23] reduce 累积计算
来源：http://ghy.xuetiantiany.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wsz.ppjwa.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://kwe.hongshengwenyu.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://svq.svipenyu.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xds.quarkkingdee.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://qvv.hfpthk.cn

Go:   // 手写循环
来源：http://otx.hesvh.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://igm.cheryme.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://bxl.aizwys.cn

[D24] 字典 / Map 基本操作
来源：http://rgt.yuanzhike.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mnl.epnwcf.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://aow.dashuyun.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://kje.hesvh.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://xri.jyoumei.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://gfk.redwolf501.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://frn.ehwqpu.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mjm.guowangkeji.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hyt.yvedp.cn

[D25] Set 集合去重与交并差
来源：http://yvb.ppjwa.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://lis.xziqi.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://fmd.hywenlv.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://sro.hnxiangtu.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://zks.hnqzz.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://tqy.xylfe.cn


<!-- 参考信息 -->