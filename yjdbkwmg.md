代发 wailian999

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hhf.chenzaomai.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ytn.0kj1m.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://bar.jinqigufen.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://gez.shzxlz.cn

[C10] 变量作用域
来源：http://hyx.sweek.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://gat.yj20258.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://axn.52xcode.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://qxr.smart0.xyz

TS:   同 JS
来源：http://tpw.hnqzz.top

Java: 方法内为块级作用域
来源：http://yem.zhongyouzk.top

Go:   花括号块级作用域
来源：http://hkm.cqqwz.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://yzg.fehbvm.com

C#:   块级作用域
来源：http://ikj.zhongyouzk.top

[C11] 模块导入与导出
来源：http://itn.cdnleiting.top

Py:   from module import func
来源：http://vax.316326.xyz

PHP:  require "file.php";  或 use App\Service;
来源：http://urt.guowangkeji.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://nkt.gotoacloud.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xmi.pycfn.com

Java: import java.util.List;
来源：http://ycz.hnxiangtu.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://raf.jlsjyb.cn

Ruby: require "json"; require_relative "./util"
来源：http://mrd.9152youxi.cn

C#:   using System.Text;
来源：http://zqn.zhoulong.xyz

[C12] 立即执行函数 IIFE
来源：http://fcw.hcnkem.com

Py:   (lambda: print("run"))()
来源：http://igh.feifeiyinyue.top

PHP:  (function () { echo "run"; })();
来源：http://yiy.snrcjt.cn

JS:   (() => { console.log("run"); })();
来源：http://thh.gaohongyu789.top

TS:   (() => { console.log("run"); })();
来源：http://mxp.ydzc1.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://eri.nanxuanxn.top

Go:   func() { fmt.Println("run") }()
来源：http://yxl.shuidangran.top

Ruby: -> { puts "run" }.call
来源：http://mbd.yueranfly.top

C#:   // 无 IIFE：用静态构造函数
来源：http://qba.wangshuangyany.cn

[C13] 类型声明 / 类型注解
来源：http://npx.chenjidiqi.icu

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://bke.yfazqb.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cyi.wangdashe.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://fzt.xuetiantiany.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pzz.zdqjudy.top

Java: int add(int a, int b) { return a + b; }
来源：http://qjf.guowangkeji.top

Go:   func add(a, b int) int
来源：http://brd.hongshengwenyu.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://zlp.quarkkingdee.top

C#:   int Add(int a, int b) => a + b;
来源：http://duj.cucudq.cn

[C14] 泛型函数
来源：http://auq.zycfv.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hll.epnwcf.com

PHP:  // 无泛型
来源：http://bvk.svipenyu.cn

JS:   // 无泛型
来源：http://xum.snrcjt.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://pqc.nanxuanxn.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://psp.yfazqb.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mfs.ivvv.top

Ruby: # 无泛型
来源：http://ojk.hesvh.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://trp.xinyue.icu

[C15] 解构 / 展开参数
来源：http://ltu.meibo888.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://czq.dashuyun.cn

PHP:  [$a, $b] = $pair;
来源：http://dsf.hfpthk.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mty.haohaochexian.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://rol.yfazqb.com

Java: // 无解构
来源：http://gws.daria6918.cn

Go:   // 无解构
来源：http://ipq.sufxvd.cn

Ruby: a, b = pair
来源：http://owb.chenlongwang.top

C#:   var (a, b) = pair;
来源：http://zye.shanyushiyangkeji.top

[C16] 函数 / 方法重载
来源：http://mbd.gzhubu.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://obb.shanyushiyangkeji.top

PHP:  // 无重载
来源：http://xkh.jinyuanbaomall.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://qzg.andypj.xyz

TS:   // 用联合类型或重载签名声明
来源：http://osj.tianlin.xyz

Java: void f(int a) {}  void f(String a) {}
来源：http://kvx.ppjwa.cn

Go:   // 无重载：用不同函数名
来源：http://xpz.vqdsnc.cn

Ruby: # 无重载：靠动态参数
来源：http://wfm.cdnleiting.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://moo.uphjek.com

================================================================================
来源：http://dqm.yongpay.top

D. 数组 / 列表 / 集合
来源：http://idt.shangyingyoupin.top

================================================================================
来源：http://pxy.zhengqikj.top

[D01] 创建数组 / 列表
来源：http://aax.wangshuangyany.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://xln.jqgfzy.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://rmn.snrcjt.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://eag.hcnkem.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://uvw.nanxinkj.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://qhs.jiagoushi.top

Go:   arr := []int{1, 2, 3}
来源：http://fjp.yuxming.cn

Ruby: arr = [1, 2, 3]
来源：http://gyk.sjlbkw.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://tca.jqgfzy.top

[D02] 追加元素到末尾
来源：http://qbw.gotoacloud.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://jfg.hnqzz.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://xvj.yj20258888.top

JS:   arr.push(4);
来源：http://rag.chenjidiqi.icu

TS:   arr.push(4);
来源：http://tvp.hnxiangtu.top

Java: list.add(4);
来源：http://wrj.jyoumei.cn

Go:   arr = append(arr, 4)
来源：http://kns.jlsjyb.cn

Ruby: arr << 4; arr.push(5)
来源：http://mzk.yvedp.cn

C#:   list.Add(4);
来源：http://zwr.shuidangran.top

[D03] 在指定位置插入元素
来源：http://izn.hnqzz.top

Py:   arr.insert(0, 0)
来源：http://lmp.zycfv.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://tql.yongpay.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://tks.jqgfzy.top

TS:   arr.splice(0, 0, 0);
来源：http://tlz.zhaomingkeji.xyz

Java: list.add(0, 0);
来源：http://jyy.snrcjt.cn

Go:   arr = append([]int{0}, arr...)
来源：http://bfd.wangshuangyany.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://uum.daria6918.cn

C#:   list.Insert(0, 0);
来源：http://upd.shuidangran.top

[D04] 删除元素
来源：http://fvi.chenzaomai.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://pbn.shanyushiyangkeji.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://tof.shanyushiyangkeji.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://lil.zdbjq.cn

TS:   arr.splice(0, 1);
来源：http://txv.feifeiyinyue.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://qvr.kuanghao11.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://far.jqgfzy.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://pmw.zhiwuduotai.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://eos.zhongyouzk.top

[D05] 访问与修改元素
来源：http://bml.yuxming.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://cij.chenlongwang.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://loh.hfpthk.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://xym.uphjek.com

TS:   arr[0]; arr.at(-1);
来源：http://mhu.shuidangran.top

Java: list.get(0); list.set(0, 9);
来源：http://bvt.yfazqb.com

Go:   arr[0]; arr[0] = 9
来源：http://xre.cdnleiting.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://xbq.yfazqb.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://agb.fehbvm.com

[D06] 数组长度
来源：http://qfs.gogol.net.cn

Py:   len(arr)
来源：http://icx.yj20258888.top

PHP:  count($arr);
来源：http://tok.shanyushiyangtech.top

JS:   arr.length
来源：http://eoe.jinyuanbaomall.cn

TS:   arr.length
来源：http://hdw.jianghu66.top

Java: list.size();
来源：http://rik.cucudq.cn

Go:   len(arr)
来源：http://uet.zhaomingkeji.xyz

Ruby: arr.length; arr.size
来源：http://tcs.316326.xyz

C#:   list.Count;
来源：http://jas.yongpay.top

[D07] 切片 / 取子数组
来源：http://yrm.yj202588.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ybm.0kj1m.cn

PHP:  array_slice($arr, 1, 3);
来源：http://hyk.shzxlz.cn

JS:   arr.slice(1, 4);
来源：http://ifg.52xcode.cn

TS:   arr.slice(1, 4);
来源：http://phr.daria6918.cn

Java: list.subList(1, 4);
来源：http://aot.wangdashe.top

Go:   arr[1:4]
来源：http://gyv.hysaishi.cn

Ruby: arr[1, 3]
来源：http://esx.zdbjq.cn

C#:   list.GetRange(1, 3);
来源：http://xpz.yj20258888.top

[D08] 合并两个数组
来源：http://fsd.xziqi.cn

Py:   a + b;  a.extend(b)
来源：http://nxh.yangfankeji.com

PHP:  array_merge($a, $b);
来源：http://viq.tarul.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://wot.iojbl.cn

TS:   [...a, ...b];
来源：http://csm.hcnkem.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://fkz.cqqwz.cn

Go:   append(a, b...)
来源：http://txz.cdnleiting.top

Ruby: a + b;  a.concat(b)
来源：http://hjl.jinyuanbaomall.cn

C#:   a.Concat(b).ToList()
来源：http://eer.yj20258888.top

[D09] 排序（升序）
来源：http://jwp.uphjek.com

Py:   sorted(arr);  arr.sort()
来源：http://itn.epnwcf.com

PHP:  sort($arr);
来源：http://ext.hfpthk.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://cfq.jinqigfzy.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://mei.zdqjudy.top

Java: Collections.sort(list);  list.sort(null);
来源：http://wbv.pengpengdd.cyou

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://oxq.svipenyu.cn

Ruby: arr.sort
来源：http://sdx.yangfankeji.com

C#:   list.Sort();
来源：http://bqo.daxiang520.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://dwf.yueranfly.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ugk.hysaishi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tnu.jqgufenzy.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ipt.gzhubu.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fwt.fzhhl.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://kou.zycfv.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://vrt.sweek.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mgm.jqgufenzy.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wnc.9152youxi.cn

[D11] 反转数组
来源：http://tnf.tarul.cn

Py:   arr[::-1];  arr.reverse()
来源：http://hbo.aizwys.cn

PHP:  array_reverse($arr);
来源：http://klh.vehdjk.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://xnp.smart0.xyz

TS:   [...arr].reverse();
来源：http://oqf.sysykeji.top

Java: Collections.reverse(list);
来源：http://wgx.jiagoushi.top

Go:   slices.Reverse(arr)
来源：http://qwm.ppjwa.cn

Ruby: arr.reverse
来源：http://tnx.yfazqb.com

C#:   list.Reverse();
来源：http://ifw.sufxvd.cn

[D12] 查找元素下标
来源：http://bqm.hnqzz.top

Py:   arr.index(x);  x in arr
来源：http://vab.yueranfly.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://kvu.hesvh.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xys.nanxuanxn.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wrg.yvedp.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ijv.wangshuangyany.cn

Go:   slices.Index(arr, x)
来源：http://cak.yj20258.top

Ruby: arr.index(x)
来源：http://ldc.xingfuxueyuan.xyz

C#:   list.IndexOf(x);
来源：http://yjq.zhiwuduotai.top

[D13] 过滤（保留满足条件的）
来源：http://plr.yvedp.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://kqg.jinqigufen.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ubu.yueranfly.top

JS:   arr.filter(x => x > 3)
来源：http://blr.c1oappe.top

TS:   arr.filter(x => x > 3)
来源：http://ymu.tanke756.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ufd.yonumen.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://rvg.dashuyun.cn

Ruby: arr.select { |x| x > 3 }
来源：http://myk.xuetiantiany.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://uap.yuanzhike.top

[D14] 映射转换（每个元素变形）
来源：http://qxh.yj20258888.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://abq.jianghu66.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://kbm.yj20258888.top

JS:   arr.map(x => x * 2)
来源：http://flf.gaohongyu789.top

TS:   arr.map(x => x * 2)
来源：http://rdy.jinghuilouyu.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://vtf.tanke756.top

Go:   // 手写循环
来源：http://uhn.xziqi.cn

Ruby: arr.map { |x| x * 2 }
来源：http://lpa.pycfn.com

C#:   list.Select(x => x * 2).ToList()
来源：http://uwl.havefunace.top

[D15] 去重
来源：http://gly.birdmap.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://cfj.bjfxy.top

PHP:  array_unique($arr);
来源：http://jxh.chenlongwang.top

JS:   [...new Set(arr)]
来源：http://evq.yj20258.top

TS:   [...new Set(arr)]
来源：http://lcc.fzhhl.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ovj.quarkkingdee.top

Go:   // 用 map[T]struct{} 手写
来源：http://jsa.wangshuangyany.cn

Ruby: arr.uniq
来源：http://afv.jinqigfzy.top

C#:   list.Distinct().ToList()
来源：http://clx.birdmap.top

[D16] 求和与平均值
来源：http://yld.jianghu66.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://uth.vqdsnc.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://rca.yj20258888.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://khk.zycfv.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://muw.yongpay.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://lkh.hysaishi.cn

Go:   // 手写循环累加
来源：http://fik.chenzaomai.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://gqp.zhaomingkeji.xyz

C#:   list.Sum();  list.Average()
来源：http://ycv.jqgufenzy.top

[D17] 最大值与最小值
来源：http://agi.xziqi.cn

Py:   max(arr);  min(arr)
来源：http://oet.hongshengwenyu.top

PHP:  max($arr);  min($arr);
来源：http://vjw.xylfe.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://roi.vehdjk.com

TS:   Math.max(...arr);
来源：http://xar.jinyuanbaomall.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://pmg.guannengcc.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://bfi.jqgufenzy.top

Ruby: arr.max;  arr.min
来源：http://npl.zdqjudy.top

C#:   list.Max();  list.Min()
来源：http://fdk.epnwcf.com

[D18] 扁平化嵌套数组
来源：http://iwh.shanyushiyangtech.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xga.ydzc1.top

PHP:  array_merge(...$nested);
来源：http://sso.tarul.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ghl.mhx1999.top

TS:   nested.flat();
来源：http://gjk.tianlin.xyz

Java: nested.stream().flatMap(List::stream).toList()
来源：http://fub.guowangkeji.top

Go:   // 手写双层循环
来源：http://ndm.shzxlz.cn

Ruby: nested.flatten
来源：http://ikm.ctjpmb.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://ujh.daria6918.cn

[D19] 按字段分组
来源：http://iom.cqqwz.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://pqp.wangshuangyany.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://pwb.snrcjt.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://cau.xziqi.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://rsm.gzhubu.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://xet.hongshengwenyu.top

Go:   // 手写 map[string][]T
来源：http://try.aizwys.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://fhq.yfazqb.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://fgs.c1oappe.top

[D20] 统计每个元素出现次数
来源：http://poz.ydjk.org.cn

Py:   Counter(arr)
来源：http://xkn.ydzc1.top

PHP:  array_count_values($arr);
来源：http://fhm.daria6918.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jnz.zycfv.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xze.cucudq.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://llx.zhiwuduotai.top

Go:   // 手写 map[T]int
来源：http://fzb.sysykeji.top

Ruby: arr.tally
来源：http://dqa.haohaochexian.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://kvv.zhongyouzk.top

[D21] 判断是否包含某元素
来源：http://cbd.shuidangran.top

Py:   x in arr
来源：http://ixi.sysykeji.top

PHP:  in_array($x, $arr, true);
来源：http://vyu.ehwqpu.com

JS:   arr.includes(x)
来源：http://brz.kuanghao11.cn

TS:   arr.includes(x)
来源：http://asw.gzhubu.top

Java: list.contains(x)
来源：http://qtd.zdqjudy.top

Go:   slices.Contains(arr, x)
来源：http://ctq.ywan-chungtsiang.top

Ruby: arr.include?(x)
来源：http://xtr.yongpay.top

C#:   list.Contains(x)
来源：http://fjw.ppjwa.cn

[D22] 复制数组（避免共享引用）
来源：http://pew.zdbjq.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wvs.snrcjt.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://zzv.jinqigfzy.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://kec.tian-w.cn

TS:   [...arr];
来源：http://hhv.uphjek.com

Java: new ArrayList<>(list);
来源：http://zbq.quarkkingdee.top

Go:   copied := append([]int(nil), arr...)
来源：http://mfb.ywan-chungtsiang.top

Ruby: arr.dup;  arr.clone
来源：http://dqi.tarul.cn

C#:   new List<int>(list);
来源：http://dea.jinqigfzy.top

[D23] reduce 累积计算
来源：http://sve.xziqi.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://agc.xingfuxueyuan.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hzx.ppjwa.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jay.wangdashe.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://czi.kuanghao11.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://acv.ehwqpu.com

Go:   // 手写循环
来源：http://zuv.gaohongyu789.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://szp.shzxlz.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://jbp.guowangkeji.top

[D24] 字典 / Map 基本操作
来源：http://aas.pengpengdd.cyou

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://khb.zhiwuduotai.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://gzn.iojbl.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://kco.jiagoushi.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://irn.zycfv.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hvc.pycfn.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://jnw.chenjidiqi.icu

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://rtu.yanxiufei.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://oqj.jianghu66.top

[D25] Set 集合去重与交并差
来源：http://gow.hfpthk.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://rwu.hammf.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ktm.xziqi.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://bwf.vqdsnc.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://lbw.fanxiaobao.xyz

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://zyn.birdmap.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://tma.daria6918.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://npr.cqqwz.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://fhj.jinyuanbaomall.cn

[D26] 数组转字符串
来源：http://uyn.cucudq.cn

Py:   ", ".join(map(str, arr))
来源：http://vmk.tanke756.top

PHP:  implode(", ", $arr);
来源：http://jum.cheryme.top

JS:   arr.join(", ")
来源：http://ext.jlsjyb.cn

TS:   arr.join(", ")
来源：http://hbt.fengsongda.top


<!-- 参考信息 -->