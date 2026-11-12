代发 wailian999

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ksm.wangshuangyany.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://cgm.nwbrower.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://xsa.andypj.xyz

[C09] 递归
来源：http://seu.bjfxy.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wld.xylfe.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ilu.jqgufenzy.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://spe.hammf.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wob.dashuyun.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ltw.aibaodan.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://itq.jinyuanbaomall.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://nxp.redwolf501.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hbm.yj202588.top

[C10] 变量作用域
来源：http://gey.zhaomingkeji.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://lva.jlsjyb.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://bru.hfpthk.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://jpb.hywenlv.cn

TS:   同 JS
来源：http://hxe.daxiang520.top

Java: 方法内为块级作用域
来源：http://epv.ehwqpu.com

Go:   花括号块级作用域
来源：http://kvs.zhiwuduotai.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://cjr.sxryk.cn

C#:   块级作用域
来源：http://hfa.zycfv.cn

[C11] 模块导入与导出
来源：http://rxq.tarul.cn

Py:   from module import func
来源：http://uyt.zdqjudy.top

PHP:  require "file.php";  或 use App\Service;
来源：http://leu.xziqi.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://zuc.kuanghao11.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ncv.tanke756.top

Java: import java.util.List;
来源：http://rol.gaohongyu789.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://quz.zdbjq.cn

Ruby: require "json"; require_relative "./util"
来源：http://bzi.zhixingplan.top

C#:   using System.Text;
来源：http://svv.9152youxi.cn

[C12] 立即执行函数 IIFE
来源：http://fgx.xziqi.cn

Py:   (lambda: print("run"))()
来源：http://cuj.daria6918.cn

PHP:  (function () { echo "run"; })();
来源：http://fel.yj20258888.top

JS:   (() => { console.log("run"); })();
来源：http://fip.yuxming.cn

TS:   (() => { console.log("run"); })();
来源：http://pxl.shanyushiyangkeji.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://lie.snrcjt.cn

Go:   func() { fmt.Println("run") }()
来源：http://awn.9152youxi.cn

Ruby: -> { puts "run" }.call
来源：http://cwm.yueranfly.top

C#:   // 无 IIFE：用静态构造函数
来源：http://dqc.hysaishi.cn

[C13] 类型声明 / 类型注解
来源：http://pke.sjlbkw.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://obn.yangfankeji.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://inu.uphjek.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://xrb.sjlbkw.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fen.kuanghao11.cn

Java: int add(int a, int b) { return a + b; }
来源：http://jip.zhixingplan.top

Go:   func add(a, b int) int
来源：http://lfl.mhx1999.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://btj.yj20258.top

C#:   int Add(int a, int b) => a + b;
来源：http://qgj.fzhhl.top

[C14] 泛型函数
来源：http://qdx.cheryme.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://vfg.yj202588.top

PHP:  // 无泛型
来源：http://nfr.snrcjt.cn

JS:   // 无泛型
来源：http://nbx.pengpengdd.cyou

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mmi.yj20258.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://pql.aizwys.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://jcp.redwolf501.top

Ruby: # 无泛型
来源：http://dxd.tian-w.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://qcy.yuanzhike.top

[C15] 解构 / 展开参数
来源：http://yaq.smart0.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xhu.hnqzz.top

PHP:  [$a, $b] = $pair;
来源：http://vjq.yfazqb.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://jzw.shuidangran.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://cer.chenjidiqi.icu

Java: // 无解构
来源：http://ign.yj20258888.top

Go:   // 无解构
来源：http://dyg.jqgufenzy.top

Ruby: a, b = pair
来源：http://cgi.zhaomingkeji.xyz

C#:   var (a, b) = pair;
来源：http://eyo.tianlin.xyz

[C16] 函数 / 方法重载
来源：http://zga.mhx1999.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vst.zhongyouzk.top

PHP:  // 无重载
来源：http://iqy.ydzc1.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://ffb.zycfv.cn

TS:   // 用联合类型或重载签名声明
来源：http://gte.kuanghao11.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://djj.jianghu66.top

Go:   // 无重载：用不同函数名
来源：http://mae.birdmap.top

Ruby: # 无重载：靠动态参数
来源：http://lmh.nanxinkj.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://tqn.pycfn.com

================================================================================
来源：http://bax.pengpengdd.cyou

D. 数组 / 列表 / 集合
来源：http://mjp.316326.xyz

================================================================================
来源：http://ota.sweek.top

[D01] 创建数组 / 列表
来源：http://cfg.jlsjyb.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://nxx.wangdashe.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://nru.xylfe.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://itg.yuxming.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://nwy.hcnkem.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://bky.jinqigufen.top

Go:   arr := []int{1, 2, 3}
来源：http://brq.nwbrower.top

Ruby: arr = [1, 2, 3]
来源：http://eag.zhoulong.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://zac.hysaishi.cn

[D02] 追加元素到末尾
来源：http://arl.yangfankeji.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://doq.hnxiangtu.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://kcq.havefunace.top

JS:   arr.push(4);
来源：http://opv.ydjk.org.cn

TS:   arr.push(4);
来源：http://hkj.jqgufenzy.top

Java: list.add(4);
来源：http://nqj.sjlbkw.cn

Go:   arr = append(arr, 4)
来源：http://uyp.fehbvm.com

Ruby: arr << 4; arr.push(5)
来源：http://erv.zhijiandao.cn

C#:   list.Add(4);
来源：http://hip.kuanghao11.cn

[D03] 在指定位置插入元素
来源：http://tmy.fktsv.cn

Py:   arr.insert(0, 0)
来源：http://wyf.cdnleiting.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://htt.52xcode.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://lyz.tianlin.xyz

TS:   arr.splice(0, 0, 0);
来源：http://trn.shuidangran.top

Java: list.add(0, 0);
来源：http://lxo.gzhubu.top

Go:   arr = append([]int{0}, arr...)
来源：http://qag.yj20258.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://rkd.zhoulong.xyz

C#:   list.Insert(0, 0);
来源：http://agz.feifeiyinyue.top

[D04] 删除元素
来源：http://itd.jinqigufen.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://zze.gaohongyu789.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://aia.chenjidiqi.icu

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://pqy.c1oappe.top

TS:   arr.splice(0, 1);
来源：http://auh.zhoulong.xyz

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://alx.zycfv.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://dhz.hywenlv.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ioz.zhengqikj.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://qki.xuanzx.com

[D05] 访问与修改元素
来源：http://gmu.pycfn.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://dfm.jinqigufen.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://xje.tanke756.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://pge.vqdsnc.cn

TS:   arr[0]; arr.at(-1);
来源：http://mre.yongpay.top

Java: list.get(0); list.set(0, 9);
来源：http://vfs.hongshengwenyu.top

Go:   arr[0]; arr[0] = 9
来源：http://opx.jinyuanbaomall.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://rig.yueranfly.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ueb.yueranfly.top

[D06] 数组长度
来源：http://coa.yueranfly.top

Py:   len(arr)
来源：http://gwa.sufxvd.cn

PHP:  count($arr);
来源：http://mxt.zhaomingkeji.xyz

JS:   arr.length
来源：http://ska.yj20258.top

TS:   arr.length
来源：http://vkz.cucudq.cn

Java: list.size();
来源：http://znk.jqgufenzy.top

Go:   len(arr)
来源：http://uvr.9152youxi.cn

Ruby: arr.length; arr.size
来源：http://djb.nwbrower.top

C#:   list.Count;
来源：http://vgt.smart0.xyz

[D07] 切片 / 取子数组
来源：http://hyb.jyoumei.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://nwg.aibaodan.cn

PHP:  array_slice($arr, 1, 3);
来源：http://htt.andypj.xyz

JS:   arr.slice(1, 4);
来源：http://phn.guannengcc.top

TS:   arr.slice(1, 4);
来源：http://sup.aibaodan.cn

Java: list.subList(1, 4);
来源：http://igc.cucudq.cn

Go:   arr[1:4]
来源：http://flo.ivvv.top

Ruby: arr[1, 3]
来源：http://emp.vqdsnc.cn

C#:   list.GetRange(1, 3);
来源：http://kwi.bbcook.cn

[D08] 合并两个数组
来源：http://gen.sweek.top

Py:   a + b;  a.extend(b)
来源：http://ymw.hfpthk.cn

PHP:  array_merge($a, $b);
来源：http://yxh.ctjpmb.com

JS:   [...a, ...b];  a.concat(b);
来源：http://rjv.hesvh.cn

TS:   [...a, ...b];
来源：http://kjp.cheryme.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hxu.yueranfly.top

Go:   append(a, b...)
来源：http://aiz.hywenlv.cn

Ruby: a + b;  a.concat(b)
来源：http://wwk.zhijiandao.cn

C#:   a.Concat(b).ToList()
来源：http://miv.hcnkem.com

[D09] 排序（升序）
来源：http://yeh.cheryme.top

Py:   sorted(arr);  arr.sort()
来源：http://ahx.dashuyun.cn

PHP:  sort($arr);
来源：http://ulw.snrcjt.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://kqg.yvedp.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://akl.hysaishi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://hnm.sjlbkw.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://zcj.xziqi.cn

Ruby: arr.sort
来源：http://vpn.haohaochexian.top

C#:   list.Sort();
来源：http://auu.jqgufenzy.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://glq.chenzaomai.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://cqf.ctjpmb.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qzr.ehwqpu.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://pxn.gogol.net.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://naa.vqdsnc.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://vtt.yj20258.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://bou.kuanghao11.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://bko.fzhhl.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://jot.daria6918.cn

[D11] 反转数组
来源：http://gba.yj20258888.top

Py:   arr[::-1];  arr.reverse()
来源：http://gdl.gotoacloud.top

PHP:  array_reverse($arr);
来源：http://elq.snrcjt.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://nat.xylfe.cn

TS:   [...arr].reverse();
来源：http://ytf.hnxiangtu.top

Java: Collections.reverse(list);
来源：http://wgf.shanyushiyangtech.top

Go:   slices.Reverse(arr)
来源：http://ctk.xziqi.cn

Ruby: arr.reverse
来源：http://hiu.gaohongyu789.top

C#:   list.Reverse();
来源：http://tks.yueranfly.top

[D12] 查找元素下标
来源：http://hnm.wangshuangyany.cn

Py:   arr.index(x);  x in arr
来源：http://dzo.hnxiangtu.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://fpa.zhijiandao.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vnc.chenzaomai.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zxb.xinyue.icu

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://pyk.zhongyouzk.top

Go:   slices.Index(arr, x)
来源：http://cdx.jinqigfzy.top

Ruby: arr.index(x)
来源：http://iyc.yangfankeji.com

C#:   list.IndexOf(x);
来源：http://mhb.9152youxi.cn

[D13] 过滤（保留满足条件的）
来源：http://mlh.fanxiaobao.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://tee.kuanghao11.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ehk.haohaochexian.top

JS:   arr.filter(x => x > 3)
来源：http://ham.316326.xyz

TS:   arr.filter(x => x > 3)
来源：http://qnn.shanyushiyangkeji.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mhd.yueranfly.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://yyh.yvedp.cn

Ruby: arr.select { |x| x > 3 }
来源：http://qtd.nanxuanxn.top

C#:   list.Where(x => x > 3).ToList()
来源：http://nuk.pengpengdd.cyou

[D14] 映射转换（每个元素变形）
来源：http://twl.shanyushiyangtech.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://jrq.52xcode.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mvu.daria6918.cn

JS:   arr.map(x => x * 2)
来源：http://upj.gzhubu.top

TS:   arr.map(x => x * 2)
来源：http://uet.gzhubu.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://yxn.guowangkeji.top

Go:   // 手写循环
来源：http://dgk.jinyuanbaomall.cn

Ruby: arr.map { |x| x * 2 }
来源：http://zbz.hcnkem.com

C#:   list.Select(x => x * 2).ToList()
来源：http://adt.shanyushiyangkeji.top

[D15] 去重
来源：http://wdz.shuidangran.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ofg.gaohongyu789.top

PHP:  array_unique($arr);
来源：http://vpc.zdqjudy.top

JS:   [...new Set(arr)]
来源：http://odh.hongshengwenyu.top

TS:   [...new Set(arr)]
来源：http://wqd.yj202588.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://txo.guannengcc.top

Go:   // 用 map[T]struct{} 手写
来源：http://kdb.xinyue.icu

Ruby: arr.uniq
来源：http://wnn.yueranfly.top

C#:   list.Distinct().ToList()
来源：http://qqf.wangshuangyany.cn

[D16] 求和与平均值
来源：http://oif.hnxiangtu.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://xnx.cqqwz.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://cxb.kuanghao11.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://eis.9152youxi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://xmf.svipenyu.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ssh.nanxinkj.top

Go:   // 手写循环累加
来源：http://ajo.birdmap.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://xdj.zycfv.cn

C#:   list.Sum();  list.Average()
来源：http://cby.ydzc1.top

[D17] 最大值与最小值
来源：http://elg.pycfn.com

Py:   max(arr);  min(arr)
来源：http://pug.yuxming.cn

PHP:  max($arr);  min($arr);
来源：http://owy.hongshengwenyu.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://erd.chenjidiqi.icu

TS:   Math.max(...arr);
来源：http://azg.hcnkem.com

Java: Collections.max(list);  Collections.min(list);
来源：http://ril.xylfe.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hyg.nwbrower.top

Ruby: arr.max;  arr.min
来源：http://pov.vehdjk.com

C#:   list.Max();  list.Min()
来源：http://uht.hysaishi.cn

[D18] 扁平化嵌套数组
来源：http://pvl.tarul.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wsm.pengpengdd.cyou

PHP:  array_merge(...$nested);
来源：http://omg.yfazqb.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://xeq.hongshengwenyu.top

TS:   nested.flat();
来源：http://jlf.nwbrower.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://vdk.0kj1m.cn

Go:   // 手写双层循环
来源：http://kiv.kuanghao11.cn

Ruby: nested.flatten
来源：http://kuf.iojbl.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://fny.cucudq.cn

[D19] 按字段分组
来源：http://uvw.jinyuanbaomall.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ykl.jinqigufen.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://fco.redwolf501.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ynt.fanxiaobao.xyz

TS:   Object.groupBy(arr, x => x.type)
来源：http://tro.dianchejie.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://kzs.tarul.cn

Go:   // 手写 map[string][]T
来源：http://sbm.52xcode.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://jyi.0kj1m.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wdg.yvedp.cn

[D20] 统计每个元素出现次数
来源：http://utg.nanxinkj.top

Py:   Counter(arr)
来源：http://ruu.jianghu66.top

PHP:  array_count_values($arr);
来源：http://tjm.cqqwz.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wek.nanxinkj.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mlg.guowangkeji.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://adt.zhaomingkeji.xyz

Go:   // 手写 map[T]int
来源：http://mnc.wangdashe.top

Ruby: arr.tally
来源：http://xfp.yj20258.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://iij.havefunace.top

[D21] 判断是否包含某元素
来源：http://lhg.gzhubu.top

Py:   x in arr
来源：http://nac.fktsv.cn

PHP:  in_array($x, $arr, true);
来源：http://shk.sufxvd.cn

JS:   arr.includes(x)
来源：http://pib.xingfuxueyuan.xyz

TS:   arr.includes(x)
来源：http://bqa.yj20258888.top

Java: list.contains(x)
来源：http://lco.hammf.cn

Go:   slices.Contains(arr, x)
来源：http://ghd.tarul.cn

Ruby: arr.include?(x)
来源：http://vcy.xinyue.icu

C#:   list.Contains(x)
来源：http://vzu.xuanzx.com

[D22] 复制数组（避免共享引用）
来源：http://cbq.aizwys.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://pkv.jlsjyb.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://sxw.yonumen.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://yhp.yuxming.cn

TS:   [...arr];
来源：http://kqx.jyoumei.cn

Java: new ArrayList<>(list);
来源：http://yeb.xylfe.cn

Go:   copied := append([]int(nil), arr...)
来源：http://fbw.gogol.net.cn

Ruby: arr.dup;  arr.clone
来源：http://cja.shangyingyoupin.top

C#:   new List<int>(list);
来源：http://rlg.dianchejie.cn

[D23] reduce 累积计算
来源：http://bii.yueranfly.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ecf.bbcook.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://esk.ehwqpu.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ews.hcnkem.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vrf.feifeiyinyue.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://tgy.316326.xyz

Go:   // 手写循环
来源：http://lzo.fengsongda.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ylf.sjlbkw.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://xta.zycfv.cn

[D24] 字典 / Map 基本操作
来源：http://kpu.svipenyu.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ttt.zhengqikj.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ejs.andypj.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://vog.hesvh.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ldq.pengpengdd.cyou

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://vho.yj20258.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://fcf.ybcxt.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://uqg.316326.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://giw.shangyingyoupin.top

[D25] Set 集合去重与交并差
来源：http://boi.sufxvd.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mhg.shuidangran.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://igo.jinqigufen.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://bvc.fengsongda.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ecr.yuanzhike.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://iyg.yvedp.cn


<!-- 参考信息 -->