代发 wailian999

[C14] 泛型函数
来源：http://pjt.uphjek.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ypj.jinghuilouyu.cn

PHP:  // 无泛型
来源：http://dbd.uphjek.com

JS:   // 无泛型
来源：http://czn.haohaochexian.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://uly.quarkkingdee.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://opx.ydzc1.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://eql.vehdjk.com

Ruby: # 无泛型
来源：http://ade.tanke756.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://khz.zhiwuduotai.top

[C15] 解构 / 展开参数
来源：http://lhr.fanxiaobao.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://jmy.xziqi.cn

PHP:  [$a, $b] = $pair;
来源：http://pxe.ybcxt.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wsn.sufxvd.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://iun.zhongyouzk.top

Java: // 无解构
来源：http://ytv.gogol.net.cn

Go:   // 无解构
来源：http://nzg.shzxlz.cn

Ruby: a, b = pair
来源：http://xxp.jqgufenzy.top

C#:   var (a, b) = pair;
来源：http://jnc.andypj.xyz

[C16] 函数 / 方法重载
来源：http://pwk.316326.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://xux.cqqwz.cn

PHP:  // 无重载
来源：http://csz.havefunace.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://yze.ivvv.top

TS:   // 用联合类型或重载签名声明
来源：http://wcm.ydzc1.top

Java: void f(int a) {}  void f(String a) {}
来源：http://nog.0kj1m.cn

Go:   // 无重载：用不同函数名
来源：http://olw.feifeiyinyue.top

Ruby: # 无重载：靠动态参数
来源：http://lby.ydzc1.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://xbo.birdmap.top

================================================================================
来源：http://ehr.smart0.xyz

D. 数组 / 列表 / 集合
来源：http://gmb.cheryme.top

================================================================================
来源：http://dpk.zhongyouzk.top

[D01] 创建数组 / 列表
来源：http://nwz.ehwqpu.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://bjf.feifeiyinyue.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://phs.smart0.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://bzb.jinyuanbaomall.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://cqf.cqqwz.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://jif.jianghu66.top

Go:   arr := []int{1, 2, 3}
来源：http://ypl.dashuyun.cn

Ruby: arr = [1, 2, 3]
来源：http://qfj.aibaodan.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://zxa.c1oappe.top

[D02] 追加元素到末尾
来源：http://bmi.tian-w.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://yje.yongpay.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ien.chenlongwang.top

JS:   arr.push(4);
来源：http://gig.yangfankeji.com

TS:   arr.push(4);
来源：http://cxr.sxryk.cn

Java: list.add(4);
来源：http://smk.ehwqpu.com

Go:   arr = append(arr, 4)
来源：http://vqm.yvedp.cn

Ruby: arr << 4; arr.push(5)
来源：http://xel.cucudq.cn

C#:   list.Add(4);
来源：http://fxz.havefunace.top

[D03] 在指定位置插入元素
来源：http://dur.tarul.cn

Py:   arr.insert(0, 0)
来源：http://vwj.hywenlv.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://efe.aibaodan.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://yxx.yj20258888.top

TS:   arr.splice(0, 0, 0);
来源：http://qrr.hnqzz.top

Java: list.add(0, 0);
来源：http://wfn.cdnleiting.top

Go:   arr = append([]int{0}, arr...)
来源：http://goo.hfpthk.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://pjo.bjfxy.top

C#:   list.Insert(0, 0);
来源：http://ovj.fengsongda.top

[D04] 删除元素
来源：http://kab.cheryme.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://jmv.hammf.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://qrj.zdbjq.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ndj.chenzaomai.com

TS:   arr.splice(0, 1);
来源：http://hen.bjfxy.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://rwq.vehdjk.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://pdx.jiagoushi.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://dun.bbcook.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://jik.xylfe.cn

[D05] 访问与修改元素
来源：http://nhe.tarul.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://tjy.sxryk.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://zkb.chenlongwang.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://amf.dianchejie.cn

TS:   arr[0]; arr.at(-1);
来源：http://ohj.quarkkingdee.top

Java: list.get(0); list.set(0, 9);
来源：http://mtr.yueranfly.top

Go:   arr[0]; arr[0] = 9
来源：http://uus.tarul.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://cfz.feifeiyinyue.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://dbn.wangshuangyany.cn

[D06] 数组长度
来源：http://dco.xylfe.cn

Py:   len(arr)
来源：http://bnb.quarkkingdee.top

PHP:  count($arr);
来源：http://wmd.daxiang520.top

JS:   arr.length
来源：http://nkj.meibo888.top

TS:   arr.length
来源：http://jgw.quarkkingdee.top

Java: list.size();
来源：http://zng.yonumen.top

Go:   len(arr)
来源：http://kgt.yangfankeji.com

Ruby: arr.length; arr.size
来源：http://qbm.yj20258.top

C#:   list.Count;
来源：http://tjr.yj20258.top

[D07] 切片 / 取子数组
来源：http://pce.jlsjyb.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://cll.jinqigufen.top

PHP:  array_slice($arr, 1, 3);
来源：http://uhb.gaohongyu789.top

JS:   arr.slice(1, 4);
来源：http://avx.cdnleiting.top

TS:   arr.slice(1, 4);
来源：http://krw.uphjek.com

Java: list.subList(1, 4);
来源：http://mte.fzhhl.top

Go:   arr[1:4]
来源：http://zxf.zhaomingkeji.xyz

Ruby: arr[1, 3]
来源：http://prb.hongshengwenyu.top

C#:   list.GetRange(1, 3);
来源：http://hrt.ivvv.top

[D08] 合并两个数组
来源：http://skh.jianghu66.top

Py:   a + b;  a.extend(b)
来源：http://mrq.316326.xyz

PHP:  array_merge($a, $b);
来源：http://byf.tian-w.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://grt.jianghu66.top

TS:   [...a, ...b];
来源：http://xcj.jyoumei.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://yif.ydzc1.top

Go:   append(a, b...)
来源：http://loe.0kj1m.cn

Ruby: a + b;  a.concat(b)
来源：http://ikj.zhoulong.xyz

C#:   a.Concat(b).ToList()
来源：http://lfh.jqgfzy.top

[D09] 排序（升序）
来源：http://anf.ywan-chungtsiang.top

Py:   sorted(arr);  arr.sort()
来源：http://nfp.xingfuxueyuan.xyz

PHP:  sort($arr);
来源：http://oxv.bbcook.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://lrs.birdmap.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://irh.fengsongda.top

Java: Collections.sort(list);  list.sort(null);
来源：http://lig.aizwys.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://aqp.xuanzx.com

Ruby: arr.sort
来源：http://mwr.redwolf501.top

C#:   list.Sort();
来源：http://nzm.chenjidiqi.icu

[D10] 自定义排序（按字段 / 多条件）
来源：http://vuw.hysaishi.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://sac.ctjpmb.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jsk.hongshengwenyu.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://qxq.hesvh.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mmd.yanxiufei.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mer.zhoulong.xyz

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://omc.yueranfly.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://abb.tarul.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://nda.zhijiandao.cn

[D11] 反转数组
来源：http://kcd.dianchejie.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ber.shanyushiyangtech.top

PHP:  array_reverse($arr);
来源：http://bci.shzxlz.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://xil.fzhhl.top

TS:   [...arr].reverse();
来源：http://vya.shuidangran.top

Java: Collections.reverse(list);
来源：http://kkh.fanxiaobao.xyz

Go:   slices.Reverse(arr)
来源：http://tll.vqdsnc.cn

Ruby: arr.reverse
来源：http://zjs.yueranfly.top

C#:   list.Reverse();
来源：http://opy.tarul.cn

[D12] 查找元素下标
来源：http://svk.fktsv.cn

Py:   arr.index(x);  x in arr
来源：http://ttp.pengpengdd.cyou

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://typ.yj20258888.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rld.zhiwuduotai.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rwa.gzhubu.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wfr.wangshuangyany.cn

Go:   slices.Index(arr, x)
来源：http://rcp.birdmap.top

Ruby: arr.index(x)
来源：http://tvq.sufxvd.cn

C#:   list.IndexOf(x);
来源：http://elx.tarul.cn

[D13] 过滤（保留满足条件的）
来源：http://wtu.daxiang520.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://kur.hnqzz.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://bgd.yj20258.top

JS:   arr.filter(x => x > 3)
来源：http://qob.fzhhl.top

TS:   arr.filter(x => x > 3)
来源：http://ufz.hnqzz.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://fvt.tian-w.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://nmj.yanxiufei.cn

Ruby: arr.select { |x| x > 3 }
来源：http://rer.kuanghao11.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://dpn.fktsv.cn

[D14] 映射转换（每个元素变形）
来源：http://skf.nwbrower.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://npb.mhx1999.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ucr.meibo888.top

JS:   arr.map(x => x * 2)
来源：http://jqg.pengpengdd.cyou

TS:   arr.map(x => x * 2)
来源：http://crf.birdmap.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://qsv.jinghuilouyu.cn

Go:   // 手写循环
来源：http://jiu.ybcxt.top

Ruby: arr.map { |x| x * 2 }
来源：http://tte.yanxiufei.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://dze.xuanzx.com

[D15] 去重
来源：http://gze.jinghuilouyu.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wnx.jyoumei.cn

PHP:  array_unique($arr);
来源：http://oaq.guannengcc.top

JS:   [...new Set(arr)]
来源：http://jgm.chenjidiqi.icu

TS:   [...new Set(arr)]
来源：http://haq.shangyingyoupin.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://oli.52xcode.cn

Go:   // 用 map[T]struct{} 手写
来源：http://zij.tian-w.cn

Ruby: arr.uniq
来源：http://eps.ppjwa.cn

C#:   list.Distinct().ToList()
来源：http://nra.sweek.top

[D16] 求和与平均值
来源：http://fqf.jinqigufen.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://coi.xziqi.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://oub.52xcode.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://gad.zhijiandao.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://vwm.cucudq.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://kcs.uphjek.com

Go:   // 手写循环累加
来源：http://qxn.dashuyun.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://eym.bbcook.cn

C#:   list.Sum();  list.Average()
来源：http://dor.yongpay.top

[D17] 最大值与最小值
来源：http://ilc.wangshuangyany.cn

Py:   max(arr);  min(arr)
来源：http://dbh.jinqigfzy.top

PHP:  max($arr);  min($arr);
来源：http://jci.shzxlz.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://iae.316326.xyz

TS:   Math.max(...arr);
来源：http://eda.shanyushiyangtech.top

Java: Collections.max(list);  Collections.min(list);
来源：http://vhj.daria6918.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://bej.cucudq.cn

Ruby: arr.max;  arr.min
来源：http://upf.wangdashe.top

C#:   list.Max();  list.Min()
来源：http://kkx.xylfe.cn

[D18] 扁平化嵌套数组
来源：http://qis.iojbl.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://lcc.hywenlv.cn

PHP:  array_merge(...$nested);
来源：http://pjm.smart0.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://zpl.guannengcc.top

TS:   nested.flat();
来源：http://qwe.jianghu66.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ysb.dianchejie.cn

Go:   // 手写双层循环
来源：http://tke.birdmap.top

Ruby: nested.flatten
来源：http://lva.pycfn.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://zut.zdbjq.cn

[D19] 按字段分组
来源：http://phh.chenzaomai.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://age.xinyue.icu

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ddl.hywenlv.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wdo.vqdsnc.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://wlu.sysykeji.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://gjv.yj20258888.top

Go:   // 手写 map[string][]T
来源：http://aaw.nanxuanxn.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://mba.pycfn.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://icb.nwbrower.top

[D20] 统计每个元素出现次数
来源：http://vmq.fengsongda.top

Py:   Counter(arr)
来源：http://xlc.yueranfly.top

PHP:  array_count_values($arr);
来源：http://ezt.nwbrower.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ber.ydjk.org.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://avg.vqdsnc.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://yqr.hammf.cn

Go:   // 手写 map[T]int
来源：http://jvc.sysykeji.top

Ruby: arr.tally
来源：http://uyp.316326.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://rtv.fzhhl.top

[D21] 判断是否包含某元素
来源：http://zpx.hcnkem.com

Py:   x in arr
来源：http://mmz.daxiang520.top

PHP:  in_array($x, $arr, true);
来源：http://rmu.yuanzhike.top

JS:   arr.includes(x)
来源：http://neb.guannengcc.top

TS:   arr.includes(x)
来源：http://doj.iojbl.cn

Java: list.contains(x)
来源：http://eky.ydzc1.top

Go:   slices.Contains(arr, x)
来源：http://qeb.zhongyouzk.top

Ruby: arr.include?(x)
来源：http://twi.jinghuilouyu.cn

C#:   list.Contains(x)
来源：http://amw.hywenlv.cn

[D22] 复制数组（避免共享引用）
来源：http://rjk.svipenyu.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ats.zhongyouzk.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://fwk.c1oappe.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://yth.zdqjudy.top

TS:   [...arr];
来源：http://zgy.chenjidiqi.icu

Java: new ArrayList<>(list);
来源：http://tiz.shanyushiyangtech.top

Go:   copied := append([]int(nil), arr...)
来源：http://nkb.daxiang520.top

Ruby: arr.dup;  arr.clone
来源：http://dbq.hysaishi.cn

C#:   new List<int>(list);
来源：http://nhl.havefunace.top

[D23] reduce 累积计算
来源：http://jwu.hywenlv.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blp.xinyue.icu

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://vjx.cashguo.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tin.0kj1m.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://llq.chenjidiqi.icu

Java: list.stream().reduce(0, Integer::sum)
来源：http://wfz.hywenlv.cn

Go:   // 手写循环
来源：http://lei.bbcook.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://twf.shangyingyoupin.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mzq.hcnkem.com

[D24] 字典 / Map 基本操作
来源：http://dtv.zhoulong.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://xws.sjlbkw.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://djc.bjfxy.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xkn.havefunace.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://vcq.guannengcc.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://kid.svipenyu.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://aof.zhoulong.xyz

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://zos.zhijiandao.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://bpm.dashuyun.cn

[D25] Set 集合去重与交并差
来源：http://zwq.zycfv.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://zzs.jinyuanbaomall.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://bve.hnqzz.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://fyy.yvedp.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://tto.haohaochexian.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://eyq.sxryk.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://rwm.fanxiaobao.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://stx.jianghu66.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mkq.nanxuanxn.top

[D26] 数组转字符串
来源：http://vzf.zhaomingkeji.xyz

Py:   ", ".join(map(str, arr))
来源：http://cds.quarkkingdee.top

PHP:  implode(", ", $arr);
来源：http://ugr.52xcode.cn

JS:   arr.join(", ")
来源：http://drg.0kj1m.cn

TS:   arr.join(", ")
来源：http://mbp.jlsjyb.cn

Java: String.join(", ", list)
来源：http://njn.xingfuxueyuan.xyz

Go:   strings.Join(strs, ", ")
来源：http://hmw.jqgufenzy.top

Ruby: arr.join(", ")
来源：http://naa.vehdjk.com

C#:   string.Join(", ", list)
来源：http://yxq.316326.xyz

================================================================================
来源：http://blw.gzhubu.top

E. 字符串处理
来源：http://bnv.cucudq.cn

================================================================================
来源：http://lnm.sufxvd.cn

[E01] 拼接字符串
来源：http://wpw.shanyushiyangtech.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ufr.jlsjyb.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://lxq.gzhubu.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ule.yj20258888.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://eiz.andypj.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://oim.chenzaomai.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://vkc.wangshuangyany.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blq.hywenlv.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://afo.ybcxt.top

[E02] 重复字符串
来源：http://zmt.pycfn.com

Py:   "ab" * 3
来源：http://mes.kuanghao11.cn

PHP:  str_repeat("ab", 3);
来源：http://vfs.jianghu66.top

JS:   "ab".repeat(3)
来源：http://ogw.sufxvd.cn

TS:   "ab".repeat(3)
来源：http://zsz.redwolf501.top

Java: "ab".repeat(3)
来源：http://zkh.dashuyun.cn

Go:   strings.Repeat("ab", 3)
来源：http://byn.yfazqb.com

Ruby: "ab" * 3
来源：http://kqv.sxryk.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ncx.wangdashe.top

[E03] 截取子串
来源：http://ouf.dianchejie.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://tzr.aizwys.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://zot.sjlbkw.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wkx.hcnkem.com

TS:   s.slice(1, 4)
来源：http://oht.shangyingyoupin.top

Java: s.substring(1, 4)
来源：http://idn.316326.xyz

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://jsy.xuetiantiany.cn

Ruby: s[1, 3];  s[1..3]
来源：http://pqq.sysykeji.top

C#:   s.Substring(1, 3)
来源：http://kzw.daria6918.cn

[E04] 查找子串位置
来源：http://bqm.feifeiyinyue.top

Py:   s.find("x");  s.index("x")
来源：http://gcl.jyoumei.cn

PHP:  strpos($s, "x");
来源：http://bxi.hywenlv.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://uuu.pycfn.com

TS:   s.indexOf("x")
来源：http://jzm.yj202588.top

Java: s.indexOf("x")
来源：http://iae.vqdsnc.cn


<!-- 参考信息 -->