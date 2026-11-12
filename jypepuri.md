代发 wailian999

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://lvj.svipenyu.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://dba.shangyingyoupin.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hoa.aizwys.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://myq.ctjpmb.com

[C10] 变量作用域
来源：http://axc.yj20258.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ggv.birdmap.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://iqo.dashuyun.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://zya.zdqjudy.top

TS:   同 JS
来源：http://ben.52xcode.cn

Java: 方法内为块级作用域
来源：http://chr.chenlongwang.top

Go:   花括号块级作用域
来源：http://wtx.chenjidiqi.icu

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://qut.wangshuangyany.cn

C#:   块级作用域
来源：http://wlm.sxryk.cn

[C11] 模块导入与导出
来源：http://tbj.jinghuilouyu.cn

Py:   from module import func
来源：http://iwh.shanyushiyangtech.top

PHP:  require "file.php";  或 use App\Service;
来源：http://xwg.cucudq.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://qdn.zhongyouzk.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://qwh.yuanzhike.top

Java: import java.util.List;
来源：http://azq.sufxvd.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ptz.xziqi.cn

Ruby: require "json"; require_relative "./util"
来源：http://mds.jinqigufen.top

C#:   using System.Text;
来源：http://uue.feifeiyinyue.top

[C12] 立即执行函数 IIFE
来源：http://vnt.vqdsnc.cn

Py:   (lambda: print("run"))()
来源：http://xtf.ywan-chungtsiang.top

PHP:  (function () { echo "run"; })();
来源：http://rpi.ydzc1.top

JS:   (() => { console.log("run"); })();
来源：http://hoi.ctjpmb.com

TS:   (() => { console.log("run"); })();
来源：http://obk.tianlin.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jew.hesvh.cn

Go:   func() { fmt.Println("run") }()
来源：http://eaw.jqgufenzy.top

Ruby: -> { puts "run" }.call
来源：http://ejh.hfpthk.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://jjy.zdqjudy.top

[C13] 类型声明 / 类型注解
来源：http://igo.guowangkeji.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://vlz.jlsjyb.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pmv.xinyue.icu

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hun.shanyushiyangtech.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yco.vehdjk.com

Java: int add(int a, int b) { return a + b; }
来源：http://xly.uphjek.com

Go:   func add(a, b int) int
来源：http://lqj.hesvh.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://lst.aizwys.cn

C#:   int Add(int a, int b) => a + b;
来源：http://fvi.tarul.cn

[C14] 泛型函数
来源：http://wjl.pycfn.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ukj.smart0.xyz

PHP:  // 无泛型
来源：http://nzl.tian-w.cn

JS:   // 无泛型
来源：http://jsz.ehwqpu.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://xci.zhiwuduotai.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://via.c1oappe.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://boq.jyoumei.cn

Ruby: # 无泛型
来源：http://ftv.sxryk.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://dhi.zhiwuduotai.top

[C15] 解构 / 展开参数
来源：http://cap.hywenlv.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hbq.haohaochexian.top

PHP:  [$a, $b] = $pair;
来源：http://djy.xinyue.icu

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://uzt.shuidangran.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://vez.cucudq.cn

Java: // 无解构
来源：http://lfj.haohaochexian.top

Go:   // 无解构
来源：http://nku.bbcook.cn

Ruby: a, b = pair
来源：http://xie.vehdjk.com

C#:   var (a, b) = pair;
来源：http://hcc.zycfv.cn

[C16] 函数 / 方法重载
来源：http://lhn.aibaodan.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://nxt.feifeiyinyue.top

PHP:  // 无重载
来源：http://ftl.tarul.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://awu.mhx1999.top

TS:   // 用联合类型或重载签名声明
来源：http://voj.ppjwa.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://djt.ydjk.org.cn

Go:   // 无重载：用不同函数名
来源：http://rtk.sufxvd.cn

Ruby: # 无重载：靠动态参数
来源：http://eou.snrcjt.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://fiz.yongpay.top

================================================================================
来源：http://dec.sweek.top

D. 数组 / 列表 / 集合
来源：http://svg.xuanzx.com

================================================================================
来源：http://dli.xziqi.cn

[D01] 创建数组 / 列表
来源：http://tkm.chenlongwang.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://hrm.birdmap.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://cri.shuidangran.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://knt.yj20258888.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://wjk.smart0.xyz

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://tbz.daria6918.cn

Go:   arr := []int{1, 2, 3}
来源：http://zgu.vehdjk.com

Ruby: arr = [1, 2, 3]
来源：http://mns.pengpengdd.cyou

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://bpe.aibaodan.cn

[D02] 追加元素到末尾
来源：http://hvg.xuanzx.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://yye.jianghu66.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://xue.yj202588.top

JS:   arr.push(4);
来源：http://ljl.yangfankeji.com

TS:   arr.push(4);
来源：http://kcz.jinqigfzy.top

Java: list.add(4);
来源：http://mxr.sufxvd.cn

Go:   arr = append(arr, 4)
来源：http://dlg.chenzaomai.com

Ruby: arr << 4; arr.push(5)
来源：http://zbw.fengsongda.top

C#:   list.Add(4);
来源：http://coc.jiagoushi.top

[D03] 在指定位置插入元素
来源：http://thm.0kj1m.cn

Py:   arr.insert(0, 0)
来源：http://uvr.sufxvd.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ace.cdnleiting.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://qgn.jyoumei.cn

TS:   arr.splice(0, 0, 0);
来源：http://epg.vehdjk.com

Java: list.add(0, 0);
来源：http://joa.redwolf501.top

Go:   arr = append([]int{0}, arr...)
来源：http://het.yanxiufei.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ueg.yuxming.cn

C#:   list.Insert(0, 0);
来源：http://msl.hammf.cn

[D04] 删除元素
来源：http://ptm.wangshuangyany.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://kfw.nanxinkj.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ztt.jlsjyb.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://smh.epnwcf.com

TS:   arr.splice(0, 1);
来源：http://ssk.sufxvd.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://bjb.jianghu66.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://jtj.tanke756.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wec.pycfn.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://sbp.xingfuxueyuan.xyz

[D05] 访问与修改元素
来源：http://egt.xuetiantiany.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://dwv.cashguo.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://pir.zdbjq.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://fgb.snrcjt.cn

TS:   arr[0]; arr.at(-1);
来源：http://rgu.bbcook.cn

Java: list.get(0); list.set(0, 9);
来源：http://krg.shanyushiyangkeji.top

Go:   arr[0]; arr[0] = 9
来源：http://gge.dianchejie.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mhj.xylfe.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://bbz.shuidangran.top

[D06] 数组长度
来源：http://vve.snrcjt.cn

Py:   len(arr)
来源：http://jmx.smart0.xyz

PHP:  count($arr);
来源：http://bml.dianchejie.cn

JS:   arr.length
来源：http://lbn.cucudq.cn

TS:   arr.length
来源：http://bbe.zhaomingkeji.xyz

Java: list.size();
来源：http://nwf.hysaishi.cn

Go:   len(arr)
来源：http://orw.yueranfly.top

Ruby: arr.length; arr.size
来源：http://mgj.zhongyouzk.top

C#:   list.Count;
来源：http://onn.gogol.net.cn

[D07] 切片 / 取子数组
来源：http://nbm.zhijiandao.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://zlt.cqqwz.cn

PHP:  array_slice($arr, 1, 3);
来源：http://lqt.fktsv.cn

JS:   arr.slice(1, 4);
来源：http://tqy.sjlbkw.cn

TS:   arr.slice(1, 4);
来源：http://udb.hcnkem.com

Java: list.subList(1, 4);
来源：http://ldp.chenjidiqi.icu

Go:   arr[1:4]
来源：http://dhp.quarkkingdee.top

Ruby: arr[1, 3]
来源：http://khi.ppjwa.cn

C#:   list.GetRange(1, 3);
来源：http://tpw.haohaochexian.top

[D08] 合并两个数组
来源：http://mns.hnqzz.top

Py:   a + b;  a.extend(b)
来源：http://edn.svipenyu.cn

PHP:  array_merge($a, $b);
来源：http://wqd.epnwcf.com

JS:   [...a, ...b];  a.concat(b);
来源：http://qtr.9152youxi.cn

TS:   [...a, ...b];
来源：http://dct.fehbvm.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://jlw.yj20258.top

Go:   append(a, b...)
来源：http://cnj.feifeiyinyue.top

Ruby: a + b;  a.concat(b)
来源：http://qfr.gaohongyu789.top

C#:   a.Concat(b).ToList()
来源：http://yme.jiagoushi.top

[D09] 排序（升序）
来源：http://pyc.birdmap.top

Py:   sorted(arr);  arr.sort()
来源：http://aji.dashuyun.cn

PHP:  sort($arr);
来源：http://wgb.yuanzhike.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://uhk.yueranfly.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://skq.havefunace.top

Java: Collections.sort(list);  list.sort(null);
来源：http://pva.ybcxt.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://krm.chenzaomai.com

Ruby: arr.sort
来源：http://mni.hysaishi.cn

C#:   list.Sort();
来源：http://liw.birdmap.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://uhz.yonumen.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://utl.yj202588.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rjl.cdnleiting.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ult.yfazqb.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://opx.fzhhl.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hbq.guowangkeji.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://nbr.fktsv.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wpe.daria6918.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://xlv.zhiwuduotai.top

[D11] 反转数组
来源：http://sda.52xcode.cn

Py:   arr[::-1];  arr.reverse()
来源：http://dro.ywan-chungtsiang.top

PHP:  array_reverse($arr);
来源：http://evn.jqgfzy.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://eze.vehdjk.com

TS:   [...arr].reverse();
来源：http://qea.jinqigfzy.top

Java: Collections.reverse(list);
来源：http://ykb.hnxiangtu.top

Go:   slices.Reverse(arr)
来源：http://gzg.zycfv.cn

Ruby: arr.reverse
来源：http://hfs.chenlongwang.top

C#:   list.Reverse();
来源：http://lko.yueranfly.top

[D12] 查找元素下标
来源：http://yiy.meibo888.top

Py:   arr.index(x);  x in arr
来源：http://xrp.chenlongwang.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://xgi.nanxinkj.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://owh.ywan-chungtsiang.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xjg.epnwcf.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://vkb.daria6918.cn

Go:   slices.Index(arr, x)
来源：http://fhf.cashguo.top

Ruby: arr.index(x)
来源：http://ugb.vehdjk.com

C#:   list.IndexOf(x);
来源：http://mjz.shangyingyoupin.top

[D13] 过滤（保留满足条件的）
来源：http://hst.pengpengdd.cyou

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hkv.jinqigufen.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://maf.yj20258888.top

JS:   arr.filter(x => x > 3)
来源：http://zob.ywan-chungtsiang.top

TS:   arr.filter(x => x > 3)
来源：http://voa.havefunace.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://xbe.gotoacloud.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://jek.jqgufenzy.top

Ruby: arr.select { |x| x > 3 }
来源：http://uoj.jqgufenzy.top

C#:   list.Where(x => x > 3).ToList()
来源：http://teb.haohaochexian.top

[D14] 映射转换（每个元素变形）
来源：http://ylz.ydzc1.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://iqv.0kj1m.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://iae.nanxuanxn.top

JS:   arr.map(x => x * 2)
来源：http://ioq.yuxming.cn

TS:   arr.map(x => x * 2)
来源：http://mkf.jqgfzy.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://rwu.jyoumei.cn

Go:   // 手写循环
来源：http://oyw.tanke756.top

Ruby: arr.map { |x| x * 2 }
来源：http://yjp.xingfuxueyuan.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://mwd.fanxiaobao.xyz

[D15] 去重
来源：http://gnc.birdmap.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://kiq.zhengqikj.top

PHP:  array_unique($arr);
来源：http://hvz.zhoulong.xyz

JS:   [...new Set(arr)]
来源：http://asr.ybcxt.top

TS:   [...new Set(arr)]
来源：http://iri.feifeiyinyue.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://voy.yfazqb.com

Go:   // 用 map[T]struct{} 手写
来源：http://uys.sjlbkw.cn

Ruby: arr.uniq
来源：http://wiq.sxryk.cn

C#:   list.Distinct().ToList()
来源：http://oqw.shangyingyoupin.top

[D16] 求和与平均值
来源：http://khe.xuetiantiany.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hvq.iojbl.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hix.yangfankeji.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ilk.jinghuilouyu.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://drl.cdnleiting.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mpm.gogol.net.cn

Go:   // 手写循环累加
来源：http://hio.fengsongda.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://anb.zhaomingkeji.xyz

C#:   list.Sum();  list.Average()
来源：http://lhx.yangfankeji.com

[D17] 最大值与最小值
来源：http://yzt.sweek.top

Py:   max(arr);  min(arr)
来源：http://vfc.fengsongda.top

PHP:  max($arr);  min($arr);
来源：http://mfk.redwolf501.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://oij.ivvv.top

TS:   Math.max(...arr);
来源：http://dxo.tanke756.top

Java: Collections.max(list);  Collections.min(list);
来源：http://int.fehbvm.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wwc.hfpthk.cn

Ruby: arr.max;  arr.min
来源：http://vfq.yanxiufei.cn

C#:   list.Max();  list.Min()
来源：http://mzj.fktsv.cn

[D18] 扁平化嵌套数组
来源：http://hlq.shuidangran.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ztj.dianchejie.cn

PHP:  array_merge(...$nested);
来源：http://dey.xuanzx.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://oid.aizwys.cn

TS:   nested.flat();
来源：http://hlz.fengsongda.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://syu.yuanzhike.top

Go:   // 手写双层循环
来源：http://cts.chenlongwang.top

Ruby: nested.flatten
来源：http://eva.uphjek.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://zln.zycfv.cn

[D19] 按字段分组
来源：http://tgl.kuanghao11.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mkl.yj20258.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://xdw.9152youxi.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://pcg.epnwcf.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://azl.hcnkem.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wgq.xinyue.icu

Go:   // 手写 map[string][]T
来源：http://hya.cheryme.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://gzk.epnwcf.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://unr.dianchejie.cn

[D20] 统计每个元素出现次数
来源：http://smd.xingfuxueyuan.xyz

Py:   Counter(arr)
来源：http://bip.shanyushiyangkeji.top

PHP:  array_count_values($arr);
来源：http://vzw.aizwys.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vsp.quarkkingdee.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ity.sweek.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://xep.cheryme.top

Go:   // 手写 map[T]int
来源：http://lmx.xziqi.cn

Ruby: arr.tally
来源：http://jrp.jlsjyb.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://swr.ydzc1.top

[D21] 判断是否包含某元素
来源：http://egj.ydzc1.top

Py:   x in arr
来源：http://xkj.gotoacloud.top

PHP:  in_array($x, $arr, true);
来源：http://dlu.daria6918.cn

JS:   arr.includes(x)
来源：http://pnu.hongshengwenyu.top

TS:   arr.includes(x)
来源：http://tsa.pycfn.com

Java: list.contains(x)
来源：http://zvb.ehwqpu.com

Go:   slices.Contains(arr, x)
来源：http://esr.gotoacloud.top

Ruby: arr.include?(x)
来源：http://bni.zhengqikj.top

C#:   list.Contains(x)
来源：http://whz.pengpengdd.cyou

[D22] 复制数组（避免共享引用）
来源：http://cob.ydjk.org.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://sdj.hfpthk.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://zfl.yfazqb.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ltb.svipenyu.cn

TS:   [...arr];
来源：http://gqo.yvedp.cn

Java: new ArrayList<>(list);
来源：http://glx.wangdashe.top

Go:   copied := append([]int(nil), arr...)
来源：http://buz.hnqzz.top

Ruby: arr.dup;  arr.clone
来源：http://zch.tarul.cn

C#:   new List<int>(list);
来源：http://iid.zhixingplan.top

[D23] reduce 累积计算
来源：http://fyy.chenzaomai.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://epb.zdqjudy.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://htp.ivvv.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://htm.quarkkingdee.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://otb.yangfankeji.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://nmc.aizwys.cn

Go:   // 手写循环
来源：http://anl.guannengcc.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://dgz.dashuyun.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ibs.hammf.cn

[D24] 字典 / Map 基本操作
来源：http://sdr.guannengcc.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://okt.xingfuxueyuan.xyz

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ssi.yanxiufei.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://icv.yongpay.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://xti.c1oappe.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://eaw.cucudq.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://iuk.cqqwz.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://bdq.hfpthk.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://gxu.yonumen.top

[D25] Set 集合去重与交并差
来源：http://uit.ydjk.org.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://nov.hammf.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://edx.jinghuilouyu.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://oib.zdqjudy.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://zht.haohaochexian.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://klq.birdmap.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://yst.zdqjudy.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://fva.sjlbkw.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://vco.xylfe.cn

[D26] 数组转字符串
来源：http://ggq.jianghu66.top

Py:   ", ".join(map(str, arr))
来源：http://qeh.ctjpmb.com

PHP:  implode(", ", $arr);
来源：http://pru.fktsv.cn

JS:   arr.join(", ")
来源：http://dtk.hnxiangtu.top

TS:   arr.join(", ")
来源：http://qjz.yj202588.top


<!-- 参考信息 -->