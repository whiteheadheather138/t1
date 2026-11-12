代发 wailian999

[C10] 变量作用域
来源：http://ovz.mhx1999.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mnr.yuxming.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ora.birdmap.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hqz.ppjwa.cn

TS:   同 JS
来源：http://wsv.kuanghao11.cn

Java: 方法内为块级作用域
来源：http://ihl.kuanghao11.cn

Go:   花括号块级作用域
来源：http://uxv.jlsjyb.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wop.yj20258.top

C#:   块级作用域
来源：http://tme.sysykeji.top

[C11] 模块导入与导出
来源：http://bqm.zhijiandao.cn

Py:   from module import func
来源：http://tbb.jiagoushi.top

PHP:  require "file.php";  或 use App\Service;
来源：http://cqq.c1oappe.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://qgs.zycfv.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ugc.chenlongwang.top

Java: import java.util.List;
来源：http://swj.redwolf501.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://kfy.cashguo.top

Ruby: require "json"; require_relative "./util"
来源：http://rik.havefunace.top

C#:   using System.Text;
来源：http://fmk.iojbl.cn

[C12] 立即执行函数 IIFE
来源：http://chi.tianlin.xyz

Py:   (lambda: print("run"))()
来源：http://qfm.shuidangran.top

PHP:  (function () { echo "run"; })();
来源：http://ism.52xcode.cn

JS:   (() => { console.log("run"); })();
来源：http://ynl.nanxinkj.top

TS:   (() => { console.log("run"); })();
来源：http://fad.andypj.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://esj.xylfe.cn

Go:   func() { fmt.Println("run") }()
来源：http://wnq.jyoumei.cn

Ruby: -> { puts "run" }.call
来源：http://hjj.jinghuilouyu.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://bjt.andypj.xyz

[C13] 类型声明 / 类型注解
来源：http://lmh.ywan-chungtsiang.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://yza.epnwcf.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fxt.jlsjyb.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://vjz.hysaishi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://iua.zhijiandao.cn

Java: int add(int a, int b) { return a + b; }
来源：http://gdh.shuidangran.top

Go:   func add(a, b int) int
来源：http://phg.shanyushiyangtech.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wun.xylfe.cn

C#:   int Add(int a, int b) => a + b;
来源：http://djl.jyoumei.cn

[C14] 泛型函数
来源：http://qrj.bbcook.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hmk.yanxiufei.cn

PHP:  // 无泛型
来源：http://oln.ppjwa.cn

JS:   // 无泛型
来源：http://glo.hywenlv.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hpr.iojbl.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://udf.jyoumei.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wlu.xziqi.cn

Ruby: # 无泛型
来源：http://abu.uphjek.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hed.hfpthk.cn

[C15] 解构 / 展开参数
来源：http://ziw.ydzc1.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://bof.sufxvd.cn

PHP:  [$a, $b] = $pair;
来源：http://xot.zhixingplan.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://kmq.aibaodan.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://gtq.fzhhl.top

Java: // 无解构
来源：http://raa.hnqzz.top

Go:   // 无解构
来源：http://wlj.gzhubu.top

Ruby: a, b = pair
来源：http://nbs.zhengqikj.top

C#:   var (a, b) = pair;
来源：http://qoc.sweek.top

[C16] 函数 / 方法重载
来源：http://rzg.tianlin.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://jda.yj20258.top

PHP:  // 无重载
来源：http://cxz.iojbl.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://oua.dianchejie.cn

TS:   // 用联合类型或重载签名声明
来源：http://kev.cucudq.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://faa.fehbvm.com

Go:   // 无重载：用不同函数名
来源：http://gpc.fanxiaobao.xyz

Ruby: # 无重载：靠动态参数
来源：http://xxi.sufxvd.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://gjo.daxiang520.top

================================================================================
来源：http://yfe.hesvh.cn

D. 数组 / 列表 / 集合
来源：http://fmx.shuidangran.top

================================================================================
来源：http://zxe.yuxming.cn

[D01] 创建数组 / 列表
来源：http://pdq.andypj.xyz

Py:   arr = [1, 2, 3];  empty = []
来源：http://ukj.jyoumei.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://tav.vehdjk.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ord.haohaochexian.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://row.redwolf501.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://fau.epnwcf.com

Go:   arr := []int{1, 2, 3}
来源：http://zyt.yueranfly.top

Ruby: arr = [1, 2, 3]
来源：http://irr.zdqjudy.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mmn.cucudq.cn

[D02] 追加元素到末尾
来源：http://qjb.yuxming.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://pzg.guowangkeji.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://lhr.zycfv.cn

JS:   arr.push(4);
来源：http://foc.pycfn.com

TS:   arr.push(4);
来源：http://rok.xylfe.cn

Java: list.add(4);
来源：http://zmz.andypj.xyz

Go:   arr = append(arr, 4)
来源：http://pke.sxryk.cn

Ruby: arr << 4; arr.push(5)
来源：http://odv.zhaomingkeji.xyz

C#:   list.Add(4);
来源：http://yae.chenlongwang.top

[D03] 在指定位置插入元素
来源：http://igw.shanyushiyangkeji.top

Py:   arr.insert(0, 0)
来源：http://ckp.haohaochexian.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://gsu.shzxlz.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ztf.gaohongyu789.top

TS:   arr.splice(0, 0, 0);
来源：http://bja.52xcode.cn

Java: list.add(0, 0);
来源：http://kft.jqgufenzy.top

Go:   arr = append([]int{0}, arr...)
来源：http://ufv.dashuyun.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://fuq.uphjek.com

C#:   list.Insert(0, 0);
来源：http://hpr.ppjwa.cn

[D04] 删除元素
来源：http://uji.cashguo.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://fbc.zhiwuduotai.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://plr.chenjidiqi.icu

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ezh.xziqi.cn

TS:   arr.splice(0, 1);
来源：http://lnp.aizwys.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://rdr.xuanzx.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://pax.jinyuanbaomall.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://dsx.jqgufenzy.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://kvb.vqdsnc.cn

[D05] 访问与修改元素
来源：http://wrg.yueranfly.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://sgh.jyoumei.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://gen.fzhhl.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://yqo.xinyue.icu

TS:   arr[0]; arr.at(-1);
来源：http://aqx.ehwqpu.com

Java: list.get(0); list.set(0, 9);
来源：http://urg.ydzc1.top

Go:   arr[0]; arr[0] = 9
来源：http://lab.xuanzx.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://unw.yonumen.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wwy.ywan-chungtsiang.top

[D06] 数组长度
来源：http://yje.316326.xyz

Py:   len(arr)
来源：http://wlz.xingfuxueyuan.xyz

PHP:  count($arr);
来源：http://rqx.yuanzhike.top

JS:   arr.length
来源：http://nqh.jqgfzy.top

TS:   arr.length
来源：http://rlt.vqdsnc.cn

Java: list.size();
来源：http://gtf.zhiwuduotai.top

Go:   len(arr)
来源：http://jtf.wangdashe.top

Ruby: arr.length; arr.size
来源：http://ugd.ehwqpu.com

C#:   list.Count;
来源：http://pzo.vqdsnc.cn

[D07] 切片 / 取子数组
来源：http://yjj.fanxiaobao.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mpa.haohaochexian.top

PHP:  array_slice($arr, 1, 3);
来源：http://tvv.gotoacloud.top

JS:   arr.slice(1, 4);
来源：http://ocz.zycfv.cn

TS:   arr.slice(1, 4);
来源：http://nbe.cdnleiting.top

Java: list.subList(1, 4);
来源：http://auj.nwbrower.top

Go:   arr[1:4]
来源：http://igg.iojbl.cn

Ruby: arr[1, 3]
来源：http://ubc.316326.xyz

C#:   list.GetRange(1, 3);
来源：http://gjk.yuxming.cn

[D08] 合并两个数组
来源：http://hdw.gaohongyu789.top

Py:   a + b;  a.extend(b)
来源：http://hdi.zhaomingkeji.xyz

PHP:  array_merge($a, $b);
来源：http://ydm.hesvh.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://lkm.hysaishi.cn

TS:   [...a, ...b];
来源：http://bnc.ctjpmb.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://yqt.zhaomingkeji.xyz

Go:   append(a, b...)
来源：http://uub.birdmap.top

Ruby: a + b;  a.concat(b)
来源：http://jqy.tarul.cn

C#:   a.Concat(b).ToList()
来源：http://dyt.tian-w.cn

[D09] 排序（升序）
来源：http://edo.nanxuanxn.top

Py:   sorted(arr);  arr.sort()
来源：http://bah.cdnleiting.top

PHP:  sort($arr);
来源：http://cce.cheryme.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://jbp.zdqjudy.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://jre.meibo888.top

Java: Collections.sort(list);  list.sort(null);
来源：http://leq.zhaomingkeji.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://nkt.mhx1999.top

Ruby: arr.sort
来源：http://lss.guowangkeji.top

C#:   list.Sort();
来源：http://hqm.aibaodan.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://uxd.jinghuilouyu.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://kga.daria6918.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pqy.aizwys.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://doi.xziqi.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://sbg.tianlin.xyz

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mgg.hcnkem.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://cio.gaohongyu789.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mqf.yj202588.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://xbg.c1oappe.top

[D11] 反转数组
来源：http://bdy.zdbjq.cn

Py:   arr[::-1];  arr.reverse()
来源：http://wmw.fanxiaobao.xyz

PHP:  array_reverse($arr);
来源：http://dnh.chenlongwang.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://dzg.yanxiufei.cn

TS:   [...arr].reverse();
来源：http://qxd.yangfankeji.com

Java: Collections.reverse(list);
来源：http://hva.fehbvm.com

Go:   slices.Reverse(arr)
来源：http://wpj.zhongyouzk.top

Ruby: arr.reverse
来源：http://wtg.yuanzhike.top

C#:   list.Reverse();
来源：http://owl.ivvv.top

[D12] 查找元素下标
来源：http://mhj.xuetiantiany.cn

Py:   arr.index(x);  x in arr
来源：http://ycb.meibo888.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://xcd.zhaomingkeji.xyz

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rpa.ivvv.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://eje.c1oappe.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://umh.gaohongyu789.top

Go:   slices.Index(arr, x)
来源：http://aue.zdqjudy.top

Ruby: arr.index(x)
来源：http://cpn.hfpthk.cn

C#:   list.IndexOf(x);
来源：http://qzq.gaohongyu789.top

[D13] 过滤（保留满足条件的）
来源：http://zqa.iojbl.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ulz.mhx1999.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://pha.sweek.top

JS:   arr.filter(x => x > 3)
来源：http://vhb.sysykeji.top

TS:   arr.filter(x => x > 3)
来源：http://ojo.wangdashe.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://uvz.yonumen.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ycw.sxryk.cn

Ruby: arr.select { |x| x > 3 }
来源：http://hcy.nanxuanxn.top

C#:   list.Where(x => x > 3).ToList()
来源：http://lbg.fehbvm.com

[D14] 映射转换（每个元素变形）
来源：http://vdi.ppjwa.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://iqk.yueranfly.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://qwf.gaohongyu789.top

JS:   arr.map(x => x * 2)
来源：http://jsh.cdnleiting.top

TS:   arr.map(x => x * 2)
来源：http://ulp.redwolf501.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://mwr.jinyuanbaomall.cn

Go:   // 手写循环
来源：http://fle.yuxming.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ecf.xylfe.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://qkn.wangshuangyany.cn

[D15] 去重
来源：http://ksh.nanxuanxn.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://tat.yfazqb.com

PHP:  array_unique($arr);
来源：http://tzv.dianchejie.cn

JS:   [...new Set(arr)]
来源：http://omw.redwolf501.top

TS:   [...new Set(arr)]
来源：http://fla.dianchejie.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ygv.hesvh.cn

Go:   // 用 map[T]struct{} 手写
来源：http://zye.jinqigufen.top

Ruby: arr.uniq
来源：http://uoi.sysykeji.top

C#:   list.Distinct().ToList()
来源：http://tbw.zdbjq.cn

[D16] 求和与平均值
来源：http://zqz.meibo888.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://xeg.gogol.net.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qka.xziqi.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://zlv.cdnleiting.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://tuy.ydjk.org.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mll.hongshengwenyu.top

Go:   // 手写循环累加
来源：http://uci.zdqjudy.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://btu.tanke756.top

C#:   list.Sum();  list.Average()
来源：http://ini.xinyue.icu

[D17] 最大值与最小值
来源：http://obo.zhengqikj.top

Py:   max(arr);  min(arr)
来源：http://oki.hfpthk.cn

PHP:  max($arr);  min($arr);
来源：http://lyf.xuetiantiany.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://xkh.fktsv.cn

TS:   Math.max(...arr);
来源：http://ala.haohaochexian.top

Java: Collections.max(list);  Collections.min(list);
来源：http://flg.xziqi.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://bkd.zdbjq.cn

Ruby: arr.max;  arr.min
来源：http://xle.ivvv.top

C#:   list.Max();  list.Min()
来源：http://jip.9152youxi.cn

[D18] 扁平化嵌套数组
来源：http://aok.mhx1999.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ckp.nanxinkj.top

PHP:  array_merge(...$nested);
来源：http://skb.sweek.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wve.hysaishi.cn

TS:   nested.flat();
来源：http://uvm.iojbl.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://syc.chenlongwang.top

Go:   // 手写双层循环
来源：http://wsc.cashguo.top

Ruby: nested.flatten
来源：http://akd.bjfxy.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://vbd.fehbvm.com

[D19] 按字段分组
来源：http://vzs.daria6918.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://rtq.yuanzhike.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://fnh.andypj.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://bci.tarul.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://zuj.cdnleiting.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://oha.jqgufenzy.top

Go:   // 手写 map[string][]T
来源：http://xwg.shanyushiyangtech.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://ifm.pycfn.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://vau.zdbjq.cn

[D20] 统计每个元素出现次数
来源：http://osw.yuanzhike.top

Py:   Counter(arr)
来源：http://pcc.aibaodan.cn

PHP:  array_count_values($arr);
来源：http://jsr.epnwcf.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lom.shanyushiyangkeji.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lbp.hfpthk.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://gat.yangfankeji.com

Go:   // 手写 map[T]int
来源：http://qcl.yueranfly.top

Ruby: arr.tally
来源：http://jon.zhaomingkeji.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://lpt.yfazqb.com

[D21] 判断是否包含某元素
来源：http://hzm.ywan-chungtsiang.top

Py:   x in arr
来源：http://kph.zycfv.cn

PHP:  in_array($x, $arr, true);
来源：http://lqp.haohaochexian.top

JS:   arr.includes(x)
来源：http://mzv.andypj.xyz

TS:   arr.includes(x)
来源：http://kzg.xinyue.icu

Java: list.contains(x)
来源：http://kpx.gzhubu.top

Go:   slices.Contains(arr, x)
来源：http://tob.fanxiaobao.xyz

Ruby: arr.include?(x)
来源：http://dey.snrcjt.cn

C#:   list.Contains(x)
来源：http://bdd.hysaishi.cn

[D22] 复制数组（避免共享引用）
来源：http://bwe.meibo888.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://jqx.feifeiyinyue.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://stg.ydzc1.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://rud.fehbvm.com

TS:   [...arr];
来源：http://mqz.tarul.cn

Java: new ArrayList<>(list);
来源：http://bcw.xuanzx.com

Go:   copied := append([]int(nil), arr...)
来源：http://ifd.hesvh.cn

Ruby: arr.dup;  arr.clone
来源：http://jia.ydjk.org.cn

C#:   new List<int>(list);
来源：http://lnn.9152youxi.cn

[D23] reduce 累积计算
来源：http://lmk.wangshuangyany.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://vvm.svipenyu.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://tav.mhx1999.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pdk.quarkkingdee.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://aga.mhx1999.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://aza.bbcook.cn

Go:   // 手写循环
来源：http://lrq.0kj1m.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://jmc.yj20258888.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://pgp.shangyingyoupin.top

[D24] 字典 / Map 基本操作
来源：http://jxl.uphjek.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://vgl.chenzaomai.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://vpw.yanxiufei.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://fxw.fehbvm.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://dai.birdmap.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://aml.yj202588.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://kfd.tanke756.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://uuy.zhixingplan.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://sip.dianchejie.cn

[D25] Set 集合去重与交并差
来源：http://cpp.9152youxi.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://lwa.yj20258888.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wad.yonumen.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://diw.yonumen.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://frr.shzxlz.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://rra.0kj1m.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://tlt.xuetiantiany.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xhm.sysykeji.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://xlk.guowangkeji.top

[D26] 数组转字符串
来源：http://hwz.pycfn.com

Py:   ", ".join(map(str, arr))
来源：http://itg.yfazqb.com

PHP:  implode(", ", $arr);
来源：http://zvh.yvedp.cn

JS:   arr.join(", ")
来源：http://bpl.ivvv.top

TS:   arr.join(", ")
来源：http://fph.jiagoushi.top

Java: String.join(", ", list)
来源：http://toi.havefunace.top

Go:   strings.Join(strs, ", ")
来源：http://yth.pengpengdd.cyou

Ruby: arr.join(", ")
来源：http://zuz.jinghuilouyu.cn

C#:   string.Join(", ", list)
来源：http://hkt.cqqwz.cn


<!-- 参考信息 -->