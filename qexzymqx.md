代发 wailian999

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ssx.gaohongyu789.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mbu.epnwcf.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://zdo.ivvv.top

[C09] 递归
来源：http://hhp.hesvh.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://snr.guannengcc.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wci.jiagoushi.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rjd.cucudq.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qlq.wangshuangyany.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ueh.hywenlv.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://jxv.fehbvm.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hbt.jinqigufen.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://acq.bbcook.cn

[C10] 变量作用域
来源：http://xvj.fengsongda.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://nap.xuetiantiany.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://lqq.jqgfzy.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://zjr.quarkkingdee.top

TS:   同 JS
来源：http://waq.snrcjt.cn

Java: 方法内为块级作用域
来源：http://jfu.jlsjyb.cn

Go:   花括号块级作用域
来源：http://rjl.havefunace.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://tcw.bjfxy.top

C#:   块级作用域
来源：http://bbo.birdmap.top

[C11] 模块导入与导出
来源：http://gbj.tian-w.cn

Py:   from module import func
来源：http://qfh.sjlbkw.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://cqy.shuidangran.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://mgo.cqqwz.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://quf.zdbjq.cn

Java: import java.util.List;
来源：http://tlo.jqgfzy.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://pht.andypj.xyz

Ruby: require "json"; require_relative "./util"
来源：http://ywa.zhengqikj.top

C#:   using System.Text;
来源：http://hnz.shzxlz.cn

[C12] 立即执行函数 IIFE
来源：http://mqy.ehwqpu.com

Py:   (lambda: print("run"))()
来源：http://llh.cdnleiting.top

PHP:  (function () { echo "run"; })();
来源：http://grn.xuetiantiany.cn

JS:   (() => { console.log("run"); })();
来源：http://gxh.sufxvd.cn

TS:   (() => { console.log("run"); })();
来源：http://nba.fengsongda.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://egy.hongshengwenyu.top

Go:   func() { fmt.Println("run") }()
来源：http://als.yangfankeji.com

Ruby: -> { puts "run" }.call
来源：http://mcy.daxiang520.top

C#:   // 无 IIFE：用静态构造函数
来源：http://due.andypj.xyz

[C13] 类型声明 / 类型注解
来源：http://yii.zhengqikj.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://gfr.bbcook.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://aef.zhongyouzk.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://bnr.fanxiaobao.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://laq.pycfn.com

Java: int add(int a, int b) { return a + b; }
来源：http://trg.9152youxi.cn

Go:   func add(a, b int) int
来源：http://gil.jqgfzy.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://tem.wangshuangyany.cn

C#:   int Add(int a, int b) => a + b;
来源：http://tnv.snrcjt.cn

[C14] 泛型函数
来源：http://sbx.yuanzhike.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://cah.yj202588.top

PHP:  // 无泛型
来源：http://ewe.tanke756.top

JS:   // 无泛型
来源：http://dle.hnqzz.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hnu.sysykeji.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://nep.pengpengdd.cyou

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wjl.jinghuilouyu.cn

Ruby: # 无泛型
来源：http://kmh.jqgfzy.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mds.yonumen.top

[C15] 解构 / 展开参数
来源：http://for.bjfxy.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://zhd.yonumen.top

PHP:  [$a, $b] = $pair;
来源：http://lto.chenzaomai.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://erh.cqqwz.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://yow.cucudq.cn

Java: // 无解构
来源：http://mmt.yonumen.top

Go:   // 无解构
来源：http://fbf.yj202588.top

Ruby: a, b = pair
来源：http://sgq.iojbl.cn

C#:   var (a, b) = pair;
来源：http://ybi.snrcjt.cn

[C16] 函数 / 方法重载
来源：http://ldh.nanxuanxn.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://egk.chenzaomai.com

PHP:  // 无重载
来源：http://bjw.ydzc1.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://zdw.shanyushiyangtech.top

TS:   // 用联合类型或重载签名声明
来源：http://tyy.redwolf501.top

Java: void f(int a) {}  void f(String a) {}
来源：http://qxi.cheryme.top

Go:   // 无重载：用不同函数名
来源：http://gzx.aizwys.cn

Ruby: # 无重载：靠动态参数
来源：http://eyf.svipenyu.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://odk.iojbl.cn

================================================================================
来源：http://lbk.dashuyun.cn

D. 数组 / 列表 / 集合
来源：http://gvz.tanke756.top

================================================================================
来源：http://gzx.ywan-chungtsiang.top

[D01] 创建数组 / 列表
来源：http://nax.jinghuilouyu.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://wbm.cdnleiting.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://qyn.zdqjudy.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://jol.yueranfly.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://zwe.gzhubu.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://bsj.yongpay.top

Go:   arr := []int{1, 2, 3}
来源：http://onz.316326.xyz

Ruby: arr = [1, 2, 3]
来源：http://hxo.zhaomingkeji.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://dbz.zhongyouzk.top

[D02] 追加元素到末尾
来源：http://lip.jinqigfzy.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://swd.zdbjq.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://vzs.aibaodan.cn

JS:   arr.push(4);
来源：http://eim.uphjek.com

TS:   arr.push(4);
来源：http://ztn.cdnleiting.top

Java: list.add(4);
来源：http://rrq.zhijiandao.cn

Go:   arr = append(arr, 4)
来源：http://cxw.jinghuilouyu.cn

Ruby: arr << 4; arr.push(5)
来源：http://nlv.0kj1m.cn

C#:   list.Add(4);
来源：http://log.ywan-chungtsiang.top

[D03] 在指定位置插入元素
来源：http://htk.yueranfly.top

Py:   arr.insert(0, 0)
来源：http://jbv.hcnkem.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ddz.cucudq.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://evu.nanxinkj.top

TS:   arr.splice(0, 0, 0);
来源：http://fvx.yangfankeji.com

Java: list.add(0, 0);
来源：http://sdf.sjlbkw.cn

Go:   arr = append([]int{0}, arr...)
来源：http://xqu.bbcook.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://jzq.sxryk.cn

C#:   list.Insert(0, 0);
来源：http://wnu.ydzc1.top

[D04] 删除元素
来源：http://vha.birdmap.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://dok.jlsjyb.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://qfs.zhiwuduotai.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://pko.316326.xyz

TS:   arr.splice(0, 1);
来源：http://rci.uphjek.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://nel.hywenlv.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://xpn.nwbrower.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://xva.shzxlz.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://spw.yuxming.cn

[D05] 访问与修改元素
来源：http://orm.yj20258.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://xmn.gogol.net.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://jux.sysykeji.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://amg.bbcook.cn

TS:   arr[0]; arr.at(-1);
来源：http://obz.shangyingyoupin.top

Java: list.get(0); list.set(0, 9);
来源：http://fue.yfazqb.com

Go:   arr[0]; arr[0] = 9
来源：http://lum.iojbl.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://tlk.jiagoushi.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://qad.haohaochexian.top

[D06] 数组长度
来源：http://kty.tanke756.top

Py:   len(arr)
来源：http://ypo.sufxvd.cn

PHP:  count($arr);
来源：http://xya.kuanghao11.cn

JS:   arr.length
来源：http://khi.9152youxi.cn

TS:   arr.length
来源：http://okn.cashguo.top

Java: list.size();
来源：http://gct.fehbvm.com

Go:   len(arr)
来源：http://tak.sweek.top

Ruby: arr.length; arr.size
来源：http://xsy.jinqigfzy.top

C#:   list.Count;
来源：http://cts.hfpthk.cn

[D07] 切片 / 取子数组
来源：http://yhj.hcnkem.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://fbz.cqqwz.cn

PHP:  array_slice($arr, 1, 3);
来源：http://klj.guannengcc.top

JS:   arr.slice(1, 4);
来源：http://rvr.yuanzhike.top

TS:   arr.slice(1, 4);
来源：http://mpd.ehwqpu.com

Java: list.subList(1, 4);
来源：http://epr.mhx1999.top

Go:   arr[1:4]
来源：http://sgw.zycfv.cn

Ruby: arr[1, 3]
来源：http://pom.yangfankeji.com

C#:   list.GetRange(1, 3);
来源：http://ipn.aibaodan.cn

[D08] 合并两个数组
来源：http://rrb.sjlbkw.cn

Py:   a + b;  a.extend(b)
来源：http://ghi.vqdsnc.cn

PHP:  array_merge($a, $b);
来源：http://ovx.hongshengwenyu.top

JS:   [...a, ...b];  a.concat(b);
来源：http://iro.chenjidiqi.icu

TS:   [...a, ...b];
来源：http://fqd.zhiwuduotai.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://fwf.hywenlv.cn

Go:   append(a, b...)
来源：http://rgz.meibo888.top

Ruby: a + b;  a.concat(b)
来源：http://fhq.tianlin.xyz

C#:   a.Concat(b).ToList()
来源：http://tyr.zhengqikj.top

[D09] 排序（升序）
来源：http://jto.shanyushiyangtech.top

Py:   sorted(arr);  arr.sort()
来源：http://xne.hongshengwenyu.top

PHP:  sort($arr);
来源：http://bxj.zhongyouzk.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ynp.gaohongyu789.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://jwe.gaohongyu789.top

Java: Collections.sort(list);  list.sort(null);
来源：http://eyq.shangyingyoupin.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://tgs.zhixingplan.top

Ruby: arr.sort
来源：http://tpe.shuidangran.top

C#:   list.Sort();
来源：http://stt.hfpthk.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.havefunace.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mej.sysykeji.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://joy.bjfxy.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://eeu.ybcxt.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://tkg.chenlongwang.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://vvp.yvedp.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://zet.vehdjk.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://bak.hfpthk.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://rxn.yj202588.top

[D11] 反转数组
来源：http://sox.jinghuilouyu.cn

Py:   arr[::-1];  arr.reverse()
来源：http://fiy.aibaodan.cn

PHP:  array_reverse($arr);
来源：http://nkn.vehdjk.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://aoh.yuanzhike.top

TS:   [...arr].reverse();
来源：http://pig.ydzc1.top

Java: Collections.reverse(list);
来源：http://kio.chenjidiqi.icu

Go:   slices.Reverse(arr)
来源：http://zxy.hywenlv.cn

Ruby: arr.reverse
来源：http://qkk.haohaochexian.top

C#:   list.Reverse();
来源：http://kpq.wangdashe.top

[D12] 查找元素下标
来源：http://yhu.jlsjyb.cn

Py:   arr.index(x);  x in arr
来源：http://lry.nwbrower.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://jbp.fengsongda.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bxx.c1oappe.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fjk.jianghu66.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://iyz.cheryme.top

Go:   slices.Index(arr, x)
来源：http://chu.havefunace.top

Ruby: arr.index(x)
来源：http://lme.cucudq.cn

C#:   list.IndexOf(x);
来源：http://rdu.zhaomingkeji.xyz

[D13] 过滤（保留满足条件的）
来源：http://cxl.smart0.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://tuq.9152youxi.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://eeo.gzhubu.top

JS:   arr.filter(x => x > 3)
来源：http://ntf.aibaodan.cn

TS:   arr.filter(x => x > 3)
来源：http://zla.hammf.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://cgw.chenlongwang.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://nhd.hnqzz.top

Ruby: arr.select { |x| x > 3 }
来源：http://gru.smart0.xyz

C#:   list.Where(x => x > 3).ToList()
来源：http://bgj.aizwys.cn

[D14] 映射转换（每个元素变形）
来源：http://iid.shanyushiyangkeji.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://auy.shangyingyoupin.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://tzw.yangfankeji.com

JS:   arr.map(x => x * 2)
来源：http://srl.haohaochexian.top

TS:   arr.map(x => x * 2)
来源：http://tzt.hfpthk.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://lnc.bbcook.cn

Go:   // 手写循环
来源：http://rpd.gogol.net.cn

Ruby: arr.map { |x| x * 2 }
来源：http://nvs.nwbrower.top

C#:   list.Select(x => x * 2).ToList()
来源：http://tva.epnwcf.com

[D15] 去重
来源：http://ooe.jinghuilouyu.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://dyf.nanxinkj.top

PHP:  array_unique($arr);
来源：http://sly.fktsv.cn

JS:   [...new Set(arr)]
来源：http://hwn.sjlbkw.cn

TS:   [...new Set(arr)]
来源：http://ijb.zhaomingkeji.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://leh.zhengqikj.top

Go:   // 用 map[T]struct{} 手写
来源：http://ktt.snrcjt.cn

Ruby: arr.uniq
来源：http://vur.vqdsnc.cn

C#:   list.Distinct().ToList()
来源：http://wkd.sufxvd.cn

[D16] 求和与平均值
来源：http://shi.yvedp.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://jrd.pengpengdd.cyou

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://yvd.nwbrower.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://xjo.feifeiyinyue.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://bug.yongpay.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://rzt.yvedp.cn

Go:   // 手写循环累加
来源：http://bjj.yj20258888.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://swh.xingfuxueyuan.xyz

C#:   list.Sum();  list.Average()
来源：http://ggq.hesvh.cn

[D17] 最大值与最小值
来源：http://jrs.nanxuanxn.top

Py:   max(arr);  min(arr)
来源：http://fxy.yangfankeji.com

PHP:  max($arr);  min($arr);
来源：http://yyo.shangyingyoupin.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ovs.daxiang520.top

TS:   Math.max(...arr);
来源：http://qji.hcnkem.com

Java: Collections.max(list);  Collections.min(list);
来源：http://skj.sxryk.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://iwk.cqqwz.cn

Ruby: arr.max;  arr.min
来源：http://nuk.iojbl.cn

C#:   list.Max();  list.Min()
来源：http://wku.yueranfly.top

[D18] 扁平化嵌套数组
来源：http://tex.kuanghao11.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://dbv.ppjwa.cn

PHP:  array_merge(...$nested);
来源：http://gin.cdnleiting.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://waq.chenlongwang.top

TS:   nested.flat();
来源：http://yei.chenlongwang.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://elb.aibaodan.cn

Go:   // 手写双层循环
来源：http://mre.yongpay.top

Ruby: nested.flatten
来源：http://dsm.kuanghao11.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://bln.xziqi.cn

[D19] 按字段分组
来源：http://mfa.quarkkingdee.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hqo.shanyushiyangtech.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qii.yongpay.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://jxy.hywenlv.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ruo.tianlin.xyz

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://dme.wangshuangyany.cn

Go:   // 手写 map[string][]T
来源：http://orp.fzhhl.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://jna.aizwys.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://fff.haohaochexian.top

[D20] 统计每个元素出现次数
来源：http://sqt.sxryk.cn

Py:   Counter(arr)
来源：http://cgt.jqgufenzy.top

PHP:  array_count_values($arr);
来源：http://ytu.pycfn.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wda.xinyue.icu

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qyi.gzhubu.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ynr.52xcode.cn

Go:   // 手写 map[T]int
来源：http://ubi.cqqwz.cn

Ruby: arr.tally
来源：http://urv.jiagoushi.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://sdw.cdnleiting.top

[D21] 判断是否包含某元素
来源：http://zct.hcnkem.com

Py:   x in arr
来源：http://xvu.redwolf501.top

PHP:  in_array($x, $arr, true);
来源：http://tys.zhengqikj.top

JS:   arr.includes(x)
来源：http://rbv.hywenlv.cn

TS:   arr.includes(x)
来源：http://cfj.kuanghao11.cn

Java: list.contains(x)
来源：http://dfo.hnqzz.top

Go:   slices.Contains(arr, x)
来源：http://nhq.daxiang520.top

Ruby: arr.include?(x)
来源：http://dom.gogol.net.cn

C#:   list.Contains(x)
来源：http://haa.ybcxt.top

[D22] 复制数组（避免共享引用）
来源：http://yxk.cashguo.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ceu.dianchejie.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ewf.fengsongda.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://xxu.fehbvm.com

TS:   [...arr];
来源：http://bvv.sufxvd.cn

Java: new ArrayList<>(list);
来源：http://xcu.tanke756.top

Go:   copied := append([]int(nil), arr...)
来源：http://yuf.ydzc1.top

Ruby: arr.dup;  arr.clone
来源：http://mtd.fanxiaobao.xyz

C#:   new List<int>(list);
来源：http://aub.ivvv.top

[D23] reduce 累积计算
来源：http://bvp.zhixingplan.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mpo.zhaomingkeji.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://fsa.xinyue.icu

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ywn.guowangkeji.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qbl.ydjk.org.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ndv.sweek.top

Go:   // 手写循环
来源：http://mqi.daria6918.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://dmi.fzhhl.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://nfp.hysaishi.cn

[D24] 字典 / Map 基本操作
来源：http://cru.gzhubu.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://cvv.shzxlz.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ngp.tanke756.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://lnf.aizwys.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ciw.shangyingyoupin.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://yfd.nanxinkj.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ceb.vehdjk.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://fst.hcnkem.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://dig.yangfankeji.com

[D25] Set 集合去重与交并差
来源：http://qal.xuanzx.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ztu.chenlongwang.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://doj.yj20258888.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://tku.316326.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://jtr.zhijiandao.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://saa.jqgfzy.top


<!-- 参考信息 -->