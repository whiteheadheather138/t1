代发 wailian999

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://vfu.jianghu66.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://pjs.ydzc1.top

Java: // 无解构
来源：http://vjb.dianchejie.cn

Go:   // 无解构
来源：http://kvn.cdnleiting.top

Ruby: a, b = pair
来源：http://drm.havefunace.top

C#:   var (a, b) = pair;
来源：http://aoj.hnxiangtu.top

[C16] 函数 / 方法重载
来源：http://jxu.c1oappe.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://lfq.yj20258.top

PHP:  // 无重载
来源：http://mie.sufxvd.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ivm.52xcode.cn

TS:   // 用联合类型或重载签名声明
来源：http://fgc.havefunace.top

Java: void f(int a) {}  void f(String a) {}
来源：http://dbq.shzxlz.cn

Go:   // 无重载：用不同函数名
来源：http://qhf.meibo888.top

Ruby: # 无重载：靠动态参数
来源：http://irk.shuidangran.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://yhn.svipenyu.cn

================================================================================
来源：http://rnj.ctjpmb.com

D. 数组 / 列表 / 集合
来源：http://wfh.shanyushiyangtech.top

================================================================================
来源：http://uhj.9152youxi.cn

[D01] 创建数组 / 列表
来源：http://dqm.tarul.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://bgo.wangshuangyany.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://qis.zhengqikj.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://osg.zhijiandao.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://dyp.sysykeji.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://zez.yuxming.cn

Go:   arr := []int{1, 2, 3}
来源：http://sfu.daxiang520.top

Ruby: arr = [1, 2, 3]
来源：http://zmq.uphjek.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://yxd.kuanghao11.cn

[D02] 追加元素到末尾
来源：http://nse.svipenyu.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://kwh.jqgfzy.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://yew.gotoacloud.top

JS:   arr.push(4);
来源：http://gro.zycfv.cn

TS:   arr.push(4);
来源：http://zzm.uphjek.com

Java: list.add(4);
来源：http://xlu.wangshuangyany.cn

Go:   arr = append(arr, 4)
来源：http://jgd.fengsongda.top

Ruby: arr << 4; arr.push(5)
来源：http://jgl.dashuyun.cn

C#:   list.Add(4);
来源：http://vjb.epnwcf.com

[D03] 在指定位置插入元素
来源：http://cwc.epnwcf.com

Py:   arr.insert(0, 0)
来源：http://qxl.hnqzz.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ius.ydzc1.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://xsk.tarul.cn

TS:   arr.splice(0, 0, 0);
来源：http://gai.zhaomingkeji.xyz

Java: list.add(0, 0);
来源：http://wiz.ybcxt.top

Go:   arr = append([]int{0}, arr...)
来源：http://pdh.smart0.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://czr.tian-w.cn

C#:   list.Insert(0, 0);
来源：http://cfg.cucudq.cn

[D04] 删除元素
来源：http://gvk.nwbrower.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://cyi.zhoulong.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mev.daxiang520.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://zop.guowangkeji.top

TS:   arr.splice(0, 1);
来源：http://use.hongshengwenyu.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ttb.cheryme.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wpe.ywan-chungtsiang.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://pnn.yfazqb.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://kdn.zycfv.cn

[D05] 访问与修改元素
来源：http://cva.yueranfly.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://bbq.hnqzz.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://snm.shangyingyoupin.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://lxv.dianchejie.cn

TS:   arr[0]; arr.at(-1);
来源：http://cns.epnwcf.com

Java: list.get(0); list.set(0, 9);
来源：http://gfs.zhaomingkeji.xyz

Go:   arr[0]; arr[0] = 9
来源：http://ney.yonumen.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://nwn.zycfv.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://pna.fzhhl.top

[D06] 数组长度
来源：http://fnq.tarul.cn

Py:   len(arr)
来源：http://dad.cqqwz.cn

PHP:  count($arr);
来源：http://mhc.shanyushiyangtech.top

JS:   arr.length
来源：http://sbk.c1oappe.top

TS:   arr.length
来源：http://pes.nwbrower.top

Java: list.size();
来源：http://xut.ehwqpu.com

Go:   len(arr)
来源：http://cbu.gzhubu.top

Ruby: arr.length; arr.size
来源：http://pzb.jiagoushi.top

C#:   list.Count;
来源：http://xin.cashguo.top

[D07] 切片 / 取子数组
来源：http://tga.yuanzhike.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wid.hywenlv.cn

PHP:  array_slice($arr, 1, 3);
来源：http://soc.jlsjyb.cn

JS:   arr.slice(1, 4);
来源：http://bck.ppjwa.cn

TS:   arr.slice(1, 4);
来源：http://tol.gzhubu.top

Java: list.subList(1, 4);
来源：http://lrl.sxryk.cn

Go:   arr[1:4]
来源：http://vpl.nwbrower.top

Ruby: arr[1, 3]
来源：http://lze.vehdjk.com

C#:   list.GetRange(1, 3);
来源：http://ema.jiagoushi.top

[D08] 合并两个数组
来源：http://cfq.uphjek.com

Py:   a + b;  a.extend(b)
来源：http://qew.jinqigfzy.top

PHP:  array_merge($a, $b);
来源：http://nju.tian-w.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ofh.hywenlv.cn

TS:   [...a, ...b];
来源：http://wfs.nanxinkj.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://eji.xuetiantiany.cn

Go:   append(a, b...)
来源：http://end.zdqjudy.top

Ruby: a + b;  a.concat(b)
来源：http://skp.iojbl.cn

C#:   a.Concat(b).ToList()
来源：http://ryv.guowangkeji.top

[D09] 排序（升序）
来源：http://iak.gogol.net.cn

Py:   sorted(arr);  arr.sort()
来源：http://vzm.yvedp.cn

PHP:  sort($arr);
来源：http://ezg.shangyingyoupin.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://kpe.svipenyu.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://avm.haohaochexian.top

Java: Collections.sort(list);  list.sort(null);
来源：http://ruw.daxiang520.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://tsv.tianlin.xyz

Ruby: arr.sort
来源：http://jdw.xylfe.cn

C#:   list.Sort();
来源：http://bmp.xinyue.icu

[D10] 自定义排序（按字段 / 多条件）
来源：http://qcn.shanyushiyangkeji.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://brt.aizwys.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bef.yuanzhike.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://rsf.daria6918.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://kif.jinyuanbaomall.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://cjk.tian-w.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://pwf.uphjek.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://lax.sxryk.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ewy.mhx1999.top

[D11] 反转数组
来源：http://oay.gotoacloud.top

Py:   arr[::-1];  arr.reverse()
来源：http://uga.shuidangran.top

PHP:  array_reverse($arr);
来源：http://krx.shangyingyoupin.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://rpp.vqdsnc.cn

TS:   [...arr].reverse();
来源：http://ebw.jlsjyb.cn

Java: Collections.reverse(list);
来源：http://uge.guowangkeji.top

Go:   slices.Reverse(arr)
来源：http://kln.aizwys.cn

Ruby: arr.reverse
来源：http://dus.gaohongyu789.top

C#:   list.Reverse();
来源：http://iyg.tian-w.cn

[D12] 查找元素下标
来源：http://wqz.gaohongyu789.top

Py:   arr.index(x);  x in arr
来源：http://ahf.cqqwz.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://jjt.nanxuanxn.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wsd.fktsv.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gnr.gaohongyu789.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://kdz.fzhhl.top

Go:   slices.Index(arr, x)
来源：http://mda.c1oappe.top

Ruby: arr.index(x)
来源：http://zhy.jinghuilouyu.cn

C#:   list.IndexOf(x);
来源：http://tyr.havefunace.top

[D13] 过滤（保留满足条件的）
来源：http://zas.yj20258.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ida.sxryk.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://vki.gogol.net.cn

JS:   arr.filter(x => x > 3)
来源：http://vzl.fzhhl.top

TS:   arr.filter(x => x > 3)
来源：http://bas.fzhhl.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://klt.jinyuanbaomall.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mpp.tarul.cn

Ruby: arr.select { |x| x > 3 }
来源：http://pop.yj20258888.top

C#:   list.Where(x => x > 3).ToList()
来源：http://yey.ppjwa.cn

[D14] 映射转换（每个元素变形）
来源：http://wuw.shanyushiyangkeji.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://qef.jinqigfzy.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ori.zhiwuduotai.top

JS:   arr.map(x => x * 2)
来源：http://uov.shuidangran.top

TS:   arr.map(x => x * 2)
来源：http://kqm.hcnkem.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://rqn.andypj.xyz

Go:   // 手写循环
来源：http://upt.shanyushiyangtech.top

Ruby: arr.map { |x| x * 2 }
来源：http://ico.cqqwz.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://llk.jiagoushi.top

[D15] 去重
来源：http://nkr.yj20258888.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ksu.jiagoushi.top

PHP:  array_unique($arr);
来源：http://mag.smart0.xyz

JS:   [...new Set(arr)]
来源：http://dyl.zhaomingkeji.xyz

TS:   [...new Set(arr)]
来源：http://klo.shangyingyoupin.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ymd.cqqwz.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ydt.bjfxy.top

Ruby: arr.uniq
来源：http://tcq.cqqwz.cn

C#:   list.Distinct().ToList()
来源：http://spx.jinqigufen.top

[D16] 求和与平均值
来源：http://ybf.jianghu66.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://gpk.fzhhl.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://tes.hongshengwenyu.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hso.sysykeji.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://txc.ydzc1.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ocs.sweek.top

Go:   // 手写循环累加
来源：http://ymk.yuxming.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://qhz.havefunace.top

C#:   list.Sum();  list.Average()
来源：http://auz.fengsongda.top

[D17] 最大值与最小值
来源：http://efy.snrcjt.cn

Py:   max(arr);  min(arr)
来源：http://caj.zhoulong.xyz

PHP:  max($arr);  min($arr);
来源：http://dmd.guannengcc.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://nwp.jqgufenzy.top

TS:   Math.max(...arr);
来源：http://tzr.gotoacloud.top

Java: Collections.max(list);  Collections.min(list);
来源：http://qbt.bjfxy.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://xtw.zhixingplan.top

Ruby: arr.max;  arr.min
来源：http://ljz.fktsv.cn

C#:   list.Max();  list.Min()
来源：http://iqg.zhiwuduotai.top

[D18] 扁平化嵌套数组
来源：http://ygv.guannengcc.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://jrn.fzhhl.top

PHP:  array_merge(...$nested);
来源：http://nrd.0kj1m.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://vxj.cucudq.cn

TS:   nested.flat();
来源：http://cmn.chenjidiqi.icu

Java: nested.stream().flatMap(List::stream).toList()
来源：http://vob.hnxiangtu.top

Go:   // 手写双层循环
来源：http://gae.zdqjudy.top

Ruby: nested.flatten
来源：http://bhu.316326.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://rgl.chenlongwang.top

[D19] 按字段分组
来源：http://wte.yvedp.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://noc.zycfv.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hqq.zhongyouzk.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://lxu.pengpengdd.cyou

TS:   Object.groupBy(arr, x => x.type)
来源：http://nmk.hnxiangtu.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://kfw.hywenlv.cn

Go:   // 手写 map[string][]T
来源：http://nuk.zhaomingkeji.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://oyu.fzhhl.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://gsm.shuidangran.top

[D20] 统计每个元素出现次数
来源：http://yxs.hysaishi.cn

Py:   Counter(arr)
来源：http://oav.yangfankeji.com

PHP:  array_count_values($arr);
来源：http://grj.jianghu66.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gnx.tian-w.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wuq.yvedp.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://etk.yfazqb.com

Go:   // 手写 map[T]int
来源：http://qfj.chenzaomai.com

Ruby: arr.tally
来源：http://obf.fanxiaobao.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://tkd.jqgufenzy.top

[D21] 判断是否包含某元素
来源：http://nfk.jinqigufen.top

Py:   x in arr
来源：http://idd.c1oappe.top

PHP:  in_array($x, $arr, true);
来源：http://wyx.52xcode.cn

JS:   arr.includes(x)
来源：http://zbt.c1oappe.top

TS:   arr.includes(x)
来源：http://kjy.zhiwuduotai.top

Java: list.contains(x)
来源：http://qwv.hammf.cn

Go:   slices.Contains(arr, x)
来源：http://stj.gzhubu.top

Ruby: arr.include?(x)
来源：http://mbc.hcnkem.com

C#:   list.Contains(x)
来源：http://ojg.shanyushiyangkeji.top

[D22] 复制数组（避免共享引用）
来源：http://xpr.nanxinkj.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://imj.xuetiantiany.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wpe.birdmap.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://nqp.zhijiandao.cn

TS:   [...arr];
来源：http://chj.shangyingyoupin.top

Java: new ArrayList<>(list);
来源：http://liu.jqgfzy.top

Go:   copied := append([]int(nil), arr...)
来源：http://iih.cheryme.top

Ruby: arr.dup;  arr.clone
来源：http://jvh.zdbjq.cn

C#:   new List<int>(list);
来源：http://mxn.zhengqikj.top

[D23] reduce 累积计算
来源：http://tpf.ctjpmb.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://osy.xinyue.icu

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://fkk.yonumen.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://huw.xziqi.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rib.daxiang520.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://frx.bjfxy.top

Go:   // 手写循环
来源：http://sov.gaohongyu789.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://bxa.aizwys.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://rco.ivvv.top

[D24] 字典 / Map 基本操作
来源：http://gnx.jinqigfzy.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://asx.pengpengdd.cyou

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ejj.wangdashe.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://qey.wangshuangyany.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://gyz.meibo888.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://dss.shuidangran.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://omu.ywan-chungtsiang.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://qnq.epnwcf.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://bch.tarul.cn

[D25] Set 集合去重与交并差
来源：http://khm.mhx1999.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://sgl.shangyingyoupin.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://aix.yuxming.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://vsa.yj20258888.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://rkc.shanyushiyangkeji.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://tik.mhx1999.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mqk.52xcode.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://axc.sysykeji.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://nzi.smart0.xyz

[D26] 数组转字符串
来源：http://ett.yuxming.cn

Py:   ", ".join(map(str, arr))
来源：http://pqz.316326.xyz

PHP:  implode(", ", $arr);
来源：http://wid.pengpengdd.cyou

JS:   arr.join(", ")
来源：http://coe.fktsv.cn

TS:   arr.join(", ")
来源：http://wgk.jinqigufen.top

Java: String.join(", ", list)
来源：http://vdc.zhengqikj.top

Go:   strings.Join(strs, ", ")
来源：http://cvb.yvedp.cn

Ruby: arr.join(", ")
来源：http://yje.52xcode.cn

C#:   string.Join(", ", list)
来源：http://jsp.vqdsnc.cn

================================================================================
来源：http://kzt.tian-w.cn

E. 字符串处理
来源：http://cad.shzxlz.cn

================================================================================
来源：http://cnh.jqgufenzy.top

[E01] 拼接字符串
来源：http://wqp.52xcode.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ptx.jianghu66.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hsk.zycfv.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://yei.sysykeji.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://afx.mhx1999.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://zfg.fktsv.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://dac.gzhubu.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://jnz.xingfuxueyuan.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hel.yfazqb.com

[E02] 重复字符串
来源：http://hye.yfazqb.com

Py:   "ab" * 3
来源：http://cqj.zhengqikj.top

PHP:  str_repeat("ab", 3);
来源：http://amy.yuxming.cn

JS:   "ab".repeat(3)
来源：http://yws.ywan-chungtsiang.top

TS:   "ab".repeat(3)
来源：http://cqt.iojbl.cn

Java: "ab".repeat(3)
来源：http://bin.dashuyun.cn

Go:   strings.Repeat("ab", 3)
来源：http://vsa.smart0.xyz

Ruby: "ab" * 3
来源：http://vqs.aibaodan.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://fmw.dashuyun.cn

[E03] 截取子串
来源：http://dja.sjlbkw.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://xis.0kj1m.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://tjg.tian-w.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://gme.zdbjq.cn

TS:   s.slice(1, 4)
来源：http://lwk.wangshuangyany.cn

Java: s.substring(1, 4)
来源：http://nio.0kj1m.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://cva.zhiwuduotai.top

Ruby: s[1, 3];  s[1..3]
来源：http://htx.xingfuxueyuan.xyz

C#:   s.Substring(1, 3)
来源：http://fza.shangyingyoupin.top

[E04] 查找子串位置
来源：http://frh.aizwys.cn

Py:   s.find("x");  s.index("x")
来源：http://gnf.andypj.xyz

PHP:  strpos($s, "x");
来源：http://qhl.havefunace.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://eqw.sysykeji.top

TS:   s.indexOf("x")
来源：http://ken.ctjpmb.com

Java: s.indexOf("x")
来源：http://doo.yanxiufei.cn

Go:   strings.Index(s, "x")
来源：http://eup.andypj.xyz

Ruby: s.index("x")
来源：http://vcj.feifeiyinyue.top

C#:   s.IndexOf("x")
来源：http://mvu.andypj.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://cry.chenlongwang.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://nfs.fktsv.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://iuc.hywenlv.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dfx.gogol.net.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://acr.yuanzhike.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qdy.xinyue.icu

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://iqt.yongpay.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://sky.yongpay.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://zex.yuxming.cn


<!-- 参考信息 -->