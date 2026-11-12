代发 wailian999

Java: int add(int a, int b) { return a + b; }
来源：http://qvz.shzxlz.cn

Go:   func add(a, b int) int
来源：http://xyh.jqgufenzy.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ghi.fanxiaobao.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://pfn.c1oappe.top

[C14] 泛型函数
来源：http://fes.fanxiaobao.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ahw.ywan-chungtsiang.top

PHP:  // 无泛型
来源：http://slc.xuetiantiany.cn

JS:   // 无泛型
来源：http://fus.fzhhl.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://jtj.shzxlz.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://qnf.zhengqikj.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://urb.zhijiandao.cn

Ruby: # 无泛型
来源：http://zbt.dashuyun.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mzy.jinyuanbaomall.cn

[C15] 解构 / 展开参数
来源：http://cma.hywenlv.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ruy.sysykeji.top

PHP:  [$a, $b] = $pair;
来源：http://ahv.pengpengdd.cyou

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wcn.yuanzhike.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://sav.uphjek.com

Java: // 无解构
来源：http://hag.tanke756.top

Go:   // 无解构
来源：http://aor.chenzaomai.com

Ruby: a, b = pair
来源：http://cnp.xuetiantiany.cn

C#:   var (a, b) = pair;
来源：http://fxx.cheryme.top

[C16] 函数 / 方法重载
来源：http://uts.yonumen.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://zfn.zhijiandao.cn

PHP:  // 无重载
来源：http://xzp.ydzc1.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://mtj.chenjidiqi.icu

TS:   // 用联合类型或重载签名声明
来源：http://uts.9152youxi.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://jcj.wangshuangyany.cn

Go:   // 无重载：用不同函数名
来源：http://ned.yangfankeji.com

Ruby: # 无重载：靠动态参数
来源：http://ocl.cucudq.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://wqu.shanyushiyangtech.top

================================================================================
来源：http://msq.yueranfly.top

D. 数组 / 列表 / 集合
来源：http://vev.guannengcc.top

================================================================================
来源：http://vgn.guannengcc.top

[D01] 创建数组 / 列表
来源：http://ayr.meibo888.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://nqe.shuidangran.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://zkm.jyoumei.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ywy.hysaishi.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://kmm.52xcode.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://eno.daxiang520.top

Go:   arr := []int{1, 2, 3}
来源：http://dup.epnwcf.com

Ruby: arr = [1, 2, 3]
来源：http://geb.yongpay.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hwj.yanxiufei.cn

[D02] 追加元素到末尾
来源：http://uje.tian-w.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://vgb.zhongyouzk.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://abv.gzhubu.top

JS:   arr.push(4);
来源：http://zkb.nanxinkj.top

TS:   arr.push(4);
来源：http://tsc.vehdjk.com

Java: list.add(4);
来源：http://kyg.9152youxi.cn

Go:   arr = append(arr, 4)
来源：http://hrq.gogol.net.cn

Ruby: arr << 4; arr.push(5)
来源：http://dbq.redwolf501.top

C#:   list.Add(4);
来源：http://yph.zhongyouzk.top

[D03] 在指定位置插入元素
来源：http://pgt.chenzaomai.com

Py:   arr.insert(0, 0)
来源：http://anb.chenjidiqi.icu

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://epg.hnqzz.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://oxz.xziqi.cn

TS:   arr.splice(0, 0, 0);
来源：http://dre.bbcook.cn

Java: list.add(0, 0);
来源：http://urg.tian-w.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ecs.zhaomingkeji.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wrq.aibaodan.cn

C#:   list.Insert(0, 0);
来源：http://gjc.jlsjyb.cn

[D04] 删除元素
来源：http://tbv.meibo888.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://nse.xinyue.icu

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://nsk.andypj.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://gbx.zhaomingkeji.xyz

TS:   arr.splice(0, 1);
来源：http://pof.fengsongda.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mwp.sysykeji.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://rlf.ppjwa.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hmk.0kj1m.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://nwe.hammf.cn

[D05] 访问与修改元素
来源：http://iqo.shzxlz.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ihe.tianlin.xyz

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://izn.nanxinkj.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://czi.ivvv.top

TS:   arr[0]; arr.at(-1);
来源：http://jvn.yj20258.top

Java: list.get(0); list.set(0, 9);
来源：http://gnh.aizwys.cn

Go:   arr[0]; arr[0] = 9
来源：http://ife.guannengcc.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://fle.tanke756.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://vsn.xinyue.icu

[D06] 数组长度
来源：http://odo.52xcode.cn

Py:   len(arr)
来源：http://rcg.chenjidiqi.icu

PHP:  count($arr);
来源：http://kut.yuxming.cn

JS:   arr.length
来源：http://llr.redwolf501.top

TS:   arr.length
来源：http://azz.chenlongwang.top

Java: list.size();
来源：http://jfr.andypj.xyz

Go:   len(arr)
来源：http://kfj.shangyingyoupin.top

Ruby: arr.length; arr.size
来源：http://obg.zycfv.cn

C#:   list.Count;
来源：http://uny.daria6918.cn

[D07] 切片 / 取子数组
来源：http://nmz.uphjek.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://gck.zhengqikj.top

PHP:  array_slice($arr, 1, 3);
来源：http://zri.cqqwz.cn

JS:   arr.slice(1, 4);
来源：http://bta.gotoacloud.top

TS:   arr.slice(1, 4);
来源：http://mpq.fehbvm.com

Java: list.subList(1, 4);
来源：http://fae.aibaodan.cn

Go:   arr[1:4]
来源：http://kkz.zhoulong.xyz

Ruby: arr[1, 3]
来源：http://gsr.svipenyu.cn

C#:   list.GetRange(1, 3);
来源：http://mpl.ydzc1.top

[D08] 合并两个数组
来源：http://mbz.nanxinkj.top

Py:   a + b;  a.extend(b)
来源：http://bpk.uphjek.com

PHP:  array_merge($a, $b);
来源：http://tga.bbcook.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://kep.9152youxi.cn

TS:   [...a, ...b];
来源：http://xrf.birdmap.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://omt.wangshuangyany.cn

Go:   append(a, b...)
来源：http://bsq.tian-w.cn

Ruby: a + b;  a.concat(b)
来源：http://bbt.chenlongwang.top

C#:   a.Concat(b).ToList()
来源：http://gfm.fanxiaobao.xyz

[D09] 排序（升序）
来源：http://yfc.mhx1999.top

Py:   sorted(arr);  arr.sort()
来源：http://ukb.sjlbkw.cn

PHP:  sort($arr);
来源：http://enq.vqdsnc.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mla.meibo888.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://cem.smart0.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://ycs.tarul.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wli.ppjwa.cn

Ruby: arr.sort
来源：http://vmg.shanyushiyangkeji.top

C#:   list.Sort();
来源：http://vva.52xcode.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://vhk.zdbjq.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://fwh.yuxming.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rlc.ivvv.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://snx.dashuyun.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ojm.ehwqpu.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wot.9152youxi.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://zoo.zhengqikj.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://yep.tarul.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hoc.chenjidiqi.icu

[D11] 反转数组
来源：http://iyg.yanxiufei.cn

Py:   arr[::-1];  arr.reverse()
来源：http://etu.yuxming.cn

PHP:  array_reverse($arr);
来源：http://ihw.pengpengdd.cyou

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mmg.xingfuxueyuan.xyz

TS:   [...arr].reverse();
来源：http://mbz.yj202588.top

Java: Collections.reverse(list);
来源：http://omo.xuanzx.com

Go:   slices.Reverse(arr)
来源：http://qup.tanke756.top

Ruby: arr.reverse
来源：http://xrt.jqgfzy.top

C#:   list.Reverse();
来源：http://ira.yj20258888.top

[D12] 查找元素下标
来源：http://wwn.smart0.xyz

Py:   arr.index(x);  x in arr
来源：http://oyu.pycfn.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://swf.shuidangran.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://soq.zhongyouzk.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rrn.nwbrower.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://kao.zhiwuduotai.top

Go:   slices.Index(arr, x)
来源：http://lri.haohaochexian.top

Ruby: arr.index(x)
来源：http://jax.hysaishi.cn

C#:   list.IndexOf(x);
来源：http://nhi.snrcjt.cn

[D13] 过滤（保留满足条件的）
来源：http://kgo.tarul.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://kfl.yj20258.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ecb.nwbrower.top

JS:   arr.filter(x => x > 3)
来源：http://hus.9152youxi.cn

TS:   arr.filter(x => x > 3)
来源：http://dsk.hesvh.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://sgd.haohaochexian.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://sto.jianghu66.top

Ruby: arr.select { |x| x > 3 }
来源：http://sqa.xuetiantiany.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://wpt.ivvv.top

[D14] 映射转换（每个元素变形）
来源：http://ooq.zhaomingkeji.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xpf.nwbrower.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ozw.zhijiandao.cn

JS:   arr.map(x => x * 2)
来源：http://xra.pengpengdd.cyou

TS:   arr.map(x => x * 2)
来源：http://shv.guannengcc.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://uyr.yongpay.top

Go:   // 手写循环
来源：http://hky.dianchejie.cn

Ruby: arr.map { |x| x * 2 }
来源：http://pmr.zhixingplan.top

C#:   list.Select(x => x * 2).ToList()
来源：http://enj.zdbjq.cn

[D15] 去重
来源：http://wwf.xylfe.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://xqh.fehbvm.com

PHP:  array_unique($arr);
来源：http://vsh.fzhhl.top

JS:   [...new Set(arr)]
来源：http://apr.guowangkeji.top

TS:   [...new Set(arr)]
来源：http://akv.yanxiufei.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ldo.jqgufenzy.top

Go:   // 用 map[T]struct{} 手写
来源：http://kxe.jinqigufen.top

Ruby: arr.uniq
来源：http://mxa.quarkkingdee.top

C#:   list.Distinct().ToList()
来源：http://mkz.sufxvd.cn

[D16] 求和与平均值
来源：http://kvo.ybcxt.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://vlw.52xcode.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://yta.yj20258.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://uok.fengsongda.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://afs.ybcxt.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ymv.jlsjyb.cn

Go:   // 手写循环累加
来源：http://dqt.yj20258888.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hbv.shzxlz.cn

C#:   list.Sum();  list.Average()
来源：http://sit.gogol.net.cn

[D17] 最大值与最小值
来源：http://ams.jqgfzy.top

Py:   max(arr);  min(arr)
来源：http://pof.daria6918.cn

PHP:  max($arr);  min($arr);
来源：http://gkj.iojbl.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mrr.wangdashe.top

TS:   Math.max(...arr);
来源：http://rdg.yanxiufei.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://bvg.yj20258.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ihm.redwolf501.top

Ruby: arr.max;  arr.min
来源：http://ohc.ydjk.org.cn

C#:   list.Max();  list.Min()
来源：http://jxd.hnqzz.top

[D18] 扁平化嵌套数组
来源：http://ssj.yfazqb.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://huv.zdbjq.cn

PHP:  array_merge(...$nested);
来源：http://eeu.nanxinkj.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://tmq.ppjwa.cn

TS:   nested.flat();
来源：http://tur.fzhhl.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://btn.daria6918.cn

Go:   // 手写双层循环
来源：http://wso.sjlbkw.cn

Ruby: nested.flatten
来源：http://ksf.zhaomingkeji.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://dhp.hesvh.cn

[D19] 按字段分组
来源：http://lue.zhiwuduotai.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ish.daxiang520.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://oxw.svipenyu.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://vtg.xylfe.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://vjc.meibo888.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://qll.sxryk.cn

Go:   // 手写 map[string][]T
来源：http://ygy.vqdsnc.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://wpi.hammf.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://tdp.jianghu66.top

[D20] 统计每个元素出现次数
来源：http://mbj.hywenlv.cn

Py:   Counter(arr)
来源：http://kym.shzxlz.cn

PHP:  array_count_values($arr);
来源：http://kud.pycfn.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mtp.cheryme.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bet.zhijiandao.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://gix.fanxiaobao.xyz

Go:   // 手写 map[T]int
来源：http://qgc.zdqjudy.top

Ruby: arr.tally
来源：http://oen.ywan-chungtsiang.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://lio.52xcode.cn

[D21] 判断是否包含某元素
来源：http://laj.yfazqb.com

Py:   x in arr
来源：http://yeo.shanyushiyangtech.top

PHP:  in_array($x, $arr, true);
来源：http://vuy.zhiwuduotai.top

JS:   arr.includes(x)
来源：http://vqa.yonumen.top

TS:   arr.includes(x)
来源：http://nrx.snrcjt.cn

Java: list.contains(x)
来源：http://ktn.tarul.cn

Go:   slices.Contains(arr, x)
来源：http://phx.svipenyu.cn

Ruby: arr.include?(x)
来源：http://fct.jqgfzy.top

C#:   list.Contains(x)
来源：http://gdq.sweek.top

[D22] 复制数组（避免共享引用）
来源：http://avi.vqdsnc.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://keg.xziqi.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://rps.zhaomingkeji.xyz

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://lqj.fanxiaobao.xyz

TS:   [...arr];
来源：http://guc.yj20258.top

Java: new ArrayList<>(list);
来源：http://pbs.cashguo.top

Go:   copied := append([]int(nil), arr...)
来源：http://nch.dianchejie.cn

Ruby: arr.dup;  arr.clone
来源：http://hhy.jinqigufen.top

C#:   new List<int>(list);
来源：http://jhu.gaohongyu789.top

[D23] reduce 累积计算
来源：http://ubu.pengpengdd.cyou

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://grt.c1oappe.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://gae.zhijiandao.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://imd.cqqwz.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cnn.sweek.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://lhh.zhiwuduotai.top

Go:   // 手写循环
来源：http://cma.zdqjudy.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://gkr.zhongyouzk.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://tde.kuanghao11.cn

[D24] 字典 / Map 基本操作
来源：http://yoq.jinyuanbaomall.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://pkz.cashguo.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qdd.ehwqpu.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hva.zhaomingkeji.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://piy.c1oappe.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://amm.shzxlz.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://isz.hysaishi.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://nym.fzhhl.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://esc.316326.xyz

[D25] Set 集合去重与交并差
来源：http://rmi.gzhubu.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://zkz.c1oappe.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://dsh.yuxming.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://xje.pengpengdd.cyou

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://nvk.cqqwz.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://jem.cucudq.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://phr.redwolf501.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://tjx.zdqjudy.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qgw.shzxlz.cn

[D26] 数组转字符串
来源：http://dvh.xziqi.cn

Py:   ", ".join(map(str, arr))
来源：http://lro.wangdashe.top

PHP:  implode(", ", $arr);
来源：http://bvj.9152youxi.cn

JS:   arr.join(", ")
来源：http://zbj.haohaochexian.top

TS:   arr.join(", ")
来源：http://jjh.fengsongda.top

Java: String.join(", ", list)
来源：http://mzt.gaohongyu789.top

Go:   strings.Join(strs, ", ")
来源：http://hhb.xingfuxueyuan.xyz

Ruby: arr.join(", ")
来源：http://vri.shanyushiyangtech.top

C#:   string.Join(", ", list)
来源：http://ymi.316326.xyz

================================================================================
来源：http://cyh.xinyue.icu

E. 字符串处理
来源：http://wom.jinyuanbaomall.cn

================================================================================
来源：http://msh.gaohongyu789.top

[E01] 拼接字符串
来源：http://ujt.quarkkingdee.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://pen.sufxvd.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://geo.quarkkingdee.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wvd.xziqi.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://xir.ydzc1.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://jlb.fengsongda.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://bra.sysykeji.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://qlz.yueranfly.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wys.xinyue.icu

[E02] 重复字符串
来源：http://fxj.ywan-chungtsiang.top

Py:   "ab" * 3
来源：http://xal.shuidangran.top

PHP:  str_repeat("ab", 3);
来源：http://prf.hysaishi.cn

JS:   "ab".repeat(3)
来源：http://bac.ydjk.org.cn

TS:   "ab".repeat(3)
来源：http://dgg.sjlbkw.cn

Java: "ab".repeat(3)
来源：http://lbr.zhixingplan.top

Go:   strings.Repeat("ab", 3)
来源：http://fkc.kuanghao11.cn

Ruby: "ab" * 3
来源：http://nfg.daria6918.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ael.cqqwz.cn

[E03] 截取子串
来源：http://mem.shanyushiyangtech.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://fun.jqgufenzy.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://nyh.yj20258.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://sjq.bbcook.cn

TS:   s.slice(1, 4)
来源：http://uyx.shanyushiyangtech.top

Java: s.substring(1, 4)
来源：http://xgc.zhijiandao.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://fny.jinyuanbaomall.cn

Ruby: s[1, 3];  s[1..3]
来源：http://zdf.kuanghao11.cn

C#:   s.Substring(1, 3)
来源：http://jmk.gogol.net.cn

[E04] 查找子串位置
来源：http://fqj.redwolf501.top

Py:   s.find("x");  s.index("x")
来源：http://ett.nanxuanxn.top


<!-- 参考信息 -->