代发 wailian999

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://usm.shanyushiyangkeji.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://uew.jqgfzy.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://syl.gogol.net.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jce.zycfv.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mnm.yfazqb.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://eog.yongpay.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://irx.zhijiandao.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://rsg.ydzc1.top

[C10] 变量作用域
来源：http://oso.gzhubu.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://xuy.cashguo.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://syg.guowangkeji.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://phz.uphjek.com

TS:   同 JS
来源：http://mbw.hesvh.cn

Java: 方法内为块级作用域
来源：http://qcr.aibaodan.cn

Go:   花括号块级作用域
来源：http://mew.fanxiaobao.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://etd.cheryme.top

C#:   块级作用域
来源：http://rqm.hcnkem.com

[C11] 模块导入与导出
来源：http://jou.xuanzx.com

Py:   from module import func
来源：http://ayq.svipenyu.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://cge.yj202588.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://min.xuetiantiany.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://vya.xylfe.cn

Java: import java.util.List;
来源：http://gya.zdbjq.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://qfr.chenlongwang.top

Ruby: require "json"; require_relative "./util"
来源：http://pff.sjlbkw.cn

C#:   using System.Text;
来源：http://gyc.jyoumei.cn

[C12] 立即执行函数 IIFE
来源：http://srx.birdmap.top

Py:   (lambda: print("run"))()
来源：http://drg.zhengqikj.top

PHP:  (function () { echo "run"; })();
来源：http://bzo.zhengqikj.top

JS:   (() => { console.log("run"); })();
来源：http://gej.vqdsnc.cn

TS:   (() => { console.log("run"); })();
来源：http://ckl.pycfn.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://cha.chenjidiqi.icu

Go:   func() { fmt.Println("run") }()
来源：http://ylv.yanxiufei.cn

Ruby: -> { puts "run" }.call
来源：http://mta.zdbjq.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://zfc.zhongyouzk.top

[C13] 类型声明 / 类型注解
来源：http://qsx.hammf.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://rvy.fktsv.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zkt.bjfxy.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://vkc.shzxlz.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://uur.cdnleiting.top

Java: int add(int a, int b) { return a + b; }
来源：http://xzw.shanyushiyangtech.top

Go:   func add(a, b int) int
来源：http://oej.jiagoushi.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://tjf.yj20258888.top

C#:   int Add(int a, int b) => a + b;
来源：http://zzg.9152youxi.cn

[C14] 泛型函数
来源：http://htv.yj20258888.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://dod.nwbrower.top

PHP:  // 无泛型
来源：http://sqj.kuanghao11.cn

JS:   // 无泛型
来源：http://plu.zhengqikj.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mnq.hcnkem.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://shs.zdbjq.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://xus.zhijiandao.cn

Ruby: # 无泛型
来源：http://nmr.tanke756.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xkb.iojbl.cn

[C15] 解构 / 展开参数
来源：http://qsd.meibo888.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://rsv.ivvv.top

PHP:  [$a, $b] = $pair;
来源：http://pfl.c1oappe.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://qdc.wangshuangyany.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wie.hammf.cn

Java: // 无解构
来源：http://lyi.guowangkeji.top

Go:   // 无解构
来源：http://foq.daxiang520.top

Ruby: a, b = pair
来源：http://ijm.daxiang520.top

C#:   var (a, b) = pair;
来源：http://hpm.guowangkeji.top

[C16] 函数 / 方法重载
来源：http://shx.yuxming.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://fnx.sweek.top

PHP:  // 无重载
来源：http://elo.cqqwz.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://dyx.andypj.xyz

TS:   // 用联合类型或重载签名声明
来源：http://key.jiagoushi.top

Java: void f(int a) {}  void f(String a) {}
来源：http://tmp.ehwqpu.com

Go:   // 无重载：用不同函数名
来源：http://jsk.dashuyun.cn

Ruby: # 无重载：靠动态参数
来源：http://dxp.zhixingplan.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://iow.yuxming.cn

================================================================================
来源：http://qsu.redwolf501.top

D. 数组 / 列表 / 集合
来源：http://tye.0kj1m.cn

================================================================================
来源：http://iff.yuxming.cn

[D01] 创建数组 / 列表
来源：http://cme.9152youxi.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://fha.snrcjt.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://gev.jqgufenzy.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ntj.c1oappe.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://ypq.guannengcc.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://qxj.jinqigfzy.top

Go:   arr := []int{1, 2, 3}
来源：http://krk.ydjk.org.cn

Ruby: arr = [1, 2, 3]
来源：http://zva.xuanzx.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://lvz.shanyushiyangkeji.top

[D02] 追加元素到末尾
来源：http://ywz.shanyushiyangtech.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://glz.hfpthk.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://spx.shanyushiyangkeji.top

JS:   arr.push(4);
来源：http://kdh.ybcxt.top

TS:   arr.push(4);
来源：http://ppo.hcnkem.com

Java: list.add(4);
来源：http://mcf.jinghuilouyu.cn

Go:   arr = append(arr, 4)
来源：http://ehj.jqgfzy.top

Ruby: arr << 4; arr.push(5)
来源：http://xjo.redwolf501.top

C#:   list.Add(4);
来源：http://zgb.gzhubu.top

[D03] 在指定位置插入元素
来源：http://qjc.hesvh.cn

Py:   arr.insert(0, 0)
来源：http://bnu.yonumen.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://vun.smart0.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://str.ppjwa.cn

TS:   arr.splice(0, 0, 0);
来源：http://gzb.ivvv.top

Java: list.add(0, 0);
来源：http://mvl.zhongyouzk.top

Go:   arr = append([]int{0}, arr...)
来源：http://pbr.jinqigfzy.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://oud.hongshengwenyu.top

C#:   list.Insert(0, 0);
来源：http://irr.haohaochexian.top

[D04] 删除元素
来源：http://pga.chenzaomai.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://kws.yangfankeji.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://bzq.52xcode.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://txl.aizwys.cn

TS:   arr.splice(0, 1);
来源：http://dyy.uphjek.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://cab.chenjidiqi.icu

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://rms.guannengcc.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://kxj.sysykeji.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://aep.xylfe.cn

[D05] 访问与修改元素
来源：http://oti.wangdashe.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://efh.aizwys.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://oen.dashuyun.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://kln.tianlin.xyz

TS:   arr[0]; arr.at(-1);
来源：http://ubh.feifeiyinyue.top

Java: list.get(0); list.set(0, 9);
来源：http://fbu.aibaodan.cn

Go:   arr[0]; arr[0] = 9
来源：http://zdz.cucudq.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hrs.nanxuanxn.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://fcy.zhoulong.xyz

[D06] 数组长度
来源：http://vok.fktsv.cn

Py:   len(arr)
来源：http://rcb.zhengqikj.top

PHP:  count($arr);
来源：http://pxo.iojbl.cn

JS:   arr.length
来源：http://xnq.pycfn.com

TS:   arr.length
来源：http://itf.ydjk.org.cn

Java: list.size();
来源：http://gyg.yuxming.cn

Go:   len(arr)
来源：http://vqg.ctjpmb.com

Ruby: arr.length; arr.size
来源：http://gle.ppjwa.cn

C#:   list.Count;
来源：http://ruf.hywenlv.cn

[D07] 切片 / 取子数组
来源：http://qru.tian-w.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://nsx.yj202588.top

PHP:  array_slice($arr, 1, 3);
来源：http://uep.ydjk.org.cn

JS:   arr.slice(1, 4);
来源：http://aro.xinyue.icu

TS:   arr.slice(1, 4);
来源：http://arw.zdqjudy.top

Java: list.subList(1, 4);
来源：http://hke.haohaochexian.top

Go:   arr[1:4]
来源：http://wqe.hywenlv.cn

Ruby: arr[1, 3]
来源：http://vzs.daria6918.cn

C#:   list.GetRange(1, 3);
来源：http://cpw.shanyushiyangkeji.top

[D08] 合并两个数组
来源：http://cto.hysaishi.cn

Py:   a + b;  a.extend(b)
来源：http://kqb.hesvh.cn

PHP:  array_merge($a, $b);
来源：http://utc.kuanghao11.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://eid.epnwcf.com

TS:   [...a, ...b];
来源：http://cpy.zhaomingkeji.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://tzo.uphjek.com

Go:   append(a, b...)
来源：http://qyr.hnxiangtu.top

Ruby: a + b;  a.concat(b)
来源：http://qit.pycfn.com

C#:   a.Concat(b).ToList()
来源：http://uww.mhx1999.top

[D09] 排序（升序）
来源：http://ehv.yangfankeji.com

Py:   sorted(arr);  arr.sort()
来源：http://mfl.yonumen.top

PHP:  sort($arr);
来源：http://eem.ydjk.org.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hjp.jinyuanbaomall.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://dwe.jinqigfzy.top

Java: Collections.sort(list);  list.sort(null);
来源：http://nxh.yuanzhike.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qgw.bjfxy.top

Ruby: arr.sort
来源：http://zlv.9152youxi.cn

C#:   list.Sort();
来源：http://ftq.hnqzz.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://jej.guowangkeji.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://bnr.zhengqikj.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://luw.hnqzz.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://lwn.yangfankeji.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://kvs.fzhhl.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://igk.haohaochexian.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://nsi.hnxiangtu.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://qld.xylfe.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ylt.daria6918.cn

[D11] 反转数组
来源：http://iwb.fktsv.cn

Py:   arr[::-1];  arr.reverse()
来源：http://rft.sxryk.cn

PHP:  array_reverse($arr);
来源：http://dnm.c1oappe.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ytk.bjfxy.top

TS:   [...arr].reverse();
来源：http://iek.gaohongyu789.top

Java: Collections.reverse(list);
来源：http://kat.tanke756.top

Go:   slices.Reverse(arr)
来源：http://imj.andypj.xyz

Ruby: arr.reverse
来源：http://adb.nanxinkj.top

C#:   list.Reverse();
来源：http://hmt.ydjk.org.cn

[D12] 查找元素下标
来源：http://xvk.sweek.top

Py:   arr.index(x);  x in arr
来源：http://ixg.shanyushiyangkeji.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://rgr.jyoumei.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xls.tian-w.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://oov.hammf.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://rix.andypj.xyz

Go:   slices.Index(arr, x)
来源：http://pat.yj20258.top

Ruby: arr.index(x)
来源：http://meb.vqdsnc.cn

C#:   list.IndexOf(x);
来源：http://pie.daria6918.cn

[D13] 过滤（保留满足条件的）
来源：http://tps.yanxiufei.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://udy.zhoulong.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://jnc.jyoumei.cn

JS:   arr.filter(x => x > 3)
来源：http://pyr.xingfuxueyuan.xyz

TS:   arr.filter(x => x > 3)
来源：http://whn.jlsjyb.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://aoz.zhaomingkeji.xyz

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://jvm.pycfn.com

Ruby: arr.select { |x| x > 3 }
来源：http://vcw.zhiwuduotai.top

C#:   list.Where(x => x > 3).ToList()
来源：http://jlu.cucudq.cn

[D14] 映射转换（每个元素变形）
来源：http://dgj.yuxming.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://kzz.zhengqikj.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://frk.chenzaomai.com

JS:   arr.map(x => x * 2)
来源：http://rdv.hammf.cn

TS:   arr.map(x => x * 2)
来源：http://huc.zycfv.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://gvp.fengsongda.top

Go:   // 手写循环
来源：http://byq.jiagoushi.top

Ruby: arr.map { |x| x * 2 }
来源：http://bie.yj20258.top

C#:   list.Select(x => x * 2).ToList()
来源：http://llj.daria6918.cn

[D15] 去重
来源：http://gbe.jyoumei.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wmj.jlsjyb.cn

PHP:  array_unique($arr);
来源：http://dpz.sysykeji.top

JS:   [...new Set(arr)]
来源：http://gyp.xuanzx.com

TS:   [...new Set(arr)]
来源：http://tva.fktsv.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://iii.vehdjk.com

Go:   // 用 map[T]struct{} 手写
来源：http://gzf.nanxinkj.top

Ruby: arr.uniq
来源：http://lse.havefunace.top

C#:   list.Distinct().ToList()
来源：http://xdu.yangfankeji.com

[D16] 求和与平均值
来源：http://ssd.yangfankeji.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://usr.ctjpmb.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://aef.hesvh.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://lzt.xinyue.icu

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://bcm.dashuyun.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://sjb.yuanzhike.top

Go:   // 手写循环累加
来源：http://nin.jianghu66.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://dao.yuanzhike.top

C#:   list.Sum();  list.Average()
来源：http://omi.gaohongyu789.top

[D17] 最大值与最小值
来源：http://vlq.hfpthk.cn

Py:   max(arr);  min(arr)
来源：http://qwf.zhengqikj.top

PHP:  max($arr);  min($arr);
来源：http://ipd.wangshuangyany.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://toe.zdbjq.cn

TS:   Math.max(...arr);
来源：http://hof.vehdjk.com

Java: Collections.max(list);  Collections.min(list);
来源：http://iwj.sjlbkw.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://eqe.fehbvm.com

Ruby: arr.max;  arr.min
来源：http://mdh.zdqjudy.top

C#:   list.Max();  list.Min()
来源：http://fqp.iojbl.cn

[D18] 扁平化嵌套数组
来源：http://dmk.cqqwz.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xmt.xinyue.icu

PHP:  array_merge(...$nested);
来源：http://sbf.daria6918.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://icc.zhoulong.xyz

TS:   nested.flat();
来源：http://sjp.9152youxi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://pak.nanxuanxn.top

Go:   // 手写双层循环
来源：http://wbw.jinyuanbaomall.cn

Ruby: nested.flatten
来源：http://lwx.c1oappe.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://thy.9152youxi.cn

[D19] 按字段分组
来源：http://rqo.cheryme.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://xxo.kuanghao11.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://yen.jinqigufen.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://dng.ywan-chungtsiang.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://aeo.jyoumei.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ihy.yvedp.cn

Go:   // 手写 map[string][]T
来源：http://rdg.bjfxy.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://pvv.hcnkem.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mxz.epnwcf.com

[D20] 统计每个元素出现次数
来源：http://mfo.uphjek.com

Py:   Counter(arr)
来源：http://ocs.zhoulong.xyz

PHP:  array_count_values($arr);
来源：http://cpb.xuanzx.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tqh.aizwys.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://afm.zycfv.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ibf.fengsongda.top

Go:   // 手写 map[T]int
来源：http://ecp.zycfv.cn

Ruby: arr.tally
来源：http://ekw.yj20258.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://aus.zhoulong.xyz

[D21] 判断是否包含某元素
来源：http://dvj.wangshuangyany.cn

Py:   x in arr
来源：http://ybe.tanke756.top

PHP:  in_array($x, $arr, true);
来源：http://jrj.sjlbkw.cn

JS:   arr.includes(x)
来源：http://vrm.vqdsnc.cn

TS:   arr.includes(x)
来源：http://xue.pengpengdd.cyou

Java: list.contains(x)
来源：http://etl.gotoacloud.top

Go:   slices.Contains(arr, x)
来源：http://xmk.ctjpmb.com

Ruby: arr.include?(x)
来源：http://whg.hnqzz.top

C#:   list.Contains(x)
来源：http://tbv.ybcxt.top

[D22] 复制数组（避免共享引用）
来源：http://yea.dashuyun.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://xeu.bbcook.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ceo.yuxming.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://nmi.fehbvm.com

TS:   [...arr];
来源：http://ahu.yj202588.top

Java: new ArrayList<>(list);
来源：http://ktv.jlsjyb.cn

Go:   copied := append([]int(nil), arr...)
来源：http://jwy.hysaishi.cn

Ruby: arr.dup;  arr.clone
来源：http://nxj.meibo888.top

C#:   new List<int>(list);
来源：http://tys.jyoumei.cn

[D23] reduce 累积计算
来源：http://yxm.yueranfly.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://jad.hongshengwenyu.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://fdz.vqdsnc.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hgz.yongpay.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gxv.ppjwa.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://sgc.yj20258888.top

Go:   // 手写循环
来源：http://ivt.yangfankeji.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://tmo.bjfxy.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://fzd.tianlin.xyz

[D24] 字典 / Map 基本操作
来源：http://ika.yangfankeji.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://uqp.sufxvd.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://vxf.zhongyouzk.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mgc.jinqigfzy.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://iov.svipenyu.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://kin.wangdashe.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://glu.dashuyun.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://gnr.xziqi.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://rot.mhx1999.top

[D25] Set 集合去重与交并差
来源：http://wee.tian-w.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://uwk.quarkkingdee.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ftz.tanke756.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://etg.pycfn.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://eqp.feifeiyinyue.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hbh.quarkkingdee.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://iag.nanxinkj.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xyo.zhijiandao.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ldz.zhoulong.xyz

[D26] 数组转字符串
来源：http://jvn.9152youxi.cn


<!-- 参考信息 -->