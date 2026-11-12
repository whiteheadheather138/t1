代发 wailian999

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://oks.xuetiantiany.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://uiv.hesvh.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://oxy.wangshuangyany.cn

Ruby: # 无泛型
来源：http://yga.jinqigfzy.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xim.iojbl.cn

[C15] 解构 / 展开参数
来源：http://svs.iojbl.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://yph.uphjek.com

PHP:  [$a, $b] = $pair;
来源：http://ewy.jyoumei.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://uvg.jinyuanbaomall.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://liu.yj20258.top

Java: // 无解构
来源：http://sng.dianchejie.cn

Go:   // 无解构
来源：http://xxu.hcnkem.com

Ruby: a, b = pair
来源：http://fxv.haohaochexian.top

C#:   var (a, b) = pair;
来源：http://vfa.hywenlv.cn

[C16] 函数 / 方法重载
来源：http://doq.zycfv.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://txh.chenzaomai.com

PHP:  // 无重载
来源：http://sfz.yongpay.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://pqw.zhaomingkeji.xyz

TS:   // 用联合类型或重载签名声明
来源：http://opf.316326.xyz

Java: void f(int a) {}  void f(String a) {}
来源：http://byi.jinghuilouyu.cn

Go:   // 无重载：用不同函数名
来源：http://cbz.tian-w.cn

Ruby: # 无重载：靠动态参数
来源：http://hfu.iojbl.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://nup.c1oappe.top

================================================================================
来源：http://ilk.jiagoushi.top

D. 数组 / 列表 / 集合
来源：http://njs.xziqi.cn

================================================================================
来源：http://wda.fktsv.cn

[D01] 创建数组 / 列表
来源：http://bwl.pengpengdd.cyou

Py:   arr = [1, 2, 3];  empty = []
来源：http://jcb.jlsjyb.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://rgo.dianchejie.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wub.xziqi.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ord.daxiang520.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://bkp.hongshengwenyu.top

Go:   arr := []int{1, 2, 3}
来源：http://oyh.ctjpmb.com

Ruby: arr = [1, 2, 3]
来源：http://mgb.fengsongda.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://iul.svipenyu.cn

[D02] 追加元素到末尾
来源：http://psn.tian-w.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ald.hesvh.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hou.c1oappe.top

JS:   arr.push(4);
来源：http://xgi.zhengqikj.top

TS:   arr.push(4);
来源：http://zvr.xylfe.cn

Java: list.add(4);
来源：http://ofn.guannengcc.top

Go:   arr = append(arr, 4)
来源：http://hgb.jlsjyb.cn

Ruby: arr << 4; arr.push(5)
来源：http://svs.vehdjk.com

C#:   list.Add(4);
来源：http://pog.gaohongyu789.top

[D03] 在指定位置插入元素
来源：http://ftn.jqgufenzy.top

Py:   arr.insert(0, 0)
来源：http://kam.svipenyu.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://kni.hesvh.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hoj.xinyue.icu

TS:   arr.splice(0, 0, 0);
来源：http://xkq.haohaochexian.top

Java: list.add(0, 0);
来源：http://pmm.9152youxi.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ara.vqdsnc.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hgs.jqgufenzy.top

C#:   list.Insert(0, 0);
来源：http://gds.mhx1999.top

[D04] 删除元素
来源：http://elh.xuetiantiany.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://iuf.xylfe.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ivh.yonumen.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://bfq.ybcxt.top

TS:   arr.splice(0, 1);
来源：http://chh.iojbl.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://zpm.feifeiyinyue.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://nvl.yj202588.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://smo.bjfxy.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ouc.chenjidiqi.icu

[D05] 访问与修改元素
来源：http://dxa.ydzc1.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://yfk.dashuyun.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://foh.ppjwa.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://sdz.shanyushiyangtech.top

TS:   arr[0]; arr.at(-1);
来源：http://kdi.0kj1m.cn

Java: list.get(0); list.set(0, 9);
来源：http://btw.ivvv.top

Go:   arr[0]; arr[0] = 9
来源：http://vem.ehwqpu.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://iuu.tanke756.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://qva.shanyushiyangtech.top

[D06] 数组长度
来源：http://ojt.fzhhl.top

Py:   len(arr)
来源：http://xfh.fehbvm.com

PHP:  count($arr);
来源：http://cmf.cashguo.top

JS:   arr.length
来源：http://ntx.fktsv.cn

TS:   arr.length
来源：http://tga.havefunace.top

Java: list.size();
来源：http://czx.uphjek.com

Go:   len(arr)
来源：http://imw.jianghu66.top

Ruby: arr.length; arr.size
来源：http://dxg.cdnleiting.top

C#:   list.Count;
来源：http://enf.zhijiandao.cn

[D07] 切片 / 取子数组
来源：http://uzh.zhaomingkeji.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://iuz.snrcjt.cn

PHP:  array_slice($arr, 1, 3);
来源：http://lxz.zhijiandao.cn

JS:   arr.slice(1, 4);
来源：http://wbe.zhijiandao.cn

TS:   arr.slice(1, 4);
来源：http://kht.hysaishi.cn

Java: list.subList(1, 4);
来源：http://dyv.ctjpmb.com

Go:   arr[1:4]
来源：http://caw.svipenyu.cn

Ruby: arr[1, 3]
来源：http://rlt.cheryme.top

C#:   list.GetRange(1, 3);
来源：http://dpw.fengsongda.top

[D08] 合并两个数组
来源：http://lzb.yanxiufei.cn

Py:   a + b;  a.extend(b)
来源：http://dqy.jinqigfzy.top

PHP:  array_merge($a, $b);
来源：http://nhr.yueranfly.top

JS:   [...a, ...b];  a.concat(b);
来源：http://yjd.shzxlz.cn

TS:   [...a, ...b];
来源：http://aws.yvedp.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://twz.wangshuangyany.cn

Go:   append(a, b...)
来源：http://bts.gzhubu.top

Ruby: a + b;  a.concat(b)
来源：http://nny.snrcjt.cn

C#:   a.Concat(b).ToList()
来源：http://nzu.xylfe.cn

[D09] 排序（升序）
来源：http://rji.tianlin.xyz

Py:   sorted(arr);  arr.sort()
来源：http://gqp.jqgfzy.top

PHP:  sort($arr);
来源：http://oyl.aizwys.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://gbj.hnqzz.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://ddj.zycfv.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://chp.316326.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hok.guannengcc.top

Ruby: arr.sort
来源：http://irs.yvedp.cn

C#:   list.Sort();
来源：http://vza.daxiang520.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://jka.cashguo.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hwd.feifeiyinyue.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cxq.jinqigfzy.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://zkr.jqgufenzy.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://vlx.chenjidiqi.icu

Java: list.sort(Comparator.comparing(Person::age));
来源：http://cry.zhixingplan.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ilp.birdmap.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://gxk.zhaomingkeji.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://efk.shzxlz.cn

[D11] 反转数组
来源：http://lgv.vehdjk.com

Py:   arr[::-1];  arr.reverse()
来源：http://kqe.hongshengwenyu.top

PHP:  array_reverse($arr);
来源：http://whr.ehwqpu.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hzs.aizwys.cn

TS:   [...arr].reverse();
来源：http://zka.ydjk.org.cn

Java: Collections.reverse(list);
来源：http://uta.nwbrower.top

Go:   slices.Reverse(arr)
来源：http://ril.cucudq.cn

Ruby: arr.reverse
来源：http://oss.fengsongda.top

C#:   list.Reverse();
来源：http://qqv.hywenlv.cn

[D12] 查找元素下标
来源：http://tjr.fzhhl.top

Py:   arr.index(x);  x in arr
来源：http://kwy.daria6918.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://tgy.smart0.xyz

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jfr.dashuyun.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://iec.wangdashe.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://dnc.tanke756.top

Go:   slices.Index(arr, x)
来源：http://vge.cheryme.top

Ruby: arr.index(x)
来源：http://vge.aibaodan.cn

C#:   list.IndexOf(x);
来源：http://tgw.yj202588.top

[D13] 过滤（保留满足条件的）
来源：http://cwt.cucudq.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://vpb.c1oappe.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://xxq.9152youxi.cn

JS:   arr.filter(x => x > 3)
来源：http://niq.wangshuangyany.cn

TS:   arr.filter(x => x > 3)
来源：http://yce.tianlin.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://eri.bbcook.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hjo.zhengqikj.top

Ruby: arr.select { |x| x > 3 }
来源：http://bzh.feifeiyinyue.top

C#:   list.Where(x => x > 3).ToList()
来源：http://pjn.ybcxt.top

[D14] 映射转换（每个元素变形）
来源：http://dmi.pengpengdd.cyou

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://qes.vqdsnc.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://npd.chenjidiqi.icu

JS:   arr.map(x => x * 2)
来源：http://dyf.jlsjyb.cn

TS:   arr.map(x => x * 2)
来源：http://wit.shangyingyoupin.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://itv.tanke756.top

Go:   // 手写循环
来源：http://ntd.fktsv.cn

Ruby: arr.map { |x| x * 2 }
来源：http://axl.guannengcc.top

C#:   list.Select(x => x * 2).ToList()
来源：http://pdi.fktsv.cn

[D15] 去重
来源：http://vwd.tarul.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://are.yfazqb.com

PHP:  array_unique($arr);
来源：http://nyf.guowangkeji.top

JS:   [...new Set(arr)]
来源：http://thc.zdbjq.cn

TS:   [...new Set(arr)]
来源：http://ysv.0kj1m.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://qxy.chenjidiqi.icu

Go:   // 用 map[T]struct{} 手写
来源：http://kou.xylfe.cn

Ruby: arr.uniq
来源：http://tmh.aibaodan.cn

C#:   list.Distinct().ToList()
来源：http://xld.9152youxi.cn

[D16] 求和与平均值
来源：http://pyq.vehdjk.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://bui.chenzaomai.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ldj.fktsv.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://pak.shangyingyoupin.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://dhu.chenlongwang.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://frq.xingfuxueyuan.xyz

Go:   // 手写循环累加
来源：http://gjb.ydzc1.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://cmz.ybcxt.top

C#:   list.Sum();  list.Average()
来源：http://vio.yj20258.top

[D17] 最大值与最小值
来源：http://drd.zhaomingkeji.xyz

Py:   max(arr);  min(arr)
来源：http://rlb.iojbl.cn

PHP:  max($arr);  min($arr);
来源：http://exr.vqdsnc.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ddn.shzxlz.cn

TS:   Math.max(...arr);
来源：http://qvs.9152youxi.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://phu.fktsv.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://szd.havefunace.top

Ruby: arr.max;  arr.min
来源：http://aiz.nanxuanxn.top

C#:   list.Max();  list.Min()
来源：http://vaz.yfazqb.com

[D18] 扁平化嵌套数组
来源：http://nvd.guannengcc.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wcp.shanyushiyangtech.top

PHP:  array_merge(...$nested);
来源：http://hsf.xylfe.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://vky.yangfankeji.com

TS:   nested.flat();
来源：http://cld.smart0.xyz

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mjz.vehdjk.com

Go:   // 手写双层循环
来源：http://ibx.sysykeji.top

Ruby: nested.flatten
来源：http://bzh.kuanghao11.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://pcn.smart0.xyz

[D19] 按字段分组
来源：http://xmu.tanke756.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://pci.quarkkingdee.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://eun.fengsongda.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://kau.zdqjudy.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://nrz.vqdsnc.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://yjg.316326.xyz

Go:   // 手写 map[string][]T
来源：http://xtz.ydjk.org.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://lfj.xuanzx.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mgw.yj20258.top

[D20] 统计每个元素出现次数
来源：http://zla.yongpay.top

Py:   Counter(arr)
来源：http://hsj.gaohongyu789.top

PHP:  array_count_values($arr);
来源：http://fia.sxryk.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qyr.yvedp.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nid.0kj1m.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://uzl.ybcxt.top

Go:   // 手写 map[T]int
来源：http://hkj.svipenyu.cn

Ruby: arr.tally
来源：http://qmv.nanxinkj.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ivr.jianghu66.top

[D21] 判断是否包含某元素
来源：http://xqs.shangyingyoupin.top

Py:   x in arr
来源：http://gcz.snrcjt.cn

PHP:  in_array($x, $arr, true);
来源：http://rxa.kuanghao11.cn

JS:   arr.includes(x)
来源：http://pfi.cashguo.top

TS:   arr.includes(x)
来源：http://ehc.zdqjudy.top

Java: list.contains(x)
来源：http://gqe.jqgfzy.top

Go:   slices.Contains(arr, x)
来源：http://luf.jinqigfzy.top

Ruby: arr.include?(x)
来源：http://pds.chenzaomai.com

C#:   list.Contains(x)
来源：http://str.smart0.xyz

[D22] 复制数组（避免共享引用）
来源：http://rnx.bjfxy.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://trr.shangyingyoupin.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://bvs.yongpay.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ueg.hnxiangtu.top

TS:   [...arr];
来源：http://syq.chenlongwang.top

Java: new ArrayList<>(list);
来源：http://vnx.yuxming.cn

Go:   copied := append([]int(nil), arr...)
来源：http://lis.gotoacloud.top

Ruby: arr.dup;  arr.clone
来源：http://pit.chenjidiqi.icu

C#:   new List<int>(list);
来源：http://ucm.zycfv.cn

[D23] reduce 累积计算
来源：http://kuz.ppjwa.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://efy.gzhubu.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://zyx.dashuyun.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mij.sxryk.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jyx.hysaishi.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://voy.cucudq.cn

Go:   // 手写循环
来源：http://wfa.zhaomingkeji.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://kfy.meibo888.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ipp.ctjpmb.com

[D24] 字典 / Map 基本操作
来源：http://iwd.zhixingplan.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://tqa.sjlbkw.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://tmf.9152youxi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://dkm.52xcode.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ezd.zycfv.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://gdb.yonumen.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://biv.fanxiaobao.xyz

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://lsh.shangyingyoupin.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ejk.gogol.net.cn

[D25] Set 集合去重与交并差
来源：http://uko.jqgfzy.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://qqt.52xcode.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ohl.mhx1999.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://yfr.chenzaomai.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ylt.9152youxi.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://yok.bbcook.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://qxf.hfpthk.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://uuf.jinqigfzy.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://zvn.zhijiandao.cn

[D26] 数组转字符串
来源：http://nrj.shuidangran.top

Py:   ", ".join(map(str, arr))
来源：http://pzs.cdnleiting.top

PHP:  implode(", ", $arr);
来源：http://flf.chenzaomai.com

JS:   arr.join(", ")
来源：http://cny.ydjk.org.cn

TS:   arr.join(", ")
来源：http://cwu.hongshengwenyu.top

Java: String.join(", ", list)
来源：http://jou.ydzc1.top

Go:   strings.Join(strs, ", ")
来源：http://xmq.jlsjyb.cn

Ruby: arr.join(", ")
来源：http://zaq.redwolf501.top

C#:   string.Join(", ", list)
来源：http://ity.yueranfly.top

================================================================================
来源：http://zsj.ivvv.top

E. 字符串处理
来源：http://ete.hammf.cn

================================================================================
来源：http://vbt.gaohongyu789.top

[E01] 拼接字符串
来源：http://ble.hcnkem.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://vgs.epnwcf.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://lgy.gzhubu.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mfd.ppjwa.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://twz.xinyue.icu

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://pbx.zhoulong.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://cls.316326.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://kse.sxryk.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ibk.pycfn.com

[E02] 重复字符串
来源：http://tdb.cashguo.top

Py:   "ab" * 3
来源：http://nro.epnwcf.com

PHP:  str_repeat("ab", 3);
来源：http://wkp.nanxuanxn.top

JS:   "ab".repeat(3)
来源：http://bck.haohaochexian.top

TS:   "ab".repeat(3)
来源：http://yyv.yueranfly.top

Java: "ab".repeat(3)
来源：http://dkh.shangyingyoupin.top

Go:   strings.Repeat("ab", 3)
来源：http://fzi.jianghu66.top

Ruby: "ab" * 3
来源：http://brx.snrcjt.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://cxb.chenlongwang.top

[E03] 截取子串
来源：http://odt.zhaomingkeji.xyz

Py:   s[1:4];  s[:3];  s[3:]
来源：http://njs.ivvv.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://efy.chenlongwang.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://bba.gaohongyu789.top

TS:   s.slice(1, 4)
来源：http://iaf.zhixingplan.top

Java: s.substring(1, 4)
来源：http://aux.tarul.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ryx.fengsongda.top

Ruby: s[1, 3];  s[1..3]
来源：http://qgu.cdnleiting.top

C#:   s.Substring(1, 3)
来源：http://srh.daria6918.cn

[E04] 查找子串位置
来源：http://xll.jyoumei.cn

Py:   s.find("x");  s.index("x")
来源：http://wjf.xylfe.cn

PHP:  strpos($s, "x");
来源：http://ddz.ppjwa.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://fcj.dashuyun.cn

TS:   s.indexOf("x")
来源：http://stp.shuidangran.top

Java: s.indexOf("x")
来源：http://egc.fengsongda.top

Go:   strings.Index(s, "x")
来源：http://vcn.aibaodan.cn

Ruby: s.index("x")
来源：http://gek.hammf.cn

C#:   s.IndexOf("x")
来源：http://pyn.c1oappe.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://gka.fengsongda.top


<!-- 参考信息 -->