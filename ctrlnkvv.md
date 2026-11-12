代发 wailian999

JS:   export default function f() {};  import f from "./m.js";
来源：http://svz.jinghuilouyu.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://pfc.snrcjt.cn

Java: import java.util.List;
来源：http://xzs.tanke756.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wne.nanxinkj.top

Ruby: require "json"; require_relative "./util"
来源：http://lbq.hongshengwenyu.top

C#:   using System.Text;
来源：http://bfe.chenzaomai.com

[C12] 立即执行函数 IIFE
来源：http://znf.pycfn.com

Py:   (lambda: print("run"))()
来源：http://jhy.shuidangran.top

PHP:  (function () { echo "run"; })();
来源：http://pix.wangdashe.top

JS:   (() => { console.log("run"); })();
来源：http://mpz.jinqigfzy.top

TS:   (() => { console.log("run"); })();
来源：http://odj.ywan-chungtsiang.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wue.hywenlv.cn

Go:   func() { fmt.Println("run") }()
来源：http://dfe.jinqigufen.top

Ruby: -> { puts "run" }.call
来源：http://ano.uphjek.com

C#:   // 无 IIFE：用静态构造函数
来源：http://djd.andypj.xyz

[C13] 类型声明 / 类型注解
来源：http://uuh.guannengcc.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hss.hongshengwenyu.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jen.bjfxy.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://dkj.0kj1m.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://win.hnxiangtu.top

Java: int add(int a, int b) { return a + b; }
来源：http://xdk.ehwqpu.com

Go:   func add(a, b int) int
来源：http://tly.wangshuangyany.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://uod.jyoumei.cn

C#:   int Add(int a, int b) => a + b;
来源：http://xas.meibo888.top

[C14] 泛型函数
来源：http://ofx.c1oappe.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://pxh.yanxiufei.cn

PHP:  // 无泛型
来源：http://nak.zycfv.cn

JS:   // 无泛型
来源：http://pug.hywenlv.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://soy.jinqigufen.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://veh.cdnleiting.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://lbc.gogol.net.cn

Ruby: # 无泛型
来源：http://hoe.guannengcc.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://nay.jianghu66.top

[C15] 解构 / 展开参数
来源：http://jqk.shangyingyoupin.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wxi.yj20258888.top

PHP:  [$a, $b] = $pair;
来源：http://rku.pengpengdd.cyou

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xts.tianlin.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mhd.yuxming.cn

Java: // 无解构
来源：http://xbs.cheryme.top

Go:   // 无解构
来源：http://ple.feifeiyinyue.top

Ruby: a, b = pair
来源：http://rsq.svipenyu.cn

C#:   var (a, b) = pair;
来源：http://llo.andypj.xyz

[C16] 函数 / 方法重载
来源：http://pvh.fanxiaobao.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mtw.ctjpmb.com

PHP:  // 无重载
来源：http://pdq.fehbvm.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://oda.dianchejie.cn

TS:   // 用联合类型或重载签名声明
来源：http://qng.fehbvm.com

Java: void f(int a) {}  void f(String a) {}
来源：http://fil.nwbrower.top

Go:   // 无重载：用不同函数名
来源：http://rsi.yueranfly.top

Ruby: # 无重载：靠动态参数
来源：http://agf.dashuyun.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://bzr.daxiang520.top

================================================================================
来源：http://xof.uphjek.com

D. 数组 / 列表 / 集合
来源：http://iey.jinqigfzy.top

================================================================================
来源：http://cyr.haohaochexian.top

[D01] 创建数组 / 列表
来源：http://rnr.ydjk.org.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://sbt.haohaochexian.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://jcm.yongpay.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://vpw.yfazqb.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://pad.hysaishi.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://bbb.feifeiyinyue.top

Go:   arr := []int{1, 2, 3}
来源：http://feu.hcnkem.com

Ruby: arr = [1, 2, 3]
来源：http://tmm.yueranfly.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://tbf.tianlin.xyz

[D02] 追加元素到末尾
来源：http://icg.yonumen.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wdq.wangdashe.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://nli.yuanzhike.top

JS:   arr.push(4);
来源：http://oif.shangyingyoupin.top

TS:   arr.push(4);
来源：http://mtl.xuetiantiany.cn

Java: list.add(4);
来源：http://xcd.zhaomingkeji.xyz

Go:   arr = append(arr, 4)
来源：http://bci.c1oappe.top

Ruby: arr << 4; arr.push(5)
来源：http://ogj.zhongyouzk.top

C#:   list.Add(4);
来源：http://hum.fzhhl.top

[D03] 在指定位置插入元素
来源：http://hxm.cashguo.top

Py:   arr.insert(0, 0)
来源：http://ehb.316326.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://loe.jqgfzy.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://vps.jlsjyb.cn

TS:   arr.splice(0, 0, 0);
来源：http://ygg.yj20258888.top

Java: list.add(0, 0);
来源：http://jrx.redwolf501.top

Go:   arr = append([]int{0}, arr...)
来源：http://kzq.cucudq.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://bjn.shanyushiyangkeji.top

C#:   list.Insert(0, 0);
来源：http://dhb.xylfe.cn

[D04] 删除元素
来源：http://gue.hfpthk.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://cnb.hysaishi.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://fuh.xingfuxueyuan.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ydk.uphjek.com

TS:   arr.splice(0, 1);
来源：http://kds.tarul.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://yqt.yj20258888.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://zgi.shanyushiyangtech.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://moi.shanyushiyangkeji.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ibf.jinqigfzy.top

[D05] 访问与修改元素
来源：http://ypy.andypj.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://lky.zhijiandao.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://pxk.cashguo.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://vbx.shangyingyoupin.top

TS:   arr[0]; arr.at(-1);
来源：http://azm.zdbjq.cn

Java: list.get(0); list.set(0, 9);
来源：http://vor.andypj.xyz

Go:   arr[0]; arr[0] = 9
来源：http://grs.chenzaomai.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://fgy.vehdjk.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://nbu.hesvh.cn

[D06] 数组长度
来源：http://wbf.zhongyouzk.top

Py:   len(arr)
来源：http://qiy.cucudq.cn

PHP:  count($arr);
来源：http://oav.tianlin.xyz

JS:   arr.length
来源：http://lds.uphjek.com

TS:   arr.length
来源：http://lpk.fktsv.cn

Java: list.size();
来源：http://eua.hesvh.cn

Go:   len(arr)
来源：http://pnh.havefunace.top

Ruby: arr.length; arr.size
来源：http://ijy.hesvh.cn

C#:   list.Count;
来源：http://csq.jyoumei.cn

[D07] 切片 / 取子数组
来源：http://bnm.zhixingplan.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ejj.fehbvm.com

PHP:  array_slice($arr, 1, 3);
来源：http://zzg.shanyushiyangtech.top

JS:   arr.slice(1, 4);
来源：http://zjm.zhaomingkeji.xyz

TS:   arr.slice(1, 4);
来源：http://hkw.ivvv.top

Java: list.subList(1, 4);
来源：http://gal.shanyushiyangkeji.top

Go:   arr[1:4]
来源：http://fem.hnqzz.top

Ruby: arr[1, 3]
来源：http://aht.yj202588.top

C#:   list.GetRange(1, 3);
来源：http://mbd.birdmap.top

[D08] 合并两个数组
来源：http://rao.jqgufenzy.top

Py:   a + b;  a.extend(b)
来源：http://kne.hesvh.cn

PHP:  array_merge($a, $b);
来源：http://lki.hywenlv.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://lzm.svipenyu.cn

TS:   [...a, ...b];
来源：http://auq.xziqi.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://qfw.fzhhl.top

Go:   append(a, b...)
来源：http://xdg.zhengqikj.top

Ruby: a + b;  a.concat(b)
来源：http://yru.hysaishi.cn

C#:   a.Concat(b).ToList()
来源：http://pzg.9152youxi.cn

[D09] 排序（升序）
来源：http://avf.quarkkingdee.top

Py:   sorted(arr);  arr.sort()
来源：http://cvi.hywenlv.cn

PHP:  sort($arr);
来源：http://vbk.hnqzz.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://tzx.zhaomingkeji.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://eit.yj20258.top

Java: Collections.sort(list);  list.sort(null);
来源：http://cnz.nwbrower.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://lyh.316326.xyz

Ruby: arr.sort
来源：http://efq.snrcjt.cn

C#:   list.Sort();
来源：http://lja.fzhhl.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://ipg.xylfe.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://yhz.xuanzx.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zlf.zdqjudy.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://frd.zycfv.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://vgp.hnqzz.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ljr.dashuyun.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ihh.meibo888.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://aiq.xuetiantiany.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ofh.yvedp.cn

[D11] 反转数组
来源：http://gzw.snrcjt.cn

Py:   arr[::-1];  arr.reverse()
来源：http://lfq.xuetiantiany.cn

PHP:  array_reverse($arr);
来源：http://bzf.chenzaomai.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://snm.sxryk.cn

TS:   [...arr].reverse();
来源：http://owi.shuidangran.top

Java: Collections.reverse(list);
来源：http://zfj.xuanzx.com

Go:   slices.Reverse(arr)
来源：http://kcj.pycfn.com

Ruby: arr.reverse
来源：http://lap.yvedp.cn

C#:   list.Reverse();
来源：http://yqr.fktsv.cn

[D12] 查找元素下标
来源：http://hph.hesvh.cn

Py:   arr.index(x);  x in arr
来源：http://yph.fktsv.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://azv.aibaodan.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zin.tianlin.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://brq.jiagoushi.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://njv.xingfuxueyuan.xyz

Go:   slices.Index(arr, x)
来源：http://kzp.sjlbkw.cn

Ruby: arr.index(x)
来源：http://suz.andypj.xyz

C#:   list.IndexOf(x);
来源：http://lxl.meibo888.top

[D13] 过滤（保留满足条件的）
来源：http://pet.hnqzz.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://vfl.smart0.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hhy.xinyue.icu

JS:   arr.filter(x => x > 3)
来源：http://adx.xingfuxueyuan.xyz

TS:   arr.filter(x => x > 3)
来源：http://dlt.yfazqb.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mkq.yanxiufei.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://clw.nwbrower.top

Ruby: arr.select { |x| x > 3 }
来源：http://hcv.vqdsnc.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://qlo.xingfuxueyuan.xyz

[D14] 映射转换（每个元素变形）
来源：http://bjt.yj202588.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://njx.ivvv.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://nes.tarul.cn

JS:   arr.map(x => x * 2)
来源：http://tic.sxryk.cn

TS:   arr.map(x => x * 2)
来源：http://rfq.cheryme.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://yzg.snrcjt.cn

Go:   // 手写循环
来源：http://ypz.sufxvd.cn

Ruby: arr.map { |x| x * 2 }
来源：http://cwl.dianchejie.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://tza.zhaomingkeji.xyz

[D15] 去重
来源：http://qhf.0kj1m.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://uje.xuanzx.com

PHP:  array_unique($arr);
来源：http://lmv.cashguo.top

JS:   [...new Set(arr)]
来源：http://pca.yangfankeji.com

TS:   [...new Set(arr)]
来源：http://efj.yj202588.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://xqx.yj20258888.top

Go:   // 用 map[T]struct{} 手写
来源：http://fvn.yvedp.cn

Ruby: arr.uniq
来源：http://zly.guannengcc.top

C#:   list.Distinct().ToList()
来源：http://glp.epnwcf.com

[D16] 求和与平均值
来源：http://esb.gzhubu.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://omu.fengsongda.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://fdh.yanxiufei.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://rju.shzxlz.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://jxv.fehbvm.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wyt.hammf.cn

Go:   // 手写循环累加
来源：http://nog.havefunace.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://aug.dianchejie.cn

C#:   list.Sum();  list.Average()
来源：http://clf.zhongyouzk.top

[D17] 最大值与最小值
来源：http://ast.wangdashe.top

Py:   max(arr);  min(arr)
来源：http://rkl.dashuyun.cn

PHP:  max($arr);  min($arr);
来源：http://xlk.ctjpmb.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ogl.pengpengdd.cyou

TS:   Math.max(...arr);
来源：http://tdh.iojbl.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://plz.yj202588.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://zuc.zdqjudy.top

Ruby: arr.max;  arr.min
来源：http://agi.tanke756.top

C#:   list.Max();  list.Min()
来源：http://xzg.pengpengdd.cyou

[D18] 扁平化嵌套数组
来源：http://htp.aibaodan.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://nkb.zycfv.cn

PHP:  array_merge(...$nested);
来源：http://ovi.yfazqb.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://xyi.yangfankeji.com

TS:   nested.flat();
来源：http://box.havefunace.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://tgl.cqqwz.cn

Go:   // 手写双层循环
来源：http://djx.hysaishi.cn

Ruby: nested.flatten
来源：http://brw.daria6918.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://kio.zhixingplan.top

[D19] 按字段分组
来源：http://abd.yj20258.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ifl.zhijiandao.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wej.tanke756.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://lul.ywan-chungtsiang.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://lyc.hnxiangtu.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://kyt.ybcxt.top

Go:   // 手写 map[string][]T
来源：http://qsd.shuidangran.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://xou.yonumen.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://pry.zhoulong.xyz

[D20] 统计每个元素出现次数
来源：http://dom.dianchejie.cn

Py:   Counter(arr)
来源：http://wxu.chenjidiqi.icu

PHP:  array_count_values($arr);
来源：http://xos.guannengcc.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://uzt.ydzc1.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jxk.snrcjt.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mrm.xylfe.cn

Go:   // 手写 map[T]int
来源：http://bvg.xylfe.cn

Ruby: arr.tally
来源：http://zgg.shuidangran.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://qma.c1oappe.top

[D21] 判断是否包含某元素
来源：http://gnz.9152youxi.cn

Py:   x in arr
来源：http://ppg.fanxiaobao.xyz

PHP:  in_array($x, $arr, true);
来源：http://hhx.cqqwz.cn

JS:   arr.includes(x)
来源：http://fls.dianchejie.cn

TS:   arr.includes(x)
来源：http://huq.zhaomingkeji.xyz

Java: list.contains(x)
来源：http://hnn.yueranfly.top

Go:   slices.Contains(arr, x)
来源：http://jvi.gaohongyu789.top

Ruby: arr.include?(x)
来源：http://pmd.jiagoushi.top

C#:   list.Contains(x)
来源：http://iww.iojbl.cn

[D22] 复制数组（避免共享引用）
来源：http://dgw.ydzc1.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://srv.ppjwa.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://qkp.nanxinkj.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://nqn.hnxiangtu.top

TS:   [...arr];
来源：http://ibw.svipenyu.cn

Java: new ArrayList<>(list);
来源：http://qav.cdnleiting.top

Go:   copied := append([]int(nil), arr...)
来源：http://wkl.chenjidiqi.icu

Ruby: arr.dup;  arr.clone
来源：http://egk.kuanghao11.cn

C#:   new List<int>(list);
来源：http://qhd.chenzaomai.com

[D23] reduce 累积计算
来源：http://bos.hywenlv.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wbc.ctjpmb.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://qfv.smart0.xyz

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pei.nanxuanxn.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qgc.meibo888.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://hxb.shangyingyoupin.top

Go:   // 手写循环
来源：http://hmb.gogol.net.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://tnb.cdnleiting.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://uxj.zhongyouzk.top

[D24] 字典 / Map 基本操作
来源：http://qoz.uphjek.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ujw.bjfxy.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://zri.zhiwuduotai.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://izr.ppjwa.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://vxx.zdqjudy.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://bos.zhiwuduotai.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wxe.daria6918.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://pcx.chenzaomai.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mnz.kuanghao11.cn

[D25] Set 集合去重与交并差
来源：http://tgf.hesvh.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://qdv.jiagoushi.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://qhd.feifeiyinyue.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://dyi.ydzc1.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://uly.wangdashe.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://bdq.nwbrower.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mfm.ivvv.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ffv.ywan-chungtsiang.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://rxj.svipenyu.cn

[D26] 数组转字符串
来源：http://oya.chenjidiqi.icu

Py:   ", ".join(map(str, arr))
来源：http://lzv.vqdsnc.cn

PHP:  implode(", ", $arr);
来源：http://nim.xylfe.cn

JS:   arr.join(", ")
来源：http://dxd.wangdashe.top

TS:   arr.join(", ")
来源：http://osk.haohaochexian.top

Java: String.join(", ", list)
来源：http://yam.redwolf501.top

Go:   strings.Join(strs, ", ")
来源：http://wwa.shanyushiyangkeji.top

Ruby: arr.join(", ")
来源：http://xdj.zhengqikj.top

C#:   string.Join(", ", list)
来源：http://hva.quarkkingdee.top

================================================================================
来源：http://aul.ivvv.top

E. 字符串处理
来源：http://xiu.ywan-chungtsiang.top

================================================================================
来源：http://dpv.zhixingplan.top

[E01] 拼接字符串
来源：http://xqp.gogol.net.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://oky.yueranfly.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://xhs.jinqigfzy.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://zun.ywan-chungtsiang.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://sdh.meibo888.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://alq.zhixingplan.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://vbz.zhongyouzk.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://qjg.haohaochexian.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://fva.sweek.top


<!-- 参考信息 -->