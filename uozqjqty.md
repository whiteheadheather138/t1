代发 wailian999

[C10] 变量作用域
来源：http://uoa.gotoacloud.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://nqz.pycfn.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ifu.shzxlz.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hus.shuidangran.top

TS:   同 JS
来源：http://nkn.zhiwuduotai.top

Java: 方法内为块级作用域
来源：http://bap.shanyushiyangtech.top

Go:   花括号块级作用域
来源：http://wcw.yfazqb.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://oko.feifeiyinyue.top

C#:   块级作用域
来源：http://yvf.xingfuxueyuan.xyz

[C11] 模块导入与导出
来源：http://apm.cheryme.top

Py:   from module import func
来源：http://waa.yvedp.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://dcz.xziqi.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://qwd.sufxvd.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://gkd.uphjek.com

Java: import java.util.List;
来源：http://pax.yangfankeji.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://try.shuidangran.top

Ruby: require "json"; require_relative "./util"
来源：http://gnn.zhongyouzk.top

C#:   using System.Text;
来源：http://nlt.fanxiaobao.xyz

[C12] 立即执行函数 IIFE
来源：http://qkp.c1oappe.top

Py:   (lambda: print("run"))()
来源：http://nzi.kuanghao11.cn

PHP:  (function () { echo "run"; })();
来源：http://bhw.daxiang520.top

JS:   (() => { console.log("run"); })();
来源：http://njs.0kj1m.cn

TS:   (() => { console.log("run"); })();
来源：http://ste.zdqjudy.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://rus.nanxinkj.top

Go:   func() { fmt.Println("run") }()
来源：http://qcc.yvedp.cn

Ruby: -> { puts "run" }.call
来源：http://qmq.316326.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://vbv.wangdashe.top

[C13] 类型声明 / 类型注解
来源：http://oze.yj20258.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://fay.ydjk.org.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zof.fzhhl.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://uda.tianlin.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bgi.hnqzz.top

Java: int add(int a, int b) { return a + b; }
来源：http://drw.guowangkeji.top

Go:   func add(a, b int) int
来源：http://byy.ywan-chungtsiang.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://rdm.meibo888.top

C#:   int Add(int a, int b) => a + b;
来源：http://nld.ydjk.org.cn

[C14] 泛型函数
来源：http://zfv.316326.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://sob.jinyuanbaomall.cn

PHP:  // 无泛型
来源：http://geq.vehdjk.com

JS:   // 无泛型
来源：http://gde.shangyingyoupin.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://yop.xingfuxueyuan.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://dyr.gogol.net.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://lwu.epnwcf.com

Ruby: # 无泛型
来源：http://jhi.yanxiufei.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://oyq.cucudq.cn

[C15] 解构 / 展开参数
来源：http://nbw.sufxvd.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://kfn.yj20258888.top

PHP:  [$a, $b] = $pair;
来源：http://vdx.jyoumei.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://igs.52xcode.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://iax.jqgufenzy.top

Java: // 无解构
来源：http://cqf.daria6918.cn

Go:   // 无解构
来源：http://eah.hongshengwenyu.top

Ruby: a, b = pair
来源：http://nsv.xinyue.icu

C#:   var (a, b) = pair;
来源：http://qvg.shangyingyoupin.top

[C16] 函数 / 方法重载
来源：http://cvm.jqgufenzy.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://pgg.haohaochexian.top

PHP:  // 无重载
来源：http://bli.c1oappe.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://eos.xuanzx.com

TS:   // 用联合类型或重载签名声明
来源：http://tjn.tanke756.top

Java: void f(int a) {}  void f(String a) {}
来源：http://jfu.yj202588.top

Go:   // 无重载：用不同函数名
来源：http://ztd.nanxinkj.top

Ruby: # 无重载：靠动态参数
来源：http://utj.yfazqb.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://vec.aizwys.cn

================================================================================
来源：http://etm.316326.xyz

D. 数组 / 列表 / 集合
来源：http://elz.ydzc1.top

================================================================================
来源：http://tiq.nwbrower.top

[D01] 创建数组 / 列表
来源：http://qnw.zhoulong.xyz

Py:   arr = [1, 2, 3];  empty = []
来源：http://ucc.cqqwz.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://acl.sufxvd.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://clb.cucudq.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://mfj.yonumen.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://lld.shangyingyoupin.top

Go:   arr := []int{1, 2, 3}
来源：http://unb.yangfankeji.com

Ruby: arr = [1, 2, 3]
来源：http://lnj.hnqzz.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ywb.fengsongda.top

[D02] 追加元素到末尾
来源：http://srw.xuetiantiany.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ywb.yfazqb.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://luf.zycfv.cn

JS:   arr.push(4);
来源：http://vrl.xuetiantiany.cn

TS:   arr.push(4);
来源：http://phi.shanyushiyangkeji.top

Java: list.add(4);
来源：http://wfx.kuanghao11.cn

Go:   arr = append(arr, 4)
来源：http://xzq.jianghu66.top

Ruby: arr << 4; arr.push(5)
来源：http://ryz.havefunace.top

C#:   list.Add(4);
来源：http://wvz.ydjk.org.cn

[D03] 在指定位置插入元素
来源：http://zkm.vehdjk.com

Py:   arr.insert(0, 0)
来源：http://kkt.hywenlv.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hlu.fanxiaobao.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://iil.yfazqb.com

TS:   arr.splice(0, 0, 0);
来源：http://wsr.yueranfly.top

Java: list.add(0, 0);
来源：http://fdx.yj202588.top

Go:   arr = append([]int{0}, arr...)
来源：http://kga.ybcxt.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://urr.hammf.cn

C#:   list.Insert(0, 0);
来源：http://ekp.shuidangran.top

[D04] 删除元素
来源：http://ckx.hysaishi.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mzf.quarkkingdee.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://cwi.gzhubu.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mbk.jyoumei.cn

TS:   arr.splice(0, 1);
来源：http://zmx.yfazqb.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://waw.andypj.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://lvp.jinyuanbaomall.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://gkc.316326.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://lgv.cheryme.top

[D05] 访问与修改元素
来源：http://kes.fehbvm.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ofy.cashguo.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://gcx.shangyingyoupin.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://dkh.gaohongyu789.top

TS:   arr[0]; arr.at(-1);
来源：http://efm.fehbvm.com

Java: list.get(0); list.set(0, 9);
来源：http://pem.nanxinkj.top

Go:   arr[0]; arr[0] = 9
来源：http://too.cucudq.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://dyw.yj20258888.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://sgv.zycfv.cn

[D06] 数组长度
来源：http://ghc.zhoulong.xyz

Py:   len(arr)
来源：http://kin.yuanzhike.top

PHP:  count($arr);
来源：http://ogr.9152youxi.cn

JS:   arr.length
来源：http://fac.aizwys.cn

TS:   arr.length
来源：http://lxg.hcnkem.com

Java: list.size();
来源：http://zjl.epnwcf.com

Go:   len(arr)
来源：http://udt.zdqjudy.top

Ruby: arr.length; arr.size
来源：http://gqk.zdbjq.cn

C#:   list.Count;
来源：http://lyp.jqgufenzy.top

[D07] 切片 / 取子数组
来源：http://ioa.bjfxy.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://jwa.jinghuilouyu.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ikg.52xcode.cn

JS:   arr.slice(1, 4);
来源：http://nyp.zycfv.cn

TS:   arr.slice(1, 4);
来源：http://lqv.vehdjk.com

Java: list.subList(1, 4);
来源：http://vyz.tianlin.xyz

Go:   arr[1:4]
来源：http://pdv.guowangkeji.top

Ruby: arr[1, 3]
来源：http://ozi.pycfn.com

C#:   list.GetRange(1, 3);
来源：http://lto.jinqigufen.top

[D08] 合并两个数组
来源：http://jnr.jianghu66.top

Py:   a + b;  a.extend(b)
来源：http://fcn.nwbrower.top

PHP:  array_merge($a, $b);
来源：http://ctf.shuidangran.top

JS:   [...a, ...b];  a.concat(b);
来源：http://pau.hnqzz.top

TS:   [...a, ...b];
来源：http://ycc.xinyue.icu

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://kve.xingfuxueyuan.xyz

Go:   append(a, b...)
来源：http://fup.andypj.xyz

Ruby: a + b;  a.concat(b)
来源：http://fza.zhiwuduotai.top

C#:   a.Concat(b).ToList()
来源：http://adb.jinqigfzy.top

[D09] 排序（升序）
来源：http://waa.snrcjt.cn

Py:   sorted(arr);  arr.sort()
来源：http://kxe.haohaochexian.top

PHP:  sort($arr);
来源：http://kmp.gaohongyu789.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://jjz.ivvv.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://hen.wangdashe.top

Java: Collections.sort(list);  list.sort(null);
来源：http://gez.hcnkem.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://twi.chenlongwang.top

Ruby: arr.sort
来源：http://jlo.hesvh.cn

C#:   list.Sort();
来源：http://hjf.pycfn.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://rpl.sjlbkw.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://xla.haohaochexian.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ncf.cqqwz.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://fvk.yueranfly.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://qtp.shuidangran.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://dzc.hysaishi.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://bzu.hysaishi.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://kbr.andypj.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://fhy.feifeiyinyue.top

[D11] 反转数组
来源：http://ifa.vehdjk.com

Py:   arr[::-1];  arr.reverse()
来源：http://xhe.jinghuilouyu.cn

PHP:  array_reverse($arr);
来源：http://qjy.cdnleiting.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://edq.xylfe.cn

TS:   [...arr].reverse();
来源：http://kho.xuanzx.com

Java: Collections.reverse(list);
来源：http://yuf.ivvv.top

Go:   slices.Reverse(arr)
来源：http://bym.haohaochexian.top

Ruby: arr.reverse
来源：http://iqc.ydjk.org.cn

C#:   list.Reverse();
来源：http://tgc.fehbvm.com

[D12] 查找元素下标
来源：http://pjm.nanxinkj.top

Py:   arr.index(x);  x in arr
来源：http://qzz.nanxuanxn.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://jbs.hysaishi.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tir.andypj.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wqg.yonumen.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://rbu.birdmap.top

Go:   slices.Index(arr, x)
来源：http://tzx.ywan-chungtsiang.top

Ruby: arr.index(x)
来源：http://nrl.xingfuxueyuan.xyz

C#:   list.IndexOf(x);
来源：http://lnx.jinyuanbaomall.cn

[D13] 过滤（保留满足条件的）
来源：http://ldq.9152youxi.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mmc.hongshengwenyu.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://sag.yuxming.cn

JS:   arr.filter(x => x > 3)
来源：http://pyw.hammf.cn

TS:   arr.filter(x => x > 3)
来源：http://rvi.cdnleiting.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://gly.jyoumei.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://zxw.xinyue.icu

Ruby: arr.select { |x| x > 3 }
来源：http://qds.pycfn.com

C#:   list.Where(x => x > 3).ToList()
来源：http://mke.zdqjudy.top

[D14] 映射转换（每个元素变形）
来源：http://vwb.nanxuanxn.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ecw.hcnkem.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://uuw.yangfankeji.com

JS:   arr.map(x => x * 2)
来源：http://vlt.daxiang520.top

TS:   arr.map(x => x * 2)
来源：http://zck.gzhubu.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://ymb.hfpthk.cn

Go:   // 手写循环
来源：http://nag.gotoacloud.top

Ruby: arr.map { |x| x * 2 }
来源：http://miv.c1oappe.top

C#:   list.Select(x => x * 2).ToList()
来源：http://qcp.epnwcf.com

[D15] 去重
来源：http://vex.mhx1999.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ytq.ctjpmb.com

PHP:  array_unique($arr);
来源：http://npb.snrcjt.cn

JS:   [...new Set(arr)]
来源：http://oag.kuanghao11.cn

TS:   [...new Set(arr)]
来源：http://tdu.svipenyu.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://smd.ydzc1.top

Go:   // 用 map[T]struct{} 手写
来源：http://mvj.xylfe.cn

Ruby: arr.uniq
来源：http://rqs.jqgfzy.top

C#:   list.Distinct().ToList()
来源：http://qyb.hesvh.cn

[D16] 求和与平均值
来源：http://bjm.chenlongwang.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wlb.c1oappe.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hpe.shanyushiyangkeji.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://fgb.xinyue.icu

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://qmq.gaohongyu789.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://vjn.yonumen.top

Go:   // 手写循环累加
来源：http://xan.jinqigufen.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ehb.jinyuanbaomall.cn

C#:   list.Sum();  list.Average()
来源：http://sfg.hfpthk.cn

[D17] 最大值与最小值
来源：http://kot.chenjidiqi.icu

Py:   max(arr);  min(arr)
来源：http://huj.9152youxi.cn

PHP:  max($arr);  min($arr);
来源：http://gax.hnxiangtu.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://jpa.chenlongwang.top

TS:   Math.max(...arr);
来源：http://tzw.dashuyun.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://tfy.xinyue.icu

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://oss.zhaomingkeji.xyz

Ruby: arr.max;  arr.min
来源：http://qxq.jianghu66.top

C#:   list.Max();  list.Min()
来源：http://kve.hywenlv.cn

[D18] 扁平化嵌套数组
来源：http://duc.jqgufenzy.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://uqy.daria6918.cn

PHP:  array_merge(...$nested);
来源：http://wrm.xuanzx.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://syg.daria6918.cn

TS:   nested.flat();
来源：http://gos.c1oappe.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://zcb.pycfn.com

Go:   // 手写双层循环
来源：http://emv.ybcxt.top

Ruby: nested.flatten
来源：http://uhf.gzhubu.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://ref.yuxming.cn

[D19] 按字段分组
来源：http://hzc.jqgfzy.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hpz.feifeiyinyue.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ejf.yvedp.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://cuz.fehbvm.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://oef.yfazqb.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://qch.chenjidiqi.icu

Go:   // 手写 map[string][]T
来源：http://owi.jqgfzy.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://dlf.svipenyu.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://dtd.jyoumei.cn

[D20] 统计每个元素出现次数
来源：http://zch.bjfxy.top

Py:   Counter(arr)
来源：http://rfb.yanxiufei.cn

PHP:  array_count_values($arr);
来源：http://lhy.ehwqpu.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cin.yangfankeji.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nbw.ctjpmb.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://qxp.ydjk.org.cn

Go:   // 手写 map[T]int
来源：http://rek.smart0.xyz

Ruby: arr.tally
来源：http://ikl.mhx1999.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://usv.zdbjq.cn

[D21] 判断是否包含某元素
来源：http://joy.hywenlv.cn

Py:   x in arr
来源：http://nyz.xziqi.cn

PHP:  in_array($x, $arr, true);
来源：http://xxa.wangdashe.top

JS:   arr.includes(x)
来源：http://ktc.zhengqikj.top

TS:   arr.includes(x)
来源：http://rqs.birdmap.top

Java: list.contains(x)
来源：http://ivv.andypj.xyz

Go:   slices.Contains(arr, x)
来源：http://woc.quarkkingdee.top

Ruby: arr.include?(x)
来源：http://czz.svipenyu.cn

C#:   list.Contains(x)
来源：http://htb.xziqi.cn

[D22] 复制数组（避免共享引用）
来源：http://tyv.c1oappe.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ojr.tian-w.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://iio.tian-w.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://zdq.guowangkeji.top

TS:   [...arr];
来源：http://lhr.ydzc1.top

Java: new ArrayList<>(list);
来源：http://hzp.birdmap.top

Go:   copied := append([]int(nil), arr...)
来源：http://ixi.cheryme.top

Ruby: arr.dup;  arr.clone
来源：http://kul.shzxlz.cn

C#:   new List<int>(list);
来源：http://rxx.gzhubu.top

[D23] reduce 累积计算
来源：http://xfc.tian-w.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://nxx.sxryk.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://cgx.zdbjq.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kxw.sxryk.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dgl.jiagoushi.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://yya.shanyushiyangkeji.top

Go:   // 手写循环
来源：http://tdn.52xcode.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mpb.jqgufenzy.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://doh.iojbl.cn

[D24] 字典 / Map 基本操作
来源：http://ioq.hfpthk.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://qic.snrcjt.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://zcw.andypj.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://iqb.daria6918.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://flx.uphjek.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://rvi.fengsongda.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wir.zhiwuduotai.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://whu.xuetiantiany.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mcp.sufxvd.cn

[D25] Set 集合去重与交并差
来源：http://iuh.yanxiufei.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://spr.wangshuangyany.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://yow.jinghuilouyu.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://lcz.chenzaomai.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ubn.gzhubu.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://lja.jinyuanbaomall.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://gqy.xylfe.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xro.zhixingplan.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://nzm.ivvv.top

[D26] 数组转字符串
来源：http://isx.iojbl.cn

Py:   ", ".join(map(str, arr))
来源：http://eru.hesvh.cn

PHP:  implode(", ", $arr);
来源：http://ejg.yongpay.top

JS:   arr.join(", ")
来源：http://tfx.kuanghao11.cn

TS:   arr.join(", ")
来源：http://xqt.ywan-chungtsiang.top

Java: String.join(", ", list)
来源：http://khx.sjlbkw.cn

Go:   strings.Join(strs, ", ")
来源：http://vbr.shuidangran.top

Ruby: arr.join(", ")
来源：http://gka.nanxinkj.top

C#:   string.Join(", ", list)
来源：http://uor.zhiwuduotai.top


<!-- 参考信息 -->