代发 wailian999

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://xbd.daria6918.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ori.dashuyun.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://yuw.jyoumei.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://jug.fanxiaobao.xyz

[C10] 变量作用域
来源：http://jyg.shangyingyoupin.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://cik.fktsv.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ajl.cheryme.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mha.meibo888.top

TS:   同 JS
来源：http://dpy.tian-w.cn

Java: 方法内为块级作用域
来源：http://jvy.epnwcf.com

Go:   花括号块级作用域
来源：http://pqn.xylfe.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://lcf.feifeiyinyue.top

C#:   块级作用域
来源：http://ivr.yvedp.cn

[C11] 模块导入与导出
来源：http://ucx.dashuyun.cn

Py:   from module import func
来源：http://uvh.tianlin.xyz

PHP:  require "file.php";  或 use App\Service;
来源：http://qju.316326.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://ske.ybcxt.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xts.redwolf501.top

Java: import java.util.List;
来源：http://ewo.yanxiufei.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://por.haohaochexian.top

Ruby: require "json"; require_relative "./util"
来源：http://fva.hammf.cn

C#:   using System.Text;
来源：http://vmm.yj202588.top

[C12] 立即执行函数 IIFE
来源：http://miq.shuidangran.top

Py:   (lambda: print("run"))()
来源：http://iac.sweek.top

PHP:  (function () { echo "run"; })();
来源：http://nsu.ywan-chungtsiang.top

JS:   (() => { console.log("run"); })();
来源：http://wrg.jqgfzy.top

TS:   (() => { console.log("run"); })();
来源：http://abu.jqgufenzy.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://zue.jyoumei.cn

Go:   func() { fmt.Println("run") }()
来源：http://jbf.zhixingplan.top

Ruby: -> { puts "run" }.call
来源：http://dge.wangdashe.top

C#:   // 无 IIFE：用静态构造函数
来源：http://qlz.havefunace.top

[C13] 类型声明 / 类型注解
来源：http://qou.cashguo.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://lfc.wangshuangyany.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vyd.gaohongyu789.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://plc.jinqigufen.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rvk.kuanghao11.cn

Java: int add(int a, int b) { return a + b; }
来源：http://rqk.redwolf501.top

Go:   func add(a, b int) int
来源：http://usu.cheryme.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://kdg.guowangkeji.top

C#:   int Add(int a, int b) => a + b;
来源：http://akn.zhiwuduotai.top

[C14] 泛型函数
来源：http://pgr.uphjek.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://tbj.andypj.xyz

PHP:  // 无泛型
来源：http://old.ydjk.org.cn

JS:   // 无泛型
来源：http://rqo.zhongyouzk.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://leb.zhengqikj.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://nlb.yj20258888.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://keu.xuetiantiany.cn

Ruby: # 无泛型
来源：http://gsv.c1oappe.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://zfh.dianchejie.cn

[C15] 解构 / 展开参数
来源：http://agw.zycfv.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mjl.guowangkeji.top

PHP:  [$a, $b] = $pair;
来源：http://bhs.yuanzhike.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://okf.tanke756.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hpu.tarul.cn

Java: // 无解构
来源：http://ihm.redwolf501.top

Go:   // 无解构
来源：http://jtj.fehbvm.com

Ruby: a, b = pair
来源：http://miv.bbcook.cn

C#:   var (a, b) = pair;
来源：http://xhw.ehwqpu.com

[C16] 函数 / 方法重载
来源：http://bsn.nanxuanxn.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://zoj.meibo888.top

PHP:  // 无重载
来源：http://xvj.xingfuxueyuan.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://wqd.dianchejie.cn

TS:   // 用联合类型或重载签名声明
来源：http://qdn.zdbjq.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://asn.vqdsnc.cn

Go:   // 无重载：用不同函数名
来源：http://fef.ywan-chungtsiang.top

Ruby: # 无重载：靠动态参数
来源：http://cxa.epnwcf.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://gof.jyoumei.cn

================================================================================
来源：http://iqw.yanxiufei.cn

D. 数组 / 列表 / 集合
来源：http://qgf.jyoumei.cn

================================================================================
来源：http://jwn.ppjwa.cn

[D01] 创建数组 / 列表
来源：http://sed.guowangkeji.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://zko.jianghu66.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hbj.zhaomingkeji.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ynj.kuanghao11.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://sgg.shangyingyoupin.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://zes.aizwys.cn

Go:   arr := []int{1, 2, 3}
来源：http://bfs.svipenyu.cn

Ruby: arr = [1, 2, 3]
来源：http://qlm.wangshuangyany.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ink.zycfv.cn

[D02] 追加元素到末尾
来源：http://zue.hysaishi.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://asq.hongshengwenyu.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wpp.yonumen.top

JS:   arr.push(4);
来源：http://ijw.wangshuangyany.cn

TS:   arr.push(4);
来源：http://ijk.tian-w.cn

Java: list.add(4);
来源：http://uus.ehwqpu.com

Go:   arr = append(arr, 4)
来源：http://nso.yj20258.top

Ruby: arr << 4; arr.push(5)
来源：http://iwy.cucudq.cn

C#:   list.Add(4);
来源：http://gsb.gogol.net.cn

[D03] 在指定位置插入元素
来源：http://jaq.hysaishi.cn

Py:   arr.insert(0, 0)
来源：http://cax.jinqigfzy.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://rtt.ydjk.org.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://toz.316326.xyz

TS:   arr.splice(0, 0, 0);
来源：http://soq.chenzaomai.com

Java: list.add(0, 0);
来源：http://wqx.yonumen.top

Go:   arr = append([]int{0}, arr...)
来源：http://okz.gzhubu.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ybd.sxryk.cn

C#:   list.Insert(0, 0);
来源：http://cof.zhoulong.xyz

[D04] 删除元素
来源：http://lmt.tian-w.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ixl.gotoacloud.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ebs.cdnleiting.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ayg.svipenyu.cn

TS:   arr.splice(0, 1);
来源：http://jbs.snrcjt.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://aah.vqdsnc.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://oea.jinghuilouyu.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://uow.ppjwa.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://oia.cheryme.top

[D05] 访问与修改元素
来源：http://hsx.fktsv.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://qst.tian-w.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://qfy.yuanzhike.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://nbo.yj20258888.top

TS:   arr[0]; arr.at(-1);
来源：http://ufz.hesvh.cn

Java: list.get(0); list.set(0, 9);
来源：http://vvm.wangdashe.top

Go:   arr[0]; arr[0] = 9
来源：http://hzp.hcnkem.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://gor.andypj.xyz

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://xhu.fanxiaobao.xyz

[D06] 数组长度
来源：http://bst.xuetiantiany.cn

Py:   len(arr)
来源：http://xas.guannengcc.top

PHP:  count($arr);
来源：http://pzl.ywan-chungtsiang.top

JS:   arr.length
来源：http://twa.ppjwa.cn

TS:   arr.length
来源：http://edj.0kj1m.cn

Java: list.size();
来源：http://azc.yj20258888.top

Go:   len(arr)
来源：http://uao.bjfxy.top

Ruby: arr.length; arr.size
来源：http://aip.ivvv.top

C#:   list.Count;
来源：http://vvo.xinyue.icu

[D07] 切片 / 取子数组
来源：http://esm.chenjidiqi.icu

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://cuv.jianghu66.top

PHP:  array_slice($arr, 1, 3);
来源：http://nyv.vehdjk.com

JS:   arr.slice(1, 4);
来源：http://byx.meibo888.top

TS:   arr.slice(1, 4);
来源：http://ide.bjfxy.top

Java: list.subList(1, 4);
来源：http://vzd.hammf.cn

Go:   arr[1:4]
来源：http://mta.hcnkem.com

Ruby: arr[1, 3]
来源：http://tjl.ywan-chungtsiang.top

C#:   list.GetRange(1, 3);
来源：http://dfo.jqgufenzy.top

[D08] 合并两个数组
来源：http://bti.hnxiangtu.top

Py:   a + b;  a.extend(b)
来源：http://ovk.uphjek.com

PHP:  array_merge($a, $b);
来源：http://tjl.316326.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://hts.yongpay.top

TS:   [...a, ...b];
来源：http://ita.iojbl.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://xwq.gzhubu.top

Go:   append(a, b...)
来源：http://rlv.sysykeji.top

Ruby: a + b;  a.concat(b)
来源：http://txx.fanxiaobao.xyz

C#:   a.Concat(b).ToList()
来源：http://xyw.yj202588.top

[D09] 排序（升序）
来源：http://jxp.gzhubu.top

Py:   sorted(arr);  arr.sort()
来源：http://sdf.shangyingyoupin.top

PHP:  sort($arr);
来源：http://dry.guannengcc.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://auz.zhijiandao.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://qah.jyoumei.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://uxt.sufxvd.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://tqh.haohaochexian.top

Ruby: arr.sort
来源：http://gww.gotoacloud.top

C#:   list.Sort();
来源：http://wnc.daxiang520.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://lve.hesvh.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://eku.hesvh.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://auz.vqdsnc.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://eai.yangfankeji.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://rty.nanxuanxn.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://fqr.52xcode.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://vxb.jiagoushi.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://tih.nanxinkj.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://laj.xinyue.icu

[D11] 反转数组
来源：http://cya.sxryk.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ksp.smart0.xyz

PHP:  array_reverse($arr);
来源：http://vfr.jinyuanbaomall.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://pxm.redwolf501.top

TS:   [...arr].reverse();
来源：http://ebo.wangshuangyany.cn

Java: Collections.reverse(list);
来源：http://jyd.birdmap.top

Go:   slices.Reverse(arr)
来源：http://dbj.smart0.xyz

Ruby: arr.reverse
来源：http://exe.bbcook.cn

C#:   list.Reverse();
来源：http://wev.snrcjt.cn

[D12] 查找元素下标
来源：http://qek.jqgufenzy.top

Py:   arr.index(x);  x in arr
来源：http://gyd.jinqigufen.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://gxe.zhongyouzk.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pgw.zhongyouzk.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bof.nanxuanxn.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://afg.316326.xyz

Go:   slices.Index(arr, x)
来源：http://uxf.xziqi.cn

Ruby: arr.index(x)
来源：http://dxz.jinqigfzy.top

C#:   list.IndexOf(x);
来源：http://azr.ydjk.org.cn

[D13] 过滤（保留满足条件的）
来源：http://pky.yuanzhike.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://reo.wangdashe.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://zui.xylfe.cn

JS:   arr.filter(x => x > 3)
来源：http://gck.sxryk.cn

TS:   arr.filter(x => x > 3)
来源：http://rmr.zhaomingkeji.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://rwx.jinqigufen.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://kkm.wangshuangyany.cn

Ruby: arr.select { |x| x > 3 }
来源：http://nkg.yj20258.top

C#:   list.Where(x => x > 3).ToList()
来源：http://pcz.zycfv.cn

[D14] 映射转换（每个元素变形）
来源：http://icd.shanyushiyangtech.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xbu.daxiang520.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://cjj.sweek.top

JS:   arr.map(x => x * 2)
来源：http://wbf.cqqwz.cn

TS:   arr.map(x => x * 2)
来源：http://qws.meibo888.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://vls.yuxming.cn

Go:   // 手写循环
来源：http://tdi.cdnleiting.top

Ruby: arr.map { |x| x * 2 }
来源：http://cdj.yonumen.top

C#:   list.Select(x => x * 2).ToList()
来源：http://zsy.jqgfzy.top

[D15] 去重
来源：http://bhg.aizwys.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mib.9152youxi.cn

PHP:  array_unique($arr);
来源：http://jfd.yonumen.top

JS:   [...new Set(arr)]
来源：http://xef.bjfxy.top

TS:   [...new Set(arr)]
来源：http://ggq.jiagoushi.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://eue.zycfv.cn

Go:   // 用 map[T]struct{} 手写
来源：http://dhz.9152youxi.cn

Ruby: arr.uniq
来源：http://rhl.gogol.net.cn

C#:   list.Distinct().ToList()
来源：http://twq.tianlin.xyz

[D16] 求和与平均值
来源：http://kpn.vqdsnc.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://pyd.feifeiyinyue.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mee.fktsv.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://jfu.fehbvm.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://skl.pengpengdd.cyou

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://tct.aibaodan.cn

Go:   // 手写循环累加
来源：http://lfu.aizwys.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://kij.uphjek.com

C#:   list.Sum();  list.Average()
来源：http://igm.ywan-chungtsiang.top

[D17] 最大值与最小值
来源：http://kqu.kuanghao11.cn

Py:   max(arr);  min(arr)
来源：http://plf.zhijiandao.cn

PHP:  max($arr);  min($arr);
来源：http://zrm.yonumen.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mbs.sufxvd.cn

TS:   Math.max(...arr);
来源：http://aph.ivvv.top

Java: Collections.max(list);  Collections.min(list);
来源：http://ajy.cdnleiting.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ncj.yj20258888.top

Ruby: arr.max;  arr.min
来源：http://hiv.zhengqikj.top

C#:   list.Max();  list.Min()
来源：http://lpr.jianghu66.top

[D18] 扁平化嵌套数组
来源：http://vit.chenlongwang.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://uvu.hnqzz.top

PHP:  array_merge(...$nested);
来源：http://ldx.ydzc1.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://njv.pycfn.com

TS:   nested.flat();
来源：http://zzm.haohaochexian.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://toe.chenzaomai.com

Go:   // 手写双层循环
来源：http://pko.zhaomingkeji.xyz

Ruby: nested.flatten
来源：http://xuz.hfpthk.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://rzs.xingfuxueyuan.xyz

[D19] 按字段分组
来源：http://yfw.9152youxi.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://oqg.gotoacloud.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://iqj.chenjidiqi.icu

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://eyx.shuidangran.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://yil.wangdashe.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://lmb.shanyushiyangkeji.top

Go:   // 手写 map[string][]T
来源：http://kpc.yfazqb.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://gha.wangdashe.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://gby.sweek.top

[D20] 统计每个元素出现次数
来源：http://zym.cheryme.top

Py:   Counter(arr)
来源：http://zoj.pycfn.com

PHP:  array_count_values($arr);
来源：http://qow.andypj.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vyo.sufxvd.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fcu.yvedp.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://sdt.chenzaomai.com

Go:   // 手写 map[T]int
来源：http://nbb.jinqigufen.top

Ruby: arr.tally
来源：http://lat.yvedp.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ufu.hongshengwenyu.top

[D21] 判断是否包含某元素
来源：http://mkp.haohaochexian.top

Py:   x in arr
来源：http://iko.bjfxy.top

PHP:  in_array($x, $arr, true);
来源：http://lbp.kuanghao11.cn

JS:   arr.includes(x)
来源：http://pja.fanxiaobao.xyz

TS:   arr.includes(x)
来源：http://xgo.yonumen.top

Java: list.contains(x)
来源：http://wgd.wangshuangyany.cn

Go:   slices.Contains(arr, x)
来源：http://puw.birdmap.top

Ruby: arr.include?(x)
来源：http://hgu.guannengcc.top

C#:   list.Contains(x)
来源：http://kgm.hnqzz.top

[D22] 复制数组（避免共享引用）
来源：http://dud.zycfv.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mbh.zdbjq.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://fpd.yj20258.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://naf.iojbl.cn

TS:   [...arr];
来源：http://pbn.pycfn.com

Java: new ArrayList<>(list);
来源：http://jja.bbcook.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ryk.shzxlz.cn

Ruby: arr.dup;  arr.clone
来源：http://xej.bbcook.cn

C#:   new List<int>(list);
来源：http://lvx.tianlin.xyz

[D23] reduce 累积计算
来源：http://vxa.cdnleiting.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wfm.jinghuilouyu.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ufn.yuanzhike.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tnq.jinghuilouyu.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ycu.yangfankeji.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://vkr.jinqigfzy.top

Go:   // 手写循环
来源：http://wpl.jinqigufen.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://jct.chenjidiqi.icu

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wyl.fengsongda.top

[D24] 字典 / Map 基本操作
来源：http://osn.shanyushiyangkeji.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://bcg.gaohongyu789.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://exm.ehwqpu.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mvh.hfpthk.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://tzu.zhengqikj.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://tvi.fanxiaobao.xyz

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://fnw.kuanghao11.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://qtb.xziqi.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://vnu.wangshuangyany.cn

[D25] Set 集合去重与交并差
来源：http://rab.wangshuangyany.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wkn.fzhhl.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://txd.ppjwa.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ggu.daxiang520.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://jgy.redwolf501.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://zgz.jianghu66.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://vbp.ywan-chungtsiang.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://dfb.haohaochexian.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://tcp.pycfn.com

[D26] 数组转字符串
来源：http://sig.ehwqpu.com

Py:   ", ".join(map(str, arr))
来源：http://gmg.gzhubu.top

PHP:  implode(", ", $arr);
来源：http://mjj.hnqzz.top

JS:   arr.join(", ")
来源：http://eaj.aizwys.cn

TS:   arr.join(", ")
来源：http://bkb.yangfankeji.com


<!-- 参考信息 -->