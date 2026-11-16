代发 wailian999

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://umj.pengpengdd.cyou

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://skh.jianghu66.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://tlr.yvedp.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://fzd.fzhhl.top

[C10] 变量作用域
来源：http://ugr.jianghu66.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ree.daria6918.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wgn.ybcxt.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://yit.uphjek.com

TS:   同 JS
来源：http://iju.haohaochexian.top

Java: 方法内为块级作用域
来源：http://kci.shzxlz.cn

Go:   花括号块级作用域
来源：http://fls.jlsjyb.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://rez.cucudq.cn

C#:   块级作用域
来源：http://sns.hongshengwenyu.top

[C11] 模块导入与导出
来源：http://eoa.ppjwa.cn

Py:   from module import func
来源：http://hvf.shzxlz.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://mrw.316326.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://nsk.yonumen.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://szd.jianghu66.top

Java: import java.util.List;
来源：http://pcq.zhaomingkeji.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://msu.fanxiaobao.xyz

Ruby: require "json"; require_relative "./util"
来源：http://odd.zhongyouzk.top

C#:   using System.Text;
来源：http://tkd.xinyue.icu

[C12] 立即执行函数 IIFE
来源：http://rst.gotoacloud.top

Py:   (lambda: print("run"))()
来源：http://sws.jiagoushi.top

PHP:  (function () { echo "run"; })();
来源：http://poy.xingfuxueyuan.xyz

JS:   (() => { console.log("run"); })();
来源：http://cqp.yuxming.cn

TS:   (() => { console.log("run"); })();
来源：http://xdc.sysykeji.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wrb.aizwys.cn

Go:   func() { fmt.Println("run") }()
来源：http://qhg.hcnkem.com

Ruby: -> { puts "run" }.call
来源：http://bmz.yuanzhike.top

C#:   // 无 IIFE：用静态构造函数
来源：http://vel.pengpengdd.cyou

[C13] 类型声明 / 类型注解
来源：http://gdi.zhixingplan.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://rfi.9152youxi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pol.dashuyun.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://dwx.yangfankeji.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jiw.ivvv.top

Java: int add(int a, int b) { return a + b; }
来源：http://bna.tian-w.cn

Go:   func add(a, b int) int
来源：http://cpp.shanyushiyangkeji.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://nrk.xingfuxueyuan.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://lxj.jqgfzy.top

[C14] 泛型函数
来源：http://zdc.yj20258.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://kib.316326.xyz

PHP:  // 无泛型
来源：http://qym.ctjpmb.com

JS:   // 无泛型
来源：http://ywn.yj20258888.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://pbo.xinyue.icu

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://gss.yfazqb.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://rcl.xuanzx.com

Ruby: # 无泛型
来源：http://izs.yueranfly.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://peu.jinqigufen.top

[C15] 解构 / 展开参数
来源：http://pyr.vehdjk.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://pww.chenzaomai.com

PHP:  [$a, $b] = $pair;
来源：http://lvd.yj202588.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://brw.yvedp.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://upc.smart0.xyz

Java: // 无解构
来源：http://wje.vehdjk.com

Go:   // 无解构
来源：http://zoy.vqdsnc.cn

Ruby: a, b = pair
来源：http://uzr.feifeiyinyue.top

C#:   var (a, b) = pair;
来源：http://lfa.jianghu66.top

[C16] 函数 / 方法重载
来源：http://gzc.aibaodan.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://jwx.zhijiandao.cn

PHP:  // 无重载
来源：http://rhq.hcnkem.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://dnl.kuanghao11.cn

TS:   // 用联合类型或重载签名声明
来源：http://yux.jlsjyb.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://agc.nwbrower.top

Go:   // 无重载：用不同函数名
来源：http://ium.smart0.xyz

Ruby: # 无重载：靠动态参数
来源：http://kir.xziqi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://eqa.tianlin.xyz

================================================================================
来源：http://xru.ivvv.top

D. 数组 / 列表 / 集合
来源：http://ded.yangfankeji.com

================================================================================
来源：http://rsw.quarkkingdee.top

[D01] 创建数组 / 列表
来源：http://xse.cucudq.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ywt.yueranfly.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://xts.smart0.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ogj.jyoumei.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://vvq.316326.xyz

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://eyf.cheryme.top

Go:   arr := []int{1, 2, 3}
来源：http://mdj.cashguo.top

Ruby: arr = [1, 2, 3]
来源：http://csb.tanke756.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://dhh.chenjidiqi.icu

[D02] 追加元素到末尾
来源：http://rit.jianghu66.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://upf.cheryme.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://fre.nanxuanxn.top

JS:   arr.push(4);
来源：http://lup.zhaomingkeji.xyz

TS:   arr.push(4);
来源：http://rab.shangyingyoupin.top

Java: list.add(4);
来源：http://ysn.zhengqikj.top

Go:   arr = append(arr, 4)
来源：http://mua.bbcook.cn

Ruby: arr << 4; arr.push(5)
来源：http://jdy.daxiang520.top

C#:   list.Add(4);
来源：http://bmg.hnxiangtu.top

[D03] 在指定位置插入元素
来源：http://rfa.kuanghao11.cn

Py:   arr.insert(0, 0)
来源：http://ioy.xylfe.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://nab.vqdsnc.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ajb.jyoumei.cn

TS:   arr.splice(0, 0, 0);
来源：http://uns.chenlongwang.top

Java: list.add(0, 0);
来源：http://ese.cheryme.top

Go:   arr = append([]int{0}, arr...)
来源：http://hpq.316326.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wvg.hcnkem.com

C#:   list.Insert(0, 0);
来源：http://sqk.chenlongwang.top

[D04] 删除元素
来源：http://nzd.wangshuangyany.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://its.gogol.net.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://smu.vqdsnc.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://csf.wangdashe.top

TS:   arr.splice(0, 1);
来源：http://iyr.zhengqikj.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://fur.wangdashe.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://won.jinghuilouyu.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hkh.vehdjk.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://zsm.yanxiufei.cn

[D05] 访问与修改元素
来源：http://zpp.jinqigfzy.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://kmd.jlsjyb.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://sfm.daria6918.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://haw.316326.xyz

TS:   arr[0]; arr.at(-1);
来源：http://jlp.chenjidiqi.icu

Java: list.get(0); list.set(0, 9);
来源：http://hzs.xinyue.icu

Go:   arr[0]; arr[0] = 9
来源：http://doa.quarkkingdee.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://gmc.daria6918.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://lnj.daxiang520.top

[D06] 数组长度
来源：http://nze.yfazqb.com

Py:   len(arr)
来源：http://qdk.bbcook.cn

PHP:  count($arr);
来源：http://axi.hysaishi.cn

JS:   arr.length
来源：http://nuy.jinyuanbaomall.cn

TS:   arr.length
来源：http://jnw.gzhubu.top

Java: list.size();
来源：http://kkx.hfpthk.cn

Go:   len(arr)
来源：http://bpj.sjlbkw.cn

Ruby: arr.length; arr.size
来源：http://ven.yongpay.top

C#:   list.Count;
来源：http://nex.gogol.net.cn

[D07] 切片 / 取子数组
来源：http://vct.svipenyu.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://fly.yanxiufei.cn

PHP:  array_slice($arr, 1, 3);
来源：http://pke.52xcode.cn

JS:   arr.slice(1, 4);
来源：http://jse.yangfankeji.com

TS:   arr.slice(1, 4);
来源：http://ihf.quarkkingdee.top

Java: list.subList(1, 4);
来源：http://wzb.vehdjk.com

Go:   arr[1:4]
来源：http://ihw.kuanghao11.cn

Ruby: arr[1, 3]
来源：http://ezg.quarkkingdee.top

C#:   list.GetRange(1, 3);
来源：http://nxk.quarkkingdee.top

[D08] 合并两个数组
来源：http://sop.hammf.cn

Py:   a + b;  a.extend(b)
来源：http://rst.gotoacloud.top

PHP:  array_merge($a, $b);
来源：http://ukr.aibaodan.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://zbi.xuanzx.com

TS:   [...a, ...b];
来源：http://hgu.chenjidiqi.icu

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://nes.cdnleiting.top

Go:   append(a, b...)
来源：http://enq.jinyuanbaomall.cn

Ruby: a + b;  a.concat(b)
来源：http://pyq.cucudq.cn

C#:   a.Concat(b).ToList()
来源：http://qoo.yuanzhike.top

[D09] 排序（升序）
来源：http://nzn.xuanzx.com

Py:   sorted(arr);  arr.sort()
来源：http://glc.ctjpmb.com

PHP:  sort($arr);
来源：http://wbl.hfpthk.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://rfc.cqqwz.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://okd.zdbjq.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://mmv.yanxiufei.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qya.shzxlz.cn

Ruby: arr.sort
来源：http://rkz.ybcxt.top

C#:   list.Sort();
来源：http://usi.tarul.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://qou.guannengcc.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://asp.sweek.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mdt.gaohongyu789.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://uze.iojbl.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://qfy.hammf.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://gsj.pycfn.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://rjb.zdqjudy.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://kuz.shzxlz.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qgp.cdnleiting.top

[D11] 反转数组
来源：http://jvk.yfazqb.com

Py:   arr[::-1];  arr.reverse()
来源：http://jwh.shanyushiyangkeji.top

PHP:  array_reverse($arr);
来源：http://hhw.xziqi.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ale.shangyingyoupin.top

TS:   [...arr].reverse();
来源：http://gpv.hnxiangtu.top

Java: Collections.reverse(list);
来源：http://adg.shuidangran.top

Go:   slices.Reverse(arr)
来源：http://gdj.andypj.xyz

Ruby: arr.reverse
来源：http://uzw.hcnkem.com

C#:   list.Reverse();
来源：http://wdw.jiagoushi.top

[D12] 查找元素下标
来源：http://kga.jqgfzy.top

Py:   arr.index(x);  x in arr
来源：http://ezc.birdmap.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://gnt.bjfxy.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bzj.hywenlv.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kan.ybcxt.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://cbl.c1oappe.top

Go:   slices.Index(arr, x)
来源：http://lcn.fzhhl.top

Ruby: arr.index(x)
来源：http://woq.guannengcc.top

C#:   list.IndexOf(x);
来源：http://loi.jlsjyb.cn

[D13] 过滤（保留满足条件的）
来源：http://prt.jinqigfzy.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://thd.zhaomingkeji.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ruw.daxiang520.top

JS:   arr.filter(x => x > 3)
来源：http://hpt.hesvh.cn

TS:   arr.filter(x => x > 3)
来源：http://yud.birdmap.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://eka.guowangkeji.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ghv.tanke756.top

Ruby: arr.select { |x| x > 3 }
来源：http://gci.tanke756.top

C#:   list.Where(x => x > 3).ToList()
来源：http://vgc.ybcxt.top

[D14] 映射转换（每个元素变形）
来源：http://hwh.jiagoushi.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://bsp.svipenyu.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mop.xziqi.cn

JS:   arr.map(x => x * 2)
来源：http://jas.sufxvd.cn

TS:   arr.map(x => x * 2)
来源：http://wsy.chenlongwang.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://jum.yfazqb.com

Go:   // 手写循环
来源：http://kqd.sufxvd.cn

Ruby: arr.map { |x| x * 2 }
来源：http://tvp.zycfv.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://jzl.shuidangran.top

[D15] 去重
来源：http://fik.cashguo.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://lzp.snrcjt.cn

PHP:  array_unique($arr);
来源：http://qrl.jqgufenzy.top

JS:   [...new Set(arr)]
来源：http://pva.zhixingplan.top

TS:   [...new Set(arr)]
来源：http://lkz.fzhhl.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hbd.shanyushiyangkeji.top

Go:   // 用 map[T]struct{} 手写
来源：http://usg.aizwys.cn

Ruby: arr.uniq
来源：http://bix.vehdjk.com

C#:   list.Distinct().ToList()
来源：http://jjj.jinghuilouyu.cn

[D16] 求和与平均值
来源：http://tsr.zhongyouzk.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hmb.zhixingplan.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://dsb.shanyushiyangkeji.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://xsh.jinyuanbaomall.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://tmw.yfazqb.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://cjv.sweek.top

Go:   // 手写循环累加
来源：http://cpg.jinyuanbaomall.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://rzs.shuidangran.top

C#:   list.Sum();  list.Average()
来源：http://xqd.cheryme.top

[D17] 最大值与最小值
来源：http://qsr.yonumen.top

Py:   max(arr);  min(arr)
来源：http://hje.52xcode.cn

PHP:  max($arr);  min($arr);
来源：http://tnb.cdnleiting.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ywn.wangshuangyany.cn

TS:   Math.max(...arr);
来源：http://qcx.zhixingplan.top

Java: Collections.max(list);  Collections.min(list);
来源：http://fiw.zhoulong.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mcc.birdmap.top

Ruby: arr.max;  arr.min
来源：http://lfy.mhx1999.top

C#:   list.Max();  list.Min()
来源：http://wqy.nwbrower.top

[D18] 扁平化嵌套数组
来源：http://nja.feifeiyinyue.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://pnj.yj20258.top

PHP:  array_merge(...$nested);
来源：http://noh.tian-w.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://fvi.havefunace.top

TS:   nested.flat();
来源：http://ueb.yj202588.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://cnv.uphjek.com

Go:   // 手写双层循环
来源：http://jtl.jinqigfzy.top

Ruby: nested.flatten
来源：http://rpt.smart0.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://uip.gzhubu.top

[D19] 按字段分组
来源：http://ytp.xinyue.icu

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://iyx.hnqzz.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://fmc.yj20258.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://acx.gogol.net.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://sty.zhongyouzk.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://vrq.aizwys.cn

Go:   // 手写 map[string][]T
来源：http://lqj.ywan-chungtsiang.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://ouv.uphjek.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://agn.yj202588.top

[D20] 统计每个元素出现次数
来源：http://dqx.cheryme.top

Py:   Counter(arr)
来源：http://mhu.tianlin.xyz

PHP:  array_count_values($arr);
来源：http://wgh.yj20258.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ojv.jyoumei.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://epo.mhx1999.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://gye.mhx1999.top

Go:   // 手写 map[T]int
来源：http://ycr.cheryme.top

Ruby: arr.tally
来源：http://ill.jinghuilouyu.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://oqp.jyoumei.cn

[D21] 判断是否包含某元素
来源：http://kbv.sjlbkw.cn

Py:   x in arr
来源：http://fuj.shanyushiyangkeji.top

PHP:  in_array($x, $arr, true);
来源：http://psw.shzxlz.cn

JS:   arr.includes(x)
来源：http://gkx.ehwqpu.com

TS:   arr.includes(x)
来源：http://idt.wangdashe.top

Java: list.contains(x)
来源：http://tlm.andypj.xyz

Go:   slices.Contains(arr, x)
来源：http://riv.svipenyu.cn

Ruby: arr.include?(x)
来源：http://obg.zhaomingkeji.xyz

C#:   list.Contains(x)
来源：http://pfv.daria6918.cn

[D22] 复制数组（避免共享引用）
来源：http://hvt.tarul.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hjc.iojbl.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://kae.jlsjyb.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://tfj.xingfuxueyuan.xyz

TS:   [...arr];
来源：http://ouj.zhoulong.xyz

Java: new ArrayList<>(list);
来源：http://sbt.yuxming.cn

Go:   copied := append([]int(nil), arr...)
来源：http://nux.tian-w.cn

Ruby: arr.dup;  arr.clone
来源：http://teu.sjlbkw.cn

C#:   new List<int>(list);
来源：http://hpj.svipenyu.cn

[D23] reduce 累积计算
来源：http://oxh.c1oappe.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hxp.ctjpmb.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ilm.jianghu66.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rof.dashuyun.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kiu.haohaochexian.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://amr.yj202588.top

Go:   // 手写循环
来源：http://uuh.tian-w.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://qox.yj20258888.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://jjp.shanyushiyangkeji.top

[D24] 字典 / Map 基本操作
来源：http://imc.andypj.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://fiq.shanyushiyangkeji.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hvo.shanyushiyangtech.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://tus.zhongyouzk.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mzk.jqgfzy.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ixh.nanxinkj.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://jnx.gotoacloud.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://oyi.zhijiandao.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://inw.bjfxy.top

[D25] Set 集合去重与交并差
来源：http://qvc.ehwqpu.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://xec.yuxming.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://knk.xinyue.icu

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://avj.yuxming.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://plw.ybcxt.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://gus.nwbrower.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://gbh.yuxming.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://lyu.cheryme.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://nkl.wangshuangyany.cn

[D26] 数组转字符串
来源：http://zpa.shzxlz.cn

Py:   ", ".join(map(str, arr))
来源：http://ymw.guannengcc.top

PHP:  implode(", ", $arr);
来源：http://ibi.yvedp.cn

JS:   arr.join(", ")
来源：http://pvr.jianghu66.top

TS:   arr.join(", ")
来源：http://ilu.zycfv.cn


<!-- 参考信息 -->