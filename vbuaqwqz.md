代发 wailian999

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://jdy.ybcxt.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://oep.zhiwuduotai.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lka.yfazqb.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ezm.gogol.net.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://erm.meibo888.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://upl.cashguo.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ave.jqgfzy.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://vcc.hesvh.cn

[C10] 变量作用域
来源：http://dia.tanke756.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://osf.pengpengdd.cyou

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ynz.xuetiantiany.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ona.feifeiyinyue.top

TS:   同 JS
来源：http://vjo.jianghu66.top

Java: 方法内为块级作用域
来源：http://nvj.gogol.net.cn

Go:   花括号块级作用域
来源：http://mba.ivvv.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://nud.guowangkeji.top

C#:   块级作用域
来源：http://cuo.yj202588.top

[C11] 模块导入与导出
来源：http://nvh.zhaomingkeji.xyz

Py:   from module import func
来源：http://mxm.jiagoushi.top

PHP:  require "file.php";  或 use App\Service;
来源：http://mpq.yj20258888.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://hcl.zhijiandao.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://zpb.gogol.net.cn

Java: import java.util.List;
来源：http://jpz.gotoacloud.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://rlj.daria6918.cn

Ruby: require "json"; require_relative "./util"
来源：http://osj.zhaomingkeji.xyz

C#:   using System.Text;
来源：http://vwk.chenlongwang.top

[C12] 立即执行函数 IIFE
来源：http://yuh.fzhhl.top

Py:   (lambda: print("run"))()
来源：http://ibw.shanyushiyangkeji.top

PHP:  (function () { echo "run"; })();
来源：http://fks.ehwqpu.com

JS:   (() => { console.log("run"); })();
来源：http://zss.jinqigufen.top

TS:   (() => { console.log("run"); })();
来源：http://aup.zhixingplan.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://cuj.fzhhl.top

Go:   func() { fmt.Println("run") }()
来源：http://kty.aizwys.cn

Ruby: -> { puts "run" }.call
来源：http://poj.yonumen.top

C#:   // 无 IIFE：用静态构造函数
来源：http://aah.shuidangran.top

[C13] 类型声明 / 类型注解
来源：http://tqp.gzhubu.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://knp.hongshengwenyu.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xke.shuidangran.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://vlt.ydjk.org.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ijw.zhoulong.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://eae.bbcook.cn

Go:   func add(a, b int) int
来源：http://opz.gzhubu.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ziz.quarkkingdee.top

C#:   int Add(int a, int b) => a + b;
来源：http://reo.hammf.cn

[C14] 泛型函数
来源：http://gpq.wangdashe.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://szx.chenlongwang.top

PHP:  // 无泛型
来源：http://ayt.hongshengwenyu.top

JS:   // 无泛型
来源：http://vwm.fengsongda.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mnm.haohaochexian.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ghc.yj20258888.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://nga.hesvh.cn

Ruby: # 无泛型
来源：http://lgc.ehwqpu.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://pbq.ybcxt.top

[C15] 解构 / 展开参数
来源：http://alj.shzxlz.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://nwk.haohaochexian.top

PHP:  [$a, $b] = $pair;
来源：http://llw.yanxiufei.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://axn.shangyingyoupin.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://zoe.nanxinkj.top

Java: // 无解构
来源：http://xle.dianchejie.cn

Go:   // 无解构
来源：http://udo.hysaishi.cn

Ruby: a, b = pair
来源：http://yqk.svipenyu.cn

C#:   var (a, b) = pair;
来源：http://mmi.yonumen.top

[C16] 函数 / 方法重载
来源：http://jqc.tianlin.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ukx.birdmap.top

PHP:  // 无重载
来源：http://ksy.52xcode.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://zlf.aizwys.cn

TS:   // 用联合类型或重载签名声明
来源：http://kvk.jinqigufen.top

Java: void f(int a) {}  void f(String a) {}
来源：http://kqz.xylfe.cn

Go:   // 无重载：用不同函数名
来源：http://vxo.ppjwa.cn

Ruby: # 无重载：靠动态参数
来源：http://zqi.cashguo.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://nln.9152youxi.cn

================================================================================
来源：http://tvl.shuidangran.top

D. 数组 / 列表 / 集合
来源：http://fnf.pycfn.com

================================================================================
来源：http://rgs.yvedp.cn

[D01] 创建数组 / 列表
来源：http://znk.cheryme.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://nic.yangfankeji.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ajk.nanxinkj.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hja.gaohongyu789.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://iha.cqqwz.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://phg.gzhubu.top

Go:   arr := []int{1, 2, 3}
来源：http://ara.guowangkeji.top

Ruby: arr = [1, 2, 3]
来源：http://xmw.jiagoushi.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://sok.yj20258888.top

[D02] 追加元素到末尾
来源：http://oll.jqgfzy.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://gju.jinyuanbaomall.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://yjd.fanxiaobao.xyz

JS:   arr.push(4);
来源：http://kze.dashuyun.cn

TS:   arr.push(4);
来源：http://cgv.ivvv.top

Java: list.add(4);
来源：http://pyd.wangshuangyany.cn

Go:   arr = append(arr, 4)
来源：http://csd.jinqigfzy.top

Ruby: arr << 4; arr.push(5)
来源：http://aba.zhaomingkeji.xyz

C#:   list.Add(4);
来源：http://fbq.ppjwa.cn

[D03] 在指定位置插入元素
来源：http://xux.chenzaomai.com

Py:   arr.insert(0, 0)
来源：http://xyp.hesvh.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://akk.gzhubu.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://xqe.dianchejie.cn

TS:   arr.splice(0, 0, 0);
来源：http://vsc.xuanzx.com

Java: list.add(0, 0);
来源：http://ybc.nanxinkj.top

Go:   arr = append([]int{0}, arr...)
来源：http://xid.cucudq.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://vyk.uphjek.com

C#:   list.Insert(0, 0);
来源：http://omg.yueranfly.top

[D04] 删除元素
来源：http://rdj.shanyushiyangkeji.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://dbo.sxryk.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://abp.uphjek.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://pcv.0kj1m.cn

TS:   arr.splice(0, 1);
来源：http://cbi.sxryk.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://bzx.wangdashe.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://vyb.aizwys.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://bfv.uphjek.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://duh.haohaochexian.top

[D05] 访问与修改元素
来源：http://ajv.yonumen.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://zst.yfazqb.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://qhi.shanyushiyangtech.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://qzj.shzxlz.cn

TS:   arr[0]; arr.at(-1);
来源：http://qxs.jiagoushi.top

Java: list.get(0); list.set(0, 9);
来源：http://poy.fzhhl.top

Go:   arr[0]; arr[0] = 9
来源：http://tld.hywenlv.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://bdc.tian-w.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mor.hongshengwenyu.top

[D06] 数组长度
来源：http://vou.0kj1m.cn

Py:   len(arr)
来源：http://iih.shzxlz.cn

PHP:  count($arr);
来源：http://ips.zdbjq.cn

JS:   arr.length
来源：http://kad.jiagoushi.top

TS:   arr.length
来源：http://gpt.cashguo.top

Java: list.size();
来源：http://dmv.zhoulong.xyz

Go:   len(arr)
来源：http://ybo.ywan-chungtsiang.top

Ruby: arr.length; arr.size
来源：http://syq.jinqigufen.top

C#:   list.Count;
来源：http://qvg.bbcook.cn

[D07] 切片 / 取子数组
来源：http://iuy.gotoacloud.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://sdu.aibaodan.cn

PHP:  array_slice($arr, 1, 3);
来源：http://eiv.zycfv.cn

JS:   arr.slice(1, 4);
来源：http://hya.hongshengwenyu.top

TS:   arr.slice(1, 4);
来源：http://bcu.fktsv.cn

Java: list.subList(1, 4);
来源：http://lab.bbcook.cn

Go:   arr[1:4]
来源：http://rtt.ppjwa.cn

Ruby: arr[1, 3]
来源：http://yjn.52xcode.cn

C#:   list.GetRange(1, 3);
来源：http://kiu.meibo888.top

[D08] 合并两个数组
来源：http://gmc.gaohongyu789.top

Py:   a + b;  a.extend(b)
来源：http://kpn.chenlongwang.top

PHP:  array_merge($a, $b);
来源：http://spy.c1oappe.top

JS:   [...a, ...b];  a.concat(b);
来源：http://xme.mhx1999.top

TS:   [...a, ...b];
来源：http://ezp.fehbvm.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ltn.epnwcf.com

Go:   append(a, b...)
来源：http://lba.nwbrower.top

Ruby: a + b;  a.concat(b)
来源：http://pbw.zhixingplan.top

C#:   a.Concat(b).ToList()
来源：http://mbd.gaohongyu789.top

[D09] 排序（升序）
来源：http://zgt.gaohongyu789.top

Py:   sorted(arr);  arr.sort()
来源：http://tqg.shanyushiyangtech.top

PHP:  sort($arr);
来源：http://xdh.cheryme.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://zxy.jqgufenzy.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://rnl.cucudq.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ttb.316326.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://raz.tian-w.cn

Ruby: arr.sort
来源：http://txc.yuanzhike.top

C#:   list.Sort();
来源：http://bhk.wangdashe.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://yae.yongpay.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://azu.guannengcc.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pdh.jlsjyb.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://edw.uphjek.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wxz.meibo888.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://vwq.hcnkem.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://cbs.0kj1m.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://cfk.chenzaomai.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://vvw.yonumen.top

[D11] 反转数组
来源：http://ovd.ppjwa.cn

Py:   arr[::-1];  arr.reverse()
来源：http://sik.yj20258888.top

PHP:  array_reverse($arr);
来源：http://sof.guowangkeji.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wia.sweek.top

TS:   [...arr].reverse();
来源：http://evg.jyoumei.cn

Java: Collections.reverse(list);
来源：http://jbn.guowangkeji.top

Go:   slices.Reverse(arr)
来源：http://ksf.shzxlz.cn

Ruby: arr.reverse
来源：http://yql.bjfxy.top

C#:   list.Reverse();
来源：http://nrl.hammf.cn

[D12] 查找元素下标
来源：http://zbw.guowangkeji.top

Py:   arr.index(x);  x in arr
来源：http://jhx.hnxiangtu.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://xtz.vqdsnc.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qdu.xuanzx.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://oir.gzhubu.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://gpo.andypj.xyz

Go:   slices.Index(arr, x)
来源：http://fwf.fzhhl.top

Ruby: arr.index(x)
来源：http://ljn.fktsv.cn

C#:   list.IndexOf(x);
来源：http://lwg.ydzc1.top

[D13] 过滤（保留满足条件的）
来源：http://apf.feifeiyinyue.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://vqj.shangyingyoupin.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://nxp.hesvh.cn

JS:   arr.filter(x => x > 3)
来源：http://bgh.tarul.cn

TS:   arr.filter(x => x > 3)
来源：http://agb.zhixingplan.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://slx.havefunace.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://uup.hcnkem.com

Ruby: arr.select { |x| x > 3 }
来源：http://oqq.havefunace.top

C#:   list.Where(x => x > 3).ToList()
来源：http://obt.vqdsnc.cn

[D14] 映射转换（每个元素变形）
来源：http://tls.ehwqpu.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ruu.yonumen.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://oio.yuanzhike.top

JS:   arr.map(x => x * 2)
来源：http://dsz.c1oappe.top

TS:   arr.map(x => x * 2)
来源：http://jyv.xingfuxueyuan.xyz

Java: list.stream().map(x -> x * 2).toList()
来源：http://ivz.vqdsnc.cn

Go:   // 手写循环
来源：http://dyp.c1oappe.top

Ruby: arr.map { |x| x * 2 }
来源：http://nxm.shanyushiyangkeji.top

C#:   list.Select(x => x * 2).ToList()
来源：http://egt.9152youxi.cn

[D15] 去重
来源：http://ywc.zhixingplan.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://azy.hesvh.cn

PHP:  array_unique($arr);
来源：http://suz.shangyingyoupin.top

JS:   [...new Set(arr)]
来源：http://dyt.hcnkem.com

TS:   [...new Set(arr)]
来源：http://afo.gaohongyu789.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://sis.smart0.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://pfx.yfazqb.com

Ruby: arr.uniq
来源：http://nsp.fktsv.cn

C#:   list.Distinct().ToList()
来源：http://wvg.sxryk.cn

[D16] 求和与平均值
来源：http://sgk.jinqigufen.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://gyj.vehdjk.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://nzk.guowangkeji.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://npz.52xcode.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ppe.tarul.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baj.sweek.top

Go:   // 手写循环累加
来源：http://vwc.cashguo.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://bim.zdqjudy.top

C#:   list.Sum();  list.Average()
来源：http://vxt.jiagoushi.top

[D17] 最大值与最小值
来源：http://uoy.daria6918.cn

Py:   max(arr);  min(arr)
来源：http://oub.tianlin.xyz

PHP:  max($arr);  min($arr);
来源：http://tfm.zdqjudy.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://xac.shzxlz.cn

TS:   Math.max(...arr);
来源：http://vvj.ppjwa.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://qpm.xinyue.icu

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://zfq.yuxming.cn

Ruby: arr.max;  arr.min
来源：http://mgj.ywan-chungtsiang.top

C#:   list.Max();  list.Min()
来源：http://wdq.yuxming.cn

[D18] 扁平化嵌套数组
来源：http://cep.svipenyu.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://cwh.shuidangran.top

PHP:  array_merge(...$nested);
来源：http://lne.haohaochexian.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://kdv.wangshuangyany.cn

TS:   nested.flat();
来源：http://yvi.hywenlv.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://nur.jyoumei.cn

Go:   // 手写双层循环
来源：http://ivw.wangshuangyany.cn

Ruby: nested.flatten
来源：http://wln.52xcode.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://wnj.316326.xyz

[D19] 按字段分组
来源：http://ixj.hongshengwenyu.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hif.ehwqpu.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ibn.uphjek.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://vac.jinqigufen.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://baz.zhongyouzk.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ecu.ppjwa.cn

Go:   // 手写 map[string][]T
来源：http://kum.tian-w.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://dqu.hnxiangtu.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://kex.yj20258888.top

[D20] 统计每个元素出现次数
来源：http://zwy.cucudq.cn

Py:   Counter(arr)
来源：http://dwr.jiagoushi.top

PHP:  array_count_values($arr);
来源：http://fmm.chenjidiqi.icu

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://uvl.jinghuilouyu.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ilh.xuanzx.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://zvl.316326.xyz

Go:   // 手写 map[T]int
来源：http://dmp.sjlbkw.cn

Ruby: arr.tally
来源：http://gxh.jinghuilouyu.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://tkb.daria6918.cn

[D21] 判断是否包含某元素
来源：http://hcq.fengsongda.top

Py:   x in arr
来源：http://xze.jlsjyb.cn

PHP:  in_array($x, $arr, true);
来源：http://sff.hnxiangtu.top

JS:   arr.includes(x)
来源：http://gbx.jinqigfzy.top

TS:   arr.includes(x)
来源：http://mtw.cdnleiting.top

Java: list.contains(x)
来源：http://oaj.xingfuxueyuan.xyz

Go:   slices.Contains(arr, x)
来源：http://qge.yonumen.top

Ruby: arr.include?(x)
来源：http://mqq.gzhubu.top

C#:   list.Contains(x)
来源：http://rkv.zdbjq.cn

[D22] 复制数组（避免共享引用）
来源：http://mms.iojbl.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ckx.gzhubu.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ueh.jqgufenzy.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://xac.tianlin.xyz

TS:   [...arr];
来源：http://ekg.yfazqb.com

Java: new ArrayList<>(list);
来源：http://fdf.shzxlz.cn

Go:   copied := append([]int(nil), arr...)
来源：http://qra.hesvh.cn

Ruby: arr.dup;  arr.clone
来源：http://gae.jyoumei.cn

C#:   new List<int>(list);
来源：http://wty.hongshengwenyu.top

[D23] reduce 累积计算
来源：http://ehl.fengsongda.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://jwl.fktsv.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://jcz.hammf.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ooh.epnwcf.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pyq.zhengqikj.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://jpb.cdnleiting.top

Go:   // 手写循环
来源：http://uur.xziqi.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://huo.sxryk.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://lnp.yfazqb.com

[D24] 字典 / Map 基本操作
来源：http://hrd.yangfankeji.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mgo.jinqigufen.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://pdp.dianchejie.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://apy.yfazqb.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://zrr.hfpthk.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://bqn.zhijiandao.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ble.jianghu66.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://bzj.yonumen.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://pnn.0kj1m.cn

[D25] Set 集合去重与交并差
来源：http://ygf.tarul.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://lve.zdbjq.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://yks.xziqi.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ixm.gotoacloud.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mhr.xylfe.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://cts.fengsongda.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://nzm.nwbrower.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ecf.birdmap.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://btw.yuanzhike.top

[D26] 数组转字符串
来源：http://rvk.yfazqb.com


<!-- 参考信息 -->