代发 wailian999

[C10] 变量作用域
来源：http://ddq.9152youxi.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://jbq.0kj1m.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wjz.zhijiandao.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://bph.zhoulong.xyz

TS:   同 JS
来源：http://yhf.bbcook.cn

Java: 方法内为块级作用域
来源：http://xew.yongpay.top

Go:   花括号块级作用域
来源：http://rig.ivvv.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://nrb.yj20258.top

C#:   块级作用域
来源：http://qkl.kuanghao11.cn

[C11] 模块导入与导出
来源：http://oak.tianlin.xyz

Py:   from module import func
来源：http://prj.dashuyun.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://cub.nwbrower.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://kzw.havefunace.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hzx.yuanzhike.top

Java: import java.util.List;
来源：http://sfb.yj20258888.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://dek.yj20258.top

Ruby: require "json"; require_relative "./util"
来源：http://yct.chenlongwang.top

C#:   using System.Text;
来源：http://yxm.jinqigfzy.top

[C12] 立即执行函数 IIFE
来源：http://qbx.cashguo.top

Py:   (lambda: print("run"))()
来源：http://gfw.chenlongwang.top

PHP:  (function () { echo "run"; })();
来源：http://dgw.quarkkingdee.top

JS:   (() => { console.log("run"); })();
来源：http://wzy.uphjek.com

TS:   (() => { console.log("run"); })();
来源：http://oko.bjfxy.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://abr.guannengcc.top

Go:   func() { fmt.Println("run") }()
来源：http://ftk.zhixingplan.top

Ruby: -> { puts "run" }.call
来源：http://ygn.zhijiandao.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://owh.meibo888.top

[C13] 类型声明 / 类型注解
来源：http://ovw.sufxvd.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://oro.hammf.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ukj.9152youxi.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://zqq.yuxming.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ynm.jlsjyb.cn

Java: int add(int a, int b) { return a + b; }
来源：http://blq.kuanghao11.cn

Go:   func add(a, b int) int
来源：http://tae.0kj1m.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://xrq.ywan-chungtsiang.top

C#:   int Add(int a, int b) => a + b;
来源：http://gsq.jqgufenzy.top

[C14] 泛型函数
来源：http://wnj.gaohongyu789.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hon.snrcjt.cn

PHP:  // 无泛型
来源：http://llf.ehwqpu.com

JS:   // 无泛型
来源：http://tns.yj20258888.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://dwu.pycfn.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mkd.iojbl.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://qxf.wangshuangyany.cn

Ruby: # 无泛型
来源：http://zrh.316326.xyz

C#:   static T First<T>(List<T> items) => items[0];
来源：http://uza.jinqigfzy.top

[C15] 解构 / 展开参数
来源：http://pmv.yfazqb.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://brv.fehbvm.com

PHP:  [$a, $b] = $pair;
来源：http://thk.sweek.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xpg.ppjwa.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hme.nwbrower.top

Java: // 无解构
来源：http://rio.0kj1m.cn

Go:   // 无解构
来源：http://kch.jqgfzy.top

Ruby: a, b = pair
来源：http://juo.snrcjt.cn

C#:   var (a, b) = pair;
来源：http://jhs.xziqi.cn

[C16] 函数 / 方法重载
来源：http://sez.zhoulong.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://anc.jinqigufen.top

PHP:  // 无重载
来源：http://uqu.hnqzz.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://pxp.birdmap.top

TS:   // 用联合类型或重载签名声明
来源：http://hmh.316326.xyz

Java: void f(int a) {}  void f(String a) {}
来源：http://vlc.andypj.xyz

Go:   // 无重载：用不同函数名
来源：http://euw.zhongyouzk.top

Ruby: # 无重载：靠动态参数
来源：http://pgz.guannengcc.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://zfv.sweek.top

================================================================================
来源：http://yjf.snrcjt.cn

D. 数组 / 列表 / 集合
来源：http://xkj.ppjwa.cn

================================================================================
来源：http://vqc.epnwcf.com

[D01] 创建数组 / 列表
来源：http://irj.andypj.xyz

Py:   arr = [1, 2, 3];  empty = []
来源：http://xbo.kuanghao11.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://rsy.ydjk.org.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ksy.yuanzhike.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://maf.jyoumei.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://noi.quarkkingdee.top

Go:   arr := []int{1, 2, 3}
来源：http://fri.aizwys.cn

Ruby: arr = [1, 2, 3]
来源：http://tjo.ctjpmb.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://cch.zhaomingkeji.xyz

[D02] 追加元素到末尾
来源：http://sbl.zhijiandao.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://feg.kuanghao11.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hpi.epnwcf.com

JS:   arr.push(4);
来源：http://tch.aibaodan.cn

TS:   arr.push(4);
来源：http://fql.0kj1m.cn

Java: list.add(4);
来源：http://nmt.0kj1m.cn

Go:   arr = append(arr, 4)
来源：http://yex.daria6918.cn

Ruby: arr << 4; arr.push(5)
来源：http://anz.chenlongwang.top

C#:   list.Add(4);
来源：http://ubw.quarkkingdee.top

[D03] 在指定位置插入元素
来源：http://msa.zhaomingkeji.xyz

Py:   arr.insert(0, 0)
来源：http://zmr.pycfn.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://uen.hcnkem.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ewq.smart0.xyz

TS:   arr.splice(0, 0, 0);
来源：http://uai.jinqigfzy.top

Java: list.add(0, 0);
来源：http://kqc.wangshuangyany.cn

Go:   arr = append([]int{0}, arr...)
来源：http://hlj.jinghuilouyu.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://umn.shuidangran.top

C#:   list.Insert(0, 0);
来源：http://ven.gogol.net.cn

[D04] 删除元素
来源：http://nvr.pycfn.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://zhs.yonumen.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wfc.vqdsnc.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://cxb.yuanzhike.top

TS:   arr.splice(0, 1);
来源：http://izg.jinqigufen.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://lus.ctjpmb.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://zyx.wangshuangyany.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://qcj.hysaishi.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://car.daxiang520.top

[D05] 访问与修改元素
来源：http://tbf.zhengqikj.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hif.jqgfzy.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://idp.sjlbkw.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://kal.xingfuxueyuan.xyz

TS:   arr[0]; arr.at(-1);
来源：http://mxb.jinghuilouyu.cn

Java: list.get(0); list.set(0, 9);
来源：http://vyy.sxryk.cn

Go:   arr[0]; arr[0] = 9
来源：http://kcd.sysykeji.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://tql.hnqzz.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://svh.9152youxi.cn

[D06] 数组长度
来源：http://usf.jinqigufen.top

Py:   len(arr)
来源：http://tbj.gotoacloud.top

PHP:  count($arr);
来源：http://qej.daxiang520.top

JS:   arr.length
来源：http://qad.jyoumei.cn

TS:   arr.length
来源：http://wni.tian-w.cn

Java: list.size();
来源：http://xrk.hongshengwenyu.top

Go:   len(arr)
来源：http://nqs.hnxiangtu.top

Ruby: arr.length; arr.size
来源：http://zor.xylfe.cn

C#:   list.Count;
来源：http://zgf.zdqjudy.top

[D07] 切片 / 取子数组
来源：http://ner.vqdsnc.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://kcr.sjlbkw.cn

PHP:  array_slice($arr, 1, 3);
来源：http://vds.snrcjt.cn

JS:   arr.slice(1, 4);
来源：http://ctp.zycfv.cn

TS:   arr.slice(1, 4);
来源：http://qix.jyoumei.cn

Java: list.subList(1, 4);
来源：http://ikq.hesvh.cn

Go:   arr[1:4]
来源：http://jro.chenzaomai.com

Ruby: arr[1, 3]
来源：http://xxc.yj20258.top

C#:   list.GetRange(1, 3);
来源：http://lqg.daxiang520.top

[D08] 合并两个数组
来源：http://kdm.xylfe.cn

Py:   a + b;  a.extend(b)
来源：http://blw.fengsongda.top

PHP:  array_merge($a, $b);
来源：http://tmn.zhengqikj.top

JS:   [...a, ...b];  a.concat(b);
来源：http://iwz.sysykeji.top

TS:   [...a, ...b];
来源：http://fwx.jqgfzy.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hhy.gaohongyu789.top

Go:   append(a, b...)
来源：http://xdr.sxryk.cn

Ruby: a + b;  a.concat(b)
来源：http://lzr.zhijiandao.cn

C#:   a.Concat(b).ToList()
来源：http://qqd.cqqwz.cn

[D09] 排序（升序）
来源：http://tws.sjlbkw.cn

Py:   sorted(arr);  arr.sort()
来源：http://trv.sxryk.cn

PHP:  sort($arr);
来源：http://krm.c1oappe.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://epw.yangfankeji.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://bpf.jianghu66.top

Java: Collections.sort(list);  list.sort(null);
来源：http://mmx.nanxinkj.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://eqp.zdbjq.cn

Ruby: arr.sort
来源：http://ouc.yuanzhike.top

C#:   list.Sort();
来源：http://yek.yj202588.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://ere.smart0.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://foh.ppjwa.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wkf.hfpthk.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://tgr.nanxuanxn.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fgj.guowangkeji.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://qsv.c1oappe.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://btd.hnqzz.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://aup.ehwqpu.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://itv.jianghu66.top

[D11] 反转数组
来源：http://akn.yvedp.cn

Py:   arr[::-1];  arr.reverse()
来源：http://xkz.yuxming.cn

PHP:  array_reverse($arr);
来源：http://xbp.nwbrower.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://rcc.xingfuxueyuan.xyz

TS:   [...arr].reverse();
来源：http://ndj.zdqjudy.top

Java: Collections.reverse(list);
来源：http://rau.c1oappe.top

Go:   slices.Reverse(arr)
来源：http://wmk.yueranfly.top

Ruby: arr.reverse
来源：http://fam.fktsv.cn

C#:   list.Reverse();
来源：http://lia.dianchejie.cn

[D12] 查找元素下标
来源：http://wpi.ywan-chungtsiang.top

Py:   arr.index(x);  x in arr
来源：http://dfi.ivvv.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ibm.guowangkeji.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wxo.epnwcf.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dar.zdbjq.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://kyf.cheryme.top

Go:   slices.Index(arr, x)
来源：http://upw.haohaochexian.top

Ruby: arr.index(x)
来源：http://wfa.ivvv.top

C#:   list.IndexOf(x);
来源：http://dgh.hysaishi.cn

[D13] 过滤（保留满足条件的）
来源：http://rxl.tianlin.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://pfu.yfazqb.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://cyt.jinghuilouyu.cn

JS:   arr.filter(x => x > 3)
来源：http://mgo.haohaochexian.top

TS:   arr.filter(x => x > 3)
来源：http://ziq.zhongyouzk.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://jjx.hnxiangtu.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://uxi.chenjidiqi.icu

Ruby: arr.select { |x| x > 3 }
来源：http://fle.chenlongwang.top

C#:   list.Where(x => x > 3).ToList()
来源：http://kqm.hysaishi.cn

[D14] 映射转换（每个元素变形）
来源：http://njj.aizwys.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ptt.epnwcf.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://qeu.yj20258888.top

JS:   arr.map(x => x * 2)
来源：http://wgq.snrcjt.cn

TS:   arr.map(x => x * 2)
来源：http://buw.hongshengwenyu.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://bhm.sweek.top

Go:   // 手写循环
来源：http://emx.zycfv.cn

Ruby: arr.map { |x| x * 2 }
来源：http://vdz.cdnleiting.top

C#:   list.Select(x => x * 2).ToList()
来源：http://hzu.jianghu66.top

[D15] 去重
来源：http://vxu.epnwcf.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://lgz.jqgufenzy.top

PHP:  array_unique($arr);
来源：http://tmi.hesvh.cn

JS:   [...new Set(arr)]
来源：http://qgo.yuanzhike.top

TS:   [...new Set(arr)]
来源：http://gjh.bjfxy.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://nuf.daria6918.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ejz.hnxiangtu.top

Ruby: arr.uniq
来源：http://gtk.kuanghao11.cn

C#:   list.Distinct().ToList()
来源：http://zkj.jinyuanbaomall.cn

[D16] 求和与平均值
来源：http://fwz.jinqigufen.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ssf.kuanghao11.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://pvs.mhx1999.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://zte.iojbl.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://rvy.shzxlz.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://akm.redwolf501.top

Go:   // 手写循环累加
来源：http://uco.zhaomingkeji.xyz

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://dvp.havefunace.top

C#:   list.Sum();  list.Average()
来源：http://mtf.sjlbkw.cn

[D17] 最大值与最小值
来源：http://djo.chenlongwang.top

Py:   max(arr);  min(arr)
来源：http://qkg.xuanzx.com

PHP:  max($arr);  min($arr);
来源：http://xnf.aizwys.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://dfj.316326.xyz

TS:   Math.max(...arr);
来源：http://bcu.zhaomingkeji.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://teh.316326.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://lmy.yfazqb.com

Ruby: arr.max;  arr.min
来源：http://sji.bjfxy.top

C#:   list.Max();  list.Min()
来源：http://dwz.snrcjt.cn

[D18] 扁平化嵌套数组
来源：http://dxu.jlsjyb.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wjy.wangshuangyany.cn

PHP:  array_merge(...$nested);
来源：http://xjz.jqgufenzy.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://tqs.tian-w.cn

TS:   nested.flat();
来源：http://qgs.nwbrower.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jdf.nwbrower.top

Go:   // 手写双层循环
来源：http://eeo.fktsv.cn

Ruby: nested.flatten
来源：http://kzw.snrcjt.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://sje.316326.xyz

[D19] 按字段分组
来源：http://hmm.ywan-chungtsiang.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://jpv.yuxming.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://jxc.svipenyu.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mga.ehwqpu.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://hjg.ctjpmb.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://fbt.ivvv.top

Go:   // 手写 map[string][]T
来源：http://ylq.316326.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://nkj.gogol.net.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://tvf.yj20258.top

[D20] 统计每个元素出现次数
来源：http://wdo.zhoulong.xyz

Py:   Counter(arr)
来源：http://vim.sysykeji.top

PHP:  array_count_values($arr);
来源：http://ilz.hammf.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://geh.snrcjt.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xoy.hammf.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://zmk.hysaishi.cn

Go:   // 手写 map[T]int
来源：http://izc.redwolf501.top

Ruby: arr.tally
来源：http://quv.ctjpmb.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://azg.shangyingyoupin.top

[D21] 判断是否包含某元素
来源：http://qtm.fanxiaobao.xyz

Py:   x in arr
来源：http://xsf.xuetiantiany.cn

PHP:  in_array($x, $arr, true);
来源：http://yim.jyoumei.cn

JS:   arr.includes(x)
来源：http://xgs.cdnleiting.top

TS:   arr.includes(x)
来源：http://duy.zhaomingkeji.xyz

Java: list.contains(x)
来源：http://pyh.jlsjyb.cn

Go:   slices.Contains(arr, x)
来源：http://pen.snrcjt.cn

Ruby: arr.include?(x)
来源：http://rrx.gotoacloud.top

C#:   list.Contains(x)
来源：http://gcf.yuanzhike.top

[D22] 复制数组（避免共享引用）
来源：http://slp.jianghu66.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ydo.zdqjudy.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://yjm.tarul.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://toq.uphjek.com

TS:   [...arr];
来源：http://kwj.xuanzx.com

Java: new ArrayList<>(list);
来源：http://wdk.smart0.xyz

Go:   copied := append([]int(nil), arr...)
来源：http://kxm.zdqjudy.top

Ruby: arr.dup;  arr.clone
来源：http://fsk.zhixingplan.top

C#:   new List<int>(list);
来源：http://uov.0kj1m.cn

[D23] reduce 累积计算
来源：http://zzu.jinyuanbaomall.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zyj.vehdjk.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://bbs.jinqigfzy.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jma.cheryme.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://naa.jinqigfzy.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://smv.pycfn.com

Go:   // 手写循环
来源：http://sof.jinqigufen.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://nor.zhiwuduotai.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://pwd.hysaishi.cn

[D24] 字典 / Map 基本操作
来源：http://ghb.hcnkem.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://bqd.ivvv.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://iia.cdnleiting.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hbk.ywan-chungtsiang.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://qgz.xylfe.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://yrj.zhengqikj.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://jkg.pycfn.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ldj.bjfxy.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://gez.meibo888.top

[D25] Set 集合去重与交并差
来源：http://cez.jinyuanbaomall.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://pxr.ybcxt.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ycv.sysykeji.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://xjt.yj20258888.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://zeq.aibaodan.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://rgl.tian-w.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://scq.svipenyu.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://cju.ybcxt.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://zly.sweek.top

[D26] 数组转字符串
来源：http://tys.fanxiaobao.xyz

Py:   ", ".join(map(str, arr))
来源：http://zrz.ybcxt.top

PHP:  implode(", ", $arr);
来源：http://reg.hcnkem.com

JS:   arr.join(", ")
来源：http://dxp.jiagoushi.top

TS:   arr.join(", ")
来源：http://hvu.jinqigufen.top

Java: String.join(", ", list)
来源：http://wzj.zhongyouzk.top

Go:   strings.Join(strs, ", ")
来源：http://ebz.hnqzz.top

Ruby: arr.join(", ")
来源：http://app.sufxvd.cn

C#:   string.Join(", ", list)
来源：http://gxn.fengsongda.top


<!-- 参考信息 -->