代发 wailian999

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://oed.gotoacloud.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ate.jyoumei.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://njn.yj20258.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ozf.yj202588.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://yda.yueranfly.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://oyl.guannengcc.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://pyn.hcnkem.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://uwf.sjlbkw.cn

[C10] 变量作用域
来源：http://msn.cashguo.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wnq.zhongyouzk.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://web.hcnkem.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://svr.zhongyouzk.top

TS:   同 JS
来源：http://wpv.fzhhl.top

Java: 方法内为块级作用域
来源：http://xpa.yongpay.top

Go:   花括号块级作用域
来源：http://wrj.hongshengwenyu.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://toy.shanyushiyangkeji.top

C#:   块级作用域
来源：http://zil.shanyushiyangkeji.top

[C11] 模块导入与导出
来源：http://drh.sxryk.cn

Py:   from module import func
来源：http://nqf.jiagoushi.top

PHP:  require "file.php";  或 use App\Service;
来源：http://swc.yuxming.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://lvd.fktsv.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hbx.nwbrower.top

Java: import java.util.List;
来源：http://rtb.hongshengwenyu.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wne.hnqzz.top

Ruby: require "json"; require_relative "./util"
来源：http://srd.ybcxt.top

C#:   using System.Text;
来源：http://qjx.tianlin.xyz

[C12] 立即执行函数 IIFE
来源：http://epo.zhixingplan.top

Py:   (lambda: print("run"))()
来源：http://yds.dianchejie.cn

PHP:  (function () { echo "run"; })();
来源：http://lkk.yuxming.cn

JS:   (() => { console.log("run"); })();
来源：http://hcf.jinqigfzy.top

TS:   (() => { console.log("run"); })();
来源：http://tod.cdnleiting.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://zki.shuidangran.top

Go:   func() { fmt.Println("run") }()
来源：http://euc.gaohongyu789.top

Ruby: -> { puts "run" }.call
来源：http://pdd.ydjk.org.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://jpx.shanyushiyangkeji.top

[C13] 类型声明 / 类型注解
来源：http://aky.pengpengdd.cyou

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://lco.meibo888.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ddf.cheryme.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://oug.aibaodan.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://utq.zdbjq.cn

Java: int add(int a, int b) { return a + b; }
来源：http://yew.zhaomingkeji.xyz

Go:   func add(a, b int) int
来源：http://uao.yuxming.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://jmp.yueranfly.top

C#:   int Add(int a, int b) => a + b;
来源：http://lay.smart0.xyz

[C14] 泛型函数
来源：http://zqt.zhoulong.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zzy.yuanzhike.top

PHP:  // 无泛型
来源：http://ocd.chenjidiqi.icu

JS:   // 无泛型
来源：http://liq.yangfankeji.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://dnt.dianchejie.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://jsd.jianghu66.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://yrl.shzxlz.cn

Ruby: # 无泛型
来源：http://ipw.xziqi.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://cls.zhixingplan.top

[C15] 解构 / 展开参数
来源：http://uig.sysykeji.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://van.gaohongyu789.top

PHP:  [$a, $b] = $pair;
来源：http://abm.yj20258.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://nnf.ydjk.org.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://uep.wangdashe.top

Java: // 无解构
来源：http://ewk.jianghu66.top

Go:   // 无解构
来源：http://vex.zycfv.cn

Ruby: a, b = pair
来源：http://axt.jqgfzy.top

C#:   var (a, b) = pair;
来源：http://hfx.shanyushiyangkeji.top

[C16] 函数 / 方法重载
来源：http://hth.sweek.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://utw.ehwqpu.com

PHP:  // 无重载
来源：http://spy.316326.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://qef.cheryme.top

TS:   // 用联合类型或重载签名声明
来源：http://mqj.bbcook.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://fer.yj20258.top

Go:   // 无重载：用不同函数名
来源：http://xcg.dashuyun.cn

Ruby: # 无重载：靠动态参数
来源：http://hhw.jqgufenzy.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://ten.yonumen.top

================================================================================
来源：http://wyp.zhiwuduotai.top

D. 数组 / 列表 / 集合
来源：http://ret.yangfankeji.com

================================================================================
来源：http://yjh.snrcjt.cn

[D01] 创建数组 / 列表
来源：http://bie.xuanzx.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://nxf.yonumen.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://qwl.ybcxt.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://erg.yueranfly.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://vcg.mhx1999.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://xyy.tianlin.xyz

Go:   arr := []int{1, 2, 3}
来源：http://ngy.hcnkem.com

Ruby: arr = [1, 2, 3]
来源：http://olp.hfpthk.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ecf.redwolf501.top

[D02] 追加元素到末尾
来源：http://hoz.chenzaomai.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://nds.yanxiufei.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://jts.snrcjt.cn

JS:   arr.push(4);
来源：http://oit.cucudq.cn

TS:   arr.push(4);
来源：http://gni.svipenyu.cn

Java: list.add(4);
来源：http://kyi.kuanghao11.cn

Go:   arr = append(arr, 4)
来源：http://vwl.yuxming.cn

Ruby: arr << 4; arr.push(5)
来源：http://gkb.yfazqb.com

C#:   list.Add(4);
来源：http://jpk.zdqjudy.top

[D03] 在指定位置插入元素
来源：http://dxe.uphjek.com

Py:   arr.insert(0, 0)
来源：http://bpr.sweek.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://bpd.uphjek.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://aoq.zhongyouzk.top

TS:   arr.splice(0, 0, 0);
来源：http://axl.jinqigufen.top

Java: list.add(0, 0);
来源：http://uiv.jianghu66.top

Go:   arr = append([]int{0}, arr...)
来源：http://ese.hfpthk.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://nzd.xziqi.cn

C#:   list.Insert(0, 0);
来源：http://xxt.gotoacloud.top

[D04] 删除元素
来源：http://vhp.meibo888.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://qnl.bjfxy.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://njs.dianchejie.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hvk.zhongyouzk.top

TS:   arr.splice(0, 1);
来源：http://fuk.tarul.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://sfw.zhongyouzk.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://peo.andypj.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://yjv.9152youxi.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mlw.guowangkeji.top

[D05] 访问与修改元素
来源：http://cqi.tianlin.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://uuw.meibo888.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wtx.yj202588.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://aau.wangshuangyany.cn

TS:   arr[0]; arr.at(-1);
来源：http://ydt.shuidangran.top

Java: list.get(0); list.set(0, 9);
来源：http://vjc.hywenlv.cn

Go:   arr[0]; arr[0] = 9
来源：http://yoa.zhongyouzk.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://qzt.zycfv.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://lgf.ybcxt.top

[D06] 数组长度
来源：http://poi.epnwcf.com

Py:   len(arr)
来源：http://lvi.shuidangran.top

PHP:  count($arr);
来源：http://bfl.zhixingplan.top

JS:   arr.length
来源：http://qec.hywenlv.cn

TS:   arr.length
来源：http://zxe.chenzaomai.com

Java: list.size();
来源：http://mdi.kuanghao11.cn

Go:   len(arr)
来源：http://tss.chenzaomai.com

Ruby: arr.length; arr.size
来源：http://uwt.shanyushiyangkeji.top

C#:   list.Count;
来源：http://beu.hammf.cn

[D07] 切片 / 取子数组
来源：http://vke.ppjwa.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://yuw.nanxuanxn.top

PHP:  array_slice($arr, 1, 3);
来源：http://pnw.cashguo.top

JS:   arr.slice(1, 4);
来源：http://qlf.jqgufenzy.top

TS:   arr.slice(1, 4);
来源：http://pbj.chenzaomai.com

Java: list.subList(1, 4);
来源：http://pwj.hcnkem.com

Go:   arr[1:4]
来源：http://sea.vehdjk.com

Ruby: arr[1, 3]
来源：http://chs.hfpthk.cn

C#:   list.GetRange(1, 3);
来源：http://tub.yongpay.top

[D08] 合并两个数组
来源：http://coi.uphjek.com

Py:   a + b;  a.extend(b)
来源：http://pdf.guannengcc.top

PHP:  array_merge($a, $b);
来源：http://rwy.jqgufenzy.top

JS:   [...a, ...b];  a.concat(b);
来源：http://ryw.gzhubu.top

TS:   [...a, ...b];
来源：http://hvl.zycfv.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://rhr.vehdjk.com

Go:   append(a, b...)
来源：http://yac.aibaodan.cn

Ruby: a + b;  a.concat(b)
来源：http://xcx.yonumen.top

C#:   a.Concat(b).ToList()
来源：http://yzn.jinghuilouyu.cn

[D09] 排序（升序）
来源：http://zrg.tanke756.top

Py:   sorted(arr);  arr.sort()
来源：http://gxh.guowangkeji.top

PHP:  sort($arr);
来源：http://prp.jiagoushi.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://twi.tian-w.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://aru.bjfxy.top

Java: Collections.sort(list);  list.sort(null);
来源：http://tln.havefunace.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://lbt.zhixingplan.top

Ruby: arr.sort
来源：http://tgm.gogol.net.cn

C#:   list.Sort();
来源：http://ijl.meibo888.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://sgy.epnwcf.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://agt.xziqi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://unr.dianchejie.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://pcs.daria6918.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://rhf.gaohongyu789.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://srl.nanxuanxn.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://run.jianghu66.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://onn.bjfxy.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ggm.xziqi.cn

[D11] 反转数组
来源：http://avn.yuxming.cn

Py:   arr[::-1];  arr.reverse()
来源：http://drq.chenjidiqi.icu

PHP:  array_reverse($arr);
来源：http://rey.jlsjyb.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://pag.yj20258.top

TS:   [...arr].reverse();
来源：http://obq.cashguo.top

Java: Collections.reverse(list);
来源：http://mhf.mhx1999.top

Go:   slices.Reverse(arr)
来源：http://rqm.vehdjk.com

Ruby: arr.reverse
来源：http://rcm.gaohongyu789.top

C#:   list.Reverse();
来源：http://qce.sweek.top

[D12] 查找元素下标
来源：http://kln.jqgfzy.top

Py:   arr.index(x);  x in arr
来源：http://fuu.dashuyun.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://gei.smart0.xyz

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qvl.ywan-chungtsiang.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lan.yuanzhike.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://sdy.zhongyouzk.top

Go:   slices.Index(arr, x)
来源：http://bvm.cheryme.top

Ruby: arr.index(x)
来源：http://ffi.gzhubu.top

C#:   list.IndexOf(x);
来源：http://jrm.nanxinkj.top

[D13] 过滤（保留满足条件的）
来源：http://rus.gogol.net.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://pzh.zdqjudy.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://zbb.yongpay.top

JS:   arr.filter(x => x > 3)
来源：http://jzc.jqgfzy.top

TS:   arr.filter(x => x > 3)
来源：http://sye.hfpthk.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://snp.jqgfzy.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://pze.andypj.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://zdk.jinghuilouyu.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://nal.meibo888.top

[D14] 映射转换（每个元素变形）
来源：http://kxp.shuidangran.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://elv.nanxinkj.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://qji.ehwqpu.com

JS:   arr.map(x => x * 2)
来源：http://tul.nwbrower.top

TS:   arr.map(x => x * 2)
来源：http://kyl.cqqwz.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://rtj.aibaodan.cn

Go:   // 手写循环
来源：http://tpx.yanxiufei.cn

Ruby: arr.map { |x| x * 2 }
来源：http://kyo.zhiwuduotai.top

C#:   list.Select(x => x * 2).ToList()
来源：http://otu.xinyue.icu

[D15] 去重
来源：http://oqs.feifeiyinyue.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://kiz.wangshuangyany.cn

PHP:  array_unique($arr);
来源：http://vcj.jqgfzy.top

JS:   [...new Set(arr)]
来源：http://bho.tianlin.xyz

TS:   [...new Set(arr)]
来源：http://ufm.sufxvd.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://boz.zhengqikj.top

Go:   // 用 map[T]struct{} 手写
来源：http://olq.hcnkem.com

Ruby: arr.uniq
来源：http://noi.yvedp.cn

C#:   list.Distinct().ToList()
来源：http://ury.dianchejie.cn

[D16] 求和与平均值
来源：http://qcb.zdbjq.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://lpk.0kj1m.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://jtj.sysykeji.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://xwq.nwbrower.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hxp.zdqjudy.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://gfg.chenlongwang.top

Go:   // 手写循环累加
来源：http://ppn.smart0.xyz

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mar.yuxming.cn

C#:   list.Sum();  list.Average()
来源：http://mxk.jinqigufen.top

[D17] 最大值与最小值
来源：http://avt.yangfankeji.com

Py:   max(arr);  min(arr)
来源：http://zwb.shanyushiyangtech.top

PHP:  max($arr);  min($arr);
来源：http://dng.tarul.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://fgx.chenzaomai.com

TS:   Math.max(...arr);
来源：http://ihy.9152youxi.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://cio.cheryme.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://iqi.zdqjudy.top

Ruby: arr.max;  arr.min
来源：http://eof.52xcode.cn

C#:   list.Max();  list.Min()
来源：http://res.mhx1999.top

[D18] 扁平化嵌套数组
来源：http://mob.zycfv.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://bvk.hysaishi.cn

PHP:  array_merge(...$nested);
来源：http://adz.zdbjq.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://omt.quarkkingdee.top

TS:   nested.flat();
来源：http://apb.sweek.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://gas.shanyushiyangtech.top

Go:   // 手写双层循环
来源：http://bsx.chenzaomai.com

Ruby: nested.flatten
来源：http://ygx.xuetiantiany.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ldh.jlsjyb.cn

[D19] 按字段分组
来源：http://jhd.yongpay.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://pss.xuanzx.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://knb.zycfv.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://rfx.sysykeji.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://zve.xziqi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://uyd.yj20258888.top

Go:   // 手写 map[string][]T
来源：http://vxw.hammf.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://hsu.jqgufenzy.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://cun.meibo888.top

[D20] 统计每个元素出现次数
来源：http://clk.gaohongyu789.top

Py:   Counter(arr)
来源：http://lms.yvedp.cn

PHP:  array_count_values($arr);
来源：http://yll.nanxuanxn.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vdy.hnxiangtu.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://inl.pycfn.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://dty.guannengcc.top

Go:   // 手写 map[T]int
来源：http://ydb.chenzaomai.com

Ruby: arr.tally
来源：http://wfc.xinyue.icu

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://qaw.fengsongda.top

[D21] 判断是否包含某元素
来源：http://cpg.hfpthk.cn

Py:   x in arr
来源：http://ivw.fengsongda.top

PHP:  in_array($x, $arr, true);
来源：http://vmo.jqgufenzy.top

JS:   arr.includes(x)
来源：http://dzx.zhijiandao.cn

TS:   arr.includes(x)
来源：http://wxu.sxryk.cn

Java: list.contains(x)
来源：http://fbt.hongshengwenyu.top

Go:   slices.Contains(arr, x)
来源：http://keu.mhx1999.top

Ruby: arr.include?(x)
来源：http://ger.0kj1m.cn

C#:   list.Contains(x)
来源：http://yhw.jianghu66.top

[D22] 复制数组（避免共享引用）
来源：http://dve.yueranfly.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://tkg.xuetiantiany.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://xio.sweek.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://uun.xylfe.cn

TS:   [...arr];
来源：http://htv.fzhhl.top

Java: new ArrayList<>(list);
来源：http://oxs.bjfxy.top

Go:   copied := append([]int(nil), arr...)
来源：http://kgh.sjlbkw.cn

Ruby: arr.dup;  arr.clone
来源：http://jey.ppjwa.cn

C#:   new List<int>(list);
来源：http://hdi.fanxiaobao.xyz

[D23] reduce 累积计算
来源：http://qpj.daria6918.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://cyj.jinghuilouyu.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://zgl.hnxiangtu.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ryn.daxiang520.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://teu.c1oappe.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://nqf.jqgfzy.top

Go:   // 手写循环
来源：http://kpn.shuidangran.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://psk.yj202588.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mvv.tarul.cn

[D24] 字典 / Map 基本操作
来源：http://egt.ctjpmb.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://szd.jinyuanbaomall.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://whx.nanxuanxn.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://okm.fanxiaobao.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wgw.zhoulong.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://jft.shuidangran.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://lxj.shzxlz.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mmw.tian-w.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hqx.yanxiufei.cn

[D25] Set 集合去重与交并差
来源：http://awv.ehwqpu.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://nvt.tian-w.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ssw.smart0.xyz

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://moc.ybcxt.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://lol.c1oappe.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://krf.hnxiangtu.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ayp.shuidangran.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://cql.shzxlz.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://fnb.fengsongda.top

[D26] 数组转字符串
来源：http://yyn.yonumen.top


<!-- 参考信息 -->