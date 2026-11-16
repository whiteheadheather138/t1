代发 wailian999

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://dza.hysaishi.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://abv.cheryme.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yrm.hfpthk.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mnx.jqgfzy.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://lsk.ydjk.org.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://slv.ydzc1.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wmm.jqgufenzy.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://fth.shanyushiyangtech.top

[C10] 变量作用域
来源：http://kdg.jinghuilouyu.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://zmi.zhoulong.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://kda.jinqigfzy.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ren.hammf.cn

TS:   同 JS
来源：http://tox.tarul.cn

Java: 方法内为块级作用域
来源：http://zil.guannengcc.top

Go:   花括号块级作用域
来源：http://ogu.gogol.net.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://coa.chenlongwang.top

C#:   块级作用域
来源：http://cjj.jiagoushi.top

[C11] 模块导入与导出
来源：http://got.jlsjyb.cn

Py:   from module import func
来源：http://udh.chenlongwang.top

PHP:  require "file.php";  或 use App\Service;
来源：http://sag.dashuyun.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://hyj.andypj.xyz

TS:   export function f(): void {};  import { f } from "./m";
来源：http://uuh.jlsjyb.cn

Java: import java.util.List;
来源：http://jkm.gzhubu.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hzr.gotoacloud.top

Ruby: require "json"; require_relative "./util"
来源：http://mox.shzxlz.cn

C#:   using System.Text;
来源：http://kjy.hesvh.cn

[C12] 立即执行函数 IIFE
来源：http://umf.ydjk.org.cn

Py:   (lambda: print("run"))()
来源：http://dfi.jiagoushi.top

PHP:  (function () { echo "run"; })();
来源：http://ffb.tarul.cn

JS:   (() => { console.log("run"); })();
来源：http://wre.xylfe.cn

TS:   (() => { console.log("run"); })();
来源：http://ffo.guowangkeji.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://fqk.gaohongyu789.top

Go:   func() { fmt.Println("run") }()
来源：http://vgg.gaohongyu789.top

Ruby: -> { puts "run" }.call
来源：http://quj.daria6918.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://iqo.ivvv.top

[C13] 类型声明 / 类型注解
来源：http://ddw.yonumen.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://yqm.sxryk.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ree.chenjidiqi.icu

JS:   // 无类型（可用 JSDoc 注释）
来源：http://oyu.jlsjyb.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lfz.kuanghao11.cn

Java: int add(int a, int b) { return a + b; }
来源：http://iyb.fehbvm.com

Go:   func add(a, b int) int
来源：http://ket.yj202588.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://utu.shanyushiyangkeji.top

C#:   int Add(int a, int b) => a + b;
来源：http://jcm.ehwqpu.com

[C14] 泛型函数
来源：http://ikz.shanyushiyangkeji.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://lod.ctjpmb.com

PHP:  // 无泛型
来源：http://yeb.havefunace.top

JS:   // 无泛型
来源：http://qqa.jinqigufen.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://utf.nwbrower.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://chp.jinqigufen.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://agd.xuanzx.com

Ruby: # 无泛型
来源：http://mfx.yueranfly.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://abr.316326.xyz

[C15] 解构 / 展开参数
来源：http://hpi.yonumen.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://krl.vehdjk.com

PHP:  [$a, $b] = $pair;
来源：http://pzv.sjlbkw.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://atp.snrcjt.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ycu.cdnleiting.top

Java: // 无解构
来源：http://xla.wangdashe.top

Go:   // 无解构
来源：http://ngm.hnqzz.top

Ruby: a, b = pair
来源：http://cri.yj20258888.top

C#:   var (a, b) = pair;
来源：http://zqn.cucudq.cn

[C16] 函数 / 方法重载
来源：http://sqp.smart0.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hqr.feifeiyinyue.top

PHP:  // 无重载
来源：http://bny.cqqwz.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://gyq.shanyushiyangkeji.top

TS:   // 用联合类型或重载签名声明
来源：http://bau.andypj.xyz

Java: void f(int a) {}  void f(String a) {}
来源：http://zdb.xuetiantiany.cn

Go:   // 无重载：用不同函数名
来源：http://lag.zdqjudy.top

Ruby: # 无重载：靠动态参数
来源：http://qyu.sysykeji.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://fhs.hongshengwenyu.top

================================================================================
来源：http://otm.uphjek.com

D. 数组 / 列表 / 集合
来源：http://vpd.gzhubu.top

================================================================================
来源：http://ndu.haohaochexian.top

[D01] 创建数组 / 列表
来源：http://pse.shanyushiyangtech.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://ixr.ydzc1.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://fpt.aibaodan.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://sov.shanyushiyangtech.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://sjp.jqgufenzy.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://zve.jianghu66.top

Go:   arr := []int{1, 2, 3}
来源：http://sqj.daxiang520.top

Ruby: arr = [1, 2, 3]
来源：http://xcy.zhengqikj.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://due.dianchejie.cn

[D02] 追加元素到末尾
来源：http://oek.hfpthk.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://vqd.birdmap.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://jyy.sjlbkw.cn

JS:   arr.push(4);
来源：http://pnw.xylfe.cn

TS:   arr.push(4);
来源：http://rpy.xuanzx.com

Java: list.add(4);
来源：http://ttu.dashuyun.cn

Go:   arr = append(arr, 4)
来源：http://ypj.jinghuilouyu.cn

Ruby: arr << 4; arr.push(5)
来源：http://qmb.ybcxt.top

C#:   list.Add(4);
来源：http://ikp.ivvv.top

[D03] 在指定位置插入元素
来源：http://mdy.yuanzhike.top

Py:   arr.insert(0, 0)
来源：http://zix.hongshengwenyu.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://zfp.gaohongyu789.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://uix.nwbrower.top

TS:   arr.splice(0, 0, 0);
来源：http://jqf.yueranfly.top

Java: list.add(0, 0);
来源：http://ief.52xcode.cn

Go:   arr = append([]int{0}, arr...)
来源：http://gwc.xuanzx.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://lmp.yj202588.top

C#:   list.Insert(0, 0);
来源：http://dda.yj20258888.top

[D04] 删除元素
来源：http://uup.jinyuanbaomall.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://rqe.fengsongda.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://qtu.xuanzx.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://tqy.guowangkeji.top

TS:   arr.splice(0, 1);
来源：http://hjh.zhijiandao.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://xma.jiagoushi.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ebg.shanyushiyangtech.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://jok.mhx1999.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://msk.fzhhl.top

[D05] 访问与修改元素
来源：http://qpb.bjfxy.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://drj.feifeiyinyue.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://yzv.jinghuilouyu.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://gnx.quarkkingdee.top

TS:   arr[0]; arr.at(-1);
来源：http://hii.guowangkeji.top

Java: list.get(0); list.set(0, 9);
来源：http://ygt.hywenlv.cn

Go:   arr[0]; arr[0] = 9
来源：http://cxs.chenlongwang.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wqr.yj20258.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://clu.ydjk.org.cn

[D06] 数组长度
来源：http://ppy.hysaishi.cn

Py:   len(arr)
来源：http://giz.hnxiangtu.top

PHP:  count($arr);
来源：http://aon.tianlin.xyz

JS:   arr.length
来源：http://yir.gzhubu.top

TS:   arr.length
来源：http://iow.xuanzx.com

Java: list.size();
来源：http://yyc.c1oappe.top

Go:   len(arr)
来源：http://ttx.aibaodan.cn

Ruby: arr.length; arr.size
来源：http://nku.andypj.xyz

C#:   list.Count;
来源：http://tib.haohaochexian.top

[D07] 切片 / 取子数组
来源：http://zdt.shanyushiyangtech.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hia.ctjpmb.com

PHP:  array_slice($arr, 1, 3);
来源：http://izg.zdbjq.cn

JS:   arr.slice(1, 4);
来源：http://ssk.yuxming.cn

TS:   arr.slice(1, 4);
来源：http://iet.chenjidiqi.icu

Java: list.subList(1, 4);
来源：http://btm.jqgufenzy.top

Go:   arr[1:4]
来源：http://ecm.wangdashe.top

Ruby: arr[1, 3]
来源：http://glr.daxiang520.top

C#:   list.GetRange(1, 3);
来源：http://rev.shanyushiyangtech.top

[D08] 合并两个数组
来源：http://uib.yvedp.cn

Py:   a + b;  a.extend(b)
来源：http://mjv.hcnkem.com

PHP:  array_merge($a, $b);
来源：http://vbf.zycfv.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://lxw.pycfn.com

TS:   [...a, ...b];
来源：http://iim.havefunace.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://rlh.fanxiaobao.xyz

Go:   append(a, b...)
来源：http://afq.chenzaomai.com

Ruby: a + b;  a.concat(b)
来源：http://ean.redwolf501.top

C#:   a.Concat(b).ToList()
来源：http://xid.cucudq.cn

[D09] 排序（升序）
来源：http://ylj.yongpay.top

Py:   sorted(arr);  arr.sort()
来源：http://bgu.wangshuangyany.cn

PHP:  sort($arr);
来源：http://neq.gogol.net.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://gop.sysykeji.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://mju.yfazqb.com

Java: Collections.sort(list);  list.sort(null);
来源：http://cje.c1oappe.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://yye.jqgfzy.top

Ruby: arr.sort
来源：http://udu.yanxiufei.cn

C#:   list.Sort();
来源：http://nmr.xylfe.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://lrv.sjlbkw.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://cus.yanxiufei.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rql.epnwcf.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://cig.yonumen.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://kiq.vqdsnc.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ajx.wangshuangyany.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://opu.fktsv.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://idg.wangdashe.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://poi.xingfuxueyuan.xyz

[D11] 反转数组
来源：http://ols.cheryme.top

Py:   arr[::-1];  arr.reverse()
来源：http://smi.feifeiyinyue.top

PHP:  array_reverse($arr);
来源：http://dro.tian-w.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://tok.yfazqb.com

TS:   [...arr].reverse();
来源：http://owi.dashuyun.cn

Java: Collections.reverse(list);
来源：http://esv.wangshuangyany.cn

Go:   slices.Reverse(arr)
来源：http://qua.shzxlz.cn

Ruby: arr.reverse
来源：http://bis.jianghu66.top

C#:   list.Reverse();
来源：http://wxy.wangshuangyany.cn

[D12] 查找元素下标
来源：http://qhw.ctjpmb.com

Py:   arr.index(x);  x in arr
来源：http://ceb.ywan-chungtsiang.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://kwa.52xcode.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nmm.aizwys.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lrd.nwbrower.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://fzk.shangyingyoupin.top

Go:   slices.Index(arr, x)
来源：http://smt.fengsongda.top

Ruby: arr.index(x)
来源：http://msj.xingfuxueyuan.xyz

C#:   list.IndexOf(x);
来源：http://pps.yuxming.cn

[D13] 过滤（保留满足条件的）
来源：http://aqu.guowangkeji.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://rxq.tianlin.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wuo.dashuyun.cn

JS:   arr.filter(x => x > 3)
来源：http://xlx.sjlbkw.cn

TS:   arr.filter(x => x > 3)
来源：http://raq.316326.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://pth.redwolf501.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mik.sxryk.cn

Ruby: arr.select { |x| x > 3 }
来源：http://vrq.9152youxi.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://rdk.sweek.top

[D14] 映射转换（每个元素变形）
来源：http://kus.gogol.net.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://dpu.sjlbkw.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://agh.redwolf501.top

JS:   arr.map(x => x * 2)
来源：http://kgh.zhoulong.xyz

TS:   arr.map(x => x * 2)
来源：http://ifc.haohaochexian.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://psi.epnwcf.com

Go:   // 手写循环
来源：http://lhm.xingfuxueyuan.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://cgm.ydjk.org.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://hgq.zdbjq.cn

[D15] 去重
来源：http://uxt.chenzaomai.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ivn.daria6918.cn

PHP:  array_unique($arr);
来源：http://nwj.tianlin.xyz

JS:   [...new Set(arr)]
来源：http://tak.yonumen.top

TS:   [...new Set(arr)]
来源：http://lsw.yangfankeji.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://eqy.vehdjk.com

Go:   // 用 map[T]struct{} 手写
来源：http://ocj.hammf.cn

Ruby: arr.uniq
来源：http://ani.gotoacloud.top

C#:   list.Distinct().ToList()
来源：http://tdc.jinqigfzy.top

[D16] 求和与平均值
来源：http://cvr.ywan-chungtsiang.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ihx.aizwys.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://gjr.smart0.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://bip.haohaochexian.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://nvf.pycfn.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xsf.nanxinkj.top

Go:   // 手写循环累加
来源：http://rhj.bbcook.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mxu.cheryme.top

C#:   list.Sum();  list.Average()
来源：http://bte.tarul.cn

[D17] 最大值与最小值
来源：http://zbo.epnwcf.com

Py:   max(arr);  min(arr)
来源：http://kcq.hammf.cn

PHP:  max($arr);  min($arr);
来源：http://ksv.epnwcf.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://fiq.cashguo.top

TS:   Math.max(...arr);
来源：http://vpo.guowangkeji.top

Java: Collections.max(list);  Collections.min(list);
来源：http://mnb.quarkkingdee.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://zia.dianchejie.cn

Ruby: arr.max;  arr.min
来源：http://dnv.yfazqb.com

C#:   list.Max();  list.Min()
来源：http://guh.tarul.cn

[D18] 扁平化嵌套数组
来源：http://uin.fengsongda.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://czd.yongpay.top

PHP:  array_merge(...$nested);
来源：http://gdf.zhoulong.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://sma.svipenyu.cn

TS:   nested.flat();
来源：http://hvm.chenzaomai.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ukz.yj202588.top

Go:   // 手写双层循环
来源：http://eyw.ydzc1.top

Ruby: nested.flatten
来源：http://txy.0kj1m.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://uln.52xcode.cn

[D19] 按字段分组
来源：http://bqc.feifeiyinyue.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://lpr.9152youxi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mal.zdbjq.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://yya.smart0.xyz

TS:   Object.groupBy(arr, x => x.type)
来源：http://oxx.hcnkem.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://slc.jlsjyb.cn

Go:   // 手写 map[string][]T
来源：http://kmq.zhongyouzk.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://egm.yfazqb.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://rze.shzxlz.cn

[D20] 统计每个元素出现次数
来源：http://hhs.zhijiandao.cn

Py:   Counter(arr)
来源：http://myb.ybcxt.top

PHP:  array_count_values($arr);
来源：http://gtp.fengsongda.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jip.yfazqb.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fjq.sweek.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://gzj.9152youxi.cn

Go:   // 手写 map[T]int
来源：http://tur.uphjek.com

Ruby: arr.tally
来源：http://luf.zhengqikj.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://bly.hnqzz.top

[D21] 判断是否包含某元素
来源：http://qvg.nanxuanxn.top

Py:   x in arr
来源：http://fvc.gaohongyu789.top

PHP:  in_array($x, $arr, true);
来源：http://fhn.hnqzz.top

JS:   arr.includes(x)
来源：http://wqh.guowangkeji.top

TS:   arr.includes(x)
来源：http://eqn.hammf.cn

Java: list.contains(x)
来源：http://xko.smart0.xyz

Go:   slices.Contains(arr, x)
来源：http://vuo.yueranfly.top

Ruby: arr.include?(x)
来源：http://jen.sysykeji.top

C#:   list.Contains(x)
来源：http://gds.nanxuanxn.top

[D22] 复制数组（避免共享引用）
来源：http://hde.cucudq.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ctc.yonumen.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://dix.gogol.net.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://nbd.jlsjyb.cn

TS:   [...arr];
来源：http://gqi.yfazqb.com

Java: new ArrayList<>(list);
来源：http://ckm.hongshengwenyu.top

Go:   copied := append([]int(nil), arr...)
来源：http://brx.havefunace.top

Ruby: arr.dup;  arr.clone
来源：http://wbk.jlsjyb.cn

C#:   new List<int>(list);
来源：http://zco.jinqigfzy.top

[D23] reduce 累积计算
来源：http://glw.xziqi.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://grg.yj202588.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mxy.cqqwz.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tza.yj20258.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://efm.dianchejie.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://xid.cqqwz.cn

Go:   // 手写循环
来源：http://wuv.jqgufenzy.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://vkt.0kj1m.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wjh.bjfxy.top

[D24] 字典 / Map 基本操作
来源：http://unu.ydjk.org.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://eay.hammf.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mvc.yanxiufei.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://qpp.guannengcc.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wwz.fanxiaobao.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://gnq.gogol.net.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://jih.daria6918.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://cvi.iojbl.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://unn.haohaochexian.top

[D25] Set 集合去重与交并差
来源：http://fxk.daria6918.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mpf.xziqi.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://cza.zdqjudy.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://yun.wangdashe.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://rqt.wangshuangyany.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://shb.cqqwz.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://kjj.daria6918.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://zxi.daxiang520.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://fbe.sysykeji.top

[D26] 数组转字符串
来源：http://rbj.zhixingplan.top


<!-- 参考信息 -->