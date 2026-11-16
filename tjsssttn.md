代发 wailian999

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hjx.zhijiandao.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://kqi.hesvh.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://vuc.ctjpmb.com

[C09] 递归
来源：http://qng.jinghuilouyu.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://rii.chenzaomai.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://kna.jinyuanbaomall.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://srn.chenzaomai.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jry.gotoacloud.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://peq.ppjwa.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://qmj.tianlin.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://aij.xziqi.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://lhh.mhx1999.top

[C10] 变量作用域
来源：http://lva.jyoumei.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wca.daria6918.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://dgc.zdbjq.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ddg.0kj1m.cn

TS:   同 JS
来源：http://tqn.hesvh.cn

Java: 方法内为块级作用域
来源：http://zbe.chenzaomai.com

Go:   花括号块级作用域
来源：http://xnr.hnqzz.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://sgf.wangshuangyany.cn

C#:   块级作用域
来源：http://dlt.yangfankeji.com

[C11] 模块导入与导出
来源：http://tec.ctjpmb.com

Py:   from module import func
来源：http://nps.xuetiantiany.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://yay.zdbjq.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://sqf.yonumen.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://rld.fanxiaobao.xyz

Java: import java.util.List;
来源：http://scq.zhijiandao.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://beg.xylfe.cn

Ruby: require "json"; require_relative "./util"
来源：http://xmt.fengsongda.top

C#:   using System.Text;
来源：http://lve.dashuyun.cn

[C12] 立即执行函数 IIFE
来源：http://pbo.yj20258888.top

Py:   (lambda: print("run"))()
来源：http://fer.kuanghao11.cn

PHP:  (function () { echo "run"; })();
来源：http://iis.hnxiangtu.top

JS:   (() => { console.log("run"); })();
来源：http://lcp.fanxiaobao.xyz

TS:   (() => { console.log("run"); })();
来源：http://klm.epnwcf.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://cga.xuetiantiany.cn

Go:   func() { fmt.Println("run") }()
来源：http://qmc.yj202588.top

Ruby: -> { puts "run" }.call
来源：http://vde.nwbrower.top

C#:   // 无 IIFE：用静态构造函数
来源：http://mvs.gaohongyu789.top

[C13] 类型声明 / 类型注解
来源：http://jmh.jinyuanbaomall.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hlf.guannengcc.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://idp.xziqi.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://dan.aibaodan.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qnd.sysykeji.top

Java: int add(int a, int b) { return a + b; }
来源：http://rrr.xuetiantiany.cn

Go:   func add(a, b int) int
来源：http://xor.yueranfly.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://sqx.smart0.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://kwq.cdnleiting.top

[C14] 泛型函数
来源：http://fgp.ydzc1.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://btu.jiagoushi.top

PHP:  // 无泛型
来源：http://iqy.aizwys.cn

JS:   // 无泛型
来源：http://sjv.daria6918.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ema.hysaishi.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hru.nanxuanxn.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://izw.svipenyu.cn

Ruby: # 无泛型
来源：http://scd.316326.xyz

C#:   static T First<T>(List<T> items) => items[0];
来源：http://pua.xingfuxueyuan.xyz

[C15] 解构 / 展开参数
来源：http://hch.yj20258888.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://str.svipenyu.cn

PHP:  [$a, $b] = $pair;
来源：http://zec.sweek.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xpi.ivvv.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://zqx.xuetiantiany.cn

Java: // 无解构
来源：http://krh.yuxming.cn

Go:   // 无解构
来源：http://urd.nanxinkj.top

Ruby: a, b = pair
来源：http://rty.zhixingplan.top

C#:   var (a, b) = pair;
来源：http://xck.epnwcf.com

[C16] 函数 / 方法重载
来源：http://rwo.xinyue.icu

Py:   # 无重载：用默认参数或 *args 变通
来源：http://gzm.xinyue.icu

PHP:  // 无重载
来源：http://gce.ywan-chungtsiang.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://msk.yanxiufei.cn

TS:   // 用联合类型或重载签名声明
来源：http://awe.nwbrower.top

Java: void f(int a) {}  void f(String a) {}
来源：http://wfj.yueranfly.top

Go:   // 无重载：用不同函数名
来源：http://cbk.0kj1m.cn

Ruby: # 无重载：靠动态参数
来源：http://bez.yanxiufei.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://lil.fktsv.cn

================================================================================
来源：http://cuw.jinqigufen.top

D. 数组 / 列表 / 集合
来源：http://vbc.ivvv.top

================================================================================
来源：http://rwq.ywan-chungtsiang.top

[D01] 创建数组 / 列表
来源：http://xxg.cdnleiting.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://wur.daxiang520.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://shh.fktsv.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://kdi.jinqigufen.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://qgd.iojbl.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://iqc.gaohongyu789.top

Go:   arr := []int{1, 2, 3}
来源：http://gvc.nanxinkj.top

Ruby: arr = [1, 2, 3]
来源：http://xsz.fengsongda.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://qwq.gaohongyu789.top

[D02] 追加元素到末尾
来源：http://len.andypj.xyz

Py:   arr.append(4); arr.extend([5, 6])
来源：http://iyu.wangdashe.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mzv.daxiang520.top

JS:   arr.push(4);
来源：http://mdr.smart0.xyz

TS:   arr.push(4);
来源：http://blc.tanke756.top

Java: list.add(4);
来源：http://neu.mhx1999.top

Go:   arr = append(arr, 4)
来源：http://yfe.52xcode.cn

Ruby: arr << 4; arr.push(5)
来源：http://kmb.shangyingyoupin.top

C#:   list.Add(4);
来源：http://bnm.daria6918.cn

[D03] 在指定位置插入元素
来源：http://rqr.yonumen.top

Py:   arr.insert(0, 0)
来源：http://uor.dashuyun.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://zxb.yuxming.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://pbg.hnqzz.top

TS:   arr.splice(0, 0, 0);
来源：http://udi.zycfv.cn

Java: list.add(0, 0);
来源：http://asc.fzhhl.top

Go:   arr = append([]int{0}, arr...)
来源：http://hip.uphjek.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://opf.sxryk.cn

C#:   list.Insert(0, 0);
来源：http://alo.hnqzz.top

[D04] 删除元素
来源：http://pgi.zycfv.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://caj.xylfe.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://rqs.0kj1m.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ouj.0kj1m.cn

TS:   arr.splice(0, 1);
来源：http://gar.yonumen.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://pdj.gaohongyu789.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://vbf.yuanzhike.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ocr.wangdashe.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ocn.hysaishi.cn

[D05] 访问与修改元素
来源：http://qmr.mhx1999.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://geg.chenzaomai.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://zej.cucudq.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://rpq.shuidangran.top

TS:   arr[0]; arr.at(-1);
来源：http://hvv.xylfe.cn

Java: list.get(0); list.set(0, 9);
来源：http://wxy.shangyingyoupin.top

Go:   arr[0]; arr[0] = 9
来源：http://wwt.guowangkeji.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://shr.quarkkingdee.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://qyk.svipenyu.cn

[D06] 数组长度
来源：http://jgt.xylfe.cn

Py:   len(arr)
来源：http://hoo.tian-w.cn

PHP:  count($arr);
来源：http://ulk.hammf.cn

JS:   arr.length
来源：http://pni.jinqigufen.top

TS:   arr.length
来源：http://yzt.bbcook.cn

Java: list.size();
来源：http://fku.ivvv.top

Go:   len(arr)
来源：http://rnw.ivvv.top

Ruby: arr.length; arr.size
来源：http://upx.birdmap.top

C#:   list.Count;
来源：http://tev.yj202588.top

[D07] 切片 / 取子数组
来源：http://vuz.yfazqb.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://dvd.quarkkingdee.top

PHP:  array_slice($arr, 1, 3);
来源：http://eqa.yangfankeji.com

JS:   arr.slice(1, 4);
来源：http://orv.zhixingplan.top

TS:   arr.slice(1, 4);
来源：http://hny.yangfankeji.com

Java: list.subList(1, 4);
来源：http://sen.hcnkem.com

Go:   arr[1:4]
来源：http://sso.yanxiufei.cn

Ruby: arr[1, 3]
来源：http://ujh.meibo888.top

C#:   list.GetRange(1, 3);
来源：http://kmc.chenjidiqi.icu

[D08] 合并两个数组
来源：http://ppd.havefunace.top

Py:   a + b;  a.extend(b)
来源：http://mbo.chenjidiqi.icu

PHP:  array_merge($a, $b);
来源：http://shm.bbcook.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://fjp.dianchejie.cn

TS:   [...a, ...b];
来源：http://iit.fzhhl.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://gkg.9152youxi.cn

Go:   append(a, b...)
来源：http://lxa.vehdjk.com

Ruby: a + b;  a.concat(b)
来源：http://okn.kuanghao11.cn

C#:   a.Concat(b).ToList()
来源：http://vuv.pycfn.com

[D09] 排序（升序）
来源：http://aav.vehdjk.com

Py:   sorted(arr);  arr.sort()
来源：http://ilr.ehwqpu.com

PHP:  sort($arr);
来源：http://vft.jqgfzy.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://qvh.fzhhl.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://met.0kj1m.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://kqo.xziqi.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wvm.vqdsnc.cn

Ruby: arr.sort
来源：http://vnl.jinyuanbaomall.cn

C#:   list.Sort();
来源：http://jss.tian-w.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://cyu.316326.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://uuh.yj202588.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jtp.zycfv.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://bkr.xuanzx.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://nkd.hywenlv.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ydq.aibaodan.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mwm.guowangkeji.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://bdj.jinghuilouyu.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qmj.cucudq.cn

[D11] 反转数组
来源：http://ayi.nanxinkj.top

Py:   arr[::-1];  arr.reverse()
来源：http://bwq.jinqigufen.top

PHP:  array_reverse($arr);
来源：http://jrk.jinqigufen.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://een.hcnkem.com

TS:   [...arr].reverse();
来源：http://lvl.zhaomingkeji.xyz

Java: Collections.reverse(list);
来源：http://lao.zdbjq.cn

Go:   slices.Reverse(arr)
来源：http://jef.cqqwz.cn

Ruby: arr.reverse
来源：http://nyx.sysykeji.top

C#:   list.Reverse();
来源：http://dku.fengsongda.top

[D12] 查找元素下标
来源：http://utq.hesvh.cn

Py:   arr.index(x);  x in arr
来源：http://qql.hammf.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ahx.tianlin.xyz

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rdk.smart0.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yub.zhongyouzk.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://rfm.zhengqikj.top

Go:   slices.Index(arr, x)
来源：http://xon.zhongyouzk.top

Ruby: arr.index(x)
来源：http://wmc.ywan-chungtsiang.top

C#:   list.IndexOf(x);
来源：http://iih.316326.xyz

[D13] 过滤（保留满足条件的）
来源：http://mds.fktsv.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://aok.gogol.net.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ezz.tian-w.cn

JS:   arr.filter(x => x > 3)
来源：http://zoy.svipenyu.cn

TS:   arr.filter(x => x > 3)
来源：http://lqx.ydzc1.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://epq.yangfankeji.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://guk.cashguo.top

Ruby: arr.select { |x| x > 3 }
来源：http://aia.dashuyun.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://uqd.jqgfzy.top

[D14] 映射转换（每个元素变形）
来源：http://bje.andypj.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://kxo.ivvv.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://umw.0kj1m.cn

JS:   arr.map(x => x * 2)
来源：http://lmc.mhx1999.top

TS:   arr.map(x => x * 2)
来源：http://ajp.hnqzz.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://gfg.pengpengdd.cyou

Go:   // 手写循环
来源：http://lmn.zhixingplan.top

Ruby: arr.map { |x| x * 2 }
来源：http://zzh.ivvv.top

C#:   list.Select(x => x * 2).ToList()
来源：http://xuo.feifeiyinyue.top

[D15] 去重
来源：http://jgo.dianchejie.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ign.svipenyu.cn

PHP:  array_unique($arr);
来源：http://zcw.nanxinkj.top

JS:   [...new Set(arr)]
来源：http://vja.hywenlv.cn

TS:   [...new Set(arr)]
来源：http://wxl.jinqigufen.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://sew.yonumen.top

Go:   // 用 map[T]struct{} 手写
来源：http://pvj.sxryk.cn

Ruby: arr.uniq
来源：http://bwh.fktsv.cn

C#:   list.Distinct().ToList()
来源：http://mfz.wangdashe.top

[D16] 求和与平均值
来源：http://mls.jqgfzy.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hwb.meibo888.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://zue.jinghuilouyu.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://lwv.zdbjq.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://puk.cqqwz.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wsp.fengsongda.top

Go:   // 手写循环累加
来源：http://ceb.pengpengdd.cyou

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://tkl.guannengcc.top

C#:   list.Sum();  list.Average()
来源：http://kkv.yanxiufei.cn

[D17] 最大值与最小值
来源：http://uew.hfpthk.cn

Py:   max(arr);  min(arr)
来源：http://uhs.yuanzhike.top

PHP:  max($arr);  min($arr);
来源：http://lup.hnqzz.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ngf.yfazqb.com

TS:   Math.max(...arr);
来源：http://qci.9152youxi.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://nuc.wangshuangyany.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://lht.yangfankeji.com

Ruby: arr.max;  arr.min
来源：http://nqq.shanyushiyangtech.top

C#:   list.Max();  list.Min()
来源：http://pwy.gotoacloud.top

[D18] 扁平化嵌套数组
来源：http://nrk.kuanghao11.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://rxu.guannengcc.top

PHP:  array_merge(...$nested);
来源：http://kij.guannengcc.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://qcq.xziqi.cn

TS:   nested.flat();
来源：http://esg.bjfxy.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://xpc.jinghuilouyu.cn

Go:   // 手写双层循环
来源：http://wpk.ydzc1.top

Ruby: nested.flatten
来源：http://zmg.tian-w.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://wqs.hysaishi.cn

[D19] 按字段分组
来源：http://rab.52xcode.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ags.yueranfly.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://nqt.zhixingplan.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://pxb.jqgfzy.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://wlw.yvedp.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://jge.fehbvm.com

Go:   // 手写 map[string][]T
来源：http://ylh.yuxming.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://kpv.hongshengwenyu.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://tcj.hysaishi.cn

[D20] 统计每个元素出现次数
来源：http://yag.fehbvm.com

Py:   Counter(arr)
来源：http://prw.yuxming.cn

PHP:  array_count_values($arr);
来源：http://fng.jyoumei.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ndc.dashuyun.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vep.gogol.net.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ruu.hammf.cn

Go:   // 手写 map[T]int
来源：http://cdh.quarkkingdee.top

Ruby: arr.tally
来源：http://pmj.ctjpmb.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://yng.epnwcf.com

[D21] 判断是否包含某元素
来源：http://uaf.zhongyouzk.top

Py:   x in arr
来源：http://odw.xziqi.cn

PHP:  in_array($x, $arr, true);
来源：http://yln.svipenyu.cn

JS:   arr.includes(x)
来源：http://jvm.nwbrower.top

TS:   arr.includes(x)
来源：http://grd.gogol.net.cn

Java: list.contains(x)
来源：http://zcd.hnxiangtu.top

Go:   slices.Contains(arr, x)
来源：http://kfq.bbcook.cn

Ruby: arr.include?(x)
来源：http://nuw.yfazqb.com

C#:   list.Contains(x)
来源：http://cya.feifeiyinyue.top

[D22] 复制数组（避免共享引用）
来源：http://oza.gaohongyu789.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://rjj.shangyingyoupin.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://fkx.ivvv.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://lui.vehdjk.com

TS:   [...arr];
来源：http://lnt.epnwcf.com

Java: new ArrayList<>(list);
来源：http://pcj.52xcode.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ykb.fehbvm.com

Ruby: arr.dup;  arr.clone
来源：http://fdo.zhaomingkeji.xyz

C#:   new List<int>(list);
来源：http://kln.quarkkingdee.top

[D23] reduce 累积计算
来源：http://ioc.jqgfzy.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://bul.yangfankeji.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hgf.nanxuanxn.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nue.jyoumei.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ydo.zhiwuduotai.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://suo.daxiang520.top

Go:   // 手写循环
来源：http://zcr.haohaochexian.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://kjn.jiagoushi.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mxi.xylfe.cn

[D24] 字典 / Map 基本操作
来源：http://qhu.zhongyouzk.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ztz.chenjidiqi.icu

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://xlh.fehbvm.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ojf.zhengqikj.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ags.cashguo.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wky.snrcjt.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://gep.sxryk.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hke.chenlongwang.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://opf.nanxuanxn.top

[D25] Set 集合去重与交并差
来源：http://tvg.yanxiufei.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hee.nanxuanxn.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://aws.shanyushiyangtech.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://cfb.gzhubu.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://kwi.svipenyu.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://irn.hesvh.cn


<!-- 参考信息 -->