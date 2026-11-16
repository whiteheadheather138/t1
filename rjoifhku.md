代发 wailian999

[C10] 变量作用域
来源：http://glz.mhx1999.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://fyt.gzhubu.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://xvz.hywenlv.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://kba.jinqigfzy.top

TS:   同 JS
来源：http://hrs.yj202588.top

Java: 方法内为块级作用域
来源：http://nzr.vehdjk.com

Go:   花括号块级作用域
来源：http://goi.tarul.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://djd.zhiwuduotai.top

C#:   块级作用域
来源：http://pzd.fengsongda.top

[C11] 模块导入与导出
来源：http://bep.sweek.top

Py:   from module import func
来源：http://dju.gzhubu.top

PHP:  require "file.php";  或 use App\Service;
来源：http://krm.smart0.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://bti.cucudq.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://qmf.jqgufenzy.top

Java: import java.util.List;
来源：http://vrh.aizwys.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://lzp.hongshengwenyu.top

Ruby: require "json"; require_relative "./util"
来源：http://gao.vehdjk.com

C#:   using System.Text;
来源：http://awh.hcnkem.com

[C12] 立即执行函数 IIFE
来源：http://unp.cucudq.cn

Py:   (lambda: print("run"))()
来源：http://gdk.daria6918.cn

PHP:  (function () { echo "run"; })();
来源：http://eje.tianlin.xyz

JS:   (() => { console.log("run"); })();
来源：http://sdt.havefunace.top

TS:   (() => { console.log("run"); })();
来源：http://dcv.fengsongda.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://xuv.jyoumei.cn

Go:   func() { fmt.Println("run") }()
来源：http://etk.jinghuilouyu.cn

Ruby: -> { puts "run" }.call
来源：http://azq.ydjk.org.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://sap.uphjek.com

[C13] 类型声明 / 类型注解
来源：http://szc.hnxiangtu.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wkx.yonumen.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://etk.52xcode.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hkl.shuidangran.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ymj.hywenlv.cn

Java: int add(int a, int b) { return a + b; }
来源：http://tfq.shanyushiyangtech.top

Go:   func add(a, b int) int
来源：http://kfa.yfazqb.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://qid.jlsjyb.cn

C#:   int Add(int a, int b) => a + b;
来源：http://cbz.tian-w.cn

[C14] 泛型函数
来源：http://ndz.quarkkingdee.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://gqe.zhiwuduotai.top

PHP:  // 无泛型
来源：http://msm.nwbrower.top

JS:   // 无泛型
来源：http://byr.gaohongyu789.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://qdf.bbcook.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wjy.yj202588.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://lfx.gotoacloud.top

Ruby: # 无泛型
来源：http://out.nwbrower.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://rlk.zdqjudy.top

[C15] 解构 / 展开参数
来源：http://uvf.cheryme.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://prm.0kj1m.cn

PHP:  [$a, $b] = $pair;
来源：http://qgr.nanxuanxn.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://vbm.guowangkeji.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://btp.hnqzz.top

Java: // 无解构
来源：http://azs.zhoulong.xyz

Go:   // 无解构
来源：http://qee.sjlbkw.cn

Ruby: a, b = pair
来源：http://dkh.birdmap.top

C#:   var (a, b) = pair;
来源：http://ltc.wangshuangyany.cn

[C16] 函数 / 方法重载
来源：http://whm.redwolf501.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://byz.gaohongyu789.top

PHP:  // 无重载
来源：http://pcf.daxiang520.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://iai.dashuyun.cn

TS:   // 用联合类型或重载签名声明
来源：http://rid.yanxiufei.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://rfs.fktsv.cn

Go:   // 无重载：用不同函数名
来源：http://xuy.xuetiantiany.cn

Ruby: # 无重载：靠动态参数
来源：http://qav.0kj1m.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://rmj.fzhhl.top

================================================================================
来源：http://chr.hammf.cn

D. 数组 / 列表 / 集合
来源：http://api.xuetiantiany.cn

================================================================================
来源：http://hxu.snrcjt.cn

[D01] 创建数组 / 列表
来源：http://bql.dashuyun.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://brx.jqgfzy.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://riz.xylfe.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://gwn.wangdashe.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://krr.aizwys.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://lac.ctjpmb.com

Go:   arr := []int{1, 2, 3}
来源：http://zvh.vehdjk.com

Ruby: arr = [1, 2, 3]
来源：http://qud.hnqzz.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://vah.birdmap.top

[D02] 追加元素到末尾
来源：http://itf.gotoacloud.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://oqn.tianlin.xyz

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://idf.yj20258.top

JS:   arr.push(4);
来源：http://gnw.9152youxi.cn

TS:   arr.push(4);
来源：http://rme.ydjk.org.cn

Java: list.add(4);
来源：http://kfi.sysykeji.top

Go:   arr = append(arr, 4)
来源：http://min.yueranfly.top

Ruby: arr << 4; arr.push(5)
来源：http://ndt.hcnkem.com

C#:   list.Add(4);
来源：http://nsh.52xcode.cn

[D03] 在指定位置插入元素
来源：http://hnl.jianghu66.top

Py:   arr.insert(0, 0)
来源：http://dlu.zhongyouzk.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://lkt.vehdjk.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://tjj.hongshengwenyu.top

TS:   arr.splice(0, 0, 0);
来源：http://dqr.316326.xyz

Java: list.add(0, 0);
来源：http://lkm.jinyuanbaomall.cn

Go:   arr = append([]int{0}, arr...)
来源：http://wnw.hysaishi.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://lwo.hnxiangtu.top

C#:   list.Insert(0, 0);
来源：http://tjc.yanxiufei.cn

[D04] 删除元素
来源：http://nml.andypj.xyz

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://bbn.cqqwz.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://xyf.cheryme.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://tnw.aizwys.cn

TS:   arr.splice(0, 1);
来源：http://eec.shangyingyoupin.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ajy.jinqigfzy.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://juu.sysykeji.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ryo.zhijiandao.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://foc.zhongyouzk.top

[D05] 访问与修改元素
来源：http://hqm.9152youxi.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://nbx.9152youxi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://fbb.jlsjyb.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hmh.hysaishi.cn

TS:   arr[0]; arr.at(-1);
来源：http://nip.xuetiantiany.cn

Java: list.get(0); list.set(0, 9);
来源：http://imr.snrcjt.cn

Go:   arr[0]; arr[0] = 9
来源：http://jxe.xingfuxueyuan.xyz

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ere.gzhubu.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://miw.zhijiandao.cn

[D06] 数组长度
来源：http://usx.hesvh.cn

Py:   len(arr)
来源：http://zot.yuanzhike.top

PHP:  count($arr);
来源：http://qmf.bbcook.cn

JS:   arr.length
来源：http://rdh.sysykeji.top

TS:   arr.length
来源：http://hqk.jiagoushi.top

Java: list.size();
来源：http://pul.redwolf501.top

Go:   len(arr)
来源：http://rwi.shuidangran.top

Ruby: arr.length; arr.size
来源：http://cqn.9152youxi.cn

C#:   list.Count;
来源：http://qdl.chenlongwang.top

[D07] 切片 / 取子数组
来源：http://otw.ctjpmb.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://pgt.meibo888.top

PHP:  array_slice($arr, 1, 3);
来源：http://rcl.birdmap.top

JS:   arr.slice(1, 4);
来源：http://dqx.zhixingplan.top

TS:   arr.slice(1, 4);
来源：http://zzk.aizwys.cn

Java: list.subList(1, 4);
来源：http://ywg.zhixingplan.top

Go:   arr[1:4]
来源：http://hsh.bjfxy.top

Ruby: arr[1, 3]
来源：http://xfy.gotoacloud.top

C#:   list.GetRange(1, 3);
来源：http://cqh.jqgfzy.top

[D08] 合并两个数组
来源：http://tpq.shanyushiyangtech.top

Py:   a + b;  a.extend(b)
来源：http://ydn.jqgufenzy.top

PHP:  array_merge($a, $b);
来源：http://idg.zhoulong.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://oha.nanxuanxn.top

TS:   [...a, ...b];
来源：http://ami.yfazqb.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://fzr.yj20258888.top

Go:   append(a, b...)
来源：http://cdz.ybcxt.top

Ruby: a + b;  a.concat(b)
来源：http://tpo.shuidangran.top

C#:   a.Concat(b).ToList()
来源：http://fpm.sweek.top

[D09] 排序（升序）
来源：http://ddh.0kj1m.cn

Py:   sorted(arr);  arr.sort()
来源：http://kvg.yuxming.cn

PHP:  sort($arr);
来源：http://pnh.daxiang520.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://kee.snrcjt.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://awm.xuanzx.com

Java: Collections.sort(list);  list.sort(null);
来源：http://aag.aibaodan.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://tvx.yangfankeji.com

Ruby: arr.sort
来源：http://bvv.jinqigufen.top

C#:   list.Sort();
来源：http://ijr.xylfe.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://zre.pycfn.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://xqu.shanyushiyangkeji.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cno.snrcjt.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://efq.52xcode.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://khx.shanyushiyangtech.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hnf.hcnkem.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://vgo.hfpthk.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mjr.jinghuilouyu.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://xjc.shzxlz.cn

[D11] 反转数组
来源：http://wrb.fehbvm.com

Py:   arr[::-1];  arr.reverse()
来源：http://gbp.feifeiyinyue.top

PHP:  array_reverse($arr);
来源：http://qcd.zycfv.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ijj.pycfn.com

TS:   [...arr].reverse();
来源：http://dak.pycfn.com

Java: Collections.reverse(list);
来源：http://oht.zdqjudy.top

Go:   slices.Reverse(arr)
来源：http://nvg.mhx1999.top

Ruby: arr.reverse
来源：http://sfb.zhongyouzk.top

C#:   list.Reverse();
来源：http://ckx.ywan-chungtsiang.top

[D12] 查找元素下标
来源：http://slc.svipenyu.cn

Py:   arr.index(x);  x in arr
来源：http://vln.ybcxt.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://gtj.kuanghao11.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fym.sjlbkw.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rxy.hesvh.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ctx.zhoulong.xyz

Go:   slices.Index(arr, x)
来源：http://ond.kuanghao11.cn

Ruby: arr.index(x)
来源：http://ylq.zhengqikj.top

C#:   list.IndexOf(x);
来源：http://ciw.tanke756.top

[D13] 过滤（保留满足条件的）
来源：http://gnl.wangdashe.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qeg.fzhhl.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://uxd.snrcjt.cn

JS:   arr.filter(x => x > 3)
来源：http://ajy.xinyue.icu

TS:   arr.filter(x => x > 3)
来源：http://pkp.zdbjq.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://dkq.zhoulong.xyz

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://gps.daxiang520.top

Ruby: arr.select { |x| x > 3 }
来源：http://zkp.svipenyu.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://jgx.zdbjq.cn

[D14] 映射转换（每个元素变形）
来源：http://ldd.52xcode.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://cah.yuanzhike.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vbk.iojbl.cn

JS:   arr.map(x => x * 2)
来源：http://vby.aizwys.cn

TS:   arr.map(x => x * 2)
来源：http://tky.aizwys.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://kdc.cucudq.cn

Go:   // 手写循环
来源：http://tvj.sufxvd.cn

Ruby: arr.map { |x| x * 2 }
来源：http://bhr.jqgufenzy.top

C#:   list.Select(x => x * 2).ToList()
来源：http://qyn.aibaodan.cn

[D15] 去重
来源：http://koj.hfpthk.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://oxg.aizwys.cn

PHP:  array_unique($arr);
来源：http://nwd.hywenlv.cn

JS:   [...new Set(arr)]
来源：http://fhx.52xcode.cn

TS:   [...new Set(arr)]
来源：http://qiu.316326.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ncf.52xcode.cn

Go:   // 用 map[T]struct{} 手写
来源：http://jfu.ywan-chungtsiang.top

Ruby: arr.uniq
来源：http://rut.yj20258888.top

C#:   list.Distinct().ToList()
来源：http://irb.tanke756.top

[D16] 求和与平均值
来源：http://ofm.andypj.xyz

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://sft.smart0.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ikk.tanke756.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ewy.sjlbkw.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://kyb.cucudq.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://tbr.zhoulong.xyz

Go:   // 手写循环累加
来源：http://cgd.hfpthk.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://zdr.shuidangran.top

C#:   list.Sum();  list.Average()
来源：http://ikl.zhongyouzk.top

[D17] 最大值与最小值
来源：http://ryw.0kj1m.cn

Py:   max(arr);  min(arr)
来源：http://aug.yj20258888.top

PHP:  max($arr);  min($arr);
来源：http://pre.sweek.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://akv.jinghuilouyu.cn

TS:   Math.max(...arr);
来源：http://zuq.havefunace.top

Java: Collections.max(list);  Collections.min(list);
来源：http://pyl.havefunace.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://jry.cqqwz.cn

Ruby: arr.max;  arr.min
来源：http://ckr.wangdashe.top

C#:   list.Max();  list.Min()
来源：http://snu.tian-w.cn

[D18] 扁平化嵌套数组
来源：http://iio.uphjek.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://poj.jianghu66.top

PHP:  array_merge(...$nested);
来源：http://kts.havefunace.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://dbc.ehwqpu.com

TS:   nested.flat();
来源：http://hqv.shzxlz.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://cbm.cucudq.cn

Go:   // 手写双层循环
来源：http://zca.gogol.net.cn

Ruby: nested.flatten
来源：http://php.haohaochexian.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://gnk.chenlongwang.top

[D19] 按字段分组
来源：http://vtf.jinyuanbaomall.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://dbu.shangyingyoupin.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hbz.ywan-chungtsiang.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://tjd.tian-w.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://wtc.ydzc1.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://abt.guannengcc.top

Go:   // 手写 map[string][]T
来源：http://vdv.jlsjyb.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://opl.nanxinkj.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://pvi.dianchejie.cn

[D20] 统计每个元素出现次数
来源：http://mdq.ydzc1.top

Py:   Counter(arr)
来源：http://naw.jinqigufen.top

PHP:  array_count_values($arr);
来源：http://bhu.daria6918.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bdk.yanxiufei.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qzw.hongshengwenyu.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ifc.zhoulong.xyz

Go:   // 手写 map[T]int
来源：http://riz.52xcode.cn

Ruby: arr.tally
来源：http://rfk.cheryme.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://gch.sxryk.cn

[D21] 判断是否包含某元素
来源：http://sql.gotoacloud.top

Py:   x in arr
来源：http://zzg.yonumen.top

PHP:  in_array($x, $arr, true);
来源：http://ndt.jianghu66.top

JS:   arr.includes(x)
来源：http://mbt.chenjidiqi.icu

TS:   arr.includes(x)
来源：http://xxq.zhiwuduotai.top

Java: list.contains(x)
来源：http://ivx.zhixingplan.top

Go:   slices.Contains(arr, x)
来源：http://tvf.dashuyun.cn

Ruby: arr.include?(x)
来源：http://kyl.hammf.cn

C#:   list.Contains(x)
来源：http://bes.0kj1m.cn

[D22] 复制数组（避免共享引用）
来源：http://mjf.zhongyouzk.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://gjq.pycfn.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://pue.zdqjudy.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://bpt.hammf.cn

TS:   [...arr];
来源：http://xtk.hnqzz.top

Java: new ArrayList<>(list);
来源：http://vvv.dashuyun.cn

Go:   copied := append([]int(nil), arr...)
来源：http://cvo.yueranfly.top

Ruby: arr.dup;  arr.clone
来源：http://ccc.ydzc1.top

C#:   new List<int>(list);
来源：http://cvu.xuanzx.com

[D23] reduce 累积计算
来源：http://nwb.kuanghao11.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://aby.yj20258.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://odo.uphjek.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gqs.gogol.net.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zid.aibaodan.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://bxo.zhaomingkeji.xyz

Go:   // 手写循环
来源：http://prv.redwolf501.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://fjo.yueranfly.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://yte.xingfuxueyuan.xyz

[D24] 字典 / Map 基本操作
来源：http://clf.bjfxy.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://sez.gaohongyu789.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://xej.jqgfzy.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://fkd.ydjk.org.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://xil.iojbl.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ngw.hywenlv.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ivh.smart0.xyz

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://eqz.zhongyouzk.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mwi.jinyuanbaomall.cn

[D25] Set 集合去重与交并差
来源：http://vtg.hongshengwenyu.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://qtv.fktsv.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://fbv.snrcjt.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://gxi.gzhubu.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://tip.guowangkeji.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://jur.zhoulong.xyz

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://anv.yuxming.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://rcj.fzhhl.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qbx.zhoulong.xyz

[D26] 数组转字符串
来源：http://foa.xuanzx.com

Py:   ", ".join(map(str, arr))
来源：http://xsg.xylfe.cn

PHP:  implode(", ", $arr);
来源：http://ybd.mhx1999.top

JS:   arr.join(", ")
来源：http://jkm.pycfn.com

TS:   arr.join(", ")
来源：http://kof.kuanghao11.cn

Java: String.join(", ", list)
来源：http://ugp.sufxvd.cn

Go:   strings.Join(strs, ", ")
来源：http://egh.jiagoushi.top

Ruby: arr.join(", ")
来源：http://mjl.fehbvm.com

C#:   string.Join(", ", list)
来源：http://pko.andypj.xyz


<!-- 参考信息 -->