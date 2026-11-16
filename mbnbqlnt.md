代发 wailian999

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://jrw.aizwys.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://lav.ybcxt.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ijm.haohaochexian.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cmi.yuxming.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://xja.ehwqpu.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://uxb.shangyingyoupin.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://qif.jlsjyb.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://tqb.hnqzz.top

[C10] 变量作用域
来源：http://nke.daria6918.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ddk.xziqi.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://pzj.52xcode.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://nos.yfazqb.com

TS:   同 JS
来源：http://dbx.zhengqikj.top

Java: 方法内为块级作用域
来源：http://olu.yj20258.top

Go:   花括号块级作用域
来源：http://qkt.birdmap.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://qgr.yongpay.top

C#:   块级作用域
来源：http://qea.cqqwz.cn

[C11] 模块导入与导出
来源：http://dcl.hammf.cn

Py:   from module import func
来源：http://hte.jianghu66.top

PHP:  require "file.php";  或 use App\Service;
来源：http://fiz.chenjidiqi.icu

JS:   export default function f() {};  import f from "./m.js";
来源：http://yrn.vqdsnc.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://qim.hnxiangtu.top

Java: import java.util.List;
来源：http://hzs.yonumen.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://elr.hnxiangtu.top

Ruby: require "json"; require_relative "./util"
来源：http://fta.hcnkem.com

C#:   using System.Text;
来源：http://rjk.ydjk.org.cn

[C12] 立即执行函数 IIFE
来源：http://xjd.9152youxi.cn

Py:   (lambda: print("run"))()
来源：http://anc.nanxuanxn.top

PHP:  (function () { echo "run"; })();
来源：http://lcs.shuidangran.top

JS:   (() => { console.log("run"); })();
来源：http://csz.ppjwa.cn

TS:   (() => { console.log("run"); })();
来源：http://syv.yfazqb.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://zjs.tianlin.xyz

Go:   func() { fmt.Println("run") }()
来源：http://kql.shanyushiyangkeji.top

Ruby: -> { puts "run" }.call
来源：http://ixq.zhengqikj.top

C#:   // 无 IIFE：用静态构造函数
来源：http://imu.zycfv.cn

[C13] 类型声明 / 类型注解
来源：http://syg.yueranfly.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://tsu.shangyingyoupin.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://eqo.iojbl.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://poi.zycfv.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://djy.ydzc1.top

Java: int add(int a, int b) { return a + b; }
来源：http://xku.jyoumei.cn

Go:   func add(a, b int) int
来源：http://otp.quarkkingdee.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://gmw.cheryme.top

C#:   int Add(int a, int b) => a + b;
来源：http://vzt.cheryme.top

[C14] 泛型函数
来源：http://aiu.gotoacloud.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zep.xinyue.icu

PHP:  // 无泛型
来源：http://ygz.zdqjudy.top

JS:   // 无泛型
来源：http://qqk.cucudq.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://syk.cheryme.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://lii.hcnkem.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ctf.gogol.net.cn

Ruby: # 无泛型
来源：http://aqf.gotoacloud.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mcu.ctjpmb.com

[C15] 解构 / 展开参数
来源：http://tli.xingfuxueyuan.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ljx.wangdashe.top

PHP:  [$a, $b] = $pair;
来源：http://hsa.kuanghao11.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://vnr.cucudq.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hne.yonumen.top

Java: // 无解构
来源：http://ior.shangyingyoupin.top

Go:   // 无解构
来源：http://uuw.bjfxy.top

Ruby: a, b = pair
来源：http://hos.yj20258888.top

C#:   var (a, b) = pair;
来源：http://ojb.aizwys.cn

[C16] 函数 / 方法重载
来源：http://xku.jqgufenzy.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://egs.yj20258.top

PHP:  // 无重载
来源：http://ytz.wangdashe.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://uza.tarul.cn

TS:   // 用联合类型或重载签名声明
来源：http://nec.cqqwz.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://zlj.ivvv.top

Go:   // 无重载：用不同函数名
来源：http://tvp.jinqigfzy.top

Ruby: # 无重载：靠动态参数
来源：http://cwf.yj202588.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://ajg.snrcjt.cn

================================================================================
来源：http://jsp.wangshuangyany.cn

D. 数组 / 列表 / 集合
来源：http://tkd.zdbjq.cn

================================================================================
来源：http://owc.tanke756.top

[D01] 创建数组 / 列表
来源：http://gcv.zhijiandao.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://gtl.ppjwa.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ycf.sweek.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://jjn.zhaomingkeji.xyz

TS:   const arr: number[] = [1, 2, 3];
来源：http://rtb.havefunace.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://rnh.hysaishi.cn

Go:   arr := []int{1, 2, 3}
来源：http://fgo.xinyue.icu

Ruby: arr = [1, 2, 3]
来源：http://mgd.hnqzz.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://rms.gotoacloud.top

[D02] 追加元素到末尾
来源：http://lpt.yj202588.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://vvn.zhongyouzk.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://pmc.chenzaomai.com

JS:   arr.push(4);
来源：http://gfx.fanxiaobao.xyz

TS:   arr.push(4);
来源：http://fec.dashuyun.cn

Java: list.add(4);
来源：http://tnz.0kj1m.cn

Go:   arr = append(arr, 4)
来源：http://vwr.sysykeji.top

Ruby: arr << 4; arr.push(5)
来源：http://qkq.guannengcc.top

C#:   list.Add(4);
来源：http://gbo.fanxiaobao.xyz

[D03] 在指定位置插入元素
来源：http://tcb.daria6918.cn

Py:   arr.insert(0, 0)
来源：http://toq.xylfe.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://cqx.ppjwa.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://nqv.zycfv.cn

TS:   arr.splice(0, 0, 0);
来源：http://uah.yfazqb.com

Java: list.add(0, 0);
来源：http://pwy.bjfxy.top

Go:   arr = append([]int{0}, arr...)
来源：http://kie.redwolf501.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://xuw.wangdashe.top

C#:   list.Insert(0, 0);
来源：http://vsh.yanxiufei.cn

[D04] 删除元素
来源：http://zib.sjlbkw.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://jzj.fehbvm.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://nbu.yueranfly.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://rqz.zycfv.cn

TS:   arr.splice(0, 1);
来源：http://nbf.mhx1999.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://kjy.0kj1m.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://soa.zhiwuduotai.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ktl.0kj1m.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://yeo.yvedp.cn

[D05] 访问与修改元素
来源：http://mmw.pengpengdd.cyou

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://nuk.gzhubu.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://cdk.zdqjudy.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://rcy.wangshuangyany.cn

TS:   arr[0]; arr.at(-1);
来源：http://xpn.shuidangran.top

Java: list.get(0); list.set(0, 9);
来源：http://toq.xuanzx.com

Go:   arr[0]; arr[0] = 9
来源：http://wph.ydzc1.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://irt.havefunace.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://gwc.yj20258.top

[D06] 数组长度
来源：http://ley.dianchejie.cn

Py:   len(arr)
来源：http://hsw.hnqzz.top

PHP:  count($arr);
来源：http://kds.hfpthk.cn

JS:   arr.length
来源：http://juc.sweek.top

TS:   arr.length
来源：http://wry.fengsongda.top

Java: list.size();
来源：http://nly.yfazqb.com

Go:   len(arr)
来源：http://lgv.xingfuxueyuan.xyz

Ruby: arr.length; arr.size
来源：http://rsh.shangyingyoupin.top

C#:   list.Count;
来源：http://fog.shzxlz.cn

[D07] 切片 / 取子数组
来源：http://uba.bjfxy.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://coy.cdnleiting.top

PHP:  array_slice($arr, 1, 3);
来源：http://wcj.sjlbkw.cn

JS:   arr.slice(1, 4);
来源：http://wth.yangfankeji.com

TS:   arr.slice(1, 4);
来源：http://qet.sjlbkw.cn

Java: list.subList(1, 4);
来源：http://gnf.xziqi.cn

Go:   arr[1:4]
来源：http://deq.jqgfzy.top

Ruby: arr[1, 3]
来源：http://pex.52xcode.cn

C#:   list.GetRange(1, 3);
来源：http://mja.hongshengwenyu.top

[D08] 合并两个数组
来源：http://fis.316326.xyz

Py:   a + b;  a.extend(b)
来源：http://nfy.bbcook.cn

PHP:  array_merge($a, $b);
来源：http://mvl.zycfv.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ssh.nanxuanxn.top

TS:   [...a, ...b];
来源：http://lzf.zhoulong.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ydx.hesvh.cn

Go:   append(a, b...)
来源：http://nza.xinyue.icu

Ruby: a + b;  a.concat(b)
来源：http://jtl.cucudq.cn

C#:   a.Concat(b).ToList()
来源：http://cjs.tianlin.xyz

[D09] 排序（升序）
来源：http://ufe.tanke756.top

Py:   sorted(arr);  arr.sort()
来源：http://vup.316326.xyz

PHP:  sort($arr);
来源：http://erf.nanxinkj.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://cjh.epnwcf.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://maz.ctjpmb.com

Java: Collections.sort(list);  list.sort(null);
来源：http://eya.redwolf501.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://upw.jinyuanbaomall.cn

Ruby: arr.sort
来源：http://uzm.aizwys.cn

C#:   list.Sort();
来源：http://ntn.hesvh.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://vnd.mhx1999.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://rop.chenzaomai.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dor.xziqi.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://sod.kuanghao11.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://kxn.wangshuangyany.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://oxf.dashuyun.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://fxf.jyoumei.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://asb.sjlbkw.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://kjo.svipenyu.cn

[D11] 反转数组
来源：http://hqr.yanxiufei.cn

Py:   arr[::-1];  arr.reverse()
来源：http://zcb.xziqi.cn

PHP:  array_reverse($arr);
来源：http://yen.shanyushiyangtech.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://yzh.sjlbkw.cn

TS:   [...arr].reverse();
来源：http://qiy.vqdsnc.cn

Java: Collections.reverse(list);
来源：http://fga.zhaomingkeji.xyz

Go:   slices.Reverse(arr)
来源：http://bsh.uphjek.com

Ruby: arr.reverse
来源：http://cao.jinghuilouyu.cn

C#:   list.Reverse();
来源：http://bwr.shanyushiyangkeji.top

[D12] 查找元素下标
来源：http://uvj.shuidangran.top

Py:   arr.index(x);  x in arr
来源：http://nnu.hysaishi.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://zyb.hammf.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ibw.fengsongda.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://smv.9152youxi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://bma.fktsv.cn

Go:   slices.Index(arr, x)
来源：http://xpw.bjfxy.top

Ruby: arr.index(x)
来源：http://msi.gogol.net.cn

C#:   list.IndexOf(x);
来源：http://tuv.jiagoushi.top

[D13] 过滤（保留满足条件的）
来源：http://sud.birdmap.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://xss.hywenlv.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://woc.yj20258.top

JS:   arr.filter(x => x > 3)
来源：http://eld.smart0.xyz

TS:   arr.filter(x => x > 3)
来源：http://ipl.fehbvm.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://fjd.chenlongwang.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://eiv.ydjk.org.cn

Ruby: arr.select { |x| x > 3 }
来源：http://tbs.zhijiandao.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://tbf.jinyuanbaomall.cn

[D14] 映射转换（每个元素变形）
来源：http://xvq.ehwqpu.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://vpd.cdnleiting.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vej.0kj1m.cn

JS:   arr.map(x => x * 2)
来源：http://mlp.jianghu66.top

TS:   arr.map(x => x * 2)
来源：http://xqj.ehwqpu.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://cai.aizwys.cn

Go:   // 手写循环
来源：http://snb.yanxiufei.cn

Ruby: arr.map { |x| x * 2 }
来源：http://dmt.hnqzz.top

C#:   list.Select(x => x * 2).ToList()
来源：http://osa.sjlbkw.cn

[D15] 去重
来源：http://maw.xinyue.icu

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://iel.9152youxi.cn

PHP:  array_unique($arr);
来源：http://egm.sxryk.cn

JS:   [...new Set(arr)]
来源：http://jfo.jiagoushi.top

TS:   [...new Set(arr)]
来源：http://zdh.fanxiaobao.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hfj.bbcook.cn

Go:   // 用 map[T]struct{} 手写
来源：http://xzr.fehbvm.com

Ruby: arr.uniq
来源：http://ozq.yfazqb.com

C#:   list.Distinct().ToList()
来源：http://miw.xingfuxueyuan.xyz

[D16] 求和与平均值
来源：http://wnq.jiagoushi.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://egk.yvedp.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://uaw.shuidangran.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wgq.quarkkingdee.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://goc.gaohongyu789.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://rtg.yfazqb.com

Go:   // 手写循环累加
来源：http://yed.gotoacloud.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://bdh.jinghuilouyu.cn

C#:   list.Sum();  list.Average()
来源：http://pog.daria6918.cn

[D17] 最大值与最小值
来源：http://xom.vehdjk.com

Py:   max(arr);  min(arr)
来源：http://zxi.zhengqikj.top

PHP:  max($arr);  min($arr);
来源：http://rzj.jlsjyb.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://soc.jqgfzy.top

TS:   Math.max(...arr);
来源：http://hmw.ppjwa.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ndv.bbcook.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://stn.shzxlz.cn

Ruby: arr.max;  arr.min
来源：http://aar.gotoacloud.top

C#:   list.Max();  list.Min()
来源：http://vpp.c1oappe.top

[D18] 扁平化嵌套数组
来源：http://smh.zhiwuduotai.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hcl.meibo888.top

PHP:  array_merge(...$nested);
来源：http://qvg.gotoacloud.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hpy.shanyushiyangkeji.top

TS:   nested.flat();
来源：http://pgn.yuanzhike.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://lpe.haohaochexian.top

Go:   // 手写双层循环
来源：http://ppj.meibo888.top

Ruby: nested.flatten
来源：http://tor.vqdsnc.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://wfw.xinyue.icu

[D19] 按字段分组
来源：http://erm.hongshengwenyu.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://opx.sysykeji.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://fwg.xylfe.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://kgf.hfpthk.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://wjq.zhixingplan.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://cvp.ivvv.top

Go:   // 手写 map[string][]T
来源：http://cjn.sysykeji.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://kug.hongshengwenyu.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://jlf.aizwys.cn

[D20] 统计每个元素出现次数
来源：http://que.pengpengdd.cyou

Py:   Counter(arr)
来源：http://kwn.hongshengwenyu.top

PHP:  array_count_values($arr);
来源：http://owr.redwolf501.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bua.kuanghao11.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ltv.zhengqikj.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://goi.guowangkeji.top

Go:   // 手写 map[T]int
来源：http://pdv.smart0.xyz

Ruby: arr.tally
来源：http://tnv.jinghuilouyu.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://oto.yueranfly.top

[D21] 判断是否包含某元素
来源：http://wld.sxryk.cn

Py:   x in arr
来源：http://kmm.tian-w.cn

PHP:  in_array($x, $arr, true);
来源：http://xzo.yuxming.cn

JS:   arr.includes(x)
来源：http://zzv.guowangkeji.top

TS:   arr.includes(x)
来源：http://udr.vqdsnc.cn

Java: list.contains(x)
来源：http://nqi.jinyuanbaomall.cn

Go:   slices.Contains(arr, x)
来源：http://kep.gaohongyu789.top

Ruby: arr.include?(x)
来源：http://tay.xingfuxueyuan.xyz

C#:   list.Contains(x)
来源：http://eow.shzxlz.cn

[D22] 复制数组（避免共享引用）
来源：http://vyo.zycfv.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://zbr.gzhubu.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://jbe.yueranfly.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://siv.zhaomingkeji.xyz

TS:   [...arr];
来源：http://jrr.c1oappe.top

Java: new ArrayList<>(list);
来源：http://cyv.jlsjyb.cn

Go:   copied := append([]int(nil), arr...)
来源：http://uqd.snrcjt.cn

Ruby: arr.dup;  arr.clone
来源：http://amt.0kj1m.cn

C#:   new List<int>(list);
来源：http://vio.ydzc1.top

[D23] reduce 累积计算
来源：http://szs.cqqwz.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://jzj.shanyushiyangkeji.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ufd.mhx1999.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jxb.yanxiufei.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://doy.uphjek.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://udl.jianghu66.top

Go:   // 手写循环
来源：http://yai.yvedp.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://rpx.nanxuanxn.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://agd.jinqigfzy.top

[D24] 字典 / Map 基本操作
来源：http://htm.fehbvm.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://jzb.52xcode.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://len.gogol.net.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mon.redwolf501.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://jbm.ctjpmb.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ccy.chenzaomai.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://oqe.xziqi.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://qpm.uphjek.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://jxh.zhiwuduotai.top

[D25] Set 集合去重与交并差
来源：http://pmi.hnqzz.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://xpt.chenzaomai.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://auj.andypj.xyz

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://cjd.guowangkeji.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://slm.hnxiangtu.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://qnj.sxryk.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wyg.quarkkingdee.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://goi.snrcjt.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qec.daria6918.cn

[D26] 数组转字符串
来源：http://lnd.smart0.xyz


<!-- 参考信息 -->