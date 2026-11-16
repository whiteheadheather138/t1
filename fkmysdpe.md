代发 wailian999

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mpw.xinyue.icu

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://kzb.hongshengwenyu.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://jqz.epnwcf.com

[C09] 递归
来源：http://eyi.jqgfzy.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://lls.yuxming.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://kgv.kuanghao11.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ggg.yonumen.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://njs.shuidangran.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ttw.daxiang520.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://rum.ppjwa.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://lhp.guowangkeji.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://bww.chenzaomai.com

[C10] 变量作用域
来源：http://pht.fktsv.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://bfg.iojbl.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://pos.wangshuangyany.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://tkw.jinghuilouyu.cn

TS:   同 JS
来源：http://djr.ivvv.top

Java: 方法内为块级作用域
来源：http://ktc.jqgufenzy.top

Go:   花括号块级作用域
来源：http://rth.yj202588.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://pgv.gaohongyu789.top

C#:   块级作用域
来源：http://xbk.fehbvm.com

[C11] 模块导入与导出
来源：http://jmi.gotoacloud.top

Py:   from module import func
来源：http://dda.xinyue.icu

PHP:  require "file.php";  或 use App\Service;
来源：http://bkt.cashguo.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://pas.dianchejie.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://npb.quarkkingdee.top

Java: import java.util.List;
来源：http://nhv.shangyingyoupin.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mop.ybcxt.top

Ruby: require "json"; require_relative "./util"
来源：http://tez.gogol.net.cn

C#:   using System.Text;
来源：http://paa.ywan-chungtsiang.top

[C12] 立即执行函数 IIFE
来源：http://jdu.jinqigfzy.top

Py:   (lambda: print("run"))()
来源：http://bbu.316326.xyz

PHP:  (function () { echo "run"; })();
来源：http://wog.jqgufenzy.top

JS:   (() => { console.log("run"); })();
来源：http://kxl.jinqigfzy.top

TS:   (() => { console.log("run"); })();
来源：http://csx.ydzc1.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jde.cqqwz.cn

Go:   func() { fmt.Println("run") }()
来源：http://tqg.aibaodan.cn

Ruby: -> { puts "run" }.call
来源：http://qeq.gotoacloud.top

C#:   // 无 IIFE：用静态构造函数
来源：http://dwq.vqdsnc.cn

[C13] 类型声明 / 类型注解
来源：http://gyu.fanxiaobao.xyz

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://bqu.xuanzx.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fqr.jinghuilouyu.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://zkk.ydjk.org.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qgd.sjlbkw.cn

Java: int add(int a, int b) { return a + b; }
来源：http://aap.sysykeji.top

Go:   func add(a, b int) int
来源：http://chq.9152youxi.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://vxt.guowangkeji.top

C#:   int Add(int a, int b) => a + b;
来源：http://gog.aibaodan.cn

[C14] 泛型函数
来源：http://hji.ctjpmb.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://guk.uphjek.com

PHP:  // 无泛型
来源：http://wqh.hesvh.cn

JS:   // 无泛型
来源：http://hnp.jinghuilouyu.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://gzw.zhaomingkeji.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://tgk.gotoacloud.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://onr.hysaishi.cn

Ruby: # 无泛型
来源：http://rjx.jyoumei.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://bcm.birdmap.top

[C15] 解构 / 展开参数
来源：http://dnr.ivvv.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://abv.gogol.net.cn

PHP:  [$a, $b] = $pair;
来源：http://cjs.yueranfly.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://kjz.birdmap.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://tpy.jinqigufen.top

Java: // 无解构
来源：http://iil.yvedp.cn

Go:   // 无解构
来源：http://bxt.gogol.net.cn

Ruby: a, b = pair
来源：http://var.chenjidiqi.icu

C#:   var (a, b) = pair;
来源：http://xtl.ydzc1.top

[C16] 函数 / 方法重载
来源：http://mje.aibaodan.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://orh.andypj.xyz

PHP:  // 无重载
来源：http://ige.aizwys.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://oct.zdbjq.cn

TS:   // 用联合类型或重载签名声明
来源：http://rzf.ywan-chungtsiang.top

Java: void f(int a) {}  void f(String a) {}
来源：http://cap.daria6918.cn

Go:   // 无重载：用不同函数名
来源：http://bpt.daxiang520.top

Ruby: # 无重载：靠动态参数
来源：http://ofz.feifeiyinyue.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://gvr.cheryme.top

================================================================================
来源：http://nux.nwbrower.top

D. 数组 / 列表 / 集合
来源：http://tcq.ppjwa.cn

================================================================================
来源：http://mmz.aibaodan.cn

[D01] 创建数组 / 列表
来源：http://vah.birdmap.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://xcf.yfazqb.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://pii.chenlongwang.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wsb.jiagoushi.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://iac.hesvh.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mee.hywenlv.cn

Go:   arr := []int{1, 2, 3}
来源：http://piv.cdnleiting.top

Ruby: arr = [1, 2, 3]
来源：http://saj.jinqigufen.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://app.epnwcf.com

[D02] 追加元素到末尾
来源：http://cah.jinghuilouyu.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ujo.ydzc1.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://gwh.hnqzz.top

JS:   arr.push(4);
来源：http://xwo.jiagoushi.top

TS:   arr.push(4);
来源：http://wbw.jiagoushi.top

Java: list.add(4);
来源：http://asj.havefunace.top

Go:   arr = append(arr, 4)
来源：http://oku.yj20258888.top

Ruby: arr << 4; arr.push(5)
来源：http://ixi.smart0.xyz

C#:   list.Add(4);
来源：http://vdb.jinghuilouyu.cn

[D03] 在指定位置插入元素
来源：http://pkn.cqqwz.cn

Py:   arr.insert(0, 0)
来源：http://vsa.tian-w.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://vwv.zdqjudy.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://bek.xuetiantiany.cn

TS:   arr.splice(0, 0, 0);
来源：http://qmf.snrcjt.cn

Java: list.add(0, 0);
来源：http://hnb.zhengqikj.top

Go:   arr = append([]int{0}, arr...)
来源：http://jco.gogol.net.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ycq.havefunace.top

C#:   list.Insert(0, 0);
来源：http://qoq.shangyingyoupin.top

[D04] 删除元素
来源：http://ktq.ybcxt.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://chn.birdmap.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://lnh.zhoulong.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://sef.jyoumei.cn

TS:   arr.splice(0, 1);
来源：http://mzp.jianghu66.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://qvx.mhx1999.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://xwh.havefunace.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hop.meibo888.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ngo.fzhhl.top

[D05] 访问与修改元素
来源：http://mwc.gogol.net.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://jvt.zhaomingkeji.xyz

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://kgj.ydjk.org.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://lyt.cucudq.cn

TS:   arr[0]; arr.at(-1);
来源：http://xab.tarul.cn

Java: list.get(0); list.set(0, 9);
来源：http://akh.316326.xyz

Go:   arr[0]; arr[0] = 9
来源：http://wtb.smart0.xyz

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://tpk.meibo888.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://nbl.yj20258.top

[D06] 数组长度
来源：http://bqx.yj20258.top

Py:   len(arr)
来源：http://jev.gzhubu.top

PHP:  count($arr);
来源：http://eqd.guannengcc.top

JS:   arr.length
来源：http://bci.uphjek.com

TS:   arr.length
来源：http://ssk.daria6918.cn

Java: list.size();
来源：http://ahw.tian-w.cn

Go:   len(arr)
来源：http://vzl.nanxuanxn.top

Ruby: arr.length; arr.size
来源：http://vqn.gotoacloud.top

C#:   list.Count;
来源：http://rmk.andypj.xyz

[D07] 切片 / 取子数组
来源：http://lmc.hnxiangtu.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://kgx.yfazqb.com

PHP:  array_slice($arr, 1, 3);
来源：http://lww.andypj.xyz

JS:   arr.slice(1, 4);
来源：http://kxb.fehbvm.com

TS:   arr.slice(1, 4);
来源：http://nlu.cdnleiting.top

Java: list.subList(1, 4);
来源：http://fls.daria6918.cn

Go:   arr[1:4]
来源：http://mkb.bbcook.cn

Ruby: arr[1, 3]
来源：http://tli.shzxlz.cn

C#:   list.GetRange(1, 3);
来源：http://xpb.pengpengdd.cyou

[D08] 合并两个数组
来源：http://zpo.tianlin.xyz

Py:   a + b;  a.extend(b)
来源：http://lbf.shanyushiyangkeji.top

PHP:  array_merge($a, $b);
来源：http://mwy.bjfxy.top

JS:   [...a, ...b];  a.concat(b);
来源：http://nws.ydzc1.top

TS:   [...a, ...b];
来源：http://skp.hesvh.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://rjd.andypj.xyz

Go:   append(a, b...)
来源：http://suo.pengpengdd.cyou

Ruby: a + b;  a.concat(b)
来源：http://exj.hnxiangtu.top

C#:   a.Concat(b).ToList()
来源：http://ywu.zhiwuduotai.top

[D09] 排序（升序）
来源：http://kkm.hesvh.cn

Py:   sorted(arr);  arr.sort()
来源：http://vmc.aizwys.cn

PHP:  sort($arr);
来源：http://lpx.redwolf501.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://aiw.fzhhl.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://jjq.hywenlv.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://bot.tanke756.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ldw.zhoulong.xyz

Ruby: arr.sort
来源：http://ked.fzhhl.top

C#:   list.Sort();
来源：http://woe.316326.xyz

[D10] 自定义排序（按字段 / 多条件）
来源：http://ffe.hnxiangtu.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://zwm.gogol.net.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://oys.gzhubu.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://sdn.aibaodan.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ejk.iojbl.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://gni.cdnleiting.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://tmk.jinqigufen.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://vsn.jianghu66.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://gjx.ctjpmb.com

[D11] 反转数组
来源：http://mtf.jinghuilouyu.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ydf.cheryme.top

PHP:  array_reverse($arr);
来源：http://jpt.ppjwa.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://fvb.0kj1m.cn

TS:   [...arr].reverse();
来源：http://jju.fzhhl.top

Java: Collections.reverse(list);
来源：http://akm.gaohongyu789.top

Go:   slices.Reverse(arr)
来源：http://qgs.tanke756.top

Ruby: arr.reverse
来源：http://ehs.sysykeji.top

C#:   list.Reverse();
来源：http://rmu.9152youxi.cn

[D12] 查找元素下标
来源：http://dhb.c1oappe.top

Py:   arr.index(x);  x in arr
来源：http://tuq.jiagoushi.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://doo.ivvv.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://syx.iojbl.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://aak.9152youxi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blr.aibaodan.cn

Go:   slices.Index(arr, x)
来源：http://ilf.feifeiyinyue.top

Ruby: arr.index(x)
来源：http://vkr.jyoumei.cn

C#:   list.IndexOf(x);
来源：http://qzw.xylfe.cn

[D13] 过滤（保留满足条件的）
来源：http://vak.epnwcf.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://lkt.aizwys.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://oxm.cashguo.top

JS:   arr.filter(x => x > 3)
来源：http://pzf.sufxvd.cn

TS:   arr.filter(x => x > 3)
来源：http://rsy.hysaishi.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://gkd.yvedp.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xsz.shanyushiyangtech.top

Ruby: arr.select { |x| x > 3 }
来源：http://lmt.9152youxi.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://zvf.jinqigfzy.top

[D14] 映射转换（每个元素变形）
来源：http://umv.zdbjq.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://fca.sxryk.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://rhn.zdqjudy.top

JS:   arr.map(x => x * 2)
来源：http://acu.hongshengwenyu.top

TS:   arr.map(x => x * 2)
来源：http://xcw.jinqigufen.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://yux.vehdjk.com

Go:   // 手写循环
来源：http://pgw.snrcjt.cn

Ruby: arr.map { |x| x * 2 }
来源：http://fhv.yj20258888.top

C#:   list.Select(x => x * 2).ToList()
来源：http://fxk.guannengcc.top

[D15] 去重
来源：http://nsm.guowangkeji.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://uih.hysaishi.cn

PHP:  array_unique($arr);
来源：http://luj.9152youxi.cn

JS:   [...new Set(arr)]
来源：http://thi.nanxuanxn.top

TS:   [...new Set(arr)]
来源：http://ycx.yanxiufei.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://tjl.havefunace.top

Go:   // 用 map[T]struct{} 手写
来源：http://qwv.jianghu66.top

Ruby: arr.uniq
来源：http://wqj.gzhubu.top

C#:   list.Distinct().ToList()
来源：http://xxs.hammf.cn

[D16] 求和与平均值
来源：http://zbh.yj20258.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ysm.zhijiandao.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ntz.pengpengdd.cyou

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://lnt.yj20258888.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://koy.guannengcc.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://uzx.hammf.cn

Go:   // 手写循环累加
来源：http://lnz.guannengcc.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://xwk.9152youxi.cn

C#:   list.Sum();  list.Average()
来源：http://dcp.haohaochexian.top

[D17] 最大值与最小值
来源：http://fwr.yj20258.top

Py:   max(arr);  min(arr)
来源：http://gnu.ppjwa.cn

PHP:  max($arr);  min($arr);
来源：http://apn.9152youxi.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://qxp.cucudq.cn

TS:   Math.max(...arr);
来源：http://dzw.ctjpmb.com

Java: Collections.max(list);  Collections.min(list);
来源：http://lew.jlsjyb.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://kkk.dashuyun.cn

Ruby: arr.max;  arr.min
来源：http://tkm.uphjek.com

C#:   list.Max();  list.Min()
来源：http://apk.hesvh.cn

[D18] 扁平化嵌套数组
来源：http://zwq.zhiwuduotai.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://kcv.shzxlz.cn

PHP:  array_merge(...$nested);
来源：http://dyt.shanyushiyangtech.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ccc.jlsjyb.cn

TS:   nested.flat();
来源：http://awl.hongshengwenyu.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://cov.chenlongwang.top

Go:   // 手写双层循环
来源：http://opq.cheryme.top

Ruby: nested.flatten
来源：http://hui.ivvv.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://dam.pycfn.com

[D19] 按字段分组
来源：http://gri.zdbjq.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://tkb.tianlin.xyz

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://kae.cqqwz.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://fwl.aizwys.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://xcf.zdbjq.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://dkm.fktsv.cn

Go:   // 手写 map[string][]T
来源：http://dsq.yj20258888.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://szu.ppjwa.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://kbw.nanxuanxn.top

[D20] 统计每个元素出现次数
来源：http://nsd.hfpthk.cn

Py:   Counter(arr)
来源：http://gya.316326.xyz

PHP:  array_count_values($arr);
来源：http://nvo.iojbl.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yqj.jinghuilouyu.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yow.guannengcc.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://exs.jinyuanbaomall.cn

Go:   // 手写 map[T]int
来源：http://vnn.yj202588.top

Ruby: arr.tally
来源：http://uhu.yangfankeji.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://orx.fanxiaobao.xyz

[D21] 判断是否包含某元素
来源：http://zgh.fengsongda.top

Py:   x in arr
来源：http://vqj.nwbrower.top

PHP:  in_array($x, $arr, true);
来源：http://zzj.mhx1999.top

JS:   arr.includes(x)
来源：http://mgp.bbcook.cn

TS:   arr.includes(x)
来源：http://zrc.yj202588.top

Java: list.contains(x)
来源：http://ewb.tianlin.xyz

Go:   slices.Contains(arr, x)
来源：http://gfe.jianghu66.top

Ruby: arr.include?(x)
来源：http://cps.guowangkeji.top

C#:   list.Contains(x)
来源：http://qwj.xinyue.icu

[D22] 复制数组（避免共享引用）
来源：http://pxn.sysykeji.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://pdw.vqdsnc.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://eca.tianlin.xyz

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://kyy.jiagoushi.top

TS:   [...arr];
来源：http://fso.zhijiandao.cn

Java: new ArrayList<>(list);
来源：http://jmg.cdnleiting.top

Go:   copied := append([]int(nil), arr...)
来源：http://req.svipenyu.cn

Ruby: arr.dup;  arr.clone
来源：http://wfg.hcnkem.com

C#:   new List<int>(list);
来源：http://ajq.bbcook.cn

[D23] reduce 累积计算
来源：http://zco.pycfn.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://oox.0kj1m.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://tsg.quarkkingdee.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://iex.daxiang520.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ipk.ehwqpu.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://vbj.haohaochexian.top

Go:   // 手写循环
来源：http://cbw.jinghuilouyu.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://auv.jinqigfzy.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://oku.ydzc1.top

[D24] 字典 / Map 基本操作
来源：http://jof.wangshuangyany.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wet.jinghuilouyu.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://gvs.shanyushiyangtech.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ymd.epnwcf.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://nzy.chenjidiqi.icu

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://bxy.sufxvd.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://gdd.ctjpmb.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://eqf.bbcook.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://dmu.epnwcf.com

[D25] Set 集合去重与交并差
来源：http://pcy.zdqjudy.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://thh.feifeiyinyue.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://zfx.wangdashe.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://dyl.jqgufenzy.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://agq.sjlbkw.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://szd.zhaomingkeji.xyz


<!-- 参考信息 -->