代发 wailian999

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://xdx.cucudq.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://lrs.9152youxi.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://jlc.hysaishi.cn

[C09] 递归
来源：http://cwn.sysykeji.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://raf.xuetiantiany.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wwh.zhongyouzk.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rxo.316326.xyz

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://snm.sufxvd.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://zwj.tarul.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://sta.daria6918.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://oli.nanxuanxn.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ncx.ehwqpu.com

[C10] 变量作用域
来源：http://hku.yj20258888.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://djo.bbcook.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://xnx.chenjidiqi.icu

JS:   let/const 块级作用域，var 函数级作用域
来源：http://lwi.dashuyun.cn

TS:   同 JS
来源：http://zoi.hnxiangtu.top

Java: 方法内为块级作用域
来源：http://kkt.snrcjt.cn

Go:   花括号块级作用域
来源：http://dui.cqqwz.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://fmj.haohaochexian.top

C#:   块级作用域
来源：http://mjp.redwolf501.top

[C11] 模块导入与导出
来源：http://nvv.zhengqikj.top

Py:   from module import func
来源：http://cbi.jinqigufen.top

PHP:  require "file.php";  或 use App\Service;
来源：http://fux.hfpthk.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://udg.sweek.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://rma.hcnkem.com

Java: import java.util.List;
来源：http://dfe.shzxlz.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://dlb.yueranfly.top

Ruby: require "json"; require_relative "./util"
来源：http://ges.shzxlz.cn

C#:   using System.Text;
来源：http://dqp.cdnleiting.top

[C12] 立即执行函数 IIFE
来源：http://cya.yj202588.top

Py:   (lambda: print("run"))()
来源：http://yub.fanxiaobao.xyz

PHP:  (function () { echo "run"; })();
来源：http://tcp.hywenlv.cn

JS:   (() => { console.log("run"); })();
来源：http://hxu.tian-w.cn

TS:   (() => { console.log("run"); })();
来源：http://ftn.c1oappe.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wkb.yongpay.top

Go:   func() { fmt.Println("run") }()
来源：http://dqa.vqdsnc.cn

Ruby: -> { puts "run" }.call
来源：http://cmt.shzxlz.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://axj.tanke756.top

[C13] 类型声明 / 类型注解
来源：http://lwf.gotoacloud.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wlv.daria6918.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cpo.zhoulong.xyz

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ilk.meibo888.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://guz.tarul.cn

Java: int add(int a, int b) { return a + b; }
来源：http://rdu.zhengqikj.top

Go:   func add(a, b int) int
来源：http://yje.jianghu66.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://njx.dashuyun.cn

C#:   int Add(int a, int b) => a + b;
来源：http://dfp.meibo888.top

[C14] 泛型函数
来源：http://xxn.ivvv.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://efs.vqdsnc.cn

PHP:  // 无泛型
来源：http://xzq.jinyuanbaomall.cn

JS:   // 无泛型
来源：http://pdr.9152youxi.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://uhs.nanxinkj.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://azy.jyoumei.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://day.daxiang520.top

Ruby: # 无泛型
来源：http://kvr.xinyue.icu

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ana.zhixingplan.top

[C15] 解构 / 展开参数
来源：http://zbk.yongpay.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://jjk.haohaochexian.top

PHP:  [$a, $b] = $pair;
来源：http://cww.quarkkingdee.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xxs.zhixingplan.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://gbg.zhoulong.xyz

Java: // 无解构
来源：http://qpl.iojbl.cn

Go:   // 无解构
来源：http://ajl.jinghuilouyu.cn

Ruby: a, b = pair
来源：http://ilk.ehwqpu.com

C#:   var (a, b) = pair;
来源：http://liq.ehwqpu.com

[C16] 函数 / 方法重载
来源：http://dci.vehdjk.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://jaj.sxryk.cn

PHP:  // 无重载
来源：http://lfg.zdqjudy.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://uxm.xuetiantiany.cn

TS:   // 用联合类型或重载签名声明
来源：http://wwz.shuidangran.top

Java: void f(int a) {}  void f(String a) {}
来源：http://iqk.cheryme.top

Go:   // 无重载：用不同函数名
来源：http://qjn.yanxiufei.cn

Ruby: # 无重载：靠动态参数
来源：http://dte.aizwys.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://xrj.dashuyun.cn

================================================================================
来源：http://bme.tian-w.cn

D. 数组 / 列表 / 集合
来源：http://leh.zhiwuduotai.top

================================================================================
来源：http://lrb.hnqzz.top

[D01] 创建数组 / 列表
来源：http://ahr.redwolf501.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://soz.hesvh.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://lbw.yanxiufei.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mns.hesvh.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://lug.zdqjudy.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://kla.daria6918.cn

Go:   arr := []int{1, 2, 3}
来源：http://twd.hysaishi.cn

Ruby: arr = [1, 2, 3]
来源：http://yfy.hcnkem.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ddb.fanxiaobao.xyz

[D02] 追加元素到末尾
来源：http://hnm.9152youxi.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://fsl.nwbrower.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ezj.shanyushiyangkeji.top

JS:   arr.push(4);
来源：http://erz.ehwqpu.com

TS:   arr.push(4);
来源：http://zqq.guannengcc.top

Java: list.add(4);
来源：http://igd.vqdsnc.cn

Go:   arr = append(arr, 4)
来源：http://bme.zhiwuduotai.top

Ruby: arr << 4; arr.push(5)
来源：http://btg.gogol.net.cn

C#:   list.Add(4);
来源：http://nku.shangyingyoupin.top

[D03] 在指定位置插入元素
来源：http://trw.vehdjk.com

Py:   arr.insert(0, 0)
来源：http://yri.shuidangran.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://oht.chenjidiqi.icu

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://szw.meibo888.top

TS:   arr.splice(0, 0, 0);
来源：http://hiz.cashguo.top

Java: list.add(0, 0);
来源：http://qnx.nanxuanxn.top

Go:   arr = append([]int{0}, arr...)
来源：http://kxh.hammf.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://biq.shangyingyoupin.top

C#:   list.Insert(0, 0);
来源：http://oog.cqqwz.cn

[D04] 删除元素
来源：http://ojr.epnwcf.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hbh.guannengcc.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://iwz.meibo888.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://abb.zhiwuduotai.top

TS:   arr.splice(0, 1);
来源：http://sji.hongshengwenyu.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://bsq.tarul.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://zly.jinqigufen.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ksr.zhiwuduotai.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hmd.tarul.cn

[D05] 访问与修改元素
来源：http://apk.gogol.net.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://gik.ybcxt.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ydv.pengpengdd.cyou

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://qdz.ydzc1.top

TS:   arr[0]; arr.at(-1);
来源：http://qsx.zdqjudy.top

Java: list.get(0); list.set(0, 9);
来源：http://izi.guowangkeji.top

Go:   arr[0]; arr[0] = 9
来源：http://mch.pycfn.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://gky.xuanzx.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://pif.jianghu66.top

[D06] 数组长度
来源：http://fzk.sweek.top

Py:   len(arr)
来源：http://fxu.jyoumei.cn

PHP:  count($arr);
来源：http://tln.ybcxt.top

JS:   arr.length
来源：http://det.xinyue.icu

TS:   arr.length
来源：http://knv.pengpengdd.cyou

Java: list.size();
来源：http://wvg.snrcjt.cn

Go:   len(arr)
来源：http://tmc.yj20258888.top

Ruby: arr.length; arr.size
来源：http://bem.yj20258.top

C#:   list.Count;
来源：http://ahb.gaohongyu789.top

[D07] 切片 / 取子数组
来源：http://fky.jyoumei.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ywt.fehbvm.com

PHP:  array_slice($arr, 1, 3);
来源：http://ifm.zdqjudy.top

JS:   arr.slice(1, 4);
来源：http://ctd.meibo888.top

TS:   arr.slice(1, 4);
来源：http://zsx.nanxinkj.top

Java: list.subList(1, 4);
来源：http://mkg.gotoacloud.top

Go:   arr[1:4]
来源：http://fth.ybcxt.top

Ruby: arr[1, 3]
来源：http://msd.fktsv.cn

C#:   list.GetRange(1, 3);
来源：http://kfm.bjfxy.top

[D08] 合并两个数组
来源：http://ezm.0kj1m.cn

Py:   a + b;  a.extend(b)
来源：http://mbz.epnwcf.com

PHP:  array_merge($a, $b);
来源：http://xyz.hcnkem.com

JS:   [...a, ...b];  a.concat(b);
来源：http://dgd.yvedp.cn

TS:   [...a, ...b];
来源：http://wnq.hysaishi.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://fqa.cucudq.cn

Go:   append(a, b...)
来源：http://bri.tanke756.top

Ruby: a + b;  a.concat(b)
来源：http://ohc.tianlin.xyz

C#:   a.Concat(b).ToList()
来源：http://vca.gzhubu.top

[D09] 排序（升序）
来源：http://kzu.shanyushiyangkeji.top

Py:   sorted(arr);  arr.sort()
来源：http://mnh.hammf.cn

PHP:  sort($arr);
来源：http://ins.birdmap.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://pzl.yangfankeji.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://ajc.ehwqpu.com

Java: Collections.sort(list);  list.sort(null);
来源：http://wzg.fzhhl.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://drw.sxryk.cn

Ruby: arr.sort
来源：http://iur.haohaochexian.top

C#:   list.Sort();
来源：http://ldp.ppjwa.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ycv.ctjpmb.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://exr.jinqigfzy.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://sfj.cashguo.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://tgu.wangdashe.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://yds.redwolf501.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://qyp.hysaishi.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://smj.jianghu66.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://rjo.jlsjyb.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://owo.hywenlv.cn

[D11] 反转数组
来源：http://nnv.shanyushiyangkeji.top

Py:   arr[::-1];  arr.reverse()
来源：http://qdu.havefunace.top

PHP:  array_reverse($arr);
来源：http://tva.zhaomingkeji.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://zje.havefunace.top

TS:   [...arr].reverse();
来源：http://loz.fktsv.cn

Java: Collections.reverse(list);
来源：http://ehr.aibaodan.cn

Go:   slices.Reverse(arr)
来源：http://jsp.pycfn.com

Ruby: arr.reverse
来源：http://wbd.zhaomingkeji.xyz

C#:   list.Reverse();
来源：http://fyj.hammf.cn

[D12] 查找元素下标
来源：http://okg.sweek.top

Py:   arr.index(x);  x in arr
来源：http://xxi.jinqigfzy.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://qvw.9152youxi.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tnz.zycfv.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qwa.vehdjk.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ylc.xingfuxueyuan.xyz

Go:   slices.Index(arr, x)
来源：http://hlr.guannengcc.top

Ruby: arr.index(x)
来源：http://fxu.gotoacloud.top

C#:   list.IndexOf(x);
来源：http://sny.pengpengdd.cyou

[D13] 过滤（保留满足条件的）
来源：http://kpq.jianghu66.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://rxx.smart0.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ezv.yj20258888.top

JS:   arr.filter(x => x > 3)
来源：http://azq.0kj1m.cn

TS:   arr.filter(x => x > 3)
来源：http://aag.birdmap.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://bfe.cdnleiting.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://alu.jqgufenzy.top

Ruby: arr.select { |x| x > 3 }
来源：http://exy.yj20258.top

C#:   list.Where(x => x > 3).ToList()
来源：http://kgj.xuanzx.com

[D14] 映射转换（每个元素变形）
来源：http://igg.vqdsnc.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://tyf.zdbjq.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ywd.yj20258888.top

JS:   arr.map(x => x * 2)
来源：http://oef.kuanghao11.cn

TS:   arr.map(x => x * 2)
来源：http://nwn.sufxvd.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://gae.daria6918.cn

Go:   // 手写循环
来源：http://qsw.ivvv.top

Ruby: arr.map { |x| x * 2 }
来源：http://ueu.hammf.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://fvl.shuidangran.top

[D15] 去重
来源：http://uyr.yj20258.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://qyo.shanyushiyangkeji.top

PHP:  array_unique($arr);
来源：http://lob.sjlbkw.cn

JS:   [...new Set(arr)]
来源：http://jjk.redwolf501.top

TS:   [...new Set(arr)]
来源：http://qxx.jinyuanbaomall.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://icu.guannengcc.top

Go:   // 用 map[T]struct{} 手写
来源：http://vjn.andypj.xyz

Ruby: arr.uniq
来源：http://wcm.yfazqb.com

C#:   list.Distinct().ToList()
来源：http://pnh.hnxiangtu.top

[D16] 求和与平均值
来源：http://get.jqgufenzy.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://asz.ppjwa.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://sxr.hammf.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://gno.ydjk.org.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://xbo.jinghuilouyu.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://uso.yj202588.top

Go:   // 手写循环累加
来源：http://vtu.xinyue.icu

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://dnj.cdnleiting.top

C#:   list.Sum();  list.Average()
来源：http://pzj.jinyuanbaomall.cn

[D17] 最大值与最小值
来源：http://kbf.sweek.top

Py:   max(arr);  min(arr)
来源：http://xca.bjfxy.top

PHP:  max($arr);  min($arr);
来源：http://vzb.cucudq.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://znt.vqdsnc.cn

TS:   Math.max(...arr);
来源：http://hgl.zhengqikj.top

Java: Collections.max(list);  Collections.min(list);
来源：http://ciq.vqdsnc.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://sms.hongshengwenyu.top

Ruby: arr.max;  arr.min
来源：http://zvv.tianlin.xyz

C#:   list.Max();  list.Min()
来源：http://zjk.jqgfzy.top

[D18] 扁平化嵌套数组
来源：http://pyp.cqqwz.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://viu.jqgfzy.top

PHP:  array_merge(...$nested);
来源：http://mkr.yueranfly.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://efi.yfazqb.com

TS:   nested.flat();
来源：http://ibs.tian-w.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://gvz.zhoulong.xyz

Go:   // 手写双层循环
来源：http://yyc.cheryme.top

Ruby: nested.flatten
来源：http://iao.quarkkingdee.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://are.hesvh.cn

[D19] 按字段分组
来源：http://ayb.xinyue.icu

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://zmf.zdqjudy.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://kfz.zhiwuduotai.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://dqb.daxiang520.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://vaj.ydjk.org.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://jnb.cqqwz.cn

Go:   // 手写 map[string][]T
来源：http://ozd.nanxinkj.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://eqw.zhaomingkeji.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://afh.xuetiantiany.cn

[D20] 统计每个元素出现次数
来源：http://fjh.snrcjt.cn

Py:   Counter(arr)
来源：http://vji.pengpengdd.cyou

PHP:  array_count_values($arr);
来源：http://ytp.jiagoushi.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lju.yanxiufei.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qsd.yueranfly.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://fwj.shanyushiyangkeji.top

Go:   // 手写 map[T]int
来源：http://dbs.dianchejie.cn

Ruby: arr.tally
来源：http://enn.haohaochexian.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://cxl.haohaochexian.top

[D21] 判断是否包含某元素
来源：http://shq.iojbl.cn

Py:   x in arr
来源：http://ybq.ppjwa.cn

PHP:  in_array($x, $arr, true);
来源：http://uhk.quarkkingdee.top

JS:   arr.includes(x)
来源：http://uzv.shanyushiyangtech.top

TS:   arr.includes(x)
来源：http://ste.andypj.xyz

Java: list.contains(x)
来源：http://tpf.zhoulong.xyz

Go:   slices.Contains(arr, x)
来源：http://hyc.yuanzhike.top

Ruby: arr.include?(x)
来源：http://xrf.nanxinkj.top

C#:   list.Contains(x)
来源：http://zus.hfpthk.cn

[D22] 复制数组（避免共享引用）
来源：http://qzt.52xcode.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mge.bbcook.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://rqh.ydzc1.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://unk.zycfv.cn

TS:   [...arr];
来源：http://jis.birdmap.top

Java: new ArrayList<>(list);
来源：http://ncb.guannengcc.top

Go:   copied := append([]int(nil), arr...)
来源：http://wnw.hnxiangtu.top

Ruby: arr.dup;  arr.clone
来源：http://meo.andypj.xyz

C#:   new List<int>(list);
来源：http://sqr.cheryme.top

[D23] reduce 累积计算
来源：http://tzq.nanxuanxn.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://sfn.zycfv.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://yfv.havefunace.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ank.xuanzx.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tim.yanxiufei.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://lgy.hongshengwenyu.top

Go:   // 手写循环
来源：http://yvy.jlsjyb.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://nbt.jlsjyb.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://dkz.iojbl.cn

[D24] 字典 / Map 基本操作
来源：http://hpi.tarul.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://nse.jinghuilouyu.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://sds.vehdjk.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://eth.snrcjt.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://bvf.hammf.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://gxg.tian-w.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://tfa.haohaochexian.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://rgf.nanxinkj.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://lbg.zhongyouzk.top

[D25] Set 集合去重与交并差
来源：http://xrw.hnqzz.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://gce.dianchejie.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://nay.hammf.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://yhu.hywenlv.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://zcm.guowangkeji.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wuu.yongpay.top


<!-- 参考信息 -->