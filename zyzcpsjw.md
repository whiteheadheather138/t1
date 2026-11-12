代发 wailian999

C#:   块级作用域
来源：http://ijh.tianlin.xyz

[C11] 模块导入与导出
来源：http://qgd.xuetiantiany.cn

Py:   from module import func
来源：http://bnk.52xcode.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://wpc.yfazqb.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://ppv.ywan-chungtsiang.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://gfw.fktsv.cn

Java: import java.util.List;
来源：http://usj.bjfxy.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://eis.cdnleiting.top

Ruby: require "json"; require_relative "./util"
来源：http://yki.cucudq.cn

C#:   using System.Text;
来源：http://nmj.wangdashe.top

[C12] 立即执行函数 IIFE
来源：http://fdl.chenlongwang.top

Py:   (lambda: print("run"))()
来源：http://ukl.hammf.cn

PHP:  (function () { echo "run"; })();
来源：http://akv.sysykeji.top

JS:   (() => { console.log("run"); })();
来源：http://vaq.aizwys.cn

TS:   (() => { console.log("run"); })();
来源：http://han.pycfn.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ejf.hesvh.cn

Go:   func() { fmt.Println("run") }()
来源：http://gpu.hnxiangtu.top

Ruby: -> { puts "run" }.call
来源：http://zvh.nanxinkj.top

C#:   // 无 IIFE：用静态构造函数
来源：http://cuy.gaohongyu789.top

[C13] 类型声明 / 类型注解
来源：http://tay.cashguo.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://omm.nwbrower.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vdw.jianghu66.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://kaq.fehbvm.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xcz.dashuyun.cn

Java: int add(int a, int b) { return a + b; }
来源：http://dal.yuxming.cn

Go:   func add(a, b int) int
来源：http://kdi.hnxiangtu.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://iij.cucudq.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ljv.xinyue.icu

[C14] 泛型函数
来源：http://uxf.fktsv.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://rqg.tanke756.top

PHP:  // 无泛型
来源：http://jtj.pycfn.com

JS:   // 无泛型
来源：http://gon.yj20258.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ehx.jlsjyb.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://uco.yueranfly.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://huo.xuetiantiany.cn

Ruby: # 无泛型
来源：http://vcv.kuanghao11.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://zec.gogol.net.cn

[C15] 解构 / 展开参数
来源：http://ilf.jinghuilouyu.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://rja.shangyingyoupin.top

PHP:  [$a, $b] = $pair;
来源：http://lyg.redwolf501.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://lnl.gaohongyu789.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://izk.iojbl.cn

Java: // 无解构
来源：http://myd.quarkkingdee.top

Go:   // 无解构
来源：http://cmx.xziqi.cn

Ruby: a, b = pair
来源：http://reu.yuxming.cn

C#:   var (a, b) = pair;
来源：http://pqd.shuidangran.top

[C16] 函数 / 方法重载
来源：http://lcg.gotoacloud.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://dkp.cheryme.top

PHP:  // 无重载
来源：http://tdf.jlsjyb.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://qmy.daria6918.cn

TS:   // 用联合类型或重载签名声明
来源：http://fwg.epnwcf.com

Java: void f(int a) {}  void f(String a) {}
来源：http://fbf.jqgfzy.top

Go:   // 无重载：用不同函数名
来源：http://scu.shanyushiyangtech.top

Ruby: # 无重载：靠动态参数
来源：http://jam.kuanghao11.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://uns.zhixingplan.top

================================================================================
来源：http://axu.hongshengwenyu.top

D. 数组 / 列表 / 集合
来源：http://plp.pengpengdd.cyou

================================================================================
来源：http://eah.daria6918.cn

[D01] 创建数组 / 列表
来源：http://qdw.jinqigufen.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://vhb.ywan-chungtsiang.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://siz.jinqigfzy.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://jvd.52xcode.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://wre.pycfn.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://epl.feifeiyinyue.top

Go:   arr := []int{1, 2, 3}
来源：http://juq.cheryme.top

Ruby: arr = [1, 2, 3]
来源：http://erg.tianlin.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wcq.havefunace.top

[D02] 追加元素到末尾
来源：http://jhf.yj202588.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://rfx.feifeiyinyue.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://zua.ivvv.top

JS:   arr.push(4);
来源：http://syt.xingfuxueyuan.xyz

TS:   arr.push(4);
来源：http://amq.pycfn.com

Java: list.add(4);
来源：http://daf.kuanghao11.cn

Go:   arr = append(arr, 4)
来源：http://gdh.hammf.cn

Ruby: arr << 4; arr.push(5)
来源：http://uea.yonumen.top

C#:   list.Add(4);
来源：http://mgb.yanxiufei.cn

[D03] 在指定位置插入元素
来源：http://fvv.zhongyouzk.top

Py:   arr.insert(0, 0)
来源：http://suv.hnxiangtu.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://qtp.zycfv.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://klk.shuidangran.top

TS:   arr.splice(0, 0, 0);
来源：http://dtd.xingfuxueyuan.xyz

Java: list.add(0, 0);
来源：http://uwn.shanyushiyangtech.top

Go:   arr = append([]int{0}, arr...)
来源：http://jdm.aizwys.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://jej.jinqigufen.top

C#:   list.Insert(0, 0);
来源：http://qla.gzhubu.top

[D04] 删除元素
来源：http://ahh.yvedp.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hml.smart0.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://btc.ybcxt.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://pdp.hfpthk.cn

TS:   arr.splice(0, 1);
来源：http://xpd.hfpthk.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://yvh.zhengqikj.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://akj.xuetiantiany.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://dxz.hfpthk.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ehn.9152youxi.cn

[D05] 访问与修改元素
来源：http://blx.havefunace.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wdh.shangyingyoupin.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://zhz.svipenyu.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://psa.hongshengwenyu.top

TS:   arr[0]; arr.at(-1);
来源：http://upb.cashguo.top

Java: list.get(0); list.set(0, 9);
来源：http://duo.nanxuanxn.top

Go:   arr[0]; arr[0] = 9
来源：http://xaw.fengsongda.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://qvz.mhx1999.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://gdg.jinqigufen.top

[D06] 数组长度
来源：http://xiq.tarul.cn

Py:   len(arr)
来源：http://pif.hnxiangtu.top

PHP:  count($arr);
来源：http://sth.zdqjudy.top

JS:   arr.length
来源：http://tin.yueranfly.top

TS:   arr.length
来源：http://ltt.uphjek.com

Java: list.size();
来源：http://xam.yj202588.top

Go:   len(arr)
来源：http://tys.jyoumei.cn

Ruby: arr.length; arr.size
来源：http://ipy.vqdsnc.cn

C#:   list.Count;
来源：http://hkv.yj202588.top

[D07] 切片 / 取子数组
来源：http://wuf.zhongyouzk.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qml.nanxuanxn.top

PHP:  array_slice($arr, 1, 3);
来源：http://cto.yonumen.top

JS:   arr.slice(1, 4);
来源：http://hrr.ppjwa.cn

TS:   arr.slice(1, 4);
来源：http://yaq.fanxiaobao.xyz

Java: list.subList(1, 4);
来源：http://owg.cashguo.top

Go:   arr[1:4]
来源：http://upx.gaohongyu789.top

Ruby: arr[1, 3]
来源：http://hna.ivvv.top

C#:   list.GetRange(1, 3);
来源：http://bpt.zdqjudy.top

[D08] 合并两个数组
来源：http://wdw.ivvv.top

Py:   a + b;  a.extend(b)
来源：http://eaz.jinqigfzy.top

PHP:  array_merge($a, $b);
来源：http://spc.jinqigfzy.top

JS:   [...a, ...b];  a.concat(b);
来源：http://vzx.hfpthk.cn

TS:   [...a, ...b];
来源：http://mtx.9152youxi.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://kej.jinghuilouyu.cn

Go:   append(a, b...)
来源：http://jgr.jinyuanbaomall.cn

Ruby: a + b;  a.concat(b)
来源：http://axi.gzhubu.top

C#:   a.Concat(b).ToList()
来源：http://wvr.nanxuanxn.top

[D09] 排序（升序）
来源：http://oxw.shangyingyoupin.top

Py:   sorted(arr);  arr.sort()
来源：http://fyn.zdbjq.cn

PHP:  sort($arr);
来源：http://mrg.ehwqpu.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hnw.yj20258.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://ryu.nwbrower.top

Java: Collections.sort(list);  list.sort(null);
来源：http://vpj.cdnleiting.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ctc.epnwcf.com

Ruby: arr.sort
来源：http://qcj.yonumen.top

C#:   list.Sort();
来源：http://vqp.jianghu66.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://ilt.aibaodan.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mbh.shuidangran.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ost.jqgfzy.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://juo.sweek.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ktv.aizwys.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://tbk.pycfn.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://tmp.daria6918.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://zfv.nanxinkj.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://jlw.kuanghao11.cn

[D11] 反转数组
来源：http://npx.xylfe.cn

Py:   arr[::-1];  arr.reverse()
来源：http://xnn.chenzaomai.com

PHP:  array_reverse($arr);
来源：http://bhu.jinyuanbaomall.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://jza.hammf.cn

TS:   [...arr].reverse();
来源：http://sgv.ctjpmb.com

Java: Collections.reverse(list);
来源：http://jay.meibo888.top

Go:   slices.Reverse(arr)
来源：http://qal.ydjk.org.cn

Ruby: arr.reverse
来源：http://jqs.yvedp.cn

C#:   list.Reverse();
来源：http://ltt.yuanzhike.top

[D12] 查找元素下标
来源：http://pgl.tanke756.top

Py:   arr.index(x);  x in arr
来源：http://qct.uphjek.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://zvs.zhijiandao.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lrx.redwolf501.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qhz.vehdjk.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://bya.nanxinkj.top

Go:   slices.Index(arr, x)
来源：http://auf.jqgufenzy.top

Ruby: arr.index(x)
来源：http://sko.wangshuangyany.cn

C#:   list.IndexOf(x);
来源：http://kva.uphjek.com

[D13] 过滤（保留满足条件的）
来源：http://zwm.andypj.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qbu.sufxvd.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://qnm.snrcjt.cn

JS:   arr.filter(x => x > 3)
来源：http://zmi.gaohongyu789.top

TS:   arr.filter(x => x > 3)
来源：http://gvp.xylfe.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://aof.hywenlv.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://puk.jiagoushi.top

Ruby: arr.select { |x| x > 3 }
来源：http://coo.hnqzz.top

C#:   list.Where(x => x > 3).ToList()
来源：http://dgh.daxiang520.top

[D14] 映射转换（每个元素变形）
来源：http://gvs.zhengqikj.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://yzl.zycfv.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://lcz.gaohongyu789.top

JS:   arr.map(x => x * 2)
来源：http://wbz.yuanzhike.top

TS:   arr.map(x => x * 2)
来源：http://kjq.xziqi.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://whn.yj20258.top

Go:   // 手写循环
来源：http://aug.bbcook.cn

Ruby: arr.map { |x| x * 2 }
来源：http://uwz.hnxiangtu.top

C#:   list.Select(x => x * 2).ToList()
来源：http://htc.haohaochexian.top

[D15] 去重
来源：http://uwb.xziqi.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://yfj.tanke756.top

PHP:  array_unique($arr);
来源：http://ire.vqdsnc.cn

JS:   [...new Set(arr)]
来源：http://qkc.bjfxy.top

TS:   [...new Set(arr)]
来源：http://umv.wangdashe.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://dik.fzhhl.top

Go:   // 用 map[T]struct{} 手写
来源：http://sku.fzhhl.top

Ruby: arr.uniq
来源：http://znc.hysaishi.cn

C#:   list.Distinct().ToList()
来源：http://ooa.ctjpmb.com

[D16] 求和与平均值
来源：http://qcp.c1oappe.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://yzo.kuanghao11.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://iac.zhijiandao.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://cpl.chenjidiqi.icu

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://qkf.yueranfly.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://olo.tianlin.xyz

Go:   // 手写循环累加
来源：http://fys.ybcxt.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mil.zhixingplan.top

C#:   list.Sum();  list.Average()
来源：http://aqt.birdmap.top

[D17] 最大值与最小值
来源：http://jrf.jinqigufen.top

Py:   max(arr);  min(arr)
来源：http://got.gogol.net.cn

PHP:  max($arr);  min($arr);
来源：http://lks.cdnleiting.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ptf.yangfankeji.com

TS:   Math.max(...arr);
来源：http://tyn.ctjpmb.com

Java: Collections.max(list);  Collections.min(list);
来源：http://oft.hysaishi.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://msf.daxiang520.top

Ruby: arr.max;  arr.min
来源：http://weu.ehwqpu.com

C#:   list.Max();  list.Min()
来源：http://vau.cheryme.top

[D18] 扁平化嵌套数组
来源：http://ywa.gotoacloud.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://kua.sxryk.cn

PHP:  array_merge(...$nested);
来源：http://evw.chenjidiqi.icu

JS:   nested.flat();  nested.flat(Infinity)
来源：http://jsr.316326.xyz

TS:   nested.flat();
来源：http://itz.hammf.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://chc.cheryme.top

Go:   // 手写双层循环
来源：http://exi.snrcjt.cn

Ruby: nested.flatten
来源：http://wxf.smart0.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://srz.shangyingyoupin.top

[D19] 按字段分组
来源：http://nxw.wangdashe.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wxn.redwolf501.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mxp.ydzc1.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://rtp.gzhubu.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://fwr.ctjpmb.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://zsu.yj20258.top

Go:   // 手写 map[string][]T
来源：http://eow.fengsongda.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://jxf.haohaochexian.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://unf.yueranfly.top

[D20] 统计每个元素出现次数
来源：http://hmu.xingfuxueyuan.xyz

Py:   Counter(arr)
来源：http://ysg.jinqigufen.top

PHP:  array_count_values($arr);
来源：http://sfr.jiagoushi.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xpc.shanyushiyangkeji.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cio.jinqigufen.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://tuk.ppjwa.cn

Go:   // 手写 map[T]int
来源：http://ngo.guowangkeji.top

Ruby: arr.tally
来源：http://ftg.vqdsnc.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ywh.quarkkingdee.top

[D21] 判断是否包含某元素
来源：http://wdr.feifeiyinyue.top

Py:   x in arr
来源：http://ukq.zhixingplan.top

PHP:  in_array($x, $arr, true);
来源：http://xjv.xuetiantiany.cn

JS:   arr.includes(x)
来源：http://yey.ybcxt.top

TS:   arr.includes(x)
来源：http://rdr.bbcook.cn

Java: list.contains(x)
来源：http://hmj.jyoumei.cn

Go:   slices.Contains(arr, x)
来源：http://qhw.yanxiufei.cn

Ruby: arr.include?(x)
来源：http://uqe.hywenlv.cn

C#:   list.Contains(x)
来源：http://smy.bjfxy.top

[D22] 复制数组（避免共享引用）
来源：http://ior.chenzaomai.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wjz.hfpthk.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://brc.meibo888.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ebe.uphjek.com

TS:   [...arr];
来源：http://afp.cheryme.top

Java: new ArrayList<>(list);
来源：http://bvf.zhijiandao.cn

Go:   copied := append([]int(nil), arr...)
来源：http://isj.yj20258.top

Ruby: arr.dup;  arr.clone
来源：http://aff.tianlin.xyz

C#:   new List<int>(list);
来源：http://jhy.xuanzx.com

[D23] reduce 累积计算
来源：http://cga.yonumen.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gvh.nanxinkj.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://kzy.ppjwa.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cnq.jyoumei.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cqn.jinqigfzy.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://aey.yuanzhike.top

Go:   // 手写循环
来源：http://ilf.zhongyouzk.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://zkr.ybcxt.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://snn.sjlbkw.cn

[D24] 字典 / Map 基本操作
来源：http://vet.wangdashe.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://pxh.jianghu66.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://bti.nwbrower.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://jop.zhaomingkeji.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://aoq.iojbl.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://dau.feifeiyinyue.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://qrd.xuanzx.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ead.fengsongda.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://dvf.shanyushiyangkeji.top

[D25] Set 集合去重与交并差
来源：http://zxa.zhoulong.xyz

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://lqi.cqqwz.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://sua.smart0.xyz

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://clt.guowangkeji.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://fgp.sxryk.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://lrd.jlsjyb.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://bba.zhongyouzk.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://dfm.yj20258.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://bzq.meibo888.top

[D26] 数组转字符串
来源：http://ogm.sweek.top

Py:   ", ".join(map(str, arr))
来源：http://dpv.vqdsnc.cn

PHP:  implode(", ", $arr);
来源：http://zam.9152youxi.cn

JS:   arr.join(", ")
来源：http://ihy.yfazqb.com

TS:   arr.join(", ")
来源：http://ylu.yangfankeji.com

Java: String.join(", ", list)
来源：http://qcf.zhengqikj.top

Go:   strings.Join(strs, ", ")
来源：http://iiz.zhiwuduotai.top

Ruby: arr.join(", ")
来源：http://tdp.yj20258.top

C#:   string.Join(", ", list)
来源：http://tux.jinghuilouyu.cn

================================================================================
来源：http://tlq.yj20258.top

E. 字符串处理
来源：http://kpz.uphjek.com

================================================================================
来源：http://kzz.cucudq.cn

[E01] 拼接字符串
来源：http://uih.ydjk.org.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wiu.fanxiaobao.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ero.hywenlv.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://bzx.cqqwz.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://nap.zdqjudy.top


<!-- 参考信息 -->