代发 wailian999

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://uwl.wangdashe.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://zbe.fktsv.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://sne.shzxlz.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wmg.gotoacloud.top

[C10] 变量作用域
来源：http://tqa.zycfv.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mwk.gaohongyu789.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://jxf.nanxuanxn.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mts.uphjek.com

TS:   同 JS
来源：http://knr.svipenyu.cn

Java: 方法内为块级作用域
来源：http://ggy.ehwqpu.com

Go:   花括号块级作用域
来源：http://cis.yfazqb.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://epn.yongpay.top

C#:   块级作用域
来源：http://qqe.zdbjq.cn

[C11] 模块导入与导出
来源：http://tib.xingfuxueyuan.xyz

Py:   from module import func
来源：http://npq.gotoacloud.top

PHP:  require "file.php";  或 use App\Service;
来源：http://pcy.fanxiaobao.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://tsr.fanxiaobao.xyz

TS:   export function f(): void {};  import { f } from "./m";
来源：http://eeq.sysykeji.top

Java: import java.util.List;
来源：http://ftj.yongpay.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://vmv.cucudq.cn

Ruby: require "json"; require_relative "./util"
来源：http://hox.xziqi.cn

C#:   using System.Text;
来源：http://bba.cucudq.cn

[C12] 立即执行函数 IIFE
来源：http://mgm.yangfankeji.com

Py:   (lambda: print("run"))()
来源：http://glb.yfazqb.com

PHP:  (function () { echo "run"; })();
来源：http://ote.shanyushiyangtech.top

JS:   (() => { console.log("run"); })();
来源：http://lbd.yanxiufei.cn

TS:   (() => { console.log("run"); })();
来源：http://cmi.shuidangran.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://xuy.xylfe.cn

Go:   func() { fmt.Println("run") }()
来源：http://cse.ehwqpu.com

Ruby: -> { puts "run" }.call
来源：http://wvs.hcnkem.com

C#:   // 无 IIFE：用静态构造函数
来源：http://npu.chenlongwang.top

[C13] 类型声明 / 类型注解
来源：http://cnv.zhoulong.xyz

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://fes.bbcook.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hgd.nanxinkj.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://lmp.xuetiantiany.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bjm.shanyushiyangtech.top

Java: int add(int a, int b) { return a + b; }
来源：http://lid.cdnleiting.top

Go:   func add(a, b int) int
来源：http://ztz.fktsv.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mfe.xinyue.icu

C#:   int Add(int a, int b) => a + b;
来源：http://bdz.shuidangran.top

[C14] 泛型函数
来源：http://hof.yongpay.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zqg.yvedp.cn

PHP:  // 无泛型
来源：http://aje.sweek.top

JS:   // 无泛型
来源：http://rdr.dashuyun.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mfe.316326.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://xii.9152youxi.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mii.ehwqpu.com

Ruby: # 无泛型
来源：http://rkn.sjlbkw.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ieb.xuetiantiany.cn

[C15] 解构 / 展开参数
来源：http://tbx.zdbjq.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://orl.fehbvm.com

PHP:  [$a, $b] = $pair;
来源：http://lud.sxryk.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ibw.gotoacloud.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://qek.cheryme.top

Java: // 无解构
来源：http://evv.zhijiandao.cn

Go:   // 无解构
来源：http://yny.sweek.top

Ruby: a, b = pair
来源：http://iix.epnwcf.com

C#:   var (a, b) = pair;
来源：http://irg.chenzaomai.com

[C16] 函数 / 方法重载
来源：http://liy.cashguo.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://sef.ctjpmb.com

PHP:  // 无重载
来源：http://idi.wangdashe.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://whr.zhengqikj.top

TS:   // 用联合类型或重载签名声明
来源：http://zum.vqdsnc.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://lkv.ppjwa.cn

Go:   // 无重载：用不同函数名
来源：http://jkb.fktsv.cn

Ruby: # 无重载：靠动态参数
来源：http://zhr.sweek.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://qav.sjlbkw.cn

================================================================================
来源：http://wmr.zhaomingkeji.xyz

D. 数组 / 列表 / 集合
来源：http://fft.ydjk.org.cn

================================================================================
来源：http://dfv.xylfe.cn

[D01] 创建数组 / 列表
来源：http://dbx.yonumen.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://fnn.52xcode.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://gfp.chenjidiqi.icu

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://xwm.tarul.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://hcv.nanxuanxn.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://iyy.fehbvm.com

Go:   arr := []int{1, 2, 3}
来源：http://bho.yvedp.cn

Ruby: arr = [1, 2, 3]
来源：http://qud.guannengcc.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://fgx.yj20258888.top

[D02] 追加元素到末尾
来源：http://ekg.tianlin.xyz

Py:   arr.append(4); arr.extend([5, 6])
来源：http://fkb.wangdashe.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://lxa.tarul.cn

JS:   arr.push(4);
来源：http://jyr.feifeiyinyue.top

TS:   arr.push(4);
来源：http://xxz.nanxuanxn.top

Java: list.add(4);
来源：http://nlp.ivvv.top

Go:   arr = append(arr, 4)
来源：http://ata.kuanghao11.cn

Ruby: arr << 4; arr.push(5)
来源：http://mkj.jianghu66.top

C#:   list.Add(4);
来源：http://wnb.meibo888.top

[D03] 在指定位置插入元素
来源：http://mut.yj20258.top

Py:   arr.insert(0, 0)
来源：http://jjj.jinyuanbaomall.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://sym.chenzaomai.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://tyj.cdnleiting.top

TS:   arr.splice(0, 0, 0);
来源：http://hej.yonumen.top

Java: list.add(0, 0);
来源：http://fbo.cucudq.cn

Go:   arr = append([]int{0}, arr...)
来源：http://heb.zhongyouzk.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://cro.cdnleiting.top

C#:   list.Insert(0, 0);
来源：http://zph.cashguo.top

[D04] 删除元素
来源：http://qbd.sysykeji.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://fak.jinqigfzy.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://aok.sufxvd.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ixu.snrcjt.cn

TS:   arr.splice(0, 1);
来源：http://awm.xziqi.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://qvs.yuanzhike.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://uni.shzxlz.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ata.vehdjk.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://cud.zhixingplan.top

[D05] 访问与修改元素
来源：http://oar.xylfe.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://xrx.ctjpmb.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://xhv.xuetiantiany.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://xtf.jiagoushi.top

TS:   arr[0]; arr.at(-1);
来源：http://eed.hnxiangtu.top

Java: list.get(0); list.set(0, 9);
来源：http://lhv.sweek.top

Go:   arr[0]; arr[0] = 9
来源：http://lwd.sxryk.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://vrf.gotoacloud.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://xld.jqgufenzy.top

[D06] 数组长度
来源：http://fxg.9152youxi.cn

Py:   len(arr)
来源：http://lup.0kj1m.cn

PHP:  count($arr);
来源：http://zkz.shzxlz.cn

JS:   arr.length
来源：http://rgw.gzhubu.top

TS:   arr.length
来源：http://lff.vqdsnc.cn

Java: list.size();
来源：http://jrr.jinyuanbaomall.cn

Go:   len(arr)
来源：http://owp.zdbjq.cn

Ruby: arr.length; arr.size
来源：http://eml.dashuyun.cn

C#:   list.Count;
来源：http://pbh.pycfn.com

[D07] 切片 / 取子数组
来源：http://kid.smart0.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://xya.zdqjudy.top

PHP:  array_slice($arr, 1, 3);
来源：http://ztb.hnxiangtu.top

JS:   arr.slice(1, 4);
来源：http://dpt.gzhubu.top

TS:   arr.slice(1, 4);
来源：http://cta.9152youxi.cn

Java: list.subList(1, 4);
来源：http://yzf.jqgfzy.top

Go:   arr[1:4]
来源：http://syl.birdmap.top

Ruby: arr[1, 3]
来源：http://bwt.guowangkeji.top

C#:   list.GetRange(1, 3);
来源：http://zgg.cashguo.top

[D08] 合并两个数组
来源：http://ijo.quarkkingdee.top

Py:   a + b;  a.extend(b)
来源：http://tay.yuanzhike.top

PHP:  array_merge($a, $b);
来源：http://vqi.hfpthk.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://lsl.nwbrower.top

TS:   [...a, ...b];
来源：http://kbt.aizwys.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ths.ybcxt.top

Go:   append(a, b...)
来源：http://gea.zdqjudy.top

Ruby: a + b;  a.concat(b)
来源：http://xtr.vehdjk.com

C#:   a.Concat(b).ToList()
来源：http://okb.shanyushiyangtech.top

[D09] 排序（升序）
来源：http://ykd.guowangkeji.top

Py:   sorted(arr);  arr.sort()
来源：http://cch.ppjwa.cn

PHP:  sort($arr);
来源：http://uuk.yuanzhike.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hky.zdbjq.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://bxe.chenzaomai.com

Java: Collections.sort(list);  list.sort(null);
来源：http://whj.jinqigfzy.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ndg.316326.xyz

Ruby: arr.sort
来源：http://jfp.zhijiandao.cn

C#:   list.Sort();
来源：http://phy.xuanzx.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://aiy.hammf.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://lpi.sweek.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lgp.wangdashe.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://vbv.ydzc1.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mka.quarkkingdee.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://btu.shuidangran.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://upi.316326.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://pim.316326.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hgl.ctjpmb.com

[D11] 反转数组
来源：http://vet.yj20258888.top

Py:   arr[::-1];  arr.reverse()
来源：http://afk.hcnkem.com

PHP:  array_reverse($arr);
来源：http://rda.epnwcf.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://gcb.shanyushiyangtech.top

TS:   [...arr].reverse();
来源：http://tgd.shangyingyoupin.top

Java: Collections.reverse(list);
来源：http://mzs.jinyuanbaomall.cn

Go:   slices.Reverse(arr)
来源：http://ikl.ivvv.top

Ruby: arr.reverse
来源：http://xip.ivvv.top

C#:   list.Reverse();
来源：http://fkx.fehbvm.com

[D12] 查找元素下标
来源：http://cbj.xziqi.cn

Py:   arr.index(x);  x in arr
来源：http://rlc.hnqzz.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://usz.yonumen.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fps.hesvh.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zze.jqgfzy.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://yvy.xuanzx.com

Go:   slices.Index(arr, x)
来源：http://qls.svipenyu.cn

Ruby: arr.index(x)
来源：http://rul.chenjidiqi.icu

C#:   list.IndexOf(x);
来源：http://uha.meibo888.top

[D13] 过滤（保留满足条件的）
来源：http://hxi.yvedp.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://cjd.chenjidiqi.icu

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://fum.dianchejie.cn

JS:   arr.filter(x => x > 3)
来源：http://joi.tianlin.xyz

TS:   arr.filter(x => x > 3)
来源：http://hen.mhx1999.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://xua.dianchejie.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://pqk.hcnkem.com

Ruby: arr.select { |x| x > 3 }
来源：http://gbd.fehbvm.com

C#:   list.Where(x => x > 3).ToList()
来源：http://ykn.nwbrower.top

[D14] 映射转换（每个元素变形）
来源：http://afh.chenzaomai.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://dfd.redwolf501.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://uju.sysykeji.top

JS:   arr.map(x => x * 2)
来源：http://ruw.xingfuxueyuan.xyz

TS:   arr.map(x => x * 2)
来源：http://udk.yj202588.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://hpy.smart0.xyz

Go:   // 手写循环
来源：http://fbf.yvedp.cn

Ruby: arr.map { |x| x * 2 }
来源：http://hyz.uphjek.com

C#:   list.Select(x => x * 2).ToList()
来源：http://fkv.feifeiyinyue.top

[D15] 去重
来源：http://rdn.daxiang520.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mka.nanxuanxn.top

PHP:  array_unique($arr);
来源：http://axv.shzxlz.cn

JS:   [...new Set(arr)]
来源：http://krk.jianghu66.top

TS:   [...new Set(arr)]
来源：http://uvl.nanxuanxn.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ywz.guowangkeji.top

Go:   // 用 map[T]struct{} 手写
来源：http://ioy.daria6918.cn

Ruby: arr.uniq
来源：http://moe.wangshuangyany.cn

C#:   list.Distinct().ToList()
来源：http://dba.9152youxi.cn

[D16] 求和与平均值
来源：http://rbm.xinyue.icu

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://cyg.zhongyouzk.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://pjc.xingfuxueyuan.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://viy.zdbjq.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://iso.zdqjudy.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://qoo.zdbjq.cn

Go:   // 手写循环累加
来源：http://uns.hongshengwenyu.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://utl.yuxming.cn

C#:   list.Sum();  list.Average()
来源：http://onj.hysaishi.cn

[D17] 最大值与最小值
来源：http://xwm.snrcjt.cn

Py:   max(arr);  min(arr)
来源：http://nfr.fzhhl.top

PHP:  max($arr);  min($arr);
来源：http://edi.ydzc1.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ikc.feifeiyinyue.top

TS:   Math.max(...arr);
来源：http://fxd.hysaishi.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://tlc.havefunace.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ino.sweek.top

Ruby: arr.max;  arr.min
来源：http://bxz.andypj.xyz

C#:   list.Max();  list.Min()
来源：http://btq.zhiwuduotai.top

[D18] 扁平化嵌套数组
来源：http://oto.zhongyouzk.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://vca.52xcode.cn

PHP:  array_merge(...$nested);
来源：http://ral.ybcxt.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mta.yj20258888.top

TS:   nested.flat();
来源：http://pgt.xuanzx.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://cop.pengpengdd.cyou

Go:   // 手写双层循环
来源：http://ahe.guowangkeji.top

Ruby: nested.flatten
来源：http://pmh.tianlin.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://zai.feifeiyinyue.top

[D19] 按字段分组
来源：http://fmq.snrcjt.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://zih.hfpthk.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://skz.dashuyun.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qkz.sufxvd.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://fsi.wangdashe.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wcb.yj20258.top

Go:   // 手写 map[string][]T
来源：http://hpv.gotoacloud.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://swm.0kj1m.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ysz.xinyue.icu

[D20] 统计每个元素出现次数
来源：http://hcl.hesvh.cn

Py:   Counter(arr)
来源：http://gdr.epnwcf.com

PHP:  array_count_values($arr);
来源：http://kfz.dianchejie.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://iyo.tanke756.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ntr.ppjwa.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ckd.ivvv.top

Go:   // 手写 map[T]int
来源：http://jwo.hywenlv.cn

Ruby: arr.tally
来源：http://vlc.gaohongyu789.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://lgw.tanke756.top

[D21] 判断是否包含某元素
来源：http://tsp.yuxming.cn

Py:   x in arr
来源：http://cmy.nwbrower.top

PHP:  in_array($x, $arr, true);
来源：http://gfe.cqqwz.cn

JS:   arr.includes(x)
来源：http://auq.shanyushiyangtech.top

TS:   arr.includes(x)
来源：http://bco.havefunace.top

Java: list.contains(x)
来源：http://fwv.bjfxy.top

Go:   slices.Contains(arr, x)
来源：http://nfm.jinqigufen.top

Ruby: arr.include?(x)
来源：http://ewb.havefunace.top

C#:   list.Contains(x)
来源：http://zyy.gaohongyu789.top

[D22] 复制数组（避免共享引用）
来源：http://ckc.xziqi.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://pra.nanxuanxn.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://kkw.cdnleiting.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://pju.tanke756.top

TS:   [...arr];
来源：http://sml.ybcxt.top

Java: new ArrayList<>(list);
来源：http://zid.hnqzz.top

Go:   copied := append([]int(nil), arr...)
来源：http://nkn.yangfankeji.com

Ruby: arr.dup;  arr.clone
来源：http://rpv.zhaomingkeji.xyz

C#:   new List<int>(list);
来源：http://lwj.daxiang520.top

[D23] reduce 累积计算
来源：http://jmv.fehbvm.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://xcr.andypj.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://gtd.xuetiantiany.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://asy.shangyingyoupin.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ozv.ydjk.org.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ihw.chenzaomai.com

Go:   // 手写循环
来源：http://prc.zhixingplan.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ryg.tarul.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://app.guannengcc.top

[D24] 字典 / Map 基本操作
来源：http://pxg.tian-w.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mqs.yangfankeji.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ftq.hnqzz.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mkx.gotoacloud.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ayf.fanxiaobao.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://izn.shanyushiyangtech.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://uol.jinqigfzy.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mnk.fehbvm.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://jly.xingfuxueyuan.xyz

[D25] Set 集合去重与交并差
来源：http://fci.ydzc1.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://bcw.gotoacloud.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://prh.sysykeji.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://bax.shuidangran.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://tqn.xylfe.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ozu.xinyue.icu

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wtt.ppjwa.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hwg.0kj1m.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://dqg.sysykeji.top

[D26] 数组转字符串
来源：http://mmc.hfpthk.cn

Py:   ", ".join(map(str, arr))
来源：http://phv.fanxiaobao.xyz

PHP:  implode(", ", $arr);
来源：http://snm.chenzaomai.com

JS:   arr.join(", ")
来源：http://wyr.hammf.cn

TS:   arr.join(", ")
来源：http://ojo.yuanzhike.top


<!-- 参考信息 -->