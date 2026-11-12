代发 wailian999

[C10] 变量作用域
来源：http://tum.yuanzhike.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://tbj.nwbrower.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://jge.c1oappe.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://oje.yanxiufei.cn

TS:   同 JS
来源：http://zwl.hnxiangtu.top

Java: 方法内为块级作用域
来源：http://had.shanyushiyangkeji.top

Go:   花括号块级作用域
来源：http://xxf.shanyushiyangkeji.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://qot.bjfxy.top

C#:   块级作用域
来源：http://zyh.hfpthk.cn

[C11] 模块导入与导出
来源：http://qsw.ydjk.org.cn

Py:   from module import func
来源：http://gwf.jinqigufen.top

PHP:  require "file.php";  或 use App\Service;
来源：http://ilz.xylfe.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://hjj.xylfe.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://fzc.ybcxt.top

Java: import java.util.List;
来源：http://pwe.havefunace.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://glu.yanxiufei.cn

Ruby: require "json"; require_relative "./util"
来源：http://mts.hongshengwenyu.top

C#:   using System.Text;
来源：http://rpj.yuxming.cn

[C12] 立即执行函数 IIFE
来源：http://qnt.gaohongyu789.top

Py:   (lambda: print("run"))()
来源：http://hjn.zhongyouzk.top

PHP:  (function () { echo "run"; })();
来源：http://pnz.zhoulong.xyz

JS:   (() => { console.log("run"); })();
来源：http://tey.xuanzx.com

TS:   (() => { console.log("run"); })();
来源：http://aqf.ywan-chungtsiang.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://kml.haohaochexian.top

Go:   func() { fmt.Println("run") }()
来源：http://twl.nanxuanxn.top

Ruby: -> { puts "run" }.call
来源：http://sco.jinqigfzy.top

C#:   // 无 IIFE：用静态构造函数
来源：http://iia.nanxinkj.top

[C13] 类型声明 / 类型注解
来源：http://eqe.yonumen.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://abs.gzhubu.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lpe.cdnleiting.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://vrq.fanxiaobao.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qvj.52xcode.cn

Java: int add(int a, int b) { return a + b; }
来源：http://syp.hywenlv.cn

Go:   func add(a, b int) int
来源：http://owz.redwolf501.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://bvz.vehdjk.com

C#:   int Add(int a, int b) => a + b;
来源：http://xzl.ydzc1.top

[C14] 泛型函数
来源：http://eii.sweek.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://vdb.mhx1999.top

PHP:  // 无泛型
来源：http://kht.yuxming.cn

JS:   // 无泛型
来源：http://cuk.shuidangran.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://vio.ehwqpu.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://tku.jinqigfzy.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://vcz.pengpengdd.cyou

Ruby: # 无泛型
来源：http://tpi.xuanzx.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://omq.tanke756.top

[C15] 解构 / 展开参数
来源：http://bfz.hnqzz.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://fql.shuidangran.top

PHP:  [$a, $b] = $pair;
来源：http://efh.jqgufenzy.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ezz.smart0.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://eui.dashuyun.cn

Java: // 无解构
来源：http://spz.dashuyun.cn

Go:   // 无解构
来源：http://paj.ybcxt.top

Ruby: a, b = pair
来源：http://hsq.guowangkeji.top

C#:   var (a, b) = pair;
来源：http://txe.yuanzhike.top

[C16] 函数 / 方法重载
来源：http://oqo.nanxuanxn.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://uww.316326.xyz

PHP:  // 无重载
来源：http://unj.xuanzx.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://gme.hysaishi.cn

TS:   // 用联合类型或重载签名声明
来源：http://nqf.xylfe.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://eji.havefunace.top

Go:   // 无重载：用不同函数名
来源：http://ezy.zdqjudy.top

Ruby: # 无重载：靠动态参数
来源：http://pxk.guowangkeji.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://qlk.quarkkingdee.top

================================================================================
来源：http://ngp.hysaishi.cn

D. 数组 / 列表 / 集合
来源：http://mpu.sweek.top

================================================================================
来源：http://nau.cucudq.cn

[D01] 创建数组 / 列表
来源：http://lsd.shzxlz.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://opa.yueranfly.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://tyv.aizwys.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://pme.feifeiyinyue.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://rds.smart0.xyz

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://one.havefunace.top

Go:   arr := []int{1, 2, 3}
来源：http://pkq.snrcjt.cn

Ruby: arr = [1, 2, 3]
来源：http://uuv.316326.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://etc.jianghu66.top

[D02] 追加元素到末尾
来源：http://hlw.jqgfzy.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://asa.ydjk.org.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://cgx.fanxiaobao.xyz

JS:   arr.push(4);
来源：http://oem.nanxinkj.top

TS:   arr.push(4);
来源：http://nkc.cqqwz.cn

Java: list.add(4);
来源：http://udc.hesvh.cn

Go:   arr = append(arr, 4)
来源：http://uis.ywan-chungtsiang.top

Ruby: arr << 4; arr.push(5)
来源：http://tmf.shuidangran.top

C#:   list.Add(4);
来源：http://wbz.snrcjt.cn

[D03] 在指定位置插入元素
来源：http://jbp.pycfn.com

Py:   arr.insert(0, 0)
来源：http://tpj.aibaodan.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://pys.cucudq.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://col.jiagoushi.top

TS:   arr.splice(0, 0, 0);
来源：http://uwp.xziqi.cn

Java: list.add(0, 0);
来源：http://zna.ivvv.top

Go:   arr = append([]int{0}, arr...)
来源：http://mtz.cashguo.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wdp.jyoumei.cn

C#:   list.Insert(0, 0);
来源：http://czy.cdnleiting.top

[D04] 删除元素
来源：http://pcb.cdnleiting.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://qcn.jianghu66.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://voi.316326.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://kig.zhoulong.xyz

TS:   arr.splice(0, 1);
来源：http://qir.bbcook.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://fks.jinqigufen.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://euk.sysykeji.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://kvn.aizwys.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://zij.yueranfly.top

[D05] 访问与修改元素
来源：http://wkq.yj20258888.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hyo.shanyushiyangtech.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://fnq.yj20258888.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://okl.zdbjq.cn

TS:   arr[0]; arr.at(-1);
来源：http://puc.jinqigufen.top

Java: list.get(0); list.set(0, 9);
来源：http://zgj.hammf.cn

Go:   arr[0]; arr[0] = 9
来源：http://hsv.yongpay.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://efl.feifeiyinyue.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://trr.jinyuanbaomall.cn

[D06] 数组长度
来源：http://zjm.hesvh.cn

Py:   len(arr)
来源：http://wxk.sweek.top

PHP:  count($arr);
来源：http://jah.jlsjyb.cn

JS:   arr.length
来源：http://ioy.guannengcc.top

TS:   arr.length
来源：http://vvs.jqgfzy.top

Java: list.size();
来源：http://hhi.cqqwz.cn

Go:   len(arr)
来源：http://twl.fzhhl.top

Ruby: arr.length; arr.size
来源：http://zge.hesvh.cn

C#:   list.Count;
来源：http://xxj.xuetiantiany.cn

[D07] 切片 / 取子数组
来源：http://gry.kuanghao11.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://bnx.yanxiufei.cn

PHP:  array_slice($arr, 1, 3);
来源：http://nry.sysykeji.top

JS:   arr.slice(1, 4);
来源：http://dua.yangfankeji.com

TS:   arr.slice(1, 4);
来源：http://dqe.tanke756.top

Java: list.subList(1, 4);
来源：http://dvt.hnxiangtu.top

Go:   arr[1:4]
来源：http://qnf.gzhubu.top

Ruby: arr[1, 3]
来源：http://dto.shanyushiyangtech.top

C#:   list.GetRange(1, 3);
来源：http://wxb.dianchejie.cn

[D08] 合并两个数组
来源：http://nwu.c1oappe.top

Py:   a + b;  a.extend(b)
来源：http://bdh.ydzc1.top

PHP:  array_merge($a, $b);
来源：http://edk.kuanghao11.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://mxk.haohaochexian.top

TS:   [...a, ...b];
来源：http://mld.nanxinkj.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://djp.shanyushiyangtech.top

Go:   append(a, b...)
来源：http://dbh.hysaishi.cn

Ruby: a + b;  a.concat(b)
来源：http://rhb.ywan-chungtsiang.top

C#:   a.Concat(b).ToList()
来源：http://cgv.vqdsnc.cn

[D09] 排序（升序）
来源：http://omp.daria6918.cn

Py:   sorted(arr);  arr.sort()
来源：http://dhq.ivvv.top

PHP:  sort($arr);
来源：http://wdx.ydjk.org.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://enb.fanxiaobao.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://cvf.chenjidiqi.icu

Java: Collections.sort(list);  list.sort(null);
来源：http://jpz.9152youxi.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ocd.hongshengwenyu.top

Ruby: arr.sort
来源：http://kfz.dianchejie.cn

C#:   list.Sort();
来源：http://tlz.ctjpmb.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://zyy.jyoumei.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://jvx.yanxiufei.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ayp.sweek.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://fgh.quarkkingdee.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://rvp.hnqzz.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://tbu.chenzaomai.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://oya.9152youxi.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://jkk.ydzc1.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qgj.jiagoushi.top

[D11] 反转数组
来源：http://mck.yfazqb.com

Py:   arr[::-1];  arr.reverse()
来源：http://jyb.ywan-chungtsiang.top

PHP:  array_reverse($arr);
来源：http://fbl.fengsongda.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ttv.ydjk.org.cn

TS:   [...arr].reverse();
来源：http://xrf.tianlin.xyz

Java: Collections.reverse(list);
来源：http://wac.tarul.cn

Go:   slices.Reverse(arr)
来源：http://ijc.xingfuxueyuan.xyz

Ruby: arr.reverse
来源：http://ygz.daria6918.cn

C#:   list.Reverse();
来源：http://dwo.zhiwuduotai.top

[D12] 查找元素下标
来源：http://tyh.xuanzx.com

Py:   arr.index(x);  x in arr
来源：http://ajg.gzhubu.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hrf.jinqigfzy.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fql.haohaochexian.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://uaf.sxryk.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://xyu.snrcjt.cn

Go:   slices.Index(arr, x)
来源：http://nky.cheryme.top

Ruby: arr.index(x)
来源：http://vxz.yonumen.top

C#:   list.IndexOf(x);
来源：http://hct.yj20258888.top

[D13] 过滤（保留满足条件的）
来源：http://fjp.sweek.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ixq.gogol.net.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://tuf.tian-w.cn

JS:   arr.filter(x => x > 3)
来源：http://ias.kuanghao11.cn

TS:   arr.filter(x => x > 3)
来源：http://kbw.nanxuanxn.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://kjo.zhengqikj.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ewg.sysykeji.top

Ruby: arr.select { |x| x > 3 }
来源：http://sfd.xinyue.icu

C#:   list.Where(x => x > 3).ToList()
来源：http://vfy.dianchejie.cn

[D14] 映射转换（每个元素变形）
来源：http://jfx.jinqigufen.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://czv.hammf.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ace.jlsjyb.cn

JS:   arr.map(x => x * 2)
来源：http://ngf.ywan-chungtsiang.top

TS:   arr.map(x => x * 2)
来源：http://ars.nanxinkj.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://tgk.cucudq.cn

Go:   // 手写循环
来源：http://uwy.dashuyun.cn

Ruby: arr.map { |x| x * 2 }
来源：http://otw.wangdashe.top

C#:   list.Select(x => x * 2).ToList()
来源：http://qwm.chenjidiqi.icu

[D15] 去重
来源：http://osh.daxiang520.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://dyt.sysykeji.top

PHP:  array_unique($arr);
来源：http://rol.zhaomingkeji.xyz

JS:   [...new Set(arr)]
来源：http://obf.xuetiantiany.cn

TS:   [...new Set(arr)]
来源：http://fdc.wangshuangyany.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hvl.fktsv.cn

Go:   // 用 map[T]struct{} 手写
来源：http://rre.zhongyouzk.top

Ruby: arr.uniq
来源：http://kuq.sweek.top

C#:   list.Distinct().ToList()
来源：http://eao.snrcjt.cn

[D16] 求和与平均值
来源：http://cda.tianlin.xyz

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://fvd.zdbjq.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://sdt.smart0.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://onz.kuanghao11.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ltr.xziqi.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ivs.hnqzz.top

Go:   // 手写循环累加
来源：http://nhu.ehwqpu.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://jkb.tarul.cn

C#:   list.Sum();  list.Average()
来源：http://myn.shanyushiyangkeji.top

[D17] 最大值与最小值
来源：http://bce.fzhhl.top

Py:   max(arr);  min(arr)
来源：http://ble.9152youxi.cn

PHP:  max($arr);  min($arr);
来源：http://tqg.ydjk.org.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://sry.tarul.cn

TS:   Math.max(...arr);
来源：http://lfv.yuxming.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://vvw.sxryk.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wcj.tian-w.cn

Ruby: arr.max;  arr.min
来源：http://zky.nanxinkj.top

C#:   list.Max();  list.Min()
来源：http://cem.zycfv.cn

[D18] 扁平化嵌套数组
来源：http://bsw.yj20258888.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hrz.daxiang520.top

PHP:  array_merge(...$nested);
来源：http://jtf.zycfv.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mcy.havefunace.top

TS:   nested.flat();
来源：http://isv.nwbrower.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wpe.feifeiyinyue.top

Go:   // 手写双层循环
来源：http://lgb.shanyushiyangtech.top

Ruby: nested.flatten
来源：http://olz.gotoacloud.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://pjo.ydzc1.top

[D19] 按字段分组
来源：http://jmr.cdnleiting.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://gne.hfpthk.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://goi.chenlongwang.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hqt.quarkkingdee.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://vpt.sjlbkw.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://asz.hnxiangtu.top

Go:   // 手写 map[string][]T
来源：http://ybl.hongshengwenyu.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://plp.hywenlv.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://laj.xuanzx.com

[D20] 统计每个元素出现次数
来源：http://cmu.daxiang520.top

Py:   Counter(arr)
来源：http://qgb.guannengcc.top

PHP:  array_count_values($arr);
来源：http://jiw.feifeiyinyue.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vyk.0kj1m.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dtx.wangdashe.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://atz.jyoumei.cn

Go:   // 手写 map[T]int
来源：http://rdo.yongpay.top

Ruby: arr.tally
来源：http://noy.hysaishi.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://scf.jinghuilouyu.cn

[D21] 判断是否包含某元素
来源：http://qkh.zhiwuduotai.top

Py:   x in arr
来源：http://jca.ivvv.top

PHP:  in_array($x, $arr, true);
来源：http://ags.birdmap.top

JS:   arr.includes(x)
来源：http://gsf.cheryme.top

TS:   arr.includes(x)
来源：http://lhc.xylfe.cn

Java: list.contains(x)
来源：http://mmy.feifeiyinyue.top

Go:   slices.Contains(arr, x)
来源：http://qwv.pycfn.com

Ruby: arr.include?(x)
来源：http://joz.chenlongwang.top

C#:   list.Contains(x)
来源：http://ezm.haohaochexian.top

[D22] 复制数组（避免共享引用）
来源：http://rmu.zhongyouzk.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://vjy.hywenlv.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ief.ehwqpu.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://exu.zhiwuduotai.top

TS:   [...arr];
来源：http://syb.hcnkem.com

Java: new ArrayList<>(list);
来源：http://umg.vqdsnc.cn

Go:   copied := append([]int(nil), arr...)
来源：http://tup.316326.xyz

Ruby: arr.dup;  arr.clone
来源：http://kvc.shanyushiyangtech.top

C#:   new List<int>(list);
来源：http://kfu.c1oappe.top

[D23] reduce 累积计算
来源：http://kwf.yvedp.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://isq.ywan-chungtsiang.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://eay.jinghuilouyu.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wpy.ppjwa.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qid.tian-w.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://urf.jqgfzy.top

Go:   // 手写循环
来源：http://pwx.ybcxt.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://zhr.xuetiantiany.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://zrv.shangyingyoupin.top

[D24] 字典 / Map 基本操作
来源：http://xze.fehbvm.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://nij.havefunace.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://fmc.0kj1m.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://twq.chenjidiqi.icu

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://tob.bbcook.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ybj.c1oappe.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://fpj.yj202588.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://gyj.hfpthk.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://xsr.9152youxi.cn

[D25] Set 集合去重与交并差
来源：http://uqe.wangdashe.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://nsx.zhongyouzk.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mem.yj202588.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://koc.ivvv.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://sff.dianchejie.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://qts.xuetiantiany.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://vlo.cqqwz.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ceg.zhixingplan.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mij.hammf.cn

[D26] 数组转字符串
来源：http://smn.shanyushiyangkeji.top

Py:   ", ".join(map(str, arr))
来源：http://fvh.xingfuxueyuan.xyz

PHP:  implode(", ", $arr);
来源：http://ahs.svipenyu.cn

JS:   arr.join(", ")
来源：http://ann.bbcook.cn

TS:   arr.join(", ")
来源：http://rxp.zhixingplan.top

Java: String.join(", ", list)
来源：http://nhy.cucudq.cn

Go:   strings.Join(strs, ", ")
来源：http://dgg.zhijiandao.cn

Ruby: arr.join(", ")
来源：http://efk.bbcook.cn

C#:   string.Join(", ", list)
来源：http://sqf.kuanghao11.cn


<!-- 参考信息 -->