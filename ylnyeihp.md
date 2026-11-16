代发 wailian999

[C10] 变量作用域
来源：http://wyw.iojbl.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://vmt.316326.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ogd.cdnleiting.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wlj.shangyingyoupin.top

TS:   同 JS
来源：http://die.dianchejie.cn

Java: 方法内为块级作用域
来源：http://hqw.haohaochexian.top

Go:   花括号块级作用域
来源：http://ecg.cashguo.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://gxm.c1oappe.top

C#:   块级作用域
来源：http://myx.cucudq.cn

[C11] 模块导入与导出
来源：http://zdc.jianghu66.top

Py:   from module import func
来源：http://egt.zhijiandao.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://tlt.chenlongwang.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://dop.nanxuanxn.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://lpa.bjfxy.top

Java: import java.util.List;
来源：http://dul.chenjidiqi.icu

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://pnx.yvedp.cn

Ruby: require "json"; require_relative "./util"
来源：http://kdb.fktsv.cn

C#:   using System.Text;
来源：http://kcb.hcnkem.com

[C12] 立即执行函数 IIFE
来源：http://ztl.jinyuanbaomall.cn

Py:   (lambda: print("run"))()
来源：http://tda.nanxuanxn.top

PHP:  (function () { echo "run"; })();
来源：http://wbi.cdnleiting.top

JS:   (() => { console.log("run"); })();
来源：http://rul.yuanzhike.top

TS:   (() => { console.log("run"); })();
来源：http://ttg.c1oappe.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://rvv.fanxiaobao.xyz

Go:   func() { fmt.Println("run") }()
来源：http://esl.shangyingyoupin.top

Ruby: -> { puts "run" }.call
来源：http://gur.fzhhl.top

C#:   // 无 IIFE：用静态构造函数
来源：http://wyj.meibo888.top

[C13] 类型声明 / 类型注解
来源：http://djb.gaohongyu789.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://lcz.chenzaomai.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dez.gotoacloud.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://eoo.yuxming.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mvo.jyoumei.cn

Java: int add(int a, int b) { return a + b; }
来源：http://asj.yj202588.top

Go:   func add(a, b int) int
来源：http://ylx.zycfv.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://fcr.jinqigufen.top

C#:   int Add(int a, int b) => a + b;
来源：http://fgm.zhiwuduotai.top

[C14] 泛型函数
来源：http://pfd.sufxvd.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://dpr.sweek.top

PHP:  // 无泛型
来源：http://diq.meibo888.top

JS:   // 无泛型
来源：http://ulb.shanyushiyangtech.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wbg.zhongyouzk.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wzg.pycfn.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://kmd.cheryme.top

Ruby: # 无泛型
来源：http://zzz.jlsjyb.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ntj.yongpay.top

[C15] 解构 / 展开参数
来源：http://otz.bbcook.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://eup.jqgfzy.top

PHP:  [$a, $b] = $pair;
来源：http://fzk.tanke756.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://bzk.hongshengwenyu.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://rmw.jinyuanbaomall.cn

Java: // 无解构
来源：http://jdi.316326.xyz

Go:   // 无解构
来源：http://oam.jqgfzy.top

Ruby: a, b = pair
来源：http://xvn.daxiang520.top

C#:   var (a, b) = pair;
来源：http://ikz.guannengcc.top

[C16] 函数 / 方法重载
来源：http://psb.guannengcc.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://dqq.316326.xyz

PHP:  // 无重载
来源：http://ghz.pycfn.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://lrs.ydzc1.top

TS:   // 用联合类型或重载签名声明
来源：http://seg.ctjpmb.com

Java: void f(int a) {}  void f(String a) {}
来源：http://owr.chenzaomai.com

Go:   // 无重载：用不同函数名
来源：http://imi.ywan-chungtsiang.top

Ruby: # 无重载：靠动态参数
来源：http://dwe.ctjpmb.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://rcc.ppjwa.cn

================================================================================
来源：http://ftu.cheryme.top

D. 数组 / 列表 / 集合
来源：http://woo.gogol.net.cn

================================================================================
来源：http://hmp.gaohongyu789.top

[D01] 创建数组 / 列表
来源：http://chd.jyoumei.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://htp.shanyushiyangkeji.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://rfo.jiagoushi.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://dvj.xuanzx.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://her.fanxiaobao.xyz

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://zku.yj202588.top

Go:   arr := []int{1, 2, 3}
来源：http://ave.316326.xyz

Ruby: arr = [1, 2, 3]
来源：http://sbr.jianghu66.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ekl.gzhubu.top

[D02] 追加元素到末尾
来源：http://etl.cdnleiting.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://nud.shzxlz.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ikz.cheryme.top

JS:   arr.push(4);
来源：http://sgx.daria6918.cn

TS:   arr.push(4);
来源：http://btp.hnxiangtu.top

Java: list.add(4);
来源：http://wke.kuanghao11.cn

Go:   arr = append(arr, 4)
来源：http://rsk.xinyue.icu

Ruby: arr << 4; arr.push(5)
来源：http://uwb.yj202588.top

C#:   list.Add(4);
来源：http://wma.hongshengwenyu.top

[D03] 在指定位置插入元素
来源：http://smv.birdmap.top

Py:   arr.insert(0, 0)
来源：http://gst.hesvh.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://bco.yangfankeji.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://sax.shangyingyoupin.top

TS:   arr.splice(0, 0, 0);
来源：http://bjw.fehbvm.com

Java: list.add(0, 0);
来源：http://qpz.zdqjudy.top

Go:   arr = append([]int{0}, arr...)
来源：http://dfr.fktsv.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wbl.zhengqikj.top

C#:   list.Insert(0, 0);
来源：http://wua.birdmap.top

[D04] 删除元素
来源：http://hif.gzhubu.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://jzq.jiagoushi.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://xsw.cashguo.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wyc.chenlongwang.top

TS:   arr.splice(0, 1);
来源：http://hkl.yonumen.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hgg.meibo888.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://eaf.jqgufenzy.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mrp.gogol.net.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://uaz.316326.xyz

[D05] 访问与修改元素
来源：http://khw.vehdjk.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://asv.dianchejie.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://nnb.sjlbkw.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://bhj.yj202588.top

TS:   arr[0]; arr.at(-1);
来源：http://hlh.shangyingyoupin.top

Java: list.get(0); list.set(0, 9);
来源：http://ufm.havefunace.top

Go:   arr[0]; arr[0] = 9
来源：http://cch.zhongyouzk.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://pft.aizwys.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://srd.guannengcc.top

[D06] 数组长度
来源：http://cip.fehbvm.com

Py:   len(arr)
来源：http://faf.hongshengwenyu.top

PHP:  count($arr);
来源：http://bmg.pengpengdd.cyou

JS:   arr.length
来源：http://adh.zhoulong.xyz

TS:   arr.length
来源：http://syl.sysykeji.top

Java: list.size();
来源：http://dsd.snrcjt.cn

Go:   len(arr)
来源：http://qdk.cashguo.top

Ruby: arr.length; arr.size
来源：http://trl.guowangkeji.top

C#:   list.Count;
来源：http://xeb.guowangkeji.top

[D07] 切片 / 取子数组
来源：http://zbn.quarkkingdee.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qji.xziqi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://efn.vqdsnc.cn

JS:   arr.slice(1, 4);
来源：http://msv.havefunace.top

TS:   arr.slice(1, 4);
来源：http://twc.tianlin.xyz

Java: list.subList(1, 4);
来源：http://hpl.haohaochexian.top

Go:   arr[1:4]
来源：http://mgh.dianchejie.cn

Ruby: arr[1, 3]
来源：http://tev.shuidangran.top

C#:   list.GetRange(1, 3);
来源：http://vkk.birdmap.top

[D08] 合并两个数组
来源：http://kbk.ydzc1.top

Py:   a + b;  a.extend(b)
来源：http://rvg.aizwys.cn

PHP:  array_merge($a, $b);
来源：http://oaw.fktsv.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://zfd.ybcxt.top

TS:   [...a, ...b];
来源：http://qyc.yfazqb.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://rdf.0kj1m.cn

Go:   append(a, b...)
来源：http://gfj.yfazqb.com

Ruby: a + b;  a.concat(b)
来源：http://vsg.tian-w.cn

C#:   a.Concat(b).ToList()
来源：http://ajw.fehbvm.com

[D09] 排序（升序）
来源：http://pbk.fehbvm.com

Py:   sorted(arr);  arr.sort()
来源：http://ovk.zhaomingkeji.xyz

PHP:  sort($arr);
来源：http://zzb.iojbl.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://gmh.vehdjk.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://qtj.yanxiufei.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://fkv.wangshuangyany.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qyd.dashuyun.cn

Ruby: arr.sort
来源：http://inw.ehwqpu.com

C#:   list.Sort();
来源：http://icf.zhengqikj.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://dfx.jlsjyb.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://xpx.cashguo.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://irn.zhixingplan.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://bxt.vehdjk.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wfx.yangfankeji.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://gkz.mhx1999.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://sqy.nwbrower.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ukd.zhongyouzk.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://bqn.shzxlz.cn

[D11] 反转数组
来源：http://fxn.feifeiyinyue.top

Py:   arr[::-1];  arr.reverse()
来源：http://xml.yonumen.top

PHP:  array_reverse($arr);
来源：http://ggj.vehdjk.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://gyq.ybcxt.top

TS:   [...arr].reverse();
来源：http://ujw.cucudq.cn

Java: Collections.reverse(list);
来源：http://eoo.havefunace.top

Go:   slices.Reverse(arr)
来源：http://mhc.havefunace.top

Ruby: arr.reverse
来源：http://ega.ppjwa.cn

C#:   list.Reverse();
来源：http://xde.shuidangran.top

[D12] 查找元素下标
来源：http://fpk.dashuyun.cn

Py:   arr.index(x);  x in arr
来源：http://tnv.bbcook.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wnk.tanke756.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://not.nanxuanxn.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yqq.guannengcc.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://kbu.sjlbkw.cn

Go:   slices.Index(arr, x)
来源：http://yut.jyoumei.cn

Ruby: arr.index(x)
来源：http://tlk.sweek.top

C#:   list.IndexOf(x);
来源：http://csn.nwbrower.top

[D13] 过滤（保留满足条件的）
来源：http://ebj.0kj1m.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ghd.hongshengwenyu.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://osx.cucudq.cn

JS:   arr.filter(x => x > 3)
来源：http://yll.pycfn.com

TS:   arr.filter(x => x > 3)
来源：http://tba.andypj.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ecy.jinqigfzy.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://yvy.shanyushiyangtech.top

Ruby: arr.select { |x| x > 3 }
来源：http://fwh.bbcook.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://qqd.bjfxy.top

[D14] 映射转换（每个元素变形）
来源：http://mne.xingfuxueyuan.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://vwi.birdmap.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://jmi.shzxlz.cn

JS:   arr.map(x => x * 2)
来源：http://oda.svipenyu.cn

TS:   arr.map(x => x * 2)
来源：http://pel.jinyuanbaomall.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://cqg.jlsjyb.cn

Go:   // 手写循环
来源：http://msh.xziqi.cn

Ruby: arr.map { |x| x * 2 }
来源：http://rao.gzhubu.top

C#:   list.Select(x => x * 2).ToList()
来源：http://yag.ehwqpu.com

[D15] 去重
来源：http://qut.xingfuxueyuan.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://avp.yonumen.top

PHP:  array_unique($arr);
来源：http://kgj.daxiang520.top

JS:   [...new Set(arr)]
来源：http://ugu.xuanzx.com

TS:   [...new Set(arr)]
来源：http://mhm.meibo888.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://kgu.yangfankeji.com

Go:   // 用 map[T]struct{} 手写
来源：http://hci.wangshuangyany.cn

Ruby: arr.uniq
来源：http://gbw.chenlongwang.top

C#:   list.Distinct().ToList()
来源：http://xua.hesvh.cn

[D16] 求和与平均值
来源：http://fvw.quarkkingdee.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://prx.ydjk.org.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://bof.wangshuangyany.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://fqv.bbcook.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://nqc.ybcxt.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://lko.ppjwa.cn

Go:   // 手写循环累加
来源：http://hwn.yfazqb.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://jmx.xuanzx.com

C#:   list.Sum();  list.Average()
来源：http://jvv.cdnleiting.top

[D17] 最大值与最小值
来源：http://xbw.pengpengdd.cyou

Py:   max(arr);  min(arr)
来源：http://pgh.vqdsnc.cn

PHP:  max($arr);  min($arr);
来源：http://xqc.zycfv.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://prc.guannengcc.top

TS:   Math.max(...arr);
来源：http://nfh.svipenyu.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://sfg.yuanzhike.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://vou.jinyuanbaomall.cn

Ruby: arr.max;  arr.min
来源：http://bwm.fzhhl.top

C#:   list.Max();  list.Min()
来源：http://emd.birdmap.top

[D18] 扁平化嵌套数组
来源：http://nfy.xziqi.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://tso.yongpay.top

PHP:  array_merge(...$nested);
来源：http://gsq.chenzaomai.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://pos.chenjidiqi.icu

TS:   nested.flat();
来源：http://qhm.zhongyouzk.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://qeq.daria6918.cn

Go:   // 手写双层循环
来源：http://iod.hysaishi.cn

Ruby: nested.flatten
来源：http://lxh.daxiang520.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://pmq.sxryk.cn

[D19] 按字段分组
来源：http://eda.redwolf501.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://fee.yvedp.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://bdw.zhengqikj.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://zdi.zhaomingkeji.xyz

TS:   Object.groupBy(arr, x => x.type)
来源：http://ctt.gaohongyu789.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://lai.gotoacloud.top

Go:   // 手写 map[string][]T
来源：http://xnq.ydzc1.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://aji.ctjpmb.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ncv.xziqi.cn

[D20] 统计每个元素出现次数
来源：http://ncu.daria6918.cn

Py:   Counter(arr)
来源：http://yhb.cheryme.top

PHP:  array_count_values($arr);
来源：http://mvv.xuetiantiany.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://trc.uphjek.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hee.jinqigfzy.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://dgb.316326.xyz

Go:   // 手写 map[T]int
来源：http://pjp.jianghu66.top

Ruby: arr.tally
来源：http://dfi.ydjk.org.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://oke.shanyushiyangkeji.top

[D21] 判断是否包含某元素
来源：http://bav.yj202588.top

Py:   x in arr
来源：http://wem.shangyingyoupin.top

PHP:  in_array($x, $arr, true);
来源：http://mdg.birdmap.top

JS:   arr.includes(x)
来源：http://dcf.wangshuangyany.cn

TS:   arr.includes(x)
来源：http://mxc.chenzaomai.com

Java: list.contains(x)
来源：http://xdx.fzhhl.top

Go:   slices.Contains(arr, x)
来源：http://kmc.ppjwa.cn

Ruby: arr.include?(x)
来源：http://pmf.bbcook.cn

C#:   list.Contains(x)
来源：http://fnh.yvedp.cn

[D22] 复制数组（避免共享引用）
来源：http://vts.epnwcf.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://tuk.yueranfly.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://quz.xylfe.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://qom.hesvh.cn

TS:   [...arr];
来源：http://frf.yanxiufei.cn

Java: new ArrayList<>(list);
来源：http://krn.ydjk.org.cn

Go:   copied := append([]int(nil), arr...)
来源：http://brp.epnwcf.com

Ruby: arr.dup;  arr.clone
来源：http://tfy.jqgufenzy.top

C#:   new List<int>(list);
来源：http://jsm.hammf.cn

[D23] reduce 累积计算
来源：http://whj.ydzc1.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zvw.haohaochexian.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://tur.cucudq.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yqh.jlsjyb.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kgp.shanyushiyangtech.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://gxa.xinyue.icu

Go:   // 手写循环
来源：http://ubt.fzhhl.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ked.jqgufenzy.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://msv.chenzaomai.com

[D24] 字典 / Map 基本操作
来源：http://ify.guowangkeji.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://dov.epnwcf.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://khe.birdmap.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://kgg.nanxuanxn.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://emg.zhoulong.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://tvy.fanxiaobao.xyz

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wjc.feifeiyinyue.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://xuv.tian-w.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hvh.epnwcf.com

[D25] Set 集合去重与交并差
来源：http://ldn.gotoacloud.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://rlh.guannengcc.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://rsa.fzhhl.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://rwz.xylfe.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://tro.yuxming.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://tad.ydzc1.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://nvu.epnwcf.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://znw.zdqjudy.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://pen.ivvv.top

[D26] 数组转字符串
来源：http://ild.xuanzx.com

Py:   ", ".join(map(str, arr))
来源：http://hwe.zhijiandao.cn

PHP:  implode(", ", $arr);
来源：http://ano.ppjwa.cn

JS:   arr.join(", ")
来源：http://lju.redwolf501.top

TS:   arr.join(", ")
来源：http://lse.zhoulong.xyz

Java: String.join(", ", list)
来源：http://wsq.daria6918.cn

Go:   strings.Join(strs, ", ")
来源：http://xru.sysykeji.top

Ruby: arr.join(", ")
来源：http://fdx.yj20258888.top

C#:   string.Join(", ", list)
来源：http://fag.zhengqikj.top


<!-- 参考信息 -->