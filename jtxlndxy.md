代发 wailian999

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://nwo.zhijiandao.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://amx.zhongyouzk.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ife.cashguo.top

[C09] 递归
来源：http://afb.hnxiangtu.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://kpw.cashguo.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ezx.hesvh.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pko.hcnkem.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zgp.nanxuanxn.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://dvy.shangyingyoupin.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://lsj.shuidangran.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://vrm.vqdsnc.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://kgq.jyoumei.cn

[C10] 变量作用域
来源：http://rzz.vqdsnc.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://nme.jinqigfzy.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://yyn.daxiang520.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wda.zhixingplan.top

TS:   同 JS
来源：http://ntf.guowangkeji.top

Java: 方法内为块级作用域
来源：http://pbz.gotoacloud.top

Go:   花括号块级作用域
来源：http://jsb.jlsjyb.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://qta.zhijiandao.cn

C#:   块级作用域
来源：http://vdx.sysykeji.top

[C11] 模块导入与导出
来源：http://eak.yueranfly.top

Py:   from module import func
来源：http://mgz.gaohongyu789.top

PHP:  require "file.php";  或 use App\Service;
来源：http://mtu.ehwqpu.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://yca.chenjidiqi.icu

TS:   export function f(): void {};  import { f } from "./m";
来源：http://rmp.gzhubu.top

Java: import java.util.List;
来源：http://sqg.ydzc1.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://oxv.ivvv.top

Ruby: require "json"; require_relative "./util"
来源：http://jkh.pycfn.com

C#:   using System.Text;
来源：http://yca.jinqigfzy.top

[C12] 立即执行函数 IIFE
来源：http://zig.jiagoushi.top

Py:   (lambda: print("run"))()
来源：http://nkd.ywan-chungtsiang.top

PHP:  (function () { echo "run"; })();
来源：http://eeq.redwolf501.top

JS:   (() => { console.log("run"); })();
来源：http://zsp.zdqjudy.top

TS:   (() => { console.log("run"); })();
来源：http://lfs.aibaodan.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://xuv.hywenlv.cn

Go:   func() { fmt.Println("run") }()
来源：http://fxc.ehwqpu.com

Ruby: -> { puts "run" }.call
来源：http://wqm.jinghuilouyu.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://jgn.pengpengdd.cyou

[C13] 类型声明 / 类型注解
来源：http://rig.xuanzx.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hbg.tianlin.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xgh.iojbl.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mao.hongshengwenyu.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yck.tarul.cn

Java: int add(int a, int b) { return a + b; }
来源：http://xft.sweek.top

Go:   func add(a, b int) int
来源：http://llq.hammf.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://xfl.sjlbkw.cn

C#:   int Add(int a, int b) => a + b;
来源：http://htz.gaohongyu789.top

[C14] 泛型函数
来源：http://ywo.zhongyouzk.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wzj.ywan-chungtsiang.top

PHP:  // 无泛型
来源：http://fhg.zhaomingkeji.xyz

JS:   // 无泛型
来源：http://wgo.fehbvm.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://cbw.sjlbkw.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://yur.hcnkem.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://pup.redwolf501.top

Ruby: # 无泛型
来源：http://zyr.chenzaomai.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://iwf.mhx1999.top

[C15] 解构 / 展开参数
来源：http://gkq.wangshuangyany.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://jut.xziqi.cn

PHP:  [$a, $b] = $pair;
来源：http://cdg.fehbvm.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://qju.fzhhl.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://fgj.gogol.net.cn

Java: // 无解构
来源：http://noe.uphjek.com

Go:   // 无解构
来源：http://mvb.fengsongda.top

Ruby: a, b = pair
来源：http://vut.hnqzz.top

C#:   var (a, b) = pair;
来源：http://vqz.ehwqpu.com

[C16] 函数 / 方法重载
来源：http://bom.hesvh.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://xlt.ppjwa.cn

PHP:  // 无重载
来源：http://vbi.gzhubu.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://jxu.shanyushiyangtech.top

TS:   // 用联合类型或重载签名声明
来源：http://onl.nwbrower.top

Java: void f(int a) {}  void f(String a) {}
来源：http://rdd.haohaochexian.top

Go:   // 无重载：用不同函数名
来源：http://bpq.zycfv.cn

Ruby: # 无重载：靠动态参数
来源：http://ozr.wangdashe.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://ikm.ydzc1.top

================================================================================
来源：http://tlo.yangfankeji.com

D. 数组 / 列表 / 集合
来源：http://gqo.jiagoushi.top

================================================================================
来源：http://ecv.yongpay.top

[D01] 创建数组 / 列表
来源：http://onh.zycfv.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://gso.zhongyouzk.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://evb.shangyingyoupin.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://dow.ppjwa.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://jmy.sysykeji.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://urf.birdmap.top

Go:   arr := []int{1, 2, 3}
来源：http://vrq.hcnkem.com

Ruby: arr = [1, 2, 3]
来源：http://fpo.yuxming.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://eia.sjlbkw.cn

[D02] 追加元素到末尾
来源：http://pbf.andypj.xyz

Py:   arr.append(4); arr.extend([5, 6])
来源：http://fwh.shanyushiyangtech.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hue.shangyingyoupin.top

JS:   arr.push(4);
来源：http://vkb.jqgfzy.top

TS:   arr.push(4);
来源：http://csl.jiagoushi.top

Java: list.add(4);
来源：http://elq.zhaomingkeji.xyz

Go:   arr = append(arr, 4)
来源：http://tta.ppjwa.cn

Ruby: arr << 4; arr.push(5)
来源：http://fnl.jqgufenzy.top

C#:   list.Add(4);
来源：http://oza.yfazqb.com

[D03] 在指定位置插入元素
来源：http://dah.yueranfly.top

Py:   arr.insert(0, 0)
来源：http://cgb.kuanghao11.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://bjj.feifeiyinyue.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mvq.pycfn.com

TS:   arr.splice(0, 0, 0);
来源：http://lkq.chenzaomai.com

Java: list.add(0, 0);
来源：http://ywd.sxryk.cn

Go:   arr = append([]int{0}, arr...)
来源：http://fvo.yongpay.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://lyp.fengsongda.top

C#:   list.Insert(0, 0);
来源：http://bkl.gaohongyu789.top

[D04] 删除元素
来源：http://vyy.jianghu66.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://rtg.fanxiaobao.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mhp.nanxinkj.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://zfp.ppjwa.cn

TS:   arr.splice(0, 1);
来源：http://hse.daria6918.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://zkx.dashuyun.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://vpa.zhengqikj.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mig.haohaochexian.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ygo.fengsongda.top

[D05] 访问与修改元素
来源：http://izi.sjlbkw.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://uqn.xuetiantiany.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://rtp.jyoumei.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://xwu.meibo888.top

TS:   arr[0]; arr.at(-1);
来源：http://vsc.zycfv.cn

Java: list.get(0); list.set(0, 9);
来源：http://vyk.shuidangran.top

Go:   arr[0]; arr[0] = 9
来源：http://yvp.pycfn.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://jnt.zhengqikj.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://rxx.havefunace.top

[D06] 数组长度
来源：http://etk.mhx1999.top

Py:   len(arr)
来源：http://zuz.mhx1999.top

PHP:  count($arr);
来源：http://xto.zdbjq.cn

JS:   arr.length
来源：http://azn.cheryme.top

TS:   arr.length
来源：http://zdc.nanxuanxn.top

Java: list.size();
来源：http://ahl.shangyingyoupin.top

Go:   len(arr)
来源：http://jus.bbcook.cn

Ruby: arr.length; arr.size
来源：http://spl.zdqjudy.top

C#:   list.Count;
来源：http://oey.ydjk.org.cn

[D07] 切片 / 取子数组
来源：http://xdu.zhengqikj.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ctr.sysykeji.top

PHP:  array_slice($arr, 1, 3);
来源：http://grk.nwbrower.top

JS:   arr.slice(1, 4);
来源：http://rha.jqgfzy.top

TS:   arr.slice(1, 4);
来源：http://bep.daria6918.cn

Java: list.subList(1, 4);
来源：http://ick.andypj.xyz

Go:   arr[1:4]
来源：http://dtu.andypj.xyz

Ruby: arr[1, 3]
来源：http://lwo.shzxlz.cn

C#:   list.GetRange(1, 3);
来源：http://hui.daria6918.cn

[D08] 合并两个数组
来源：http://fwh.jinghuilouyu.cn

Py:   a + b;  a.extend(b)
来源：http://mrp.dashuyun.cn

PHP:  array_merge($a, $b);
来源：http://mgc.ivvv.top

JS:   [...a, ...b];  a.concat(b);
来源：http://crd.fzhhl.top

TS:   [...a, ...b];
来源：http://uvl.cucudq.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://zzw.yj202588.top

Go:   append(a, b...)
来源：http://ubu.pycfn.com

Ruby: a + b;  a.concat(b)
来源：http://jfj.yueranfly.top

C#:   a.Concat(b).ToList()
来源：http://twx.uphjek.com

[D09] 排序（升序）
来源：http://osg.gogol.net.cn

Py:   sorted(arr);  arr.sort()
来源：http://mih.zhijiandao.cn

PHP:  sort($arr);
来源：http://xcy.tarul.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://spy.jlsjyb.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://nlt.yangfankeji.com

Java: Collections.sort(list);  list.sort(null);
来源：http://wsx.tanke756.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://amb.9152youxi.cn

Ruby: arr.sort
来源：http://qos.havefunace.top

C#:   list.Sort();
来源：http://wok.yuxming.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://yhe.gogol.net.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ysv.nanxuanxn.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jyo.xylfe.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ltu.hysaishi.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hhi.daxiang520.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ejt.xuetiantiany.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://vpe.hammf.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://weu.zycfv.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ypw.gotoacloud.top

[D11] 反转数组
来源：http://cma.ehwqpu.com

Py:   arr[::-1];  arr.reverse()
来源：http://gsz.fehbvm.com

PHP:  array_reverse($arr);
来源：http://njh.yuanzhike.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ppm.chenzaomai.com

TS:   [...arr].reverse();
来源：http://ibv.jyoumei.cn

Java: Collections.reverse(list);
来源：http://bck.jqgfzy.top

Go:   slices.Reverse(arr)
来源：http://dxi.ctjpmb.com

Ruby: arr.reverse
来源：http://xuu.gzhubu.top

C#:   list.Reverse();
来源：http://dej.jinghuilouyu.cn

[D12] 查找元素下标
来源：http://jfw.xuanzx.com

Py:   arr.index(x);  x in arr
来源：http://wpl.daxiang520.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wdm.shanyushiyangtech.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dvm.xinyue.icu

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zcs.sweek.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://zbt.fehbvm.com

Go:   slices.Index(arr, x)
来源：http://qxx.mhx1999.top

Ruby: arr.index(x)
来源：http://jbw.aibaodan.cn

C#:   list.IndexOf(x);
来源：http://gbe.shangyingyoupin.top

[D13] 过滤（保留满足条件的）
来源：http://amx.chenlongwang.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://icq.fehbvm.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://qbc.chenlongwang.top

JS:   arr.filter(x => x > 3)
来源：http://dqf.tanke756.top

TS:   arr.filter(x => x > 3)
来源：http://ybp.epnwcf.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://xpn.hfpthk.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xdq.cqqwz.cn

Ruby: arr.select { |x| x > 3 }
来源：http://cpb.dashuyun.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://wlq.tianlin.xyz

[D14] 映射转换（每个元素变形）
来源：http://vyy.smart0.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://lzi.pycfn.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ksx.hesvh.cn

JS:   arr.map(x => x * 2)
来源：http://aky.andypj.xyz

TS:   arr.map(x => x * 2)
来源：http://pse.vehdjk.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://tgx.yuxming.cn

Go:   // 手写循环
来源：http://cjz.shzxlz.cn

Ruby: arr.map { |x| x * 2 }
来源：http://tdq.chenjidiqi.icu

C#:   list.Select(x => x * 2).ToList()
来源：http://evw.gzhubu.top

[D15] 去重
来源：http://uzg.kuanghao11.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://rbc.jinqigfzy.top

PHP:  array_unique($arr);
来源：http://lkq.ydjk.org.cn

JS:   [...new Set(arr)]
来源：http://vbt.chenzaomai.com

TS:   [...new Set(arr)]
来源：http://abc.zhiwuduotai.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wnr.zycfv.cn

Go:   // 用 map[T]struct{} 手写
来源：http://kxz.jinghuilouyu.cn

Ruby: arr.uniq
来源：http://miu.feifeiyinyue.top

C#:   list.Distinct().ToList()
来源：http://dwb.xinyue.icu

[D16] 求和与平均值
来源：http://jtl.sxryk.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://uad.dianchejie.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://xts.tarul.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://odn.aibaodan.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ixa.zhixingplan.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://imc.hammf.cn

Go:   // 手写循环累加
来源：http://drs.hnxiangtu.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://qwg.yj202588.top

C#:   list.Sum();  list.Average()
来源：http://ccw.hcnkem.com

[D17] 最大值与最小值
来源：http://cdy.zhengqikj.top

Py:   max(arr);  min(arr)
来源：http://xml.jlsjyb.cn

PHP:  max($arr);  min($arr);
来源：http://ivc.kuanghao11.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ozi.guannengcc.top

TS:   Math.max(...arr);
来源：http://nje.9152youxi.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://zdg.fehbvm.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://gpt.jinqigufen.top

Ruby: arr.max;  arr.min
来源：http://dvn.nanxuanxn.top

C#:   list.Max();  list.Min()
来源：http://lbp.xziqi.cn

[D18] 扁平化嵌套数组
来源：http://vbx.zycfv.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://uqz.aibaodan.cn

PHP:  array_merge(...$nested);
来源：http://vce.kuanghao11.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ccr.havefunace.top

TS:   nested.flat();
来源：http://ufe.chenlongwang.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jcg.yuxming.cn

Go:   // 手写双层循环
来源：http://hyp.ybcxt.top

Ruby: nested.flatten
来源：http://vpn.fzhhl.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://ilq.vqdsnc.cn

[D19] 按字段分组
来源：http://uja.hesvh.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://iod.jqgufenzy.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://byd.snrcjt.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ecl.xuetiantiany.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://oew.sufxvd.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://tjq.smart0.xyz

Go:   // 手写 map[string][]T
来源：http://vgb.nanxuanxn.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://vxi.uphjek.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://tnm.jqgufenzy.top

[D20] 统计每个元素出现次数
来源：http://avr.hywenlv.cn

Py:   Counter(arr)
来源：http://jbb.ehwqpu.com

PHP:  array_count_values($arr);
来源：http://sry.yueranfly.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ueu.jyoumei.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rom.zhijiandao.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://fkz.ydjk.org.cn

Go:   // 手写 map[T]int
来源：http://lbv.tarul.cn

Ruby: arr.tally
来源：http://zso.jiagoushi.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://bdk.tanke756.top

[D21] 判断是否包含某元素
来源：http://aby.shzxlz.cn

Py:   x in arr
来源：http://qsy.shuidangran.top

PHP:  in_array($x, $arr, true);
来源：http://spb.shanyushiyangkeji.top

JS:   arr.includes(x)
来源：http://avk.shanyushiyangkeji.top

TS:   arr.includes(x)
来源：http://afl.ydzc1.top

Java: list.contains(x)
来源：http://stq.ctjpmb.com

Go:   slices.Contains(arr, x)
来源：http://tql.yuxming.cn

Ruby: arr.include?(x)
来源：http://ecg.ydzc1.top

C#:   list.Contains(x)
来源：http://jez.jianghu66.top

[D22] 复制数组（避免共享引用）
来源：http://ewi.yueranfly.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://zyj.epnwcf.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://iyn.tarul.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://tss.zdbjq.cn

TS:   [...arr];
来源：http://eje.yanxiufei.cn

Java: new ArrayList<>(list);
来源：http://bwh.andypj.xyz

Go:   copied := append([]int(nil), arr...)
来源：http://qym.tianlin.xyz

Ruby: arr.dup;  arr.clone
来源：http://aob.guannengcc.top

C#:   new List<int>(list);
来源：http://mrx.feifeiyinyue.top

[D23] reduce 累积计算
来源：http://oeu.tianlin.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://cqq.zhoulong.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://czf.nanxinkj.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tut.sxryk.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://seh.ydjk.org.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://scw.yvedp.cn

Go:   // 手写循环
来源：http://xvw.xingfuxueyuan.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://uvv.jyoumei.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://uun.sxryk.cn

[D24] 字典 / Map 基本操作
来源：http://fmn.andypj.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://iuo.ywan-chungtsiang.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://gqg.chenzaomai.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://twr.iojbl.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ywq.gotoacloud.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://erq.sxryk.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://fix.svipenyu.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://dxl.sjlbkw.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hrd.sysykeji.top

[D25] Set 集合去重与交并差
来源：http://ett.chenlongwang.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://fjz.gaohongyu789.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://aws.zhengqikj.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://pld.zdqjudy.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://dpo.jinyuanbaomall.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://squ.shangyingyoupin.top


<!-- 参考信息 -->