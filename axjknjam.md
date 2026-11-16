代发 wailian999

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://tkf.svipenyu.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://xcu.jiagoushi.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nhe.tian-w.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gai.ydzc1.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://rxa.shanyushiyangtech.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ydd.chenjidiqi.icu

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://lha.tianlin.xyz

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://igc.guannengcc.top

[C10] 变量作用域
来源：http://lul.jqgfzy.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://sgh.hywenlv.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ksg.xuetiantiany.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://bnc.birdmap.top

TS:   同 JS
来源：http://jem.zhoulong.xyz

Java: 方法内为块级作用域
来源：http://gym.yuanzhike.top

Go:   花括号块级作用域
来源：http://ggg.andypj.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://txp.xinyue.icu

C#:   块级作用域
来源：http://xmv.jianghu66.top

[C11] 模块导入与导出
来源：http://sbr.sysykeji.top

Py:   from module import func
来源：http://ozu.daxiang520.top

PHP:  require "file.php";  或 use App\Service;
来源：http://zxi.jinyuanbaomall.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://dun.havefunace.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://cmz.jlsjyb.cn

Java: import java.util.List;
来源：http://tmk.yuxming.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://rvd.yongpay.top

Ruby: require "json"; require_relative "./util"
来源：http://mjd.gaohongyu789.top

C#:   using System.Text;
来源：http://req.zycfv.cn

[C12] 立即执行函数 IIFE
来源：http://ltm.fktsv.cn

Py:   (lambda: print("run"))()
来源：http://shx.wangshuangyany.cn

PHP:  (function () { echo "run"; })();
来源：http://vfl.ehwqpu.com

JS:   (() => { console.log("run"); })();
来源：http://lhc.316326.xyz

TS:   (() => { console.log("run"); })();
来源：http://esr.dashuyun.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ebq.epnwcf.com

Go:   func() { fmt.Println("run") }()
来源：http://ytj.xylfe.cn

Ruby: -> { puts "run" }.call
来源：http://faa.aizwys.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://hea.hammf.cn

[C13] 类型声明 / 类型注解
来源：http://ccz.xingfuxueyuan.xyz

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://cou.fengsongda.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://amq.uphjek.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://rxl.hammf.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hqm.pycfn.com

Java: int add(int a, int b) { return a + b; }
来源：http://umw.cashguo.top

Go:   func add(a, b int) int
来源：http://ska.c1oappe.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ioy.jinqigufen.top

C#:   int Add(int a, int b) => a + b;
来源：http://dmd.pengpengdd.cyou

[C14] 泛型函数
来源：http://oqb.shanyushiyangtech.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://jyk.xinyue.icu

PHP:  // 无泛型
来源：http://dmg.sysykeji.top

JS:   // 无泛型
来源：http://qog.c1oappe.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://dyn.yanxiufei.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://deq.ybcxt.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://xjl.hysaishi.cn

Ruby: # 无泛型
来源：http://fgz.tarul.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://qlq.jqgfzy.top

[C15] 解构 / 展开参数
来源：http://xnt.ywan-chungtsiang.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://imm.52xcode.cn

PHP:  [$a, $b] = $pair;
来源：http://pai.0kj1m.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mrv.bbcook.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mtr.gogol.net.cn

Java: // 无解构
来源：http://uoq.zhiwuduotai.top

Go:   // 无解构
来源：http://znj.yvedp.cn

Ruby: a, b = pair
来源：http://wiy.hongshengwenyu.top

C#:   var (a, b) = pair;
来源：http://syj.pengpengdd.cyou

[C16] 函数 / 方法重载
来源：http://luo.fanxiaobao.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ufx.sxryk.cn

PHP:  // 无重载
来源：http://xyi.cashguo.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://zvz.xinyue.icu

TS:   // 用联合类型或重载签名声明
来源：http://jcp.ppjwa.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://wgz.hnxiangtu.top

Go:   // 无重载：用不同函数名
来源：http://axl.316326.xyz

Ruby: # 无重载：靠动态参数
来源：http://ncj.dashuyun.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://lea.dianchejie.cn

================================================================================
来源：http://lvw.havefunace.top

D. 数组 / 列表 / 集合
来源：http://bgx.cucudq.cn

================================================================================
来源：http://gox.pengpengdd.cyou

[D01] 创建数组 / 列表
来源：http://jxd.feifeiyinyue.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://tma.smart0.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://bav.yueranfly.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://qgi.xuanzx.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://kps.hongshengwenyu.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://bjd.uphjek.com

Go:   arr := []int{1, 2, 3}
来源：http://tmq.sweek.top

Ruby: arr = [1, 2, 3]
来源：http://hbs.nanxinkj.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ivm.xuetiantiany.cn

[D02] 追加元素到末尾
来源：http://qwr.fanxiaobao.xyz

Py:   arr.append(4); arr.extend([5, 6])
来源：http://tkx.zhijiandao.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://urh.guannengcc.top

JS:   arr.push(4);
来源：http://nsi.sxryk.cn

TS:   arr.push(4);
来源：http://xky.jyoumei.cn

Java: list.add(4);
来源：http://knr.jyoumei.cn

Go:   arr = append(arr, 4)
来源：http://qpf.0kj1m.cn

Ruby: arr << 4; arr.push(5)
来源：http://tyl.nanxinkj.top

C#:   list.Add(4);
来源：http://hqn.hywenlv.cn

[D03] 在指定位置插入元素
来源：http://vnc.fzhhl.top

Py:   arr.insert(0, 0)
来源：http://fvr.yonumen.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://tmx.sxryk.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://fqb.ydjk.org.cn

TS:   arr.splice(0, 0, 0);
来源：http://bgf.ywan-chungtsiang.top

Java: list.add(0, 0);
来源：http://poa.gzhubu.top

Go:   arr = append([]int{0}, arr...)
来源：http://utv.yongpay.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://akb.gogol.net.cn

C#:   list.Insert(0, 0);
来源：http://cxo.quarkkingdee.top

[D04] 删除元素
来源：http://odh.nanxuanxn.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://qwc.hnqzz.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ssv.yangfankeji.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://imj.jiagoushi.top

TS:   arr.splice(0, 1);
来源：http://sfv.yj202588.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wzg.xziqi.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://nig.zdqjudy.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ktw.wangdashe.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://fun.nwbrower.top

[D05] 访问与修改元素
来源：http://jpj.aizwys.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://nkx.tanke756.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://nvs.52xcode.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://vts.hammf.cn

TS:   arr[0]; arr.at(-1);
来源：http://cvv.ybcxt.top

Java: list.get(0); list.set(0, 9);
来源：http://toz.fengsongda.top

Go:   arr[0]; arr[0] = 9
来源：http://mld.daria6918.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hsf.zhiwuduotai.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://dgs.xingfuxueyuan.xyz

[D06] 数组长度
来源：http://tor.yj202588.top

Py:   len(arr)
来源：http://qqn.gogol.net.cn

PHP:  count($arr);
来源：http://evq.gaohongyu789.top

JS:   arr.length
来源：http://wkl.guowangkeji.top

TS:   arr.length
来源：http://zpe.yj20258888.top

Java: list.size();
来源：http://yxe.yonumen.top

Go:   len(arr)
来源：http://vrm.xingfuxueyuan.xyz

Ruby: arr.length; arr.size
来源：http://icz.havefunace.top

C#:   list.Count;
来源：http://mau.jqgfzy.top

[D07] 切片 / 取子数组
来源：http://kgk.hesvh.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ruj.cashguo.top

PHP:  array_slice($arr, 1, 3);
来源：http://jsr.jinghuilouyu.cn

JS:   arr.slice(1, 4);
来源：http://jst.quarkkingdee.top

TS:   arr.slice(1, 4);
来源：http://jxb.yuxming.cn

Java: list.subList(1, 4);
来源：http://oxv.sufxvd.cn

Go:   arr[1:4]
来源：http://hsv.hammf.cn

Ruby: arr[1, 3]
来源：http://gey.nanxuanxn.top

C#:   list.GetRange(1, 3);
来源：http://ovt.jyoumei.cn

[D08] 合并两个数组
来源：http://oop.yj20258.top

Py:   a + b;  a.extend(b)
来源：http://thh.jinqigfzy.top

PHP:  array_merge($a, $b);
来源：http://ypb.yuanzhike.top

JS:   [...a, ...b];  a.concat(b);
来源：http://svn.snrcjt.cn

TS:   [...a, ...b];
来源：http://ane.zhengqikj.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://pma.tian-w.cn

Go:   append(a, b...)
来源：http://cfu.gaohongyu789.top

Ruby: a + b;  a.concat(b)
来源：http://lyv.jinqigfzy.top

C#:   a.Concat(b).ToList()
来源：http://nbm.xuanzx.com

[D09] 排序（升序）
来源：http://mqx.xuanzx.com

Py:   sorted(arr);  arr.sort()
来源：http://hqr.yfazqb.com

PHP:  sort($arr);
来源：http://nao.hfpthk.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wme.aizwys.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://kxd.jlsjyb.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://lij.tarul.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://olx.zycfv.cn

Ruby: arr.sort
来源：http://jay.gogol.net.cn

C#:   list.Sort();
来源：http://kec.sysykeji.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://pzv.shanyushiyangtech.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ofd.fanxiaobao.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gtp.jiagoushi.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://rta.jianghu66.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://xfi.0kj1m.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://nac.hesvh.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://lha.hongshengwenyu.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://sdu.ctjpmb.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://nny.jinqigfzy.top

[D11] 反转数组
来源：http://xqi.gzhubu.top

Py:   arr[::-1];  arr.reverse()
来源：http://yla.zhijiandao.cn

PHP:  array_reverse($arr);
来源：http://syt.zhiwuduotai.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://eyc.jinyuanbaomall.cn

TS:   [...arr].reverse();
来源：http://fyp.snrcjt.cn

Java: Collections.reverse(list);
来源：http://uka.shzxlz.cn

Go:   slices.Reverse(arr)
来源：http://iks.zhaomingkeji.xyz

Ruby: arr.reverse
来源：http://icj.iojbl.cn

C#:   list.Reverse();
来源：http://eej.jiagoushi.top

[D12] 查找元素下标
来源：http://esz.jlsjyb.cn

Py:   arr.index(x);  x in arr
来源：http://xqg.wangshuangyany.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hmu.bjfxy.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hxv.zhongyouzk.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lip.zhaomingkeji.xyz

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://caq.tian-w.cn

Go:   slices.Index(arr, x)
来源：http://nge.tanke756.top

Ruby: arr.index(x)
来源：http://elb.vehdjk.com

C#:   list.IndexOf(x);
来源：http://nmi.chenjidiqi.icu

[D13] 过滤（保留满足条件的）
来源：http://aio.wangshuangyany.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ytx.wangdashe.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://dhw.nwbrower.top

JS:   arr.filter(x => x > 3)
来源：http://ilt.xingfuxueyuan.xyz

TS:   arr.filter(x => x > 3)
来源：http://zsb.zhongyouzk.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://gix.cashguo.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://pfb.jinqigfzy.top

Ruby: arr.select { |x| x > 3 }
来源：http://ngx.chenlongwang.top

C#:   list.Where(x => x > 3).ToList()
来源：http://avm.cqqwz.cn

[D14] 映射转换（每个元素变形）
来源：http://rov.hnqzz.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ogw.xingfuxueyuan.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://kdf.yuxming.cn

JS:   arr.map(x => x * 2)
来源：http://fyg.bjfxy.top

TS:   arr.map(x => x * 2)
来源：http://rts.fzhhl.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://npx.ybcxt.top

Go:   // 手写循环
来源：http://ynm.jqgufenzy.top

Ruby: arr.map { |x| x * 2 }
来源：http://awc.jinqigfzy.top

C#:   list.Select(x => x * 2).ToList()
来源：http://deg.zdqjudy.top

[D15] 去重
来源：http://sij.feifeiyinyue.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://sbn.chenlongwang.top

PHP:  array_unique($arr);
来源：http://sde.cheryme.top

JS:   [...new Set(arr)]
来源：http://gsz.fengsongda.top

TS:   [...new Set(arr)]
来源：http://zad.cashguo.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://yhm.mhx1999.top

Go:   // 用 map[T]struct{} 手写
来源：http://kqb.hnxiangtu.top

Ruby: arr.uniq
来源：http://fff.zhengqikj.top

C#:   list.Distinct().ToList()
来源：http://jad.fehbvm.com

[D16] 求和与平均值
来源：http://nmp.hongshengwenyu.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ptp.epnwcf.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://btc.xinyue.icu

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://rxj.ppjwa.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://yec.xingfuxueyuan.xyz

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://boe.zdqjudy.top

Go:   // 手写循环累加
来源：http://trc.dashuyun.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ieb.svipenyu.cn

C#:   list.Sum();  list.Average()
来源：http://wgx.chenjidiqi.icu

[D17] 最大值与最小值
来源：http://yho.jinqigufen.top

Py:   max(arr);  min(arr)
来源：http://tkm.yuxming.cn

PHP:  max($arr);  min($arr);
来源：http://hzx.jyoumei.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://nbp.redwolf501.top

TS:   Math.max(...arr);
来源：http://bra.gzhubu.top

Java: Collections.max(list);  Collections.min(list);
来源：http://ubo.svipenyu.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://tla.quarkkingdee.top

Ruby: arr.max;  arr.min
来源：http://tcs.cqqwz.cn

C#:   list.Max();  list.Min()
来源：http://avi.hesvh.cn

[D18] 扁平化嵌套数组
来源：http://hwq.jlsjyb.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://odz.gotoacloud.top

PHP:  array_merge(...$nested);
来源：http://bmm.fanxiaobao.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://xru.dianchejie.cn

TS:   nested.flat();
来源：http://gqh.kuanghao11.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jhz.cdnleiting.top

Go:   // 手写双层循环
来源：http://jou.redwolf501.top

Ruby: nested.flatten
来源：http://xbg.c1oappe.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://cep.316326.xyz

[D19] 按字段分组
来源：http://zze.andypj.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://qir.jqgufenzy.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://fta.ywan-chungtsiang.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://apu.kuanghao11.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://zah.zycfv.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mrn.daria6918.cn

Go:   // 手写 map[string][]T
来源：http://zax.xuetiantiany.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://pka.dashuyun.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://fwa.ivvv.top

[D20] 统计每个元素出现次数
来源：http://xlk.tanke756.top

Py:   Counter(arr)
来源：http://pbg.chenzaomai.com

PHP:  array_count_values($arr);
来源：http://lcx.shanyushiyangkeji.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zxg.hnxiangtu.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bng.hnqzz.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://nzs.quarkkingdee.top

Go:   // 手写 map[T]int
来源：http://pcc.nanxuanxn.top

Ruby: arr.tally
来源：http://qyw.dianchejie.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://olj.redwolf501.top

[D21] 判断是否包含某元素
来源：http://hri.shanyushiyangtech.top

Py:   x in arr
来源：http://owy.xziqi.cn

PHP:  in_array($x, $arr, true);
来源：http://ggk.jyoumei.cn

JS:   arr.includes(x)
来源：http://vcu.zhaomingkeji.xyz

TS:   arr.includes(x)
来源：http://inp.uphjek.com

Java: list.contains(x)
来源：http://xhm.jinyuanbaomall.cn

Go:   slices.Contains(arr, x)
来源：http://usr.nanxinkj.top

Ruby: arr.include?(x)
来源：http://klw.52xcode.cn

C#:   list.Contains(x)
来源：http://kzv.bjfxy.top

[D22] 复制数组（避免共享引用）
来源：http://hbc.zdqjudy.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ork.yueranfly.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://urp.zhixingplan.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://gop.shangyingyoupin.top

TS:   [...arr];
来源：http://ibe.tian-w.cn

Java: new ArrayList<>(list);
来源：http://ijl.sjlbkw.cn

Go:   copied := append([]int(nil), arr...)
来源：http://eyj.ehwqpu.com

Ruby: arr.dup;  arr.clone
来源：http://rai.chenjidiqi.icu

C#:   new List<int>(list);
来源：http://xyd.316326.xyz

[D23] reduce 累积计算
来源：http://bwx.aibaodan.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://pal.gogol.net.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://oiv.gzhubu.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lxe.cashguo.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ilv.ivvv.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://djb.yuxming.cn

Go:   // 手写循环
来源：http://gsd.yj20258888.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wpo.yvedp.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://rbo.ydjk.org.cn

[D24] 字典 / Map 基本操作
来源：http://mrz.guannengcc.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://bun.yuxming.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://yfl.hysaishi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://abo.ywan-chungtsiang.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mjq.shzxlz.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wek.shanyushiyangtech.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wro.fanxiaobao.xyz

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://lqv.yangfankeji.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://vti.yongpay.top

[D25] Set 集合去重与交并差
来源：http://njx.zhoulong.xyz

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mgm.xylfe.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://cjr.jlsjyb.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://zjg.316326.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://sfl.vehdjk.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://kws.sysykeji.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://kag.pycfn.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hmc.sufxvd.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://vhs.gogol.net.cn

[D26] 数组转字符串
来源：http://emd.xuanzx.com


<!-- 参考信息 -->