代发 wailian999

C#:   Func<int, int> square = x => x * x;
来源：http://orl.zhengqikj.top

[C07] 把函数作为参数传入
来源：http://oix.fanxiaobao.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://tmt.guowangkeji.top

PHP:  array_map("strtoupper", $arr);
来源：http://rtq.shanyushiyangtech.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xbs.sjlbkw.cn

TS:   arr.map(String)
来源：http://rzf.shanyushiyangtech.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://vyy.316326.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://lsr.yfazqb.com

Ruby: arr.map(&:upcase)
来源：http://vlj.hnxiangtu.top

C#:   arr.Select(s => s.ToUpper())
来源：http://cwq.xziqi.cn

[C08] 闭包
来源：http://bax.ivvv.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wdb.jlsjyb.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wqy.meibo888.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ues.xinyue.icu

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://jhw.tarul.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://bay.hysaishi.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://dzr.shanyushiyangkeji.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ore.vehdjk.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://zmm.birdmap.top

[C09] 递归
来源：http://pwf.shzxlz.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ubo.tanke756.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://vxb.fanxiaobao.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kmu.hammf.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tpe.redwolf501.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ncq.316326.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ozf.cucudq.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://skh.vqdsnc.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://yhg.jyoumei.cn

[C10] 变量作用域
来源：http://yzw.jqgfzy.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://nsd.hnxiangtu.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://csv.shangyingyoupin.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://lbl.c1oappe.top

TS:   同 JS
来源：http://myy.yueranfly.top

Java: 方法内为块级作用域
来源：http://dqb.jinqigufen.top

Go:   花括号块级作用域
来源：http://wpg.zdbjq.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://dit.hnxiangtu.top

C#:   块级作用域
来源：http://jyj.c1oappe.top

[C11] 模块导入与导出
来源：http://bzf.shanyushiyangtech.top

Py:   from module import func
来源：http://wpj.gzhubu.top

PHP:  require "file.php";  或 use App\Service;
来源：http://wgq.sysykeji.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://dgi.wangdashe.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://gyb.zhongyouzk.top

Java: import java.util.List;
来源：http://ikj.jianghu66.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mgo.yueranfly.top

Ruby: require "json"; require_relative "./util"
来源：http://xgx.yanxiufei.cn

C#:   using System.Text;
来源：http://gdh.aibaodan.cn

[C12] 立即执行函数 IIFE
来源：http://pvl.hesvh.cn

Py:   (lambda: print("run"))()
来源：http://vuu.nanxinkj.top

PHP:  (function () { echo "run"; })();
来源：http://qgd.9152youxi.cn

JS:   (() => { console.log("run"); })();
来源：http://cad.sjlbkw.cn

TS:   (() => { console.log("run"); })();
来源：http://wyd.nanxinkj.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ult.guowangkeji.top

Go:   func() { fmt.Println("run") }()
来源：http://xqu.gotoacloud.top

Ruby: -> { puts "run" }.call
来源：http://wzo.fanxiaobao.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://szv.redwolf501.top

[C13] 类型声明 / 类型注解
来源：http://jof.dianchejie.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://jfb.xingfuxueyuan.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xig.vqdsnc.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mnv.cucudq.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tnb.chenzaomai.com

Java: int add(int a, int b) { return a + b; }
来源：http://mha.ybcxt.top

Go:   func add(a, b int) int
来源：http://ons.zdbjq.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://pad.dashuyun.cn

C#:   int Add(int a, int b) => a + b;
来源：http://mis.zhengqikj.top

[C14] 泛型函数
来源：http://iaq.gaohongyu789.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://usv.chenlongwang.top

PHP:  // 无泛型
来源：http://zvs.chenjidiqi.icu

JS:   // 无泛型
来源：http://zev.fanxiaobao.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://iss.aibaodan.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://vac.chenlongwang.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://xob.andypj.xyz

Ruby: # 无泛型
来源：http://zuv.wangshuangyany.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://qvh.hongshengwenyu.top

[C15] 解构 / 展开参数
来源：http://ccy.iojbl.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://yax.sysykeji.top

PHP:  [$a, $b] = $pair;
来源：http://zzf.yonumen.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://imz.zdbjq.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://uam.tanke756.top

Java: // 无解构
来源：http://qyd.nanxinkj.top

Go:   // 无解构
来源：http://tqd.yanxiufei.cn

Ruby: a, b = pair
来源：http://zpo.ivvv.top

C#:   var (a, b) = pair;
来源：http://hsi.vehdjk.com

[C16] 函数 / 方法重载
来源：http://poh.nanxinkj.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://unb.jinghuilouyu.cn

PHP:  // 无重载
来源：http://vlf.jqgfzy.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://ovz.ppjwa.cn

TS:   // 用联合类型或重载签名声明
来源：http://lcf.ehwqpu.com

Java: void f(int a) {}  void f(String a) {}
来源：http://nqt.pengpengdd.cyou

Go:   // 无重载：用不同函数名
来源：http://pfn.epnwcf.com

Ruby: # 无重载：靠动态参数
来源：http://far.jqgfzy.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://ckt.jqgufenzy.top

================================================================================
来源：http://ugj.yj20258.top

D. 数组 / 列表 / 集合
来源：http://hgj.fzhhl.top

================================================================================
来源：http://cou.hesvh.cn

[D01] 创建数组 / 列表
来源：http://ypz.yuxming.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://vps.ehwqpu.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://pqi.zdqjudy.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://lds.yfazqb.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://jjn.nwbrower.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://fvt.gotoacloud.top

Go:   arr := []int{1, 2, 3}
来源：http://jgr.jyoumei.cn

Ruby: arr = [1, 2, 3]
来源：http://kmf.zhoulong.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://sye.fengsongda.top

[D02] 追加元素到末尾
来源：http://dlh.cheryme.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ybs.bbcook.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hmc.uphjek.com

JS:   arr.push(4);
来源：http://otj.dashuyun.cn

TS:   arr.push(4);
来源：http://syx.kuanghao11.cn

Java: list.add(4);
来源：http://iwe.sysykeji.top

Go:   arr = append(arr, 4)
来源：http://hcg.jinyuanbaomall.cn

Ruby: arr << 4; arr.push(5)
来源：http://ppo.smart0.xyz

C#:   list.Add(4);
来源：http://lfy.quarkkingdee.top

[D03] 在指定位置插入元素
来源：http://kku.sjlbkw.cn

Py:   arr.insert(0, 0)
来源：http://fof.dianchejie.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://xpy.jqgufenzy.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://dzq.iojbl.cn

TS:   arr.splice(0, 0, 0);
来源：http://yvt.jinqigufen.top

Java: list.add(0, 0);
来源：http://igy.sweek.top

Go:   arr = append([]int{0}, arr...)
来源：http://blt.pycfn.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://amd.epnwcf.com

C#:   list.Insert(0, 0);
来源：http://ayb.yfazqb.com

[D04] 删除元素
来源：http://ogg.c1oappe.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://kus.hnxiangtu.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://nbh.jyoumei.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mht.cashguo.top

TS:   arr.splice(0, 1);
来源：http://enu.vqdsnc.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://gws.daxiang520.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://nbi.jqgufenzy.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mzy.jlsjyb.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://lhi.yvedp.cn

[D05] 访问与修改元素
来源：http://syx.chenjidiqi.icu

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://jqh.cdnleiting.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://xfy.zhengqikj.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://tua.xziqi.cn

TS:   arr[0]; arr.at(-1);
来源：http://ppf.feifeiyinyue.top

Java: list.get(0); list.set(0, 9);
来源：http://xom.jinghuilouyu.cn

Go:   arr[0]; arr[0] = 9
来源：http://mfv.yonumen.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mgq.chenjidiqi.icu

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ogp.epnwcf.com

[D06] 数组长度
来源：http://pqm.hysaishi.cn

Py:   len(arr)
来源：http://qvz.tianlin.xyz

PHP:  count($arr);
来源：http://hqk.aizwys.cn

JS:   arr.length
来源：http://brn.wangdashe.top

TS:   arr.length
来源：http://uyb.zhiwuduotai.top

Java: list.size();
来源：http://dzv.chenzaomai.com

Go:   len(arr)
来源：http://ttj.tarul.cn

Ruby: arr.length; arr.size
来源：http://rop.zhoulong.xyz

C#:   list.Count;
来源：http://fwf.yj202588.top

[D07] 切片 / 取子数组
来源：http://dcw.dashuyun.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://idx.snrcjt.cn

PHP:  array_slice($arr, 1, 3);
来源：http://wli.yonumen.top

JS:   arr.slice(1, 4);
来源：http://eem.fzhhl.top

TS:   arr.slice(1, 4);
来源：http://air.yvedp.cn

Java: list.subList(1, 4);
来源：http://rwq.yonumen.top

Go:   arr[1:4]
来源：http://ovy.ydjk.org.cn

Ruby: arr[1, 3]
来源：http://fow.cqqwz.cn

C#:   list.GetRange(1, 3);
来源：http://nuu.yongpay.top

[D08] 合并两个数组
来源：http://zlu.ydjk.org.cn

Py:   a + b;  a.extend(b)
来源：http://khn.guowangkeji.top

PHP:  array_merge($a, $b);
来源：http://xtk.sjlbkw.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://twq.guowangkeji.top

TS:   [...a, ...b];
来源：http://zww.yonumen.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://axc.yvedp.cn

Go:   append(a, b...)
来源：http://dfg.wangdashe.top

Ruby: a + b;  a.concat(b)
来源：http://zhl.feifeiyinyue.top

C#:   a.Concat(b).ToList()
来源：http://zbh.gogol.net.cn

[D09] 排序（升序）
来源：http://dri.ybcxt.top

Py:   sorted(arr);  arr.sort()
来源：http://abe.sufxvd.cn

PHP:  sort($arr);
来源：http://itk.ehwqpu.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://gdv.316326.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://vmv.tian-w.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://oep.jqgufenzy.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://nbv.fanxiaobao.xyz

Ruby: arr.sort
来源：http://pgp.zhiwuduotai.top

C#:   list.Sort();
来源：http://eag.jiagoushi.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://zni.hnxiangtu.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://som.nwbrower.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hcm.bjfxy.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://jgu.aibaodan.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ego.yongpay.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://rge.cashguo.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://yvz.zdqjudy.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://jfx.redwolf501.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qks.vqdsnc.cn

[D11] 反转数组
来源：http://dax.ydzc1.top

Py:   arr[::-1];  arr.reverse()
来源：http://hvx.hnxiangtu.top

PHP:  array_reverse($arr);
来源：http://wcz.yvedp.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ibg.xylfe.cn

TS:   [...arr].reverse();
来源：http://vok.xziqi.cn

Java: Collections.reverse(list);
来源：http://yds.shanyushiyangtech.top

Go:   slices.Reverse(arr)
来源：http://aca.tanke756.top

Ruby: arr.reverse
来源：http://lgb.yangfankeji.com

C#:   list.Reverse();
来源：http://mcl.chenzaomai.com

[D12] 查找元素下标
来源：http://cth.tanke756.top

Py:   arr.index(x);  x in arr
来源：http://llw.pengpengdd.cyou

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://qnt.uphjek.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://uli.cqqwz.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ano.cheryme.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://lwh.yfazqb.com

Go:   slices.Index(arr, x)
来源：http://mld.zdbjq.cn

Ruby: arr.index(x)
来源：http://wad.shangyingyoupin.top

C#:   list.IndexOf(x);
来源：http://fkl.ydjk.org.cn

[D13] 过滤（保留满足条件的）
来源：http://wcl.andypj.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://pcg.ctjpmb.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wud.yanxiufei.cn

JS:   arr.filter(x => x > 3)
来源：http://jbw.vehdjk.com

TS:   arr.filter(x => x > 3)
来源：http://rqv.pycfn.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://fjv.gzhubu.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://rwi.chenjidiqi.icu

Ruby: arr.select { |x| x > 3 }
来源：http://nxz.xuanzx.com

C#:   list.Where(x => x > 3).ToList()
来源：http://lse.yj20258.top

[D14] 映射转换（每个元素变形）
来源：http://zog.jinqigfzy.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://soe.gaohongyu789.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://jhh.shangyingyoupin.top

JS:   arr.map(x => x * 2)
来源：http://qhu.bbcook.cn

TS:   arr.map(x => x * 2)
来源：http://vbi.zhoulong.xyz

Java: list.stream().map(x -> x * 2).toList()
来源：http://odd.fzhhl.top

Go:   // 手写循环
来源：http://bsj.andypj.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://wwg.jlsjyb.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://jez.sxryk.cn

[D15] 去重
来源：http://zkd.sxryk.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ujd.daria6918.cn

PHP:  array_unique($arr);
来源：http://rjg.jiagoushi.top

JS:   [...new Set(arr)]
来源：http://thf.yvedp.cn

TS:   [...new Set(arr)]
来源：http://cft.yj202588.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ttt.zhaomingkeji.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://tqy.dianchejie.cn

Ruby: arr.uniq
来源：http://fko.ehwqpu.com

C#:   list.Distinct().ToList()
来源：http://chg.wangshuangyany.cn

[D16] 求和与平均值
来源：http://vqc.c1oappe.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wrg.yj202588.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://lmw.hesvh.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://kca.andypj.xyz

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://smf.jinqigufen.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://gpt.redwolf501.top

Go:   // 手写循环累加
来源：http://bri.ydjk.org.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://sih.ywan-chungtsiang.top

C#:   list.Sum();  list.Average()
来源：http://zwd.sweek.top

[D17] 最大值与最小值
来源：http://nwn.bbcook.cn

Py:   max(arr);  min(arr)
来源：http://chz.shanyushiyangkeji.top

PHP:  max($arr);  min($arr);
来源：http://oqg.jlsjyb.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://iod.shanyushiyangtech.top

TS:   Math.max(...arr);
来源：http://amj.guowangkeji.top

Java: Collections.max(list);  Collections.min(list);
来源：http://yav.ydzc1.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wuk.smart0.xyz

Ruby: arr.max;  arr.min
来源：http://ttj.xingfuxueyuan.xyz

C#:   list.Max();  list.Min()
来源：http://adt.cdnleiting.top

[D18] 扁平化嵌套数组
来源：http://lfo.guannengcc.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://lrm.ydzc1.top

PHP:  array_merge(...$nested);
来源：http://sis.jiagoushi.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ucm.fengsongda.top

TS:   nested.flat();
来源：http://uih.xuanzx.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://smj.jiagoushi.top

Go:   // 手写双层循环
来源：http://lzb.shanyushiyangkeji.top

Ruby: nested.flatten
来源：http://bvg.ywan-chungtsiang.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://icv.shuidangran.top

[D19] 按字段分组
来源：http://pqj.nwbrower.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mwl.sysykeji.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://fbi.mhx1999.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://tjq.zdqjudy.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://bup.nanxinkj.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mdp.yuxming.cn

Go:   // 手写 map[string][]T
来源：http://npq.daria6918.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ove.sysykeji.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hoo.wangshuangyany.cn

[D20] 统计每个元素出现次数
来源：http://pqp.c1oappe.top

Py:   Counter(arr)
来源：http://oku.vehdjk.com

PHP:  array_count_values($arr);
来源：http://gex.ctjpmb.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://klj.snrcjt.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xxs.hnxiangtu.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://xtu.jinyuanbaomall.cn

Go:   // 手写 map[T]int
来源：http://owc.xingfuxueyuan.xyz

Ruby: arr.tally
来源：http://zrp.ehwqpu.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://dde.svipenyu.cn

[D21] 判断是否包含某元素
来源：http://jhu.ehwqpu.com

Py:   x in arr
来源：http://tjx.ybcxt.top

PHP:  in_array($x, $arr, true);
来源：http://oka.cashguo.top

JS:   arr.includes(x)
来源：http://hfy.pycfn.com

TS:   arr.includes(x)
来源：http://mbi.yj20258.top

Java: list.contains(x)
来源：http://yng.yfazqb.com

Go:   slices.Contains(arr, x)
来源：http://mjo.gotoacloud.top

Ruby: arr.include?(x)
来源：http://mlz.hfpthk.cn

C#:   list.Contains(x)
来源：http://gzr.shuidangran.top

[D22] 复制数组（避免共享引用）
来源：http://trq.zdqjudy.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://rur.xuanzx.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://xwl.tanke756.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://raw.ywan-chungtsiang.top

TS:   [...arr];
来源：http://bbu.dashuyun.cn

Java: new ArrayList<>(list);
来源：http://vyl.bbcook.cn

Go:   copied := append([]int(nil), arr...)
来源：http://bay.gzhubu.top

Ruby: arr.dup;  arr.clone
来源：http://zfj.ivvv.top

C#:   new List<int>(list);
来源：http://att.xylfe.cn

[D23] reduce 累积计算
来源：http://muj.yangfankeji.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://erd.zhiwuduotai.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://cfm.pengpengdd.cyou

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qsm.wangshuangyany.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kzx.tianlin.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://eji.fanxiaobao.xyz

Go:   // 手写循环
来源：http://chg.sweek.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://pmf.hfpthk.cn


<!-- 参考信息 -->