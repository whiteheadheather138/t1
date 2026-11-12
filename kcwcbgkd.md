代发 wailian999

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://zgq.jinqigfzy.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://brl.shzxlz.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mrb.jianghu66.top

[C09] 递归
来源：http://fjh.nanxuanxn.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://nqy.jlsjyb.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://sud.redwolf501.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pwy.nanxuanxn.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://aet.sjlbkw.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://gif.yuxming.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ybn.tian-w.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://umu.ivvv.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://rgn.sysykeji.top

[C10] 变量作用域
来源：http://exh.hnxiangtu.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://eoa.yueranfly.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://gth.ydjk.org.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mpr.zhiwuduotai.top

TS:   同 JS
来源：http://kar.jqgfzy.top

Java: 方法内为块级作用域
来源：http://lmu.gaohongyu789.top

Go:   花括号块级作用域
来源：http://mwu.jinqigfzy.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://kvh.dianchejie.cn

C#:   块级作用域
来源：http://lyu.hongshengwenyu.top

[C11] 模块导入与导出
来源：http://mgp.xingfuxueyuan.xyz

Py:   from module import func
来源：http://lrb.jinghuilouyu.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://sli.epnwcf.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://zht.shanyushiyangkeji.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://sbp.zdbjq.cn

Java: import java.util.List;
来源：http://nlp.zdqjudy.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://vfb.ywan-chungtsiang.top

Ruby: require "json"; require_relative "./util"
来源：http://ciz.yonumen.top

C#:   using System.Text;
来源：http://eun.jinqigufen.top

[C12] 立即执行函数 IIFE
来源：http://pgl.52xcode.cn

Py:   (lambda: print("run"))()
来源：http://kuj.sysykeji.top

PHP:  (function () { echo "run"; })();
来源：http://mnv.jiagoushi.top

JS:   (() => { console.log("run"); })();
来源：http://mae.hammf.cn

TS:   (() => { console.log("run"); })();
来源：http://bxq.jyoumei.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://zly.hfpthk.cn

Go:   func() { fmt.Println("run") }()
来源：http://fnj.zhixingplan.top

Ruby: -> { puts "run" }.call
来源：http://sui.jinghuilouyu.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://zbe.sysykeji.top

[C13] 类型声明 / 类型注解
来源：http://bxe.cashguo.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://tdc.yonumen.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hph.aizwys.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://xjf.vqdsnc.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tka.zdbjq.cn

Java: int add(int a, int b) { return a + b; }
来源：http://mid.xingfuxueyuan.xyz

Go:   func add(a, b int) int
来源：http://spn.redwolf501.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://tys.jinghuilouyu.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ecx.wangdashe.top

[C14] 泛型函数
来源：http://amm.yj20258888.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hqg.chenzaomai.com

PHP:  // 无泛型
来源：http://mew.xinyue.icu

JS:   // 无泛型
来源：http://kyx.tianlin.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://pqw.hammf.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://oxq.hywenlv.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://suc.smart0.xyz

Ruby: # 无泛型
来源：http://ngn.pycfn.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://sxp.tanke756.top

[C15] 解构 / 展开参数
来源：http://oya.hywenlv.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://aqp.shanyushiyangkeji.top

PHP:  [$a, $b] = $pair;
来源：http://xrq.shanyushiyangkeji.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://kfw.hfpthk.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://zwx.chenjidiqi.icu

Java: // 无解构
来源：http://ihm.xingfuxueyuan.xyz

Go:   // 无解构
来源：http://vgb.shuidangran.top

Ruby: a, b = pair
来源：http://zql.redwolf501.top

C#:   var (a, b) = pair;
来源：http://nbk.ppjwa.cn

[C16] 函数 / 方法重载
来源：http://gye.feifeiyinyue.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://tuv.hammf.cn

PHP:  // 无重载
来源：http://day.hysaishi.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ogf.fehbvm.com

TS:   // 用联合类型或重载签名声明
来源：http://drr.iojbl.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ril.xuetiantiany.cn

Go:   // 无重载：用不同函数名
来源：http://uua.ctjpmb.com

Ruby: # 无重载：靠动态参数
来源：http://efn.xylfe.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://jji.yj20258.top

================================================================================
来源：http://fgi.yueranfly.top

D. 数组 / 列表 / 集合
来源：http://voj.yonumen.top

================================================================================
来源：http://psi.sufxvd.cn

[D01] 创建数组 / 列表
来源：http://fxv.pycfn.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://iog.yanxiufei.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://bas.andypj.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://xts.gotoacloud.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://ucn.iojbl.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hcs.sweek.top

Go:   arr := []int{1, 2, 3}
来源：http://kgq.yueranfly.top

Ruby: arr = [1, 2, 3]
来源：http://bef.feifeiyinyue.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://kvr.jqgfzy.top

[D02] 追加元素到末尾
来源：http://qha.hywenlv.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://nxp.shzxlz.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://szp.ybcxt.top

JS:   arr.push(4);
来源：http://exc.jqgufenzy.top

TS:   arr.push(4);
来源：http://pwv.fanxiaobao.xyz

Java: list.add(4);
来源：http://twl.xziqi.cn

Go:   arr = append(arr, 4)
来源：http://rrj.sweek.top

Ruby: arr << 4; arr.push(5)
来源：http://got.shanyushiyangtech.top

C#:   list.Add(4);
来源：http://yza.nwbrower.top

[D03] 在指定位置插入元素
来源：http://ubn.zhoulong.xyz

Py:   arr.insert(0, 0)
来源：http://plr.jqgfzy.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://vzn.jinqigufen.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wka.bjfxy.top

TS:   arr.splice(0, 0, 0);
来源：http://uth.gzhubu.top

Java: list.add(0, 0);
来源：http://kts.shangyingyoupin.top

Go:   arr = append([]int{0}, arr...)
来源：http://nhw.c1oappe.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://jxl.tianlin.xyz

C#:   list.Insert(0, 0);
来源：http://kcj.shuidangran.top

[D04] 删除元素
来源：http://gsd.sxryk.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://zwh.nanxuanxn.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://qcl.jinqigfzy.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://czo.ydjk.org.cn

TS:   arr.splice(0, 1);
来源：http://vui.hesvh.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://qwb.shzxlz.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://gay.yonumen.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://tsv.ehwqpu.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://zqw.9152youxi.cn

[D05] 访问与修改元素
来源：http://ytu.zhijiandao.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://rzg.yj202588.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://vdb.daria6918.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://vmm.fktsv.cn

TS:   arr[0]; arr.at(-1);
来源：http://skf.hnqzz.top

Java: list.get(0); list.set(0, 9);
来源：http://daq.jlsjyb.cn

Go:   arr[0]; arr[0] = 9
来源：http://bwq.shuidangran.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://sti.ivvv.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ufe.guowangkeji.top

[D06] 数组长度
来源：http://irr.9152youxi.cn

Py:   len(arr)
来源：http://wno.guowangkeji.top

PHP:  count($arr);
来源：http://qvj.vehdjk.com

JS:   arr.length
来源：http://ruu.mhx1999.top

TS:   arr.length
来源：http://rdi.sufxvd.cn

Java: list.size();
来源：http://gyb.havefunace.top

Go:   len(arr)
来源：http://ipb.c1oappe.top

Ruby: arr.length; arr.size
来源：http://yyu.daxiang520.top

C#:   list.Count;
来源：http://mxe.hywenlv.cn

[D07] 切片 / 取子数组
来源：http://sis.jinqigfzy.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://rlo.fengsongda.top

PHP:  array_slice($arr, 1, 3);
来源：http://jqs.dianchejie.cn

JS:   arr.slice(1, 4);
来源：http://krt.hongshengwenyu.top

TS:   arr.slice(1, 4);
来源：http://xvc.aizwys.cn

Java: list.subList(1, 4);
来源：http://ayn.daxiang520.top

Go:   arr[1:4]
来源：http://hbr.jinyuanbaomall.cn

Ruby: arr[1, 3]
来源：http://ihb.ywan-chungtsiang.top

C#:   list.GetRange(1, 3);
来源：http://jyc.yongpay.top

[D08] 合并两个数组
来源：http://plb.jyoumei.cn

Py:   a + b;  a.extend(b)
来源：http://lqx.chenlongwang.top

PHP:  array_merge($a, $b);
来源：http://bkz.chenjidiqi.icu

JS:   [...a, ...b];  a.concat(b);
来源：http://gbk.kuanghao11.cn

TS:   [...a, ...b];
来源：http://oyh.9152youxi.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://zsp.meibo888.top

Go:   append(a, b...)
来源：http://ttz.tian-w.cn

Ruby: a + b;  a.concat(b)
来源：http://sgw.ctjpmb.com

C#:   a.Concat(b).ToList()
来源：http://azn.daria6918.cn

[D09] 排序（升序）
来源：http://zjr.bjfxy.top

Py:   sorted(arr);  arr.sort()
来源：http://det.vehdjk.com

PHP:  sort($arr);
来源：http://bel.jqgfzy.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://yhm.ywan-chungtsiang.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://uks.sjlbkw.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://hof.sxryk.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hrj.chenlongwang.top

Ruby: arr.sort
来源：http://dui.gaohongyu789.top

C#:   list.Sort();
来源：http://tym.pycfn.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://pcx.ppjwa.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://nep.ivvv.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bvn.feifeiyinyue.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://jrk.kuanghao11.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://aft.chenlongwang.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://uof.jqgufenzy.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://yrh.jinqigufen.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://oil.yj20258888.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://aih.yuxming.cn

[D11] 反转数组
来源：http://bov.ivvv.top

Py:   arr[::-1];  arr.reverse()
来源：http://jfj.hammf.cn

PHP:  array_reverse($arr);
来源：http://blm.ctjpmb.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://zle.kuanghao11.cn

TS:   [...arr].reverse();
来源：http://qrt.mhx1999.top

Java: Collections.reverse(list);
来源：http://gkd.yj20258888.top

Go:   slices.Reverse(arr)
来源：http://der.hammf.cn

Ruby: arr.reverse
来源：http://stc.shuidangran.top

C#:   list.Reverse();
来源：http://fkq.jinqigfzy.top

[D12] 查找元素下标
来源：http://wfm.chenzaomai.com

Py:   arr.index(x);  x in arr
来源：http://zft.tian-w.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://qoo.ppjwa.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gcw.yvedp.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xgn.0kj1m.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ngo.smart0.xyz

Go:   slices.Index(arr, x)
来源：http://ovq.hysaishi.cn

Ruby: arr.index(x)
来源：http://bwm.zhaomingkeji.xyz

C#:   list.IndexOf(x);
来源：http://xtq.yj20258888.top

[D13] 过滤（保留满足条件的）
来源：http://ele.hywenlv.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hro.cdnleiting.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ogk.jqgufenzy.top

JS:   arr.filter(x => x > 3)
来源：http://glu.cheryme.top

TS:   arr.filter(x => x > 3)
来源：http://pud.zdbjq.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mck.xuetiantiany.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://cff.redwolf501.top

Ruby: arr.select { |x| x > 3 }
来源：http://bfw.shanyushiyangkeji.top

C#:   list.Where(x => x > 3).ToList()
来源：http://nop.hesvh.cn

[D14] 映射转换（每个元素变形）
来源：http://ayc.316326.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://axr.feifeiyinyue.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://fub.dashuyun.cn

JS:   arr.map(x => x * 2)
来源：http://zpb.yj20258.top

TS:   arr.map(x => x * 2)
来源：http://dnp.c1oappe.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://bfn.52xcode.cn

Go:   // 手写循环
来源：http://jcz.yonumen.top

Ruby: arr.map { |x| x * 2 }
来源：http://nhy.hongshengwenyu.top

C#:   list.Select(x => x * 2).ToList()
来源：http://zwe.sjlbkw.cn

[D15] 去重
来源：http://ege.gaohongyu789.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://xte.fehbvm.com

PHP:  array_unique($arr);
来源：http://hho.jinqigfzy.top

JS:   [...new Set(arr)]
来源：http://dvj.hcnkem.com

TS:   [...new Set(arr)]
来源：http://rsz.fanxiaobao.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://dht.daxiang520.top

Go:   // 用 map[T]struct{} 手写
来源：http://bge.uphjek.com

Ruby: arr.uniq
来源：http://dok.fzhhl.top

C#:   list.Distinct().ToList()
来源：http://waf.yuxming.cn

[D16] 求和与平均值
来源：http://nky.zycfv.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://dck.hysaishi.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://yfa.feifeiyinyue.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://szg.hnxiangtu.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://iwc.zdqjudy.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://neq.wangdashe.top

Go:   // 手写循环累加
来源：http://jfm.316326.xyz

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ren.sysykeji.top

C#:   list.Sum();  list.Average()
来源：http://mef.fzhhl.top

[D17] 最大值与最小值
来源：http://xcf.sysykeji.top

Py:   max(arr);  min(arr)
来源：http://kmy.jyoumei.cn

PHP:  max($arr);  min($arr);
来源：http://qyk.iojbl.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://vzp.jqgufenzy.top

TS:   Math.max(...arr);
来源：http://ocg.chenlongwang.top

Java: Collections.max(list);  Collections.min(list);
来源：http://aqr.uphjek.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://vwu.hysaishi.cn

Ruby: arr.max;  arr.min
来源：http://ips.nanxuanxn.top

C#:   list.Max();  list.Min()
来源：http://sud.xuetiantiany.cn

[D18] 扁平化嵌套数组
来源：http://fbr.xylfe.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://yqd.xylfe.cn

PHP:  array_merge(...$nested);
来源：http://tcw.daxiang520.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://tbn.sufxvd.cn

TS:   nested.flat();
来源：http://ynb.yj20258888.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://npc.nwbrower.top

Go:   // 手写双层循环
来源：http://ckx.xuetiantiany.cn

Ruby: nested.flatten
来源：http://kcv.pengpengdd.cyou

C#:   nested.SelectMany(x => x).ToList()
来源：http://onb.jianghu66.top

[D19] 按字段分组
来源：http://mxa.chenjidiqi.icu

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ysn.ehwqpu.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://atv.hywenlv.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wgj.ehwqpu.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://ewu.tanke756.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ylq.uphjek.com

Go:   // 手写 map[string][]T
来源：http://exp.shangyingyoupin.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://hxk.hongshengwenyu.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wnw.redwolf501.top

[D20] 统计每个元素出现次数
来源：http://npj.jianghu66.top

Py:   Counter(arr)
来源：http://igk.xziqi.cn

PHP:  array_count_values($arr);
来源：http://wgi.yanxiufei.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nzu.nwbrower.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kwo.vqdsnc.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://zrl.zhongyouzk.top

Go:   // 手写 map[T]int
来源：http://oog.xuetiantiany.cn

Ruby: arr.tally
来源：http://rtz.yfazqb.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://egm.kuanghao11.cn

[D21] 判断是否包含某元素
来源：http://cdr.hcnkem.com

Py:   x in arr
来源：http://shq.bbcook.cn

PHP:  in_array($x, $arr, true);
来源：http://epw.zhengqikj.top

JS:   arr.includes(x)
来源：http://vhe.yfazqb.com

TS:   arr.includes(x)
来源：http://wdz.sjlbkw.cn

Java: list.contains(x)
来源：http://fsu.haohaochexian.top

Go:   slices.Contains(arr, x)
来源：http://vnq.dianchejie.cn

Ruby: arr.include?(x)
来源：http://yhd.aibaodan.cn

C#:   list.Contains(x)
来源：http://uvs.kuanghao11.cn

[D22] 复制数组（避免共享引用）
来源：http://aal.zdbjq.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://gzf.aizwys.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wgv.hammf.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://vex.cheryme.top

TS:   [...arr];
来源：http://kup.zdqjudy.top

Java: new ArrayList<>(list);
来源：http://jyf.jyoumei.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ovj.birdmap.top

Ruby: arr.dup;  arr.clone
来源：http://zeg.hnqzz.top

C#:   new List<int>(list);
来源：http://qsv.dianchejie.cn

[D23] reduce 累积计算
来源：http://qou.9152youxi.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://vzc.yanxiufei.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://isv.haohaochexian.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fvn.tarul.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nla.zhaomingkeji.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://xdv.xinyue.icu

Go:   // 手写循环
来源：http://qsv.yfazqb.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://eir.zycfv.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://rmw.316326.xyz

[D24] 字典 / Map 基本操作
来源：http://zko.zhiwuduotai.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ncc.yanxiufei.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://fhe.shzxlz.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://yzc.cucudq.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://tqp.nwbrower.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://atn.ydzc1.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://fai.meibo888.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://exd.shanyushiyangtech.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wzz.zhiwuduotai.top

[D25] Set 集合去重与交并差
来源：http://eme.fengsongda.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://bbg.hnxiangtu.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://qzh.jianghu66.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://pvs.hongshengwenyu.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://nnq.meibo888.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ivx.jinqigufen.top


<!-- 参考信息 -->