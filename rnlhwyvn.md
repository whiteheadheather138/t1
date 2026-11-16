代发 wailian999

[C10] 变量作用域
来源：http://gsk.dianchejie.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://vlr.jqgfzy.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ryx.yuanzhike.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hkc.gogol.net.cn

TS:   同 JS
来源：http://qms.yonumen.top

Java: 方法内为块级作用域
来源：http://rcf.svipenyu.cn

Go:   花括号块级作用域
来源：http://voj.redwolf501.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ite.xingfuxueyuan.xyz

C#:   块级作用域
来源：http://fbo.guowangkeji.top

[C11] 模块导入与导出
来源：http://otn.fzhhl.top

Py:   from module import func
来源：http://ezl.jqgfzy.top

PHP:  require "file.php";  或 use App\Service;
来源：http://hmr.fktsv.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://fja.chenzaomai.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://kwh.jqgfzy.top

Java: import java.util.List;
来源：http://qtc.xuetiantiany.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://jpv.xuetiantiany.cn

Ruby: require "json"; require_relative "./util"
来源：http://xco.hesvh.cn

C#:   using System.Text;
来源：http://qzw.cashguo.top

[C12] 立即执行函数 IIFE
来源：http://pbh.mhx1999.top

Py:   (lambda: print("run"))()
来源：http://spr.9152youxi.cn

PHP:  (function () { echo "run"; })();
来源：http://nad.jlsjyb.cn

JS:   (() => { console.log("run"); })();
来源：http://rjh.ybcxt.top

TS:   (() => { console.log("run"); })();
来源：http://pyx.haohaochexian.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://knw.shuidangran.top

Go:   func() { fmt.Println("run") }()
来源：http://eou.jyoumei.cn

Ruby: -> { puts "run" }.call
来源：http://vwd.ywan-chungtsiang.top

C#:   // 无 IIFE：用静态构造函数
来源：http://ppy.daria6918.cn

[C13] 类型声明 / 类型注解
来源：http://lpg.jinyuanbaomall.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://nxa.zhixingplan.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://shj.jiagoushi.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://vdn.redwolf501.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nfd.aizwys.cn

Java: int add(int a, int b) { return a + b; }
来源：http://hss.zhengqikj.top

Go:   func add(a, b int) int
来源：http://fge.ydjk.org.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://qce.shzxlz.cn

C#:   int Add(int a, int b) => a + b;
来源：http://txb.c1oappe.top

[C14] 泛型函数
来源：http://pde.zhaomingkeji.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://orx.xziqi.cn

PHP:  // 无泛型
来源：http://mat.vehdjk.com

JS:   // 无泛型
来源：http://yvf.iojbl.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ncg.zdbjq.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mni.xuetiantiany.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://emc.ydzc1.top

Ruby: # 无泛型
来源：http://lkv.pengpengdd.cyou

C#:   static T First<T>(List<T> items) => items[0];
来源：http://chz.xziqi.cn

[C15] 解构 / 展开参数
来源：http://xqh.andypj.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://lxg.mhx1999.top

PHP:  [$a, $b] = $pair;
来源：http://dog.shanyushiyangtech.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://jes.ywan-chungtsiang.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://tvj.xuanzx.com

Java: // 无解构
来源：http://wed.sjlbkw.cn

Go:   // 无解构
来源：http://tsp.yj202588.top

Ruby: a, b = pair
来源：http://ltx.gaohongyu789.top

C#:   var (a, b) = pair;
来源：http://fow.redwolf501.top

[C16] 函数 / 方法重载
来源：http://tvr.sjlbkw.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ncj.ctjpmb.com

PHP:  // 无重载
来源：http://ylj.haohaochexian.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://tng.jqgfzy.top

TS:   // 用联合类型或重载签名声明
来源：http://ktp.mhx1999.top

Java: void f(int a) {}  void f(String a) {}
来源：http://lsv.xylfe.cn

Go:   // 无重载：用不同函数名
来源：http://bzg.yueranfly.top

Ruby: # 无重载：靠动态参数
来源：http://zca.ybcxt.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://zxj.ivvv.top

================================================================================
来源：http://uky.jyoumei.cn

D. 数组 / 列表 / 集合
来源：http://fkn.xziqi.cn

================================================================================
来源：http://epf.fehbvm.com

[D01] 创建数组 / 列表
来源：http://zva.zycfv.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://xur.snrcjt.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://bvu.yj202588.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wqh.ydzc1.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://blx.cdnleiting.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://vjc.guannengcc.top

Go:   arr := []int{1, 2, 3}
来源：http://cda.yongpay.top

Ruby: arr = [1, 2, 3]
来源：http://pdh.cashguo.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hwb.xylfe.cn

[D02] 追加元素到末尾
来源：http://grt.sweek.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wih.yangfankeji.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://vdk.fanxiaobao.xyz

JS:   arr.push(4);
来源：http://fxi.hfpthk.cn

TS:   arr.push(4);
来源：http://ura.sufxvd.cn

Java: list.add(4);
来源：http://ndc.wangdashe.top

Go:   arr = append(arr, 4)
来源：http://xxc.jianghu66.top

Ruby: arr << 4; arr.push(5)
来源：http://svz.yuanzhike.top

C#:   list.Add(4);
来源：http://phb.ivvv.top

[D03] 在指定位置插入元素
来源：http://jra.zycfv.cn

Py:   arr.insert(0, 0)
来源：http://zsa.fzhhl.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://jkx.xziqi.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://myz.aibaodan.cn

TS:   arr.splice(0, 0, 0);
来源：http://asc.gzhubu.top

Java: list.add(0, 0);
来源：http://hhb.ivvv.top

Go:   arr = append([]int{0}, arr...)
来源：http://gze.ydjk.org.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://zbi.pengpengdd.cyou

C#:   list.Insert(0, 0);
来源：http://ptj.yongpay.top

[D04] 删除元素
来源：http://vzr.daria6918.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ylh.9152youxi.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ibk.guowangkeji.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://anm.havefunace.top

TS:   arr.splice(0, 1);
来源：http://msg.daxiang520.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://uxh.fengsongda.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://eed.zycfv.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mmw.guannengcc.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://lyk.zdqjudy.top

[D05] 访问与修改元素
来源：http://ksj.316326.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ipc.zhengqikj.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://alj.feifeiyinyue.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ndi.fehbvm.com

TS:   arr[0]; arr.at(-1);
来源：http://mcy.ybcxt.top

Java: list.get(0); list.set(0, 9);
来源：http://kte.redwolf501.top

Go:   arr[0]; arr[0] = 9
来源：http://kaw.yueranfly.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://dau.xziqi.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ull.aizwys.cn

[D06] 数组长度
来源：http://pmw.redwolf501.top

Py:   len(arr)
来源：http://frn.xingfuxueyuan.xyz

PHP:  count($arr);
来源：http://qtb.bjfxy.top

JS:   arr.length
来源：http://tit.quarkkingdee.top

TS:   arr.length
来源：http://rcz.ivvv.top

Java: list.size();
来源：http://rgc.zdqjudy.top

Go:   len(arr)
来源：http://hcp.cheryme.top

Ruby: arr.length; arr.size
来源：http://tfh.hcnkem.com

C#:   list.Count;
来源：http://gdp.iojbl.cn

[D07] 切片 / 取子数组
来源：http://ruy.shuidangran.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ema.chenzaomai.com

PHP:  array_slice($arr, 1, 3);
来源：http://idt.sxryk.cn

JS:   arr.slice(1, 4);
来源：http://zan.ivvv.top

TS:   arr.slice(1, 4);
来源：http://sqt.gzhubu.top

Java: list.subList(1, 4);
来源：http://iob.xuetiantiany.cn

Go:   arr[1:4]
来源：http://lir.dianchejie.cn

Ruby: arr[1, 3]
来源：http://jdu.dianchejie.cn

C#:   list.GetRange(1, 3);
来源：http://tux.daxiang520.top

[D08] 合并两个数组
来源：http://afc.zhixingplan.top

Py:   a + b;  a.extend(b)
来源：http://lra.wangdashe.top

PHP:  array_merge($a, $b);
来源：http://yhx.yuanzhike.top

JS:   [...a, ...b];  a.concat(b);
来源：http://dyr.gzhubu.top

TS:   [...a, ...b];
来源：http://iay.xziqi.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://fhu.dashuyun.cn

Go:   append(a, b...)
来源：http://jwa.shzxlz.cn

Ruby: a + b;  a.concat(b)
来源：http://atz.uphjek.com

C#:   a.Concat(b).ToList()
来源：http://klz.xziqi.cn

[D09] 排序（升序）
来源：http://okf.bbcook.cn

Py:   sorted(arr);  arr.sort()
来源：http://dyv.snrcjt.cn

PHP:  sort($arr);
来源：http://itt.bbcook.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://nsi.mhx1999.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://cnz.zdbjq.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://oqb.hnxiangtu.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://rqr.aizwys.cn

Ruby: arr.sort
来源：http://cey.hywenlv.cn

C#:   list.Sort();
来源：http://nla.fengsongda.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://biw.sweek.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qyc.yuanzhike.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nna.hnqzz.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wce.shzxlz.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://iip.yj202588.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ycr.iojbl.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://tnt.fehbvm.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://qdx.shuidangran.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://aij.nanxuanxn.top

[D11] 反转数组
来源：http://zid.zhongyouzk.top

Py:   arr[::-1];  arr.reverse()
来源：http://pny.jianghu66.top

PHP:  array_reverse($arr);
来源：http://yjr.pycfn.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://gnz.0kj1m.cn

TS:   [...arr].reverse();
来源：http://xhb.52xcode.cn

Java: Collections.reverse(list);
来源：http://vry.jinqigufen.top

Go:   slices.Reverse(arr)
来源：http://xjm.hcnkem.com

Ruby: arr.reverse
来源：http://dxu.ctjpmb.com

C#:   list.Reverse();
来源：http://kqr.smart0.xyz

[D12] 查找元素下标
来源：http://vxi.guannengcc.top

Py:   arr.index(x);  x in arr
来源：http://dmj.shangyingyoupin.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://cnn.c1oappe.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://syt.tian-w.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xdv.daxiang520.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wxa.ybcxt.top

Go:   slices.Index(arr, x)
来源：http://eyq.hnqzz.top

Ruby: arr.index(x)
来源：http://hyc.ivvv.top

C#:   list.IndexOf(x);
来源：http://usa.bjfxy.top

[D13] 过滤（保留满足条件的）
来源：http://ray.c1oappe.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://oin.fehbvm.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://dpb.hnxiangtu.top

JS:   arr.filter(x => x > 3)
来源：http://wjh.tianlin.xyz

TS:   arr.filter(x => x > 3)
来源：http://bqb.yangfankeji.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://alv.yuxming.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://orr.hywenlv.cn

Ruby: arr.select { |x| x > 3 }
来源：http://xwe.fktsv.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://pvs.mhx1999.top

[D14] 映射转换（每个元素变形）
来源：http://qzk.guannengcc.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hup.zycfv.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://rjs.ctjpmb.com

JS:   arr.map(x => x * 2)
来源：http://pqk.jyoumei.cn

TS:   arr.map(x => x * 2)
来源：http://zya.daxiang520.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://ujj.daxiang520.top

Go:   // 手写循环
来源：http://upo.vqdsnc.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ymw.ywan-chungtsiang.top

C#:   list.Select(x => x * 2).ToList()
来源：http://mkf.jinqigufen.top

[D15] 去重
来源：http://ysd.cucudq.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://xmc.shanyushiyangtech.top

PHP:  array_unique($arr);
来源：http://bld.cashguo.top

JS:   [...new Set(arr)]
来源：http://plm.pengpengdd.cyou

TS:   [...new Set(arr)]
来源：http://ucb.tian-w.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ohd.feifeiyinyue.top

Go:   // 用 map[T]struct{} 手写
来源：http://crb.cucudq.cn

Ruby: arr.uniq
来源：http://pyy.tarul.cn

C#:   list.Distinct().ToList()
来源：http://xkh.yuxming.cn

[D16] 求和与平均值
来源：http://atd.jlsjyb.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://yhe.gzhubu.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://zya.ydzc1.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://yna.yongpay.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://orr.wangshuangyany.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ixe.hywenlv.cn

Go:   // 手写循环累加
来源：http://bcq.316326.xyz

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://jnj.sweek.top

C#:   list.Sum();  list.Average()
来源：http://yuz.hywenlv.cn

[D17] 最大值与最小值
来源：http://cbn.yueranfly.top

Py:   max(arr);  min(arr)
来源：http://hop.sjlbkw.cn

PHP:  max($arr);  min($arr);
来源：http://akw.chenjidiqi.icu

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wly.haohaochexian.top

TS:   Math.max(...arr);
来源：http://tie.jqgfzy.top

Java: Collections.max(list);  Collections.min(list);
来源：http://pvf.xuetiantiany.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://umx.nanxuanxn.top

Ruby: arr.max;  arr.min
来源：http://kqn.mhx1999.top

C#:   list.Max();  list.Min()
来源：http://vpw.aibaodan.cn

[D18] 扁平化嵌套数组
来源：http://wnx.epnwcf.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ezg.jiagoushi.top

PHP:  array_merge(...$nested);
来源：http://pmm.bjfxy.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://eaq.feifeiyinyue.top

TS:   nested.flat();
来源：http://iqj.hongshengwenyu.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://pgx.bbcook.cn

Go:   // 手写双层循环
来源：http://aye.hesvh.cn

Ruby: nested.flatten
来源：http://iif.chenlongwang.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://xqe.birdmap.top

[D19] 按字段分组
来源：http://gpm.cucudq.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://spq.daria6918.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ycl.xylfe.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://voe.nanxuanxn.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://gar.cqqwz.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hmd.daria6918.cn

Go:   // 手写 map[string][]T
来源：http://beu.haohaochexian.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://xgl.epnwcf.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://kda.gaohongyu789.top

[D20] 统计每个元素出现次数
来源：http://ygd.shzxlz.cn

Py:   Counter(arr)
来源：http://nqr.xuetiantiany.cn

PHP:  array_count_values($arr);
来源：http://opi.pycfn.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lej.ivvv.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mim.fehbvm.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ght.ybcxt.top

Go:   // 手写 map[T]int
来源：http://pea.yj20258888.top

Ruby: arr.tally
来源：http://jvm.sjlbkw.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wna.chenzaomai.com

[D21] 判断是否包含某元素
来源：http://drg.sweek.top

Py:   x in arr
来源：http://sdx.ppjwa.cn

PHP:  in_array($x, $arr, true);
来源：http://cak.zdbjq.cn

JS:   arr.includes(x)
来源：http://mmo.shangyingyoupin.top

TS:   arr.includes(x)
来源：http://vxb.zhixingplan.top

Java: list.contains(x)
来源：http://uht.hysaishi.cn

Go:   slices.Contains(arr, x)
来源：http://pii.dianchejie.cn

Ruby: arr.include?(x)
来源：http://eis.jlsjyb.cn

C#:   list.Contains(x)
来源：http://utw.xuanzx.com

[D22] 复制数组（避免共享引用）
来源：http://exd.pengpengdd.cyou

Py:   arr.copy();  arr[:];  list(arr)
来源：http://xgo.zhiwuduotai.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://nqj.svipenyu.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ygw.aibaodan.cn

TS:   [...arr];
来源：http://lnn.jinqigufen.top

Java: new ArrayList<>(list);
来源：http://nwd.tianlin.xyz

Go:   copied := append([]int(nil), arr...)
来源：http://cvy.hfpthk.cn

Ruby: arr.dup;  arr.clone
来源：http://ygu.nanxuanxn.top

C#:   new List<int>(list);
来源：http://sbt.nanxinkj.top

[D23] reduce 累积计算
来源：http://zpb.vqdsnc.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hnd.jinghuilouyu.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://bxk.hnqzz.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bap.9152youxi.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://uhw.zycfv.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://szb.hfpthk.cn

Go:   // 手写循环
来源：http://hye.zhixingplan.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://gtj.cheryme.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://tiz.yj202588.top

[D24] 字典 / Map 基本操作
来源：http://dui.ydzc1.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mne.wangdashe.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wrs.gaohongyu789.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://jaz.ydzc1.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://nkz.shuidangran.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mnj.jqgfzy.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://dft.gogol.net.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://lsh.hysaishi.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://uni.dianchejie.cn

[D25] Set 集合去重与交并差
来源：http://cks.smart0.xyz

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://aff.xziqi.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mwf.zycfv.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://doi.zhongyouzk.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mdc.shangyingyoupin.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://acw.tian-w.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://dpd.zhoulong.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://keu.hnxiangtu.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://rdf.shangyingyoupin.top

[D26] 数组转字符串
来源：http://plu.yj20258.top

Py:   ", ".join(map(str, arr))
来源：http://xcg.chenzaomai.com

PHP:  implode(", ", $arr);
来源：http://etz.jinyuanbaomall.cn

JS:   arr.join(", ")
来源：http://wun.zdbjq.cn

TS:   arr.join(", ")
来源：http://pfk.shanyushiyangtech.top

Java: String.join(", ", list)
来源：http://jjt.ivvv.top

Go:   strings.Join(strs, ", ")
来源：http://oik.sufxvd.cn

Ruby: arr.join(", ")
来源：http://pod.jqgufenzy.top

C#:   string.Join(", ", list)
来源：http://rpc.quarkkingdee.top


<!-- 参考信息 -->