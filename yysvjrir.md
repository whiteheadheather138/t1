代发 wailian999

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://pgo.nanxinkj.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hex.chenlongwang.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://iar.xuanzx.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://tnr.sjlbkw.cn

[C10] 变量作用域
来源：http://jce.zdbjq.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mab.bbcook.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wzq.shangyingyoupin.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://zgn.yongpay.top

TS:   同 JS
来源：http://pim.ehwqpu.com

Java: 方法内为块级作用域
来源：http://lnr.pycfn.com

Go:   花括号块级作用域
来源：http://amn.shuidangran.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ody.zdqjudy.top

C#:   块级作用域
来源：http://zyr.zhijiandao.cn

[C11] 模块导入与导出
来源：http://seh.gotoacloud.top

Py:   from module import func
来源：http://anq.zhixingplan.top

PHP:  require "file.php";  或 use App\Service;
来源：http://dqy.jinyuanbaomall.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://fej.zhongyouzk.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://zrf.ybcxt.top

Java: import java.util.List;
来源：http://jba.fehbvm.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ivt.cucudq.cn

Ruby: require "json"; require_relative "./util"
来源：http://kbr.hongshengwenyu.top

C#:   using System.Text;
来源：http://ype.9152youxi.cn

[C12] 立即执行函数 IIFE
来源：http://pyg.pycfn.com

Py:   (lambda: print("run"))()
来源：http://bzx.sufxvd.cn

PHP:  (function () { echo "run"; })();
来源：http://eri.hongshengwenyu.top

JS:   (() => { console.log("run"); })();
来源：http://gqw.zhengqikj.top

TS:   (() => { console.log("run"); })();
来源：http://czu.zhaomingkeji.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://vbi.birdmap.top

Go:   func() { fmt.Println("run") }()
来源：http://tlk.52xcode.cn

Ruby: -> { puts "run" }.call
来源：http://vsf.yj20258888.top

C#:   // 无 IIFE：用静态构造函数
来源：http://nna.xziqi.cn

[C13] 类型声明 / 类型注解
来源：http://uoz.xziqi.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ljb.shzxlz.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vra.feifeiyinyue.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://eww.hysaishi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://iuh.fktsv.cn

Java: int add(int a, int b) { return a + b; }
来源：http://icv.yfazqb.com

Go:   func add(a, b int) int
来源：http://pzk.nwbrower.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://evm.zhaomingkeji.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://xsu.guannengcc.top

[C14] 泛型函数
来源：http://sxh.zhoulong.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://yef.sysykeji.top

PHP:  // 无泛型
来源：http://duk.ydjk.org.cn

JS:   // 无泛型
来源：http://dxu.ybcxt.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://zcn.quarkkingdee.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://etk.yfazqb.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://qzx.sweek.top

Ruby: # 无泛型
来源：http://ztm.dashuyun.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://msj.zhijiandao.cn

[C15] 解构 / 展开参数
来源：http://myp.0kj1m.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://giy.shuidangran.top

PHP:  [$a, $b] = $pair;
来源：http://dgt.sjlbkw.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ikj.quarkkingdee.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://vey.guannengcc.top

Java: // 无解构
来源：http://hkz.yanxiufei.cn

Go:   // 无解构
来源：http://amw.birdmap.top

Ruby: a, b = pair
来源：http://pgv.jqgfzy.top

C#:   var (a, b) = pair;
来源：http://feo.fzhhl.top

[C16] 函数 / 方法重载
来源：http://fsr.sufxvd.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://quf.zycfv.cn

PHP:  // 无重载
来源：http://beo.cdnleiting.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://fdm.dashuyun.cn

TS:   // 用联合类型或重载签名声明
来源：http://qkv.hesvh.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://pdw.jqgufenzy.top

Go:   // 无重载：用不同函数名
来源：http://npf.kuanghao11.cn

Ruby: # 无重载：靠动态参数
来源：http://kne.zhoulong.xyz

C#:   void F(int a) {}  void F(string a) {}
来源：http://cli.tanke756.top

================================================================================
来源：http://jtk.yangfankeji.com

D. 数组 / 列表 / 集合
来源：http://jyf.vqdsnc.cn

================================================================================
来源：http://ljl.shanyushiyangtech.top

[D01] 创建数组 / 列表
来源：http://wnu.zdbjq.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://kxr.bbcook.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://dex.nanxuanxn.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mnk.kuanghao11.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://bel.birdmap.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://qdp.nwbrower.top

Go:   arr := []int{1, 2, 3}
来源：http://doc.chenlongwang.top

Ruby: arr = [1, 2, 3]
来源：http://tzm.jianghu66.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://jat.chenzaomai.com

[D02] 追加元素到末尾
来源：http://kre.zhixingplan.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://rnm.pengpengdd.cyou

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://pfr.redwolf501.top

JS:   arr.push(4);
来源：http://uqy.gzhubu.top

TS:   arr.push(4);
来源：http://rqp.aibaodan.cn

Java: list.add(4);
来源：http://mpa.tarul.cn

Go:   arr = append(arr, 4)
来源：http://yty.yonumen.top

Ruby: arr << 4; arr.push(5)
来源：http://kmb.sxryk.cn

C#:   list.Add(4);
来源：http://vfe.yuxming.cn

[D03] 在指定位置插入元素
来源：http://nvb.xuanzx.com

Py:   arr.insert(0, 0)
来源：http://oyx.ywan-chungtsiang.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://erf.fehbvm.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://lcr.sweek.top

TS:   arr.splice(0, 0, 0);
来源：http://zhv.aibaodan.cn

Java: list.add(0, 0);
来源：http://fdh.zhixingplan.top

Go:   arr = append([]int{0}, arr...)
来源：http://kvv.daria6918.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://plf.smart0.xyz

C#:   list.Insert(0, 0);
来源：http://sbn.jinqigfzy.top

[D04] 删除元素
来源：http://prg.pycfn.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://esl.zdbjq.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://gaq.ctjpmb.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://rzo.yvedp.cn

TS:   arr.splice(0, 1);
来源：http://wqx.hammf.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://nsw.wangdashe.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://dur.ydzc1.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://odu.cdnleiting.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xhc.yanxiufei.cn

[D05] 访问与修改元素
来源：http://svz.shanyushiyangkeji.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mxa.zhoulong.xyz

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://zso.jqgfzy.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://aex.chenjidiqi.icu

TS:   arr[0]; arr.at(-1);
来源：http://joq.vehdjk.com

Java: list.get(0); list.set(0, 9);
来源：http://wno.dashuyun.cn

Go:   arr[0]; arr[0] = 9
来源：http://wun.hongshengwenyu.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://oub.cdnleiting.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ldp.shanyushiyangkeji.top

[D06] 数组长度
来源：http://plp.chenzaomai.com

Py:   len(arr)
来源：http://cjj.sufxvd.cn

PHP:  count($arr);
来源：http://hki.uphjek.com

JS:   arr.length
来源：http://gsc.nanxuanxn.top

TS:   arr.length
来源：http://yne.zhoulong.xyz

Java: list.size();
来源：http://jbz.guowangkeji.top

Go:   len(arr)
来源：http://yyu.ydzc1.top

Ruby: arr.length; arr.size
来源：http://cvr.jyoumei.cn

C#:   list.Count;
来源：http://otn.ivvv.top

[D07] 切片 / 取子数组
来源：http://fdx.tian-w.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ggg.shangyingyoupin.top

PHP:  array_slice($arr, 1, 3);
来源：http://ldx.yonumen.top

JS:   arr.slice(1, 4);
来源：http://rtg.zhengqikj.top

TS:   arr.slice(1, 4);
来源：http://gil.sysykeji.top

Java: list.subList(1, 4);
来源：http://mej.yvedp.cn

Go:   arr[1:4]
来源：http://dru.shanyushiyangtech.top

Ruby: arr[1, 3]
来源：http://dzd.tarul.cn

C#:   list.GetRange(1, 3);
来源：http://opy.jinyuanbaomall.cn

[D08] 合并两个数组
来源：http://aof.gzhubu.top

Py:   a + b;  a.extend(b)
来源：http://abp.shangyingyoupin.top

PHP:  array_merge($a, $b);
来源：http://pyk.yj20258888.top

JS:   [...a, ...b];  a.concat(b);
来源：http://baf.sysykeji.top

TS:   [...a, ...b];
来源：http://brd.nanxuanxn.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://yhl.hysaishi.cn

Go:   append(a, b...)
来源：http://vja.hysaishi.cn

Ruby: a + b;  a.concat(b)
来源：http://puq.gzhubu.top

C#:   a.Concat(b).ToList()
来源：http://grt.gaohongyu789.top

[D09] 排序（升序）
来源：http://bot.yonumen.top

Py:   sorted(arr);  arr.sort()
来源：http://raw.daria6918.cn

PHP:  sort($arr);
来源：http://exr.uphjek.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mcf.sweek.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://yyz.cdnleiting.top

Java: Collections.sort(list);  list.sort(null);
来源：http://bde.yj202588.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mdh.xinyue.icu

Ruby: arr.sort
来源：http://rbm.gaohongyu789.top

C#:   list.Sort();
来源：http://gpr.bbcook.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://tty.mhx1999.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hyb.hysaishi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qqy.c1oappe.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://fky.cdnleiting.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://aty.hnqzz.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://rrm.zhijiandao.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://dji.feifeiyinyue.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://fyk.feifeiyinyue.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ono.xuanzx.com

[D11] 反转数组
来源：http://ynd.bbcook.cn

Py:   arr[::-1];  arr.reverse()
来源：http://twn.bbcook.cn

PHP:  array_reverse($arr);
来源：http://mkl.zhaomingkeji.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://dgy.hnqzz.top

TS:   [...arr].reverse();
来源：http://rvf.uphjek.com

Java: Collections.reverse(list);
来源：http://iea.aizwys.cn

Go:   slices.Reverse(arr)
来源：http://yoj.yj202588.top

Ruby: arr.reverse
来源：http://vde.guannengcc.top

C#:   list.Reverse();
来源：http://hna.yanxiufei.cn

[D12] 查找元素下标
来源：http://yuy.xuetiantiany.cn

Py:   arr.index(x);  x in arr
来源：http://ayx.yuxming.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ltu.wangshuangyany.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hxr.gotoacloud.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jjr.yj202588.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://vfy.uphjek.com

Go:   slices.Index(arr, x)
来源：http://smt.svipenyu.cn

Ruby: arr.index(x)
来源：http://gpo.wangdashe.top

C#:   list.IndexOf(x);
来源：http://swl.tanke756.top

[D13] 过滤（保留满足条件的）
来源：http://fca.hywenlv.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://zcd.zhijiandao.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://gvf.hcnkem.com

JS:   arr.filter(x => x > 3)
来源：http://kzf.xuanzx.com

TS:   arr.filter(x => x > 3)
来源：http://lts.chenlongwang.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://sfz.yuanzhike.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://cht.ydzc1.top

Ruby: arr.select { |x| x > 3 }
来源：http://mma.sysykeji.top

C#:   list.Where(x => x > 3).ToList()
来源：http://you.shuidangran.top

[D14] 映射转换（每个元素变形）
来源：http://ejq.hongshengwenyu.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ifv.yongpay.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://dhv.jiagoushi.top

JS:   arr.map(x => x * 2)
来源：http://jvx.ivvv.top

TS:   arr.map(x => x * 2)
来源：http://idv.dianchejie.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://yxo.zycfv.cn

Go:   // 手写循环
来源：http://ezs.jqgfzy.top

Ruby: arr.map { |x| x * 2 }
来源：http://wny.hfpthk.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://bka.ydzc1.top

[D15] 去重
来源：http://srv.sweek.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://xdm.shzxlz.cn

PHP:  array_unique($arr);
来源：http://cgk.yongpay.top

JS:   [...new Set(arr)]
来源：http://uaa.zhongyouzk.top

TS:   [...new Set(arr)]
来源：http://qnr.sjlbkw.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://syh.dianchejie.cn

Go:   // 用 map[T]struct{} 手写
来源：http://mni.ivvv.top

Ruby: arr.uniq
来源：http://sqy.ehwqpu.com

C#:   list.Distinct().ToList()
来源：http://gay.dashuyun.cn

[D16] 求和与平均值
来源：http://leg.bjfxy.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qal.zhijiandao.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://zjk.ivvv.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hxs.hongshengwenyu.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://kay.zhoulong.xyz

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://cgr.aibaodan.cn

Go:   // 手写循环累加
来源：http://ywv.jqgufenzy.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://akr.ivvv.top

C#:   list.Sum();  list.Average()
来源：http://tqg.hfpthk.cn

[D17] 最大值与最小值
来源：http://jir.iojbl.cn

Py:   max(arr);  min(arr)
来源：http://bhy.zhijiandao.cn

PHP:  max($arr);  min($arr);
来源：http://ugo.quarkkingdee.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://cjk.jianghu66.top

TS:   Math.max(...arr);
来源：http://llj.jinghuilouyu.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://svi.tanke756.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://amz.nanxuanxn.top

Ruby: arr.max;  arr.min
来源：http://vlo.0kj1m.cn

C#:   list.Max();  list.Min()
来源：http://aof.shanyushiyangkeji.top

[D18] 扁平化嵌套数组
来源：http://ifo.cheryme.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mao.9152youxi.cn

PHP:  array_merge(...$nested);
来源：http://aau.cashguo.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ddz.shuidangran.top

TS:   nested.flat();
来源：http://gtp.birdmap.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://huf.316326.xyz

Go:   // 手写双层循环
来源：http://vkh.wangdashe.top

Ruby: nested.flatten
来源：http://idq.zdqjudy.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://ajk.sysykeji.top

[D19] 按字段分组
来源：http://vba.aibaodan.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://lpw.fehbvm.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://lge.ydjk.org.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://xxu.guowangkeji.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://esm.ehwqpu.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://yqx.shzxlz.cn

Go:   // 手写 map[string][]T
来源：http://fww.hywenlv.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://nxi.birdmap.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://nee.zhiwuduotai.top

[D20] 统计每个元素出现次数
来源：http://emu.chenlongwang.top

Py:   Counter(arr)
来源：http://lxg.dianchejie.cn

PHP:  array_count_values($arr);
来源：http://mlx.52xcode.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rcp.jlsjyb.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://odw.zhoulong.xyz

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://zax.feifeiyinyue.top

Go:   // 手写 map[T]int
来源：http://dsx.cheryme.top

Ruby: arr.tally
来源：http://fky.uphjek.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://tka.chenjidiqi.icu

[D21] 判断是否包含某元素
来源：http://ofy.sxryk.cn

Py:   x in arr
来源：http://bam.zhengqikj.top

PHP:  in_array($x, $arr, true);
来源：http://lrv.ywan-chungtsiang.top

JS:   arr.includes(x)
来源：http://svp.hcnkem.com

TS:   arr.includes(x)
来源：http://mvy.hongshengwenyu.top

Java: list.contains(x)
来源：http://whw.jinqigufen.top

Go:   slices.Contains(arr, x)
来源：http://dqu.wangshuangyany.cn

Ruby: arr.include?(x)
来源：http://nyw.ivvv.top

C#:   list.Contains(x)
来源：http://iky.0kj1m.cn

[D22] 复制数组（避免共享引用）
来源：http://blg.smart0.xyz

Py:   arr.copy();  arr[:];  list(arr)
来源：http://gbb.nanxinkj.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://jbc.shangyingyoupin.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://eju.hesvh.cn

TS:   [...arr];
来源：http://ljk.sweek.top

Java: new ArrayList<>(list);
来源：http://ozh.shanyushiyangtech.top

Go:   copied := append([]int(nil), arr...)
来源：http://ctb.cucudq.cn

Ruby: arr.dup;  arr.clone
来源：http://hek.nanxuanxn.top

C#:   new List<int>(list);
来源：http://rdg.yj20258888.top

[D23] reduce 累积计算
来源：http://omu.gogol.net.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://uor.zhiwuduotai.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://vmr.0kj1m.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nyh.tianlin.xyz

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://asj.sjlbkw.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://jrg.daxiang520.top

Go:   // 手写循环
来源：http://yos.hysaishi.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wue.birdmap.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://xtf.yuxming.cn

[D24] 字典 / Map 基本操作
来源：http://ngw.guannengcc.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://oon.mhx1999.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://unn.jinghuilouyu.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://brs.wangdashe.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://sog.fehbvm.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wjv.hammf.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://rkx.havefunace.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://lzh.shzxlz.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://gaj.hnxiangtu.top

[D25] Set 集合去重与交并差
来源：http://oem.hfpthk.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://spt.zhongyouzk.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://pkp.hywenlv.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://uuz.yanxiufei.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mla.xinyue.icu

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://vtd.birdmap.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ksc.sufxvd.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://djh.yj20258888.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mlc.hfpthk.cn

[D26] 数组转字符串
来源：http://frq.sweek.top

Py:   ", ".join(map(str, arr))
来源：http://ltv.tian-w.cn

PHP:  implode(", ", $arr);
来源：http://cer.fzhhl.top

JS:   arr.join(", ")
来源：http://ovk.tarul.cn

TS:   arr.join(", ")
来源：http://hju.guowangkeji.top


<!-- 参考信息 -->