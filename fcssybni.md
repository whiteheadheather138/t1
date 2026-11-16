代发 wailian999

[C10] 变量作用域
来源：http://mih.tarul.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://jca.chenjidiqi.icu

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://agr.xuetiantiany.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://opb.yuanzhike.top

TS:   同 JS
来源：http://tbq.aizwys.cn

Java: 方法内为块级作用域
来源：http://eam.hnqzz.top

Go:   花括号块级作用域
来源：http://qjl.xingfuxueyuan.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://see.pengpengdd.cyou

C#:   块级作用域
来源：http://iex.daxiang520.top

[C11] 模块导入与导出
来源：http://oyb.ydjk.org.cn

Py:   from module import func
来源：http://lgy.shangyingyoupin.top

PHP:  require "file.php";  或 use App\Service;
来源：http://cmz.shanyushiyangkeji.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://fpu.zhiwuduotai.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wna.fktsv.cn

Java: import java.util.List;
来源：http://eqq.tanke756.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://fjx.yj20258.top

Ruby: require "json"; require_relative "./util"
来源：http://hds.ppjwa.cn

C#:   using System.Text;
来源：http://ogb.cucudq.cn

[C12] 立即执行函数 IIFE
来源：http://sdx.chenzaomai.com

Py:   (lambda: print("run"))()
来源：http://ecc.jyoumei.cn

PHP:  (function () { echo "run"; })();
来源：http://yfl.nanxinkj.top

JS:   (() => { console.log("run"); })();
来源：http://soi.cucudq.cn

TS:   (() => { console.log("run"); })();
来源：http://hzs.zhiwuduotai.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://boy.fktsv.cn

Go:   func() { fmt.Println("run") }()
来源：http://tuc.chenlongwang.top

Ruby: -> { puts "run" }.call
来源：http://uqv.zhixingplan.top

C#:   // 无 IIFE：用静态构造函数
来源：http://xay.hfpthk.cn

[C13] 类型声明 / 类型注解
来源：http://flz.cheryme.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://xet.snrcjt.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kur.316326.xyz

JS:   // 无类型（可用 JSDoc 注释）
来源：http://txf.gotoacloud.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xhs.svipenyu.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ykz.wangdashe.top

Go:   func add(a, b int) int
来源：http://obi.hysaishi.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://yns.fengsongda.top

C#:   int Add(int a, int b) => a + b;
来源：http://nlz.zhaomingkeji.xyz

[C14] 泛型函数
来源：http://gai.sjlbkw.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zlw.hcnkem.com

PHP:  // 无泛型
来源：http://vpz.yuxming.cn

JS:   // 无泛型
来源：http://qkk.yonumen.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://kar.sysykeji.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ebk.shanyushiyangkeji.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://osv.jyoumei.cn

Ruby: # 无泛型
来源：http://wzl.shuidangran.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://frv.gogol.net.cn

[C15] 解构 / 展开参数
来源：http://mkg.zhijiandao.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ial.feifeiyinyue.top

PHP:  [$a, $b] = $pair;
来源：http://req.jianghu66.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://atz.cucudq.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://jmn.tanke756.top

Java: // 无解构
来源：http://goo.jqgufenzy.top

Go:   // 无解构
来源：http://vlu.jlsjyb.cn

Ruby: a, b = pair
来源：http://nzb.guannengcc.top

C#:   var (a, b) = pair;
来源：http://bgt.chenzaomai.com

[C16] 函数 / 方法重载
来源：http://ltq.jinqigfzy.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ysp.yongpay.top

PHP:  // 无重载
来源：http://gvs.ppjwa.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://fjg.iojbl.cn

TS:   // 用联合类型或重载签名声明
来源：http://xbl.shangyingyoupin.top

Java: void f(int a) {}  void f(String a) {}
来源：http://jlb.52xcode.cn

Go:   // 无重载：用不同函数名
来源：http://igu.snrcjt.cn

Ruby: # 无重载：靠动态参数
来源：http://ffz.hnxiangtu.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://ueh.hesvh.cn

================================================================================
来源：http://ttf.cucudq.cn

D. 数组 / 列表 / 集合
来源：http://tko.ppjwa.cn

================================================================================
来源：http://wfa.yongpay.top

[D01] 创建数组 / 列表
来源：http://vbj.dashuyun.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://egm.tanke756.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ubr.ppjwa.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://bkg.cqqwz.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://hou.xuanzx.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://bxz.cqqwz.cn

Go:   arr := []int{1, 2, 3}
来源：http://vmx.xylfe.cn

Ruby: arr = [1, 2, 3]
来源：http://xxa.ybcxt.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://rbd.aizwys.cn

[D02] 追加元素到末尾
来源：http://tdn.chenjidiqi.icu

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ffb.sxryk.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://osi.xingfuxueyuan.xyz

JS:   arr.push(4);
来源：http://aml.gaohongyu789.top

TS:   arr.push(4);
来源：http://ihq.birdmap.top

Java: list.add(4);
来源：http://sba.9152youxi.cn

Go:   arr = append(arr, 4)
来源：http://wmi.chenlongwang.top

Ruby: arr << 4; arr.push(5)
来源：http://bcr.shangyingyoupin.top

C#:   list.Add(4);
来源：http://ybn.pengpengdd.cyou

[D03] 在指定位置插入元素
来源：http://ctd.birdmap.top

Py:   arr.insert(0, 0)
来源：http://yuo.xuanzx.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://nsx.9152youxi.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://opy.9152youxi.cn

TS:   arr.splice(0, 0, 0);
来源：http://qjj.fengsongda.top

Java: list.add(0, 0);
来源：http://nrw.zhaomingkeji.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://glo.zhijiandao.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://xbb.chenjidiqi.icu

C#:   list.Insert(0, 0);
来源：http://ykm.quarkkingdee.top

[D04] 删除元素
来源：http://ely.zdbjq.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://glz.fehbvm.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://gsr.kuanghao11.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://jvz.feifeiyinyue.top

TS:   arr.splice(0, 1);
来源：http://eru.vehdjk.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://cht.dashuyun.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ckp.sufxvd.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://enn.yuanzhike.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://iob.tarul.cn

[D05] 访问与修改元素
来源：http://icc.hcnkem.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://sga.shanyushiyangkeji.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ttx.snrcjt.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ggl.jqgfzy.top

TS:   arr[0]; arr.at(-1);
来源：http://hnl.hfpthk.cn

Java: list.get(0); list.set(0, 9);
来源：http://nhg.daxiang520.top

Go:   arr[0]; arr[0] = 9
来源：http://lts.xuetiantiany.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://dvn.shuidangran.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ffl.guowangkeji.top

[D06] 数组长度
来源：http://zee.iojbl.cn

Py:   len(arr)
来源：http://cii.9152youxi.cn

PHP:  count($arr);
来源：http://hpw.xingfuxueyuan.xyz

JS:   arr.length
来源：http://lrw.cucudq.cn

TS:   arr.length
来源：http://zuj.svipenyu.cn

Java: list.size();
来源：http://ffc.shzxlz.cn

Go:   len(arr)
来源：http://bxd.shanyushiyangkeji.top

Ruby: arr.length; arr.size
来源：http://ehq.yj202588.top

C#:   list.Count;
来源：http://yuz.tanke756.top

[D07] 切片 / 取子数组
来源：http://zat.bbcook.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://gib.yvedp.cn

PHP:  array_slice($arr, 1, 3);
来源：http://nmr.zdqjudy.top

JS:   arr.slice(1, 4);
来源：http://uit.zhaomingkeji.xyz

TS:   arr.slice(1, 4);
来源：http://xhm.vqdsnc.cn

Java: list.subList(1, 4);
来源：http://tle.zdbjq.cn

Go:   arr[1:4]
来源：http://ztm.zhoulong.xyz

Ruby: arr[1, 3]
来源：http://jzp.guannengcc.top

C#:   list.GetRange(1, 3);
来源：http://bhm.redwolf501.top

[D08] 合并两个数组
来源：http://eot.xylfe.cn

Py:   a + b;  a.extend(b)
来源：http://gzj.vehdjk.com

PHP:  array_merge($a, $b);
来源：http://xil.ehwqpu.com

JS:   [...a, ...b];  a.concat(b);
来源：http://fqi.zycfv.cn

TS:   [...a, ...b];
来源：http://kuk.daxiang520.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://xzf.aibaodan.cn

Go:   append(a, b...)
来源：http://pmd.ehwqpu.com

Ruby: a + b;  a.concat(b)
来源：http://xgw.xingfuxueyuan.xyz

C#:   a.Concat(b).ToList()
来源：http://uwv.pengpengdd.cyou

[D09] 排序（升序）
来源：http://kky.guannengcc.top

Py:   sorted(arr);  arr.sort()
来源：http://koz.havefunace.top

PHP:  sort($arr);
来源：http://tgd.gogol.net.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://fet.hesvh.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://flc.jiagoushi.top

Java: Collections.sort(list);  list.sort(null);
来源：http://ger.xuanzx.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wto.yj202588.top

Ruby: arr.sort
来源：http://rgq.snrcjt.cn

C#:   list.Sort();
来源：http://men.zhijiandao.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://wpr.zhiwuduotai.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://osz.yj20258.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://arv.wangdashe.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://nul.snrcjt.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wml.yuanzhike.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://nat.ydzc1.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://gqm.tian-w.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://vlg.52xcode.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ebz.xingfuxueyuan.xyz

[D11] 反转数组
来源：http://pgx.jinqigufen.top

Py:   arr[::-1];  arr.reverse()
来源：http://ant.fanxiaobao.xyz

PHP:  array_reverse($arr);
来源：http://kld.zhoulong.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://prj.yongpay.top

TS:   [...arr].reverse();
来源：http://xqj.nwbrower.top

Java: Collections.reverse(list);
来源：http://bun.meibo888.top

Go:   slices.Reverse(arr)
来源：http://dpz.zdqjudy.top

Ruby: arr.reverse
来源：http://vek.yuxming.cn

C#:   list.Reverse();
来源：http://dzs.wangdashe.top

[D12] 查找元素下标
来源：http://qnc.ywan-chungtsiang.top

Py:   arr.index(x);  x in arr
来源：http://xwc.daxiang520.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://qlp.fzhhl.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jls.shanyushiyangkeji.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bng.52xcode.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://glx.jinghuilouyu.cn

Go:   slices.Index(arr, x)
来源：http://mpg.iojbl.cn

Ruby: arr.index(x)
来源：http://fhm.hnxiangtu.top

C#:   list.IndexOf(x);
来源：http://dsh.vehdjk.com

[D13] 过滤（保留满足条件的）
来源：http://rdg.zhongyouzk.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://jwa.gogol.net.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://tnn.yj20258.top

JS:   arr.filter(x => x > 3)
来源：http://crf.daxiang520.top

TS:   arr.filter(x => x > 3)
来源：http://jhe.sufxvd.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://guc.fktsv.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://zjm.shuidangran.top

Ruby: arr.select { |x| x > 3 }
来源：http://xmo.shuidangran.top

C#:   list.Where(x => x > 3).ToList()
来源：http://bvv.shanyushiyangkeji.top

[D14] 映射转换（每个元素变形）
来源：http://yli.ivvv.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://lvz.c1oappe.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://qhx.birdmap.top

JS:   arr.map(x => x * 2)
来源：http://tqh.daria6918.cn

TS:   arr.map(x => x * 2)
来源：http://lrz.hfpthk.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://lsh.daria6918.cn

Go:   // 手写循环
来源：http://dys.sxryk.cn

Ruby: arr.map { |x| x * 2 }
来源：http://jsn.xylfe.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://byi.bbcook.cn

[D15] 去重
来源：http://czk.9152youxi.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://gjf.tanke756.top

PHP:  array_unique($arr);
来源：http://lbb.chenzaomai.com

JS:   [...new Set(arr)]
来源：http://pvs.tian-w.cn

TS:   [...new Set(arr)]
来源：http://teb.hnxiangtu.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mnj.hcnkem.com

Go:   // 用 map[T]struct{} 手写
来源：http://yde.pengpengdd.cyou

Ruby: arr.uniq
来源：http://wha.jqgfzy.top

C#:   list.Distinct().ToList()
来源：http://ykv.guannengcc.top

[D16] 求和与平均值
来源：http://smz.yfazqb.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://orh.bbcook.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://vwg.yj20258888.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wiy.daxiang520.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://zwt.yanxiufei.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://otg.zhixingplan.top

Go:   // 手写循环累加
来源：http://nif.tian-w.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ron.sysykeji.top

C#:   list.Sum();  list.Average()
来源：http://huk.yangfankeji.com

[D17] 最大值与最小值
来源：http://ctg.tianlin.xyz

Py:   max(arr);  min(arr)
来源：http://net.hywenlv.cn

PHP:  max($arr);  min($arr);
来源：http://xed.vqdsnc.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://idv.shuidangran.top

TS:   Math.max(...arr);
来源：http://mvv.zhongyouzk.top

Java: Collections.max(list);  Collections.min(list);
来源：http://xhr.aizwys.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ndh.jlsjyb.cn

Ruby: arr.max;  arr.min
来源：http://dsv.yj20258888.top

C#:   list.Max();  list.Min()
来源：http://ljc.sysykeji.top

[D18] 扁平化嵌套数组
来源：http://qlu.xuetiantiany.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://opz.nanxinkj.top

PHP:  array_merge(...$nested);
来源：http://yul.nanxuanxn.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wnb.hcnkem.com

TS:   nested.flat();
来源：http://mbj.gaohongyu789.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jiw.wangshuangyany.cn

Go:   // 手写双层循环
来源：http://uep.fengsongda.top

Ruby: nested.flatten
来源：http://xss.guowangkeji.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://sda.jianghu66.top

[D19] 按字段分组
来源：http://joo.ywan-chungtsiang.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://loh.dashuyun.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qia.9152youxi.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://nll.vehdjk.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://vbg.nwbrower.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://myz.chenjidiqi.icu

Go:   // 手写 map[string][]T
来源：http://hbw.zhiwuduotai.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://wbf.sysykeji.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://zhm.hnxiangtu.top

[D20] 统计每个元素出现次数
来源：http://hpb.ppjwa.cn

Py:   Counter(arr)
来源：http://aqd.andypj.xyz

PHP:  array_count_values($arr);
来源：http://tok.jyoumei.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://csb.nanxinkj.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://aqe.zdbjq.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ocy.cheryme.top

Go:   // 手写 map[T]int
来源：http://ztp.smart0.xyz

Ruby: arr.tally
来源：http://ack.chenlongwang.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://lfl.jyoumei.cn

[D21] 判断是否包含某元素
来源：http://ipx.ydzc1.top

Py:   x in arr
来源：http://hhi.gaohongyu789.top

PHP:  in_array($x, $arr, true);
来源：http://zmc.xinyue.icu

JS:   arr.includes(x)
来源：http://mbp.hongshengwenyu.top

TS:   arr.includes(x)
来源：http://zhr.shzxlz.cn

Java: list.contains(x)
来源：http://pbl.shanyushiyangtech.top

Go:   slices.Contains(arr, x)
来源：http://rdl.guowangkeji.top

Ruby: arr.include?(x)
来源：http://sel.uphjek.com

C#:   list.Contains(x)
来源：http://lug.bbcook.cn

[D22] 复制数组（避免共享引用）
来源：http://taf.jqgfzy.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mrb.vehdjk.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://vit.birdmap.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ckf.svipenyu.cn

TS:   [...arr];
来源：http://gsp.cheryme.top

Java: new ArrayList<>(list);
来源：http://gof.hnqzz.top

Go:   copied := append([]int(nil), arr...)
来源：http://qqu.9152youxi.cn

Ruby: arr.dup;  arr.clone
来源：http://fmx.smart0.xyz

C#:   new List<int>(list);
来源：http://iat.andypj.xyz

[D23] reduce 累积计算
来源：http://iiz.smart0.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ngd.fktsv.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mnn.nwbrower.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dlg.redwolf501.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://knd.nanxuanxn.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://ksd.xylfe.cn

Go:   // 手写循环
来源：http://xbk.tian-w.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://gyq.aibaodan.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://zio.shuidangran.top

[D24] 字典 / Map 基本操作
来源：http://slo.xuanzx.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://zhu.xuetiantiany.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mhj.daria6918.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ewl.feifeiyinyue.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://bqq.0kj1m.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://rku.iojbl.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ddz.quarkkingdee.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://nwi.jianghu66.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://cji.52xcode.cn

[D25] Set 集合去重与交并差
来源：http://wgo.shangyingyoupin.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://tbv.bjfxy.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://yet.xinyue.icu

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://iah.vqdsnc.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://sfk.vehdjk.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://kbv.xylfe.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://luk.gotoacloud.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://yuj.zhaomingkeji.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://jjo.yongpay.top

[D26] 数组转字符串
来源：http://qac.hammf.cn

Py:   ", ".join(map(str, arr))
来源：http://adb.chenlongwang.top

PHP:  implode(", ", $arr);
来源：http://csh.nwbrower.top

JS:   arr.join(", ")
来源：http://lbn.fehbvm.com

TS:   arr.join(", ")
来源：http://zfi.mhx1999.top

Java: String.join(", ", list)
来源：http://kgs.yanxiufei.cn

Go:   strings.Join(strs, ", ")
来源：http://fde.epnwcf.com

Ruby: arr.join(", ")
来源：http://lqi.shanyushiyangtech.top

C#:   string.Join(", ", list)
来源：http://ubq.ehwqpu.com


<!-- 参考信息 -->