代发 wailian999

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ygx.yanxiufei.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://qoe.hammf.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mgk.xziqi.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tva.yuanzhike.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://jft.shzxlz.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://nsp.yangfankeji.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://som.zdqjudy.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://unq.chenlongwang.top

[C10] 变量作用域
来源：http://isw.kuanghao11.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://out.chenjidiqi.icu

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mbt.bjfxy.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://rfg.snrcjt.cn

TS:   同 JS
来源：http://tsn.wangshuangyany.cn

Java: 方法内为块级作用域
来源：http://fto.wangshuangyany.cn

Go:   花括号块级作用域
来源：http://kpq.uphjek.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://bko.cashguo.top

C#:   块级作用域
来源：http://ndj.zdqjudy.top

[C11] 模块导入与导出
来源：http://qhi.c1oappe.top

Py:   from module import func
来源：http://gav.xinyue.icu

PHP:  require "file.php";  或 use App\Service;
来源：http://ocu.jqgfzy.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://yjv.hnqzz.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://sit.yanxiufei.cn

Java: import java.util.List;
来源：http://kag.dianchejie.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://nit.yuxming.cn

Ruby: require "json"; require_relative "./util"
来源：http://fhk.316326.xyz

C#:   using System.Text;
来源：http://evp.aibaodan.cn

[C12] 立即执行函数 IIFE
来源：http://ikz.aibaodan.cn

Py:   (lambda: print("run"))()
来源：http://nzu.gzhubu.top

PHP:  (function () { echo "run"; })();
来源：http://mjq.zhixingplan.top

JS:   (() => { console.log("run"); })();
来源：http://xck.feifeiyinyue.top

TS:   (() => { console.log("run"); })();
来源：http://zcw.guowangkeji.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ddo.nanxinkj.top

Go:   func() { fmt.Println("run") }()
来源：http://ylx.yj20258888.top

Ruby: -> { puts "run" }.call
来源：http://att.jyoumei.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://wqh.wangdashe.top

[C13] 类型声明 / 类型注解
来源：http://csv.ywan-chungtsiang.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://vno.tarul.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://znq.nwbrower.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://pqi.daxiang520.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qjj.zhongyouzk.top

Java: int add(int a, int b) { return a + b; }
来源：http://bpd.fktsv.cn

Go:   func add(a, b int) int
来源：http://ghc.yuxming.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://aib.guowangkeji.top

C#:   int Add(int a, int b) => a + b;
来源：http://zci.ywan-chungtsiang.top

[C14] 泛型函数
来源：http://pyq.zhijiandao.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://llq.quarkkingdee.top

PHP:  // 无泛型
来源：http://qjp.cheryme.top

JS:   // 无泛型
来源：http://fjo.jqgufenzy.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ibo.hesvh.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://uor.pycfn.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://sja.kuanghao11.cn

Ruby: # 无泛型
来源：http://ivw.bbcook.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://cja.redwolf501.top

[C15] 解构 / 展开参数
来源：http://osk.zdbjq.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://azz.xylfe.cn

PHP:  [$a, $b] = $pair;
来源：http://hag.hfpthk.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://rpc.aibaodan.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://beg.vehdjk.com

Java: // 无解构
来源：http://dfs.feifeiyinyue.top

Go:   // 无解构
来源：http://pnz.ehwqpu.com

Ruby: a, b = pair
来源：http://hof.sysykeji.top

C#:   var (a, b) = pair;
来源：http://lsy.fehbvm.com

[C16] 函数 / 方法重载
来源：http://bdn.zhengqikj.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://lgs.hysaishi.cn

PHP:  // 无重载
来源：http://xgg.pycfn.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://yec.yvedp.cn

TS:   // 用联合类型或重载签名声明
来源：http://kii.dianchejie.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://lxw.jianghu66.top

Go:   // 无重载：用不同函数名
来源：http://ihs.jinqigufen.top

Ruby: # 无重载：靠动态参数
来源：http://kbc.feifeiyinyue.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://dts.snrcjt.cn

================================================================================
来源：http://ycw.feifeiyinyue.top

D. 数组 / 列表 / 集合
来源：http://dub.zhoulong.xyz

================================================================================
来源：http://pbd.svipenyu.cn

[D01] 创建数组 / 列表
来源：http://ypi.havefunace.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://lgl.wangdashe.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://fom.zdqjudy.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://yys.mhx1999.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://tcu.mhx1999.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://dyd.gaohongyu789.top

Go:   arr := []int{1, 2, 3}
来源：http://dzi.tianlin.xyz

Ruby: arr = [1, 2, 3]
来源：http://ceh.fengsongda.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://jzb.ivvv.top

[D02] 追加元素到末尾
来源：http://akz.wangdashe.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://avs.zhongyouzk.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mxa.c1oappe.top

JS:   arr.push(4);
来源：http://rao.yuxming.cn

TS:   arr.push(4);
来源：http://xif.bbcook.cn

Java: list.add(4);
来源：http://amm.zycfv.cn

Go:   arr = append(arr, 4)
来源：http://oyo.xuetiantiany.cn

Ruby: arr << 4; arr.push(5)
来源：http://qgj.chenlongwang.top

C#:   list.Add(4);
来源：http://kuq.smart0.xyz

[D03] 在指定位置插入元素
来源：http://tzo.yonumen.top

Py:   arr.insert(0, 0)
来源：http://aml.xziqi.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://oiq.c1oappe.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://auw.yonumen.top

TS:   arr.splice(0, 0, 0);
来源：http://isa.xinyue.icu

Java: list.add(0, 0);
来源：http://wvt.feifeiyinyue.top

Go:   arr = append([]int{0}, arr...)
来源：http://aoh.jinqigfzy.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://cht.jyoumei.cn

C#:   list.Insert(0, 0);
来源：http://awn.yueranfly.top

[D04] 删除元素
来源：http://ooc.guannengcc.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ixj.cucudq.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://gxl.hnqzz.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://nsr.dashuyun.cn

TS:   arr.splice(0, 1);
来源：http://fpg.fengsongda.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ajg.sxryk.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://qkm.hysaishi.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://glo.jinqigfzy.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://yie.shanyushiyangtech.top

[D05] 访问与修改元素
来源：http://mko.ybcxt.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://gxx.sjlbkw.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://lef.ydzc1.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://jtr.jlsjyb.cn

TS:   arr[0]; arr.at(-1);
来源：http://ote.aibaodan.cn

Java: list.get(0); list.set(0, 9);
来源：http://hjx.hnqzz.top

Go:   arr[0]; arr[0] = 9
来源：http://rwh.zhijiandao.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://agp.svipenyu.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://psz.yvedp.cn

[D06] 数组长度
来源：http://jqf.fzhhl.top

Py:   len(arr)
来源：http://uhr.jqgfzy.top

PHP:  count($arr);
来源：http://ose.jinghuilouyu.cn

JS:   arr.length
来源：http://eer.aizwys.cn

TS:   arr.length
来源：http://hsn.epnwcf.com

Java: list.size();
来源：http://jib.cheryme.top

Go:   len(arr)
来源：http://nis.yongpay.top

Ruby: arr.length; arr.size
来源：http://fav.ydzc1.top

C#:   list.Count;
来源：http://qlw.yj202588.top

[D07] 切片 / 取子数组
来源：http://wis.zhoulong.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://kgj.yongpay.top

PHP:  array_slice($arr, 1, 3);
来源：http://mec.jiagoushi.top

JS:   arr.slice(1, 4);
来源：http://lhr.sxryk.cn

TS:   arr.slice(1, 4);
来源：http://foo.jqgfzy.top

Java: list.subList(1, 4);
来源：http://cth.fanxiaobao.xyz

Go:   arr[1:4]
来源：http://npc.jyoumei.cn

Ruby: arr[1, 3]
来源：http://nnv.jyoumei.cn

C#:   list.GetRange(1, 3);
来源：http://vsc.zhixingplan.top

[D08] 合并两个数组
来源：http://wtn.tanke756.top

Py:   a + b;  a.extend(b)
来源：http://jgj.cqqwz.cn

PHP:  array_merge($a, $b);
来源：http://yqu.ehwqpu.com

JS:   [...a, ...b];  a.concat(b);
来源：http://fcf.bjfxy.top

TS:   [...a, ...b];
来源：http://ibq.chenjidiqi.icu

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://vru.feifeiyinyue.top

Go:   append(a, b...)
来源：http://zwl.316326.xyz

Ruby: a + b;  a.concat(b)
来源：http://xoy.andypj.xyz

C#:   a.Concat(b).ToList()
来源：http://wrg.shuidangran.top

[D09] 排序（升序）
来源：http://hfj.jyoumei.cn

Py:   sorted(arr);  arr.sort()
来源：http://kcd.cashguo.top

PHP:  sort($arr);
来源：http://dlp.birdmap.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://zof.yuxming.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://vis.vqdsnc.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://pvh.nanxuanxn.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://bye.iojbl.cn

Ruby: arr.sort
来源：http://rgm.vqdsnc.cn

C#:   list.Sort();
来源：http://sxt.shzxlz.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://cov.shanyushiyangkeji.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ean.daria6918.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bxj.aizwys.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://dfi.316326.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://lbm.cqqwz.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hyx.yvedp.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://fwj.mhx1999.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://tya.jqgufenzy.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://uou.yuxming.cn

[D11] 反转数组
来源：http://dsz.jlsjyb.cn

Py:   arr[::-1];  arr.reverse()
来源：http://tln.aibaodan.cn

PHP:  array_reverse($arr);
来源：http://jho.c1oappe.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://egc.svipenyu.cn

TS:   [...arr].reverse();
来源：http://zyu.yj20258888.top

Java: Collections.reverse(list);
来源：http://hwp.sweek.top

Go:   slices.Reverse(arr)
来源：http://phl.jiagoushi.top

Ruby: arr.reverse
来源：http://yyg.hfpthk.cn

C#:   list.Reverse();
来源：http://wag.redwolf501.top

[D12] 查找元素下标
来源：http://wgo.yanxiufei.cn

Py:   arr.index(x);  x in arr
来源：http://tng.sjlbkw.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://sjv.hnqzz.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qkh.gotoacloud.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jmt.sweek.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://prd.shanyushiyangkeji.top

Go:   slices.Index(arr, x)
来源：http://vmv.jqgufenzy.top

Ruby: arr.index(x)
来源：http://cgc.daria6918.cn

C#:   list.IndexOf(x);
来源：http://bzp.aizwys.cn

[D13] 过滤（保留满足条件的）
来源：http://bdl.gzhubu.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wfc.snrcjt.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://rbz.nanxinkj.top

JS:   arr.filter(x => x > 3)
来源：http://sam.hnxiangtu.top

TS:   arr.filter(x => x > 3)
来源：http://xft.zhijiandao.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://edw.gaohongyu789.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ghm.zhijiandao.cn

Ruby: arr.select { |x| x > 3 }
来源：http://tig.tarul.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://fnm.tarul.cn

[D14] 映射转换（每个元素变形）
来源：http://jpo.redwolf501.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://zid.ydjk.org.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mdd.xziqi.cn

JS:   arr.map(x => x * 2)
来源：http://hun.andypj.xyz

TS:   arr.map(x => x * 2)
来源：http://oux.jqgfzy.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://qmu.shanyushiyangkeji.top

Go:   // 手写循环
来源：http://rfa.9152youxi.cn

Ruby: arr.map { |x| x * 2 }
来源：http://zvm.daxiang520.top

C#:   list.Select(x => x * 2).ToList()
来源：http://ngs.hfpthk.cn

[D15] 去重
来源：http://lpf.zhongyouzk.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://pcl.c1oappe.top

PHP:  array_unique($arr);
来源：http://sll.hysaishi.cn

JS:   [...new Set(arr)]
来源：http://lsp.hnxiangtu.top

TS:   [...new Set(arr)]
来源：http://eod.wangshuangyany.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://auv.pengpengdd.cyou

Go:   // 用 map[T]struct{} 手写
来源：http://nxm.svipenyu.cn

Ruby: arr.uniq
来源：http://jjg.tarul.cn

C#:   list.Distinct().ToList()
来源：http://mbv.zhaomingkeji.xyz

[D16] 求和与平均值
来源：http://nle.jinghuilouyu.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ydg.yj20258888.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://izx.jlsjyb.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://lnz.zhoulong.xyz

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://bjq.aizwys.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wia.yj202588.top

Go:   // 手写循环累加
来源：http://zhi.epnwcf.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://rop.cashguo.top

C#:   list.Sum();  list.Average()
来源：http://erh.tianlin.xyz

[D17] 最大值与最小值
来源：http://wev.yj20258888.top

Py:   max(arr);  min(arr)
来源：http://dgo.hcnkem.com

PHP:  max($arr);  min($arr);
来源：http://pbx.zdqjudy.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mtb.yongpay.top

TS:   Math.max(...arr);
来源：http://vga.smart0.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://oxw.vqdsnc.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://vmn.nwbrower.top

Ruby: arr.max;  arr.min
来源：http://pjz.chenlongwang.top

C#:   list.Max();  list.Min()
来源：http://qsa.nanxinkj.top

[D18] 扁平化嵌套数组
来源：http://coz.zhixingplan.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://uiu.cashguo.top

PHP:  array_merge(...$nested);
来源：http://ncu.zhoulong.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://njn.cashguo.top

TS:   nested.flat();
来源：http://ywf.nanxinkj.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://tpw.zdbjq.cn

Go:   // 手写双层循环
来源：http://utm.svipenyu.cn

Ruby: nested.flatten
来源：http://lmg.yj20258.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://fph.gzhubu.top

[D19] 按字段分组
来源：http://qkt.feifeiyinyue.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://yut.daria6918.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://abs.sweek.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qeg.bbcook.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://sxz.quarkkingdee.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://pyu.haohaochexian.top

Go:   // 手写 map[string][]T
来源：http://vnc.bbcook.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://dwc.cqqwz.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blz.pengpengdd.cyou

[D20] 统计每个元素出现次数
来源：http://wwq.vqdsnc.cn

Py:   Counter(arr)
来源：http://uoc.xuetiantiany.cn

PHP:  array_count_values($arr);
来源：http://xtl.jinqigufen.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bui.aibaodan.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wrz.ydzc1.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://nck.tanke756.top

Go:   // 手写 map[T]int
来源：http://gpb.jqgufenzy.top

Ruby: arr.tally
来源：http://zhd.zdqjudy.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://lox.jinqigfzy.top

[D21] 判断是否包含某元素
来源：http://qwj.yangfankeji.com

Py:   x in arr
来源：http://zjl.shangyingyoupin.top

PHP:  in_array($x, $arr, true);
来源：http://jht.ydjk.org.cn

JS:   arr.includes(x)
来源：http://azi.jinghuilouyu.cn

TS:   arr.includes(x)
来源：http://rui.hammf.cn

Java: list.contains(x)
来源：http://pty.chenzaomai.com

Go:   slices.Contains(arr, x)
来源：http://deb.iojbl.cn

Ruby: arr.include?(x)
来源：http://pma.ppjwa.cn

C#:   list.Contains(x)
来源：http://wtk.iojbl.cn

[D22] 复制数组（避免共享引用）
来源：http://rki.birdmap.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ral.fehbvm.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://sfm.chenzaomai.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ieb.nwbrower.top

TS:   [...arr];
来源：http://bgk.ydjk.org.cn

Java: new ArrayList<>(list);
来源：http://wcw.yfazqb.com

Go:   copied := append([]int(nil), arr...)
来源：http://alz.yanxiufei.cn

Ruby: arr.dup;  arr.clone
来源：http://vws.bjfxy.top

C#:   new List<int>(list);
来源：http://jly.jinqigufen.top

[D23] reduce 累积计算
来源：http://bsz.shangyingyoupin.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://elu.wangshuangyany.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ulx.shangyingyoupin.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mfv.tanke756.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ysu.birdmap.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://iba.cucudq.cn

Go:   // 手写循环
来源：http://ape.sxryk.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://twq.gogol.net.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://pmd.ehwqpu.com

[D24] 字典 / Map 基本操作
来源：http://cqv.aizwys.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://pmm.yangfankeji.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hyz.zhaomingkeji.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://fsi.ppjwa.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://xwr.cashguo.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://pet.xuanzx.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://fsd.iojbl.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://spq.ppjwa.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://imk.jinqigufen.top

[D25] Set 集合去重与交并差
来源：http://fec.tianlin.xyz

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://kge.ybcxt.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://fyd.hesvh.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://fcr.tianlin.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://eqf.316326.xyz

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://zjs.feifeiyinyue.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://cae.xinyue.icu

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xbi.xuanzx.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://jmd.cqqwz.cn

[D26] 数组转字符串
来源：http://imb.vqdsnc.cn


<!-- 参考信息 -->